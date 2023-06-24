# Comparing `tmp/sdp_transform-1.0.5.tar.gz` & `tmp/sdp_transform-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdp_transform-1.0.5.tar", max compression
+gzip compressed data, was "sdp_transform-1.0.6.tar", max compression
```

## Comparing `sdp_transform-1.0.5.tar` & `sdp_transform-1.0.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-03-21 09:31:57.405028 sdp_transform-1.0.5/LICENSE
--rw-r--r--   0        0        0      345 2023-03-21 10:02:47.514748 sdp_transform-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      113 2023-03-21 09:56:07.874815 sdp_transform-1.0.5/sdp_transform/__init__.py
--rw-r--r--   0        0        0       66 2023-03-21 10:02:29.104741 sdp_transform-1.0.5/sdp_transform/__version__.py
--rw-r--r--   0        0        0    18198 2023-03-21 10:02:29.234741 sdp_transform-1.0.5/sdp_transform/grammar.py
--rw-r--r--   0        0        0     3275 2023-03-21 10:02:29.154741 sdp_transform-1.0.5/sdp_transform/parser.py
--rw-r--r--   0        0        0     2793 2023-03-21 10:02:29.154741 sdp_transform-1.0.5/sdp_transform/writer.py
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 sdp_transform-1.0.5/setup.py
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 sdp_transform-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-24 11:30:55.940385 sdp_transform-1.0.6/LICENSE
+-rw-r--r--   0        0        0      345 2023-06-24 11:31:18.163274 sdp_transform-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-06-24 11:30:55.940674 sdp_transform-1.0.6/sdp_transform/__init__.py
+-rw-r--r--   0        0        0       66 2023-06-24 11:31:50.012658 sdp_transform-1.0.6/sdp_transform/__version__.py
+-rw-r--r--   0        0        0    18198 2023-06-24 11:30:55.940914 sdp_transform-1.0.6/sdp_transform/grammar.py
+-rw-r--r--   0        0        0     3275 2023-06-24 11:30:55.941035 sdp_transform-1.0.6/sdp_transform/parser.py
+-rw-r--r--   0        0        0     2796 2023-06-24 11:30:55.941111 sdp_transform-1.0.6/sdp_transform/writer.py
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 sdp_transform-1.0.6/PKG-INFO
```

### Comparing `sdp_transform-1.0.5/LICENSE` & `sdp_transform-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sdp_transform-1.0.5/sdp_transform/grammar.py` & `sdp_transform-1.0.6/sdp_transform/grammar.py`

 * *Files identical despite different names*

### Comparing `sdp_transform-1.0.5/sdp_transform/parser.py` & `sdp_transform-1.0.6/sdp_transform/parser.py`

 * *Files identical despite different names*

### Comparing `sdp_transform-1.0.5/sdp_transform/writer.py` & `sdp_transform-1.0.6/sdp_transform/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     if session.get("version") == None:
         session["version"] = 0  # 'v=0' must be there (only defined version atm)
     if session.get("name") == None:
         session["name"] = " "  # 's= ' must be there if no meaningful name set
 
     for media in session.get("media", []):
         if media.get("payloads") == None:
-            media.payloads = ""
+            media["payloads"] = ""
 
     sdp = []
 
     # loop through outerOrder for matching properties on session
     for field in outerOrder:
         for obj in grammar[field]:
             if obj.get("name"):
```

### Comparing `sdp_transform-1.0.5/PKG-INFO` & `sdp_transform-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdp-transform
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple Python parser and writer of SDP.
 License: MIT
 Author: Jiang Yue
 Author-email: maze1024@gmail.com
 Requires-Python: >=3.6.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

