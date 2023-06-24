# Comparing `tmp/tarn-0.7.1.tar.gz` & `tmp/tarn-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.7.1.tar", last modified: Fri Jun 23 12:54:03 2023, max compression
+gzip compressed data, was "tarn-0.8.0.tar", last modified: Sat Jun 24 14:47:56 2023, max compression
```

## Comparing `tarn-0.7.1.tar` & `tarn-0.8.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.651293 tarn-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-23 12:53:58.000000 tarn-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 12:53:58.000000 tarn-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-23 12:54:03.651293 tarn-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-23 12:53:58.000000 tarn-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-23 12:53:58.000000 tarn-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 12:53:58.000000 tarn-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 12:54:03.651293 tarn-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-23 12:53:58.000000 tarn-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.643293 tarn-0.7.1/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.651293 tarn-0.7.1/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/tools/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.643293 tarn-0.7.1/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-23 12:54:03.000000 tarn-0.7.1/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 12:54:03.000000 tarn-0.7.1/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:54:03.000000 tarn-0.7.1/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 12:54:03.000000 tarn-0.7.1/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 12:54:03.000000 tarn-0.7.1/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-24 14:47:54.000000 tarn-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-24 14:47:54.000000 tarn-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-24 14:47:56.973829 tarn-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-24 14:47:54.000000 tarn-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-24 14:47:54.000000 tarn-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-24 14:47:54.000000 tarn-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:47:56.973829 tarn-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-24 14:47:54.000000 tarn-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.969829 tarn-0.8.0/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.969829 tarn-0.8.0/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/tools/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.969829 tarn-0.8.0/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-24 14:47:56.000000 tarn-0.8.0/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-24 14:47:56.000000 tarn-0.8.0/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:47:56.000000 tarn-0.8.0/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-24 14:47:56.000000 tarn-0.8.0/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 14:47:56.000000 tarn-0.8.0/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.7.1/LICENSE` & `tarn-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.7.1/PKG-INFO` & `tarn-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.7.1
+Version: 0.8.0
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.7.1.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.8.0.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.7.1/README.md` & `tarn-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.7.1/pyproject.toml` & `tarn-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tarn-0.7.1/setup.py` & `tarn-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.1/tarn/cache/storage.py` & `tarn-0.8.0/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.1/tarn/compat.py` & `tarn-0.8.0/tarn/compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import errno
 import os
 import platform
 import shutil
 import stat
 from pathlib import Path
-from typing import Union
 from tempfile import SpooledTemporaryFile as _SpooledTemporaryFile
+from typing import Any, Union
 
 try:
     from typing import Protocol
 except ImportError:
     Protocol = object
 try:
     from gzip import BadGzipFile
 except ImportError:
     BadGzipFile = OSError
+try:
+    from typing import Self
+except ImportError:
+    Self = Any
+
+try:
+    from mypy_boto3_s3 import S3Client
+except ImportError:
+    S3Client = Any
 
 from .interface import PathOrStr
 
 if platform.system() == 'Windows':
     def rmtree(path, ignore_errors=False):
         # source: https://docs.python.org/3.10/library/shutil.html#rmtree-example
         def remove_readonly(func, p, _):
```

### Comparing `tarn-0.7.1/tarn/config.py` & `tarn-0.8.0/tarn/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import humanfriendly
 from pydantic import BaseModel, Extra, root_validator, validator
 from yaml import safe_dump, safe_load
 
 from .compat import get_path_group
 from .interface import PathOrStr
-from .tools import DummyLocker, DummySize, DummyUsage, Locker, SizeTracker, UsageTracker, LabelsStorage, DummyLabels
+from .tools import DummyLabels, DummyLocker, DummySize, DummyUsage, LabelsStorage, Locker, SizeTracker, UsageTracker
 from .utils import mkdir
 
 CONFIG_NAME = 'config.yml'
 
 
 class _NoExtra(BaseModel):
     class Config:
```

### Comparing `tarn-0.7.1/tarn/interface.py` & `tarn-0.8.0/tarn/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,30 @@
+import datetime
 import logging
 import os
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, BinaryIO, Callable, Iterable, Optional, Sequence, Tuple, Union, Collection
+from typing import Any, BinaryIO, Callable, Collection, Iterable, Optional, Sequence, Tuple, Union
 
 Key = bytes
 Keys = Sequence[Key]
 PathOrStr = Union[Path, str, os.PathLike]
 Value = Union[BinaryIO, PathOrStr]
 MaybeValue = Optional[Value]
 MaybeLabels = Optional[Collection[str]]
 
 logger = logging.getLogger(__name__)
 
 
+class Meta:
+    last_used: Optional[datetime.datetime]
+    labels: MaybeLabels
+
+
+# TODO: deprecated
 class LocalStorage(ABC):
     """
     Storage that has a well-defined location on the filesystem
     """
 
     def __init__(self, hash, levels: Sequence[int]):
         self.hash = hash
```

### Comparing `tarn-0.7.1/tarn/local/storage.py` & `tarn-0.8.0/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.1/tarn/location/disk_dict.py` & `tarn-0.8.0/tarn/location/disk_dict.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+import datetime
 import logging
 import os
 import random
 import shutil
 import string
 from contextlib import contextmanager
 from pathlib import Path
-from typing import ContextManager, Iterable, Optional, Tuple
+from typing import ContextManager, Iterable, Optional, Tuple, Union
 
-from ..compat import copy_file, remove_file, rmtree
+from ..compat import Self, copy_file, remove_file, rmtree
 from ..config import load_config, root_params
 from ..digest import key_to_relative
 from ..exceptions import StorageCorruption
-from ..interface import Key, Keys, MaybeValue, PathOrStr, Value, MaybeLabels
+from ..interface import Key, Keys, MaybeLabels, MaybeValue, PathOrStr, Value
 from ..tools import Locker, SizeTracker, UsageTracker
 from ..tools.labels import LabelsStorage
 from ..utils import adjust_permissions, create_folders, get_size, match_buffers, match_files
-from .interface import Writable
+from .interface import Meta, Writable
 
 logger = logging.getLogger(__name__)
 MaybePath = Optional[Path]
 
 
 class DiskDict(Writable):
     def __init__(self, root: PathOrStr):
@@ -47,40 +48,54 @@
         self.min_free_size = config.free_disk_size
         self.max_size = config.max_size
 
     @property
     def key_size(self):
         return sum(self.levels)
 
+    def contents(self) -> Iterable[Tuple[Key, Self, Meta]]:
+        tools = self.root / 'tools'
+        config = self.root / 'config.yml'
+        for file in self.root.glob('/'.join('*' * len(self.levels))):
+            if file == config or file.is_relative_to(tools):
+                continue
+
+            key = bytes.fromhex(''.join(file.relative_to(self.root).parts))
+            with self.locker.read(key):
+                yield key, self, str(self.root)
+
     @contextmanager
-    def read(self, key: Key) -> ContextManager[MaybePath]:
+    def read(self, key: Key, return_labels: bool) -> ContextManager[Union[None, Value, Tuple[Value, MaybeLabels]]]:
         file = self._key_to_path(key)
         corrupted = False
         with self.locker.read(key):
             if file.exists():
                 # TODO: deprecated
                 if file.is_dir():
                     file = file / 'data'
 
                 self.usage_tracker.update(key)
                 try:
-                    yield file
+                    if return_labels:
+                        yield file, self.labels.get(key)
+                    else:
+                        yield file
                     return
                 except StorageCorruption:
                     corrupted = True
 
         if corrupted:
             self.delete(key)
             return
 
         yield None
 
-    def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, MaybeValue]]:
+    def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, Union[Value, MaybeLabels]]]:
         for key in keys:
-            with self.read(key) as value:
+            with self.read(key, True) as value:
                 yield key, value
 
     @contextmanager
     def write(self, key: Key, value: Value, labels: MaybeLabels) -> ContextManager[MaybeValue]:
         file = self._key_to_path(key)
         with self.locker.write(key):
             try:
@@ -169,14 +184,27 @@
 
         if self.max_size is not None and self.max_size < float('inf'):
             result = result and self.size_tracker.get(self.root) <= self.max_size
 
         return result
 
 
+class DiskDictMeta(Meta):
+    def __init__(self, key, usage, labels):
+        self._key, self._usage, self._labels = key, usage, labels
+
+    @property
+    def last_used(self) -> Optional[datetime.datetime]:
+        return self._usage.get(self._key)
+
+    @property
+    def labels(self) -> MaybeLabels:
+        return self._labels.get(self._key)
+
+
 def _is_pathlike(x):
     return isinstance(x, (os.PathLike, str))
 
 
 def _match(value, file, key):
     if _is_pathlike(value):
         match_files(value, file)
```

### Comparing `tarn-0.7.1/tarn/location/fanout.py` & `tarn-0.8.0/tarn/location/fanout.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from contextlib import contextmanager
-from typing import ContextManager, Iterable, Tuple
+from typing import ContextManager, Iterable, Tuple, Union
 
-from ..interface import Key, Keys, MaybeValue, Value, MaybeLabels
+from ..compat import Self
+from ..interface import Key, Keys, MaybeLabels, MaybeValue, Meta, Value
 from .interface import Location, Writable
 
 
 class Fanout(Writable):
     def __init__(self, *locations: Location):
         sizes = {location.key_size for location in locations if location.key_size is not None}
         hashes = {location.hash for location in locations if location.hash is not None}
@@ -13,18 +14,18 @@
         assert len(hashes) <= 1, hashes
 
         self._locations = locations
         self.key_size = sizes.pop() if sizes else None
         self.hash = hashes.pop() if hashes else None
 
     @contextmanager
-    def read(self, key: Key) -> ContextManager[MaybeValue]:
+    def read(self, key: Key, return_labels: bool) -> ContextManager[Union[None, Value, Tuple[Value, MaybeLabels]]]:
         raised = False
         for location in self._locations:
-            with location.read(key) as value:
+            with location.read(key, return_labels) as value:
                 if value is not None:
                     try:
                         yield value
                         return
                     except BaseException:
                         raised = True
                         raise
@@ -74,7 +75,11 @@
                 else:
                     yield key, value
 
             keys = remaining
 
         for key in keys:
             yield key, None
+
+    def contents(self) -> Iterable[Tuple[Key, Self, Meta]]:
+        for location in self._locations:
+            yield from location.contents()
```

### Comparing `tarn-0.7.1/tarn/location/interface.py` & `tarn-0.8.0/tarn/location/interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 from abc import ABC, abstractmethod
-from typing import ContextManager, Iterable, Optional, Sequence, Tuple, Type
+from typing import ContextManager, Iterable, Optional, Sequence, Tuple, Type, Union
 
-from ..compat import HashAlgorithm
-from ..interface import Key, Keys, MaybeValue, Value, MaybeLabels
+from ..compat import HashAlgorithm, Self
+from ..interface import Key, Keys, MaybeLabels, MaybeValue, Meta, Value
 
 
 class Location(ABC):
     key_size: Optional[int]
     hash: Optional[Type[HashAlgorithm]]
 
     @abstractmethod
-    def read(self, key: Key) -> ContextManager[MaybeValue]:
+    def read(self, key: Key, return_labels: bool) -> ContextManager[Union[None, Value, Tuple[Value, MaybeLabels]]]:
         """
         Read a value for a given `key`. If the result is None - the key was not found.
 
         Examples
         --------
         >>> with location.read(key) as result:
         ...     if result is None:
         ...        print('not found')
         ...     else:
         ...         with open(result) as file:
         ...             print('found', file.read())
         """
 
     @abstractmethod
-    def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, MaybeValue]]:
+    def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, Union[None, Tuple[Value, MaybeLabels]]]]:
         """
         Reads multiple values given a collection of `keys`.
 
         Examples
         --------
         >>> for key, result in location.read_batch(keys):
         ...     if result is None:
         ...        print(key, 'not found')
         ...     else:
         ...        print(key, 'found')
         """
 
+    @abstractmethod
+    def contents(self) -> Iterable[Tuple[Key, Self, Meta]]:
+        pass
+
 
 class Writable(Location, ABC):
     @abstractmethod
     def write(self, key: Key, value: Value, labels: MaybeLabels) -> ContextManager[MaybeValue]:
         pass
 
     @abstractmethod
```

### Comparing `tarn-0.7.1/tarn/location/levels.py` & `tarn-0.8.0/tarn/location/levels.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 from contextlib import contextmanager
 from itertools import islice
 from typing import ContextManager, Iterable, NamedTuple, Optional, Tuple, Union
 
-from ..interface import Key, Keys, MaybeValue, Value, MaybeLabels
+from ..compat import Self
+from ..interface import Key, Keys, MaybeLabels, MaybeValue, Meta, Value
 from ..location import Location, Writable
 
 
 class Level(NamedTuple):
     location: Location
     write: bool = True
     replicate: bool = True
@@ -26,25 +27,28 @@
         assert len(hashes) <= 1, hashes
 
         self._levels = levels
         self.key_size = sizes.pop() if sizes else None
         self.hash = hashes.pop() if hashes else None
 
     @contextmanager
-    def read(self, key: Key) -> ContextManager[MaybeValue]:
+    def read(self, key: Key, return_labels: bool) -> ContextManager[Union[None, Value, Tuple[Value, MaybeLabels]]]:
         # TODO: ExitStack?
         #  https://docs.python.org/3/library/contextlib.html#replacing-any-use-of-try-finally-and-flag-variables
         raised = False
         for index, config in enumerate(self._levels):
-            with config.location.read(key) as value:
+            with config.location.read(key, True) as value:
                 if value is not None:
                     # try to write to a level with higher priority
-                    with self._replicate(key, value, index) as mirrored:
+                    with self._replicate(key, *value, index) as (value_copy, labels_copy):
                         try:
-                            yield mirrored
+                            if return_labels:
+                                yield value_copy, labels_copy
+                            else:
+                                yield value_copy
                             return
                         except BaseException:
                             raised = True
                             raise
 
             if raised:
                 return
@@ -76,43 +80,47 @@
         for config in self._levels:
             if config.write and isinstance(config.location, Writable):
                 if config.location.delete(key):
                     deleted = True
 
         return deleted
 
-    def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, MaybeValue]]:
+    def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, Tuple[Value, MaybeLabels]]]:
         for index, config in enumerate(self._levels):
             if not keys:
                 return
 
             remaining = []
             for key, value in config.location.read_batch(keys):
                 if value is None:
                     remaining.append(key)
                 else:
-                    with self._replicate(key, value, index) as mirrored:
+                    with self._replicate(key, *value, index) as mirrored:
                         yield key, mirrored
 
             keys = remaining
 
         for key in keys:
             yield key, None
 
+    def contents(self) -> Iterable[Tuple[Key, Self, Meta]]:
+        for level in self._levels:
+            yield from level.location.contents()
+
     @contextmanager
-    def _replicate(self, key: Key, value: Value, index: int):
+    def _replicate(self, key: Key, value: Value, labels: MaybeLabels, index: int):
         for config in islice(self._levels, index):
             location = config.location
             if config.replicate and isinstance(location, Writable):
-                with _propagate_exception(location.write(key, value, None)) as written:
+                with _propagate_exception(location.write(key, value, labels)) as written:
                     if written is not None:
-                        yield written
+                        yield written, labels
                         return
 
-        yield value
+        yield value, labels
 
 
 @contextmanager
 def _propagate_exception(cm: ContextManager):
     value = cm.__enter__()
     clean = True
     try:
```

### Comparing `tarn-0.7.1/tarn/location/scp.py` & `tarn-0.8.0/tarn/location/scp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import socket
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, ContextManager, Iterable, Sequence, Tuple, Union
+from typing import ContextManager, Iterable, Sequence, Tuple, Union
 
 import paramiko
 from paramiko import AuthenticationException, SSHClient, SSHException
 from paramiko.config import SSH_PORT, SSHConfig
 from paramiko.ssh_exception import NoValidConnectionsError
 from scp import SCPClient, SCPException
 
-from ..compat import remove_file, rmtree
+from ..compat import Self, remove_file, rmtree
 from ..config import load_config
 from ..digest import key_to_relative
-from ..interface import Key, Keys, MaybeValue, PathOrStr
+from ..interface import Key, Keys, MaybeLabels, Meta, PathOrStr, Value
 from .interface import Location
 
 
 class UnknownHostException(SSHException):
     pass
 
 
@@ -52,40 +52,46 @@
         return self.__class__, (self.hostname, self.root, self.port, self.username, self.password, self.key)
 
     @property
     def key_size(self):
         return sum(self.levels) if self.levels is not None else None
 
     @contextmanager
-    def read(self, key: Key) -> ContextManager[MaybeValue]:
+    def read(self, key: Key, return_labels: bool) -> ContextManager[Union[None, Value, Tuple[Value, MaybeLabels]]]:
         with self._connect() as scp:
             if not scp:
                 yield
                 return
 
             with tempfile.TemporaryDirectory() as temp_dir:
                 source = Path(temp_dir) / 'source'
                 try:
                     scp.get(str(self.root / key_to_relative(key, self.levels)), str(source), recursive=True)
                     if not source.exists():
                         yield None
                     else:
                         # TODO: legacy
                         if source.is_dir():
-                            yield source / 'data'
+                            if return_labels:
+                                yield source / 'data', None
+                            else:
+                                yield source / 'data'
                             rmtree(source)
 
                         else:
-                            yield source
+                            if return_labels:
+                                yield source, None
+                            else:
+                                yield source
                             remove_file(source)
 
                 except (SCPException, socket.timeout, SSHException):
                     yield None
 
-    def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, MaybeValue]]:
+    def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, Union[None, Tuple[Value, MaybeLabels]]]]:
         with self._connect() as scp:
             if scp is None:
                 for key in keys:
                     yield key, None
                 return
 
             # TODO: add `retry` logic?
@@ -93,27 +99,31 @@
                 source = Path(temp_dir) / 'source'
                 for key in keys:
                     try:
                         scp.get(str(self.root / key_to_relative(key, self.levels)), str(source), recursive=True)
                         if source.exists():
                             # TODO: legacy
                             if source.is_dir():
-                                yield key, source / 'data'
+                                yield key, (source / 'data', None)
                                 rmtree(source)
 
                             else:
-                                yield key, source
+                                yield key, (source, None)
                                 remove_file(source)
 
                         else:
                             yield key, None
 
                     except (SCPException, socket.timeout, SSHException):
                         yield key, None
 
+    def contents(self) -> Iterable[Tuple[Key, Self, Meta]]:
+        # TODO
+        return []
+
     @contextmanager
     def _connect(self) -> SCPClient:
         try:
             self.ssh.connect(
                 self.hostname, self.port, self.username, self.password, key_filename=self.key,
                 auth_timeout=10
             )
```

### Comparing `tarn-0.7.1/tarn/pickler/compat.py` & `tarn-0.8.0/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.1/tarn/pickler/interface.py` & `tarn-0.8.0/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.1/tarn/pool/hash_key.py` & `tarn-0.8.0/tarn/pool/hash_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from io import BytesIO
 import os
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Callable, ContextManager, Iterable, Optional, Sequence, Tuple, Type, Union, Collection
+from typing import Any, Callable, ContextManager, Iterable, Optional, Sequence, Tuple, Type, Union
 
 from ..compat import HashAlgorithm
 from ..digest import digest_value
 from ..exceptions import ReadError, WriteError
-from ..interface import Key, Keys, MaybeValue, PathOrStr, MaybeLabels, Value
+from ..interface import Key, Keys, MaybeLabels, MaybeValue, PathOrStr, Value
 from ..location import DiskDict, Fanout, Levels, Location
 
 LocationLike = Union[Location, PathOrStr]
 LocationsLike = Union[LocationLike, Sequence[LocationLike]]
 
 
 class HashKeyStorage:
@@ -49,15 +49,15 @@
     def _read_context(self, key, fetch, error) -> ContextManager[MaybeValue]:
         fetch = self._resolve_value(fetch, self._fetch, 'fetch')
         error = self._resolve_value(error, self._error, 'error')
 
         if isinstance(key, str):
             key = bytes.fromhex(key)
         location = self._full if fetch else self._local
-        with location.read(key) as value:
+        with location.read(key, False) as value:
             if value is None and error:
                 raise ReadError(f'The key {key.hex()} is not found')
             yield value
 
     def _read_func(self, func: Callable, key: Key, *args, fetch, error, **kwargs) -> Any:
         with self._read_context(key, fetch, error) as value:
             return func(value, *args, **kwargs)
```

### Comparing `tarn-0.7.1/tarn/pool/pickle_key.py` & `tarn-0.8.0/tarn/pool/pickle_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import logging
 from io import BytesIO
 from pathlib import Path
 from typing import Any, NamedTuple, Optional, Sequence, Type, Union
 
 from ..compat import HashAlgorithm
-from ..exceptions import ReadError, StorageCorruption, WriteError, DeserializationError
-from ..interface import Key, PathOrStr, MaybeLabels
+from ..exceptions import DeserializationError, ReadError, StorageCorruption, WriteError
+from ..interface import Key, MaybeLabels, PathOrStr
 from ..location import Level, Location
 from ..pickler import PREVIOUS_VERSIONS, dumps
 from ..serializers import Serializer, SerializerError
 from .hash_key import HashKeyStorage, LocationsLike, resolve_location
 
 logger = logging.getLogger(__name__)
 
@@ -74,15 +74,15 @@
                 if error:
                     raise WriteError('The index could not be written to any storage')
                 return None
 
         return digest
 
     def _read_for_digest(self, digest):
-        with self.index.read(digest) as index:
+        with self.index.read(digest, False) as index:
             if index is None:
                 return None, False
 
             contents = list(_unpack_mapping(index))
             try:
                 return self.serializer.load(contents, self.storage.read), True
             # either the data is corrupted or missing
```

### Comparing `tarn-0.7.1/tarn/serializers.py` & `tarn-0.8.0/tarn/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from collections import defaultdict
+
 import inspect
 import json
 from pathlib import Path
 import pickle
 from abc import ABC, abstractmethod
+from collections import defaultdict
 from contextlib import suppress
 from functools import partial
 from gzip import GzipFile
+from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any, Callable, Dict, Iterable, Sequence, Tuple, Union
 
 import numpy as np
 
-from .digest import value_to_buffer
 from .compat import BadGzipFile, SpooledTemporaryFile
-from .exceptions import SerializerError, DeserializationError
-
+from .digest import value_to_buffer
+from .exceptions import DeserializationError, SerializerError
 
 __all__ = (
-    'Serializer', 'SerializerError', 'ChainSerializer', 'DictSerializer',
-    'NumpySerializer', 'JsonSerializer', 'PickleSerializer',
+    'Serializer', 'SerializerError', 'ContentsIn', 'ContentsOut',
+    'ChainSerializer', 'DictSerializer', 'NumpySerializer', 'JsonSerializer', 'PickleSerializer',
 )
 
 ContentsOut = Iterable[Tuple[str, Any]]
 ContentsIn = Sequence[Tuple[str, Any]]
 
 
 class Serializer(ABC):
@@ -54,15 +55,15 @@
 
         raise SerializerError(f'No serializer was able to save the value of type {type(value).__name__!r}.')
 
     def load(self, contents: ContentsIn, read: Callable) -> Any:
         # TODO: old style
         if isinstance(contents, (str, Path)):
             contents = [
-                (str(file.relative_to(contents)), bytes.fromhex(file.read_text())) 
+                (str(file.relative_to(contents)), bytes.fromhex(file.read_text()))
                 for file in contents.glob('**/*') if not file.is_dir()
             ]
             read = read.read
 
         contents = list(contents)
         for serializer in self.serializers:
             with suppress(SerializerError):
```

### Comparing `tarn-0.7.1/tarn/tools/labels.py` & `tarn-0.8.0/tarn/tools/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from abc import ABC, abstractmethod
 from pathlib import Path
 
-from ..compat import remove_file, get_path_group, set_path_attrs
+from ..compat import get_path_group, remove_file, set_path_attrs
 from ..digest import key_to_relative
-from ..interface import MaybeLabels, Key
+from ..interface import Key, MaybeLabels
 
 __all__ = 'LabelsStorage', 'DummyLabels'
 
 from ..utils import create_folders
 
 
 class LabelsStorage(ABC):
```

### Comparing `tarn-0.7.1/tarn/tools/locker.py` & `tarn-0.8.0/tarn/tools/locker.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.1/tarn/tools/size.py` & `tarn-0.8.0/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.1/tarn/tools/usage.py` & `tarn-0.8.0/tarn/tools/usage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.1/tarn/utils.py` & `tarn-0.8.0/tarn/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import filecmp
+import os
+from contextlib import contextmanager
+from io import BytesIO
 from pathlib import Path
 from typing import BinaryIO, Union
 
 from .compat import set_path_attrs
-from .interface import Key  # noqa
+from .interface import Key, Value  # noqa
 
 # TODO: legacy
 PathLike = Union[Path, str]
 
 
 def to_read_only(path: Path, permissions, group):
     adjust_permissions(path, permissions, group, read_only=True)
@@ -48,7 +51,20 @@
     while True:
         b1 = first.read(bufsize)
         b2 = second.read(bufsize)
         if b1 != b2:
             raise ValueError(f'Buffers do not match: {context}')
         if not b1:
             return True
+
+
+@contextmanager
+def value_to_buffer(value: Union[Value, bytes]):
+    if isinstance(value, bytes):
+        yield BytesIO(value)
+
+    elif isinstance(value, (str, os.PathLike)):
+        with open(value, 'rb') as file:
+            yield file
+
+    else:
+        yield value
```

### Comparing `tarn-0.7.1/tarn.egg-info/PKG-INFO` & `tarn-0.8.0/tarn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.7.1
+Version: 0.8.0
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.7.1.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.8.0.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.7.1/tarn.egg-info/SOURCES.txt` & `tarn-0.8.0/tarn.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 tarn/local/storage.py
 tarn/location/__init__.py
 tarn/location/disk_dict.py
 tarn/location/fanout.py
 tarn/location/interface.py
 tarn/location/levels.py
 tarn/location/nginx.py
+tarn/location/s3.py
 tarn/location/scp.py
 tarn/pickler/__init__.py
 tarn/pickler/compat.py
 tarn/pickler/interface.py
 tarn/pool/__init__.py
 tarn/pool/hash_key.py
 tarn/pool/pickle_key.py
```

