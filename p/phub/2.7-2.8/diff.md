# Comparing `tmp/phub-2.7.tar.gz` & `tmp/phub-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phub-2.7.tar", last modified: Fri Jun 23 11:47:30 2023, max compression
+gzip compressed data, was "phub-2.8.tar", last modified: Sat Jun 24 10:07:04 2023, max compression
```

## Comparing `phub-2.7.tar` & `phub-2.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.808628 phub-2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 11:47:20.000000 phub-2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-23 11:47:30.808628 phub-2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-23 11:47:20.000000 phub-2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 11:47:20.000000 phub-2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-23 11:47:30.808628 phub-2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 11:47:20.000000 phub-2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.804628 phub-2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.804628 phub-2.7/src/phub/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-23 11:47:20.000000 phub-2.7/src/phub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-23 11:47:20.000000 phub-2.7/src/phub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-06-23 11:47:20.000000 phub-2.7/src/phub/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-23 11:47:20.000000 phub-2.7/src/phub/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-23 11:47:20.000000 phub-2.7/src/phub/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-23 11:47:20.000000 phub-2.7/src/phub/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-23 11:47:20.000000 phub-2.7/src/phub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.808628 phub-2.7/src/phub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-23 11:47:30.000000 phub-2.7/src/phub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-23 11:47:30.000000 phub-2.7/src/phub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:47:30.000000 phub-2.7/src/phub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 11:47:30.000000 phub-2.7/src/phub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 11:47:30.000000 phub-2.7/src/phub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:07:04.881997 phub-2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-24 10:06:51.000000 phub-2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-24 10:07:04.881997 phub-2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-24 10:06:51.000000 phub-2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-24 10:06:51.000000 phub-2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-24 10:07:04.881997 phub-2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-24 10:06:51.000000 phub-2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:07:04.877997 phub-2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:07:04.877997 phub-2.8/src/phub/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-24 10:06:51.000000 phub-2.8/src/phub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-24 10:06:51.000000 phub-2.8/src/phub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-06-24 10:06:51.000000 phub-2.8/src/phub/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-24 10:06:51.000000 phub-2.8/src/phub/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-24 10:06:51.000000 phub-2.8/src/phub/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-24 10:06:51.000000 phub-2.8/src/phub/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-24 10:06:51.000000 phub-2.8/src/phub/phub_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-24 10:06:51.000000 phub-2.8/src/phub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:07:04.881997 phub-2.8/src/phub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-24 10:07:04.000000 phub-2.8/src/phub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-24 10:07:04.000000 phub-2.8/src/phub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:07:04.000000 phub-2.8/src/phub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-24 10:07:04.000000 phub-2.8/src/phub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 10:07:04.000000 phub-2.8/src/phub.egg-info/top_level.txt
```

### Comparing `phub-2.7/LICENSE` & `phub-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `phub-2.7/PKG-INFO` & `phub-2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.7
+Version: 2.8
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
```

### Comparing `phub-2.7/README.md` & `phub-2.8/README.md`

 * *Files identical despite different names*

### Comparing `phub-2.7/setup.cfg` & `phub-2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phub
-version = 2.7
+version = 2.8
 description = An API for PornHub
 author = Egsagon
 author_email = egsagon12@gmail.com
 url = https://github.com/Egsagon/PHUB/
 license = GPLv3
 license_file = LICENSE
 long_description = file: README.md
```

### Comparing `phub-2.7/src/phub/__init__.py` & `phub-2.8/src/phub/__init__.py`

 * *Files identical despite different names*

### Comparing `phub-2.7/src/phub/classes.py` & `phub-2.8/src/phub/classes.py`

 * *Files identical despite different names*

### Comparing `phub-2.7/src/phub/consts.py` & `phub-2.8/src/phub/consts.py`

 * *Files identical despite different names*

### Comparing `phub-2.7/src/phub/core.py` & `phub-2.8/src/phub/core.py`

 * *Files identical despite different names*

### Comparing `phub-2.7/src/phub/parser.py` & `phub-2.8/src/phub/parser.py`

 * *Files identical despite different names*

### Comparing `phub-2.7/src/phub/utils.py` & `phub-2.8/src/phub/utils.py`

 * *Files identical despite different names*

### Comparing `phub-2.7/src/phub.egg-info/PKG-INFO` & `phub-2.8/src/phub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.7
+Version: 2.8
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
```

