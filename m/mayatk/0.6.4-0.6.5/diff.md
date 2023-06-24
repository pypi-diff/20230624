# Comparing `tmp/mayatk-0.6.4.tar.gz` & `tmp/mayatk-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayatk-0.6.4.tar", last modified: Sat Jun 24 02:29:23 2023, max compression
+gzip compressed data, was "mayatk-0.6.5.tar", last modified: Sat Jun 24 02:37:21 2023, max compression
```

## Comparing `mayatk-0.6.4.tar` & `mayatk-0.6.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 02:29:23.143570 mayatk-0.6.4/
--rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.6.4/LICENSE
--rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.6.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1246 2023-06-24 02:29:23.143570 mayatk-0.6.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 02:29:23.116395 mayatk-0.6.4/mayatk/
--rw-rw-rw-   0        0        0     5784 2023-06-24 02:29:19.000000 mayatk-0.6.4/mayatk/__init__.py
--rw-rw-rw-   0        0        0     8075 2023-06-05 16:23:13.000000 mayatk-0.6.4/mayatk/cam_utils.py
--rw-rw-rw-   0        0        0     8083 2023-05-30 18:39:58.000000 mayatk-0.6.4/mayatk/cam_utils.py.bak
--rw-rw-rw-   0        0        0    65402 2023-06-14 17:05:48.000000 mayatk-0.6.4/mayatk/cmpt_utils.py
--rw-rw-rw-   0        0        0    48216 2023-05-30 18:39:58.000000 mayatk-0.6.4/mayatk/cmpt_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-24 02:29:23.130409 mayatk-0.6.4/mayatk/display_utils/
--rw-rw-rw-   0        0        0      428 2023-04-16 16:33:47.000000 mayatk-0.6.4/mayatk/display_utils/__init__.py
--rw-rw-rw-   0        0        0     7433 2023-06-13 02:25:19.000000 mayatk-0.6.4/mayatk/display_utils/exploded_view.py
--rw-rw-rw-   0        0        0    30588 2023-06-23 22:00:50.000000 mayatk-0.6.4/mayatk/edit_utils.py
--rw-rw-rw-   0        0        0    22313 2023-05-28 17:20:26.000000 mayatk-0.6.4/mayatk/macro_utils.py
--rw-rw-rw-   0        0        0    13411 2023-06-05 16:23:13.000000 mayatk-0.6.4/mayatk/mash_utils.py
--rw-rw-rw-   0        0        0    13413 2023-05-29 19:59:22.000000 mayatk-0.6.4/mayatk/mash_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-24 02:29:23.134420 mayatk-0.6.4/mayatk/mat_utils/
--rw-rw-rw-   0        0        0      367 2023-04-16 16:33:48.000000 mayatk-0.6.4/mayatk/mat_utils/__init__.py
--rw-rw-rw-   0        0        0     9122 2023-06-12 14:32:54.000000 mayatk-0.6.4/mayatk/mat_utils/mat_utils.py
--rw-rw-rw-   0        0        0    19177 2023-06-20 19:06:12.000000 mayatk-0.6.4/mayatk/mat_utils/stingray_arnold_shader.py
--rw-rw-rw-   0        0        0    15178 2023-06-23 15:06:20.000000 mayatk-0.6.4/mayatk/misc_utils.py
--rw-rw-rw-   0        0        0    15374 2023-06-17 12:29:07.000000 mayatk-0.6.4/mayatk/misc_utils.py.bak
--rw-rw-rw-   0        0        0    29580 2023-06-22 00:27:45.000000 mayatk-0.6.4/mayatk/node_utils.py
--rw-rw-rw-   0        0        0    13413 2023-06-16 01:20:55.000000 mayatk-0.6.4/mayatk/project_utils.py
--rw-rw-rw-   0        0        0    11613 2023-05-20 16:09:43.000000 mayatk-0.6.4/mayatk/project_utils.py.bak
--rw-rw-rw-   0        0        0    20346 2023-06-06 18:19:16.000000 mayatk-0.6.4/mayatk/rig_utils.py
--rw-rw-rw-   0        0        0    20342 2023-05-30 18:34:56.000000 mayatk-0.6.4/mayatk/rig_utils.py.bak
--rw-rw-rw-   0        0        0     2771 2023-05-20 16:34:41.000000 mayatk-0.6.4/mayatk/script_utils.py
--rw-rw-rw-   0        0        0    32313 2023-06-06 18:19:16.000000 mayatk-0.6.4/mayatk/xform_utils.py
--rw-rw-rw-   0        0        0    32309 2023-06-05 16:23:13.000000 mayatk-0.6.4/mayatk/xform_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-24 02:29:23.128904 mayatk-0.6.4/mayatk.egg-info/
--rw-rw-rw-   0        0        0     1246 2023-06-24 02:29:22.000000 mayatk-0.6.4/mayatk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1157 2023-05-20 15:52:44.000000 mayatk-0.6.4/mayatk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0     1016 2023-06-24 02:29:23.000000 mayatk-0.6.4/mayatk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      518 2023-03-29 13:02:37.000000 mayatk-0.6.4/mayatk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-06-24 02:29:22.000000 mayatk-0.6.4/mayatk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-24 02:29:22.000000 mayatk-0.6.4/mayatk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 02:29:23.144561 mayatk-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     2238 2023-06-06 18:19:16.000000 mayatk-0.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:29:23.142562 mayatk-0.6.4/test/
--rw-rw-rw-   0        0        0     1289 2023-05-20 14:01:35.000000 mayatk-0.6.4/test/__init__.py
--rw-rw-rw-   0        0        0    26011 2023-06-14 17:56:40.000000 mayatk-0.6.4/test/cmpt_utils_test.py
--rw-rw-rw-   0        0        0     7670 2023-05-20 15:49:30.000000 mayatk-0.6.4/test/edit_utils_test.py
--rw-rw-rw-   0        0        0     4485 2023-06-11 12:52:05.000000 mayatk-0.6.4/test/mat_utils_test.py
--rw-rw-rw-   0        0        0     7863 2023-06-17 12:29:32.000000 mayatk-0.6.4/test/misc_utils_test.py
--rw-rw-rw-   0        0        0     8241 2023-06-14 16:56:33.000000 mayatk-0.6.4/test/node_utils_test.py
--rw-rw-rw-   0        0        0     5080 2023-05-20 16:17:57.000000 mayatk-0.6.4/test/rig_utils_test.py
--rw-rw-rw-   0        0        0     3406 2023-06-14 17:14:08.000000 mayatk-0.6.4/test/run_tests.py
--rw-rw-rw-   0        0        0     7292 2023-05-20 17:08:16.000000 mayatk-0.6.4/test/xform_utils_test.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.909536 mayatk-0.6.5/
+-rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.6.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1246 2023-06-24 02:37:21.909536 mayatk-0.6.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.887192 mayatk-0.6.5/mayatk/
+-rw-rw-rw-   0        0        0     5784 2023-06-24 02:37:18.000000 mayatk-0.6.5/mayatk/__init__.py
+-rw-rw-rw-   0        0        0     8075 2023-06-05 16:23:13.000000 mayatk-0.6.5/mayatk/cam_utils.py
+-rw-rw-rw-   0        0        0     8083 2023-05-30 18:39:58.000000 mayatk-0.6.5/mayatk/cam_utils.py.bak
+-rw-rw-rw-   0        0        0    65402 2023-06-14 17:05:48.000000 mayatk-0.6.5/mayatk/cmpt_utils.py
+-rw-rw-rw-   0        0        0    48216 2023-05-30 18:39:58.000000 mayatk-0.6.5/mayatk/cmpt_utils.py.bak
+drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.896705 mayatk-0.6.5/mayatk/display_utils/
+-rw-rw-rw-   0        0        0      428 2023-04-16 16:33:47.000000 mayatk-0.6.5/mayatk/display_utils/__init__.py
+-rw-rw-rw-   0        0        0     7433 2023-06-13 02:25:19.000000 mayatk-0.6.5/mayatk/display_utils/exploded_view.py
+-rw-rw-rw-   0        0        0    30588 2023-06-23 22:00:50.000000 mayatk-0.6.5/mayatk/edit_utils.py
+-rw-rw-rw-   0        0        0    22313 2023-05-28 17:20:26.000000 mayatk-0.6.5/mayatk/macro_utils.py
+-rw-rw-rw-   0        0        0    13411 2023-06-05 16:23:13.000000 mayatk-0.6.5/mayatk/mash_utils.py
+-rw-rw-rw-   0        0        0    13413 2023-05-29 19:59:22.000000 mayatk-0.6.5/mayatk/mash_utils.py.bak
+drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.898702 mayatk-0.6.5/mayatk/mat_utils/
+-rw-rw-rw-   0        0        0      367 2023-04-16 16:33:48.000000 mayatk-0.6.5/mayatk/mat_utils/__init__.py
+-rw-rw-rw-   0        0        0     9122 2023-06-12 14:32:54.000000 mayatk-0.6.5/mayatk/mat_utils/mat_utils.py
+-rw-rw-rw-   0        0        0    19177 2023-06-20 19:06:12.000000 mayatk-0.6.5/mayatk/mat_utils/stingray_arnold_shader.py
+-rw-rw-rw-   0        0        0    15178 2023-06-23 15:06:20.000000 mayatk-0.6.5/mayatk/misc_utils.py
+-rw-rw-rw-   0        0        0    15374 2023-06-17 12:29:07.000000 mayatk-0.6.5/mayatk/misc_utils.py.bak
+-rw-rw-rw-   0        0        0    29580 2023-06-22 00:27:45.000000 mayatk-0.6.5/mayatk/node_utils.py
+-rw-rw-rw-   0        0        0    13413 2023-06-16 01:20:55.000000 mayatk-0.6.5/mayatk/project_utils.py
+-rw-rw-rw-   0        0        0    11613 2023-05-20 16:09:43.000000 mayatk-0.6.5/mayatk/project_utils.py.bak
+-rw-rw-rw-   0        0        0    20346 2023-06-06 18:19:16.000000 mayatk-0.6.5/mayatk/rig_utils.py
+-rw-rw-rw-   0        0        0    20342 2023-05-30 18:34:56.000000 mayatk-0.6.5/mayatk/rig_utils.py.bak
+-rw-rw-rw-   0        0        0     2771 2023-05-20 16:34:41.000000 mayatk-0.6.5/mayatk/script_utils.py
+-rw-rw-rw-   0        0        0    32313 2023-06-06 18:19:16.000000 mayatk-0.6.5/mayatk/xform_utils.py
+-rw-rw-rw-   0        0        0    32309 2023-06-05 16:23:13.000000 mayatk-0.6.5/mayatk/xform_utils.py.bak
+drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.894702 mayatk-0.6.5/mayatk.egg-info/
+-rw-rw-rw-   0        0        0     1246 2023-06-24 02:37:21.000000 mayatk-0.6.5/mayatk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2023-05-20 15:52:44.000000 mayatk-0.6.5/mayatk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0     1016 2023-06-24 02:37:21.000000 mayatk-0.6.5/mayatk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      518 2023-03-29 13:02:37.000000 mayatk-0.6.5/mayatk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-06-24 02:37:21.000000 mayatk-0.6.5/mayatk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-24 02:37:21.000000 mayatk-0.6.5/mayatk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 02:37:21.909536 mayatk-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     2238 2023-06-06 18:19:16.000000 mayatk-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:37:21.908531 mayatk-0.6.5/test/
+-rw-rw-rw-   0        0        0     1289 2023-05-20 14:01:35.000000 mayatk-0.6.5/test/__init__.py
+-rw-rw-rw-   0        0        0    26011 2023-06-14 17:56:40.000000 mayatk-0.6.5/test/cmpt_utils_test.py
+-rw-rw-rw-   0        0        0     7670 2023-05-20 15:49:30.000000 mayatk-0.6.5/test/edit_utils_test.py
+-rw-rw-rw-   0        0        0     4485 2023-06-11 12:52:05.000000 mayatk-0.6.5/test/mat_utils_test.py
+-rw-rw-rw-   0        0        0     7863 2023-06-17 12:29:32.000000 mayatk-0.6.5/test/misc_utils_test.py
+-rw-rw-rw-   0        0        0     8241 2023-06-14 16:56:33.000000 mayatk-0.6.5/test/node_utils_test.py
+-rw-rw-rw-   0        0        0     5080 2023-05-20 16:17:57.000000 mayatk-0.6.5/test/rig_utils_test.py
+-rw-rw-rw-   0        0        0     3406 2023-06-14 17:14:08.000000 mayatk-0.6.5/test/run_tests.py
+-rw-rw-rw-   0        0        0     7292 2023-05-20 17:08:16.000000 mayatk-0.6.5/test/xform_utils_test.py
```

### Comparing `mayatk-0.6.4/LICENSE` & `mayatk-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/PKG-INFO` & `mayatk-0.6.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayatk
-Version: 0.6.4
+Version: 0.6.5
 Summary: *mayattk is a collection of backend utilities for Autodesk Maya.*
 Home-page: https://github.com/m3trik/mayatk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mayatk-0.6.4/mayatk/__init__.py` & `mayatk-0.6.5/mayatk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 import inspect
 import importlib
 import pkgutil
 
 
 __package__ = "mayatk"
-__version__ = '0.6.4'
+__version__ = '0.6.5'
 
 
 # Define dictionaries to map class names, method names, class method names, and sub-modules to their respective modules
 CLASS_TO_MODULE = {}
 METHOD_TO_MODULE = {}
 CLASS_METHOD_TO_MODULE = {}
 SUBMODULE_TO_MODULE = {}
```

### Comparing `mayatk-0.6.4/mayatk/cam_utils.py` & `mayatk-0.6.5/mayatk/cam_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/cam_utils.py.bak` & `mayatk-0.6.5/mayatk/cam_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/cmpt_utils.py` & `mayatk-0.6.5/mayatk/cmpt_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/cmpt_utils.py.bak` & `mayatk-0.6.5/mayatk/cmpt_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/display_utils/exploded_view.py` & `mayatk-0.6.5/mayatk/display_utils/exploded_view.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/edit_utils.py` & `mayatk-0.6.5/mayatk/edit_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/macro_utils.py` & `mayatk-0.6.5/mayatk/macro_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/mash_utils.py` & `mayatk-0.6.5/mayatk/mash_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/mash_utils.py.bak` & `mayatk-0.6.5/mayatk/mash_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/mat_utils/mat_utils.py` & `mayatk-0.6.5/mayatk/mat_utils/mat_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/mat_utils/stingray_arnold_shader.py` & `mayatk-0.6.5/mayatk/mat_utils/stingray_arnold_shader.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/misc_utils.py` & `mayatk-0.6.5/mayatk/misc_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/misc_utils.py.bak` & `mayatk-0.6.5/mayatk/misc_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/node_utils.py` & `mayatk-0.6.5/mayatk/node_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/project_utils.py` & `mayatk-0.6.5/mayatk/project_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/project_utils.py.bak` & `mayatk-0.6.5/mayatk/project_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/rig_utils.py` & `mayatk-0.6.5/mayatk/rig_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/rig_utils.py.bak` & `mayatk-0.6.5/mayatk/rig_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/script_utils.py` & `mayatk-0.6.5/mayatk/script_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/xform_utils.py` & `mayatk-0.6.5/mayatk/xform_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk/xform_utils.py.bak` & `mayatk-0.6.5/mayatk/xform_utils.py.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk.egg-info/PKG-INFO` & `mayatk-0.6.5/mayatk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayatk
-Version: 0.6.4
+Version: 0.6.5
 Summary: *mayattk is a collection of backend utilities for Autodesk Maya.*
 Home-page: https://github.com/m3trik/mayatk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mayatk-0.6.4/mayatk.egg-info/PKG-INFO.bak` & `mayatk-0.6.5/mayatk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk.egg-info/SOURCES.txt` & `mayatk-0.6.5/mayatk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/mayatk.egg-info/SOURCES.txt.bak` & `mayatk-0.6.5/mayatk.egg-info/SOURCES.txt.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/setup.py` & `mayatk-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/test/__init__.py` & `mayatk-0.6.5/test/__init__.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/test/cmpt_utils_test.py` & `mayatk-0.6.5/test/cmpt_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/test/edit_utils_test.py` & `mayatk-0.6.5/test/edit_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/test/mat_utils_test.py` & `mayatk-0.6.5/test/mat_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/test/misc_utils_test.py` & `mayatk-0.6.5/test/misc_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/test/node_utils_test.py` & `mayatk-0.6.5/test/node_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/test/rig_utils_test.py` & `mayatk-0.6.5/test/rig_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/test/run_tests.py` & `mayatk-0.6.5/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.4/test/xform_utils_test.py` & `mayatk-0.6.5/test/xform_utils_test.py`

 * *Files identical despite different names*

