# Comparing `tmp/SimpleVectors-0.0.1.tar.gz` & `tmp/SimpleVectors-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleVectors-0.0.1.tar", last modified: Sat Jun 24 16:57:22 2023, max compression
+gzip compressed data, was "SimpleVectors-0.0.2.tar", last modified: Sat Jun 24 17:39:48 2023, max compression
```

## Comparing `SimpleVectors-0.0.1.tar` & `SimpleVectors-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 16:57:22.769436 SimpleVectors-0.0.1/
--rw-rw-rw-   0        0        0      824 2023-06-24 16:57:22.765462 SimpleVectors-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 16:57:22.754446 SimpleVectors-0.0.1/SimpleVectors.egg-info/
--rw-rw-rw-   0        0        0      824 2023-06-24 16:57:22.000000 SimpleVectors-0.0.1/SimpleVectors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-06-24 16:57:22.000000 SimpleVectors-0.0.1/SimpleVectors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 16:57:22.000000 SimpleVectors-0.0.1/SimpleVectors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-24 16:57:22.000000 SimpleVectors-0.0.1/SimpleVectors.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-24 16:57:22.000000 SimpleVectors-0.0.1/SimpleVectors.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 16:57:22.769436 SimpleVectors-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-06-24 16:44:32.000000 SimpleVectors-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 16:57:22.760139 SimpleVectors-0.0.1/simplevectors/
--rw-rw-rw-   0        0        0      783 2023-06-24 16:32:14.000000 SimpleVectors-0.0.1/simplevectors/SimpleVector.py
--rw-rw-rw-   0        0        0       90 2023-06-24 16:38:10.000000 SimpleVectors-0.0.1/simplevectors/__init__.py
--rw-rw-rw-   0        0        0     1195 2023-06-24 16:32:14.000000 SimpleVectors-0.0.1/simplevectors/add_vectors.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:39:48.907071 SimpleVectors-0.0.2/
+-rw-rw-rw-   0        0        0      824 2023-06-24 17:39:48.907071 SimpleVectors-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 17:39:48.895219 SimpleVectors-0.0.2/SimpleVectors.egg-info/
+-rw-rw-rw-   0        0        0      824 2023-06-24 17:39:48.000000 SimpleVectors-0.0.2/SimpleVectors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-06-24 17:39:48.000000 SimpleVectors-0.0.2/SimpleVectors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 17:39:48.000000 SimpleVectors-0.0.2/SimpleVectors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 17:39:48.000000 SimpleVectors-0.0.2/SimpleVectors.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-24 17:39:48.000000 SimpleVectors-0.0.2/SimpleVectors.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 17:39:48.907071 SimpleVectors-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-06-24 17:39:30.000000 SimpleVectors-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:39:48.903783 SimpleVectors-0.0.2/simplevectors/
+-rw-rw-rw-   0        0        0      783 2023-06-24 16:32:14.000000 SimpleVectors-0.0.2/simplevectors/SimpleVector.py
+-rw-rw-rw-   0        0        0       92 2023-06-24 17:39:39.000000 SimpleVectors-0.0.2/simplevectors/__init__.py
+-rw-rw-rw-   0        0        0     1195 2023-06-24 16:32:14.000000 SimpleVectors-0.0.2/simplevectors/add_vectors.py
```

### Comparing `SimpleVectors-0.0.1/PKG-INFO` & `SimpleVectors-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SimpleVectors
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Package for playing with Simple Vectors passing through a point
 Home-page: UNKNOWN
 Author: Jonathan Ghodke
 Author-email: Jonathanghodke@gmail.com
 License: UNKNOWN
 Description: Very easy to use module which provides to play with vectors using their magnitude and direction (angle) w.r.t x-axis, also all the vectors which will be added are assumed to be passing through the same line
 Keywords: python,Vectors,vectors,simple vectors
```

### Comparing `SimpleVectors-0.0.1/SimpleVectors.egg-info/PKG-INFO` & `SimpleVectors-0.0.2/SimpleVectors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SimpleVectors
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Package for playing with Simple Vectors passing through a point
 Home-page: UNKNOWN
 Author: Jonathan Ghodke
 Author-email: Jonathanghodke@gmail.com
 License: UNKNOWN
 Description: Very easy to use module which provides to play with vectors using their magnitude and direction (angle) w.r.t x-axis, also all the vectors which will be added are assumed to be passing through the same line
 Keywords: python,Vectors,vectors,simple vectors
```

### Comparing `SimpleVectors-0.0.1/setup.py` & `SimpleVectors-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Python Package for playing with Simple Vectors passing through a point'
 LONG_DESCRIPTION = 'Very easy to use module which provides to play with vectors using their magnitude and direction (angle) w.r.t x-axis, also all the vectors which will be added are assumed to be passing through the same line'
 
 # Setting up
 setup(
         name="SimpleVectors", 
         version=VERSION,
```

### Comparing `SimpleVectors-0.0.1/simplevectors/SimpleVector.py` & `SimpleVectors-0.0.2/simplevectors/SimpleVector.py`

 * *Files identical despite different names*

### Comparing `SimpleVectors-0.0.1/simplevectors/add_vectors.py` & `SimpleVectors-0.0.2/simplevectors/add_vectors.py`

 * *Files identical despite different names*

