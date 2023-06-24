# Comparing `tmp/torchlearn-0.2.1.tar.gz` & `tmp/torchlearn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlearn-0.2.1.tar", last modified: Sat Jun 24 05:59:40 2023, max compression
+gzip compressed data, was "torchlearn-0.2.2.tar", last modified: Sat Jun 24 06:06:54 2023, max compression
```

## Comparing `torchlearn-0.2.1.tar` & `torchlearn-0.2.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11344 2023-05-23 18:24:04.000000 torchlearn-0.2.1/LICENSE
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       69 2023-05-23 18:21:28.000000 torchlearn-0.2.1/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    14853 2023-06-24 05:59:40.180539 torchlearn-0.2.1/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1390 2023-06-07 15:43:16.000000 torchlearn-0.2.1/README.md
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        5 2023-06-24 05:50:07.000000 torchlearn-0.2.1/VERSION
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    23654 2023-06-24 05:58:51.000000 torchlearn-0.2.1/pyproject.toml
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       53 2023-06-24 05:33:22.000000 torchlearn-0.2.1/requirements-dev.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       34 2023-05-23 18:21:35.000000 torchlearn-0.2.1/requirements.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-06-24 05:59:40.180539 torchlearn-0.2.1/setup.cfg
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:40:30.000000 torchlearn-0.2.1/torchlearn/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/metric/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1276 2023-06-24 05:40:27.000000 torchlearn-0.2.1/torchlearn/metric/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1257 2023-06-24 05:46:23.000000 torchlearn-0.2.1/torchlearn/metric/average_metric.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    15346 2023-06-24 05:45:32.000000 torchlearn-0.2.1/torchlearn/metric/classification.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      545 2023-06-24 05:54:59.000000 torchlearn-0.2.1/torchlearn/metric/loss.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      384 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/metric/metric.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      887 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/metric/metric_dict.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2638 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/metric/metric_value.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2133 2023-06-24 05:44:27.000000 torchlearn-0.2.1/torchlearn/metric/state.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/model/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      227 2023-06-24 05:41:00.000000 torchlearn-0.2.1/torchlearn/model/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      557 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/model/classifier.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1146 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/model/mlp.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      796 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/model/perceptron.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/objective/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      247 2023-06-24 05:41:32.000000 torchlearn-0.2.1/torchlearn/objective/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1507 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/objective/objective.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3593 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/objective/pareto.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/processing/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      253 2023-06-24 05:40:27.000000 torchlearn-0.2.1/torchlearn/processing/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5011 2023-06-24 05:36:29.000000 torchlearn-0.2.1/torchlearn/processing/graph.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/training/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      469 2023-06-24 05:40:27.000000 torchlearn-0.2.1/torchlearn/training/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      370 2023-06-24 05:37:08.000000 torchlearn-0.2.1/torchlearn/training/callback.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1753 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/training/early_stopping.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1860 2023-06-24 05:40:11.000000 torchlearn-0.2.1/torchlearn/training/pareto.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1808 2023-06-24 05:47:33.000000 torchlearn-0.2.1/torchlearn/training/results.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      225 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/training/schedulers.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6456 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/training/trainer.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/utils/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      384 2023-06-24 05:41:18.000000 torchlearn-0.2.1/torchlearn/utils/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      738 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/utils/arguments.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2614 2023-06-24 05:37:08.000000 torchlearn-0.2.1/torchlearn/utils/graph.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      239 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/utils/numbers.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    14853 2023-06-24 05:59:40.000000 torchlearn-0.2.1/torchlearn.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1151 2023-06-24 05:59:40.000000 torchlearn-0.2.1/torchlearn.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-24 05:59:40.000000 torchlearn-0.2.1/torchlearn.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       96 2023-06-24 05:59:40.000000 torchlearn-0.2.1/torchlearn.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       22 2023-06-24 05:59:40.000000 torchlearn-0.2.1/torchlearn.egg-info/top_level.txt
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 06:06:54.421058 torchlearn-0.2.2/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11344 2023-05-23 18:24:04.000000 torchlearn-0.2.2/LICENSE
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       69 2023-05-23 18:21:28.000000 torchlearn-0.2.2/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    14853 2023-06-24 06:06:54.421058 torchlearn-0.2.2/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1390 2023-06-07 15:43:16.000000 torchlearn-0.2.2/README.md
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        5 2023-06-24 06:03:31.000000 torchlearn-0.2.2/VERSION
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    23654 2023-06-24 05:58:51.000000 torchlearn-0.2.2/pyproject.toml
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       53 2023-06-24 05:33:22.000000 torchlearn-0.2.2/requirements-dev.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       34 2023-05-23 18:21:35.000000 torchlearn-0.2.2/requirements.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-06-24 06:06:54.421058 torchlearn-0.2.2/setup.cfg
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 06:06:54.411058 torchlearn-0.2.2/torchlearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:40:30.000000 torchlearn-0.2.2/torchlearn/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 06:06:54.411058 torchlearn-0.2.2/torchlearn/metric/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1276 2023-06-24 05:40:27.000000 torchlearn-0.2.2/torchlearn/metric/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1257 2023-06-24 05:46:23.000000 torchlearn-0.2.2/torchlearn/metric/average_metric.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    15346 2023-06-24 05:45:32.000000 torchlearn-0.2.2/torchlearn/metric/classification.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      545 2023-06-24 05:54:59.000000 torchlearn-0.2.2/torchlearn/metric/loss.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      384 2023-05-23 18:21:28.000000 torchlearn-0.2.2/torchlearn/metric/metric.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      887 2023-06-08 12:01:57.000000 torchlearn-0.2.2/torchlearn/metric/metric_dict.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2638 2023-05-23 18:21:28.000000 torchlearn-0.2.2/torchlearn/metric/metric_value.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2133 2023-06-24 05:44:27.000000 torchlearn-0.2.2/torchlearn/metric/state.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 06:06:54.411058 torchlearn-0.2.2/torchlearn/model/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      227 2023-06-24 05:41:00.000000 torchlearn-0.2.2/torchlearn/model/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      557 2023-06-08 12:01:57.000000 torchlearn-0.2.2/torchlearn/model/classifier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1146 2023-06-08 12:01:57.000000 torchlearn-0.2.2/torchlearn/model/mlp.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      796 2023-06-08 12:01:57.000000 torchlearn-0.2.2/torchlearn/model/perceptron.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 06:06:54.411058 torchlearn-0.2.2/torchlearn/objective/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      247 2023-06-24 05:41:32.000000 torchlearn-0.2.2/torchlearn/objective/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1507 2023-05-23 18:21:28.000000 torchlearn-0.2.2/torchlearn/objective/objective.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3598 2023-06-24 06:03:05.000000 torchlearn-0.2.2/torchlearn/objective/pareto.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 06:06:54.411058 torchlearn-0.2.2/torchlearn/processing/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      253 2023-06-24 05:40:27.000000 torchlearn-0.2.2/torchlearn/processing/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5011 2023-06-24 05:36:29.000000 torchlearn-0.2.2/torchlearn/processing/graph.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 06:06:54.421058 torchlearn-0.2.2/torchlearn/training/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      469 2023-06-24 05:40:27.000000 torchlearn-0.2.2/torchlearn/training/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      370 2023-06-24 05:37:08.000000 torchlearn-0.2.2/torchlearn/training/callback.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1753 2023-06-08 12:01:57.000000 torchlearn-0.2.2/torchlearn/training/early_stopping.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1860 2023-06-24 05:40:11.000000 torchlearn-0.2.2/torchlearn/training/pareto.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1808 2023-06-24 05:47:33.000000 torchlearn-0.2.2/torchlearn/training/results.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      225 2023-05-23 18:21:28.000000 torchlearn-0.2.2/torchlearn/training/schedulers.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6456 2023-06-08 12:01:57.000000 torchlearn-0.2.2/torchlearn/training/trainer.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 06:06:54.421058 torchlearn-0.2.2/torchlearn/utils/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      384 2023-06-24 05:41:18.000000 torchlearn-0.2.2/torchlearn/utils/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      738 2023-05-23 18:21:28.000000 torchlearn-0.2.2/torchlearn/utils/arguments.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2614 2023-06-24 05:37:08.000000 torchlearn-0.2.2/torchlearn/utils/graph.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      239 2023-05-23 18:21:28.000000 torchlearn-0.2.2/torchlearn/utils/numbers.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 06:06:54.411058 torchlearn-0.2.2/torchlearn.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    14853 2023-06-24 06:06:54.000000 torchlearn-0.2.2/torchlearn.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1151 2023-06-24 06:06:54.000000 torchlearn-0.2.2/torchlearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-24 06:06:54.000000 torchlearn-0.2.2/torchlearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       96 2023-06-24 06:06:54.000000 torchlearn-0.2.2/torchlearn.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       22 2023-06-24 06:06:54.000000 torchlearn-0.2.2/torchlearn.egg-info/top_level.txt
```

### Comparing `torchlearn-0.2.1/LICENSE` & `torchlearn-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/PKG-INFO` & `torchlearn-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlearn
-Version: 0.2.1
+Version: 0.2.2
 Author-email: Vincent Coriou <vincent.coriou@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `torchlearn-0.2.1/README.md` & `torchlearn-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/pyproject.toml` & `torchlearn-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/metric/__init__.py` & `torchlearn-0.2.2/torchlearn/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/metric/average_metric.py` & `torchlearn-0.2.2/torchlearn/metric/average_metric.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/metric/classification.py` & `torchlearn-0.2.2/torchlearn/metric/classification.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/metric/loss.py` & `torchlearn-0.2.2/torchlearn/metric/loss.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/metric/metric_dict.py` & `torchlearn-0.2.2/torchlearn/metric/metric_dict.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/metric/metric_value.py` & `torchlearn-0.2.2/torchlearn/metric/metric_value.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/metric/state.py` & `torchlearn-0.2.2/torchlearn/metric/state.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/model/classifier.py` & `torchlearn-0.2.2/torchlearn/model/classifier.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/model/mlp.py` & `torchlearn-0.2.2/torchlearn/model/mlp.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/model/perceptron.py` & `torchlearn-0.2.2/torchlearn/model/perceptron.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/objective/objective.py` & `torchlearn-0.2.2/torchlearn/objective/objective.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/objective/pareto.py` & `torchlearn-0.2.2/torchlearn/objective/pareto.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 import os
 from pathlib import Path
 from typing import Any, Callable, List, Sequence, Set, Tuple, Union
 
 import pandas as pd
 import torch
-from matplotlib import Axes
+from matplotlib.axes import Axes
 from torch import Tensor
 
 from torchlearn.objective.objective import Objective
 
 PathLike = Union[str, os.PathLike[str]]
```

### Comparing `torchlearn-0.2.1/torchlearn/processing/graph.py` & `torchlearn-0.2.2/torchlearn/processing/graph.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/training/early_stopping.py` & `torchlearn-0.2.2/torchlearn/training/early_stopping.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/training/pareto.py` & `torchlearn-0.2.2/torchlearn/training/pareto.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/training/results.py` & `torchlearn-0.2.2/torchlearn/training/results.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/training/trainer.py` & `torchlearn-0.2.2/torchlearn/training/trainer.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/utils/arguments.py` & `torchlearn-0.2.2/torchlearn/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn/utils/graph.py` & `torchlearn-0.2.2/torchlearn/utils/graph.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.1/torchlearn.egg-info/PKG-INFO` & `torchlearn-0.2.2/torchlearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlearn
-Version: 0.2.1
+Version: 0.2.2
 Author-email: Vincent Coriou <vincent.coriou@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `torchlearn-0.2.1/torchlearn.egg-info/SOURCES.txt` & `torchlearn-0.2.2/torchlearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

