# Comparing `tmp/erikunicamp-myutils-0.0.8.tar.gz` & `tmp/erikunicamp-myutils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/erikunicamp-myutils-0.0.8.tar", last modified: Tue Aug 11 12:06:03 2020, max compression
+gzip compressed data, was "dist/erikunicamp-myutils-0.0.9.tar", last modified: Tue Aug 11 12:15:43 2020, max compression
```

## Comparing `erikunicamp-myutils-0.0.8.tar` & `erikunicamp-myutils-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 frodo     (1000) frodo     (1000)        0 2020-08-11 12:06:03.000000 erikunicamp-myutils-0.0.8/
--rw-r--r--   0 frodo     (1000) frodo     (1000)      481 2020-08-11 12:06:03.000000 erikunicamp-myutils-0.0.8/PKG-INFO
--rw-r--r--   0 frodo     (1000) frodo     (1000)       21 2020-07-29 20:23:28.000000 erikunicamp-myutils-0.0.8/README.md
-drwxr-xr-x   0 frodo     (1000) frodo     (1000)        0 2020-08-11 12:06:03.000000 erikunicamp-myutils-0.0.8/erikunicamp_myutils.egg-info/
--rw-r--r--   0 frodo     (1000) frodo     (1000)      481 2020-08-11 12:06:02.000000 erikunicamp-myutils-0.0.8/erikunicamp_myutils.egg-info/PKG-INFO
--rw-r--r--   0 frodo     (1000) frodo     (1000)      259 2020-08-11 12:06:02.000000 erikunicamp-myutils-0.0.8/erikunicamp_myutils.egg-info/SOURCES.txt
--rw-r--r--   0 frodo     (1000) frodo     (1000)        1 2020-08-11 12:06:02.000000 erikunicamp-myutils-0.0.8/erikunicamp_myutils.egg-info/dependency_links.txt
--rw-r--r--   0 frodo     (1000) frodo     (1000)        8 2020-08-11 12:06:02.000000 erikunicamp-myutils-0.0.8/erikunicamp_myutils.egg-info/top_level.txt
-drwxr-xr-x   0 frodo     (1000) frodo     (1000)        0 2020-08-11 12:06:03.000000 erikunicamp-myutils-0.0.8/myutils/
--rw-r--r--   0 frodo     (1000) frodo     (1000)      607 2020-08-07 12:16:13.000000 erikunicamp-myutils-0.0.8/myutils/__init__.py
--rw-r--r--   0 frodo     (1000) frodo     (1000)     1728 2020-08-07 12:33:16.000000 erikunicamp-myutils-0.0.8/myutils/graph.py
--rw-r--r--   0 frodo     (1000) frodo     (1000)     1527 2020-07-30 01:41:01.000000 erikunicamp-myutils-0.0.8/myutils/plot.py
--rw-r--r--   0 frodo     (1000) frodo     (1000)    11474 2020-08-11 12:05:25.000000 erikunicamp-myutils-0.0.8/myutils/xnet.py
--rw-r--r--   0 frodo     (1000) frodo     (1000)       38 2020-08-11 12:06:03.000000 erikunicamp-myutils-0.0.8/setup.cfg
--rw-r--r--   0 frodo     (1000) frodo     (1000)      642 2020-08-11 12:05:55.000000 erikunicamp-myutils-0.0.8/setup.py
+drwxr-xr-x   0 frodo     (1000) frodo     (1000)        0 2020-08-11 12:15:43.000000 erikunicamp-myutils-0.0.9/
+-rw-r--r--   0 frodo     (1000) frodo     (1000)      481 2020-08-11 12:15:43.000000 erikunicamp-myutils-0.0.9/PKG-INFO
+-rw-r--r--   0 frodo     (1000) frodo     (1000)       21 2020-07-29 20:23:28.000000 erikunicamp-myutils-0.0.9/README.md
+drwxr-xr-x   0 frodo     (1000) frodo     (1000)        0 2020-08-11 12:15:43.000000 erikunicamp-myutils-0.0.9/erikunicamp_myutils.egg-info/
+-rw-r--r--   0 frodo     (1000) frodo     (1000)      481 2020-08-11 12:15:43.000000 erikunicamp-myutils-0.0.9/erikunicamp_myutils.egg-info/PKG-INFO
+-rw-r--r--   0 frodo     (1000) frodo     (1000)      259 2020-08-11 12:15:43.000000 erikunicamp-myutils-0.0.9/erikunicamp_myutils.egg-info/SOURCES.txt
+-rw-r--r--   0 frodo     (1000) frodo     (1000)        1 2020-08-11 12:15:43.000000 erikunicamp-myutils-0.0.9/erikunicamp_myutils.egg-info/dependency_links.txt
+-rw-r--r--   0 frodo     (1000) frodo     (1000)        8 2020-08-11 12:15:43.000000 erikunicamp-myutils-0.0.9/erikunicamp_myutils.egg-info/top_level.txt
+drwxr-xr-x   0 frodo     (1000) frodo     (1000)        0 2020-08-11 12:15:43.000000 erikunicamp-myutils-0.0.9/myutils/
+-rw-r--r--   0 frodo     (1000) frodo     (1000)      607 2020-08-07 12:16:13.000000 erikunicamp-myutils-0.0.9/myutils/__init__.py
+-rw-r--r--   0 frodo     (1000) frodo     (1000)     1728 2020-08-07 12:33:16.000000 erikunicamp-myutils-0.0.9/myutils/graph.py
+-rw-r--r--   0 frodo     (1000) frodo     (1000)     1527 2020-07-30 01:41:01.000000 erikunicamp-myutils-0.0.9/myutils/plot.py
+-rw-r--r--   0 frodo     (1000) frodo     (1000)    11474 2020-08-11 12:05:25.000000 erikunicamp-myutils-0.0.9/myutils/xnet.py
+-rw-r--r--   0 frodo     (1000) frodo     (1000)       38 2020-08-11 12:15:43.000000 erikunicamp-myutils-0.0.9/setup.cfg
+-rw-r--r--   0 frodo     (1000) frodo     (1000)      642 2020-08-11 12:15:38.000000 erikunicamp-myutils-0.0.9/setup.py
```

### Comparing `erikunicamp-myutils-0.0.8/myutils/__init__.py` & `erikunicamp-myutils-0.0.9/myutils/__init__.py`

 * *Files identical despite different names*

### Comparing `erikunicamp-myutils-0.0.8/myutils/graph.py` & `erikunicamp-myutils-0.0.9/myutils/graph.py`

 * *Files identical despite different names*

### Comparing `erikunicamp-myutils-0.0.8/myutils/plot.py` & `erikunicamp-myutils-0.0.9/myutils/plot.py`

 * *Files identical despite different names*

### Comparing `erikunicamp-myutils-0.0.8/myutils/xnet.py` & `erikunicamp-myutils-0.0.9/myutils/xnet.py`

 * *Files identical despite different names*

### Comparing `erikunicamp-myutils-0.0.8/setup.py` & `erikunicamp-myutils-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="erikunicamp-myutils",
-    version="0.0.8",
+    version="0.0.9",
     author="erikunicamp",
     author_email="erik.unicamp@gmail.com",
     description="Utilities package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tokudaek/myutils",
     packages=setuptools.find_packages(),
```

