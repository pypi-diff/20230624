# Comparing `tmp/multion-0.1.0.tar.gz` & `tmp/multion-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multion-0.1.0.tar", max compression
+gzip compressed data, was "multion-0.1.1.tar", max compression
```

## Comparing `multion-0.1.0.tar` & `multion-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      188 2023-06-24 00:14:48.342052 multion-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-24 00:14:48.352052 multion-0.1.0/multion/__init__.py
--rw-r--r--   0        0        0     5556 2023-06-24 00:14:48.352052 multion-0.1.0/multion/multion.py
--rw-r--r--   0        0        0      325 2023-06-24 00:14:48.352052 multion-0.1.0/multion/setup.py
--rw-r--r--   0        0        0      360 2023-06-24 00:19:48.461990 multion-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      764 1970-01-01 00:00:00.000000 multion-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      188 2023-06-24 00:14:48.342052 multion-0.1.1/README.md
+-rw-r--r--   0        0        0       37 2023-06-24 00:28:26.361883 multion-0.1.1/multion/__init__.py
+-rw-r--r--   0        0        0     5556 2023-06-24 00:14:48.352052 multion-0.1.1/multion/multion.py
+-rw-r--r--   0        0        0      325 2023-06-24 00:14:48.352052 multion-0.1.1/multion/setup.py
+-rw-r--r--   0        0        0      360 2023-06-24 00:29:18.451872 multion-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      764 1970-01-01 00:00:00.000000 multion-0.1.1/PKG-INFO
```

### Comparing `multion-0.1.0/multion/multion.py` & `multion-0.1.1/multion/multion.py`

 * *Files identical despite different names*

### Comparing `multion-0.1.0/PKG-INFO` & `multion-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multion
-Version: 0.1.0
+Version: 0.1.1
 Summary: MULTION API
 Author: Div Garg
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

