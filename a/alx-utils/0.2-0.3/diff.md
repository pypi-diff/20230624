# Comparing `tmp/alx-utils-0.2.tar.gz` & `tmp/alx-utils-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alx-utils-0.2.tar", last modified: Sat Jun 24 16:54:30 2023, max compression
+gzip compressed data, was "alx-utils-0.3.tar", last modified: Sat Jun 24 17:05:52 2023, max compression
```

## Comparing `alx-utils-0.2.tar` & `alx-utils-0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 16:54:30.043473 alx-utils-0.2/
--rw-r--r--   0 bio       (1000) bio       (1000)       32 2023-06-24 16:49:04.000000 alx-utils-0.2/MANIFEST.in
--rw-r--r--   0 bio       (1000) bio       (1000)      159 2023-06-24 16:54:30.042473 alx-utils-0.2/PKG-INFO
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 16:54:30.037473 alx-utils-0.2/alx_utils.egg-info/
--rw-r--r--   0 bio       (1000) bio       (1000)      159 2023-06-24 16:54:29.000000 alx-utils-0.2/alx_utils.egg-info/PKG-INFO
--rw-r--r--   0 bio       (1000) bio       (1000)      398 2023-06-24 16:54:29.000000 alx-utils-0.2/alx_utils.egg-info/SOURCES.txt
--rw-r--r--   0 bio       (1000) bio       (1000)        1 2023-06-24 16:54:29.000000 alx-utils-0.2/alx_utils.egg-info/dependency_links.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       49 2023-06-24 16:54:29.000000 alx-utils-0.2/alx_utils.egg-info/entry_points.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       15 2023-06-24 16:54:29.000000 alx-utils-0.2/alx_utils.egg-info/requires.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       10 2023-06-24 16:54:29.000000 alx-utils-0.2/alx_utils.egg-info/top_level.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       38 2023-06-24 16:54:30.043473 alx-utils-0.2/setup.cfg
--rw-r--r--   0 bio       (1000) bio       (1000)      459 2023-06-24 16:54:11.000000 alx-utils-0.2/setup.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 16:54:30.038473 alx-utils-0.2/src/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:08:14.000000 alx-utils-0.2/src/__init__.py
--rw-r--r--   0 bio       (1000) bio       (1000)      527 2023-06-24 14:46:49.000000 alx-utils-0.2/src/alx_utils.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 16:54:30.039473 alx-utils-0.2/tools/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 20:10:13.000000 alx-utils-0.2/tools/__init__.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 16:54:30.041473 alx-utils-0.2/tools/checker/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-24 09:57:35.000000 alx-utils-0.2/tools/checker/__init__.py
--rw-r--r--   0 bio       (1000) bio       (1000)      552 2023-06-24 12:56:55.000000 alx-utils-0.2/tools/checker/main.py
--rwxr--r--   0 bio       (1000) bio       (1000)     6586 2023-06-24 13:33:08.000000 alx-utils-0.2/tools/checker/test.bash
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 16:54:30.042473 alx-utils-0.2/tools/init_task/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:13:03.000000 alx-utils-0.2/tools/init_task/__init__.py
--rwxr--r--   0 bio       (1000) bio       (1000)     4184 2023-06-24 14:51:42.000000 alx-utils-0.2/tools/init_task/scraper.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.400800 alx-utils-0.3/
+-rw-r--r--   0 bio       (1000) bio       (1000)       32 2023-06-24 16:49:04.000000 alx-utils-0.3/MANIFEST.in
+-rw-r--r--   0 bio       (1000) bio       (1000)      159 2023-06-24 17:05:52.400800 alx-utils-0.3/PKG-INFO
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.397800 alx-utils-0.3/alx_utils.egg-info/
+-rw-r--r--   0 bio       (1000) bio       (1000)      159 2023-06-24 17:05:51.000000 alx-utils-0.3/alx_utils.egg-info/PKG-INFO
+-rw-r--r--   0 bio       (1000) bio       (1000)      398 2023-06-24 17:05:52.000000 alx-utils-0.3/alx_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)        1 2023-06-24 17:05:51.000000 alx-utils-0.3/alx_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       49 2023-06-24 17:05:51.000000 alx-utils-0.3/alx_utils.egg-info/entry_points.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       15 2023-06-24 17:05:52.000000 alx-utils-0.3/alx_utils.egg-info/requires.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       10 2023-06-24 17:05:52.000000 alx-utils-0.3/alx_utils.egg-info/top_level.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       38 2023-06-24 17:05:52.400800 alx-utils-0.3/setup.cfg
+-rw-r--r--   0 bio       (1000) bio       (1000)      459 2023-06-24 17:05:43.000000 alx-utils-0.3/setup.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.398800 alx-utils-0.3/src/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:08:14.000000 alx-utils-0.3/src/__init__.py
+-rw-r--r--   0 bio       (1000) bio       (1000)      527 2023-06-24 14:46:49.000000 alx-utils-0.3/src/alx_utils.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.398800 alx-utils-0.3/tools/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 20:10:13.000000 alx-utils-0.3/tools/__init__.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.399800 alx-utils-0.3/tools/checker/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-24 09:57:35.000000 alx-utils-0.3/tools/checker/__init__.py
+-rw-r--r--   0 bio       (1000) bio       (1000)      551 2023-06-24 16:59:57.000000 alx-utils-0.3/tools/checker/main.py
+-rwxr--r--   0 bio       (1000) bio       (1000)     6586 2023-06-24 13:33:08.000000 alx-utils-0.3/tools/checker/test.bash
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.399800 alx-utils-0.3/tools/init_task/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:13:03.000000 alx-utils-0.3/tools/init_task/__init__.py
+-rwxr--r--   0 bio       (1000) bio       (1000)     4184 2023-06-24 14:51:42.000000 alx-utils-0.3/tools/init_task/scraper.py
```

### Comparing `alx-utils-0.2/src/alx_utils.py` & `alx-utils-0.3/src/alx_utils.py`

 * *Files identical despite different names*

### Comparing `alx-utils-0.2/tools/checker/main.py` & `alx-utils-0.3/tools/checker/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import shutil
 from pathlib import Path
-from .shell import main as shell_checker
+from .main import main as shell_checker
 
 
 def main(*args):
     # Get the path to the checker directory
     checker_dir = Path(__file__).resolve().parent
     # Get the checker type and arguments
     checker_type = args[0]
```

### Comparing `alx-utils-0.2/tools/checker/test.bash` & `alx-utils-0.3/tools/checker/test.bash`

 * *Files identical despite different names*

### Comparing `alx-utils-0.2/tools/init_task/scraper.py` & `alx-utils-0.3/tools/init_task/scraper.py`

 * *Files identical despite different names*

