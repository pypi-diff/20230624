# Comparing `tmp/nligraphspacy-1.1.3.tar.gz` & `tmp/nligraphspacy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nligraphspacy-1.1.3.tar", last modified: Sat Jun 24 08:07:54 2023, max compression
+gzip compressed data, was "nligraphspacy-1.1.4.tar", last modified: Sat Jun 24 14:36:58 2023, max compression
```

## Comparing `nligraphspacy-1.1.3.tar` & `nligraphspacy-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:07:54.980027 nligraphspacy-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-24 08:07:41.000000 nligraphspacy-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-24 08:07:54.976027 nligraphspacy-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 08:07:41.000000 nligraphspacy-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:07:54.976027 nligraphspacy-1.1.3/nligraphspacy/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-24 08:07:41.000000 nligraphspacy-1.1.3/nligraphspacy/NLIGRAPH.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:07:41.000000 nligraphspacy-1.1.3/nligraphspacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:07:54.976027 nligraphspacy-1.1.3/nligraphspacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 08:07:54.000000 nligraphspacy-1.1.3/nligraphspacy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 08:07:54.980027 nligraphspacy-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-24 08:07:41.000000 nligraphspacy-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:36:58.183829 nligraphspacy-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-24 14:36:47.000000 nligraphspacy-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-24 14:36:58.183829 nligraphspacy-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-24 14:36:47.000000 nligraphspacy-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:36:58.183829 nligraphspacy-1.1.4/nligraphspacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-24 14:36:47.000000 nligraphspacy-1.1.4/nligraphspacy/NLIGRAPH.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:36:47.000000 nligraphspacy-1.1.4/nligraphspacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:36:58.183829 nligraphspacy-1.1.4/nligraphspacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-24 14:36:58.000000 nligraphspacy-1.1.4/nligraphspacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-24 14:36:58.000000 nligraphspacy-1.1.4/nligraphspacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:36:58.000000 nligraphspacy-1.1.4/nligraphspacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:36:58.000000 nligraphspacy-1.1.4/nligraphspacy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-24 14:36:58.000000 nligraphspacy-1.1.4/nligraphspacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 14:36:58.000000 nligraphspacy-1.1.4/nligraphspacy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:36:58.183829 nligraphspacy-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-24 14:36:47.000000 nligraphspacy-1.1.4/setup.py
```

### Comparing `nligraphspacy-1.1.3/LICENSE` & `nligraphspacy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nligraphspacy-1.1.3/PKG-INFO` & `nligraphspacy-1.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nligraphspacy
-Version: 1.1.3
+Version: 1.1.4
 Summary: Knowledge graph using Spacy NLP
 Home-page: https://github.com/Vishnunkumar/nligraphspacy/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacy nli keywords entities
 Classifier: Development Status :: 3 - Alpha
@@ -16,7 +16,22 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NLIGraphSpacy
 Knowledge graph using NLP Spacy
+
+## Installation
+
+```python
+pip install nligraphspacy
+```
+
+## Implementation
+
+```python
+from nligraphspacy import NLIGRAPH
+nligraph = NLIGRAPH.RelationEntityExtract("She worked in the city of London")
+nligraph.process_text()
+# ('She', 'worked', 'London')
+```
```

### Comparing `nligraphspacy-1.1.3/nligraphspacy.egg-info/PKG-INFO` & `nligraphspacy-1.1.4/nligraphspacy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nligraphspacy
-Version: 1.1.3
+Version: 1.1.4
 Summary: Knowledge graph using Spacy NLP
 Home-page: https://github.com/Vishnunkumar/nligraphspacy/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacy nli keywords entities
 Classifier: Development Status :: 3 - Alpha
@@ -16,7 +16,22 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NLIGraphSpacy
 Knowledge graph using NLP Spacy
+
+## Installation
+
+```python
+pip install nligraphspacy
+```
+
+## Implementation
+
+```python
+from nligraphspacy import NLIGRAPH
+nligraph = NLIGRAPH.RelationEntityExtract("She worked in the city of London")
+nligraph.process_text()
+# ('She', 'worked', 'London')
+```
```

### Comparing `nligraphspacy-1.1.3/setup.py` & `nligraphspacy-1.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 requirements = [
     'spacy',
     'en-nligraphspacy'
 ]
 
 setuptools.setup(
     name="nligraphspacy",
-    version="1.1.3",
+    version="1.1.4",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Knowledge graph using Spacy NLP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/nligraphspacy/',
     packages=[
```

