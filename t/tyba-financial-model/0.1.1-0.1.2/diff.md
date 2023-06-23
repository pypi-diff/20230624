# Comparing `tmp/tyba_financial_model-0.1.1.tar.gz` & `tmp/tyba_financial_model-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyba_financial_model-0.1.1.tar", max compression
+gzip compressed data, was "tyba_financial_model-0.1.2.tar", max compression
```

## Comparing `tyba_financial_model-0.1.1.tar` & `tyba_financial_model-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     7058 2023-06-23 20:51:16.379145 tyba_financial_model-0.1.1/project_finance/__init__.py
--rw-r--r--   0        0        0     7747 2023-02-09 21:50:53.599614 tyba_financial_model-0.1.1/project_finance/finance.py
--rw-r--r--   0        0        0      415 2023-06-23 20:52:21.720510 tyba_financial_model-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 tyba_financial_model-0.1.1/setup.py
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 tyba_financial_model-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7059 2023-06-23 22:47:41.908660 tyba_financial_model-0.1.2/project_finance/__init__.py
+-rw-r--r--   0        0        0     7747 2023-02-09 21:50:53.599614 tyba_financial_model-0.1.2/project_finance/finance.py
+-rw-r--r--   0        0        0      415 2023-06-23 22:47:41.909721 tyba_financial_model-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 tyba_financial_model-0.1.2/setup.py
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 tyba_financial_model-0.1.2/PKG-INFO
```

### Comparing `tyba_financial_model-0.1.1/project_finance/__init__.py` & `tyba_financial_model-0.1.2/project_finance/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,23 @@
     :param opex: series of operating expenses for each period, in $
     :param revenue: series of revenue generated for each period in $
     :return: series of cash_flow values
 
     - Positive sign assumed for all arguments
     - Cashflows are assumed to occur at the end of the period, i.e. the capital expenditures are assumed to occur at the
     end of period "0", and revenue and operating expenses first hit the project account at the end of year 1, etc.
+
     :meta private:
     """
 
     return np.array([-capex] + (revenue - opex).tolist())
 
 
 class BaseFinanceInputs(BaseModel):
-    """ """
+    """_"""
 
     frequency: str
 
     class Config:
         arbitrary_types_allowed = True
 
     @validator("frequency")
@@ -40,71 +41,71 @@
         return v
 
     def get_cash_flow(self) -> np.ndarray:
         return cash_flow(capex=self.capex, opex=self.opex, revenue=self.revenue)
 
 
 class SolarInputs(BaseModel):
-    """ """
+    """_"""
 
     array_capacity_wdc: float
     capex_cost_per_wdc: float = 0.80
     opex_cost_per_wdc: float = 0.01
 
     @property
     def capex(self):
         return self.array_capacity_wdc * self.capex_cost_per_wdc
 
     def _opex_per_period(self, periods_per_year):
         return self.array_capacity_wdc * self.opex_cost_per_wdc / periods_per_year
 
 
 class SolarFinanceInputs(BaseFinanceInputs, SolarInputs):
-    """ """
+    """_"""
 
     revenue: np.ndarray
 
     @property
     def opex(self):
         return np.array(
             [self._opex_per_period(valid_frequencies[self.frequency])]
             * len(self.revenue)
         )
 
 
 class StorageInputs(BaseModel):
-    """ """
+    """_"""
 
     capacity_kwh: float
     capex_cost_per_kwh: float = 200.00
     opex_cost_per_kwh: float = 7.00
 
     @property
     def capex(self):
         return self.capacity_kwh * self.capex_cost_per_kwh
 
     def _opex_per_period(self, periods_per_year):
         return self.capacity_kwh * self.opex_cost_per_kwh / periods_per_year
 
 
 class StorageFinanceInputs(BaseFinanceInputs, StorageInputs):
-    """ """
+    """_"""
 
     revenue: np.ndarray
 
     @property
     def opex(self):
         return np.array(
             [self._opex_per_period(valid_frequencies[self.frequency])]
             * len(self.revenue)
         )
 
 
 class HybridFinanceInputsSingleRev(BaseFinanceInputs):
-    """ """
+    """_"""
 
     revenue: np.ndarray
     solar: SolarInputs
     storage: StorageInputs
 
     @property
     def capex(self):
@@ -118,15 +119,15 @@
                 + self.storage._opex_per_period(valid_frequencies[self.frequency])
             ]
             * len(self.revenue)
         )
 
 
 class HybridFinanceInputs(BaseModel):
-    """ """
+    """_"""
 
     solar: SolarFinanceInputs
     storage: StorageFinanceInputs
 
     @root_validator(skip_on_failure=True)
     def check_revs_and_freqs(cls, values):
         try:
@@ -172,15 +173,15 @@
     return finance.npv(
         rate=annual_discount_rate / valid_frequencies[inputs.frequency],
         values=inputs.get_cash_flow(),
     )
 
 
 class HybridDetailResults(BaseModel):
-    """ """
+    """_"""
 
     solar: float
     storage: float
     project: float
 
 
 def hybrid_detailed_npv(
```

### Comparing `tyba_financial_model-0.1.1/project_finance/finance.py` & `tyba_financial_model-0.1.2/project_finance/finance.py`

 * *Files identical despite different names*

### Comparing `tyba_financial_model-0.1.1/setup.py` & `tyba_financial_model-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.24.1,<2.0.0', 'pydantic>=1.10.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'tyba-financial-model',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': 'None',
     'author': 'Casey Zak',
     'author_email': 'czak24@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

