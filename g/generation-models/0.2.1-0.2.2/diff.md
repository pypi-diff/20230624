# Comparing `tmp/generation_models-0.2.1.tar.gz` & `tmp/generation_models-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generation_models-0.2.1.tar", max compression
+gzip compressed data, was "generation_models-0.2.2.tar", max compression
```

## Comparing `generation_models-0.2.1.tar` & `generation_models-0.2.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    34110 2023-05-25 19:28:19.185968 generation_models-0.2.1/generation_models.py
--rw-r--r--   0        0        0      600 2023-05-25 19:28:11.792032 generation_models-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 generation_models-0.2.1/setup.py
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 generation_models-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    36983 2023-06-23 19:36:06.072920 generation_models-0.2.2/generation_models.py
+-rw-r--r--   0        0        0      656 2023-06-23 22:21:47.589050 generation_models-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 generation_models-0.2.2/setup.py
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 generation_models-0.2.2/PKG-INFO
```

### Comparing `generation_models-0.2.1/generation_models.py` & `generation_models-0.2.2/generation_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
+
+import json
 from enum import Enum
 
-from pydantic import BaseModel, ValidationError, Field, validator, root_validator, parse_obj_as
+from pydantic import BaseModel, ValidationError, Field, validator, root_validator, parse_obj_as, conlist
 from pydantic.fields import Validator
 import typing as t
 from typing_extensions import Annotated
-from numpy import mod
 
 
-def optional_discriminators(unions: t.List[str]):
-    def dec(model: t.Type[BaseModel]):
+ModelVariable = t.TypeVar("ModelVariable", bound=t.Type[BaseModel])
+
+
+def optional_discriminators(unions: t.List[str]) -> t.Callable[[ModelVariable], ModelVariable]:
+    def dec(model: ModelVariable) -> ModelVariable:
         for k in unions:
             field = model.__fields__[k]
             discriminator_lookup = {v.type_: k for k, v in field.sub_fields_mapping.items()}
 
             def handle_missing_discriminator(cls, values):
                 if isinstance(values, dict) and field.discriminator_key not in values:
                     parsed = parse_obj_as(t.Union[tuple(f.type_ for f in field.sub_fields)], values)
@@ -148,17 +152,17 @@
             return len(v)
 
 
 class DARTPrices(BaseModel):
     """Mirrors Pandera schema used by the library, but allows for columns of different length, so that users can
     pass, e.g., 5M RTM prices and 1H DAM prices"""
 
-    rtm: t.List[float]
-    dam: t.List[float]
-    rtorpa: t.Optional[t.List[float]]
+    rtm: conlist(float, min_items=1)
+    dam: conlist(float, min_items=1)
+    rtorpa: t.Optional[conlist(float, min_items=1)]
 
     @root_validator(skip_on_failure=True)
     def check_rtorpa_len(cls, values):
         if values["rtorpa"]:
             assert len(values["rtorpa"]) == len(values["rtm"]), "RTORPA must have same lenght as RTM"
         return values
 
@@ -167,49 +171,26 @@
     rt_intervals_per_hour, err = divmod(len(sub_hourly), len(hourly))
     assert err == 0, f"length of {hourly_str} must divide length of {subhourly_str}"
     assert (
         60 / rt_intervals_per_hour == time_interval_mins
     ), f"lengths of {subhourly_str} and {hourly_str} must reflect time_interval_mins"
 
 
-class PriceScenarios(BaseModel):
-    prices: t.List[t.List[float]]
-    weights: t.List[float]
-
-    @root_validator(skip_on_failure=True)
-    def check_weight_length(cls, values):
-        assert len(values["weights"]) == len(values["prices"]), "length of weights must equal length of prices"
-        return values
-
-    @validator("prices")
-    def check_price_lengths(cls, v):
-        # assert all prices have the same lengths
-        l0 = len(v[0])
-        assert all(len(v1) == l0 for v1 in v), "all prices must have the same length"
-        return v
-
-    def __len__(self):
-        return len(self.prices[0])
-
-    @property
-    def shape(self):
-        return len(self.prices), len(self.prices[0])
-
-
 class DARTPriceScenarios(BaseModel):
-    dam: PriceScenarios
-    rtm: PriceScenarios
+    rtm: conlist(conlist(float, min_items=1), min_items=1)
+    dam: conlist(conlist(float, min_items=1), min_items=1)
+    weights: t.List[float]
 
     @root_validator(skip_on_failure=True)
-    def check_equal_lengths(cls, values):
-        assert values["dam"].shape[1] == values["rtm"].shape[1]
+    def check_lengths(cls, values):
+        assert len(values["dam"]) == len(values["rtm"]) == len(values["weights"])
         return values
 
     def __len__(self):
-        return self.dam.shape[1]
+        return len(self.rtm[0])
 
 
 class MarketBase(BaseModel):
     energy_prices: t.Union[DARTPrices, t.List[float], DARTPriceScenarios]
     reserve_markets: t.Optional[ReserveMarkets]
     time_interval_mins: t.Optional[int] = 60
     load_peak_reduction: t.Optional[LoadPeakReduction]
@@ -225,17 +206,19 @@
                 "dam prices",
             )
         return values
 
     @root_validator(skip_on_failure=True)
     def check_length(cls, values):
         if values["reserve_markets"]:
-            _check_lengths(
-                {"dam prices": values["energy_prices"].dam, "reserve market data": values["reserve_markets"]}
-            )
+            if isinstance(values["energy_prices"], DARTPriceScenarios):
+                dam_prices = values["energy_prices"].dam[0]
+            else:
+                dam_prices = values["energy_prices"].dam
+            _check_lengths({"dam prices": dam_prices, "reserve market data": values["reserve_markets"]})
 
         if values["load_peak_reduction"]:
             _check_lengths(
                 {"rtm prices": values["energy_prices"].rtm, "peak reduction data": values["load_peak_reduction"]}
             )
         return values
 
@@ -255,15 +238,14 @@
     wdir: t.List[float]
     wspd: t.List[float]
     alb: t.Optional[t.List[float]]
     snow: t.Optional[t.List[float]]
 
     @root_validator(skip_on_failure=True)
     def check_lengths(cls, values):
-        assert mod(len(next(iter(values.values()))), 8760) == 0, "solar resource time series data must represent 1 year"
         try:
             _check_lengths({k: v for k, v in values.items() if v is not None})
         except AssertionError:
             raise AssertionError("solar resource time series data must have consistent lengths")
         return values
 
     def __len__(self) -> int:
@@ -273,14 +255,28 @@
 class SolarResource(BaseModel):
     latitude: float
     longitude: float
     time_zone_offset: float
     elevation: float
     data: SolarResourceTimeSeries
     monthly_albedo: t.Optional[t.List[float]]
+    typical: bool = True
+
+    @root_validator(skip_on_failure=True)
+    def check_data_if_typical(cls, values):
+        if values["typical"]:
+            assert (
+                len(values["data"].year) % 8760 == 0
+            ), "solar resource time series data must represent 1 year when typical is true"
+            assert (values["data"].month[0], values["data"].day[0], values["data"].hour[0]) == (
+                1,
+                1,
+                0,
+            ), "solar resource data must start at Jan 1, hour 0 when typical is true"
+        return values
 
     def __len__(self) -> int:
         return len(self.data)
 
 
 class PSMRegion(str, Enum):
     NorthAmerica = "North America"
@@ -529,15 +525,15 @@
 
 
 @optional_discriminators(["tracking"])
 class PVSystemDesign(BaseSystemDesign):
     modules_per_string: t.Optional[int]
     strings_in_parallel: t.Optional[int]
     tracking: t.Union[FixedTilt, SingleAxisTracking] = Field(..., discriminator="tracking_type")
-    azimuth: float = 180.0
+    azimuth: t.Optional[float]
     gcr: float
 
 
 class TermUnits(str, Enum):
     hours = "hours"
     days = "days"
     years = "years"
@@ -568,17 +564,18 @@
     """
     For more on why we treat project_term as an int and validate like we do check out this PR comment:
     https://github.com/Tyba-Energy/generation/pull/186#discussion_r1054578658. The broader PR has even more context
     should it be needed
     """
     signal_hours = int(signal_len * (time_interval_mins / 60))
     project_term_hours = scale_project_term_to_hours(project_term, project_term_units)
-    assert (
-        project_term_hours == signal_hours
-    ), f"project_term, project_term_units, time_interval_mins, and length of {signal_str} must be consistent"
+    assert project_term_hours == signal_hours, (
+        f"project_term, project_term_units, time_interval_mins, and length of {signal_str} must be consistent; "
+        f"got {project_term}, {project_term_units}, {time_interval_mins}, and {signal_len} respectively"
+    )
 
 
 class ExternalGenerationModel(BaseGenerationModel):
     losses: t.Union[ACLosses, Losses]
     production_override: ProductionProfile
     system_design: BaseSystemDesign
 
@@ -630,50 +627,81 @@
 
 
 class ArrayDegradationMode(str, Enum):
     linear = "linear"
     compounding = "compounding"
 
 
-def _pv_gen_len(sol_res, pt):
-    if isinstance(sol_res, SolarResource):
-        return len(sol_res) * pt
-    else:
-        return 8760 * pt
+def _solar_resource_is_typical(solar_resource) -> bool:
+    if isinstance(solar_resource, SolarResource) and not solar_resource.typical:
+        return False
+    return True
+
+
+def _pv_gen_len(solar_resource, project_term) -> int:
+    if isinstance(solar_resource, SolarResource):
+        if _solar_resource_is_typical(solar_resource):
+            return len(solar_resource) * project_term
+        return len(solar_resource)
+    return 8760 * project_term
 
 
 class PVGenerationModel(BaseGenerationModel):
     generation_type: t.Optional[t.Literal["PV"]] = "PV"
     solar_resource: t.Union[SolarResource, t.Tuple[float, float], SolarResourceLocation]
     inverter: InverterTypes
     pv_module: PVModuleTypes
     layout: Layout = Layout()
     losses: Losses = Losses()
     system_design: PVSystemDesign
     array_degradation_rate: float = 0.005
-    array_degradation_mode: ArrayDegradationMode = ArrayDegradationMode.linear
+    array_degradation_mode: t.Optional[ArrayDegradationMode] = ArrayDegradationMode.linear
 
     def __len__(self) -> int:
         return _pv_gen_len(self.solar_resource, self.project_term)
 
     @root_validator(skip_on_failure=True)
+    def check_project_term_units(cls, values):
+        if _solar_resource_is_typical(values["solar_resource"]):
+            assert (
+                values["project_term_units"] == "years"
+            ), "project_term_units of 'years' required when typical year is being modeled"
+        return values
+
+    @root_validator(skip_on_failure=True)
     def check_time_interval_project_term(cls, values):
         _check_time_interval_project_term(
             _pv_gen_len(values["solar_resource"], values["project_term"]),
             "solar_resource",
             values["project_term"],
             values["time_interval_mins"],
             values["project_term_units"],
         )
         return values
 
-    @validator("project_term_units")
-    def check_project_term_units(cls, v):
-        assert v == "years", "Currently only project_term_units of 'years' is supported for PVGenerationModel objects"
-        return v
+    @root_validator(skip_on_failure=True)
+    def check_degradation_mode_for_nontypical(cls, values):
+        if not _solar_resource_is_typical(values["solar_resource"]):
+            assert (
+                values["array_degradation_mode"] is None
+            ), "PV array degradation not currently supported for non-typical year simulations"
+        return values
+
+    @root_validator(skip_on_failure=True)
+    def default_azimuth_from_location(cls, values):
+        system_design: PVSystemDesign = values["system_design"]
+        solar_resource = values["solar_resource"]
+        if system_design.azimuth is None:
+            if isinstance(solar_resource, tuple):
+                system_design.azimuth = 180.0 if solar_resource[0] >= 0.0 else 0.0
+            elif isinstance(solar_resource, (SolarResource, SolarResourceLocation)):
+                system_design.azimuth = 180.0 if solar_resource.latitude >= 0.0 else 0.0
+            else:
+                raise NotImplementedError("No default azimuth handling for this solar resource model")
+        return values
 
 
 GenerationModel = Annotated[
     t.Union[PVGenerationModel, DCExternalGenerationModel, ACExternalGenerationModel],
     Field(discriminator="generation_type"),
 ]
 
@@ -731,45 +759,78 @@
 
 
 class EnergyStrategy(str, Enum):
     da = "DA"
     rt = "RT"
     dart = "DART"
 
+    def to_market_config(self) -> MarketConfig:
+        return {
+            "DA": MarketConfig(da=BidOfferStrategy.quantity_only, rt=None),
+            "RT": MarketConfig(da=None, rt=BidOfferStrategy.quantity_only),
+            "DART": MarketConfig(da=BidOfferStrategy.quantity_only, rt=BidOfferStrategy.quantity_only),
+        }[self]
+
+
+class BidOfferStrategy(str, Enum):
+    quantity_only = "quantity-only"
+    price_quantity = "price-quantity"
+
+
+class MarketConfig(BaseModel):
+    da: t.Optional[BidOfferStrategy]
+    rt: t.Optional[BidOfferStrategy]
+
+    @validator("rt")
+    def valid_rt_configs(cls, v):
+        if v == "price-quantity":
+            raise ValueError("rt price-quantity not yet implemented")
+        return v
+
+    @property
+    def independent_dam(self) -> bool:
+        return self.da is not None and self.rt is not None
+
+    @property
+    def value(self) -> str:
+        """For symmetry with EnergyStrategy"""
+        return json.dumps({"DAM": self.da.value, "RTM": self.rt.value})
+
+
+class Solver(str, Enum):
+    HiGHS = "HiGHS"
+    GLPK = "GLPK"
+    HiGHS_GLPK = "HiGHS-GLPK"
+    GLPK_HiGHS = "GLPK-HiGHS"
+
 
 class StorageSolverOptions(BaseModel):
     cycling_cost_adder: float = 0.0
     annual_cycle_limit: float = None
     disable_intra_interval_variation: bool = False
     window: int = None
     step: int = None
     flexible_solar: bool = False
     symmetric_reg: bool = False
-    energy_strategy: t.Optional[EnergyStrategy]
+    energy_strategy: t.Optional[t.Union[EnergyStrategy, MarketConfig]]
     dart: t.Optional[bool]
     uncertain_soe: bool = True
     dam_annual_cycle_limit: float = None
     no_virtual_trades: bool = False
     initial_soe: float = 0.0
     duration_requirement_on_discharge: bool = True  # True for ERCOT
-    solver: t.Optional[str] = None
+    solver: t.Optional[Solver] = None
     solver_config: SolverConfig = SolverConfig()
 
     @root_validator(skip_on_failure=True)
     def check_dam_annual_cycle_limit(cls, values):
         if values["dam_annual_cycle_limit"] is not None and not (values["dart"] or values["energy_strategy"] == "DART"):
             raise AssertionError("dart must be `true` if dam_annual_cycle_limit is set")
         return values
 
-    @validator("solver")
-    def check_solver_name(cls, v):
-        valid_solvers = ["HiGHS", "GLPK", "HiGHS-GLPK", None]
-        assert v in valid_solvers, f"solver must be one of {valid_solvers}"
-        return v
-
     @root_validator(skip_on_failure=True)
     def check_solver_config(cls, values):
         if values["solver_config"].solver_specific and (values["solver"] not in {"HiGHS", "GLPK"}):
             raise ValueError("solver_specific options may only be passed when using HiGHS or GLPK solver")
         return values
 
     @root_validator(skip_on_failure=True)
@@ -792,17 +853,20 @@
         if len(v) > 1:  # don't worry about terms if there's only one battery
             for battery in v:
                 assert battery.term, "if multiple batteries are provided, terms must also be provided"
         return v
 
 
 def _get_price_str_and_price(values):
-    if isinstance(values["energy_prices"], (DARTPrices, DARTPriceScenarios)):
+    if isinstance(values["energy_prices"], DARTPrices):
         return "rtm prices", values["energy_prices"].rtm
-    return "energy_prices", values["energy_prices"]
+    elif isinstance(values["energy_prices"], DARTPriceScenarios):
+        return "rtm price", values["energy_prices"]
+    else:
+        return "energy_prices", values["energy_prices"]
 
 
 class PeakWindow(BaseModel):
     mask: t.List[bool]
     price: float
```

### Comparing `generation_models-0.2.1/pyproject.toml` & `generation_models-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [tool.poetry]
 name = "generation-models"
-version = "0.2.1"
+version = "0.2.2"
 description = "generation API data model"
 authors = ["battery_al <allenlawrence94@gmail.com>"]
 packages = [{include = "generation_models.py"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.5.1"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+
 
 [tool.black]
 line-length = 120
 preview = true
 
 [tool.ruff]
 line-length = 120
```

### Comparing `generation_models-0.2.1/setup.py` & `generation_models-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 modules = \
 ['generation_models']
 install_requires = \
 ['pydantic>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'generation-models',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'generation API data model',
     'long_description': 'None',
     'author': 'battery_al',
     'author_email': 'allenlawrence94@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

