# Comparing `tmp/simplePythonModule-0.0.1.tar.gz` & `tmp/simplePythonModule-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplePythonModule-0.0.1.tar", last modified: Sat Jun 24 14:08:09 2023, max compression
+gzip compressed data, was "simplePythonModule-0.0.2.tar", last modified: Sat Jun 24 15:20:18 2023, max compression
```

## Comparing `simplePythonModule-0.0.1.tar` & `simplePythonModule-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 14:08:09.784356 simplePythonModule-0.0.1/
--rw-rw-rw-   0        0        0      538 2023-06-24 14:08:09.783355 simplePythonModule-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-24 14:08:09.784860 simplePythonModule-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-06-24 13:09:57.000000 simplePythonModule-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 14:08:09.772101 simplePythonModule-0.0.1/simplePythonModule/
--rw-rw-rw-   0        0        0       52 2023-06-24 12:36:17.000000 simplePythonModule-0.0.1/simplePythonModule/__init__.py
--rw-rw-rw-   0        0        0       38 2023-06-24 12:36:17.000000 simplePythonModule-0.0.1/simplePythonModule/add.py
-drwxrwxrwx   0        0        0        0 2023-06-24 14:08:09.782355 simplePythonModule-0.0.1/simplePythonModule/extras/
--rw-rw-rw-   0        0        0       58 2023-06-24 12:36:17.000000 simplePythonModule-0.0.1/simplePythonModule/extras/__init__.py
--rw-rw-rw-   0        0        0       35 2023-06-24 12:36:17.000000 simplePythonModule-0.0.1/simplePythonModule/extras/divide.py
--rw-rw-rw-   0        0        0       34 2023-06-24 12:36:17.000000 simplePythonModule-0.0.1/simplePythonModule/extras/multiply.py
--rw-rw-rw-   0        0        0       37 2023-06-24 13:29:35.000000 simplePythonModule-0.0.1/simplePythonModule/subtract.py
-drwxrwxrwx   0        0        0        0 2023-06-24 14:08:09.778351 simplePythonModule-0.0.1/simplePythonModule.egg-info/
--rw-rw-rw-   0        0        0      538 2023-06-24 14:08:09.000000 simplePythonModule-0.0.1/simplePythonModule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-06-24 14:08:09.000000 simplePythonModule-0.0.1/simplePythonModule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 14:08:09.000000 simplePythonModule-0.0.1/simplePythonModule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 14:08:09.000000 simplePythonModule-0.0.1/simplePythonModule.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-24 14:08:09.000000 simplePythonModule-0.0.1/simplePythonModule.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 15:20:18.883598 simplePythonModule-0.0.2/
+-rw-rw-rw-   0        0        0      538 2023-06-24 15:20:18.882577 simplePythonModule-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-24 15:20:18.883598 simplePythonModule-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-06-24 15:19:22.000000 simplePythonModule-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:20:18.870093 simplePythonModule-0.0.2/simplePythonModule/
+-rw-rw-rw-   0        0        0       56 2023-06-24 15:16:58.000000 simplePythonModule-0.0.2/simplePythonModule/__init__.py
+-rw-rw-rw-   0        0        0       38 2023-06-24 12:36:17.000000 simplePythonModule-0.0.2/simplePythonModule/add.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:20:18.880399 simplePythonModule-0.0.2/simplePythonModule/extras/
+-rw-rw-rw-   0        0        0       62 2023-06-24 15:16:58.000000 simplePythonModule-0.0.2/simplePythonModule/extras/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-06-24 12:36:17.000000 simplePythonModule-0.0.2/simplePythonModule/extras/divide.py
+-rw-rw-rw-   0        0        0       34 2023-06-24 12:36:17.000000 simplePythonModule-0.0.2/simplePythonModule/extras/multiply.py
+-rw-rw-rw-   0        0        0       37 2023-06-24 13:29:35.000000 simplePythonModule-0.0.2/simplePythonModule/subtract.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:20:18.877355 simplePythonModule-0.0.2/simplePythonModule.egg-info/
+-rw-rw-rw-   0        0        0      538 2023-06-24 15:20:18.000000 simplePythonModule-0.0.2/simplePythonModule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-06-24 15:20:18.000000 simplePythonModule-0.0.2/simplePythonModule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 15:20:18.000000 simplePythonModule-0.0.2/simplePythonModule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 15:20:18.000000 simplePythonModule-0.0.2/simplePythonModule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-24 15:20:18.000000 simplePythonModule-0.0.2/simplePythonModule.egg-info/top_level.txt
```

### Comparing `simplePythonModule-0.0.1/PKG-INFO` & `simplePythonModule-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplePythonModule
-Version: 0.0.1
+Version: 0.0.2
 Summary: My Python package
 Author: Kel
 Author-email: myemail@email.com
 Keywords: Keyword - python,Keyword - first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplePythonModule-0.0.1/setup.py` & `simplePythonModule-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'My Python package'
 LONG_DESCRIPTION = 'My Python package with a slightly longer description'
 
 # Setting up
 setup(
     # the name must match the folder name 'simplemodule'
     name="simplePythonModule",
```

### Comparing `simplePythonModule-0.0.1/simplePythonModule.egg-info/PKG-INFO` & `simplePythonModule-0.0.2/simplePythonModule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplePythonModule
-Version: 0.0.1
+Version: 0.0.2
 Summary: My Python package
 Author: Kel
 Author-email: myemail@email.com
 Keywords: Keyword - python,Keyword - first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

