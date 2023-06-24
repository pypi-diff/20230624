# Comparing `tmp/morel-1.6.3.tar.gz` & `tmp/morel-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.6.3.tar", last modified: Sat Jun 24 11:15:01 2023, max compression
+gzip compressed data, was "morel-1.6.4.tar", last modified: Sat Jun 24 11:36:13 2023, max compression
```

## Comparing `morel-1.6.3.tar` & `morel-1.6.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 11:15:01.592637 morel-1.6.3/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.6.3/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-24 11:15:01.591637 morel-1.6.3/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.6.3/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-24 11:14:53.000000 morel-1.6.3/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-24 11:15:01.592637 morel-1.6.3/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 11:15:01.588637 morel-1.6.3/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 11:15:01.591637 morel-1.6.3/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.6.3/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     4043 2023-06-24 10:08:46.000000 morel-1.6.3/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.6.3/src/morel/exploit_template.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1022 2023-06-23 22:08:52.000000 morel-1.6.3/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.6.3/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.6.3/src/morel/singleton.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     4037 2023-06-24 11:14:43.000000 morel-1.6.3/src/morel/target.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.6.3/src/morel/target_template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 11:15:01.591637 morel-1.6.3/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-24 11:15:01.000000 morel-1.6.3/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-24 11:15:01.000000 morel-1.6.3/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-24 11:15:01.000000 morel-1.6.3/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-24 11:15:01.000000 morel-1.6.3/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-24 11:15:01.000000 morel-1.6.3/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-24 11:15:01.000000 morel-1.6.3/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 11:36:13.797007 morel-1.6.4/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.6.4/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-24 11:36:13.797007 morel-1.6.4/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.6.4/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-24 11:36:01.000000 morel-1.6.4/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-24 11:36:13.797007 morel-1.6.4/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 11:36:13.794007 morel-1.6.4/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 11:36:13.796007 morel-1.6.4/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.6.4/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     4043 2023-06-24 10:08:46.000000 morel-1.6.4/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.6.4/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1022 2023-06-23 22:08:52.000000 morel-1.6.4/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.6.4/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.6.4/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     4080 2023-06-24 11:33:47.000000 morel-1.6.4/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.6.4/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 11:36:13.797007 morel-1.6.4/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-24 11:36:13.000000 morel-1.6.4/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-24 11:36:13.000000 morel-1.6.4/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-24 11:36:13.000000 morel-1.6.4/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-24 11:36:13.000000 morel-1.6.4/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-24 11:36:13.000000 morel-1.6.4/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-24 11:36:13.000000 morel-1.6.4/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.6.3/LICENSE` & `morel-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.6.3/PKG-INFO` & `morel-1.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.6.3
+Version: 1.6.4
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.6.3/pyproject.toml` & `morel-1.6.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.6.3"
+version = "1.6.4"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.6.3/src/morel/app.py` & `morel-1.6.4/src/morel/app.py`

 * *Files identical despite different names*

### Comparing `morel-1.6.3/src/morel/exploit_template.py` & `morel-1.6.4/src/morel/exploit_template.py`

 * *Files identical despite different names*

### Comparing `morel-1.6.3/src/morel/exploits.py` & `morel-1.6.4/src/morel/exploits.py`

 * *Files identical despite different names*

### Comparing `morel-1.6.3/src/morel/singleton.py` & `morel-1.6.4/src/morel/singleton.py`

 * *Files identical despite different names*

### Comparing `morel-1.6.3/src/morel/target.py` & `morel-1.6.4/src/morel/target.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import importlib
-import _collections_abc
 import json
 from multiprocessing import Lock
 import sys
 from collections import UserDict
 from pathlib import Path
 import time
 from typing import Iterable
+from collections import OrderedDict
+
 
-from morel.singleton import SingletonMeta
 from morel.logger import logger
 
 
 class _restrictedDict(UserDict):
     def __init__(self, initialD={}):
         super().__init__(initialD)
 
@@ -28,30 +28,31 @@
         for k, v in dict2.items():
             if k not in self:
                 self[k] = v
                 continue
 
             if isinstance(self[k], dict) and not isinstance(self[k], _restrictedDict):
                 self[k] = _restrictedDict(self[k])
-            elif isinstance(self[k], list):
-                self[k] = set(self[k])
             elif not isinstance(self[k], Iterable):
-                self[k] = {
+                self[k] = [
                     self[k],
-                }
+                ]
 
             if isinstance(self[k], _restrictedDict):
-                if isinstance(v, dict):
+                self[k].append(v)
+            elif isinstance(self[k], list):
+                if isinstance(v, list):
+                    self[k].extend(v)
+                else:
                     self[k].append(v)
-                elif isinstance(v, list | set):
-                    self[k] = {self[k], v}
-            elif isinstance(self[k], set):
-                if isinstance(v, list):  # convert to set
-                    v = set(v)
-                self[k] |= v
+                self[k] = remove_duplicates(self[k])
+
+
+def remove_duplicates(l: list) -> list:
+    return list(OrderedDict((x, True) for x in l).keys())
 
 
 class _Targets(_restrictedDict):
     def __init__(self):
         super().__init__()
         self._lock = Lock()
         self.target_functions = []
@@ -103,15 +104,18 @@
                         target = function()
                         # self.log.debug(f"{target = }")
                     except Exception as e:
                         self.log.warning(
                             f"{function.__module__} raised an exception:\n{e}"
                         )
                     else:
-                        self.append(target)
+                        try:
+                            self.append(target)
+                        except Exception as e:
+                            raise e
                     finally:
                         self.last_update = time.time()
         return
 
 
 Targets = _Targets()
```

### Comparing `morel-1.6.3/src/morel.egg-info/PKG-INFO` & `morel-1.6.4/src/morel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.6.3
+Version: 1.6.4
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

