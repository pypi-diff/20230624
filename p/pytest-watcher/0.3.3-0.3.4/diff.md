# Comparing `tmp/pytest_watcher-0.3.3.tar.gz` & `tmp/pytest_watcher-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_watcher-0.3.3.tar", max compression
+gzip compressed data, was "pytest_watcher-0.3.4.tar", max compression
```

## Comparing `pytest_watcher-0.3.3.tar` & `pytest_watcher-0.3.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/LICENSE
--rw-r--r--   0        0        0     4434 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/README.md
--rw-r--r--   0        0        0     1590 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       76 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pytest_watcher/__init__.py
--rw-r--r--   0        0        0       81 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pytest_watcher/__main__.py
--rw-r--r--   0        0        0     2393 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pytest_watcher/config.py
--rw-r--r--   0        0        0       56 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pytest_watcher/constants.py
--rw-r--r--   0        0        0     4885 2023-06-11 11:29:32.671647 pytest_watcher-0.3.3/pytest_watcher/watcher.py
--rw-r--r--   0        0        0     5533 1970-01-01 00:00:00.000000 pytest_watcher-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-24 15:13:34.648237 pytest_watcher-0.3.4/LICENSE
+-rw-r--r--   0        0        0     4447 2023-06-24 15:13:34.648237 pytest_watcher-0.3.4/README.md
+-rw-r--r--   0        0        0     1800 2023-06-24 15:13:34.652237 pytest_watcher-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-06-24 15:13:34.652237 pytest_watcher-0.3.4/pytest_watcher/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-24 15:13:34.652237 pytest_watcher-0.3.4/pytest_watcher/__main__.py
+-rw-r--r--   0        0        0     2379 2023-06-24 15:13:34.652237 pytest_watcher-0.3.4/pytest_watcher/config.py
+-rw-r--r--   0        0        0       56 2023-06-24 15:13:34.652237 pytest_watcher-0.3.4/pytest_watcher/constants.py
+-rw-r--r--   0        0        0     4885 2023-06-24 15:13:34.652237 pytest_watcher-0.3.4/pytest_watcher/watcher.py
+-rw-r--r--   0        0        0     5687 1970-01-01 00:00:00.000000 pytest_watcher-0.3.4/PKG-INFO
```

### Comparing `pytest_watcher-0.3.3/LICENSE` & `pytest_watcher-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_watcher-0.3.3/README.md` & `pytest_watcher-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 **pytest-watcher** is a tool to automatically rerun tests (using `pytest` by default) whenever your code changes.
 
 Works on Unix (Linux, MacOS, BSD) and Windows.
 
 Example:
 
-![Preview](preview.gif)
+![Preview](docs/_static/preview.gif)
 
 ## Table of contents
 
 - [Motivation](#motivation)
 - [File Events](#file-events)
 - [Installation](#installation)
 - [Usage](#usage)
```

### Comparing `pytest_watcher-0.3.3/pytest_watcher/config.py` & `pytest_watcher-0.3.4/pytest_watcher/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import List, Mapping, Optional
 
 from .constants import DEFAULT_DELAY
 
 try:
-    import tomlib
+    import tomllib
 except ImportError:
-    from pip._vendor import tomli as tomlib
+    import tomli as tomllib
 
 
 CONFIG_SECTION_NAME = "pytest-watcher"
 CLI_FIELDS = {"now", "delay", "runner", "patterns", "ignore_patterns"}
 CONFIG_FIELDS = CLI_FIELDS | {"runner_args"}
 
 
@@ -69,15 +69,15 @@
 
     return None
 
 
 def parse_config(path: Path) -> Mapping:
     with open(path, "rb") as f:
         try:
-            data = tomlib.load(f)
+            data = tomllib.load(f)
         except Exception as exc:
             raise SystemExit(f"Error parsing pyproject.toml\n{exc}")
 
     try:
         data = data["tool"][CONFIG_SECTION_NAME]
     except KeyError:
         return {}
```

### Comparing `pytest_watcher-0.3.3/pytest_watcher/watcher.py` & `pytest_watcher-0.3.4/pytest_watcher/watcher.py`

 * *Files identical despite different names*

### Comparing `pytest_watcher-0.3.3/PKG-INFO` & `pytest_watcher-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-watcher
-Version: 0.3.3
+Version: 0.3.4
 Summary: Automatically rerun your tests on file modifications
 Home-page: https://github.com/olzhasar/pytest-watcher
 License: MIT
 Keywords: pytest,watch,watcher
 Author: Olzhas Arystanov
 Author-email: o.arystanov@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -18,15 +18,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: watchdog (>=2.0.0)
+Project-URL: Documentation, https://pytest-watcher.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/olzhasar/pytest-watcher
 Description-Content-Type: text/markdown
 
 # Welcome to pytest-watcher
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-watcher)](https://pypi.org/project/pytest-watcher/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-watcher)](https://pypi.org/project/pytest-watcher/)
@@ -36,15 +38,15 @@
 
 **pytest-watcher** is a tool to automatically rerun tests (using `pytest` by default) whenever your code changes.
 
 Works on Unix (Linux, MacOS, BSD) and Windows.
 
 Example:
 
-![Preview](preview.gif)
+![Preview](docs/_static/preview.gif)
 
 ## Table of contents
 
 - [Motivation](#motivation)
 - [File Events](#file-events)
 - [Installation](#installation)
 - [Usage](#usage)
```

