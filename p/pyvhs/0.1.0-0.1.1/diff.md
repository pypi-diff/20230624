# Comparing `tmp/pyvhs-0.1.0.tar.gz` & `tmp/pyvhs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvhs-0.1.0.tar", max compression
+gzip compressed data, was "pyvhs-0.1.1.tar", max compression
```

## Comparing `pyvhs-0.1.0.tar` & `pyvhs-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-06-19 13:27:10.974931 pyvhs-0.1.0/LICENSE
--rw-r--r--   0        0        0     9066 2023-06-24 13:09:49.436740 pyvhs-0.1.0/README.md
--rw-r--r--   0        0        0   176080 2023-06-19 12:45:19.455984 pyvhs-0.1.0/doc/imgs/playback.png
--rw-r--r--   0        0        0   242536 2023-06-19 12:48:00.793752 pyvhs-0.1.0/doc/imgs/pyvhs.png
--rw-r--r--   0        0        0      570 2023-06-24 13:07:22.130287 pyvhs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-19 19:27:59.639929 pyvhs-0.1.0/pyvhs/__init__.py
--rw-r--r--   0        0        0    59151 2023-06-17 12:32:19.507485 pyvhs-0.1.0/pyvhs/template_imgs/template001.png
--rw-r--r--   0        0        0     2321 2023-06-17 12:48:13.782701 pyvhs-0.1.0/pyvhs/template_imgs/template002.png
--rw-r--r--   0        0        0        0 2023-06-18 18:24:43.368411 pyvhs-0.1.0/pyvhs/utils/__init__.py
--rw-r--r--   0        0        0     8282 2023-06-24 11:23:09.359583 pyvhs-0.1.0/pyvhs/utils/edits.py
--rw-r--r--   0        0        0      976 2023-06-22 00:50:19.366984 pyvhs-0.1.0/pyvhs/utils/files.py
--rw-r--r--   0        0        0     3863 2023-06-23 11:10:19.047482 pyvhs-0.1.0/pyvhs/vhs.py
--rw-r--r--   0        0        0     9912 1970-01-01 00:00:00.000000 pyvhs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-19 13:27:10.974931 pyvhs-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9080 2023-06-24 13:34:33.656701 pyvhs-0.1.1/README.md
+-rw-r--r--   0        0        0   176080 2023-06-19 12:45:19.455984 pyvhs-0.1.1/doc/imgs/playback.png
+-rw-r--r--   0        0        0   242536 2023-06-19 12:48:00.793752 pyvhs-0.1.1/doc/imgs/pyvhs.png
+-rw-r--r--   0        0        0      570 2023-06-24 14:00:52.772960 pyvhs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 19:27:59.639929 pyvhs-0.1.1/pyvhs/__init__.py
+-rw-r--r--   0        0        0    59151 2023-06-17 12:32:19.507485 pyvhs-0.1.1/pyvhs/template_imgs/template001.png
+-rw-r--r--   0        0        0     2321 2023-06-17 12:48:13.782701 pyvhs-0.1.1/pyvhs/template_imgs/template002.png
+-rw-r--r--   0        0        0        0 2023-06-18 18:24:43.368411 pyvhs-0.1.1/pyvhs/utils/__init__.py
+-rw-r--r--   0        0        0     8282 2023-06-24 11:23:09.359583 pyvhs-0.1.1/pyvhs/utils/edits.py
+-rw-r--r--   0        0        0      976 2023-06-22 00:50:19.366984 pyvhs-0.1.1/pyvhs/utils/files.py
+-rw-r--r--   0        0        0     4006 2023-06-24 13:58:02.727393 pyvhs-0.1.1/pyvhs/vhs.py
+-rw-r--r--   0        0        0     9926 1970-01-01 00:00:00.000000 pyvhs-0.1.1/PKG-INFO
```

### Comparing `pyvhs-0.1.0/LICENSE` & `pyvhs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.0/README.md` & `pyvhs-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 <h1 align="center">
   <a href="https://github.com/mddunlap924/VHSpy">
     <img src="https://raw.githubusercontent.com/mddunlap924/PyVHS/main/doc/imgs/pyvhs.png" width="512" height="256" alt="pyvhs">
   </a>
 </h1>
 <p align="center">
-  <a href="https://pypi.org/project/pyvhs/"><img src="https://badge.fury.io/py/pyvhs.svg"/>
-  </a>
+  <a href="https://badge.fury.io/py/pyvhs"><img src="https://badge.fury.io/py/pyvhs.png" alt="PyPI version"></a>
   <a target="_blank" href="https://github.com/mddunlap924/PyVHS/blob/main/LICENSE"><img src="https://camo.githubusercontent.com/8298ac0a88a52618cd97ba4cba6f34f63dd224a22031f283b0fec41a892c82cf/68747470733a2f2f696d672e736869656c64732e696f2f707970692f6c2f73656c656e69756d2d776972652e737667" />
   </a>
   <a target="_blank" href="https://www.linkedin.com/in/myles-dunlap/"><img height="20" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                              ****** [pyvhs] ******
-   [https://badge.fury.io/py/pyvhs.svg] [https://camo.githubusercontent.com/
+              [PyPI_version] [https://camo.githubusercontent.com/
        8298ac0a88a52618cd97ba4cba6f34f63dd224a22031f283b0fec41a892c82cf/
 68747470733a2f2f696d672e736869656c64732e696f2f707970692f6c2f73656c656e69756d2d776972652e737667]
          [https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-
                      badge&logo=linkedin&logoColor=white]
   PyVHS is a Python library developed for editing of digitized VHS cassettes.
                 This repository contains the PyVHS source code.
    Introduction  •  Installation  •  Usage  •  Documentation  •  Issues  •
```

### Comparing `pyvhs-0.1.0/doc/imgs/playback.png` & `pyvhs-0.1.1/doc/imgs/playback.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.0/doc/imgs/pyvhs.png` & `pyvhs-0.1.1/doc/imgs/pyvhs.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.0/pyproject.toml` & `pyvhs-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyvhs"
-version = "0.1.0"
+version = "0.1.1"
 description = "Digitized VHS Cassette Editing with Python"
 authors = ["Myles Dunlap"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mddunlap924/PyVHS/tree/main"
 keywords = ["vhs", "vcr", "image processing", "video"]
```

### Comparing `pyvhs-0.1.0/pyvhs/template_imgs/template001.png` & `pyvhs-0.1.1/pyvhs/template_imgs/template001.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.0/pyvhs/template_imgs/template002.png` & `pyvhs-0.1.1/pyvhs/template_imgs/template002.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.0/pyvhs/utils/edits.py` & `pyvhs-0.1.1/pyvhs/utils/edits.py`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.0/pyvhs/utils/files.py` & `pyvhs-0.1.1/pyvhs/utils/files.py`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.0/pyvhs/vhs.py` & `pyvhs-0.1.1/pyvhs/vhs.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 """
 
 # Libraries
 import sys
 import argparse
 import gc
 from pathlib import Path
+import pkg_resources
 import time
 from PIL import Image
 import numpy as np
 
 # Custom modules
 from pyvhs.utils.files import VideosToEdit
 from pyvhs.utils.edits import EditVideo
 
 
 # Detect debugging mode
 def debugger_is_active() -> bool:
     """Return if the debugger is currently active"""
     return hasattr(sys, 'gettrace') and sys.gettrace() is not None
 
+# Packaged template images with PyVHS
+DEFAULT_PATH_TEMPLATES = pkg_resources.resource_filename('pyvhs', 'template_imgs/')
+
 
 def main():
     # Determine if running in debug mode
     # If in debug manually point to CFG file
     is_debugger = debugger_is_active()
 
     # Parse the arguments
@@ -38,15 +42,15 @@
                                          description= arg_desc)
         parser.add_argument("-dir",
                             required=True,
                             type=str,
                             help = "Directory containing video files")
         parser.add_argument("-template_imgs",
                             required=False,
-                            default='./pyvhs/template_imgs',
+                            default=DEFAULT_PATH_TEMPLATES,
                             type=str,
                             help = "Path to template images")
         parser.add_argument("-threshold",
                             required=False,
                             default=0.9,
                             type=float,
                             help = ('SSIM threshold for indicating a video frame '
```

### Comparing `pyvhs-0.1.0/PKG-INFO` & `pyvhs-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvhs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Digitized VHS Cassette Editing with Python
 Home-page: https://github.com/mddunlap924/PyVHS/tree/main
 License: MIT
 Keywords: vhs,vcr,image processing,video
 Author: Myles Dunlap
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -22,16 +22,15 @@
 
 <h1 align="center">
   <a href="https://github.com/mddunlap924/VHSpy">
     <img src="https://raw.githubusercontent.com/mddunlap924/PyVHS/main/doc/imgs/pyvhs.png" width="512" height="256" alt="pyvhs">
   </a>
 </h1>
 <p align="center">
-  <a href="https://pypi.org/project/pyvhs/"><img src="https://badge.fury.io/py/pyvhs.svg"/>
-  </a>
+  <a href="https://badge.fury.io/py/pyvhs"><img src="https://badge.fury.io/py/pyvhs.png" alt="PyPI version"></a>
   <a target="_blank" href="https://github.com/mddunlap924/PyVHS/blob/main/LICENSE"><img src="https://camo.githubusercontent.com/8298ac0a88a52618cd97ba4cba6f34f63dd224a22031f283b0fec41a892c82cf/68747470733a2f2f696d672e736869656c64732e696f2f707970692f6c2f73656c656e69756d2d776972652e737667" />
   </a>
   <a target="_blank" href="https://www.linkedin.com/in/myles-dunlap/"><img height="20" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: pyvhs Version: 0.1.0 Summary: Digitized VHS
+Metadata-Version: 2.1 Name: pyvhs Version: 0.1.1 Summary: Digitized VHS
 Cassette Editing with Python Home-page: https://github.com/mddunlap924/PyVHS/
 tree/main License: MIT Keywords: vhs,vcr,image processing,video Author: Myles
 Dunlap Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-
 Dist: moviepy (>=1.0.3,<2.0.0) Requires-Dist: pygame (>=2.4.0,<3.0.0) Requires-
 Dist: scikit-image (>=0.21.0,<0.22.0) Project-URL: Repository, https://
 github.com/mddunlap924/PyVHS/tree/main Description-Content-Type: text/markdown
                              ****** [pyvhs] ******
-   [https://badge.fury.io/py/pyvhs.svg] [https://camo.githubusercontent.com/
+              [PyPI_version] [https://camo.githubusercontent.com/
        8298ac0a88a52618cd97ba4cba6f34f63dd224a22031f283b0fec41a892c82cf/
 68747470733a2f2f696d672e736869656c64732e696f2f707970692f6c2f73656c656e69756d2d776972652e737667]
          [https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-
                      badge&logo=linkedin&logoColor=white]
   PyVHS is a Python library developed for editing of digitized VHS cassettes.
                 This repository contains the PyVHS source code.
    Introduction  •  Installation  •  Usage  •  Documentation  •  Issues  •
```

