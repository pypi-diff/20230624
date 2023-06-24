# Comparing `tmp/kuut-0.0.1.tar.gz` & `tmp/kuut-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuut-0.0.1.tar", last modified: Thu Jun 22 12:35:10 2023, max compression
+gzip compressed data, was "kuut-0.0.2.tar", last modified: Sat Jun 24 12:17:53 2023, max compression
```

## Comparing `kuut-0.0.1.tar` & `kuut-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-22 12:35:10.930748 kuut-0.0.1/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 kuut-0.0.1/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 kuut-0.0.1/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1090 2023-06-22 12:35:10.930571 kuut-0.0.1/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      293 2023-06-21 20:04:04.000000 kuut-0.0.1/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-22 12:35:10.928854 kuut-0.0.1/kuut/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-22 12:35:06.000000 kuut-0.0.1/kuut/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     3601 2023-06-22 12:35:06.000000 kuut-0.0.1/kuut/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     6283 2023-06-22 12:35:06.000000 kuut-0.0.1/kuut/core.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-22 12:35:10.930221 kuut-0.0.1/kuut.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1090 2023-06-22 12:35:10.000000 kuut-0.0.1/kuut.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      294 2023-06-22 12:35:10.000000 kuut-0.0.1/kuut.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-22 12:35:10.000000 kuut-0.0.1/kuut.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-22 12:35:10.000000 kuut-0.0.1/kuut.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-22 12:35:10.000000 kuut-0.0.1/kuut.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       12 2023-06-22 12:35:10.000000 kuut-0.0.1/kuut.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-22 12:35:10.000000 kuut-0.0.1/kuut.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      985 2023-06-22 12:34:57.000000 kuut-0.0.1/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-22 12:35:10.930802 kuut-0.0.1/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 kuut-0.0.1/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-24 12:17:53.780960 kuut-0.0.2/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 kuut-0.0.2/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 kuut-0.0.2/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     1090 2023-06-24 12:17:53.780828 kuut-0.0.2/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      293 2023-06-21 20:04:04.000000 kuut-0.0.2/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-24 12:17:53.779484 kuut-0.0.2/kuut/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-24 12:17:46.000000 kuut-0.0.2/kuut/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     3601 2023-06-24 12:17:46.000000 kuut-0.0.2/kuut/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     6257 2023-06-24 12:17:46.000000 kuut-0.0.2/kuut/core.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-24 12:17:53.780611 kuut-0.0.2/kuut.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     1090 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      294 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-22 12:35:10.000000 kuut-0.0.2/kuut.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       12 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-06-24 12:17:53.000000 kuut-0.0.2/kuut.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      828 2023-06-24 12:17:46.000000 kuut-0.0.2/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-24 12:17:53.781001 kuut-0.0.2/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 kuut-0.0.2/setup.py
```

### Comparing `kuut-0.0.1/LICENSE` & `kuut-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kuut-0.0.1/PKG-INFO` & `kuut-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuut
-Version: 0.0.1
+Version: 0.0.2
 Summary: taqadum: arabic for progress (tqdm). khutuat: arabic for steps (kuut)
 Home-page: https://github.com/dsm-72/kuut
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kuut-0.0.1/kuut/_modidx.py` & `kuut-0.0.2/kuut/_modidx.py`

 * *Files identical despite different names*

### Comparing `kuut-0.0.1/kuut/core.py` & `kuut-0.0.2/kuut/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,16 +82,15 @@
         instance = super().__new__(cls, *args, **kwargs)
 
         tqdm._instances = cls._instances
         return instance
      
     def __init__(self, steps: List[kstep], *args, **kwargs):
         self.steps = steps        
-        kwargs['total'] = self.pbar_total
-        kwargs['display'] = False
+        kwargs['total'] = self.pbar_total        
         super().__init__(*args, **kwargs)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
```

### Comparing `kuut-0.0.1/kuut.egg-info/PKG-INFO` & `kuut-0.0.2/kuut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuut
-Version: 0.0.1
+Version: 0.0.2
 Summary: taqadum: arabic for progress (tqdm). khutuat: arabic for steps (kuut)
 Home-page: https://github.com/dsm-72/kuut
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kuut-0.0.1/setup.py` & `kuut-0.0.2/setup.py`

 * *Files identical despite different names*

