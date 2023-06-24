# Comparing `tmp/APIxoo-0.3.0.tar.gz` & `tmp/APIxoo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "APIxoo-0.3.0.tar", last modified: Thu Jun  1 11:30:59 2023, max compression
+gzip compressed data, was "APIxoo-0.3.1.tar", last modified: Sat Jun 24 02:48:22 2023, max compression
```

## Comparing `APIxoo-0.3.0.tar` & `APIxoo-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:30:59.852181 APIxoo-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:30:59.848181 APIxoo-0.3.0/APIxoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-01 11:30:59.000000 APIxoo-0.3.0/APIxoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 11:30:59.000000 APIxoo-0.3.0/APIxoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:30:59.000000 APIxoo-0.3.0/APIxoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 11:30:59.000000 APIxoo-0.3.0/APIxoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 11:30:59.000000 APIxoo-0.3.0/APIxoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-01 11:30:48.000000 APIxoo-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-01 11:30:59.852181 APIxoo-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-01 11:30:48.000000 APIxoo-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:30:59.852181 APIxoo-0.3.0/apixoo/
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-01 11:30:48.000000 APIxoo-0.3.0/apixoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-01 11:30:48.000000 APIxoo-0.3.0/apixoo/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-01 11:30:48.000000 APIxoo-0.3.0/apixoo/pixel_bean.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-01 11:30:48.000000 APIxoo-0.3.0/apixoo/pixel_bean_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:30:59.852181 APIxoo-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 11:30:48.000000 APIxoo-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:48:22.802231 APIxoo-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:48:22.802231 APIxoo-0.3.1/APIxoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-24 02:48:22.000000 APIxoo-0.3.1/APIxoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-24 02:48:22.000000 APIxoo-0.3.1/APIxoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 02:48:22.000000 APIxoo-0.3.1/APIxoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 02:48:22.000000 APIxoo-0.3.1/APIxoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 02:48:22.000000 APIxoo-0.3.1/APIxoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-24 02:48:11.000000 APIxoo-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-24 02:48:22.802231 APIxoo-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-24 02:48:11.000000 APIxoo-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:48:22.802231 APIxoo-0.3.1/apixoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-24 02:48:11.000000 APIxoo-0.3.1/apixoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-24 02:48:11.000000 APIxoo-0.3.1/apixoo/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-24 02:48:11.000000 APIxoo-0.3.1/apixoo/pixel_bean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-24 02:48:11.000000 APIxoo-0.3.1/apixoo/pixel_bean_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 02:48:22.802231 APIxoo-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-24 02:48:11.000000 APIxoo-0.3.1/setup.py
```

### Comparing `APIxoo-0.3.0/APIxoo.egg-info/PKG-INFO` & `APIxoo-0.3.1/APIxoo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APIxoo
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python wrapper for Divoom Pixoo server API
 Home-page: https://github.com/redphx/apixoo
 Download-URL: https://github.com/redphx/apixoo
 Author: redphx
 License: MIT
 Keywords: apixoo,divoom,pixoo,pixoo64
 Platform: any
```

### Comparing `APIxoo-0.3.0/LICENSE.md` & `APIxoo-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `APIxoo-0.3.0/PKG-INFO` & `APIxoo-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: APIxoo
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python wrapper for Divoom Pixoo server API
 Home-page: https://github.com/redphx/apixoo
 Download-URL: https://github.com/redphx/apixoo
 Author: redphx
 License: MIT
 Keywords: apixoo,divoom,pixoo,pixoo64
 Platform: any
```

### Comparing `APIxoo-0.3.0/README.md` & `APIxoo-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `APIxoo-0.3.0/apixoo/__init__.py` & `APIxoo-0.3.1/apixoo/__init__.py`

 * *Files identical despite different names*

### Comparing `APIxoo-0.3.0/apixoo/const.py` & `APIxoo-0.3.1/apixoo/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from enum import Enum
 
 
 class GalleryCategory(int, Enum):
     NEW = 0
     DEFAULT = 1
-    LED_TEXT = 2
+    # LED_TEXT = 2
     CHARACTER = 3
     EMOJI = 4
     DAILY = 5
     NATURE = 6
     SYMBOL = 7
     PATTERN = 8
     CREATIVE = 9
     PHOTO = 12
     TOP = 14
     GADGET = 15
     BUSINESS = 16
     FESTIVAL = 17
     RECOMMEND = 18
-    PLANET = 19
+    # PLANET = 19
     FOLLOW = 20
-    REVIEW_PHOTOS = 21
-    REVIEW_STOLEN_PHOTOS = 22
-    FILL_GAME = 29
+    # REVIEW_PHOTOS = 21
+    # REVIEW_STOLEN_PHOTOS = 22
+    # FILL_GAME = 29
     PIXEL_MATCH = 30  # Current event
     PLANT = 31
     ANIMAL = 32
     PERSON = 33
     EMOJI_2 = 34
     FOOD = 35
-    OTHERS = 36
-    REPORT_PHOTO = 254
-    CREATION_ALBUM = 255
+    # OTHERS = 36
+    # REPORT_PHOTO = 254
+    # CREATION_ALBUM = 255
 
 
 class GalleryType(int, Enum):
     PICTURE = 0
     ANIMATION = 1
     MULTI_PICTURE = 2
     MULTI_ANIMATION = 3
```

### Comparing `APIxoo-0.3.0/apixoo/pixel_bean.py` & `APIxoo-0.3.1/apixoo/pixel_bean.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         target_height: int = None,
     ) -> None:
         """Convert animation to GIF file"""
         gif_frames = []
 
         for frame_number in range(self._total_frames):
             img = self.get_frame_image(
-                frame_number,
+                frame_number + 1,
                 scale=scale,
                 target_width=target_width,
                 target_height=target_height,
             )
             gif_frames.append(img)
 
         # Save to GIF
```

### Comparing `APIxoo-0.3.0/apixoo/pixel_bean_decoder.py` & `APIxoo-0.3.1/apixoo/pixel_bean_decoder.py`

 * *Files identical despite different names*

### Comparing `APIxoo-0.3.0/setup.py` & `APIxoo-0.3.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from distutils.core import setup
 
 long_desc = open("README.md").read()
 required = ['requests']
 
 setup(
     name='APIxoo',
-    version="0.3.0",
+    version="0.3.1",
     author="redphx",
     license="MIT",
     url="https://github.com/redphx/apixoo",
     download_url="https://github.com/redphx/apixoo",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     description="Python wrapper for Divoom Pixoo server API",
```

