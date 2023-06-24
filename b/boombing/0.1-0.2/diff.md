# Comparing `tmp/boombing-0.1.tar.gz` & `tmp/boombing-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boombing-0.1.tar", last modified: Fri Jun 23 19:12:00 2023, max compression
+gzip compressed data, was "boombing-0.2.tar", last modified: Sat Jun 24 08:03:30 2023, max compression
```

## Comparing `boombing-0.1.tar` & `boombing-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-23 19:12:00.722069 boombing-0.1/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 boombing-0.1/LICENSE
--rw-r--r--   0 themamad  (1000) themamad  (1000)      974 2023-06-23 19:12:00.722069 boombing-0.1/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      248 2023-06-23 19:09:44.000000 boombing-0.1/README.md
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-23 19:12:00.722069 boombing-0.1/boombing.egg-info/
--rw-r--r--   0 themamad  (1000) themamad  (1000)      974 2023-06-23 19:12:00.000000 boombing-0.1/boombing.egg-info/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      154 2023-06-23 19:12:00.000000 boombing-0.1/boombing.egg-info/SOURCES.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-23 19:12:00.000000 boombing-0.1/boombing.egg-info/dependency_links.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-23 19:12:00.000000 boombing-0.1/boombing.egg-info/top_level.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-23 19:12:00.722069 boombing-0.1/setup.cfg
--rw-r--r--   0 themamad  (1000) themamad  (1000)      961 2023-06-23 19:11:32.000000 boombing-0.1/setup.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 08:03:30.090800 boombing-0.2/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 boombing-0.2/LICENSE
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      974 2023-06-24 08:03:30.090800 boombing-0.2/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      248 2023-06-23 19:09:44.000000 boombing-0.2/README.md
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 08:03:30.087467 boombing-0.2/boombing.egg-info/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      974 2023-06-24 08:03:30.000000 boombing-0.2/boombing.egg-info/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      154 2023-06-24 08:03:30.000000 boombing-0.2/boombing.egg-info/SOURCES.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-24 08:03:30.000000 boombing-0.2/boombing.egg-info/dependency_links.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-24 08:03:30.000000 boombing-0.2/boombing.egg-info/top_level.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-24 08:03:30.090800 boombing-0.2/setup.cfg
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      961 2023-06-24 08:02:54.000000 boombing-0.2/setup.py
```

### Comparing `boombing-0.1/LICENSE` & `boombing-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `boombing-0.1/PKG-INFO` & `boombing-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boombing
-Version: 0.1
+Version: 0.2
 Summary: boombing a Library Python
 Home-page: https://github.com/OnlyRad/Boombers
 Author: Mohammad and Amir
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,sms,boombers,boomber
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `boombing-0.1/boombing.egg-info/PKG-INFO` & `boombing-0.2/boombing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boombing
-Version: 0.1
+Version: 0.2
 Summary: boombing a Library Python
 Home-page: https://github.com/OnlyRad/Boombers
 Author: Mohammad and Amir
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,sms,boombers,boomber
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `boombing-0.1/setup.py` & `boombing-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'boombing',
-    version = '0.1',
+    version = '0.2',
     author='Mohammad and Amir',
     author_email = 'mohammadmehrabi175@gmail.com',
     description = 'boombing a Library Python',
     keywords = ['bot' , 'sms' , 'boombers' , 'boomber'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
```

