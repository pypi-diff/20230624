# Comparing `tmp/alx-utils-0.3.tar.gz` & `tmp/alx-utils-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alx-utils-0.3.tar", last modified: Sat Jun 24 17:05:52 2023, max compression
+gzip compressed data, was "alx-utils-0.4.tar", last modified: Sat Jun 24 18:46:10 2023, max compression
```

## Comparing `alx-utils-0.3.tar` & `alx-utils-0.4.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.400800 alx-utils-0.3/
--rw-r--r--   0 bio       (1000) bio       (1000)       32 2023-06-24 16:49:04.000000 alx-utils-0.3/MANIFEST.in
--rw-r--r--   0 bio       (1000) bio       (1000)      159 2023-06-24 17:05:52.400800 alx-utils-0.3/PKG-INFO
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.397800 alx-utils-0.3/alx_utils.egg-info/
--rw-r--r--   0 bio       (1000) bio       (1000)      159 2023-06-24 17:05:51.000000 alx-utils-0.3/alx_utils.egg-info/PKG-INFO
--rw-r--r--   0 bio       (1000) bio       (1000)      398 2023-06-24 17:05:52.000000 alx-utils-0.3/alx_utils.egg-info/SOURCES.txt
--rw-r--r--   0 bio       (1000) bio       (1000)        1 2023-06-24 17:05:51.000000 alx-utils-0.3/alx_utils.egg-info/dependency_links.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       49 2023-06-24 17:05:51.000000 alx-utils-0.3/alx_utils.egg-info/entry_points.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       15 2023-06-24 17:05:52.000000 alx-utils-0.3/alx_utils.egg-info/requires.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       10 2023-06-24 17:05:52.000000 alx-utils-0.3/alx_utils.egg-info/top_level.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       38 2023-06-24 17:05:52.400800 alx-utils-0.3/setup.cfg
--rw-r--r--   0 bio       (1000) bio       (1000)      459 2023-06-24 17:05:43.000000 alx-utils-0.3/setup.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.398800 alx-utils-0.3/src/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:08:14.000000 alx-utils-0.3/src/__init__.py
--rw-r--r--   0 bio       (1000) bio       (1000)      527 2023-06-24 14:46:49.000000 alx-utils-0.3/src/alx_utils.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.398800 alx-utils-0.3/tools/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 20:10:13.000000 alx-utils-0.3/tools/__init__.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.399800 alx-utils-0.3/tools/checker/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-24 09:57:35.000000 alx-utils-0.3/tools/checker/__init__.py
--rw-r--r--   0 bio       (1000) bio       (1000)      551 2023-06-24 16:59:57.000000 alx-utils-0.3/tools/checker/main.py
--rwxr--r--   0 bio       (1000) bio       (1000)     6586 2023-06-24 13:33:08.000000 alx-utils-0.3/tools/checker/test.bash
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 17:05:52.399800 alx-utils-0.3/tools/init_task/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:13:03.000000 alx-utils-0.3/tools/init_task/__init__.py
--rwxr--r--   0 bio       (1000) bio       (1000)     4184 2023-06-24 14:51:42.000000 alx-utils-0.3/tools/init_task/scraper.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 18:46:10.979948 alx-utils-0.4/
+-rw-r--r--   0 bio       (1000) bio       (1000)      159 2023-06-24 18:46:10.978948 alx-utils-0.4/PKG-INFO
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 18:46:10.976948 alx-utils-0.4/alx_utils.egg-info/
+-rw-r--r--   0 bio       (1000) bio       (1000)      159 2023-06-24 18:46:10.000000 alx-utils-0.4/alx_utils.egg-info/PKG-INFO
+-rw-r--r--   0 bio       (1000) bio       (1000)      363 2023-06-24 18:46:10.000000 alx-utils-0.4/alx_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)        1 2023-06-24 18:46:10.000000 alx-utils-0.4/alx_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       49 2023-06-24 18:46:10.000000 alx-utils-0.4/alx_utils.egg-info/entry_points.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       15 2023-06-24 18:46:10.000000 alx-utils-0.4/alx_utils.egg-info/requires.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       10 2023-06-24 18:46:10.000000 alx-utils-0.4/alx_utils.egg-info/top_level.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       38 2023-06-24 18:46:10.979948 alx-utils-0.4/setup.cfg
+-rw-r--r--   0 bio       (1000) bio       (1000)      459 2023-06-24 18:35:58.000000 alx-utils-0.4/setup.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 18:46:10.977948 alx-utils-0.4/src/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:08:14.000000 alx-utils-0.4/src/__init__.py
+-rw-r--r--   0 bio       (1000) bio       (1000)      534 2023-06-24 18:15:27.000000 alx-utils-0.4/src/alx_utils.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 18:46:10.977948 alx-utils-0.4/tools/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 20:10:13.000000 alx-utils-0.4/tools/__init__.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 18:46:10.978948 alx-utils-0.4/tools/checker/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-24 09:57:35.000000 alx-utils-0.4/tools/checker/__init__.py
+-rw-r--r--   0 bio       (1000) bio       (1000)      577 2023-06-24 18:30:50.000000 alx-utils-0.4/tools/checker/index.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-24 18:46:10.978948 alx-utils-0.4/tools/init_task/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:13:03.000000 alx-utils-0.4/tools/init_task/__init__.py
+-rwxr--r--   0 bio       (1000) bio       (1000)     4184 2023-06-24 14:51:42.000000 alx-utils-0.4/tools/init_task/scraper.py
```

### Comparing `alx-utils-0.3/src/alx_utils.py` & `alx-utils-0.4/src/alx_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 from tools.init_task.scraper import main as init_task, show_help
-from tools.checker.main import main as checker
+from tools.checker.index import shell_main as checker
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-init", nargs="?", const="", help="Run the init-task tool")
     parser.add_argument("-checker", nargs="+", help="Run the checker tool")
     args = parser.parse_args()
```

### Comparing `alx-utils-0.3/tools/checker/main.py` & `alx-utils-0.4/tools/checker/index.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import shutil
+import subprocess
 from pathlib import Path
-from .main import main as shell_checker
 
 
-def main(*args):
+def shell_main(*args):
     # Get the path to the checker directory
     checker_dir = Path(__file__).resolve().parent
     # Get the checker type and arguments
     checker_type = args[0]
     checker_args = args[1:]
 
     # Run the appropriate checker tool with the specified arguments
     if checker_type == "shell":
-        shell_checker("-init")
-        shutil.copy(f"{checker_dir}/test.bash", "test/test.bash")
+        subprocess.run([f"{checker_dir}/test.bash", "-init"], cwd=".")
+        shutil.copy(f"{checker_dir}/test.bash", "./test/test.bash")
     else:
         print(f"Unknown checker type: {checker_type}")
```

### Comparing `alx-utils-0.3/tools/init_task/scraper.py` & `alx-utils-0.4/tools/init_task/scraper.py`

 * *Files identical despite different names*

