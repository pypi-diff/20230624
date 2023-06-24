# Comparing `tmp/SimpleVectors-0.0.3.tar.gz` & `tmp/SimpleVectors-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleVectors-0.0.3.tar", last modified: Sat Jun 24 17:42:34 2023, max compression
+gzip compressed data, was "SimpleVectors-0.0.4.tar", last modified: Sat Jun 24 17:47:22 2023, max compression
```

## Comparing `SimpleVectors-0.0.3.tar` & `SimpleVectors-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 17:42:34.016173 SimpleVectors-0.0.3/
--rw-rw-rw-   0        0        0      824 2023-06-24 17:42:34.013814 SimpleVectors-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 17:42:33.997097 SimpleVectors-0.0.3/SimpleVectors.egg-info/
--rw-rw-rw-   0        0        0      824 2023-06-24 17:42:33.000000 SimpleVectors-0.0.3/SimpleVectors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-06-24 17:42:33.000000 SimpleVectors-0.0.3/SimpleVectors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 17:42:33.000000 SimpleVectors-0.0.3/SimpleVectors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-24 17:42:33.000000 SimpleVectors-0.0.3/SimpleVectors.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-24 17:42:33.000000 SimpleVectors-0.0.3/SimpleVectors.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 17:42:34.016173 SimpleVectors-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-06-24 17:42:27.000000 SimpleVectors-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:42:34.010543 SimpleVectors-0.0.3/simplevectors/
--rw-rw-rw-   0        0        0      783 2023-06-24 16:32:14.000000 SimpleVectors-0.0.3/simplevectors/SimpleVector.py
--rw-rw-rw-   0        0        0       92 2023-06-24 17:39:39.000000 SimpleVectors-0.0.3/simplevectors/__init__.py
--rw-rw-rw-   0        0        0     1196 2023-06-24 17:42:11.000000 SimpleVectors-0.0.3/simplevectors/add_vectors.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:47:22.579934 SimpleVectors-0.0.4/
+-rw-rw-rw-   0        0        0      824 2023-06-24 17:47:22.578607 SimpleVectors-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 17:47:22.570268 SimpleVectors-0.0.4/SimpleVectors.egg-info/
+-rw-rw-rw-   0        0        0      824 2023-06-24 17:47:22.000000 SimpleVectors-0.0.4/SimpleVectors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-06-24 17:47:22.000000 SimpleVectors-0.0.4/SimpleVectors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 17:47:22.000000 SimpleVectors-0.0.4/SimpleVectors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 17:47:22.000000 SimpleVectors-0.0.4/SimpleVectors.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-24 17:47:22.000000 SimpleVectors-0.0.4/SimpleVectors.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 17:47:22.579934 SimpleVectors-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-06-24 17:46:39.000000 SimpleVectors-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:47:22.575447 SimpleVectors-0.0.4/simplevectors/
+-rw-rw-rw-   0        0        0      783 2023-06-24 16:32:14.000000 SimpleVectors-0.0.4/simplevectors/SimpleVector.py
+-rw-rw-rw-   0        0        0       95 2023-06-24 17:45:42.000000 SimpleVectors-0.0.4/simplevectors/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-06-24 17:45:30.000000 SimpleVectors-0.0.4/simplevectors/add_vectors.py
```

### Comparing `SimpleVectors-0.0.3/PKG-INFO` & `SimpleVectors-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SimpleVectors
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Package for playing with Simple Vectors passing through a point
 Home-page: UNKNOWN
 Author: Jonathan Ghodke
 Author-email: Jonathanghodke@gmail.com
 License: UNKNOWN
 Description: Very easy to use module which provides to play with vectors using their magnitude and direction (angle) w.r.t x-axis, also all the vectors which will be added are assumed to be passing through the same line
 Keywords: python,Vectors,vectors,simple vectors
```

### Comparing `SimpleVectors-0.0.3/SimpleVectors.egg-info/PKG-INFO` & `SimpleVectors-0.0.4/SimpleVectors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SimpleVectors
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Package for playing with Simple Vectors passing through a point
 Home-page: UNKNOWN
 Author: Jonathan Ghodke
 Author-email: Jonathanghodke@gmail.com
 License: UNKNOWN
 Description: Very easy to use module which provides to play with vectors using their magnitude and direction (angle) w.r.t x-axis, also all the vectors which will be added are assumed to be passing through the same line
 Keywords: python,Vectors,vectors,simple vectors
```

### Comparing `SimpleVectors-0.0.3/setup.py` & `SimpleVectors-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'Python Package for playing with Simple Vectors passing through a point'
 LONG_DESCRIPTION = 'Very easy to use module which provides to play with vectors using their magnitude and direction (angle) w.r.t x-axis, also all the vectors which will be added are assumed to be passing through the same line'
 
 # Setting up
 setup(
         name="SimpleVectors", 
         version=VERSION,
```

### Comparing `SimpleVectors-0.0.3/simplevectors/SimpleVector.py` & `SimpleVectors-0.0.4/simplevectors/SimpleVector.py`

 * *Files identical despite different names*

### Comparing `SimpleVectors-0.0.3/simplevectors/add_vectors.py` & `SimpleVectors-0.0.4/simplevectors/add_vectors.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .SimpleVector import simplevector, InvalidVectorError
 
 
 
 
 
 #add accepts multiple vectors as simplevector objects and returns a resultant vector as a simplevector object. 
-def add(*args):
+def addvectors(*args):
     resultant_vector = simplevector(0,0)
     unit_vectors = []
     magnitude_vectors = []
     force_vectors = []
 
     for vector in args:
         #
```

