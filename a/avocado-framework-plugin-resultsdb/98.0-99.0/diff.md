# Comparing `tmp/avocado-framework-plugin-resultsdb-98.0.tar.gz` & `tmp/avocado-framework-plugin-resultsdb-99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocado-framework-plugin-resultsdb-98.0.tar", last modified: Thu Jul 14 20:54:05 2022, max compression
+gzip compressed data, was "avocado-framework-plugin-resultsdb-99.0.tar", last modified: Thu Nov 10 19:13:03 2022, max compression
```

## Comparing `avocado-framework-plugin-resultsdb-98.0.tar` & `avocado-framework-plugin-resultsdb-99.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:05.398713 avocado-framework-plugin-resultsdb-98.0/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       16 2019-07-19 21:00:45.000000 avocado-framework-plugin-resultsdb-98.0/MANIFEST.in
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      252 2022-07-14 20:54:05.398713 avocado-framework-plugin-resultsdb-98.0/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        5 2022-07-14 20:50:57.000000 avocado-framework-plugin-resultsdb-98.0/VERSION
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:05.397713 avocado-framework-plugin-resultsdb-98.0/avocado_framework_plugin_resultsdb.egg-info/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      252 2022-07-14 20:54:05.000000 avocado-framework-plugin-resultsdb-98.0/avocado_framework_plugin_resultsdb.egg-info/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      409 2022-07-14 20:54:05.000000 avocado-framework-plugin-resultsdb-98.0/avocado_framework_plugin_resultsdb.egg-info/SOURCES.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2022-07-14 20:54:05.000000 avocado-framework-plugin-resultsdb-98.0/avocado_framework_plugin_resultsdb.egg-info/dependency_links.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      251 2022-07-14 20:54:05.000000 avocado-framework-plugin-resultsdb-98.0/avocado_framework_plugin_resultsdb.egg-info/entry_points.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       45 2022-07-14 20:54:05.000000 avocado-framework-plugin-resultsdb-98.0/avocado_framework_plugin_resultsdb.egg-info/requires.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       18 2022-07-14 20:54:05.000000 avocado-framework-plugin-resultsdb-98.0/avocado_framework_plugin_resultsdb.egg-info/top_level.txt
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:05.397713 avocado-framework-plugin-resultsdb-98.0/avocado_resultsdb/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     6372 2022-07-11 13:32:25.000000 avocado-framework-plugin-resultsdb-98.0/avocado_resultsdb/resultsdb.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       38 2022-07-14 20:54:05.398713 avocado-framework-plugin-resultsdb-98.0/setup.cfg
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1683 2022-07-11 13:32:25.000000 avocado-framework-plugin-resultsdb-98.0/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:03.788231 avocado-framework-plugin-resultsdb-99.0/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       16 2019-07-19 21:00:45.000000 avocado-framework-plugin-resultsdb-99.0/MANIFEST.in
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      252 2022-11-10 19:13:03.788231 avocado-framework-plugin-resultsdb-99.0/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        5 2022-11-10 19:09:51.000000 avocado-framework-plugin-resultsdb-99.0/VERSION
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:03.788231 avocado-framework-plugin-resultsdb-99.0/avocado_framework_plugin_resultsdb.egg-info/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      252 2022-11-10 19:13:03.000000 avocado-framework-plugin-resultsdb-99.0/avocado_framework_plugin_resultsdb.egg-info/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      409 2022-11-10 19:13:03.000000 avocado-framework-plugin-resultsdb-99.0/avocado_framework_plugin_resultsdb.egg-info/SOURCES.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2022-11-10 19:13:03.000000 avocado-framework-plugin-resultsdb-99.0/avocado_framework_plugin_resultsdb.egg-info/dependency_links.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      251 2022-11-10 19:13:03.000000 avocado-framework-plugin-resultsdb-99.0/avocado_framework_plugin_resultsdb.egg-info/entry_points.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       45 2022-11-10 19:13:03.000000 avocado-framework-plugin-resultsdb-99.0/avocado_framework_plugin_resultsdb.egg-info/requires.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       18 2022-11-10 19:13:03.000000 avocado-framework-plugin-resultsdb-99.0/avocado_framework_plugin_resultsdb.egg-info/top_level.txt
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:13:03.788231 avocado-framework-plugin-resultsdb-99.0/avocado_resultsdb/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     6372 2022-11-04 17:27:10.000000 avocado-framework-plugin-resultsdb-99.0/avocado_resultsdb/resultsdb.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       38 2022-11-10 19:13:03.788231 avocado-framework-plugin-resultsdb-99.0/setup.cfg
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1683 2022-11-04 17:27:10.000000 avocado-framework-plugin-resultsdb-99.0/setup.py
```

### Comparing `avocado-framework-plugin-resultsdb-98.0/avocado_resultsdb/resultsdb.py` & `avocado-framework-plugin-resultsdb-99.0/avocado_resultsdb/resultsdb.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-resultsdb-98.0/setup.py` & `avocado-framework-plugin-resultsdb-99.0/setup.py`

 * *Files identical despite different names*

