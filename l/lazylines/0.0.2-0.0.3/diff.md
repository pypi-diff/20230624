# Comparing `tmp/lazylines-0.0.2.tar.gz` & `tmp/lazylines-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazylines-0.0.2.tar", last modified: Sat Jun  3 12:31:54 2023, max compression
+gzip compressed data, was "lazylines-0.0.3.tar", last modified: Sat Jun 24 18:17:56 2023, max compression
```

## Comparing `lazylines-0.0.2.tar` & `lazylines-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-03 12:31:54.993568 lazylines-0.0.2/
--rw-r--r--   0 vincent    (501) staff       (20)     1076 2023-06-03 12:12:42.000000 lazylines-0.0.2/LICENSE
--rw-r--r--   0 vincent    (501) staff       (20)     1135 2023-06-03 12:31:54.993307 lazylines-0.0.2/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      620 2023-06-03 12:12:42.000000 lazylines-0.0.2/README.md
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-03 12:31:54.991451 lazylines-0.0.2/lazylines/
--rw-r--r--   0 vincent    (501) staff       (20)     8306 2023-06-03 12:27:05.000000 lazylines-0.0.2/lazylines/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      323 2023-06-03 12:12:42.000000 lazylines-0.0.2/lazylines/functions.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-03 12:31:54.993128 lazylines-0.0.2/lazylines.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)     1135 2023-06-03 12:31:54.000000 lazylines-0.0.2/lazylines.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      235 2023-06-03 12:31:54.000000 lazylines-0.0.2/lazylines.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-06-03 12:31:54.000000 lazylines-0.0.2/lazylines.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)      173 2023-06-03 12:31:54.000000 lazylines-0.0.2/lazylines.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)       10 2023-06-03 12:31:54.000000 lazylines-0.0.2/lazylines.egg-info/top_level.txt
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-06-03 12:31:54.993606 lazylines-0.0.2/setup.cfg
--rw-r--r--   0 vincent    (501) staff       (20)     1178 2023-06-03 12:31:26.000000 lazylines-0.0.2/setup.py
+drwxr-xr-x   0 vincentwarmerdam   (501) staff       (20)        0 2023-06-24 18:17:56.735427 lazylines-0.0.3/
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)     1076 2023-06-03 18:43:46.000000 lazylines-0.0.3/LICENSE
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)     1135 2023-06-24 18:17:56.735275 lazylines-0.0.3/PKG-INFO
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)      620 2023-06-03 18:43:46.000000 lazylines-0.0.3/README.md
+drwxr-xr-x   0 vincentwarmerdam   (501) staff       (20)        0 2023-06-24 18:17:56.734442 lazylines-0.0.3/lazylines/
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)    12548 2023-06-24 18:17:18.000000 lazylines-0.0.3/lazylines/__init__.py
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)     1357 2023-06-24 18:11:04.000000 lazylines-0.0.3/lazylines/functions.py
+drwxr-xr-x   0 vincentwarmerdam   (501) staff       (20)        0 2023-06-24 18:17:56.735110 lazylines-0.0.3/lazylines.egg-info/
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)     1135 2023-06-24 18:17:56.000000 lazylines-0.0.3/lazylines.egg-info/PKG-INFO
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)      235 2023-06-24 18:17:56.000000 lazylines-0.0.3/lazylines.egg-info/SOURCES.txt
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)        1 2023-06-24 18:17:56.000000 lazylines-0.0.3/lazylines.egg-info/dependency_links.txt
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)      180 2023-06-24 18:17:56.000000 lazylines-0.0.3/lazylines.egg-info/requires.txt
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)       10 2023-06-24 18:17:56.000000 lazylines-0.0.3/lazylines.egg-info/top_level.txt
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)       38 2023-06-24 18:17:56.735464 lazylines-0.0.3/setup.cfg
+-rw-r--r--   0 vincentwarmerdam   (501) staff       (20)     1185 2023-06-24 18:17:36.000000 lazylines-0.0.3/setup.py
```

### Comparing `lazylines-0.0.2/LICENSE` & `lazylines-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lazylines-0.0.2/PKG-INFO` & `lazylines-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazylines
-Version: 0.0.2
+Version: 0.0.3
 Author: Vincent D. Warmerdam
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lazylines-0.0.2/README.md` & `lazylines-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lazylines-0.0.2/lazylines.egg-info/PKG-INFO` & `lazylines-0.0.3/lazylines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazylines
-Version: 0.0.2
+Version: 0.0.3
 Author: Vincent D. Warmerdam
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lazylines-0.0.2/setup.py` & `lazylines-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,27 @@
     "interrogate>=1.2.0",
     "isort==5.12.0",
     "autoflake==2.0.1",
 ]
 
 docs_packages = [
     "mkdocs-material",
-    "mkdocstrings",
+    "mkdocstrings-python",
 ]
 
 dev_packages = test_packages + docs_packages
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="lazylines",
-    version="0.0.2",
+    version="0.0.3",
     author="Vincent D. Warmerdam",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(include=["lazylines", "lazylines.*"]),
     install_requires=base_packages,
     extras_require={"dev": dev_packages},
     classifiers=[
```

