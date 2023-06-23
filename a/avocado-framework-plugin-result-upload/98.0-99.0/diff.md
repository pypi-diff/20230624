# Comparing `tmp/avocado-framework-plugin-result-upload-98.0.tar.gz` & `tmp/avocado-framework-plugin-result-upload-99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocado-framework-plugin-result-upload-98.0.tar", last modified: Thu Jul 14 20:54:00 2022, max compression
+gzip compressed data, was "avocado-framework-plugin-result-upload-99.0.tar", last modified: Thu Nov 10 19:12:58 2022, max compression
```

## Comparing `avocado-framework-plugin-result-upload-98.0.tar` & `avocado-framework-plugin-result-upload-99.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:00.272680 avocado-framework-plugin-result-upload-98.0/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       16 2019-07-19 21:00:45.000000 avocado-framework-plugin-result-upload-98.0/MANIFEST.in
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      258 2022-07-14 20:54:00.272680 avocado-framework-plugin-result-upload-98.0/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        5 2022-07-14 20:50:57.000000 avocado-framework-plugin-result-upload-98.0/VERSION
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:00.271680 avocado-framework-plugin-result-upload-98.0/avocado_framework_plugin_result_upload.egg-info/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      258 2022-07-14 20:54:00.000000 avocado-framework-plugin-result-upload-98.0/avocado_framework_plugin_result_upload.egg-info/PKG-INFO
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      441 2022-07-14 20:54:00.000000 avocado-framework-plugin-result-upload-98.0/avocado_framework_plugin_result_upload.egg-info/SOURCES.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)        1 2022-07-14 20:54:00.000000 avocado-framework-plugin-result-upload-98.0/avocado_framework_plugin_result_upload.egg-info/dependency_links.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)      183 2022-07-14 20:54:00.000000 avocado-framework-plugin-result-upload-98.0/avocado_framework_plugin_result_upload.egg-info/entry_points.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       24 2022-07-14 20:54:00.000000 avocado-framework-plugin-result-upload-98.0/avocado_framework_plugin_result_upload.egg-info/requires.txt
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       22 2022-07-14 20:54:00.000000 avocado-framework-plugin-result-upload-98.0/avocado_framework_plugin_result_upload.egg-info/top_level.txt
-drwxrwxr-x   0 cleber    (1000) cleber    (1000)        0 2022-07-14 20:54:00.271680 avocado-framework-plugin-result-upload-98.0/avocado_result_upload/
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     3293 2022-07-11 13:32:25.000000 avocado-framework-plugin-result-upload-98.0/avocado_result_upload/result_upload.py
--rw-rw-r--   0 cleber    (1000) cleber    (1000)       38 2022-07-14 20:54:00.272680 avocado-framework-plugin-result-upload-98.0/setup.cfg
--rw-rw-r--   0 cleber    (1000) cleber    (1000)     1578 2022-07-11 13:32:25.000000 avocado-framework-plugin-result-upload-98.0/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:58.338205 avocado-framework-plugin-result-upload-99.0/
+-rw-rw-r--   0 cleber    (1000) cleber    (1000)       16 2019-07-19 21:00:45.000000 avocado-framework-plugin-result-upload-99.0/MANIFEST.in
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      258 2022-11-10 19:12:58.338205 avocado-framework-plugin-result-upload-99.0/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        5 2022-11-10 19:09:51.000000 avocado-framework-plugin-result-upload-99.0/VERSION
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:58.338205 avocado-framework-plugin-result-upload-99.0/avocado_framework_plugin_result_upload.egg-info/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      258 2022-11-10 19:12:58.000000 avocado-framework-plugin-result-upload-99.0/avocado_framework_plugin_result_upload.egg-info/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      441 2022-11-10 19:12:58.000000 avocado-framework-plugin-result-upload-99.0/avocado_framework_plugin_result_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2022-11-10 19:12:58.000000 avocado-framework-plugin-result-upload-99.0/avocado_framework_plugin_result_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      183 2022-11-10 19:12:58.000000 avocado-framework-plugin-result-upload-99.0/avocado_framework_plugin_result_upload.egg-info/entry_points.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       24 2022-11-10 19:12:58.000000 avocado-framework-plugin-result-upload-99.0/avocado_framework_plugin_result_upload.egg-info/requires.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       22 2022-11-10 19:12:58.000000 avocado-framework-plugin-result-upload-99.0/avocado_framework_plugin_result_upload.egg-info/top_level.txt
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2022-11-10 19:12:58.338205 avocado-framework-plugin-result-upload-99.0/avocado_result_upload/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     3293 2022-11-04 17:27:10.000000 avocado-framework-plugin-result-upload-99.0/avocado_result_upload/result_upload.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       38 2022-11-10 19:12:58.338205 avocado-framework-plugin-result-upload-99.0/setup.cfg
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1578 2022-11-04 17:27:10.000000 avocado-framework-plugin-result-upload-99.0/setup.py
```

### Comparing `avocado-framework-plugin-result-upload-98.0/avocado_result_upload/result_upload.py` & `avocado-framework-plugin-result-upload-99.0/avocado_result_upload/result_upload.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-result-upload-98.0/setup.py` & `avocado-framework-plugin-result-upload-99.0/setup.py`

 * *Files identical despite different names*

