# Comparing `tmp/uitk-0.7.0.tar.gz` & `tmp/uitk-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uitk-0.7.0.tar", last modified: Sat Jun 24 02:39:07 2023, max compression
+gzip compressed data, was "uitk-0.7.1.tar", last modified: Sat Jun 24 02:39:57 2023, max compression
```

## Comparing `uitk-0.7.0.tar` & `uitk-0.7.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 02:39:07.965526 uitk-0.7.0/
--rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-0.7.0/COPYING.LESSER
--rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3650 2023-06-24 02:39:07.963543 uitk-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-24 02:39:07.965526 uitk-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     2455 2023-06-22 16:49:58.000000 uitk-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:39:07.921570 uitk-0.7.0/uitk/
--rw-rw-rw-   0        0        0     2860 2023-06-24 02:39:04.000000 uitk-0.7.0/uitk/__init__.py
--rw-rw-rw-   0        0        0    14530 2023-05-20 02:32:52.000000 uitk-0.7.0/uitk/events.py
--rw-rw-rw-   0        0        0   102708 2023-06-23 22:14:06.000000 uitk-0.7.0/uitk/switchboard.py
--rw-rw-rw-   0        0        0   104164 2023-06-18 15:45:21.000000 uitk-0.7.0/uitk/switchboard.py.bak
-drwxrwxrwx   0        0        0        0 2023-06-24 02:39:07.954295 uitk-0.7.0/uitk/widgets/
--rw-rw-rw-   0        0        0    18485 2023-06-20 17:13:55.000000 uitk-0.7.0/uitk/widgets/MainWindow.py
--rw-rw-rw-   0        0        0     3204 2023-05-24 20:56:51.000000 uitk-0.7.0/uitk/widgets/__init__.py
--rw-rw-rw-   0        0        0    15870 2023-06-24 02:15:31.000000 uitk-0.7.0/uitk/widgets/attributeWindow.py
--rw-rw-rw-   0        0        0     4207 2023-06-02 17:31:37.000000 uitk-0.7.0/uitk/widgets/checkBox.py
--rw-rw-rw-   0        0        0     8332 2023-06-20 19:15:01.000000 uitk-0.7.0/uitk/widgets/comboBox.py
--rw-rw-rw-   0        0        0     7036 2023-06-10 13:16:59.000000 uitk-0.7.0/uitk/widgets/draggableHeader.py
--rw-rw-rw-   0        0        0    22380 2023-06-02 21:56:26.000000 uitk-0.7.0/uitk/widgets/expandableList.py
--rw-rw-rw-   0        0        0     2498 2023-06-02 17:31:37.000000 uitk-0.7.0/uitk/widgets/label.py
--rw-rw-rw-   0        0        0     3295 2023-06-15 19:41:53.000000 uitk-0.7.0/uitk/widgets/lineEdit.py
--rw-rw-rw-   0        0        0    23456 2023-06-19 14:36:41.000000 uitk-0.7.0/uitk/widgets/menu.py
--rw-rw-rw-   0        0        0     8559 2023-06-23 14:22:44.000000 uitk-0.7.0/uitk/widgets/messageBox.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:39:07.962522 uitk-0.7.0/uitk/widgets/mixins/
--rw-rw-rw-   0        0        0     3028 2023-05-12 17:13:16.000000 uitk-0.7.0/uitk/widgets/mixins/__init__.py
--rw-rw-rw-   0        0        0    12559 2023-06-22 01:40:58.000000 uitk-0.7.0/uitk/widgets/mixins/attributes.py
--rw-rw-rw-   0        0        0     4023 2023-05-12 17:25:02.000000 uitk-0.7.0/uitk/widgets/mixins/convert.py
--rw-rw-rw-   0        0        0     9499 2023-05-20 02:33:14.000000 uitk-0.7.0/uitk/widgets/mixins/docking.py
--rw-rw-rw-   0        0        0     5044 2023-06-17 23:02:35.000000 uitk-0.7.0/uitk/widgets/mixins/menu_instance.py
--rw-rw-rw-   0        0        0     1967 2023-05-12 17:25:39.000000 uitk-0.7.0/uitk/widgets/mixins/state_manager.py
--rw-rw-rw-   0        0        0    48184 2023-06-24 02:14:57.000000 uitk-0.7.0/uitk/widgets/mixins/style_sheet.py
--rw-rw-rw-   0        0        0     3409 2023-05-12 17:27:14.000000 uitk-0.7.0/uitk/widgets/mixins/tasks.py
--rw-rw-rw-   0        0        0    11099 2023-05-12 17:26:59.000000 uitk-0.7.0/uitk/widgets/mixins/text.py
--rw-rw-rw-   0        0        0     6204 2023-06-10 12:44:09.000000 uitk-0.7.0/uitk/widgets/optionBox.py
--rw-rw-rw-   0        0        0     3278 2023-06-05 16:23:13.000000 uitk-0.7.0/uitk/widgets/progressBar.py
--rw-rw-rw-   0        0        0     3069 2023-06-15 19:57:41.000000 uitk-0.7.0/uitk/widgets/pushButton.py
--rw-rw-rw-   0        0        0     7907 2023-05-28 21:08:35.000000 uitk-0.7.0/uitk/widgets/region.py
--rw-rw-rw-   0        0        0     3709 2023-06-12 14:42:27.000000 uitk-0.7.0/uitk/widgets/textEdit.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:39:07.936154 uitk-0.7.0/uitk.egg-info/
--rw-rw-rw-   0        0        0     3650 2023-06-24 02:39:07.000000 uitk-0.7.0/uitk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4282 2023-05-11 02:02:25.000000 uitk-0.7.0/uitk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0     1022 2023-06-24 02:39:07.000000 uitk-0.7.0/uitk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      767 2023-04-15 12:48:17.000000 uitk-0.7.0/uitk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-06-24 02:39:07.000000 uitk-0.7.0/uitk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-24 02:39:07.000000 uitk-0.7.0/uitk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 02:39:57.765365 uitk-0.7.1/
+-rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-0.7.1/COPYING.LESSER
+-rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3650 2023-06-24 02:39:57.764365 uitk-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-24 02:39:57.765365 uitk-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     2455 2023-06-22 16:49:58.000000 uitk-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:39:57.722664 uitk-0.7.1/uitk/
+-rw-rw-rw-   0        0        0     2860 2023-06-24 02:39:54.000000 uitk-0.7.1/uitk/__init__.py
+-rw-rw-rw-   0        0        0    14530 2023-05-20 02:32:52.000000 uitk-0.7.1/uitk/events.py
+-rw-rw-rw-   0        0        0   102708 2023-06-23 22:14:06.000000 uitk-0.7.1/uitk/switchboard.py
+-rw-rw-rw-   0        0        0   104164 2023-06-18 15:45:21.000000 uitk-0.7.1/uitk/switchboard.py.bak
+drwxrwxrwx   0        0        0        0 2023-06-24 02:39:57.754298 uitk-0.7.1/uitk/widgets/
+-rw-rw-rw-   0        0        0    18485 2023-06-20 17:13:55.000000 uitk-0.7.1/uitk/widgets/MainWindow.py
+-rw-rw-rw-   0        0        0     3204 2023-05-24 20:56:51.000000 uitk-0.7.1/uitk/widgets/__init__.py
+-rw-rw-rw-   0        0        0    15870 2023-06-24 02:15:31.000000 uitk-0.7.1/uitk/widgets/attributeWindow.py
+-rw-rw-rw-   0        0        0     4207 2023-06-02 17:31:37.000000 uitk-0.7.1/uitk/widgets/checkBox.py
+-rw-rw-rw-   0        0        0     8332 2023-06-20 19:15:01.000000 uitk-0.7.1/uitk/widgets/comboBox.py
+-rw-rw-rw-   0        0        0     7036 2023-06-10 13:16:59.000000 uitk-0.7.1/uitk/widgets/draggableHeader.py
+-rw-rw-rw-   0        0        0    22380 2023-06-02 21:56:26.000000 uitk-0.7.1/uitk/widgets/expandableList.py
+-rw-rw-rw-   0        0        0     2498 2023-06-02 17:31:37.000000 uitk-0.7.1/uitk/widgets/label.py
+-rw-rw-rw-   0        0        0     3295 2023-06-15 19:41:53.000000 uitk-0.7.1/uitk/widgets/lineEdit.py
+-rw-rw-rw-   0        0        0    23456 2023-06-19 14:36:41.000000 uitk-0.7.1/uitk/widgets/menu.py
+-rw-rw-rw-   0        0        0     8559 2023-06-23 14:22:44.000000 uitk-0.7.1/uitk/widgets/messageBox.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:39:57.763365 uitk-0.7.1/uitk/widgets/mixins/
+-rw-rw-rw-   0        0        0     3028 2023-05-12 17:13:16.000000 uitk-0.7.1/uitk/widgets/mixins/__init__.py
+-rw-rw-rw-   0        0        0    12559 2023-06-22 01:40:58.000000 uitk-0.7.1/uitk/widgets/mixins/attributes.py
+-rw-rw-rw-   0        0        0     4023 2023-05-12 17:25:02.000000 uitk-0.7.1/uitk/widgets/mixins/convert.py
+-rw-rw-rw-   0        0        0     9499 2023-05-20 02:33:14.000000 uitk-0.7.1/uitk/widgets/mixins/docking.py
+-rw-rw-rw-   0        0        0     5044 2023-06-17 23:02:35.000000 uitk-0.7.1/uitk/widgets/mixins/menu_instance.py
+-rw-rw-rw-   0        0        0     1967 2023-05-12 17:25:39.000000 uitk-0.7.1/uitk/widgets/mixins/state_manager.py
+-rw-rw-rw-   0        0        0    48184 2023-06-24 02:14:57.000000 uitk-0.7.1/uitk/widgets/mixins/style_sheet.py
+-rw-rw-rw-   0        0        0     3409 2023-05-12 17:27:14.000000 uitk-0.7.1/uitk/widgets/mixins/tasks.py
+-rw-rw-rw-   0        0        0    11099 2023-05-12 17:26:59.000000 uitk-0.7.1/uitk/widgets/mixins/text.py
+-rw-rw-rw-   0        0        0     6204 2023-06-10 12:44:09.000000 uitk-0.7.1/uitk/widgets/optionBox.py
+-rw-rw-rw-   0        0        0     3278 2023-06-05 16:23:13.000000 uitk-0.7.1/uitk/widgets/progressBar.py
+-rw-rw-rw-   0        0        0     3069 2023-06-15 19:57:41.000000 uitk-0.7.1/uitk/widgets/pushButton.py
+-rw-rw-rw-   0        0        0     7907 2023-05-28 21:08:35.000000 uitk-0.7.1/uitk/widgets/region.py
+-rw-rw-rw-   0        0        0     3709 2023-06-12 14:42:27.000000 uitk-0.7.1/uitk/widgets/textEdit.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:39:57.738717 uitk-0.7.1/uitk.egg-info/
+-rw-rw-rw-   0        0        0     3650 2023-06-24 02:39:57.000000 uitk-0.7.1/uitk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4282 2023-05-11 02:02:25.000000 uitk-0.7.1/uitk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0     1022 2023-06-24 02:39:57.000000 uitk-0.7.1/uitk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      767 2023-04-15 12:48:17.000000 uitk-0.7.1/uitk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-06-24 02:39:57.000000 uitk-0.7.1/uitk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-24 02:39:57.000000 uitk-0.7.1/uitk.egg-info/top_level.txt
```

### Comparing `uitk-0.7.0/COPYING.LESSER` & `uitk-0.7.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/PKG-INFO` & `uitk-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 0.7.0
+Version: 0.7.1
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `uitk-0.7.0/setup.py` & `uitk-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/__init__.py` & `uitk-0.7.1/uitk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import importlib
 import pkgutil
 import inspect
 
 
 __package__ = "uitk"
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 __path__ = [os.path.abspath(os.path.dirname(__file__))]
 
 
 # Define a dictionary to map class names to their respective modules
 CLASS_TO_MODULE = {}
 
 # Build the CLASS_TO_MODULE dictionary by iterating over all submodules of the package
```

### Comparing `uitk-0.7.0/uitk/events.py` & `uitk-0.7.1/uitk/events.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/switchboard.py` & `uitk-0.7.1/uitk/switchboard.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/switchboard.py.bak` & `uitk-0.7.1/uitk/switchboard.py.bak`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/MainWindow.py` & `uitk-0.7.1/uitk/widgets/MainWindow.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/__init__.py` & `uitk-0.7.1/uitk/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/attributeWindow.py` & `uitk-0.7.1/uitk/widgets/attributeWindow.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/checkBox.py` & `uitk-0.7.1/uitk/widgets/checkBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/comboBox.py` & `uitk-0.7.1/uitk/widgets/comboBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/draggableHeader.py` & `uitk-0.7.1/uitk/widgets/draggableHeader.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/expandableList.py` & `uitk-0.7.1/uitk/widgets/expandableList.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/label.py` & `uitk-0.7.1/uitk/widgets/label.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/lineEdit.py` & `uitk-0.7.1/uitk/widgets/lineEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/menu.py` & `uitk-0.7.1/uitk/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/messageBox.py` & `uitk-0.7.1/uitk/widgets/messageBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/mixins/__init__.py` & `uitk-0.7.1/uitk/widgets/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/mixins/attributes.py` & `uitk-0.7.1/uitk/widgets/mixins/attributes.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/mixins/convert.py` & `uitk-0.7.1/uitk/widgets/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/mixins/docking.py` & `uitk-0.7.1/uitk/widgets/mixins/docking.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/mixins/menu_instance.py` & `uitk-0.7.1/uitk/widgets/mixins/menu_instance.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/mixins/state_manager.py` & `uitk-0.7.1/uitk/widgets/mixins/state_manager.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/mixins/style_sheet.py` & `uitk-0.7.1/uitk/widgets/mixins/style_sheet.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/mixins/tasks.py` & `uitk-0.7.1/uitk/widgets/mixins/tasks.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/mixins/text.py` & `uitk-0.7.1/uitk/widgets/mixins/text.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/optionBox.py` & `uitk-0.7.1/uitk/widgets/optionBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/progressBar.py` & `uitk-0.7.1/uitk/widgets/progressBar.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/pushButton.py` & `uitk-0.7.1/uitk/widgets/pushButton.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/region.py` & `uitk-0.7.1/uitk/widgets/region.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk/widgets/textEdit.py` & `uitk-0.7.1/uitk/widgets/textEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk.egg-info/PKG-INFO` & `uitk-0.7.1/uitk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 0.7.0
+Version: 0.7.1
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `uitk-0.7.0/uitk.egg-info/PKG-INFO.bak` & `uitk-0.7.1/uitk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk.egg-info/SOURCES.txt` & `uitk-0.7.1/uitk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uitk-0.7.0/uitk.egg-info/SOURCES.txt.bak` & `uitk-0.7.1/uitk.egg-info/SOURCES.txt.bak`

 * *Files identical despite different names*

