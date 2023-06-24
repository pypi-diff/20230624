# Comparing `tmp/atro-pyrsync-0.0.2.tar.gz` & `tmp/atro-pyrsync-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pyrsync-0.0.2.tar", last modified: Sat Jun 24 19:14:39 2023, max compression
+gzip compressed data, was "atro-pyrsync-0.0.3.tar", last modified: Sat Jun 24 19:21:45 2023, max compression
```

## Comparing `atro-pyrsync-0.0.2.tar` & `atro-pyrsync-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:14:39.305836 atro-pyrsync-0.0.2/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-24 19:14:39.305836 atro-pyrsync-0.0.2/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pyrsync-0.0.2/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:14:39.305836 atro-pyrsync-0.0.2/atro_pyrsync.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-24 19:14:39.000000 atro-pyrsync-0.0.2/atro_pyrsync.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      217 2023-06-24 19:14:39.000000 atro-pyrsync-0.0.2/atro_pyrsync.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-24 19:14:39.000000 atro-pyrsync-0.0.2/atro_pyrsync.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)       11 2023-06-24 19:14:39.000000 atro-pyrsync-0.0.2/atro_pyrsync.egg-info/requires.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        8 2023-06-24 19:14:39.000000 atro-pyrsync-0.0.2/atro_pyrsync.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:14:39.305836 atro-pyrsync-0.0.2/pyrsync/
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1266 2023-06-24 19:14:18.000000 atro-pyrsync-0.0.2/pyrsync/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-24 19:14:39.305836 atro-pyrsync-0.0.2/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)      904 2023-06-24 19:14:27.000000 atro-pyrsync-0.0.2/setup.py
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:21:45.977888 atro-pyrsync-0.0.3/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-24 19:21:45.977888 atro-pyrsync-0.0.3/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pyrsync-0.0.3/README.md
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:21:45.974555 atro-pyrsync-0.0.3/atro_pyrsync.egg-info/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      697 2023-06-24 19:21:45.000000 atro-pyrsync-0.0.3/atro_pyrsync.egg-info/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      217 2023-06-24 19:21:45.000000 atro-pyrsync-0.0.3/atro_pyrsync.egg-info/SOURCES.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-24 19:21:45.000000 atro-pyrsync-0.0.3/atro_pyrsync.egg-info/dependency_links.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       11 2023-06-24 19:21:45.000000 atro-pyrsync-0.0.3/atro_pyrsync.egg-info/requires.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        8 2023-06-24 19:21:45.000000 atro-pyrsync-0.0.3/atro_pyrsync.egg-info/top_level.txt
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 19:21:45.974555 atro-pyrsync-0.0.3/pyrsync/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1334 2023-06-24 19:21:20.000000 atro-pyrsync-0.0.3/pyrsync/__init__.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-24 19:21:45.977888 atro-pyrsync-0.0.3/setup.cfg
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      904 2023-06-24 19:21:35.000000 atro-pyrsync-0.0.3/setup.py
```

### Comparing `atro-pyrsync-0.0.2/PKG-INFO` & `atro-pyrsync-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pyrsync
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple rsync.wrapper with atro-pylog logging.
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pyrsync-0.0.2/atro_pyrsync.egg-info/PKG-INFO` & `atro-pyrsync-0.0.3/atro_pyrsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pyrsync
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple rsync.wrapper with atro-pylog logging.
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pyrsync-0.0.2/pyrsync/__init__.py` & `atro-pyrsync-0.0.3/pyrsync/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         log_msg += f" with options {', '.join(options)}"
     exclusion_command = []
     if len(exclusions) > 0:
         if len(exclusions) == 1:
             log_msg += f" excluding {exclusions[0]}"
         else:
             log_msg += f" excluding {', '.join(exclusions)}"
+        exclusions = [f'"{exclusion}"' for exclusion in exclusions]
         exclusion_command = [f"--exclude={{{','.join(exclusions) }}}"]
 
     logger.info(log_msg)
     command_list = ["rsync", *options, *exclusion_command, str(source) + "/", str(destination) + "/"]
     command = " ".join(command_list)
     logger.info("Command ran: '" + command + "'")
```

### Comparing `atro-pyrsync-0.0.2/setup.py` & `atro-pyrsync-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="atro-pyrsync",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     author="Atropos",
     author_email="pypi.rising@atro.xyz",
     description="A simple rsync.wrapper with atro-pylog logging.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atropos/atro-pylog",
```

