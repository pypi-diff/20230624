# Comparing `tmp/labelprinterkit-0.4.1.tar.gz` & `tmp/labelprinterkit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelprinterkit-0.4.1.tar", max compression
+gzip compressed data, was "labelprinterkit-0.4.2.tar", max compression
```

## Comparing `labelprinterkit-0.4.1.tar` & `labelprinterkit-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.4.1/LICENSE
--rw-r--r--   0        0        0     2235 2023-06-23 21:07:41.479689 labelprinterkit-0.4.1/README.md
--rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.4.1/labelprinterkit/__init__.py
--rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.4.1/labelprinterkit/backends/__init__.py
--rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.4.1/labelprinterkit/backends/bluetooth.py
--rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.4.1/labelprinterkit/backends/network.py
--rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.4.1/labelprinterkit/backends/usb.py
--rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.4.1/labelprinterkit/constants.py
--rw-r--r--   0        0        0     1864 2023-06-23 21:07:41.480689 labelprinterkit-0.4.1/labelprinterkit/job.py
--rw-r--r--   0        0        0     6822 2023-06-23 22:30:20.680886 labelprinterkit-0.4.1/labelprinterkit/label.py
--rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.4.1/labelprinterkit/page.py
--rw-r--r--   0        0        0     8654 2023-06-23 21:07:41.480689 labelprinterkit-0.4.1/labelprinterkit/printers.py
--rw-r--r--   0        0        0      667 2023-06-23 22:30:20.681886 labelprinterkit-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 labelprinterkit-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2247 2023-06-24 10:59:26.674400 labelprinterkit-0.4.2/README.md
+-rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.4.2/labelprinterkit/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.4.2/labelprinterkit/backends/__init__.py
+-rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.4.2/labelprinterkit/backends/bluetooth.py
+-rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.4.2/labelprinterkit/backends/network.py
+-rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.4.2/labelprinterkit/backends/usb.py
+-rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.4.2/labelprinterkit/constants.py
+-rw-r--r--   0        0        0     1878 2023-06-24 10:56:51.609529 labelprinterkit-0.4.2/labelprinterkit/doc/examples/complex_label_with_qrcode.py
+-rw-r--r--   0        0        0     1864 2023-06-23 21:07:41.480689 labelprinterkit-0.4.2/labelprinterkit/job.py
+-rw-r--r--   0        0        0     6822 2023-06-24 10:59:15.379263 labelprinterkit-0.4.2/labelprinterkit/label.py
+-rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.4.2/labelprinterkit/page.py
+-rw-r--r--   0        0        0     8578 2023-06-24 10:59:26.675400 labelprinterkit-0.4.2/labelprinterkit/printers.py
+-rw-r--r--   0        0        0      667 2023-06-24 10:59:26.677400 labelprinterkit-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 labelprinterkit-0.4.2/PKG-INFO
```

### Comparing `labelprinterkit-0.4.1/LICENSE` & `labelprinterkit-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.1/README.md` & `labelprinterkit-0.4.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 Brother P-Touch devices. It was developed for the Networking department of
 KIT (Karlsruhe Institute of Technology).
 
 Labelprinterkit's simple layout engine can be used to create simple labels:
 
 ```python
 from labelprinterkit.backends.usb import PyUSBBackend
-from labelprinterkit.printers import P750W
+from labelprinterkit.printers import P700
 from labelprinterkit.label import Label, Text, Box, Padding
 from labelprinterkit.job import Job
 from labelprinterkit.constants import MediaType, MediaSize
 from labelprinterkit.page import Page
 from PIL import Image
 
 # Create text for the label
 
-text1 = Text("First line", 'comic.ttf', padding=Padding(0, 0, 1, 0))
-text2 = Text("Some text", 'comic.ttf')
-text3 = Text("Other text", 'comic.ttf')
+text1 = Text("First line", 45, 'comic.ttf', padding=Padding(0, 0, 1, 0))
+text2 = Text("Some text", 25, 'comic.ttf')
+text3 = Text("Other text", 25, 'comic.ttf')
 
 # Insert Text into boxes
 box1 = Box(45, text1)
 box2 = Box(25, text2, text3)
 
 # Create label with rows from above
 label = Label(box1, box2)
 
 # Create job with configuration and add label as page
 job = Job(MediaSize.W12, MediaType.LAMINATED_TAPE)
 job.add_page(label)
 
-# Creat a page from a Pillow image and add it to the job
+# Create a page from a Pillow image and add it to the job
 image = Image.new("1", (70, 200), "white")
 page = Page.from_image(image)
 job.add_page(page)
 
 # scan for a USB printer using the PyUSBBackend
 backend = PyUSBBackend()
 printer = P700(backend)
```

### Comparing `labelprinterkit-0.4.1/labelprinterkit/backends/bluetooth.py` & `labelprinterkit-0.4.2/labelprinterkit/backends/bluetooth.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.1/labelprinterkit/backends/network.py` & `labelprinterkit-0.4.2/labelprinterkit/backends/network.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.1/labelprinterkit/backends/usb.py` & `labelprinterkit-0.4.2/labelprinterkit/backends/usb.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.1/labelprinterkit/constants.py` & `labelprinterkit-0.4.2/labelprinterkit/constants.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.1/labelprinterkit/job.py` & `labelprinterkit-0.4.2/labelprinterkit/job.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.1/labelprinterkit/label.py` & `labelprinterkit-0.4.2/labelprinterkit/label.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.1/labelprinterkit/page.py` & `labelprinterkit-0.4.2/labelprinterkit/page.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.1/labelprinterkit/printers.py` & `labelprinterkit-0.4.2/labelprinterkit/printers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from abc import ABC, abstractmethod
 from logging import getLogger
 import struct
 from typing import TypeVar
 
 import packbits
 
-from .backends import BiDirectionalBackend, UniDirectionalBackend
-from .constants import Resolution, ErrorCodes, MediaSize, MediaType, StatusCodes, NotificationCodes, TapeColor, \
+from .backends import BaseBackend
+from .constants import Resolution, ErrorCodes, MediaType, StatusCodes, NotificationCodes, TapeColor, \
     TextColor, VariousModesSettings, AdvancedModeSettings
 from .job import Job
 
 logger = getLogger(__name__)
 
-BackendType = TypeVar('BackendType', bound=BiDirectionalBackend | UniDirectionalBackend)
+BackendType = TypeVar('BackendType', bound=BaseBackend)
 
 
 class Error:
     def __init__(self, byte1: int, byte2: int) -> None:
         value = byte1 | (byte2 << 8)
         self._errors = {
             err.name: bool(value & err_code)
```

### Comparing `labelprinterkit-0.4.1/pyproject.toml` & `labelprinterkit-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labelprinterkit"
-version = "0.4.1"
+version = "0.4.2"
 description = "A library for creating and printing labels for Brother P-Touch devices"
 authors = ["Adrian Tschira <packages@notafile.com>", "Benedikt Neuffer <benedikt.neuffer@kit.edu>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `labelprinterkit-0.4.1/PKG-INFO` & `labelprinterkit-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelprinterkit
-Version: 0.4.1
+Version: 0.4.2
 Summary: A library for creating and printing labels for Brother P-Touch devices
 License: Apache License, Version 2.0
 Author: Adrian Tschira
 Author-email: packages@notafile.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -25,39 +25,39 @@
 Brother P-Touch devices. It was developed for the Networking department of
 KIT (Karlsruhe Institute of Technology).
 
 Labelprinterkit's simple layout engine can be used to create simple labels:
 
 ```python
 from labelprinterkit.backends.usb import PyUSBBackend
-from labelprinterkit.printers import P750W
+from labelprinterkit.printers import P700
 from labelprinterkit.label import Label, Text, Box, Padding
 from labelprinterkit.job import Job
 from labelprinterkit.constants import MediaType, MediaSize
 from labelprinterkit.page import Page
 from PIL import Image
 
 # Create text for the label
 
-text1 = Text("First line", 'comic.ttf', padding=Padding(0, 0, 1, 0))
-text2 = Text("Some text", 'comic.ttf')
-text3 = Text("Other text", 'comic.ttf')
+text1 = Text("First line", 45, 'comic.ttf', padding=Padding(0, 0, 1, 0))
+text2 = Text("Some text", 25, 'comic.ttf')
+text3 = Text("Other text", 25, 'comic.ttf')
 
 # Insert Text into boxes
 box1 = Box(45, text1)
 box2 = Box(25, text2, text3)
 
 # Create label with rows from above
 label = Label(box1, box2)
 
 # Create job with configuration and add label as page
 job = Job(MediaSize.W12, MediaType.LAMINATED_TAPE)
 job.add_page(label)
 
-# Creat a page from a Pillow image and add it to the job
+# Create a page from a Pillow image and add it to the job
 image = Image.new("1", (70, 200), "white")
 page = Page.from_image(image)
 job.add_page(page)
 
 # scan for a USB printer using the PyUSBBackend
 backend = PyUSBBackend()
 printer = P700(backend)
```

