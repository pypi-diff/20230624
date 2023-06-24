# Comparing `tmp/mypiprandomdata-0.3.0.tar.gz` & `tmp/mypiprandomdata-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypiprandomdata-0.3.0.tar", last modified: Sat Jun 24 00:06:30 2023, max compression
+gzip compressed data, was "mypiprandomdata-0.4.0.tar", last modified: Sat Jun 24 00:14:11 2023, max compression
```

## Comparing `mypiprandomdata-0.3.0.tar` & `mypiprandomdata-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 00:06:30.404446 mypiprandomdata-0.3.0/
--rw-rw-rw-   0        0        0      250 2023-06-24 00:06:30.402155 mypiprandomdata-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 00:06:30.241788 mypiprandomdata-0.3.0/mypiprandomdata/
--rw-rw-rw-   0        0        0        0 2023-06-23 22:27:10.000000 mypiprandomdata-0.3.0/mypiprandomdata/__init__.py
--rw-rw-rw-   0        0        0     2448 2023-06-23 23:34:28.000000 mypiprandomdata-0.3.0/mypiprandomdata/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-24 00:06:30.288460 mypiprandomdata-0.3.0/mypiprandomdata/data/
--rw-rw-rw-   0        0        0     3817 2023-06-18 04:52:48.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/Cities.txt
--rw-rw-rw-   0        0        0    10204 2023-06-18 04:53:08.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/FirstName.txt
--rw-rw-rw-   0        0        0    12825 2023-06-18 04:53:22.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/LastName.txt
--rw-rw-rw-   0        0        0        0 2023-06-23 23:17:05.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/Real_Address.txt
--rw-rw-rw-   0        0        0      839 2023-06-23 23:05:29.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/States.txt
--rw-rw-rw-   0        0        0    11708 2023-06-18 04:54:13.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/UserAgent.txt
--rw-rw-rw-   0        0        0     8764 2023-06-18 04:53:50.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/ZipCode.txt
--rw-rw-rw-   0        0        0   488475 2023-06-23 23:25:47.000000 mypiprandomdata-0.3.0/mypiprandomdata/data/data.json
-drwxrwxrwx   0        0        0        0 2023-06-24 00:06:30.250764 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/
--rw-rw-rw-   0        0        0      250 2023-06-24 00:06:30.000000 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2023-06-24 00:06:30.000000 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 00:06:30.000000 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-24 00:06:30.000000 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-06-24 00:06:30.000000 mypiprandomdata-0.3.0/mypiprandomdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 00:06:30.404446 mypiprandomdata-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      568 2023-06-24 00:06:09.000000 mypiprandomdata-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 00:14:11.252181 mypiprandomdata-0.4.0/
+-rw-rw-rw-   0        0        0      250 2023-06-24 00:14:11.250156 mypiprandomdata-0.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 00:14:11.079136 mypiprandomdata-0.4.0/mypiprandomdata/
+-rw-rw-rw-   0        0        0        0 2023-06-23 22:27:10.000000 mypiprandomdata-0.4.0/mypiprandomdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 00:14:11.124490 mypiprandomdata-0.4.0/mypiprandomdata/data/
+-rw-rw-rw-   0        0        0     3817 2023-06-18 04:52:48.000000 mypiprandomdata-0.4.0/mypiprandomdata/data/Cities.txt
+-rw-rw-rw-   0        0        0    10204 2023-06-18 04:53:08.000000 mypiprandomdata-0.4.0/mypiprandomdata/data/FirstName.txt
+-rw-rw-rw-   0        0        0    12825 2023-06-18 04:53:22.000000 mypiprandomdata-0.4.0/mypiprandomdata/data/LastName.txt
+-rw-rw-rw-   0        0        0        0 2023-06-23 23:17:05.000000 mypiprandomdata-0.4.0/mypiprandomdata/data/Real_Address.txt
+-rw-rw-rw-   0        0        0      839 2023-06-23 23:05:29.000000 mypiprandomdata-0.4.0/mypiprandomdata/data/States.txt
+-rw-rw-rw-   0        0        0    11708 2023-06-18 04:54:13.000000 mypiprandomdata-0.4.0/mypiprandomdata/data/UserAgent.txt
+-rw-rw-rw-   0        0        0     8764 2023-06-18 04:53:50.000000 mypiprandomdata-0.4.0/mypiprandomdata/data/ZipCode.txt
+-rw-rw-rw-   0        0        0   488475 2023-06-23 23:25:47.000000 mypiprandomdata-0.4.0/mypiprandomdata/data/data.json
+drwxrwxrwx   0        0        0        0 2023-06-24 00:14:11.086117 mypiprandomdata-0.4.0/mypiprandomdata.egg-info/
+-rw-rw-rw-   0        0        0      250 2023-06-24 00:14:10.000000 mypiprandomdata-0.4.0/mypiprandomdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-06-24 00:14:11.000000 mypiprandomdata-0.4.0/mypiprandomdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 00:14:10.000000 mypiprandomdata-0.4.0/mypiprandomdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-24 00:14:10.000000 mypiprandomdata-0.4.0/mypiprandomdata.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-06-24 00:14:10.000000 mypiprandomdata-0.4.0/mypiprandomdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 00:14:11.252181 mypiprandomdata-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-06-24 00:13:59.000000 mypiprandomdata-0.4.0/setup.py
```

### Comparing `mypiprandomdata-0.3.0/mypiprandomdata/data/Cities.txt` & `mypiprandomdata-0.4.0/mypiprandomdata/data/Cities.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.3.0/mypiprandomdata/data/FirstName.txt` & `mypiprandomdata-0.4.0/mypiprandomdata/data/FirstName.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.3.0/mypiprandomdata/data/LastName.txt` & `mypiprandomdata-0.4.0/mypiprandomdata/data/LastName.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.3.0/mypiprandomdata/data/States.txt` & `mypiprandomdata-0.4.0/mypiprandomdata/data/States.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.3.0/mypiprandomdata/data/UserAgent.txt` & `mypiprandomdata-0.4.0/mypiprandomdata/data/UserAgent.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.3.0/mypiprandomdata/data/ZipCode.txt` & `mypiprandomdata-0.4.0/mypiprandomdata/data/ZipCode.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.3.0/mypiprandomdata/data/data.json` & `mypiprandomdata-0.4.0/mypiprandomdata/data/data.json`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.3.0/setup.py` & `mypiprandomdata-0.4.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup
 
 setup(
     name='mypiprandomdata',
-    version='0.3.0',
+    version='0.4.0',
     packages=['mypiprandomdata'],
     package_data={'mypiprandomdata': ['data/*.txt', 'data/*.json']},
     entry_points={
         'console_scripts': [
-            'mypiprandomdata = mypiprandomdata.cli:main'
+            'mypiprandomdata = mypiprandomdata:main'
         ]
     },
+
     install_requires=[],
     author='Inzmamul Haq',
     author_email='spat959@gmail.com',
     description='A package to generate random data.',
     keywords='random data generator',
     url='https://github.com/spat959/mypiprandomdata',
 )
```

