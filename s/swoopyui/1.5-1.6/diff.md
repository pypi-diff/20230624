# Comparing `tmp/swoopyui-1.5.tar.gz` & `tmp/swoopyui-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoopyui-1.5.tar", last modified: Thu May 25 15:47:22 2023, max compression
+gzip compressed data, was "swoopyui-1.6.tar", last modified: Sat Jun 24 19:21:54 2023, max compression
```

## Comparing `swoopyui-1.5.tar` & `swoopyui-1.6.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.640205 swoopyui-1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 15:47:10.000000 swoopyui-1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 15:47:10.000000 swoopyui-1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-25 15:47:22.640205 swoopyui-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-25 15:47:10.000000 swoopyui-1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-25 15:47:10.000000 swoopyui-1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:47:22.640205 swoopyui-1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-25 15:47:10.000000 swoopyui-1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui/UIkits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/UIkits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   339523 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/assets/swoopyui.zip
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/swoopyui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/check_if_mac.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/on_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/pyinstaller_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/run_swiftUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/run_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/unzip_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/navigationlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/navigationstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/navigationview.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/scrollview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.640205 swoopyui-1.5/swoopyui/views/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/shapes/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/spacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/textfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-25 15:47:22.000000 swoopyui-1.5/swoopyui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 15:47:22.000000 swoopyui-1.5/swoopyui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:47:22.000000 swoopyui-1.5/swoopyui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-25 15:47:22.000000 swoopyui-1.5/swoopyui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 15:47:22.000000 swoopyui-1.5/swoopyui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:54.388429 swoopyui-1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-24 19:21:44.000000 swoopyui-1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-24 19:21:44.000000 swoopyui-1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-24 19:21:54.388429 swoopyui-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-24 19:21:44.000000 swoopyui-1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 19:21:44.000000 swoopyui-1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:21:54.388429 swoopyui-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-24 19:21:44.000000 swoopyui-1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:54.384429 swoopyui-1.6/swoopyui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:54.384429 swoopyui-1.6/swoopyui/UIkits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/UIkits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:54.384429 swoopyui-1.6/swoopyui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   693026 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/assets/swoopyui.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/swoopyui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:54.388429 swoopyui-1.6/swoopyui/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/tools/check_if_mac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/tools/on_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/tools/pyinstaller_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/tools/run_swiftUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/tools/run_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/tools/unzip_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:54.388429 swoopyui-1.6/swoopyui/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/animatedview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/navigationlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/navigationstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/navigationview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/scrollview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:54.388429 swoopyui-1.6/swoopyui/views/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/shapes/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/spacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/textfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-24 19:21:44.000000 swoopyui-1.6/swoopyui/views/webview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:21:54.384429 swoopyui-1.6/swoopyui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-24 19:21:54.000000 swoopyui-1.6/swoopyui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-24 19:21:54.000000 swoopyui-1.6/swoopyui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:21:54.000000 swoopyui-1.6/swoopyui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-24 19:21:54.000000 swoopyui-1.6/swoopyui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 19:21:54.000000 swoopyui-1.6/swoopyui.egg-info/top_level.txt
```

### Comparing `swoopyui-1.5/LICENSE` & `swoopyui-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/PKG-INFO` & `swoopyui-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoopyui
-Version: 1.5
+Version: 1.6
 Summary: A python library that allow you to build swiftUI apps using python.
 Home-page: https://github.com/SKbarbon/swoopyui
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `swoopyui-1.5/README.md` & `swoopyui-1.6/README.md`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/setup.py` & `swoopyui-1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_des = str(f.read())
 
 setup(
     name='swoopyui',
-    version='1.5',
+    version='1.6',
     author='SKbarbon',
     description='A python library that allow you to build swiftUI apps using python.',
     long_description=long_des,
     long_description_content_type='text/markdown',
     url='https://github.com/SKbarbon/swoopyui',
     install_requires=["flask", "requests"],
     packages=find_packages(),
```

### Comparing `swoopyui-1.5/swoopyui/__init__.py` & `swoopyui-1.6/swoopyui/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,9 +12,12 @@
 from .views.navigationstack import NavigationStack
 from .views.navigationlink import NavigationLink
 from .views.textfield import TextField
 from .views.stack import Stack, VSTACK, HSTACK, ZSTACK
 from .views.scrollview import ScrollView
 from .views.spacer import Spacer
 from .views.list import List
+from .views.image import Image
+from .views.webview import WebView
+from .views.animatedview import AnimatedView
 
 from .views.shapes.circle import Circle
```

### Comparing `swoopyui-1.5/swoopyui/protocol.py` & `swoopyui-1.6/swoopyui/protocol.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/swoopyui/swoopyui.py` & `swoopyui-1.6/swoopyui/swoopyui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from flask import Flask, request
+from flask import Flask, request, send_file
 import socketserver
 import tempfile
 import threading
 import logging
 import shutil
 import os
 import sys
@@ -52,14 +52,24 @@
                 action_content = next_update["action_content"]
                 update_number = next_update["update_number"]
                 del self.__all_waited_updates[0]
                 return onClientRequestUpdate(
                     update_number, 
                     action_name, 
                     action_content).load_as_dict()
+        
+
+        @flask_app.route("/get_assets")
+        def get_assets ():
+            path = request.values['path']
+            if os.path.isfile (path):
+                return send_file (path)
+            else:
+                return "error"
+
 
         @flask_app.route("/start_the_target_function")
         def start_the_target_function ():
             threading.Thread(target=run_the_target, args=[self.__target_function, [self.__main_view], self], daemon=True).start()
             return ""
         
         @flask_app.route("/client_side_update", methods=["POST"])
@@ -78,14 +88,15 @@
             if os.path.isdir (self.current_tmp_dir):
                 shutil.rmtree(self.current_tmp_dir)
             # exit the script.
             os._exit(0)
 
         with socketserver.TCPServer(("localhost", 0), None) as s:
             free_port = s.server_address[1]
+            self.app_port = free_port
         
         if is_run_on_pyinstaller():
             self.current_tmp_dir = getattr(sys, "_MEIPASS", os.path.dirname(os.path.abspath(__file__)))
         else:
             self.current_tmp_dir = tempfile.mkdtemp()
         threading.Thread(target=run_swiftUI_on_new_process, args=[free_port, self.current_tmp_dir]).start()
         flask_app.run(port=free_port)
```

### Comparing `swoopyui-1.5/swoopyui/tools/run_swiftUI.py` & `swoopyui-1.6/swoopyui/tools/run_swiftUI.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/swoopyui/views/button.py` & `swoopyui-1.6/swoopyui/views/button.py`

 * *Files 9% similar despite different names*

```diff
@@ -92,16 +92,19 @@
         return self.__width
     
     @width.setter
     def width (self, value):
         if self.__mother_view == None:
             raise Exception("Cannot change the sub_view property while its not on the screen.")
         
-        if not isinstance(value, float) or not isinstance(value, int):
-            raise ValueError(f"width must be a number")
+        try:
+            int(value)
+        except:
+            raise ValueError(f"height must be a number")
+        
         self.__width = value
         self.__id = self.__mother_view.get_new_view_id()
         self.__mother_view.update(self)
         self.__last_view_id = self.__id
     
 
     @property
@@ -109,13 +112,16 @@
         return self.__height
     
     @height.setter
     def height (self, value):
         if self.__mother_view == None:
             raise Exception("Cannot change the sub_view property while its not on the screen.")
         
-        if not isinstance(value, float) or not isinstance(value, int):
+        try:
+            int(value)
+        except:
             raise ValueError(f"height must be a number")
+        
         self.__height = value
         self.__id = self.__mother_view.get_new_view_id()
         self.__mother_view.update(self)
         self.__last_view_id = self.__id
```

### Comparing `swoopyui-1.5/swoopyui/views/list.py` & `swoopyui-1.6/swoopyui/views/list.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/swoopyui/views/navigationlink.py` & `swoopyui-1.6/swoopyui/views/navigationlink.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/swoopyui/views/navigationstack.py` & `swoopyui-1.6/swoopyui/views/navigationstack.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/swoopyui/views/navigationview.py` & `swoopyui-1.6/swoopyui/views/navigationview.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/swoopyui/views/scrollview.py` & `swoopyui-1.6/swoopyui/views/scrollview.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/swoopyui/views/shapes/circle.py` & `swoopyui-1.6/swoopyui/views/shapes/circle.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/swoopyui/views/spacer.py` & `swoopyui-1.6/swoopyui/views/spacer.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/swoopyui/views/stack.py` & `swoopyui-1.6/swoopyui/views/stack.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/swoopyui/views/text.py` & `swoopyui-1.6/swoopyui/views/text.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.5/swoopyui/views/textfield.py` & `swoopyui-1.6/swoopyui/views/textfield.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,16 +95,19 @@
         return self.__width
     
     @width.setter
     def width (self, value):
         if self.__mother_view == None:
             raise Exception("Cannot change the sub_view property while its not on the screen.")
         
-        if not isinstance(value, float) or not isinstance(value, int):
-            raise ValueError(f"width must be a number")
+        try:
+            int(value)
+        except:
+            raise ValueError(f"height must be a number")
+        
         self.__width = value
         self.__id = self.__mother_view.get_new_view_id()
         self.__mother_view.update(self)
         self.__last_view_id = self.__id
     
 
     @property
@@ -112,16 +115,19 @@
         return self.__height
     
     @height.setter
     def height (self, value):
         if self.__mother_view == None:
             raise Exception("Cannot change the sub_view property while its not on the screen.")
         
-        if not isinstance(value, float) or not isinstance(value, int):
+        try:
+            int(value)
+        except:
             raise ValueError(f"height must be a number")
+        
         self.__height = value
         self.__id = self.__mother_view.get_new_view_id()
         self.__mother_view.update(self)
         self.__last_view_id = self.__id
     
     @property
     def foreground_color (self): return self.__foreground_color
```

### Comparing `swoopyui-1.5/swoopyui.egg-info/PKG-INFO` & `swoopyui-1.6/swoopyui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoopyui
-Version: 1.5
+Version: 1.6
 Summary: A python library that allow you to build swiftUI apps using python.
 Home-page: https://github.com/SKbarbon/swoopyui
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `swoopyui-1.5/swoopyui.egg-info/SOURCES.txt` & `swoopyui-1.6/swoopyui.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,19 +19,22 @@
 swoopyui/tools/check_if_mac.py
 swoopyui/tools/on_action.py
 swoopyui/tools/pyinstaller_check.py
 swoopyui/tools/run_swiftUI.py
 swoopyui/tools/run_target.py
 swoopyui/tools/unzip_assets.py
 swoopyui/views/__init__.py
+swoopyui/views/animatedview.py
 swoopyui/views/button.py
+swoopyui/views/image.py
 swoopyui/views/list.py
 swoopyui/views/navigationlink.py
 swoopyui/views/navigationstack.py
 swoopyui/views/navigationview.py
 swoopyui/views/scrollview.py
 swoopyui/views/spacer.py
 swoopyui/views/stack.py
 swoopyui/views/text.py
 swoopyui/views/textfield.py
+swoopyui/views/webview.py
 swoopyui/views/shapes/__init__.py
 swoopyui/views/shapes/circle.py
```

