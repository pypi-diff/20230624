# Comparing `tmp/mellon-1.3.0.tar.gz` & `tmp/mellon-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mellon-1.3.0.tar", last modified: Tue Jun 20 18:58:45 2023, max compression
+gzip compressed data, was "mellon-1.3.1.tar", last modified: Sat Jun 24 02:09:14 2023, max compression
```

## Comparing `mellon-1.3.0.tar` & `mellon-1.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-06-20 18:58:45.574584 mellon-1.3.0/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    35148 2022-09-23 00:29:04.000000 mellon-1.3.0/LICENSE
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2586 2023-06-20 18:58:45.573214 mellon-1.3.0/PKG-INFO
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2166 2023-05-17 21:27:55.000000 mellon-1.3.0/README.rst
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-06-20 18:58:45.552487 mellon-1.3.0/mellon/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      961 2023-06-20 18:33:48.000000 mellon-1.3.0/mellon/__init__.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      452 2023-06-17 22:03:44.000000 mellon-1.3.0/mellon/_conditional.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      290 2023-06-17 22:06:30.000000 mellon-1.3.0/mellon/_cov.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      196 2023-06-17 22:01:57.000000 mellon-1.3.0/mellon/_derivatives.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      898 2023-06-17 21:58:49.000000 mellon-1.3.0/mellon/_inference.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      711 2023-06-17 21:44:25.000000 mellon-1.3.0/mellon/_parameters.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      235 2023-06-17 21:48:14.000000 mellon-1.3.0/mellon/_util.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     8960 2023-06-17 21:51:01.000000 mellon-1.3.0/mellon/base_cov.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    12053 2023-06-16 02:26:14.000000 mellon-1.3.0/mellon/base_model.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    19174 2023-06-17 22:03:30.000000 mellon-1.3.0/mellon/base_predictor.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     3679 2023-06-16 05:31:47.000000 mellon-1.3.0/mellon/compute_ls_time.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     7453 2023-06-17 21:51:59.000000 mellon-1.3.0/mellon/conditional.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     9028 2023-06-17 21:50:46.000000 mellon-1.3.0/mellon/cov.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     9199 2023-06-16 02:26:11.000000 mellon-1.3.0/mellon/decomposition.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    17357 2023-06-16 02:26:11.000000 mellon-1.3.0/mellon/density_estimator.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     4360 2023-06-16 18:57:29.000000 mellon-1.3.0/mellon/derivatives.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    19510 2023-06-16 02:26:11.000000 mellon-1.3.0/mellon/dimensionality_estimator.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    13774 2023-06-16 02:26:11.000000 mellon-1.3.0/mellon/function_estimator.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    19432 2023-06-17 21:52:29.000000 mellon-1.3.0/mellon/inference.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      368 2023-06-16 02:26:11.000000 mellon-1.3.0/mellon/model.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    16164 2023-06-17 21:52:14.000000 mellon-1.3.0/mellon/parameters.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    24211 2023-06-17 07:12:35.000000 mellon-1.3.0/mellon/time_sensitive_density_estimator.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    12525 2023-06-17 21:52:36.000000 mellon-1.3.0/mellon/util.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     9661 2023-06-17 22:04:30.000000 mellon-1.3.0/mellon/validation.py
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-06-20 18:58:45.569512 mellon-1.3.0/mellon.egg-info/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2586 2023-06-20 18:58:45.000000 mellon-1.3.0/mellon.egg-info/PKG-INFO
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      716 2023-06-20 18:58:45.000000 mellon-1.3.0/mellon.egg-info/SOURCES.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)        1 2023-06-20 18:58:45.000000 mellon-1.3.0/mellon.egg-info/dependency_links.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)       24 2023-06-20 18:58:45.000000 mellon-1.3.0/mellon.egg-info/requires.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)        7 2023-06-20 18:58:45.000000 mellon-1.3.0/mellon.egg-info/top_level.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)       38 2023-06-20 18:58:45.575395 mellon-1.3.0/setup.cfg
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1100 2023-06-15 06:16:23.000000 mellon-1.3.0/setup.py
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-06-24 02:09:14.308592 mellon-1.3.1/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    35148 2022-09-23 00:29:04.000000 mellon-1.3.1/LICENSE
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2588 2023-06-24 02:09:14.307321 mellon-1.3.1/PKG-INFO
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2166 2023-05-17 21:27:55.000000 mellon-1.3.1/README.rst
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-06-24 02:09:14.286517 mellon-1.3.1/mellon/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      961 2023-06-24 02:07:23.000000 mellon-1.3.1/mellon/__init__.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      452 2023-06-17 22:03:44.000000 mellon-1.3.1/mellon/_conditional.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      290 2023-06-17 22:06:30.000000 mellon-1.3.1/mellon/_cov.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      196 2023-06-17 22:01:57.000000 mellon-1.3.1/mellon/_derivatives.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      898 2023-06-17 21:58:49.000000 mellon-1.3.1/mellon/_inference.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      711 2023-06-17 21:44:25.000000 mellon-1.3.1/mellon/_parameters.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      235 2023-06-17 21:48:14.000000 mellon-1.3.1/mellon/_util.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     9092 2023-06-23 23:23:27.000000 mellon-1.3.1/mellon/base_cov.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    12053 2023-06-16 02:26:14.000000 mellon-1.3.1/mellon/base_model.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    19422 2023-06-23 23:23:27.000000 mellon-1.3.1/mellon/base_predictor.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     3679 2023-06-16 05:31:47.000000 mellon-1.3.1/mellon/compute_ls_time.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     7253 2023-06-23 23:23:27.000000 mellon-1.3.1/mellon/conditional.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     9028 2023-06-17 21:50:46.000000 mellon-1.3.1/mellon/cov.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     9199 2023-06-16 02:26:11.000000 mellon-1.3.1/mellon/decomposition.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    17357 2023-06-16 02:26:11.000000 mellon-1.3.1/mellon/density_estimator.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     4360 2023-06-16 18:57:29.000000 mellon-1.3.1/mellon/derivatives.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    19510 2023-06-16 02:26:11.000000 mellon-1.3.1/mellon/dimensionality_estimator.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    13774 2023-06-16 02:26:11.000000 mellon-1.3.1/mellon/function_estimator.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    19432 2023-06-17 21:52:29.000000 mellon-1.3.1/mellon/inference.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      368 2023-06-16 02:26:11.000000 mellon-1.3.1/mellon/model.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    16164 2023-06-17 21:52:14.000000 mellon-1.3.1/mellon/parameters.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    24211 2023-06-17 07:12:35.000000 mellon-1.3.1/mellon/time_sensitive_density_estimator.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    12944 2023-06-23 23:23:27.000000 mellon-1.3.1/mellon/util.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    10151 2023-06-23 23:23:27.000000 mellon-1.3.1/mellon/validation.py
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-06-24 02:09:14.303357 mellon-1.3.1/mellon.egg-info/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2588 2023-06-24 02:09:14.000000 mellon-1.3.1/mellon.egg-info/PKG-INFO
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      716 2023-06-24 02:09:14.000000 mellon-1.3.1/mellon.egg-info/SOURCES.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)        1 2023-06-24 02:09:14.000000 mellon-1.3.1/mellon.egg-info/dependency_links.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)       24 2023-06-24 02:09:14.000000 mellon-1.3.1/mellon.egg-info/requires.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)        7 2023-06-24 02:09:14.000000 mellon-1.3.1/mellon.egg-info/top_level.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)       38 2023-06-24 02:09:14.309585 mellon-1.3.1/setup.cfg
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1102 2023-06-21 01:32:34.000000 mellon-1.3.1/setup.py
```

### Comparing `mellon-1.3.0/LICENSE` & `mellon-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/PKG-INFO` & `mellon-1.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mellon
-Version: 1.3.0
+Version: 1.3.1
 Summary: Non-parametric density estimator.
 Home-page: https://github.com/settylab/mellon
 Author: Setty Lab
-Author-email: msetty@fredhutch.org
+Author-email: dominik.otto@gmail.com
 License: GNU General Public License v3.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Mellon
```

### Comparing `mellon-1.3.0/README.rst` & `mellon-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/__init__.py` & `mellon-1.3.1/mellon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from . import _util as util
 from . import _cov as cov
 from . import _parameters as parameters
 from . import _inference as inference
 from . import _conditional as conditional
 from . import _derivatives as derivatives
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 __all__ = [
     "DensityEstimator",
     "FunctionEstimator",
     "DimensionalityEstimator",
     "TimeSensitiveDensityEstimator",
     "Predictor",
```

### Comparing `mellon-1.3.0/mellon/_inference.py` & `mellon-1.3.1/mellon/_inference.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/_parameters.py` & `mellon-1.3.1/mellon/_parameters.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/base_cov.py` & `mellon-1.3.1/mellon/base_cov.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,18 @@
             )
         elif module_name.split(".")[0] != MELLON_NAME:
             logger.warning(
                 f'The covariance function "{clsname}" is not part of {MELLON_NAME} '
                 f'but of the module "{module_name}". Make sure the module '
                 "is available for deserialization."
             )
+        metamodule = import_module(module_name.split(".")[0])
         module = import_module(module_name)
-        version = getattr(module, "__version__", "NA")
+        metaversion = getattr(metamodule, "__version__", "NA")
+        version = getattr(module, "__version__", metaversion)
         state = {
             "type": "mellon.Covariance",
             "data": self._data_dict(),
             "metadata": {
                 "classname": clsname,
                 "module_name": module_name,
                 "module_version": version,
```

### Comparing `mellon-1.3.0/mellon/base_model.py` & `mellon-1.3.1/mellon/base_model.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/base_predictor.py` & `mellon-1.3.1/mellon/base_predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 
 import gzip
 import bz2
 
 import json
 
 from .base_cov import Covariance
-from .util import Log, deserialize, ensure_2d, make_multi_time_argument
+from .util import (
+    Log,
+    make_serializable,
+    deserialize,
+    ensure_2d,
+    make_multi_time_argument,
+)
 from .derivatives import (
     gradient,
     hessian,
     hessian_log_determinant,
 )
 from .validation import _validate_time_x, _validate_float, _validate_array
 
@@ -113,15 +119,15 @@
                 "Please ensure that the input data has the same number of features as the training data."
             )
         return self._predict(x)
 
     @abstractmethod
     def _data_dict(self):
         """Return a dictionary containing the predictor's state data.
-        All arrays nee to be numpy arrays for serialization.
+        All arrays nee to be (jax) numpy arrays for serialization.
 
         This method must be implemented by subclasses. It should return a
         dictionary where each key-value pair corresponds to an attribute of
         the predictor and its current state.
 
         :return: A dictionary containing the predictor's state data.
         :rtype: dict
@@ -185,18 +191,21 @@
         returns a dictionary that represents the current state of the
         predictor.
 
         :return: A dictionary representing the state of the predictor.
         :rtype: dict
         """
         module_name = self.__class__.__module__
+        metamodule = import_module(module_name.split(".")[0])
         module = import_module(module_name)
-        version = getattr(module, "__version__", "NA")
+        metaversion = getattr(metamodule, "__version__", "NA")
+        version = getattr(module, "__version__", metaversion)
         data = self._data_dict()
         data.update({"n_input_features": self.n_input_features})
+        data = {k: make_serializable(v) for k, v in data.items()}
 
         state = {
             "data": data,
             "cov_func": self.cov_func.__getstate__(),
             "metadata": {
                 "classname": self.__class__.__name__,
                 "module_name": module_name,
@@ -310,37 +319,37 @@
         This method deserializes the predictor from a python dictionary.
 
         :param data_dict: The dictionary from which to deserialize the predictor.
         :type data_dict: dict
         :return: An instance of the predictor.
         :rtype: Predictor subclass instance
         """
-        return cls.from_json_str(json.dumps(data_dict))
+        clsname = data_dict["metadata"]["classname"]
+        module_name = data_dict["metadata"]["module_name"]
+
+        module = import_module(module_name)
+        Subclass = getattr(module, clsname)
+        instance = Subclass.__new__(Subclass)
+        instance.__setstate__(data_dict)
+
+        return instance
 
     @classmethod
     def from_json_str(cls, json_str):
         """Deserialize the predictor from a JSON string.
 
         This method deserializes the predictor from the content of a JSON file.
 
         :param json_str: The JSON string from which to deserialize the predictor.
         :type json_str: str
         :return: An instance of the predictor.
         :rtype: Predictor subclass instance
         """
-        state = json.loads(json_str)
-        clsname = state["metadata"]["classname"]
-        module_name = state["metadata"]["module_name"]
-
-        module = import_module(module_name)
-        Subclass = getattr(module, clsname)
-        instance = Subclass.__new__(Subclass)
-        instance.__setstate__(state)
-
-        return instance
+        data_dict = json.loads(json_str)
+        return cls.from_dict(data_dict)
 
 
 class PredictorTime(Predictor):
     """
     Abstract base class for predictor models with a time covariate.
 
     An instance `predictor` of a subclass of `PredictorTime` can be used to
```

### Comparing `mellon-1.3.0/mellon/compute_ls_time.py` & `mellon-1.3.1/mellon/compute_ls_time.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/conditional.py` & `mellon-1.3.1/mellon/conditional.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from jax.numpy import dot, square, isnan, any
 from jax.numpy.linalg import cholesky
 from jax.scipy.linalg import solve_triangular
-from .util import ensure_2d, make_serializable, stabilize, DEFAULT_JITTER, Log
+from .util import ensure_2d, stabilize, DEFAULT_JITTER, Log
 from .base_predictor import Predictor, PredictorTime
 
 
 logger = Log()
 
 
 class _FullConditionalMean:
@@ -55,17 +55,17 @@
         self.x = x
         self.weights = weights
         self.mu = mu
         self.n_input_features = x.shape[1]
 
     def _data_dict(self):
         return {
-            "x": make_serializable(self.x),
-            "weights": make_serializable(self.weights),
-            "mu": make_serializable(self.mu),
+            "x": self.x,
+            "weights": self.weights,
+            "mu": self.mu,
         }
 
     def _predict(self, Xnew):
         cov_func = self.cov_func
         x = self.x
         weights = self.weights
         mu = self.mu
@@ -139,17 +139,17 @@
         self.landmarks = xu
         self.weights = weights
         self.mu = mu
         self.n_input_features = xu.shape[1]
 
     def _data_dict(self):
         return {
-            "landmarks": make_serializable(self.landmarks),
-            "weights": make_serializable(self.weights),
-            "mu": make_serializable(self.mu),
+            "landmarks": self.landmarks,
+            "weights": self.weights,
+            "mu": self.mu,
         }
 
     def _predict(self, Xnew):
         cov_func = self.cov_func
         xu = self.landmarks
         weights = self.weights
         mu = self.mu
@@ -213,32 +213,30 @@
         self.landmarks = xu
         self.weights = weights
         self.mu = mu
         self.n_input_features = xu.shape[1]
 
     def _data_dict(self):
         return {
-            "landmarks": make_serializable(self.landmarks),
-            "weights": make_serializable(self.weights),
-            "mu": make_serializable(self.mu),
+            "landmarks": self.landmarks,
+            "weights": self.weights,
+            "mu": self.mu,
         }
 
     def _predict(self, Xnew):
         cov_func = self.cov_func
         xu = self.landmarks
         weights = self.weights
         mu = self.mu
 
         Kus = cov_func(Xnew, xu)
         return mu + dot(Kus, weights)
 
 
-class LandmarksConditionalMeanCholesky(
-    _LandmarksConditionalMeanCholesky, PredictorTime
-):
+class LandmarksConditionalMeanCholesky(_LandmarksConditionalMeanCholesky, Predictor):
     pass
 
 
 class LandmarksConditionalMeanCholeskyTime(
     _LandmarksConditionalMeanCholesky, PredictorTime
 ):
     pass
```

### Comparing `mellon-1.3.0/mellon/cov.py` & `mellon-1.3.1/mellon/cov.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/decomposition.py` & `mellon-1.3.1/mellon/decomposition.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/density_estimator.py` & `mellon-1.3.1/mellon/density_estimator.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/derivatives.py` & `mellon-1.3.1/mellon/derivatives.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/dimensionality_estimator.py` & `mellon-1.3.1/mellon/dimensionality_estimator.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/function_estimator.py` & `mellon-1.3.1/mellon/function_estimator.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/inference.py` & `mellon-1.3.1/mellon/inference.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/parameters.py` & `mellon-1.3.1/mellon/parameters.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/time_sensitive_density_estimator.py` & `mellon-1.3.1/mellon/time_sensitive_density_estimator.py`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/mellon/util.py` & `mellon-1.3.1/mellon/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     concatenate,
     atleast_2d,
     ndarray,
     array,
     isscalar,
     exp,
 )
+from numpy import integer, floating
 from jax.numpy import sum as arraysum
 from jax.numpy.linalg import norm, lstsq, matrix_rank
 from jax.scipy.special import gammaln
 from jax import vmap, jit
 from sklearn.neighbors import BallTree, KDTree
 
 from .validation import _validate_array
@@ -44,14 +45,20 @@
 
     def new_func(x):
         return exp(func(x))
 
     return new_func
 
 
+def _None_to_str(v):
+    if v is None:
+        return "None"
+    return v
+
+
 def make_serializable(x):
     """
     Convert the input into a serializable format.
 
     Parameters
     ----------
     x : variable
@@ -60,20 +67,31 @@
     Returns
     -------
     serializable_x : variable
         The input variable converted into a serializable format.
     """
     if isinstance(x, ndarray):
         return {"type": "jax.numpy", "data": x.tolist()}
+    if isinstance(x, integer):
+        return int(x)
+    if isinstance(x, floating):
+        return float(x)
     elif isinstance(x, slice):
-        return {"type": "slice", "data": (x.start, x.stop, x.step)}
+        dat = [_None_to_str(v) for v in (x.start, x.stop, x.step)]
+        return {"type": "slice", "data": dat}
     elif isinstance(x, dict):
         return {"type": "dict", "data": {k: make_serializable(v) for k, v in x.items()}}
     else:
-        return x
+        return _None_to_str(x)
+
+
+def _str_to_None(v):
+    if v == "None":
+        return None
+    return v
 
 
 def deserialize(serializable_x):
     """
     Convert the serializable input back into the original format.
 
     Parameters
@@ -87,19 +105,20 @@
         The input variable converted back into its original format.
     """
     if isinstance(serializable_x, dict):
         data_type = serializable_x["type"]
         if data_type == "jax.numpy":
             return array(serializable_x["data"])
         elif data_type == "slice":
-            return slice(*serializable_x["data"])
+            dat = [_str_to_None(v) for v in serializable_x["data"]]
+            return slice(*dat)
         elif data_type == "dict":
             return {k: deserialize(v) for k, v in serializable_x["data"].items()}
     else:
-        return serializable_x
+        return _str_to_None(serializable_x)
 
 
 def ensure_2d(X):
     """
     Ensures that the input JAX array, X, is at least 2-dimensional.
 
     :param X: The input JAX array to be made 2-dimensional.
```

### Comparing `mellon-1.3.0/mellon/validation.py` & `mellon-1.3.1/mellon/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,26 +85,37 @@
     return x
 
 
 def _validate_float_or_int(value, param_name, optional=False):
     if value is None and optional:
         return None
 
-    if not isinstance(value, (float, int)):
-        raise ValueError(f"'{param_name}' should be a positive integer or float number")
-    return value
+    if isinstance(value, (float, int)):
+        return value
+    try:
+        return float(value)
+    except TypeError:
+        its_type = type(value)
+        raise ValueError(
+            f"'{param_name}' should be a positive integer or float number but is {its_type}"
+        )
 
 
 def _validate_positive_float(value, param_name, optional=False):
     if value is None and optional:
         return None
 
-    if not isinstance(value, (float, int)) or value < 0:
+    try:
+        value = float(value)
+    except TypeError:
+        its_type = type(value)
+        raise ValueError(f"'{param_name}' should be a float number but is {its_type}")
+    if value < 0:
         raise ValueError(f"'{param_name}' should be a positive float number")
-    return float(value)
+    return value
 
 
 def _validate_float(value, param_name, optional=False):
     """
     Validates if the input is a float or can be converted to a float.
 
     Parameters
@@ -139,18 +150,21 @@
     if isinstance(value, ndarray) and value.size == 1:
         try:
             value = value.item()
         except ConcretizationTypeError:
             # this must be a JAX tracer
             return value
 
-    if not isinstance(value, (float, int)):
-        raise ValueError(f"'{param_name}' should be a float number")
-
-    return float(value)
+    if isinstance(value, (float, int)):
+        return value
+    try:
+        return float(value)
+    except TypeError:
+        its_type = type(value)
+        raise ValueError(f"'{param_name}' should be a float number but is {its_type}")
 
 
 def _validate_positive_int(value, param_name, optional=False):
     if optional and value is None:
         return None
     if not isinstance(value, int) or value < 0:
         raise ValueError(f"'{param_name}' should be a positive integer number")
@@ -195,18 +209,22 @@
 
     if iterable is None:
         if optional:
             return None
         else:
             raise TypeError(f"'{name}' can't be None.")
 
-    if isinstance(iterable, Iterable):
+    if hasattr(iterable, "todense"):
+        array = asarray(iterable.todense(), dtype=float)
+    elif isinstance(iterable, Iterable):
         array = asarray(iterable, dtype=float)
     else:
-        raise TypeError(f"'{name}' should be iterable, got {type(iterable)} instead.")
+        raise TypeError(
+            f"'{name}' should be iterable or sparse, got {type(iterable)} instead."
+        )
 
     if ndim is not None:
         if isinstance(ndim, int):
             ndim = (ndim,)
         if array.ndim not in ndim:
             raise ValueError(
                 f"'{name}' must be a {ndim}-dimensional array, got {array.ndim}-dimensional array instead."
```

### Comparing `mellon-1.3.0/mellon.egg-info/PKG-INFO` & `mellon-1.3.1/mellon.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mellon
-Version: 1.3.0
+Version: 1.3.1
 Summary: Non-parametric density estimator.
 Home-page: https://github.com/settylab/mellon
 Author: Setty Lab
-Author-email: msetty@fredhutch.org
+Author-email: dominik.otto@gmail.com
 License: GNU General Public License v3.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Mellon
```

### Comparing `mellon-1.3.0/mellon.egg-info/SOURCES.txt` & `mellon-1.3.1/mellon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mellon-1.3.0/setup.py` & `mellon-1.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 setup(
     name="mellon",
     version=get_version("mellon/__init__.py"),
     description="Non-parametric density estimator.",
     url="https://github.com/settylab/mellon",
     author="Setty Lab",
-    author_email="msetty@fredhutch.org",
+    author_email="dominik.otto@gmail.com",
     license="GNU General Public License v3.0",
     packages=["mellon"],
     install_requires=[
         "jax",
         "jaxopt",
         "scikit-learn",
     ],
```

