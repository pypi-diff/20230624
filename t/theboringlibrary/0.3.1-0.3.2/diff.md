# Comparing `tmp/theboringlibrary-0.3.1.tar.gz` & `tmp/theboringlibrary-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theboringlibrary-0.3.1.tar", max compression
+gzip compressed data, was "theboringlibrary-0.3.2.tar", max compression
```

## Comparing `theboringlibrary-0.3.1.tar` & `theboringlibrary-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-24 14:34:02.523634 theboringlibrary-0.3.1/LICENSE
--rw-r--r--   0        0        0       37 2023-06-24 14:34:02.523634 theboringlibrary-0.3.1/README.md
--rw-r--r--   0        0        0      526 2023-06-24 14:34:02.527634 theboringlibrary-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-24 14:34:02.527634 theboringlibrary-0.3.1/src/theboringlibrary/__init__.py
--rw-r--r--   0        0        0      121 2023-06-24 14:34:02.527634 theboringlibrary-0.3.1/src/theboringlibrary/core.py
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 theboringlibrary-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-24 20:06:37.336862 theboringlibrary-0.3.2/LICENSE
+-rw-r--r--   0        0        0       37 2023-06-24 20:06:37.336862 theboringlibrary-0.3.2/README.md
+-rw-r--r--   0        0        0      526 2023-06-24 20:06:37.336862 theboringlibrary-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-24 20:06:37.336862 theboringlibrary-0.3.2/src/theboringlibrary/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-24 20:06:37.336862 theboringlibrary-0.3.2/src/theboringlibrary/core.py
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 theboringlibrary-0.3.2/PKG-INFO
```

### Comparing `theboringlibrary-0.3.1/LICENSE` & `theboringlibrary-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `theboringlibrary-0.3.1/pyproject.toml` & `theboringlibrary-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "theboringlibrary"
-version = "0.3.1"
+version = "0.3.2"
 description = "It does nothing!"
 authors = ["Stefano Frassetto <frassetto.stefano@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "theboringlibrary", from = "src" }
 ]
```

### Comparing `theboringlibrary-0.3.1/PKG-INFO` & `theboringlibrary-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theboringlibrary
-Version: 0.3.1
+Version: 0.3.2
 Summary: It does nothing!
 Author: Stefano Frassetto
 Author-email: frassetto.stefano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

