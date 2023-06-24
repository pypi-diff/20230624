# Comparing `tmp/banana_dev-5.0.0.tar.gz` & `tmp/banana_dev-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banana_dev-5.0.0.tar", last modified: Fri Jun 23 20:03:39 2023, max compression
+gzip compressed data, was "banana_dev-5.0.1.tar", last modified: Sat Jun 24 00:17:32 2023, max compression
```

## Comparing `banana_dev-5.0.0.tar` & `banana_dev-5.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-23 20:03:39.643908 banana_dev-5.0.0/
--rw-r--r--   0 erik       (501) staff       (20)     1867 2023-06-23 20:03:39.643964 banana_dev-5.0.0/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     1220 2023-04-25 00:43:43.000000 banana_dev-5.0.0/README.md
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-23 20:03:39.643159 banana_dev-5.0.0/banana_dev/
--rw-r--r--   0 erik       (501) staff       (20)       26 2023-04-25 02:04:09.000000 banana_dev-5.0.0/banana_dev/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     4026 2023-06-23 18:35:30.000000 banana_dev-5.0.0/banana_dev/client.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-23 20:03:39.643817 banana_dev-5.0.0/banana_dev.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     1867 2023-06-23 20:03:39.000000 banana_dev-5.0.0/banana_dev.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)      241 2023-06-23 20:03:39.000000 banana_dev-5.0.0/banana_dev.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2023-06-23 20:03:39.000000 banana_dev-5.0.0/banana_dev.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)       24 2023-06-23 20:03:39.000000 banana_dev-5.0.0/banana_dev.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       11 2023-06-23 20:03:39.000000 banana_dev-5.0.0/banana_dev.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)       79 2023-06-23 20:03:39.644527 banana_dev-5.0.0/setup.cfg
--rw-r--r--   0 erik       (501) staff       (20)     1222 2023-06-23 19:58:15.000000 banana_dev-5.0.0/setup.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-24 00:17:32.754984 banana_dev-5.0.1/
+-rw-r--r--   0 erik       (501) staff       (20)     1867 2023-06-24 00:17:32.755069 banana_dev-5.0.1/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     1220 2023-04-25 00:43:43.000000 banana_dev-5.0.1/README.md
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-24 00:17:32.754062 banana_dev-5.0.1/banana_dev/
+-rw-r--r--   0 erik       (501) staff       (20)       26 2023-06-24 00:11:50.000000 banana_dev-5.0.1/banana_dev/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     4050 2023-06-24 00:14:10.000000 banana_dev-5.0.1/banana_dev/client.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-24 00:17:32.754878 banana_dev-5.0.1/banana_dev.egg-info/
+-rw-r--r--   0 erik       (501) staff       (20)     1867 2023-06-24 00:17:32.000000 banana_dev-5.0.1/banana_dev.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)      241 2023-06-24 00:17:32.000000 banana_dev-5.0.1/banana_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2023-06-24 00:17:32.000000 banana_dev-5.0.1/banana_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (501) staff       (20)       24 2023-06-24 00:17:32.000000 banana_dev-5.0.1/banana_dev.egg-info/requires.txt
+-rw-r--r--   0 erik       (501) staff       (20)       11 2023-06-24 00:17:32.000000 banana_dev-5.0.1/banana_dev.egg-info/top_level.txt
+-rw-r--r--   0 erik       (501) staff       (20)       79 2023-06-24 00:17:32.755311 banana_dev-5.0.1/setup.cfg
+-rw-r--r--   0 erik       (501) staff       (20)     1222 2023-06-24 00:15:02.000000 banana_dev-5.0.1/setup.py
```

### Comparing `banana_dev-5.0.0/PKG-INFO` & `banana_dev-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banana_dev
-Version: 5.0.0
+Version: 5.0.1
 Summary: The banana package is a python client to interact with your machine learning models hosted on Banana
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: MIT
 Keywords: Banana client,API wrapper,Banana,SDK
 Classifier: Development Status :: 4 - Beta
```

### Comparing `banana_dev-5.0.0/README.md` & `banana_dev-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `banana_dev-5.0.0/banana_dev/client.py` & `banana_dev-5.0.1/banana_dev/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             
             if first_call:
                 first_call = False
             else:
                 if self.verbose:
                     print("Retrying...")
             
-            backoff_interval *= 2
+            backoff_interval = min(backoff_interval*2, 3)
             
             res = requests.post(endpoint, json=json, headers=headers)
 
             if self.verbose:
                 if res.status_code != 200:
                     print("Status code:", res.status_code)
                     print(res.text)
```

### Comparing `banana_dev-5.0.0/banana_dev.egg-info/PKG-INFO` & `banana_dev-5.0.1/banana_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banana-dev
-Version: 5.0.0
+Version: 5.0.1
 Summary: The banana package is a python client to interact with your machine learning models hosted on Banana
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: MIT
 Keywords: Banana client,API wrapper,Banana,SDK
 Classifier: Development Status :: 4 - Beta
```

### Comparing `banana_dev-5.0.0/setup.py` & `banana_dev-5.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='banana_dev',
     packages=['banana_dev'],
-    version='5.0.0',
+    version='5.0.1',
     license='MIT',
     # Give a short description about your library
     description='The banana package is a python client to interact with your machine learning models hosted on Banana',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Erik Dunteman',
     author_email='erik@banana.dev',
```

