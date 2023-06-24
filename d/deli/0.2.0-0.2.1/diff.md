# Comparing `tmp/deli-0.2.0.tar.gz` & `tmp/deli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deli-0.2.0.tar", last modified: Mon Apr 17 09:55:14 2023, max compression
+gzip compressed data, was "deli-0.2.1.tar", last modified: Sat Jun 24 14:45:50 2023, max compression
```

## Comparing `deli-0.2.0.tar` & `deli-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:55:14.641601 deli-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-17 09:55:12.000000 deli-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 09:55:12.000000 deli-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 09:55:14.641601 deli-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 09:55:12.000000 deli-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:55:14.637601 deli-0.2.0/deli/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 09:55:12.000000 deli-0.2.0/deli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 09:55:12.000000 deli-0.2.0/deli/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-17 09:55:12.000000 deli-0.2.0/deli/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:55:14.641601 deli-0.2.0/deli/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/dicom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/nifty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/numpy_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/packaged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:55:14.641601 deli-0.2.0/deli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 09:55:14.000000 deli-0.2.0/deli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 09:55:14.000000 deli-0.2.0/deli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:55:14.000000 deli-0.2.0/deli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 09:55:14.000000 deli-0.2.0/deli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 09:55:14.000000 deli-0.2.0/deli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-17 09:55:12.000000 deli-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 09:55:12.000000 deli-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:55:14.641601 deli-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-17 09:55:12.000000 deli-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:45:50.339832 deli-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-24 14:45:47.000000 deli-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-24 14:45:47.000000 deli-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-24 14:45:50.339832 deli-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-24 14:45:47.000000 deli-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:45:50.335832 deli-0.2.1/deli/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 14:45:47.000000 deli-0.2.1/deli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 14:45:47.000000 deli-0.2.1/deli/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-24 14:45:47.000000 deli-0.2.1/deli/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:45:50.339832 deli-0.2.1/deli/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/nifty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/numpy_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-24 14:45:47.000000 deli-0.2.1/deli/serializers/packaged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:45:50.335832 deli-0.2.1/deli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-24 14:45:50.000000 deli-0.2.1/deli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-24 14:45:50.000000 deli-0.2.1/deli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:45:50.000000 deli-0.2.1/deli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 14:45:50.000000 deli-0.2.1/deli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 14:45:50.000000 deli-0.2.1/deli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-24 14:45:47.000000 deli-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 14:45:47.000000 deli-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:45:50.339832 deli-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-24 14:45:47.000000 deli-0.2.1/setup.py
```

### Comparing `deli-0.2.0/LICENSE` & `deli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deli-0.2.0/PKG-INFO` & `deli-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: deli
-Version: 0.2.0
+Version: 0.2.1
 Summary: Smart serialization and deserialization for (almost) any python object
 Home-page: https://github.com/maxme1/deli
 License: MIT
-Download-URL: https://github.com/maxme1/deli/archive/v0.2.0.tar.gz
+Download-URL: https://github.com/maxme1/deli/archive/v0.2.1.tar.gz
 Keywords: serialization
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `deli-0.2.0/deli/interface.py` & `deli-0.2.1/deli/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,15 @@
         return os.path.basename(os.fspath(path))
     return None
 
 
 # TODO: rewrite as generic calls with hints
 def load_json(path: PathLike):
     """Load the contents of a json file."""
-    with open(path, 'r') as f:
-        return json.load(f)
+    return load(path, hint='.json')
 
 
 def save_json(value, path: PathLike, *, indent: int = None):
     """Dump a json-serializable object to a json file."""
     with open(path, 'w') as f:
         json.dump(value, f, indent=indent)
```

### Comparing `deli-0.2.0/deli/serializer.py` & `deli-0.2.1/deli/serializer.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.0/deli/serializers/choice.py` & `deli-0.2.1/deli/serializers/choice.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.0/deli/serializers/csv.py` & `deli-0.2.1/deli/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.0/deli/serializers/dicom.py` & `deli-0.2.1/deli/serializers/dicom.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.0/deli/serializers/helpers.py` & `deli-0.2.1/deli/serializers/helpers.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.0/deli/serializers/images.py` & `deli-0.2.1/deli/serializers/images.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.0/deli/serializers/nifty.py` & `deli-0.2.1/deli/serializers/nifty.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.0/deli/serializers/numpy_.py` & `deli-0.2.1/deli/serializers/numpy_.py`

 * *Files identical despite different names*

### Comparing `deli-0.2.0/deli/serializers/packaged.py` & `deli-0.2.1/deli/serializers/packaged.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ..serializer import Serializer, MaybeSerializer, MaybeHint, WrongSerializer, REGISTRY, Hint
 
 
 class JSON(PathAsBuffer, ExtensionMatch):
     extensions = '.json',
 
     def _match_save_params(self, params: dict):
-        return set(params) <= {'indent'}
+        return set(params) <= {'indent', 'cls'}
 
     def load_buffer(self, source: BinaryIO, hint: MaybeHint, allow_lazy: bool, params: dict) -> Any:
         wrapper = TextIOWrapper(source)
         try:
             return json.load(wrapper)
         except (TypeError, json.JSONDecodeError) as e:
             if hint is not None:
```

### Comparing `deli-0.2.0/deli.egg-info/PKG-INFO` & `deli-0.2.1/deli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: deli
-Version: 0.2.0
+Version: 0.2.1
 Summary: Smart serialization and deserialization for (almost) any python object
 Home-page: https://github.com/maxme1/deli
 License: MIT
-Download-URL: https://github.com/maxme1/deli/archive/v0.2.0.tar.gz
+Download-URL: https://github.com/maxme1/deli/archive/v0.2.1.tar.gz
 Keywords: serialization
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `deli-0.2.0/deli.egg-info/SOURCES.txt` & `deli-0.2.1/deli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deli-0.2.0/pyproject.toml` & `deli-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deli-0.2.0/setup.py` & `deli-0.2.1/setup.py`

 * *Files identical despite different names*

