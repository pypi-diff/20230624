# Comparing `tmp/paradigm-4.1.1.tar.gz` & `tmp/paradigm-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradigm-4.1.1.tar", last modified: Thu May 25 07:21:09 2023, max compression
+gzip compressed data, was "paradigm-4.2.0.tar", last modified: Sat Jun 24 13:28:49 2023, max compression
```

## Comparing `paradigm-4.1.1.tar` & `paradigm-4.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:21:09.221447 paradigm-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 07:20:58.000000 paradigm-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 07:20:58.000000 paradigm-4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-05-25 07:21:09.221447 paradigm-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-25 07:20:58.000000 paradigm-4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:21:09.217446 paradigm-4.1.1/paradigm/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:21:09.217446 paradigm-4.1.1/paradigm/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:21:09.221447 paradigm-4.1.1/paradigm/_core/arboreal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/arboreal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/arboreal/construction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/arboreal/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/arboreal/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/arboreal/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/arboreal/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/arboreal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    24186 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/namespacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/scoping.py
--rw-r--r--   0 runner    (1001) docker     (123)    26241 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)    47999 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/_core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:20:58.000000 paradigm-4.1.1/paradigm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:21:09.217446 paradigm-4.1.1/paradigm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-05-25 07:21:09.000000 paradigm-4.1.1/paradigm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-25 07:21:09.000000 paradigm-4.1.1/paradigm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:21:09.000000 paradigm-4.1.1/paradigm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 07:21:09.000000 paradigm-4.1.1/paradigm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 07:21:09.000000 paradigm-4.1.1/paradigm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-25 07:20:58.000000 paradigm-4.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:21:09.221447 paradigm-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-25 07:20:58.000000 paradigm-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:28:49.740119 paradigm-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 13:28:40.000000 paradigm-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-24 13:28:40.000000 paradigm-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-06-24 13:28:49.740119 paradigm-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-24 13:28:40.000000 paradigm-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:28:49.736119 paradigm-4.2.0/paradigm/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:28:49.740119 paradigm-4.2.0/paradigm/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:28:49.740119 paradigm-4.2.0/paradigm/_core/arboreal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/arboreal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/arboreal/construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/arboreal/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/arboreal/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/arboreal/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/arboreal/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/arboreal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24186 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/namespacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/scoping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26241 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47999 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/_core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 13:28:40.000000 paradigm-4.2.0/paradigm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:28:49.740119 paradigm-4.2.0/paradigm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-06-24 13:28:49.000000 paradigm-4.2.0/paradigm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-24 13:28:49.000000 paradigm-4.2.0/paradigm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 13:28:49.000000 paradigm-4.2.0/paradigm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-24 13:28:49.000000 paradigm-4.2.0/paradigm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 13:28:49.000000 paradigm-4.2.0/paradigm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-24 13:28:40.000000 paradigm-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 13:28:49.740119 paradigm-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-24 13:28:40.000000 paradigm-4.2.0/setup.py
```

### Comparing `paradigm-4.1.1/LICENSE` & `paradigm-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/PKG-INFO` & `paradigm-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm
-Version: 4.1.1
+Version: 4.2.0
 Summary: Python objects metadata parser.
 Home-page: https://github.com/lycantropos/paradigm/
 Download-URL: https://github.com/lycantropos/paradigm/archive/master.zip
 Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Azat Ibrakov
```

### Comparing `paradigm-4.1.1/README.md` & `paradigm-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/annotated.py` & `paradigm-4.2.0/paradigm/_core/annotated.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/arboreal/construction.py` & `paradigm-4.2.0/paradigm/_core/arboreal/construction.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/arboreal/conversion.py` & `paradigm-4.2.0/paradigm/_core/arboreal/conversion.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/arboreal/evaluation.py` & `paradigm-4.2.0/paradigm/_core/arboreal/evaluation.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/arboreal/execution.py` & `paradigm-4.2.0/paradigm/_core/arboreal/execution.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/arboreal/utils.py` & `paradigm-4.2.0/paradigm/_core/arboreal/utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/caching.py` & `paradigm-4.2.0/paradigm/_core/caching.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/catalog.py` & `paradigm-4.2.0/paradigm/_core/catalog.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/discovery.py` & `paradigm-4.2.0/paradigm/_core/discovery.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/execution.py` & `paradigm-4.2.0/paradigm/_core/execution.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/file_system.py` & `paradigm-4.2.0/paradigm/_core/file_system.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/index.py` & `paradigm-4.2.0/paradigm/_core/index.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/models.py` & `paradigm-4.2.0/paradigm/_core/models.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/modules.py` & `paradigm-4.2.0/paradigm/_core/modules.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/pretty.py` & `paradigm-4.2.0/paradigm/_core/pretty.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/scoping.py` & `paradigm-4.2.0/paradigm/_core/scoping.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/signatures.py` & `paradigm-4.2.0/paradigm/_core/signatures.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/sources.py` & `paradigm-4.2.0/paradigm/_core/sources.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/stubs.py` & `paradigm-4.2.0/paradigm/_core/stubs.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm/_core/utils.py` & `paradigm-4.2.0/paradigm/_core/utils.py`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/paradigm.egg-info/PKG-INFO` & `paradigm-4.2.0/paradigm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm
-Version: 4.1.1
+Version: 4.2.0
 Summary: Python objects metadata parser.
 Home-page: https://github.com/lycantropos/paradigm/
 Download-URL: https://github.com/lycantropos/paradigm/archive/master.zip
 Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Azat Ibrakov
```

### Comparing `paradigm-4.1.1/paradigm.egg-info/SOURCES.txt` & `paradigm-4.2.0/paradigm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paradigm-4.1.1/pyproject.toml` & `paradigm-4.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy"
 ]
 requires-python = ">=3.7"
 dependencies = [
-    "mypy>=1.3.0,<2.0",
-    "typing-extensions>=4.6.1,<5.0"
+    "mypy>=1.4.0,<2.0",
+    "typing-extensions>=4.6.3,<5.0"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 tests = [
-    "hypothesis>=6.75.3,<7.0",
-    "pytest>=7.3.1,<8.0"
+    "hypothesis>=6.79.2,<7.0",
+    "pytest>=7.4.0,<8.0"
 ]
 
 [build-system]
 requires = [
     "setuptools",
     "wheel"
 ]
```

