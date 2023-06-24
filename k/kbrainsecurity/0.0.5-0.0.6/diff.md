# Comparing `tmp/kbrainsecurity-0.0.5.tar.gz` & `tmp/kbrainsecurity-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbrainsecurity-0.0.5.tar", max compression
+gzip compressed data, was "kbrainsecurity-0.0.6.tar", max compression
```

## Comparing `kbrainsecurity-0.0.5.tar` & `kbrainsecurity-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    34353 2023-06-24 06:24:22.504184 kbrainsecurity-0.0.5/LICENSE.md
--rw-r--r--   0        0        0      982 2023-06-24 06:24:22.504184 kbrainsecurity-0.0.5/README.md
--rw-r--r--   0        0        0      547 2023-06-24 06:25:10.910041 kbrainsecurity-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1313 2023-06-24 06:24:22.504184 kbrainsecurity-0.0.5/src/azure_authentication.py
--rw-r--r--   0        0        0     1336 2023-06-24 06:24:22.504184 kbrainsecurity-0.0.5/src/bearer.py
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 kbrainsecurity-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34353 2023-06-24 06:37:42.856779 kbrainsecurity-0.0.6/LICENSE.md
+-rw-r--r--   0        0        0      982 2023-06-24 06:37:42.856779 kbrainsecurity-0.0.6/README.md
+-rw-r--r--   0        0        0      547 2023-06-24 06:38:34.425607 kbrainsecurity-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-24 06:37:42.856779 kbrainsecurity-0.0.6/src/__init__.py
+-rw-r--r--   0        0        0     1313 2023-06-24 06:37:42.856779 kbrainsecurity-0.0.6/src/azure_authentication.py
+-rw-r--r--   0        0        0     1336 2023-06-24 06:37:42.856779 kbrainsecurity-0.0.6/src/bearer.py
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 kbrainsecurity-0.0.6/PKG-INFO
```

### Comparing `kbrainsecurity-0.0.5/LICENSE.md` & `kbrainsecurity-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.5/README.md` & `kbrainsecurity-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.5/pyproject.toml` & `kbrainsecurity-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kbrainsecurity"
-version = "0.0.5"
+version = "0.0.6"
 description = "Security and authentication functions for use in KBRAIN"
 authors = ["Daniel E. Fredriksen <daniel.fredriksen@us.kbr.com>"]
 license = "AGPLv3"
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `kbrainsecurity-0.0.5/src/azure_authentication.py` & `kbrainsecurity-0.0.6/src/azure_authentication.py`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.5/src/bearer.py` & `kbrainsecurity-0.0.6/src/bearer.py`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.5/PKG-INFO` & `kbrainsecurity-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbrainsecurity
-Version: 0.0.5
+Version: 0.0.6
 Summary: Security and authentication functions for use in KBRAIN
 License: AGPLv3
 Author: Daniel E. Fredriksen
 Author-email: daniel.fredriksen@us.kbr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

