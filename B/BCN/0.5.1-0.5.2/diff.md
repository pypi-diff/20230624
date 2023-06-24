# Comparing `tmp/BCN-0.5.1.tar.gz` & `tmp/BCN-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BCN-0.5.1.tar", last modified: Fri Apr 21 19:39:55 2023, max compression
+gzip compressed data, was "dist/BCN-0.5.2.tar", last modified: Sat Jun 24 02:47:30 2023, max compression
```

## Comparing `BCN-0.5.1.tar` & `BCN-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.320455 BCN-0.5.1/
-drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.312237 BCN-0.5.1/BCN/
--rw-r--r--   0 t          (501) staff       (20)     5946 2023-04-21 19:36:22.000000 BCN-0.5.1/BCN/BCNClassifier.py
--rw-r--r--   0 t          (501) staff       (20)     5647 2023-04-21 19:36:12.000000 BCN-0.5.1/BCN/BCNRegressor.py
--rw-r--r--   0 t          (501) staff       (20)      252 2023-04-21 19:37:10.000000 BCN-0.5.1/BCN/__init__.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.316614 BCN-0.5.1/BCN.egg-info/
--rw-r--r--   0 t          (501) staff       (20)      763 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/PKG-INFO
--rw-r--r--   0 t          (501) staff       (20)      354 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/SOURCES.txt
--rw-r--r--   0 t          (501) staff       (20)        1 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/dependency_links.txt
--rw-r--r--   0 t          (501) staff       (20)        1 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/not-zip-safe
--rw-r--r--   0 t          (501) staff       (20)      139 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/requires.txt
--rw-r--r--   0 t          (501) staff       (20)        4 2023-04-21 19:39:55.000000 BCN-0.5.1/BCN.egg-info/top_level.txt
--rw-r--r--   0 t          (501) staff       (20)     1455 2022-08-12 14:12:40.000000 BCN-0.5.1/CONTRIBUTING.rst
--rw-r--r--   0 t          (501) staff       (20)      318 2022-08-18 09:42:24.000000 BCN-0.5.1/HISTORY.rst
--rw-r--r--   0 t          (501) staff       (20)     1690 2022-08-09 13:17:37.000000 BCN-0.5.1/LICENSE
--rw-r--r--   0 t          (501) staff       (20)      242 2022-08-09 13:17:37.000000 BCN-0.5.1/MANIFEST.in
--rw-r--r--   0 t          (501) staff       (20)      763 2023-04-21 19:39:55.320747 BCN-0.5.1/PKG-INFO
--rw-r--r--   0 t          (501) staff       (20)     2917 2022-08-18 09:42:24.000000 BCN-0.5.1/README.rst
-drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.303765 BCN-0.5.1/docs/
-drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.303934 BCN-0.5.1/docs/site/
-drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.317222 BCN-0.5.1/docs/site/img/
--rw-r--r--   0 t          (501) staff       (20)     1458 2022-10-04 06:04:46.000000 BCN-0.5.1/docs/site/img/grid.png
--rw-r--r--   0 t          (501) staff       (20)      375 2023-04-21 19:39:55.321925 BCN-0.5.1/setup.cfg
--rw-r--r--   0 t          (501) staff       (20)     1767 2023-04-21 19:19:50.000000 BCN-0.5.1/setup.py
-drwxr-xr-x   0 t          (501) staff       (20)        0 2023-04-21 19:39:55.319347 BCN-0.5.1/tests/
--rw-r--r--   0 t          (501) staff       (20)       33 2022-08-09 13:17:37.000000 BCN-0.5.1/tests/__init__.py
--rw-r--r--   0 t          (501) staff       (20)      367 2022-08-09 13:17:37.000000 BCN-0.5.1/tests/test_BCN.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-06-24 02:47:30.425915 BCN-0.5.2/
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-06-24 02:47:30.409390 BCN-0.5.2/BCN/
+-rw-r--r--   0 t          (501) staff       (20)     5946 2023-04-21 19:36:22.000000 BCN-0.5.2/BCN/BCNClassifier.py
+-rw-r--r--   0 t          (501) staff       (20)     5647 2023-04-21 19:36:12.000000 BCN-0.5.2/BCN/BCNRegressor.py
+-rw-r--r--   0 t          (501) staff       (20)      252 2023-06-24 02:40:55.000000 BCN-0.5.2/BCN/__init__.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-06-24 02:47:30.420058 BCN-0.5.2/BCN.egg-info/
+-rw-r--r--   0 t          (501) staff       (20)      763 2023-06-24 02:47:30.000000 BCN-0.5.2/BCN.egg-info/PKG-INFO
+-rw-r--r--   0 t          (501) staff       (20)      354 2023-06-24 02:47:30.000000 BCN-0.5.2/BCN.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (501) staff       (20)        1 2023-06-24 02:47:30.000000 BCN-0.5.2/BCN.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (501) staff       (20)        1 2023-06-24 02:47:30.000000 BCN-0.5.2/BCN.egg-info/not-zip-safe
+-rw-r--r--   0 t          (501) staff       (20)      166 2023-06-24 02:47:30.000000 BCN-0.5.2/BCN.egg-info/requires.txt
+-rw-r--r--   0 t          (501) staff       (20)        4 2023-06-24 02:47:30.000000 BCN-0.5.2/BCN.egg-info/top_level.txt
+-rw-r--r--   0 t          (501) staff       (20)     1455 2022-08-12 14:12:40.000000 BCN-0.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 t          (501) staff       (20)      318 2022-08-18 09:42:24.000000 BCN-0.5.2/HISTORY.rst
+-rw-r--r--   0 t          (501) staff       (20)     1690 2022-08-09 13:17:37.000000 BCN-0.5.2/LICENSE
+-rw-r--r--   0 t          (501) staff       (20)      242 2022-08-09 13:17:37.000000 BCN-0.5.2/MANIFEST.in
+-rw-r--r--   0 t          (501) staff       (20)      763 2023-06-24 02:47:30.426123 BCN-0.5.2/PKG-INFO
+-rw-r--r--   0 t          (501) staff       (20)     3168 2023-06-24 02:00:49.000000 BCN-0.5.2/README.rst
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-06-24 02:47:30.395193 BCN-0.5.2/docs/
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-06-24 02:47:30.395383 BCN-0.5.2/docs/site/
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-06-24 02:47:30.420837 BCN-0.5.2/docs/site/img/
+-rw-r--r--   0 t          (501) staff       (20)     1458 2022-10-04 06:04:46.000000 BCN-0.5.2/docs/site/img/grid.png
+-rw-r--r--   0 t          (501) staff       (20)      375 2023-06-24 02:47:30.427646 BCN-0.5.2/setup.cfg
+-rw-r--r--   0 t          (501) staff       (20)     1767 2023-06-24 02:40:21.000000 BCN-0.5.2/setup.py
+drwxr-xr-x   0 t          (501) staff       (20)        0 2023-06-24 02:47:30.424791 BCN-0.5.2/tests/
+-rw-r--r--   0 t          (501) staff       (20)       33 2022-08-09 13:17:37.000000 BCN-0.5.2/tests/__init__.py
+-rw-r--r--   0 t          (501) staff       (20)      367 2022-08-09 13:17:37.000000 BCN-0.5.2/tests/test_BCN.py
```

### Comparing `BCN-0.5.1/BCN/BCNClassifier.py` & `BCN-0.5.2/BCN/BCNClassifier.py`

 * *Files identical despite different names*

### Comparing `BCN-0.5.1/BCN/BCNRegressor.py` & `BCN-0.5.2/BCN/BCNRegressor.py`

 * *Files identical despite different names*

### Comparing `BCN-0.5.1/BCN.egg-info/PKG-INFO` & `BCN-0.5.2/BCN.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BCN
-Version: 0.5.1
+Version: 0.5.2
 Summary: Boosted Configuration Networks
 Home-page: https://github.com/Techtonique/bcn_python
 Author: T. Moudiki
 Author-email: thierry.moudiki@gmail.com
 License: BSD license
 Keywords: BCN,Machine Learning,Statistical Learning
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `BCN-0.5.1/CONTRIBUTING.rst` & `BCN-0.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `BCN-0.5.1/LICENSE` & `BCN-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BCN-0.5.1/PKG-INFO` & `BCN-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BCN
-Version: 0.5.1
+Version: 0.5.2
 Summary: Boosted Configuration Networks
 Home-page: https://github.com/Techtonique/bcn_python
 Author: T. Moudiki
 Author-email: thierry.moudiki@gmail.com
 License: BSD license
 Keywords: BCN,Machine Learning,Statistical Learning
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `BCN-0.5.1/README.rst` & `BCN-0.5.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,20 @@
 
 .. image:: https://img.shields.io/badge/documentation-is_here-green
         :target: https://techtonique.github.io/bcn_python/   
 
 
 This package contains an implementation of **Boosted Configuration (*neural*) Networks** 
 (BCNs). How do BCNs work? By creating ensembles (boosting in a supervised way) of single-layered 
-feedforward (*neural*) Networks.
+feedforward (*neural*) Networks. Interested in learning more about BCNs? You can read: 
+
+* https://thierrymoudiki.github.io/blog/2022/07/21/r/misc/boosted-configuration-networks 
+
+* https://thierrymoudiki.github.io/blog/2022/10/05/python/explainableml/interpretation-and-PI-for-BCN.
+
 
 It's worth mentioning that this Python package is built on top of the `R package`_, thanks 
 to ``rpy2``.
 
 Installing BCN
 --------
```

### Comparing `BCN-0.5.1/docs/site/img/grid.png` & `BCN-0.5.2/docs/site/img/grid.png`

 * *Files identical despite different names*

### Comparing `BCN-0.5.1/setup.py` & `BCN-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     include_package_data=True,
     keywords=['BCN', 'Machine Learning', 'Statistical Learning'],
     name='BCN',
     packages=find_packages(include=['BCN', 'BCN.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Techtonique/bcn_python',
-    version='0.5.1',
+    version='0.5.2',
     zip_safe=False,
 )
```

