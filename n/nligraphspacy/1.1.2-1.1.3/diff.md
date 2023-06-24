# Comparing `tmp/nligraphspacy-1.1.2.tar.gz` & `tmp/nligraphspacy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nligraphspacy-1.1.2.tar", last modified: Thu Jun 22 13:08:17 2023, max compression
+gzip compressed data, was "nligraphspacy-1.1.3.tar", last modified: Sat Jun 24 08:07:54 2023, max compression
```

## Comparing `nligraphspacy-1.1.2.tar` & `nligraphspacy-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:08:17.278044 nligraphspacy-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 13:08:06.000000 nligraphspacy-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-22 13:08:17.278044 nligraphspacy-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-22 13:08:06.000000 nligraphspacy-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:08:17.278044 nligraphspacy-1.1.2/nligraphspacy/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-22 13:08:06.000000 nligraphspacy-1.1.2/nligraphspacy/NLIGRAPH.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:08:06.000000 nligraphspacy-1.1.2/nligraphspacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:08:17.278044 nligraphspacy-1.1.2/nligraphspacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-22 13:08:17.000000 nligraphspacy-1.1.2/nligraphspacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-22 13:08:17.000000 nligraphspacy-1.1.2/nligraphspacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:08:17.000000 nligraphspacy-1.1.2/nligraphspacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:08:17.000000 nligraphspacy-1.1.2/nligraphspacy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 13:08:17.000000 nligraphspacy-1.1.2/nligraphspacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 13:08:17.000000 nligraphspacy-1.1.2/nligraphspacy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:08:17.282044 nligraphspacy-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-22 13:08:07.000000 nligraphspacy-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:07:54.980027 nligraphspacy-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-24 08:07:41.000000 nligraphspacy-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-24 08:07:54.976027 nligraphspacy-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 08:07:41.000000 nligraphspacy-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:07:54.976027 nligraphspacy-1.1.3/nligraphspacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-24 08:07:41.000000 nligraphspacy-1.1.3/nligraphspacy/NLIGRAPH.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:07:41.000000 nligraphspacy-1.1.3/nligraphspacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:07:54.976027 nligraphspacy-1.1.3/nligraphspacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 08:07:54.980027 nligraphspacy-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-24 08:07:41.000000 nligraphspacy-1.1.3/setup.py
```

### Comparing `nligraphspacy-1.1.2/LICENSE` & `nligraphspacy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nligraphspacy-1.1.2/PKG-INFO` & `nligraphspacy-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nligraphspacy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Knowledge graph using Spacy NLP
 Home-page: https://github.com/Vishnunkumar/nligraphspacy/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacy nli keywords entities
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nligraphspacy-1.1.2/nligraphspacy.egg-info/PKG-INFO` & `nligraphspacy-1.1.3/nligraphspacy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nligraphspacy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Knowledge graph using Spacy NLP
 Home-page: https://github.com/Vishnunkumar/nligraphspacy/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacy nli keywords entities
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nligraphspacy-1.1.2/setup.py` & `nligraphspacy-1.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = [
-  'spacy'
+    'spacy',
+    'en-nligraphspacy'
 ]
 
 setuptools.setup(
     name="nligraphspacy",
-    version="1.1.2",
+    version="1.1.3",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Knowledge graph using Spacy NLP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/nligraphspacy/',
     packages=[
```

