# Comparing `tmp/avocado-framework-plugin-varianter-cit-98.0.tar.gz` & `tmp/avocado-framework-plugin-varianter-cit-99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocado-framework-plugin-varianter-cit-98.0.tar", last modified: Thu Jul 14 20:54:15 2022, max compression
+gzip compressed data, was "avocado-framework-plugin-varianter-cit-99.0.tar", last modified: Thu Nov 10 19:13:14 2022, max compression
```

## Comparing `avocado-framework-plugin-varianter-cit-98.0.tar` & `avocado-framework-plugin-varianter-cit-99.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:15.619778 avocado-framework-plugin-varianter-cit-98.0/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       16 2019-07-23 15:43:52.000000 avocado-framework-plugin-varianter-cit-98.0/MANIFEST.in
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      245 2022-07-14 20:54:15.619778 avocado-framework-plugin-varianter-cit-98.0/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        5 2022-07-14 20:50:57.000000 avocado-framework-plugin-varianter-cit-98.0/VERSION
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:15.617778 avocado-framework-plugin-varianter-cit-98.0/avocado_framework_plugin_varianter_cit.egg-info/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      245 2022-07-14 20:54:15.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_framework_plugin_varianter_cit.egg-info/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      617 2022-07-14 20:54:15.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_framework_plugin_varianter_cit.egg-info/SOURCES.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2022-07-14 20:54:15.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_framework_plugin_varianter_cit.egg-info/dependency_links.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      184 2022-07-14 20:54:15.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_framework_plugin_varianter_cit.egg-info/entry_points.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       24 2022-07-14 20:54:15.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_framework_plugin_varianter_cit.egg-info/requires.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       22 2022-07-14 20:54:15.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_framework_plugin_varianter_cit.egg-info/top_level.txt
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:15.619778 avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)    14452 2022-07-11 13:32:25.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/Cit.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7498 2022-07-11 13:32:25.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/CombinationMatrix.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     4150 2022-07-11 13:32:25.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/CombinationRow.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3901 2022-07-11 13:32:25.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/Parser.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     7655 2022-07-11 13:32:25.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/Solver.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     5803 2022-07-11 13:32:25.000000 avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/varianter_cit.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       38 2022-07-14 20:54:15.619778 avocado-framework-plugin-varianter-cit-98.0/setup.cfg
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1687 2022-07-11 13:32:25.000000 avocado-framework-plugin-varianter-cit-98.0/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:14.913283 avocado-framework-plugin-varianter-cit-99.0/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       16 2019-07-23 15:43:52.000000 avocado-framework-plugin-varianter-cit-99.0/MANIFEST.in
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      245 2022-11-10 19:13:14.912283 avocado-framework-plugin-varianter-cit-99.0/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        5 2022-11-10 19:09:51.000000 avocado-framework-plugin-varianter-cit-99.0/VERSION
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:14.912283 avocado-framework-plugin-varianter-cit-99.0/avocado_framework_plugin_varianter_cit.egg-info/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      245 2022-11-10 19:13:14.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_framework_plugin_varianter_cit.egg-info/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      617 2022-11-10 19:13:14.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_framework_plugin_varianter_cit.egg-info/SOURCES.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2022-11-10 19:13:14.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_framework_plugin_varianter_cit.egg-info/dependency_links.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      184 2022-11-10 19:13:14.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_framework_plugin_varianter_cit.egg-info/entry_points.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       24 2022-11-10 19:13:14.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_framework_plugin_varianter_cit.egg-info/requires.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       22 2022-11-10 19:13:14.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_framework_plugin_varianter_cit.egg-info/top_level.txt
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:14.912283 avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)    14452 2022-11-04 17:27:10.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/Cit.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7498 2022-11-04 17:27:10.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/CombinationMatrix.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     4150 2022-11-04 17:27:10.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/CombinationRow.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3901 2022-11-04 17:27:10.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/Parser.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     7655 2022-11-04 17:27:10.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/Solver.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     5803 2022-11-04 17:27:10.000000 avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/varianter_cit.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       38 2022-11-10 19:13:14.913283 avocado-framework-plugin-varianter-cit-99.0/setup.cfg
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1687 2022-11-04 17:27:10.000000 avocado-framework-plugin-varianter-cit-99.0/setup.py
```

### Comparing `avocado-framework-plugin-varianter-cit-98.0/avocado_framework_plugin_varianter_cit.egg-info/SOURCES.txt` & `avocado-framework-plugin-varianter-cit-99.0/avocado_framework_plugin_varianter_cit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/Cit.py` & `avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/Cit.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/CombinationMatrix.py` & `avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/CombinationMatrix.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/CombinationRow.py` & `avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/CombinationRow.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/Parser.py` & `avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/Parser.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/Solver.py` & `avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/Solver.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-varianter-cit-98.0/avocado_varianter_cit/varianter_cit.py` & `avocado-framework-plugin-varianter-cit-99.0/avocado_varianter_cit/varianter_cit.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-varianter-cit-98.0/setup.py` & `avocado-framework-plugin-varianter-cit-99.0/setup.py`

 * *Files identical despite different names*

