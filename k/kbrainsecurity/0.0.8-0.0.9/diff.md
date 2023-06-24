# Comparing `tmp/kbrainsecurity-0.0.8.tar.gz` & `tmp/kbrainsecurity-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbrainsecurity-0.0.8.tar", max compression
+gzip compressed data, was "kbrainsecurity-0.0.9.tar", max compression
```

## Comparing `kbrainsecurity-0.0.8.tar` & `kbrainsecurity-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    34353 2023-06-24 06:58:57.520653 kbrainsecurity-0.0.8/LICENSE.md
--rw-r--r--   0        0        0      982 2023-06-24 06:58:57.520653 kbrainsecurity-0.0.8/README.md
--rw-r--r--   0        0        0      551 2023-06-24 06:59:38.990254 kbrainsecurity-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-24 06:58:57.520653 kbrainsecurity-0.0.8/src/__init__.py
--rw-r--r--   0        0        0     1358 2023-06-24 06:58:57.520653 kbrainsecurity-0.0.8/src/authentication/azure_authentication.py
--rw-r--r--   0        0        0     1336 2023-06-24 06:58:57.520653 kbrainsecurity-0.0.8/src/authentication/bearer.py
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 kbrainsecurity-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    34353 2023-06-24 14:13:14.234140 kbrainsecurity-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0      982 2023-06-24 14:13:14.234140 kbrainsecurity-0.0.9/README.md
+-rw-r--r--   0        0        0      640 2023-06-24 14:14:05.559002 kbrainsecurity-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1358 2023-06-24 14:13:14.234140 kbrainsecurity-0.0.9/src/authentication/azure_authentication.py
+-rw-r--r--   0        0        0     1336 2023-06-24 14:13:14.234140 kbrainsecurity-0.0.9/src/authentication/bearer.py
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 kbrainsecurity-0.0.9/PKG-INFO
```

### Comparing `kbrainsecurity-0.0.8/LICENSE.md` & `kbrainsecurity-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.8/README.md` & `kbrainsecurity-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.8/src/authentication/azure_authentication.py` & `kbrainsecurity-0.0.9/src/authentication/azure_authentication.py`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.8/src/authentication/bearer.py` & `kbrainsecurity-0.0.9/src/authentication/bearer.py`

 * *Files identical despite different names*

### Comparing `kbrainsecurity-0.0.8/PKG-INFO` & `kbrainsecurity-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbrainsecurity
-Version: 0.0.8
+Version: 0.0.9
 Summary: Security and authentication functions for use in KBRAIN
 License: AGPLv3
 Author: Daniel E. Fredriksen
 Author-email: daniel.fredriksen@us.kbr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

