# Comparing `tmp/spacecutter_lightning-0.3.2.tar.gz` & `tmp/spacecutter_lightning-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacecutter_lightning-0.3.2.tar", max compression
+gzip compressed data, was "spacecutter_lightning-1.0.1.tar", max compression
```

## Comparing `spacecutter_lightning-0.3.2.tar` & `spacecutter_lightning-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1369 2023-02-28 04:32:24.629238 spacecutter_lightning-0.3.2/README.md
--rw-r--r--   0        0        0      647 2023-02-28 04:32:24.633238 spacecutter_lightning-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      229 2023-02-28 04:32:24.633238 spacecutter_lightning-0.3.2/spacecutter_lightning/__init__.py
--rw-r--r--   0        0        0     1178 2023-02-28 04:32:24.633238 spacecutter_lightning-0.3.2/spacecutter_lightning/callback.py
--rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 spacecutter_lightning-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1369 2023-06-24 08:38:38.597851 spacecutter_lightning-1.0.1/README.md
+-rw-r--r--   0        0        0      647 2023-06-24 08:38:38.601851 spacecutter_lightning-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      229 2023-06-24 08:38:38.601851 spacecutter_lightning-1.0.1/spacecutter_lightning/__init__.py
+-rw-r--r--   0        0        0     1178 2023-06-24 08:38:38.601851 spacecutter_lightning-1.0.1/spacecutter_lightning/callback.py
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 spacecutter_lightning-1.0.1/PKG-INFO
```

### Comparing `spacecutter_lightning-0.3.2/README.md` & `spacecutter_lightning-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `spacecutter_lightning-0.3.2/pyproject.toml` & `spacecutter_lightning-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "spacecutter-lightning"
-version = "0.3.2"
+version = "1.0.1"
 description = "PyTorch-Lightning callback for spacecutter"
 authors = ["Soof Golan <pypi@soofgolan.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "spacecutter_lightning"}]
 homepage = "https://github.com/soof-golan/spacecutter-lightning"
 repository = "https://github.com/soof-golan/spacecutter-lightning"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
-pytorch-lightning = "^1.9.3"
-spacecutter-torch = "^0.4.0"
+pytorch-lightning = "^2.0.1"
+spacecutter-torch = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 black = "^23.1.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `spacecutter_lightning-0.3.2/spacecutter_lightning/callback.py` & `spacecutter_lightning-1.0.1/spacecutter_lightning/callback.py`

 * *Files identical despite different names*

### Comparing `spacecutter_lightning-0.3.2/PKG-INFO` & `spacecutter_lightning-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: spacecutter-lightning
-Version: 0.3.2
+Version: 1.0.1
 Summary: PyTorch-Lightning callback for spacecutter
 Home-page: https://github.com/soof-golan/spacecutter-lightning
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
-Requires-Dist: pytorch-lightning (>=1.9.3,<2.0.0)
-Requires-Dist: spacecutter-torch (>=0.4.0,<0.5.0)
+Requires-Dist: pytorch-lightning (>=2.0.1,<3.0.0)
+Requires-Dist: spacecutter-torch (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/soof-golan/spacecutter-lightning
 Description-Content-Type: text/markdown
 
 # Spacecutter Lightning
 
 A PyTorch Lightning Callback for Spacecutter.
```

