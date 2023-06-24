# Comparing `tmp/spyder_line_profiler-0.3.1.tar.gz` & `tmp/spyder_line_profiler-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyder_line_profiler-0.3.1.tar", last modified: Sun Aug  7 19:32:35 2022, max compression
+gzip compressed data, was "spyder_line_profiler-0.3.2.tar", last modified: Fri Jun 23 21:13:45 2023, max compression
```

## Comparing `spyder_line_profiler-0.3.1.tar` & `spyder_line_profiler-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-08-07 19:32:35.982733 spyder_line_profiler-0.3.1/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      481 2022-06-03 21:23:40.000000 spyder_line_profiler-0.3.1/AUTHORS.md
--rw-r--r--   0 jitse     (1000) jitse     (1000)     5742 2022-08-07 19:09:42.000000 spyder_line_profiler-0.3.1/CHANGELOG.md
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1094 2022-06-03 21:21:29.000000 spyder_line_profiler-0.3.1/LICENSE.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)       84 2022-06-03 21:21:29.000000 spyder_line_profiler-0.3.1/MANIFEST.in
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1655 2022-08-07 19:32:35.982733 spyder_line_profiler-0.3.1/PKG-INFO
--rwxr-xr-x   0 jitse     (1000) jitse     (1000)     3339 2022-06-03 21:23:40.000000 spyder_line_profiler-0.3.1/README.md
--rw-r--r--   0 jitse     (1000) jitse     (1000)       38 2022-08-07 19:32:35.982733 spyder_line_profiler-0.3.1/setup.cfg
--rw-r--r--   0 jitse     (1000) jitse     (1000)     3307 2022-06-03 21:23:40.000000 spyder_line_profiler-0.3.1/setup.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-08-07 19:32:35.978733 spyder_line_profiler-0.3.1/spyder_line_profiler/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      341 2022-08-07 19:31:19.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/__init__.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-08-07 19:32:35.978733 spyder_line_profiler-0.3.1/spyder_line_profiler/example/
--rw-r--r--   0 jitse     (1000) jitse     (1000)        0 2022-06-03 21:21:29.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/example/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1001 2022-08-07 19:03:05.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/example/profiling_test_script.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-08-07 19:32:35.982733 spyder_line_profiler-0.3.1/spyder_line_profiler/example/subdir/
--rw-r--r--   0 jitse     (1000) jitse     (1000)        0 2022-06-03 21:21:29.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/example/subdir/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)      497 2022-06-03 21:21:29.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/example/subdir/profiling_test_script2.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-08-07 19:32:35.982733 spyder_line_profiler-0.3.1/spyder_line_profiler/spyder/
--rw-r--r--   0 jitse     (1000) jitse     (1000)      314 2022-06-03 21:23:40.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/spyder/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)      910 2022-06-03 21:23:40.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/spyder/config.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2250 2022-06-03 21:23:40.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/spyder/confpage.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     4811 2022-06-03 21:23:40.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/spyder/plugin.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)    29755 2022-08-07 19:02:54.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/spyder/widgets.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-08-07 19:32:35.982733 spyder_line_profiler-0.3.1/spyder_line_profiler/tests/
--rw-r--r--   0 jitse     (1000) jitse     (1000)        0 2022-06-03 21:23:40.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/tests/__init__.py
--rw-r--r--   0 jitse     (1000) jitse     (1000)     2007 2022-06-03 21:23:40.000000 spyder_line_profiler-0.3.1/spyder_line_profiler/tests/test_lineprofiler.py
-drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2022-08-07 19:32:35.978733 spyder_line_profiler-0.3.1/spyder_line_profiler.egg-info/
--rw-r--r--   0 jitse     (1000) jitse     (1000)     1655 2022-08-07 19:32:35.000000 spyder_line_profiler-0.3.1/spyder_line_profiler.egg-info/PKG-INFO
--rw-r--r--   0 jitse     (1000) jitse     (1000)      852 2022-08-07 19:32:35.000000 spyder_line_profiler-0.3.1/spyder_line_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)        1 2022-08-07 19:32:35.000000 spyder_line_profiler-0.3.1/spyder_line_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)       95 2022-08-07 19:32:35.000000 spyder_line_profiler-0.3.1/spyder_line_profiler.egg-info/entry_points.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)       36 2022-08-07 19:32:35.000000 spyder_line_profiler-0.3.1/spyder_line_profiler.egg-info/requires.txt
--rw-r--r--   0 jitse     (1000) jitse     (1000)       21 2022-08-07 19:32:35.000000 spyder_line_profiler-0.3.1/spyder_line_profiler.egg-info/top_level.txt
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-06-23 21:13:45.790435 spyder_line_profiler-0.3.2/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      358 2023-06-10 16:07:14.000000 spyder_line_profiler-0.3.2/AUTHORS.md
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     7413 2023-06-23 20:58:44.000000 spyder_line_profiler-0.3.2/CHANGELOG.md
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1094 2023-05-04 17:48:51.000000 spyder_line_profiler-0.3.2/LICENSE.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       84 2023-05-04 17:48:51.000000 spyder_line_profiler-0.3.2/MANIFEST.in
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1632 2023-06-23 21:13:45.786435 spyder_line_profiler-0.3.2/PKG-INFO
+-rwxr-xr-x   0 jitse     (1000) jitse     (1000)     3339 2023-05-04 17:48:51.000000 spyder_line_profiler-0.3.2/README.md
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       38 2023-06-23 21:13:45.790435 spyder_line_profiler-0.3.2/setup.cfg
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     3503 2023-06-23 20:25:34.000000 spyder_line_profiler-0.3.2/setup.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-06-23 21:13:45.786435 spyder_line_profiler-0.3.2/spyder_line_profiler/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      400 2023-06-23 21:05:17.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/__init__.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-06-23 21:13:45.786435 spyder_line_profiler-0.3.2/spyder_line_profiler/example/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)        0 2023-05-04 17:48:51.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/example/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1244 2023-06-10 16:07:14.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/example/profiling_test_script.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-06-23 21:13:45.786435 spyder_line_profiler-0.3.2/spyder_line_profiler/example/subdir/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)        0 2023-05-04 17:48:51.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/example/subdir/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      740 2023-06-10 16:07:14.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/example/subdir/profiling_test_script2.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-06-23 21:13:45.786435 spyder_line_profiler-0.3.2/spyder_line_profiler/spyder/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      379 2023-06-10 16:07:14.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/spyder/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1102 2023-06-10 16:07:14.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/spyder/config.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2311 2023-06-10 16:07:14.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/spyder/confpage.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     4496 2023-06-23 20:25:34.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/spyder/plugin.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)    29445 2023-06-23 20:25:34.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/spyder/widgets.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-06-23 21:13:45.786435 spyder_line_profiler-0.3.2/spyder_line_profiler/tests/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)        0 2023-05-04 17:48:51.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/tests/__init__.py
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     2471 2023-06-10 16:07:14.000000 spyder_line_profiler-0.3.2/spyder_line_profiler/tests/test_lineprofiler.py
+drwxr-xr-x   0 jitse     (1000) jitse     (1000)        0 2023-06-23 21:13:45.786435 spyder_line_profiler-0.3.2/spyder_line_profiler.egg-info/
+-rw-r--r--   0 jitse     (1000) jitse     (1000)     1632 2023-06-23 21:13:45.000000 spyder_line_profiler-0.3.2/spyder_line_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 jitse     (1000) jitse     (1000)      852 2023-06-23 21:13:45.000000 spyder_line_profiler-0.3.2/spyder_line_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)        1 2023-06-23 21:13:45.000000 spyder_line_profiler-0.3.2/spyder_line_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       94 2023-06-23 21:13:45.000000 spyder_line_profiler-0.3.2/spyder_line_profiler.egg-info/entry_points.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       41 2023-06-23 21:13:45.000000 spyder_line_profiler-0.3.2/spyder_line_profiler.egg-info/requires.txt
+-rw-r--r--   0 jitse     (1000) jitse     (1000)       21 2023-06-23 21:13:45.000000 spyder_line_profiler-0.3.2/spyder_line_profiler.egg-info/top_level.txt
```

### Comparing `spyder_line_profiler-0.3.1/CHANGELOG.md` & `spyder_line_profiler-0.3.2/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # History of changes
 
+## Version 0.3.2 (2023/06/24)
+
+This version contains some bug fixes and is compatible with Spyder 5.4.
+
+### Bug fixes
+
+* Use Python interpreter/environment from Preferences ([Issue 67](https://github.com/spyder-ide/spyder-line-profiler/issues/67), [Issue 5](https://github.com/spyder-ide/spyder-line-profiler/issues/5), [PR 78](https://github.com/spyder-ide/spyder-line-profiler/pull/78))
+* Adapt colors to Spyder's palette ([Issue 50](https://github.com/spyder-ide/spyder-line-profiler/issues/50), [PR 82](https://github.com/spyder-ide/spyder-line-profiler/pull/82))
+* Update LICENSE.txt to match individual file copyright statements ([Issue 74](https://github.com/spyder-ide/spyder-line-profiler/issues/74), [PR 79](https://github.com/spyder-ide/spyder-line-profiler/pull/79))
+* Update description on PyPI ([Issue 73](https://github.com/spyder-ide/spyder-line-profiler/issues/73), [PR 83](https://github.com/spyder-ide/spyder-line-profiler/pull/83))
+
+### Maintenance
+
+* Updates for Spyder 5.4 ([Issue 80](https://github.com/spyder-ide/spyder-line-profiler/issues/80), [Issue 72](https://github.com/spyder-ide/spyder-line-profiler/issues/72), [PR 77](https://github.com/spyder-ide/spyder-line-profiler/pull/77), [PR 84](https://github.com/spyder-ide/spyder-line-profiler/pull/84))
+* Remove last bits of Python 2 support ([PR 68](https://github.com/spyder-ide/spyder-line-profiler/pull/68))
+* Update test for line_profiler 4.x ([Issue 75](https://github.com/spyder-ide/spyder-line-profiler/issues/75), [PR 68](https://github.com/spyder-ide/spyder-line-profiler/pull/68))
+* Update GitHub test action ([PR 76](https://github.com/spyder-ide/spyder-line-profiler/pull/76))
+
+
 ## Version 0.3.1 (2022/08/07)
 
 This version fixes a compatibility issue with Spyder 5.3.2 ([Issue 65](https://github.com/spyder-ide/spyder-line-profiler/issues/65), [PR 66](https://github.com/spyder-ide/spyder-line-profiler/pull/66)).
 
 
 ## Version 0.3.0 (2022/06/03)
```

### Comparing `spyder_line_profiler-0.3.1/LICENSE.txt` & `spyder_line_profiler-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spyder_line_profiler-0.3.1/PKG-INFO` & `spyder_line_profiler-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: spyder_line_profiler
-Version: 0.3.1
+Version: 0.3.2
 Summary: Plugin for the Spyder 5 IDE that integrates the Python line profiler.
 Home-page: https://github.com/spyder-ide/spyder-line-profiler
 Author: Spyder Project Contributors
 License: MIT
 Keywords: Qt PyQt5 PySide2 spyder plugins spyplugins line_profiler profiler
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +28,13 @@
 It allows you to see the time spent in every line.
 
 Usage
 -----
 
 Add a ``@profile`` decorator to the functions that you wish to profile
 then press Shift+F10 (line profiler default) to run the profiler on
-the current script, or go to ``Run > Profile line by line``.
+the current script, or go to ``Run > Run line profiler``.
 
 The results will be shown in a dockwidget, grouped by function. Lines
 with a stronger color take more time to run.
 
 .. image: https://raw.githubusercontent.com/spyder-ide/spyder-line-profiler/master/img_src/screenshot_profiler.png
-
-
```

### Comparing `spyder_line_profiler-0.3.1/README.md` & `spyder_line_profiler-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `spyder_line_profiler-0.3.1/setup.py` & `spyder_line_profiler-0.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2022 Spyder Project Contributors
-# Licensed under the terms of the MIT License
-# (see LICENSE.txt for details)
+# -----------------------------------------------------------------------------
+# Copyright (c) 2015- Spyder Project Contributors
+#
+# Released under the terms of the MIT License
+# (see LICENSE.txt in the project root directory for details)
+# -----------------------------------------------------------------------------
 
 """
 Setup script for spyder_line_profiler
 """
 
 from setuptools import setup, find_packages
 import os
@@ -34,29 +37,29 @@
         for fname in filenames:
             if not fname.startswith('.') and osp.splitext(fname)[1] in extlist:
                 flist.append(osp.join(dirpath, fname)[offset:])
     return flist
 
 
 # Requirements
-REQUIREMENTS = ['line_profiler', 'qtawesome', 'spyder>=5.2']
+REQUIREMENTS = ['line_profiler', 'qtawesome', 'spyder>=5.4.1,<6']
 EXTLIST = ['.jpg', '.png', '.json', '.mo', '.ini']
 LIBNAME = 'spyder_line_profiler'
 
 
 LONG_DESCRIPTION = """
 This is a plugin for the Spyder 5 IDE that integrates the Python line profiler.
 It allows you to see the time spent in every line.
 
 Usage
 -----
 
 Add a ``@profile`` decorator to the functions that you wish to profile
 then press Shift+F10 (line profiler default) to run the profiler on
-the current script, or go to ``Run > Profile line by line``.
+the current script, or go to ``Run > Run line profiler``.
 
 The results will be shown in a dockwidget, grouped by function. Lines
 with a stronger color take more time to run.
 
 .. image: https://raw.githubusercontent.com/spyder-ide/spyder-line-profiler/master/img_src/screenshot_profiler.png
 """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spyder_line_profiler-0.3.1/spyder_line_profiler/example/profiling_test_script.py` & `spyder_line_profiler-0.3.2/spyder_line_profiler/example/subdir/profiling_test_script2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,31 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
-u"""
-:author: Joseph Martinot-Lagarde
-
-Created on Sat Jan 19 14:57:57 2013
-"""
+#
+# -----------------------------------------------------------------------------
+# Copyright (c) 2013- Spyder Project Contributors
+#
+# Released under the terms of the MIT License
+# (see LICENSE.txt in the project root directory for details)
+# -----------------------------------------------------------------------------
 
 from __future__ import (
     print_function, division, unicode_literals, absolute_import)
 
 
-import subdir.profiling_test_script2 as script2
-
-
 @profile
-def fact(n):
-    result = 1
-    for i in range(2, n // 4):
-        result *= i
-    result = 1
-    # This is a comment
-    for i in range(2, n // 16):
-        result *= i
+def fact2(n):
     result = 1
-
-    if False:
-        # This won't be run
-        raise RuntimeError("What are you doing here ???")
-
     for i in range(2, n + 1):
-        result *= i
+        result *= i * 2
     return result
-    # This is after the end of the function.
-
-    if False:
-        # This won't be run
-        raise RuntimeError("It's getting bad.")
 
 
-@profile
-def sum_(n):
+def sum2(n):
     result = 0
-
     for i in range(1, n + 1):
-        result += i
+        result += i * 2
     return result
 
 if __name__ == "__main__":
-    print(fact(120))
-    print(sum_(120))
-    print(script2.fact2(120))
-    print(script2.sum2(120))
+    print(fact2(120))
+    print(sum2(120))
```

### Comparing `spyder_line_profiler-0.3.1/spyder_line_profiler/spyder/confpage.py` & `spyder_line_profiler-0.3.2/spyder_line_profiler/spyder/confpage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
-# ----------------------------------------------------------------------------
-# Copyright © 2021, Spyder Line Profiler contributors
 #
-# Licensed under the terms of the MIT license
-# ----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
+# Copyright (c) 2013- Spyder Project Contributors
+#
+# Released under the terms of the MIT License
+# (see LICENSE.txt in the project root directory for details)
+# -----------------------------------------------------------------------------
 
 """
 Spyder Line Profiler 5 Preferences Page.
 """
 
 # Third party imports
 from qtpy.QtCore import Qt
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spyder_line_profiler-0.3.1/spyder_line_profiler/spyder/plugin.py` & `spyder_line_profiler-0.3.2/spyder_line_profiler/spyder/plugin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 # -*- coding: utf-8 -*-
-# ----------------------------------------------------------------------------
-# Copyright © 2021, Spyder Line Profiler contributors
 #
-# Licensed under the terms of the MIT license
-# ----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
+# Copyright (c) 2013- Spyder Project Contributors
+#
+# Released under the terms of the MIT License
+# (see LICENSE.txt in the project root directory for details)
+# -----------------------------------------------------------------------------
 
 """
-Spyder Line Profiler 5 Plugin.
+Spyder Line Profiler Plugin.
 """
 
-# Standard library imports
-import os.path as osp
-
 # Third-party imports
+import qtawesome as qta
 from qtpy.QtCore import Qt, Signal
-from qtpy.QtGui import QIcon
+
+# Spyder imports
 from spyder.api.plugins import Plugins, SpyderDockablePlugin
 from spyder.api.translations import get_translation
-from spyder.api.plugin_registration.decorators import on_plugin_available
-from spyder.api.plugin_registration.decorators import on_plugin_teardown
+from spyder.api.plugin_registration.decorators import (
+    on_plugin_available, on_plugin_teardown)
 from spyder.plugins.mainmenu.api import ApplicationMenus
 from spyder.utils.icon_manager import ima
-import qtawesome as qta
 
 # Local imports
 from spyder_line_profiler.spyder.config import (
     CONF_SECTION, CONF_DEFAULTS, CONF_VERSION)
 from spyder_line_profiler.spyder.confpage import SpyderLineProfilerConfigPage
-from spyder_line_profiler.spyder.widgets import SpyderLineProfilerWidget
-from spyder_line_profiler.spyder.widgets import is_lineprofiler_installed
+from spyder_line_profiler.spyder.widgets import (
+    SpyderLineProfilerWidget, is_lineprofiler_installed)
 
 # Localization
 _ = get_translation("spyder_line_profiler.spyder")
 
 
 class SpyderLineProfilerActions:
     # Triggers
-    Run = 'run_profiler_action'
+    Run = 'Run file in spyder_line_profiler'
 
 
 class SpyderLineProfiler(SpyderDockablePlugin):
     """
     Spyder Line Profiler plugin for Spyder 5.
     """
 
@@ -95,48 +95,42 @@
 
     @on_plugin_teardown(plugin=Plugins.MainMenu)
     def on_main_menu_teardown(self):
         mainmenu = self.get_plugin(Plugins.MainMenu)
         mainmenu.remove_item_from_application_menu(
             SpyderLineProfilerActions.Run,
             menu_id=ApplicationMenus.Run
-        )
+         )
 
     @on_plugin_available(plugin=Plugins.Preferences)
     def on_preferences_available(self):
         preferences = self.get_plugin(Plugins.Preferences)
         preferences.register_plugin_preferences(self)
 
+    @on_plugin_teardown(plugin=Plugins.Preferences)
+    def on_preferences_teardown(self):
+        preferences = self.get_plugin(Plugins.Preferences)
+        preferences.deregister_plugin_preferences(self)
+
     def check_compatibility(self):
         valid = True
         message = ""  # Note: Remember to use _("") to localize the string
         return valid, message
 
     def on_close(self, cancellable=True):
         return True
 
     # --- Public API
     # ------------------------------------------------------------------------
-    def update_pythonpath(self):
-        """
-        Update the PYTHONPATH used when running the line_profiler.
-
-        This function is called whenever the Python path set in Spyder changes.
-        It synchronizes the PYTHONPATH in the line_profiler widget with the
-        PYTHONPATH in Spyder.
-        """
-        self.widget.spyder_pythonpath = self.main.get_spyder_pythonpath()
 
     def run_lineprofiler(self):
         """Run line profiler."""
         editor = self.get_plugin(Plugins.Editor)
         if editor.save():
             self.switch_to_plugin()
             self.analyze(editor.get_current_filename())
 
-        self.analyze(self.main.editor.get_current_filename())
-
     def analyze(self, filename):
         """Analyze a file."""
         if self.dockwidget:
             self.switch_to_plugin()
         self.widget.analyze(filename=filename)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spyder_line_profiler-0.3.1/spyder_line_profiler/spyder/widgets.py` & `spyder_line_profiler-0.3.2/spyder_line_profiler/spyder/widgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,76 @@
 # -*- coding: utf-8 -*-
-# ----------------------------------------------------------------------------
-# Copyright © 2021, Spyder Line Profiler contributors
 #
-# Licensed under the terms of the MIT license
-# ----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
+# Copyright (c) 2013- Spyder Project Contributors
+#
+# Released under the terms of the MIT License
+# (see LICENSE.txt in the project root directory for details)
+# -----------------------------------------------------------------------------
 """
 Spyder Line Profiler Main Widget.
 """
 # Standard library imports
-import hashlib
 import inspect
 import linecache
-import re
+import logging
 import os
 import os.path as osp
+import pickle
+import re
 import time
 from datetime import datetime
 
 # Third party imports
 from qtpy.QtGui import QBrush, QColor, QFont
 from qtpy.QtCore import (QByteArray, QProcess, Qt, QTextCodec,
                          QProcessEnvironment, Signal, QTimer)
 from qtpy.QtWidgets import (QMessageBox, QVBoxLayout, QLabel,
                             QTreeWidget, QTreeWidgetItem, QApplication)
 from qtpy.compat import getopenfilename, getsavefilename
 
 # Spyder imports
 from spyder.api.config.decorators import on_conf_change
 from spyder.api.translations import get_translation
+from spyder.api.widgets.main_widget import PluginMainWidget
 from spyder.config.base import get_conf_path
 from spyder.plugins.variableexplorer.widgets.texteditor import TextEditor
-from spyder.api.widgets.main_widget import PluginMainWidget
-from spyder.widgets.comboboxes import PythonModulesComboBox
+from spyder.plugins.run.widgets import get_run_configuration
 from spyder.utils import programs
 from spyder.utils.misc import getcwd_or_home
-from spyder.plugins.run.widgets import get_run_configuration
-from spyder.py3compat import to_text_string, pickle
+from spyder.utils.palette import SpyderPalette
+from spyder.widgets.comboboxes import PythonModulesComboBox
 
 # Local imports
 from spyder_line_profiler.spyder.config import CONF_SECTION
 
-# Localization
+# Localization and logging
 _ = get_translation("spyder")
-
+logger = logging.getLogger(__name__)
 
 COL_NO = 0
 COL_HITS = 1
 COL_TIME = 2
 COL_PERHIT = 3
 COL_PERCENT = 4
 COL_LINE = 5
 COL_POS = 0  # Position is not displayed but set as Qt.UserRole
 
 CODE_NOT_RUN_COLOR = QBrush(QColor.fromRgb(128, 128, 128, 200))
 
+# Cycle to use when coloring lines from different functions
+COLOR_CYCLE = [
+    SpyderPalette.GROUP_1,
+    SpyderPalette.GROUP_4,
+    SpyderPalette.GROUP_10,
+    SpyderPalette.GROUP_12,
+    SpyderPalette.GROUP_2,
+    SpyderPalette.GROUP_8,
+    SpyderPalette.GROUP_6]
+
 WEBSITE_URL = 'http://pythonhosted.org/line_profiler/'
 
 locale_codec = QTextCodec.codecForLocale()
 
 
 def is_lineprofiler_installed():
     """
@@ -163,19 +176,18 @@
     def __init__(self, name=None, plugin=None, parent=None):
         super().__init__(name, plugin, parent)
         self.setWindowTitle("Line profiler")
 
         # Attributes
         self._last_wdir = None
         self._last_args = None
-        self._last_pythonpath = None
+        self.pythonpath = None
         self.error_output = None
         self.output = None
         self.use_colors = True
-        self.spyder_pythonpath = None
         self.process = None
         self.started_time = None
 
         # Widgets
         self.filecombo = PythonModulesComboBox(
             self, id_=SpyderLineProfilerWidgetMainToolbarItems.FileCombo)
         self.datatree = LineProfilerDataTree(self)
@@ -303,33 +315,32 @@
                 '<b>Please install the <a href="%s">line_profiler module</a></b>'
                 ) % WEBSITE_URL
             self.datelabel.setText(text)
             self.datelabel.setOpenExternalLinks(True)
         else:
             pass
 
-    def analyze(self, filename=None, wdir=None, args=None, pythonpath=None,
-                use_colors=True):
+    def analyze(self, filename=None, wdir=None, args=None, use_colors=True):
         self.use_colors = use_colors
         if not is_lineprofiler_installed():
             return
         self.kill_if_running()
         #index, _data = self.get_data(filename) # FIXME: storing data is not implemented yet
         if filename is not None:
-            filename = osp.abspath(to_text_string(filename))
+            filename = osp.abspath(str(filename))
             index = self.filecombo.findText(filename)
             if index == -1:
                 self.filecombo.addItem(filename)
                 self.filecombo.setCurrentIndex(self.filecombo.count()-1)
             else:
                 self.filecombo.setCurrentIndex(index)
             self.filecombo.selected()
 
         if self.filecombo.is_valid():
-            filename = to_text_string(self.filecombo.currentText())
+            filename = str(self.filecombo.currentText())
             runconf = get_run_configuration(filename)
             if runconf is not None:
                 if wdir is None:
                     if runconf.wdir_enabled:
                         wdir = runconf.wdir
                     elif runconf.cw_dir:
                         wdir = os.getcwd()
@@ -338,17 +349,15 @@
                     elif runconf.fixed_dir:
                         wdir = runconf.dir
                 if args is None:
                     if runconf.args_enabled:
                         args = runconf.args
             if wdir is None:
                 wdir = osp.dirname(filename)
-            if pythonpath is None:
-                pythonpath = self.spyder_pythonpath
-            self.start(wdir, args, pythonpath)
+            self.start(wdir, args)
 
     def select_file(self):
         self.redirect_stdio.emit(False)
         pwd = getcwd_or_home()
 
         filename, _selfilter = getopenfilename(
             self, _("Select Python script"), pwd,
@@ -379,76 +388,71 @@
             editor.show()
             editor.exec_()
 
     def update_timer(self):
         elapsed = str(datetime.now() - self.started_time).split(".")[0]
         self.datelabel.setText(_(f'Profiling, please wait... elapsed: {elapsed}'))
 
-    def start(self, wdir=None, args=None, pythonpath=None):
-        filename = to_text_string(self.filecombo.currentText())
+    def start(self, wdir=None, args=None):
+        filename = str(self.filecombo.currentText())
 
         if wdir in [None, False]:
             wdir = self._last_wdir
             if wdir in [None, False]:
                 wdir = osp.basename(filename)
 
         if args is None:
             args = self._last_args
             if args is None:
                 args = []
-        if pythonpath is None:
-            pythonpath = self._last_pythonpath
 
         self._last_wdir = wdir
         self._last_args = args
-        self._last_pythonpath = pythonpath
 
         self.datelabel.setText(_('Profiling starting up, please wait...'))
         self.started_time = datetime.now()
 
         self.process = QProcess(self)
         self.process.setProcessChannelMode(QProcess.SeparateChannels)
         self.process.setWorkingDirectory(wdir)
         self.process.readyReadStandardOutput.connect(self.read_output)
         self.process.readyReadStandardError.connect(
             lambda: self.read_output(error=True))
         self.process.finished.connect(self.finished)
 
-        if pythonpath is not None:
-            env = [to_text_string(_pth)
-                   for _pth in self.process.systemEnvironment()]
-            env.append(f'PYTHONPATH={pythonpath}')
-            processEnvironment = QProcessEnvironment()
-            for envItem in env:
-                envName, separator, envValue = envItem.partition('=')
-                processEnvironment.insert(envName, envValue)
-            self.process.setProcessEnvironment(processEnvironment)
+        proc_env = QProcessEnvironment()
+        for k, v in os.environ.items():
+            proc_env.insert(k, v)
+        proc_env.remove('PYTHONPATH')
+        if self.pythonpath is not None:
+            logger.debug(f"Pass Pythonpath {self.pythonpath} to process")
+            proc_env.insert('PYTHONPATH', os.pathsep.join(self.pythonpath))
+        self.process.setProcessEnvironment(proc_env)
 
         self.clear_data()
         self.error_output = ''
 
+        p_args = ['-m', 'kernprof', '-lvb', '-o', self.DATAPATH]
         if os.name == 'nt':
             # On Windows, one has to replace backslashes by slashes to avoid
             # confusion with escape characters (otherwise, for example, '\t'
             # will be interpreted as a tabulation):
-            filename = osp.normpath(filename).replace(os.sep, '/')
-            p_args = ['-lvb', '-o', '"' + self.DATAPATH + '"',
-                      '"' + filename + '"']
-            if args:
-                p_args.extend(programs.shell_split(args))
-            executable = '"' + programs.find_program('kernprof') + '"'
-            executable += ' ' + ' '.join(p_args)
-            executable = executable.replace(os.sep, '/')
-            self.process.start(executable)
+            p_args.append(osp.normpath(filename).replace(os.sep, '/'))
         else:
-            p_args = ['-lvb', '-o', self.DATAPATH, filename]
-            if args:
-                p_args.extend(programs.shell_split(args))
-            executable = 'kernprof'
-            self.process.start(executable, p_args)
+            p_args.append(filename)
+        if args:
+            p_args.extend(programs.shell_split(args))
+
+        executable = self.get_conf('executable', section='main_interpreter')
+        if executable.endswith('spyder.exe'):
+            # py2exe distribution
+            executable = 'python.exe'
+
+        logger.debug(f'Starting process with {executable=} and {p_args=}')
+        self.process.start(executable, p_args)
 
         running = self.process.waitForStarted()
         self.set_running_state(running)
         self.timer.timeout.connect(self.update_timer)
         self.timer.start(1000)
 
         if not running:
@@ -466,15 +470,15 @@
             self.process.setReadChannel(QProcess.StandardOutput)
         qba = QByteArray()
         while self.process.bytesAvailable():
             if error:
                 qba += self.process.readAllStandardError()
             else:
                 qba += self.process.readAllStandardOutput()
-        text = to_text_string(locale_codec.toUnicode(qba.data()))
+        text = str(locale_codec.toUnicode(qba.data()))
         if error:
             self.error_output += text
         else:
             self.output += text
 
     def finished(self):
         self.timer.stop()
@@ -491,14 +495,18 @@
         self.datelabel.setText(_('Profiling aborted.'))
         if self.process is not None:
             if self.process.state() == QProcess.Running:
                 self.process.kill()
                 self.output = 'aborted'
                 self.process.waitForFinished()
 
+    @on_conf_change(section='pythonpath_manager', option='spyder_pythonpath')
+    def _update_pythonpath(self, value):
+        self.pythonpath = value
+
     def clear_data(self):
         self.datatree.clear()
         self.clear_action.setEnabled(False)
         self.log_action.setEnabled(False)
         self.save_action.setEnabled(False)
         self.output = ''
 
@@ -507,15 +515,15 @@
             self.clear_data()
         output_exists = self.output is not None and len(self.output) > 0
         self.clear_action.setEnabled(output_exists)
         self.log_action.setEnabled(output_exists)
         self.save_action.setEnabled(output_exists)
 
         self.kill_if_running()
-        filename = to_text_string(self.filecombo.currentText())
+        filename = str(self.filecombo.currentText())
         if not filename:
             return
 
         self.datatree.load_data(self.DATAPATH)
         QApplication.processEvents()
         self.datatree.show_tree()
 
@@ -547,18 +555,14 @@
                 f.write(results)
 
             self.datelabel.setText(_(f"Saved results to {filename}"))
 
     def update_actions(self):
         pass
 
-    @on_conf_change
-    def on_section_conf_change(self, section):
-        pass
-
 
 class LineProfilerDataTree(QTreeWidget):
     """
     Convenience tree widget (with built-in model)
     to store and view line profiler data.
     """
     sig_edit_goto_requested = Signal(str, int, str)
@@ -704,16 +708,17 @@
 
         try:
             monospace_font = self.window().editor.get_plugin_font()
         except AttributeError:  # If run standalone for testing
             monospace_font = QFont("Courier New")
             monospace_font.setPointSize(10)
 
-        for func_info, func_data in self.stats.items():
+        for func_index, stat_item in enumerate(self.stats.items()):
             # Function name and position
+            func_info, func_data = stat_item
             filename, start_line_no, func_name = func_info
             func_stats, func_total_time = func_data
             func_item = TreeWidgetItem(self)
             func_item.setData(
                 0, Qt.DisplayRole,
                 _('{func_name} ({time_ms:.3f}ms) in file "{filename}", '
                   'line {line_no}').format(
@@ -727,21 +732,18 @@
 
             # For sorting by time
             func_item.setData(COL_TIME, Qt.DisplayRole, func_total_time * 1e3)
             func_item.setData(COL_PERCENT, Qt.DisplayRole,
                               func_total_time * 1e3)
 
             if self.parent().use_colors:
-                # Choose deteministic unique color for the function
-                md5 = hashlib.md5((filename + func_name).encode("utf8")).hexdigest()
-                hue = (int(md5[:2], 16) - 68) % 360  # avoid blue (unreadable)
-                func_color = QColor.fromHsv(hue, 200, 255)
+                color_index = func_index % len(COLOR_CYCLE)
             else:
-                # Red color only
-                func_color = QColor.fromRgb(255, 0, 0)
+                color_index = 0
+            func_color = COLOR_CYCLE[color_index]
 
             # Lines of code
             for line_info in func_stats:
                 line_item = TreeWidgetItem(func_item)
                 (line_no, code_line, line_total_time, time_per_hit,
                  hits, percent) = line_info
                 self.fill_item(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spyder_line_profiler-0.3.1/spyder_line_profiler.egg-info/PKG-INFO` & `spyder_line_profiler-0.3.2/spyder_line_profiler.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: spyder-line-profiler
-Version: 0.3.1
+Version: 0.3.2
 Summary: Plugin for the Spyder 5 IDE that integrates the Python line profiler.
 Home-page: https://github.com/spyder-ide/spyder-line-profiler
 Author: Spyder Project Contributors
 License: MIT
 Keywords: Qt PyQt5 PySide2 spyder plugins spyplugins line_profiler profiler
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +28,13 @@
 It allows you to see the time spent in every line.
 
 Usage
 -----
 
 Add a ``@profile`` decorator to the functions that you wish to profile
 then press Shift+F10 (line profiler default) to run the profiler on
-the current script, or go to ``Run > Profile line by line``.
+the current script, or go to ``Run > Run line profiler``.
 
 The results will be shown in a dockwidget, grouped by function. Lines
 with a stronger color take more time to run.
 
 .. image: https://raw.githubusercontent.com/spyder-ide/spyder-line-profiler/master/img_src/screenshot_profiler.png
-
-
```

### Comparing `spyder_line_profiler-0.3.1/spyder_line_profiler.egg-info/SOURCES.txt` & `spyder_line_profiler-0.3.2/spyder_line_profiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

