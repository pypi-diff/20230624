# Comparing `tmp/pydts-0.7.6.tar.gz` & `tmp/pydts-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydts-0.7.6.tar", max compression
+gzip compressed data, was "pydts-0.7.7.tar", max compression
```

## Comparing `pydts-0.7.6.tar` & `pydts-0.7.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.7.6/LICENSE
--rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.7.6/README.md
--rw-r--r--   0        0        0     1441 2023-06-24 11:52:17.701596 pydts-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.7.6/src/pydts/.DS_Store
--rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.7.6/src/pydts/__init__.py
--rw-r--r--   0        0        0    12925 2023-05-02 14:58:03.593428 pydts-0.7.6/src/pydts/base_fitters.py
--rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.7.6/src/pydts/config.py
--rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.7.6/src/pydts/cross_validation.py
--rw-r--r--   0        0        0    15114 2023-05-03 10:21:44.094825 pydts-0.7.6/src/pydts/data_generation.py
--rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.7.6/src/pydts/datasets/.DS_Store
--rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.7.6/src/pydts/datasets/LOS_simulated_data.csv
--rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.7.6/src/pydts/evaluation.py
--rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.7.6/src/pydts/examples_utils/__init__.py
--rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.7.6/src/pydts/examples_utils/datasets.py
--rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.7.6/src/pydts/examples_utils/generate_simulations_data.py
--rw-r--r--   0        0        0    14554 2023-06-22 21:08:27.939724 pydts-0.7.6/src/pydts/examples_utils/mimic_consts.py
--rw-r--r--   0        0        0    35475 2023-06-24 11:37:12.510709 pydts-0.7.6/src/pydts/examples_utils/plots.py
--rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.7.6/src/pydts/examples_utils/simulations_data_config.py
--rw-r--r--   0        0        0    31476 2023-06-23 19:40:20.471655 pydts-0.7.6/src/pydts/fitters.py
--rw-r--r--   0        0        0     8936 2023-02-22 11:16:27.801701 pydts-0.7.6/src/pydts/model_selection.py
--rw-r--r--   0        0        0     5994 2022-12-02 13:43:44.154153 pydts-0.7.6/src/pydts/utils.py
--rw-r--r--   0        0        0     4026 1970-01-01 00:00:00.000000 pydts-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.7.7/LICENSE
+-rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.7.7/README.md
+-rw-r--r--   0        0        0     1441 2023-06-24 12:15:38.501195 pydts-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.7.7/src/pydts/.DS_Store
+-rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.7.7/src/pydts/__init__.py
+-rw-r--r--   0        0        0    12925 2023-05-02 14:58:03.593428 pydts-0.7.7/src/pydts/base_fitters.py
+-rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.7.7/src/pydts/config.py
+-rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.7.7/src/pydts/cross_validation.py
+-rw-r--r--   0        0        0    15114 2023-05-03 10:21:44.094825 pydts-0.7.7/src/pydts/data_generation.py
+-rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.7.7/src/pydts/datasets/.DS_Store
+-rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.7.7/src/pydts/datasets/LOS_simulated_data.csv
+-rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.7.7/src/pydts/evaluation.py
+-rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.7.7/src/pydts/examples_utils/__init__.py
+-rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.7.7/src/pydts/examples_utils/datasets.py
+-rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.7.7/src/pydts/examples_utils/generate_simulations_data.py
+-rw-r--r--   0        0        0    14554 2023-06-22 21:08:27.939724 pydts-0.7.7/src/pydts/examples_utils/mimic_consts.py
+-rw-r--r--   0        0        0    35420 2023-06-24 12:18:25.376596 pydts-0.7.7/src/pydts/examples_utils/plots.py
+-rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.7.7/src/pydts/examples_utils/simulations_data_config.py
+-rw-r--r--   0        0        0    31476 2023-06-23 19:40:20.471655 pydts-0.7.7/src/pydts/fitters.py
+-rw-r--r--   0        0        0     8936 2023-02-22 11:16:27.801701 pydts-0.7.7/src/pydts/model_selection.py
+-rw-r--r--   0        0        0     5994 2022-12-02 13:43:44.154153 pydts-0.7.7/src/pydts/utils.py
+-rw-r--r--   0        0        0     4026 1970-01-01 00:00:00.000000 pydts-0.7.7/PKG-INFO
```

### Comparing `pydts-0.7.6/LICENSE` & `pydts-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/README.md` & `pydts-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/pyproject.toml` & `pydts-0.7.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydts"
-version = "0.7.6"
+version = "0.7.7"
 description = "Discrete time survival analysis with competing risks"
 authors = ["Tomer Meir <tomer1812@gmail.com>", "Rom Gutman <rom.gutman1@gmail.com>", "Malka Gorfine <malkago12@gmail.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 homepage = "https://github.com/tomer1812/pydts"
 repository = "https://github.com/tomer1812/pydts"
 keywords = ["Discrete Time", "Time to Event" ,"Survival Analysis", "Competing Events"]
```

### Comparing `pydts-0.7.6/src/pydts/.DS_Store` & `pydts-0.7.7/src/pydts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/base_fitters.py` & `pydts-0.7.7/src/pydts/base_fitters.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/cross_validation.py` & `pydts-0.7.7/src/pydts/cross_validation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/data_generation.py` & `pydts-0.7.7/src/pydts/data_generation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/datasets/.DS_Store` & `pydts-0.7.7/src/pydts/datasets/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/datasets/LOS_simulated_data.csv` & `pydts-0.7.7/src/pydts/datasets/LOS_simulated_data.csv`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/evaluation.py` & `pydts-0.7.7/src/pydts/evaluation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/examples_utils/generate_simulations_data.py` & `pydts-0.7.7/src/pydts/examples_utils/generate_simulations_data.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/examples_utils/mimic_consts.py` & `pydts-0.7.7/src/pydts/examples_utils/mimic_consts.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/examples_utils/plots.py` & `pydts-0.7.7/src/pydts/examples_utils/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import Iterable, Tuple
 
 import numpy as np
-from pydts.examples_utils.plots import add_panel_text
-
 from .simulations_data_config import *
 from matplotlib import pyplot as plt
 import matplotlib.gridspec as gridspec
 import seaborn as sns
 from lifelines import KaplanMeierFitter
 from ..config import *
 import os
```

### Comparing `pydts-0.7.6/src/pydts/examples_utils/simulations_data_config.py` & `pydts-0.7.7/src/pydts/examples_utils/simulations_data_config.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/fitters.py` & `pydts-0.7.7/src/pydts/fitters.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/model_selection.py` & `pydts-0.7.7/src/pydts/model_selection.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/src/pydts/utils.py` & `pydts-0.7.7/src/pydts/utils.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.6/PKG-INFO` & `pydts-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydts
-Version: 0.7.6
+Version: 0.7.7
 Summary: Discrete time survival analysis with competing risks
 Home-page: https://github.com/tomer1812/pydts
 License: GNU GPLv3
 Keywords: Discrete Time,Time to Event,Survival Analysis,Competing Events
 Author: Tomer Meir
 Author-email: tomer1812@gmail.com
 Requires-Python: >=3.8,<3.11
```

