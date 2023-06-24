# Comparing `tmp/generation_models-0.2.2.tar.gz` & `tmp/generation_models-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generation_models-0.2.2.tar", max compression
+gzip compressed data, was "generation_models-0.2.3.tar", max compression
```

## Comparing `generation_models-0.2.2.tar` & `generation_models-0.2.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    36983 2023-06-23 19:36:06.072920 generation_models-0.2.2/generation_models.py
--rw-r--r--   0        0        0      656 2023-06-23 22:21:47.589050 generation_models-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 generation_models-0.2.2/setup.py
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 generation_models-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    37936 2023-06-24 00:20:25.625866 generation_models-0.2.3/generation_models.py
+-rw-r--r--   0        0        0      656 2023-06-24 00:20:25.628234 generation_models-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 generation_models-0.2.3/setup.py
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 generation_models-0.2.3/PKG-INFO
```

### Comparing `generation_models-0.2.2/generation_models.py` & `generation_models-0.2.3/generation_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
             field.populate_validators()
         return model
 
     return dec
 
 
 class SolverConfig(BaseModel):
+    """_"""
+
     initial_time_limit: float = 8.0
     secondary_time_limit: float = 8.0  # not used
     initial_mip_gap_tolerance: float = 0.0
     secondary_mip_gap_tolerance: float = 0.02  # not used
     initial_verbose: bool = False
     secondary_verbose: bool = True  # not used
     hybrid_infeasible_tol: float = 0
@@ -57,25 +59,31 @@
 class StorageCoupling(str, Enum):
     ac = "ac"
     dc = "dc"
     hv_ac = "hv_ac"
 
 
 class SingleAxisTracking(BaseModel):
+    """_"""
+
     tracking_type: t.Optional[t.Literal["SAT"]] = "SAT"
     rotation_limit: float = 45.0
     backtrack: bool = True
 
 
 class FixedTilt(BaseModel):
+    """_"""
+
     tracking_type: t.Optional[t.Literal["FT"]] = "FT"
     tilt: float
 
 
 class ScalarUtilization(BaseModel):
+    """_"""
+
     dimension_type: t.Optional[t.Literal["scalar"]] = "scalar"
     actual: float
     lower: float
     upper: float
 
     @root_validator(skip_on_failure=True)
     def between_0_and_1(cls, values):
@@ -88,14 +96,16 @@
     str1 = next(iter(strs_lists.keys()))
     len1 = len(next(iter(strs_lists.values())))
     for k, v in strs_lists.items():
         assert len(v) == len1, f"{str1} and {k} must be the same length"
 
 
 class TimeSeriesUtilization(BaseModel):
+    """_"""
+
     dimension_type: t.Optional[t.Literal["time_series"]] = "time_series"
     actual: t.List[float]
     lower: t.List[float]
     upper: t.List[float]
 
     @root_validator(skip_on_failure=True)
     def between_0_and_1(cls, values):
@@ -110,14 +120,16 @@
 
     def __len__(self) -> int:
         return len(self.actual)
 
 
 @optional_discriminators(["utilization"])
 class ReserveMarket(BaseModel):
+    """_"""
+
     price: t.List[float]
     offer_cap: float
     utilization: t.Union[ScalarUtilization, TimeSeriesUtilization] = Field(..., discriminator="dimension_type")
     duration_requirement: float = Field(0.0, description="market requirement for offer duration (hours)")
     obligation: t.Optional[t.List[float]]
 
     @root_validator(skip_on_failure=True)
@@ -129,14 +141,16 @@
         return values
 
     def __len__(self) -> int:
         return len(self.price)
 
 
 class ReserveMarkets(BaseModel):
+    """_"""
+
     up: t.Optional[t.Dict[str, ReserveMarket]]
     down: t.Optional[t.Dict[str, ReserveMarket]]
 
     @root_validator(skip_on_failure=True)
     def check_length(cls, values):
         length = None
         for attrib in "up", "down":
@@ -172,28 +186,32 @@
     assert err == 0, f"length of {hourly_str} must divide length of {subhourly_str}"
     assert (
         60 / rt_intervals_per_hour == time_interval_mins
     ), f"lengths of {subhourly_str} and {hourly_str} must reflect time_interval_mins"
 
 
 class DARTPriceScenarios(BaseModel):
+    """_"""
+
     rtm: conlist(conlist(float, min_items=1), min_items=1)
     dam: conlist(conlist(float, min_items=1), min_items=1)
     weights: t.List[float]
 
     @root_validator(skip_on_failure=True)
     def check_lengths(cls, values):
         assert len(values["dam"]) == len(values["rtm"]) == len(values["weights"])
         return values
 
     def __len__(self):
         return len(self.rtm[0])
 
 
 class MarketBase(BaseModel):
+    """_"""
+
     energy_prices: t.Union[DARTPrices, t.List[float], DARTPriceScenarios]
     reserve_markets: t.Optional[ReserveMarkets]
     time_interval_mins: t.Optional[int] = 60
     load_peak_reduction: t.Optional[LoadPeakReduction]
 
     @root_validator(skip_on_failure=True)
     def check_time_interval(cls, values):
@@ -220,14 +238,16 @@
             _check_lengths(
                 {"rtm prices": values["energy_prices"].rtm, "peak reduction data": values["load_peak_reduction"]}
             )
         return values
 
 
 class SolarResourceTimeSeries(BaseModel):
+    """_"""
+
     year: t.List[int]
     month: t.List[int]
     day: t.List[int]
     hour: t.List[int]
     minute: t.List[int]
     tdew: t.List[float]
     df: t.List[float]
@@ -249,14 +269,16 @@
         return values
 
     def __len__(self) -> int:
         return len(self.year)
 
 
 class SolarResource(BaseModel):
+    """_"""
+
     latitude: float
     longitude: float
     time_zone_offset: float
     elevation: float
     data: SolarResourceTimeSeries
     monthly_albedo: t.Optional[t.List[float]]
     typical: bool = True
@@ -275,32 +297,40 @@
         return values
 
     def __len__(self) -> int:
         return len(self.data)
 
 
 class PSMRegion(str, Enum):
+    """_"""
+
     NorthAmerica = "North America"
     AsiaPacific = "Asia/Pacific"
 
 
 class SolarResourceLocation(BaseModel):
+    """_"""
+
     latitude: float
     longitude: float
     region: PSMRegion = PSMRegion.NorthAmerica
 
     class Config:
         extra = "forbid"
 
 
 class FileComponent(BaseModel):
+    """_"""
+
     path: str
 
 
 class PVModuleCEC(BaseModel):
+    """_"""
+
     bifacial: bool
     a_c: float
     n_s: float
     i_sc_ref: float
     v_oc_ref: float
     i_mp_ref: float
     v_mp_ref: float
@@ -316,22 +346,26 @@
     gamma_r: float
     bifacial_transmission_factor: float
     bifaciality: float
     bifacial_ground_clearance_height: float
 
 
 class MermoudModuleTech(str, Enum):
+    """_"""
+
     SiMono = "mtSiMono"
     SiPoly = "mtSiPoly"
     CdTe = "mtCdTe"
     CIS = "mtCIS"
     uCSi_aSiH = "mtuCSi_aSiH"
 
 
 class PVModuleMermoudLejeune(BaseModel):
+    """_"""
+
     bifacial: bool
     bifacial_transmission_factor: float
     bifaciality: float
     bifacial_ground_clearance_height: float
     tech: MermoudModuleTech
     iam_c_cs_iam_value: t.Optional[t.List[float]]
     iam_c_cs_inc_angle: t.Optional[t.List[float]]
@@ -355,44 +389,54 @@
     beta_oc: float
     mu_n: float
     n_0: float
     custom_d2_mu_tau: t.Optional[float]
 
 
 class BaseInverter(BaseModel):
+    """_"""
+
     mppt_low: float
     mppt_high: float
     paco: float
     vdco: float
     pnt: float
     includes_xfmr: bool = False
 
 
 class Inverter(BaseInverter):
+    """_"""
+
     pso: float
     pdco: float
     c0: float
     c1: float
     c2: float
     c3: float
     vdcmax: float
     tdc: t.List[t.List[float]] = Field(default_factory=lambda: [[1.0, 52.8, -0.021]])
 
 
 class ONDTemperatureDerateCurve(BaseModel):
+    """_"""
+
     ambient_temp: t.List[float]
     max_ac_power: t.List[float]
 
 
 class ONDEfficiencyCurve(BaseModel):
+    """_"""
+
     dc_power: t.List[float]
     ac_power: t.List[float]
 
 
 class ONDInverter(BaseInverter):
+    """_"""
+
     temp_derate_curve: ONDTemperatureDerateCurve
     nominal_voltages: t.List[float]
     power_curves: t.List[ONDEfficiencyCurve]
     dc_turn_on: float
     aux_loss: t.Optional[float]
     aux_loss_threshold: t.Optional[float]
 
@@ -411,33 +455,39 @@
 
 
 InverterTypes = t.Union[Inverter, ONDInverter, str, FileComponent]
 PVModuleTypes = t.Union[PVModuleCEC, PVModuleMermoudLejeune, str, FileComponent]
 
 
 class Layout(BaseModel):
+    """_"""
+
     orientation: t.Optional[str]
     vertical: t.Optional[int]
     horizontal: t.Optional[int]
     aspect_ratio: t.Optional[float]
 
     @root_validator(skip_on_failure=True)
     def all_or_none(cls, values):
         missing = [v is None for k, v in values.items()]
         assert all(missing) or not any(missing), "Either all or no attributes must be assigned in Layout"
         return values
 
 
 class Transformer(BaseModel):
+    """_"""
+
     rating: t.Optional[float]
     load_loss: float
     no_load_loss: float
 
 
 class ACLosses(BaseModel):
+    """_"""
+
     ac_wiring: float = 0.01
     transmission: float = 0.0
     # Feeds into nrel_sam.AdjustmentFactors rather than nrel_sam.Losses
     poi_adjustment: float = 0.0  # TODO: deprecate this?
     transformer_load: t.Optional[float]  # deprecate
     transformer_no_load: t.Optional[float]  # deprecate
     hv_transformer: t.Optional[Transformer]
@@ -448,14 +498,16 @@
         assert (values["transformer_load"] is None and values["transformer_no_load"] is None) or values[
             "hv_transformer"
         ] is None, "Cannot provide hv_transformer if transformer_load or transformer_no_load are provided"
         return values
 
 
 class DCLosses(BaseModel):
+    """_"""
+
     dc_optimizer: float = 0.0
     enable_snow_model: bool = False
     dc_wiring: float = 0.02
     soiling: t.List[float] = Field(default_factory=lambda: 12 * [0.0])
     diodes_connections: float = 0.005
     mismatch: float = 0.01
     nameplate: float = 0.0
@@ -472,19 +524,23 @@
         assert (
             values["mppt_error"] * values["tracking_error"] == 0.0
         ), "Only one of mppt_error and tracking_error may be nonzero"
         return values
 
 
 class Losses(ACLosses, DCLosses):
+    """_"""
+
     class Config:
         extra = "forbid"
 
 
 class DCProductionProfile(BaseModel):
+    """_"""
+
     power: t.List[float]
     voltage: t.List[float]
     ambient_temp: t.Optional[t.List[float]]
 
     @root_validator(skip_on_failure=True)
     def check_length(cls, values):
         _check_lengths({"power": values["power"], "voltage": values["voltage"]})
@@ -493,14 +549,16 @@
         return values
 
     def __len__(self) -> int:
         return len(self.power)
 
 
 class ACProductionProfile(BaseModel):
+    """_"""
+
     power: t.List[float]
     ambient_temp: t.Optional[t.List[float]]
 
     # if ACProductionProfile is allowed to have extra fields in the payload, then a DCProductionProfile payload will be
     # coerced into an ACProductionProfile object if something is wrong with voltage
     class Config:
         extra = "forbid"
@@ -515,40 +573,50 @@
         return len(self.power)
 
 
 ProductionProfile = t.Union[DCProductionProfile, ACProductionProfile]
 
 
 class BaseSystemDesign(BaseModel):
+    """_"""
+
     dc_capacity: float
     ac_capacity: float
     poi_limit: float
 
 
 @optional_discriminators(["tracking"])
 class PVSystemDesign(BaseSystemDesign):
+    """_"""
+
     modules_per_string: t.Optional[int]
     strings_in_parallel: t.Optional[int]
     tracking: t.Union[FixedTilt, SingleAxisTracking] = Field(..., discriminator="tracking_type")
     azimuth: t.Optional[float]
     gcr: float
 
 
 class TermUnits(str, Enum):
+    """_"""
+
     hours = "hours"
     days = "days"
     years = "years"
 
 
 class ProjectTermMixin(BaseModel):
+    """_"""
+
     project_term: int = 1
     project_term_units: TermUnits = "years"
 
 
 class BaseGenerationModel(ProjectTermMixin):
+    """_"""
+
     project_type: t.Optional[t.Literal["generation"]] = "generation"
     time_interval_mins: int = 60
 
 
 def scale_project_term_to_hours(project_term: int, project_term_units: TermUnits) -> int:
     if project_term_units == "hours":
         return project_term
@@ -571,14 +639,16 @@
     assert project_term_hours == signal_hours, (
         f"project_term, project_term_units, time_interval_mins, and length of {signal_str} must be consistent; "
         f"got {project_term}, {project_term_units}, {time_interval_mins}, and {signal_len} respectively"
     )
 
 
 class ExternalGenerationModel(BaseGenerationModel):
+    """_"""
+
     losses: t.Union[ACLosses, Losses]
     production_override: ProductionProfile
     system_design: BaseSystemDesign
 
     @root_validator(skip_on_failure=True)
     def check_time_interval_project_term(cls, values):
         _check_time_interval_project_term(
@@ -597,40 +667,48 @@
 class Bus(str, Enum):
     DC = "DC"
     MV = "MV"
     HV = "HV"
 
 
 class DownstreamSystem(BaseModel):
+    """_"""
+
     losses: ACLosses  # still only ACLosses if modeling from inverter input, since almost every DC loss pertains to PV.
     system_design: BaseSystemDesign
     model_losses_from: Bus
     inverter: t.Optional[InverterTypes]
 
     @root_validator(skip_on_failure=True)
     def inverter_only_if_dc(cls, values):
         if values["inverter"] is not None:
             assert values["model_losses_from"] == Bus.DC, "model_losses_from must be 'DC' if inverter is provided"
         return values
 
 
 class ACExternalGenerationModel(ExternalGenerationModel):
+    """_"""
+
     generation_type: t.Optional[t.Literal["ExternalAC"]] = "ExternalAC"
     losses: ACLosses = ACLosses()
     production_override: ACProductionProfile
 
 
 class DCExternalGenerationModel(ExternalGenerationModel):
+    """_"""
+
     generation_type: t.Optional[t.Literal["ExternalDC"]] = "ExternalDC"
     losses: Losses = Losses()
     production_override: DCProductionProfile
     inverter: InverterTypes
 
 
 class ArrayDegradationMode(str, Enum):
+    """_"""
+
     linear = "linear"
     compounding = "compounding"
 
 
 def _solar_resource_is_typical(solar_resource) -> bool:
     if isinstance(solar_resource, SolarResource) and not solar_resource.typical:
         return False
@@ -642,14 +720,16 @@
         if _solar_resource_is_typical(solar_resource):
             return len(solar_resource) * project_term
         return len(solar_resource)
     return 8760 * project_term
 
 
 class PVGenerationModel(BaseGenerationModel):
+    """_"""
+
     generation_type: t.Optional[t.Literal["PV"]] = "PV"
     solar_resource: t.Union[SolarResource, t.Tuple[float, float], SolarResourceLocation]
     inverter: InverterTypes
     pv_module: PVModuleTypes
     layout: Layout = Layout()
     losses: Losses = Losses()
     system_design: PVSystemDesign
@@ -703,33 +783,41 @@
 GenerationModel = Annotated[
     t.Union[PVGenerationModel, DCExternalGenerationModel, ACExternalGenerationModel],
     Field(discriminator="generation_type"),
 ]
 
 
 class TableCapDegradationModel(BaseModel):
+    """_"""
+
     annual_capacity_derates: t.List[float]
 
 
 class TableEffDegradationModel(BaseModel):
+    """_"""
+
     annual_efficiency_derates: t.List[float]
 
 
 class BatteryHVACParams(BaseModel):
+    """_"""
+
     container_temperature: float
     cop: float
     u_ambient: float
     discharge_efficiency_container: float
     charge_efficiency_container: float
     aux_xfmr_efficiency: float
     container_surface_area: float = 20.0
     design_energy_per_container: float = 750.0
 
 
 class BatteryParams(BaseModel):
+    """_"""
+
     power_capacity: float
     energy_capacity: float
     charge_efficiency: float
     discharge_efficiency: float
     degradation_rate: t.Optional[float]
     degradation_annual_cycles: float = 261  # cycle / work day
     hvac: t.Optional[BatteryHVACParams]
@@ -773,14 +861,16 @@
 
 class BidOfferStrategy(str, Enum):
     quantity_only = "quantity-only"
     price_quantity = "price-quantity"
 
 
 class MarketConfig(BaseModel):
+    """_"""
+
     da: t.Optional[BidOfferStrategy]
     rt: t.Optional[BidOfferStrategy]
 
     @validator("rt")
     def valid_rt_configs(cls, v):
         if v == "price-quantity":
             raise ValueError("rt price-quantity not yet implemented")
@@ -800,14 +890,16 @@
     HiGHS = "HiGHS"
     GLPK = "GLPK"
     HiGHS_GLPK = "HiGHS-GLPK"
     GLPK_HiGHS = "GLPK-HiGHS"
 
 
 class StorageSolverOptions(BaseModel):
+    """_"""
+
     cycling_cost_adder: float = 0.0
     annual_cycle_limit: float = None
     disable_intra_interval_variation: bool = False
     window: int = None
     step: int = None
     flexible_solar: bool = False
     symmetric_reg: bool = False
@@ -842,14 +934,16 @@
         if values["energy_strategy"] is None:
             values["energy_strategy"] = EnergyStrategy.dart if values["dart"] else EnergyStrategy.da
             values["dart"] = None
         return values
 
 
 class MultiStorageInputs(StorageSolverOptions):
+    """_"""
+
     batteries: t.List[BatteryParams]
 
     @validator("batteries")
     def check_battery_terms(cls, v):
         if len(v) > 1:  # don't worry about terms if there's only one battery
             for battery in v:
                 assert battery.term, "if multiple batteries are provided, terms must also be provided"
@@ -862,19 +956,23 @@
     elif isinstance(values["energy_prices"], DARTPriceScenarios):
         return "rtm price", values["energy_prices"]
     else:
         return "energy_prices", values["energy_prices"]
 
 
 class PeakWindow(BaseModel):
+    """_"""
+
     mask: t.List[bool]
     price: float
 
 
 class LoadPeakReduction(BaseModel):
+    """_"""
+
     load: t.List[float]
     max_load: t.List[float]  # TODO: should be optional -- https://app.asana.com/0/1178990154879730/1203603348130562/f
     seasonal_peak_windows: t.List[PeakWindow] = []
     daily_peak_windows: t.List[PeakWindow] = []
 
     @root_validator(skip_on_failure=True)
     def check_lengths(cls, values):
@@ -889,14 +987,16 @@
         return values
 
     def __len__(self) -> int:
         return len(self.load)
 
 
 class ImportExportLimitMixin(BaseModel):
+    """_"""
+
     import_limit: t.Optional[t.List[float]]
     export_limit: t.Optional[t.List[float]]
 
     @root_validator(skip_on_failure=True)
     def validate_limits(cls, values):
         if values["import_limit"] is not None:
             assert all([v <= 0 for v in values["import_limit"]]), "import_limit must be <= 0"
@@ -940,14 +1040,16 @@
         ), "when storage_inputs.symmetric_reg is True, both reg_up and reg_down reg markets must be provided"
 
     return values
 
 
 @optional_discriminators(["pv_inputs"])
 class PVStorageModel(ImportExportLimitMixin, MarketBase):
+    """_"""
+
     project_type: t.Optional[t.Literal["hybrid"]] = "hybrid"
     storage_inputs: MultiStorageInputs
     storage_coupling: StorageCoupling
     pv_inputs: GenerationModel
     enable_grid_charge_year: t.Optional[float]
 
     @property
@@ -958,22 +1060,28 @@
     @property
     def project_term_units(self) -> TermUnits:
         return self.pv_inputs.project_term_units
 
     @root_validator(skip_on_failure=True)
     def check_time_intervals(cls, values):
         assert (
-            values["time_interval_mins"] == values["pv_inputs"].time_interval_mins
-        ), "pv and price time_interval_mins must be equal"
+            values["time_interval_mins"] <= values["pv_inputs"].time_interval_mins
+        ), "price time_interval_mins must less than or equal to pv time_interval_mins"
         return values
 
     @root_validator(skip_on_failure=True)
-    def check_pv_length(cls, values):
+    def check_price_time_interval_against_pv_project_term(cls, values):
         price_str, price = _get_price_str_and_price(values)
-        _check_lengths({price_str: price, "pv_inputs": values["pv_inputs"]})
+        _check_time_interval_project_term(
+            len(price),
+            price_str,
+            values["pv_inputs"].project_term,
+            values["time_interval_mins"],
+            values["pv_inputs"].project_term_units,
+        )
         return values
 
     @root_validator(skip_on_failure=True)
     def check_battery_terms(cls, values):
         if len(values["storage_inputs"].batteries) > 1:
             total_batt_yrs = sum(bat.term for bat in values["storage_inputs"].batteries)
             assert (
@@ -988,14 +1096,16 @@
 
     @root_validator(skip_on_failure=True)
     def check_sym_reg_inputs(cls, values):
         return _check_symmetric_reg_inputs(values)
 
 
 class StandaloneStorageModel(ProjectTermMixin, ImportExportLimitMixin, MarketBase):
+    """_"""
+
     project_type: t.Optional[t.Literal["storage"]] = "storage"
     storage_inputs: MultiStorageInputs
     downstream_system: t.Optional[DownstreamSystem]
     ambient_temp: t.Optional[t.List[float]]
 
     @root_validator(skip_on_failure=True)
     def check_ambient_temp_length(cls, values):
@@ -1060,26 +1170,34 @@
 JobModel = Annotated[
     t.Union[StandaloneStorageModel, PVStorageModel, GenerationModel], Field(discriminator="project_type")
 ]
 
 
 @optional_discriminators(["model"])
 class AsyncModelBase(BaseModel):
+    """_"""
+
     id: str
     model: JobModel
     results_path: t.Optional[str]
 
 
 @optional_discriminators(["model"])
 class AsyncPVModel(AsyncModelBase):
+    """_"""
+
     id: str
     model: GenerationModel
 
 
 class AsyncPVStorageModel(AsyncModelBase):
+    """_"""
+
     id: str
     model: PVStorageModel
 
 
 class AsyncStandaloneStorageModel(AsyncModelBase):
+    """_"""
+
     id: str
     model: StandaloneStorageModel
```

### Comparing `generation_models-0.2.2/pyproject.toml` & `generation_models-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "generation-models"
-version = "0.2.2"
+version = "0.2.3"
 description = "generation API data model"
 authors = ["battery_al <allenlawrence94@gmail.com>"]
 packages = [{include = "generation_models.py"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.5.1"
```

### Comparing `generation_models-0.2.2/setup.py` & `generation_models-0.2.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 modules = \
 ['generation_models']
 install_requires = \
 ['pydantic>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'generation-models',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'generation API data model',
     'long_description': 'None',
     'author': 'battery_al',
     'author_email': 'allenlawrence94@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

