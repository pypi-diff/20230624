# Comparing `tmp/kbrainsecurity-0.0.4.tar.gz` & `tmp/kbrainsecurity-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbrainsecurity-0.0.4.tar", max compression
+gzip compressed data, was "kbrainsecurity-0.0.4a0.tar", max compression
```

## Comparing `kbrainsecurity-0.0.4.tar` & `kbrainsecurity-0.0.4a0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      982 2023-06-24 00:19:25.455653 kbrainsecurity-0.0.4/README.md
--rw-r--r--   0        0        0      551 2023-06-24 00:20:08.860056 kbrainsecurity-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1313 2023-06-24 00:19:25.459653 kbrainsecurity-0.0.4/src/azure_authentication.py
--rw-r--r--   0        0        0     1336 2023-06-24 00:19:25.459653 kbrainsecurity-0.0.4/src/bearer.py
--rw-r--r--   0        0        0     1560 1970-01-01 00:00:00.000000 kbrainsecurity-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      982 2023-06-24 00:12:31.686943 kbrainsecurity-0.0.4a0/README.md
+-rw-r--r--   0        0        0      553 2023-06-24 00:13:15.942541 kbrainsecurity-0.0.4a0/pyproject.toml
+-rw-r--r--   0        0        0     1313 2023-06-24 00:12:31.686943 kbrainsecurity-0.0.4a0/src/azure_authentication.py
+-rw-r--r--   0        0        0     1336 2023-06-24 00:12:31.686943 kbrainsecurity-0.0.4a0/src/bearer.py
+-rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 kbrainsecurity-0.0.4a0/PKG-INFO
```

### Comparing `kbrainsecurity-0.0.4/README.md` & `kbrainsecurity-0.0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.4/pyproject.toml` & `kbrainsecurity-0.0.4a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kbrainsecurity"
-version = "0.0.4"
+version = "0.0.4a0"
 description = "Security and authentication functions for use in KBRAIN"
 authors = ["Daniel E. Fredriksen <daniel.fredriksen@us.kbr.com>"]
 license = "UNLICENSED"
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `kbrainsecurity-0.0.4/src/azure_authentication.py` & `kbrainsecurity-0.0.4a0/src/azure_authentication.py`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.4/src/bearer.py` & `kbrainsecurity-0.0.4a0/src/bearer.py`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.4/PKG-INFO` & `kbrainsecurity-0.0.4a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbrainsecurity
-Version: 0.0.4
+Version: 0.0.4a0
 Summary: Security and authentication functions for use in KBRAIN
 License: UNLICENSED
 Author: Daniel E. Fredriksen
 Author-email: daniel.fredriksen@us.kbr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

