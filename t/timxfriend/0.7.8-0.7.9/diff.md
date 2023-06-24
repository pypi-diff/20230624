# Comparing `tmp/timxfriend-0.7.8.tar.gz` & `tmp/timxfriend-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timxfriend-0.7.8.tar", last modified: Fri Jan 20 08:40:45 2023, max compression
+gzip compressed data, was "timxfriend-0.7.9.tar", last modified: Sat Jun 24 15:12:48 2023, max compression
```

## Comparing `timxfriend-0.7.8.tar` & `timxfriend-0.7.9.tar`

### file list

```diff
@@ -1,20 +1,12 @@
-drwxr-xr-x   0 tmx        (501) staff       (20)        0 2023-01-20 08:40:45.036982 timxfriend-0.7.8/
--rw-r--r--   0 tmx        (501) staff       (20)     1062 2023-01-18 06:22:32.000000 timxfriend-0.7.8/LICENSE.txt
--rw-r--r--   0 tmx        (501) staff       (20)      724 2023-01-20 08:40:45.037170 timxfriend-0.7.8/PKG-INFO
--rw-r--r--   0 tmx        (501) staff       (20)     6007 2023-01-18 06:01:46.000000 timxfriend-0.7.8/README.md
--rw-r--r--   0 tmx        (501) staff       (20)       79 2023-01-20 08:40:45.037945 timxfriend-0.7.8/setup.cfg
--rw-r--r--   0 tmx        (501) staff       (20)     1698 2023-01-20 08:40:27.000000 timxfriend-0.7.8/setup.py
-drwxr-xr-x   0 tmx        (501) staff       (20)        0 2023-01-20 08:40:45.032820 timxfriend-0.7.8/timxfriend/
--rw-r--r--   0 tmx        (501) staff       (20)    10207 2023-01-18 14:21:35.000000 timxfriend-0.7.8/timxfriend/CA.py
--rw-r--r--   0 tmx        (501) staff       (20)     1027 2023-01-20 08:39:04.000000 timxfriend-0.7.8/timxfriend/PCA.py
--rw-r--r--   0 tmx        (501) staff       (20)       60 2023-01-20 08:17:24.000000 timxfriend-0.7.8/timxfriend/__init__.py
--rw-r--r--   0 tmx        (501) staff       (20)     1322 2023-01-18 07:48:42.000000 timxfriend-0.7.8/timxfriend/plot.py
--rw-r--r--   0 tmx        (501) staff       (20)      975 2023-01-18 07:48:42.000000 timxfriend-0.7.8/timxfriend/svd.py
--rw-r--r--   0 tmx        (501) staff       (20)       28 2023-01-18 07:21:06.000000 timxfriend-0.7.8/timxfriend/test.py
--rw-r--r--   0 tmx        (501) staff       (20)      504 2023-01-18 07:48:42.000000 timxfriend-0.7.8/timxfriend/util.py
-drwxr-xr-x   0 tmx        (501) staff       (20)        0 2023-01-20 08:40:45.036499 timxfriend-0.7.8/timxfriend.egg-info/
--rw-r--r--   0 tmx        (501) staff       (20)      724 2023-01-20 08:40:45.000000 timxfriend-0.7.8/timxfriend.egg-info/PKG-INFO
--rw-r--r--   0 tmx        (501) staff       (20)      342 2023-01-20 08:40:45.000000 timxfriend-0.7.8/timxfriend.egg-info/SOURCES.txt
--rw-r--r--   0 tmx        (501) staff       (20)        1 2023-01-20 08:40:45.000000 timxfriend-0.7.8/timxfriend.egg-info/dependency_links.txt
--rw-r--r--   0 tmx        (501) staff       (20)       26 2023-01-20 08:40:45.000000 timxfriend-0.7.8/timxfriend.egg-info/requires.txt
--rw-r--r--   0 tmx        (501) staff       (20)       11 2023-01-20 08:40:45.000000 timxfriend-0.7.8/timxfriend.egg-info/top_level.txt
+drwxr-xr-x   0 tmx        (501) staff       (20)        0 2023-06-24 15:12:48.218021 timxfriend-0.7.9/
+-rw-r--r--   0 tmx        (501) staff       (20)      737 2023-06-24 15:12:48.218292 timxfriend-0.7.9/PKG-INFO
+-rw-r--r--   0 tmx        (501) staff       (20)       62 2023-01-18 06:22:24.431408 timxfriend-0.7.9/setup.cfg
+-rw-r--r--   0 tmx        (501) staff       (20)     1698 2023-06-24 15:11:48.216437 timxfriend-0.7.9/setup.py
+drwxr-xr-x   0 tmx        (501) staff       (20)        0 2023-06-24 15:12:48.217895 timxfriend-0.7.9/timxfriend/
+-rw-r--r--   0 tmx        (501) staff       (20)    10207 2023-01-18 14:21:35.549159 timxfriend-0.7.9/timxfriend/CA.py
+-rw-r--r--   0 tmx        (501) staff       (20)     1027 2023-01-20 08:39:04.886593 timxfriend-0.7.9/timxfriend/PCA.py
+-rw-r--r--   0 tmx        (501) staff       (20)       60 2023-01-20 08:17:24.962232 timxfriend-0.7.9/timxfriend/__init__.py
+-rw-r--r--   0 tmx        (501) staff       (20)     1322 2023-01-18 07:48:42.730646 timxfriend-0.7.9/timxfriend/plot.py
+-rw-r--r--   0 tmx        (501) staff       (20)      975 2023-01-18 07:48:42.730963 timxfriend-0.7.9/timxfriend/svd.py
+-rw-r--r--   0 tmx        (501) staff       (20)       28 2023-01-18 07:21:06.030005 timxfriend-0.7.9/timxfriend/test.py
+-rw-r--r--   0 tmx        (501) staff       (20)      504 2023-01-18 07:48:42.731309 timxfriend-0.7.9/timxfriend/util.py
```

### Comparing `timxfriend-0.7.8/PKG-INFO` & `timxfriend-0.7.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: timxfriend
-Version: 0.7.8
+Version: 0.7.9
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/user/reponame
-Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: YOUR NAME
 Author-email: your.email@domain.com
 License: MIT
+Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
+Description: UNKNOWN
 Keywords: SOME,MEANINGFULL,KEYWORDS
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-License-File: LICENSE.txt
```

### Comparing `timxfriend-0.7.8/setup.py` & `timxfriend-0.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'timxfriend',         # How you named your package folder (MyLib)
   packages = ['timxfriend'],   # Chose the same as "name"
-  version = '0.7.8',      # Start with a small number and increase it with every change you make
+  version = '0.7.9',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'YOUR NAME',                   # Type in your name
   author_email = 'your.email@domain.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
```

### Comparing `timxfriend-0.7.8/timxfriend/CA.py` & `timxfriend-0.7.9/timxfriend/CA.py`

 * *Files identical despite different names*

### Comparing `timxfriend-0.7.8/timxfriend/PCA.py` & `timxfriend-0.7.9/timxfriend/PCA.py`

 * *Files identical despite different names*

### Comparing `timxfriend-0.7.8/timxfriend/plot.py` & `timxfriend-0.7.9/timxfriend/plot.py`

 * *Files identical despite different names*

### Comparing `timxfriend-0.7.8/timxfriend/svd.py` & `timxfriend-0.7.9/timxfriend/svd.py`

 * *Files identical despite different names*

