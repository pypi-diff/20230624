# Comparing `tmp/tkadw-0.2.0.tar.gz` & `tmp/tkadw-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkadw-0.2.0.tar", max compression
+gzip compressed data, was "tkadw-0.2.1.tar", max compression
```

## Comparing `tkadw-0.2.0.tar` & `tkadw-0.2.1.tar`

### file list

```diff
@@ -1,49 +1,46 @@
--rw-r--r--   0        0        0      291 2023-06-24 02:04:47.136489 tkadw-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3059 2023-06-23 09:04:32.302087 tkadw-0.2.0/README.md
--rw-r--r--   0        0        0      112 2023-06-23 03:45:25.577456 tkadw-0.2.0/tkadw/__init__.py
--rw-r--r--   0        0        0     1176 2023-06-23 11:43:30.799302 tkadw-0.2.0/tkadw/__main__.py
--rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.2.0/tkadw/app.config
--rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.2.0/tkadw/appconfig.py
--rw-r--r--   0        0        0      959 2023-06-23 11:43:18.569764 tkadw-0.2.0/tkadw/canvas/__init__.py
--rw-r--r--   0        0        0     1801 2023-06-23 11:43:18.792347 tkadw-0.2.0/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.2.0/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    22598 2023-06-24 01:20:36.024808 tkadw-0.2.0/tkadw/canvas/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.2.0/tkadw/canvas/__pycache__/button.cpython-38.pyc
--rw-r--r--   0        0        0    24261 2023-06-23 09:59:53.052039 tkadw-0.2.0/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
--rw-r--r--   0        0        0    23648 2023-06-24 01:42:47.540397 tkadw-0.2.0/tkadw/canvas/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0    11871 2023-06-24 01:50:40.515094 tkadw-0.2.0/tkadw/canvas/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.2.0/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     4481 2023-06-24 01:55:47.753570 tkadw-0.2.0/tkadw/canvas/__pycache__/label.cpython-311.pyc
--rw-r--r--   0        0        0    29583 2023-06-24 02:03:31.982563 tkadw-0.2.0/tkadw/canvas/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0    16890 2023-06-24 01:20:35.915877 tkadw-0.2.0/tkadw/canvas/button.py
--rw-r--r--   0        0        0    20930 2023-06-23 09:59:52.869076 tkadw-0.2.0/tkadw/canvas/drawengine.py
--rw-r--r--   0        0        0    17378 2023-06-24 02:04:47.104845 tkadw-0.2.0/tkadw/canvas/entry.py
--rw-r--r--   0        0        0     6326 2023-06-24 01:50:40.374060 tkadw-0.2.0/tkadw/canvas/frame.py
--rw-r--r--   0        0        0     2051 2023-06-10 01:20:40.907297 tkadw-0.2.0/tkadw/canvas/fun.py
--rw-r--r--   0        0        0    15490 2023-06-10 01:25:11.532315 tkadw-0.2.0/tkadw/canvas/fun2.py
--rw-r--r--   0        0        0     8108 2023-06-10 01:29:02.970946 tkadw-0.2.0/tkadw/canvas/fun3.py
--rw-r--r--   0        0        0     3202 2023-06-10 03:27:44.231516 tkadw-0.2.0/tkadw/canvas/fun4.py
--rw-r--r--   0        0        0      942 2023-06-10 03:50:17.322506 tkadw-0.2.0/tkadw/canvas/fun5.py
--rw-r--r--   0        0        0     9870 2023-06-10 07:36:40.103845 tkadw-0.2.0/tkadw/canvas/fun6.py
--rw-r--r--   0        0        0     2056 2023-06-24 01:55:37.753942 tkadw-0.2.0/tkadw/canvas/label.py
--rw-r--r--   0        0        0     5690 2023-06-10 03:45:21.292347 tkadw-0.2.0/tkadw/canvas/poly.tcl
--rw-r--r--   0        0        0    21800 2023-06-24 02:03:31.849264 tkadw-0.2.0/tkadw/canvas/textbox.py
--rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.2.0/tkadw/canvas/titlebar.py
--rw-r--r--   0        0        0     3120 2021-12-23 08:06:14.000000 tkadw-0.2.0/tkadw/tkfontawesome/__init__.py
--rw-r--r--   0        0        0  1412156 2021-12-23 07:57:18.000000 tkadw-0.2.0/tkadw/tkfontawesome/svgs.py
--rw-r--r--   0        0        0       29 2023-06-23 03:52:51.957932 tkadw-0.2.0/tkadw/tkite/__init__.py
--rw-r--r--   0        0        0      181 2023-06-23 03:52:52.129145 tkadw-0.2.0/tkadw/tkite/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      341 2023-06-23 11:43:18.508873 tkadw-0.2.0/tkadw/tkite/gtk/__init__.py
--rw-r--r--   0        0        0      719 2023-06-23 11:43:19.769317 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4723 2023-06-24 01:29:02.487008 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     3193 2023-06-24 01:44:55.068151 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     2375 2023-06-24 01:51:31.925168 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0     1471 2023-06-23 11:43:19.785605 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/label.cpython-311.pyc
--rw-r--r--   0        0        0     3149 2023-06-24 02:03:32.305960 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0     4735 2023-06-24 01:29:02.053861 tkadw-0.2.0/tkadw/tkite/gtk/button.py
--rw-r--r--   0        0        0     2551 2023-06-24 01:44:54.644195 tkadw-0.2.0/tkadw/tkite/gtk/entry.py
--rw-r--r--   0        0        0     1125 2023-06-24 01:51:31.490298 tkadw-0.2.0/tkadw/tkite/gtk/frame.py
--rw-r--r--   0        0        0      359 2023-06-23 11:43:18.648390 tkadw-0.2.0/tkadw/tkite/gtk/label.py
--rw-r--r--   0        0        0     3555 2023-06-24 00:34:13.973458 tkadw-0.2.0/tkadw/tkite/gtk/notebook.py
--rw-r--r--   0        0        0     2461 2023-06-24 02:03:31.840946 tkadw-0.2.0/tkadw/tkite/gtk/textbox.py
--rw-r--r--   0        0        0     3508 1970-01-01 00:00:00.000000 tkadw-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      291 2023-06-24 02:48:13.231068 tkadw-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6554 2023-06-24 02:48:07.830846 tkadw-0.2.1/README.md
+-rw-r--r--   0        0        0      142 2023-06-24 02:43:29.598698 tkadw-0.2.1/tkadw/__init__.py
+-rw-r--r--   0        0        0     1162 2023-06-24 02:46:00.468947 tkadw-0.2.1/tkadw/__main__.py
+-rw-r--r--   0        0        0      142 2023-06-24 02:43:29.551423 tkadw-0.2.1/tkadw/advanced/__init__.py
+-rw-r--r--   0        0        0      383 2023-06-24 02:43:30.014259 tkadw-0.2.1/tkadw/advanced/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2906 2023-06-24 02:46:00.929979 tkadw-0.2.1/tkadw/advanced/__pycache__/adw.cpython-311.pyc
+-rw-r--r--   0        0        0    18187 2023-06-24 02:38:22.924598 tkadw-0.2.1/tkadw/advanced/__pycache__/icon.cpython-311.pyc
+-rw-r--r--   0        0        0     1598 2023-06-24 02:45:43.966706 tkadw-0.2.1/tkadw/advanced/adw.py
+-rw-r--r--   0        0        0    17230 2023-06-24 02:38:22.074901 tkadw-0.2.1/tkadw/advanced/icon.py
+-rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.2.1/tkadw/app.config
+-rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.2.1/tkadw/appconfig.py
+-rw-r--r--   0        0        0      959 2023-06-23 11:43:18.569764 tkadw-0.2.1/tkadw/canvas/__init__.py
+-rw-r--r--   0        0        0     1801 2023-06-23 11:43:18.792347 tkadw-0.2.1/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.2.1/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    22598 2023-06-24 01:20:36.024808 tkadw-0.2.1/tkadw/canvas/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.2.1/tkadw/canvas/__pycache__/button.cpython-38.pyc
+-rw-r--r--   0        0        0    24261 2023-06-23 09:59:53.052039 tkadw-0.2.1/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
+-rw-r--r--   0        0        0    23658 2023-06-24 02:25:14.940246 tkadw-0.2.1/tkadw/canvas/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0    11871 2023-06-24 01:50:40.515094 tkadw-0.2.1/tkadw/canvas/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.2.1/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     4481 2023-06-24 01:55:47.753570 tkadw-0.2.1/tkadw/canvas/__pycache__/label.cpython-311.pyc
+-rw-r--r--   0        0        0    29583 2023-06-24 02:03:31.982563 tkadw-0.2.1/tkadw/canvas/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0    16890 2023-06-24 01:20:35.915877 tkadw-0.2.1/tkadw/canvas/button.py
+-rw-r--r--   0        0        0    20930 2023-06-23 09:59:52.869076 tkadw-0.2.1/tkadw/canvas/drawengine.py
+-rw-r--r--   0        0        0    17378 2023-06-24 02:04:47.104845 tkadw-0.2.1/tkadw/canvas/entry.py
+-rw-r--r--   0        0        0     6326 2023-06-24 01:50:40.374060 tkadw-0.2.1/tkadw/canvas/frame.py
+-rw-r--r--   0        0        0     2056 2023-06-24 01:55:37.753942 tkadw-0.2.1/tkadw/canvas/label.py
+-rw-r--r--   0        0        0    21800 2023-06-24 02:03:31.849264 tkadw-0.2.1/tkadw/canvas/textbox.py
+-rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.2.1/tkadw/canvas/titlebar.py
+-rw-r--r--   0        0        0       29 2023-06-23 03:52:51.957932 tkadw-0.2.1/tkadw/tkite/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-23 03:52:52.129145 tkadw-0.2.1/tkadw/tkite/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      341 2023-06-23 11:43:18.508873 tkadw-0.2.1/tkadw/tkite/gtk/__init__.py
+-rw-r--r--   0        0        0      719 2023-06-23 11:43:19.769317 tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4723 2023-06-24 01:29:02.487008 tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     3193 2023-06-24 01:44:55.068151 tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     2375 2023-06-24 01:51:31.925168 tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0     1471 2023-06-23 11:43:19.785605 tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/label.cpython-311.pyc
+-rw-r--r--   0        0        0     3149 2023-06-24 02:03:32.305960 tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0     4735 2023-06-24 01:29:02.053861 tkadw-0.2.1/tkadw/tkite/gtk/button.py
+-rw-r--r--   0        0        0     2551 2023-06-24 01:44:54.644195 tkadw-0.2.1/tkadw/tkite/gtk/entry.py
+-rw-r--r--   0        0        0     1125 2023-06-24 01:51:31.490298 tkadw-0.2.1/tkadw/tkite/gtk/frame.py
+-rw-r--r--   0        0        0      359 2023-06-23 11:43:18.648390 tkadw-0.2.1/tkadw/tkite/gtk/label.py
+-rw-r--r--   0        0        0     3555 2023-06-24 00:34:13.973458 tkadw-0.2.1/tkadw/tkite/gtk/notebook.py
+-rw-r--r--   0        0        0     2461 2023-06-24 02:03:31.840946 tkadw-0.2.1/tkadw/tkite/gtk/textbox.py
+-rw-r--r--   0        0        0     6876 1970-01-01 00:00:00.000000 tkadw-0.2.1/PKG-INFO
```

### Comparing `tkadw-0.2.0/tkadw/__main__.py` & `tkadw-0.2.1/tkadw/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from tkinter import Tk
 from tkadw import *
 
-root = Tk()
-root.configure(background="#1f1f1f")
+root = Adw(wincaption=(53, 53, 53))
 
 frame = GTkFrame(root)
 
 label1 = GTkLabel(frame.frame, text="GTkLabel")
 label1.pack(fill="x", ipadx=5, padx=5, pady=5)
 
 button1 = GTkButton(frame.frame, text="GTkButton")
```

### Comparing `tkadw-0.2.0/tkadw/appconfig.py` & `tkadw-0.2.1/tkadw/appconfig.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/__init__.py` & `tkadw-0.2.1/tkadw/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.2.1/tkadw/canvas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/__pycache__/button.cpython-311.pyc` & `tkadw-0.2.1/tkadw/canvas/__pycache__/button.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/__pycache__/button.cpython-38.pyc` & `tkadw-0.2.1/tkadw/canvas/__pycache__/button.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc` & `tkadw-0.2.1/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/__pycache__/entry.cpython-311.pyc` & `tkadw-0.2.1/tkadw/canvas/__pycache__/entry.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x174a9664 (Sat Jun 24 01:42:47 2023 UTC)
-files sz: 17356
+moddate:  0x3f4f9664 (Sat Jun 24 02:04:47 2023 UTC)
+files sz: 17378
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -403,42 +403,42 @@
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c047c017c02640164029c037c05a4018e
                   010100640164036c026d037d066d047d07010002007c06a6000000ab0000
                   000000000000007c005f0500000000000000007c006a0500000000000000
                   00a00600000000000000000000000000000000000000007c03a6010000ab
                   010000000000000000010002007c077c0064017c006a0500000000000000
-                  00ac04a6030000ab0300000000000000007c005f0700000000000000007c
-                  00a0080000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000001007c00a0090000000000000000000000000000000000
-                  000000a6000000ab00000000000000000001007c037c005f0a0000000000
-                  0000007c006a0b00000000000000007c005f0c00000000000000007c006a
-                  0d00000000000000007c005f0e00000000000000007c006a0f0000000000
-                  0000007c005f1000000000000000007c006a1100000000000000007c005f
-                  1200000000000000007c006a1300000000000000007c005f140000000000
-                  000000742b000000000000000000006405a6010000ab0100000000000000
-                  007c005f1600000000000000007c00a01700000000000000000000000000
-                  0000000000000064067c006a1800000000000000006407ac08a6030000ab
+                  006401ac04a6040000ab0400000000000000007c005f0700000000000000
+                  007c00a0080000000000000000000000000000000000000000a6000000ab
+                  00000000000000000001007c00a009000000000000000000000000000000
+                  0000000000a6000000ab00000000000000000001007c037c005f0a000000
+                  00000000007c006a0b00000000000000007c005f0c00000000000000007c
+                  006a0d00000000000000007c005f0e00000000000000007c006a0f000000
+                  00000000007c005f1000000000000000007c006a1100000000000000007c
+                  005f1200000000000000007c006a1300000000000000007c005f14000000
+                  0000000000742b000000000000000000006405a6010000ab010000000000
+                  0000007c005f1600000000000000007c00a0170000000000000000000000
+                  00000000000000000064067c006a1800000000000000006407ac08a60300
+                  00ab03000000000000000001007c00a01700000000000000000000000000
+                  0000000000000064097c006a1900000000000000006407ac08a6030000ab
                   03000000000000000001007c00a017000000000000000000000000000000
-                  000000000064097c006a1900000000000000006407ac08a6030000ab0300
+                  0000000000640a7c006a1a00000000000000006407ac08a6030000ab0300
                   0000000000000001007c00a0170000000000000000000000000000000000
-                  000000640a7c006a1a00000000000000006407ac08a6030000ab03000000
+                  000000640b7c006a1b00000000000000006407ac08a6030000ab03000000
                   000000000001007c00a01700000000000000000000000000000000000000
-                  00640b7c006a1b00000000000000006407ac08a6030000ab030000000000
-                  00000001007c00a017000000000000000000000000000000000000000064
-                  0c7c006a1c00000000000000006407ac08a6030000ab0300000000000000
-                  0001007c006a070000000000000000a01700000000000000000000000000
-                  00000000000000640c7c006a1c00000000000000006407ac08a6030000ab
-                  03000000000000000001007c00a017000000000000000000000000000000
-                  0000000000640d7c006a1d00000000000000006407ac08a6030000ab0300
-                  0000000000000001007c006a070000000000000000a01700000000000000
-                  00000000000000000000000000640d7c006a1d00000000000000006407ac
-                  08a6030000ab03000000000000000001007c00a018000000000000000000
-                  00000000000000000000006400a6010000ab010000000000000000010064
-                  005300
+                  00640c7c006a1c00000000000000006407ac08a6030000ab030000000000
+                  00000001007c006a070000000000000000a0170000000000000000000000
+                  000000000000000000640c7c006a1c00000000000000006407ac08a60300
+                  00ab03000000000000000001007c00a01700000000000000000000000000
+                  00000000000000640d7c006a1d00000000000000006407ac08a6030000ab
+                  03000000000000000001007c006a070000000000000000a0170000000000
+                  000000000000000000000000000000640d7c006a1d000000000000000064
+                  07ac08a6030000ab03000000000000000001007c00a01800000000000000
+                  000000000000000000000000006400a6010000ab01000000000000000001
+                  0064005300
                              0 COPY_FREE_VARS           1
                
                  7           2 RESUME                   0
                
                  9           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
@@ -481,172 +481,173 @@
                
                 16         160 PUSH_NULL
                            162 LOAD_FAST                7 (Entry)
                            164 LOAD_FAST                0 (self)
                            166 LOAD_CONST               1 (0)
                            168 LOAD_FAST                0 (self)
                            170 LOAD_ATTR                5 (var)
-                           180 KW_NAMES                 4
-                           182 PRECALL                  3
-                           186 CALL                     3
-                           196 LOAD_FAST                0 (self)
-                           198 STORE_ATTR               7 (entry)
-               
-                18         208 LOAD_FAST                0 (self)
-                           210 LOAD_METHOD              8 (_other)
-                           232 PRECALL                  0
-                           236 CALL                     0
-                           246 POP_TOP
-               
-                20         248 LOAD_FAST                0 (self)
-                           250 LOAD_METHOD              9 (default_palette)
-                           272 PRECALL                  0
-                           276 CALL                     0
-                           286 POP_TOP
-               
-                22         288 LOAD_FAST                3 (text)
-                           290 LOAD_FAST                0 (self)
-                           292 STORE_ATTR              10 (text)
-               
-                24         302 LOAD_FAST                0 (self)
-                           304 LOAD_ATTR               11 (entry_back)
-                           314 LOAD_FAST                0 (self)
-                           316 STORE_ATTR              12 (_entry_back)
-               
-                25         326 LOAD_FAST                0 (self)
-                           328 LOAD_ATTR               13 (entry_border)
-                           338 LOAD_FAST                0 (self)
-                           340 STORE_ATTR              14 (_entry_border)
-               
-                26         350 LOAD_FAST                0 (self)
-                           352 LOAD_ATTR               15 (entry_text_back)
-                           362 LOAD_FAST                0 (self)
-                           364 STORE_ATTR              16 (_entry_text_back)
-               
-                27         374 LOAD_FAST                0 (self)
-                           376 LOAD_ATTR               17 (entry_bottom_line)
-                           386 LOAD_FAST                0 (self)
-                           388 STORE_ATTR              18 (_entry_bottom_line)
-               
-                28         398 LOAD_FAST                0 (self)
-                           400 LOAD_ATTR               19 (entry_bottom_width)
-                           410 LOAD_FAST                0 (self)
-                           412 STORE_ATTR              20 (_entry_bottom_width)
-               
-                30         422 LOAD_GLOBAL             43 (NULL + nametofont)
-                           434 LOAD_CONST               5 ('TkDefaultFont')
-                           436 PRECALL                  1
-                           440 CALL                     1
-                           450 LOAD_FAST                0 (self)
-                           452 STORE_ATTR              22 (entry_text_font)
-               
-                32         462 LOAD_FAST                0 (self)
-                           464 LOAD_METHOD             23 (bind)
-                           486 LOAD_CONST               6 ('<Configure>')
-                           488 LOAD_FAST                0 (self)
-                           490 LOAD_ATTR               24 (_draw)
-                           500 LOAD_CONST               7 ('+')
-                           502 KW_NAMES                 8
-                           504 PRECALL                  3
-                           508 CALL                     3
-                           518 POP_TOP
-               
-                33         520 LOAD_FAST                0 (self)
-                           522 LOAD_METHOD             23 (bind)
-                           544 LOAD_CONST               9 ('<Button>')
-                           546 LOAD_FAST                0 (self)
-                           548 LOAD_ATTR               25 (_click)
-                           558 LOAD_CONST               7 ('+')
-                           560 KW_NAMES                 8
-                           562 PRECALL                  3
-                           566 CALL                     3
-                           576 POP_TOP
-               
-                34         578 LOAD_FAST                0 (self)
-                           580 LOAD_METHOD             23 (bind)
-                           602 LOAD_CONST              10 ('<Enter>')
-                           604 LOAD_FAST                0 (self)
-                           606 LOAD_ATTR               26 (_hover)
-                           616 LOAD_CONST               7 ('+')
-                           618 KW_NAMES                 8
-                           620 PRECALL                  3
-                           624 CALL                     3
-                           634 POP_TOP
-               
-                35         636 LOAD_FAST                0 (self)
-                           638 LOAD_METHOD             23 (bind)
-                           660 LOAD_CONST              11 ('<Leave>')
-                           662 LOAD_FAST                0 (self)
-                           664 LOAD_ATTR               27 (_hover_release)
-                           674 LOAD_CONST               7 ('+')
-                           676 KW_NAMES                 8
-                           678 PRECALL                  3
-                           682 CALL                     3
-                           692 POP_TOP
-               
-                36         694 LOAD_FAST                0 (self)
-                           696 LOAD_METHOD             23 (bind)
-                           718 LOAD_CONST              12 ('<FocusIn>')
-                           720 LOAD_FAST                0 (self)
-                           722 LOAD_ATTR               28 (_focus)
-                           732 LOAD_CONST               7 ('+')
-                           734 KW_NAMES                 8
-                           736 PRECALL                  3
-                           740 CALL                     3
-                           750 POP_TOP
-               
-                37         752 LOAD_FAST                0 (self)
-                           754 LOAD_ATTR                7 (entry)
-                           764 LOAD_METHOD             23 (bind)
-                           786 LOAD_CONST              12 ('<FocusIn>')
-                           788 LOAD_FAST                0 (self)
-                           790 LOAD_ATTR               28 (_focus)
-                           800 LOAD_CONST               7 ('+')
-                           802 KW_NAMES                 8
-                           804 PRECALL                  3
-                           808 CALL                     3
-                           818 POP_TOP
-               
-                38         820 LOAD_FAST                0 (self)
-                           822 LOAD_METHOD             23 (bind)
-                           844 LOAD_CONST              13 ('<FocusOut>')
-                           846 LOAD_FAST                0 (self)
-                           848 LOAD_ATTR               29 (_focusout)
-                           858 LOAD_CONST               7 ('+')
-                           860 KW_NAMES                 8
-                           862 PRECALL                  3
-                           866 CALL                     3
-                           876 POP_TOP
-               
-                39         878 LOAD_FAST                0 (self)
-                           880 LOAD_ATTR                7 (entry)
-                           890 LOAD_METHOD             23 (bind)
-                           912 LOAD_CONST              13 ('<FocusOut>')
-                           914 LOAD_FAST                0 (self)
-                           916 LOAD_ATTR               29 (_focusout)
-                           926 LOAD_CONST               7 ('+')
-                           928 KW_NAMES                 8
-                           930 PRECALL                  3
-                           934 CALL                     3
-                           944 POP_TOP
-               
-                41         946 LOAD_FAST                0 (self)
-                           948 LOAD_METHOD             24 (_draw)
-                           970 LOAD_CONST               0 (None)
-                           972 PRECALL                  1
-                           976 CALL                     1
-                           986 POP_TOP
-                           988 LOAD_CONST               0 (None)
-                           990 RETURN_VALUE
+                           180 LOAD_CONST               1 (0)
+                           182 KW_NAMES                 4
+                           184 PRECALL                  4
+                           188 CALL                     4
+                           198 LOAD_FAST                0 (self)
+                           200 STORE_ATTR               7 (entry)
+               
+                18         210 LOAD_FAST                0 (self)
+                           212 LOAD_METHOD              8 (_other)
+                           234 PRECALL                  0
+                           238 CALL                     0
+                           248 POP_TOP
+               
+                20         250 LOAD_FAST                0 (self)
+                           252 LOAD_METHOD              9 (default_palette)
+                           274 PRECALL                  0
+                           278 CALL                     0
+                           288 POP_TOP
+               
+                22         290 LOAD_FAST                3 (text)
+                           292 LOAD_FAST                0 (self)
+                           294 STORE_ATTR              10 (text)
+               
+                24         304 LOAD_FAST                0 (self)
+                           306 LOAD_ATTR               11 (entry_back)
+                           316 LOAD_FAST                0 (self)
+                           318 STORE_ATTR              12 (_entry_back)
+               
+                25         328 LOAD_FAST                0 (self)
+                           330 LOAD_ATTR               13 (entry_border)
+                           340 LOAD_FAST                0 (self)
+                           342 STORE_ATTR              14 (_entry_border)
+               
+                26         352 LOAD_FAST                0 (self)
+                           354 LOAD_ATTR               15 (entry_text_back)
+                           364 LOAD_FAST                0 (self)
+                           366 STORE_ATTR              16 (_entry_text_back)
+               
+                27         376 LOAD_FAST                0 (self)
+                           378 LOAD_ATTR               17 (entry_bottom_line)
+                           388 LOAD_FAST                0 (self)
+                           390 STORE_ATTR              18 (_entry_bottom_line)
+               
+                28         400 LOAD_FAST                0 (self)
+                           402 LOAD_ATTR               19 (entry_bottom_width)
+                           412 LOAD_FAST                0 (self)
+                           414 STORE_ATTR              20 (_entry_bottom_width)
+               
+                30         424 LOAD_GLOBAL             43 (NULL + nametofont)
+                           436 LOAD_CONST               5 ('TkDefaultFont')
+                           438 PRECALL                  1
+                           442 CALL                     1
+                           452 LOAD_FAST                0 (self)
+                           454 STORE_ATTR              22 (entry_text_font)
+               
+                32         464 LOAD_FAST                0 (self)
+                           466 LOAD_METHOD             23 (bind)
+                           488 LOAD_CONST               6 ('<Configure>')
+                           490 LOAD_FAST                0 (self)
+                           492 LOAD_ATTR               24 (_draw)
+                           502 LOAD_CONST               7 ('+')
+                           504 KW_NAMES                 8
+                           506 PRECALL                  3
+                           510 CALL                     3
+                           520 POP_TOP
+               
+                33         522 LOAD_FAST                0 (self)
+                           524 LOAD_METHOD             23 (bind)
+                           546 LOAD_CONST               9 ('<Button>')
+                           548 LOAD_FAST                0 (self)
+                           550 LOAD_ATTR               25 (_click)
+                           560 LOAD_CONST               7 ('+')
+                           562 KW_NAMES                 8
+                           564 PRECALL                  3
+                           568 CALL                     3
+                           578 POP_TOP
+               
+                34         580 LOAD_FAST                0 (self)
+                           582 LOAD_METHOD             23 (bind)
+                           604 LOAD_CONST              10 ('<Enter>')
+                           606 LOAD_FAST                0 (self)
+                           608 LOAD_ATTR               26 (_hover)
+                           618 LOAD_CONST               7 ('+')
+                           620 KW_NAMES                 8
+                           622 PRECALL                  3
+                           626 CALL                     3
+                           636 POP_TOP
+               
+                35         638 LOAD_FAST                0 (self)
+                           640 LOAD_METHOD             23 (bind)
+                           662 LOAD_CONST              11 ('<Leave>')
+                           664 LOAD_FAST                0 (self)
+                           666 LOAD_ATTR               27 (_hover_release)
+                           676 LOAD_CONST               7 ('+')
+                           678 KW_NAMES                 8
+                           680 PRECALL                  3
+                           684 CALL                     3
+                           694 POP_TOP
+               
+                36         696 LOAD_FAST                0 (self)
+                           698 LOAD_METHOD             23 (bind)
+                           720 LOAD_CONST              12 ('<FocusIn>')
+                           722 LOAD_FAST                0 (self)
+                           724 LOAD_ATTR               28 (_focus)
+                           734 LOAD_CONST               7 ('+')
+                           736 KW_NAMES                 8
+                           738 PRECALL                  3
+                           742 CALL                     3
+                           752 POP_TOP
+               
+                37         754 LOAD_FAST                0 (self)
+                           756 LOAD_ATTR                7 (entry)
+                           766 LOAD_METHOD             23 (bind)
+                           788 LOAD_CONST              12 ('<FocusIn>')
+                           790 LOAD_FAST                0 (self)
+                           792 LOAD_ATTR               28 (_focus)
+                           802 LOAD_CONST               7 ('+')
+                           804 KW_NAMES                 8
+                           806 PRECALL                  3
+                           810 CALL                     3
+                           820 POP_TOP
+               
+                38         822 LOAD_FAST                0 (self)
+                           824 LOAD_METHOD             23 (bind)
+                           846 LOAD_CONST              13 ('<FocusOut>')
+                           848 LOAD_FAST                0 (self)
+                           850 LOAD_ATTR               29 (_focusout)
+                           860 LOAD_CONST               7 ('+')
+                           862 KW_NAMES                 8
+                           864 PRECALL                  3
+                           868 CALL                     3
+                           878 POP_TOP
+               
+                39         880 LOAD_FAST                0 (self)
+                           882 LOAD_ATTR                7 (entry)
+                           892 LOAD_METHOD             23 (bind)
+                           914 LOAD_CONST              13 ('<FocusOut>')
+                           916 LOAD_FAST                0 (self)
+                           918 LOAD_ATTR               29 (_focusout)
+                           928 LOAD_CONST               7 ('+')
+                           930 KW_NAMES                 8
+                           932 PRECALL                  3
+                           936 CALL                     3
+                           946 POP_TOP
+               
+                41         948 LOAD_FAST                0 (self)
+                           950 LOAD_METHOD             24 (_draw)
+                           972 LOAD_CONST               0 (None)
+                           974 PRECALL                  1
+                           978 CALL                     1
+                           988 POP_TOP
+                           990 LOAD_CONST               0 (None)
+                           992 RETURN_VALUE
                consts
                   None
                   0
                   ('width', 'height', 'highlightthickness')
                   ('StringVar', 'Entry')
-                  ('bd', 'textvariable')
+                  ('bd', 'textvariable', 'highlightthickness')
                   'TkDefaultFont'
                   '<Configure>'
                   '+'
                   ('add',)
                   '<Button>'
                   '<Enter>'
                   '<Leave>'
@@ -656,15 +657,15 @@
                varnames   ('self', 'width', 'height', 'text', 'args', 'kwargs', 'StringVar', 'Entry')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '__init__'
                firstlineno 7
                lnotab
-                  0x04023a0210021e0134023002280228020e021801180118011801180228
+                  0x04023a0210021e0134023202280228020e021801180118011801180228
                   023a013a013a013a013a0144013a014402
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
```

### Comparing `tkadw-0.2.0/tkadw/canvas/__pycache__/frame.cpython-311.pyc` & `tkadw-0.2.1/tkadw/canvas/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc` & `tkadw-0.2.1/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/__pycache__/label.cpython-311.pyc` & `tkadw-0.2.1/tkadw/canvas/__pycache__/label.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.2.1/tkadw/canvas/__pycache__/textbox.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/button.py` & `tkadw-0.2.1/tkadw/canvas/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/drawengine.py` & `tkadw-0.2.1/tkadw/canvas/drawengine.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/entry.py` & `tkadw-0.2.1/tkadw/canvas/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/frame.py` & `tkadw-0.2.1/tkadw/canvas/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/label.py` & `tkadw-0.2.1/tkadw/canvas/label.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/textbox.py` & `tkadw-0.2.1/tkadw/canvas/textbox.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/canvas/titlebar.py` & `tkadw-0.2.1/tkadw/canvas/titlebar.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc` & `tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc` & `tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc` & `tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/label.cpython-311.pyc` & `tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/label.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.2.1/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/tkite/gtk/button.py` & `tkadw-0.2.1/tkadw/tkite/gtk/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/tkite/gtk/entry.py` & `tkadw-0.2.1/tkadw/tkite/gtk/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/tkite/gtk/frame.py` & `tkadw-0.2.1/tkadw/tkite/gtk/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/tkite/gtk/notebook.py` & `tkadw-0.2.1/tkadw/tkite/gtk/notebook.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.0/tkadw/tkite/gtk/textbox.py` & `tkadw-0.2.1/tkadw/tkite/gtk/textbox.py`

 * *Files identical despite different names*

