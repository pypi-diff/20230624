# Comparing `tmp/labelprinterkit-0.4.0.tar.gz` & `tmp/labelprinterkit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelprinterkit-0.4.0.tar", max compression
+gzip compressed data, was "labelprinterkit-0.4.1.tar", max compression
```

## Comparing `labelprinterkit-0.4.0.tar` & `labelprinterkit-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.4.0/LICENSE
--rw-r--r--   0        0        0     2235 2023-06-23 21:07:41.479689 labelprinterkit-0.4.0/README.md
--rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.4.0/labelprinterkit/__init__.py
--rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.4.0/labelprinterkit/backends/__init__.py
--rw-r--r--   0        0        0      635 2023-06-23 21:07:41.479689 labelprinterkit-0.4.0/labelprinterkit/backends/bluetooth.py
--rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.4.0/labelprinterkit/backends/network.py
--rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/backends/usb.py
--rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/constants.py
--rw-r--r--   0        0        0     1864 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/job.py
--rw-r--r--   0        0        0     5075 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/label.py
--rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/page.py
--rw-r--r--   0        0        0     8654 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/printers.py
--rw-r--r--   0        0        0      507 2023-06-23 21:07:41.481689 labelprinterkit-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 labelprinterkit-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2235 2023-06-23 21:07:41.479689 labelprinterkit-0.4.1/README.md
+-rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.4.1/labelprinterkit/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.4.1/labelprinterkit/backends/__init__.py
+-rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.4.1/labelprinterkit/backends/bluetooth.py
+-rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.4.1/labelprinterkit/backends/network.py
+-rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.4.1/labelprinterkit/backends/usb.py
+-rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.4.1/labelprinterkit/constants.py
+-rw-r--r--   0        0        0     1864 2023-06-23 21:07:41.480689 labelprinterkit-0.4.1/labelprinterkit/job.py
+-rw-r--r--   0        0        0     6822 2023-06-23 22:30:20.680886 labelprinterkit-0.4.1/labelprinterkit/label.py
+-rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.4.1/labelprinterkit/page.py
+-rw-r--r--   0        0        0     8654 2023-06-23 21:07:41.480689 labelprinterkit-0.4.1/labelprinterkit/printers.py
+-rw-r--r--   0        0        0      667 2023-06-23 22:30:20.681886 labelprinterkit-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 labelprinterkit-0.4.1/PKG-INFO
```

### Comparing `labelprinterkit-0.4.0/LICENSE` & `labelprinterkit-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.0/README.md` & `labelprinterkit-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.0/labelprinterkit/backends/bluetooth.py` & `labelprinterkit-0.4.1/labelprinterkit/backends/bluetooth.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import serial
-
+try:
+    import serial
+except ImportError:
+    serial = None
 from . import BiDirectionalBackend
 
 
 class BTSerialBackend(BiDirectionalBackend):
     def __init__(self, dev_path: str):
         dev = serial.Serial(
             dev_path,
```

### Comparing `labelprinterkit-0.4.0/labelprinterkit/backends/network.py` & `labelprinterkit-0.4.1/labelprinterkit/backends/network.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.0/labelprinterkit/backends/usb.py` & `labelprinterkit-0.4.1/labelprinterkit/backends/usb.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.0/labelprinterkit/constants.py` & `labelprinterkit-0.4.1/labelprinterkit/constants.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.0/labelprinterkit/job.py` & `labelprinterkit-0.4.1/labelprinterkit/job.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.0/labelprinterkit/page.py` & `labelprinterkit-0.4.1/labelprinterkit/page.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.0/labelprinterkit/printers.py` & `labelprinterkit-0.4.1/labelprinterkit/printers.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.4.0/PKG-INFO` & `labelprinterkit-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: labelprinterkit
-Version: 0.4.0
+Version: 0.4.1
 Summary: A library for creating and printing labels for Brother P-Touch devices
 License: Apache License, Version 2.0
 Author: Adrian Tschira
 Author-email: packages@notafile.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: bluetooth
+Provides-Extra: qrcode
 Requires-Dist: packbits (>=0.6,<0.7)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
-Requires-Dist: pyserial (>=3.5,<4.0)
+Requires-Dist: pyserial (>=3.5,<4.0) ; extra == "bluetooth"
 Requires-Dist: pyusb (>=1.2.1,<2.0.0)
+Requires-Dist: qrcode[pil] (>=7.4.2,<8.0.0) ; extra == "qrcode"
 Description-Content-Type: text/markdown
 
 ### Labelprinterkit
 
 Labelprinterkit is a Python3 library for creating and printing labels with
 Brother P-Touch devices. It was developed for the Networking department of
 KIT (Karlsruhe Institute of Technology).
```

