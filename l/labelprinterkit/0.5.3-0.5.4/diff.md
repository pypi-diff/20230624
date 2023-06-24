# Comparing `tmp/labelprinterkit-0.5.3.tar.gz` & `tmp/labelprinterkit-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelprinterkit-0.5.3.tar", max compression
+gzip compressed data, was "labelprinterkit-0.5.4.tar", max compression
```

## Comparing `labelprinterkit-0.5.3.tar` & `labelprinterkit-0.5.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.5.3/LICENSE
--rw-r--r--   0        0        0     2247 2023-06-24 11:50:05.192647 labelprinterkit-0.5.3/README.md
--rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.5.3/labelprinterkit/__init__.py
--rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.5.3/labelprinterkit/backends/__init__.py
--rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.5.3/labelprinterkit/backends/bluetooth.py
--rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.5.3/labelprinterkit/backends/network.py
--rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.5.3/labelprinterkit/backends/usb.py
--rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.5.3/labelprinterkit/constants.py
--rw-r--r--   0        0        0     1864 2023-06-23 21:07:41.480689 labelprinterkit-0.5.3/labelprinterkit/job.py
--rw-r--r--   0        0        0     6450 2023-06-24 11:50:05.192647 labelprinterkit-0.5.3/labelprinterkit/label.py
--rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.5.3/labelprinterkit/page.py
--rw-r--r--   0        0        0     8578 2023-06-24 10:59:26.675400 labelprinterkit-0.5.3/labelprinterkit/printers.py
--rw-r--r--   0        0        0      667 2023-06-24 12:03:51.080179 labelprinterkit-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 labelprinterkit-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.5.4/LICENSE
+-rw-r--r--   0        0        0     2247 2023-06-24 11:50:05.192647 labelprinterkit-0.5.4/README.md
+-rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.5.4/labelprinterkit/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.5.4/labelprinterkit/backends/__init__.py
+-rw-r--r--   0        0        0      681 2023-06-23 22:30:20.680886 labelprinterkit-0.5.4/labelprinterkit/backends/bluetooth.py
+-rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.5.4/labelprinterkit/backends/network.py
+-rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.5.4/labelprinterkit/backends/usb.py
+-rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.5.4/labelprinterkit/constants.py
+-rw-r--r--   0        0        0     1864 2023-06-24 12:23:33.620108 labelprinterkit-0.5.4/labelprinterkit/job.py
+-rw-r--r--   0        0        0     6450 2023-06-24 11:50:05.192647 labelprinterkit-0.5.4/labelprinterkit/label.py
+-rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.5.4/labelprinterkit/page.py
+-rw-r--r--   0        0        0     8694 2023-06-24 12:43:54.859120 labelprinterkit-0.5.4/labelprinterkit/printers.py
+-rw-r--r--   0        0        0      667 2023-06-24 12:43:54.859120 labelprinterkit-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 labelprinterkit-0.5.4/PKG-INFO
```

### Comparing `labelprinterkit-0.5.3/LICENSE` & `labelprinterkit-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.3/README.md` & `labelprinterkit-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.3/labelprinterkit/backends/bluetooth.py` & `labelprinterkit-0.5.4/labelprinterkit/backends/bluetooth.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.3/labelprinterkit/backends/network.py` & `labelprinterkit-0.5.4/labelprinterkit/backends/network.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.3/labelprinterkit/backends/usb.py` & `labelprinterkit-0.5.4/labelprinterkit/backends/usb.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.3/labelprinterkit/constants.py` & `labelprinterkit-0.5.4/labelprinterkit/constants.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.3/labelprinterkit/job.py` & `labelprinterkit-0.5.4/labelprinterkit/job.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.3/labelprinterkit/label.py` & `labelprinterkit-0.5.4/labelprinterkit/label.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.3/labelprinterkit/page.py` & `labelprinterkit-0.5.4/labelprinterkit/page.py`

 * *Files identical despite different names*

### Comparing `labelprinterkit-0.5.3/labelprinterkit/printers.py` & `labelprinterkit-0.5.4/labelprinterkit/printers.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,17 @@
         media_type = job.media_type.value.to_bytes(1, 'big')
         media_size = job.media_size.value.width.to_bytes(1, 'big')
         offset = job.media_size.value.lmargin
 
         various_mode = 0
         if job.auto_cut:
             various_mode = various_mode | VariousModesSettings.AUTO_CUT.value
+            auto_cut = True
+        else:
+            auto_cut = False
         if job.mirror_printing:
             various_mode = various_mode | VariousModesSettings.MIRROR_PRINTING.value
         various_mode = various_mode.to_bytes(1, 'big')
 
         advanced_mode = 0
         if job.half_cut:
             if not self._FEATURE_HALF_CUT:
@@ -192,16 +195,15 @@
             # switch dynamic command mode: enable raster mode
             self._backend.write(b'\x1Bia\x01')
 
             # Print information command
             # b'\x1Biz\x86\x01\x0c\x00\x00\x00\00\x00\x00'
             information_command = b'\x1Biz\x86' + media_type + media_size + b'\x00\x00\x00\00\x00\x00'
             self._backend.write(information_command)
-
-            if i == 0:
+            if i == 0 and auto_cut:
                 # Ugly workaround
                 # Print information command a second time forces cutting after first page.
                 # No idea why this is needed, but it works
                 self._backend.write(information_command)
 
             # Various mode
             logger.debug(f"various_mode: {various_mode}")
@@ -210,16 +212,17 @@
             # Advanced mode
             logger.debug(f"advanced_mode: {advanced_mode}")
             self._backend.write(b'\x1biK' + advanced_mode)
 
             # margin
             self._backend.write(b'\x1bid' + margin)
 
-            # Configure after how many pages a cut should be done
-            self._backend.write(b'\x1BiA' + cut_each)
+            if auto_cut:
+                # Configure after how many pages a cut should be done
+                self._backend.write(b'\x1BiA' + cut_each)
 
             # Enable compression mode
             self._backend.write(b'M\x02')
 
             # send rastered lines
             for line in page:
                 logging.debug(f"line: {line}")
```

### Comparing `labelprinterkit-0.5.3/pyproject.toml` & `labelprinterkit-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labelprinterkit"
-version = "0.5.3"
+version = "0.5.4"
 description = "A library for creating and printing labels for Brother P-Touch devices"
 authors = ["Adrian Tschira <packages@notafile.com>", "Benedikt Neuffer <benedikt.neuffer@kit.edu>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `labelprinterkit-0.5.3/PKG-INFO` & `labelprinterkit-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelprinterkit
-Version: 0.5.3
+Version: 0.5.4
 Summary: A library for creating and printing labels for Brother P-Touch devices
 License: Apache License, Version 2.0
 Author: Adrian Tschira
 Author-email: packages@notafile.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

