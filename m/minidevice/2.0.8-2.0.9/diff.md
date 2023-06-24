# Comparing `tmp/minidevice-2.0.8.tar.gz` & `tmp/minidevice-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.0.8.tar", last modified: Sat Jun 24 08:13:29 2023, max compression
+gzip compressed data, was "minidevice-2.0.9.tar", last modified: Sat Jun 24 08:53:38 2023, max compression
```

## Comparing `minidevice-2.0.8.tar` & `minidevice-2.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 08:13:29.876531 minidevice-2.0.8/
--rw-rw-rw-   0        0        0      616 2023-06-24 08:13:29.875550 minidevice-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-06-24 07:57:44.000000 minidevice-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 08:13:29.863844 minidevice-2.0.8/minidevice/
--rw-rw-rw-   0        0        0     3036 2023-06-24 07:04:06.000000 minidevice-2.0.8/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.8/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      344 2023-06-24 07:38:48.000000 minidevice-2.0.8/minidevice/__init__.py
--rw-rw-rw-   0        0        0     5036 2023-06-24 07:17:55.000000 minidevice-2.0.8/minidevice/adb.py
--rw-rw-rw-   0        0        0      493 2023-06-24 07:46:39.000000 minidevice-2.0.8/minidevice/adbcap.py
--rw-rw-rw-   0        0        0      812 2023-06-24 07:22:29.000000 minidevice-2.0.8/minidevice/adbtouch.py
--rw-rw-rw-   0        0        0    20739 2023-06-18 02:48:13.000000 minidevice-2.0.8/minidevice/images.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.8/minidevice/logger.py
--rw-rw-rw-   0        0        0    13065 2023-06-24 07:03:45.000000 minidevice-2.0.8/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1498 2023-06-24 07:22:12.000000 minidevice-2.0.8/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      515 2023-06-24 07:15:12.000000 minidevice-2.0.8/minidevice/scrcpycap.py
--rw-rw-rw-   0        0        0      905 2023-06-24 07:22:50.000000 minidevice-2.0.8/minidevice/scrcpytouch.py
--rw-rw-rw-   0        0        0      687 2023-06-21 07:24:32.000000 minidevice-2.0.8/minidevice/screencap.py
--rw-rw-rw-   0        0        0      620 2023-06-24 07:21:44.000000 minidevice-2.0.8/minidevice/touch.py
--rw-rw-rw-   0        0        0     7503 2023-06-22 06:33:34.000000 minidevice-2.0.8/minidevice/win.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:13:29.874164 minidevice-2.0.8/minidevice.egg-info/
--rw-rw-rw-   0        0        0      616 2023-06-24 08:13:29.000000 minidevice-2.0.8/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2023-06-24 08:13:29.000000 minidevice-2.0.8/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 08:13:29.000000 minidevice-2.0.8/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-24 08:13:29.000000 minidevice-2.0.8/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 08:13:29.000000 minidevice-2.0.8/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 08:13:29.876531 minidevice-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0      825 2023-06-24 07:59:49.000000 minidevice-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:53:38.700639 minidevice-2.0.9/
+-rw-rw-rw-   0        0        0      616 2023-06-24 08:53:38.699663 minidevice-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-06-24 07:57:44.000000 minidevice-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 08:53:38.691095 minidevice-2.0.9/minidevice/
+-rw-rw-rw-   0        0        0     3036 2023-06-24 07:04:06.000000 minidevice-2.0.9/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.9/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      344 2023-06-24 07:38:48.000000 minidevice-2.0.9/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     5036 2023-06-24 07:17:55.000000 minidevice-2.0.9/minidevice/adb.py
+-rw-rw-rw-   0        0        0      493 2023-06-24 07:46:39.000000 minidevice-2.0.9/minidevice/adbcap.py
+-rw-rw-rw-   0        0        0      812 2023-06-24 07:22:29.000000 minidevice-2.0.9/minidevice/adbtouch.py
+-rw-rw-rw-   0        0        0    20739 2023-06-18 02:48:13.000000 minidevice-2.0.9/minidevice/images.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.9/minidevice/logger.py
+-rw-rw-rw-   0        0        0    13065 2023-06-24 07:03:45.000000 minidevice-2.0.9/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1498 2023-06-24 07:22:12.000000 minidevice-2.0.9/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      515 2023-06-24 07:15:12.000000 minidevice-2.0.9/minidevice/scrcpycap.py
+-rw-rw-rw-   0        0        0      916 2023-06-24 08:53:14.000000 minidevice-2.0.9/minidevice/scrcpytouch.py
+-rw-rw-rw-   0        0        0      687 2023-06-21 07:24:32.000000 minidevice-2.0.9/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      620 2023-06-24 07:21:44.000000 minidevice-2.0.9/minidevice/touch.py
+-rw-rw-rw-   0        0        0     7503 2023-06-22 06:33:34.000000 minidevice-2.0.9/minidevice/win.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:53:38.698682 minidevice-2.0.9/minidevice.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-06-24 08:53:38.000000 minidevice-2.0.9/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2023-06-24 08:53:38.000000 minidevice-2.0.9/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 08:53:38.000000 minidevice-2.0.9/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-24 08:53:38.000000 minidevice-2.0.9/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 08:53:38.000000 minidevice-2.0.9/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 08:53:38.700639 minidevice-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      825 2023-06-24 08:53:29.000000 minidevice-2.0.9/setup.py
```

### Comparing `minidevice-2.0.8/PKG-INFO` & `minidevice-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.8
+Version: 2.0.9
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.0.8/minidevice/DroidCast.py` & `minidevice-2.0.9/minidevice/DroidCast.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/minidevice/QueueUtils.py` & `minidevice-2.0.9/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/minidevice/adb.py` & `minidevice-2.0.9/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/minidevice/adbtouch.py` & `minidevice-2.0.9/minidevice/adbtouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/minidevice/images.py` & `minidevice-2.0.9/minidevice/images.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/minidevice/minicap.py` & `minidevice-2.0.9/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/minidevice/minitouch.py` & `minidevice-2.0.9/minidevice/minitouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/minidevice/scrcpycap.py` & `minidevice-2.0.9/minidevice/scrcpycap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/minidevice/scrcpytouch.py` & `minidevice-2.0.9/minidevice/scrcpytouch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import scrcpy
-from touch import Touch
+from minidevice.touch import Touch
 
 
 class ScrcpyTouch(Touch):
     def __init__(self, device: scrcpy.Client) -> None:
         """
         __init__ ScrcpyCap
```

### Comparing `minidevice-2.0.8/minidevice/screencap.py` & `minidevice-2.0.9/minidevice/screencap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/minidevice/touch.py` & `minidevice-2.0.9/minidevice/touch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/minidevice/win.py` & `minidevice-2.0.9/minidevice/win.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/minidevice.egg-info/PKG-INFO` & `minidevice-2.0.9/minidevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.8
+Version: 2.0.9
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.0.8/minidevice.egg-info/SOURCES.txt` & `minidevice-2.0.9/minidevice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.8/setup.py` & `minidevice-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.0.8',
+      version='2.0.9',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

