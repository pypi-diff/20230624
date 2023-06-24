# Comparing `tmp/drupaljsonapiclient-1.0.2.tar.gz` & `tmp/drupaljsonapiclient-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drupaljsonapiclient-1.0.2.tar", max compression
+gzip compressed data, was "drupaljsonapiclient-1.0.3.tar", max compression
```

## Comparing `drupaljsonapiclient-1.0.2.tar` & `drupaljsonapiclient-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1690 2023-06-24 05:36:15.776561 drupaljsonapiclient-1.0.2/LICENSE
--rw-r--r--   0        0        0     1244 2023-06-24 05:36:15.776561 drupaljsonapiclient-1.0.2/README.md
--rw-r--r--   0        0        0      156 2023-06-24 05:36:15.776561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/common.py
--rw-r--r--   0        0        0     4383 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/document.py
--rw-r--r--   0        0        0      620 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/exceptions.py
--rw-r--r--   0        0        0     3145 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/filter.py
--rw-r--r--   0        0        0     4283 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/objects.py
--rw-r--r--   0        0        0    14266 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/relationships.py
--rw-r--r--   0        0        0    26340 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/resourceobject.py
--rw-r--r--   0        0        0    28096 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/session.py
--rw-r--r--   0        0        0     1008 2023-06-24 05:36:15.779560 drupaljsonapiclient-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1690 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1244 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/README.md
+-rw-r--r--   0        0        0      156 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/common.py
+-rw-r--r--   0        0        0     4383 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/document.py
+-rw-r--r--   0        0        0      620 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/exceptions.py
+-rw-r--r--   0        0        0     3145 2023-06-24 13:39:22.571047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/filter.py
+-rw-r--r--   0        0        0     4283 2023-06-24 13:39:22.572047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/objects.py
+-rw-r--r--   0        0        0    14266 2023-06-24 13:39:22.572047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/relationships.py
+-rw-r--r--   0        0        0    26340 2023-06-24 13:39:22.572047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/resourceobject.py
+-rw-r--r--   0        0        0    28104 2023-06-24 13:39:22.572047 drupaljsonapiclient-1.0.3/drupaljsonapiclient/session.py
+-rw-r--r--   0        0        0     1008 2023-06-24 13:39:22.573047 drupaljsonapiclient-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.3/PKG-INFO
```

### Comparing `drupaljsonapiclient-1.0.2/LICENSE` & `drupaljsonapiclient-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.2/README.md` & `drupaljsonapiclient-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.2/drupaljsonapiclient/common.py` & `drupaljsonapiclient-1.0.3/drupaljsonapiclient/common.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.2/drupaljsonapiclient/document.py` & `drupaljsonapiclient-1.0.3/drupaljsonapiclient/document.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.2/drupaljsonapiclient/exceptions.py` & `drupaljsonapiclient-1.0.3/drupaljsonapiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.2/drupaljsonapiclient/filter.py` & `drupaljsonapiclient-1.0.3/drupaljsonapiclient/filter.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.2/drupaljsonapiclient/objects.py` & `drupaljsonapiclient-1.0.3/drupaljsonapiclient/objects.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.2/drupaljsonapiclient/relationships.py` & `drupaljsonapiclient-1.0.3/drupaljsonapiclient/relationships.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.2/drupaljsonapiclient/resourceobject.py` & `drupaljsonapiclient-1.0.3/drupaljsonapiclient/resourceobject.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.2/drupaljsonapiclient/session.py` & `drupaljsonapiclient-1.0.3/drupaljsonapiclient/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
 class Schema:
     """
     Container for model schemas with associated methods.
     Session contains Schema.
     """
 
-    def __init__(self, schema_data: dict=None) -> None:
-        self._schema_data = schema_data
+    def __init__(self, schema_data: dict = None) -> None:
+        self._schema_data = schema_data or {}
 
     def find_spec(self, model_name: str, attribute_name: str) -> dict:
         """
         Find specification from model_name for attribute_name which can
         be nested format, i.e. 'attribute-group1.attribute-group2.attribute-item'
         """
```

### Comparing `drupaljsonapiclient-1.0.2/pyproject.toml` & `drupaljsonapiclient-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drupaljsonapiclient"
-version = "1.0.2"
+version = "1.0.3"
 description = "Drupal CMS JSON:API client for Python."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drupaljsonapiclient"}]
 repository = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient"
 documentation = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient/-/blob/main/README.md"
```

### Comparing `drupaljsonapiclient-1.0.2/PKG-INFO` & `drupaljsonapiclient-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drupaljsonapiclient
-Version: 1.0.2
+Version: 1.0.3
 Summary: Drupal CMS JSON:API client for Python.
 Home-page: https://gitlab.com/martins-bruvelis/drupaljsonapiclient
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

