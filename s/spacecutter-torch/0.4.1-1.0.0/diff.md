# Comparing `tmp/spacecutter_torch-0.4.1.tar.gz` & `tmp/spacecutter_torch-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacecutter_torch-0.4.1.tar", max compression
+gzip compressed data, was "spacecutter_torch-1.0.0.tar", max compression
```

## Comparing `spacecutter_torch-0.4.1.tar` & `spacecutter_torch-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2146 2023-02-28 04:28:16.651021 spacecutter_torch-0.4.1/LICENSE
--rw-r--r--   0        0        0     2638 2023-02-28 04:28:16.651021 spacecutter_torch-0.4.1/README.md
--rw-r--r--   0        0        0      941 2023-02-28 04:28:16.651021 spacecutter_torch-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      213 2023-02-28 04:28:16.651021 spacecutter_torch-0.4.1/spacecutter/__init__.py
--rw-r--r--   0        0        0     1604 2023-02-28 04:28:16.651021 spacecutter_torch-0.4.1/spacecutter/callbacks.py
--rw-r--r--   0        0        0     3417 2023-02-28 04:28:16.651021 spacecutter_torch-0.4.1/spacecutter/losses.py
--rw-r--r--   0        0        0     3893 2023-02-28 04:28:16.651021 spacecutter_torch-0.4.1/spacecutter/models.py
--rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 spacecutter_torch-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2146 2023-06-24 08:24:28.735594 spacecutter_torch-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2638 2023-06-24 08:24:28.735594 spacecutter_torch-1.0.0/README.md
+-rw-r--r--   0        0        0      939 2023-06-24 08:24:28.735594 spacecutter_torch-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      213 2023-06-24 08:24:28.735594 spacecutter_torch-1.0.0/spacecutter/__init__.py
+-rw-r--r--   0        0        0     1604 2023-06-24 08:24:28.735594 spacecutter_torch-1.0.0/spacecutter/callbacks.py
+-rw-r--r--   0        0        0     3417 2023-06-24 08:24:28.735594 spacecutter_torch-1.0.0/spacecutter/losses.py
+-rw-r--r--   0        0        0     3893 2023-06-24 08:24:28.735594 spacecutter_torch-1.0.0/spacecutter/models.py
+-rw-r--r--   0        0        0     3215 1970-01-01 00:00:00.000000 spacecutter_torch-1.0.0/PKG-INFO
```

### Comparing `spacecutter_torch-0.4.1/LICENSE` & `spacecutter_torch-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spacecutter_torch-0.4.1/README.md` & `spacecutter_torch-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `spacecutter_torch-0.4.1/pyproject.toml` & `spacecutter_torch-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 ]
 keywords = ['ordinal regression', 'pytorch', 'machine learning', 'statistics', 'regression']
 homepage= "https://github.com/soof-golan/spacecutter"
 repository = "https://github.com/soof-golan/spacecutter"
 
 [tool.poetry]
 name = "spacecutter-torch"
-version = "0.4.1"
+version = "1.0.0"
 description = "Ordinal regression models in PyTorch"
 authors = ["Soof Golan <pypi@soofgolan.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "spacecutter" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-torch = "^1.1.0"
+torch = "^2.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
 [build-system]
```

### Comparing `spacecutter_torch-0.4.1/spacecutter/callbacks.py` & `spacecutter_torch-1.0.0/spacecutter/callbacks.py`

 * *Files identical despite different names*

### Comparing `spacecutter_torch-0.4.1/spacecutter/losses.py` & `spacecutter_torch-1.0.0/spacecutter/losses.py`

 * *Files identical despite different names*

### Comparing `spacecutter_torch-0.4.1/spacecutter/models.py` & `spacecutter_torch-1.0.0/spacecutter/models.py`

 * *Files identical despite different names*

### Comparing `spacecutter_torch-0.4.1/PKG-INFO` & `spacecutter_torch-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: spacecutter-torch
-Version: 0.4.1
+Version: 1.0.0
 Summary: Ordinal regression models in PyTorch
 License: MIT
 Author: Soof Golan
 Author-email: pypi@soofgolan.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: torch (>=1.1.0,<2.0.0)
+Requires-Dist: torch (>=2.0,<3.0)
 Description-Content-Type: text/markdown
 
 # spacecutter-torch
 
 `spacecutter-torch` is a library for implementing ordinal regression models in PyTorch. The library consists of models and loss functions.
 
 ## Installation
```

