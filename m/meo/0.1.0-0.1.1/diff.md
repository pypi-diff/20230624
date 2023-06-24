# Comparing `tmp/meo-0.1.0.tar.gz` & `tmp/meo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meo-0.1.0.tar", last modified: Sat Jun 24 11:34:12 2023, max compression
+gzip compressed data, was "meo-0.1.1.tar", last modified: Sat Jun 24 12:07:38 2023, max compression
```

## Comparing `meo-0.1.0.tar` & `meo-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/
--rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-06-24 09:52:08.000000 meo-0.1.0/LICENSE
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-24 11:34:12.412438 meo-0.1.0/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-06-24 09:52:08.000000 meo-0.1.0/README.md
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/meo/
--rw-r--r--   0 meo       (1000) meo       (1000)      127 2023-06-24 10:23:38.000000 meo-0.1.0/meo/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)      300 2023-06-24 11:31:33.000000 meo-0.1.0/meo/__version__.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/meo/crack/
--rw-r--r--   0 meo       (1000) meo       (1000)     4164 2023-06-24 11:27:45.000000 meo-0.1.0/meo/crack/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)        0 2023-06-24 11:23:59.000000 meo-0.1.0/meo/crack/zip.py
--rw-r--r--   0 meo       (1000) meo       (1000)     1492 2023-06-24 09:52:08.000000 meo-0.1.0/meo/data.py
--rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-06-24 09:52:08.000000 meo-0.1.0/meo/flask.py
--rw-r--r--   0 meo       (1000) meo       (1000)      814 2023-06-24 09:52:08.000000 meo-0.1.0/meo/net.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-06-24 10:20:41.000000 meo-0.1.0/meo/screen.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/meo/sound/
--rw-r--r--   0 meo       (1000) meo       (1000)      980 2023-06-24 09:52:08.000000 meo-0.1.0/meo/sound/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)      167 2023-06-24 09:52:08.000000 meo-0.1.0/meo/utils.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/meo.egg-info/
--rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-24 11:34:12.000000 meo-0.1.0/meo.egg-info/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      324 2023-06-24 11:34:12.000000 meo-0.1.0/meo.egg-info/SOURCES.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-06-24 11:34:12.000000 meo-0.1.0/meo.egg-info/dependency_links.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-06-24 11:34:12.000000 meo-0.1.0/meo.egg-info/top_level.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-06-24 11:34:12.412438 meo-0.1.0/setup.cfg
--rwxr-xr-x   0 meo       (1000) meo       (1000)     1024 2023-06-24 11:23:01.000000 meo-0.1.0/setup.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/test/
--rw-r--r--   0 meo       (1000) meo       (1000)       56 2023-06-24 10:34:35.000000 meo-0.1.0/test/test-read.py
--rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-06-24 10:57:51.000000 meo-0.1.0/test/test.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 12:07:38.089032 meo-0.1.1/
+-rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-06-24 09:52:08.000000 meo-0.1.1/LICENSE
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-24 12:07:38.089032 meo-0.1.1/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-06-24 09:52:08.000000 meo-0.1.1/README.md
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 12:07:38.085699 meo-0.1.1/meo/
+-rw-r--r--   0 meo       (1000) meo       (1000)      125 2023-06-24 12:03:20.000000 meo-0.1.1/meo/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      300 2023-06-24 12:05:02.000000 meo-0.1.1/meo/__version__.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 12:07:38.085699 meo-0.1.1/meo/crack/
+-rw-r--r--   0 meo       (1000) meo       (1000)     4164 2023-06-24 11:27:45.000000 meo-0.1.1/meo/crack/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)        0 2023-06-24 11:23:59.000000 meo-0.1.1/meo/crack/zip.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-06-24 09:52:08.000000 meo-0.1.1/meo/flask.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2220 2023-06-24 11:57:52.000000 meo-0.1.1/meo/io.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      814 2023-06-24 09:52:08.000000 meo-0.1.1/meo/net.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-06-24 10:20:41.000000 meo-0.1.1/meo/screen.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      167 2023-06-24 09:52:08.000000 meo-0.1.1/meo/utils.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 12:07:38.085699 meo-0.1.1/meo.egg-info/
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-24 12:07:37.000000 meo-0.1.1/meo.egg-info/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      326 2023-06-24 12:07:38.000000 meo-0.1.1/meo.egg-info/SOURCES.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-06-24 12:07:37.000000 meo-0.1.1/meo.egg-info/dependency_links.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       11 2023-06-24 12:07:37.000000 meo-0.1.1/meo.egg-info/requires.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-06-24 12:07:37.000000 meo-0.1.1/meo.egg-info/top_level.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-06-24 12:07:38.089032 meo-0.1.1/setup.cfg
+-rwxr-xr-x   0 meo       (1000) meo       (1000)     1314 2023-06-24 12:07:31.000000 meo-0.1.1/setup.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 12:07:38.085699 meo-0.1.1/test/
+-rw-r--r--   0 meo       (1000) meo       (1000)       56 2023-06-24 10:34:35.000000 meo-0.1.1/test/test-read.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-06-24 10:57:51.000000 meo-0.1.1/test/test.py
```

### Comparing `meo-0.1.0/LICENSE` & `meo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meo-0.1.0/PKG-INFO` & `meo-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.0
+Version: 0.1.1
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.0/meo/crack/__init__.py` & `meo-0.1.1/meo/crack/__init__.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.0/meo/data.py` & `meo-0.1.1/meo/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,72 @@
 """ IO of formatted file and object """
+import json5
 import json
 import os
 
-
 def checkout_dir(dir_path):
     """Create if the folder does not exist"""
     if not os.path.exists(dir_path):
         os.makedirs(dir_path)
 
-def _checkout_file_path(path):
+def __checkout_file_path(path):
     fdir, _ = os.path.split(path)
     checkout_dir(fdir)
 
+def to_json5(obj, path: str, encoding='utf8', ensure_ascii=False, indent=None, auto_mkdirs=True):
+    if auto_mkdirs:
+        __checkout_file_path(path)
+    with open(path, 'w+', encoding=encoding) as _f:
+        json5.dump(obj, _f, ensure_ascii=ensure_ascii, indent=indent)
+
+def load_json5(path: str):
+    with open(path, 'rb') as _f:
+        return json5.load(_f)
 
 def to_json(obj, path: str, encoding='utf8', ensure_ascii=False, indent=None, auto_mkdirs=True):
     """ Serialize obj as a JSON formatted stream to ```path```` """
     if auto_mkdirs:
-        _checkout_file_path(path)
+        __checkout_file_path(path)
     with open(path, 'w+', encoding=encoding) as _f:
         json.dump(obj, _f, ensure_ascii=ensure_ascii, indent=indent)
 
-
-def to_file(path, data, mode='w+', encoding="utf8", auto_mkdirs=True):
-    """write file and auto create dir not existed """
-    if auto_mkdirs:
-        _checkout_file_path(path)
-    with open(path, mode, encoding=encoding) as _f:
-        return _f.write(data)
-
-
 def load_json(path: str):
     """ load json file from ```path``` """
     with open(path, 'rb') as _f:
         return json.load(_f)
 
+def to_file(path, data, mode='w+', encoding=..., auto_mkdirs=True):
+    """write file and auto create dir not existed """
+    if auto_mkdirs:
+        __checkout_file_path(path)
+    if 'b' in mode:
+        if encoding is ...:
+            encoding = None
+    elif encoding is ...:
+        encoding = 'utf8'
+    with open(path, mode, encoding=encoding) as _f:
+        return _f.write(data)
 
 def load_file(path, encoding=None):
     '''read file auto-closed'''
     with open(path, 'rb') as _f:
         content = _f.read()
+    if encoding is None:
+        return content
+    return content.decode(encoding=encoding)
 
-    if encoding:
-        return content.decode(encoding=encoding)
-    return content
-
-def decode(_bytes: bytes):
+def auto_decode(_bytes: bytes):
     """decide encoding and decode `_bytes`"""
     assert isinstance(_bytes, bytes)
     for encoding in ["utf8", 'gbk', 'utf16', 'utf32']:
         try:
             return _bytes.decode(encoding)
         except: pass
+    raise ValueError("bytes must be {utf8, gbk, utf16, utf32}")
+
+
+if __name__ == '__main__':
+    data = {
+        "test": 111
+    }
+    to_json(data, "./test/output.json")
+    to_json5(data, "./test/output.json5")
```

### Comparing `meo-0.1.0/meo/flask.py` & `meo-0.1.1/meo/flask.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.0/meo/net.py` & `meo-0.1.1/meo/net.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.0/meo/screen.py` & `meo-0.1.1/meo/screen.py`

 * *Files identical despite different names*

### Comparing `meo-0.1.0/meo.egg-info/PKG-INFO` & `meo-0.1.1/meo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meo
-Version: 0.1.0
+Version: 0.1.1
 Summary: frequently-used function library
 Home-page: http://github.com/miaobuao/meo
 Author: miaobuao
 Author-email: miaobuao@outlook.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `meo-0.1.0/setup.py` & `meo-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 #!/usr/bin/env python
 import os
 import shutil
 from setuptools import setup, find_packages
 
 CUR_PATH = os.path.dirname(os.path.abspath(__file__))
+path = os.path.join(CUR_PATH, "build")
+if os.path.isdir(path):
+    print("INFO DEL DIR ", path)
+    shutil.rmtree(path)
+path = os.path.join(CUR_PATH, "dist")
+if os.path.isdir(path):
+    print("INFO DEL DIR ", path)
+    shutil.rmtree(path)
 
 info = {}
 with open(os.path.join(CUR_PATH, "meo/__version__.py"), 'r+', encoding='utf8') as f:
     exec(f.read(), info)
 
 with open(os.path.join(CUR_PATH, "description.md"), 'r+', encoding='utf8') as f:
     long_description = f.read()
@@ -25,8 +33,11 @@
     long_description     = long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
+    install_requires=[
+        'json5>=0.9'
+    ],
 )
```

