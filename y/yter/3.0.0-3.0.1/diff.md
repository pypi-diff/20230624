# Comparing `tmp/yter-3.0.0.tar.gz` & `tmp/yter-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yter-3.0.0.tar", last modified: Sat Jun 24 02:17:15 2023, max compression
+gzip compressed data, was "yter-3.0.1.tar", last modified: Sat Jun 24 02:29:29 2023, max compression
```

## Comparing `yter-3.0.0.tar` & `yter-3.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 02:17:15.428684 yter-3.0.0/
--rw-rw-rw-   0        0        0     1081 2023-03-09 15:02:41.000000 yter-3.0.0/LICENSE
--rw-rw-rw-   0        0        0       18 2023-03-09 15:02:41.000000 yter-3.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2519 2023-06-24 02:17:15.427698 yter-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1874 2023-06-24 02:08:31.000000 yter-3.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 02:17:15.428684 yter-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      926 2023-03-09 15:02:41.000000 yter-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:17:15.405369 yter-3.0.0/test/
--rw-rw-rw-   0        0        0     3893 2023-05-29 14:39:48.000000 yter-3.0.0/test/test_fun.py
--rw-rw-rw-   0        0        0     1287 2023-06-14 05:23:52.000000 yter-3.0.0/test/test_key.py
--rw-rw-rw-   0        0        0      158 2023-03-09 15:02:41.000000 yter-3.0.0/test/test_star.py
--rw-rw-rw-   0        0        0     2142 2023-06-22 03:20:01.000000 yter-3.0.0/test/test_ytr.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:17:15.410013 yter-3.0.0/yter/
--rw-rw-rw-   0        0        0      419 2023-06-14 05:20:37.000000 yter-3.0.0/yter/__init__.py
--rw-rw-rw-   0        0        0    11952 2023-06-22 02:44:16.000000 yter-3.0.0/yter/_fun.py
--rw-rw-rw-   0        0        0     4692 2023-06-22 02:46:02.000000 yter-3.0.0/yter/_key.py
--rw-rw-rw-   0        0        0     7960 2023-06-22 03:17:54.000000 yter-3.0.0/yter/_ytr.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:17:15.424689 yter-3.0.0/yter.egg-info/
--rw-rw-rw-   0        0        0     2519 2023-06-24 02:17:15.000000 yter-3.0.0/yter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-24 02:17:15.000000 yter-3.0.0/yter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 02:17:15.000000 yter-3.0.0/yter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-24 02:17:15.000000 yter-3.0.0/yter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 15:10:32.000000 yter-3.0.0/yter.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-24 02:29:29.763522 yter-3.0.1/
+-rw-rw-rw-   0        0        0     1081 2023-03-09 15:02:41.000000 yter-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-03-09 15:02:41.000000 yter-3.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2567 2023-06-24 02:29:29.762514 yter-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1921 2023-06-24 02:28:36.000000 yter-3.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 02:29:29.763522 yter-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      926 2023-03-09 15:02:41.000000 yter-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:29:29.742767 yter-3.0.1/test/
+-rw-rw-rw-   0        0        0     3893 2023-05-29 14:39:48.000000 yter-3.0.1/test/test_fun.py
+-rw-rw-rw-   0        0        0     1287 2023-06-14 05:23:52.000000 yter-3.0.1/test/test_key.py
+-rw-rw-rw-   0        0        0      158 2023-03-09 15:02:41.000000 yter-3.0.1/test/test_star.py
+-rw-rw-rw-   0        0        0     2142 2023-06-22 03:20:01.000000 yter-3.0.1/test/test_ytr.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:29:29.748007 yter-3.0.1/yter/
+-rw-rw-rw-   0        0        0      419 2023-06-14 05:20:37.000000 yter-3.0.1/yter/__init__.py
+-rw-rw-rw-   0        0        0    11952 2023-06-22 02:44:16.000000 yter-3.0.1/yter/_fun.py
+-rw-rw-rw-   0        0        0     4692 2023-06-22 02:46:02.000000 yter-3.0.1/yter/_key.py
+-rw-rw-rw-   0        0        0     7960 2023-06-24 02:26:42.000000 yter-3.0.1/yter/_ytr.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:29:29.762008 yter-3.0.1/yter.egg-info/
+-rw-rw-rw-   0        0        0     2567 2023-06-24 02:29:29.000000 yter-3.0.1/yter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-24 02:29:29.000000 yter-3.0.1/yter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 02:29:29.000000 yter-3.0.1/yter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-24 02:29:29.000000 yter-3.0.1/yter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 15:10:32.000000 yter-3.0.1/yter.egg-info/zip-safe
```

### Comparing `yter-3.0.0/LICENSE` & `yter-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yter-3.0.0/PKG-INFO` & `yter-3.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yter
-Version: 3.0.0
+Version: 3.0.1
 Summary: Clever, quick iterators that make your smile whiter
 Home-page: https://gitlab.com/shredwheat/yter
 Author: Peter Shinners
 Author-email: pete@shinners.org
 License: MIT
 Keywords: iterator itertools
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 # yter
 
-Version 3.0.0
+Version 3.0.1`
 2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
 This will work with versions of Python 2.6+ and 3.2+.
 
 
@@ -50,14 +50,15 @@
 * `percent` -- Iterator that skips a percentage of values
 * `flat` -- Iterator of values from a iterable of iterators
 * `chunk` -- Iterator of lists with a fixed size from iterable
 * `key` -- Iterator of pairs of key result and original values
 * `choose` -- Split into iterators for true and false values
 * `unique` -- Iterate only the unique values
 * `duplicates` -- Iterate only the duplicated values
+* `recurse` -- Recurse values from a callable
 
 
 ## Keys
 
 Utility functions that are useful to use as a key argument
 
 * `format` -- Create a function that formats given values into strings
```

### Comparing `yter-3.0.0/README.md` & `yter-3.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # yter
 
-Version 3.0.0
+Version 3.0.1`
 2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
 This will work with versions of Python 2.6+ and 3.2+.
 
 
@@ -33,14 +33,15 @@
 * `percent` -- Iterator that skips a percentage of values
 * `flat` -- Iterator of values from a iterable of iterators
 * `chunk` -- Iterator of lists with a fixed size from iterable
 * `key` -- Iterator of pairs of key result and original values
 * `choose` -- Split into iterators for true and false values
 * `unique` -- Iterate only the unique values
 * `duplicates` -- Iterate only the duplicated values
+* `recurse` -- Recurse values from a callable
 
 
 ## Keys
 
 Utility functions that are useful to use as a key argument
 
 * `format` -- Create a function that formats given values into strings
```

### Comparing `yter-3.0.0/setup.py` & `yter-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `yter-3.0.0/test/test_fun.py` & `yter-3.0.1/test/test_fun.py`

 * *Files identical despite different names*

### Comparing `yter-3.0.0/test/test_key.py` & `yter-3.0.1/test/test_key.py`

 * *Files identical despite different names*

### Comparing `yter-3.0.0/test/test_ytr.py` & `yter-3.0.1/test/test_ytr.py`

 * *Files identical despite different names*

### Comparing `yter-3.0.0/yter/_fun.py` & `yter-3.0.1/yter/_fun.py`

 * *Files identical despite different names*

### Comparing `yter-3.0.0/yter/_key.py` & `yter-3.0.1/yter/_key.py`

 * *Files identical despite different names*

### Comparing `yter-3.0.0/yter/_ytr.py` & `yter-3.0.1/yter/_ytr.py`

 * *Files identical despite different names*

### Comparing `yter-3.0.0/yter.egg-info/PKG-INFO` & `yter-3.0.1/yter.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yter
-Version: 3.0.0
+Version: 3.0.1
 Summary: Clever, quick iterators that make your smile whiter
 Home-page: https://gitlab.com/shredwheat/yter
 Author: Peter Shinners
 Author-email: pete@shinners.org
 License: MIT
 Keywords: iterator itertools
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 # yter
 
-Version 3.0.0
+Version 3.0.1`
 2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
 This will work with versions of Python 2.6+ and 3.2+.
 
 
@@ -50,14 +50,15 @@
 * `percent` -- Iterator that skips a percentage of values
 * `flat` -- Iterator of values from a iterable of iterators
 * `chunk` -- Iterator of lists with a fixed size from iterable
 * `key` -- Iterator of pairs of key result and original values
 * `choose` -- Split into iterators for true and false values
 * `unique` -- Iterate only the unique values
 * `duplicates` -- Iterate only the duplicated values
+* `recurse` -- Recurse values from a callable
 
 
 ## Keys
 
 Utility functions that are useful to use as a key argument
 
 * `format` -- Create a function that formats given values into strings
```

