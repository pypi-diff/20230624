# Comparing `tmp/coreli-0.0.4.tar.gz` & `tmp/coreli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coreli-0.0.4.tar", last modified: Sun Oct 30 21:30:49 2022, max compression
+gzip compressed data, was "coreli-0.0.5.tar", last modified: Sat Jun 24 12:59:51 2023, max compression
```

## Comparing `coreli-0.0.4.tar` & `coreli-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2022-10-30 21:30:49.590240 coreli-0.0.4/
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     1071 2022-10-30 17:15:46.000000 coreli-0.0.4/LICENSE
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4486 2022-10-30 21:30:49.590240 coreli-0.0.4/PKG-INFO
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3972 2022-10-30 17:15:46.000000 coreli-0.0.4/README.md
-drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2022-10-30 21:30:49.590240 coreli-0.0.4/coreli/
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4028 2022-10-30 17:15:46.000000 coreli-0.0.4/coreli/Collatz_maps.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3294 2022-10-30 17:15:46.000000 coreli-0.0.4/coreli/Collatz_tilings.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      202 2022-10-30 17:15:46.000000 coreli-0.0.4/coreli/__init__.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)    14584 2022-10-30 17:15:46.000000 coreli-0.0.4/coreli/padic_integers.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     9193 2022-10-30 21:30:04.000000 coreli-0.0.4/coreli/parity_vectors.py
-drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2022-10-30 21:30:49.590240 coreli-0.0.4/coreli/tinytiles/
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      119 2022-10-30 17:15:46.000000 coreli-0.0.4/coreli/tinytiles/__init__.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     1406 2022-10-30 17:15:46.000000 coreli-0.0.4/coreli/tinytiles/interactive.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3503 2022-10-30 21:19:25.000000 coreli-0.0.4/coreli/tinytiles/model.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3327 2022-10-30 17:15:46.000000 coreli-0.0.4/coreli/tinytiles/svg_view.py
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     2445 2022-10-30 17:15:46.000000 coreli-0.0.4/coreli/utils.py
-drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2022-10-30 21:30:49.590240 coreli-0.0.4/coreli.egg-info/
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4486 2022-10-30 21:30:49.000000 coreli-0.0.4/coreli.egg-info/PKG-INFO
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      425 2022-10-30 21:30:49.000000 coreli-0.0.4/coreli.egg-info/SOURCES.txt
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)        1 2022-10-30 21:30:49.000000 coreli-0.0.4/coreli.egg-info/dependency_links.txt
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)       25 2022-10-30 21:30:49.000000 coreli-0.0.4/coreli.egg-info/requires.txt
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)        7 2022-10-30 21:30:49.000000 coreli-0.0.4/coreli.egg-info/top_level.txt
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)       38 2022-10-30 21:30:49.590240 coreli-0.0.4/setup.cfg
--rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      824 2022-10-30 21:30:23.000000 coreli-0.0.4/setup.py
+drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-06-24 12:59:51.421962 coreli-0.0.5/
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     1071 2023-06-24 12:55:12.000000 coreli-0.0.5/LICENSE
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4486 2023-06-24 12:59:51.421962 coreli-0.0.5/PKG-INFO
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3972 2023-06-24 12:55:12.000000 coreli-0.0.5/README.md
+drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-06-24 12:59:51.417962 coreli-0.0.5/coreli/
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4028 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/Collatz_maps.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3294 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/Collatz_tilings.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      202 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/__init__.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)    14584 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/padic_integers.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     9193 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/parity_vectors.py
+drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-06-24 12:59:51.421962 coreli-0.0.5/coreli/tinytiles/
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      119 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/tinytiles/__init__.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     1406 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/tinytiles/interactive.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3503 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/tinytiles/model.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     3327 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/tinytiles/svg_view.py
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     2445 2023-06-24 12:55:12.000000 coreli-0.0.5/coreli/utils.py
+drwxrwxr-x   0 cosmo     (1000) cosmo     (1000)        0 2023-06-24 12:59:51.421962 coreli-0.0.5/coreli.egg-info/
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)     4486 2023-06-24 12:59:51.000000 coreli-0.0.5/coreli.egg-info/PKG-INFO
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      425 2023-06-24 12:59:51.000000 coreli-0.0.5/coreli.egg-info/SOURCES.txt
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)        1 2023-06-24 12:59:51.000000 coreli-0.0.5/coreli.egg-info/dependency_links.txt
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)       47 2023-06-24 12:59:51.000000 coreli-0.0.5/coreli.egg-info/requires.txt
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)        7 2023-06-24 12:59:51.000000 coreli-0.0.5/coreli.egg-info/top_level.txt
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)       38 2023-06-24 12:59:51.421962 coreli-0.0.5/setup.cfg
+-rw-rw-r--   0 cosmo     (1000) cosmo     (1000)      846 2023-06-24 12:56:15.000000 coreli-0.0.5/setup.py
```

### Comparing `coreli-0.0.4/LICENSE` & `coreli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `coreli-0.0.4/PKG-INFO` & `coreli-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coreli
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Collatz Research Library provides tools for experimenting and testing hypothesises related to the Collatz Process.
 Home-page: https://github.com/tcosmo/coreli
 Author: Tristan Stérin
 Author-email: tristan.sterin@mu.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `coreli-0.0.4/README.md` & `coreli-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `coreli-0.0.4/coreli/Collatz_maps.py` & `coreli-0.0.5/coreli/Collatz_maps.py`

 * *Files identical despite different names*

### Comparing `coreli-0.0.4/coreli/Collatz_tilings.py` & `coreli-0.0.5/coreli/Collatz_tilings.py`

 * *Files identical despite different names*

### Comparing `coreli-0.0.4/coreli/padic_integers.py` & `coreli-0.0.5/coreli/padic_integers.py`

 * *Files identical despite different names*

### Comparing `coreli-0.0.4/coreli/parity_vectors.py` & `coreli-0.0.5/coreli/parity_vectors.py`

 * *Files identical despite different names*

### Comparing `coreli-0.0.4/coreli/tinytiles/interactive.py` & `coreli-0.0.5/coreli/tinytiles/interactive.py`

 * *Files identical despite different names*

### Comparing `coreli-0.0.4/coreli/tinytiles/model.py` & `coreli-0.0.5/coreli/tinytiles/model.py`

 * *Files identical despite different names*

### Comparing `coreli-0.0.4/coreli/tinytiles/svg_view.py` & `coreli-0.0.5/coreli/tinytiles/svg_view.py`

 * *Files identical despite different names*

### Comparing `coreli-0.0.4/coreli/utils.py` & `coreli-0.0.5/coreli/utils.py`

 * *Files identical despite different names*

### Comparing `coreli-0.0.4/coreli.egg-info/PKG-INFO` & `coreli-0.0.5/coreli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coreli
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Collatz Research Library provides tools for experimenting and testing hypothesises related to the Collatz Process.
 Home-page: https://github.com/tcosmo/coreli
 Author: Tristan Stérin
 Author-email: tristan.sterin@mu.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

