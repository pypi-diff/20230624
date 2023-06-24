# Comparing `tmp/quickpathstr-0.0.3.tar.gz` & `tmp/quickpathstr-0.0.4.tar.gz`

## Comparing `quickpathstr-0.0.3.tar` & `quickpathstr-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/quickpathstr/__init__.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/quickpathstr/quickpathstr.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/tests/test.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/LICENSE
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 quickpathstr-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 quickpathstr-0.0.4/info/LICENSE
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 quickpathstr-0.0.4/quickpathstr/__init__.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 quickpathstr-0.0.4/quickpathstr/quickpathstr.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 quickpathstr-0.0.4/quickpathstr/tests/test.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 quickpathstr-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 quickpathstr-0.0.4/../README.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 quickpathstr-0.0.4/PKG-INFO
```

### Comparing `quickpathstr-0.0.3/quickpathstr/quickpathstr.py` & `quickpathstr-0.0.4/quickpathstr/quickpathstr.py`

 * *Files identical despite different names*

### Comparing `quickpathstr-0.0.3/LICENSE` & `quickpathstr-0.0.4/info/LICENSE`

 * *Files identical despite different names*

### Comparing `quickpathstr-0.0.3/README.md` & `quickpathstr-0.0.4/../README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # QuickPathStr
-==============
 
 *Copyright (c) 2023 Sean Yeatts. All rights reserved.*
 
 This module provides syntax for working with strings in the context of file
 management. It's designed to reinforce a universal nomenclature by which files,
 their types, and their directories may be referred.
 
 ## API Reference
-----------------
 The core of the API is captured within the ```Filepath``` class:
 
 ```python
 class Filepath:
 # Deconstructs a complete filepath into its constituent elements
     def __init__(self, complete: str) -> None:
         self.complete   = complete                          # Ex: C:\Users\myself\Desktop\MyFile.txt
```

### Comparing `quickpathstr-0.0.3/pyproject.toml` & `quickpathstr-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "quickpathstr"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Sean Yeatts" },
 ]
 description = "Provides syntax for working with strings in the context of file management."
-readme = "README.md"
+readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `quickpathstr-0.0.3/PKG-INFO` & `quickpathstr-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: quickpathstr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Provides syntax for working with strings in the context of file management.
 Project-URL: GitHub, https://github.com/SeanYeatts/quickpathstr.git
 Author: Sean Yeatts
-License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # QuickPathStr
-==============
 
 *Copyright (c) 2023 Sean Yeatts. All rights reserved.*
 
 This module provides syntax for working with strings in the context of file
 management. It's designed to reinforce a universal nomenclature by which files,
 their types, and their directories may be referred.
 
 ## API Reference
-----------------
 The core of the API is captured within the ```Filepath``` class:
 
 ```python
 class Filepath:
 # Deconstructs a complete filepath into its constituent elements
     def __init__(self, complete: str) -> None:
         self.complete   = complete                          # Ex: C:\Users\myself\Desktop\MyFile.txt
```

