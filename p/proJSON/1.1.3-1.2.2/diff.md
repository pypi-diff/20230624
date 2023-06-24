# Comparing `tmp/proJSON-1.1.3.tar.gz` & `tmp/proJSON-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proJSON-1.1.3.tar", last modified: Sat Jun 17 21:39:16 2023, max compression
+gzip compressed data, was "proJSON-1.2.2.tar", last modified: Sat Jun 24 13:42:31 2023, max compression
```

## Comparing `proJSON-1.1.3.tar` & `proJSON-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:39:16.970172 proJSON-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-17 21:39:07.000000 proJSON-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-17 21:39:16.970172 proJSON-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-17 21:39:07.000000 proJSON-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-17 21:39:07.000000 proJSON-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 21:39:16.970172 proJSON-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:39:16.970172 proJSON-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:39:16.970172 proJSON-1.1.3/src/proJSON/
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-17 21:39:07.000000 proJSON-1.1.3/src/proJSON/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:39:16.970172 proJSON-1.1.3/src/proJSON.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-17 21:39:16.000000 proJSON-1.1.3/src/proJSON.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 21:39:16.000000 proJSON-1.1.3/src/proJSON.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 21:39:16.000000 proJSON-1.1.3/src/proJSON.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 21:39:16.000000 proJSON-1.1.3/src/proJSON.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:39:16.970172 proJSON-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-17 21:39:07.000000 proJSON-1.1.3/tests/test_projson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:42:31.898164 proJSON-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-24 13:42:19.000000 proJSON-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-24 13:42:31.898164 proJSON-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-24 13:42:19.000000 proJSON-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-24 13:42:19.000000 proJSON-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 13:42:31.898164 proJSON-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:42:31.894164 proJSON-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:42:31.898164 proJSON-1.2.2/src/proJSON/
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-06-24 13:42:19.000000 proJSON-1.2.2/src/proJSON/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:42:31.898164 proJSON-1.2.2/src/proJSON.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-24 13:42:31.000000 proJSON-1.2.2/src/proJSON.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-24 13:42:31.000000 proJSON-1.2.2/src/proJSON.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 13:42:31.000000 proJSON-1.2.2/src/proJSON.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 13:42:31.000000 proJSON-1.2.2/src/proJSON.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-24 13:42:31.000000 proJSON-1.2.2/src/proJSON.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:42:31.898164 proJSON-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-24 13:42:19.000000 proJSON-1.2.2/tests/test_projson.py
```

### Comparing `proJSON-1.1.3/LICENSE` & `proJSON-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proJSON-1.1.3/PKG-INFO` & `proJSON-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proJSON
-Version: 1.1.3
+Version: 1.2.2
 Summary: A python library to compress a dict into a bytearray.
 Author-email: JKinc <communications@jkinc.co.uk>
 Project-URL: Homepage, https://github.com/The-Geiger-Network-Project/proJSON/tree/main
 Project-URL: Bug Tracker, https://github.com/The-Geiger-Network-Project/proJSON/tree/main/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,22 +47,32 @@
 "stringExample" : {
     "type": "string",  # Set string type
     "maxlen": 1        # Set max size of string ( the max size of the string is calculated by (2^(8*n)-1). if n is 1 then the max size is 255) (optional defaults to 2)
 } 
 
 "bytesExample" : {
     "type": "bytes",   # Set bytes type
-    "maxlen": 1          # Set max size of string ( the max size of the string is calculated by (2^(8*n)-1). if n is 1 then the max size is 255) (optional defaults to 2)
+    "maxlen": 1        # Set max size of string ( the max size of the string is calculated by (2^(8*n)-1). if n is 1 then the max size is 255) (optional defaults to 2)
 } 
 
 "dirExample" : {
     "type": "dir",     # Set dir type
     "subdirs": {}      # A dictionary of int, string and byte types in the format above.
 } 
 
+"boolExample" : {
+    "type" : "bool"    # Set bool type
+}
+
+"listExample" : {
+    "type" : "list",   # Set list type
+    "subtype": "int",  # Set list contents type to an "int"
+    "maxlen": 1        # The "maxlen" parameter for bytes or str (for "int" maxlen is still used instead of "byte")
+}
+
 ```
 
 ***Don't put a dir in another dir. It won't work***
 
 ### Init
 
 ``` python
```

### Comparing `proJSON-1.1.3/README.md` & `proJSON-1.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -33,22 +33,32 @@
 "stringExample" : {
     "type": "string",  # Set string type
     "maxlen": 1        # Set max size of string ( the max size of the string is calculated by (2^(8*n)-1). if n is 1 then the max size is 255) (optional defaults to 2)
 } 
 
 "bytesExample" : {
     "type": "bytes",   # Set bytes type
-    "maxlen": 1          # Set max size of string ( the max size of the string is calculated by (2^(8*n)-1). if n is 1 then the max size is 255) (optional defaults to 2)
+    "maxlen": 1        # Set max size of string ( the max size of the string is calculated by (2^(8*n)-1). if n is 1 then the max size is 255) (optional defaults to 2)
 } 
 
 "dirExample" : {
     "type": "dir",     # Set dir type
     "subdirs": {}      # A dictionary of int, string and byte types in the format above.
 } 
 
+"boolExample" : {
+    "type" : "bool"    # Set bool type
+}
+
+"listExample" : {
+    "type" : "list",   # Set list type
+    "subtype": "int",  # Set list contents type to an "int"
+    "maxlen": 1        # The "maxlen" parameter for bytes or str (for "int" maxlen is still used instead of "byte")
+}
+
 ```
 
 ***Don't put a dir in another dir. It won't work***
 
 ### Init
 
 ``` python
```

### Comparing `proJSON-1.1.3/pyproject.toml` & `proJSON-1.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proJSON"
-version = "1.1.3"
+version = "1.2.2"
 authors = [
   { name="JKinc", email="communications@jkinc.co.uk" },
 ]
 description = "A python library to compress a dict into a bytearray."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+    "lz4 == 4.3.2"
+]
+
 [project.urls]
 "Homepage" = "https://github.com/The-Geiger-Network-Project/proJSON/tree/main"
 "Bug Tracker" = "https://github.com/The-Geiger-Network-Project/proJSON/tree/main/issues"
```

### Comparing `proJSON-1.1.3/src/proJSON.egg-info/PKG-INFO` & `proJSON-1.2.2/src/proJSON.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proJSON
-Version: 1.1.3
+Version: 1.2.2
 Summary: A python library to compress a dict into a bytearray.
 Author-email: JKinc <communications@jkinc.co.uk>
 Project-URL: Homepage, https://github.com/The-Geiger-Network-Project/proJSON/tree/main
 Project-URL: Bug Tracker, https://github.com/The-Geiger-Network-Project/proJSON/tree/main/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,22 +47,32 @@
 "stringExample" : {
     "type": "string",  # Set string type
     "maxlen": 1        # Set max size of string ( the max size of the string is calculated by (2^(8*n)-1). if n is 1 then the max size is 255) (optional defaults to 2)
 } 
 
 "bytesExample" : {
     "type": "bytes",   # Set bytes type
-    "maxlen": 1          # Set max size of string ( the max size of the string is calculated by (2^(8*n)-1). if n is 1 then the max size is 255) (optional defaults to 2)
+    "maxlen": 1        # Set max size of string ( the max size of the string is calculated by (2^(8*n)-1). if n is 1 then the max size is 255) (optional defaults to 2)
 } 
 
 "dirExample" : {
     "type": "dir",     # Set dir type
     "subdirs": {}      # A dictionary of int, string and byte types in the format above.
 } 
 
+"boolExample" : {
+    "type" : "bool"    # Set bool type
+}
+
+"listExample" : {
+    "type" : "list",   # Set list type
+    "subtype": "int",  # Set list contents type to an "int"
+    "maxlen": 1        # The "maxlen" parameter for bytes or str (for "int" maxlen is still used instead of "byte")
+}
+
 ```
 
 ***Don't put a dir in another dir. It won't work***
 
 ### Init
 
 ``` python
```

### Comparing `proJSON-1.1.3/tests/test_projson.py` & `proJSON-1.2.2/tests/test_projson.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,31 +29,41 @@
                     "maxlen": 1
                 },
                 "bytesExample" : {
                     "type": "bytes",
                     "maxlen": 2
                 },
             }
-        } 
+        },
+        "boolExample" : {
+            "type": "bool"
+        },
+        "listExample" : {
+            "type": "list",
+            "subtype": "int",
+            "maxlen": 1 # the same as the "byte" field on the "intExample" field
+        }
     }
 
-    crafter = Crafter(template)
+    crafter = Crafter(template, compression="dev")
 
     exampledata = {
         "intExample" : 200,
         "stringExample" : "Hello World!",
         "bytesExample": b"This is bytes",
         "dirExample" : {
             "intExample2" : 201,
             "stringExample2": "Hello Again!",
             "bytesExample": b"Again, This is bytes"
-        }
+        },
+        "boolExample" : True,
+        "listExample" : [1,2,3]
     }
 
-    assert crafter.encode(exampledata) == b'\xc8\x0cHello World!\x00\rThis is bytes\xc9\x0cHello Again!\x00\x14Again, This is bytes'
+    assert crafter.encode(exampledata) == b'\xc8\x0cHello World!\x00\rThis is bytes\xc9\x0cHello Again!\x00\x14Again, This is bytes\x01\x01\x02\x03\xff'
 
 def test_decode():
     template = {
         "intExample" : {
             "type": "int",
             "byte": 1
         },
@@ -77,26 +87,36 @@
                     "maxlen": 1
                 },
                 "bytesExample" : {
                     "type": "bytes",
                     "maxlen": 2
                 },
             }
-        } 
+        },
+        "boolExample" : {
+            "type": "bool"
+        },
+        "listExample" : {
+            "type": "list",
+            "subtype": "int",
+            "maxlen": 1 # the same as the "byte" field on the "intExample" field
+        }
     }
 
     crafter = Crafter(template)
 
     exampledata = {
         "intExample" : 200,
         "stringExample" : "Hello World!",
         "bytesExample": b"This is bytes",
         "dirExample" : {
             "intExample2" : 201,
             "stringExample2": "Hello Again!",
             "bytesExample": b"Again, This is bytes"
-        }
+        },
+        "boolExample" : True,
+        "listExample" : [1,2,3]
     }
 
     x = crafter.encode(exampledata)
 
     assert crafter.decode(x) == exampledata
```

