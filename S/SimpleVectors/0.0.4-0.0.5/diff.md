# Comparing `tmp/SimpleVectors-0.0.4.tar.gz` & `tmp/SimpleVectors-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleVectors-0.0.4.tar", last modified: Sat Jun 24 17:47:22 2023, max compression
+gzip compressed data, was "SimpleVectors-0.0.5.tar", last modified: Sat Jun 24 17:56:22 2023, max compression
```

## Comparing `SimpleVectors-0.0.4.tar` & `SimpleVectors-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 17:47:22.579934 SimpleVectors-0.0.4/
--rw-rw-rw-   0        0        0      824 2023-06-24 17:47:22.578607 SimpleVectors-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 17:47:22.570268 SimpleVectors-0.0.4/SimpleVectors.egg-info/
--rw-rw-rw-   0        0        0      824 2023-06-24 17:47:22.000000 SimpleVectors-0.0.4/SimpleVectors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-06-24 17:47:22.000000 SimpleVectors-0.0.4/SimpleVectors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 17:47:22.000000 SimpleVectors-0.0.4/SimpleVectors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-24 17:47:22.000000 SimpleVectors-0.0.4/SimpleVectors.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-24 17:47:22.000000 SimpleVectors-0.0.4/SimpleVectors.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 17:47:22.579934 SimpleVectors-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-06-24 17:46:39.000000 SimpleVectors-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:47:22.575447 SimpleVectors-0.0.4/simplevectors/
--rw-rw-rw-   0        0        0      783 2023-06-24 16:32:14.000000 SimpleVectors-0.0.4/simplevectors/SimpleVector.py
--rw-rw-rw-   0        0        0       95 2023-06-24 17:45:42.000000 SimpleVectors-0.0.4/simplevectors/__init__.py
--rw-rw-rw-   0        0        0     1203 2023-06-24 17:45:30.000000 SimpleVectors-0.0.4/simplevectors/add_vectors.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:56:22.731849 SimpleVectors-0.0.5/
+-rw-rw-rw-   0        0        0     1503 2023-06-24 17:56:22.730791 SimpleVectors-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-06-24 17:54:02.000000 SimpleVectors-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 17:56:22.723702 SimpleVectors-0.0.5/SimpleVectors.egg-info/
+-rw-rw-rw-   0        0        0     1503 2023-06-24 17:56:22.000000 SimpleVectors-0.0.5/SimpleVectors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-24 17:56:22.000000 SimpleVectors-0.0.5/SimpleVectors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 17:56:22.000000 SimpleVectors-0.0.5/SimpleVectors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 17:56:22.000000 SimpleVectors-0.0.5/SimpleVectors.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-24 17:56:22.000000 SimpleVectors-0.0.5/SimpleVectors.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 17:56:22.731849 SimpleVectors-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2023-06-24 17:56:15.000000 SimpleVectors-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:56:22.726921 SimpleVectors-0.0.5/simplevectors/
+-rw-rw-rw-   0        0        0      783 2023-06-24 16:32:14.000000 SimpleVectors-0.0.5/simplevectors/SimpleVector.py
+-rw-rw-rw-   0        0        0       95 2023-06-24 17:45:42.000000 SimpleVectors-0.0.5/simplevectors/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-06-24 17:45:30.000000 SimpleVectors-0.0.5/simplevectors/add_vectors.py
```

### Comparing `SimpleVectors-0.0.4/setup.py` & `SimpleVectors-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from setuptools import setup, find_packages
+from pathlib import Path
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'Python Package for playing with Simple Vectors passing through a point'
-LONG_DESCRIPTION = 'Very easy to use module which provides to play with vectors using their magnitude and direction (angle) w.r.t x-axis, also all the vectors which will be added are assumed to be passing through the same line'
 
+this_directory = Path(__file__).parent
+LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 # Setting up
 setup(
         name="SimpleVectors", 
         version=VERSION,
         author="Jonathan Ghodke",
         author_email="Jonathanghodke@gmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
+	long_description_content_type='text/markdown',
         packages=find_packages(),
         install_requires=['numpy', 'matplotlib'],
         keywords=['python', 'Vectors', 'vectors', 'simple vectors'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
```

### Comparing `SimpleVectors-0.0.4/simplevectors/SimpleVector.py` & `SimpleVectors-0.0.5/simplevectors/SimpleVector.py`

 * *Files identical despite different names*

### Comparing `SimpleVectors-0.0.4/simplevectors/add_vectors.py` & `SimpleVectors-0.0.5/simplevectors/add_vectors.py`

 * *Files identical despite different names*

