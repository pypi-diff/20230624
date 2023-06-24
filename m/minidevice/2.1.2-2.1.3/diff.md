# Comparing `tmp/minidevice-2.1.2.tar.gz` & `tmp/minidevice-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.1.2.tar", last modified: Sat Jun 24 09:47:49 2023, max compression
+gzip compressed data, was "minidevice-2.1.3.tar", last modified: Sat Jun 24 12:07:43 2023, max compression
```

## Comparing `minidevice-2.1.2.tar` & `minidevice-2.1.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 09:47:49.814124 minidevice-2.1.2/
--rw-rw-rw-   0        0        0      616 2023-06-24 09:47:49.813128 minidevice-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-06-24 07:57:44.000000 minidevice-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 09:47:49.801798 minidevice-2.1.2/minidevice/
--rw-rw-rw-   0        0        0     2954 2023-06-24 09:47:37.000000 minidevice-2.1.2/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.1.2/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      344 2023-06-24 07:38:48.000000 minidevice-2.1.2/minidevice/__init__.py
--rw-rw-rw-   0        0        0     5035 2023-06-24 09:21:19.000000 minidevice-2.1.2/minidevice/adb.py
--rw-rw-rw-   0        0        0      467 2023-06-24 09:21:26.000000 minidevice-2.1.2/minidevice/adbcap.py
--rw-rw-rw-   0        0        0      819 2023-06-24 09:18:16.000000 minidevice-2.1.2/minidevice/adbtouch.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.1.2/minidevice/logger.py
--rw-rw-rw-   0        0        0    13045 2023-06-24 09:46:11.000000 minidevice-2.1.2/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1498 2023-06-24 07:22:12.000000 minidevice-2.1.2/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      651 2023-06-24 09:39:45.000000 minidevice-2.1.2/minidevice/scrcpycap.py
--rw-rw-rw-   0        0        0     1049 2023-06-24 09:39:50.000000 minidevice-2.1.2/minidevice/scrcpytouch.py
--rw-rw-rw-   0        0        0      687 2023-06-21 07:24:32.000000 minidevice-2.1.2/minidevice/screencap.py
--rw-rw-rw-   0        0        0      620 2023-06-24 07:21:44.000000 minidevice-2.1.2/minidevice/touch.py
--rw-rw-rw-   0        0        0     7503 2023-06-22 06:33:34.000000 minidevice-2.1.2/minidevice/win.py
-drwxrwxrwx   0        0        0        0 2023-06-24 09:47:49.812121 minidevice-2.1.2/minidevice.egg-info/
--rw-rw-rw-   0        0        0      616 2023-06-24 09:47:49.000000 minidevice-2.1.2/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-06-24 09:47:49.000000 minidevice-2.1.2/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 09:47:49.000000 minidevice-2.1.2/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-24 09:47:49.000000 minidevice-2.1.2/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 09:47:49.000000 minidevice-2.1.2/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 09:47:49.814124 minidevice-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-24 09:47:48.000000 minidevice-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 12:07:43.174934 minidevice-2.1.3/
+-rw-rw-rw-   0        0        0      811 2023-06-24 12:07:43.174934 minidevice-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-06-24 12:06:18.000000 minidevice-2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 12:07:43.168070 minidevice-2.1.3/minidevice/
+-rw-rw-rw-   0        0        0     2954 2023-06-24 09:47:37.000000 minidevice-2.1.3/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.1.3/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      300 2023-06-24 12:06:51.000000 minidevice-2.1.3/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     5035 2023-06-24 09:21:19.000000 minidevice-2.1.3/minidevice/adb.py
+-rw-rw-rw-   0        0        0      467 2023-06-24 09:21:26.000000 minidevice-2.1.3/minidevice/adbcap.py
+-rw-rw-rw-   0        0        0      819 2023-06-24 09:18:16.000000 minidevice-2.1.3/minidevice/adbtouch.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.1.3/minidevice/logger.py
+-rw-rw-rw-   0        0        0    13045 2023-06-24 09:46:11.000000 minidevice-2.1.3/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1498 2023-06-24 07:22:12.000000 minidevice-2.1.3/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      651 2023-06-24 09:39:45.000000 minidevice-2.1.3/minidevice/scrcpycap.py
+-rw-rw-rw-   0        0        0     1049 2023-06-24 09:39:50.000000 minidevice-2.1.3/minidevice/scrcpytouch.py
+-rw-rw-rw-   0        0        0      687 2023-06-21 07:24:32.000000 minidevice-2.1.3/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      620 2023-06-24 07:21:44.000000 minidevice-2.1.3/minidevice/touch.py
+drwxrwxrwx   0        0        0        0 2023-06-24 12:07:43.173958 minidevice-2.1.3/minidevice.egg-info/
+-rw-rw-rw-   0        0        0      811 2023-06-24 12:07:43.000000 minidevice-2.1.3/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-06-24 12:07:43.000000 minidevice-2.1.3/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 12:07:43.000000 minidevice-2.1.3/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-24 12:07:43.000000 minidevice-2.1.3/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 12:07:43.000000 minidevice-2.1.3/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 12:07:43.174934 minidevice-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-24 12:07:04.000000 minidevice-2.1.3/setup.py
```

### Comparing `minidevice-2.1.2/PKG-INFO` & `minidevice-2.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.2
+Version: 2.1.3
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
@@ -14,7 +14,19 @@
 一个对安卓设备(主要是安卓模拟器)进行基础操作的工具包
 ## requirements
 `opencv-python` [`pyminitouch`](https://github.com/williamfzc/pyminitouch),`scrcpy-client`
 ## 安装
 `pip install minidevice`
 ## API文档以及使用说明
 [跳转](https://nakanosanku.github.io/minidevice/)
+## 已知bug
+- [ ] 转发端口清理失败
+## Feature
+- screencap
+    - Minicap
+    - ADBcap
+    - DroidCast
+    - ScrcpyCap
+- touch
+    - Minitouch
+    - ADBtouch
+    - ScrcpyTouch
```

### Comparing `minidevice-2.1.2/minidevice/DroidCast.py` & `minidevice-2.1.3/minidevice/DroidCast.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.2/minidevice/QueueUtils.py` & `minidevice-2.1.3/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.2/minidevice/adb.py` & `minidevice-2.1.3/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.2/minidevice/adbtouch.py` & `minidevice-2.1.3/minidevice/adbtouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.2/minidevice/minicap.py` & `minidevice-2.1.3/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.2/minidevice/minitouch.py` & `minidevice-2.1.3/minidevice/minitouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.2/minidevice/scrcpycap.py` & `minidevice-2.1.3/minidevice/scrcpycap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.2/minidevice/scrcpytouch.py` & `minidevice-2.1.3/minidevice/scrcpytouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.2/minidevice/screencap.py` & `minidevice-2.1.3/minidevice/screencap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.2/minidevice/touch.py` & `minidevice-2.1.3/minidevice/touch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.2/minidevice.egg-info/PKG-INFO` & `minidevice-2.1.3/minidevice.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.2
+Version: 2.1.3
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
@@ -14,7 +14,19 @@
 一个对安卓设备(主要是安卓模拟器)进行基础操作的工具包
 ## requirements
 `opencv-python` [`pyminitouch`](https://github.com/williamfzc/pyminitouch),`scrcpy-client`
 ## 安装
 `pip install minidevice`
 ## API文档以及使用说明
 [跳转](https://nakanosanku.github.io/minidevice/)
+## 已知bug
+- [ ] 转发端口清理失败
+## Feature
+- screencap
+    - Minicap
+    - ADBcap
+    - DroidCast
+    - ScrcpyCap
+- touch
+    - Minitouch
+    - ADBtouch
+    - ScrcpyTouch
```

### Comparing `minidevice-2.1.2/setup.py` & `minidevice-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.1.2',
+      version='2.1.3',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

