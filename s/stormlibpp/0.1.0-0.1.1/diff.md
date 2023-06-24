# Comparing `tmp/stormlibpp-0.1.0.tar.gz` & `tmp/stormlibpp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stormlibpp-0.1.0.tar", last modified: Sat Jun 24 18:25:30 2023, max compression
+gzip compressed data, was "stormlibpp-0.1.1.tar", last modified: Sat Jun 24 18:41:55 2023, max compression
```

## Comparing `stormlibpp-0.1.0.tar` & `stormlibpp-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:25:30.987517 stormlibpp-0.1.0/
--rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-24 17:20:21.000000 stormlibpp-0.1.0/LICENSE
--rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-24 18:25:30.987386 stormlibpp-0.1.0/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      108 2023-06-24 18:24:05.000000 stormlibpp-0.1.0/README.md
--rw-r--r--   0 gormo      (501) staff       (20)      557 2023-06-24 18:25:26.000000 stormlibpp-0.1.0/pyproject.toml
--rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-24 18:25:30.987558 stormlibpp-0.1.0/setup.cfg
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:25:30.984583 stormlibpp-0.1.0/src/
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:25:30.985649 stormlibpp-0.1.0/src/stormlibpp/
--rw-r--r--   0 gormo      (501) staff       (20)      566 2023-06-24 18:25:26.000000 stormlibpp-0.1.0/src/stormlibpp/__init__.py
--rw-r--r--   0 gormo      (501) staff       (20)      448 2023-06-24 17:27:58.000000 stormlibpp-0.1.0/src/stormlibpp/errors.py
--rw-r--r--   0 gormo      (501) staff       (20)     5779 2023-06-24 18:11:27.000000 stormlibpp-0.1.0/src/stormlibpp/stormpkg.py
--rw-r--r--   0 gormo      (501) staff       (20)     1289 2023-06-24 18:18:30.000000 stormlibpp-0.1.0/src/stormlibpp/telepath.py
--rw-r--r--   0 gormo      (501) staff       (20)      618 2023-06-24 18:23:17.000000 stormlibpp-0.1.0/src/stormlibpp/utils.py
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:25:30.986550 stormlibpp-0.1.0/src/stormlibpp.egg-info/
--rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-24 18:25:30.000000 stormlibpp-0.1.0/src/stormlibpp.egg-info/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      417 2023-06-24 18:25:30.000000 stormlibpp-0.1.0/src/stormlibpp.egg-info/SOURCES.txt
--rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-24 18:25:30.000000 stormlibpp-0.1.0/src/stormlibpp.egg-info/dependency_links.txt
--rw-r--r--   0 gormo      (501) staff       (20)       17 2023-06-24 18:25:30.000000 stormlibpp-0.1.0/src/stormlibpp.egg-info/requires.txt
--rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-24 18:25:30.000000 stormlibpp-0.1.0/src/stormlibpp.egg-info/top_level.txt
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:25:30.987168 stormlibpp-0.1.0/tests/
--rw-r--r--   0 gormo      (501) staff       (20)     1241 2023-06-24 18:17:59.000000 stormlibpp-0.1.0/tests/test_stormpkg.py
--rw-r--r--   0 gormo      (501) staff       (20)      481 2023-06-24 18:18:58.000000 stormlibpp-0.1.0/tests/test_telepath.py
--rw-r--r--   0 gormo      (501) staff       (20)      419 2023-06-24 18:22:09.000000 stormlibpp-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:41:55.004569 stormlibpp-0.1.1/
+-rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-24 17:20:21.000000 stormlibpp-0.1.1/LICENSE
+-rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-24 18:41:55.004427 stormlibpp-0.1.1/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      108 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/README.md
+-rw-r--r--   0 gormo      (501) staff       (20)      557 2023-06-24 18:41:50.000000 stormlibpp-0.1.1/pyproject.toml
+-rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-24 18:41:55.004613 stormlibpp-0.1.1/setup.cfg
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:41:55.001406 stormlibpp-0.1.1/src/
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:41:55.002697 stormlibpp-0.1.1/src/stormlibpp/
+-rw-r--r--   0 gormo      (501) staff       (20)      566 2023-06-24 18:41:50.000000 stormlibpp-0.1.1/src/stormlibpp/__init__.py
+-rw-r--r--   0 gormo      (501) staff       (20)      448 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/src/stormlibpp/errors.py
+-rw-r--r--   0 gormo      (501) staff       (20)     5746 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/src/stormlibpp/stormpkg.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1396 2023-06-24 18:39:56.000000 stormlibpp-0.1.1/src/stormlibpp/telepath.py
+-rw-r--r--   0 gormo      (501) staff       (20)      618 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/src/stormlibpp/utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:41:55.003487 stormlibpp-0.1.1/src/stormlibpp.egg-info/
+-rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-24 18:41:54.000000 stormlibpp-0.1.1/src/stormlibpp.egg-info/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      417 2023-06-24 18:41:55.000000 stormlibpp-0.1.1/src/stormlibpp.egg-info/SOURCES.txt
+-rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-24 18:41:54.000000 stormlibpp-0.1.1/src/stormlibpp.egg-info/dependency_links.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       17 2023-06-24 18:41:54.000000 stormlibpp-0.1.1/src/stormlibpp.egg-info/requires.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-24 18:41:54.000000 stormlibpp-0.1.1/src/stormlibpp.egg-info/top_level.txt
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-24 18:41:55.004207 stormlibpp-0.1.1/tests/
+-rw-r--r--   0 gormo      (501) staff       (20)     1241 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/tests/test_stormpkg.py
+-rw-r--r--   0 gormo      (501) staff       (20)      720 2023-06-24 18:41:02.000000 stormlibpp-0.1.1/tests/test_telepath.py
+-rw-r--r--   0 gormo      (501) staff       (20)      419 2023-06-24 18:31:15.000000 stormlibpp-0.1.1/tests/test_utils.py
```

### Comparing `stormlibpp-0.1.0/LICENSE` & `stormlibpp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stormlibpp-0.1.0/PKG-INFO` & `stormlibpp-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormlibpp
-Version: 0.1.0
+Version: 0.1.1
 Summary: The stormlibpp Python package
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stormlibpp-0.1.0/pyproject.toml` & `stormlibpp-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stormlibpp"
-version = "0.1.0"
+version = "0.1.1"
 description = "The stormlibpp Python package"
 readme = "README.md"
 requires-python = ">=3.11"
 
 # Fill in dependencies here.
 dependencies = [
     "synapse==2.139.0"
```

### Comparing `stormlibpp-0.1.0/src/stormlibpp/__init__.py` & `stormlibpp-0.1.1/src/stormlibpp/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     synapse.common -> s_common
     synapse.exc -> s_exc
     synapse.genpkg -> s_genpkg
 
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 
 import synapse.common as s_common
 import synapse.exc as s_exc
 import synapse.tools.genpkg as s_genpkg
 
 from . import errors
```

### Comparing `stormlibpp-0.1.0/src/stormlibpp/stormpkg.py` & `stormlibpp-0.1.1/src/stormlibpp/stormpkg.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,32 @@
 
     This object is ready to use on init - access the ``pkgdef`` prop for
     the full Storm package definition loaded from the definied package proto.
     The ``pkgdef`` property is also returned by this object's ``asdict`` method.
 
     It takes the following steps on start up:
 
-        - Resolves the path of the package proto based on ``proto_name`` and
-        ``proto_dir``.
-        - Loads the package proto using ``synapse.tools.genpkg.tryLoadPkgProto``.
-        - Converts the returned object to a ``dict`` using ``json.dumps`` and
-        ``json.loads``.
-            - This is necessary because ``tryLoadPkgProto`` returns a "tuplified"
-            object (the return of ``synapse.common.tuplify``). Which can return
-            immutable objects that ``synapse.cortex.Cortex.addStormPkg`` expects
-            to be mutable. So a ``StormSvc._storm_svc_pkgs`` works best when it
-            is set to a ``dict``.
-        - Sets the loaded package definition's ``build`` key to a ``dict`` containing
-        the time using ``synapse.common.now``.
-        - Stores the package definition ``dict`` in the ``pkdef`` property.
+    - Resolves the path of the package proto based on ``proto_name`` and
+      ``proto_dir``.
+
+    - Loads the package proto using ``synapse.tools.genpkg.tryLoadPkgProto``.
+
+    - Converts the returned object to a ``dict`` using ``json.dumps`` and
+      ``json.loads``.
+
+        - This is necessary because ``tryLoadPkgProto`` returns a "tuplified"
+          object (the return of ``synapse.common.tuplify``). Which can return
+          immutable objects that ``synapse.cortex.Cortex.addStormPkg`` expects
+          to be mutable. So a ``StormSvc._storm_svc_pkgs`` works best when it
+          is set to a ``dict``.
+
+    - Sets the loaded package definition's ``build`` key to a ``dict``
+      containing the time using ``synapse.common.now``.
+
+    - Stores the package definition ``dict`` in the ``pkdef`` property.
 
     Parameters
     ----------
     proto_name : str | None, optional
         The name of the package's proto Yaml file, without the extension,
         if it is different from ``pkg_name``. A value of ``None`` means
         ``pkg_name`` is used. By default None.
```

### Comparing `stormlibpp-0.1.0/src/stormlibpp/telepath.py` & `stormlibpp-0.1.1/src/stormlibpp/telepath.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,7 +32,12 @@
     """Generate a default TelepathRetn return object, or the given subclass.
 
     Default values have a ``status`` of ``True``, an empty ``mesg``, and
     ``data`` is set to the ``default_data`` arg - which defaults to ``None``.
     """
 
     return obj(status=True, mesg="", data=default_data)
+
+
+class BoolRetn(TelepathRetn):
+    """A TelepathRetn where ``data`` is a boolean value."""
+    data: bool
```

### Comparing `stormlibpp-0.1.0/src/stormlibpp/utils.py` & `stormlibpp-0.1.1/src/stormlibpp/utils.py`

 * *Files identical despite different names*

### Comparing `stormlibpp-0.1.0/src/stormlibpp.egg-info/PKG-INFO` & `stormlibpp-0.1.1/src/stormlibpp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormlibpp
-Version: 0.1.0
+Version: 0.1.1
 Summary: The stormlibpp Python package
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stormlibpp-0.1.0/tests/test_stormpkg.py` & `stormlibpp-0.1.1/tests/test_stormpkg.py`

 * *Files identical despite different names*

