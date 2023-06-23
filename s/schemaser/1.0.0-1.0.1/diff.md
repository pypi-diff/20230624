# Comparing `tmp/schemaser-1.0.0.tar.gz` & `tmp/schemaser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemaser-1.0.0.tar", last modified: Thu Jun 15 22:04:17 2023, max compression
+gzip compressed data, was "schemaser-1.0.1.tar", last modified: Fri Jun 23 22:12:10 2023, max compression
```

## Comparing `schemaser-1.0.0.tar` & `schemaser-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 22:04:17.762302 schemaser-1.0.0/
--rw-rw-rw-   0        0        0     1320 2023-06-15 22:04:17.762302 schemaser-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-06-15 22:02:03.000000 schemaser-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 22:04:17.752238 schemaser-1.0.0/schemaser/
--rw-rw-rw-   0        0        0     4359 2023-06-15 22:00:34.000000 schemaser-1.0.0/schemaser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 22:04:17.761302 schemaser-1.0.0/schemaser.egg-info/
--rw-rw-rw-   0        0        0     1320 2023-06-15 22:04:17.000000 schemaser-1.0.0/schemaser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-15 22:04:17.000000 schemaser-1.0.0/schemaser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 22:04:17.000000 schemaser-1.0.0/schemaser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-15 22:04:17.000000 schemaser-1.0.0/schemaser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-06-15 22:04:17.762302 schemaser-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1110 2023-06-15 21:57:04.000000 schemaser-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 22:12:10.532510 schemaser-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2023-06-15 22:05:40.000000 schemaser-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1343 2023-06-23 22:12:10.532510 schemaser-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-06-15 22:02:03.000000 schemaser-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 22:12:10.519441 schemaser-1.0.1/schemaser/
+-rw-rw-rw-   0        0        0     4377 2023-06-23 22:10:15.000000 schemaser-1.0.1/schemaser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 22:12:10.531510 schemaser-1.0.1/schemaser.egg-info/
+-rw-rw-rw-   0        0        0     1343 2023-06-23 22:12:10.000000 schemaser-1.0.1/schemaser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-23 22:12:10.000000 schemaser-1.0.1/schemaser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 22:12:10.000000 schemaser-1.0.1/schemaser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-23 22:12:10.000000 schemaser-1.0.1/schemaser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-06-23 22:12:10.533510 schemaser-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2023-06-23 22:11:21.000000 schemaser-1.0.1/setup.py
```

### Comparing `schemaser-1.0.0/PKG-INFO` & `schemaser-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: schemaser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Converts a Python class or method to a JSON schema.
 Home-page: https://github.com/legopitstop/schemaser
 Author: Legopitstop
 Author-email: officiallegopitstop@gmail.com
 License: MIT
 Keywords: json,jsonschema,schema,class,method
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # schemaser
 Converts a Python class or method to a JSON schema.
 
 ## Install
 ```
 pip install schemaser
```

### Comparing `schemaser-1.0.0/README.md` & `schemaser-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `schemaser-1.0.0/schemaser/__init__.py` & `schemaser-1.0.1/schemaser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import EnumMeta
 import typing
 import inspect
 import types
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 def to_json_type(instance, root:dict=None) -> dict:
     """
     Converts a Python type to JSON type.
 
     Arguments
     ---
@@ -107,11 +107,12 @@
                     if v.default == inspect._empty: result['required'].append(k)
 
                     obj = to_json_type(v.annotation, result if root is None else root) # type, definitions, refrance
                     if obj is not None:
                         for k,v in obj.items(): prop[k] = v # Merge with prop
                 else:
                     result['additionalProperties'] = to_json_type(v.annotation, result if root is None else root)
+            i+=1
 
         # Description
         if cls_or_func.__doc__ is not None: result['description'] = cls_or_func.__doc__
         return result
```

### Comparing `schemaser-1.0.0/schemaser.egg-info/PKG-INFO` & `schemaser-1.0.1/schemaser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: schemaser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Converts a Python class or method to a JSON schema.
 Home-page: https://github.com/legopitstop/schemaser
 Author: Legopitstop
 Author-email: officiallegopitstop@gmail.com
 License: MIT
 Keywords: json,jsonschema,schema,class,method
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # schemaser
 Converts a Python class or method to a JSON schema.
 
 ## Install
 ```
 pip install schemaser
```

### Comparing `schemaser-1.0.0/setup.py` & `schemaser-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     long_description = f.read()
 
 required_modules = []
 
 setuptools.setup(
     name='schemaser',
-    version='1.0.0',
+    version='1.0.1',
     author='Legopitstop',
     description='Converts a Python class or method to a JSON schema.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/legopitstop/schemaser',
     packages=setuptools.find_packages(),
     install_requires=required_modules,
```

