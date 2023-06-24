# Comparing `tmp/pyextremes-2.3.0.tar.gz` & `tmp/pyextremes-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyextremes-2.3.0.tar", max compression
+gzip compressed data, was "pyextremes-2.3.1.tar", max compression
```

## Comparing `pyextremes-2.3.0.tar` & `pyextremes-2.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1056 2023-04-09 21:48:52.099873 pyextremes-2.3.0/LICENSE
--rw-r--r--   0        0        0     4380 2023-04-09 21:48:52.099873 pyextremes-2.3.0/README.md
--rw-r--r--   0        0        0     2774 2023-04-09 21:48:52.103873 pyextremes-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      533 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/__init__.py
--rw-r--r--   0        0        0    63915 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/eva.py
--rw-r--r--   0        0        0      275 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/__init__.py
--rw-r--r--   0        0        0     5130 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/block_maxima.py
--rw-r--r--   0        0        0     3134 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/extremes.py
--rw-r--r--   0        0        0     3934 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/peaks_over_threshold.py
--rw-r--r--   0        0        0     5599 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/return_periods.py
--rw-r--r--   0        0        0     2318 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/transformation.py
--rw-r--r--   0        0        0      252 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/__init__.py
--rw-r--r--   0        0        0    16195 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/distribution.py
--rw-r--r--   0        0        0     6562 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/model_base.py
--rw-r--r--   0        0        0     8988 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/model_emcee.py
--rw-r--r--   0        0        0    10946 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/model_mle.py
--rw-r--r--   0        0        0     3586 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/models.py
--rw-r--r--   0        0        0        0 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/multivariate/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/multivariate/meva.py
--rw-r--r--   0        0        0      444 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/__init__.py
--rw-r--r--   0        0        0     6661 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/extremes.py
--rw-r--r--   0        0        0    11766 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/mcmc.py
--rw-r--r--   0        0        0     2796 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/probability_plots.py
--rw-r--r--   0        0        0     4381 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/return_values.py
--rw-r--r--   0        0        0     1523 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/style.py
--rw-r--r--   0        0        0        1 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/py.typed
--rw-r--r--   0        0        0       88 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tests/__init__.py
--rw-r--r--   0        0        0     3018 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tests/ks_test.py
--rw-r--r--   0        0        0     2827 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tests/test_base.py
--rw-r--r--   0        0        0      365 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tuning/__init__.py
--rw-r--r--   0        0        0      259 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tuning/hyperparameters.py
--rw-r--r--   0        0        0      148 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tuning/model_comparison.py
--rw-r--r--   0        0        0    32873 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tuning/threshold_selection.py
--rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 pyextremes-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-06-24 19:49:47.091270 pyextremes-2.3.1/LICENSE
+-rw-r--r--   0        0        0     4380 2023-06-24 19:49:47.091270 pyextremes-2.3.1/README.md
+-rw-r--r--   0        0        0     2774 2023-06-24 19:49:47.099270 pyextremes-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0      533 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/__init__.py
+-rw-r--r--   0        0        0    64042 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/eva.py
+-rw-r--r--   0        0        0      275 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/extremes/__init__.py
+-rw-r--r--   0        0        0     5130 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/extremes/block_maxima.py
+-rw-r--r--   0        0        0     3134 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/extremes/extremes.py
+-rw-r--r--   0        0        0     3934 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/extremes/peaks_over_threshold.py
+-rw-r--r--   0        0        0     5601 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/extremes/return_periods.py
+-rw-r--r--   0        0        0     2318 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/extremes/transformation.py
+-rw-r--r--   0        0        0      252 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/models/__init__.py
+-rw-r--r--   0        0        0    16197 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/models/distribution.py
+-rw-r--r--   0        0        0     6561 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/models/model_base.py
+-rw-r--r--   0        0        0     8990 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/models/model_emcee.py
+-rw-r--r--   0        0        0    10946 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/models/model_mle.py
+-rw-r--r--   0        0        0     3585 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/models/models.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/multivariate/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/multivariate/meva.py
+-rw-r--r--   0        0        0      444 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/plotting/__init__.py
+-rw-r--r--   0        0        0     6661 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/plotting/extremes.py
+-rw-r--r--   0        0        0    11766 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/plotting/mcmc.py
+-rw-r--r--   0        0        0     2796 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/plotting/probability_plots.py
+-rw-r--r--   0        0        0     4381 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/plotting/return_values.py
+-rw-r--r--   0        0        0     1523 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/plotting/style.py
+-rw-r--r--   0        0        0        1 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/py.typed
+-rw-r--r--   0        0        0       88 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/tests/__init__.py
+-rw-r--r--   0        0        0     3018 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/tests/ks_test.py
+-rw-r--r--   0        0        0     2827 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/tests/test_base.py
+-rw-r--r--   0        0        0      365 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/tuning/__init__.py
+-rw-r--r--   0        0        0      259 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/tuning/hyperparameters.py
+-rw-r--r--   0        0        0      148 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/tuning/model_comparison.py
+-rw-r--r--   0        0        0    32873 2023-06-24 19:49:47.099270 pyextremes-2.3.1/src/pyextremes/tuning/threshold_selection.py
+-rw-r--r--   0        0        0     5726 1970-01-01 00:00:00.000000 pyextremes-2.3.1/PKG-INFO
```

### Comparing `pyextremes-2.3.0/LICENSE` & `pyextremes-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/README.md` & `pyextremes-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/pyproject.toml` & `pyextremes-2.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyextremes"
-version = "2.3.0"
+version = "2.3.1"
 description = "Extreme Value Analysis (EVA) in Python"
 license = "MIT"
 authors = ["George Bocharov <bocharovgeorgii@gmail.com>"]
 readme = "README.md"
 homepage = "https://georgebv.github.io/pyextremes"
 repository = "https://github.com/georgebv/pyextremes"
 keywords=[
```

### Comparing `pyextremes-2.3.0/src/pyextremes/__init__.py` & `pyextremes-2.3.1/src/pyextremes/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.3.0"
+__version__ = "2.3.1"
 __all__ = [
     "EVA",
     "get_extremes",
     "get_return_periods",
     "get_model",
     "plot_mean_residual_life",
     "plot_parameter_stability",
```

### Comparing `pyextremes-2.3.0/src/pyextremes/eva.py` & `pyextremes-2.3.1/src/pyextremes/eva.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,28 +213,31 @@
 
     @property
     def AIC(self) -> float:
         return self.model.AIC
 
     def test_ks(self, significance_level: float = 0.05) -> KolmogorovSmirnov:
         return KolmogorovSmirnov(
-            extremes=self.extremes,
+            extremes=self.extremes_transformer.transformed_extremes,
             distribution=self.distribution.distribution,
-            fit_parameters=self.model.fit_parameters,
+            fit_parameters={
+                **self.model.fit_parameters,
+                **self.model.distribution._fixed_parameters,
+            },
             significance_level=significance_level,
         )
 
     def __repr__(self) -> str:
         # Width of repr block
         width = 88
 
         # Separator used to separate two columns of the repr block
         sep = " " * 6
 
-        # Widths of left and ridght columns
+        # Widths of left and right columns
         lwidth = (width - len(sep)) // 2
         rwidth = width - (lwidth + len(sep))
 
         # Function used to convert label-value pair
         # into a sequence of lines within a column
         def align_text(label: str, value: str, position: str) -> typing.List[str]:
             assert position in ["left", "right"]
@@ -906,15 +909,15 @@
             or a subclass of scipy.stats.rv_continuous.
             See https://docs.scipy.org/doc/scipy/reference/stats.html
             By default the distribution is selected automatically
             as best between 'genextreme' and 'gumbel_r' for 'BM' extremes
             and 'genpareto' and 'expon' for 'POT' extremes.
             Best distribution is selected using the AIC metric.
         distribution_kwargs : dict, optional
-            Special keyword arguments, passsed to the `.fit` method of the distribution.
+            Special keyword arguments, passed to the `.fit` method of the distribution.
             These keyword arguments represent parameters to be held fixed.
             Names of parameters to be fixed must have 'f' prefixes. Valid parameters:
                 - shape(s): 'fc', e.g. fc=0
                 - location: 'floc', e.g. floc=0
                 - scale: 'fscale', e.g. fscale=1
             See documentation of a specific scipy.stats distribution
             for names of available parameters.
```

### Comparing `pyextremes-2.3.0/src/pyextremes/extremes/block_maxima.py` & `pyextremes-2.3.1/src/pyextremes/extremes/block_maxima.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/extremes/extremes.py` & `pyextremes-2.3.1/src/pyextremes/extremes/extremes.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/extremes/peaks_over_threshold.py` & `pyextremes-2.3.1/src/pyextremes/extremes/peaks_over_threshold.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/extremes/return_periods.py` & `pyextremes-2.3.1/src/pyextremes/extremes/return_periods.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,18 +135,18 @@
         alpha, beta = plotting_positions[plotting_position.lower()]
     except KeyError as _error:
         raise ValueError(
             f"invalid value in '{plotting_position}' "
             f"for the 'plotting_position' argument"
         ) from _error
 
-    # Caclucate exceedance probabilities
+    # Calculate exceedance probabilities
     exceedance_probability = (ranks - alpha) / (len(extremes) + 1 - alpha - beta)
 
-    # Calcule return periods
+    # Calculate return periods
     return_periods = 1 / exceedance_probability / extremes_rate
 
     # Copy `extremes` to make the returned DataFrame independent from the original
     extremes = extremes.copy(deep=True)
 
     return pd.DataFrame(
         data={
```

### Comparing `pyextremes-2.3.0/src/pyextremes/extremes/transformation.py` & `pyextremes-2.3.1/src/pyextremes/extremes/transformation.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/models/distribution.py` & `pyextremes-2.3.1/src/pyextremes/models/distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,27 +24,27 @@
         extremes: pd.Series,
         distribution: typing.Union[str, scipy.stats.rv_continuous],
         **kwargs,
     ) -> None:
         """
         Distribution class compatible with pyextremes models.
 
-        It is a wrapper around the scipy.stats.rv_continous class and its subclasses.
+        It is a wrapper around the scipy.stats.rv_continuous class and its subclasses.
         https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_continuous.html
 
         Parameters
         ----------
         extremes : pandas.Series
             Time series of extreme events.
         distribution : str or scipy.stats.rv_continuous
             Distribution name compatible with scipy.stats
             or a subclass of scipy.stats.rv_continuous.
             See https://docs.scipy.org/doc/scipy/reference/stats.html
         kwargs
-            Special keyword arguments, passsed to the `.fit` method of the distribution.
+            Special keyword arguments, passed to the `.fit` method of the distribution.
             These keyword arguments represent parameters to be held fixed.
             Names of parameters to be fixed must have 'f' prefixes. Valid parameters:
                 - shape(s): 'fc', e.g. fc=0
                 - location: 'floc', e.g. floc=0
                 - scale: 'fscale', e.g. fscale=1
             By default, no parameters are fixed.
             See documentation of a specific scipy.stats distribution
@@ -134,15 +134,15 @@
         parameters : dict
             Dictionary with MLE of free distribution parameters.
 
         """
         # Calculate full MLE of distribution parameters
         full_mle = self.distribution.fit(data=data, **self.fixed_parameters)
 
-        # Package distribtuon parameters into ordered free distribution parameters
+        # Package distribution parameters into ordered free distribution parameters
         free_parameters = {}
         for i, parameter in enumerate(self.distribution_parameters):
             if parameter in self.free_parameters:
                 free_parameters[parameter] = full_mle[i]
             else:
                 assert np.isclose(full_mle[i], self._fixed_parameters[parameter])
         return free_parameters
@@ -377,15 +377,15 @@
         result : float or numpy.ndarray
             Calculated property value.
             If x is scalar:
                 output is scalar or 1D array
                 with length equal to number of `free_parameters` combinations
                     for 1D free_parameters=[1, 2] output is a scalar
                     for 2D free parameters=[[1, 2], [3, 4], [5, 6]]
-                        output is an array of length len(free_paramters)
+                        output is an array of length len(free_parameters)
             If x is a 1D array:
                 output is a 1D or 2D array
                     for 1D free_parameters=[1, 2] output is a 1D array of length len(x)
                     for 2D free_parameters=[[1, 2], [3, 4], ...]
                     output is a 2D array of shape (len(x), len(free_parameters)
 
         """
```

### Comparing `pyextremes-2.3.0/src/pyextremes/models/model_base.py` & `pyextremes-2.3.1/src/pyextremes/models/model_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         extremes : pandas.Series
             Time series of extreme events.
         distribution : str or scipy.stats.rv_continuous
             Distribution name compatible with scipy.stats
             or a subclass of scipy.stats.rv_continuous.
             See https://docs.scipy.org/doc/scipy/reference/stats.html
         distribution_kwargs : dict, optional
-            Special keyword arguments, passsed to the `.fit` method of the distribution.
+            Special keyword arguments, passed to the `.fit` method of the distribution.
             These keyword arguments represent parameters to be held fixed.
             Names of parameters to be fixed must have 'f' prefixes. Valid parameters:
                 - shape(s): 'fc', e.g. fc=0
                 - location: 'floc', e.g. floc=0
                 - scale: 'fscale', e.g. fscale=1
             By default, no parameters are fixed.
             See documentation of a specific scipy.stats distribution
```

### Comparing `pyextremes-2.3.0/src/pyextremes/models/model_emcee.py` & `pyextremes-2.3.1/src/pyextremes/models/model_emcee.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,18 @@
 
         # Calculate fit parameters as MAP of distribution parameters
         kernel = scipy.stats.gaussian_kde(np.vstack(self._trace).transpose())
 
         def kde_func(x):
             return -kernel(x)[0]
 
-        fit_paramters = self._trace.mean(axis=(0, 1))
+        fit_parameters = self._trace.mean(axis=(0, 1))
         solution = scipy.optimize.minimize(
             kde_func,
-            x0=fit_paramters,
+            x0=fit_parameters,
             method="Nelder-Mead",
         )
         if solution.success:
             fit_parameters = solution.x
         else:  # pragma: no cover
             warnings.warn(
                 message=(
```

### Comparing `pyextremes-2.3.0/src/pyextremes/models/model_mle.py` & `pyextremes-2.3.1/src/pyextremes/models/model_mle.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/models/models.py` & `pyextremes-2.3.1/src/pyextremes/models/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     extremes : pandas.Series
         Time series of extreme events.
     distribution : str or scipy.stats.rv_continuous
         Distribution name compatible with scipy.stats
         or a subclass of scipy.stats.rv_continuous.
         See https://docs.scipy.org/doc/scipy/reference/stats.html
     distribution_kwargs : dict, optional
-        Special keyword arguments, passsed to the `.fit` method of the distribution.
+        Special keyword arguments, passed to the `.fit` method of the distribution.
         These keyword arguments represent parameters to be held fixed.
         Names of parameters to be fixed must have 'f' prefixes. Valid parameters:
             - shape(s): 'fc', e.g. fc=0
             - location: 'floc', e.g. floc=0
             - scale: 'fscale', e.g. fscale=1
         By default, no parameters are fixed.
         See documentation of a specific scipy.stats distribution
```

### Comparing `pyextremes-2.3.0/src/pyextremes/plotting/extremes.py` & `pyextremes-2.3.1/src/pyextremes/plotting/extremes.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/plotting/mcmc.py` & `pyextremes-2.3.1/src/pyextremes/plotting/mcmc.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/plotting/probability_plots.py` & `pyextremes-2.3.1/src/pyextremes/plotting/probability_plots.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/plotting/return_values.py` & `pyextremes-2.3.1/src/pyextremes/plotting/return_values.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/plotting/style.py` & `pyextremes-2.3.1/src/pyextremes/plotting/style.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/tests/ks_test.py` & `pyextremes-2.3.1/src/pyextremes/tests/ks_test.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/tests/test_base.py` & `pyextremes-2.3.1/src/pyextremes/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/src/pyextremes/tuning/threshold_selection.py` & `pyextremes-2.3.1/src/pyextremes/tuning/threshold_selection.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.3.0/PKG-INFO` & `pyextremes-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyextremes
-Version: 2.3.0
+Version: 2.3.1
 Summary: Extreme Value Analysis (EVA) in Python
 Home-page: https://georgebv.github.io/pyextremes
 License: MIT
 Keywords: statistics,extreme,extreme value analysis,eva,coastal,ocean,marine,environmental,engineering
 Author: George Bocharov
 Author-email: bocharovgeorgii@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -13,16 +13,14 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Provides-Extra: full
 Requires-Dist: emcee (>=3.0.3,<4.0.0)
 Requires-Dist: matplotlib (>=3.3.0,<4.0.0)
 Requires-Dist: numpy (>=1.19.0,<2.0.0)
```

#### html2text {}

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 2.1 Name: pyextremes Version: 2.3.0 Summary: Extreme Value
+Metadata-Version: 2.1 Name: pyextremes Version: 2.3.1 Summary: Extreme Value
 Analysis (EVA) in Python Home-page: https://georgebv.github.io/pyextremes
 License: MIT Keywords: statistics,extreme,extreme value
 analysis,eva,coastal,ocean,marine,environmental,engineering Author: George
 Bocharov Author-email: bocharovgeorgii@gmail.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
-Scientific/Engineering :: Hydrology Classifier: Topic :: Scientific/Engineering
-:: Mathematics Provides-Extra: full Requires-Dist: emcee (>=3.0.3,<4.0.0)
-Requires-Dist: matplotlib (>=3.3.0,<4.0.0) Requires-Dist: numpy
-(>=1.19.0,<2.0.0) Requires-Dist: pandas (>=1.0.0,<3.0.0) Requires-Dist: scipy
-(>=1.5.0,<2.0.0) Requires-Dist: tqdm (>=4.0.0,<5.0.0) ; extra == "full"
-Project-URL: Repository, https://github.com/georgebv/pyextremes Description-
-Content-Type: text/markdown
+Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Hydrology Classifier: Topic :: Scientific/Engineering :: Mathematics Provides-
+Extra: full Requires-Dist: emcee (>=3.0.3,<4.0.0) Requires-Dist: matplotlib
+(>=3.3.0,<4.0.0) Requires-Dist: numpy (>=1.19.0,<2.0.0) Requires-Dist: pandas
+(>=1.0.0,<3.0.0) Requires-Dist: scipy (>=1.5.0,<2.0.0) Requires-Dist: tqdm
+(>=4.0.0,<5.0.0) ; extra == "full" Project-URL: Repository, https://github.com/
+georgebv/pyextremes Description-Content-Type: text/markdown
                                   pyextremes
                     Extreme Value Analysis (EVA) in Python
               [Test] [Coverage] [PyPI_Package] [Anaconda_Package]
 # About **Documentation:** https://georgebv.github.io/pyextremes/ **License:**
 [MIT](https://opensource.org/licenses/MIT) **Support:** [ask a question](https:
 //github.com/georgebv/pyextremes/discussions) or [create an issue](https://
 github.com/georgebv/pyextremes/issues/new/choose), any input is appreciated and
```

