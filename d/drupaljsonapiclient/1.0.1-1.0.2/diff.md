# Comparing `tmp/drupaljsonapiclient-1.0.1.tar.gz` & `tmp/drupaljsonapiclient-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drupaljsonapiclient-1.0.1.tar", max compression
+gzip compressed data, was "drupaljsonapiclient-1.0.2.tar", max compression
```

## Comparing `drupaljsonapiclient-1.0.1.tar` & `drupaljsonapiclient-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1690 2023-06-24 05:22:47.332196 drupaljsonapiclient-1.0.1/LICENSE
--rw-r--r--   0        0        0     1244 2023-06-24 05:22:47.332196 drupaljsonapiclient-1.0.1/README.md
--rw-r--r--   0        0        0      156 2023-06-24 05:22:47.332196 drupaljsonapiclient-1.0.1/drupaljsonapiclient/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-24 05:22:47.332196 drupaljsonapiclient-1.0.1/drupaljsonapiclient/common.py
--rw-r--r--   0        0        0     4383 2023-06-24 05:22:47.332196 drupaljsonapiclient-1.0.1/drupaljsonapiclient/document.py
--rw-r--r--   0        0        0      620 2023-06-24 05:22:47.332196 drupaljsonapiclient-1.0.1/drupaljsonapiclient/exceptions.py
--rw-r--r--   0        0        0     3145 2023-06-24 05:22:47.332196 drupaljsonapiclient-1.0.1/drupaljsonapiclient/filter.py
--rw-r--r--   0        0        0     4283 2023-06-24 05:22:47.333196 drupaljsonapiclient-1.0.1/drupaljsonapiclient/objects.py
--rw-r--r--   0        0        0    14266 2023-06-24 05:22:47.333196 drupaljsonapiclient-1.0.1/drupaljsonapiclient/relationships.py
--rw-r--r--   0        0        0    26876 2023-06-24 05:22:47.333196 drupaljsonapiclient-1.0.1/drupaljsonapiclient/resourceobject.py
--rw-r--r--   0        0        0    28096 2023-06-24 05:22:47.333196 drupaljsonapiclient-1.0.1/drupaljsonapiclient/session.py
--rw-r--r--   0        0        0     1008 2023-06-24 05:22:47.334196 drupaljsonapiclient-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1690 2023-06-24 05:36:15.776561 drupaljsonapiclient-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1244 2023-06-24 05:36:15.776561 drupaljsonapiclient-1.0.2/README.md
+-rw-r--r--   0        0        0      156 2023-06-24 05:36:15.776561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/common.py
+-rw-r--r--   0        0        0     4383 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/document.py
+-rw-r--r--   0        0        0      620 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/exceptions.py
+-rw-r--r--   0        0        0     3145 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/filter.py
+-rw-r--r--   0        0        0     4283 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/objects.py
+-rw-r--r--   0        0        0    14266 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/relationships.py
+-rw-r--r--   0        0        0    26340 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/resourceobject.py
+-rw-r--r--   0        0        0    28096 2023-06-24 05:36:15.777561 drupaljsonapiclient-1.0.2/drupaljsonapiclient/session.py
+-rw-r--r--   0        0        0     1008 2023-06-24 05:36:15.779560 drupaljsonapiclient-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.2/PKG-INFO
```

### Comparing `drupaljsonapiclient-1.0.1/LICENSE` & `drupaljsonapiclient-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.1/README.md` & `drupaljsonapiclient-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.1/drupaljsonapiclient/common.py` & `drupaljsonapiclient-1.0.2/drupaljsonapiclient/common.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.1/drupaljsonapiclient/document.py` & `drupaljsonapiclient-1.0.2/drupaljsonapiclient/document.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.1/drupaljsonapiclient/exceptions.py` & `drupaljsonapiclient-1.0.2/drupaljsonapiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.1/drupaljsonapiclient/filter.py` & `drupaljsonapiclient-1.0.2/drupaljsonapiclient/filter.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.1/drupaljsonapiclient/objects.py` & `drupaljsonapiclient-1.0.2/drupaljsonapiclient/objects.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.1/drupaljsonapiclient/relationships.py` & `drupaljsonapiclient-1.0.2/drupaljsonapiclient/relationships.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.1/drupaljsonapiclient/resourceobject.py` & `drupaljsonapiclient-1.0.2/drupaljsonapiclient/resourceobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,22 +277,14 @@
             return rel.SingleRelationship
         else:
             raise ValidationError('Must have either links, data or meta in relationship')
 
     def _make_relationship(self, data, relation_type=None, resource_types=None):
         cls = self._determine_class(data, relation_type)
         return cls(self.session, data, resource_types=resource_types,
-                           relation_type=relation_type)
-                           
-                               def mark_clean(self):
-                                       """
-                                               Mark all relationships as clean (not dirty).
-                                                       """
-                                                               for attr in self.values():
-                                                               (self.session, data, resource_types=resource_types,
                    relation_type=relation_type)
 
     def mark_clean(self):
         """
         Mark all relationships as clean (not dirty).
         """
         for attr in self.values():
```

### Comparing `drupaljsonapiclient-1.0.1/drupaljsonapiclient/session.py` & `drupaljsonapiclient-1.0.2/drupaljsonapiclient/session.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.1/pyproject.toml` & `drupaljsonapiclient-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drupaljsonapiclient"
-version = "1.0.1"
+version = "1.0.2"
 description = "Drupal CMS JSON:API client for Python."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drupaljsonapiclient"}]
 repository = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient"
 documentation = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient/-/blob/main/README.md"
```

### Comparing `drupaljsonapiclient-1.0.1/PKG-INFO` & `drupaljsonapiclient-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drupaljsonapiclient
-Version: 1.0.1
+Version: 1.0.2
 Summary: Drupal CMS JSON:API client for Python.
 Home-page: https://gitlab.com/martins-bruvelis/drupaljsonapiclient
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

