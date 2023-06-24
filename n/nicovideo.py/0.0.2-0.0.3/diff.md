# Comparing `tmp/nicovideo.py-0.0.2.tar.gz` & `tmp/nicovideo.py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicovideo.py-0.0.2.tar", last modified: Sat Jun 24 10:10:07 2023, max compression
+gzip compressed data, was "nicovideo.py-0.0.3.tar", last modified: Sat Jun 24 13:38:19 2023, max compression
```

## Comparing `nicovideo.py-0.0.2.tar` & `nicovideo.py-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-06-24 10:10:07.582972 nicovideo.py-0.0.2/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     7559 2023-06-24 05:49:10.000000 nicovideo.py-0.0.2/LICENSE.md
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     3057 2023-06-24 10:10:07.582972 nicovideo.py-0.0.2/PKG-INFO
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     2302 2023-06-24 05:53:31.000000 nicovideo.py-0.0.2/README.md
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-06-24 10:10:07.582972 nicovideo.py-0.0.2/nicovideo/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     3879 2023-06-24 10:06:19.000000 nicovideo.py-0.0.2/nicovideo/__init__.py
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-06-24 10:10:07.582972 nicovideo.py-0.0.2/nicovideo.py.egg-info/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     3057 2023-06-24 10:10:07.000000 nicovideo.py-0.0.2/nicovideo.py.egg-info/PKG-INFO
--rw-rw-r--   0 okaits    (1000) okaits    (1000)      195 2023-06-24 10:10:07.000000 nicovideo.py-0.0.2/nicovideo.py.egg-info/SOURCES.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)        1 2023-06-24 10:10:07.000000 nicovideo.py-0.0.2/nicovideo.py.egg-info/dependency_links.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)       10 2023-06-24 10:10:07.000000 nicovideo.py-0.0.2/nicovideo.py.egg-info/top_level.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)       38 2023-06-24 10:10:07.582972 nicovideo.py-0.0.2/setup.cfg
--rw-rw-r--   0 okaits    (1000) okaits    (1000)      976 2023-06-24 10:09:21.000000 nicovideo.py-0.0.2/setup.py
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-06-24 13:38:19.690008 nicovideo.py-0.0.3/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     7559 2023-06-24 05:49:10.000000 nicovideo.py-0.0.3/LICENSE.md
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     3057 2023-06-24 13:38:19.686007 nicovideo.py-0.0.3/PKG-INFO
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     2302 2023-06-24 05:53:31.000000 nicovideo.py-0.0.3/README.md
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-06-24 13:38:19.682007 nicovideo.py-0.0.3/nicovideo/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     4430 2023-06-24 13:37:46.000000 nicovideo.py-0.0.3/nicovideo/__init__.py
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-06-24 13:38:19.686007 nicovideo.py-0.0.3/nicovideo.py.egg-info/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     3057 2023-06-24 13:38:19.000000 nicovideo.py-0.0.3/nicovideo.py.egg-info/PKG-INFO
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)      195 2023-06-24 13:38:19.000000 nicovideo.py-0.0.3/nicovideo.py.egg-info/SOURCES.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)        1 2023-06-24 13:38:19.000000 nicovideo.py-0.0.3/nicovideo.py.egg-info/dependency_links.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)       10 2023-06-24 13:38:19.000000 nicovideo.py-0.0.3/nicovideo.py.egg-info/top_level.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)       38 2023-06-24 13:38:19.690008 nicovideo.py-0.0.3/setup.cfg
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)      976 2023-06-24 13:37:51.000000 nicovideo.py-0.0.3/setup.py
```

### Comparing `nicovideo.py-0.0.2/LICENSE.md` & `nicovideo.py-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nicovideo.py-0.0.2/PKG-INFO` & `nicovideo.py-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicovideo.py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Get nicovideo's video metadata.
 Home-page: https://github.com/okaits/nicovideo.py
 Author: okaits#7534
 Author-email: okaits@okaits7534.mydns.jp
 License: GNU Lesser General Public License 3.0
 Keywords: nicovideo
 Platform: UNKNOWN
```

### Comparing `nicovideo.py-0.0.2/README.md` & `nicovideo.py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nicovideo.py-0.0.2/nicovideo/__init__.py` & `nicovideo.py-0.0.3/nicovideo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ nicovideo.py (video) """
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 import pprint
 import urllib.request
 from html import unescape
 import datetime
 
 import json5
@@ -21,34 +21,46 @@
         """ Meta data """
 
         class User():
             """ User data """
             def __init__(self, nickname: str, videoid: str):
                 self.nickname: str = nickname
                 self.id      : str = videoid #pylint: disable=C0103
+            def __str__(self):
+                return f'{self.nickname} [ID: {self.id}]'
 
         class Counts():
             """ Counts data """
             def __init__(self, comments: int, likes: int, mylists: int, views: int):
                 self.comments: int = comments
                 self.likes   : int = likes
                 self.mylists : int = mylists
                 self.views   : int = views
+            def __str__(self):
+                returndata = f'Comments: {self.comments}\n'
+                returndata += f'Likes: {self.likes}\n'
+                returndata += f'Mylists: {self.mylists}\n'
+                returndata += f'Views: {self.views}'
+                return returndata
 
         class Genre():
             """ Genre data """
             def __init__(self, label, key):
                 self.label   : str = label
                 self.key     : str = key
+            def __str__(self):
+                return self.label
 
         class Tag():
             """ Tag data """
             def __init__(self, name: str, locked: bool):
                 self.name  : str  = name
                 self.locked: bool = locked
+            def __str__(self):
+                return f'{self.name}{" [Locked]" if self.locked else ""}'
 
         def __init__(
                 self,
                 videoid : str,
                 title   : str,
                 owner   : User,
                 counts  : Counts,
```

### Comparing `nicovideo.py-0.0.2/nicovideo.py.egg-info/PKG-INFO` & `nicovideo.py-0.0.3/nicovideo.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicovideo.py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Get nicovideo's video metadata.
 Home-page: https://github.com/okaits/nicovideo.py
 Author: okaits#7534
 Author-email: okaits@okaits7534.mydns.jp
 License: GNU Lesser General Public License 3.0
 Keywords: nicovideo
 Platform: UNKNOWN
```

### Comparing `nicovideo.py-0.0.2/setup.py` & `nicovideo.py-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_packages, setup
 
 readme = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='nicovideo.py',
-    version='0.0.2',
+    version='0.0.3',
     description='Get nicovideo\'s video metadata.',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='okaits#7534',
     author_email='okaits@okaits7534.mydns.jp',
     url='https://github.com/okaits/nicovideo.py',
     classifiers=[
```

