# Comparing `tmp/eulerpi-0.3.1.tar.gz` & `tmp/eulerpi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulerpi-0.3.1.tar", max compression
+gzip compressed data, was "eulerpi-0.4.0.tar", max compression
```

## Comparing `eulerpi-0.3.1.tar` & `eulerpi-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0     1117 2023-05-03 13:37:52.817343 eulerpi-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     4704 2023-05-03 13:37:52.817343 eulerpi-0.3.1/README.md
--rw-r--r--   0        0        0      564 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/__init__.py
--rw-r--r--   0        0        0      191 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/__init__.py
--rw-r--r--   0        0        0     7531 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/data_transformation.py
--rw-r--r--   0        0        0      362 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/data_transformation_types.py
--rw-r--r--   0        0        0    11433 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/dense_grid.py
--rw-r--r--   0        0        0      355 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/dense_grid_types.py
--rw-r--r--   0        0        0     6790 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/inference.py
--rw-r--r--   0        0        0      514 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/inference_types.py
--rw-r--r--   0        0        0     3684 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/kde.py
--rw-r--r--   0        0        0    15896 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/model.py
--rw-r--r--   0        0        0    18493 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/result_manager.py
--rw-r--r--   0        0        0    15655 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/sampling.py
--rw-r--r--   0        0        0    21145 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/sparsegrid.py
--rw-r--r--   0        0        0     7006 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/transformations.py
--rw-r--r--   0        0        0    14800 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/corona/CoronaData.csv
--rw-r--r--   0        0        0       94 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/corona/__init__.py
--rw-r--r--   0        0        0     2767 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/corona/corona.py
--rw-r--r--   0        0        0     1295 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/CMakeLists.txt
--rw-r--r--   0        0        0        0 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/__init__.py
--rw-r--r--   0        0        0     2214 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/cpp_model.hpp
--rw-r--r--   0        0        0     1191 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/cpp_plant.py
--rw-r--r--   0        0        0     2559 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/python_reference_plants.py
--rw-r--r--   0        0        0      357 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/wrapper.cpp
--rw-r--r--   0        0        0     1811 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
--rw-r--r--   0        0        0     1133 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/sbml/sbml_caffeine_model.py
--rw-r--r--   0        0        0     1859 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/sbml/sbml_menten_model.py
--rw-r--r--   0        0        0     5493 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/sbml/sbml_menten_model.xml
--rw-r--r--   0        0        0     2241 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/simple_models.py
--rw-r--r--   0        0        0   189602 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/stock/ETF.csv
--rw-r--r--   0        0        0      268 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/stock/ETF50.csv
--rw-r--r--   0        0        0       88 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/stock/__init__.py
--rw-r--r--   0        0        0     5556 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/examples/stock/stock.py
--rw-r--r--   0        0        0     5877 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/examples/temperature/TemperatureArtificialParams.csv
--rw-r--r--   0        0        0     5046 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/examples/temperature/TemperatureData.csv
--rw-r--r--   0        0        0      215 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/examples/temperature/__init__.py
--rw-r--r--   0        0        0     2136 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/examples/temperature/temperature.py
--rw-r--r--   0        0        0     2169 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/jax_extension.py
--rw-r--r--   0        0        0     2340 2023-05-03 13:37:52.829343 eulerpi-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6173 1970-01-01 00:00:00.000000 eulerpi-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-06-24 19:44:36.673968 eulerpi-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     4828 2023-06-24 19:44:36.673968 eulerpi-0.4.0/README.md
+-rw-r--r--   0        0        0      564 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/__init__.py
+-rw-r--r--   0        0        0     7531 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/data_transformation.py
+-rw-r--r--   0        0        0      362 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/data_transformation_types.py
+-rw-r--r--   0        0        0    11548 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/dense_grid.py
+-rw-r--r--   0        0        0      355 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/dense_grid_types.py
+-rw-r--r--   0        0        0     6790 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/inference.py
+-rw-r--r--   0        0        0      514 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/inference_types.py
+-rw-r--r--   0        0        0     3684 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/kde.py
+-rw-r--r--   0        0        0    16765 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/model.py
+-rw-r--r--   0        0        0    18493 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/result_manager.py
+-rw-r--r--   0        0        0    15655 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/sampling.py
+-rw-r--r--   0        0        0    21145 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/sparsegrid.py
+-rw-r--r--   0        0        0     7581 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/core/transformations.py
+-rw-r--r--   0        0        0    14800 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/corona/CoronaData.csv
+-rw-r--r--   0        0        0       94 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/corona/__init__.py
+-rw-r--r--   0        0        0     2560 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/corona/corona.py
+-rw-r--r--   0        0        0     1295 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/__init__.py
+-rw-r--r--   0        0        0     2214 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/cpp_model.hpp
+-rw-r--r--   0        0        0     1191 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/cpp_plant.py
+-rw-r--r--   0        0        0     2559 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/python_reference_plants.py
+-rw-r--r--   0        0        0      357 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/cpp/wrapper.cpp
+-rw-r--r--   0        0        0       82 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/heat/__init__.py
+-rw-r--r--   0        0        0     9613 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/heat/heat.py
+-rw-r--r--   0        0        0     1811 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
+-rw-r--r--   0        0        0     1133 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/sbml/sbml_caffeine_model.py
+-rw-r--r--   0        0        0     1859 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/sbml/sbml_menten_model.py
+-rw-r--r--   0        0        0     5493 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/sbml/sbml_menten_model.xml
+-rw-r--r--   0        0        0     2241 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/simple_models.py
+-rw-r--r--   0        0        0   189602 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/stock/ETF.csv
+-rw-r--r--   0        0        0      268 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/stock/ETF50.csv
+-rw-r--r--   0        0        0       88 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/stock/__init__.py
+-rw-r--r--   0        0        0     5556 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/stock/stock.py
+-rw-r--r--   0        0        0     5877 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv
+-rw-r--r--   0        0        0     5046 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/temperature/TemperatureData.csv
+-rw-r--r--   0        0        0      215 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/temperature/__init__.py
+-rw-r--r--   0        0        0     2136 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/examples/temperature/temperature.py
+-rw-r--r--   0        0        0     2169 2023-06-24 19:44:36.681968 eulerpi-0.4.0/eulerpi/jax_extension.py
+-rw-r--r--   0        0        0     2340 2023-06-24 19:44:36.685968 eulerpi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6249 1970-01-01 00:00:00.000000 eulerpi-0.4.0/PKG-INFO
```

### Comparing `eulerpi-0.3.1/LICENSE.md` & `eulerpi-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/README.md` & `eulerpi-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 
 [![flake8](https://img.shields.io/badge/flake8-checked-blue.svg)](https://flake8.pycqa.org/)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE.md)
 [![Python](https://img.shields.io/badge/python-3.10-purple.svg)](https://www.python.org/)
 ![PyPI](https://img.shields.io/pypi/v/eulerpi)
 
-Euler Parameter Inference (EPI) is a Python package for inverse parameter inference. It provides an implementation of the EPI algorithm, which takes observed data and a model as input and returns a parameter distribution consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
+Eulerian Parameter Inference (EPI) is a powerful and novel method for inverse model parameter inference. The eulerpi package provides an implementation of the EPI algorithm, which takes observed data and a model as input and returns a parameter distribution consistent with the observed data by solving the inverse problem directly. In case the model describes a one-to-one mapping between parameters and simulation results, the inferred parameter distribution is the true underlying distribution.
 
 ## Documentation
 
-The full documentation to this software, including a detailed tutorial on how to use EPI and the api documentation, can be found under [Documentation](https://Systems-Theory-in-Systems-Biology.github.io/EPI/).
+The full documentation of this software, including a detailed tutorial on how to use EPI and the api documentation, can be found under [Documentation](https://Systems-Theory-in-Systems-Biology.github.io/EPI/).
 
 ## Features
 
 EPI supports
 
 - SBML ode models
 - User provided models
-- Models with automatic differentation using jax
+- Models with automatic differentiation using jax
 
 ## Installation
 
 The package is available on pypi and can be installed with:
 
 ```bash
 pip install eulerpi
```

### Comparing `eulerpi-0.3.1/eulerpi/__init__.py` & `eulerpi-0.4.0/eulerpi/__init__.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/core/data_transformation.py` & `eulerpi-0.4.0/eulerpi/core/data_transformation.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/core/dense_grid.py` & `eulerpi-0.4.0/eulerpi/core/dense_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 from eulerpi.core.model import Model
 from eulerpi.core.result_manager import ResultManager
 from eulerpi.core.sampling import calc_kernel_width
 from eulerpi.core.transformations import evaluate_density
 
 
 def generate_chebyshev_grid(
-    num_grid_points: np.ndarray, limits: np.ndarray, flatten=False
+    num_grid_points: np.ndarray,
+    limits: np.ndarray,
+    flatten=False,
 ) -> Union[np.ndarray, list[np.ndarray]]:
     """Generate a grid with the given number of grid points for each dimension.
 
     Args:
         num_grid_points(np.ndarray): The number of grid points for each dimension.
         limits(np.ndarray): The limits for each dimension.
         flatten(bool): If True, the grid is returned as a flatten array. If False, the grid is returned as a list of arrays, one for each dimension. (Default value = False)
@@ -39,15 +41,17 @@
     if flatten:
         return np.array(mesh).reshape(ndim, -1).T
     else:
         return mesh
 
 
 def generate_regular_grid(
-    num_grid_points: np.ndarray, limits: np.ndarray, flatten=False
+    num_grid_points: np.ndarray,
+    limits: np.ndarray,
+    flatten=False,
 ) -> Union[np.ndarray, list[np.ndarray]]:
     """Generate a grid with the given number of grid points for each dimension.
 
     Args:
         num_grid_points(np.ndarray): The number of grid points for each dimension.
         limits(np.ndarray): The limits for each dimension.
         flatten(bool): If True, the grid is returned as a flatten array. If False, the grid is returned as a list of arrays, one for each dimension. (Default value = False)
@@ -142,24 +146,27 @@
 
     """
 
     if slice.shape[0] != num_grid_points.shape[0]:
         raise ValueError(
             f"The dimension of the numbers of grid points {num_grid_points} does not match the number of parameters in the slice {slice}"
         )
-    limits = model.param_limits
-    data_stdevs = calc_kernel_width(data)
+    if model.param_limits.ndim == 1:
+        limits = model.param_limits
+    else:
+        limits = model.param_limits[slice, :]
 
     if dense_grid_type == DenseGridType.CHEBYSHEV:
         grid = generate_chebyshev_grid(num_grid_points, limits, flatten=True)
     elif dense_grid_type == DenseGridType.EQUIDISTANT:
         grid = generate_regular_grid(num_grid_points, limits, flatten=True)
     else:
         raise ValueError(f"Unknown grid type: {dense_grid_type}")
 
+    data_stdevs = calc_kernel_width(data)
     # Split the grid into chunks that can be evaluated by each process
     grid_chunks = np.array_split(
         grid, num_processes * load_balancing_safety_faktor
     )
 
     pool = get_context("spawn").Pool(processes=num_processes)
     tasks = zip(
```

### Comparing `eulerpi-0.3.1/eulerpi/core/inference.py` & `eulerpi-0.4.0/eulerpi/core/inference.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/core/inference_types.py` & `eulerpi-0.4.0/eulerpi/core/inference_types.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/core/kde.py` & `eulerpi-0.4.0/eulerpi/core/kde.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/core/model.py` & `eulerpi-0.4.0/eulerpi/core/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class Model(ABC):
     """The base class for all models using the EPI algorithm.
 
     Args:
         central_param(np.ndarray): The central parameter for the model. (Default value = None)
-        param_limits(np.ndarray): The limits for the parameters. The limits are given as a 2D array with shape (param_dim, 2). (Default value = None)
+        param_limits(np.ndarray): Box limits for the parameters. The limits are given as a 2D array with shape (param_dim, 2). The parameter limits are used as limits as well as for the movement policy for MCMC sampling, and as boundaries for the grid when using grid-based inference. Overwrite the function param_is_within_domain if the domain is more complex than a box - the grid will still be build based on param_limits, but actual model evaluations only take place within the limits specified in param_is_within_domain. (Default value = None)
         name(str): The name of the model. The class name is used if no name is given. (Default value = None)
     """
 
     param_dim: Optional[
         np.ndarray
     ] = None  #: The dimension of the parameter space of the model. It must be defined in the subclass.
     data_dim: Optional[
@@ -92,14 +92,27 @@
         Returns:
             typing.Tuple[np.ndarray, np.ndarray]: The data generated from the parameter and the jacobian for the variables returned by the :func:`~eulerpi.core.model.Model.forward` method with respect to the parameters.
 
         """
 
         return self.forward(param), self.jacobian(param)
 
+    def param_is_within_domain(self, param: np.ndarray) -> bool:
+        """Checks whether a parameter is within the parameter domain of the model.
+        Overwrite this function if your model has a more complex parameter domain than a box. The param_limits are checked automatically.
+
+        Args:
+            param(np.ndarray): The parameter to check.
+
+        Returns:
+            bool: True if the parameter is within the limits.
+
+        """
+        return True
+
     def is_artificial(self) -> bool:
         """Determines whether the model provides artificial parameter and data sets.
 
         Returns:
             bool: True if the model inherits from the ArtificialModelInterface
 
         """
```

### Comparing `eulerpi-0.3.1/eulerpi/core/result_manager.py` & `eulerpi-0.4.0/eulerpi/core/result_manager.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/core/sampling.py` & `eulerpi-0.4.0/eulerpi/core/sampling.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/core/sparsegrid.py` & `eulerpi-0.4.0/eulerpi/core/sparsegrid.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/core/transformations.py` & `eulerpi-0.4.0/eulerpi/core/transformations.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,24 +37,37 @@
     limits = model.param_limits
 
     # Build the full parameter vector for evaluation based on the passed param slice and the constant central points
     fullParam = model.central_param
     fullParam[slice] = param
 
     # Check if the tried parameter is within the just-defined bounds and return the lowest possible density if not.
-    if np.any((param < limits[slice, 0]) | (param > limits[slice, 1])):
+    if (
+        np.any(param < model.param_limits[slice, 0])
+        or np.any(param > model.param_limits[slice, 1])
+        or not model.param_is_within_domain(fullParam)
+    ):
         logger.info(
             "Parameters outside of predefined range"
         )  # Slows down the sampling to much? -> Change logger level to warning or even error
         return 0, np.zeros(slice.shape[0] + model.data_dim + 1)
 
     # If the parameter is within the valid ranges...
     else:
-        # Evaluating the model and the jacobian for the specified parameter simultaneously provide a little speedup over calculating it separately in some cases.
-        sim_res, model_jac = model.forward_and_jacobian(fullParam)
+        # Try evaluating the model for the given parameters. Evaluating the model and the jacobian for the specified parameter simultaneously provide a little speedup over calculating it separately in some cases.
+        try:
+            sim_res, model_jac = model.forward_and_jacobian(fullParam)
+        except Exception as e:
+            logger.error(
+                "Error while evaluating model and its jacobian."
+                "The program will continue, but the density will be set to 0."
+                f"The parameter that caused the error is: {fullParam}"
+                f"The error message is: {e}"
+            )
+            return 0, np.zeros(slice.shape[0] + model.data_dim + 1)
 
         # normalize sim_res
         transformed_sim_res = data_transformation.transform(sim_res)
 
         # Evaluate the data density in the simulation result.
         densityEvaluation = eval_kde_gauss(
             data, transformed_sim_res, data_stdevs
```

### Comparing `eulerpi-0.3.1/eulerpi/examples/corona/CoronaData.csv` & `eulerpi-0.4.0/eulerpi/examples/corona/CoronaData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/corona/corona.py` & `eulerpi-0.4.0/eulerpi/examples/corona/corona.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,20 +22,14 @@
         central_param: np.ndarray = CENTRAL_PARAM,
         param_limits: np.ndarray = PARAM_LIMITS,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
         super().__init__(central_param, param_limits, name=name, **kwargs)
 
-    def get_data_bounds(self):
-        return np.array([[0.0, 4.0], [0.0, 40.0], [0.0, 80.0], [0.0, 3.5]])
-
-    def get_param_bounds(self):
-        return np.array([[-3.5, -0.5], [-1.0, 2.0], [-1.0, 2.0]])
-
     @classmethod
     def forward(cls, log_param):
         param = jnp.power(10, log_param)
         xInit = jnp.array([999.0, 0.0, 1.0, 0.0])
 
         def rhs(t, x, param):
             return jnp.array(
```

### Comparing `eulerpi-0.3.1/eulerpi/examples/cpp/CMakeLists.txt` & `eulerpi-0.4.0/eulerpi/examples/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/cpp/cpp_model.hpp` & `eulerpi-0.4.0/eulerpi/examples/cpp/cpp_model.hpp`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/cpp/cpp_plant.py` & `eulerpi-0.4.0/eulerpi/examples/cpp/cpp_plant.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/cpp/python_reference_plants.py` & `eulerpi-0.4.0/eulerpi/examples/cpp/python_reference_plants.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml` & `eulerpi-0.4.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/sbml/sbml_caffeine_model.py` & `eulerpi-0.4.0/eulerpi/examples/sbml/sbml_caffeine_model.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/sbml/sbml_menten_model.py` & `eulerpi-0.4.0/eulerpi/examples/sbml/sbml_menten_model.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/sbml/sbml_menten_model.xml` & `eulerpi-0.4.0/eulerpi/examples/sbml/sbml_menten_model.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/simple_models.py` & `eulerpi-0.4.0/eulerpi/examples/simple_models.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/stock/ETF.csv` & `eulerpi-0.4.0/eulerpi/examples/stock/ETF.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/stock/stock.py` & `eulerpi-0.4.0/eulerpi/examples/stock/stock.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/temperature/TemperatureArtificialParams.csv` & `eulerpi-0.4.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/temperature/TemperatureData.csv` & `eulerpi-0.4.0/eulerpi/examples/temperature/TemperatureData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/examples/temperature/temperature.py` & `eulerpi-0.4.0/eulerpi/examples/temperature/temperature.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/eulerpi/jax_extension.py` & `eulerpi-0.4.0/eulerpi/jax_extension.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.1/pyproject.toml` & `eulerpi-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eulerpi"
-version = "0.3.1"
+version = "0.4.0"
 description = "The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution."
 authors = ["Lars Kaiser <lars.g.kaiser@gmx.de>", "Sebastian Hoepfl <sebastian.hoepfl@ist.uni-stuttgart.de>", "Vincent Wagner <vincent.wagner@ist.uni-stuttgart.de>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `eulerpi-0.3.1/PKG-INFO` & `eulerpi-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: eulerpi
-Version: 0.3.1
+Version: 0.4.0
 Summary: The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
 Author: Lars Kaiser
 Author-email: lars.g.kaiser@gmx.de
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: amici (>=0.16.1,<0.17.0)
 Requires-Dist: diffrax (>=0.3.1,<0.4.0)
 Requires-Dist: emcee (>=3.1.4,<4.0.0)
 Requires-Dist: jax (>=0.4.8,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
@@ -41,27 +40,27 @@
 
 [![flake8](https://img.shields.io/badge/flake8-checked-blue.svg)](https://flake8.pycqa.org/)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE.md)
 [![Python](https://img.shields.io/badge/python-3.10-purple.svg)](https://www.python.org/)
 ![PyPI](https://img.shields.io/pypi/v/eulerpi)
 
-Euler Parameter Inference (EPI) is a Python package for inverse parameter inference. It provides an implementation of the EPI algorithm, which takes observed data and a model as input and returns a parameter distribution consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
+Eulerian Parameter Inference (EPI) is a powerful and novel method for inverse model parameter inference. The eulerpi package provides an implementation of the EPI algorithm, which takes observed data and a model as input and returns a parameter distribution consistent with the observed data by solving the inverse problem directly. In case the model describes a one-to-one mapping between parameters and simulation results, the inferred parameter distribution is the true underlying distribution.
 
 ## Documentation
 
-The full documentation to this software, including a detailed tutorial on how to use EPI and the api documentation, can be found under [Documentation](https://Systems-Theory-in-Systems-Biology.github.io/EPI/).
+The full documentation of this software, including a detailed tutorial on how to use EPI and the api documentation, can be found under [Documentation](https://Systems-Theory-in-Systems-Biology.github.io/EPI/).
 
 ## Features
 
 EPI supports
 
 - SBML ode models
 - User provided models
-- Models with automatic differentation using jax
+- Models with automatic differentiation using jax
 
 ## Installation
 
 The package is available on pypi and can be installed with:
 
 ```bash
 pip install eulerpi
```

