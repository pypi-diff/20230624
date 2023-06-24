# Comparing `tmp/torchlearn-0.2.0.tar.gz` & `tmp/torchlearn-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlearn-0.2.0.tar", last modified: Tue May 23 18:28:34 2023, max compression
+gzip compressed data, was "torchlearn-0.2.1.tar", last modified: Sat Jun 24 05:59:40 2023, max compression
```

## Comparing `torchlearn-0.2.0.tar` & `torchlearn-0.2.1.tar`

### file list

```diff
@@ -1,54 +1,52 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11344 2023-05-23 18:24:04.000000 torchlearn-0.2.0/LICENSE
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       69 2023-05-23 18:21:28.000000 torchlearn-0.2.0/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1848 2023-05-23 18:28:34.649558 torchlearn-0.2.0/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1390 2023-05-23 18:21:28.000000 torchlearn-0.2.0/README.md
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        5 2023-05-23 18:21:28.000000 torchlearn-0.2.0/VERSION
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    22727 2023-05-23 18:21:28.000000 torchlearn-0.2.0/pyproject.toml
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      158 2023-05-23 18:21:28.000000 torchlearn-0.2.0/requirements-dev.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       34 2023-05-23 18:21:35.000000 torchlearn-0.2.0/requirements.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      684 2023-05-23 18:28:34.649558 torchlearn-0.2.0/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      123 2023-05-23 18:21:28.000000 torchlearn-0.2.0/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/metric/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1089 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/average_metric.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    15375 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/classification.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      563 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/loss.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      384 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/metric.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      886 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/metric_dict.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2638 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/metric_value.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2039 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/state.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/model/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/model/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/model/classifier.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1182 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/model/mlp.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      826 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/model/perceptron.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/objective/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/objective/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1507 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/objective/objective.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3592 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/objective/pareto.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/processing/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/processing/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5011 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/processing/graph.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/training/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      366 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/callback.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1756 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/early_stopping.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1875 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/pareto.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1786 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/results.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      225 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/schedulers.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6408 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/trainer.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/utils/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/utils/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      738 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/utils/arguments.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2604 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/utils/graph.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      239 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/utils/numbers.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1848 2023-05-23 18:28:34.000000 torchlearn-0.2.0/torchlearn.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1203 2023-05-23 18:28:34.000000 torchlearn-0.2.0/torchlearn.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-23 18:28:34.000000 torchlearn-0.2.0/torchlearn.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-16 14:51:48.000000 torchlearn-0.2.0/torchlearn.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      201 2023-05-23 18:28:34.000000 torchlearn-0.2.0/torchlearn.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       11 2023-05-23 18:28:34.000000 torchlearn-0.2.0/torchlearn.egg-info/top_level.txt
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11344 2023-05-23 18:24:04.000000 torchlearn-0.2.1/LICENSE
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       69 2023-05-23 18:21:28.000000 torchlearn-0.2.1/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    14853 2023-06-24 05:59:40.180539 torchlearn-0.2.1/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1390 2023-06-07 15:43:16.000000 torchlearn-0.2.1/README.md
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        5 2023-06-24 05:50:07.000000 torchlearn-0.2.1/VERSION
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    23654 2023-06-24 05:58:51.000000 torchlearn-0.2.1/pyproject.toml
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       53 2023-06-24 05:33:22.000000 torchlearn-0.2.1/requirements-dev.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       34 2023-05-23 18:21:35.000000 torchlearn-0.2.1/requirements.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-06-24 05:59:40.180539 torchlearn-0.2.1/setup.cfg
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:40:30.000000 torchlearn-0.2.1/torchlearn/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/metric/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1276 2023-06-24 05:40:27.000000 torchlearn-0.2.1/torchlearn/metric/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1257 2023-06-24 05:46:23.000000 torchlearn-0.2.1/torchlearn/metric/average_metric.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    15346 2023-06-24 05:45:32.000000 torchlearn-0.2.1/torchlearn/metric/classification.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      545 2023-06-24 05:54:59.000000 torchlearn-0.2.1/torchlearn/metric/loss.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      384 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/metric/metric.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      887 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/metric/metric_dict.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2638 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/metric/metric_value.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2133 2023-06-24 05:44:27.000000 torchlearn-0.2.1/torchlearn/metric/state.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/model/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      227 2023-06-24 05:41:00.000000 torchlearn-0.2.1/torchlearn/model/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      557 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/model/classifier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1146 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/model/mlp.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      796 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/model/perceptron.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/objective/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      247 2023-06-24 05:41:32.000000 torchlearn-0.2.1/torchlearn/objective/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1507 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/objective/objective.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3593 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/objective/pareto.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/processing/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      253 2023-06-24 05:40:27.000000 torchlearn-0.2.1/torchlearn/processing/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5011 2023-06-24 05:36:29.000000 torchlearn-0.2.1/torchlearn/processing/graph.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/training/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      469 2023-06-24 05:40:27.000000 torchlearn-0.2.1/torchlearn/training/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      370 2023-06-24 05:37:08.000000 torchlearn-0.2.1/torchlearn/training/callback.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1753 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/training/early_stopping.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1860 2023-06-24 05:40:11.000000 torchlearn-0.2.1/torchlearn/training/pareto.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1808 2023-06-24 05:47:33.000000 torchlearn-0.2.1/torchlearn/training/results.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      225 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/training/schedulers.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6456 2023-06-08 12:01:57.000000 torchlearn-0.2.1/torchlearn/training/trainer.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn/utils/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      384 2023-06-24 05:41:18.000000 torchlearn-0.2.1/torchlearn/utils/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      738 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/utils/arguments.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2614 2023-06-24 05:37:08.000000 torchlearn-0.2.1/torchlearn/utils/graph.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      239 2023-05-23 18:21:28.000000 torchlearn-0.2.1/torchlearn/utils/numbers.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-24 05:59:40.180539 torchlearn-0.2.1/torchlearn.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    14853 2023-06-24 05:59:40.000000 torchlearn-0.2.1/torchlearn.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1151 2023-06-24 05:59:40.000000 torchlearn-0.2.1/torchlearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-24 05:59:40.000000 torchlearn-0.2.1/torchlearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       96 2023-06-24 05:59:40.000000 torchlearn-0.2.1/torchlearn.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       22 2023-06-24 05:59:40.000000 torchlearn-0.2.1/torchlearn.egg-info/top_level.txt
```

### Comparing `torchlearn-0.2.0/LICENSE` & `torchlearn-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.0/README.md` & `torchlearn-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.0/pyproject.toml` & `torchlearn-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,54 @@
 [build-system]
 requires = [
-    "setuptools>=62",
+    "setuptools",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
+[project]
+name = "torchlearn"
+description = ""
+authors = [
+    { name = "Vincent Coriou", email = "vincent.coriou@gmail.com" },
+]
+requires-python = "~=3.10"
+license = { file = "LICENSE" }
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+]
+dynamic = [
+    "version",
+    "dependencies",
+    "optional-dependencies",
+    "readme",
+]
+
+[tool.setuptools.packages.find]
+exclude = [
+    "CICD*",
+    "Docker*",
+    "docs*",
+    "Kubernetes",
+    "Makefiles*",
+    "tests*",
+]
+
+[tool.setuptools.dynamic]
+version = { file = "VERSION" }
+dependencies = { file = "requirements.txt" }
+optional-dependencies = { dev = { file = "requirements-dev.txt" } }
+readme = { file = "README.md", content-type = "text/markdown"}
+
+[project.urls]
+homepage = "https://github.com/VincentCoriou"
+repository = "https://github.com/VincentCoriou/torchlearn"
+
 
 [tool.black]
 line-length = 120
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
@@ -38,15 +78,15 @@
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
     "from",
     "import"
-    ]
+]
 
 [tool.pylint.main]
 # Analyse import fallback blocks. This can be used to support both Python 2 and 3
 # compatible code, which means that the block might have code that exists only in
 # one or another interpreter, leading to false positives when analysed.
 # analyse-fallback-blocks =
```

### Comparing `torchlearn-0.2.0/torchlearn/metric/average_metric.py` & `torchlearn-0.2.1/torchlearn/metric/average_metric.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """TODO average_metric docstring
 """
 from abc import ABC, abstractmethod
+from inspect import Signature, signature
 from typing import Any, Sequence
 
 from torch import Tensor
 
 from .metric import Metric
 
 
@@ -26,21 +27,24 @@
 
     def reset(self) -> None:
         self._value = 0
         self._counter = 0
 
     @staticmethod
     @abstractmethod
-    def compute(*args: Any) -> Tensor:
+    def compute(*args: Any, **kwargs: Any) -> Tensor:
         raise NotImplementedError
 
     @staticmethod
     @abstractmethod
-    def compute_size(*args: Any) -> int:
+    def compute_size(*args: Any, **kwargs: Any) -> int:
         raise NotImplementedError
 
-    def update(self, *args: Any) -> Tensor:  # type: ignore
-        value = self.compute(*args)
-        size = self.compute_size(*args)
+    def update(self, *args: Any, **kwargs: Any) -> Tensor:
+        value = self.compute(*args, **kwargs)
+        size = self.compute_size(*args, **kwargs)
         self._value += value.mean().item() * size
         self._counter += size
         return value
+
+    def signature(self) -> Signature:
+        return signature(self.compute)
```

### Comparing `torchlearn-0.2.0/torchlearn/metric/classification.py` & `torchlearn-0.2.1/torchlearn/metric/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 """TODO confusion_matrix docstring
 """
 from abc import ABC
 from functools import partial
-from typing import Optional, Tuple, Type, Dict, Callable, Any, KeysView
+from typing import Any, Callable, Dict, KeysView, Optional, Tuple, Type
 
 import torch
-from torch import Tensor, LongTensor
+from torch import LongTensor, Tensor
 
 from torchlearn.metric.metric_value import MetricValue
 from torchlearn.metric.state import State
 
 
 class ConfusionMatrix(State):
     """TODO ConfusionMatrix docstring"""
 
     _num_classes: int
     _confusion_matrix: LongTensor
 
     metrics: Dict[str, Type["ClassificationMetric"]] = {}
 
     @classmethod
-    def register_metric(cls, metric: Type["ClassificationMetric"], name: Optional[str] = None) -> Type[
-        "ClassificationMetric"]:
+    def register_metric(
+        cls, metric: Type["ClassificationMetric"], name: Optional[str] = None
+    ) -> Type["ClassificationMetric"]:
         if name is None:
             name = metric.__name__
         if name in cls.metrics:
             raise NameError(f"Metric {name} is already registered.")
         cls.metrics[name] = metric
         return metric
 
     @classmethod
-    def register(cls, name: Optional[str] = None) -> Callable[
-        [Type["ClassificationMetric"]], Type["ClassificationMetric"]]:
+    def register(
+        cls, name: Optional[str] = None
+    ) -> Callable[[Type["ClassificationMetric"]], Type["ClassificationMetric"]]:
         return partial(cls.register_metric, name=name)
 
     def get_metric(self, name: str, *args: Any, **kwargs: Any) -> "ClassificationMetric":
         return self.metrics[name](self, *args, **kwargs)
 
     def get_metrics(self) -> KeysView[str]:
         return self.metrics.keys()
@@ -44,21 +46,21 @@
         super().__init__(parameters)
         self._num_classes = num_classes
         self._confusion_matrix = torch.empty(num_classes, num_classes).long()  # type: ignore
 
     def reset(self) -> None:
         self._confusion_matrix.zero_()
 
-    def update(self, predicted: LongTensor, target: LongTensor) -> Tensor:  # type: ignore
+    def update(self, predicted: LongTensor, target: LongTensor) -> Tensor:
         confusion_matrix = self.compute(predicted, target, self._num_classes)
-        self._confusion_matrix += confusion_matrix # type: ignore
+        self._confusion_matrix += confusion_matrix  # type: ignore
         return confusion_matrix
 
     @staticmethod
-    def compute(predicted: LongTensor, target: LongTensor, num_classes: int) -> LongTensor:  # type: ignore
+    def compute(predicted: LongTensor, target: LongTensor, num_classes: int) -> LongTensor:
         confusion_matrix = torch.zeros(num_classes, num_classes).long()
         values = torch.ones(()).long()
         confusion_matrix.index_put_((target, predicted), values, accumulate=True)
         return confusion_matrix  # type: ignore
 
     @property
     def num_classes(self) -> int:
@@ -131,16 +133,16 @@
 
 class ClassificationMetric(MetricValue, ABC):
     """TODO ClassificationMetric docstring"""
 
     _confusion_matrix: ConfusionMatrix
 
     def __init__(
-            self,
-            confusion_matrix: ConfusionMatrix,
+        self,
+        confusion_matrix: ConfusionMatrix,
     ) -> None:
         super().__init__()
         self._confusion_matrix = confusion_matrix
 
 
 class ClassMetric(ClassificationMetric, ABC):
     """TODO ClassMetric docstring"""
@@ -278,15 +280,15 @@
         return self._confusion_matrix.sensitivity(self._class).item()
 
     @staticmethod
     def compute(confusion_matrix: LongTensor, class_: Optional[int] = None) -> Tensor:
         rel = Relevant.compute(confusion_matrix, class_)
         tp = TruePositive.compute(confusion_matrix, class_)
         sen = tp / rel
-        sen[rel == 0] = 0.
+        sen[rel == 0] = 0.0
         return sen
 
 
 @ConfusionMatrix.register()
 class Specificity(ClassMetric):
     """TODO Specificity docstring"""
 
@@ -322,15 +324,15 @@
         return self._confusion_matrix.precision(self._class).item()
 
     @staticmethod
     def compute(confusion_matrix: LongTensor, class_: Optional[int] = None) -> Tensor:
         ret = Retrieved.compute(confusion_matrix, class_)
         tp = TruePositive.compute(confusion_matrix, class_)
         pre = tp / ret
-        pre[ret == 0] = 0.
+        pre[ret == 0] = 0.0
         return pre
 
 
 @ConfusionMatrix.register()
 class Recall(ClassMetric):
     """TODO Recall docstring"""
 
@@ -338,35 +340,35 @@
         return self._confusion_matrix.recall(self._class).item()
 
     @staticmethod
     def compute(confusion_matrix: LongTensor, class_: Optional[int] = None) -> Tensor:
         rel = Relevant.compute(confusion_matrix, class_)
         tp = TruePositive.compute(confusion_matrix, class_)
         rec = tp / rel
-        rec[rel == 0] = 0.
+        rec[rel == 0] = 0.0
         return rec
 
 
 @ConfusionMatrix.register()
 class FScore(ClassMetric):
     """TODO FScore docstring"""
 
-    def __init__(self, confusion_matrix: ConfusionMatrix, class_: int, beta: float = 1.) -> None:
+    def __init__(self, confusion_matrix: ConfusionMatrix, class_: int, beta: float = 1.0) -> None:
         super().__init__(confusion_matrix, class_)
         self._beta = beta
 
     def value(self) -> float:
         return self._confusion_matrix.fscore(self._beta, self._class).item()
 
     @staticmethod
     def compute(confusion_matrix: LongTensor, beta: float, class_: Optional[int] = None) -> Tensor:
         tp = TruePositive.compute(confusion_matrix, class_)
         fn = FalseNegative.compute(confusion_matrix, class_)
         fp = FalsePositive.compute(confusion_matrix, class_)
-        fs = (1 + beta ** 2) * tp / ((1 + beta ** 2) * tp + beta ** 2 * fn + fp)
+        fs = (1 + beta**2) * tp / ((1 + beta**2) * tp + beta**2 * fn + fp)
         fs[(tp == 0) & (fn == 0) & (fp == 0)] = 0
         return fs
 
 
 @ConfusionMatrix.register()
 class WeightedPrecision(ClassificationMetric):
     """TODO WeightedPrecision docstring"""
@@ -393,15 +395,15 @@
         return _weighted_avg(confusion_matrix, rec)
 
 
 @ConfusionMatrix.register()
 class WeightedFScore(ClassificationMetric):
     """TODO WeightedFScore docstring"""
 
-    def __init__(self, confusion_matrix: ConfusionMatrix, beta: float = 1.) -> None:
+    def __init__(self, confusion_matrix: ConfusionMatrix, beta: float = 1.0) -> None:
         super().__init__(confusion_matrix)
         self._beta = beta
 
     def value(self) -> float:
         return self._confusion_matrix.weighted_fscore(self._beta).item()
 
     @staticmethod
@@ -436,15 +438,15 @@
         return _macro_avg(confusion_matrix, rec)
 
 
 @ConfusionMatrix.register()
 class MacroFScore(ClassificationMetric):
     """TODO MacroFScore docstring"""
 
-    def __init__(self, confusion_matrix: ConfusionMatrix, beta: float = 1.) -> None:
+    def __init__(self, confusion_matrix: ConfusionMatrix, beta: float = 1.0) -> None:
         super().__init__(confusion_matrix)
         self._beta = beta
 
     def value(self) -> float:
         return self._confusion_matrix.macro_fscore(self._beta).item()
 
     @staticmethod
```

### Comparing `torchlearn-0.2.0/torchlearn/metric/loss.py` & `torchlearn-0.2.1/torchlearn/metric/loss.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Loss(AverageMetric):
     """TODO Loss docstring"""
 
     def __init__(self, name: str = "loss", size_name: str = "batch_size") -> None:
         super().__init__((name, size_name))
 
     @staticmethod
-    def compute(loss: Tensor, batch_size: int) -> Any: # type: ignore
+    def compute(loss: Tensor, batch_size: int) -> Any:
         del batch_size
         return loss
 
     @staticmethod
-    def compute_size(loss: Tensor, size: int) -> int: # type: ignore
+    def compute_size(loss: Tensor, batch_size: int) -> int:
         del loss
-        return size
+        return batch_size
```

### Comparing `torchlearn-0.2.0/torchlearn/metric/metric_dict.py` & `torchlearn-0.2.1/torchlearn/metric/metric_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from torchlearn.metric.metric_value import MetricValue
 from torchlearn.metric.state import State
 
 
 class MetricDict(dict):
     """TODO MetricDict docstring"""
+
     _states: FrozenSet[State]
     _parameters: FrozenSet[str]
 
     def __init__(self, **metrics: MetricValue) -> None:
         super().__init__(**metrics)
         self._states = reduce(or_, (set(v.states()) for v in metrics.values()), frozenset())
         self._parameters = reduce(or_, (set(v.parameters) for v in self._states), frozenset())
```

### Comparing `torchlearn-0.2.0/torchlearn/metric/metric_value.py` & `torchlearn-0.2.1/torchlearn/metric/metric_value.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.0/torchlearn/metric/state.py` & `torchlearn-0.2.1/torchlearn/metric/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """TODO metric_state docstring
 """
-import inspect
 from abc import ABC, abstractmethod
-from typing import Any, Mapping, Sequence, Union, Optional
+from inspect import Signature, signature
+from typing import Any, Mapping, Optional, Sequence, Union
 
 import torch
 
 
 class State(ABC):
     """TODO MetricState docstring"""
 
     _parameters: Sequence[str]
 
     def __init__(self, parameters: Optional[Sequence[str]] = None) -> None:
-        signature = inspect.signature(self.update)
+        sig = self.signature()
         if parameters is None:
-            parameters = list(signature.parameters)
+            parameters = list(sig.parameters)
 
-        if len(parameters) != len(signature.parameters):
+        if len(parameters) != len(sig.parameters):
             raise ValueError(
-                f"State expects {len(signature.parameters)} parameters ({signature.parameters}),"
-                f"but only {len(parameters)} parameters were given ({parameters}).")
+                f"State expects {len(sig.parameters)} parameters ({sig.parameters}),"
+                f"but {len(parameters)} parameters were given ({parameters})."
+            )
 
         self._parameters = tuple(parameters)
 
     @torch.no_grad()
     def __call__(self, kwargs: Mapping[str, Any]) -> Any:
         kwargs = {name: kwargs[name] for name in self.parameters if name in kwargs}
         return self.update(**kwargs)
@@ -34,20 +35,20 @@
         return self._parameters
 
     @abstractmethod
     def reset(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def update(self, **kwargs: Any) -> Any:
+    def update(self, *args: Any, **kwargs: Any) -> Any:
         pass
 
     @staticmethod
     @abstractmethod
-    def compute(*args: Any) -> Any:
+    def compute(*args: Any, **kwargs: Any) -> Any:
         pass
 
     def process(self, outputs: Union[Sequence[Any], Mapping[str, Any]]) -> Any:
         if isinstance(outputs, Mapping):
             try:
                 outputs = tuple(outputs[a] for a in self._parameters)
             except KeyError as exception:
@@ -56,7 +57,10 @@
                     f"Missing key from output: expected '{key}' to be present, but only found {tuple(outputs)}."
                 ) from exception
         if len(outputs) != len(self._parameters):
             raise ValueError(
                 f"Argument mismatch: expected {len(self._parameters)} " f"arguments, but got {len(outputs)} arguments."
             )
         return self.update(*outputs)
+
+    def signature(self) -> Signature:
+        return signature(self.update)
```

### Comparing `torchlearn-0.2.0/torchlearn/model/classifier.py` & `torchlearn-0.2.1/torchlearn/model/classifier.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """TODO
 """
 from typing import Any
 
 import torch
-from torch import nn, Tensor, LongTensor
+from torch import LongTensor, Tensor, nn
 
 
 class Classifier(nn.Module):
     """TODO"""
 
     def __init__(self, model: nn.Module) -> None:
         super().__init__()
@@ -17,8 +17,8 @@
         return self.model(*args)  # type: ignore
 
     def predict(self, *args: Any) -> LongTensor:
         return self.classify(self(*args))
 
     @classmethod
     def classify(cls, outputs: Tensor) -> LongTensor:
-        return torch.argmax(outputs, -1) # type: ignore
+        return torch.argmax(outputs, -1)  # type: ignore
```

### Comparing `torchlearn-0.2.0/torchlearn/model/mlp.py` & `torchlearn-0.2.1/torchlearn/model/mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """TODO
 """
-from typing import Optional, Type, Sequence
+from typing import Optional, Sequence, Type
 
 import torch
 from torch import nn
 
 from torchlearn.model.perceptron import Perceptron
 from torchlearn.utils.arguments import expand_list
 
 
 class MultiLayerPerceptron(nn.Sequential):
     """TODO"""
 
     def __init__(
-            self,
-            input_size: int,
-            output_size: int,
-            num_layers: int,
-            hidden_units: int | Sequence[int],
-            activation: nn.Module | Type[nn.Module] = nn.ReLU,
-            dropout: float | Sequence[float] = 0.0,
-            bias: bool = True,
-            device: Optional[torch.device] = None,
+        self,
+        input_size: int,
+        output_size: int,
+        num_layers: int,
+        hidden_units: int | Sequence[int],
+        activation: nn.Module | Type[nn.Module] = nn.ReLU,
+        dropout: float | Sequence[float] = 0.0,
+        bias: bool = True,
+        device: Optional[torch.device] = None,
     ) -> None:
         hidden_units = expand_list(num_layers, hidden_units)
         sizes = (input_size, *hidden_units)
         activations = expand_list(num_layers, activation)
         dropouts = expand_list(num_layers, dropout)
         input_sizes = sizes[:-1]
         output_sizes = sizes[1:]
```

### Comparing `torchlearn-0.2.0/torchlearn/model/perceptron.py` & `torchlearn-0.2.1/torchlearn/model/perceptron.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """TODO
 """
-from typing import Any, Optional, Type, List
+from typing import Any, List, Optional, Type
 
 import torch
 from torch import nn
 
 
 class Perceptron(nn.Sequential):
     """TODO"""
 
     def __init__(
-            self,
-            in_size: int,
-            out_size: int,
-            activation: Optional[nn.Module | Type[nn.Module]] = None,
-            bias: bool = True,
-            device: Optional[torch.device] = None,
-            dropout: float = 0.,
-            **kwargs: Any
+        self,
+        in_size: int,
+        out_size: int,
+        activation: Optional[nn.Module | Type[nn.Module]] = None,
+        bias: bool = True,
+        device: Optional[torch.device] = None,
+        dropout: float = 0.0,
+        **kwargs: Any,
     ) -> None:
         modules: List[nn.Module] = [nn.Linear(in_size, out_size, bias=bias, device=device)]
         if activation is not None:
             if isinstance(activation, type):
                 activation = activation(**kwargs)
             modules.append(activation)
         if dropout > 0:
```

### Comparing `torchlearn-0.2.0/torchlearn/objective/objective.py` & `torchlearn-0.2.1/torchlearn/objective/objective.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.0/torchlearn/objective/pareto.py` & `torchlearn-0.2.1/torchlearn/objective/pareto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """TODO
 """
 import os
 from pathlib import Path
-from typing import Sequence, Callable, List, Set, Tuple, Any, Union
+from typing import Any, Callable, List, Sequence, Set, Tuple, Union
 
 import pandas as pd
 import torch
 from matplotlib import Axes
 from torch import Tensor
 
 from torchlearn.objective.objective import Objective
@@ -24,14 +24,15 @@
         b[..., :] = o.better_fn(s1i, s2i)
         s[..., :] = o.same_fn(s1i, s2i)
     return better.any(-1) & same.all(-1)
 
 
 class ParetoSet:
     """TODO"""
+
     all_solutions: List[Tensor]
     pareto_set: Set[int]
     objectives: Sequence[Objective]
 
     def __init__(self, objectives: Sequence[Objective]):
         self.all_solutions = []
         self.pareto_set = set()
```

### Comparing `torchlearn-0.2.0/torchlearn/processing/graph.py` & `torchlearn-0.2.1/torchlearn/processing/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """TODO
 """
 
-from typing import Dict, Any, Union, Sequence, Callable, Mapping, Optional, Tuple, Protocol, TypeVar
+from typing import Any, Callable, Dict, Mapping, Optional, Protocol, Sequence, Tuple, TypeVar, Union
 
 from torch import nn
 
 from torchlearn.utils.graph import Graph
 
 
 class ProcessingValues:
@@ -88,15 +88,15 @@
 class ProcessingGraph:
     """TODO"""
 
     graph: Graph
     nodes: Mapping[str, ProcessingNode]
 
     def __init__(
-            self, *, inputs: Sequence[str], functions: Sequence[_GraphFunction], constants: Optional[_Constants] = None
+        self, *, inputs: Sequence[str], functions: Sequence[_GraphFunction], constants: Optional[_Constants] = None
     ):
         inputs = tuple(inputs)
         processing_nodes = tuple(
             ProcessingNode(*data) if not isinstance(data, ProcessingNode) else data for data in functions
         )
         nodes = {o: n for n in processing_nodes for o in n.outputs}
         if constants is None:
@@ -148,13 +148,13 @@
 
     def get_outputs(self, *outputs: str) -> Mapping[str, Any]:
         if len(outputs) == 0:
             outputs = tuple(self.nodes)
         return {a: self.values[a] for a in outputs}
 
 
-T_contra = TypeVar("T_contra", bound=nn.Module, contravariant=True)
+_T_contra = TypeVar("_T_contra", bound=nn.Module, contravariant=True)
 
 
-class ProcessingFunction(Protocol[T_contra]):
-    def __call__(self, model: T_contra, *args: Any, **kwargs: Any) -> ProcessingGraph:
+class ProcessingFunction(Protocol[_T_contra]):
+    def __call__(self, model: _T_contra, *args: Any, **kwargs: Any) -> ProcessingGraph:
         pass
```

### Comparing `torchlearn-0.2.0/torchlearn/training/early_stopping.py` & `torchlearn-0.2.1/torchlearn/training/early_stopping.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """TODO
 """
 from abc import abstractmethod
-from typing import Mapping
-from typing import Optional
+from typing import Mapping, Optional
 
 import torch
 
 from torchlearn.objective.objective import Objective
 from torchlearn.training.results import Result
 
 
@@ -15,20 +14,22 @@
     def step(self, epoch: int, train_result: Result, validation_result: Optional[Result] = None) -> bool:
         pass
 
 
 class Patience(EarlyStopping):
     """TODO"""
 
-    def __init__(self, patience: int, objective: Objective | Mapping[str, str], validation: bool = False,
-                 threshold: float = 0.) -> None:
+    def __init__(
+        self, patience: int, objective: Objective | Mapping[str, str], validation: bool = False, threshold: float = 0.0
+    ) -> None:
         if isinstance(objective, Mapping):
             if not len(objective) == 1:
                 raise ValueError(
-                    f"Early stopping expects only 1 objective, but {len(objective)} were given: '{objective}'.")
+                    f"Early stopping expects only 1 objective, but {len(objective)} were given: '{objective}'."
+                )
             name, config = next(iter(objective.items()))
             obj = Objective.from_config(name, config)
         else:
             obj = objective
         self.patience = patience
         self.objective = obj
         self.validation = validation
```

### Comparing `torchlearn-0.2.0/torchlearn/training/pareto.py` & `torchlearn-0.2.1/torchlearn/training/pareto.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """TODO
 """
 import os
 from pathlib import Path
-from typing import Sequence, Callable, Union
+from typing import Callable, Sequence, Union
 
 import torch
-from torch import Tensor
-from torch import nn
+from torch import Tensor, nn
 
 from torchlearn.objective.objective import Objective
 from torchlearn.objective.pareto import ParetoSet
 from torchlearn.training.results import Result
 
-PathLike = Union[str, os.PathLike[str]]
+_PathLike = Union[str, os.PathLike[str]]
 
 
 class ParetoManager:
     """TODO"""
 
-    def __init__(self, *path: PathLike, objectives: Sequence[Objective], validation: bool = False) -> None:
+    def __init__(self, *path: _PathLike, objectives: Sequence[Objective], validation: bool = False) -> None:
         self.path = Path(*path)
         self.objectives = objectives
         self.validation = validation
         self.pareto_set = ParetoSet(objectives)
 
         self.path.mkdir(parents=True, exist_ok=False)
```

### Comparing `torchlearn-0.2.0/torchlearn/training/results.py` & `torchlearn-0.2.1/torchlearn/training/results.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 """TODO
 """
 import os
 from pathlib import Path
-from typing import Mapping, Union, Dict
+from typing import Dict, Mapping, Union
 
 import pandas as pd
 
 from torchlearn.metric.metric_value import MetricValue
 
-PathLike = Union[str, os.PathLike]
+_PathLike = Union[str, os.PathLike]
 
 
 class EpochResult:
     """TODO"""
+
     metrics: Mapping[str, MetricValue]
 
     def __init__(self, metrics: Mapping[str, MetricValue]) -> None:
         self.metrics = metrics
 
     def values(self, prefix: str = "") -> Mapping[str, float]:
         return {prefix + n: m.value() for n, m in self.metrics.items()}
 
     def to_pandas(self) -> pd.Series:
         return pd.Series({n: m.value() for n, m in self.metrics.items()})
 
-    def save(self, *segments: PathLike) -> None:
+    def save(self, *segments: _PathLike) -> None:
         path = Path(*segments)
         self.to_pandas().to_csv(path)
 
 
 class Result:
     """TODO"""
+
     results: Dict[int, Mapping[str, float]]
 
     def __init__(self) -> None:
         self.results = {}
 
     def add(self, epoch: int, result: EpochResult) -> None:
         self.results[epoch] = result.values()
 
     def to_pandas(self) -> pd.DataFrame:
         return pd.DataFrame.from_dict(self.results, orient="index")
 
     @classmethod
     def from_pandas(cls, df: pd.DataFrame) -> "Result":
         result = cls()
-        result.results = df.to_dict(orient="index")
+        result.results = df.to_dict(orient="index")  # type: ignore
         return result
 
-    def save(self, *segments: PathLike) -> None:
+    def save(self, *segments: _PathLike) -> None:
         path = Path(*segments)
         self.to_pandas().to_csv(path)
 
     @classmethod
-    def load(cls, *segments: PathLike) -> "Result":
+    def load(cls, *segments: _PathLike) -> "Result":
         path = Path(*segments)
         df = pd.read_csv(path, index_col=0)
         return cls.from_pandas(df)
 
     def __getitem__(self, epoch: int) -> Mapping[str, float]:
         return self.results[epoch]
```

### Comparing `torchlearn-0.2.0/torchlearn/training/trainer.py` & `torchlearn-0.2.1/torchlearn/training/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 """TODO
 """
-from typing import Sequence, Type, Union, Optional, Any, Mapping, Dict, Sized
+from typing import Any, Dict, Mapping, Optional, Sequence, Sized, Type, Union
 
 import torch
 from torch import nn
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader
 from tqdm.autonotebook import tqdm
 
 from torchlearn.metric.metric_dict import MetricDict
 from torchlearn.metric.metric_value import MetricValue
-from torchlearn.processing.graph import ProcessingGraph, ProcessingFunction
+from torchlearn.processing.graph import ProcessingFunction, ProcessingGraph
 from torchlearn.training.callback import Callback
 from torchlearn.training.early_stopping import EarlyStopping
-from torchlearn.training.results import Result, EpochResult
+from torchlearn.training.results import EpochResult, Result
 from torchlearn.training.schedulers import Scheduler
 
 
 class Trainer:
     """TODO"""
+
     device: Optional[torch.device]
     model: nn.Module
     optimizer: Optimizer
 
-    def __init__(self, model: nn.Module, optimizer: Union[Type[Optimizer], Optimizer], *args: Any,
-                 device: Optional[torch.device] = None, **kwargs: Any) -> None:
+    def __init__(
+        self,
+        model: nn.Module,
+        optimizer: Union[Type[Optimizer], Optimizer],
+        *args: Any,
+        device: Optional[torch.device] = None,
+        **kwargs: Any,
+    ) -> None:
         if device is not None:
             model = model.to(device)
         self.device = device
         self.model = model
         if isinstance(optimizer, type):
             optimizer = optimizer(model.parameters(), *args, **kwargs)
         self.optimizer = optimizer
 
-    def train(self, processing_function: ProcessingFunction, epochs: int,
-              train_dataloader: DataLoader,
-              val_dataloader: Optional[DataLoader] = None, schedulers: Sequence[Scheduler] = (),
-              callbacks: Sequence[Callback] = (),
-              metrics: Optional[MetricDict | Mapping[str, MetricValue]] = None,
-              val_metrics: Optional[MetricDict | Mapping[str, MetricValue]] = None,
-              early_stopping: Optional[EarlyStopping] = None,
-              trace: bool = False,
-              progress: bool = True,
-              show_metrics: bool = True) -> Sequence[Result]:
+    def train(
+        self,
+        processing_function: ProcessingFunction,
+        epochs: int,
+        train_dataloader: DataLoader,
+        val_dataloader: Optional[DataLoader] = None,
+        schedulers: Sequence[Scheduler] = (),
+        callbacks: Sequence[Callback] = (),
+        metrics: Optional[MetricDict | Mapping[str, MetricValue]] = None,
+        val_metrics: Optional[MetricDict | Mapping[str, MetricValue]] = None,
+        early_stopping: Optional[EarlyStopping] = None,
+        trace: bool = False,
+        progress: bool = True,
+        show_metrics: bool = True,
+    ) -> Sequence[Result]:
         if metrics is None:
             metrics = {}
         if not isinstance(metrics, MetricDict):
             metrics = MetricDict(**metrics)
         if val_metrics is None:
             val_metrics = metrics
         if not isinstance(val_metrics, MetricDict):
@@ -65,16 +77,17 @@
                 for epoch in pbar:
                     train_result = self.training(processing_graph, train_dataloader, metrics, progress, show_metrics)
                     train_results.add(epoch, train_result)
                     if show_metrics:
                         postfix.update(train_result.values())
                         pbar.set_postfix(ordered_dict=postfix)
                     if val_dataloader is not None:
-                        valid_result = self.evaluate(processing_graph, val_dataloader, val_metrics, progress,
-                                                     show_metrics)
+                        valid_result = self.evaluate(
+                            processing_graph, val_dataloader, val_metrics, progress, show_metrics
+                        )
                         valid_results.add(epoch, valid_result)
                         if show_metrics:
                             postfix.update(valid_result.values("val_"))
                             pbar.set_postfix(ordered_dict=postfix)
                     for scheduler in schedulers:
                         scheduler.step(self.model, epoch)
                     for callback in callbacks:
@@ -82,26 +95,30 @@
                     if early_stopping is not None and early_stopping.step(epoch, *results):
                         pbar.set_description(f"Early stopping (Epoch {epoch}/{epochs})")
                         break
             except KeyboardInterrupt:
                 pass
         return results
 
-    def training(self, processing_graph: ProcessingGraph, dataloader: DataLoader, metrics: MetricDict,
-                 progress: bool = True,
-                 show_metrics: bool = True) -> EpochResult:
+    def training(
+        self,
+        processing_graph: ProcessingGraph,
+        dataloader: DataLoader,
+        metrics: MetricDict,
+        progress: bool = True,
+        show_metrics: bool = True,
+    ) -> EpochResult:
         optimizer = self.optimizer
         self.model.train()
         epoch_metrics = EpochResult(metrics)
         states = metrics.states
         metrics.reset()
         parameters = metrics.parameters | {"loss", "batch_size"}
         sized = len(dataloader.dataset) if isinstance(dataloader.dataset, Sized) else None
-        with tqdm(dataloader, desc="Training", leave=False, disable=not progress,
-                  total=sized) as pbar:
+        with tqdm(dataloader, desc="Training", leave=False, disable=not progress, total=sized) as pbar:
             for batch in pbar:
                 batch = tuple(t.to(self.device) for t in batch)
                 outputs = processing_graph(*parameters, inputs=batch)
                 optimizer.zero_grad()
                 outputs["loss"].backward()
                 optimizer.step()
                 for s in states:
@@ -109,25 +126,30 @@
                 if sized:
                     pbar.update(outputs["batch_size"])
                 if show_metrics:
                     pbar.set_postfix(epoch_metrics.values())
         return epoch_metrics
 
     @torch.no_grad()
-    def evaluate(self, processing_graph: ProcessingGraph, dataloader: DataLoader, metrics: MetricDict,
-                 progress: bool = True, show_metrics: bool = True) -> EpochResult:
+    def evaluate(
+        self,
+        processing_graph: ProcessingGraph,
+        dataloader: DataLoader,
+        metrics: MetricDict,
+        progress: bool = True,
+        show_metrics: bool = True,
+    ) -> EpochResult:
         model = self.model
         model.eval()
         epoch_metrics = EpochResult(metrics)
         states = metrics.states
         metrics.reset()
         parameters = metrics.parameters | {"batch_size"}
         sized = len(dataloader.dataset) if isinstance(dataloader.dataset, Sized) else None
-        with tqdm(dataloader, desc="Evaluating", leave=False, disable=not progress,
-                  total=sized) as pbar:
+        with tqdm(dataloader, desc="Evaluating", leave=False, disable=not progress, total=sized) as pbar:
             for batch in pbar:
                 batch = tuple(t.to(self.device) for t in batch)
                 outputs = processing_graph(*parameters, inputs=batch)
                 for s in states:
                     s(outputs)
                 if sized:
                     pbar.update(outputs["batch_size"])
```

### Comparing `torchlearn-0.2.0/torchlearn/utils/arguments.py` & `torchlearn-0.2.1/torchlearn/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `torchlearn-0.2.0/torchlearn/utils/graph.py` & `torchlearn-0.2.1/torchlearn/utils/graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """TODO
 """
 import itertools
-from typing import Union, Sequence, Tuple, Generic, TypeVar, Hashable, Iterator
+from typing import Generic, Hashable, Iterator, Sequence, Tuple, TypeVar, Union
 
 import torch
 from torch import Tensor
 
-T = TypeVar("T", bound=Hashable)
-Edge = Union[Tuple[T, T], Tuple[T, T, float]]
+_T = TypeVar("_T", bound=Hashable)
+Edge = Union[Tuple[_T, _T], Tuple[_T, _T, float]]
 
 
 class CyclicGraphException(BaseException):
     pass
 
 
-class Graph(Generic[T]):
+class Graph(Generic[_T]):
     """TODO"""
 
-    nodes: Sequence[T]
+    nodes: Sequence[_T]
     n: int
     adjacency: torch.Tensor
 
-    def __init__(self, nodes: Sequence[T], adjacency: torch.Tensor) -> None:
+    def __init__(self, nodes: Sequence[_T], adjacency: torch.Tensor) -> None:
         for x, y in itertools.combinations(nodes, 2):
             if x == y:
                 raise ValueError(f"Duplicated node found: '{x}'")
         n = len(nodes)
         if adjacency.size() != (n, n):
             raise ValueError(
                 f"Expected square adjacency matrix of size ({n}, {n}) but found {tuple(adjacency.size())}."
             )
         self.nodes = nodes
         self.n = len(nodes)
         self.adjacency = adjacency
 
     @classmethod
-    def from_edge_list(cls, nodes: Sequence[T], edges: Sequence[Edge]) -> "Graph":
+    def from_edge_list(cls, nodes: Sequence[_T], edges: Sequence[Edge]) -> "Graph":
         n = len(nodes)
         adjacency = torch.zeros(n, n)
         id2node = dict(enumerate(nodes))
         node2id = {k: i for i, k in id2node.items()}
         for edge in edges:
             src, dst, weight = (*edge, 1) if len(edge) == 2 else edge
             for node in (src, dst):
```

### Comparing `torchlearn-0.2.0/torchlearn.egg-info/SOURCES.txt` & `torchlearn-0.2.1/torchlearn.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
 pyproject.toml
 requirements-dev.txt
 requirements.txt
-setup.cfg
-setup.py
 torchlearn/__init__.py
 torchlearn.egg-info/PKG-INFO
 torchlearn.egg-info/SOURCES.txt
 torchlearn.egg-info/dependency_links.txt
-torchlearn.egg-info/not-zip-safe
 torchlearn.egg-info/requires.txt
 torchlearn.egg-info/top_level.txt
 torchlearn/metric/__init__.py
 torchlearn/metric/average_metric.py
 torchlearn/metric/classification.py
 torchlearn/metric/loss.py
 torchlearn/metric/metric.py
```

