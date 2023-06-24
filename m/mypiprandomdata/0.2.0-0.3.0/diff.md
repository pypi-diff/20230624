# Comparing `tmp/mypiprandomdata-0.2.0.tar.gz` & `tmp/mypiprandomdata-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypiprandomdata-0.2.0.tar", last modified: Fri Jun 23 23:58:52 2023, max compression
+gzip compressed data, was "mypiprandomdata-0.3.0.tar", last modified: Sat Jun 24 00:06:30 2023, max compression
```

## Comparing `mypiprandomdata-0.2.0.tar` & `mypiprandomdata-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 23:58:52.223544 mypiprandomdata-0.2.0/
--rw-rw-rw-   0        0        0      250 2023-06-23 23:58:52.221549 mypiprandomdata-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-23 23:58:52.173664 mypiprandomdata-0.2.0/mypiprandomdata/
--rw-rw-rw-   0        0        0        0 2023-06-23 22:27:10.000000 mypiprandomdata-0.2.0/mypiprandomdata/__init__.py
--rw-rw-rw-   0        0        0     2448 2023-06-23 23:34:28.000000 mypiprandomdata-0.2.0/mypiprandomdata/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-23 23:58:52.215585 mypiprandomdata-0.2.0/mypiprandomdata/data/
--rw-rw-rw-   0        0        0     3817 2023-06-18 04:52:48.000000 mypiprandomdata-0.2.0/mypiprandomdata/data/Cities.txt
--rw-rw-rw-   0        0        0    10204 2023-06-18 04:53:08.000000 mypiprandomdata-0.2.0/mypiprandomdata/data/FirstName.txt
--rw-rw-rw-   0        0        0    12825 2023-06-18 04:53:22.000000 mypiprandomdata-0.2.0/mypiprandomdata/data/LastName.txt
--rw-rw-rw-   0        0        0        0 2023-06-23 23:17:05.000000 mypiprandomdata-0.2.0/mypiprandomdata/data/Real_Address.txt
--rw-rw-rw-   0        0        0      839 2023-06-23 23:05:29.000000 mypiprandomdata-0.2.0/mypiprandomdata/data/States.txt
--rw-rw-rw-   0        0        0    11708 2023-06-18 04:54:13.000000 mypiprandomdata-0.2.0/mypiprandomdata/data/UserAgent.txt
--rw-rw-rw-   0        0        0     8764 2023-06-18 04:53:50.000000 mypiprandomdata-0.2.0/mypiprandomdata/data/ZipCode.txt
-drwxrwxrwx   0        0        0        0 2023-06-23 23:58:52.183637 mypiprandomdata-0.2.0/mypiprandomdata.egg-info/
--rw-rw-rw-   0        0        0      250 2023-06-23 23:58:52.000000 mypiprandomdata-0.2.0/mypiprandomdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-06-23 23:58:52.000000 mypiprandomdata-0.2.0/mypiprandomdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 23:58:52.000000 mypiprandomdata-0.2.0/mypiprandomdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-23 23:58:52.000000 mypiprandomdata-0.2.0/mypiprandomdata.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-06-23 23:58:52.000000 mypiprandomdata-0.2.0/mypiprandomdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 23:58:52.223544 mypiprandomdata-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-06-23 23:58:14.000000 mypiprandomdata-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 00:06:30.404446 mypiprandomdata-0.3.0/
+-rw-rw-rw-   0        0        0      250 2023-06-24 00:06:30.402155 mypiprandomdata-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 00:06:30.241788 mypiprandomdata-0.3.0/mypiprandomdata/
+-rw-rw-rw-   0        0        0        0 2023-06-23 22:27:10.000000 mypiprandomdata-0.3.0/mypiprandomdata/__init__.py
+-rw-rw-rw-   0        0        0     2448 2023-06-23 23:34:28.000000 mypiprandomdata-0.3.0/mypiprandomdata/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-24 00:06:30.288460 mypiprandomdata-0.3.0/mypiprandomdata/data/
+-rw-rw-rw-   0        0        0     3817 2023-06-18 04:52:48.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/Cities.txt
+-rw-rw-rw-   0        0        0    10204 2023-06-18 04:53:08.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/FirstName.txt
+-rw-rw-rw-   0        0        0    12825 2023-06-18 04:53:22.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/LastName.txt
+-rw-rw-rw-   0        0        0        0 2023-06-23 23:17:05.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/Real_Address.txt
+-rw-rw-rw-   0        0        0      839 2023-06-23 23:05:29.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/States.txt
+-rw-rw-rw-   0        0        0    11708 2023-06-18 04:54:13.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/UserAgent.txt
+-rw-rw-rw-   0        0        0     8764 2023-06-18 04:53:50.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/ZipCode.txt
+-rw-rw-rw-   0        0        0   488475 2023-06-23 23:25:47.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/data.json
+drwxrwxrwx   0        0        0        0 2023-06-24 00:06:30.250764 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/
+-rw-rw-rw-   0        0        0      250 2023-06-24 00:06:30.000000 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2023-06-24 00:06:30.000000 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 00:06:30.000000 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-24 00:06:30.000000 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-06-24 00:06:30.000000 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 00:06:30.404446 mypiprandomdata-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      568 2023-06-24 00:06:09.000000 mypiprandomdata-0.3.0/setup.py
```

### Comparing `mypiprandomdata-0.2.0/mypiprandomdata/cli.py` & `mypiprandomdata-0.3.0/mypiprandomdata/cli.py`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.2.0/mypiprandomdata/data/Cities.txt` & `mypiprandomdata-0.3.0/mypiprandomdata/data/Cities.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.2.0/mypiprandomdata/data/FirstName.txt` & `mypiprandomdata-0.3.0/mypiprandomdata/data/FirstName.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.2.0/mypiprandomdata/data/LastName.txt` & `mypiprandomdata-0.3.0/mypiprandomdata/data/LastName.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.2.0/mypiprandomdata/data/States.txt` & `mypiprandomdata-0.3.0/mypiprandomdata/data/States.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.2.0/mypiprandomdata/data/UserAgent.txt` & `mypiprandomdata-0.3.0/mypiprandomdata/data/UserAgent.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.2.0/mypiprandomdata/data/ZipCode.txt` & `mypiprandomdata-0.3.0/mypiprandomdata/data/ZipCode.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.2.0/setup.py` & `mypiprandomdata-0.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='mypiprandomdata',
-    version='0.2.0',
+    version='0.3.0',
     packages=['mypiprandomdata'],
-    package_data={'mypiprandomdata': ['data/*.txt']},
+    package_data={'mypiprandomdata': ['data/*.txt', 'data/*.json']},
     entry_points={
         'console_scripts': [
             'mypiprandomdata = mypiprandomdata.cli:main'
         ]
     },
     install_requires=[],
     author='Inzmamul Haq',
```

