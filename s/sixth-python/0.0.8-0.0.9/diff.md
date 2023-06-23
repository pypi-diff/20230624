# Comparing `tmp/sixth-python-0.0.8.tar.gz` & `tmp/sixth-python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-python-0.0.8.tar", last modified: Fri Jun 23 11:51:07 2023, max compression
+gzip compressed data, was "dist/sixth-python-0.0.9.tar", last modified: Fri Jun 23 22:30:16 2023, max compression
```

## Comparing `sixth-python-0.0.8.tar` & `sixth-python-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/
--rw-r--r--   0 mac        (501) staff       (20)     3114 2023-06-23 11:51:07.000000 sixth-python-0.0.8/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.0.8/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-23 11:51:07.000000 sixth-python-0.0.8/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     3773 2023-06-23 11:49:27.000000 sixth-python-0.0.8/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth/
--rw-r--r--   0 mac        (501) staff       (20)       32 2023-06-17 23:23:30.000000 sixth-python-0.0.8/sixth/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.0.8/sixth/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3703 2023-06-19 19:50:08.000000 sixth-python-0.0.8/sixth/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.0.8/sixth/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3924 2023-06-19 19:50:08.000000 sixth-python-0.0.8/sixth/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     5026 2023-06-22 10:58:05.000000 sixth-python-0.0.8/sixth/middlewares/six_rate_limiter_middleware.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth/pen_test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.0.8/sixth/pen_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-python-0.0.8/sixth/pen_test/auto_pen_test.py
--rw-r--r--   0 mac        (501) staff       (20)      850 2023-06-19 15:54:59.000000 sixth-python-0.0.8/sixth/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     4160 2023-06-23 02:36:25.000000 sixth-python-0.0.8/sixth/sdk.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.0.8/sixth/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.0.8/sixth/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.0.8/sixth/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     3114 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      604 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/
+-rw-r--r--   0 mac        (501) staff       (20)     3114 2023-06-23 22:30:16.000000 sixth-python-0.0.9/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.0.9/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-23 22:30:16.000000 sixth-python-0.0.9/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     3773 2023-06-23 22:30:02.000000 sixth-python-0.0.9/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth/
+-rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.0.9/sixth/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.0.9/sixth/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3703 2023-06-19 19:50:08.000000 sixth-python-0.0.9/sixth/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.0.9/sixth/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3924 2023-06-19 19:50:08.000000 sixth-python-0.0.9/sixth/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     5026 2023-06-22 10:58:05.000000 sixth-python-0.0.9/sixth/middlewares/six_rate_limiter_middleware.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth/pen_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.0.9/sixth/pen_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-python-0.0.9/sixth/pen_test/auto_pen_test.py
+-rw-r--r--   0 mac        (501) staff       (20)      850 2023-06-19 15:54:59.000000 sixth-python-0.0.9/sixth/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     4160 2023-06-23 02:36:25.000000 sixth-python-0.0.9/sixth/sdk.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.0.9/sixth/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.0.9/sixth/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.0.9/sixth/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth_python.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3114 2023-06-23 22:30:15.000000 sixth-python-0.0.9/sixth_python.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      604 2023-06-23 22:30:16.000000 sixth-python-0.0.9/sixth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-23 22:30:15.000000 sixth-python-0.0.9/sixth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-23 22:30:15.000000 sixth-python-0.0.9/sixth_python.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-06-23 22:30:15.000000 sixth-python-0.0.9/sixth_python.egg-info/top_level.txt
```

### Comparing `sixth-python-0.0.8/PKG-INFO` & `sixth-python-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Six offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.0.8/README.md` & `sixth-python-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.8/setup.py` & `sixth-python-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Six offical python package'
 LONG_DESCRIPTION = '''
 # **Sixth**
 
 
 [![N|Solid](https://firebasestorage.googleapis.com/v0/b/test-103bf.appspot.com/o/waves.png?alt=media&token=0fa4c489-d9c9-4a3b-9178-593b2b018613)](https://nodesource.com/products/nsolid)
```

### Comparing `sixth-python-0.0.8/sixth/middlewares/encryption_middleware.py` & `sixth-python-0.0.9/sixth/middlewares/encryption_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.8/sixth/middlewares/six_base_http_middleware.py` & `sixth-python-0.0.9/sixth/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.8/sixth/middlewares/six_independent_rate_limiter.py` & `sixth-python-0.0.9/sixth/middlewares/six_independent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.8/sixth/middlewares/six_rate_limiter_middleware.py` & `sixth-python-0.0.9/sixth/middlewares/six_rate_limiter_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.8/sixth/schemas.py` & `sixth-python-0.0.9/sixth/schemas.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.8/sixth/sdk.py` & `sixth-python-0.0.9/sixth/sdk.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.8/sixth/utils/encryption_utils.py` & `sixth-python-0.0.9/sixth/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.8/sixth/utils/time_utils.py` & `sixth-python-0.0.9/sixth/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.8/sixth_python.egg-info/PKG-INFO` & `sixth-python-0.0.9/sixth_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Six offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.0.8/sixth_python.egg-info/SOURCES.txt` & `sixth-python-0.0.9/sixth_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.8/sixth_python.egg-info/requires.txt` & `sixth-python-0.0.9/sixth_python.egg-info/requires.txt`

 * *Files identical despite different names*

