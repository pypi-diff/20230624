# Comparing `tmp/ngpa-0.0.1.tar.gz` & `tmp/ngpa-0.0.2.tar.gz`

## Comparing `ngpa-0.0.1.tar` & `ngpa-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ngpa-0.0.1/ngpa/__init__.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 ngpa-0.0.1/ngpa/ngpa.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ngpa-0.0.1/.gitignore
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 ngpa-0.0.1/LICENSE
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ngpa-0.0.1/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ngpa-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 ngpa-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ngpa-0.0.2/ngpa/__init__.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 ngpa-0.0.2/ngpa/ngpa.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ngpa-0.0.2/.gitignore
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 ngpa-0.0.2/LICENSE
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ngpa-0.0.2/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ngpa-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 ngpa-0.0.2/PKG-INFO
```

### Comparing `ngpa-0.0.1/ngpa/ngpa.py` & `ngpa-0.0.2/ngpa/ngpa.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   Returns:
       list[Course]: a list of Course
   """
   with open(f, mode='r', encoding='utf-8'):
     return courses_from_fd(f)
 
 def courses_from_stdin() -> list[Course]:
-  """almost the same function as `credits_from_file` except reading from stdin
+  """almost the same function as `courses_from_file` except reading from stdin
 
   Returns:
       list[Course]: a list of Course
   """
   from sys import stdin
   return courses_from_fd(stdin)
```

### Comparing `ngpa-0.0.1/LICENSE` & `ngpa-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ngpa-0.0.1/pyproject.toml` & `ngpa-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "ngpa"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = 'DingZhen', email = "realdingzhen@outlook.com" }]
 description = "Some handy functions for computing NJU gpa"
 requires-python = ">=3.5"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ngpa-0.0.1/PKG-INFO` & `ngpa-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngpa
-Version: 0.0.1
+Version: 0.0.2
 Summary: Some handy functions for computing NJU gpa
 Project-URL: Homepage, https://github.com/UshioA/ngpa
 Project-URL: Bug Track, https://github.com/UshioA/ngpa/issues
 Author-email: DingZhen <realdingzhen@outlook.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

