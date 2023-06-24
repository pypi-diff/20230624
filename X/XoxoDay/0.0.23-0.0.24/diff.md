# Comparing `tmp/XoxoDay-0.0.23.tar.gz` & `tmp/XoxoDay-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.23.tar", last modified: Fri Jun 23 22:30:46 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.24.tar", last modified: Sat Jun 24 11:28:00 2023, max compression
```

## Comparing `XoxoDay-0.0.23.tar` & `XoxoDay-0.0.24.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 22:30:46.837635 XoxoDay-0.0.23/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.23/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 22:30:46.837524 XoxoDay-0.0.23/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.23/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 22:30:46.834221 XoxoDay-0.0.23/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-23 22:30:39.000000 XoxoDay-0.0.23/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.23/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 22:30:46.835477 XoxoDay-0.0.23/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.23/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      618 2023-06-23 20:29:54.000000 XoxoDay-0.0.23/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      938 2023-06-23 22:30:27.000000 XoxoDay-0.0.23/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.23/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 22:30:46.837216 XoxoDay-0.0.23/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.23/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.23/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.23/XoxoDay/service/placeOrder.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     3003 2023-06-23 22:30:27.000000 XoxoDay-0.0.23/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.23/XoxoDay/service/voucher.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.23/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 22:30:46.834971 XoxoDay-0.0.23/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 22:30:46.000000 XoxoDay-0.0.23/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-06-23 22:30:46.000000 XoxoDay-0.0.23/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-23 22:30:46.000000 XoxoDay-0.0.23/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-23 22:30:46.000000 XoxoDay-0.0.23/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-23 22:30:46.000000 XoxoDay-0.0.23/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-23 22:30:46.837673 XoxoDay-0.0.23/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-23 22:30:27.000000 XoxoDay-0.0.23/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-24 11:28:00.525806 XoxoDay-0.0.24/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.24/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-24 11:28:00.525659 XoxoDay-0.0.24/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.24/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-24 11:28:00.522240 XoxoDay-0.0.24/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-24 11:27:48.000000 XoxoDay-0.0.24/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.24/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-24 11:28:00.523955 XoxoDay-0.0.24/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.24/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      618 2023-06-23 20:29:54.000000 XoxoDay-0.0.24/XoxoDay/helper/sqlite.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      943 2023-06-24 11:26:47.000000 XoxoDay-0.0.24/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        4 2023-06-24 11:27:30.000000 XoxoDay-0.0.24/XoxoDay/helper/xoxo.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.24/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-24 11:28:00.525324 XoxoDay-0.0.24/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.24/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.24/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.24/XoxoDay/service/placeOrder.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     3003 2023-06-23 22:30:27.000000 XoxoDay-0.0.24/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.24/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.24/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-24 11:28:00.523126 XoxoDay-0.0.24/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-24 11:28:00.000000 XoxoDay-0.0.24/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      533 2023-06-24 11:28:00.000000 XoxoDay-0.0.24/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-24 11:28:00.000000 XoxoDay-0.0.24/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-24 11:28:00.000000 XoxoDay-0.0.24/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-24 11:28:00.000000 XoxoDay-0.0.24/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-24 11:28:00.525849 XoxoDay-0.0.24/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-24 11:27:46.000000 XoxoDay-0.0.24/setup.py
```

### Comparing `XoxoDay-0.0.23/LICENSE` & `XoxoDay-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.23/PKG-INFO` & `XoxoDay-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.23
+Version: 0.0.24
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.23/README.md` & `XoxoDay-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.23/XoxoDay/exception.py` & `XoxoDay-0.0.24/XoxoDay/exception.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.23/XoxoDay/helper/sqlite.py` & `XoxoDay-0.0.24/XoxoDay/helper/sqlite.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.23/XoxoDay/helper/token.py` & `XoxoDay-0.0.24/XoxoDay/helper/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 
 from XoxoDay.exception import XoxoDayException
 from XoxoDay.serializer import Serializer
 
-file_path = f'{os.path.dirname(os.path.abspath(__file__))}/xoxo'
+file_path = f'{os.path.dirname(os.path.abspath(__file__))}/xoxo.json'
 
 ROOT_DIR = sys.path[1]
 
 
 def get_token():
     try:
         with open(file_path, "r") as file:
```

### Comparing `XoxoDay-0.0.23/XoxoDay/service/http_service.py` & `XoxoDay-0.0.24/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.23/XoxoDay/service/token_service.py` & `XoxoDay-0.0.24/XoxoDay/service/token_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.23/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.24/XoxoDay/service/xoxoday_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.23/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.24/XoxoDay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.23
+Version: 0.0.24
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.23/setup.py` & `XoxoDay-0.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='XoxoDay',
-    version="0.0.23",
+    version="0.0.24",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='XoxoDay Api Client For Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/XoxoDay.git',
     project_urls={
```

