# Comparing `tmp/bhv-0.6.0b0.tar.gz` & `tmp/bhv-0.6.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.6.0b0.tar", last modified: Sat Jun 24 10:11:05 2023, max compression
+gzip compressed data, was "bhv-0.6.0rc0.tar", last modified: Sat Jun 24 10:50:01 2023, max compression
```

## Comparing `bhv-0.6.0b0.tar` & `bhv-0.6.0rc0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:11:05.385984 bhv-0.6.0b0/
--rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.6.0b0/LICENSE
--rw-r--r--   0 adam      (1000) adam      (1000)     1092 2023-06-24 10:11:05.385984 bhv-0.6.0b0/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.6.0b0/README.md
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:11:05.384984 bhv-0.6.0b0/bhv/
--rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.6.0b0/bhv/__init__.py
--rw-r--r--   0 adam      (1000) adam      (1000)    16739 2023-06-24 07:40:55.000000 bhv-0.6.0b0/bhv/abstract.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:11:05.384984 bhv-0.6.0b0/bhv/cnative/
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:11:05.385984 bhv-0.6.0b0/bhv/cnative/TurboSHAKEref/
--rw-r--r--   0 adam      (1000) adam      (1000)    11896 2023-06-11 12:27:27.000000 bhv-0.6.0b0/bhv/cnative/TurboSHAKEref/KeccakP-1600-reference.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)     2537 2023-06-11 12:27:27.000000 bhv-0.6.0b0/bhv/cnative/TurboSHAKEref/KeccakSponge.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)     2381 2023-06-11 12:27:27.000000 bhv-0.6.0b0/bhv/cnative/TurboSHAKEref/TurboSHAKE.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)    11558 2023-06-24 09:31:02.000000 bhv-0.6.0b0/bhv/cnative/bindings.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-06-24 07:34:04.000000 bhv-0.6.0b0/bhv/embedding.py
--rw-r--r--   0 adam      (1000) adam      (1000)     4208 2023-06-24 07:40:55.000000 bhv-0.6.0b0/bhv/lookup.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1897 2023-06-24 07:40:55.000000 bhv-0.6.0b0/bhv/native.py
--rw-r--r--   0 adam      (1000) adam      (1000)    12443 2023-06-24 07:40:55.000000 bhv-0.6.0b0/bhv/np.py
--rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.6.0b0/bhv/poibin.py
--rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.6.0b0/bhv/pytorch.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-06-16 16:14:43.000000 bhv-0.6.0b0/bhv/shared.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.6.0b0/bhv/slice.py
--rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.6.0b0/bhv/symbolic.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.6.0b0/bhv/unification.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3575 2023-06-18 07:52:14.000000 bhv-0.6.0b0/bhv/vanilla.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1372 2023-06-24 07:40:55.000000 bhv-0.6.0b0/bhv/visualization.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:11:05.384984 bhv-0.6.0b0/bhv.egg-info/
--rw-r--r--   0 adam      (1000) adam      (1000)     1092 2023-06-24 10:11:05.000000 bhv-0.6.0b0/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)      536 2023-06-24 10:11:05.000000 bhv-0.6.0b0/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-24 10:11:05.000000 bhv-0.6.0b0/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       44 2023-06-24 10:11:05.000000 bhv-0.6.0b0/bhv.egg-info/requires.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-24 10:11:05.000000 bhv-0.6.0b0/bhv.egg-info/top_level.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-24 10:11:05.385984 bhv-0.6.0b0/setup.cfg
--rw-r--r--   0 adam      (1000) adam      (1000)     1967 2023-06-24 10:10:33.000000 bhv-0.6.0b0/setup.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:50:01.316209 bhv-0.6.0rc0/
+-rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.6.0rc0/LICENSE
+-rw-r--r--   0 adam      (1000) adam      (1000)     1093 2023-06-24 10:50:01.316209 bhv-0.6.0rc0/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.6.0rc0/README.md
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:50:01.315209 bhv-0.6.0rc0/bhv/
+-rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.6.0rc0/bhv/__init__.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    16739 2023-06-24 07:40:55.000000 bhv-0.6.0rc0/bhv/abstract.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:50:01.315209 bhv-0.6.0rc0/bhv/cnative/
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:50:01.316209 bhv-0.6.0rc0/bhv/cnative/TurboSHAKEref/
+-rw-r--r--   0 adam      (1000) adam      (1000)    11896 2023-06-11 12:27:27.000000 bhv-0.6.0rc0/bhv/cnative/TurboSHAKEref/KeccakP-1600-reference.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     2537 2023-06-11 12:27:27.000000 bhv-0.6.0rc0/bhv/cnative/TurboSHAKEref/KeccakSponge.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     2381 2023-06-11 12:27:27.000000 bhv-0.6.0rc0/bhv/cnative/TurboSHAKEref/TurboSHAKE.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)    11558 2023-06-24 09:31:02.000000 bhv-0.6.0rc0/bhv/cnative/bindings.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-06-24 07:34:04.000000 bhv-0.6.0rc0/bhv/embedding.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     4208 2023-06-24 07:40:55.000000 bhv-0.6.0rc0/bhv/lookup.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1897 2023-06-24 07:40:55.000000 bhv-0.6.0rc0/bhv/native.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    12443 2023-06-24 07:40:55.000000 bhv-0.6.0rc0/bhv/np.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.6.0rc0/bhv/poibin.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.6.0rc0/bhv/pytorch.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-06-16 16:14:43.000000 bhv-0.6.0rc0/bhv/shared.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.6.0rc0/bhv/slice.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.6.0rc0/bhv/symbolic.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.6.0rc0/bhv/unification.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3575 2023-06-18 07:52:14.000000 bhv-0.6.0rc0/bhv/vanilla.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1372 2023-06-24 07:40:55.000000 bhv-0.6.0rc0/bhv/visualization.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:50:01.315209 bhv-0.6.0rc0/bhv.egg-info/
+-rw-r--r--   0 adam      (1000) adam      (1000)     1093 2023-06-24 10:50:01.000000 bhv-0.6.0rc0/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)      536 2023-06-24 10:50:01.000000 bhv-0.6.0rc0/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-24 10:50:01.000000 bhv-0.6.0rc0/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       44 2023-06-24 10:50:01.000000 bhv-0.6.0rc0/bhv.egg-info/requires.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-24 10:50:01.000000 bhv-0.6.0rc0/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-24 10:50:01.316209 bhv-0.6.0rc0/setup.cfg
+-rw-r--r--   0 adam      (1000) adam      (1000)     2001 2023-06-24 10:48:37.000000 bhv-0.6.0rc0/setup.py
```

### Comparing `bhv-0.6.0b0/LICENSE` & `bhv-0.6.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/PKG-INFO` & `bhv-0.6.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.6.0b0
+Version: 0.6.0rc0
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
```

### Comparing `bhv-0.6.0b0/README.md` & `bhv-0.6.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/abstract.py` & `bhv-0.6.0rc0/bhv/abstract.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/cnative/TurboSHAKEref/KeccakP-1600-reference.cpp` & `bhv-0.6.0rc0/bhv/cnative/TurboSHAKEref/KeccakP-1600-reference.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/cnative/TurboSHAKEref/KeccakSponge.cpp` & `bhv-0.6.0rc0/bhv/cnative/TurboSHAKEref/KeccakSponge.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/cnative/TurboSHAKEref/TurboSHAKE.cpp` & `bhv-0.6.0rc0/bhv/cnative/TurboSHAKEref/TurboSHAKE.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/cnative/bindings.cpp` & `bhv-0.6.0rc0/bhv/cnative/bindings.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/embedding.py` & `bhv-0.6.0rc0/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/lookup.py` & `bhv-0.6.0rc0/bhv/lookup.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/native.py` & `bhv-0.6.0rc0/bhv/native.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/np.py` & `bhv-0.6.0rc0/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/poibin.py` & `bhv-0.6.0rc0/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/pytorch.py` & `bhv-0.6.0rc0/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/shared.py` & `bhv-0.6.0rc0/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/slice.py` & `bhv-0.6.0rc0/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/symbolic.py` & `bhv-0.6.0rc0/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/unification.py` & `bhv-0.6.0rc0/bhv/unification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/vanilla.py` & `bhv-0.6.0rc0/bhv/vanilla.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv/visualization.py` & `bhv-0.6.0rc0/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/bhv.egg-info/PKG-INFO` & `bhv-0.6.0rc0/bhv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.6.0b0
+Version: 0.6.0rc0
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
```

### Comparing `bhv-0.6.0b0/bhv.egg-info/SOURCES.txt` & `bhv-0.6.0rc0/bhv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.6.0b0/setup.py` & `bhv-0.6.0rc0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages, Extension
 
-VERSION = '0.6.0b'
+VERSION = '0.6.0c'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 native = Extension("bhv.cnative",
                    sources=['bhv/cnative/bindings.cpp',
-                            'bhv/cnative/TurboSHAKEref/TurboSHAKE.cpp',
-                            'bhv/cnative/TurboSHAKEref/KeccakSponge.cpp',
-                            'bhv/cnative/TurboSHAKEref/KeccakP-1600-reference.cpp',
+                            # 'bhv/cnative/TurboSHAKEref/TurboSHAKE.cpp',
+                            # 'bhv/cnative/TurboSHAKEref/KeccakSponge.cpp',
+                            # 'bhv/cnative/TurboSHAKEref/KeccakP-1600-reference.cpp',
                             ],
-                   include_dirs=['bhv/cnative', 'bhv/cnative/TurboSHAKEref'],
+                   include_dirs=['bhv/cnative', 'bhv/cnative/TurboSHAKEAVX2'],
+                   extra_objects=['bhv/cnative/BHV-TurboSHAKE-AVX2.a'],
                    extra_compile_args=['-std=c++2a', '-O3', '-march=native'],
-                   depends=['brg_endian.h'],
                    language='c++')
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
     author_email="contact@adamv.be",
     description=DESCRIPTION,
```

