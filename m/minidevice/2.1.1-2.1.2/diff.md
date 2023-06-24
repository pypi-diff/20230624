# Comparing `tmp/minidevice-2.1.1.tar.gz` & `tmp/minidevice-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.1.1.tar", last modified: Sat Jun 24 09:33:08 2023, max compression
+gzip compressed data, was "minidevice-2.1.2.tar", last modified: Sat Jun 24 09:47:49 2023, max compression
```

## Comparing `minidevice-2.1.1.tar` & `minidevice-2.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 09:33:08.360051 minidevice-2.1.1/
--rw-rw-rw-   0        0        0      616 2023-06-24 09:33:08.360051 minidevice-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-06-24 07:57:44.000000 minidevice-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 09:33:08.352661 minidevice-2.1.1/minidevice/
--rw-rw-rw-   0        0        0     3036 2023-06-24 07:04:06.000000 minidevice-2.1.1/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.1.1/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      344 2023-06-24 07:38:48.000000 minidevice-2.1.1/minidevice/__init__.py
--rw-rw-rw-   0        0        0     5035 2023-06-24 09:21:19.000000 minidevice-2.1.1/minidevice/adb.py
--rw-rw-rw-   0        0        0      467 2023-06-24 09:21:26.000000 minidevice-2.1.1/minidevice/adbcap.py
--rw-rw-rw-   0        0        0      819 2023-06-24 09:18:16.000000 minidevice-2.1.1/minidevice/adbtouch.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.1.1/minidevice/logger.py
--rw-rw-rw-   0        0        0    13043 2023-06-24 09:09:38.000000 minidevice-2.1.1/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1498 2023-06-24 07:22:12.000000 minidevice-2.1.1/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      676 2023-06-24 09:32:40.000000 minidevice-2.1.1/minidevice/scrcpycap.py
--rw-rw-rw-   0        0        0     1087 2023-06-24 09:32:58.000000 minidevice-2.1.1/minidevice/scrcpytouch.py
--rw-rw-rw-   0        0        0      687 2023-06-21 07:24:32.000000 minidevice-2.1.1/minidevice/screencap.py
--rw-rw-rw-   0        0        0      620 2023-06-24 07:21:44.000000 minidevice-2.1.1/minidevice/touch.py
--rw-rw-rw-   0        0        0     7503 2023-06-22 06:33:34.000000 minidevice-2.1.1/minidevice/win.py
-drwxrwxrwx   0        0        0        0 2023-06-24 09:33:08.358095 minidevice-2.1.1/minidevice.egg-info/
--rw-rw-rw-   0        0        0      616 2023-06-24 09:33:08.000000 minidevice-2.1.1/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-06-24 09:33:08.000000 minidevice-2.1.1/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 09:33:08.000000 minidevice-2.1.1/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-24 09:33:08.000000 minidevice-2.1.1/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 09:33:08.000000 minidevice-2.1.1/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 09:33:08.361027 minidevice-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-24 09:10:16.000000 minidevice-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:47:49.814124 minidevice-2.1.2/
+-rw-rw-rw-   0        0        0      616 2023-06-24 09:47:49.813128 minidevice-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-06-24 07:57:44.000000 minidevice-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 09:47:49.801798 minidevice-2.1.2/minidevice/
+-rw-rw-rw-   0        0        0     2954 2023-06-24 09:47:37.000000 minidevice-2.1.2/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.1.2/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      344 2023-06-24 07:38:48.000000 minidevice-2.1.2/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     5035 2023-06-24 09:21:19.000000 minidevice-2.1.2/minidevice/adb.py
+-rw-rw-rw-   0        0        0      467 2023-06-24 09:21:26.000000 minidevice-2.1.2/minidevice/adbcap.py
+-rw-rw-rw-   0        0        0      819 2023-06-24 09:18:16.000000 minidevice-2.1.2/minidevice/adbtouch.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.1.2/minidevice/logger.py
+-rw-rw-rw-   0        0        0    13045 2023-06-24 09:46:11.000000 minidevice-2.1.2/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1498 2023-06-24 07:22:12.000000 minidevice-2.1.2/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      651 2023-06-24 09:39:45.000000 minidevice-2.1.2/minidevice/scrcpycap.py
+-rw-rw-rw-   0        0        0     1049 2023-06-24 09:39:50.000000 minidevice-2.1.2/minidevice/scrcpytouch.py
+-rw-rw-rw-   0        0        0      687 2023-06-21 07:24:32.000000 minidevice-2.1.2/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      620 2023-06-24 07:21:44.000000 minidevice-2.1.2/minidevice/touch.py
+-rw-rw-rw-   0        0        0     7503 2023-06-22 06:33:34.000000 minidevice-2.1.2/minidevice/win.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:47:49.812121 minidevice-2.1.2/minidevice.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-06-24 09:47:49.000000 minidevice-2.1.2/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-06-24 09:47:49.000000 minidevice-2.1.2/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 09:47:49.000000 minidevice-2.1.2/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-24 09:47:49.000000 minidevice-2.1.2/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 09:47:49.000000 minidevice-2.1.2/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 09:47:49.814124 minidevice-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-24 09:47:48.000000 minidevice-2.1.2/setup.py
```

### Comparing `minidevice-2.1.1/PKG-INFO` & `minidevice-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.1
+Version: 2.1.2
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.1.1/minidevice/DroidCast.py` & `minidevice-2.1.2/minidevice/DroidCast.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,20 +75,19 @@
 
     def __start(self):
         self.__start_droidcast()
         self.__forward_port()
         print("DroidCast启动完成")
 
     def __stop(self):
-        self.droidcast_adb.remove_forward(self.droidcast_port)  # 清理转发端口
         if self.droidcast_popen.poll() is None:
             self.droidcast_popen.kill()  # 关闭管道
 
     def screencap_raw(self) -> bytes:
         if self.droidcast_popen.poll() is not None:
             self.__stop()
             self.__start()
         return self.DroidCastSession.get(self.droidcast_url, timeout=3).content
 
-    def __del__(self):
-        self.__stop()
+    # def __del__(self):
+    #     self.__stop()
```

### Comparing `minidevice-2.1.1/minidevice/QueueUtils.py` & `minidevice-2.1.2/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.1/minidevice/adb.py` & `minidevice-2.1.2/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.1/minidevice/adbtouch.py` & `minidevice-2.1.2/minidevice/adbtouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.1/minidevice/minicap.py` & `minidevice-2.1.2/minidevice/minicap.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
             if not self.__start_minicap():
                 raise Exception("minicap不可用")
         self.__forward_minicap()
         self.__read_minicap_stream()
 
     def __stop_minicap_by_stream(self):
         self.minicap_stream.stop()  # 停止stream
-        self.minicap_adb.remove_forward(self.minicap_port)  # 清理端口
+        # self.minicap_adb.remove_forward(self.minicap_port)  # 清理端口
         if self.minicap_popen.poll() is None:  # 清理管道
             self.minicap_popen.kill()
 
     def __del__(self):
         self.__stop_minicap_by_stream()
         
 if __name__ == "__main__":
```

### Comparing `minidevice-2.1.1/minidevice/minitouch.py` & `minidevice-2.1.2/minidevice/minitouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.1/minidevice/screencap.py` & `minidevice-2.1.2/minidevice/screencap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.1/minidevice/touch.py` & `minidevice-2.1.2/minidevice/touch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.1/minidevice/win.py` & `minidevice-2.1.2/minidevice/win.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.1/minidevice.egg-info/PKG-INFO` & `minidevice-2.1.2/minidevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.1
+Version: 2.1.2
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.1.1/setup.py` & `minidevice-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.1.1',
+      version='2.1.2',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

