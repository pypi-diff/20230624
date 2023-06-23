# Comparing `tmp/echolog-0.0.4.tar.gz` & `tmp/echolog-0.0.5.tar.gz`

## Comparing `echolog-0.0.4.tar` & `echolog-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10950 2020-02-02 00:00:00.000000 echolog-0.0.4/src/echolog/__init__.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 echolog-0.0.4/src/echolog/demo.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 echolog-0.0.4/LICENSE
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 echolog-0.0.4/README.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 echolog-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 echolog-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 echolog-0.0.5/src/echolog/__init__.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 echolog-0.0.5/src/echolog/demo.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 echolog-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 echolog-0.0.5/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 echolog-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 echolog-0.0.5/PKG-INFO
```

### Comparing `echolog-0.0.4/src/echolog/__init__.py` & `echolog-0.0.5/src/echolog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import re
 import inspect
 import logging
 from datetime import datetime
 
 try:
-    # REQUIRED (might make optional at some point) dependency: dotmap
+    # currently required dependency: dotmap
+    # (might make optional at some point)
     # nice dict wrapper class that allows calling entries as attributes OR keys
     # e.g. DotMap.entry is equivalent to DotMap['entry']
     from dotmap import DotMap
 
 except ModuleNotFoundError:
     raise ModuleNotFoundError("DotMap module not installed")
 
@@ -153,26 +154,26 @@
         # set up formatting strings
         if fmt in ['short', 'short-time']:
             __rename_logging_level_names(tags.short, values)
             
             if fmt == 'short':
                 fmt_str = f"[%(levelname)s]"
             else: # fmt == 'short-time'
-                fmt_str = f"%(asctime)s.%(msecs)3d [%(levelname)s]"
+                fmt_str = f"%(asctime)s.%(msecs)03d [%(levelname)s]"
         
         elif fmt in ['long', 'long-time']:
             
             if fmt == 'long':
                 fmt_str = f"%(levelname)s]"
                 for lvl, tag in tags.long.items():
                     tags.long[lvl] = '[' + tag
                     if len(tag) == 4:
                         tags.long[lvl] = ' ' + tags.long[lvl]
             else: # fmt == 'long-time'
-                fmt_str = f"[%(asctime)s.%(msecs)3d %(levelname)s]"
+                fmt_str = f"[%(asctime)s.%(msecs)03d %(levelname)s]"
                 for lvl, tag in tags.long.items():
                     if len(tag) == 4:
                         tags.long[lvl] = ' ' + tag
     
             __rename_logging_level_names(tags.long, values)
             
         else:
```

### Comparing `echolog-0.0.4/src/echolog/demo.py` & `echolog-0.0.5/src/echolog/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Runs a short demo.
 
 import logging
-from echolog import echo, get_logger, newline
+from __init__ import echo, get_logger, newline
 
 newline(3)
 
 for fmt in ['short-time', 'short', 'long-time', 'long']:
     log = get_logger(level=logging.DEBUG, fmt=fmt)
 
     echo(       f"Demo echo() call with   fmt={fmt}")
```

### Comparing `echolog-0.0.4/LICENSE` & `echolog-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `echolog-0.0.4/README.md` & `echolog-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `echolog-0.0.4/pyproject.toml` & `echolog-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "echolog"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="nerdpersonthing" },
 ]
 description = "A logging package that adds an echo() function to return both the input expression/variable and its results. Also sets up nicely-formatted logging."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `echolog-0.0.4/PKG-INFO` & `echolog-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolog
-Version: 0.0.4
+Version: 0.0.5
 Summary: A logging package that adds an echo() function to return both the input expression/variable and its results. Also sets up nicely-formatted logging.
 Project-URL: Homepage, https://github.com/nerdpersonthing/echolog
 Author: nerdpersonthing
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

