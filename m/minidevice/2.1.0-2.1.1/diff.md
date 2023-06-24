# Comparing `tmp/minidevice-2.1.0.tar.gz` & `tmp/minidevice-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.1.0.tar", last modified: Sat Jun 24 09:04:40 2023, max compression
+gzip compressed data, was "minidevice-2.1.1.tar", last modified: Sat Jun 24 09:33:08 2023, max compression
```

## Comparing `minidevice-2.1.0.tar` & `minidevice-2.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 09:04:40.566657 minidevice-2.1.0/
--rw-rw-rw-   0        0        0      616 2023-06-24 09:04:40.566657 minidevice-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-06-24 07:57:44.000000 minidevice-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 09:04:40.558845 minidevice-2.1.0/minidevice/
--rw-rw-rw-   0        0        0     3036 2023-06-24 07:04:06.000000 minidevice-2.1.0/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.1.0/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      344 2023-06-24 07:38:48.000000 minidevice-2.1.0/minidevice/__init__.py
--rw-rw-rw-   0        0        0     5036 2023-06-24 07:17:55.000000 minidevice-2.1.0/minidevice/adb.py
--rw-rw-rw-   0        0        0      493 2023-06-24 07:46:39.000000 minidevice-2.1.0/minidevice/adbcap.py
--rw-rw-rw-   0        0        0      812 2023-06-24 07:22:29.000000 minidevice-2.1.0/minidevice/adbtouch.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.1.0/minidevice/logger.py
--rw-rw-rw-   0        0        0    13039 2023-06-24 09:01:43.000000 minidevice-2.1.0/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1498 2023-06-24 07:22:12.000000 minidevice-2.1.0/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      515 2023-06-24 07:15:12.000000 minidevice-2.1.0/minidevice/scrcpycap.py
--rw-rw-rw-   0        0        0      916 2023-06-24 08:53:14.000000 minidevice-2.1.0/minidevice/scrcpytouch.py
--rw-rw-rw-   0        0        0      687 2023-06-21 07:24:32.000000 minidevice-2.1.0/minidevice/screencap.py
--rw-rw-rw-   0        0        0      620 2023-06-24 07:21:44.000000 minidevice-2.1.0/minidevice/touch.py
--rw-rw-rw-   0        0        0     7503 2023-06-22 06:33:34.000000 minidevice-2.1.0/minidevice/win.py
-drwxrwxrwx   0        0        0        0 2023-06-24 09:04:40.565682 minidevice-2.1.0/minidevice.egg-info/
--rw-rw-rw-   0        0        0      616 2023-06-24 09:04:40.000000 minidevice-2.1.0/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-06-24 09:04:40.000000 minidevice-2.1.0/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 09:04:40.000000 minidevice-2.1.0/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-24 09:04:40.000000 minidevice-2.1.0/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 09:04:40.000000 minidevice-2.1.0/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 09:04:40.566657 minidevice-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      838 2023-06-24 09:04:17.000000 minidevice-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:33:08.360051 minidevice-2.1.1/
+-rw-rw-rw-   0        0        0      616 2023-06-24 09:33:08.360051 minidevice-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-06-24 07:57:44.000000 minidevice-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 09:33:08.352661 minidevice-2.1.1/minidevice/
+-rw-rw-rw-   0        0        0     3036 2023-06-24 07:04:06.000000 minidevice-2.1.1/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.1.1/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      344 2023-06-24 07:38:48.000000 minidevice-2.1.1/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     5035 2023-06-24 09:21:19.000000 minidevice-2.1.1/minidevice/adb.py
+-rw-rw-rw-   0        0        0      467 2023-06-24 09:21:26.000000 minidevice-2.1.1/minidevice/adbcap.py
+-rw-rw-rw-   0        0        0      819 2023-06-24 09:18:16.000000 minidevice-2.1.1/minidevice/adbtouch.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.1.1/minidevice/logger.py
+-rw-rw-rw-   0        0        0    13043 2023-06-24 09:09:38.000000 minidevice-2.1.1/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1498 2023-06-24 07:22:12.000000 minidevice-2.1.1/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      676 2023-06-24 09:32:40.000000 minidevice-2.1.1/minidevice/scrcpycap.py
+-rw-rw-rw-   0        0        0     1087 2023-06-24 09:32:58.000000 minidevice-2.1.1/minidevice/scrcpytouch.py
+-rw-rw-rw-   0        0        0      687 2023-06-21 07:24:32.000000 minidevice-2.1.1/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      620 2023-06-24 07:21:44.000000 minidevice-2.1.1/minidevice/touch.py
+-rw-rw-rw-   0        0        0     7503 2023-06-22 06:33:34.000000 minidevice-2.1.1/minidevice/win.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:33:08.358095 minidevice-2.1.1/minidevice.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-06-24 09:33:08.000000 minidevice-2.1.1/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-06-24 09:33:08.000000 minidevice-2.1.1/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 09:33:08.000000 minidevice-2.1.1/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-24 09:33:08.000000 minidevice-2.1.1/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 09:33:08.000000 minidevice-2.1.1/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 09:33:08.361027 minidevice-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-24 09:10:16.000000 minidevice-2.1.1/setup.py
```

### Comparing `minidevice-2.1.0/PKG-INFO` & `minidevice-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.0
+Version: 2.1.1
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.1.0/minidevice/DroidCast.py` & `minidevice-2.1.1/minidevice/DroidCast.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.0/minidevice/QueueUtils.py` & `minidevice-2.1.1/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.0/minidevice/adb.py` & `minidevice-2.1.1/minidevice/adb.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
     def change_file_permission(self, permission, file_path):
         self.__run_adb_command(["shell", "chmod", permission, file_path])
 
     def kill_process(self, pid):
         self.__run_adb_command(["shell", "kill", str(pid)])
 
-    def __screencap_raw(self):
+    def _screencap_raw(self):
         """获取截图源数据"""
         return self.adb_command(["exec-out", "screencap", "-p"])
 
 
 def str_to_dict(str):
     dict_info = {}
     lines = str.splitlines()
```

### Comparing `minidevice-2.1.0/minidevice/adbtouch.py` & `minidevice-2.1.1/minidevice/adbtouch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from minidevice import logger
+from minidevice.logger import logger
 from minidevice.adb import ADB
 from minidevice.touch import Touch
 
 class ADBtouch(Touch, ADB):
     def __init__(self, device) -> None:
         """
         __init__ ADB 操作方式
```

### Comparing `minidevice-2.1.0/minidevice/minicap.py` & `minidevice-2.1.1/minidevice/minicap.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
 
     def __forward_minicap(self):
         self.minicap_port = self.minicap_adb.forward_port(
             "localabstract:{}".format(self.minicap_name)
         )
 
     def __read_minicap_stream(self):
-        self.minicap_stream = MinicapStream.getBuilder(self.ip, self.minicap_port)
+        self.minicap_stream = MinicapStream.getBuilder("127.0.0.1", self.minicap_port)
         self.minicap_stream.run()
         self.banner = self.minicap_stream.banner
         self.screen_queue = self.minicap_stream.queue
 
     def __start_minicap_by_stream(self):
         if not self.__start_minicap():
             self.__minicap_install()
```

### Comparing `minidevice-2.1.0/minidevice/minitouch.py` & `minidevice-2.1.1/minidevice/minitouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.0/minidevice/screencap.py` & `minidevice-2.1.1/minidevice/screencap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.0/minidevice/touch.py` & `minidevice-2.1.1/minidevice/touch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.0/minidevice/win.py` & `minidevice-2.1.1/minidevice/win.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.0/minidevice.egg-info/PKG-INFO` & `minidevice-2.1.1/minidevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.0
+Version: 2.1.1
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.1.0/setup.py` & `minidevice-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.1.0',
+      version='2.1.1',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
       keywords='game',
       project_urls={},
       packages=find_packages(),
       include_package_data=True,
       install_requires=['opencv-python>=4.7.0.72',
                         'pyminitouch>=0.3.3',
                         'scrcpy-client',
-                        'request>=2.31.0'
+                        'requests>=2.31.0'
                         ],
       python_requires='>=3'
       )
```

