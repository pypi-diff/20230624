# Comparing `tmp/mflag-1.6.5.tar.gz` & `tmp/mflag-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mflag-1.6.5.tar", last modified: Sat Jun 24 10:59:50 2023, max compression
+gzip compressed data, was "mflag-1.6.6.tar", last modified: Sat Jun 24 11:02:07 2023, max compression
```

## Comparing `mflag-1.6.5.tar` & `mflag-1.6.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:59:50.198704 mflag-1.6.5/
--rwxrwxrwx   0 root         (0) root         (0)     1071 2023-06-24 10:44:31.000000 mflag-1.6.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-24 10:59:50.198558 mflag-1.6.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2026 2023-06-24 10:44:31.000000 mflag-1.6.5/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:59:50.195871 mflag-1.6.5/mflag/
--rwxrwxrwx   0 root         (0) root         (0)      202 2023-06-24 10:49:16.000000 mflag-1.6.5/mflag/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:59:50.197109 mflag-1.6.5/mflag/src/
--rwxrwxrwx   0 root         (0) root         (0)     4962 2023-06-24 10:44:31.000000 mflag-1.6.5/mflag/src/flag.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:59:50.195038 mflag-1.6.5/mflag/src/rcmng/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:59:50.197534 mflag-1.6.5/mflag/src/rcmng/client/
--rwxrwxrwx   0 root         (0) root         (0)     1631 2023-06-24 10:41:50.000000 mflag-1.6.5/mflag/src/rcmng/client/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      433 2023-06-24 09:19:59.000000 mflag-1.6.5/mflag/src/rcmng/client/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:59:50.197928 mflag-1.6.5/mflag/src/rcmng/server/
--rwxrwxrwx   0 root         (0) root         (0)     6832 2023-06-24 10:42:40.000000 mflag-1.6.5/mflag/src/rcmng/server/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      255 2023-06-24 08:55:53.000000 mflag-1.6.5/mflag/src/rcmng/server/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:59:50.198297 mflag-1.6.5/mflag/src/rcmng/submit/
--rwxrwxrwx   0 root         (0) root         (0)      844 2023-06-24 10:18:10.000000 mflag-1.6.5/mflag/src/rcmng/submit/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      444 2023-06-24 10:33:05.000000 mflag-1.6.5/mflag/src/rcmng/submit/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:59:50.196910 mflag-1.6.5/mflag.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-24 10:59:50.000000 mflag-1.6.5/mflag.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      401 2023-06-24 10:59:50.000000 mflag-1.6.5/mflag.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-24 10:59:50.000000 mflag-1.6.5/mflag.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       47 2023-06-24 10:59:50.000000 mflag-1.6.5/mflag.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-06-24 10:59:50.000000 mflag-1.6.5/mflag.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-24 10:59:50.198752 mflag-1.6.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      513 2023-06-24 10:59:47.000000 mflag-1.6.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.597144 mflag-1.6.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1071 2023-06-24 10:44:31.000000 mflag-1.6.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-24 11:02:07.597003 mflag-1.6.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2026 2023-06-24 10:44:31.000000 mflag-1.6.6/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.594468 mflag-1.6.6/mflag/
+-rwxrwxrwx   0 root         (0) root         (0)      202 2023-06-24 10:49:16.000000 mflag-1.6.6/mflag/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.595604 mflag-1.6.6/mflag/src/
+-rwxrwxrwx   0 root         (0) root         (0)     4962 2023-06-24 10:44:31.000000 mflag-1.6.6/mflag/src/flag.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.593740 mflag-1.6.6/mflag/src/rcmng/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.596006 mflag-1.6.6/mflag/src/rcmng/client/
+-rwxrwxrwx   0 root         (0) root         (0)     1631 2023-06-24 10:41:50.000000 mflag-1.6.6/mflag/src/rcmng/client/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      433 2023-06-24 09:19:59.000000 mflag-1.6.6/mflag/src/rcmng/client/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.596393 mflag-1.6.6/mflag/src/rcmng/server/
+-rwxrwxrwx   0 root         (0) root         (0)     6832 2023-06-24 10:42:40.000000 mflag-1.6.6/mflag/src/rcmng/server/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      255 2023-06-24 08:55:53.000000 mflag-1.6.6/mflag/src/rcmng/server/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.596762 mflag-1.6.6/mflag/src/rcmng/submit/
+-rwxrwxrwx   0 root         (0) root         (0)      844 2023-06-24 10:18:10.000000 mflag-1.6.6/mflag/src/rcmng/submit/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      444 2023-06-24 10:33:05.000000 mflag-1.6.6/mflag/src/rcmng/submit/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 11:02:07.595414 mflag-1.6.6/mflag.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-24 11:02:07.000000 mflag-1.6.6/mflag.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      401 2023-06-24 11:02:07.000000 mflag-1.6.6/mflag.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-24 11:02:07.000000 mflag-1.6.6/mflag.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       26 2023-06-24 11:02:07.000000 mflag-1.6.6/mflag.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2023-06-24 11:02:07.000000 mflag-1.6.6/mflag.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-24 11:02:07.597189 mflag-1.6.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      483 2023-06-24 11:02:05.000000 mflag-1.6.6/setup.py
```

### Comparing `mflag-1.6.5/LICENSE` & `mflag-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mflag-1.6.5/PKG-INFO` & `mflag-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflag
-Version: 1.6.5
+Version: 1.6.6
 Summary: put/remove flags for files and folders
 Author: Moses Dastmard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mflag: powerful Python toolkit for mark/unmark files and directories 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/mflag/)
```

### Comparing `mflag-1.6.5/README.md` & `mflag-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `mflag-1.6.5/mflag/src/flag.py` & `mflag-1.6.6/mflag/src/flag.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.5/mflag/src/rcmng/client/__init__.py` & `mflag-1.6.6/mflag/src/rcmng/client/__init__.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.5/mflag/src/rcmng/server/__init__.py` & `mflag-1.6.6/mflag/src/rcmng/server/__init__.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.5/mflag/src/rcmng/submit/__init__.py` & `mflag-1.6.6/mflag/src/rcmng/submit/__init__.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.5/mflag.egg-info/PKG-INFO` & `mflag-1.6.6/mflag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflag
-Version: 1.6.5
+Version: 1.6.6
 Summary: put/remove flags for files and folders
 Author: Moses Dastmard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mflag: powerful Python toolkit for mark/unmark files and directories 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/mflag/)
```

