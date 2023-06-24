# Comparing `tmp/kbrainsecurity-0.0.4.tar.gz` & `tmp/kbrainsecurity-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbrainsecurity-0.0.4.tar", max compression
+gzip compressed data, was "kbrainsecurity-0.0.5.tar", max compression
```

## Comparing `kbrainsecurity-0.0.4.tar` & `kbrainsecurity-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      982 2023-06-24 00:19:25.455653 kbrainsecurity-0.0.4/README.md
--rw-r--r--   0        0        0      551 2023-06-24 00:20:08.860056 kbrainsecurity-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1313 2023-06-24 00:19:25.459653 kbrainsecurity-0.0.4/src/azure_authentication.py
--rw-r--r--   0        0        0     1336 2023-06-24 00:19:25.459653 kbrainsecurity-0.0.4/src/bearer.py
--rw-r--r--   0        0        0     1560 1970-01-01 00:00:00.000000 kbrainsecurity-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34353 2023-06-24 06:24:22.504184 kbrainsecurity-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0      982 2023-06-24 06:24:22.504184 kbrainsecurity-0.0.5/README.md
+-rw-r--r--   0        0        0      547 2023-06-24 06:25:10.910041 kbrainsecurity-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1313 2023-06-24 06:24:22.504184 kbrainsecurity-0.0.5/src/azure_authentication.py
+-rw-r--r--   0        0        0     1336 2023-06-24 06:24:22.504184 kbrainsecurity-0.0.5/src/bearer.py
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 kbrainsecurity-0.0.5/PKG-INFO
```

### Comparing `kbrainsecurity-0.0.4/README.md` & `kbrainsecurity-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.4/pyproject.toml` & `kbrainsecurity-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "kbrainsecurity"
-version = "0.0.4"
+version = "0.0.5"
 description = "Security and authentication functions for use in KBRAIN"
 authors = ["Daniel E. Fredriksen <daniel.fredriksen@us.kbr.com>"]
-license = "UNLICENSED"
+license = "AGPLv3"
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 python-jose = "^3.3.0"
 azure-functions = "^1.15.0"
```

### Comparing `kbrainsecurity-0.0.4/src/azure_authentication.py` & `kbrainsecurity-0.0.5/src/azure_authentication.py`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.4/src/bearer.py` & `kbrainsecurity-0.0.5/src/bearer.py`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.4/PKG-INFO` & `kbrainsecurity-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kbrainsecurity
-Version: 0.0.4
+Version: 0.0.5
 Summary: Security and authentication functions for use in KBRAIN
-License: UNLICENSED
+License: AGPLv3
 Author: Daniel E. Fredriksen
 Author-email: daniel.fredriksen@us.kbr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

