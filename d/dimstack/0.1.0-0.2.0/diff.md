# Comparing `tmp/dimstack-0.1.0.tar.gz` & `tmp/dimstack-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimstack-0.1.0.tar", last modified: Wed May  3 23:44:37 2023, max compression
+gzip compressed data, was "dimstack-0.2.0.tar", last modified: Sat Jun 24 02:29:11 2023, max compression
```

## Comparing `dimstack-0.1.0.tar` & `dimstack-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      858 2023-05-01 02:46:24.847886 dimstack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7164 2023-05-03 23:43:57.757807 dimstack-0.1.0/README.md
--rw-r--r--   0        0        0      472 2023-05-01 02:30:22.173505 dimstack-0.1.0/src/dimstack/__init__.py
--rw-r--r--   0        0        0      999 2023-05-01 02:28:16.205031 dimstack-0.1.0/src/dimstack/display.py
--rw-r--r--   0        0        0     3080 2023-05-02 23:48:17.980525 dimstack-0.1.0/src/dimstack/dist.py
--rw-r--r--   0        0        0    20673 2023-05-03 00:39:32.757721 dimstack-0.1.0/src/dimstack/eval.py
--rw-r--r--   0        0        0     4737 2023-05-03 00:22:58.861932 dimstack-0.1.0/src/dimstack/plot.py
--rw-r--r--   0        0        0     2276 2023-05-01 01:42:18.033521 dimstack-0.1.0/src/dimstack/stats.py
--rw-r--r--   0        0        0     1602 2023-05-02 00:59:08.364543 dimstack-0.1.0/src/dimstack/tolerance.py
--rw-r--r--   0        0        0      888 2023-05-02 23:58:10.807614 dimstack-0.1.0/src/dimstack/utils.py
--rw-r--r--   0        0        0        0 2023-03-13 21:19:03.810731 dimstack-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      482 2023-03-13 21:19:03.814714 dimstack-0.1.0/tests/test_doctest.py
--rw-r--r--   0        0        0     5294 2023-03-21 23:00:50.382907 dimstack-0.1.0/tests/test_McGrawHill.py
--rw-r--r--   0        0        0     4591 2023-03-21 22:49:23.311505 dimstack-0.1.0/tests/test_mitcalc.py
--rw-r--r--   0        0        0     2736 2023-03-16 00:41:22.536854 dimstack-0.1.0/tests/test_newconceptdesigns.py
--rw-r--r--   0        0        0     7209 1970-01-01 00:00:00.000000 dimstack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      944 2023-06-24 02:29:06.635800 dimstack-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7029 2023-06-23 02:16:21.182105 dimstack-0.2.0/README.md
+-rw-r--r--   0        0        0      473 2023-06-24 02:01:21.085947 dimstack-0.2.0/src/dimstack/__init__.py
+-rw-r--r--   0        0        0    20451 2023-06-24 02:07:06.201396 dimstack-0.2.0/src/dimstack/dim.py
+-rw-r--r--   0        0        0      939 2023-06-24 01:45:34.192106 dimstack-0.2.0/src/dimstack/display.py
+-rw-r--r--   0        0        0     3593 2023-06-24 01:45:59.133084 dimstack-0.2.0/src/dimstack/dist.py
+-rw-r--r--   0        0        0     5649 2023-06-24 02:02:47.771756 dimstack-0.2.0/src/dimstack/plot.py
+-rw-r--r--   0        0        0     2276 2023-05-01 01:42:18.033521 dimstack-0.2.0/src/dimstack/stats.py
+-rw-r--r--   0        0        0     1913 2023-06-24 01:35:28.755457 dimstack-0.2.0/src/dimstack/tolerance.py
+-rw-r--r--   0        0        0      888 2023-05-02 23:58:10.807614 dimstack-0.2.0/src/dimstack/utils.py
+-rw-r--r--   0        0        0        0 2023-03-13 21:19:03.810731 dimstack-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      480 2023-06-24 02:09:23.016258 dimstack-0.2.0/tests/test_doctest.py
+-rw-r--r--   0        0        0     5092 2023-06-24 02:09:09.811393 dimstack-0.2.0/tests/test_McGrawHill.py
+-rw-r--r--   0        0        0     4584 2023-06-24 02:09:01.071299 dimstack-0.2.0/tests/test_mitcalc.py
+-rw-r--r--   0        0        0     2694 2023-06-24 02:08:06.255732 dimstack-0.2.0/tests/test_newconceptdesigns.py
+-rw-r--r--   0        0        0     7079 1970-01-01 00:00:00.000000 dimstack-0.2.0/PKG-INFO
```

### Comparing `dimstack-0.1.0/pyproject.toml` & `dimstack-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dimstack"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = [
     { name = "phcreery", email = "phcreery@gmail.com" },
 ]
 dependencies = [
     "pandas>=1.5.2",
     "jinja2>=3.1.2",
@@ -22,26 +22,29 @@
 [project.optional-dependencies]
 dev = [
     "black>=23.1.0",
     "ruff>=0.0.254",
     "pkginfo>=1.9.6",
     "jupyter>=1.0.0",
     "jupyterlab>=3.6.1",
-    "jupyterlite-core>=0.1.0b19",
-    "jupyterlite-pyodide-kernel>=0.0.5",
+    "mkdocs>=1.4.3",
+    "mkdocstrings[python]>=0.21.2",
+    "mkdocs-material>=9.1.9",
 ]
 
 [tool.black]
 line-length = 160
 
 [tool.ruff]
 line-length = 160
 
 [tool.pdm.scripts]
 after_build = "cp '.\\dist\\*.whl' '.\\notebooks\\pypi\\'"
 test = "python -m unittest"
+docs = "python -m mkdocs serve"
+deploydocs = "python -m mkdocs gh-deploy"
 
 [build-system]
 requires = [
     "pdm-pep517>=1.0",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `dimstack-0.1.0/README.md` & `dimstack-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -99,54 +99,49 @@
 WARNING:root:Converting BasicDimension (5: f Bearing Sleeve +20 ± 0.026) to StatisticalDimension
 Spec: stack spec
       Name Description                                                                                                        Dimension Spec. Limits Median       k     C_p    C_pk Yield Probability Reject PPM
 stack spec             16: stacks on stacks '6 Sigma' Analysis (assuming inputs with Normal Distribution) +0.4 ± 0.26433 @ ± 4.5σ & k=0  [0.05, 0.8]  0.425 0.06667 2.12804 1.98617               100          0
 
 ```
 
-![](./doc/newplot.png)
-![](./doc/newplot2.png)
+![](./docs/newplot.png)
+![](./docs/newplot2.png)
 
 ## Usage
 
 dimstack can be used in a standard python script, or as a REPL, allowing use in JupyterLab.
 
 Demo usage in a JupyterLite Lab
+
 - https://phcreery.github.io/dimstack/lab/index.html
 
 Demo usage in a JuptyerLite REPL:
+
 - https://phcreery.github.io/dimstack/repl/index.html?kernel=python&toolbar=1&code=%pip%20install%20-q%20ds%0Aimport%20dimstack%20as%20ds
 
 Embed in your site:
+
 ```html
 <iframe
   src="https://phcreery.github.io/dimstack/repl/index.html?kernel=python&toolbar=1&code=%pip%20install%20-q%20ds%0Aimport%20dimstack%20as%20ds"
   width="100%"
   height="100%"
 ></iframe>
 ```
 
 ## Dev
 
 ### Notebooks
+
 In JupyterLite instances, you first have to pip install the wheel embedded.
 
 ```
 %pip install -q dimstack
 ```
 
-### Build
-
-```
-pdm build
-cp '.\\dist\\*.whl' '.\\notebooks\\pypi\\'
-cd notebooks
-jupyter lite build --contents .
-jupyter lite serve
-```
 ### Testing
 
 ```
 python -m unittest discover .\tests\
 ```
 
 # Acknowledgements
```

### Comparing `dimstack-0.1.0/src/dimstack/display.py` & `dimstack-0.2.0/src/dimstack/display.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pandas as pd
 
-DISPLAY_MODE = "text"  # "text", "str"/"string", "plot", or "df"
+DISPLAY_MODE = "text"
 FIGSIZE = (6, 3)
 
 
 def mode(dispmode: str):
     """Set the display mode for the stack.
 
     Args:
-        mode (str): "text", "str"/'string, "plot", or "df"
+        mode (str): "text", "str"/"string", "plot", or "df"
     """
     global DISPLAY_MODE
     DISPLAY_MODE = dispmode
 
 
-def display_df(data: dict, title: str = None, dispmode=None) -> pd.DataFrame:
+def display_df(data: dict, title: str = "", dispmode=None):
     """Display a dataframe.
 
     Args:
         df (pd.DataFrame): _description_
     """
     if dispmode is None:
         dispmode = DISPLAY_MODE
```

### Comparing `dimstack-0.1.0/src/dimstack/dist.py` & `dimstack-0.2.0/src/dimstack/dist.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 DIST_SCREENED = "Screened"  # Normal distribution which has been screened. e.g. Go-NoGo or Pass-Fail fixture.
 # DIST_NOTCHED = "Notched"  # This is a common distribution when parts are being sorted and the leftover parts are used.
 # DIST_NORMAL_LT = "Normal LT"  # Normal distribution which has been screened in order to remove lengths above a limit.
 # DIST_NORMAL_GT = "Normal GT"  # Normal distribution which has been screened in order to remove lengths below a limit.
 
 
 class Uniform:
+    """Uniform distribution.
+
+    Args:
+        lower (float): Lower limit.
+        upper (float): Upper limit.
+    """
+
     def __init__(self, lower: float, upper: float):
         self.lower = lower
         self.upper = upper
 
     def __repr__(self) -> str:
         return f"UniformDistribution({self.lower}, {self.upper})"
 
@@ -27,14 +34,21 @@
         return uniform.pdf(x, loc=self.lower, scale=self.upper - self.lower)
 
     def cdf(self, x: float):
         return uniform.cdf(x, loc=self.lower, scale=self.upper - self.lower)
 
 
 class Normal:
+    """Normal distribution.
+
+    Args:
+        mean (float): Mean.
+        stdev (float): Standard deviation.
+    """
+
     def __init__(self, mean: float, stdev: float):
         self.mean = mean
         self.stdev = stdev
 
     def __repr__(self) -> str:
         return f"NormalDistribution({self.mean}, {self.stdev})"
 
@@ -51,14 +65,23 @@
     @classmethod
     def fit(cls, data: Union[np.ndarray, List[float], List[int], List[np.float64], pd.Series]):
         mean, stdev = norm.fit(data)
         return cls(mean, stdev)
 
 
 class NormalScreened:
+    """Normal distribution which has been screened. e.g. Go-NoGo or Pass-Fail fixture.
+
+    Args:
+        mean (float): Mean.
+        stdev (float): Standard deviation.
+        lower (float): Lower limit.
+        upper (float): Upper limit.
+    """
+
     def __init__(self, mean: float, stdev: float, lower: float, upper: float):
         self.mean = mean
         self.stdev = stdev
         self.lower = lower
         self.upper = upper
 
     def __repr__(self) -> str:
```

### Comparing `dimstack-0.1.0/src/dimstack/eval.py` & `dimstack-0.2.0/src/dimstack/dim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import itertools
 import logging
 
 from typing import List, Union, Dict, Any
 
 from .display import display_df
-from .stats import C_p, C_pk, RSS_func, normal_cdf
+from .stats import C_p, C_pk, RSS_func
 from .tolerance import SymmetricBilateral, UnequalBilateral, Bilateral
 from .utils import nround, sign
 from . import dist
 
 POSITIVE = "+"
 NEGATIVE = "-"
 
 
-class BasicDimension:
+class Basic:
     """
     A measurement is a single measurement of a part.
 
     Args:
         nom (float, optional): The nominal value of the measurement. Defaults to 0.
         tol (Union[SymmetricBilateral, UnequalBilateral], optional): The tolerance of the measurement. Defaults to SymmetricBilateral(0).
         a (float, optional): The sensitivity of the measurement. Defaults to 1. If the nominal value is negative, the sensitivity will be multiplied by a -1
@@ -32,37 +32,37 @@
         self,
         nom: float,
         tol: Union[SymmetricBilateral, UnequalBilateral],
         a: float = 1,
         name: str = "Dimension",
         desc: str = "Dimension",
     ):
-        self.id = BasicDimension.newID()
+        self.id = Basic.newID()
         self.dir = sign(nom) * sign(a)
         self.nominal = abs(nom)
         self.tolerance = tol
         self.a = abs(a)
         self.name = name
         self.description = desc
         self.distribution = dist.DIST_UNIFORM
 
     def __repr__(self) -> str:
-        return f"BasicDimension({self.nominal}, {repr(self.tolerance)}, {self.a}, {self.name}, {self.description})"
+        return f"Basic({self.nominal}, {repr(self.tolerance)}, {self.a}, {self.name}, {self.description})"
 
     def __str__(self) -> str:
         return f"{self.id}: {self.name} {self.description} {self.direction}{nround(self.nominal)} {str(self.tolerance)}"
 
     def _repr_html_(self) -> str:
         return display_df(self.dict, f"Dimension: {self.name} - {self.description}", dispmode="plot")._repr_html_()
 
     def show(self):
         return display_df(self.dict, f"Dimension: {self.name} - {self.description}")
 
     @property
-    def dict(self) -> Dict[str, Any]:
+    def dict(self) -> List[Dict[str, Any]]:
         return [
             {
                 "ID": self.id,
                 "Name": self.name,
                 "Description": (self.description),
                 "dir": self.direction,
                 "Nom.": nround(self.nominal),
@@ -116,20 +116,20 @@
         self.nominal = median
         self.tolerance = SymmetricBilateral(tol)
         return self
 
     @classmethod
     def from_statistical_dimension(
         cls,
-        stat: "StatisticalDimension",
+        stat: "Statistical",
     ):
-        if type(stat) is BasicDimension:
+        if type(stat) is Basic:
             return stat
 
-        logging.warning(f"Converting StatisticalDimension ({stat}) to BasicDimension")
+        logging.warning(f"Converting Statistical ({stat}) to Basic")
         return cls(
             nom=stat.nominal * stat.dir,
             tol=stat.tolerance,
             a=stat.a,
             name=stat.name,
             desc=stat.description,
         )
@@ -137,16 +137,16 @@
     def get_dist(self):
         return dist.Uniform(self.lower_rel, self.upper_rel)
 
     def get_alt_dists(self):
         return []
 
 
-class StatisticalDimension(BasicDimension):
-    """StatisticalDimension
+class Statistical(Basic):
+    """Statistical
 
     Args:
         process_sigma (float, optional): The standard deviation of the process represented as ±σ. Defaults to ±3σ.
         k (float, optional): The ratio of the amount the center of the distribution is shifted from the mean represented as a multiple of the process
                             standard deviation. Defaults to 0σ.
         distribution (str, optional): The distribution of the measurement. Defaults to "Normal".
     """
@@ -157,61 +157,61 @@
         k: float = 0,
         distribution: str = dist.DIST_NORMAL,
         data=None,
         *args,
         **kwargs,
     ):
         # super().__init__(*args, **kwargs)
-        super(StatisticalDimension, self).__init__(*args, **kwargs)
+        super(Statistical, self).__init__(*args, **kwargs)
         self.distribution = distribution
         self.process_sigma = process_sigma
         self.k = k
         self.data = data
 
     def __repr__(self) -> str:
-        return f"StatisticalDimension({self.nominal}, {repr(self.tolerance)}, {self.a}, {self.name}, {self.description}, {self.process_sigma}, {self.k}, {self.distribution})"  # noqa: E501
+        return f"Statistical({self.nominal}, {repr(self.tolerance)}, {self.a}, {self.name}, {self.description}, {self.process_sigma}, {self.k}, {self.distribution})"  # noqa: E501
 
     def __str__(self) -> str:
         return f"{self.id}: {self.name} {self.description} {self.direction}{nround(self.nominal)} {str(self.tolerance)} @ ± {self.process_sigma}σ & k={self.k}"
 
     def _repr_html_(self) -> str:
         return display_df(self.dict, f"Dimension: {self.name} - {self.description}", dispmode="plot")._repr_html_()
 
     def show(self):
         return display_df(self.dict, f"Dimension: {self.name} - {self.description}")
 
     @classmethod
     def from_basic_dimension(
         cls,
-        basic: Union[BasicDimension, "StatisticalDimension"],
+        basic: Union[Basic, "Statistical"],
         process_sigma: float = 3,
         k: float = 0,
         distribution: str = "Normal",
     ):
-        if type(basic) is StatisticalDimension:
+        if type(basic) is Statistical:
             return basic
 
-        logging.warning(f"Converting BasicDimension ({basic}) to StatisticalDimension")
+        logging.warning(f"Converting Basic ({basic}) to Statistical dimension")
         return cls(
             nom=basic.nominal * basic.dir,
             tol=basic.tolerance,
             a=basic.a,
             name=basic.name,
             desc=basic.description,
             process_sigma=process_sigma,
             k=k,
             distribution=distribution,
         )
 
     @classmethod
     def from_data(cls, data, sigma=3, name="data", desc="data"):
-        """Create a StatisticalDimension from data
+        """Create a Statistical dimension from data
 
         Args:
-            data (np.ndarray): The data to create the dimension from
+            data (np.ndarray or similar): The data to create the dimension from
         """
         distribution = dist.Normal.fit(data)
 
         return cls(
             nom=distribution.mean,
             tol=SymmetricBilateral(distribution.stdev * sigma),
             a=1,
@@ -220,15 +220,15 @@
             process_sigma=sigma,
             k=0,
             distribution=dist.DIST_NORMAL,
             data=data,
         )
 
     @property
-    def dict(self) -> Dict[str, Any]:
+    def dict(self) -> List[Dict[str, Any]]:
         return [
             {
                 "ID": self.id,
                 "Name": self.name,
                 "Description": (self.description),
                 "dir": self.direction,
                 "Nom.": nround(self.nominal),
@@ -281,14 +281,17 @@
         effective standard deviation
         "6 stdev" is the standard deviation of the distribution
         """
         return abs(self.tolerance.T) / (6 * self.C_pk)
 
     @property
     def yield_loss_probability(self):
+        """
+        Returns the probability of a part being out of spec.
+        """
         UL = self.upper_rel
         LL = self.lower_rel
         # return 1 - normal_cdf(UL, self.mean_eff, self.stdev_eff) + normal_cdf(LL, self.mean_eff, self.stdev_eff)
         return 1 - self.get_dist().cdf(UL) + self.get_dist().cdf(LL)
 
     @property
     def yield_probability(self):
@@ -314,15 +317,15 @@
             return []
 
 
 class Stack:
     def __init__(
         self,
         title: str = "Stack",
-        items: List[Union[BasicDimension, StatisticalDimension]] = [],
+        items: List[Union[Basic, Statistical]] = [],
     ):
         self.title = title
         self.items = items
 
     def __repr__(self) -> str:
         return f"Stack({self.title}, [{', '.join([repr(item) for item in self.items])}])"
 
@@ -331,112 +334,118 @@
 
     def _repr_html_(self) -> str:
         return display_df(self.dict, f"Stack: {self.title}", dispmode="plot")._repr_html_()
 
     def show(self):
         return display_df(self.dict, f"Stack: {self.title}")
 
-    def append(self, measurement: Union[BasicDimension, StatisticalDimension]):
+    def append(self, measurement: Union[Basic, Statistical]):
         self.items.append(measurement)
 
     @property
-    def Closed(self) -> BasicDimension:
+    def Closed(self) -> Basic:
         nominal = sum([item.nominal * item.a * item.dir for item in self.items])
         tolerance = Bilateral(
             sum(filter(None, [item.tolerance_absolute.upper for item in self.items])),
             sum(filter(None, [item.tolerance_absolute.lower for item in self.items])),
         )
-        return BasicDimension(
+        return Basic(
             nominal,
             tolerance,
             name=f"{self.title} - Closed Analysis",
             desc="",
         )
 
     @property
-    def WC(self) -> BasicDimension:
+    def WC(self) -> Basic:
         """
         This is a simple WC calculation. This results in a Bilateral dimension with a tolerance that is the sum of the component tolerances.
         It states that in any combination of tolerances, you can be sure the result will be within the this resulting tolerance.
         """
         mean = sum([item.median * item.a * item.dir for item in self.items])
         t_wc = sum([abs(item.a * (item.tolerance.T / 2) * item.dir) for item in self.items])
         tolerance = Bilateral(t_wc)
-        return BasicDimension(
+        return Basic(
             nom=mean,
             tol=tolerance,
             name=f"{self.title} - WC Analysis",
             desc="",
         )
 
     @property
-    def RSS(self) -> StatisticalDimension:
+    def RSS(self) -> Statistical:
         """
         This is a simple RSS calculation. This is uses the RSS calculation method in the Dimensioning and Tolerancing Handbook, McGraw Hill.
         It is really only useful for a Bilateral stack of same process-stdev items. The RSS result has the same uncertainty as the measurements.
         Historically, Eq. (9.11) assumed that all of the component tolerances (t_i) represent a 3si value for their
         manufacturing processes. Thus, if all the component distributions are assumed to be normal, then the
         probability that a dimension is between ±t_i is 99.73%. If this is true, then the assembly gap distribution is
         normal and the probability that it is ±t_rss between is 99.73%.
         Although most people have assumed a value of ±3s for piecepart tolerances, the RSS equation works
         for “equal s” values. If the designer assumed that the input tolerances were ±4s values for the piecepart
         manufacturing processes, then the probability that the assembly is between ±t_rss is 99.9937 (4s).
         The 3s process limits using the RSS Model are similar to the Worst Case Model. The minimum gap is
         equal to the mean value minus the RSS variation at the gap. The maximum gap is equal to the mean value
         plus the RSS variation at the gap.
 
-        # Dimensioning and Tolerancing Handbook, McGraw Hill
-        # http://files.engineering.com/getfile.aspx?folder=69759f43-e81a-4801-9090-a0c95402bfc0&file=RSS_explanation.GIF
+        See:
+         - Dimensioning and Tolerancing Handbook, McGraw Hill
+         - http://files.engineering.com/getfile.aspx?folder=69759f43-e81a-4801-9090-a0c95402bfc0&file=RSS_explanation.GIF
         """
-        items: List[StatisticalDimension] = [StatisticalDimension.from_basic_dimension(item) for item in self.items]
+        items: List[Statistical] = [Statistical.from_basic_dimension(item) for item in self.items]
         d_g = sum([item.mean_eff * item.a * item.dir for item in items])
         t_rss = RSS_func(*[item.a * (item.tolerance.T / 2) * item.dir for item in items])
         tolerance = Bilateral(t_rss)
-        return StatisticalDimension(
+        return Statistical(
             nom=d_g,
             tol=tolerance,
             name=f"{self.title} - RSS Analysis",
             desc="(assuming inputs with Normal Distribution & ± 3σ)",
         )
 
     @property
-    def MRSS(self) -> StatisticalDimension:
-        items: List[StatisticalDimension] = [StatisticalDimension.from_basic_dimension(item) for item in self.items]
+    def MRSS(self) -> Statistical:
+        """Basically RSS with a coefficient modifier to make the tolerance tighter.
+
+        Returns:
+            Statistical: _description_
+        """
+        items: List[Statistical] = [Statistical.from_basic_dimension(item) for item in self.items]
         d_g = sum([item.mean_eff * item.a * item.dir for item in items])
         t_wc = sum([abs(item.a * (item.tolerance.T / 2) * item.dir) for item in self.items])
         t_rss = RSS_func(*[item.a * (item.tolerance.T / 2) * item.dir for item in items])
         n = len(self.items)
         C_f = (0.5 * (t_wc - t_rss)) / (t_rss * (n**0.5 - 1)) + 1
         t_mrss = C_f * t_rss
         tolerance = Bilateral(t_mrss)
         stdev = t_wc / 6
         sigma = t_mrss / stdev
-        return StatisticalDimension(
+        return Statistical(
             nom=d_g,
             tol=tolerance,
             name=f"{self.title} - MRSS Analysis",
             desc="(assuming inputs with Normal Distribution & ± 3σ)",
             process_sigma=sigma,
         )
 
-    def SixSigma(self, at: float = 3) -> StatisticalDimension:
-        items: List[StatisticalDimension] = [StatisticalDimension.from_basic_dimension(item) for item in self.items]
+    def SixSigma(self, at: float = 3) -> Statistical:
+        items: List[Statistical] = [Statistical.from_basic_dimension(item) for item in self.items]
         mean = sum([item.mean_eff * item.dir for item in items])
         stdev = RSS_func(*[item.stdev_eff for item in items])
         tolerance = Bilateral(stdev * at)
-        return StatisticalDimension(
+        return Statistical(
             nom=mean,
             tol=tolerance,
             process_sigma=at,
             name=f"{self.title} - '6 Sigma' Analysis",
             desc="(assuming inputs with Normal Distribution)",
         )
 
     @property
-    def dict(self) -> Dict[str, Any]:
+    def dict(self) -> List[Dict[str, Any]]:
         return [
             {
                 "ID": item.id,
                 "Name": item.name,
                 "Description": (item.description),
                 "dir": item.direction,
                 "Nom.": nround(item.nominal),
@@ -456,15 +465,15 @@
                 "Reject PPM": f"{nround(item.yield_loss_probability*1000000, 2)}" if hasattr(item, "yield_loss_probability") else "",
             }
             for item in self.items
         ]
 
 
 class Spec:
-    def __init__(self, name, description, dim: StatisticalDimension, LL, UL):
+    def __init__(self, name, description, dim: Union[Statistical, Basic], LL, UL):
         self.name = name
         self.description = description
         self.dim = dim
         self.LL = LL
         self.UL = UL
 
     def __repr__(self) -> str:
@@ -485,67 +494,60 @@
         return (self.LL + self.UL) / 2
 
     # @property
     # def mean(self):
     #     mean_shift = self.k * self.process_sigma * self.stdev
     #     return self.median + mean_shift
 
-    @property
-    def k(self):
-        """k"""
-        return abs((self.dim.mean - self.median) / ((self.UL - self.LL) / 2))
+    # @property
+    # def k(self):
+    #     """k"""
+    #     return abs((self.dim.mean - self.median) / ((self.UL - self.LL) / 2))
 
-    @property
-    def C_p(self):
-        return C_p(self.UL, self.LL, self.dim.stdev)
+    # @property
+    # def C_p(self):
+    #     return C_p(self.UL, self.LL, self.dim.stdev)
 
-    @property
-    def C_pk(self):
-        # return C_pk(self.C_p, self.k)
-        return min(
-            (self.UL - self.dim.mean) / (3 * self.dim.stdev),
-            (self.dim.mean - self.LL) / (3 * self.dim.stdev),
-        )
+    # @property
+    # def C_pk(self):
+    #     # return C_pk(self.C_p, self.k)
+    #     return min(
+    #         (self.UL - self.dim.mean) / (3 * self.dim.stdev),
+    #         (self.dim.mean - self.LL) / (3 * self.dim.stdev),
+    #     )
 
     @property
     def yield_loss_probability(self):
-        if self.UL > self.dim.Z_max:
-            upper = 1
-        else:
-            upper = normal_cdf(self.UL, self.dim.mean, self.dim.stdev)
-        if self.LL < self.dim.Z_min:
-            lower = 0
-        else:
-            lower = normal_cdf(self.LL, self.dim.mean, self.dim.stdev)
-        return 1 - (upper - lower)
+        """
+        Returns the probability of a part being out of spec.
+        """
+        return 1 - self.dim.get_dist().cdf(self.UL) + self.dim.get_dist().cdf(self.LL)
 
     @property
     def yield_probability(self):
         return 1 - self.yield_loss_probability
 
     @property
     def R(self):
         """Return the yield loss probability in PPM"""
         return self.yield_loss_probability * 1000000
 
     @property
-    def dict(self) -> Dict[str, Any]:
-        return [
-            {
-                "Name": self.name,
-                "Description": self.description,
-                "Dimension": f"{self.dim}",
-                "Spec. Limits": f"[{nround(self.LL)}, {nround(self.UL)}]",
-                "Median": nround(self.median),
-                "k": nround(self.k),
-                "C_p": nround(self.C_p),
-                "C_pk": nround(self.C_pk),
-                "Yield Probability": f"{nround(self.yield_probability*100, 8)}",
-                "Reject PPM": f"{nround(self.R, 2)}",
-            }
-        ]
+    def dict(self) -> List[Dict[str, Any]]:
+        return [{
+            "Name": self.name,
+            "Description": self.description,
+            "Dimension": f"{self.dim}",
+            "Spec. Limits": f"[{nround(self.LL)}, {nround(self.UL)}]",
+            "Median": nround(self.median),
+            # "k": nround(self.k),
+            # "C_p": nround(self.C_p),
+            # "C_pk": nround(self.C_pk),
+            "Yield Probability": f"{nround(self.yield_probability*100, 8)}",
+            "Reject PPM": f"{nround(self.R, 2)}",
+        }]
 
 
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `dimstack-0.1.0/src/dimstack/plot.py` & `dimstack-0.2.0/src/dimstack/plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,33 +2,43 @@
 import itertools
 
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 import plotly.express as px
 
-from .eval import Stack, BasicDimension, StatisticalDimension
+from .dim import Stack, Basic, Statistical
 
 
 class StackPlot:
+    """Plot a stack of dimensions. This is a wrapper around Plotly."""
+
     def __init__(self):
         colors = px.colors.qualitative.Plotly
         self.col_pal_iterator = itertools.cycle(colors)
+        self.title = "Dimension chart"
 
         # fig = go.Figure()
         fig = make_subplots(specs=[[{"secondary_y": True}]], x_title="Distance (mm)")
         self.fig = fig
         self.fig.update_yaxes(title_text="Dimension", secondary_y=False)
         self.fig.update_yaxes(title_text="Probability Density", secondary_y=True)
-        self.fig.update_layout(go.Layout(title="Dimension chart"))
+        self.fig.update_layout(go.Layout(title=self.title))
 
     def show(self):
+        """Show the plot. This works in both Jupyter notebooks and in a Python script."""
         return self.fig.show()
 
-    def add_dimension(self, item: Union[BasicDimension, StatisticalDimension], start_pos=0):
+    def add_dimension(self, item: Union[Basic, Statistical], start_pos=0):
+        """Add a dimension to the plot.
+
+        Args:
+            item (Union[Basic, Statistical]): _description_
+            start_pos (int, optional): _description_. Defaults to 0.
+        """
         prev_pos = start_pos
         color = next(self.col_pal_iterator)
 
         new_pos = prev_pos + item.nominal * item.dir
         ll = min(new_pos + item.tolerance.upper * item.dir, new_pos - item.tolerance.lower * item.dir)
         ul = max(new_pos + item.tolerance.upper * item.dir, new_pos - item.tolerance.lower * item.dir)
 
@@ -107,24 +117,45 @@
                 name=f"{item.name} Data",
                 legendgroup=f"{item.name}",
                 marker_color=color,
                 opacity=0.5,
             )
 
     def add_stack(self, stack: Stack):
+        """Add a stack of dimensions to the plot.
+
+        Args:
+            stack (Stack): _description_
+
+        Returns:
+            _type_: _description_
+        """ """"""
         prev_pos = 0
         for item in stack.items:
             new_pos = prev_pos + item.nominal * item.dir
             self.add_dimension(item, start_pos=prev_pos)
             prev_pos = new_pos
 
+        self.fig.update_layout(go.Layout(title=stack.title))
+
         return self
 
-    def add(self, item):
+    def add(self, item: Union[Stack, Basic, Statistical]):
+        """Add a dimension or stack to the plot.
+
+        Args:
+            item (Stack, Basic, Statistical): _description_
+
+        Raises:
+            TypeError: If the item is not a Stack, Basic, or Statistical.
+
+        Returns:
+            StackPlot: self
+        """
         if isinstance(item, Stack):
             self.add_stack(item)
-        elif isinstance(item, (BasicDimension, StatisticalDimension)):
+        elif isinstance(item, (Basic, Statistical)):
             self.add_dimension(item)
         else:
             raise TypeError(f"Cannot add {type(item)} to StackPlot")
 
         return self
```

### Comparing `dimstack-0.1.0/src/dimstack/stats.py` & `dimstack-0.2.0/src/dimstack/stats.py`

 * *Files identical despite different names*

### Comparing `dimstack-0.1.0/src/dimstack/utils.py` & `dimstack-0.2.0/src/dimstack/utils.py`

 * *Files identical despite different names*

### Comparing `dimstack-0.1.0/tests/test_McGrawHill.py` & `dimstack-0.2.0/tests/test_McGrawHill.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,75 +3,75 @@
 
 import dimstack
 
 # this test is a copy Dimensioning and Tolerancing Handbook by McGraw Hill, Chapter 9
 
 
 class McGrawHill_1(unittest.TestCase):
-    m1 = dimstack.eval.BasicDimension(
+    m1 = dimstack.dim.Basic(
         nom=-0.375,
         tol=dimstack.tolerance.UnequalBilateral(0, 0.031),
         name="A",
         desc="Screw thread length",
     )
-    m2 = dimstack.eval.BasicDimension(
+    m2 = dimstack.dim.Basic(
         nom=0.032,
         tol=dimstack.tolerance.SymmetricBilateral(0.002),
         name="B",
         desc="Washer Length",
     )
-    m3 = dimstack.eval.BasicDimension(
+    m3 = dimstack.dim.Basic(
         nom=0.06,
         tol=dimstack.tolerance.SymmetricBilateral(0.003),
         name="C",
         desc="Inner bearing cap turned length",
     )
-    m4 = dimstack.eval.BasicDimension(
+    m4 = dimstack.dim.Basic(
         nom=0.438,
         tol=dimstack.tolerance.UnequalBilateral(0, 0.015),
         name="D",
         desc="Bearing length",
     )
-    m5 = dimstack.eval.BasicDimension(
+    m5 = dimstack.dim.Basic(
         nom=0.12,
         tol=dimstack.tolerance.SymmetricBilateral(0.005),
         name="E",
         desc="Spacer turned length",
     )
-    m6 = dimstack.eval.BasicDimension(
+    m6 = dimstack.dim.Basic(
         nom=1.5,
         tol=dimstack.tolerance.UnequalBilateral(0.01, 0.004),
         name="F",
         desc="Rotor length",
     )
     m7 = deepcopy(m5)
     m7.name = "G"
     m8 = deepcopy(m4)
     m8.name = "H"
-    m9 = dimstack.eval.BasicDimension(
+    m9 = dimstack.dim.Basic(
         nom=0.450,
         tol=dimstack.tolerance.SymmetricBilateral(0.007),
         name="I",
         desc="Pulley casting length",
     )
-    m10 = dimstack.eval.BasicDimension(
+    m10 = dimstack.dim.Basic(
         nom=-3.019,
         tol=dimstack.tolerance.UnequalBilateral(0.012, 0),
         name="J",
         desc="Shaft turned length",
     )
-    m11 = dimstack.eval.BasicDimension(
+    m11 = dimstack.dim.Basic(
         nom=0.3,
         tol=dimstack.tolerance.SymmetricBilateral(0.03),
         name="K",
         desc="Tapped hole depth",
     )
     items = [m1, m2, m3, m4, m5, m6, m7, m8, m9, m10, m11]
 
-    stack = dimstack.eval.Stack(title="stacks on stacks", items=items)
+    stack = dimstack.dim.Stack(title="stacks on stacks", items=items)
 
     def test_WC(self):
         self.assertEqual(dimstack.utils.nround(McGrawHill_1.stack.WC.nominal), 0.0615)
         self.assertEqual(dimstack.utils.nround(McGrawHill_1.stack.WC.tolerance.T / 2), 0.0915)  # 0.0955
         self.assertEqual(dimstack.utils.nround(McGrawHill_1.stack.WC.Z_min, 5), -0.03)  # -0.034
         self.assertEqual(dimstack.utils.nround(McGrawHill_1.stack.WC.Z_max, 3), 0.153)  # 0.157
 
@@ -88,28 +88,28 @@
         self.assertEqual(dimstack.utils.nround(McGrawHill_1.stack.MRSS.Z_max, 3), 0.111)  # 0.1120
 
 
 # this test is a copy Dimensioning and Tolerancing Handbook by McGraw Hill, Chaper 12-12
 
 
 class McGrawHill_2(unittest.TestCase):
-    m1 = dimstack.eval.BasicDimension(nom=0.875, tol=dimstack.tolerance.SymmetricBilateral(0.010), a=-0.5146, name="A")
-    m2 = dimstack.eval.BasicDimension(nom=1.625, tol=dimstack.tolerance.SymmetricBilateral(0.020), a=0.1567, name="B")
-    m3 = dimstack.eval.BasicDimension(nom=1.700, tol=dimstack.tolerance.SymmetricBilateral(0.012), a=0.4180, name="C")
-    m4 = dimstack.eval.BasicDimension(nom=0.875, tol=dimstack.tolerance.SymmetricBilateral(0.010), a=-1.000, name="D")
-    m5 = dimstack.eval.BasicDimension(nom=2.625, tol=dimstack.tolerance.SymmetricBilateral(0.020), a=-0.0540, name="E")
-    m6 = dimstack.eval.BasicDimension(nom=7.875, tol=dimstack.tolerance.SymmetricBilateral(0.030), a=0.4372, name="F")
-    m7 = dimstack.eval.BasicDimension(nom=4.125, tol=dimstack.tolerance.SymmetricBilateral(0.010), a=1.000, name="G")
-    m8 = dimstack.eval.BasicDimension(nom=1.125, tol=dimstack.tolerance.SymmetricBilateral(0.020), a=-0.9956, name="H")
-    m9 = dimstack.eval.BasicDimension(nom=3.625, tol=dimstack.tolerance.SymmetricBilateral(0.015), a=-0.7530, name="J")
-    m10 = dimstack.eval.BasicDimension(nom=5.125, tol=dimstack.tolerance.SymmetricBilateral(0.020), a=-0.4006, name="K")
-    m11 = dimstack.eval.BasicDimension(nom=1.000, tol=dimstack.tolerance.SymmetricBilateral(0.010), a=-1.0914, name="M")
+    m1 = dimstack.dim.Basic(nom=0.875, tol=dimstack.tolerance.SymmetricBilateral(0.010), a=-0.5146, name="A")
+    m2 = dimstack.dim.Basic(nom=1.625, tol=dimstack.tolerance.SymmetricBilateral(0.020), a=0.1567, name="B")
+    m3 = dimstack.dim.Basic(nom=1.700, tol=dimstack.tolerance.SymmetricBilateral(0.012), a=0.4180, name="C")
+    m4 = dimstack.dim.Basic(nom=0.875, tol=dimstack.tolerance.SymmetricBilateral(0.010), a=-1.000, name="D")
+    m5 = dimstack.dim.Basic(nom=2.625, tol=dimstack.tolerance.SymmetricBilateral(0.020), a=-0.0540, name="E")
+    m6 = dimstack.dim.Basic(nom=7.875, tol=dimstack.tolerance.SymmetricBilateral(0.030), a=0.4372, name="F")
+    m7 = dimstack.dim.Basic(nom=4.125, tol=dimstack.tolerance.SymmetricBilateral(0.010), a=1.000, name="G")
+    m8 = dimstack.dim.Basic(nom=1.125, tol=dimstack.tolerance.SymmetricBilateral(0.020), a=-0.9956, name="H")
+    m9 = dimstack.dim.Basic(nom=3.625, tol=dimstack.tolerance.SymmetricBilateral(0.015), a=-0.7530, name="J")
+    m10 = dimstack.dim.Basic(nom=5.125, tol=dimstack.tolerance.SymmetricBilateral(0.020), a=-0.4006, name="K")
+    m11 = dimstack.dim.Basic(nom=1.000, tol=dimstack.tolerance.SymmetricBilateral(0.010), a=-1.0914, name="M")
     items = [m1, m2, m3, m4, m5, m6, m7, m8, m9, m10, m11]
 
-    stack = dimstack.eval.Stack(title="stacks on stacks", items=items)
+    stack = dimstack.dim.Stack(title="stacks on stacks", items=items)
 
     def test_WC(self):
         self.assertEqual(dimstack.utils.nround(McGrawHill_2.stack.WC.nominal), 0.07201)  # 0.0719
         self.assertEqual(dimstack.utils.nround(McGrawHill_2.stack.WC.tolerance.T / 2), 0.09763)  # 0.0967
         self.assertEqual(dimstack.utils.nround(McGrawHill_2.stack.WC.Z_min, 5), -0.02561)  # -0.0248
```

### Comparing `dimstack-0.1.0/tests/test_mitcalc.py` & `dimstack-0.2.0/tests/test_mitcalc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import unittest
 import dimstack
 
 # this test is a copy of MITCalc User Interface diagram
 
-m1 = dimstack.eval.StatisticalDimension(
+m1 = dimstack.dim.Statistical(
     nom=208,
     tol=dimstack.tolerance.SymmetricBilateral(0.036),
     process_sigma=6,
     k=0.25,
     name="a",
     desc="Shaft",
 )
-m2 = dimstack.eval.StatisticalDimension(
+m2 = dimstack.dim.Statistical(
     nom=-1.75,
     tol=dimstack.tolerance.UnequalBilateral(0, 0.06),
     process_sigma=3,
     name="b",
     desc="Retainer ring",
 )
-m3 = dimstack.eval.StatisticalDimension(nom=-23, tol=dimstack.tolerance.UnequalBilateral(0, 0.12), process_sigma=3, name="c", desc="Bearing")
-m4 = dimstack.eval.StatisticalDimension(
+m3 = dimstack.dim.Statistical(nom=-23, tol=dimstack.tolerance.UnequalBilateral(0, 0.12), process_sigma=3, name="c", desc="Bearing")
+m4 = dimstack.dim.Statistical(
     nom=20,
     tol=dimstack.tolerance.SymmetricBilateral(0.026),
     process_sigma=3,
     name="d",
     desc="Bearing Sleeve",
 )
-m5 = dimstack.eval.StatisticalDimension(nom=-200, tol=dimstack.tolerance.SymmetricBilateral(0.145), process_sigma=3, name="e", desc="Case")
-m6 = dimstack.eval.StatisticalDimension(
+m5 = dimstack.dim.Statistical(nom=-200, tol=dimstack.tolerance.SymmetricBilateral(0.145), process_sigma=3, name="e", desc="Case")
+m6 = dimstack.dim.Statistical(
     nom=20,
     tol=dimstack.tolerance.SymmetricBilateral(0.026),
     process_sigma=3,
     name="f",
     desc="Bearing Sleeve",
 )
-m7 = dimstack.eval.StatisticalDimension(nom=-23, tol=dimstack.tolerance.UnequalBilateral(0, 0.12), process_sigma=3, name="g", desc="Bearing")
+m7 = dimstack.dim.Statistical(nom=-23, tol=dimstack.tolerance.UnequalBilateral(0, 0.12), process_sigma=3, name="g", desc="Bearing")
 items = [m1, m2, m3, m4, m5, m6, m7]
 
-stack = dimstack.eval.Stack(title="stacks on stacks", items=items)
+stack = dimstack.dim.Stack(title="stacks on stacks", items=items)
 
 
 class MITCalc(unittest.TestCase):
     def test_input(self):
         self.assertEqual(len(stack.items), 7)
         self.assertEqual(stack.items[0].nominal, 208)
         self.assertEqual(stack.items[0].tolerance.upper, 0.036)
@@ -62,15 +62,15 @@
         # self.assertEqual(dimstack.utils.nround(stack.RSS.mean), 0.4)
         self.assertEqual(dimstack.utils.nround(stack.RSS.nominal), 0.4)
         self.assertEqual(dimstack.utils.nround(stack.RSS.tolerance.T / 2), 0.17825)
         # self.assertEqual(dimstack.utils.nround(stack.RSS.stdev, 6), 0.059417)
 
     def test_RSS_assembly(self):
         eval = stack.RSS
-        spec = dimstack.eval.Spec("spec", "", dim=eval, LL=0.05, UL=0.8)
+        spec = dimstack.dim.Spec("spec", "", dim=eval, LL=0.05, UL=0.8)
 
         self.assertEqual(dimstack.utils.nround(spec.R, 1), 0.0)
 
     # def test_MRSS(self):
     #     self.assertEqual(dimstack.utils.nround(stack.MRSS.mean), 0.4)
     #     self.assertEqual(dimstack.utils.nround(stack.MRSS.nominal), 0.4)
     #     # self.assertEqual(dimstack.utils.nround(stack.MRSS.tolerance.T / 2), 0.17825)
@@ -89,16 +89,16 @@
         self.assertEqual(dimstack.utils.nround(stack.SixSigma(at=4.5).tolerance.T / 2), 0.26433)
         self.assertEqual(dimstack.utils.nround(stack.SixSigma(at=4.5).stdev, 6), 0.05874)
         self.assertEqual(dimstack.utils.nround(stack.SixSigma(at=4.5).Z_min), 0.13567)
         self.assertEqual(dimstack.utils.nround(stack.SixSigma(at=4.5).Z_max), 0.66433)
 
     def test_SixSigma_assembly(self):
         eval = stack.SixSigma(at=4.5)
-        spec = dimstack.eval.Spec("spec", "", dim=eval, LL=0.05, UL=0.8)
+        spec = dimstack.dim.Spec("spec", "", dim=eval, LL=0.05, UL=0.8)
 
-        self.assertEqual(dimstack.utils.nround(spec.C_p), 2.12804)
-        self.assertEqual(dimstack.utils.nround(spec.C_pk), 1.98617)
+        # self.assertEqual(dimstack.utils.nround(spec.C_p), 2.12804) # temporarily removed 20230623
+        # self.assertEqual(dimstack.utils.nround(spec.C_pk), 1.98617) # temporarily removed 20230623
         self.assertEqual(dimstack.utils.nround(spec.R, 1), 0.0)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `dimstack-0.1.0/tests/test_newconceptdesigns.py` & `dimstack-0.2.0/tests/test_newconceptdesigns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import unittest
 import dimstack
 
 # this test is a copy of "My First Stackup" in newconceptzdesign http://www.newconceptzdesign.com/tutorial/Tutorial-My_first_stackup.html
 
-m1 = dimstack.eval.StatisticalDimension(
+m1 = dimstack.dim.Statistical(
     nom=-0.3190,
     tol=dimstack.tolerance.SymmetricBilateral(0.0050),
     process_sigma=6,
     name="PN16",
     desc="Mounting face to rt. end",
 )
-m2 = dimstack.eval.StatisticalDimension(
+m2 = dimstack.dim.Statistical(
     nom=10.4860,
     tol=dimstack.tolerance.SymmetricBilateral(0.0100),
     process_sigma=6,
     name="PN07",
     desc="Overall width",
 )
-m3 = dimstack.eval.StatisticalDimension(
-    nom=-0.3190, tol=dimstack.tolerance.SymmetricBilateral(0.0050), process_sigma=6, name="PN16", desc="Mounting face to rt. end"
-)
+m3 = dimstack.dim.Statistical(nom=-0.3190, tol=dimstack.tolerance.SymmetricBilateral(0.0050), process_sigma=6, name="PN16", desc="Mounting face to rt. end")
 items = [m1, m2, m3]
 
-stack = dimstack.eval.Stack(title="PN16/NJ210E - gap between cover and bearing (shaft pushed rt.)", items=items)
+stack = dimstack.dim.Stack(title="PN16/NJ210E - gap between cover and bearing (shaft pushed rt.)", items=items)
 
 
 class MITCalc(unittest.TestCase):
     def test_Closed(self):
         self.assertEqual(dimstack.utils.nround(stack.Closed.nominal), 9.8480)
         self.assertEqual(dimstack.utils.nround(stack.Closed.tolerance.T / 2), 0.0200)
         self.assertEqual(dimstack.utils.nround(stack.Closed.Z_min), 9.8280)
@@ -43,16 +41,16 @@
         self.assertEqual(dimstack.utils.nround(stack.SixSigma(at=6).nominal), 9.8480)
         self.assertEqual(dimstack.utils.nround(stack.SixSigma(at=6).tolerance.T / 2, 4), 0.0122)
         self.assertEqual(dimstack.utils.nround(stack.SixSigma(at=6).stdev * 2, 5), 0.00408)  # times 2 !?!?
         self.assertEqual(dimstack.utils.nround(stack.SixSigma(at=6).Z_min, 4), 9.8358)
         self.assertEqual(dimstack.utils.nround(stack.SixSigma(at=6).Z_max, 4), 9.8602)
 
     # def test_SixSigma_assembly(self):
-    #     eval = stack.SixSigma(at=4.5)
-    #     assy = dimstack.eval.Assembly("assy", "", dim=eval, LL=0.05, UL=0.8, process_sigma=4.5)
+    #     dim = stack.SixSigma(at=4.5)
+    #     assy = dimstack.dim.Assembly("assy", "", dim=dim, LL=0.05, UL=0.8, process_sigma=4.5)
 
     #     self.assertEqual(dimstack.utils.nround(assy.C_p), 2.12804)
     #     self.assertEqual(dimstack.utils.nround(assy.C_pk), 1.98617)
     #     self.assertEqual(dimstack.utils.nround(assy.R, 1), 0.0)
 
 
 if __name__ == "__main__":
```

### Comparing `dimstack-0.1.0/PKG-INFO` & `dimstack-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimstack
-Version: 0.1.0
+Version: 0.2.0
 License: MIT
 Author-email: phcreery <phcreery@gmail.com>
 Requires-Python: >=3.8, <3.11
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # dimstack
@@ -108,54 +108,49 @@
 WARNING:root:Converting BasicDimension (5: f Bearing Sleeve +20 ± 0.026) to StatisticalDimension
 Spec: stack spec
       Name Description                                                                                                        Dimension Spec. Limits Median       k     C_p    C_pk Yield Probability Reject PPM
 stack spec             16: stacks on stacks '6 Sigma' Analysis (assuming inputs with Normal Distribution) +0.4 ± 0.26433 @ ± 4.5σ & k=0  [0.05, 0.8]  0.425 0.06667 2.12804 1.98617               100          0
 
 ```
 
-![](./doc/newplot.png)
-![](./doc/newplot2.png)
+![](./docs/newplot.png)
+![](./docs/newplot2.png)
 
 ## Usage
 
 dimstack can be used in a standard python script, or as a REPL, allowing use in JupyterLab.
 
 Demo usage in a JupyterLite Lab
+
 - https://phcreery.github.io/dimstack/lab/index.html
 
 Demo usage in a JuptyerLite REPL:
+
 - https://phcreery.github.io/dimstack/repl/index.html?kernel=python&toolbar=1&code=%pip%20install%20-q%20ds%0Aimport%20dimstack%20as%20ds
 
 Embed in your site:
+
 ```html
 <iframe
   src="https://phcreery.github.io/dimstack/repl/index.html?kernel=python&toolbar=1&code=%pip%20install%20-q%20ds%0Aimport%20dimstack%20as%20ds"
   width="100%"
   height="100%"
 ></iframe>
 ```
 
 ## Dev
 
 ### Notebooks
+
 In JupyterLite instances, you first have to pip install the wheel embedded.
 
 ```
 %pip install -q dimstack
 ```
 
-### Build
-
-```
-pdm build
-cp '.\\dist\\*.whl' '.\\notebooks\\pypi\\'
-cd notebooks
-jupyter lite build --contents .
-jupyter lite serve
-```
 ### Testing
 
 ```
 python -m unittest discover .\tests\
 ```
 
 # Acknowledgements
```

