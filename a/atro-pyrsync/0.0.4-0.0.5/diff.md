# Comparing `tmp/atro-pyrsync-0.0.4.tar.gz` & `tmp/atro-pyrsync-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pyrsync-0.0.4.tar", last modified: Sat Jun 24 19:26:07 2023, max compression
+gzip compressed data, was "atro-pyrsync-0.0.5.tar", last modified: Sat Jun 24 19:53:45 2023, max compression
```

## Comparing `atro-pyrsync-0.0.4.tar` & `atro-pyrsync-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:26:07.276411 atro-pyrsync-0.0.4/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-24 19:26:07.276411 atro-pyrsync-0.0.4/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pyrsync-0.0.4/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:26:07.276411 atro-pyrsync-0.0.4/atro_pyrsync.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-24 19:26:07.000000 atro-pyrsync-0.0.4/atro_pyrsync.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      217 2023-06-24 19:26:07.000000 atro-pyrsync-0.0.4/atro_pyrsync.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-24 19:26:07.000000 atro-pyrsync-0.0.4/atro_pyrsync.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)       11 2023-06-24 19:26:07.000000 atro-pyrsync-0.0.4/atro_pyrsync.egg-info/requires.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        8 2023-06-24 19:26:07.000000 atro-pyrsync-0.0.4/atro_pyrsync.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:26:07.276411 atro-pyrsync-0.0.4/pyrsync/
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1289 2023-06-24 19:25:53.000000 atro-pyrsync-0.0.4/pyrsync/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-24 19:26:07.276411 atro-pyrsync-0.0.4/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)      904 2023-06-24 19:26:05.000000 atro-pyrsync-0.0.4/setup.py
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:53:45.969360 atro-pyrsync-0.0.5/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-24 19:53:45.966027 atro-pyrsync-0.0.5/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pyrsync-0.0.5/README.md
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:53:45.966027 atro-pyrsync-0.0.5/atro_pyrsync.egg-info/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-24 19:53:45.000000 atro-pyrsync-0.0.5/atro_pyrsync.egg-info/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      236 2023-06-24 19:53:45.000000 atro-pyrsync-0.0.5/atro_pyrsync.egg-info/SOURCES.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-24 19:53:45.000000 atro-pyrsync-0.0.5/atro_pyrsync.egg-info/dependency_links.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       11 2023-06-24 19:53:45.000000 atro-pyrsync-0.0.5/atro_pyrsync.egg-info/requires.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        8 2023-06-24 19:53:45.000000 atro-pyrsync-0.0.5/atro_pyrsync.egg-info/top_level.txt
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:53:45.966027 atro-pyrsync-0.0.5/pyrsync/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1398 2023-06-24 19:53:16.000000 atro-pyrsync-0.0.5/pyrsync/__init__.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       80 2023-06-24 19:43:49.000000 atro-pyrsync-0.0.5/pyrsync/helpers.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-24 19:53:45.969360 atro-pyrsync-0.0.5/setup.cfg
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      904 2023-06-24 19:53:34.000000 atro-pyrsync-0.0.5/setup.py
```

### Comparing `atro-pyrsync-0.0.4/PKG-INFO` & `atro-pyrsync-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pyrsync
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple rsync.wrapper with atro-pylog logging.
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pyrsync-0.0.4/atro_pyrsync.egg-info/PKG-INFO` & `atro-pyrsync-0.0.5/atro_pyrsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pyrsync
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple rsync.wrapper with atro-pylog logging.
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pyrsync-0.0.4/pyrsync/__init__.py` & `atro-pyrsync-0.0.5/pyrsync/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import subprocess
 from pathlib import Path
-
+from pyrsync.helpers import wrap_in_double_quotes
 from pylog import get_logger
 
 
 def rsync(source: Path, destination: Path, options: list[str] = [], exclusions: list[str] = [], cwd=os.getcwd(), logger=get_logger()):
     log_msg = f"Running rsync from {source.as_posix()} to {destination.as_posix()}"
     if len(options) == 1:
         log_msg += f" with option {options[0]}"
@@ -17,17 +17,17 @@
             log_msg += f" excluding {exclusions[0]}"
         else:
             log_msg += f" excluding {', '.join(exclusions)}"
         
         exclusion_command = [f'--exclude="{exclusion}"' for exclusion in exclusions]
 
     logger.info(log_msg)
-    command_list = ["rsync", *options, *exclusion_command, str(source) + "/", str(destination) + "/"]
+    command_list = ["rsync", *options, wrap_in_double_quotes(str(source) + "/"), wrap_in_double_quotes(str(destination) + "/"), *exclusion_command, ]
     command = " ".join(command_list)
     logger.info("Command ran: '" + command + "'")
-
-    output = subprocess.run(command_list, cwd=cwd, shell=False, capture_output=True)
+    print(command)
+    output = subprocess.run(command, cwd=cwd, shell=True, capture_output=True)
     logger.debug("Rsync output: " + output.stdout.decode())
     if output.stderr:
         logger.error("Rsync error: " + output.stderr.decode())
     if output.returncode != 0:
         raise Exception("Rsync failed")
```

### Comparing `atro-pyrsync-0.0.4/setup.py` & `atro-pyrsync-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="atro-pyrsync",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     author="Atropos",
     author_email="pypi.rising@atro.xyz",
     description="A simple rsync.wrapper with atro-pylog logging.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atropos/atro-pylog",
```

