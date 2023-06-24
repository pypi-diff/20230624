# Comparing `tmp/mloptimizer-0.5.7.tar.gz` & `tmp/mloptimizer-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mloptimizer-0.5.7.tar", last modified: Fri Jun 23 14:21:06 2023, max compression
+gzip compressed data, was "mloptimizer-0.5.8.tar", last modified: Sat Jun 24 10:43:44 2023, max compression
```

## Comparing `mloptimizer-0.5.7.tar` & `mloptimizer-0.5.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:21:06.654225 mloptimizer-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-23 14:21:06.654225 mloptimizer-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:21:06.650225 mloptimizer-0.5.7/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1954444 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/data/data_sample.csv
--rw-r--r--   0 runner    (1001) docker     (123)   694332 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/data/data_sample_test.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1260187 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/data/data_sample_train.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:21:06.650225 mloptimizer-0.5.7/mloptimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    39217 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/genoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/model_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:21:06.654225 mloptimizer-0.5.7/mloptimizer/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/test_TreeOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/test_XGBClassifierOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/test_alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/test_genoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/mloptimizer/test/test_param.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:21:06.654225 mloptimizer-0.5.7/mloptimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-23 14:21:06.000000 mloptimizer-0.5.7/mloptimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-23 14:21:06.000000 mloptimizer-0.5.7/mloptimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:21:06.000000 mloptimizer-0.5.7/mloptimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-23 14:21:06.000000 mloptimizer-0.5.7/mloptimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 14:21:06.000000 mloptimizer-0.5.7/mloptimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:21:06.654225 mloptimizer-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-06-23 14:20:56.000000 mloptimizer-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:44.900845 mloptimizer-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-24 10:43:44.900845 mloptimizer-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:44.896845 mloptimizer-0.5.8/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1954444 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/data/data_sample.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   694332 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/data/data_sample_test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1260187 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/data/data_sample_train.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:44.896845 mloptimizer-0.5.8/mloptimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/genoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/model_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:44.900845 mloptimizer-0.5.8/mloptimizer/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/test_TreeOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/test_XGBClassifierOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/test_alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/test_genoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/mloptimizer/test/test_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:43:44.900845 mloptimizer-0.5.8/mloptimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-24 10:43:44.000000 mloptimizer-0.5.8/mloptimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-24 10:43:44.000000 mloptimizer-0.5.8/mloptimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:43:44.000000 mloptimizer-0.5.8/mloptimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-24 10:43:44.000000 mloptimizer-0.5.8/mloptimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-24 10:43:44.000000 mloptimizer-0.5.8/mloptimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 10:43:44.900845 mloptimizer-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-06-24 10:43:33.000000 mloptimizer-0.5.8/setup.py
```

### Comparing `mloptimizer-0.5.7/LICENSE` & `mloptimizer-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.7/PKG-INFO` & `mloptimizer-0.5.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.5.7
+Version: 0.5.8
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mloptimizer-0.5.7/README.md` & `mloptimizer-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.7/data/data_sample.csv` & `mloptimizer-0.5.8/data/data_sample.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.7/data/data_sample_test.csv` & `mloptimizer-0.5.8/data/data_sample_test.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.7/data/data_sample_train.csv` & `mloptimizer-0.5.8/data/data_sample_train.csv`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.7/mloptimizer/alg_wrapper.py` & `mloptimizer-0.5.8/mloptimizer/alg_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
+import keras
+import numpy as np
 import xgboost as xgb
+from keras.layers import Dense, Dropout
+from keras.models import Sequential
 from sklearn.base import BaseEstimator
 from sklearn.utils import check_array
-import numpy as np
-from keras.models import Sequential
-from keras.layers import Dense, Dropout
-from sklearn.utils import class_weight
-from sklearn.preprocessing import OneHotEncoder
-from keras.wrappers.scikit_learn import KerasClassifier
-import keras
 
 
 class CustomXGBClassifier(BaseEstimator):
     def __init__(self, base_score=0.5, booster="gbtree", eval_metric="auc",
                  eta=0.077, gamma=18, subsample=0.728, colsample_bylevel=1,
                  colsample_bytree=0.46, max_delta_step=0, max_depth=7,
                  min_child_weight=1, seed=1, alpha=0, reg_lambda=1, scale_pos_weight=4.43,
```

### Comparing `mloptimizer-0.5.7/mloptimizer/genoptimizer.py` & `mloptimizer-0.5.8/mloptimizer/genoptimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-import multiprocessing
+import os
+import random
+import shutil
 from abc import ABCMeta, abstractmethod, ABC
+from datetime import datetime
 from random import randint
-import random
+
+import joblib
 import matplotlib.pyplot as plt
 import numpy as np
-import copy
 import pandas as pd
+import xgboost as xgb
+from catboost import CatBoostClassifier
 from deap import creator, tools, base
 from deap.algorithms import varAnd
+from keras.wrappers.scikit_learn import KerasClassifier
 from sklearn.ensemble import RandomForestClassifier, ExtraTreesClassifier, GradientBoostingClassifier
+from sklearn.metrics import balanced_accuracy_score
 from sklearn.neural_network import MLPClassifier
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
-from mloptimizer.model_evaluation import KFoldStratifiedAccuracy
+
 from mloptimizer import miscellaneous
 from mloptimizer.alg_wrapper import CustomXGBClassifier, generate_model
-import xgboost as xgb
-from keras.wrappers.scikit_learn import KerasClassifier
-from catboost import CatBoostClassifier
-import joblib
-import os
-import shutil
-from datetime import datetime
-import time
+from mloptimizer.model_evaluation import kfold_stratified_score
 from mloptimizer.plots import plot_search_space, plot_logbook
 
 
 class Param(object):
     """
     Object to store param info, type and range of values
     """
 
     def __init__(self, name: str, min_value: int, max_value: int, param_type,
                  denominator: int = 100, values_str: list = None):
         """
-        Init object
+        Init param
 
-        :param name: (str) Name of the param. It will be use as key in a dictionary
-        :param min_value: (int) Minimum value of the param
-        :param max_value: (int) Maximum value of the param
-        :param param_type: (type) type of the param (int, float, 'nexp', 'x10')
+        :param str name: Name of the param. It will be use as key in a dictionary
+        :param int min_value: Minimum value of the param
+        :param int max_value: Maximum value of the param
+        :param type param_type: Type of the param (int, float, 'nexp', 'x10')
+        :param int denominator: Optional param in case the type=float
+        :param list values_str: List of string with possible values (TODO)
         """
         if values_str is None:
             values_str = []
         self.name = name
         self.min_value = min_value
         self.max_value = max_value
         self.type = param_type
@@ -77,36 +79,40 @@
             ret = 10 ** (-value)
         elif self.type == "x10":
             ret = value * 10
         return ret
 
     def __eq__(self, other_param):
         """Overrides the default implementation"""
-
         equals = (self.name == other_param.name and self.min_value == other_param.min_value and
                   self.type == other_param.type and self.denominator == other_param.denominator and
                   self.max_value == other_param.max_value)
         return equals
 
     def __str__(self):
         """Overrides the default implementation"""
+        if type(self.type) == type:
+            type_str = self.type.__name__
+        elif type(self.type) == str:
+            type_str = "'{}'".format(self.type)
+
         if self.type == float:
             param_str = "Param('{}', {}, {}, {}, {})".format(
                 self.name,
                 self.min_value,
                 self.max_value,
-                self.type.__name__,
+                type_str,
                 self.denominator
             )
         else:
             param_str = "Param('{}', {}, {}, {})".format(
                 self.name,
                 self.min_value,
                 self.max_value,
-                self.type.__name__
+                type_str
             )
 
         return param_str
 
     def __repr__(self):
         """Overrides the default implementation"""
         return self.__str__()
@@ -116,34 +122,62 @@
     """
     Abstract class to create optimizer for different machine learning classifier algorithms
     """
     __metaclass__ = ABCMeta
 
     def __init__(self, features: np.array, labels: np.array, folder=None, log_file="mloptimizer.log",
                  custom_params: dict = {},
-                 custom_fixed_params: dict = {}, eval_function=KFoldStratifiedAccuracy):
-        self.logbook = None
-        self.progress_path = None
-        self.progress_path = None
-        self.exe_path = None
+                 custom_fixed_params: dict = {}, eval_function=kfold_stratified_score,
+                 score_function=balanced_accuracy_score):
+        """
+        Init the optimizer
+        :param list features: np.array with the features
+        :param list labels: np.array with the labels
+        :param path folder: folder to store the results
+        :param str log_file: log file name
+        :param dict custom_params: dictionary with custom params
+        :param dict custom_fixed_params: dictionary with custom fixed params
+        :param func eval_function: function to evaluate the model from X, y, clf
+        :param func score_function: function to score from y, y_pred
+        """
+        # Input mandatory variables
         self.features = features
         self.labels = labels
-        self.folder = miscellaneous.create_optimization_folder(folder)
+        # Input parameters (optional)
         self.custom_params = custom_params
         self.custom_fixed_params = custom_fixed_params
-        self.params = self.get_params()
         self.fixed_params = self.get_fixed_params()
-        self.eval_dict = {}
+        self.params = self.get_params()
+        # Main folder (autogenerated if None)
+        self.folder = miscellaneous.create_optimization_folder(folder)
+        # Log files
         self.mloptimizer_logger, self.log_file = miscellaneous.init_logger(log_file, self.folder)
         self.optimization_logger = None
         self.eval_function = eval_function
+        self.score_function = score_function
+        # Paths
+        self.exe_path = None
         self.checkpoint_path = None
-        self.populations = []
+        self.progress_path = None
+        self.progress_path = None
         self.results_path = None
         self.graphics_path = None
+        # State vars
+        self.eval_dict = {}
+        self.populations = []
+        self.logbook = None
+
+    @staticmethod
+    def get_subclasses(my_class):
+        subclasses = my_class.__subclasses__()
+        if len(subclasses) == 0:
+            return []
+        next_subclasses = []
+        [next_subclasses.extend(BaseOptimizer.get_subclasses(x)) for x in subclasses]
+        return [*subclasses, *next_subclasses]
 
     def get_folder(self):
         return self.folder
 
     def get_log_file(self):
         return self.log_file
 
@@ -206,23 +240,23 @@
         }
         return default_fixed_params
 
     @abstractmethod
     def get_clf(self, individual):
         pass
 
-
     def evaluate_clf(self, individual):
         """
         Method to evaluate the individual, in this case the classifier
 
         :param individual: individual for evaluation
         :return: fitness
         """
-        mean = self.eval_function(self.features, self.labels, self.get_clf(individual))
+        mean = self.eval_function(self.features, self.labels, self.get_clf(individual),
+                                  score_function=self.score_function)
         return (mean,)
 
     def population_2_df(self):
         data = []
         n = 0
         for p in self.populations:
             for i in p:
@@ -252,20 +286,23 @@
         data = []
         if os.path.exists(filename):
             data = pd.read_csv(filename)
         else:
             self.optimization_logger.error("File {} does not exist".format(filename))
         return data
 
-    def optimize_clf(self, population: int = 10, generations: int = 3, checkpoint: str = None) -> object:
+    def optimize_clf(self, population: int = 10, generations: int = 3,
+                     checkpoint: str = None, exe_folder: str = None) -> object:
         """
         Searches through a genetic algorithm the best classifier
 
         :param int population: Number of members of the first generation
         :param int generations: Number of generations
+        :param str checkpoint: Path to a checkpoint file
+        :param str exe_folder: Path to the folder where the execution will be saved
         :return: Trained classifier
         """
         self.mloptimizer_logger.info("Initiating genetic optimization...")
         self.mloptimizer_logger.info("Algorithm: {}".format(type(self).__name__))
         # Creation of individual and population
         toolbox = base.Toolbox()
         stats = tools.Statistics(lambda ind: ind.fitness.values)
@@ -305,17 +342,20 @@
             self.results_path = os.path.join(self.checkpoint_path, "results")
             self.graphics_path = os.path.join(self.checkpoint_path, "graphics")
         else:
 
             self.logbook.header = ['gen', 'nevals'] + (stats.fields if stats else [])
 
             # Create checkpoint_path from date and algorithm
-            exe_name = "{}_{}".format(
-                datetime.now().strftime("%Y%m%d_%s"),
-                type(self).__name__)
+            if exe_folder:
+                exe_name = exe_folder
+            else:
+                exe_name = "{}_{}".format(
+                    datetime.now().strftime("%Y%m%d_%s"),
+                    type(self).__name__)
             self.exe_path = os.path.join(self.folder, exe_name)
             self.checkpoint_path = os.path.join(self.exe_path, "checkpoints")
             self.results_path = os.path.join(self.exe_path, "results")
             self.graphics_path = os.path.join(self.exe_path, "graphics")
             self.progress_path = os.path.join(self.exe_path, "progress")
             if os.path.exists(self.exe_path):
                 shutil.rmtree(self.exe_path)
@@ -442,15 +482,15 @@
             raise NotADirectoryError(error_msg)
 
         # Begin the generational process
 
         for gen in range(start_gen, ngen + 1):
             progress_gen_path = os.path.join(self.progress_path, "Generation_{}.csv".format(gen))
             progress_gen_file = open(progress_gen_path, "w")
-            header_progress_gen_file = "i;total;time(s);Individual;fitness\n"
+            header_progress_gen_file = "i;total;Individual;fitness\n"
             progress_gen_file.write(header_progress_gen_file)
             self.optimization_logger.info("Generation: {}".format(gen))
             # Vary the pool of individuals
             population = varAnd(population, toolbox, cxpb, mutpb)
 
             # Evaluate the individuals with an invalid fitness
             invalid_ind = [ind for ind in population if not ind.fitness.valid]
@@ -459,24 +499,20 @@
             evaluations_pending = len(invalid_ind)
             for ind, fit in zip(invalid_ind, fitnesses):
                 self.optimization_logger.info(
                     "Fitting individual (informational purpose): gen {} - ind {} of {}".format(
                         gen, c, evaluations_pending
                     )
                 )
-                t0_evaluation = time.time()
                 ind.fitness.values = fit
-                t1_evaluation = time.time()
-                t_evaluation = t1_evaluation - t0_evaluation
                 ind_formatted = self.individual2dict(ind)
                 progress_gen_file.write(
-                    "{};{};{};{};{}\n".format(c,
-                                              evaluations_pending,
-                                              t_evaluation,
-                                              ind_formatted, fit)
+                    "{};{};{};{}\n".format(c,
+                                           evaluations_pending,
+                                           ind_formatted, fit)
                 )
                 c = c + 1
 
             halloffame.update(population)
 
             record = stats.compile(population) if stats else {}
 
@@ -571,15 +607,16 @@
         """
         individual_dict = self.individual2dict(individual)
 
         clf = RandomForestClassifier(n_estimators=individual_dict['n_estimators'],
                                      criterion="gini",
                                      max_depth=individual_dict['max_depth'],
                                      max_samples=individual_dict['max_samples'],
-                                     min_weight_fraction_leaf=0,
+                                     min_weight_fraction_leaf=individual_dict['min_weight_fraction_leaf'],
+                                     min_impurity_decrease=individual_dict['min_impurity_decrease'],
                                      max_features=individual_dict['max_features'],
                                      max_leaf_nodes=None,
                                      bootstrap=True,
                                      oob_score=True,
                                      n_jobs=-1,
                                      random_state=None,
                                      verbose=0,
@@ -591,17 +628,17 @@
     @staticmethod
     def get_default_params():
         default_params = {
             "max_features": Param("max_features", 1, 100, float, 100),
             "n_estimators": Param("n_estimators", 5, 250, int),
             "max_samples": Param("max_samples", 10, 100, float, 100),
             "max_depth": Param("max_depth", 2, 14, int),
-            "scale_pos_weight": Param("scale_pos_weight", 1, 1000, float, 100),
             "min_impurity_decrease": Param("min_impurity_decrease", 0, 500, float, 100),
-            "min_weight_fraction_leaf": Param("min_weight_fraction_leaf", 1, 1000, float, 100)
+            # min_weight_fraction_leaf must be a float in the range [0.0, 0.5]
+            "min_weight_fraction_leaf": Param("min_weight_fraction_leaf", 0, 50, float, 100)
         }
         return default_params
 
 
 class ExtraTreesOptimizer(ForestOptimizer, ABC):
     """
     Concrete optimizer for sklearn extra trees -> sklearn.ensemble.ExtraTreesClassifier
@@ -634,15 +671,15 @@
                                    # min_samples_split=individual_dict['min_samples_split'],
                                    # min_samples_leaf=individual_dict['min_samples_leaf'],
                                    min_weight_fraction_leaf=individual_dict['min_weight_fraction_leaf'],
                                    min_impurity_decrease=individual_dict['min_impurity_decrease'],
                                    max_features=individual_dict['max_features'],
                                    max_samples=individual_dict['max_samples'],
                                    max_leaf_nodes=None,
-                                   bootstrap=False,
+                                   bootstrap=True,
                                    oob_score=False,
                                    n_jobs=-1,
                                    random_state=None,
                                    verbose=0,
                                    warm_start=False,
                                    class_weight=class_weight
                                    )
@@ -660,34 +697,37 @@
         Params for the creation of individuals (relative to the algorithm)
         These params define the name of the param, min value, max value, and type
 
         :return: list of params
         """
         params = super(GradientBoostingOptimizer, self).get_params()
         # learning_rate
-        params.append(Param("learning_rate", 1, 10000, float, 1000000))
+        params["learning_rate"] = Param('learning_rate', 1, 10000, float, 1000000)
         # subsample
-        params.append(Param("subsample", 0, 100, float, 100))
+        del params["max_samples"]
+        # subsample must be a float in the range (0.0, 1.0]
+        params["subsample"] = Param('subsample', 10, 100, float, 100)
         # Return all the params
         return params
 
     def get_clf(self, individual):
         """
         Builds a classifier object from an individual one
 
         :param individual: individual to create a classifier
         :return: classifier ExtraTreesClassifier
         """
         individual_dict = self.individual2dict(individual)
         clf = GradientBoostingClassifier(n_estimators=individual_dict['n_estimators'],
                                          criterion="friedman_mse",
                                          max_depth=individual_dict['max_depth'],
-                                         min_samples_split=individual_dict['min_samples_split'],
-                                         min_samples_leaf=individual_dict['min_samples_leaf'],
-                                         min_weight_fraction_leaf=0,
+                                         # min_samples_split=individual_dict['min_samples_split'],
+                                         # min_samples_leaf=individual_dict['min_samples_leaf'],
+                                         min_weight_fraction_leaf=individual_dict['min_weight_fraction_leaf'],
+                                         min_impurity_decrease=individual_dict['min_impurity_decrease'],
                                          max_features=individual_dict['max_features'],
                                          max_leaf_nodes=None,
                                          random_state=None,
                                          verbose=0,
                                          warm_start=False,
                                          learning_rate=individual_dict['learning_rate'],
                                          subsample=individual_dict['subsample'])
```

### Comparing `mloptimizer-0.5.7/mloptimizer/miscellaneous.py` & `mloptimizer-0.5.8/mloptimizer/miscellaneous.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 import logging
+import os
 from logging import FileHandler
 from logging import Formatter
-import os
 
 
 def init_logger(filename='mloptimizer.log', log_path="."):
-    FILENAME = os.path.join(log_path, filename)
-    LOG_FORMAT = (
+    """
+    Initializes a logger with the given filename and log_path.
+    The logger is configured to log INFO messages and above.
+    :param filename: the name of the log file
+    :param log_path: the path where the log file will be created
+    :return: the logger object and the log file path
+    :rtype: tuple
+    """
+    filename = os.path.join(log_path, filename)
+    log_format = (
         "%(asctime)s [%(levelname)s]: %(message)s in %(pathname)s:%(lineno)d")
-    LOG_LEVEL = logging.INFO
+    log_level = logging.INFO
     custom_logger = logging.getLogger(filename)
-    custom_logger.setLevel(LOG_LEVEL)
-    custom_logger_file_handler = FileHandler(FILENAME)
-    custom_logger_file_handler.setLevel(LOG_LEVEL)
-    custom_logger_file_handler.setFormatter(Formatter(LOG_FORMAT))
+    custom_logger.setLevel(log_level)
+    custom_logger_file_handler = FileHandler(filename)
+    custom_logger_file_handler.setLevel(log_level)
+    custom_logger_file_handler.setFormatter(Formatter(log_format))
     custom_logger.addHandler(custom_logger_file_handler)
     custom_logger.debug("Logger configured")
-    return custom_logger, FILENAME
+    return custom_logger, filename
 
 
 def create_optimization_folder(folder):
     """
     Creates a folder at the given path, if it doesn't already exist.
     If the folder already exists, prompts the user to delete it.
+    :param folder: the path of the folder to be created
+    :return: the path of the folder
+    :rtype: str
     """
     if folder is None:
         folder = os.path.join(os.curdir, "Optimizer")
     if os.path.exists(folder):
-        print("The folder already exists and it will be used")
+        print("The folder {} already exists and it will be used".format(folder))
     else:
         os.mkdir(folder)
-        print("The folder has been created.")
+        print("The folder {} has been created.".format(folder))
     return folder
```

### Comparing `mloptimizer-0.5.7/mloptimizer/model_evaluation.py` & `mloptimizer-0.5.8/mloptimizer/model_evaluation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 import logging
+import time
+
+import numpy as np
 from sklearn.metrics import balanced_accuracy_score
 from sklearn.model_selection import StratifiedKFold, TimeSeriesSplit
-import numpy as np
-import time
 
 
-def unpackDF(df, target_variable="class"):
-    '''
+def unpack_df(df, target_variable="class"):
+    """
     Extract classes, features, and labels from a pandas.DataFrame.
-    One column of the DataFrame should be called "class" and
+    One column of the DataFrame should be called as target_variable="class" and
     the rest are features.
 
     :param DataFrame df: pandas.DataFrame with the dataset
+    :param str target_variable: str with the name of the target column
     :return: Classes, features, labels
-    '''
+    """
     class_list = list(df[target_variable].drop_duplicates())
     labels = df[target_variable]
     features = np.array(df.drop(columns=[target_variable]))
     return class_list, features, labels
 
 
-def KFoldStratifiedAccuracy(features, labels, clf, n_splits=4, score_function=balanced_accuracy_score,
-                            random_state=None):
-    '''
-    Computes KFold cross validation accuracy using n_splits folds over the data in the pandas.DataFrame given.
-    Uses an stratified KFold with the random_state specified.
+def kfold_stratified_score(features, labels, clf, n_splits=4, score_function=balanced_accuracy_score,
+                           random_state=None):
+    """
+    Computes KFold cross validation score using n_splits folds.
+    It uses the features and labels to train the k-folds.
+    Uses a stratified KFold with the random_state specified.
+    The score_function is the one used to score each k-fold.
 
-    :param df: pandas.DataFrame where is the data for train/test splits
+    :param list features: List of features
+    :param list labels: List of labels
     :param clf: classifier with methods fit, predict and score
     :param n_splits: number of splits
+    :param func score_function: function that receives X, y and return a score
     :param random_state: random state seed
-    :return: mean accuracy, std
-    '''
+    :return: mean score among k-folds test splits
+    """
     logging.info("KFold Stratified accuracy\nClassifier:{}\nn_splits:{}\n"
                  "score_metric:{}".format(clf, n_splits, score_function))
 
     clfs = []
 
     # Create object to split the dataset (in 5 at random but preserving percentage of each class)
     skf = StratifiedKFold(n_splits=n_splits, shuffle=True, random_state=random_state)
@@ -79,37 +85,40 @@
 
         labels_kfold.extend(labels_test)
         labels_kfold_predicted.extend(labels_pred_test)
 
         kcounter += 1
         clfs.append(clf)
 
-    meanAccuracy = np.mean(accuracies_kfold)
+    mean_accuracy = np.mean(accuracies_kfold)
     std = np.std(accuracies_kfold)
-    logging.info("Accuracy: {:.3f} +- {:.3f}".format(round(meanAccuracy, 3), round(std, 3)))
+    logging.info("Accuracy: {:.3f} +- {:.3f}".format(round(mean_accuracy, 3), round(std, 3)))
 
-    # return meanAccuracy, std, labels, labels_predicted, clfs
-    return meanAccuracy
+    # return mean_accuracy, std, labels, labels_predicted, clfs
+    return mean_accuracy
 
 
-def TemporalKFoldAccuracy(features, labels, clf, n_splits=4, score_function=balanced_accuracy_score):
-    '''
-    Computes KFold cross validation accuracy using n_splits folds over the data in the pandas.DataFrame given.
-    Uses an stratified KFold with the random_state specified.
+def temporal_kfold_score(features, labels, clf, n_splits=4, score_function=balanced_accuracy_score):
+    """
+    Computes KFold cross validation score using n_splits folds.
+    It uses the features and labels to train the k-folds.
+    Uses a temporal KFold split.
+    The score_function is the one used to score each k-fold.
 
-    :param df: pandas.DataFrame where is the data for train/test splits
+    :param list features: List of features
+    :param list labels: List of labels
     :param clf: classifier with methods fit, predict and score
     :param n_splits: number of splits
-    :param random_state: random state seed
-    :return: mean accuracy, std
-    '''
+    :param func score_function: function that receives X, y and return a score
+    :return: mean score among k-folds test splits
+    """
     logging.info("TemporalKFold accuracy\nClassifier:{}\nn_splits:{}\n"
                  "score_metric:{}".format(clf, n_splits, score_function))
     print("TemporalKFold accuracy\nClassifier:{}\nn_splits:{}\n"
-                 "score_metric:{}".format(clf, n_splits, score_function))
+          "score_metric:{}".format(clf, n_splits, score_function))
 
     clfs = []
 
     # Create object to split the dataset (in 5 at random but preserving percentage of each class)
     tscv = TimeSeriesSplit(n_splits=n_splits)
     # Split the dataset. The skf saves splits index
     tscv.get_n_splits(features, labels)
@@ -155,14 +164,14 @@
 
             labels_kfold.extend(labels_test)
             labels_kfold_predicted.extend(labels_pred_test)
 
             kcounter += 1
             clfs.append(clf)
 
-    meanAccuracy = np.mean(accuracies_kfold)
+    mean_accuracy = np.mean(accuracies_kfold)
     std = np.std(accuracies_kfold)
-    logging.info("Accuracy: {:.2f} +- {:.2f}".format(round(meanAccuracy, 3), round(std, 3)))
-    print("Accuracy: {:.2f} +- {:.2f}".format(round(meanAccuracy, 3), round(std, 3)))
+    logging.info("Accuracy: {:.2f} +- {:.2f}".format(round(mean_accuracy, 3), round(std, 3)))
+    print("Accuracy: {:.2f} +- {:.2f}".format(round(mean_accuracy, 3), round(std, 3)))
 
-    # return meanAccuracy, std, labels, labels_predicted, clfs
-    return meanAccuracy
+    # return mean_accuracy, std, labels, labels_predicted, clfs
+    return mean_accuracy
```

### Comparing `mloptimizer-0.5.7/mloptimizer/test/test_TreeOptimizer.py` & `mloptimizer-0.5.8/mloptimizer/test/test_TreeOptimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import numpy as np
-import pytest
-import pandas as pd
 import os
+import shutil
+
+import pytest
+from sklearn.datasets import load_iris, load_breast_cancer
 
 from mloptimizer.genoptimizer import Param
 from mloptimizer.genoptimizer import TreeOptimizer
-from sklearn.datasets import load_iris, load_breast_cancer
-import shutil
 
 
 @pytest.fixture
 def default_tree_optimizer():
     X, y = load_iris(return_X_y=True)
     return TreeOptimizer(X, y)
 
@@ -36,14 +35,26 @@
         "max_depth": 4,
         "min_samples_split": 10
     }
     X, y = load_iris(return_X_y=True)
     return TreeOptimizer(X, y, custom_fixed_params=fixed_params)
 
 
+@pytest.fixture
+def custom_all_params_tree_optimizer():
+    fixed_params = {
+        "min_samples_split": 10
+    }
+    custom_params = {
+        "max_depth": Param("max_depth", 2, 4, int),
+    }
+    X, y = load_iris(return_X_y=True)
+    return TreeOptimizer(X, y, custom_params=custom_params, custom_fixed_params=fixed_params)
+
+
 # Test vanilla TreeOptimizer
 # Test custom parameters TreeOptimizer
 # Test fixed parameters TreeOptimizer
 
 def test_tree_optimizer_get_params(default_tree_optimizer):
     assert default_tree_optimizer.get_params() == default_tree_optimizer.get_default_params()
 
@@ -69,9 +80,9 @@
 
 def test_create_tree_optimizer2(default_tree_optimizer2):
     assert os.path.isdir(default_tree_optimizer2.get_folder()) and os.path.exists(
         default_tree_optimizer2.get_log_file())
     shutil.rmtree(default_tree_optimizer2.get_folder())
 
 
-def test_tree_optimizer_get_params(default_tree_optimizer):
-    default_tree_optimizer.optimize_clf(8, 10)
+def test_tree_all_params_tree_optimizer(custom_all_params_tree_optimizer):
+    custom_all_params_tree_optimizer.optimize_clf(8, 10)
```

### Comparing `mloptimizer-0.5.7/mloptimizer/test/test_alg_wrapper.py` & `mloptimizer-0.5.8/mloptimizer/test/test_alg_wrapper.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.7/mloptimizer/test/test_genoptimizer.py` & `mloptimizer-0.5.8/mloptimizer/test/test_genoptimizer.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.7/mloptimizer/test/test_param.py` & `mloptimizer-0.5.8/mloptimizer/test/test_param.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from mloptimizer.genoptimizer import Param
 
 
 @pytest.fixture
 def int_param():
     return Param('int_param', 1, 10, int)
```

### Comparing `mloptimizer-0.5.7/mloptimizer.egg-info/PKG-INFO` & `mloptimizer-0.5.8/mloptimizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.5.7
+Version: 0.5.8
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mloptimizer-0.5.7/mloptimizer.egg-info/SOURCES.txt` & `mloptimizer-0.5.8/mloptimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.5.7/setup.py` & `mloptimizer-0.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     name="mloptimizer",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.5.7",  # Required
+    version="0.5.8",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="mloptimizer is a Python library "
                 "for optimizing hyperparameters of machine learning algorithms using genetic algorithms.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
```

