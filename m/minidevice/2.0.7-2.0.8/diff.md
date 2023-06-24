# Comparing `tmp/minidevice-2.0.7.tar.gz` & `tmp/minidevice-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.0.7.tar", last modified: Mon Jun 19 01:19:03 2023, max compression
+gzip compressed data, was "minidevice-2.0.8.tar", last modified: Sat Jun 24 08:13:29 2023, max compression
```

## Comparing `minidevice-2.0.7.tar` & `minidevice-2.0.8.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:19:03.627362 minidevice-2.0.7/
--rw-rw-rw-   0        0        0     3077 2023-06-19 01:19:03.627362 minidevice-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2783 2023-06-18 05:30:28.000000 minidevice-2.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 01:19:03.608809 minidevice-2.0.7/minidevice/
--rw-rw-rw-   0        0        0     2809 2023-06-19 01:16:20.000000 minidevice-2.0.7/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.7/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      268 2023-06-18 05:20:44.000000 minidevice-2.0.7/minidevice/__init__.py
--rw-rw-rw-   0        0        0    21023 2023-06-18 04:23:42.000000 minidevice-2.0.7/minidevice/adb.py
--rw-rw-rw-   0        0        0     1659 2023-06-18 05:27:30.000000 minidevice-2.0.7/minidevice/device.py
--rw-rw-rw-   0        0        0    20739 2023-06-18 02:48:13.000000 minidevice-2.0.7/minidevice/images.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.7/minidevice/logger.py
--rw-rw-rw-   0        0        0    12881 2023-06-19 01:17:22.000000 minidevice-2.0.7/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1774 2023-06-19 01:14:32.000000 minidevice-2.0.7/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      687 2023-06-18 04:29:14.000000 minidevice-2.0.7/minidevice/screencap.py
--rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.7/minidevice/touch.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:19:03.625410 minidevice-2.0.7/minidevice.egg-info/
--rw-rw-rw-   0        0        0     3077 2023-06-19 01:19:03.000000 minidevice-2.0.7/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-06-19 01:19:03.000000 minidevice-2.0.7/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:19:03.000000 minidevice-2.0.7/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-19 01:19:03.000000 minidevice-2.0.7/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 01:19:03.000000 minidevice-2.0.7/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 01:19:03.628339 minidevice-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-19 01:18:33.000000 minidevice-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:13:29.876531 minidevice-2.0.8/
+-rw-rw-rw-   0        0        0      616 2023-06-24 08:13:29.875550 minidevice-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-06-24 07:57:44.000000 minidevice-2.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 08:13:29.863844 minidevice-2.0.8/minidevice/
+-rw-rw-rw-   0        0        0     3036 2023-06-24 07:04:06.000000 minidevice-2.0.8/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.8/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      344 2023-06-24 07:38:48.000000 minidevice-2.0.8/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     5036 2023-06-24 07:17:55.000000 minidevice-2.0.8/minidevice/adb.py
+-rw-rw-rw-   0        0        0      493 2023-06-24 07:46:39.000000 minidevice-2.0.8/minidevice/adbcap.py
+-rw-rw-rw-   0        0        0      812 2023-06-24 07:22:29.000000 minidevice-2.0.8/minidevice/adbtouch.py
+-rw-rw-rw-   0        0        0    20739 2023-06-18 02:48:13.000000 minidevice-2.0.8/minidevice/images.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.8/minidevice/logger.py
+-rw-rw-rw-   0        0        0    13065 2023-06-24 07:03:45.000000 minidevice-2.0.8/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1498 2023-06-24 07:22:12.000000 minidevice-2.0.8/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      515 2023-06-24 07:15:12.000000 minidevice-2.0.8/minidevice/scrcpycap.py
+-rw-rw-rw-   0        0        0      905 2023-06-24 07:22:50.000000 minidevice-2.0.8/minidevice/scrcpytouch.py
+-rw-rw-rw-   0        0        0      687 2023-06-21 07:24:32.000000 minidevice-2.0.8/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      620 2023-06-24 07:21:44.000000 minidevice-2.0.8/minidevice/touch.py
+-rw-rw-rw-   0        0        0     7503 2023-06-22 06:33:34.000000 minidevice-2.0.8/minidevice/win.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:13:29.874164 minidevice-2.0.8/minidevice.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-06-24 08:13:29.000000 minidevice-2.0.8/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2023-06-24 08:13:29.000000 minidevice-2.0.8/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 08:13:29.000000 minidevice-2.0.8/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-24 08:13:29.000000 minidevice-2.0.8/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 08:13:29.000000 minidevice-2.0.8/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 08:13:29.876531 minidevice-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      825 2023-06-24 07:59:49.000000 minidevice-2.0.8/setup.py
```

### Comparing `minidevice-2.0.7/minidevice/DroidCast.py` & `minidevice-2.0.8/minidevice/DroidCast.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 
 WORK_DIR = os.path.dirname(__file__)
 APK_PATH = "{}/bin/DroidCast-debug-1.1.0.apk".format(WORK_DIR)
 APK_ANDROID_PATH = "/data/local/tmp/DroidCast-debug-1.0.apk"
 
 class DroidCast(ScreenCap):
     def __init__(self, device, DroidCastServerPort=53516) -> None:
+        """
+        __init__ DroidCast截图方法
+
+        Args:
+            device (str): 设备id
+            DroidCastServerPort (int, optional): DroidCastServerPort服务端端口号. Defaults to 53516.
+        """
         self.droidcast_adb = ADB(device)
         self.DroidCastServerPort = DroidCastServerPort
         self.class_path = APK_ANDROID_PATH 
         self.DroidCastSession = requests.Session()
         self.__install()
         self.__start()
```

### Comparing `minidevice-2.0.7/minidevice/QueueUtils.py` & `minidevice-2.0.8/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.7/minidevice/images.py` & `minidevice-2.0.8/minidevice/images.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.7/minidevice/minicap.py` & `minidevice-2.0.8/minidevice/minicap.py`

 * *Files 5% similar despite different names*

```diff
@@ -194,30 +194,35 @@
             self.minicapSocket.close()  # 关闭 minicap 的 socket 连接
 
 
 class Minicap(ScreenCap):
     def __init__(
         self,
         device,
-        minicap_name=None,
         rate=15,
         quality=100,
         use_stream=True,
-        ip="127.0.0.1",
     ) -> None:
+        """
+        __init__ minicap截图方式
+
+        Args:
+            device (str): 设备id
+            rate (int, optional): 截图帧率. Defaults to 15.
+            quality (int, optional): 截图品质1~100之间. Defaults to 100.
+            use_stream (bool, optional): 是否使用stream的方式. Defaults to True.
+        """
         self.minicap_adb = ADB(device)
         self.use_stream = use_stream
         self.__get_device_info()
-        if minicap_name is None:
-            minicap_name = "minicap_{}".format(time.time())
+        minicap_name = "minicap_{}".format(time.time())
         minicap_params = {
             "minicap_name": minicap_name,
             "rate": rate,
             "quality": quality,
-            "ip": ip,
         }
         self.__get_minicap_params(**minicap_params)
         if self.use_stream:
             self.__start_minicap_by_stream()
 
     def screencap_raw(self) -> bytes:
         if self.use_stream:
@@ -286,15 +291,14 @@
         self.minicap_adb.push_file(
             f"{MINICAPSO_PATH}/android-{self.sdk}/{self.abi}/minicap.so", MNC_SO_HOME
         )
         self.minicap_adb.change_file_permission("+x", MNC_HOME)
 
     @__minicap_available
     def __start_minicap(self):
-        """启动adb"""
         adb_command = [ADB_PATH]
         if self.minicap_adb.device is not None:
             adb_command.extend(["-s", self.minicap_adb.device])
         adb_command.extend(
             ["shell", "LD_LIBRARY_PATH=/data/local/tmp", "/data/local/tmp/minicap"]
         )
         adb_command.extend(["-n", f"{self.minicap_name}"])
@@ -306,15 +310,14 @@
             adb_command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
         )
         time.sleep(2)
         logger.info("启动minicap")
         return True
 
     def __forward_minicap(self):
-        """端口转发"""
         self.minicap_port = self.minicap_adb.forward_port(
             "localabstract:{}".format(self.minicap_name)
         )
 
     def __read_minicap_stream(self):
         self.minicap_stream = MinicapStream.getBuilder(self.ip, self.minicap_port)
         self.minicap_stream.run()
```

### Comparing `minidevice-2.0.7/minidevice/minitouch.py` & `minidevice-2.0.8/minidevice/minitouch.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,47 +7,38 @@
 
 WORK_DIR = os.path.dirname(__file__)
 MINITOUCH_PATH = "{}/bin/minitouch/libs".format(WORK_DIR)
 
 
 class Minitouch(Touch, MNTDevice):
     def __init__(self, device):
+        """
+        __init__ minitouch点击方式
+
+        Args:
+            device (str): 设备id
+        """
         self.minitouch_adb = ADB(device)
         self.__get_device_info()
         self.__minitouch_install()
         MNTDevice.__init__(self, device)
 
     def __get_device_info(self):
         self.abi = self.minitouch_adb.get_abi()
 
     def __minitouch_install(self):
         MNT_HOME = "/data/local/tmp/minitouch"
         self.minitouch_adb.push_file(f"{MINITOUCH_PATH}/{self.abi}/minitouch", MNT_HOME)
         self.minitouch_adb.change_file_permission("+x", MNT_HOME)
 
     def click(self, x: int, y: int, duration: int = 100):
-        """
-        click minitouch 点击
-
-        Args:
-            x (int): 横坐标
-            y (int): 纵坐标
-            duration (int, optional): 持续时间. Defaults to 100.
-        """
         MNTDevice.tap(self, [(x, y)], duration=duration)
         logger.debug(f"minitouch click ({x},{y}) consume:{duration}ms")
 
     def swipe(self, points: list, duration: int = 300):
-        """
-        swipe 滑动
-
-        Args:
-            points (list): [(x,y),(x,y),(x,y)] 坐标列表
-            duration (int): 持续时间. Defaults to 300.
-        """
         MNTDevice.swipe(self, points, duration=duration)
         logger.debug(
             f"minitouch swipe from ({points[0]}) to ({points[-1]}) consume:{duration}ms"
         )
 
     def __del__(self):
         MNTDevice.stop(self)
```

### Comparing `minidevice-2.0.7/minidevice/screencap.py` & `minidevice-2.0.8/minidevice/screencap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.7/setup.py` & `minidevice-2.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.0.7',
+      version='2.0.8',
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
-      install_requires=['opencv-python>=4.7.0.72',
-                        'pyminitouch>=0.3.3'
+      install_requires=['opencv-python',
+                        'pyminitouch',
+                        'scrcpy-client',
+                        'requests>=2.31.0',
                         ],
       python_requires='>=3'
       )
```

