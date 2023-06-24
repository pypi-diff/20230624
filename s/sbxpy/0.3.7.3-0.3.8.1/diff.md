# Comparing `tmp/sbxpy-0.3.7.3.tar.gz` & `tmp/sbxpy-0.3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbxpy-0.3.7.3.tar", last modified: Fri Apr 14 15:24:05 2023, max compression
+gzip compressed data, was "sbxpy-0.3.8.1.tar", last modified: Sat Jun 24 18:22:05 2023, max compression
```

## Comparing `sbxpy-0.3.7.3.tar` & `sbxpy-0.3.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 martinzuleta   (501) staff       (20)        0 2023-04-14 15:24:05.549284 sbxpy-0.3.7.3/
--rw-r--r--   0 martinzuleta   (501) staff       (20)     1061 2023-04-14 14:56:05.000000 sbxpy-0.3.7.3/LICENSE
--rw-r--r--   0 martinzuleta   (501) staff       (20)      529 2023-04-14 15:24:05.549063 sbxpy-0.3.7.3/PKG-INFO
--rw-r--r--   0 martinzuleta   (501) staff       (20)      338 2023-04-14 14:56:05.000000 sbxpy-0.3.7.3/README.md
-drwxr-xr-x   0 martinzuleta   (501) staff       (20)        0 2023-04-14 15:24:05.547930 sbxpy-0.3.7.3/sbxpy/
--rw-r--r--   0 martinzuleta   (501) staff       (20)     3460 2023-04-14 14:56:05.000000 sbxpy-0.3.7.3/sbxpy/QueryBuilder.py
--rw-r--r--   0 martinzuleta   (501) staff       (20)    30408 2023-04-14 14:56:05.000000 sbxpy-0.3.7.3/sbxpy/__init__.py
-drwxr-xr-x   0 martinzuleta   (501) staff       (20)        0 2023-04-14 15:24:05.548848 sbxpy-0.3.7.3/sbxpy.egg-info/
--rw-r--r--   0 martinzuleta   (501) staff       (20)      529 2023-04-14 15:24:05.000000 sbxpy-0.3.7.3/sbxpy.egg-info/PKG-INFO
--rw-r--r--   0 martinzuleta   (501) staff       (20)      210 2023-04-14 15:24:05.000000 sbxpy-0.3.7.3/sbxpy.egg-info/SOURCES.txt
--rw-r--r--   0 martinzuleta   (501) staff       (20)        1 2023-04-14 15:24:05.000000 sbxpy-0.3.7.3/sbxpy.egg-info/dependency_links.txt
--rw-r--r--   0 martinzuleta   (501) staff       (20)       15 2023-04-14 15:24:05.000000 sbxpy-0.3.7.3/sbxpy.egg-info/requires.txt
--rw-r--r--   0 martinzuleta   (501) staff       (20)        6 2023-04-14 15:24:05.000000 sbxpy-0.3.7.3/sbxpy.egg-info/top_level.txt
--rw-r--r--   0 martinzuleta   (501) staff       (20)       38 2023-04-14 15:24:05.549324 sbxpy-0.3.7.3/setup.cfg
--rw-r--r--   0 martinzuleta   (501) staff       (20)      791 2023-04-14 15:23:34.000000 sbxpy-0.3.7.3/setup.py
+drwxr-xr-x   0 luisguzman   (501) staff       (20)        0 2023-06-24 18:22:05.766777 sbxpy-0.3.8.1/
+-rw-r--r--   0 luisguzman   (501) staff       (20)     1061 2022-10-11 16:44:17.000000 sbxpy-0.3.8.1/LICENSE
+-rw-r--r--   0 luisguzman   (501) staff       (20)      529 2023-06-24 18:22:05.766356 sbxpy-0.3.8.1/PKG-INFO
+-rw-r--r--   0 luisguzman   (501) staff       (20)      338 2022-10-11 16:44:17.000000 sbxpy-0.3.8.1/README.md
+drwxr-xr-x   0 luisguzman   (501) staff       (20)        0 2023-06-24 18:22:05.764282 sbxpy-0.3.8.1/sbxpy/
+-rw-r--r--   0 luisguzman   (501) staff       (20)     3460 2023-06-24 18:21:30.000000 sbxpy-0.3.8.1/sbxpy/QueryBuilder.py
+-rw-r--r--   0 luisguzman   (501) staff       (20)    30408 2023-06-24 18:21:30.000000 sbxpy-0.3.8.1/sbxpy/__init__.py
+drwxr-xr-x   0 luisguzman   (501) staff       (20)        0 2023-06-24 18:22:05.765950 sbxpy-0.3.8.1/sbxpy.egg-info/
+-rw-r--r--   0 luisguzman   (501) staff       (20)      529 2023-06-24 18:22:05.000000 sbxpy-0.3.8.1/sbxpy.egg-info/PKG-INFO
+-rw-r--r--   0 luisguzman   (501) staff       (20)      210 2023-06-24 18:22:05.000000 sbxpy-0.3.8.1/sbxpy.egg-info/SOURCES.txt
+-rw-r--r--   0 luisguzman   (501) staff       (20)        1 2023-06-24 18:22:05.000000 sbxpy-0.3.8.1/sbxpy.egg-info/dependency_links.txt
+-rw-r--r--   0 luisguzman   (501) staff       (20)       15 2023-06-24 18:22:05.000000 sbxpy-0.3.8.1/sbxpy.egg-info/requires.txt
+-rw-r--r--   0 luisguzman   (501) staff       (20)        6 2023-06-24 18:22:05.000000 sbxpy-0.3.8.1/sbxpy.egg-info/top_level.txt
+-rw-r--r--   0 luisguzman   (501) staff       (20)       38 2023-06-24 18:22:05.766891 sbxpy-0.3.8.1/setup.cfg
+-rw-r--r--   0 luisguzman   (501) staff       (20)      791 2023-06-24 18:22:03.000000 sbxpy-0.3.8.1/setup.py
```

### Comparing `sbxpy-0.3.7.3/LICENSE` & `sbxpy-0.3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sbxpy-0.3.7.3/PKG-INFO` & `sbxpy-0.3.8.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbxpy
-Version: 0.3.7.3
+Version: 0.3.8.1
 Summary: This is the module  create all request used to communicate with SbxCloud
 Home-page: https://github.com/sbxcloud/sbxcloudpython
 Author: Luis Guzmán
 Author-email: lgguzman890414@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sbxpy-0.3.7.3/sbxpy/QueryBuilder.py` & `sbxpy-0.3.8.1/sbxpy/QueryBuilder.py`

 * *Files identical despite different names*

### Comparing `sbxpy-0.3.7.3/sbxpy/__init__.py` & `sbxpy-0.3.8.1/sbxpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sbxpy-0.3.7.3/sbxpy.egg-info/PKG-INFO` & `sbxpy-0.3.8.1/sbxpy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbxpy
-Version: 0.3.7.3
+Version: 0.3.8.1
 Summary: This is the module  create all request used to communicate with SbxCloud
 Home-page: https://github.com/sbxcloud/sbxcloudpython
 Author: Luis Guzmán
 Author-email: lgguzman890414@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sbxpy-0.3.7.3/setup.py` & `sbxpy-0.3.8.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sbxpy",
-    version="0.3.7.3",
+    version="0.3.8.1",
     author="Luis Guzmán",
     author_email="lgguzman890414@gmail.com",
     description="This is the module  create all request used to communicate with SbxCloud",
     long_description="This is the module  create all request used to communicate with SbxCloud",
     long_description_content_type="text/markdown",
     url="https://github.com/sbxcloud/sbxcloudpython",
     packages=setuptools.find_packages(),
```

