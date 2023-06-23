# Comparing `tmp/cirq-1.2.0.dev20230623200337-py3-none-any.whl.zip` & `tmp/cirq-1.2.0.dev20230623220557-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 7983 bytes, number of entries: 5
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-23 20:03 cirq-1.2.0.dev20230623200337.dist-info/LICENSE
--rw-r--r--  2.0 unx     7885 b- defN 23-Jun-23 20:03 cirq-1.2.0.dev20230623200337.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 20:03 cirq-1.2.0.dev20230623200337.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-23 20:03 cirq-1.2.0.dev20230623200337.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      461 b- defN 23-Jun-23 20:03 cirq-1.2.0.dev20230623200337.dist-info/RECORD
-5 files, 19796 bytes uncompressed, 7113 bytes compressed:  64.1%
+Zip file size: 8385 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      292 b- defN 23-Jun-23 22:06 cirq-1.2.0.dev20230623220557.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-23 22:06 cirq-1.2.0.dev20230623220557.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7885 b- defN 23-Jun-23 22:06 cirq-1.2.0.dev20230623220557.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 22:06 cirq-1.2.0.dev20230623220557.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-23 22:06 cirq-1.2.0.dev20230623220557.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 23-Jun-23 22:06 cirq-1.2.0.dev20230623220557.dist-info/RECORD
+6 files, 20190 bytes uncompressed, 7347 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
-Filename: cirq-1.2.0.dev20230623200337.dist-info/LICENSE
+Filename: cirq-1.2.0.dev20230623220557.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.2.0.dev20230623200337.dist-info/METADATA
+Filename: cirq-1.2.0.dev20230623220557.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.2.0.dev20230623200337.dist-info/WHEEL
+Filename: cirq-1.2.0.dev20230623220557.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.2.0.dev20230623200337.dist-info/top_level.txt
+Filename: cirq-1.2.0.dev20230623220557.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.2.0.dev20230623200337.dist-info/RECORD
+Filename: cirq-1.2.0.dev20230623220557.dist-info/top_level.txt
+Comment: 
+
+Filename: cirq-1.2.0.dev20230623220557.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.2.0.dev20230623200337.dist-info/LICENSE` & `cirq-1.2.0.dev20230623220557.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.2.0.dev20230623200337.dist-info/METADATA` & `cirq-1.2.0.dev20230623220557.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.2.0.dev20230623200337
+Version: 1.2.0.dev20230623220557
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
-Requires-Dist: cirq-aqt (==1.2.0.dev20230623200337)
-Requires-Dist: cirq-core (==1.2.0.dev20230623200337)
-Requires-Dist: cirq-ft (==1.2.0.dev20230623200337)
-Requires-Dist: cirq-google (==1.2.0.dev20230623200337)
-Requires-Dist: cirq-ionq (==1.2.0.dev20230623200337)
-Requires-Dist: cirq-pasqal (==1.2.0.dev20230623200337)
-Requires-Dist: cirq-rigetti (==1.2.0.dev20230623200337)
-Requires-Dist: cirq-web (==1.2.0.dev20230623200337)
+Requires-Dist: cirq-aqt (==1.2.0.dev20230623220557)
+Requires-Dist: cirq-core (==1.2.0.dev20230623220557)
+Requires-Dist: cirq-ft (==1.2.0.dev20230623220557)
+Requires-Dist: cirq-google (==1.2.0.dev20230623220557)
+Requires-Dist: cirq-ionq (==1.2.0.dev20230623220557)
+Requires-Dist: cirq-pasqal (==1.2.0.dev20230623220557)
+Requires-Dist: cirq-rigetti (==1.2.0.dev20230623220557)
+Requires-Dist: cirq-web (==1.2.0.dev20230623220557)
 Provides-Extra: dev_env
 Requires-Dist: mypy (==1.2.0) ; extra == 'dev_env'
 Requires-Dist: types-backports (==0.1.3) ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
 Requires-Dist: types-protobuf (==3.19.22) ; extra == 'dev_env'
 Requires-Dist: types-requests (==2.28.1) ; extra == 'dev_env'
 Requires-Dist: types-setuptools (==62.6.1) ; extra == 'dev_env'
```

