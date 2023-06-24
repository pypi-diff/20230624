# Comparing `tmp/bhv-0.6.1.tar.gz` & `tmp/bhv-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.6.1.tar", last modified: Sat Jun 24 11:13:42 2023, max compression
+gzip compressed data, was "bhv-0.6.2.tar", last modified: Sat Jun 24 11:24:42 2023, max compression
```

## Comparing `bhv-0.6.1.tar` & `bhv-0.6.2.tar`

### file list

```diff
@@ -1,33 +1,49 @@
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 11:13:42.952196 bhv-0.6.1/
--rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.6.1/LICENSE
--rw-r--r--   0 adam      (1000) adam      (1000)     1090 2023-06-24 11:13:42.951196 bhv-0.6.1/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.6.1/README.md
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 11:13:42.951196 bhv-0.6.1/bhv/
--rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.6.1/bhv/__init__.py
--rw-r--r--   0 adam      (1000) adam      (1000)    16739 2023-06-24 07:40:55.000000 bhv-0.6.1/bhv/abstract.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 11:13:42.951196 bhv-0.6.1/bhv/cnative/
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 11:13:42.951196 bhv-0.6.1/bhv/cnative/TurboSHAKEopt/
--rw-r--r--   0 adam      (1000) adam      (1000)    18997 2023-06-24 11:07:09.000000 bhv-0.6.1/bhv/cnative/TurboSHAKEopt/KeccakP-1600-opt64.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)     2537 2023-06-24 11:07:09.000000 bhv-0.6.1/bhv/cnative/TurboSHAKEopt/KeccakSponge.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)     2381 2023-06-24 11:07:09.000000 bhv-0.6.1/bhv/cnative/TurboSHAKEopt/TurboSHAKE.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)    11558 2023-06-24 09:31:02.000000 bhv-0.6.1/bhv/cnative/bindings.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-06-24 07:34:04.000000 bhv-0.6.1/bhv/embedding.py
--rw-r--r--   0 adam      (1000) adam      (1000)     4208 2023-06-24 07:40:55.000000 bhv-0.6.1/bhv/lookup.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1897 2023-06-24 07:40:55.000000 bhv-0.6.1/bhv/native.py
--rw-r--r--   0 adam      (1000) adam      (1000)    12443 2023-06-24 07:40:55.000000 bhv-0.6.1/bhv/np.py
--rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.6.1/bhv/poibin.py
--rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.6.1/bhv/pytorch.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-06-16 16:14:43.000000 bhv-0.6.1/bhv/shared.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.6.1/bhv/slice.py
--rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.6.1/bhv/symbolic.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.6.1/bhv/unification.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3575 2023-06-18 07:52:14.000000 bhv-0.6.1/bhv/vanilla.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1372 2023-06-24 07:40:55.000000 bhv-0.6.1/bhv/visualization.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 11:13:42.951196 bhv-0.6.1/bhv.egg-info/
--rw-r--r--   0 adam      (1000) adam      (1000)     1090 2023-06-24 11:13:42.000000 bhv-0.6.1/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)      532 2023-06-24 11:13:42.000000 bhv-0.6.1/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-24 11:13:42.000000 bhv-0.6.1/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       44 2023-06-24 11:13:42.000000 bhv-0.6.1/bhv.egg-info/requires.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-24 11:13:42.000000 bhv-0.6.1/bhv.egg-info/top_level.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-24 11:13:42.952196 bhv-0.6.1/setup.cfg
--rw-r--r--   0 adam      (1000) adam      (1000)     1926 2023-06-24 11:09:07.000000 bhv-0.6.1/setup.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 11:24:42.097119 bhv-0.6.2/
+-rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.6.2/LICENSE
+-rw-r--r--   0 adam      (1000) adam      (1000)       50 2023-06-24 11:24:21.000000 bhv-0.6.2/MANIFEST.in
+-rw-r--r--   0 adam      (1000) adam      (1000)     1090 2023-06-24 11:24:42.097119 bhv-0.6.2/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.6.2/README.md
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 11:24:42.092120 bhv-0.6.2/bhv/
+-rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.6.2/bhv/__init__.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    16739 2023-06-24 07:40:55.000000 bhv-0.6.2/bhv/abstract.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 11:24:42.094119 bhv-0.6.2/bhv/cnative/
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 11:24:42.097119 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/
+-rw-r--r--   0 adam      (1000) adam      (1000)    22154 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/KeccakP-1600-64.macros
+-rw-r--r--   0 adam      (1000) adam      (1000)     2383 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/KeccakP-1600-SnP.h
+-rw-r--r--   0 adam      (1000) adam      (1000)      186 2023-06-11 09:42:52.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/KeccakP-1600-opt64-config.h
+-rw-r--r--   0 adam      (1000) adam      (1000)    18997 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/KeccakP-1600-opt64.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     9730 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/KeccakP-1600-unrolling.macros
+-rw-r--r--   0 adam      (1000) adam      (1000)     2537 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/KeccakSponge.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     2811 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/KeccakSponge.h
+-rw-r--r--   0 adam      (1000) adam      (1000)    11249 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/KeccakSponge.inc
+-rw-r--r--   0 adam      (1000) adam      (1000)     6272 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/SnP-Relaned.h
+-rw-r--r--   0 adam      (1000) adam      (1000)     2381 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/TurboSHAKE.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     1673 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/TurboSHAKE.h
+-rw-r--r--   0 adam      (1000) adam      (1000)      873 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/align.h
+-rw-r--r--   0 adam      (1000) adam      (1000)     5638 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/brg_endian.h
+-rw-r--r--   0 adam      (1000) adam      (1000)      136 2023-06-24 11:07:09.000000 bhv-0.6.2/bhv/cnative/TurboSHAKEopt/config.h
+-rw-r--r--   0 adam      (1000) adam      (1000)    11558 2023-06-24 09:31:02.000000 bhv-0.6.2/bhv/cnative/bindings.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     8239 2023-06-24 11:05:04.000000 bhv-0.6.2/bhv/cnative/packed.h
+-rw-r--r--   0 adam      (1000) adam      (1000)     1566 2023-06-08 12:48:26.000000 bhv-0.6.2/bhv/cnative/plain_test.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)       68 2023-06-08 12:42:27.000000 bhv-0.6.2/bhv/cnative/run.sh
+-rw-r--r--   0 adam      (1000) adam      (1000)      392 2023-06-11 11:32:10.000000 bhv-0.6.2/bhv/cnative/shared.h
+-rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-06-24 07:34:04.000000 bhv-0.6.2/bhv/embedding.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     4208 2023-06-24 07:40:55.000000 bhv-0.6.2/bhv/lookup.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1897 2023-06-24 07:40:55.000000 bhv-0.6.2/bhv/native.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    12443 2023-06-24 07:40:55.000000 bhv-0.6.2/bhv/np.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.6.2/bhv/poibin.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.6.2/bhv/pytorch.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-06-16 16:14:43.000000 bhv-0.6.2/bhv/shared.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.6.2/bhv/slice.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.6.2/bhv/symbolic.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.6.2/bhv/unification.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3575 2023-06-18 07:52:14.000000 bhv-0.6.2/bhv/vanilla.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1372 2023-06-24 07:40:55.000000 bhv-0.6.2/bhv/visualization.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 11:24:42.092120 bhv-0.6.2/bhv.egg-info/
+-rw-r--r--   0 adam      (1000) adam      (1000)     1090 2023-06-24 11:24:42.000000 bhv-0.6.2/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)     1107 2023-06-24 11:24:42.000000 bhv-0.6.2/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-24 11:24:42.000000 bhv-0.6.2/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       44 2023-06-24 11:24:42.000000 bhv-0.6.2/bhv.egg-info/requires.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-24 11:24:42.000000 bhv-0.6.2/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-24 11:24:42.097119 bhv-0.6.2/setup.cfg
+-rw-r--r--   0 adam      (1000) adam      (1000)     1926 2023-06-24 11:24:28.000000 bhv-0.6.2/setup.py
```

### Comparing `bhv-0.6.1/LICENSE` & `bhv-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/PKG-INFO` & `bhv-0.6.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.6.1
+Version: 0.6.2
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
```

### Comparing `bhv-0.6.1/README.md` & `bhv-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/abstract.py` & `bhv-0.6.2/bhv/abstract.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/cnative/TurboSHAKEopt/KeccakP-1600-opt64.cpp` & `bhv-0.6.2/bhv/cnative/TurboSHAKEopt/KeccakP-1600-opt64.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/cnative/TurboSHAKEopt/KeccakSponge.cpp` & `bhv-0.6.2/bhv/cnative/TurboSHAKEopt/KeccakSponge.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/cnative/TurboSHAKEopt/TurboSHAKE.cpp` & `bhv-0.6.2/bhv/cnative/TurboSHAKEopt/TurboSHAKE.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/cnative/bindings.cpp` & `bhv-0.6.2/bhv/cnative/bindings.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/embedding.py` & `bhv-0.6.2/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/lookup.py` & `bhv-0.6.2/bhv/lookup.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/native.py` & `bhv-0.6.2/bhv/native.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/np.py` & `bhv-0.6.2/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/poibin.py` & `bhv-0.6.2/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/pytorch.py` & `bhv-0.6.2/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/shared.py` & `bhv-0.6.2/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/slice.py` & `bhv-0.6.2/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/symbolic.py` & `bhv-0.6.2/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/unification.py` & `bhv-0.6.2/bhv/unification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/vanilla.py` & `bhv-0.6.2/bhv/vanilla.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv/visualization.py` & `bhv-0.6.2/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.6.1/bhv.egg-info/PKG-INFO` & `bhv-0.6.2/bhv.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.6.1
+Version: 0.6.2
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
```

### Comparing `bhv-0.6.1/setup.py` & `bhv-0.6.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages, Extension
 
-VERSION = '0.6.1'
+VERSION = '0.6.2'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 native = Extension("bhv.cnative",
                    sources=['bhv/cnative/bindings.cpp',
                             'bhv/cnative/TurboSHAKEopt/TurboSHAKE.cpp',
                             'bhv/cnative/TurboSHAKEopt/KeccakSponge.cpp',
```

