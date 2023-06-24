# Comparing `tmp/tkadw-0.1.5.tar.gz` & `tmp/tkadw-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkadw-0.1.5.tar", max compression
+gzip compressed data, was "tkadw-0.2.0.tar", max compression
```

## Comparing `tkadw-0.1.5.tar` & `tkadw-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0      272 2023-06-23 09:08:46.990419 tkadw-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3059 2023-06-23 09:04:32.302087 tkadw-0.1.5/README.md
--rw-r--r--   0        0        0      112 2023-06-23 03:45:25.577456 tkadw-0.1.5/tkadw/__init__.py
--rw-r--r--   0        0        0      948 2023-06-23 07:49:26.692233 tkadw-0.1.5/tkadw/__main__.py
--rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.1.5/tkadw/app.config
--rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.1.5/tkadw/appconfig.py
--rw-r--r--   0        0        0      896 2023-06-23 07:36:10.506439 tkadw-0.1.5/tkadw/canvas/__init__.py
--rw-r--r--   0        0        0     1701 2023-06-23 07:38:42.890718 tkadw-0.1.5/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.1.5/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    22885 2023-06-23 04:54:52.588047 tkadw-0.1.5/tkadw/canvas/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.1.5/tkadw/canvas/__pycache__/button.cpython-38.pyc
--rw-r--r--   0        0        0    23239 2023-06-23 05:05:08.679421 tkadw-0.1.5/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
--rw-r--r--   0        0        0    25982 2023-06-23 07:48:50.831965 tkadw-0.1.5/tkadw/canvas/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0    13288 2023-06-23 07:38:42.954769 tkadw-0.1.5/tkadw/canvas/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.1.5/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    29855 2023-06-23 09:08:58.842594 tkadw-0.1.5/tkadw/canvas/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-06-10 10:53:44.353940 tkadw-0.1.5/tkadw/canvas/adwite/__init__.py
--rw-r--r--   0        0        0     1363 2023-06-10 11:23:03.996035 tkadw-0.1.5/tkadw/canvas/adwite/button.py
--rw-r--r--   0        0        0       80 2023-06-09 13:54:04.880107 tkadw-0.1.5/tkadw/canvas/atomize/__init__.py
--rw-r--r--   0        0        0     2520 2023-06-10 04:30:03.863844 tkadw-0.1.5/tkadw/canvas/atomize/button.py
--rw-r--r--   0        0        0    17270 2023-06-23 04:54:52.447686 tkadw-0.1.5/tkadw/canvas/button.py
--rw-r--r--   0        0        0    20382 2023-06-23 05:05:08.591410 tkadw-0.1.5/tkadw/canvas/drawengine.py
--rw-r--r--   0        0        0    22377 2023-06-23 07:48:50.714445 tkadw-0.1.5/tkadw/canvas/entry.py
--rw-r--r--   0        0        0      513 2023-06-09 23:26:21.009369 tkadw-0.1.5/tkadw/canvas/fluent/__init__.py
--rw-r--r--   0        0        0     8629 2023-06-23 05:15:43.010231 tkadw-0.1.5/tkadw/canvas/frame.py
--rw-r--r--   0        0        0     2051 2023-06-10 01:20:40.907297 tkadw-0.1.5/tkadw/canvas/fun.py
--rw-r--r--   0        0        0    15490 2023-06-10 01:25:11.532315 tkadw-0.1.5/tkadw/canvas/fun2.py
--rw-r--r--   0        0        0     8108 2023-06-10 01:29:02.970946 tkadw-0.1.5/tkadw/canvas/fun3.py
--rw-r--r--   0        0        0     3202 2023-06-10 03:27:44.231516 tkadw-0.1.5/tkadw/canvas/fun4.py
--rw-r--r--   0        0        0      942 2023-06-10 03:50:17.322506 tkadw-0.1.5/tkadw/canvas/fun5.py
--rw-r--r--   0        0        0     9870 2023-06-10 07:36:40.103845 tkadw-0.1.5/tkadw/canvas/fun6.py
--rw-r--r--   0        0        0     5690 2023-06-10 03:45:21.292347 tkadw-0.1.5/tkadw/canvas/poly.tcl
--rw-r--r--   0        0        0    23435 2023-06-23 09:08:40.755238 tkadw-0.1.5/tkadw/canvas/textbox.py
--rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.1.5/tkadw/canvas/titlebar.py
--rw-r--r--   0        0        0       29 2023-06-23 03:52:51.957932 tkadw-0.1.5/tkadw/tkite/__init__.py
--rw-r--r--   0        0        0      181 2023-06-23 03:52:52.129145 tkadw-0.1.5/tkadw/tkite/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      283 2023-06-23 07:44:06.875178 tkadw-0.1.5/tkadw/tkite/gtk/__init__.py
--rw-r--r--   0        0        0      620 2023-06-23 07:44:06.983012 tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4518 2023-06-23 08:34:35.190496 tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     3287 2023-06-23 08:39:30.900894 tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     2457 2023-06-23 07:42:27.405172 tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0     3908 2023-06-23 07:45:23.356231 tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0     3726 2023-06-23 08:34:35.056325 tkadw-0.1.5/tkadw/tkite/gtk/button.py
--rw-r--r--   0        0        0     2441 2023-06-23 08:39:30.782792 tkadw-0.1.5/tkadw/tkite/gtk/entry.py
--rw-r--r--   0        0        0     1141 2023-06-23 07:40:36.374539 tkadw-0.1.5/tkadw/tkite/gtk/frame.py
--rw-r--r--   0        0        0      500 2023-06-23 00:56:14.658098 tkadw-0.1.5/tkadw/tkite/gtk/notebook.py
--rw-r--r--   0        0        0     2785 2023-06-23 07:45:23.240982 tkadw-0.1.5/tkadw/tkite/gtk/textbox.py
--rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 tkadw-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      291 2023-06-24 02:04:47.136489 tkadw-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3059 2023-06-23 09:04:32.302087 tkadw-0.2.0/README.md
+-rw-r--r--   0        0        0      112 2023-06-23 03:45:25.577456 tkadw-0.2.0/tkadw/__init__.py
+-rw-r--r--   0        0        0     1176 2023-06-23 11:43:30.799302 tkadw-0.2.0/tkadw/__main__.py
+-rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.2.0/tkadw/app.config
+-rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.2.0/tkadw/appconfig.py
+-rw-r--r--   0        0        0      959 2023-06-23 11:43:18.569764 tkadw-0.2.0/tkadw/canvas/__init__.py
+-rw-r--r--   0        0        0     1801 2023-06-23 11:43:18.792347 tkadw-0.2.0/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.2.0/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    22598 2023-06-24 01:20:36.024808 tkadw-0.2.0/tkadw/canvas/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.2.0/tkadw/canvas/__pycache__/button.cpython-38.pyc
+-rw-r--r--   0        0        0    24261 2023-06-23 09:59:53.052039 tkadw-0.2.0/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
+-rw-r--r--   0        0        0    23648 2023-06-24 01:42:47.540397 tkadw-0.2.0/tkadw/canvas/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0    11871 2023-06-24 01:50:40.515094 tkadw-0.2.0/tkadw/canvas/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.2.0/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     4481 2023-06-24 01:55:47.753570 tkadw-0.2.0/tkadw/canvas/__pycache__/label.cpython-311.pyc
+-rw-r--r--   0        0        0    29583 2023-06-24 02:03:31.982563 tkadw-0.2.0/tkadw/canvas/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0    16890 2023-06-24 01:20:35.915877 tkadw-0.2.0/tkadw/canvas/button.py
+-rw-r--r--   0        0        0    20930 2023-06-23 09:59:52.869076 tkadw-0.2.0/tkadw/canvas/drawengine.py
+-rw-r--r--   0        0        0    17378 2023-06-24 02:04:47.104845 tkadw-0.2.0/tkadw/canvas/entry.py
+-rw-r--r--   0        0        0     6326 2023-06-24 01:50:40.374060 tkadw-0.2.0/tkadw/canvas/frame.py
+-rw-r--r--   0        0        0     2051 2023-06-10 01:20:40.907297 tkadw-0.2.0/tkadw/canvas/fun.py
+-rw-r--r--   0        0        0    15490 2023-06-10 01:25:11.532315 tkadw-0.2.0/tkadw/canvas/fun2.py
+-rw-r--r--   0        0        0     8108 2023-06-10 01:29:02.970946 tkadw-0.2.0/tkadw/canvas/fun3.py
+-rw-r--r--   0        0        0     3202 2023-06-10 03:27:44.231516 tkadw-0.2.0/tkadw/canvas/fun4.py
+-rw-r--r--   0        0        0      942 2023-06-10 03:50:17.322506 tkadw-0.2.0/tkadw/canvas/fun5.py
+-rw-r--r--   0        0        0     9870 2023-06-10 07:36:40.103845 tkadw-0.2.0/tkadw/canvas/fun6.py
+-rw-r--r--   0        0        0     2056 2023-06-24 01:55:37.753942 tkadw-0.2.0/tkadw/canvas/label.py
+-rw-r--r--   0        0        0     5690 2023-06-10 03:45:21.292347 tkadw-0.2.0/tkadw/canvas/poly.tcl
+-rw-r--r--   0        0        0    21800 2023-06-24 02:03:31.849264 tkadw-0.2.0/tkadw/canvas/textbox.py
+-rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.2.0/tkadw/canvas/titlebar.py
+-rw-r--r--   0        0        0     3120 2021-12-23 08:06:14.000000 tkadw-0.2.0/tkadw/tkfontawesome/__init__.py
+-rw-r--r--   0        0        0  1412156 2021-12-23 07:57:18.000000 tkadw-0.2.0/tkadw/tkfontawesome/svgs.py
+-rw-r--r--   0        0        0       29 2023-06-23 03:52:51.957932 tkadw-0.2.0/tkadw/tkite/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-23 03:52:52.129145 tkadw-0.2.0/tkadw/tkite/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      341 2023-06-23 11:43:18.508873 tkadw-0.2.0/tkadw/tkite/gtk/__init__.py
+-rw-r--r--   0        0        0      719 2023-06-23 11:43:19.769317 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4723 2023-06-24 01:29:02.487008 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     3193 2023-06-24 01:44:55.068151 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     2375 2023-06-24 01:51:31.925168 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0     1471 2023-06-23 11:43:19.785605 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/label.cpython-311.pyc
+-rw-r--r--   0        0        0     3149 2023-06-24 02:03:32.305960 tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0     4735 2023-06-24 01:29:02.053861 tkadw-0.2.0/tkadw/tkite/gtk/button.py
+-rw-r--r--   0        0        0     2551 2023-06-24 01:44:54.644195 tkadw-0.2.0/tkadw/tkite/gtk/entry.py
+-rw-r--r--   0        0        0     1125 2023-06-24 01:51:31.490298 tkadw-0.2.0/tkadw/tkite/gtk/frame.py
+-rw-r--r--   0        0        0      359 2023-06-23 11:43:18.648390 tkadw-0.2.0/tkadw/tkite/gtk/label.py
+-rw-r--r--   0        0        0     3555 2023-06-24 00:34:13.973458 tkadw-0.2.0/tkadw/tkite/gtk/notebook.py
+-rw-r--r--   0        0        0     2461 2023-06-24 02:03:31.840946 tkadw-0.2.0/tkadw/tkite/gtk/textbox.py
+-rw-r--r--   0        0        0     3508 1970-01-01 00:00:00.000000 tkadw-0.2.0/PKG-INFO
```

### Comparing `tkadw-0.1.5/README.md` & `tkadw-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/__main__.py` & `tkadw-0.2.0/tkadw/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 from tkinter import Tk
-from tkadw import GTkFrame, GTkDarkFrame, GTkButton, GTkDarkButton, GTkEntry, GTkDarkEntry, GTkTextBox, GTkDarkTextBox
+from tkadw import *
 
 root = Tk()
 root.configure(background="#1f1f1f")
 
 frame = GTkFrame(root)
 
+label1 = GTkLabel(frame.frame, text="GTkLabel")
+label1.pack(fill="x", ipadx=5, padx=5, pady=5)
+
 button1 = GTkButton(frame.frame, text="GTkButton")
 button1.pack(fill="x", ipadx=5, padx=5, pady=5)
 
-entry1 = GTkEntry(frame.frame)
+entry1 = GTkEntry(frame.frame, text="GTkEntry")
 entry1.pack(fill="x", ipadx=5, padx=5, pady=5)
 
 textbox1 = GTkTextBox(frame.frame)
+textbox1.tinsert("1.0", "GTkTextBox")
 textbox1.pack(fill="x", ipadx=5, padx=5, pady=5)
 
 frame.pack(fill="both", expand="yes", side="right")
 
 frame2 = GTkDarkFrame(root)
 
+label2 = GTkDarkLabel(frame2.frame, text="GTkDarkLabel")
+label2.pack(fill="x", ipadx=5, padx=5, pady=5)
+
 button2 = GTkDarkButton(frame2.frame, text="GTkDarkButton")
 button2.pack(fill="x", ipadx=5, padx=5, pady=5)
 
-entry2 = GTkDarkEntry(frame2.frame)
+entry2 = GTkDarkEntry(frame2.frame, text="GTkDarkEntry")
 entry2.pack(fill="x", ipadx=5, padx=5, pady=5)
 
 textbox2 = GTkDarkTextBox(frame2.frame)
+textbox2.tinsert("1.0", "GTkDarkTextBox")
 textbox2.pack(fill="x", ipadx=5, padx=5, pady=5)
 
 frame2.pack(fill="both", expand="yes", side="left")
 
 root.mainloop()
```

### Comparing `tkadw-0.1.5/tkadw/appconfig.py` & `tkadw-0.2.0/tkadw/appconfig.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/canvas/__init__.py` & `tkadw-0.2.0/tkadw/canvas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,7 +6,8 @@
     AdwDrawRoundButton2, AdwDrawRoundDarkButton2, AdwDrawRoundAccentButton2, \
     AdwDrawRoundButton3, AdwDrawRoundDarkButton3, AdwDrawRoundAccentButton3, \
     AdwDrawCircularButton, AdwDrawCircularDarkButton
 from tkadw.canvas.entry import AdwDrawEntry, AdwDrawDarkEntry, AdwDrawRoundEntry, AdwDrawRoundDarkEntry, \
     AdwDrawRoundEntry3, AdwDrawRoundDarkEntry3
 from tkadw.canvas.textbox import AdwDrawText, AdwDrawDarkText, AdwDrawRoundText, AdwDrawRoundDarkText, \
     AdwDrawRoundText3, AdwDrawRoundDarkText3
+from tkadw.canvas.label import AdwDrawLabel, AdwDrawDarkLabel
```

### Comparing `tkadw-0.1.5/tkadw/canvas/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.2.0/tkadw/canvas/__pycache__/__init__.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,22 +1,23 @@
 magic:    0xa70d0d0a
-moddate:  0x6a4b9564 (Fri Jun 23 07:36:10 2023 UTC)
-files sz: 896
+moddate:  0x56859564 (Fri Jun 23 11:43:18 2023 UTC)
+files sz: 959
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
       055a056d065a066d075a076d085a080100640064036c096d0a5a0a6d0b5a
       0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a106d115a116d125a126d
       135a136d145a146d155a156d165a166d175a170100640064046c186d195a
       196d1a5a1a6d1b5a1b6d1c5a1c6d1d5a1d6d1e5a1e0100640064056c1f6d
-      205a206d215a216d225a226d235a236d245a246d255a25010064065300
+      205a206d215a216d225a226d235a236d245a246d255a250100640064066c
+      266d275a276d285a28010064075300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('AdwDrawEngine',))
                  6 IMPORT_NAME              0 (tkadw.canvas.drawengine)
                  8 IMPORT_FROM              1 (AdwDrawEngine)
                 10 STORE_NAME               1 (AdwDrawEngine)
@@ -101,25 +102,35 @@
                160 IMPORT_FROM             35 (AdwDrawRoundDarkText)
                162 STORE_NAME              35 (AdwDrawRoundDarkText)
                164 IMPORT_FROM             36 (AdwDrawRoundText3)
                166 STORE_NAME              36 (AdwDrawRoundText3)
                168 IMPORT_FROM             37 (AdwDrawRoundDarkText3)
                170 STORE_NAME              37 (AdwDrawRoundDarkText3)
                172 POP_TOP
-               174 LOAD_CONST               6 (None)
-               176 RETURN_VALUE
+   
+    13         174 LOAD_CONST               0 (0)
+               176 LOAD_CONST               6 (('AdwDrawLabel', 'AdwDrawDarkLabel'))
+               178 IMPORT_NAME             38 (tkadw.canvas.label)
+               180 IMPORT_FROM             39 (AdwDrawLabel)
+               182 STORE_NAME              39 (AdwDrawLabel)
+               184 IMPORT_FROM             40 (AdwDrawDarkLabel)
+               186 STORE_NAME              40 (AdwDrawDarkLabel)
+               188 POP_TOP
+               190 LOAD_CONST               7 (None)
+               192 RETURN_VALUE
    consts
       0
       ('AdwDrawEngine',)
       ('AdwDrawFrame', 'AdwDrawDarkFrame', 'AdwDrawRoundFrame', 'AdwDrawDarkRoundFrame', 'AdwDrawRoundFrame3', 'AdwDrawDarkRoundFrame3')
       ('AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawRoundButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton')
       ('AdwDrawEntry', 'AdwDrawDarkEntry', 'AdwDrawRoundEntry', 'AdwDrawRoundDarkEntry', 'AdwDrawRoundEntry3', 'AdwDrawRoundDarkEntry3')
       ('AdwDrawText', 'AdwDrawDarkText', 'AdwDrawRoundText', 'AdwDrawRoundDarkText', 'AdwDrawRoundText3', 'AdwDrawRoundDarkText3')
+      ('AdwDrawLabel', 'AdwDrawDarkLabel')
       None
-   names      ('tkadw.canvas.drawengine', 'AdwDrawEngine', 'tkadw.canvas.frame', 'AdwDrawFrame', 'AdwDrawDarkFrame', 'AdwDrawRoundFrame', 'AdwDrawDarkRoundFrame', 'AdwDrawRoundFrame3', 'AdwDrawDarkRoundFrame3', 'tkadw.canvas.button', 'AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawRoundButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton', 'tkadw.canvas.entry', 'AdwDrawEntry', 'AdwDrawDarkEntry', 'AdwDrawRoundEntry', 'AdwDrawRoundDarkEntry', 'AdwDrawRoundEntry3', 'AdwDrawRoundDarkEntry3', 'tkadw.canvas.textbox', 'AdwDrawText', 'AdwDrawDarkText', 'AdwDrawRoundText', 'AdwDrawRoundDarkText', 'AdwDrawRoundText3', 'AdwDrawRoundDarkText3')
+   names      ('tkadw.canvas.drawengine', 'AdwDrawEngine', 'tkadw.canvas.frame', 'AdwDrawFrame', 'AdwDrawDarkFrame', 'AdwDrawRoundFrame', 'AdwDrawDarkRoundFrame', 'AdwDrawRoundFrame3', 'AdwDrawDarkRoundFrame3', 'tkadw.canvas.button', 'AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawRoundButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton', 'tkadw.canvas.entry', 'AdwDrawEntry', 'AdwDrawDarkEntry', 'AdwDrawRoundEntry', 'AdwDrawRoundDarkEntry', 'AdwDrawRoundEntry3', 'AdwDrawRoundDarkEntry3', 'tkadw.canvas.textbox', 'AdwDrawText', 'AdwDrawDarkText', 'AdwDrawRoundText', 'AdwDrawRoundDarkText', 'AdwDrawRoundText3', 'AdwDrawRoundDarkText3', 'tkadw.canvas.label', 'AdwDrawLabel', 'AdwDrawDarkLabel')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\canvas\\__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c01200240052002
+   lnotab 0x00ff02010c012002400520022002
```

### Comparing `tkadw-0.1.5/tkadw/canvas/__pycache__/button.cpython-311.pyc` & `tkadw-0.2.0/tkadw/canvas/__pycache__/button.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x9c259564 (Fri Jun 23 04:54:52 2023 UTC)
-files sz: 17270
+moddate:  0xe3449664 (Sat Jun 24 01:20:35 2023 UTC)
+files sz: 16890
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -71,337 +71,337 @@
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               4 ('AdwDrawBasicButton')
                 40 LOAD_NAME                4 (AdwDrawEngine)
                 42 PRECALL                  3
                 46 CALL                     3
                 56 STORE_NAME               5 (AdwDrawBasicButton)
    
-   189          58 PUSH_NULL
+   194          58 PUSH_NULL
                 60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               5 (<code object AdwDrawButton, file "D:\tkadw\tkadw\canvas\button.py", line 189>)
+                62 LOAD_CONST               5 (<code object AdwDrawButton, file "D:\tkadw\tkadw\canvas\button.py", line 194>)
                 64 MAKE_FUNCTION            0
                 66 LOAD_CONST               6 ('AdwDrawButton')
                 68 LOAD_NAME                5 (AdwDrawBasicButton)
                 70 PRECALL                  3
                 74 CALL                     3
                 84 STORE_NAME               6 (AdwDrawButton)
    
-   194          86 PUSH_NULL
+   199          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object AdwDrawDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 194>)
+                90 LOAD_CONST               7 (<code object AdwDrawDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 199>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('AdwDrawDarkButton')
                 96 LOAD_NAME                5 (AdwDrawBasicButton)
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME               7 (AdwDrawDarkButton)
    
-   199         114 PUSH_NULL
+   204         114 PUSH_NULL
                116 LOAD_BUILD_CLASS
-               118 LOAD_CONST               9 (<code object AdwDrawAccentButton, file "D:\tkadw\tkadw\canvas\button.py", line 199>)
+               118 LOAD_CONST               9 (<code object AdwDrawAccentButton, file "D:\tkadw\tkadw\canvas\button.py", line 204>)
                120 MAKE_FUNCTION            0
                122 LOAD_CONST              10 ('AdwDrawAccentButton')
                124 LOAD_NAME                5 (AdwDrawBasicButton)
                126 PRECALL                  3
                130 CALL                     3
                140 STORE_NAME               8 (AdwDrawAccentButton)
    
-   223         142 PUSH_NULL
+   233         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object AdwDrawBasicRoundButton, file "D:\tkadw\tkadw\canvas\button.py", line 223>)
+               146 LOAD_CONST              11 (<code object AdwDrawBasicRoundButton, file "D:\tkadw\tkadw\canvas\button.py", line 233>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('AdwDrawBasicRoundButton')
                152 LOAD_NAME                5 (AdwDrawBasicButton)
                154 PRECALL                  3
                158 CALL                     3
                168 STORE_NAME               9 (AdwDrawBasicRoundButton)
    
-   338         170 PUSH_NULL
+   318         170 PUSH_NULL
                172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              13 (<code object AdwDrawRoundButton, file "D:\tkadw\tkadw\canvas\button.py", line 338>)
+               174 LOAD_CONST              13 (<code object AdwDrawRoundButton, file "D:\tkadw\tkadw\canvas\button.py", line 318>)
                176 MAKE_FUNCTION            0
                178 LOAD_CONST              14 ('AdwDrawRoundButton')
                180 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                182 PRECALL                  3
                186 CALL                     3
                196 STORE_NAME              10 (AdwDrawRoundButton)
    
-   343         198 PUSH_NULL
+   323         198 PUSH_NULL
                200 LOAD_BUILD_CLASS
-               202 LOAD_CONST              15 (<code object AdwDrawRoundAccentButton, file "D:\tkadw\tkadw\canvas\button.py", line 343>)
+               202 LOAD_CONST              15 (<code object AdwDrawRoundAccentButton, file "D:\tkadw\tkadw\canvas\button.py", line 323>)
                204 MAKE_FUNCTION            0
                206 LOAD_CONST              16 ('AdwDrawRoundAccentButton')
                208 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                210 PRECALL                  3
                214 CALL                     3
                224 STORE_NAME              11 (AdwDrawRoundAccentButton)
    
-   366         226 PUSH_NULL
+   352         226 PUSH_NULL
                228 LOAD_BUILD_CLASS
-               230 LOAD_CONST              17 (<code object AdwDrawRoundDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 366>)
+               230 LOAD_CONST              17 (<code object AdwDrawRoundDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 352>)
                232 MAKE_FUNCTION            0
                234 LOAD_CONST              18 ('AdwDrawRoundDarkButton')
                236 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                238 PRECALL                  3
                242 CALL                     3
                252 STORE_NAME              12 (AdwDrawRoundDarkButton)
    
-   371         254 PUSH_NULL
+   357         254 PUSH_NULL
                256 LOAD_BUILD_CLASS
-               258 LOAD_CONST              19 (<code object AdwDrawRoundButton2, file "D:\tkadw\tkadw\canvas\button.py", line 371>)
+               258 LOAD_CONST              19 (<code object AdwDrawRoundButton2, file "D:\tkadw\tkadw\canvas\button.py", line 357>)
                260 MAKE_FUNCTION            0
                262 LOAD_CONST              20 ('AdwDrawRoundButton2')
                264 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                266 PRECALL                  3
                270 CALL                     3
                280 STORE_NAME              13 (AdwDrawRoundButton2)
    
-   393         282 PUSH_NULL
+   379         282 PUSH_NULL
                284 LOAD_BUILD_CLASS
-               286 LOAD_CONST              21 (<code object AdwDrawRoundAccentButton2, file "D:\tkadw\tkadw\canvas\button.py", line 393>)
+               286 LOAD_CONST              21 (<code object AdwDrawRoundAccentButton2, file "D:\tkadw\tkadw\canvas\button.py", line 379>)
                288 MAKE_FUNCTION            0
                290 LOAD_CONST              22 ('AdwDrawRoundAccentButton2')
                292 LOAD_NAME               13 (AdwDrawRoundButton2)
                294 PRECALL                  3
                298 CALL                     3
                308 STORE_NAME              14 (AdwDrawRoundAccentButton2)
    
-   416         310 PUSH_NULL
+   408         310 PUSH_NULL
                312 LOAD_BUILD_CLASS
-               314 LOAD_CONST              23 (<code object AdwDrawRoundDarkButton2, file "D:\tkadw\tkadw\canvas\button.py", line 416>)
+               314 LOAD_CONST              23 (<code object AdwDrawRoundDarkButton2, file "D:\tkadw\tkadw\canvas\button.py", line 408>)
                316 MAKE_FUNCTION            0
                318 LOAD_CONST              24 ('AdwDrawRoundDarkButton2')
                320 LOAD_NAME               13 (AdwDrawRoundButton2)
                322 PRECALL                  3
                326 CALL                     3
                336 STORE_NAME              15 (AdwDrawRoundDarkButton2)
    
-   421         338 PUSH_NULL
+   413         338 PUSH_NULL
                340 LOAD_BUILD_CLASS
-               342 LOAD_CONST              25 (<code object AdwDrawRoundButton3, file "D:\tkadw\tkadw\canvas\button.py", line 421>)
+               342 LOAD_CONST              25 (<code object AdwDrawRoundButton3, file "D:\tkadw\tkadw\canvas\button.py", line 413>)
                344 MAKE_FUNCTION            0
                346 LOAD_CONST              26 ('AdwDrawRoundButton3')
                348 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                350 PRECALL                  3
                354 CALL                     3
                364 STORE_NAME              16 (AdwDrawRoundButton3)
    
-   443         366 PUSH_NULL
+   435         366 PUSH_NULL
                368 LOAD_BUILD_CLASS
-               370 LOAD_CONST              27 (<code object AdwDrawRoundAccentButton3, file "D:\tkadw\tkadw\canvas\button.py", line 443>)
+               370 LOAD_CONST              27 (<code object AdwDrawRoundAccentButton3, file "D:\tkadw\tkadw\canvas\button.py", line 435>)
                372 MAKE_FUNCTION            0
                374 LOAD_CONST              28 ('AdwDrawRoundAccentButton3')
                376 LOAD_NAME               16 (AdwDrawRoundButton3)
                378 PRECALL                  3
                382 CALL                     3
                392 STORE_NAME              17 (AdwDrawRoundAccentButton3)
    
-   466         394 PUSH_NULL
+   464         394 PUSH_NULL
                396 LOAD_BUILD_CLASS
-               398 LOAD_CONST              29 (<code object AdwDrawRoundDarkButton3, file "D:\tkadw\tkadw\canvas\button.py", line 466>)
+               398 LOAD_CONST              29 (<code object AdwDrawRoundDarkButton3, file "D:\tkadw\tkadw\canvas\button.py", line 464>)
                400 MAKE_FUNCTION            0
                402 LOAD_CONST              30 ('AdwDrawRoundDarkButton3')
                404 LOAD_NAME               16 (AdwDrawRoundButton3)
                406 PRECALL                  3
                410 CALL                     3
                420 STORE_NAME              18 (AdwDrawRoundDarkButton3)
    
-   472         422 PUSH_NULL
+   470         422 PUSH_NULL
                424 LOAD_BUILD_CLASS
-               426 LOAD_CONST              31 (<code object AdwDrawBasicCircularButton, file "D:\tkadw\tkadw\canvas\button.py", line 472>)
+               426 LOAD_CONST              31 (<code object AdwDrawBasicCircularButton, file "D:\tkadw\tkadw\canvas\button.py", line 470>)
                428 MAKE_FUNCTION            0
                430 LOAD_CONST              32 ('AdwDrawBasicCircularButton')
                432 LOAD_NAME                5 (AdwDrawBasicButton)
                434 PRECALL                  3
                438 CALL                     3
                448 STORE_NAME              19 (AdwDrawBasicCircularButton)
    
-   492         450 PUSH_NULL
+   490         450 PUSH_NULL
                452 LOAD_BUILD_CLASS
-               454 LOAD_CONST              33 (<code object AdwDrawCircularButton, file "D:\tkadw\tkadw\canvas\button.py", line 492>)
+               454 LOAD_CONST              33 (<code object AdwDrawCircularButton, file "D:\tkadw\tkadw\canvas\button.py", line 490>)
                456 MAKE_FUNCTION            0
                458 LOAD_CONST              34 ('AdwDrawCircularButton')
                460 LOAD_NAME               19 (AdwDrawBasicCircularButton)
                462 PRECALL                  3
                466 CALL                     3
                476 STORE_NAME              20 (AdwDrawCircularButton)
    
-   497         478 PUSH_NULL
+   495         478 PUSH_NULL
                480 LOAD_BUILD_CLASS
-               482 LOAD_CONST              35 (<code object AdwDrawCircularDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 497>)
+               482 LOAD_CONST              35 (<code object AdwDrawCircularDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 495>)
                484 MAKE_FUNCTION            0
                486 LOAD_CONST              36 ('AdwDrawCircularDarkButton')
                488 LOAD_NAME               19 (AdwDrawBasicCircularButton)
                490 PRECALL                  3
                494 CALL                     3
                504 STORE_NAME              21 (AdwDrawCircularDarkButton)
    
-   502         506 LOAD_NAME               22 (__name__)
+   500         506 LOAD_NAME               22 (__name__)
                508 LOAD_CONST              37 ('__main__')
                510 COMPARE_OP               2 (==)
                516 EXTENDED_ARG             1
                518 POP_JUMP_FORWARD_IF_FALSE   333 (to 1186)
    
-   503         520 LOAD_CONST               0 (0)
+   501         520 LOAD_CONST               0 (0)
                522 LOAD_CONST              38 (('Tk',))
                524 IMPORT_NAME             23 (tkinter)
                526 IMPORT_FROM             24 (Tk)
                528 STORE_NAME              24 (Tk)
                530 POP_TOP
    
-   505         532 PUSH_NULL
+   503         532 PUSH_NULL
                534 LOAD_NAME               24 (Tk)
                536 PRECALL                  0
                540 CALL                     0
                550 STORE_NAME              25 (root)
    
-   507         552 PUSH_NULL
+   505         552 PUSH_NULL
                554 LOAD_NAME                6 (AdwDrawButton)
                556 LOAD_CONST              39 ('Hello')
                558 KW_NAMES                40
                560 PRECALL                  1
                564 CALL                     1
                574 STORE_NAME              26 (button)
    
-   508         576 LOAD_NAME               26 (button)
+   506         576 LOAD_NAME               26 (button)
                578 LOAD_METHOD             27 (bind)
                600 LOAD_CONST              41 ('<<Click>>')
-               602 LOAD_CONST              42 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 508>)
+               602 LOAD_CONST              42 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 506>)
                604 MAKE_FUNCTION            0
                606 PRECALL                  2
                610 CALL                     2
                620 POP_TOP
    
-   509         622 LOAD_NAME               26 (button)
+   507         622 LOAD_NAME               26 (button)
                624 LOAD_METHOD             28 (pack)
                646 LOAD_CONST              43 ('x')
                648 LOAD_CONST              44 (5)
                650 LOAD_CONST              44 (5)
                652 KW_NAMES                45
                654 PRECALL                  3
                658 CALL                     3
                668 POP_TOP
    
-   511         670 PUSH_NULL
+   509         670 PUSH_NULL
                672 LOAD_NAME               10 (AdwDrawRoundButton)
                674 LOAD_CONST              39 ('Hello')
                676 KW_NAMES                40
                678 PRECALL                  1
                682 CALL                     1
                692 STORE_NAME              29 (button4)
    
-   512         694 LOAD_NAME               29 (button4)
+   510         694 LOAD_NAME               29 (button4)
                696 LOAD_METHOD             27 (bind)
                718 LOAD_CONST              41 ('<<Click>>')
-               720 LOAD_CONST              46 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 512>)
+               720 LOAD_CONST              46 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 510>)
                722 MAKE_FUNCTION            0
                724 PRECALL                  2
                728 CALL                     2
                738 POP_TOP
    
-   513         740 LOAD_NAME               29 (button4)
+   511         740 LOAD_NAME               29 (button4)
                742 LOAD_METHOD             28 (pack)
                764 LOAD_CONST              43 ('x')
                766 LOAD_CONST              44 (5)
                768 LOAD_CONST              44 (5)
                770 KW_NAMES                45
                772 PRECALL                  3
                776 CALL                     3
                786 POP_TOP
    
-   515         788 PUSH_NULL
+   513         788 PUSH_NULL
                790 LOAD_NAME               13 (AdwDrawRoundButton2)
                792 LOAD_CONST              39 ('Hello')
                794 KW_NAMES                40
                796 PRECALL                  1
                800 CALL                     1
                810 STORE_NAME              30 (button7)
    
-   516         812 LOAD_NAME               30 (button7)
+   514         812 LOAD_NAME               30 (button7)
                814 LOAD_METHOD             27 (bind)
                836 LOAD_CONST              41 ('<<Click>>')
-               838 LOAD_CONST              47 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 516>)
+               838 LOAD_CONST              47 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 514>)
                840 MAKE_FUNCTION            0
                842 PRECALL                  2
                846 CALL                     2
                856 POP_TOP
    
-   517         858 LOAD_NAME               30 (button7)
+   515         858 LOAD_NAME               30 (button7)
                860 LOAD_METHOD             28 (pack)
                882 LOAD_CONST              43 ('x')
                884 LOAD_CONST              44 (5)
                886 LOAD_CONST              44 (5)
                888 KW_NAMES                45
                890 PRECALL                  3
                894 CALL                     3
                904 POP_TOP
    
-   519         906 PUSH_NULL
+   517         906 PUSH_NULL
                908 LOAD_NAME               16 (AdwDrawRoundButton3)
                910 LOAD_CONST              39 ('Hello')
                912 KW_NAMES                40
                914 PRECALL                  1
                918 CALL                     1
                928 STORE_NAME              31 (button10)
    
-   520         930 LOAD_NAME               31 (button10)
+   518         930 LOAD_NAME               31 (button10)
                932 LOAD_METHOD             27 (bind)
                954 LOAD_CONST              41 ('<<Click>>')
-               956 LOAD_CONST              48 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 520>)
+               956 LOAD_CONST              48 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 518>)
                958 MAKE_FUNCTION            0
                960 PRECALL                  2
                964 CALL                     2
                974 POP_TOP
    
-   521         976 LOAD_NAME               31 (button10)
+   519         976 LOAD_NAME               31 (button10)
                978 LOAD_METHOD             28 (pack)
               1000 LOAD_CONST              43 ('x')
               1002 LOAD_CONST              44 (5)
               1004 LOAD_CONST              44 (5)
               1006 KW_NAMES                45
               1008 PRECALL                  3
               1012 CALL                     3
               1022 POP_TOP
    
-   523        1024 PUSH_NULL
+   521        1024 PUSH_NULL
               1026 LOAD_NAME               20 (AdwDrawCircularButton)
               1028 LOAD_CONST              39 ('Hello')
               1030 KW_NAMES                40
               1032 PRECALL                  1
               1036 CALL                     1
               1046 STORE_NAME              32 (button13)
    
-   524        1048 LOAD_NAME               32 (button13)
+   522        1048 LOAD_NAME               32 (button13)
               1050 LOAD_METHOD             27 (bind)
               1072 LOAD_CONST              41 ('<<Click>>')
-              1074 LOAD_CONST              49 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 524>)
+              1074 LOAD_CONST              49 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 522>)
               1076 MAKE_FUNCTION            0
               1078 PRECALL                  2
               1082 CALL                     2
               1092 POP_TOP
    
-   525        1094 LOAD_NAME               32 (button13)
+   523        1094 LOAD_NAME               32 (button13)
               1096 LOAD_METHOD             28 (pack)
               1118 LOAD_CONST              43 ('x')
               1120 LOAD_CONST              44 (5)
               1122 LOAD_CONST              44 (5)
               1124 KW_NAMES                45
               1126 PRECALL                  3
               1130 CALL                     3
               1140 POP_TOP
    
-   527        1142 LOAD_NAME               25 (root)
+   525        1142 LOAD_NAME               25 (root)
               1144 LOAD_METHOD             33 (mainloop)
               1166 PRECALL                  0
               1170 CALL                     0
               1180 POP_TOP
               1182 LOAD_CONST              50 (None)
               1184 RETURN_VALUE
    
-   502     >> 1186 LOAD_CONST              50 (None)
+   500     >> 1186 LOAD_CONST              50 (None)
               1188 RETURN_VALUE
    consts
       0
       ('Font', 'nametofont')
       ('AdwDrawEngine',)
       code
          argcount  : 0
@@ -433,70 +433,70 @@
                       28 BUILD_TUPLE              2
                       30 LOAD_CLOSURE             0 (__class__)
                       32 BUILD_TUPLE              1
                       34 LOAD_CONST               7 (<code object __init__, file "D:\tkadw\tkadw\canvas\button.py", line 7>)
                       36 MAKE_FUNCTION           14 (kwdefaults, annotations, closure)
                       38 STORE_NAME               4 (__init__)
          
-          33          40 LOAD_CLOSURE             0 (__class__)
+          34          40 LOAD_CLOSURE             0 (__class__)
                       42 BUILD_TUPLE              1
-                      44 LOAD_CONST               8 (<code object configure, file "D:\tkadw\tkadw\canvas\button.py", line 33>)
+                      44 LOAD_CONST               8 (<code object configure, file "D:\tkadw\tkadw\canvas\button.py", line 34>)
                       46 MAKE_FUNCTION            8 (closure)
                       48 STORE_NAME               5 (configure)
          
-          43          50 LOAD_CONST               9 (<code object _other, file "D:\tkadw\tkadw\canvas\button.py", line 43>)
+          44          50 LOAD_CONST               9 (<code object _other, file "D:\tkadw\tkadw\canvas\button.py", line 44>)
                       52 MAKE_FUNCTION            0
                       54 STORE_NAME               6 (_other)
          
-          47          56 LOAD_CONST              10 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 47>)
+          48          56 LOAD_CONST              10 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 48>)
                       58 MAKE_FUNCTION            0
                       60 STORE_NAME               7 (_draw)
          
-          62          62 LOAD_CONST              21 ((None,))
-                      64 LOAD_CONST              11 (<code object _click, file "D:\tkadw\tkadw\canvas\button.py", line 62>)
+          63          62 LOAD_CONST              21 ((None,))
+                      64 LOAD_CONST              11 (<code object _click, file "D:\tkadw\tkadw\canvas\button.py", line 63>)
                       66 MAKE_FUNCTION            1 (defaults)
                       68 STORE_NAME               8 (_click)
          
-          72          70 LOAD_CONST              21 ((None,))
-                      72 LOAD_CONST              12 (<code object _unclick, file "D:\tkadw\tkadw\canvas\button.py", line 72>)
+          74          70 LOAD_CONST              21 ((None,))
+                      72 LOAD_CONST              12 (<code object _unclick, file "D:\tkadw\tkadw\canvas\button.py", line 74>)
                       74 MAKE_FUNCTION            1 (defaults)
                       76 STORE_NAME               9 (_unclick)
          
-          82          78 LOAD_CONST              21 ((None,))
-                      80 LOAD_CONST              13 (<code object _hover, file "D:\tkadw\tkadw\canvas\button.py", line 82>)
+          85          78 LOAD_CONST              21 ((None,))
+                      80 LOAD_CONST              13 (<code object _hover, file "D:\tkadw\tkadw\canvas\button.py", line 85>)
                       82 MAKE_FUNCTION            1 (defaults)
                       84 STORE_NAME              10 (_hover)
          
-          90          86 LOAD_CONST              21 ((None,))
-                      88 LOAD_CONST              14 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\button.py", line 90>)
+          94          86 LOAD_CONST              21 ((None,))
+                      88 LOAD_CONST              14 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\button.py", line 94>)
                       90 MAKE_FUNCTION            1 (defaults)
                       92 STORE_NAME              11 (_hover_release)
          
-          98          94 LOAD_CONST              21 ((None,))
+         103          94 LOAD_CONST              21 ((None,))
                       96 LOAD_CONST              15 ('font')
                       98 LOAD_NAME               12 (Font)
                      100 BUILD_TUPLE              2
-                     102 LOAD_CONST              16 (<code object font, file "D:\tkadw\tkadw\canvas\button.py", line 98>)
+                     102 LOAD_CONST              16 (<code object font, file "D:\tkadw\tkadw\canvas\button.py", line 103>)
                      104 MAKE_FUNCTION            5 (defaults, annotations)
                      106 STORE_NAME              13 (font)
          
-         104         108 LOAD_CONST              17 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 104>)
+         109         108 LOAD_CONST              17 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 109>)
                      110 MAKE_FUNCTION            0
                      112 STORE_NAME              14 (default_palette)
          
-         107         114 LOAD_CONST              18 (<code object palette_light, file "D:\tkadw\tkadw\canvas\button.py", line 107>)
+         112         114 LOAD_CONST              18 (<code object palette_light, file "D:\tkadw\tkadw\canvas\button.py", line 112>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              15 (palette_light)
          
-         128         120 LOAD_CONST              19 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\button.py", line 128>)
+         138         120 LOAD_CONST              19 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\button.py", line 138>)
                      122 MAKE_FUNCTION            0
                      124 STORE_NAME              16 (palette_dark)
          
-         149         126 LOAD_CONST              21 ((None,))
-                     128 LOAD_CONST              20 (<code object palette, file "D:\tkadw\tkadw\canvas\button.py", line 149>)
+         164         126 LOAD_CONST              21 ((None,))
+                     128 LOAD_CONST              20 (<code object palette, file "D:\tkadw\tkadw\canvas\button.py", line 164>)
                      130 MAKE_FUNCTION            1 (defaults)
                      132 STORE_NAME              17 (palette)
                      134 LOAD_CLOSURE             0 (__class__)
                      136 COPY                     1
                      138 STORE_NAME              18 (__classcell__)
                      140 RETURN_VALUE
          consts
@@ -516,30 +516,30 @@
                   0x9501870497000200740100000000000000000000a6000000ab00000000
                   00000000006a0100000000000000007c057c017c026401640164029c047c
                   06a4018e0101007c00a00200000000000000000000000000000000000000
                   00a6000000ab00000000000000000001007c00a003000000000000000000
                   0000000000000000000000a6000000ab00000000000000000001007c037c
                   005f0400000000000000007c006a0500000000000000007c005f06000000
                   00000000007c006a0700000000000000007c005f0800000000000000007c
-                  006a0900000000000000007c005f0a000000000000000074170000000000
-                  00000000006403a6010000ab0100000000000000007c005f0c0000000000
-                  0000007c00a00d000000000000000000000000000000000000000064047c
-                  006a0e00000000000000006405ac06a6030000ab03000000000000000001
-                  007c00a00d000000000000000000000000000000000000000064077c006a
-                  0f00000000000000006405ac06a6030000ab03000000000000000001007c
-                  00a00d000000000000000000000000000000000000000064087c006a1000
-                  000000000000006405ac06a6030000ab03000000000000000001007c00a0
-                  0d000000000000000000000000000000000000000064097c006a11000000
-                  00000000006405ac06a6030000ab03000000000000000001007c00a00d00
-                  00000000000000000000000000000000000000640a7c006a120000000000
-                  0000006405ac06a6030000ab0300000000000000000100890481197c00a0
-                  0d0000000000000000000000000000000000000000640b88046601640c84
-                  08a6020000ab02000000000000000001007c00a00e000000000000000000
-                  00000000000000000000006400a6010000ab010000000000000000010064
-                  005300
+                  006a0900000000000000007c005f0a00000000000000007c006a0b000000
+                  00000000007c005f0c0000000000000000741b0000000000000000000064
+                  03a6010000ab0100000000000000007c005f0e00000000000000007c00a0
+                  0f000000000000000000000000000000000000000064047c006a10000000
+                  00000000006405ac06a6030000ab03000000000000000001007c00a00f00
+                  0000000000000000000000000000000000000064077c006a110000000000
+                  0000006405ac06a6030000ab03000000000000000001007c00a00f000000
+                  000000000000000000000000000000000064087c006a1200000000000000
+                  006405ac06a6030000ab03000000000000000001007c00a00f0000000000
+                  00000000000000000000000000000064097c006a13000000000000000064
+                  05ac06a6030000ab03000000000000000001007c00a00f00000000000000
+                  00000000000000000000000000640a7c006a1400000000000000006405ac
+                  06a6030000ab0300000000000000000100890481197c00a00f0000000000
+                  000000000000000000000000000000640b88046601640c8408a6020000ab
+                  02000000000000000001007c00a010000000000000000000000000000000
+                  00000000006400a6010000ab010000000000000000010064005300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                4 (command)
                
                  7           4 RESUME                   0
                
                  8           6 PUSH_NULL
                              8 LOAD_GLOBAL              1 (NULL + super)
@@ -581,102 +581,107 @@
                
                 17         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                7 (button_border)
                            196 LOAD_FAST                0 (self)
                            198 STORE_ATTR               8 (_button_border)
                
                 18         208 LOAD_FAST                0 (self)
-                           210 LOAD_ATTR                9 (button_text_back)
+                           210 LOAD_ATTR                9 (button_border_width)
                            220 LOAD_FAST                0 (self)
-                           222 STORE_ATTR              10 (_button_text_back)
+                           222 STORE_ATTR              10 (_button_border_width)
                
-                20         232 LOAD_GLOBAL             23 (NULL + nametofont)
-                           244 LOAD_CONST               3 ('TkDefaultFont')
-                           246 PRECALL                  1
-                           250 CALL                     1
-                           260 LOAD_FAST                0 (self)
-                           262 STORE_ATTR              12 (button_text_font)
-               
-                22         272 LOAD_FAST                0 (self)
-                           274 LOAD_METHOD             13 (bind)
-                           296 LOAD_CONST               4 ('<Configure>')
-                           298 LOAD_FAST                0 (self)
-                           300 LOAD_ATTR               14 (_draw)
-                           310 LOAD_CONST               5 ('+')
-                           312 KW_NAMES                 6
-                           314 PRECALL                  3
-                           318 CALL                     3
-                           328 POP_TOP
-               
-                23         330 LOAD_FAST                0 (self)
-                           332 LOAD_METHOD             13 (bind)
-                           354 LOAD_CONST               7 ('<Button>')
-                           356 LOAD_FAST                0 (self)
-                           358 LOAD_ATTR               15 (_click)
-                           368 LOAD_CONST               5 ('+')
-                           370 KW_NAMES                 6
-                           372 PRECALL                  3
-                           376 CALL                     3
-                           386 POP_TOP
-               
-                24         388 LOAD_FAST                0 (self)
-                           390 LOAD_METHOD             13 (bind)
-                           412 LOAD_CONST               8 ('<ButtonRelease>')
-                           414 LOAD_FAST                0 (self)
-                           416 LOAD_ATTR               16 (_unclick)
-                           426 LOAD_CONST               5 ('+')
-                           428 KW_NAMES                 6
-                           430 PRECALL                  3
-                           434 CALL                     3
-                           444 POP_TOP
-               
-                25         446 LOAD_FAST                0 (self)
-                           448 LOAD_METHOD             13 (bind)
-                           470 LOAD_CONST               9 ('<Enter>')
-                           472 LOAD_FAST                0 (self)
-                           474 LOAD_ATTR               17 (_hover)
-                           484 LOAD_CONST               5 ('+')
-                           486 KW_NAMES                 6
-                           488 PRECALL                  3
-                           492 CALL                     3
-                           502 POP_TOP
-               
-                26         504 LOAD_FAST                0 (self)
-                           506 LOAD_METHOD             13 (bind)
-                           528 LOAD_CONST              10 ('<Leave>')
-                           530 LOAD_FAST                0 (self)
-                           532 LOAD_ATTR               18 (_hover_release)
-                           542 LOAD_CONST               5 ('+')
-                           544 KW_NAMES                 6
-                           546 PRECALL                  3
-                           550 CALL                     3
-                           560 POP_TOP
-               
-                28         562 LOAD_DEREF               4 (command)
-                           564 POP_JUMP_FORWARD_IF_NONE    25 (to 616)
-               
-                29         566 LOAD_FAST                0 (self)
-                           568 LOAD_METHOD             13 (bind)
-                           590 LOAD_CONST              11 ('<<Click>>')
-                           592 LOAD_CLOSURE             4 (command)
-                           594 BUILD_TUPLE              1
-                           596 LOAD_CONST              12 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 29>)
-                           598 MAKE_FUNCTION            8 (closure)
-                           600 PRECALL                  2
-                           604 CALL                     2
-                           614 POP_TOP
-               
-                31     >>  616 LOAD_FAST                0 (self)
-                           618 LOAD_METHOD             14 (_draw)
-                           640 LOAD_CONST               0 (None)
-                           642 PRECALL                  1
-                           646 CALL                     1
-                           656 POP_TOP
-                           658 LOAD_CONST               0 (None)
-                           660 RETURN_VALUE
+                19         232 LOAD_FAST                0 (self)
+                           234 LOAD_ATTR               11 (button_text_back)
+                           244 LOAD_FAST                0 (self)
+                           246 STORE_ATTR              12 (_button_text_back)
+               
+                21         256 LOAD_GLOBAL             27 (NULL + nametofont)
+                           268 LOAD_CONST               3 ('TkDefaultFont')
+                           270 PRECALL                  1
+                           274 CALL                     1
+                           284 LOAD_FAST                0 (self)
+                           286 STORE_ATTR              14 (button_text_font)
+               
+                23         296 LOAD_FAST                0 (self)
+                           298 LOAD_METHOD             15 (bind)
+                           320 LOAD_CONST               4 ('<Configure>')
+                           322 LOAD_FAST                0 (self)
+                           324 LOAD_ATTR               16 (_draw)
+                           334 LOAD_CONST               5 ('+')
+                           336 KW_NAMES                 6
+                           338 PRECALL                  3
+                           342 CALL                     3
+                           352 POP_TOP
+               
+                24         354 LOAD_FAST                0 (self)
+                           356 LOAD_METHOD             15 (bind)
+                           378 LOAD_CONST               7 ('<Button>')
+                           380 LOAD_FAST                0 (self)
+                           382 LOAD_ATTR               17 (_click)
+                           392 LOAD_CONST               5 ('+')
+                           394 KW_NAMES                 6
+                           396 PRECALL                  3
+                           400 CALL                     3
+                           410 POP_TOP
+               
+                25         412 LOAD_FAST                0 (self)
+                           414 LOAD_METHOD             15 (bind)
+                           436 LOAD_CONST               8 ('<ButtonRelease>')
+                           438 LOAD_FAST                0 (self)
+                           440 LOAD_ATTR               18 (_unclick)
+                           450 LOAD_CONST               5 ('+')
+                           452 KW_NAMES                 6
+                           454 PRECALL                  3
+                           458 CALL                     3
+                           468 POP_TOP
+               
+                26         470 LOAD_FAST                0 (self)
+                           472 LOAD_METHOD             15 (bind)
+                           494 LOAD_CONST               9 ('<Enter>')
+                           496 LOAD_FAST                0 (self)
+                           498 LOAD_ATTR               19 (_hover)
+                           508 LOAD_CONST               5 ('+')
+                           510 KW_NAMES                 6
+                           512 PRECALL                  3
+                           516 CALL                     3
+                           526 POP_TOP
+               
+                27         528 LOAD_FAST                0 (self)
+                           530 LOAD_METHOD             15 (bind)
+                           552 LOAD_CONST              10 ('<Leave>')
+                           554 LOAD_FAST                0 (self)
+                           556 LOAD_ATTR               20 (_hover_release)
+                           566 LOAD_CONST               5 ('+')
+                           568 KW_NAMES                 6
+                           570 PRECALL                  3
+                           574 CALL                     3
+                           584 POP_TOP
+               
+                29         586 LOAD_DEREF               4 (command)
+                           588 POP_JUMP_FORWARD_IF_NONE    25 (to 640)
+               
+                30         590 LOAD_FAST                0 (self)
+                           592 LOAD_METHOD             15 (bind)
+                           614 LOAD_CONST              11 ('<<Click>>')
+                           616 LOAD_CLOSURE             4 (command)
+                           618 BUILD_TUPLE              1
+                           620 LOAD_CONST              12 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 30>)
+                           622 MAKE_FUNCTION            8 (closure)
+                           624 PRECALL                  2
+                           628 CALL                     2
+                           638 POP_TOP
+               
+                32     >>  640 LOAD_FAST                0 (self)
+                           642 LOAD_METHOD             16 (_draw)
+                           664 LOAD_CONST               0 (None)
+                           666 PRECALL                  1
+                           670 CALL                     1
+                           680 POP_TOP
+                           682 LOAD_CONST               0 (None)
+                           684 RETURN_VALUE
                consts
                   None
                   0
                   ('width', 'height', 'bd', 'highlightthickness')
                   'TkDefaultFont'
                   '<Configure>'
                   '+'
@@ -690,40 +695,40 @@
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code 0x9501970002008901a6000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      29           2 RESUME                   0
+                      30           2 RESUME                   0
                                    4 PUSH_NULL
                                    6 LOAD_DEREF               1 (command)
                                    8 PRECALL                  0
                                   12 CALL                     0
                                   22 RETURN_VALUE
                      consts
                         None
                      names      ()
                      varnames   ('event',)
                      freevars   ('command',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                      name       '<lambda>'
-                     firstlineno 29
+                     firstlineno 30
                      lnotab 0x
-               names      ('super', '__init__', '_other', 'default_palette', 'text', 'button_back', '_button_back', 'button_border', '_button_border', 'button_text_back', '_button_text_back', 'nametofont', 'button_text_font', 'bind', '_draw', '_click', '_unclick', '_hover', '_hover_release')
+               names      ('super', '__init__', '_other', 'default_palette', 'text', 'button_back', '_button_back', 'button_border', '_button_border', 'button_border_width', '_button_border_width', 'button_text_back', '_button_text_back', 'nametofont', 'button_text_font', 'bind', '_draw', '_click', '_unclick', '_hover', '_hover_release')
                varnames   ('self', 'width', 'height', 'text', 'command', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ('command',)
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '__init__'
                firstlineno 7
                lnotab
-                  0x06013c02280228020e0218011801180228023a013a013a013a013a0204
-                  013202
+                  0x06013c02280228020e02180118011801180228023a013a013a013a013a
+                  0204013202
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 11
                code
                   0x95018700970064017c01760072357c01a0000000000000000000000000
@@ -735,65 +740,65 @@
                   008900a00400000000000000000000000000000000000000006400a60100
                   00ab0100000000000000000100640053000200740b000000000000000000
                   00a6000000ab0000000000000000006a060000000000000000640569007c
                   01a4018e01010064005300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                0 (self)
                
-                33           4 RESUME                   0
+                34           4 RESUME                   0
                
-                34           6 LOAD_CONST               1 ('command')
+                35           6 LOAD_CONST               1 ('command')
                              8 LOAD_FAST                1 (kwargs)
                             10 CONTAINS_OP              0
                             12 POP_JUMP_FORWARD_IF_FALSE    53 (to 120)
                
-                35          14 LOAD_FAST                1 (kwargs)
+                36          14 LOAD_FAST                1 (kwargs)
                             16 LOAD_METHOD              0 (pop)
                             38 LOAD_CONST               1 ('command')
                             40 PRECALL                  1
                             44 CALL                     1
                             54 LOAD_DEREF               0 (self)
                             56 STORE_ATTR               1 (command)
                
-                36          66 LOAD_DEREF               0 (self)
+                37          66 LOAD_DEREF               0 (self)
                             68 LOAD_METHOD              2 (bind)
                             90 LOAD_CONST               2 ('<<Click>>')
                             92 LOAD_CLOSURE             0 (self)
                             94 BUILD_TUPLE              1
-                            96 LOAD_CONST               3 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 36>)
+                            96 LOAD_CONST               3 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 37>)
                             98 MAKE_FUNCTION            8 (closure)
                            100 PRECALL                  2
                            104 CALL                     2
                            114 POP_TOP
                            116 LOAD_CONST               0 (None)
                            118 RETURN_VALUE
                
-                37     >>  120 LOAD_CONST               4 ('text')
+                38     >>  120 LOAD_CONST               4 ('text')
                            122 LOAD_FAST                1 (kwargs)
                            124 CONTAINS_OP              0
                            126 POP_JUMP_FORWARD_IF_FALSE    49 (to 226)
                
-                38         128 LOAD_FAST                1 (kwargs)
+                39         128 LOAD_FAST                1 (kwargs)
                            130 LOAD_METHOD              0 (pop)
                            152 LOAD_CONST               4 ('text')
                            154 PRECALL                  1
                            158 CALL                     1
                            168 LOAD_DEREF               0 (self)
                            170 STORE_ATTR               3 (text)
                
-                39         180 LOAD_DEREF               0 (self)
+                40         180 LOAD_DEREF               0 (self)
                            182 LOAD_METHOD              4 (_draw)
                            204 LOAD_CONST               0 (None)
                            206 PRECALL                  1
                            210 CALL                     1
                            220 POP_TOP
                            222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                
-                41     >>  226 PUSH_NULL
+                42     >>  226 PUSH_NULL
                            228 LOAD_GLOBAL             11 (NULL + super)
                            240 PRECALL                  0
                            244 CALL                     0
                            254 LOAD_ATTR                6 (configure)
                            264 LOAD_CONST               5 (())
                            266 BUILD_MAP                0
                            268 LOAD_FAST                1 (kwargs)
@@ -812,85 +817,85 @@
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      36           2 RESUME                   0
+                      37           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (command)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('command',)
                      varnames   ('event',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                      name       '<lambda>'
-                     firstlineno 36
+                     firstlineno 37
                      lnotab 0x
                   'text'
                   ()
                names      ('pop', 'command', 'bind', 'text', '_draw', 'super', 'configure')
                varnames   ('self', 'kwargs')
                freevars   ('__class__',)
                cellvars   ('self',)
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'configure'
-               firstlineno 33
+               firstlineno 34
                lnotab 0x0601080134013601080134012e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006401a6020000ab020000000000
                   000000721e7c00a00100000000000000000000000000000000000000007c
                   006a0200000000000000006402ac03a6020000ab02000000000000000001
                   006400530064005300
-                43           0 RESUME                   0
+                44           0 RESUME                   0
                
-                44           2 LOAD_GLOBAL              1 (NULL + hasattr)
+                45           2 LOAD_GLOBAL              1 (NULL + hasattr)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_CONST               1 ('button_frame_back')
                             18 PRECALL                  2
                             22 CALL                     2
                             32 POP_JUMP_FORWARD_IF_FALSE    30 (to 94)
                
-                45          34 LOAD_FAST                0 (self)
+                46          34 LOAD_FAST                0 (self)
                             36 LOAD_METHOD              1 (configure)
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                2 (button_frame_back)
                             70 LOAD_CONST               2 (0)
                             72 KW_NAMES                 3
                             74 PRECALL                  2
                             78 CALL                     2
                             88 POP_TOP
                             90 LOAD_CONST               0 (None)
                             92 RETURN_VALUE
                
-                44     >>   94 LOAD_CONST               0 (None)
+                45     >>   94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                consts
                   None
                   'button_frame_back'
                   0
                   ('background', 'borderwidth')
                names      ('hasattr', 'configure', 'button_frame_back')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_other'
-               firstlineno 43
+               firstlineno 44
                lnotab 0x020120013cff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 9
                flags     : 3
                code
@@ -904,987 +909,1089 @@
                   0000007c005f0700000000000000007c00a0080000000000000000000000
                   0000000000000000007c00a0020000000000000000000000000000000000
                   000000a6000000ab00000000000000000064057a0b00007c00a003000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0064057a0b00007c006a0900000000000000007c006a0a00000000000000
                   007c006a0b0000000000000000ac06a6050000ab0500000000000000007c
                   005f0c000000000000000064005300
-                47           0 RESUME                   0
+                48           0 RESUME                   0
                
-                48           2 LOAD_FAST                0 (self)
+                49           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-                50          44 LOAD_FAST                0 (self)
+                51          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_rectangle)
                
-                51          68 LOAD_CONST               2 (1.5)
+                52          68 LOAD_CONST               2 (1.5)
                             70 LOAD_CONST               2 (1.5)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
                            116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                
-                52         160 LOAD_FAST                0 (self)
-                           162 LOAD_ATTR                4 (button_border_width)
+                53         160 LOAD_FAST                0 (self)
+                           162 LOAD_ATTR                4 (_button_border_width)
                
-                53         172 LOAD_FAST                0 (self)
+                54         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (_button_border)
                            184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_button_back)
                
-                50         196 KW_NAMES                 4
+                51         196 KW_NAMES                 4
                            198 PRECALL                  7
                            202 CALL                     7
                            212 LOAD_FAST                0 (self)
                            214 STORE_ATTR               7 (button_frame)
                
-                56         224 LOAD_FAST                0 (self)
+                57         224 LOAD_FAST                0 (self)
                            226 LOAD_METHOD              8 (create_text)
                
-                57         248 LOAD_FAST                0 (self)
+                58         248 LOAD_FAST                0 (self)
                            250 LOAD_METHOD              2 (winfo_width)
                            272 PRECALL                  0
                            276 CALL                     0
                            286 LOAD_CONST               5 (2)
                            288 BINARY_OP               11 (/)
                            292 LOAD_FAST                0 (self)
                            294 LOAD_METHOD              3 (winfo_height)
                            316 PRECALL                  0
                            320 CALL                     0
                            330 LOAD_CONST               5 (2)
                            332 BINARY_OP               11 (/)
                
-                58         336 LOAD_FAST                0 (self)
+                59         336 LOAD_FAST                0 (self)
                            338 LOAD_ATTR                9 (text)
                            348 LOAD_FAST                0 (self)
                            350 LOAD_ATTR               10 (_button_text_back)
                
-                59         360 LOAD_FAST                0 (self)
+                60         360 LOAD_FAST                0 (self)
                            362 LOAD_ATTR               11 (button_text_font)
                
-                56         372 KW_NAMES                 6
+                57         372 KW_NAMES                 6
                            374 PRECALL                  5
                            378 CALL                     5
                            388 LOAD_FAST                0 (self)
                            390 STORE_ATTR              12 (button_text)
                            400 LOAD_CONST               0 (None)
                            402 RETURN_VALUE
                consts
                   None
                   'all'
                   1.5
                   3
                   ('width', 'outline', 'fill')
                   2
                   ('text', 'fill', 'font')
-               names      ('delete', 'create_rectangle', 'winfo_width', 'winfo_height', 'button_border_width', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
+               names      ('delete', 'create_rectangle', 'winfo_width', 'winfo_height', '_button_border_width', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_draw'
-               firstlineno 47
+               firstlineno 48
                lnotab 0x02012a0218015c010c0118fd1c061801580118010cfd
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x970064017c005f0000000000000000007c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
-                  00a0070000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000001007c00a0080000000000000000000000000000000000
-                  0000006400a6010000ab010000000000000000010064005300
-                62           0 RESUME                   0
+                  006a0700000000000000007c005f0800000000000000007c00a009000000
+                  0000000000000000000000000000000000a6000000ab0000000000000000
+                  0001007c00a00a00000000000000000000000000000000000000006400a6
+                  010000ab010000000000000000010064005300
+                63           0 RESUME                   0
                
-                63           2 LOAD_CONST               1 (True)
+                64           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                
-                64          16 LOAD_FAST                0 (self)
+                65          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_pressed_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                65          40 LOAD_FAST                0 (self)
+                66          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_pressed_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                66          64 LOAD_FAST                0 (self)
-                            66 LOAD_ATTR                5 (button_pressed_text_back)
+                67          64 LOAD_FAST                0 (self)
+                            66 LOAD_ATTR                5 (button_pressed_border_width)
                             76 LOAD_FAST                0 (self)
-                            78 STORE_ATTR               6 (_button_text_back)
+                            78 STORE_ATTR               6 (_button_border_width)
                
                 68          88 LOAD_FAST                0 (self)
-                            90 LOAD_METHOD              7 (focus_set)
-                           112 PRECALL                  0
-                           116 CALL                     0
-                           126 POP_TOP
-               
-                70         128 LOAD_FAST                0 (self)
-                           130 LOAD_METHOD              8 (_draw)
-                           152 LOAD_CONST               0 (None)
-                           154 PRECALL                  1
-                           158 CALL                     1
-                           168 POP_TOP
-                           170 LOAD_CONST               0 (None)
-                           172 RETURN_VALUE
+                            90 LOAD_ATTR                7 (button_pressed_text_back)
+                           100 LOAD_FAST                0 (self)
+                           102 STORE_ATTR               8 (_button_text_back)
+               
+                70         112 LOAD_FAST                0 (self)
+                           114 LOAD_METHOD              9 (focus_set)
+                           136 PRECALL                  0
+                           140 CALL                     0
+                           150 POP_TOP
+               
+                72         152 LOAD_FAST                0 (self)
+                           154 LOAD_METHOD             10 (_draw)
+                           176 LOAD_CONST               0 (None)
+                           178 PRECALL                  1
+                           182 CALL                     1
+                           192 POP_TOP
+                           194 LOAD_CONST               0 (None)
+                           196 RETURN_VALUE
                consts
                   None
                   True
-               names      ('hover', 'button_pressed_back', '_button_back', 'button_pressed_border', '_button_border', 'button_pressed_text_back', '_button_text_back', 'focus_set', '_draw')
+               names      ('hover', 'button_pressed_back', '_button_back', 'button_pressed_border', '_button_border', 'button_pressed_border_width', '_button_border_width', 'button_pressed_text_back', '_button_text_back', 'focus_set', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_click'
-               firstlineno 62
-               lnotab 0x02010e011801180118022802
+               firstlineno 63
+               lnotab 0x02010e0118011801180118022802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
-                  0x97007c006a00000000000000000072507c006a0100000000000000007c
+                  0x97007c006a000000000000000000725c7c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
-                  00a00700000000000000000000000000000000000000006400a6010000ab
-                  01000000000000000001007c00a008000000000000000000000000000000
-                  00000000006401a6010000ab010000000000000000010064005300640053
-                  00
-                72           0 RESUME                   0
+                  006a0700000000000000007c005f0800000000000000007c00a009000000
+                  00000000000000000000000000000000006400a6010000ab010000000000
+                  00000001007c00a00a000000000000000000000000000000000000000064
+                  01a6010000ab01000000000000000001006400530064005300
+                74           0 RESUME                   0
                
-                73           2 LOAD_FAST                0 (self)
+                75           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (hover)
-                            14 POP_JUMP_FORWARD_IF_FALSE    80 (to 176)
+                            14 POP_JUMP_FORWARD_IF_FALSE    92 (to 200)
                
-                74          16 LOAD_FAST                0 (self)
+                76          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_active_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                75          40 LOAD_FAST                0 (self)
+                77          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_active_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                76          64 LOAD_FAST                0 (self)
-                            66 LOAD_ATTR                5 (button_active_text_back)
+                78          64 LOAD_FAST                0 (self)
+                            66 LOAD_ATTR                5 (button_active_border_width)
                             76 LOAD_FAST                0 (self)
-                            78 STORE_ATTR               6 (_button_text_back)
+                            78 STORE_ATTR               6 (_button_border_width)
                
-                78          88 LOAD_FAST                0 (self)
-                            90 LOAD_METHOD              7 (_draw)
-                           112 LOAD_CONST               0 (None)
-                           114 PRECALL                  1
-                           118 CALL                     1
-                           128 POP_TOP
-               
-                80         130 LOAD_FAST                0 (self)
-                           132 LOAD_METHOD              8 (event_generate)
-                           154 LOAD_CONST               1 ('<<Click>>')
-                           156 PRECALL                  1
-                           160 CALL                     1
-                           170 POP_TOP
-                           172 LOAD_CONST               0 (None)
-                           174 RETURN_VALUE
+                79          88 LOAD_FAST                0 (self)
+                            90 LOAD_ATTR                7 (button_active_text_back)
+                           100 LOAD_FAST                0 (self)
+                           102 STORE_ATTR               8 (_button_text_back)
+               
+                81         112 LOAD_FAST                0 (self)
+                           114 LOAD_METHOD              9 (_draw)
+                           136 LOAD_CONST               0 (None)
+                           138 PRECALL                  1
+                           142 CALL                     1
+                           152 POP_TOP
+               
+                83         154 LOAD_FAST                0 (self)
+                           156 LOAD_METHOD             10 (event_generate)
+                           178 LOAD_CONST               1 ('<<Click>>')
+                           180 PRECALL                  1
+                           184 CALL                     1
+                           194 POP_TOP
+                           196 LOAD_CONST               0 (None)
+                           198 RETURN_VALUE
                
-                73     >>  176 LOAD_CONST               0 (None)
-                           178 RETURN_VALUE
+                75     >>  200 LOAD_CONST               0 (None)
+                           202 RETURN_VALUE
                consts
                   None
                   '<<Click>>'
-               names      ('hover', 'button_active_back', '_button_back', 'button_active_border', '_button_border', 'button_active_text_back', '_button_text_back', '_draw', 'event_generate')
+               names      ('hover', 'button_active_back', '_button_back', 'button_active_border', '_button_border', 'button_active_border_width', '_button_border_width', 'button_active_text_back', '_button_text_back', '_draw', 'event_generate')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_unclick'
-               firstlineno 72
-               lnotab 0x02010e011801180118022a022ef9
+               firstlineno 74
+               lnotab 0x02010e0118011801180118022a022ef8
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x970064017c005f0000000000000000007c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
-                  00a00700000000000000000000000000000000000000006400a6010000ab
-                  010000000000000000010064005300
-                82           0 RESUME                   0
+                  006a0700000000000000007c005f0800000000000000007c00a009000000
+                  00000000000000000000000000000000006400a6010000ab010000000000
+                  000000010064005300
+                85           0 RESUME                   0
                
-                83           2 LOAD_CONST               1 (True)
+                86           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                
-                84          16 LOAD_FAST                0 (self)
+                87          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_active_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                85          40 LOAD_FAST                0 (self)
+                88          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_active_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                86          64 LOAD_FAST                0 (self)
-                            66 LOAD_ATTR                5 (button_active_text_back)
+                89          64 LOAD_FAST                0 (self)
+                            66 LOAD_ATTR                5 (button_active_border_width)
                             76 LOAD_FAST                0 (self)
-                            78 STORE_ATTR               6 (_button_text_back)
+                            78 STORE_ATTR               6 (_button_border_width)
                
-                88          88 LOAD_FAST                0 (self)
-                            90 LOAD_METHOD              7 (_draw)
-                           112 LOAD_CONST               0 (None)
-                           114 PRECALL                  1
-                           118 CALL                     1
-                           128 POP_TOP
-                           130 LOAD_CONST               0 (None)
-                           132 RETURN_VALUE
+                90          88 LOAD_FAST                0 (self)
+                            90 LOAD_ATTR                7 (button_active_text_back)
+                           100 LOAD_FAST                0 (self)
+                           102 STORE_ATTR               8 (_button_text_back)
+               
+                92         112 LOAD_FAST                0 (self)
+                           114 LOAD_METHOD              9 (_draw)
+                           136 LOAD_CONST               0 (None)
+                           138 PRECALL                  1
+                           142 CALL                     1
+                           152 POP_TOP
+                           154 LOAD_CONST               0 (None)
+                           156 RETURN_VALUE
                consts
                   None
                   True
-               names      ('hover', 'button_active_back', '_button_back', 'button_active_border', '_button_border', 'button_active_text_back', '_button_text_back', '_draw')
+               names      ('hover', 'button_active_back', '_button_back', 'button_active_border', '_button_border', 'button_active_border_width', '_button_border_width', 'button_active_text_back', '_button_text_back', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_hover'
-               firstlineno 82
-               lnotab 0x02010e01180118011802
+               firstlineno 85
+               lnotab 0x02010e011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x970064017c005f0000000000000000007c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
-                  00a00700000000000000000000000000000000000000006400a6010000ab
-                  010000000000000000010064005300
-                90           0 RESUME                   0
+                  006a0700000000000000007c005f0800000000000000007c00a009000000
+                  00000000000000000000000000000000006400a6010000ab010000000000
+                  000000010064005300
+                94           0 RESUME                   0
                
-                91           2 LOAD_CONST               1 (False)
+                95           2 LOAD_CONST               1 (False)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                
-                92          16 LOAD_FAST                0 (self)
+                96          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                93          40 LOAD_FAST                0 (self)
+                97          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                94          64 LOAD_FAST                0 (self)
-                            66 LOAD_ATTR                5 (button_text_back)
+                98          64 LOAD_FAST                0 (self)
+                            66 LOAD_ATTR                5 (button_border_width)
                             76 LOAD_FAST                0 (self)
-                            78 STORE_ATTR               6 (_button_text_back)
+                            78 STORE_ATTR               6 (_button_border_width)
                
-                96          88 LOAD_FAST                0 (self)
-                            90 LOAD_METHOD              7 (_draw)
-                           112 LOAD_CONST               0 (None)
-                           114 PRECALL                  1
-                           118 CALL                     1
-                           128 POP_TOP
-                           130 LOAD_CONST               0 (None)
-                           132 RETURN_VALUE
+                99          88 LOAD_FAST                0 (self)
+                            90 LOAD_ATTR                7 (button_text_back)
+                           100 LOAD_FAST                0 (self)
+                           102 STORE_ATTR               8 (_button_text_back)
+               
+               101         112 LOAD_FAST                0 (self)
+                           114 LOAD_METHOD              9 (_draw)
+                           136 LOAD_CONST               0 (None)
+                           138 PRECALL                  1
+                           142 CALL                     1
+                           152 POP_TOP
+                           154 LOAD_CONST               0 (None)
+                           156 RETURN_VALUE
                consts
                   None
                   False
-               names      ('hover', 'button_back', '_button_back', 'button_border', '_button_border', 'button_text_back', '_button_text_back', '_draw')
+               names      ('hover', 'button_back', '_button_back', 'button_border', '_button_border', 'button_border_width', '_button_border_width', 'button_text_back', '_button_text_back', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_hover_release'
-               firstlineno 90
-               lnotab 0x02010e01180118011802
+               firstlineno 94
+               lnotab 0x02010e011801180118011802
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-                98           0 RESUME                   0
+               103           0 RESUME                   0
                
-                99           2 LOAD_FAST                1 (font)
+               104           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               100           6 LOAD_FAST                0 (self)
+               105           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_text_font)
                             18 RETURN_VALUE
                
-               102     >>   20 LOAD_FAST                1 (font)
+               107     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'font'
-               firstlineno 98
+               firstlineno 103
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               104           0 RESUME                   0
+               109           0 RESUME                   0
                
-               105           2 LOAD_FAST                0 (self)
+               110           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 104
+               firstlineno 109
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 14
+               stacksize : 13
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  02640364046405640664076408640664076409640a9c0ba6010000ab0100
-                  00000000000000010064005300
-               107           0 RESUME                   0
+                  02640364046405640664076408640564099c046406640a640b640564099c
+                  04640c9c066901a6010000ab010000000000000000010064005300
+               112           0 RESUME                   0
                
-               108           2 LOAD_FAST                0 (self)
+               113           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               110          26 LOAD_CONST               1 ('#f3f3f3')
+               115          26 LOAD_CONST               1 ('button')
+               
+               116          28 LOAD_CONST               2 ('#fdfdfd')
                
-               112          28 LOAD_CONST               2 (1)
+               117          30 LOAD_CONST               3 ('#eaeaea')
                
-               114          30 LOAD_CONST               3 ('#eaeaea')
+               118          32 LOAD_CONST               4 ('#1a1a1a')
                
-               115          32 LOAD_CONST               4 ('#fdfdfd')
+               119          34 LOAD_CONST               5 (1)
                
-               116          34 LOAD_CONST               5 ('#1a1a1a')
+               122          36 LOAD_CONST               6 ('#f9f9f9')
                
-               118          36 LOAD_CONST               6 ('#e2e2e2')
+               123          38 LOAD_CONST               7 ('#aaaaaa')
                
-               119          38 LOAD_CONST               7 ('#f9f9f9')
+               124          40 LOAD_CONST               8 ('#5f5f5f')
                
-               120          40 LOAD_CONST               8 ('#5f5f5f')
+               125          42 LOAD_CONST               5 (1)
                
-               122          42 LOAD_CONST               6 ('#e2e2e2')
+               121          44 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+                            46 BUILD_CONST_KEY_MAP      4
                
-               123          44 LOAD_CONST               7 ('#f9f9f9')
+               129          48 LOAD_CONST               6 ('#f9f9f9')
                
-               124          46 LOAD_CONST               9 ('#8a8a8a')
+               130          50 LOAD_CONST              10 ('#e2e2e2')
                
-               109          48 LOAD_CONST              10 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+               131          52 LOAD_CONST              11 ('#8a8a8a')
                
-               108          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               132          54 LOAD_CONST               5 (1)
+               
+               128          56 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+                            58 BUILD_CONST_KEY_MAP      4
+               
+               115          60 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            62 BUILD_CONST_KEY_MAP      6
+               
+               114          64 BUILD_MAP                1
+               
+               113          66 PRECALL                  1
+                            70 CALL                     1
+                            80 POP_TOP
+                            82 LOAD_CONST               0 (None)
+                            84 RETURN_VALUE
                consts
                   None
-                  '#f3f3f3'
-                  1
-                  '#eaeaea'
+                  'button'
                   '#fdfdfd'
+                  '#eaeaea'
                   '#1a1a1a'
-                  '#e2e2e2'
+                  1
                   '#f9f9f9'
+                  '#aaaaaa'
                   '#5f5f5f'
+                  ('back', 'border', 'text_back', 'border_width')
+                  '#e2e2e2'
                   '#8a8a8a'
-                  ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  ('back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette_light'
-               firstlineno 107
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               firstlineno 112
+               lnotab
+                  0x020118020201020102010201020302010201020102fc04080201020102
+                  0102fc04f304ff02ff
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 14
+               stacksize : 13
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  02640364046405640364066407640364086409640a9c0ba6010000ab0100
-                  00000000000000010064005300
-               128           0 RESUME                   0
+                  02640364046405640664036407640564089c0464096403640a640564089c
+                  04640b9c066901a6010000ab010000000000000000010064005300
+               138           0 RESUME                   0
                
-               129           2 LOAD_FAST                0 (self)
+               139           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               131          26 LOAD_CONST               1 ('#202020')
+               141          26 LOAD_CONST               1 ('button')
+               
+               142          28 LOAD_CONST               2 ('#353535')
+               
+               143          30 LOAD_CONST               3 ('#454545')
+               
+               144          32 LOAD_CONST               4 ('#ffffff')
                
-               133          28 LOAD_CONST               2 (1)
+               145          34 LOAD_CONST               5 (1)
                
-               135          30 LOAD_CONST               3 ('#454545')
+               148          36 LOAD_CONST               6 ('#3a3a3a')
                
-               136          32 LOAD_CONST               4 ('#353535')
+               149          38 LOAD_CONST               3 ('#454545')
                
-               137          34 LOAD_CONST               5 ('#ffffff')
+               150          40 LOAD_CONST               7 ('#cecece')
                
-               139          36 LOAD_CONST               3 ('#454545')
+               151          42 LOAD_CONST               5 (1)
                
-               140          38 LOAD_CONST               6 ('#3a3a3a')
+               147          44 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+                            46 BUILD_CONST_KEY_MAP      4
                
-               141          40 LOAD_CONST               7 ('#cecece')
+               155          48 LOAD_CONST               9 ('#2f2f2f')
                
-               143          42 LOAD_CONST               3 ('#454545')
+               156          50 LOAD_CONST               3 ('#454545')
                
-               144          44 LOAD_CONST               8 ('#2f2f2f')
+               157          52 LOAD_CONST              10 ('#9a9a9a')
                
-               145          46 LOAD_CONST               9 ('#9a9a9a')
+               158          54 LOAD_CONST               5 (1)
                
-               130          48 LOAD_CONST              10 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+               154          56 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+                            58 BUILD_CONST_KEY_MAP      4
                
-               129          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               141          60 LOAD_CONST              11 (('back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            62 BUILD_CONST_KEY_MAP      6
+               
+               140          64 BUILD_MAP                1
+               
+               139          66 PRECALL                  1
+                            70 CALL                     1
+                            80 POP_TOP
+                            82 LOAD_CONST               0 (None)
+                            84 RETURN_VALUE
                consts
                   None
-                  '#202020'
-                  1
-                  '#454545'
+                  'button'
                   '#353535'
+                  '#454545'
                   '#ffffff'
+                  1
                   '#3a3a3a'
                   '#cecece'
+                  ('back', 'border', 'text_back', 'border_width')
                   '#2f2f2f'
                   '#9a9a9a'
-                  ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  ('back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette_dark'
-               firstlineno 128
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               firstlineno 138
+               lnotab
+                  0x020118020201020102010201020302010201020102fc04080201020102
+                  0102fc04f304ff02ff
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 12
+               stacksize : 4
                flags     : 3
                code
-                  0x97007c0181b87c016401190000000000000000007c005f000000000000
-                  0000007c016402190000000000000000007c005f0100000000000000007c
-                  016403190000000000000000007c005f0200000000000000007c01640419
-                  0000000000000000007c005f0300000000000000007c0164051900000000
-                  00000000007c005f0400000000000000007c016406190000000000000000
-                  007c005f0500000000000000007c016407190000000000000000007c005f
-                  0600000000000000007c016408190000000000000000007c005f07000000
-                  00000000007c016409190000000000000000007c005f0800000000000000
-                  007c01640a190000000000000000007c005f0900000000000000007c0164
-                  0b190000000000000000007c005f0a000000000000000009007c00a00b00
-                  000000000000000000000000000000000000006400a6010000ab01000000
-                  000000000001006400530023007418000000000000000000002400720401
-                  0059006400530077007803590077017c006a0000000000000000007c006a
-                  0100000000000000007c006a0200000000000000007c006a030000000000
-                  0000007c006a0400000000000000007c006a0500000000000000007c006a
-                  0600000000000000007c006a0700000000000000007c006a080000000000
-                  0000007c006a0900000000000000007c006a0a0000000000000000640c9c
-                  0b5300
-               149           0 RESUME                   0
-               
-               150           2 LOAD_FAST                1 (dict)
-                             4 POP_JUMP_FORWARD_IF_NONE   184 (to 374)
-               
-               151           6 LOAD_FAST                1 (dict)
-                             8 LOAD_CONST               1 ('button_frame_back')
-                            10 BINARY_SUBSCR
-                            20 LOAD_FAST                0 (self)
-                            22 STORE_ATTR               0 (button_frame_back)
-               
-               152          32 LOAD_FAST                1 (dict)
-                            34 LOAD_CONST               2 ('button_border_width')
-                            36 BINARY_SUBSCR
-                            46 LOAD_FAST                0 (self)
-                            48 STORE_ATTR               1 (button_border_width)
-               
-               154          58 LOAD_FAST                1 (dict)
-                            60 LOAD_CONST               3 ('button_border')
-                            62 BINARY_SUBSCR
-                            72 LOAD_FAST                0 (self)
-                            74 STORE_ATTR               2 (button_border)
-               
-               155          84 LOAD_FAST                1 (dict)
-                            86 LOAD_CONST               4 ('button_back')
-                            88 BINARY_SUBSCR
-                            98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               3 (button_back)
-               
-               156         110 LOAD_FAST                1 (dict)
-                           112 LOAD_CONST               5 ('button_text_back')
-                           114 BINARY_SUBSCR
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               4 (button_text_back)
-               
-               158         136 LOAD_FAST                1 (dict)
-                           138 LOAD_CONST               6 ('button_active_border')
-                           140 BINARY_SUBSCR
-                           150 LOAD_FAST                0 (self)
-                           152 STORE_ATTR               5 (button_active_border)
-               
-               159         162 LOAD_FAST                1 (dict)
-                           164 LOAD_CONST               7 ('button_active_back')
-                           166 BINARY_SUBSCR
-                           176 LOAD_FAST                0 (self)
-                           178 STORE_ATTR               6 (button_active_back)
-               
-               160         188 LOAD_FAST                1 (dict)
-                           190 LOAD_CONST               8 ('button_active_text_back')
-                           192 BINARY_SUBSCR
-                           202 LOAD_FAST                0 (self)
-                           204 STORE_ATTR               7 (button_active_text_back)
+                  0x97007c019001815d64017c017600900172287c01640119000000000000
+                  0000006402190000000000000000007c005f0000000000000000007c0164
+                  01190000000000000000006403190000000000000000007c005f01000000
+                  00000000007c016401190000000000000000006404190000000000000000
+                  007c005f0200000000000000007c01640119000000000000000000640519
+                  0000000000000000007c005f03000000000000000064067c016401190000
+                  00000000000000760072647c016401190000000000000000006406190000
+                  000000000000006402190000000000000000007c005f0400000000000000
+                  007c01640119000000000000000000640619000000000000000000640319
+                  0000000000000000007c005f0500000000000000007c0164011900000000
+                  00000000006406190000000000000000006404190000000000000000007c
+                  005f0600000000000000007c016401190000000000000000006406190000
+                  000000000000006405190000000000000000007c005f0700000000000000
+                  0064077c01640119000000000000000000760072647c0164011900000000
+                  00000000006407190000000000000000006402190000000000000000007c
+                  005f0800000000000000007c016401190000000000000000006407190000
+                  000000000000006403190000000000000000007c005f0900000000000000
+                  007c01640119000000000000000000640719000000000000000000640419
+                  0000000000000000007c005f0a00000000000000007c0164011900000000
+                  00000000006407190000000000000000006405190000000000000000007c
+                  005f0b00000000000000007c017c005f0c000000000000000009007c00a0
+                  0d00000000000000000000000000000000000000006400a6010000ab0100
+                  000000000000000100640053002300741c00000000000000000000240072
+                  04010059006400530077007803590077017c006a0c000000000000000053
+                  00
+               164           0 RESUME                   0
                
-               162         214 LOAD_FAST                1 (dict)
-                           216 LOAD_CONST               9 ('button_pressed_border')
+               165           2 LOAD_FAST                1 (dict)
+                             4 EXTENDED_ARG             1
+                             6 POP_JUMP_FORWARD_IF_NONE   349 (to 706)
+               
+               166           8 LOAD_CONST               1 ('button')
+                            10 LOAD_FAST                1 (dict)
+                            12 CONTAINS_OP              0
+                            14 EXTENDED_ARG             1
+                            16 POP_JUMP_FORWARD_IF_FALSE   296 (to 610)
+               
+               167          18 LOAD_FAST                1 (dict)
+                            20 LOAD_CONST               1 ('button')
+                            22 BINARY_SUBSCR
+                            32 LOAD_CONST               2 ('back')
+                            34 BINARY_SUBSCR
+                            44 LOAD_FAST                0 (self)
+                            46 STORE_ATTR               0 (button_back)
+               
+               168          56 LOAD_FAST                1 (dict)
+                            58 LOAD_CONST               1 ('button')
+                            60 BINARY_SUBSCR
+                            70 LOAD_CONST               3 ('border')
+                            72 BINARY_SUBSCR
+                            82 LOAD_FAST                0 (self)
+                            84 STORE_ATTR               1 (button_border)
+               
+               169          94 LOAD_FAST                1 (dict)
+                            96 LOAD_CONST               1 ('button')
+                            98 BINARY_SUBSCR
+                           108 LOAD_CONST               4 ('text_back')
+                           110 BINARY_SUBSCR
+                           120 LOAD_FAST                0 (self)
+                           122 STORE_ATTR               2 (button_text_back)
+               
+               170         132 LOAD_FAST                1 (dict)
+                           134 LOAD_CONST               1 ('button')
+                           136 BINARY_SUBSCR
+                           146 LOAD_CONST               5 ('border_width')
+                           148 BINARY_SUBSCR
+                           158 LOAD_FAST                0 (self)
+                           160 STORE_ATTR               3 (button_border_width)
+               
+               172         170 LOAD_CONST               6 ('active')
+                           172 LOAD_FAST                1 (dict)
+                           174 LOAD_CONST               1 ('button')
+                           176 BINARY_SUBSCR
+                           186 CONTAINS_OP              0
+                           188 POP_JUMP_FORWARD_IF_FALSE   100 (to 390)
+               
+               173         190 LOAD_FAST                1 (dict)
+                           192 LOAD_CONST               1 ('button')
+                           194 BINARY_SUBSCR
+                           204 LOAD_CONST               6 ('active')
+                           206 BINARY_SUBSCR
+                           216 LOAD_CONST               2 ('back')
                            218 BINARY_SUBSCR
                            228 LOAD_FAST                0 (self)
-                           230 STORE_ATTR               8 (button_pressed_border)
+                           230 STORE_ATTR               4 (button_active_back)
                
-               163         240 LOAD_FAST                1 (dict)
-                           242 LOAD_CONST              10 ('button_pressed_back')
+               174         240 LOAD_FAST                1 (dict)
+                           242 LOAD_CONST               1 ('button')
                            244 BINARY_SUBSCR
-                           254 LOAD_FAST                0 (self)
-                           256 STORE_ATTR               9 (button_pressed_back)
-               
-               164         266 LOAD_FAST                1 (dict)
-                           268 LOAD_CONST              11 ('button_pressed_text_back')
-                           270 BINARY_SUBSCR
-                           280 LOAD_FAST                0 (self)
-                           282 STORE_ATTR              10 (button_pressed_text_back)
-               
-               166         292 NOP
-               
-               167         294 LOAD_FAST                0 (self)
-                           296 LOAD_METHOD             11 (_draw)
-                           318 LOAD_CONST               0 (None)
-                           320 PRECALL                  1
-                           324 CALL                     1
-                           334 POP_TOP
-                           336 LOAD_CONST               0 (None)
-                           338 RETURN_VALUE
-                       >>  340 PUSH_EXC_INFO
-               
-               168         342 LOAD_GLOBAL             24 (AttributeError)
-                           354 CHECK_EXC_MATCH
-                           356 POP_JUMP_FORWARD_IF_FALSE     4 (to 366)
-                           358 POP_TOP
-               
-               169         360 POP_EXCEPT
-                           362 LOAD_CONST               0 (None)
-                           364 RETURN_VALUE
-               
-               168     >>  366 RERAISE                  0
-                       >>  368 COPY                     3
-                           370 POP_EXCEPT
-                           372 RERAISE                  1
-               
-               172     >>  374 LOAD_FAST                0 (self)
-                           376 LOAD_ATTR                0 (button_frame_back)
-               
-               173         386 LOAD_FAST                0 (self)
-                           388 LOAD_ATTR                1 (button_border_width)
-               
-               175         398 LOAD_FAST                0 (self)
-                           400 LOAD_ATTR                2 (button_border)
-               
-               176         410 LOAD_FAST                0 (self)
-                           412 LOAD_ATTR                3 (button_back)
-               
-               177         422 LOAD_FAST                0 (self)
-                           424 LOAD_ATTR                4 (button_text_back)
-               
-               179         434 LOAD_FAST                0 (self)
-                           436 LOAD_ATTR                5 (button_active_border)
-               
-               180         446 LOAD_FAST                0 (self)
-                           448 LOAD_ATTR                6 (button_active_back)
-               
-               181         458 LOAD_FAST                0 (self)
-                           460 LOAD_ATTR                7 (button_active_text_back)
-               
-               183         470 LOAD_FAST                0 (self)
-                           472 LOAD_ATTR                8 (button_pressed_border)
-               
-               184         482 LOAD_FAST                0 (self)
-                           484 LOAD_ATTR                9 (button_pressed_back)
-               
-               185         494 LOAD_FAST                0 (self)
-                           496 LOAD_ATTR               10 (button_pressed_text_back)
-               
-               171         506 LOAD_CONST              12 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                           508 BUILD_CONST_KEY_MAP     11
-                           510 RETURN_VALUE
+                           254 LOAD_CONST               6 ('active')
+                           256 BINARY_SUBSCR
+                           266 LOAD_CONST               3 ('border')
+                           268 BINARY_SUBSCR
+                           278 LOAD_FAST                0 (self)
+                           280 STORE_ATTR               5 (button_active_border)
+               
+               175         290 LOAD_FAST                1 (dict)
+                           292 LOAD_CONST               1 ('button')
+                           294 BINARY_SUBSCR
+                           304 LOAD_CONST               6 ('active')
+                           306 BINARY_SUBSCR
+                           316 LOAD_CONST               4 ('text_back')
+                           318 BINARY_SUBSCR
+                           328 LOAD_FAST                0 (self)
+                           330 STORE_ATTR               6 (button_active_text_back)
+               
+               176         340 LOAD_FAST                1 (dict)
+                           342 LOAD_CONST               1 ('button')
+                           344 BINARY_SUBSCR
+                           354 LOAD_CONST               6 ('active')
+                           356 BINARY_SUBSCR
+                           366 LOAD_CONST               5 ('border_width')
+                           368 BINARY_SUBSCR
+                           378 LOAD_FAST                0 (self)
+                           380 STORE_ATTR               7 (button_active_border_width)
+               
+               178     >>  390 LOAD_CONST               7 ('pressed')
+                           392 LOAD_FAST                1 (dict)
+                           394 LOAD_CONST               1 ('button')
+                           396 BINARY_SUBSCR
+                           406 CONTAINS_OP              0
+                           408 POP_JUMP_FORWARD_IF_FALSE   100 (to 610)
+               
+               179         410 LOAD_FAST                1 (dict)
+                           412 LOAD_CONST               1 ('button')
+                           414 BINARY_SUBSCR
+                           424 LOAD_CONST               7 ('pressed')
+                           426 BINARY_SUBSCR
+                           436 LOAD_CONST               2 ('back')
+                           438 BINARY_SUBSCR
+                           448 LOAD_FAST                0 (self)
+                           450 STORE_ATTR               8 (button_pressed_back)
+               
+               180         460 LOAD_FAST                1 (dict)
+                           462 LOAD_CONST               1 ('button')
+                           464 BINARY_SUBSCR
+                           474 LOAD_CONST               7 ('pressed')
+                           476 BINARY_SUBSCR
+                           486 LOAD_CONST               3 ('border')
+                           488 BINARY_SUBSCR
+                           498 LOAD_FAST                0 (self)
+                           500 STORE_ATTR               9 (button_pressed_border)
+               
+               181         510 LOAD_FAST                1 (dict)
+                           512 LOAD_CONST               1 ('button')
+                           514 BINARY_SUBSCR
+                           524 LOAD_CONST               7 ('pressed')
+                           526 BINARY_SUBSCR
+                           536 LOAD_CONST               4 ('text_back')
+                           538 BINARY_SUBSCR
+                           548 LOAD_FAST                0 (self)
+                           550 STORE_ATTR              10 (button_pressed_text_back)
+               
+               182         560 LOAD_FAST                1 (dict)
+                           562 LOAD_CONST               1 ('button')
+                           564 BINARY_SUBSCR
+                           574 LOAD_CONST               7 ('pressed')
+                           576 BINARY_SUBSCR
+                           586 LOAD_CONST               5 ('border_width')
+                           588 BINARY_SUBSCR
+                           598 LOAD_FAST                0 (self)
+                           600 STORE_ATTR              11 (button_pressed_border_width)
+               
+               184     >>  610 LOAD_FAST                1 (dict)
+                           612 LOAD_FAST                0 (self)
+                           614 STORE_ATTR              12 (_palette)
+               
+               186         624 NOP
+               
+               187         626 LOAD_FAST                0 (self)
+                           628 LOAD_METHOD             13 (_draw)
+                           650 LOAD_CONST               0 (None)
+                           652 PRECALL                  1
+                           656 CALL                     1
+                           666 POP_TOP
+                           668 LOAD_CONST               0 (None)
+                           670 RETURN_VALUE
+                       >>  672 PUSH_EXC_INFO
+               
+               188         674 LOAD_GLOBAL             28 (AttributeError)
+                           686 CHECK_EXC_MATCH
+                           688 POP_JUMP_FORWARD_IF_FALSE     4 (to 698)
+                           690 POP_TOP
+               
+               189         692 POP_EXCEPT
+                           694 LOAD_CONST               0 (None)
+                           696 RETURN_VALUE
+               
+               188     >>  698 RERAISE                  0
+                       >>  700 COPY                     3
+                           702 POP_EXCEPT
+                           704 RERAISE                  1
+               
+               191     >>  706 LOAD_FAST                0 (self)
+                           708 LOAD_ATTR               12 (_palette)
+                           718 RETURN_VALUE
                ExceptionTable:
-                 294 to 334 -> 340 [0]
-                 340 to 358 -> 368 [1] lasti
-                 366 to 366 -> 368 [1] lasti
+                 626 to 666 -> 672 [0]
+                 672 to 690 -> 700 [1] lasti
+                 698 to 698 -> 700 [1] lasti
                consts
                   None
-                  'button_frame_back'
-                  'button_border_width'
-                  'button_border'
-                  'button_back'
-                  'button_text_back'
-                  'button_active_border'
-                  'button_active_back'
-                  'button_active_text_back'
-                  'button_pressed_border'
-                  'button_pressed_back'
-                  'button_pressed_text_back'
-                  ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
-               names      ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back', '_draw', 'AttributeError')
+                  'button'
+                  'back'
+                  'border'
+                  'text_back'
+                  'border_width'
+                  'active'
+                  'pressed'
+               names      ('button_back', 'button_border', 'button_text_back', 'button_border_width', 'button_active_back', 'button_active_border', 'button_active_text_back', 'button_active_border_width', 'button_pressed_back', 'button_pressed_border', 'button_pressed_text_back', 'button_pressed_border_width', '_palette', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette'
-               firstlineno 149
+               firstlineno 164
                lnotab
-                  0x020104011a011a021a011a011a021a011a011a021a011a011a02020130
-                  01120106ff08040c010c020c010c010c020c010c010c020c010c010cf2
+                  0x020106010a012601260126012602140132013201320132021401320132
+                  01320132020e0202013001120106ff0803
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'configure', '_other', '_draw', '_click', '_unclick', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawBasicButton'
          firstlineno 6
-         lnotab 0x0c011c1a0a0a0604060f080a080a080808080e06060306150615
+         lnotab 0x0c011c1b0a0a0604060f080b080b080908090e060603061a061a
       'AdwDrawBasicButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         189           0 RESUME                   0
+         194           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         190          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 190>)
+         195          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 195>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               190           0 RESUME                   0
+               195           0 RESUME                   0
                
-               191           2 LOAD_FAST                0 (self)
+               196           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 190
+               firstlineno 195
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawButton'
-         firstlineno 189
+         firstlineno 194
          lnotab 0x0a01
       'AdwDrawButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         194           0 RESUME                   0
+         199           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         195          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 195>)
+         200          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 200>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               195           0 RESUME                   0
+               200           0 RESUME                   0
                
-               196           2 LOAD_FAST                0 (self)
+               201           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 195
+               firstlineno 200
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawDarkButton'
-         firstlineno 194
+         firstlineno 199
          lnotab 0x0a01
       'AdwDrawDarkButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         199           0 RESUME                   0
+         204           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawAccentButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         200          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 200>)
+         205          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 205>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawAccentButton'
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 14
+               stacksize : 13
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036401640464036405640464066406640764089c0ba6010000ab0100
-                  00000000000000010064005300
-               200           0 RESUME                   0
+                  02640364046405640664036404640564079c04640864086409640564079c
+                  04640a9c066901a6010000ab010000000000000000010064005300
+               205           0 RESUME                   0
                
-               201           2 LOAD_FAST                0 (self)
+               206           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               203          26 LOAD_CONST               1 ('#0067c0')
+               208          26 LOAD_CONST               1 ('button')
+               
+               209          28 LOAD_CONST               2 ('#0067c0')
+               
+               210          30 LOAD_CONST               3 ('#1473c5')
+               
+               211          32 LOAD_CONST               4 ('#ffffff')
+               
+               212          34 LOAD_CONST               5 (1)
+               
+               215          36 LOAD_CONST               6 ('#1975c5')
                
-               205          28 LOAD_CONST               2 (1)
+               216          38 LOAD_CONST               3 ('#1473c5')
                
-               207          30 LOAD_CONST               3 ('#1473c5')
+               217          40 LOAD_CONST               4 ('#ffffff')
                
-               208          32 LOAD_CONST               1 ('#0067c0')
+               218          42 LOAD_CONST               5 (1)
                
-               209          34 LOAD_CONST               4 ('#ffffff')
+               214          44 LOAD_CONST               7 (('back', 'border', 'text_back', 'border_width'))
+                            46 BUILD_CONST_KEY_MAP      4
                
-               211          36 LOAD_CONST               3 ('#1473c5')
+               222          48 LOAD_CONST               8 ('#3284cb')
                
-               212          38 LOAD_CONST               5 ('#1975c5')
+               223          50 LOAD_CONST               8 ('#3284cb')
                
-               213          40 LOAD_CONST               4 ('#ffffff')
+               224          52 LOAD_CONST               9 ('#fdfdfd')
                
-               215          42 LOAD_CONST               6 ('#3284cb')
+               225          54 LOAD_CONST               5 (1)
                
-               216          44 LOAD_CONST               6 ('#3284cb')
+               221          56 LOAD_CONST               7 (('back', 'border', 'text_back', 'border_width'))
+                            58 BUILD_CONST_KEY_MAP      4
                
-               217          46 LOAD_CONST               7 ('#fdfdfd')
+               208          60 LOAD_CONST              10 (('back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            62 BUILD_CONST_KEY_MAP      6
                
-               202          48 LOAD_CONST               8 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+               207          64 BUILD_MAP                1
                
-               201          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               206          66 PRECALL                  1
+                            70 CALL                     1
+                            80 POP_TOP
+                            82 LOAD_CONST               0 (None)
+                            84 RETURN_VALUE
                consts
                   None
+                  'button'
                   '#0067c0'
-                  1
                   '#1473c5'
                   '#ffffff'
+                  1
                   '#1975c5'
+                  ('back', 'border', 'text_back', 'border_width')
                   '#3284cb'
                   '#fdfdfd'
-                  ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  ('back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 200
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               firstlineno 205
+               lnotab
+                  0x020118020201020102010201020302010201020102fc04080201020102
+                  0102fc04f304ff02ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawAccentButton'
-         firstlineno 199
+         firstlineno 204
          lnotab 0x0a01
       'AdwDrawAccentButton'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 4
+         stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
-            0b6404650565067a0700006602640584055a07640684005a08640784005a
-            09640884005a0a640984005a0b640b640a84015a0c880078015a0d5300
+            0384005a05640484005a06640584005a07640684005a0864098800660164
+            0884095a09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
-         223           2 RESUME                   0
+         233           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundButton')
                       10 STORE_NAME               2 (__qualname__)
          
-         224          12 LOAD_CLOSURE             0 (__class__)
+         234          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\button.py", line 224>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\button.py", line 234>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         227          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\button.py", line 227>)
+         237          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\button.py", line 237>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         230          28 LOAD_CONST              11 ((None,))
-                      30 LOAD_CONST               4 ('radius')
-                      32 LOAD_NAME                5 (float)
-                      34 LOAD_NAME                6 (int)
-                      36 BINARY_OP                7 (|)
-                      40 BUILD_TUPLE              2
-                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\button.py", line 230>)
-                      44 MAKE_FUNCTION            5 (defaults, annotations)
-                      46 STORE_NAME               7 (border_radius)
-         
-         236          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 236>)
-                      50 MAKE_FUNCTION            0
-                      52 STORE_NAME               8 (_draw)
-         
-         251          54 LOAD_CONST               7 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 251>)
-                      56 MAKE_FUNCTION            0
-                      58 STORE_NAME               9 (default_palette)
-         
-         254          60 LOAD_CONST               8 (<code object palette_light, file "D:\tkadw\tkadw\canvas\button.py", line 254>)
-                      62 MAKE_FUNCTION            0
-                      64 STORE_NAME              10 (palette_light)
-         
-         275          66 LOAD_CONST               9 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\button.py", line 275>)
-                      68 MAKE_FUNCTION            0
-                      70 STORE_NAME              11 (palette_dark)
-         
-         296          72 LOAD_CONST              11 ((None,))
-                      74 LOAD_CONST              10 (<code object palette, file "D:\tkadw\tkadw\canvas\button.py", line 296>)
-                      76 MAKE_FUNCTION            1 (defaults)
-                      78 STORE_NAME              12 (palette)
-                      80 LOAD_CLOSURE             0 (__class__)
-                      82 COPY                     1
-                      84 STORE_NAME              13 (__classcell__)
-                      86 RETURN_VALUE
+         240          28 LOAD_CONST               3 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 240>)
+                      30 MAKE_FUNCTION            0
+                      32 STORE_NAME               5 (_draw)
+         
+         255          34 LOAD_CONST               4 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 255>)
+                      36 MAKE_FUNCTION            0
+                      38 STORE_NAME               6 (default_palette)
+         
+         258          40 LOAD_CONST               5 (<code object palette_light, file "D:\tkadw\tkadw\canvas\button.py", line 258>)
+                      42 MAKE_FUNCTION            0
+                      44 STORE_NAME               7 (palette_light)
+         
+         285          46 LOAD_CONST               6 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\button.py", line 285>)
+                      48 MAKE_FUNCTION            0
+                      50 STORE_NAME               8 (palette_dark)
+         
+         312          52 LOAD_CONST               9 ((None,))
+                      54 LOAD_CLOSURE             0 (__class__)
+                      56 BUILD_TUPLE              1
+                      58 LOAD_CONST               8 (<code object palette, file "D:\tkadw\tkadw\canvas\button.py", line 312>)
+                      60 MAKE_FUNCTION            9 (defaults, closure)
+                      62 STORE_NAME               9 (palette)
+                      64 LOAD_CLOSURE             0 (__class__)
+                      66 COPY                     1
+                      68 STORE_NAME              10 (__classcell__)
+                      70 RETURN_VALUE
          consts
             'AdwDrawBasicRoundButton'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               224           2 RESUME                   0
+               234           2 RESUME                   0
                
-               225           4 PUSH_NULL
+               235           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -1897,29 +2004,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '__init__'
-               firstlineno 224
+               firstlineno 234
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               227           0 RESUME                   0
+               237           0 RESUME                   0
                
-               228           2 LOAD_FAST                0 (self)
+               238           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -1937,50 +2044,16 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_other'
-               firstlineno 227
+               firstlineno 237
                lnotab 0x0201
-            None
-            'radius'
-            code
-               argcount  : 2
-               nlocals   : 2
-               stacksize : 2
-               flags     : 3
-               code
-                  0x97007c0180077c006a00000000000000000053007c017c005f00000000
-                  000000000064005300
-               230           0 RESUME                   0
-               
-               231           2 LOAD_FAST                1 (radius)
-                             4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
-               
-               232           6 LOAD_FAST                0 (self)
-                             8 LOAD_ATTR                0 (button_radius)
-                            18 RETURN_VALUE
-               
-               234     >>   20 LOAD_FAST                1 (radius)
-                            22 LOAD_FAST                0 (self)
-                            24 STORE_ATTR               0 (button_radius)
-                            34 LOAD_CONST               0 (None)
-                            36 RETURN_VALUE
-               consts
-                  None
-               names      ('button_radius',)
-               varnames   ('self', 'radius')
-               freevars   ()
-               cellvars   ()
-               filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
-               name       'border_radius'
-               firstlineno 230
-               lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000006401a6
@@ -1993,27 +2066,27 @@
                   04a6080000ab0800000000000000007c005f0800000000000000007c00a0
                   0900000000000000000000000000000000000000007c00a0020000000000
                   000000000000000000000000000000a6000000ab00000000000000000064
                   027a0b00007c00a0030000000000000000000000000000000000000000a6
                   000000ab00000000000000000064027a0b00007c006a0a00000000000000
                   007c006a0b00000000000000007c006a0c0000000000000000ac05a60500
                   00ab0500000000000000007c005f0d000000000000000064005300
-               236           0 RESUME                   0
+               240           0 RESUME                   0
                
-               237           2 LOAD_FAST                0 (self)
+               241           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               239          44 LOAD_FAST                0 (self)
+               243          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect2)
                
-               240          68 LOAD_CONST               2 (2)
+               244          68 LOAD_CONST               2 (2)
                             70 LOAD_CONST               2 (2)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
@@ -2022,645 +2095,569 @@
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                            160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (button_radius)
                
-               241         172 LOAD_FAST                0 (self)
-                           174 LOAD_ATTR                5 (button_border_width)
+               245         172 LOAD_FAST                0 (self)
+                           174 LOAD_ATTR                5 (_button_border_width)
                
-               242         184 LOAD_FAST                0 (self)
+               246         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_button_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_button_back)
                
-               239         208 KW_NAMES                 4
+               243         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 LOAD_FAST                0 (self)
                            226 STORE_ATTR               8 (button_frame)
                
-               245         236 LOAD_FAST                0 (self)
+               249         236 LOAD_FAST                0 (self)
                            238 LOAD_METHOD              9 (create_text)
                
-               246         260 LOAD_FAST                0 (self)
+               250         260 LOAD_FAST                0 (self)
                            262 LOAD_METHOD              2 (winfo_width)
                            284 PRECALL                  0
                            288 CALL                     0
                            298 LOAD_CONST               2 (2)
                            300 BINARY_OP               11 (/)
                            304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              3 (winfo_height)
                            328 PRECALL                  0
                            332 CALL                     0
                            342 LOAD_CONST               2 (2)
                            344 BINARY_OP               11 (/)
                
-               247         348 LOAD_FAST                0 (self)
+               251         348 LOAD_FAST                0 (self)
                            350 LOAD_ATTR               10 (text)
                            360 LOAD_FAST                0 (self)
                            362 LOAD_ATTR               11 (_button_text_back)
                
-               248         372 LOAD_FAST                0 (self)
+               252         372 LOAD_FAST                0 (self)
                            374 LOAD_ATTR               12 (button_text_font)
                
-               245         384 KW_NAMES                 5
+               249         384 KW_NAMES                 5
                            386 PRECALL                  5
                            390 CALL                     5
                            400 LOAD_FAST                0 (self)
                            402 STORE_ATTR              13 (button_text)
                            412 LOAD_CONST               0 (None)
                            414 RETURN_VALUE
                consts
                   None
                   'all'
                   2
                   3
                   ('width', 'outline', 'fill')
                   ('text', 'fill', 'font')
-               names      ('delete', 'create_round_rect2', 'winfo_width', 'winfo_height', 'button_radius', 'button_border_width', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
+               names      ('delete', 'create_round_rect2', 'winfo_width', 'winfo_height', 'button_radius', '_button_border_width', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_draw'
-               firstlineno 236
+               firstlineno 240
                lnotab 0x02012a02180168010c0118fd1c061801580118010cfd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               251           0 RESUME                   0
+               255           0 RESUME                   0
                
-               252           2 LOAD_FAST                0 (self)
+               256           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 251
+               firstlineno 255
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  02640364046405640664076408640664076409640a9c0ba6010000ab0100
-                  00000000000000010064005300
-               254           0 RESUME                   0
+                  0264036404640564066407640864096406640a9c046407640b640c640664
+                  0a9c04640d9c076901a6010000ab010000000000000000010064005300
+               258           0 RESUME                   0
                
-               255           2 LOAD_FAST                0 (self)
+               259           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               257          26 LOAD_CONST               1 (8)
+               261          26 LOAD_CONST               1 ('button')
                
-               259          28 LOAD_CONST               2 (1)
+               262          28 LOAD_CONST               2 (8)
                
-               261          30 LOAD_CONST               3 ('#eaeaea')
+               263          30 LOAD_CONST               3 ('#fdfdfd')
                
-               262          32 LOAD_CONST               4 ('#fdfdfd')
+               264          32 LOAD_CONST               4 ('#eaeaea')
                
-               263          34 LOAD_CONST               5 ('#1a1a1a')
+               265          34 LOAD_CONST               5 ('#1a1a1a')
                
-               265          36 LOAD_CONST               6 ('#e2e2e2')
+               266          36 LOAD_CONST               6 (1)
                
-               266          38 LOAD_CONST               7 ('#f9f9f9')
+               269          38 LOAD_CONST               7 ('#f9f9f9')
                
-               267          40 LOAD_CONST               8 ('#5f5f5f')
+               270          40 LOAD_CONST               8 ('#454545')
                
-               269          42 LOAD_CONST               6 ('#e2e2e2')
+               271          42 LOAD_CONST               9 ('#5f5f5f')
                
-               270          44 LOAD_CONST               7 ('#f9f9f9')
+               272          44 LOAD_CONST               6 (1)
                
-               271          46 LOAD_CONST               9 ('#8a8a8a')
+               268          46 LOAD_CONST              10 (('back', 'border', 'text_back', 'border_width'))
+                            48 BUILD_CONST_KEY_MAP      4
                
-               256          48 LOAD_CONST              10 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+               276          50 LOAD_CONST               7 ('#f9f9f9')
                
-               255          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               277          52 LOAD_CONST              11 ('#e2e2e2')
+               
+               278          54 LOAD_CONST              12 ('#8a8a8a')
+               
+               279          56 LOAD_CONST               6 (1)
+               
+               275          58 LOAD_CONST              10 (('back', 'border', 'text_back', 'border_width'))
+                            60 BUILD_CONST_KEY_MAP      4
+               
+               261          62 LOAD_CONST              13 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            64 BUILD_CONST_KEY_MAP      7
+               
+               260          66 BUILD_MAP                1
+               
+               259          68 PRECALL                  1
+                            72 CALL                     1
+                            82 POP_TOP
+                            84 LOAD_CONST               0 (None)
+                            86 RETURN_VALUE
                consts
                   None
+                  'button'
                   8
-                  1
-                  '#eaeaea'
                   '#fdfdfd'
+                  '#eaeaea'
                   '#1a1a1a'
-                  '#e2e2e2'
+                  1
                   '#f9f9f9'
+                  '#454545'
                   '#5f5f5f'
+                  ('back', 'border', 'text_back', 'border_width')
+                  '#e2e2e2'
                   '#8a8a8a'
-                  ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette_light'
-               firstlineno 254
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               firstlineno 258
+               lnotab
+                  0x0201180202010201020102010201020302010201020102fc0408020102
+                  01020102fc04f204ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  02640364046405640364066407640364086409640a9c0ba6010000ab0100
-                  00000000000000010064005300
-               275           0 RESUME                   0
+                  026403640464056406640764046408640664099c04640a6404640b640664
+                  099c04640c9c076901a6010000ab010000000000000000010064005300
+               285           0 RESUME                   0
                
-               276           2 LOAD_FAST                0 (self)
+               286           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               278          26 LOAD_CONST               1 (8)
+               288          26 LOAD_CONST               1 ('button')
+               
+               289          28 LOAD_CONST               2 (8)
                
-               280          28 LOAD_CONST               2 (1)
+               290          30 LOAD_CONST               3 ('#353535')
                
-               282          30 LOAD_CONST               3 ('#454545')
+               291          32 LOAD_CONST               4 ('#454545')
                
-               283          32 LOAD_CONST               4 ('#353535')
+               292          34 LOAD_CONST               5 ('#ffffff')
                
-               284          34 LOAD_CONST               5 ('#ffffff')
+               293          36 LOAD_CONST               6 (1)
                
-               286          36 LOAD_CONST               3 ('#454545')
+               296          38 LOAD_CONST               7 ('#3a3a3a')
                
-               287          38 LOAD_CONST               6 ('#3a3a3a')
+               297          40 LOAD_CONST               4 ('#454545')
                
-               288          40 LOAD_CONST               7 ('#cecece')
+               298          42 LOAD_CONST               8 ('#cecece')
                
-               290          42 LOAD_CONST               3 ('#454545')
+               299          44 LOAD_CONST               6 (1)
                
-               291          44 LOAD_CONST               8 ('#2f2f2f')
+               295          46 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+                            48 BUILD_CONST_KEY_MAP      4
                
-               292          46 LOAD_CONST               9 ('#9a9a9a')
+               303          50 LOAD_CONST              10 ('#2f2f2f')
                
-               277          48 LOAD_CONST              10 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+               304          52 LOAD_CONST               4 ('#454545')
                
-               276          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               305          54 LOAD_CONST              11 ('#9a9a9a')
+               
+               306          56 LOAD_CONST               6 (1)
+               
+               302          58 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+                            60 BUILD_CONST_KEY_MAP      4
+               
+               288          62 LOAD_CONST              12 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            64 BUILD_CONST_KEY_MAP      7
+               
+               287          66 BUILD_MAP                1
+               
+               286          68 PRECALL                  1
+                            72 CALL                     1
+                            82 POP_TOP
+                            84 LOAD_CONST               0 (None)
+                            86 RETURN_VALUE
                consts
                   None
+                  'button'
                   8
-                  1
-                  '#454545'
                   '#353535'
+                  '#454545'
                   '#ffffff'
+                  1
                   '#3a3a3a'
                   '#cecece'
+                  ('back', 'border', 'text_back', 'border_width')
                   '#2f2f2f'
                   '#9a9a9a'
-                  ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette_dark'
-               firstlineno 275
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               firstlineno 285
+               lnotab
+                  0x0201180202010201020102010201020302010201020102fc0408020102
+                  01020102fc04f204ff02ff
+            None
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 12
+               stacksize : 3
                flags     : 3
                code
-                  0x97007c0181b87c016401190000000000000000007c005f000000000000
-                  0000007c016402190000000000000000007c005f0100000000000000007c
-                  016403190000000000000000007c005f0200000000000000007c01640419
-                  0000000000000000007c005f0300000000000000007c0164051900000000
-                  00000000007c005f0400000000000000007c016406190000000000000000
-                  007c005f0500000000000000007c016407190000000000000000007c005f
-                  0600000000000000007c016408190000000000000000007c005f07000000
-                  00000000007c016409190000000000000000007c005f0800000000000000
-                  007c01640a190000000000000000007c005f0900000000000000007c0164
-                  0b190000000000000000007c005f0a000000000000000009007c00a00b00
-                  000000000000000000000000000000000000006400a6010000ab01000000
-                  000000000001006400530023007418000000000000000000002400720401
-                  0059006400530077007803590077017c006a0d00000000000000007c006a
-                  0100000000000000007c006a0200000000000000007c006a030000000000
-                  0000007c006a0400000000000000007c006a0500000000000000007c006a
-                  0600000000000000007c006a0700000000000000007c006a080000000000
-                  0000007c006a0900000000000000007c006a0a0000000000000000640c9c
-                  0b5300
-               296           0 RESUME                   0
-               
-               297           2 LOAD_FAST                1 (dict)
-                             4 POP_JUMP_FORWARD_IF_NONE   184 (to 374)
-               
-               298           6 LOAD_FAST                1 (dict)
-                             8 LOAD_CONST               1 ('button_radius')
-                            10 BINARY_SUBSCR
-                            20 LOAD_FAST                0 (self)
-                            22 STORE_ATTR               0 (button_radius)
-               
-               300          32 LOAD_FAST                1 (dict)
-                            34 LOAD_CONST               2 ('button_border_width')
-                            36 BINARY_SUBSCR
-                            46 LOAD_FAST                0 (self)
-                            48 STORE_ATTR               1 (button_border_width)
-               
-               302          58 LOAD_FAST                1 (dict)
-                            60 LOAD_CONST               3 ('button_border')
-                            62 BINARY_SUBSCR
-                            72 LOAD_FAST                0 (self)
-                            74 STORE_ATTR               2 (button_border)
-               
-               303          84 LOAD_FAST                1 (dict)
-                            86 LOAD_CONST               4 ('button_back')
-                            88 BINARY_SUBSCR
-                            98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               3 (button_back)
-               
-               304         110 LOAD_FAST                1 (dict)
-                           112 LOAD_CONST               5 ('button_text_back')
-                           114 BINARY_SUBSCR
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               4 (button_text_back)
-               
-               306         136 LOAD_FAST                1 (dict)
-                           138 LOAD_CONST               6 ('button_active_border')
-                           140 BINARY_SUBSCR
-                           150 LOAD_FAST                0 (self)
-                           152 STORE_ATTR               5 (button_active_border)
-               
-               307         162 LOAD_FAST                1 (dict)
-                           164 LOAD_CONST               7 ('button_active_back')
-                           166 BINARY_SUBSCR
-                           176 LOAD_FAST                0 (self)
-                           178 STORE_ATTR               6 (button_active_back)
-               
-               308         188 LOAD_FAST                1 (dict)
-                           190 LOAD_CONST               8 ('button_active_text_back')
-                           192 BINARY_SUBSCR
-                           202 LOAD_FAST                0 (self)
-                           204 STORE_ATTR               7 (button_active_text_back)
-               
-               310         214 LOAD_FAST                1 (dict)
-                           216 LOAD_CONST               9 ('button_pressed_border')
-                           218 BINARY_SUBSCR
-                           228 LOAD_FAST                0 (self)
-                           230 STORE_ATTR               8 (button_pressed_border)
-               
-               311         240 LOAD_FAST                1 (dict)
-                           242 LOAD_CONST              10 ('button_pressed_back')
-                           244 BINARY_SUBSCR
-                           254 LOAD_FAST                0 (self)
-                           256 STORE_ATTR               9 (button_pressed_back)
-               
-               312         266 LOAD_FAST                1 (dict)
-                           268 LOAD_CONST              11 ('button_pressed_text_back')
-                           270 BINARY_SUBSCR
-                           280 LOAD_FAST                0 (self)
-                           282 STORE_ATTR              10 (button_pressed_text_back)
-               
-               314         292 NOP
-               
-               315         294 LOAD_FAST                0 (self)
-                           296 LOAD_METHOD             11 (_draw)
-                           318 LOAD_CONST               0 (None)
-                           320 PRECALL                  1
-                           324 CALL                     1
-                           334 POP_TOP
-                           336 LOAD_CONST               0 (None)
-                           338 RETURN_VALUE
-                       >>  340 PUSH_EXC_INFO
-               
-               316         342 LOAD_GLOBAL             24 (AttributeError)
-                           354 CHECK_EXC_MATCH
-                           356 POP_JUMP_FORWARD_IF_FALSE     4 (to 366)
-                           358 POP_TOP
-               
-               317         360 POP_EXCEPT
-                           362 LOAD_CONST               0 (None)
-                           364 RETURN_VALUE
-               
-               316     >>  366 RERAISE                  0
-                       >>  368 COPY                     3
-                           370 POP_EXCEPT
-                           372 RERAISE                  1
-               
-               320     >>  374 LOAD_FAST                0 (self)
-                           376 LOAD_ATTR               13 (button_frame_back)
-               
-               322         386 LOAD_FAST                0 (self)
-                           388 LOAD_ATTR                1 (button_border_width)
-               
-               324         398 LOAD_FAST                0 (self)
-                           400 LOAD_ATTR                2 (button_border)
-               
-               325         410 LOAD_FAST                0 (self)
-                           412 LOAD_ATTR                3 (button_back)
-               
-               326         422 LOAD_FAST                0 (self)
-                           424 LOAD_ATTR                4 (button_text_back)
-               
-               328         434 LOAD_FAST                0 (self)
-                           436 LOAD_ATTR                5 (button_active_border)
-               
-               329         446 LOAD_FAST                0 (self)
-                           448 LOAD_ATTR                6 (button_active_back)
-               
-               330         458 LOAD_FAST                0 (self)
-                           460 LOAD_ATTR                7 (button_active_text_back)
-               
-               332         470 LOAD_FAST                0 (self)
-                           472 LOAD_ATTR                8 (button_pressed_border)
+                  0x95019700740100000000000000000000a6000000ab0000000000000000
+                  00a00100000000000000000000000000000000000000007c01a6010000ab
+                  010000000000000000010064017c01760072157c01640119000000000000
+                  0000006402190000000000000000007c005f020000000000000000640053
+                  0064005300
+                             0 COPY_FREE_VARS           1
                
-               333         482 LOAD_FAST                0 (self)
-                           484 LOAD_ATTR                9 (button_pressed_back)
+               312           2 RESUME                   0
                
-               334         494 LOAD_FAST                0 (self)
-                           496 LOAD_ATTR               10 (button_pressed_text_back)
+               313           4 LOAD_GLOBAL              1 (NULL + super)
+                            16 PRECALL                  0
+                            20 CALL                     0
+                            30 LOAD_METHOD              1 (palette)
+                            52 LOAD_FAST                1 (dict)
+                            54 PRECALL                  1
+                            58 CALL                     1
+                            68 POP_TOP
+               
+               314          70 LOAD_CONST               1 ('button')
+                            72 LOAD_FAST                1 (dict)
+                            74 CONTAINS_OP              0
+                            76 POP_JUMP_FORWARD_IF_FALSE    21 (to 120)
+               
+               315          78 LOAD_FAST                1 (dict)
+                            80 LOAD_CONST               1 ('button')
+                            82 BINARY_SUBSCR
+                            92 LOAD_CONST               2 ('radius')
+                            94 BINARY_SUBSCR
+                           104 LOAD_FAST                0 (self)
+                           106 STORE_ATTR               2 (button_radius)
+                           116 LOAD_CONST               0 (None)
+                           118 RETURN_VALUE
                
-               319         506 LOAD_CONST              12 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                           508 BUILD_CONST_KEY_MAP     11
-                           510 RETURN_VALUE
-               ExceptionTable:
-                 294 to 334 -> 340 [0]
-                 340 to 358 -> 368 [1] lasti
-                 366 to 366 -> 368 [1] lasti
-               consts
-                  None
-                  'button_radius'
-                  'button_border_width'
-                  'button_border'
-                  'button_back'
-                  'button_text_back'
-                  'button_active_border'
-                  'button_active_back'
-                  'button_active_text_back'
-                  'button_pressed_border'
-                  'button_pressed_back'
-                  'button_pressed_text_back'
-                  ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
-               names      ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back', '_draw', 'AttributeError', 'button_frame_back')
+               314     >>  120 LOAD_CONST               0 (None)
+                           122 RETURN_VALUE
+               consts
+                  None
+                  'button'
+                  'radius'
+               names      ('super', 'palette', 'button_radius')
                varnames   ('self', 'dict')
-               freevars   ()
+               freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette'
-               firstlineno 296
-               lnotab
-                  0x020104011a021a021a011a011a021a011a011a021a011a011a02020130
-                  01120106ff08040c020c020c010c010c020c010c010c020c010c010cf1
+               firstlineno 312
+               lnotab 0x0401420108012aff
             (None,)
-         names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'float', 'int', 'border_radius', '_draw', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__init__', '_other', '_draw', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawBasicRoundButton'
-         firstlineno 223
-         lnotab 0x0c010a0306031406060f060306150615
+         firstlineno 233
+         lnotab 0x0c010a030603060f0603061b061b
       'AdwDrawBasicRoundButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         338           0 RESUME                   0
+         318           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         339          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 339>)
+         319          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 319>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               339           0 RESUME                   0
+               319           0 RESUME                   0
                
-               340           2 LOAD_FAST                0 (self)
+               320           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 339
+               firstlineno 319
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundButton'
-         firstlineno 338
+         firstlineno 318
          lnotab 0x0a01
       'AdwDrawRoundButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         343           0 RESUME                   0
+         323           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundAccentButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         344          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 344>)
+         324          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 324>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundAccentButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564036406640564076407640864099c0ba6010000ab0100
-                  00000000000000010064005300
-               344           0 RESUME                   0
+                  026403640464056406640764046405640664089c0464096409640a640664
+                  089c04640b9c076901a6010000ab010000000000000000010064005300
+               324           0 RESUME                   0
                
-               345           2 LOAD_FAST                0 (self)
+               325           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               347          26 LOAD_CONST               1 (8)
+               327          26 LOAD_CONST               1 ('button')
+               
+               328          28 LOAD_CONST               2 (8)
+               
+               329          30 LOAD_CONST               3 ('#0067c0')
+               
+               330          32 LOAD_CONST               4 ('#1473c5')
+               
+               331          34 LOAD_CONST               5 ('#ffffff')
+               
+               332          36 LOAD_CONST               6 (1)
                
-               349          28 LOAD_CONST               2 (1)
+               335          38 LOAD_CONST               7 ('#1975c5')
                
-               351          30 LOAD_CONST               3 ('#1473c5')
+               336          40 LOAD_CONST               4 ('#1473c5')
                
-               352          32 LOAD_CONST               4 ('#0067c0')
+               337          42 LOAD_CONST               5 ('#ffffff')
                
-               353          34 LOAD_CONST               5 ('#ffffff')
+               338          44 LOAD_CONST               6 (1)
                
-               355          36 LOAD_CONST               3 ('#1473c5')
+               334          46 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+                            48 BUILD_CONST_KEY_MAP      4
                
-               356          38 LOAD_CONST               6 ('#1975c5')
+               342          50 LOAD_CONST               9 ('#3284cb')
                
-               357          40 LOAD_CONST               5 ('#ffffff')
+               343          52 LOAD_CONST               9 ('#3284cb')
                
-               359          42 LOAD_CONST               7 ('#3284cb')
+               344          54 LOAD_CONST              10 ('#fdfdfd')
                
-               360          44 LOAD_CONST               7 ('#3284cb')
+               345          56 LOAD_CONST               6 (1)
                
-               361          46 LOAD_CONST               8 ('#fdfdfd')
+               341          58 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+                            60 BUILD_CONST_KEY_MAP      4
                
-               346          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+               327          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            64 BUILD_CONST_KEY_MAP      7
                
-               345          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               326          66 BUILD_MAP                1
+               
+               325          68 PRECALL                  1
+                            72 CALL                     1
+                            82 POP_TOP
+                            84 LOAD_CONST               0 (None)
+                            86 RETURN_VALUE
                consts
                   None
+                  'button'
                   8
-                  1
-                  '#1473c5'
                   '#0067c0'
+                  '#1473c5'
                   '#ffffff'
+                  1
                   '#1975c5'
+                  ('back', 'border', 'text_back', 'border_width')
                   '#3284cb'
                   '#fdfdfd'
-                  ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 344
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               firstlineno 324
+               lnotab
+                  0x0201180202010201020102010201020302010201020102fc0408020102
+                  01020102fc04f204ff02ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundAccentButton'
-         firstlineno 343
+         firstlineno 323
          lnotab 0x0a01
       'AdwDrawRoundAccentButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         366           0 RESUME                   0
+         352           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         367          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 367>)
+         353          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 353>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               367           0 RESUME                   0
+               353           0 RESUME                   0
                
-               368           2 LOAD_FAST                0 (self)
+               354           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 367
+               firstlineno 353
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundDarkButton'
-         firstlineno 366
+         firstlineno 352
          lnotab 0x0a01
       'AdwDrawRoundDarkButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a03640284005a0464035300
-         371           0 RESUME                   0
+         357           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundButton2')
                        8 STORE_NAME               2 (__qualname__)
          
-         372          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 372>)
+         358          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 358>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (_draw)
          
-         389          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 389>)
+         375          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 375>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (default_palette)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'AdwDrawRoundButton2'
             code
@@ -2679,29 +2676,29 @@
                   0000000000010064027c005f0700000000000000007c00a0080000000000
                   0000000000000000000000000000007c00a0020000000000000000000000
                   000000000000000000a6000000ab00000000000000000064037a0b00007c
                   00a0030000000000000000000000000000000000000000a6000000ab0000
                   0000000000000064037a0b00007c006a0900000000000000007c006a0a00
                   000000000000007c006a0b0000000000000000ac06a6050000ab05000000
                   00000000007c005f0c000000000000000064005300
-               372           0 RESUME                   0
+               358           0 RESUME                   0
                
-               373           2 LOAD_FAST                0 (self)
+               359           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               375          44 LOAD_FAST                0 (self)
+               361          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect3)
                
-               376          68 LOAD_CONST               2 ('button_frame')
+               362          68 LOAD_CONST               2 ('button_frame')
                
-               377          70 LOAD_CONST               3 (2)
+               363          70 LOAD_CONST               3 (2)
                             72 LOAD_CONST               3 (2)
                             74 LOAD_FAST                0 (self)
                             76 LOAD_METHOD              2 (winfo_width)
                             98 PRECALL                  0
                            102 CALL                     0
                            112 LOAD_CONST               4 (3)
                            114 BINARY_OP               10 (-)
@@ -2710,53 +2707,53 @@
                            142 PRECALL                  0
                            146 CALL                     0
                            156 LOAD_CONST               4 (3)
                            158 BINARY_OP               10 (-)
                            162 LOAD_FAST                0 (self)
                            164 LOAD_ATTR                4 (button_radius)
                
-               378         174 LOAD_FAST                0 (self)
+               364         174 LOAD_FAST                0 (self)
                            176 LOAD_ATTR                5 (_button_border)
                            186 LOAD_FAST                0 (self)
                            188 LOAD_ATTR                6 (_button_back)
                
-               375         198 KW_NAMES                 5
+               361         198 KW_NAMES                 5
                            200 PRECALL                  8
                            204 CALL                     8
                            214 POP_TOP
                
-               381         216 LOAD_CONST               2 ('button_frame')
+               367         216 LOAD_CONST               2 ('button_frame')
                            218 LOAD_FAST                0 (self)
                            220 STORE_ATTR               7 (button_frame)
                
-               383         230 LOAD_FAST                0 (self)
+               369         230 LOAD_FAST                0 (self)
                            232 LOAD_METHOD              8 (create_text)
                
-               384         254 LOAD_FAST                0 (self)
+               370         254 LOAD_FAST                0 (self)
                            256 LOAD_METHOD              2 (winfo_width)
                            278 PRECALL                  0
                            282 CALL                     0
                            292 LOAD_CONST               3 (2)
                            294 BINARY_OP               11 (/)
                            298 LOAD_FAST                0 (self)
                            300 LOAD_METHOD              3 (winfo_height)
                            322 PRECALL                  0
                            326 CALL                     0
                            336 LOAD_CONST               3 (2)
                            338 BINARY_OP               11 (/)
                
-               385         342 LOAD_FAST                0 (self)
+               371         342 LOAD_FAST                0 (self)
                            344 LOAD_ATTR                9 (text)
                            354 LOAD_FAST                0 (self)
                            356 LOAD_ATTR               10 (_button_text_back)
                
-               386         366 LOAD_FAST                0 (self)
+               372         366 LOAD_FAST                0 (self)
                            368 LOAD_ATTR               11 (button_text_font)
                
-               383         378 KW_NAMES                 6
+               369         378 KW_NAMES                 6
                            380 PRECALL                  5
                            384 CALL                     5
                            394 LOAD_FAST                0 (self)
                            396 STORE_ATTR              12 (button_text)
                            406 LOAD_CONST               0 (None)
                            408 RETURN_VALUE
                consts
@@ -2769,564 +2766,586 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_round_rect3', 'winfo_width', 'winfo_height', 'button_radius', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_draw'
-               firstlineno 372
+               firstlineno 358
                lnotab 0x02012a0218010201680118fd12060e021801580118010cfd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               389           0 RESUME                   0
+               375           0 RESUME                   0
                
-               390           2 LOAD_FAST                0 (self)
+               376           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 389
+               firstlineno 375
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '_draw', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundButton2'
-         firstlineno 371
+         firstlineno 357
          lnotab 0x0a010611
       'AdwDrawRoundButton2'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         393           0 RESUME                   0
+         379           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundAccentButton2')
                        8 STORE_NAME               2 (__qualname__)
          
-         394          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 394>)
+         380          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 380>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundAccentButton2'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564036406640564076407640864099c0ba6010000ab0100
-                  00000000000000010064005300
-               394           0 RESUME                   0
+                  026403640464056406640764046405640664089c0464096409640a640664
+                  089c04640b9c076901a6010000ab010000000000000000010064005300
+               380           0 RESUME                   0
                
-               395           2 LOAD_FAST                0 (self)
+               381           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               397          26 LOAD_CONST               1 (8)
+               383          26 LOAD_CONST               1 ('button')
+               
+               384          28 LOAD_CONST               2 (8)
+               
+               385          30 LOAD_CONST               3 ('#0067c0')
                
-               399          28 LOAD_CONST               2 (1)
+               386          32 LOAD_CONST               4 ('#1473c5')
                
-               401          30 LOAD_CONST               3 ('#1473c5')
+               387          34 LOAD_CONST               5 ('#ffffff')
                
-               402          32 LOAD_CONST               4 ('#0067c0')
+               388          36 LOAD_CONST               6 (1)
                
-               403          34 LOAD_CONST               5 ('#ffffff')
+               391          38 LOAD_CONST               7 ('#1975c5')
                
-               405          36 LOAD_CONST               3 ('#1473c5')
+               392          40 LOAD_CONST               4 ('#1473c5')
                
-               406          38 LOAD_CONST               6 ('#1975c5')
+               393          42 LOAD_CONST               5 ('#ffffff')
                
-               407          40 LOAD_CONST               5 ('#ffffff')
+               394          44 LOAD_CONST               6 (1)
                
-               409          42 LOAD_CONST               7 ('#3284cb')
+               390          46 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+                            48 BUILD_CONST_KEY_MAP      4
                
-               410          44 LOAD_CONST               7 ('#3284cb')
+               398          50 LOAD_CONST               9 ('#3284cb')
                
-               411          46 LOAD_CONST               8 ('#fdfdfd')
+               399          52 LOAD_CONST               9 ('#3284cb')
                
-               396          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+               400          54 LOAD_CONST              10 ('#fdfdfd')
                
-               395          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               401          56 LOAD_CONST               6 (1)
+               
+               397          58 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+                            60 BUILD_CONST_KEY_MAP      4
+               
+               383          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            64 BUILD_CONST_KEY_MAP      7
+               
+               382          66 BUILD_MAP                1
+               
+               381          68 PRECALL                  1
+                            72 CALL                     1
+                            82 POP_TOP
+                            84 LOAD_CONST               0 (None)
+                            86 RETURN_VALUE
                consts
                   None
+                  'button'
                   8
-                  1
-                  '#1473c5'
                   '#0067c0'
+                  '#1473c5'
                   '#ffffff'
+                  1
                   '#1975c5'
+                  ('back', 'border', 'text_back', 'border_width')
                   '#3284cb'
                   '#fdfdfd'
-                  ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 394
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               firstlineno 380
+               lnotab
+                  0x0201180202010201020102010201020302010201020102fc0408020102
+                  01020102fc04f204ff02ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundAccentButton2'
-         firstlineno 393
+         firstlineno 379
          lnotab 0x0a01
       'AdwDrawRoundAccentButton2'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         416           0 RESUME                   0
+         408           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkButton2')
                        8 STORE_NAME               2 (__qualname__)
          
-         417          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 417>)
+         409          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 409>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkButton2'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               417           0 RESUME                   0
+               409           0 RESUME                   0
                
-               418           2 LOAD_FAST                0 (self)
+               410           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 417
+               firstlineno 409
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundDarkButton2'
-         firstlineno 416
+         firstlineno 408
          lnotab 0x0a01
       'AdwDrawRoundDarkButton2'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a03640284005a0464035300
-         421           0 RESUME                   0
+         413           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundButton3')
                        8 STORE_NAME               2 (__qualname__)
          
-         422          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 422>)
+         414          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 414>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (_draw)
          
-         439          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 439>)
+         431          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 431>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (default_palette)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'AdwDrawRoundButton3'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab01000000000000000001007c00a0010000000000000000000000
-                  0000000000000000007c006a02000000000000000064027a0000007c006a
-                  02000000000000000064027a0000007c00a0030000000000000000000000
-                  000000000000000000a6000000ab0000000000000000007c006a02000000
-                  00000000007a0a000064037a0a00007c00a0040000000000000000000000
-                  000000000000000000a6000000ab0000000000000000007c006a02000000
-                  00000000007a0a000064037a0a00007c006a0500000000000000007c006a
-                  0200000000000000007c006a0600000000000000007c006a070000000000
-                  000000ac04a6080000ab080000000000000000010064057c005f08000000
-                  00000000007c00a00900000000000000000000000000000000000000007c
-                  00a0030000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000064037a0b00007c00a00400000000000000000000000000
-                  00000000000000a6000000ab00000000000000000064037a0b00007c006a
-                  0a00000000000000007c006a0b00000000000000007c006a0c0000000000
-                  000000ac06a6050000ab0500000000000000007c005f0d00000000000000
-                  0064005300
-               422           0 RESUME                   0
+                  000000000000000000640264027c00a00200000000000000000000000000
+                  00000000000000a6000000ab00000000000000000064037a0a00007c00a0
+                  030000000000000000000000000000000000000000a6000000ab00000000
+                  000000000064037a0a00007c006a0400000000000000007c006a05000000
+                  00000000007c006a0600000000000000007c006a070000000000000000ac
+                  04a6080000ab080000000000000000010064057c005f0800000000000000
+                  007c00a00900000000000000000000000000000000000000007c00a00200
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  00000064037a0b00007c00a0030000000000000000000000000000000000
+                  000000a6000000ab00000000000000000064037a0b00007c006a0a000000
+                  00000000007c006a0b00000000000000007c006a0c0000000000000000ac
+                  06a6050000ab0500000000000000007c005f0d0000000000000000640053
+                  00
+               414           0 RESUME                   0
                
-               423           2 LOAD_FAST                0 (self)
+               415           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               425          44 LOAD_FAST                0 (self)
+               417          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
-               426          68 LOAD_FAST                0 (self)
-                            70 LOAD_ATTR                2 (button_border_width)
-                            80 LOAD_CONST               2 (1)
-                            82 BINARY_OP                0 (+)
-                            86 LOAD_FAST                0 (self)
-                            88 LOAD_ATTR                2 (button_border_width)
-                            98 LOAD_CONST               2 (1)
-                           100 BINARY_OP                0 (+)
-                           104 LOAD_FAST                0 (self)
-                           106 LOAD_METHOD              3 (winfo_width)
-                           128 PRECALL                  0
-                           132 CALL                     0
-                           142 LOAD_FAST                0 (self)
-                           144 LOAD_ATTR                2 (button_border_width)
-                           154 BINARY_OP               10 (-)
-                           158 LOAD_CONST               3 (2)
-                           160 BINARY_OP               10 (-)
-                           164 LOAD_FAST                0 (self)
-                           166 LOAD_METHOD              4 (winfo_height)
-                           188 PRECALL                  0
-                           192 CALL                     0
-                           202 LOAD_FAST                0 (self)
-                           204 LOAD_ATTR                2 (button_border_width)
-                           214 BINARY_OP               10 (-)
-                           218 LOAD_CONST               3 (2)
-                           220 BINARY_OP               10 (-)
-                           224 LOAD_FAST                0 (self)
-                           226 LOAD_ATTR                5 (button_radius)
+               418          68 LOAD_CONST               2 (1)
+                            70 LOAD_CONST               2 (1)
+                            72 LOAD_FAST                0 (self)
+                            74 LOAD_METHOD              2 (winfo_width)
+                            96 PRECALL                  0
+                           100 CALL                     0
+                           110 LOAD_CONST               3 (2)
+                           112 BINARY_OP               10 (-)
+                           116 LOAD_FAST                0 (self)
+                           118 LOAD_METHOD              3 (winfo_height)
+                           140 PRECALL                  0
+                           144 CALL                     0
+                           154 LOAD_CONST               3 (2)
+                           156 BINARY_OP               10 (-)
+                           160 LOAD_FAST                0 (self)
+                           162 LOAD_ATTR                4 (button_radius)
                
-               427         236 LOAD_FAST                0 (self)
-                           238 LOAD_ATTR                2 (button_border_width)
+               419         172 LOAD_FAST                0 (self)
+                           174 LOAD_ATTR                5 (_button_border_width)
                
-               428         248 LOAD_FAST                0 (self)
-                           250 LOAD_ATTR                6 (_button_border)
-                           260 LOAD_FAST                0 (self)
-                           262 LOAD_ATTR                7 (_button_back)
-               
-               425         272 KW_NAMES                 4
-                           274 PRECALL                  8
-                           278 CALL                     8
-                           288 POP_TOP
+               420         184 LOAD_FAST                0 (self)
+                           186 LOAD_ATTR                6 (_button_border)
+                           196 LOAD_FAST                0 (self)
+                           198 LOAD_ATTR                7 (_button_back)
                
-               431         290 LOAD_CONST               5 ('button_frame')
-                           292 LOAD_FAST                0 (self)
-                           294 STORE_ATTR               8 (button_frame)
+               417         208 KW_NAMES                 4
+                           210 PRECALL                  8
+                           214 CALL                     8
+                           224 POP_TOP
+               
+               423         226 LOAD_CONST               5 ('button_frame')
+                           228 LOAD_FAST                0 (self)
+                           230 STORE_ATTR               8 (button_frame)
                
-               433         304 LOAD_FAST                0 (self)
-                           306 LOAD_METHOD              9 (create_text)
+               425         240 LOAD_FAST                0 (self)
+                           242 LOAD_METHOD              9 (create_text)
                
-               434         328 LOAD_FAST                0 (self)
-                           330 LOAD_METHOD              3 (winfo_width)
-                           352 PRECALL                  0
-                           356 CALL                     0
-                           366 LOAD_CONST               3 (2)
-                           368 BINARY_OP               11 (/)
-                           372 LOAD_FAST                0 (self)
-                           374 LOAD_METHOD              4 (winfo_height)
-                           396 PRECALL                  0
-                           400 CALL                     0
-                           410 LOAD_CONST               3 (2)
-                           412 BINARY_OP               11 (/)
-               
-               435         416 LOAD_FAST                0 (self)
-                           418 LOAD_ATTR               10 (text)
-                           428 LOAD_FAST                0 (self)
-                           430 LOAD_ATTR               11 (_button_text_back)
-               
-               436         440 LOAD_FAST                0 (self)
-                           442 LOAD_ATTR               12 (button_text_font)
-               
-               433         452 KW_NAMES                 6
-                           454 PRECALL                  5
-                           458 CALL                     5
-                           468 LOAD_FAST                0 (self)
-                           470 STORE_ATTR              13 (button_text)
-                           480 LOAD_CONST               0 (None)
-                           482 RETURN_VALUE
+               426         264 LOAD_FAST                0 (self)
+                           266 LOAD_METHOD              2 (winfo_width)
+                           288 PRECALL                  0
+                           292 CALL                     0
+                           302 LOAD_CONST               3 (2)
+                           304 BINARY_OP               11 (/)
+                           308 LOAD_FAST                0 (self)
+                           310 LOAD_METHOD              3 (winfo_height)
+                           332 PRECALL                  0
+                           336 CALL                     0
+                           346 LOAD_CONST               3 (2)
+                           348 BINARY_OP               11 (/)
+               
+               427         352 LOAD_FAST                0 (self)
+                           354 LOAD_ATTR               10 (text)
+                           364 LOAD_FAST                0 (self)
+                           366 LOAD_ATTR               11 (_button_text_back)
+               
+               428         376 LOAD_FAST                0 (self)
+                           378 LOAD_ATTR               12 (button_text_font)
+               
+               425         388 KW_NAMES                 6
+                           390 PRECALL                  5
+                           394 CALL                     5
+                           404 LOAD_FAST                0 (self)
+                           406 STORE_ATTR              13 (button_text)
+                           416 LOAD_CONST               0 (None)
+                           418 RETURN_VALUE
                consts
                   None
                   'all'
                   1
                   2
                   ('width', 'outline', 'fill')
                   'button_frame'
                   ('text', 'fill', 'font')
-               names      ('delete', 'create_round_rect4', 'button_border_width', 'winfo_width', 'winfo_height', 'button_radius', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
+               names      ('delete', 'create_round_rect4', 'winfo_width', 'winfo_height', 'button_radius', '_button_border_width', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_draw'
-               firstlineno 422
-               lnotab 0x02012a021801a8010c0118fd12060e021801580118010cfd
+               firstlineno 414
+               lnotab 0x02012a02180168010c0118fd12060e021801580118010cfd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               439           0 RESUME                   0
+               431           0 RESUME                   0
                
-               440           2 LOAD_FAST                0 (self)
+               432           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 439
+               firstlineno 431
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '_draw', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundButton3'
-         firstlineno 421
+         firstlineno 413
          lnotab 0x0a010611
       'AdwDrawRoundButton3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         443           0 RESUME                   0
+         435           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundAccentButton3')
                        8 STORE_NAME               2 (__qualname__)
          
-         444          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 444>)
+         436          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 436>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundAccentButton3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564036406640564076407640864099c0ba6010000ab0100
-                  00000000000000010064005300
-               444           0 RESUME                   0
+                  026403640464056406640764046405640664089c0464096409640a640664
+                  089c04640b9c076901a6010000ab010000000000000000010064005300
+               436           0 RESUME                   0
                
-               445           2 LOAD_FAST                0 (self)
+               437           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               447          26 LOAD_CONST               1 (8)
+               439          26 LOAD_CONST               1 ('button')
+               
+               440          28 LOAD_CONST               2 (8)
+               
+               441          30 LOAD_CONST               3 ('#0067c0')
+               
+               442          32 LOAD_CONST               4 ('#1473c5')
+               
+               443          34 LOAD_CONST               5 ('#ffffff')
                
-               449          28 LOAD_CONST               2 (1)
+               444          36 LOAD_CONST               6 (1)
                
-               451          30 LOAD_CONST               3 ('#1473c5')
+               447          38 LOAD_CONST               7 ('#1975c5')
                
-               452          32 LOAD_CONST               4 ('#0067c0')
+               448          40 LOAD_CONST               4 ('#1473c5')
                
-               453          34 LOAD_CONST               5 ('#ffffff')
+               449          42 LOAD_CONST               5 ('#ffffff')
                
-               455          36 LOAD_CONST               3 ('#1473c5')
+               450          44 LOAD_CONST               6 (1)
                
-               456          38 LOAD_CONST               6 ('#1975c5')
+               446          46 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+                            48 BUILD_CONST_KEY_MAP      4
                
-               457          40 LOAD_CONST               5 ('#ffffff')
+               454          50 LOAD_CONST               9 ('#3284cb')
                
-               459          42 LOAD_CONST               7 ('#3284cb')
+               455          52 LOAD_CONST               9 ('#3284cb')
                
-               460          44 LOAD_CONST               7 ('#3284cb')
+               456          54 LOAD_CONST              10 ('#fdfdfd')
                
-               461          46 LOAD_CONST               8 ('#fdfdfd')
+               457          56 LOAD_CONST               6 (1)
                
-               446          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+               453          58 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+                            60 BUILD_CONST_KEY_MAP      4
                
-               445          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               439          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            64 BUILD_CONST_KEY_MAP      7
+               
+               438          66 BUILD_MAP                1
+               
+               437          68 PRECALL                  1
+                            72 CALL                     1
+                            82 POP_TOP
+                            84 LOAD_CONST               0 (None)
+                            86 RETURN_VALUE
                consts
                   None
+                  'button'
                   8
-                  1
-                  '#1473c5'
                   '#0067c0'
+                  '#1473c5'
                   '#ffffff'
+                  1
                   '#1975c5'
+                  ('back', 'border', 'text_back', 'border_width')
                   '#3284cb'
                   '#fdfdfd'
-                  ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 444
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               firstlineno 436
+               lnotab
+                  0x0201180202010201020102010201020302010201020102fc0408020102
+                  01020102fc04f204ff02ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundAccentButton3'
-         firstlineno 443
+         firstlineno 435
          lnotab 0x0a01
       'AdwDrawRoundAccentButton3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         466           0 RESUME                   0
+         464           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkButton3')
                        8 STORE_NAME               2 (__qualname__)
          
-         467          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 467>)
+         465          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 465>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkButton3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               467           0 RESUME                   0
+               465           0 RESUME                   0
                
-               468           2 LOAD_FAST                0 (self)
+               466           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 467
+               firstlineno 465
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundDarkButton3'
-         firstlineno 466
+         firstlineno 464
          lnotab 0x0a01
       'AdwDrawRoundDarkButton3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a026401640164029c02880066016403840a5a
             03640484005a04880078015a055300
                        0 MAKE_CELL                0 (__class__)
          
-         472           2 RESUME                   0
+         470           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicCircularButton')
                       10 STORE_NAME               2 (__qualname__)
          
-         473          12 LOAD_CONST               1 (120)
+         471          12 LOAD_CONST               1 (120)
                       14 LOAD_CONST               1 (120)
                       16 LOAD_CONST               2 (('width', 'height'))
                       18 BUILD_CONST_KEY_MAP      2
                       20 LOAD_CLOSURE             0 (__class__)
                       22 BUILD_TUPLE              1
-                      24 LOAD_CONST               3 (<code object __init__, file "D:\tkadw\tkadw\canvas\button.py", line 473>)
+                      24 LOAD_CONST               3 (<code object __init__, file "D:\tkadw\tkadw\canvas\button.py", line 471>)
                       26 MAKE_FUNCTION           10 (kwdefaults, closure)
                       28 STORE_NAME               3 (__init__)
          
-         476          30 LOAD_CONST               4 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 476>)
+         474          30 LOAD_CONST               4 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 474>)
                       32 MAKE_FUNCTION            0
                       34 STORE_NAME               4 (_draw)
                       36 LOAD_CLOSURE             0 (__class__)
                       38 COPY                     1
                       40 STORE_NAME               5 (__classcell__)
                       42 RETURN_VALUE
          consts
@@ -3340,17 +3359,17 @@
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c037c017c0264019c027c04a4018e0101
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               473           2 RESUME                   0
+               471           2 RESUME                   0
                
-               474           4 PUSH_NULL
+               472           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                3 (args)
                             44 LOAD_FAST                1 (width)
                             46 LOAD_FAST                2 (height)
@@ -3367,15 +3386,15 @@
                   ('width', 'height')
                names      ('super', '__init__')
                varnames   ('self', 'width', 'height', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '__init__'
-               firstlineno 473
+               firstlineno 471
                lnotab 0x0401
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 9
                flags     : 3
                code
@@ -3389,80 +3408,80 @@
                   0000007c005f0700000000000000007c00a0080000000000000000000000
                   0000000000000000007c00a0020000000000000000000000000000000000
                   000000a6000000ab00000000000000000064057a0b00007c00a003000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0064057a0b00007c006a0900000000000000007c006a0a00000000000000
                   007c006a0b0000000000000000ac06a6050000ab0500000000000000007c
                   005f0c000000000000000064005300
-               476           0 RESUME                   0
+               474           0 RESUME                   0
                
-               477           2 LOAD_FAST                0 (self)
+               475           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               479          44 LOAD_FAST                0 (self)
+               477          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_oval)
                
-               480          68 LOAD_CONST               2 (1.5)
+               478          68 LOAD_CONST               2 (1.5)
                             70 LOAD_CONST               2 (1.5)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
                            116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                
-               481         160 LOAD_FAST                0 (self)
+               479         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (button_border_width)
                
-               482         172 LOAD_FAST                0 (self)
+               480         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (_button_border)
                            184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_button_back)
                
-               479         196 KW_NAMES                 4
+               477         196 KW_NAMES                 4
                            198 PRECALL                  7
                            202 CALL                     7
                            212 LOAD_FAST                0 (self)
                            214 STORE_ATTR               7 (button_frame)
                
-               485         224 LOAD_FAST                0 (self)
+               483         224 LOAD_FAST                0 (self)
                            226 LOAD_METHOD              8 (create_text)
                
-               486         248 LOAD_FAST                0 (self)
+               484         248 LOAD_FAST                0 (self)
                            250 LOAD_METHOD              2 (winfo_width)
                            272 PRECALL                  0
                            276 CALL                     0
                            286 LOAD_CONST               5 (2)
                            288 BINARY_OP               11 (/)
                            292 LOAD_FAST                0 (self)
                            294 LOAD_METHOD              3 (winfo_height)
                            316 PRECALL                  0
                            320 CALL                     0
                            330 LOAD_CONST               5 (2)
                            332 BINARY_OP               11 (/)
                
-               487         336 LOAD_FAST                0 (self)
+               485         336 LOAD_FAST                0 (self)
                            338 LOAD_ATTR                9 (text)
                            348 LOAD_FAST                0 (self)
                            350 LOAD_ATTR               10 (_button_text_back)
                
-               488         360 LOAD_FAST                0 (self)
+               486         360 LOAD_FAST                0 (self)
                            362 LOAD_ATTR               11 (button_text_font)
                
-               485         372 KW_NAMES                 6
+               483         372 KW_NAMES                 6
                            374 PRECALL                  5
                            378 CALL                     5
                            388 LOAD_FAST                0 (self)
                            390 STORE_ATTR              12 (button_text)
                            400 LOAD_CONST               0 (None)
                            402 RETURN_VALUE
                consts
@@ -3475,135 +3494,135 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_oval', 'winfo_width', 'winfo_height', 'button_border_width', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_draw'
-               firstlineno 476
+               firstlineno 474
                lnotab 0x02012a0218015c010c0118fd1c061801580118010cfd
          names      ('__name__', '__module__', '__qualname__', '__init__', '_draw', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawBasicCircularButton'
-         firstlineno 472
+         firstlineno 470
          lnotab 0x0c011203
       'AdwDrawBasicCircularButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         492           0 RESUME                   0
+         490           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawCircularButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         493          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 493>)
+         491          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 491>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawCircularButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               493           0 RESUME                   0
+               491           0 RESUME                   0
                
-               494           2 LOAD_FAST                0 (self)
+               492           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 493
+               firstlineno 491
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawCircularButton'
-         firstlineno 492
+         firstlineno 490
          lnotab 0x0a01
       'AdwDrawCircularButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         497           0 RESUME                   0
+         495           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawCircularDarkButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         498          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 498>)
+         496          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 496>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawCircularDarkButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               498           0 RESUME                   0
+               496           0 RESUME                   0
                
-               499           2 LOAD_FAST                0 (self)
+               497           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 498
+               firstlineno 496
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawCircularDarkButton'
-         firstlineno 497
+         firstlineno 495
          lnotab 0x0a01
       'AdwDrawCircularDarkButton'
       '__main__'
       ('Tk',)
       'Hello'
       ('text',)
       '<<Click>>'
@@ -3611,139 +3630,139 @@
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         508           0 RESUME                   0
+         506           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 508
+         firstlineno 506
          lnotab 0x
       'x'
       5
       ('fill', 'padx', 'pady')
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         512           0 RESUME                   0
+         510           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 512
+         firstlineno 510
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         516           0 RESUME                   0
+         514           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 516
+         firstlineno 514
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         520           0 RESUME                   0
+         518           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 520
+         firstlineno 518
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         524           0 RESUME                   0
+         522           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button6 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button6 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 524
+         firstlineno 522
          lnotab 0x
       None
    names      ('tkinter.font', 'Font', 'nametofont', 'tkadw.canvas.drawengine', 'AdwDrawEngine', 'AdwDrawBasicButton', 'AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawBasicRoundButton', 'AdwDrawRoundButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawBasicCircularButton', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton', '__name__', 'tkinter', 'Tk', 'root', 'button', 'bind', 'pack', 'button4', 'button7', 'button10', 'button13', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c041c7f00381c051c051c181c731c051c171c051c161c
-      171c051c161c171c061c141c051c050e010c02140218012e01300218012e
+      0x00ff020110010c041c7f003d1c051c051c1d1c551c051c1d1c051c161c
+      1d1c051c161c1d1c061c141c051c050e010c02140218012e01300218012e
       01300218012e01300218012e01300218012e0130022ce7
```

### Comparing `tkadw-0.1.5/tkadw/canvas/__pycache__/button.cpython-38.pyc` & `tkadw-0.2.0/tkadw/canvas/__pycache__/button.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc` & `tkadw-0.2.0/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x04289564 (Fri Jun 23 05:05:08 2023 UTC)
-files sz: 20382
+moddate:  0x186d9564 (Fri Jun 23 09:59:52 2023 UTC)
+files sz: 20930
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a01010064025a0264035a0302004700640484
@@ -40,105 +40,105 @@
                 28 MAKE_FUNCTION            0
                 30 LOAD_CONST               5 ('AdwDrawEngine')
                 32 LOAD_NAME                1 (Canvas)
                 34 PRECALL                  3
                 38 CALL                     3
                 48 STORE_NAME               4 (AdwDrawEngine)
    
-   583          50 LOAD_NAME                5 (__name__)
+   589          50 LOAD_NAME                5 (__name__)
                 52 LOAD_CONST               6 ('__main__')
                 54 COMPARE_OP               2 (==)
                 60 POP_JUMP_FORWARD_IF_FALSE   145 (to 352)
    
-   584          62 LOAD_CONST               0 (0)
+   590          62 LOAD_CONST               0 (0)
                 64 LOAD_CONST               7 (('Tk',))
                 66 IMPORT_NAME              0 (tkinter)
                 68 IMPORT_FROM              6 (Tk)
                 70 STORE_NAME               6 (Tk)
                 72 POP_TOP
    
-   586          74 PUSH_NULL
+   592          74 PUSH_NULL
                 76 LOAD_NAME                6 (Tk)
                 78 PRECALL                  0
                 82 CALL                     0
                 92 STORE_NAME               7 (root)
    
-   588          94 PUSH_NULL
+   594          94 PUSH_NULL
                 96 LOAD_NAME                4 (AdwDrawEngine)
                 98 PRECALL                  0
                102 CALL                     0
                112 STORE_NAME               8 (canvas)
    
-   590         114 LOAD_NAME                8 (canvas)
+   596         114 LOAD_NAME                8 (canvas)
                116 LOAD_METHOD              9 (create_round_rect3)
                138 LOAD_CONST               8 (10)
                140 LOAD_CONST               9 (15)
                142 LOAD_CONST               9 (15)
                144 LOAD_CONST              10 (150)
                146 LOAD_CONST              10 (150)
                148 LOAD_CONST              11 (50)
                150 PRECALL                  6
                154 CALL                     6
                164 POP_TOP
    
-   591         166 LOAD_NAME                8 (canvas)
+   597         166 LOAD_NAME                8 (canvas)
                168 LOAD_METHOD             10 (create_round_rect4)
                190 LOAD_CONST              12 (160)
                192 LOAD_CONST              12 (160)
                194 LOAD_CONST              13 (300)
                196 LOAD_CONST              13 (300)
                198 LOAD_CONST              11 (50)
                200 PRECALL                  5
                204 CALL                     5
                214 POP_TOP
    
-   593         216 LOAD_NAME                8 (canvas)
+   599         216 LOAD_NAME                8 (canvas)
                218 LOAD_METHOD             11 (bind)
                240 LOAD_CONST              14 ('<Configure>')
-               242 LOAD_CONST              15 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\drawengine.py", line 593>)
+               242 LOAD_CONST              15 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\drawengine.py", line 599>)
                244 MAKE_FUNCTION            0
                246 PRECALL                  2
                250 CALL                     2
                260 POP_TOP
    
-   595         262 LOAD_NAME                8 (canvas)
+   601         262 LOAD_NAME                8 (canvas)
                264 LOAD_METHOD             12 (pack)
                286 LOAD_CONST              16 ('both')
                288 LOAD_CONST              17 ('yes')
                290 KW_NAMES                18
                292 PRECALL                  2
                296 CALL                     2
                306 POP_TOP
    
-   597         308 LOAD_NAME                7 (root)
+   603         308 LOAD_NAME                7 (root)
                310 LOAD_METHOD             13 (mainloop)
                332 PRECALL                  0
                336 CALL                     0
                346 POP_TOP
                348 LOAD_CONST              19 (None)
                350 RETURN_VALUE
    
-   583     >>  352 LOAD_CONST              19 (None)
+   589     >>  352 LOAD_CONST              19 (None)
                354 RETURN_VALUE
    consts
       0
       ('Canvas',)
       '\n# poly.tcl\n\nproc poly_round {win outline fill args} {\n    if {[llength $args] % 3 != 0 || [llength $args] < 9} {\n        error "wrong # args: should be "poly_round                win outline fill x1 y1 d1 x2 y2 d2 x3 y3 d3 ?...?""\n    }\n\n    # Determine the tag to use.\n    if {![info exists ::poly_next_id]} {\n        set ::poly_next_id 1\n    }\n    set tag poly#$::poly_next_id\n    incr ::poly_next_id\n\n    # Filter out illegal circles and collinear points.\n    set pts [list]\n    lassign [lrange $args 0 4] Ux Uy d Vx Vy\n    foreach {d Wx Wy} [concat [lrange $args 5 end] [lrange $args 0 4]] {\n        set test [expr {$Ux * ($Vy - $Wy) - $Vx * ($Uy - $Wy) +\n                $Wx * ($Uy - $Vy)}]\n        if {($d > 0) && $test != 0} {\n            lappend pts $Vx $Vy $d $test\n            lassign [list $Wx $Wy $Vx $Vy] Vx Vy Ux Uy\n        } else {\n            lassign [list $Wx $Wy] Vx Vy\n        }\n    }\n\n    # V    C    T   W\n    #  *---*----*-+-*-- Given: U, V, W, d\n    #  |\\ /    /|_|     Find:  S, E, T\n    #  | *B   / |\n    #  |/ \\  /  |       The length of ES and ET each is d.\n    # A*   \\/   |\n    #  |   /\\   |       VB bisects angle UVW.  SE _|_ VU; TE _|_ VW.\n    #  |  /  \\  |       B is halfway between A and C.\n    #  | /    \\ |       Angles UVW and SET are not necessarily right.\n    #  |/      \\|       The length of AV and CV each is 1.\n    # S*-+------*E\n    #  |_|       \\      The new polygon is along USTW.\n    # U*          \\     The new arc has center E, radius d, and angle SET, and\n    #  |           \\    it is tangential to VU at S and VW at T.\n\n    # Calculate new polygon vertices and create arcs.\n    set coords [list]\n    lassign [lrange $pts 0 5] Ux Uy d test Vx Vy\n    foreach {d test Wx Wy} [concat [lrange $pts 6 end] [lrange $pts 0 5]] {\n        # Find A and C.\n        foreach {pt x y} [list A $Ux $Uy C $Wx $Wy] {\n            set      k [expr {sqrt(($Vx - $x) ** 2 + ($Vy - $y) ** 2)}]\n            set ${pt}x [expr {($x - $Vx) / $k + $Vx}]\n            set ${pt}y [expr {($y - $Vy) / $k + $Vy}]\n        }\n\n        # Find B.\n        set Bx [expr {($Ax + $Cx) / 2.0}]\n        set By [expr {($Ay + $Cy) / 2.0}]\n\n        # Find the parameters for lines VB and VW.\n        foreach {pt x y} [list B $Bx $By W $Wx $Wy] {\n            set       k [expr {sqrt(($Vx - $x) ** 2 + ($Vy - $y) ** 2)}]\n            set V${pt}a [expr {+($Vy - $y) / $k}]\n            set V${pt}b [expr {-($Vx - $x) / $k}]\n            set V${pt}c [expr {($Vx * $y - $Vy * $x) / $k}]\n        }\n\n        # Find point E.\n        set sign [expr {$test < 0 ? -1 : +1}]\n        set  k [expr {$VWa * $VBb - $VWb * $VBa}]\n        set Ex [expr {(+$VWb * $VBc - ($VWc - $d * $sign) * $VBb) / $k}]\n        set Ey [expr {(-$VWa * $VBc + ($VWc - $d * $sign) * $VBa) / $k}]\n\n        # Find tangent points S and T.\n        foreach {pt x y} [list S $Ux $Uy T $Wx $Wy] {\n            set      k [expr {($Vx - $x) ** 2 + ($Vy - $y) ** 2}]\n            set ${pt}x [expr {($Ex * ($Vx - $x) ** 2 + ($Vy - $y) *\n                              ($Ey * ($Vx - $x) - $Vx * $y + $Vy * $x)) / $k}]\n            set ${pt}y [expr {($Ex * ($Vx - $x) * ($Vy - $y) +\n                              ($Ey * ($Vy - $y) ** 2 + ($Vx - $x) *\n                              ($Vx * $y - $Vy * $x))) / $k}]\n        }\n\n        # Find directions for lines ES and ET.\n        foreach {pt x y} [list S $Sx $Sy T $Tx $Ty] {\n            set E${pt}d [expr {atan2($Ey - $y, $x - $Ex)}]\n        }\n\n        # Find start and extent directions.\n        if {$ESd < 0 && $ETd > 0} {\n            set start  [expr {180 / acos(-1) * $ETd}]\n            set extent [expr {180 / acos(-1) * ($ESd - $ETd)}]\n            if {$sign > 0} {\n                set extent [expr {$extent + 360}]\n            }\n        } else {\n            set start  [expr {180 / acos(-1) * $ESd}]\n            set extent [expr {180 / acos(-1) * ($ETd - $ESd)}]\n            if {$sign < 0 && $ESd > 0 && $ETd < 0} {\n                set extent [expr {$extent + 360}]\n            }\n        }\n\n        # Draw arc.\n        set opts [list                                             [expr {$Ex - $d}] [expr {$Ey - $d}]                [expr {$Ex + $d}] [expr {$Ey + $d}]                -start $start -extent $extent]\n        $win create arc {*}$opts -style pie -tags [list $tag pie]\n        $win create arc {*}$opts -style arc -tags [list $tag arc]\n\n        # Draw border line.\n        if {[info exists prevx]} {\n            $win create line $prevx $prevy $Sx $Sy -tags [list $tag line]\n        } else {\n            lassign [list $Sx $Sy] firstx firsty\n        }\n        lassign [list $Tx $Ty] prevx prevy\n\n        # Remember coordinates for polygon.\n        lappend coords $Sx $Sy $Tx $Ty\n\n        # Rotate vertices.\n        lassign [list $Wx $Wy $Vx $Vy] Vx Vy Ux Uy\n    }\n\n    # Draw final border line.\n    $win create line $prevx $prevy $firstx $firsty -tags [list $tag line]\n\n    # Draw fill polygon.\n    $win create polygon {*}$coords -tags [list $tag poly]\n\n    # Configure colors.\n    $win itemconfigure $tag&&(poly||pie) -fill $fill\n    $win itemconfigure $tag&&pie         -outline ""\n    $win itemconfigure $tag&&line        -fill $outline -capstyle round\n    $win itemconfigure $tag&&arc         -outline $outline\n\n    # Set proper stacking order.\n    $win raise $tag&&poly\n    $win raise $tag&&pie\n    $win raise $tag&&(line||arc)\n\n    return $tag\n}\n       '
       '\n #----------------------------------------------------------------------\n #\n # RoundPoly -- Draw a polygon with rounded corners in the canvas, based\n # off of ideas and code from "Drawing rounded rectangles"\n #\n # Parameters:\n #       w - Path name of the canvas\n #       xy - list of coordinates of the vertices of the polygon\n #       radii - list of radius of the bend each each vertex\n #       args - Other args suitable to a \'polygon\' item on the canvas\n #\n # Results:\n #       Returns the canvas item number of the rounded polygon.\n #\n # Side effects:\n #       Creates a rounded polygon in the canvas.\n #\n #----------------------------------------------------------------------\n \n proc RoundPoly {w xy radii args} {\n    set lenXY [llength $xy]\n    set lenR [llength $radii]\n    if {$lenXY != 2 * $lenR} {\n        error "wrong number of vertices and radii"\n    }\n \n    # Walk down vertices keeping previous, current and next\n    lassign [lrange $xy end-1 end] x0 y0\n    lassign $xy x1 y1\n    eval lappend xy [lrange $xy 0 1]\n    set knots {}                                ;# These are the control points\n \n    for {set i 0} {$i < $lenXY} {incr i 2} {\n        set radius [lindex $radii [expr {$i/2}]]\n        set r [winfo pixels $w $radius]\n \n        lassign [lrange $xy [expr {$i + 2}] [expr {$i + 3}]] x2 y2\n        set z [_RoundPoly2 $x0 $y0 $x1 $y1 $x2 $y2 $r]\n        eval lappend knots $z\n \n        lassign [list $x1 $y1] x0 y0           ;# Current becomes previous\n        lassign [list $x2 $y2] x1 y1           ;# Next becomes current\n    }\n    set n [eval $w create polygon $knots -smooth 1 $args]\n    return $n\n }\n proc _RoundPoly2 {x0 y0 x1 y1 x2 y2 radius} {\n    set d [expr { 2 * $radius }]\n    set maxr 0.75\n \n    set v1x [expr {$x0 - $x1}]\n    set v1y [expr {$y0 - $y1}]\n    set v2x [expr {$x2 - $x1}]\n    set v2y [expr {$y2 - $y1}]\n \n    set vlen1 [expr {sqrt($v1x*$v1x + $v1y*$v1y)}]\n    set vlen2 [expr {sqrt($v2x*$v2x + $v2y*$v2y)}]\n    if {$d > $maxr * $vlen1} {\n        set d [expr {$maxr * $vlen1}]\n    }\n    if {$d > $maxr * $vlen2} {\n        set d [expr {$maxr * $vlen2}]\n    }\n \n    lappend xy [expr {$x1 + $d * $v1x/$vlen1}] [expr {$y1 + $d * $v1y/$vlen1}]\n    lappend xy $x1 $y1\n    lappend xy [expr {$x1 + $d * $v2x/$vlen2}] [expr {$y1 + $d * $v2y/$vlen2}]\n \n    return $xy\n }\n\n'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
-            14640484015a056415640965066602640a84055a0765075a08640b84005a
-            0965095a0a6416640c650b640d650b6604640e84055a0c650c5a0d640f84
-            005a0e650e5a0f6416641084015a1065105a11641184005a126412650b66
-            02641384045a13880078015a145300
+            17640484015a056418640965066602640a84055a0765075a08640b84005a
+            0965095a0a6419640c650b640d650b6604640e84055a0c650c5a0d640f84
+            005a0e650e5a0f6419641084015a1065105a11641184005a126412650b66
+            02641384045a13641a641684015a14880078015a155300
                        0 MAKE_CELL                0 (__class__)
          
          226           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawEngine')
                       10 STORE_NAME               2 (__qualname__)
@@ -149,20 +149,20 @@
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
          230          22 LOAD_CONST               2 (<code object win32_high_dpi, file "D:\tkadw\tkadw\canvas\drawengine.py", line 230>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (win32_high_dpi)
          
-         234          28 LOAD_CONST              20 (('x',))
+         234          28 LOAD_CONST              23 (('x',))
                       30 LOAD_CONST               4 (<code object draw_gradient, file "D:\tkadw\tkadw\canvas\drawengine.py", line 234>)
                       32 MAKE_FUNCTION            1 (defaults)
                       34 STORE_NAME               5 (draw_gradient)
          
-         301          36 LOAD_CONST              21 ((5, 2, 'white', 'black'))
+         301          36 LOAD_CONST              24 ((5, 2, 'white', 'black'))
                       38 LOAD_CONST               9 ('radius')
                       40 LOAD_NAME                6 (float)
                       42 BUILD_TUPLE              2
                       44 LOAD_CONST              10 (<code object create_round_rectangle, file "D:\tkadw\tkadw\canvas\drawengine.py", line 301>)
                       46 MAKE_FUNCTION            5 (defaults, annotations)
                       48 STORE_NAME               7 (create_round_rectangle)
          
@@ -172,15 +172,15 @@
          334          54 LOAD_CONST              11 (<code object create_round_rectangle2, file "D:\tkadw\tkadw\canvas\drawengine.py", line 334>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               9 (create_round_rectangle2)
          
          402          60 LOAD_NAME                9 (create_round_rectangle2)
                       62 STORE_NAME              10 (create_round_rect2)
          
-         404          64 LOAD_CONST              22 (('black', 'black'))
+         404          64 LOAD_CONST              25 (('black', 'black'))
                       66 LOAD_CONST              12 ('fill')
                       68 LOAD_NAME               11 (str)
                       70 LOAD_CONST              13 ('outline')
                       72 LOAD_NAME               11 (str)
                       74 BUILD_TUPLE              4
                       76 LOAD_CONST              14 (<code object create_round_rectangle3, file "D:\tkadw\tkadw\canvas\drawengine.py", line 404>)
                       78 MAKE_FUNCTION            5 (defaults, annotations)
@@ -192,15 +192,15 @@
          423          86 LOAD_CONST              15 (<code object create_round_rectangle4, file "D:\tkadw\tkadw\canvas\drawengine.py", line 423>)
                       88 MAKE_FUNCTION            0
                       90 STORE_NAME              14 (create_round_rectangle4)
          
          449          92 LOAD_NAME               14 (create_round_rectangle4)
                       94 STORE_NAME              15 (create_round_rect4)
          
-         451          96 LOAD_CONST              22 (('black', 'black'))
+         451          96 LOAD_CONST              25 (('black', 'black'))
                       98 LOAD_CONST              16 (<code object polygon_round, file "D:\tkadw\tkadw\canvas\drawengine.py", line 451>)
                      100 MAKE_FUNCTION            1 (defaults)
                      102 STORE_NAME              16 (polygon_round)
          
          457         104 LOAD_NAME               16 (polygon_round)
                      106 STORE_NAME              17 (poly_round)
          
@@ -210,18 +210,23 @@
          
          567         114 LOAD_CONST              18 ('content')
                      116 LOAD_NAME               11 (str)
                      118 BUILD_TUPLE              2
                      120 LOAD_CONST              19 (<code object create_svg_image, file "D:\tkadw\tkadw\canvas\drawengine.py", line 567>)
                      122 MAKE_FUNCTION            4 (annotations)
                      124 STORE_NAME              19 (create_svg_image)
-                     126 LOAD_CLOSURE             0 (__class__)
-                     128 COPY                     1
-                     130 STORE_NAME              20 (__classcell__)
-                     132 RETURN_VALUE
+         
+         582         126 LOAD_CONST              26 ((10, 10, 18))
+                     128 LOAD_CONST              22 (<code object draw_copy_icon, file "D:\tkadw\tkadw\canvas\drawengine.py", line 582>)
+                     130 MAKE_FUNCTION            1 (defaults)
+                     132 STORE_NAME              20 (draw_copy_icon)
+                     134 LOAD_CLOSURE             0 (__class__)
+                     136 COPY                     1
+                     138 STORE_NAME              21 (__classcell__)
+                     140 RETURN_VALUE
          consts
             'AdwDrawEngine'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
@@ -1331,27 +1336,190 @@
                varnames   ('self', 'x', 'y', 'content', 'kwargs', 'mkstemp', 'SvgImage', '_', 'file', 'f', 'image', 'i')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
                name       'create_svg_image'
                firstlineno 567
                lnotab 0x02010c010c021e011e0122012a0128fe2e0318022202
+            10
+            18
+            code
+               argcount  : 6
+               nlocals   : 10
+               stacksize : 8
+               flags     : 3
+               code
+                  0x97007c00a00000000000000000000000000000000000000000007c017c
+                  027c017c0364017a0500007a0000007c027c0364017a0500007a0000007c
+                  05a6050000ab0500000000000000007d067c00a000000000000000000000
+                  00000000000000000000007c017c047a0000007c027c047a0000007c017c
+                  0364017a0500007a0000007c047a0a00007c027c0364017a0500007a0000
+                  007c047a0a00007c0564027a0b00006403ac04a6060000ab060000000000
+                  0000007d077c00a00000000000000000000000000000000000000000007c
+                  017c0364027a0500007a0000007c027c0364027a0500007a0000007c017c
+                  0364057a0500007a0000007c027c0364057a0500007a0000007c05a60500
+                  00ab0500000000000000007d087c00a00000000000000000000000000000
+                  000000000000007c017c0364027a0500007a0000007c047a0000007c027c
+                  0364027a0500007a0000007c047a0000007c017c0364057a0500007a0000
+                  007c047a0a00007c027c0364057a0500007a0000007c047a0a00007c0564
+                  027a0b00006403ac04a6060000ab0600000000000000007d097c067c077c
+                  087c0966045300
+               582           0 RESUME                   0
+               
+               583           2 LOAD_FAST                0 (self)
+                             4 LOAD_METHOD              0 (create_round_rect4)
+                            26 LOAD_FAST                1 (_AdwDrawEngine__x)
+                            28 LOAD_FAST                2 (_AdwDrawEngine__y)
+                            30 LOAD_FAST                1 (_AdwDrawEngine__x)
+                            32 LOAD_FAST                3 (size)
+                            34 LOAD_CONST               1 (5)
+                            36 BINARY_OP                5 (*)
+                            40 BINARY_OP                0 (+)
+                            44 LOAD_FAST                2 (_AdwDrawEngine__y)
+                            46 LOAD_FAST                3 (size)
+                            48 LOAD_CONST               1 (5)
+                            50 BINARY_OP                5 (*)
+                            54 BINARY_OP                0 (+)
+                            58 LOAD_FAST                5 (radius)
+                            60 PRECALL                  5
+                            64 CALL                     5
+                            74 STORE_FAST               6 (_1)
+               
+               584          76 LOAD_FAST                0 (self)
+                            78 LOAD_METHOD              0 (create_round_rect4)
+                           100 LOAD_FAST                1 (_AdwDrawEngine__x)
+                           102 LOAD_FAST                4 (padding)
+                           104 BINARY_OP                0 (+)
+                           108 LOAD_FAST                2 (_AdwDrawEngine__y)
+                           110 LOAD_FAST                4 (padding)
+                           112 BINARY_OP                0 (+)
+                           116 LOAD_FAST                1 (_AdwDrawEngine__x)
+                           118 LOAD_FAST                3 (size)
+                           120 LOAD_CONST               1 (5)
+                           122 BINARY_OP                5 (*)
+                           126 BINARY_OP                0 (+)
+                           130 LOAD_FAST                4 (padding)
+                           132 BINARY_OP               10 (-)
+                           136 LOAD_FAST                2 (_AdwDrawEngine__y)
+                           138 LOAD_FAST                3 (size)
+                           140 LOAD_CONST               1 (5)
+                           142 BINARY_OP                5 (*)
+                           146 BINARY_OP                0 (+)
+                           150 LOAD_FAST                4 (padding)
+                           152 BINARY_OP               10 (-)
+                           156 LOAD_FAST                5 (radius)
+                           158 LOAD_CONST               2 (2)
+                           160 BINARY_OP               11 (/)
+                           164 LOAD_CONST               3 ('white')
+                           166 KW_NAMES                 4
+                           168 PRECALL                  6
+                           172 CALL                     6
+                           182 STORE_FAST               7 (_2)
+               
+               585         184 LOAD_FAST                0 (self)
+                           186 LOAD_METHOD              0 (create_round_rect4)
+                           208 LOAD_FAST                1 (_AdwDrawEngine__x)
+                           210 LOAD_FAST                3 (size)
+                           212 LOAD_CONST               2 (2)
+                           214 BINARY_OP                5 (*)
+                           218 BINARY_OP                0 (+)
+                           222 LOAD_FAST                2 (_AdwDrawEngine__y)
+                           224 LOAD_FAST                3 (size)
+                           226 LOAD_CONST               2 (2)
+                           228 BINARY_OP                5 (*)
+                           232 BINARY_OP                0 (+)
+                           236 LOAD_FAST                1 (_AdwDrawEngine__x)
+                           238 LOAD_FAST                3 (size)
+                           240 LOAD_CONST               5 (7)
+                           242 BINARY_OP                5 (*)
+                           246 BINARY_OP                0 (+)
+                           250 LOAD_FAST                2 (_AdwDrawEngine__y)
+                           252 LOAD_FAST                3 (size)
+                           254 LOAD_CONST               5 (7)
+                           256 BINARY_OP                5 (*)
+                           260 BINARY_OP                0 (+)
+                           264 LOAD_FAST                5 (radius)
+                           266 PRECALL                  5
+                           270 CALL                     5
+                           280 STORE_FAST               8 (_3)
+               
+               586         282 LOAD_FAST                0 (self)
+                           284 LOAD_METHOD              0 (create_round_rect4)
+                           306 LOAD_FAST                1 (_AdwDrawEngine__x)
+                           308 LOAD_FAST                3 (size)
+                           310 LOAD_CONST               2 (2)
+                           312 BINARY_OP                5 (*)
+                           316 BINARY_OP                0 (+)
+                           320 LOAD_FAST                4 (padding)
+                           322 BINARY_OP                0 (+)
+                           326 LOAD_FAST                2 (_AdwDrawEngine__y)
+                           328 LOAD_FAST                3 (size)
+                           330 LOAD_CONST               2 (2)
+                           332 BINARY_OP                5 (*)
+                           336 BINARY_OP                0 (+)
+                           340 LOAD_FAST                4 (padding)
+                           342 BINARY_OP                0 (+)
+                           346 LOAD_FAST                1 (_AdwDrawEngine__x)
+                           348 LOAD_FAST                3 (size)
+                           350 LOAD_CONST               5 (7)
+                           352 BINARY_OP                5 (*)
+                           356 BINARY_OP                0 (+)
+                           360 LOAD_FAST                4 (padding)
+                           362 BINARY_OP               10 (-)
+                           366 LOAD_FAST                2 (_AdwDrawEngine__y)
+                           368 LOAD_FAST                3 (size)
+                           370 LOAD_CONST               5 (7)
+                           372 BINARY_OP                5 (*)
+                           376 BINARY_OP                0 (+)
+                           380 LOAD_FAST                4 (padding)
+                           382 BINARY_OP               10 (-)
+                           386 LOAD_FAST                5 (radius)
+                           388 LOAD_CONST               2 (2)
+                           390 BINARY_OP               11 (/)
+                           394 LOAD_CONST               3 ('white')
+                           396 KW_NAMES                 4
+                           398 PRECALL                  6
+                           402 CALL                     6
+                           412 STORE_FAST               9 (_4)
+               
+               587         414 LOAD_FAST                6 (_1)
+                           416 LOAD_FAST                7 (_2)
+                           418 LOAD_FAST                8 (_3)
+                           420 LOAD_FAST                9 (_4)
+                           422 BUILD_TUPLE              4
+                           424 RETURN_VALUE
+               consts
+                  None
+                  5
+                  2
+                  'white'
+                  ('fill',)
+                  7
+               names      ('create_round_rect4',)
+               varnames   ('self', '_AdwDrawEngine__x', '_AdwDrawEngine__y', 'size', 'padding', 'radius', '_1', '_2', '_3', '_4')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
+               name       'draw_copy_icon'
+               firstlineno 582
+               lnotab 0x02014a016c0162018401
             ('x',)
             (5, 2, 'white', 'black')
             ('black', 'black')
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'win32_high_dpi', 'draw_gradient', 'float', 'create_round_rectangle', 'create_round_rect', 'create_round_rectangle2', 'create_round_rect2', 'str', 'create_round_rectangle3', 'create_round_rect3', 'create_round_rectangle4', 'create_round_rect4', 'polygon_round', 'poly_round', 'demo_polygon_round', 'create_svg_image', '__classcell__')
+            (10, 10, 18)
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'win32_high_dpi', 'draw_gradient', 'float', 'create_round_rectangle', 'create_round_rect', 'create_round_rectangle2', 'create_round_rect2', 'str', 'create_round_rectangle3', 'create_round_rect3', 'create_round_rectangle4', 'create_round_rect4', 'polygon_round', 'poly_round', 'demo_polygon_round', 'create_svg_image', 'draw_copy_icon', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
          name       'AdwDrawEngine'
          firstlineno 226
          lnotab
             0x0c010a03060408430e1f04020644040212110402061a04020806040206
-            6c
+            6c0c0f
       'AdwDrawEngine'
       '__main__'
       ('Tk',)
       10
       15
       150
       50
@@ -1362,15 +1530,15 @@
          argcount  : 1
          nlocals   : 1
          stacksize : 5
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000640164026403a6030000ab0300000000000000005300
-         593           0 RESUME                   0
+         599           0 RESUME                   0
                        2 LOAD_GLOBAL              0 (canvas)
                       14 LOAD_METHOD              1 (draw_gradient)
                       36 LOAD_CONST               1 ('#87e9bb')
                       38 LOAD_CONST               2 ('#d3a6f5')
                       40 LOAD_CONST               3 ('x')
                       42 PRECALL                  3
                       46 CALL                     3
@@ -1382,23 +1550,23 @@
             'x'
          names      ('canvas', 'draw_gradient')
          varnames   ('event',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
          name       '<lambda>'
-         firstlineno 593
+         firstlineno 599
          lnotab 0x
       'both'
       'yes'
       ('fill', 'expand')
       None
    names      ('tkinter', 'Canvas', 'poly', 'poly2', 'AdwDrawEngine', '__name__', 'Tk', 'root', 'canvas', 'create_round_rect3', 'create_round_rect4', 'bind', 'pack', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c02047f0015044b1c7f007f00670c010c0214021402340132
+      0x00ff02010c02047f0015044b1c7f007f006d0c010c0214021402340132
       022e022e022cf2
```

### Comparing `tkadw-0.1.5/tkadw/canvas/__pycache__/entry.cpython-311.pyc` & `tkadw-0.2.0/tkadw/canvas/__pycache__/entry.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,24 +1,24 @@
 magic:    0xa70d0d0a
-moddate:  0x624e9564 (Fri Jun 23 07:48:50 2023 UTC)
-files sz: 22377
+moddate:  0x174a9664 (Sat Jun 24 01:42:47 2023 UTC)
+files sz: 17356
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
       00020047006403840064046504a6030000ab0300000000000000005a0502
       0047006405840064066505a6030000ab0300000000000000005a06020047
       006407840064086505a6030000ab0300000000000000005a070200470064
       098400640a6505a6030000ab0300000000000000005a0802004700640b84
       00640c6508a6030000ab0300000000000000005a0902004700640d840064
       0e6508a6030000ab0300000000000000005a0a02004700640f8400641065
-      05a6030000ab0300000000000000005a0b02004700641184006412650ba6
+      08a6030000ab0300000000000000005a0b02004700641184006412650ba6
       030000ab0300000000000000005a0c02004700641384006414650ba60300
       00ab0300000000000000005a0d650e64156b020000000072fe640064166c
       0f6d105a10010002006510a6000000ab0000000000000000005a11020065
       066417ac18a6010000ab0100000000000000005a126512a0130000000000
       0000000000000000000000000000006419641a641aac1ba6030000ab0300
       000000000000000100020065076417ac18a6010000ab0100000000000000
       005a146514a0130000000000000000000000000000000000000000641964
@@ -58,229 +58,229 @@
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               4 ('AdwDrawBasicEntry')
                 40 LOAD_NAME                4 (AdwDrawEngine)
                 42 PRECALL                  3
                 46 CALL                     3
                 56 STORE_NAME               5 (AdwDrawBasicEntry)
    
-   210          58 PUSH_NULL
+   211          58 PUSH_NULL
                 60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               5 (<code object AdwDrawEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 210>)
+                62 LOAD_CONST               5 (<code object AdwDrawEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 211>)
                 64 MAKE_FUNCTION            0
                 66 LOAD_CONST               6 ('AdwDrawEntry')
                 68 LOAD_NAME                5 (AdwDrawBasicEntry)
                 70 PRECALL                  3
                 74 CALL                     3
                 84 STORE_NAME               6 (AdwDrawEntry)
    
-   215          86 PUSH_NULL
+   216          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object AdwDrawDarkEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 215>)
+                90 LOAD_CONST               7 (<code object AdwDrawDarkEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 216>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('AdwDrawDarkEntry')
                 96 LOAD_NAME                5 (AdwDrawBasicEntry)
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME               7 (AdwDrawDarkEntry)
    
-   221         114 PUSH_NULL
+   222         114 PUSH_NULL
                116 LOAD_BUILD_CLASS
-               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 221>)
+               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 222>)
                120 MAKE_FUNCTION            0
                122 LOAD_CONST              10 ('AdwDrawBasicRoundEntry')
                124 LOAD_NAME                5 (AdwDrawBasicEntry)
                126 PRECALL                  3
                130 CALL                     3
                140 STORE_NAME               8 (AdwDrawBasicRoundEntry)
    
-   400         142 PUSH_NULL
+   372         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object AdwDrawRoundEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 400>)
+               146 LOAD_CONST              11 (<code object AdwDrawRoundEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 372>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('AdwDrawRoundEntry')
                152 LOAD_NAME                8 (AdwDrawBasicRoundEntry)
                154 PRECALL                  3
                158 CALL                     3
                168 STORE_NAME               9 (AdwDrawRoundEntry)
    
-   405         170 PUSH_NULL
+   377         170 PUSH_NULL
                172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 405>)
+               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 377>)
                176 MAKE_FUNCTION            0
                178 LOAD_CONST              14 ('AdwDrawRoundDarkEntry')
                180 LOAD_NAME                8 (AdwDrawBasicRoundEntry)
                182 PRECALL                  3
                186 CALL                     3
                196 STORE_NAME              10 (AdwDrawRoundDarkEntry)
    
-   410         198 PUSH_NULL
+   382         198 PUSH_NULL
                200 LOAD_BUILD_CLASS
-               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 410>)
+               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 382>)
                204 MAKE_FUNCTION            0
                206 LOAD_CONST              16 ('AdwDrawBasicRoundEntry3')
-               208 LOAD_NAME                5 (AdwDrawBasicEntry)
+               208 LOAD_NAME                8 (AdwDrawBasicRoundEntry)
                210 PRECALL                  3
                214 CALL                     3
                224 STORE_NAME              11 (AdwDrawBasicRoundEntry3)
    
-   594         226 PUSH_NULL
+   476         226 PUSH_NULL
                228 LOAD_BUILD_CLASS
-               230 LOAD_CONST              17 (<code object AdwDrawRoundEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 594>)
+               230 LOAD_CONST              17 (<code object AdwDrawRoundEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 476>)
                232 MAKE_FUNCTION            0
                234 LOAD_CONST              18 ('AdwDrawRoundEntry3')
                236 LOAD_NAME               11 (AdwDrawBasicRoundEntry3)
                238 PRECALL                  3
                242 CALL                     3
                252 STORE_NAME              12 (AdwDrawRoundEntry3)
    
-   599         254 PUSH_NULL
+   481         254 PUSH_NULL
                256 LOAD_BUILD_CLASS
-               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 599>)
+               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 481>)
                260 MAKE_FUNCTION            0
                262 LOAD_CONST              20 ('AdwDrawRoundDarkEntry3')
                264 LOAD_NAME               11 (AdwDrawBasicRoundEntry3)
                266 PRECALL                  3
                270 CALL                     3
                280 STORE_NAME              13 (AdwDrawRoundDarkEntry3)
    
-   604         282 LOAD_NAME               14 (__name__)
+   486         282 LOAD_NAME               14 (__name__)
                284 LOAD_CONST              21 ('__main__')
                286 COMPARE_OP               2 (==)
                292 POP_JUMP_FORWARD_IF_FALSE   254 (to 802)
    
-   605         294 LOAD_CONST               0 (0)
+   487         294 LOAD_CONST               0 (0)
                296 LOAD_CONST              22 (('Tk',))
                298 IMPORT_NAME             15 (tkinter)
                300 IMPORT_FROM             16 (Tk)
                302 STORE_NAME              16 (Tk)
                304 POP_TOP
    
-   607         306 PUSH_NULL
+   489         306 PUSH_NULL
                308 LOAD_NAME               16 (Tk)
                310 PRECALL                  0
                314 CALL                     0
                324 STORE_NAME              17 (root)
    
-   609         326 PUSH_NULL
+   491         326 PUSH_NULL
                328 LOAD_NAME                6 (AdwDrawEntry)
                330 LOAD_CONST              23 ('Hello')
                332 KW_NAMES                24
                334 PRECALL                  1
                338 CALL                     1
                348 STORE_NAME              18 (entry1)
    
-   610         350 LOAD_NAME               18 (entry1)
+   492         350 LOAD_NAME               18 (entry1)
                352 LOAD_METHOD             19 (pack)
                374 LOAD_CONST              25 ('x')
                376 LOAD_CONST              26 (5)
                378 LOAD_CONST              26 (5)
                380 KW_NAMES                27
                382 PRECALL                  3
                386 CALL                     3
                396 POP_TOP
    
-   612         398 PUSH_NULL
+   494         398 PUSH_NULL
                400 LOAD_NAME                7 (AdwDrawDarkEntry)
                402 LOAD_CONST              23 ('Hello')
                404 KW_NAMES                24
                406 PRECALL                  1
                410 CALL                     1
                420 STORE_NAME              20 (entry2)
    
-   613         422 LOAD_NAME               20 (entry2)
+   495         422 LOAD_NAME               20 (entry2)
                424 LOAD_METHOD             19 (pack)
                446 LOAD_CONST              25 ('x')
                448 LOAD_CONST              26 (5)
                450 LOAD_CONST              26 (5)
                452 KW_NAMES                27
                454 PRECALL                  3
                458 CALL                     3
                468 POP_TOP
    
-   615         470 PUSH_NULL
+   497         470 PUSH_NULL
                472 LOAD_NAME                9 (AdwDrawRoundEntry)
                474 LOAD_CONST              23 ('Hello')
                476 KW_NAMES                24
                478 PRECALL                  1
                482 CALL                     1
                492 STORE_NAME              21 (entry3)
    
-   616         494 LOAD_NAME               21 (entry3)
+   498         494 LOAD_NAME               21 (entry3)
                496 LOAD_METHOD             19 (pack)
                518 LOAD_CONST              25 ('x')
                520 LOAD_CONST              26 (5)
                522 LOAD_CONST              26 (5)
                524 KW_NAMES                27
                526 PRECALL                  3
                530 CALL                     3
                540 POP_TOP
    
-   618         542 PUSH_NULL
+   500         542 PUSH_NULL
                544 LOAD_NAME               10 (AdwDrawRoundDarkEntry)
                546 LOAD_CONST              23 ('Hello')
                548 KW_NAMES                24
                550 PRECALL                  1
                554 CALL                     1
                564 STORE_NAME              22 (entry4)
    
-   619         566 LOAD_NAME               22 (entry4)
+   501         566 LOAD_NAME               22 (entry4)
                568 LOAD_METHOD             19 (pack)
                590 LOAD_CONST              25 ('x')
                592 LOAD_CONST              26 (5)
                594 LOAD_CONST              26 (5)
                596 KW_NAMES                27
                598 PRECALL                  3
                602 CALL                     3
                612 POP_TOP
    
-   621         614 PUSH_NULL
+   503         614 PUSH_NULL
                616 LOAD_NAME               12 (AdwDrawRoundEntry3)
                618 LOAD_CONST              23 ('Hello')
                620 KW_NAMES                24
                622 PRECALL                  1
                626 CALL                     1
                636 STORE_NAME              23 (entry5)
    
-   622         638 LOAD_NAME               23 (entry5)
+   504         638 LOAD_NAME               23 (entry5)
                640 LOAD_METHOD             19 (pack)
                662 LOAD_CONST              25 ('x')
                664 LOAD_CONST              26 (5)
                666 LOAD_CONST              26 (5)
                668 KW_NAMES                27
                670 PRECALL                  3
                674 CALL                     3
                684 POP_TOP
    
-   624         686 PUSH_NULL
+   506         686 PUSH_NULL
                688 LOAD_NAME               13 (AdwDrawRoundDarkEntry3)
                690 LOAD_CONST              23 ('Hello')
                692 KW_NAMES                24
                694 PRECALL                  1
                698 CALL                     1
                708 STORE_NAME              24 (entry6)
    
-   625         710 LOAD_NAME               24 (entry6)
+   507         710 LOAD_NAME               24 (entry6)
                712 LOAD_METHOD             19 (pack)
                734 LOAD_CONST              25 ('x')
                736 LOAD_CONST              26 (5)
                738 LOAD_CONST              26 (5)
                740 KW_NAMES                27
                742 PRECALL                  3
                746 CALL                     3
                756 POP_TOP
    
-   627         758 LOAD_NAME               17 (root)
+   509         758 LOAD_NAME               17 (root)
                760 LOAD_METHOD             25 (mainloop)
                782 PRECALL                  0
                786 CALL                     0
                796 POP_TOP
                798 LOAD_CONST              28 (None)
                800 RETURN_VALUE
    
-   604     >>  802 LOAD_CONST              28 (None)
+   486     >>  802 LOAD_CONST              28 (None)
                804 RETURN_VALUE
    consts
       0
       ('Font', 'nametofont')
       ('AdwDrawEngine',)
       code
          argcount  : 0
@@ -372,20 +372,20 @@
                      124 MAKE_FUNCTION            0
                      126 STORE_NAME              16 (default_palette)
          
          125         128 LOAD_CONST              20 (<code object palette_light, file "D:\tkadw\tkadw\canvas\entry.py", line 125>)
                      130 MAKE_FUNCTION            0
                      132 STORE_NAME              17 (palette_light)
          
-         147         134 LOAD_CONST              21 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\entry.py", line 147>)
+         152         134 LOAD_CONST              21 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\entry.py", line 152>)
                      136 MAKE_FUNCTION            0
                      138 STORE_NAME              18 (palette_dark)
          
-         169         140 LOAD_CONST              23 ((None,))
-                     142 LOAD_CONST              22 (<code object palette, file "D:\tkadw\tkadw\canvas\entry.py", line 169>)
+         179         140 LOAD_CONST              23 ((None,))
+                     142 LOAD_CONST              22 (<code object palette, file "D:\tkadw\tkadw\canvas\entry.py", line 179>)
                      144 MAKE_FUNCTION            1 (defaults)
                      146 STORE_NAME              19 (palette)
                      148 LOAD_CLOSURE             0 (__class__)
                      150 COPY                     1
                      152 STORE_NAME              20 (__classcell__)
                      154 RETURN_VALUE
          consts
@@ -1296,589 +1296,627 @@
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
                firstlineno 122
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 16
+               stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564066407640564086409640a640b640c640d9c0da60100
-                  00ab010000000000000000010064005300
+                  0264036404640564066404640764086409640a6406640b640c640d9c0664
+                  0e9c086901a6010000ab010000000000000000010064005300
                125           0 RESUME                   0
                
                126           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               128          26 LOAD_CONST               1 ((3, 4))
+               128          26 LOAD_CONST               1 ('entry')
+               
+               129          28 LOAD_CONST               2 ((3, 4))
+               
+               131          30 LOAD_CONST               3 ('#fdfdfd')
                
-               130          28 LOAD_CONST               2 ('#f3f3f3')
+               132          32 LOAD_CONST               4 ('#eaeaea')
                
-               131          30 LOAD_CONST               3 (1)
+               133          34 LOAD_CONST               5 ('#5f5f5f')
                
-               132          32 LOAD_CONST               4 (0)
+               134          36 LOAD_CONST               6 (1)
                
-               134          34 LOAD_CONST               5 ('#eaeaea')
+               136          38 LOAD_CONST               4 ('#eaeaea')
                
-               135          36 LOAD_CONST               6 ('#fdfdfd')
+               137          40 LOAD_CONST               7 (0)
                
-               136          38 LOAD_CONST               7 ('#5f5f5f')
+               140          42 LOAD_CONST               8 ('#f9f9f9')
                
-               137          40 LOAD_CONST               5 ('#eaeaea')
+               141          44 LOAD_CONST               9 ('#e2e2e2')
                
-               139          42 LOAD_CONST               8 ('#e2e2e2')
+               142          46 LOAD_CONST              10 ('#1a1a1a')
                
-               140          44 LOAD_CONST               9 ('#f9f9f9')
+               143          48 LOAD_CONST               6 (1)
                
-               141          46 LOAD_CONST              10 ('#1a1a1a')
+               145          50 LOAD_CONST              11 ('#185fb4')
                
-               142          48 LOAD_CONST              11 ('#185fb4')
+               146          52 LOAD_CONST              12 (2)
                
-               143          50 LOAD_CONST              12 (2)
+               139          54 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                            56 BUILD_CONST_KEY_MAP      6
                
-               127          52 LOAD_CONST              13 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
-                            54 BUILD_CONST_KEY_MAP     13
+               128          58 LOAD_CONST              14 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                            60 BUILD_CONST_KEY_MAP      8
                
-               126          56 PRECALL                  1
-                            60 CALL                     1
-                            70 POP_TOP
-                            72 LOAD_CONST               0 (None)
-                            74 RETURN_VALUE
+               127          62 BUILD_MAP                1
+               
+               126          64 PRECALL                  1
+                            68 CALL                     1
+                            78 POP_TOP
+                            80 LOAD_CONST               0 (None)
+                            82 RETURN_VALUE
                consts
                   None
+                  'entry'
                   (3, 4)
-                  '#f3f3f3'
-                  1
-                  0
-                  '#eaeaea'
                   '#fdfdfd'
+                  '#eaeaea'
                   '#5f5f5f'
-                  '#e2e2e2'
+                  1
+                  0
                   '#f9f9f9'
+                  '#e2e2e2'
                   '#1a1a1a'
                   '#185fb4'
                   2
-                  ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
+                  ('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width')
+                  ('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette_light'
                firstlineno 125
                lnotab
-                  0x0201180202020201020102020201020102010202020102010201020102
-                  f004ff
+                  0x0201180202010202020102010201020202010203020102010201020202
+                  0102f904f504ff02ff
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 16
+               stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  02640364046405640664076408640464096407640a640b640c9c0da60100
-                  00ab010000000000000000010064005300
-               147           0 RESUME                   0
+                  026403640464056406640764086409640464076406640a640b640c9c0664
+                  0d9c086901a6010000ab010000000000000000010064005300
+               152           0 RESUME                   0
                
-               148           2 LOAD_FAST                0 (self)
+               153           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               150          26 LOAD_CONST               1 ((3, 4))
+               155          26 LOAD_CONST               1 ('entry')
+               
+               156          28 LOAD_CONST               2 ((3, 4))
+               
+               158          30 LOAD_CONST               3 ('#353535')
                
-               152          28 LOAD_CONST               2 ('#202020')
+               159          32 LOAD_CONST               4 ('#454545')
                
-               153          30 LOAD_CONST               3 (1)
+               160          34 LOAD_CONST               5 ('#cecece')
                
-               155          32 LOAD_CONST               4 ('#454545')
+               161          36 LOAD_CONST               6 (1)
                
-               156          34 LOAD_CONST               5 ('#353535')
+               163          38 LOAD_CONST               7 ('#ffffff')
                
-               157          36 LOAD_CONST               6 ('#cecece')
+               164          40 LOAD_CONST               8 (0)
                
-               158          38 LOAD_CONST               7 ('#ffffff')
+               167          42 LOAD_CONST               9 ('#2f2f2f')
                
-               159          40 LOAD_CONST               8 (0)
+               168          44 LOAD_CONST               4 ('#454545')
                
-               161          42 LOAD_CONST               4 ('#454545')
+               169          46 LOAD_CONST               7 ('#ffffff')
                
-               162          44 LOAD_CONST               9 ('#2f2f2f')
+               170          48 LOAD_CONST               6 (1)
                
-               163          46 LOAD_CONST               7 ('#ffffff')
+               172          50 LOAD_CONST              10 ('#4cc2ff')
                
-               164          48 LOAD_CONST              10 ('#4cc2ff')
+               173          52 LOAD_CONST              11 (2)
                
-               165          50 LOAD_CONST              11 (2)
+               166          54 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                            56 BUILD_CONST_KEY_MAP      6
                
-               149          52 LOAD_CONST              12 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
-                            54 BUILD_CONST_KEY_MAP     13
+               155          58 LOAD_CONST              13 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                            60 BUILD_CONST_KEY_MAP      8
                
-               148          56 PRECALL                  1
-                            60 CALL                     1
-                            70 POP_TOP
-                            72 LOAD_CONST               0 (None)
-                            74 RETURN_VALUE
+               154          62 BUILD_MAP                1
+               
+               153          64 PRECALL                  1
+                            68 CALL                     1
+                            78 POP_TOP
+                            80 LOAD_CONST               0 (None)
+                            82 RETURN_VALUE
                consts
                   None
+                  'entry'
                   (3, 4)
-                  '#202020'
-                  1
-                  '#454545'
                   '#353535'
+                  '#454545'
                   '#cecece'
+                  1
                   '#ffffff'
                   0
                   '#2f2f2f'
                   '#4cc2ff'
                   2
-                  ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
+                  ('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width')
+                  ('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette_dark'
-               firstlineno 147
+               firstlineno 152
                lnotab
-                  0x0201180202020201020202010201020102010202020102010201020102
-                  f004ff
+                  0x0201180202010202020102010201020202010203020102010201020202
+                  0102f904f504ff02ff
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 11
+               stacksize : 4
                flags     : 3
                code
-                  0x97007c0181d27c016401190000000000000000007c005f000000000000
-                  0000007c016402190000000000000000007c005f0100000000000000007c
-                  016403190000000000000000007c005f0200000000000000007c01640419
-                  0000000000000000007c005f0300000000000000007c0164051900000000
-                  00000000007c005f0400000000000000007c016406190000000000000000
-                  007c005f0500000000000000007c016407190000000000000000007c005f
-                  0600000000000000007c016408190000000000000000007c005f07000000
-                  00000000007c016409190000000000000000007c005f0800000000000000
-                  007c01640a190000000000000000007c005f0900000000000000007c0164
-                  0b190000000000000000007c005f0a00000000000000007c01640c190000
-                  000000000000007c005f0b00000000000000007c01640d19000000000000
-                  0000007c005f0c000000000000000009007c00a00d000000000000000000
-                  00000000000000000000006400a6010000ab010000000000000000010064
-                  0053002300741c0000000000000000000024007204010059006400530077
-                  007803590077017c006a0000000000000000007c006a0100000000000000
-                  007c006a0200000000000000007c006a0700000000000000007c006a0300
-                  000000000000007c006a0400000000000000007c006a0500000000000000
-                  007c006a0800000000000000007c006a0900000000000000007c006a0a00
-                  00000000000000640e9c0a5300
-               169           0 RESUME                   0
-               
-               170           2 LOAD_FAST                1 (dict)
-                             4 POP_JUMP_FORWARD_IF_NONE   210 (to 426)
-               
-               171           6 LOAD_FAST                1 (dict)
-                             8 LOAD_CONST               1 ('entry_padding')
-                            10 BINARY_SUBSCR
-                            20 LOAD_FAST                0 (self)
-                            22 STORE_ATTR               0 (entry_padding)
-               
-               173          32 LOAD_FAST                1 (dict)
-                            34 LOAD_CONST               2 ('entry_frame_back')
-                            36 BINARY_SUBSCR
-                            46 LOAD_FAST                0 (self)
-                            48 STORE_ATTR               1 (entry_frame_back)
-               
-               174          58 LOAD_FAST                1 (dict)
-                            60 LOAD_CONST               3 ('entry_border_width')
-                            62 BINARY_SUBSCR
-                            72 LOAD_FAST                0 (self)
-                            74 STORE_ATTR               2 (entry_border_width)
+                  0x97007c019001815a64017c017600900172257c01640119000000000000
+                  0000006402190000000000000000007c005f0000000000000000007c0164
+                  01190000000000000000006403190000000000000000007c005f01000000
+                  00000000007c016401190000000000000000006404190000000000000000
+                  007c005f0200000000000000007c01640119000000000000000000640519
+                  0000000000000000007c005f0300000000000000007c0164011900000000
+                  00000000006406190000000000000000007c005f0400000000000000007c
+                  016401190000000000000000006407190000000000000000007c005f0500
+                  000000000000007c01640119000000000000000000640819000000000000
+                  0000007c005f06000000000000000064097c016401190000000000000000
+                  00760072967c016401190000000000000000006409190000000000000000
+                  006403190000000000000000007c005f0700000000000000007c01640119
+                  000000000000000000640919000000000000000000640419000000000000
+                  0000007c005f0800000000000000007c0164011900000000000000000064
+                  09190000000000000000006405190000000000000000007c005f09000000
+                  00000000007c016401190000000000000000006409190000000000000000
+                  006406190000000000000000007c005f0a00000000000000007c01640119
+                  000000000000000000640919000000000000000000640719000000000000
+                  0000007c005f0b00000000000000007c0164011900000000000000000064
+                  09190000000000000000006408190000000000000000007c005f0c000000
+                  00000000007c017c005f0d000000000000000009007c00a00e0000000000
+                  0000000000000000000000000000006400a6010000ab0100000000000000
+                  000100640053002300741e00000000000000000000240072040100590064
+                  00530077007803590077017c006a0d00000000000000005300
+               179           0 RESUME                   0
+               
+               180           2 LOAD_FAST                1 (dict)
+                             4 EXTENDED_ARG             1
+                             6 POP_JUMP_FORWARD_IF_NONE   346 (to 700)
+               
+               181           8 LOAD_CONST               1 ('entry')
+                            10 LOAD_FAST                1 (dict)
+                            12 CONTAINS_OP              0
+                            14 EXTENDED_ARG             1
+                            16 POP_JUMP_FORWARD_IF_FALSE   293 (to 604)
+               
+               182          18 LOAD_FAST                1 (dict)
+                            20 LOAD_CONST               1 ('entry')
+                            22 BINARY_SUBSCR
+                            32 LOAD_CONST               2 ('padding')
+                            34 BINARY_SUBSCR
+                            44 LOAD_FAST                0 (self)
+                            46 STORE_ATTR               0 (entry_padding)
                
-               176          84 LOAD_FAST                1 (dict)
-                            86 LOAD_CONST               4 ('entry_border')
-                            88 BINARY_SUBSCR
-                            98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               3 (entry_border)
-               
-               177         110 LOAD_FAST                1 (dict)
-                           112 LOAD_CONST               5 ('entry_back')
-                           114 BINARY_SUBSCR
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               4 (entry_back)
-               
-               178         136 LOAD_FAST                1 (dict)
-                           138 LOAD_CONST               6 ('entry_text_back')
-                           140 BINARY_SUBSCR
-                           150 LOAD_FAST                0 (self)
-                           152 STORE_ATTR               5 (entry_text_back)
-               
-               179         162 LOAD_FAST                1 (dict)
-                           164 LOAD_CONST               7 ('entry_bottom_line')
-                           166 BINARY_SUBSCR
-                           176 LOAD_FAST                0 (self)
-                           178 STORE_ATTR               6 (entry_bottom_line)
-               
-               180         188 LOAD_FAST                1 (dict)
-                           190 LOAD_CONST               8 ('entry_bottom_width')
-                           192 BINARY_SUBSCR
-                           202 LOAD_FAST                0 (self)
-                           204 STORE_ATTR               7 (entry_bottom_width)
-               
-               182         214 LOAD_FAST                1 (dict)
-                           216 LOAD_CONST               9 ('entry_focusin_border')
-                           218 BINARY_SUBSCR
-                           228 LOAD_FAST                0 (self)
-                           230 STORE_ATTR               8 (entry_focusin_border)
+               184          56 LOAD_FAST                1 (dict)
+                            58 LOAD_CONST               1 ('entry')
+                            60 BINARY_SUBSCR
+                            70 LOAD_CONST               3 ('back')
+                            72 BINARY_SUBSCR
+                            82 LOAD_FAST                0 (self)
+                            84 STORE_ATTR               1 (entry_back)
+               
+               185          94 LOAD_FAST                1 (dict)
+                            96 LOAD_CONST               1 ('entry')
+                            98 BINARY_SUBSCR
+                           108 LOAD_CONST               4 ('border')
+                           110 BINARY_SUBSCR
+                           120 LOAD_FAST                0 (self)
+                           122 STORE_ATTR               2 (entry_border)
+               
+               186         132 LOAD_FAST                1 (dict)
+                           134 LOAD_CONST               1 ('entry')
+                           136 BINARY_SUBSCR
+                           146 LOAD_CONST               5 ('text_back')
+                           148 BINARY_SUBSCR
+                           158 LOAD_FAST                0 (self)
+                           160 STORE_ATTR               3 (entry_text_back)
+               
+               187         170 LOAD_FAST                1 (dict)
+                           172 LOAD_CONST               1 ('entry')
+                           174 BINARY_SUBSCR
+                           184 LOAD_CONST               6 ('border_width')
+                           186 BINARY_SUBSCR
+                           196 LOAD_FAST                0 (self)
+                           198 STORE_ATTR               4 (entry_border_width)
                
-               183         240 LOAD_FAST                1 (dict)
-                           242 LOAD_CONST              10 ('entry_focusin_back')
-                           244 BINARY_SUBSCR
-                           254 LOAD_FAST                0 (self)
-                           256 STORE_ATTR               9 (entry_focusin_back)
-               
-               184         266 LOAD_FAST                1 (dict)
-                           268 LOAD_CONST              11 ('entry_focusin_text_back')
-                           270 BINARY_SUBSCR
-                           280 LOAD_FAST                0 (self)
-                           282 STORE_ATTR              10 (entry_focusin_text_back)
-               
-               185         292 LOAD_FAST                1 (dict)
-                           294 LOAD_CONST              12 ('entry_focusin_bottom_line')
-                           296 BINARY_SUBSCR
-                           306 LOAD_FAST                0 (self)
-                           308 STORE_ATTR              11 (entry_focusin_bottom_line)
-               
-               186         318 LOAD_FAST                1 (dict)
-                           320 LOAD_CONST              13 ('entry_focusin_bottom_width')
-                           322 BINARY_SUBSCR
-                           332 LOAD_FAST                0 (self)
-                           334 STORE_ATTR              12 (entry_focusin_bottom_width)
-               
-               188         344 NOP
-               
-               189         346 LOAD_FAST                0 (self)
-                           348 LOAD_METHOD             13 (_draw)
-                           370 LOAD_CONST               0 (None)
-                           372 PRECALL                  1
-                           376 CALL                     1
-                           386 POP_TOP
-                           388 LOAD_CONST               0 (None)
-                           390 RETURN_VALUE
-                       >>  392 PUSH_EXC_INFO
-               
-               190         394 LOAD_GLOBAL             28 (AttributeError)
-                           406 CHECK_EXC_MATCH
-                           408 POP_JUMP_FORWARD_IF_FALSE     4 (to 418)
-                           410 POP_TOP
-               
-               191         412 POP_EXCEPT
-                           414 LOAD_CONST               0 (None)
-                           416 RETURN_VALUE
-               
-               190     >>  418 RERAISE                  0
-                       >>  420 COPY                     3
-                           422 POP_EXCEPT
-                           424 RERAISE                  1
-               
-               194     >>  426 LOAD_FAST                0 (self)
-                           428 LOAD_ATTR                0 (entry_padding)
-               
-               196         438 LOAD_FAST                0 (self)
-                           440 LOAD_ATTR                1 (entry_frame_back)
-               
-               197         450 LOAD_FAST                0 (self)
-                           452 LOAD_ATTR                2 (entry_border_width)
-               
-               198         462 LOAD_FAST                0 (self)
-                           464 LOAD_ATTR                7 (entry_bottom_width)
-               
-               200         474 LOAD_FAST                0 (self)
-                           476 LOAD_ATTR                3 (entry_border)
-               
-               201         486 LOAD_FAST                0 (self)
-                           488 LOAD_ATTR                4 (entry_back)
-               
-               202         498 LOAD_FAST                0 (self)
-                           500 LOAD_ATTR                5 (entry_text_back)
-               
-               204         510 LOAD_FAST                0 (self)
-                           512 LOAD_ATTR                8 (entry_focusin_border)
-               
-               205         522 LOAD_FAST                0 (self)
-                           524 LOAD_ATTR                9 (entry_focusin_back)
-               
-               206         534 LOAD_FAST                0 (self)
-                           536 LOAD_ATTR               10 (entry_focusin_text_back)
-               
-               193         546 LOAD_CONST              14 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back'))
-                           548 BUILD_CONST_KEY_MAP     10
-                           550 RETURN_VALUE
+               189         208 LOAD_FAST                1 (dict)
+                           210 LOAD_CONST               1 ('entry')
+                           212 BINARY_SUBSCR
+                           222 LOAD_CONST               7 ('bottom_line')
+                           224 BINARY_SUBSCR
+                           234 LOAD_FAST                0 (self)
+                           236 STORE_ATTR               5 (entry_bottom_line)
+               
+               190         246 LOAD_FAST                1 (dict)
+                           248 LOAD_CONST               1 ('entry')
+                           250 BINARY_SUBSCR
+                           260 LOAD_CONST               8 ('bottom_width')
+                           262 BINARY_SUBSCR
+                           272 LOAD_FAST                0 (self)
+                           274 STORE_ATTR               6 (entry_bottom_width)
+               
+               192         284 LOAD_CONST               9 ('focusin')
+                           286 LOAD_FAST                1 (dict)
+                           288 LOAD_CONST               1 ('entry')
+                           290 BINARY_SUBSCR
+                           300 CONTAINS_OP              0
+                           302 POP_JUMP_FORWARD_IF_FALSE   150 (to 604)
+               
+               193         304 LOAD_FAST                1 (dict)
+                           306 LOAD_CONST               1 ('entry')
+                           308 BINARY_SUBSCR
+                           318 LOAD_CONST               9 ('focusin')
+                           320 BINARY_SUBSCR
+                           330 LOAD_CONST               3 ('back')
+                           332 BINARY_SUBSCR
+                           342 LOAD_FAST                0 (self)
+                           344 STORE_ATTR               7 (entry_focusin_back)
+               
+               194         354 LOAD_FAST                1 (dict)
+                           356 LOAD_CONST               1 ('entry')
+                           358 BINARY_SUBSCR
+                           368 LOAD_CONST               9 ('focusin')
+                           370 BINARY_SUBSCR
+                           380 LOAD_CONST               4 ('border')
+                           382 BINARY_SUBSCR
+                           392 LOAD_FAST                0 (self)
+                           394 STORE_ATTR               8 (entry_focusin_border)
+               
+               195         404 LOAD_FAST                1 (dict)
+                           406 LOAD_CONST               1 ('entry')
+                           408 BINARY_SUBSCR
+                           418 LOAD_CONST               9 ('focusin')
+                           420 BINARY_SUBSCR
+                           430 LOAD_CONST               5 ('text_back')
+                           432 BINARY_SUBSCR
+                           442 LOAD_FAST                0 (self)
+                           444 STORE_ATTR               9 (entry_focusin_text_back)
+               
+               196         454 LOAD_FAST                1 (dict)
+                           456 LOAD_CONST               1 ('entry')
+                           458 BINARY_SUBSCR
+                           468 LOAD_CONST               9 ('focusin')
+                           470 BINARY_SUBSCR
+                           480 LOAD_CONST               6 ('border_width')
+                           482 BINARY_SUBSCR
+                           492 LOAD_FAST                0 (self)
+                           494 STORE_ATTR              10 (entry_focusin_border_width)
+               
+               198         504 LOAD_FAST                1 (dict)
+                           506 LOAD_CONST               1 ('entry')
+                           508 BINARY_SUBSCR
+                           518 LOAD_CONST               9 ('focusin')
+                           520 BINARY_SUBSCR
+                           530 LOAD_CONST               7 ('bottom_line')
+                           532 BINARY_SUBSCR
+                           542 LOAD_FAST                0 (self)
+                           544 STORE_ATTR              11 (entry_focusin_bottom_line)
+               
+               199         554 LOAD_FAST                1 (dict)
+                           556 LOAD_CONST               1 ('entry')
+                           558 BINARY_SUBSCR
+                           568 LOAD_CONST               9 ('focusin')
+                           570 BINARY_SUBSCR
+                           580 LOAD_CONST               8 ('bottom_width')
+                           582 BINARY_SUBSCR
+                           592 LOAD_FAST                0 (self)
+                           594 STORE_ATTR              12 (entry_focusin_bottom_width)
+               
+               201     >>  604 LOAD_FAST                1 (dict)
+                           606 LOAD_FAST                0 (self)
+                           608 STORE_ATTR              13 (_palette)
+               
+               203         618 NOP
+               
+               204         620 LOAD_FAST                0 (self)
+                           622 LOAD_METHOD             14 (_draw)
+                           644 LOAD_CONST               0 (None)
+                           646 PRECALL                  1
+                           650 CALL                     1
+                           660 POP_TOP
+                           662 LOAD_CONST               0 (None)
+                           664 RETURN_VALUE
+                       >>  666 PUSH_EXC_INFO
+               
+               205         668 LOAD_GLOBAL             30 (AttributeError)
+                           680 CHECK_EXC_MATCH
+                           682 POP_JUMP_FORWARD_IF_FALSE     4 (to 692)
+                           684 POP_TOP
+               
+               206         686 POP_EXCEPT
+                           688 LOAD_CONST               0 (None)
+                           690 RETURN_VALUE
+               
+               205     >>  692 RERAISE                  0
+                       >>  694 COPY                     3
+                           696 POP_EXCEPT
+                           698 RERAISE                  1
+               
+               208     >>  700 LOAD_FAST                0 (self)
+                           702 LOAD_ATTR               13 (_palette)
+                           712 RETURN_VALUE
                ExceptionTable:
-                 346 to 386 -> 392 [0]
-                 392 to 410 -> 420 [1] lasti
-                 418 to 418 -> 420 [1] lasti
-               consts
-                  None
-                  'entry_padding'
-                  'entry_frame_back'
-                  'entry_border_width'
-                  'entry_border'
-                  'entry_back'
-                  'entry_text_back'
-                  'entry_bottom_line'
-                  'entry_bottom_width'
-                  'entry_focusin_border'
-                  'entry_focusin_back'
-                  'entry_focusin_text_back'
-                  'entry_focusin_bottom_line'
-                  'entry_focusin_bottom_width'
-                  ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back')
-               names      ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width', '_draw', 'AttributeError')
+                 620 to 660 -> 666 [0]
+                 666 to 684 -> 694 [1] lasti
+                 692 to 692 -> 694 [1] lasti
+               consts
+                  None
+                  'entry'
+                  'padding'
+                  'back'
+                  'border'
+                  'text_back'
+                  'border_width'
+                  'bottom_line'
+                  'bottom_width'
+                  'focusin'
+               names      ('entry_padding', 'entry_back', 'entry_border', 'entry_text_back', 'entry_border_width', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_back', 'entry_focusin_border', 'entry_focusin_text_back', 'entry_focusin_border_width', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width', '_palette', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette'
-               firstlineno 169
+               firstlineno 179
                lnotab
-                  0x020104011a021a011a021a011a011a011a011a021a011a011a011a011a
-                  0202013001120106ff08040c020c010c010c020c010c010c020c010c010c
-                  f3
+                  0x020106010a012602260126012601260226012602140132013201320132
+                  02320132020e0202013001120106ff0803
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'set', 'get', '_other', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawBasicEntry'
          firstlineno 6
          lnotab
-            0x0c011a240c0306030604061c0809080908030803080b0e060603061606
-            16
+            0x0c011a240c0306030604061c0809080908030803080b0e060603061b06
+            1b
       'AdwDrawBasicEntry'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         210           0 RESUME                   0
+         211           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawEntry')
                        8 STORE_NAME               2 (__qualname__)
          
-         211          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 211>)
+         212          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 212>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawEntry'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               211           0 RESUME                   0
+               212           0 RESUME                   0
                
-               212           2 LOAD_FAST                0 (self)
+               213           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 211
+               firstlineno 212
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawEntry'
-         firstlineno 210
+         firstlineno 211
          lnotab 0x0a01
       'AdwDrawEntry'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         215           0 RESUME                   0
+         216           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkEntry')
                        8 STORE_NAME               2 (__qualname__)
          
-         216          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 216>)
+         217          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 217>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkEntry'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               216           0 RESUME                   0
+               217           0 RESUME                   0
                
-               217           2 LOAD_FAST                0 (self)
+               218           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 216
+               firstlineno 217
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawDarkEntry'
-         firstlineno 215
+         firstlineno 216
          lnotab 0x0a01
       'AdwDrawDarkEntry'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 4
+         stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
-            126404650565067a0700006602640584055a07640684005a086412640784
-            015a096412640884015a0a6412640984015a0b6412640a84015a0c641264
-            0b84015a0d6412640c650e6602640d84055a0f640e84005a10640f84005a
-            11641084005a126412641184015a13880078015a145300
+            11640484015a05640584005a066411640684015a076411640784015a0864
+            11640884015a096411640984015a0a6411640a84015a0b6411640b650c66
+            02640c84055a0d640d84005a0e640e84005a0f640f84005a106411880066
+            01641084095a11880078015a125300
                        0 MAKE_CELL                0 (__class__)
          
-         221           2 RESUME                   0
+         222           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundEntry')
                       10 STORE_NAME               2 (__qualname__)
          
-         222          12 LOAD_CLOSURE             0 (__class__)
+         223          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\entry.py", line 222>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\entry.py", line 223>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         225          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\entry.py", line 225>)
+         226          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\entry.py", line 226>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         229          28 LOAD_CONST              18 ((None,))
-                      30 LOAD_CONST               4 ('radius')
-                      32 LOAD_NAME                5 (float)
-                      34 LOAD_NAME                6 (int)
-                      36 BINARY_OP                7 (|)
-                      40 BUILD_TUPLE              2
-                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\entry.py", line 229>)
-                      44 MAKE_FUNCTION            5 (defaults, annotations)
-                      46 STORE_NAME               7 (border_radius)
-         
-         235          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\entry.py", line 235>)
-                      50 MAKE_FUNCTION            0
-                      52 STORE_NAME               8 (_draw)
-         
-         265          54 LOAD_CONST              18 ((None,))
-                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\entry.py", line 265>)
-                      58 MAKE_FUNCTION            1 (defaults)
-                      60 STORE_NAME               9 (_focus)
-         
-         274          62 LOAD_CONST              18 ((None,))
-                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\entry.py", line 274>)
-                      66 MAKE_FUNCTION            1 (defaults)
-                      68 STORE_NAME              10 (_focusout)
-         
-         283          70 LOAD_CONST              18 ((None,))
-                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\entry.py", line 283>)
-                      74 MAKE_FUNCTION            1 (defaults)
-                      76 STORE_NAME              11 (_click)
-         
-         286          78 LOAD_CONST              18 ((None,))
-                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\entry.py", line 286>)
-                      82 MAKE_FUNCTION            1 (defaults)
-                      84 STORE_NAME              12 (_hover)
-         
-         289          86 LOAD_CONST              18 ((None,))
-                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\entry.py", line 289>)
-                      90 MAKE_FUNCTION            1 (defaults)
-                      92 STORE_NAME              13 (_hover_release)
-         
-         300          94 LOAD_CONST              18 ((None,))
-                      96 LOAD_CONST              12 ('font')
-                      98 LOAD_NAME               14 (Font)
-                     100 BUILD_TUPLE              2
-                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\entry.py", line 300>)
-                     104 MAKE_FUNCTION            5 (defaults, annotations)
-                     106 STORE_NAME              15 (font)
+         230          28 LOAD_CONST              17 ((None,))
+                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\canvas\entry.py", line 230>)
+                      32 MAKE_FUNCTION            1 (defaults)
+                      34 STORE_NAME               5 (border_radius)
+         
+         236          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\canvas\entry.py", line 236>)
+                      38 MAKE_FUNCTION            0
+                      40 STORE_NAME               6 (_draw)
+         
+         266          42 LOAD_CONST              17 ((None,))
+                      44 LOAD_CONST               6 (<code object _focus, file "D:\tkadw\tkadw\canvas\entry.py", line 266>)
+                      46 MAKE_FUNCTION            1 (defaults)
+                      48 STORE_NAME               7 (_focus)
+         
+         275          50 LOAD_CONST              17 ((None,))
+                      52 LOAD_CONST               7 (<code object _focusout, file "D:\tkadw\tkadw\canvas\entry.py", line 275>)
+                      54 MAKE_FUNCTION            1 (defaults)
+                      56 STORE_NAME               8 (_focusout)
+         
+         284          58 LOAD_CONST              17 ((None,))
+                      60 LOAD_CONST               8 (<code object _click, file "D:\tkadw\tkadw\canvas\entry.py", line 284>)
+                      62 MAKE_FUNCTION            1 (defaults)
+                      64 STORE_NAME               9 (_click)
+         
+         287          66 LOAD_CONST              17 ((None,))
+                      68 LOAD_CONST               9 (<code object _hover, file "D:\tkadw\tkadw\canvas\entry.py", line 287>)
+                      70 MAKE_FUNCTION            1 (defaults)
+                      72 STORE_NAME              10 (_hover)
+         
+         290          74 LOAD_CONST              17 ((None,))
+                      76 LOAD_CONST              10 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\entry.py", line 290>)
+                      78 MAKE_FUNCTION            1 (defaults)
+                      80 STORE_NAME              11 (_hover_release)
+         
+         301          82 LOAD_CONST              17 ((None,))
+                      84 LOAD_CONST              11 ('font')
+                      86 LOAD_NAME               12 (Font)
+                      88 BUILD_TUPLE              2
+                      90 LOAD_CONST              12 (<code object font, file "D:\tkadw\tkadw\canvas\entry.py", line 301>)
+                      92 MAKE_FUNCTION            5 (defaults, annotations)
+                      94 STORE_NAME              13 (font)
+         
+         307          96 LOAD_CONST              13 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 307>)
+                      98 MAKE_FUNCTION            0
+                     100 STORE_NAME              14 (default_palette)
+         
+         310         102 LOAD_CONST              14 (<code object palette_light, file "D:\tkadw\tkadw\canvas\entry.py", line 310>)
+                     104 MAKE_FUNCTION            0
+                     106 STORE_NAME              15 (palette_light)
          
-         306         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 306>)
+         338         108 LOAD_CONST              15 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\entry.py", line 338>)
                      110 MAKE_FUNCTION            0
-                     112 STORE_NAME              16 (default_palette)
+                     112 STORE_NAME              16 (palette_dark)
          
-         309         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\entry.py", line 309>)
-                     116 MAKE_FUNCTION            0
-                     118 STORE_NAME              17 (palette_light)
-         
-         333         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\entry.py", line 333>)
-                     122 MAKE_FUNCTION            0
-                     124 STORE_NAME              18 (palette_dark)
-         
-         357         126 LOAD_CONST              18 ((None,))
-                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\entry.py", line 357>)
-                     130 MAKE_FUNCTION            1 (defaults)
-                     132 STORE_NAME              19 (palette)
-                     134 LOAD_CLOSURE             0 (__class__)
-                     136 COPY                     1
-                     138 STORE_NAME              20 (__classcell__)
-                     140 RETURN_VALUE
+         366         114 LOAD_CONST              17 ((None,))
+                     116 LOAD_CLOSURE             0 (__class__)
+                     118 BUILD_TUPLE              1
+                     120 LOAD_CONST              16 (<code object palette, file "D:\tkadw\tkadw\canvas\entry.py", line 366>)
+                     122 MAKE_FUNCTION            9 (defaults, closure)
+                     124 STORE_NAME              17 (palette)
+                     126 LOAD_CLOSURE             0 (__class__)
+                     128 COPY                     1
+                     130 STORE_NAME              18 (__classcell__)
+                     132 RETURN_VALUE
          consts
             'AdwDrawBasicRoundEntry'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               222           2 RESUME                   0
+               223           2 RESUME                   0
                
-               223           4 PUSH_NULL
+               224           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -1891,95 +1929,94 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '__init__'
-               firstlineno 222
+               firstlineno 223
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006401a6020000ab020000000000
                   000000721e7c00a00100000000000000000000000000000000000000007c
                   006a0200000000000000006402ac03a6020000ab02000000000000000001
                   006400530064005300
-               225           0 RESUME                   0
+               226           0 RESUME                   0
                
-               226           2 LOAD_GLOBAL              1 (NULL + hasattr)
+               227           2 LOAD_GLOBAL              1 (NULL + hasattr)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_CONST               1 ('button_frame_back')
                             18 PRECALL                  2
                             22 CALL                     2
                             32 POP_JUMP_FORWARD_IF_FALSE    30 (to 94)
                
-               227          34 LOAD_FAST                0 (self)
+               228          34 LOAD_FAST                0 (self)
                             36 LOAD_METHOD              1 (configure)
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                2 (button_frame_back)
                             70 LOAD_CONST               2 (0)
                             72 KW_NAMES                 3
                             74 PRECALL                  2
                             78 CALL                     2
                             88 POP_TOP
                             90 LOAD_CONST               0 (None)
                             92 RETURN_VALUE
                
-               226     >>   94 LOAD_CONST               0 (None)
+               227     >>   94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                consts
                   None
                   'button_frame_back'
                   0
                   ('background', 'borderwidth')
                names      ('hasattr', 'configure', 'button_frame_back')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_other'
-               firstlineno 225
+               firstlineno 226
                lnotab 0x020120013cff
             None
-            'radius'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               229           0 RESUME                   0
+               230           0 RESUME                   0
                
-               230           2 LOAD_FAST                1 (radius)
+               231           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               231           6 LOAD_FAST                0 (self)
+               232           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               233     >>   20 LOAD_FAST                1 (radius)
+               234     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'border_radius'
-               firstlineno 229
+               firstlineno 230
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -2015,27 +2052,27 @@
                   000000000000000000000000007c006a100000000000000000a6010000ab
                   01000000000000000001007c00a011000000000000000000000000000000
                   00000000007c006a1000000000000000007c006a0c0000000000000000a6
                   020000ab02000000000000000001007c006a0b0000000000000000a01200
                   000000000000000000000000000000000000007c006a0700000000000000
                   007c006a1300000000000000007c006a130000000000000000ac0ba60300
                   00ab030000000000000000010064005300
-               235           0 RESUME                   0
+               236           0 RESUME                   0
                
-               236           2 LOAD_FAST                0 (self)
+               237           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               238          44 LOAD_FAST                0 (self)
+               239          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect2)
                
-               239          68 LOAD_CONST               2 (2)
+               240          68 LOAD_CONST               2 (2)
                             70 LOAD_CONST               2 (2)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
@@ -2044,159 +2081,159 @@
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                            160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (entry_radius)
                
-               240         172 LOAD_FAST                0 (self)
+               241         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (entry_border_width)
                
-               241         184 LOAD_FAST                0 (self)
+               242         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_entry_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_entry_back)
                
-               238         208 KW_NAMES                 4
+               239         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 LOAD_FAST                0 (self)
                            226 STORE_ATTR               8 (entry_frame)
                
-               244         236 LOAD_FAST                0 (self)
+               245         236 LOAD_FAST                0 (self)
                            238 LOAD_METHOD              9 (create_window)
                
-               245         260 LOAD_FAST                0 (self)
+               246         260 LOAD_FAST                0 (self)
                            262 LOAD_METHOD              2 (winfo_width)
                            284 PRECALL                  0
                            288 CALL                     0
                            298 LOAD_CONST               2 (2)
                            300 BINARY_OP               11 (/)
                            304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              3 (winfo_height)
                            328 PRECALL                  0
                            332 CALL                     0
                            342 LOAD_CONST               2 (2)
                            344 BINARY_OP               11 (/)
                
-               246         348 LOAD_FAST                0 (self)
+               247         348 LOAD_FAST                0 (self)
                            350 LOAD_METHOD              2 (winfo_width)
                            372 PRECALL                  0
                            376 CALL                     0
                            386 LOAD_FAST                0 (self)
                            388 LOAD_ATTR                5 (entry_border_width)
                            398 BINARY_OP               10 (-)
                            402 LOAD_CONST               5 (5)
                            404 BINARY_OP               10 (-)
                            408 LOAD_FAST                0 (self)
                            410 LOAD_ATTR               10 (entry_padding)
                            420 LOAD_CONST               6 (0)
                            422 BINARY_SUBSCR
                            432 BINARY_OP               10 (-)
                
-               247         436 LOAD_FAST                0 (self)
+               248         436 LOAD_FAST                0 (self)
                            438 LOAD_METHOD              3 (winfo_height)
                            460 PRECALL                  0
                            464 CALL                     0
                            474 LOAD_FAST                0 (self)
                            476 LOAD_ATTR                5 (entry_border_width)
                            486 BINARY_OP               10 (-)
                            490 LOAD_CONST               5 (5)
                            492 BINARY_OP               10 (-)
                            496 LOAD_FAST                0 (self)
                            498 LOAD_ATTR               10 (entry_padding)
                            508 LOAD_CONST               7 (1)
                            510 BINARY_SUBSCR
                            520 BINARY_OP               10 (-)
                
-               248         524 LOAD_FAST                0 (self)
+               249         524 LOAD_FAST                0 (self)
                            526 LOAD_ATTR               11 (entry)
                
-               244         536 KW_NAMES                 8
+               245         536 KW_NAMES                 8
                            538 PRECALL                  5
                            542 CALL                     5
                            552 LOAD_FAST                0 (self)
                            554 STORE_ATTR              12 (entry_text)
                
-               251         564 LOAD_FAST                0 (self)
+               252         564 LOAD_FAST                0 (self)
                            566 LOAD_METHOD             13 (create_rectangle)
                            588 LOAD_CONST               3 (3)
                            590 LOAD_FAST                0 (self)
                            592 LOAD_ATTR                4 (entry_radius)
                            602 LOAD_CONST               2 (2)
                            604 BINARY_OP               11 (/)
                            608 BINARY_OP                0 (+)
                
-               252         612 LOAD_FAST                0 (self)
+               253         612 LOAD_FAST                0 (self)
                            614 LOAD_METHOD              3 (winfo_height)
                            636 PRECALL                  0
                            640 CALL                     0
                            650 LOAD_FAST                0 (self)
                            652 LOAD_ATTR               14 (_entry_bottom_width)
                            662 BINARY_OP               10 (-)
                            666 LOAD_CONST               3 (3)
                            668 BINARY_OP               10 (-)
                
-               253         672 LOAD_FAST                0 (self)
+               254         672 LOAD_FAST                0 (self)
                            674 LOAD_METHOD              2 (winfo_width)
                            696 PRECALL                  0
                            700 CALL                     0
                            710 LOAD_CONST               3 (3)
                            712 BINARY_OP               10 (-)
                            716 LOAD_FAST                0 (self)
                            718 LOAD_ATTR                4 (entry_radius)
                            728 LOAD_CONST               2 (2)
                            730 BINARY_OP               11 (/)
                            734 BINARY_OP               10 (-)
                
-               254         738 LOAD_FAST                0 (self)
+               255         738 LOAD_FAST                0 (self)
                            740 LOAD_METHOD              3 (winfo_height)
                            762 PRECALL                  0
                            766 CALL                     0
                            776 LOAD_CONST               9 (3.5)
                            778 BINARY_OP               10 (-)
                
-               255         782 LOAD_FAST                0 (self)
+               256         782 LOAD_FAST                0 (self)
                            784 LOAD_ATTR               15 (_entry_bottom_line)
                            794 LOAD_FAST                0 (self)
                            796 LOAD_ATTR               15 (_entry_bottom_line)
                
-               256         806 LOAD_CONST               6 (0)
+               257         806 LOAD_CONST               6 (0)
                
-               251         808 KW_NAMES                10
+               252         808 KW_NAMES                10
                            810 PRECALL                  7
                            814 CALL                     7
                            824 LOAD_FAST                0 (self)
                            826 STORE_ATTR              16 (entry_bottom)
                
-               258         836 LOAD_FAST                0 (self)
+               259         836 LOAD_FAST                0 (self)
                            838 LOAD_ATTR               14 (_entry_bottom_width)
                            848 LOAD_CONST               6 (0)
                            850 COMPARE_OP               2 (==)
                            856 POP_JUMP_FORWARD_IF_FALSE    26 (to 910)
                
-               259         858 LOAD_FAST                0 (self)
+               260         858 LOAD_FAST                0 (self)
                            860 LOAD_METHOD              0 (delete)
                            882 LOAD_FAST                0 (self)
                            884 LOAD_ATTR               16 (entry_bottom)
                            894 PRECALL                  1
                            898 CALL                     1
                            908 POP_TOP
                
-               261     >>  910 LOAD_FAST                0 (self)
+               262     >>  910 LOAD_FAST                0 (self)
                            912 LOAD_METHOD             17 (tag_raise)
                            934 LOAD_FAST                0 (self)
                            936 LOAD_ATTR               16 (entry_bottom)
                            946 LOAD_FAST                0 (self)
                            948 LOAD_ATTR               12 (entry_text)
                            958 PRECALL                  2
                            962 CALL                     2
                            972 POP_TOP
                
-               263         974 LOAD_FAST                0 (self)
+               264         974 LOAD_FAST                0 (self)
                            976 LOAD_ATTR               11 (entry)
                            986 LOAD_METHOD             18 (configure)
                           1008 LOAD_FAST                0 (self)
                           1010 LOAD_ATTR                7 (_entry_back)
                           1020 LOAD_FAST                0 (self)
                           1022 LOAD_ATTR               19 (_entry_text_back)
                           1032 LOAD_FAST                0 (self)
@@ -2222,15 +2259,15 @@
                   ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_round_rect2', 'winfo_width', 'winfo_height', 'entry_radius', 'entry_border_width', '_entry_border', '_entry_back', 'entry_frame', 'create_window', 'entry_padding', 'entry', 'entry_text', 'create_rectangle', '_entry_bottom_width', '_entry_bottom_line', 'entry_bottom', 'tag_raise', 'configure', '_entry_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_draw'
-               firstlineno 235
+               firstlineno 236
                lnotab
                   0x02012a02180168010c0118fd1c0618015801580158010cfc1c0730013c
                   0142012c01180102fb1c07160134024002
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -2238,42 +2275,42 @@
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               265           0 RESUME                   0
+               266           0 RESUME                   0
                
-               266           2 LOAD_FAST                0 (self)
+               267           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (entry_focusin_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_entry_back)
                
-               267          26 LOAD_FAST                0 (self)
+               268          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (entry_focusin_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_entry_border)
                
-               268          50 LOAD_FAST                0 (self)
+               269          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (entry_focusin_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_entry_text_back)
                
-               269          74 LOAD_FAST                0 (self)
+               270          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (entry_focusin_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_entry_bottom_line)
                
-               270          98 LOAD_FAST                0 (self)
+               271          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (entry_focusin_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_entry_bottom_width)
                
-               272         122 LOAD_FAST                0 (self)
+               273         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -2281,56 +2318,56 @@
                   None
                names      ('entry_focusin_back', '_entry_back', 'entry_focusin_border', '_entry_border', 'entry_focusin_text_back', '_entry_text_back', 'entry_focusin_bottom_line', '_entry_bottom_line', 'entry_focusin_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_focus'
-               firstlineno 265
+               firstlineno 266
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               274           0 RESUME                   0
+               275           0 RESUME                   0
                
-               275           2 LOAD_FAST                0 (self)
+               276           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (entry_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_entry_back)
                
-               276          26 LOAD_FAST                0 (self)
+               277          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (entry_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_entry_border)
                
-               277          50 LOAD_FAST                0 (self)
+               278          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (entry_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_entry_text_back)
                
-               278          74 LOAD_FAST                0 (self)
+               279          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (entry_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_entry_bottom_line)
                
-               279          98 LOAD_FAST                0 (self)
+               280          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (entry_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_entry_bottom_width)
                
-               281         122 LOAD_FAST                0 (self)
+               282         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -2338,66 +2375,66 @@
                   None
                names      ('entry_back', '_entry_back', 'entry_border', '_entry_border', 'entry_text_back', '_entry_text_back', 'entry_bottom_line', '_entry_bottom_line', 'entry_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_focusout'
-               firstlineno 274
+               firstlineno 275
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               283           0 RESUME                   0
+               284           0 RESUME                   0
                
-               284           2 LOAD_FAST                0 (self)
+               285           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_set)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('focus_set',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_click'
-               firstlineno 283
+               firstlineno 284
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064005300
-               286           0 RESUME                   0
+               287           0 RESUME                   0
                
-               287           2 LOAD_CONST               1 (True)
+               288           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                   True
                names      ('hover',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_hover'
-               firstlineno 286
+               firstlineno 287
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -2405,723 +2442,567 @@
                   00ab000000000000000000735a64017c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c006a0a00000000000000007c005f0b00000000000000007c00a0
                   0c00000000000000000000000000000000000000006400a6010000ab0100
                   0000000000000001006400530064005300
-               289           0 RESUME                   0
+               290           0 RESUME                   0
                
-               290           2 LOAD_FAST                0 (self)
+               291           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_get)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_JUMP_FORWARD_IF_TRUE    90 (to 222)
                
-               291          42 LOAD_CONST               1 (False)
+               292          42 LOAD_CONST               1 (False)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (hover)
                
-               292          56 LOAD_FAST                0 (self)
+               293          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (entry_back)
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_entry_back)
                
-               293          80 LOAD_FAST                0 (self)
+               294          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (entry_border)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               5 (_entry_border)
                
-               294         104 LOAD_FAST                0 (self)
+               295         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (entry_text_back)
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               7 (_entry_text_back)
                
-               295         128 LOAD_FAST                0 (self)
+               296         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                8 (entry_bottom_line)
                            140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               9 (_entry_bottom_line)
                
-               296         152 LOAD_FAST                0 (self)
+               297         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR               10 (entry_bottom_width)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR              11 (_entry_bottom_width)
                
-               298         176 LOAD_FAST                0 (self)
+               299         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD             12 (_draw)
                            200 LOAD_CONST               0 (None)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                
-               290     >>  222 LOAD_CONST               0 (None)
+               291     >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   False
                names      ('focus_get', 'hover', 'entry_back', '_entry_back', 'entry_border', '_entry_border', 'entry_text_back', '_entry_text_back', 'entry_bottom_line', '_entry_bottom_line', 'entry_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_hover_release'
-               firstlineno 289
+               firstlineno 290
                lnotab 0x020128010e01180118011801180118022ef8
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               300           0 RESUME                   0
+               301           0 RESUME                   0
                
-               301           2 LOAD_FAST                1 (font)
+               302           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               302           6 LOAD_FAST                0 (self)
+               303           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (entry_text_font)
                             18 RETURN_VALUE
                
-               304     >>   20 LOAD_FAST                1 (font)
+               305     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (entry_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('entry_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'font'
-               firstlineno 300
+               firstlineno 301
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               306           0 RESUME                   0
+               307           0 RESUME                   0
                
-               307           2 LOAD_FAST                0 (self)
+               308           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 306
+               firstlineno 307
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 17
+               stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564066407640864066409640a640b640c640d640e9c0ea6
-                  010000ab010000000000000000010064005300
-               309           0 RESUME                   0
+                  0264036404640564066407640564086409640a640b6407640c640d640e9c
+                  06640f9c096901a6010000ab010000000000000000010064005300
+               310           0 RESUME                   0
                
-               310           2 LOAD_FAST                0 (self)
+               311           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               312          26 LOAD_CONST               1 (6)
+               313          26 LOAD_CONST               1 ('entry')
                
-               314          28 LOAD_CONST               2 ((3, 4))
+               314          28 LOAD_CONST               2 (6)
                
-               316          30 LOAD_CONST               3 ('#f3f3f3')
+               315          30 LOAD_CONST               3 ((3, 4))
                
-               317          32 LOAD_CONST               4 (1)
+               317          32 LOAD_CONST               4 ('#fdfdfd')
                
-               318          34 LOAD_CONST               5 (0)
+               318          34 LOAD_CONST               5 ('#eaeaea')
                
-               320          36 LOAD_CONST               6 ('#eaeaea')
+               319          36 LOAD_CONST               6 ('#5f5f5f')
                
-               321          38 LOAD_CONST               7 ('#fdfdfd')
+               320          38 LOAD_CONST               7 (1)
                
-               322          40 LOAD_CONST               8 ('#5f5f5f')
+               322          40 LOAD_CONST               5 ('#eaeaea')
                
-               323          42 LOAD_CONST               6 ('#eaeaea')
+               323          42 LOAD_CONST               8 (0)
                
-               325          44 LOAD_CONST               9 ('#e2e2e2')
+               326          44 LOAD_CONST               9 ('#f9f9f9')
                
-               326          46 LOAD_CONST              10 ('#f9f9f9')
+               327          46 LOAD_CONST              10 ('#e2e2e2')
                
-               327          48 LOAD_CONST              11 ('#1a1a1a')
+               328          48 LOAD_CONST              11 ('#1a1a1a')
                
-               328          50 LOAD_CONST              12 ('#185fb4')
+               329          50 LOAD_CONST               7 (1)
                
-               329          52 LOAD_CONST              13 (2)
+               331          52 LOAD_CONST              12 ('#185fb4')
                
-               311          54 LOAD_CONST              14 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
-                            56 BUILD_CONST_KEY_MAP     14
+               332          54 LOAD_CONST              13 (2)
                
-               310          58 PRECALL                  1
-                            62 CALL                     1
-                            72 POP_TOP
-                            74 LOAD_CONST               0 (None)
-                            76 RETURN_VALUE
+               325          56 LOAD_CONST              14 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                            58 BUILD_CONST_KEY_MAP      6
+               
+               313          60 LOAD_CONST              15 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                            62 BUILD_CONST_KEY_MAP      9
+               
+               312          64 BUILD_MAP                1
+               
+               311          66 PRECALL                  1
+                            70 CALL                     1
+                            80 POP_TOP
+                            82 LOAD_CONST               0 (None)
+                            84 RETURN_VALUE
                consts
                   None
+                  'entry'
                   6
                   (3, 4)
-                  '#f3f3f3'
-                  1
-                  0
-                  '#eaeaea'
                   '#fdfdfd'
+                  '#eaeaea'
                   '#5f5f5f'
-                  '#e2e2e2'
+                  1
+                  0
                   '#f9f9f9'
+                  '#e2e2e2'
                   '#1a1a1a'
                   '#185fb4'
                   2
-                  ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
+                  ('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width')
+                  ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette_light'
-               firstlineno 309
+               firstlineno 310
                lnotab
-                  0x0201180202020202020102010202020102010201020202010201020102
-                  0102ee04ff
+                  0x0201180202010201020202010201020102020201020302010201020102
+                  02020102f904f404ff02ff
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 17
+               stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564066407640864096405640a6408640b640c640d9c0ea6
-                  010000ab010000000000000000010064005300
-               333           0 RESUME                   0
+                  026403640464056406640764086409640a640564086407640b640c640d9c
+                  06640e9c096901a6010000ab010000000000000000010064005300
+               338           0 RESUME                   0
                
-               334           2 LOAD_FAST                0 (self)
+               339           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               336          26 LOAD_CONST               1 (6)
+               341          26 LOAD_CONST               1 ('entry')
+               
+               342          28 LOAD_CONST               2 (6)
                
-               338          28 LOAD_CONST               2 ((3, 4))
+               343          30 LOAD_CONST               3 ((3, 4))
                
-               340          30 LOAD_CONST               3 ('#202020')
+               345          32 LOAD_CONST               4 ('#353535')
                
-               341          32 LOAD_CONST               4 (1)
+               346          34 LOAD_CONST               5 ('#454545')
                
-               343          34 LOAD_CONST               5 ('#454545')
+               347          36 LOAD_CONST               6 ('#cecece')
                
-               344          36 LOAD_CONST               6 ('#353535')
+               348          38 LOAD_CONST               7 (1)
                
-               345          38 LOAD_CONST               7 ('#cecece')
+               350          40 LOAD_CONST               8 ('#ffffff')
                
-               346          40 LOAD_CONST               8 ('#ffffff')
+               351          42 LOAD_CONST               9 (0)
                
-               347          42 LOAD_CONST               9 (0)
+               354          44 LOAD_CONST              10 ('#2f2f2f')
                
-               349          44 LOAD_CONST               5 ('#454545')
+               355          46 LOAD_CONST               5 ('#454545')
                
-               350          46 LOAD_CONST              10 ('#2f2f2f')
+               356          48 LOAD_CONST               8 ('#ffffff')
                
-               351          48 LOAD_CONST               8 ('#ffffff')
+               357          50 LOAD_CONST               7 (1)
                
-               352          50 LOAD_CONST              11 ('#4cc2ff')
+               359          52 LOAD_CONST              11 ('#4cc2ff')
                
-               353          52 LOAD_CONST              12 (2)
+               360          54 LOAD_CONST              12 (2)
                
-               335          54 LOAD_CONST              13 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
-                            56 BUILD_CONST_KEY_MAP     14
+               353          56 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                            58 BUILD_CONST_KEY_MAP      6
                
-               334          58 PRECALL                  1
-                            62 CALL                     1
-                            72 POP_TOP
-                            74 LOAD_CONST               0 (None)
-                            76 RETURN_VALUE
+               341          60 LOAD_CONST              14 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                            62 BUILD_CONST_KEY_MAP      9
+               
+               340          64 BUILD_MAP                1
+               
+               339          66 PRECALL                  1
+                            70 CALL                     1
+                            80 POP_TOP
+                            82 LOAD_CONST               0 (None)
+                            84 RETURN_VALUE
                consts
                   None
+                  'entry'
                   6
                   (3, 4)
-                  '#202020'
-                  1
-                  '#454545'
                   '#353535'
+                  '#454545'
                   '#cecece'
+                  1
                   '#ffffff'
                   0
                   '#2f2f2f'
                   '#4cc2ff'
                   2
-                  ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
+                  ('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width')
+                  ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette_dark'
-               firstlineno 333
+               firstlineno 338
                lnotab
-                  0x0201180202020202020102020201020102010201020202010201020102
-                  0102ee04ff
+                  0x0201180202010201020202010201020102020201020302010201020102
+                  02020102f904f404ff02ff
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 11
+               stacksize : 3
                flags     : 3
                code
-                  0x97007c0181df7c016401190000000000000000007c005f000000000000
-                  0000007c016402190000000000000000007c005f0100000000000000007c
-                  016403190000000000000000007c005f0200000000000000007c01640419
-                  0000000000000000007c005f0300000000000000007c0164051900000000
-                  00000000007c005f0400000000000000007c016406190000000000000000
-                  007c005f0500000000000000007c016407190000000000000000007c005f
-                  0600000000000000007c016408190000000000000000007c005f07000000
-                  00000000007c016409190000000000000000007c005f0800000000000000
-                  007c01640a190000000000000000007c005f0900000000000000007c0164
-                  0b190000000000000000007c005f0a00000000000000007c01640c190000
-                  000000000000007c005f0b00000000000000007c01640d19000000000000
-                  0000007c005f0c00000000000000007c01640e190000000000000000007c
-                  005f0d000000000000000009007c00a00e00000000000000000000000000
-                  000000000000006400a6010000ab01000000000000000001006400530023
-                  00741e000000000000000000002400720401005900640053007700780359
-                  0077017c006a0100000000000000007c006a0200000000000000007c006a
-                  0300000000000000007c006a0800000000000000007c006a040000000000
-                  0000007c006a0500000000000000007c006a0600000000000000007c006a
-                  0900000000000000007c006a0a00000000000000007c006a0b0000000000
-                  000000640f9c0a5300
-               357           0 RESUME                   0
-               
-               358           2 LOAD_FAST                1 (dict)
-                             4 POP_JUMP_FORWARD_IF_NONE   223 (to 452)
-               
-               359           6 LOAD_FAST                1 (dict)
-                             8 LOAD_CONST               1 ('entry_radius')
-                            10 BINARY_SUBSCR
-                            20 LOAD_FAST                0 (self)
-                            22 STORE_ATTR               0 (entry_radius)
-               
-               361          32 LOAD_FAST                1 (dict)
-                            34 LOAD_CONST               2 ('entry_padding')
-                            36 BINARY_SUBSCR
-                            46 LOAD_FAST                0 (self)
-                            48 STORE_ATTR               1 (entry_padding)
-               
-               363          58 LOAD_FAST                1 (dict)
-                            60 LOAD_CONST               3 ('entry_frame_back')
-                            62 BINARY_SUBSCR
-                            72 LOAD_FAST                0 (self)
-                            74 STORE_ATTR               2 (entry_frame_back)
+                  0x95019700740100000000000000000000a6000000ab0000000000000000
+                  00a00100000000000000000000000000000000000000007c01a6010000ab
+                  010000000000000000010064017c01760072157c01640119000000000000
+                  0000006402190000000000000000007c005f020000000000000000640053
+                  0064005300
+                             0 COPY_FREE_VARS           1
                
-               364          84 LOAD_FAST                1 (dict)
-                            86 LOAD_CONST               4 ('entry_border_width')
-                            88 BINARY_SUBSCR
-                            98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               3 (entry_border_width)
-               
-               366         110 LOAD_FAST                1 (dict)
-                           112 LOAD_CONST               5 ('entry_border')
-                           114 BINARY_SUBSCR
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               4 (entry_border)
-               
-               367         136 LOAD_FAST                1 (dict)
-                           138 LOAD_CONST               6 ('entry_back')
-                           140 BINARY_SUBSCR
-                           150 LOAD_FAST                0 (self)
-                           152 STORE_ATTR               5 (entry_back)
-               
-               368         162 LOAD_FAST                1 (dict)
-                           164 LOAD_CONST               7 ('entry_text_back')
-                           166 BINARY_SUBSCR
-                           176 LOAD_FAST                0 (self)
-                           178 STORE_ATTR               6 (entry_text_back)
-               
-               369         188 LOAD_FAST                1 (dict)
-                           190 LOAD_CONST               8 ('entry_bottom_line')
-                           192 BINARY_SUBSCR
-                           202 LOAD_FAST                0 (self)
-                           204 STORE_ATTR               7 (entry_bottom_line)
-               
-               370         214 LOAD_FAST                1 (dict)
-                           216 LOAD_CONST               9 ('entry_bottom_width')
-                           218 BINARY_SUBSCR
-                           228 LOAD_FAST                0 (self)
-                           230 STORE_ATTR               8 (entry_bottom_width)
+               366           2 RESUME                   0
                
-               372         240 LOAD_FAST                1 (dict)
-                           242 LOAD_CONST              10 ('entry_focusin_border')
-                           244 BINARY_SUBSCR
-                           254 LOAD_FAST                0 (self)
-                           256 STORE_ATTR               9 (entry_focusin_border)
-               
-               373         266 LOAD_FAST                1 (dict)
-                           268 LOAD_CONST              11 ('entry_focusin_back')
-                           270 BINARY_SUBSCR
-                           280 LOAD_FAST                0 (self)
-                           282 STORE_ATTR              10 (entry_focusin_back)
-               
-               374         292 LOAD_FAST                1 (dict)
-                           294 LOAD_CONST              12 ('entry_focusin_text_back')
-                           296 BINARY_SUBSCR
-                           306 LOAD_FAST                0 (self)
-                           308 STORE_ATTR              11 (entry_focusin_text_back)
-               
-               375         318 LOAD_FAST                1 (dict)
-                           320 LOAD_CONST              13 ('entry_focusin_bottom_line')
-                           322 BINARY_SUBSCR
-                           332 LOAD_FAST                0 (self)
-                           334 STORE_ATTR              12 (entry_focusin_bottom_line)
-               
-               376         344 LOAD_FAST                1 (dict)
-                           346 LOAD_CONST              14 ('entry_focusin_bottom_width')
-                           348 BINARY_SUBSCR
-                           358 LOAD_FAST                0 (self)
-                           360 STORE_ATTR              13 (entry_focusin_bottom_width)
-               
-               378         370 NOP
-               
-               379         372 LOAD_FAST                0 (self)
-                           374 LOAD_METHOD             14 (_draw)
-                           396 LOAD_CONST               0 (None)
-                           398 PRECALL                  1
-                           402 CALL                     1
-                           412 POP_TOP
-                           414 LOAD_CONST               0 (None)
-                           416 RETURN_VALUE
-                       >>  418 PUSH_EXC_INFO
-               
-               380         420 LOAD_GLOBAL             30 (AttributeError)
-                           432 CHECK_EXC_MATCH
-                           434 POP_JUMP_FORWARD_IF_FALSE     4 (to 444)
-                           436 POP_TOP
-               
-               381         438 POP_EXCEPT
-                           440 LOAD_CONST               0 (None)
-                           442 RETURN_VALUE
-               
-               380     >>  444 RERAISE                  0
-                       >>  446 COPY                     3
-                           448 POP_EXCEPT
-                           450 RERAISE                  1
-               
-               384     >>  452 LOAD_FAST                0 (self)
-                           454 LOAD_ATTR                1 (entry_padding)
-               
-               386         464 LOAD_FAST                0 (self)
-                           466 LOAD_ATTR                2 (entry_frame_back)
-               
-               387         476 LOAD_FAST                0 (self)
-                           478 LOAD_ATTR                3 (entry_border_width)
-               
-               388         488 LOAD_FAST                0 (self)
-                           490 LOAD_ATTR                8 (entry_bottom_width)
-               
-               390         500 LOAD_FAST                0 (self)
-                           502 LOAD_ATTR                4 (entry_border)
-               
-               391         512 LOAD_FAST                0 (self)
-                           514 LOAD_ATTR                5 (entry_back)
-               
-               392         524 LOAD_FAST                0 (self)
-                           526 LOAD_ATTR                6 (entry_text_back)
-               
-               394         536 LOAD_FAST                0 (self)
-                           538 LOAD_ATTR                9 (entry_focusin_border)
-               
-               395         548 LOAD_FAST                0 (self)
-                           550 LOAD_ATTR               10 (entry_focusin_back)
-               
-               396         560 LOAD_FAST                0 (self)
-                           562 LOAD_ATTR               11 (entry_focusin_text_back)
-               
-               383         572 LOAD_CONST              15 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back'))
-                           574 BUILD_CONST_KEY_MAP     10
-                           576 RETURN_VALUE
-               ExceptionTable:
-                 372 to 412 -> 418 [0]
-                 418 to 436 -> 446 [1] lasti
-                 444 to 444 -> 446 [1] lasti
-               consts
-                  None
-                  'entry_radius'
-                  'entry_padding'
-                  'entry_frame_back'
-                  'entry_border_width'
-                  'entry_border'
-                  'entry_back'
-                  'entry_text_back'
-                  'entry_bottom_line'
-                  'entry_bottom_width'
-                  'entry_focusin_border'
-                  'entry_focusin_back'
-                  'entry_focusin_text_back'
-                  'entry_focusin_bottom_line'
-                  'entry_focusin_bottom_width'
-                  ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back')
-               names      ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width', '_draw', 'AttributeError')
+               367           4 LOAD_GLOBAL              1 (NULL + super)
+                            16 PRECALL                  0
+                            20 CALL                     0
+                            30 LOAD_METHOD              1 (palette)
+                            52 LOAD_FAST                1 (dict)
+                            54 PRECALL                  1
+                            58 CALL                     1
+                            68 POP_TOP
+               
+               368          70 LOAD_CONST               1 ('entry')
+                            72 LOAD_FAST                1 (dict)
+                            74 CONTAINS_OP              0
+                            76 POP_JUMP_FORWARD_IF_FALSE    21 (to 120)
+               
+               369          78 LOAD_FAST                1 (dict)
+                            80 LOAD_CONST               1 ('entry')
+                            82 BINARY_SUBSCR
+                            92 LOAD_CONST               2 ('radius')
+                            94 BINARY_SUBSCR
+                           104 LOAD_FAST                0 (self)
+                           106 STORE_ATTR               2 (entry_radius)
+                           116 LOAD_CONST               0 (None)
+                           118 RETURN_VALUE
+               
+               368     >>  120 LOAD_CONST               0 (None)
+                           122 RETURN_VALUE
+               consts
+                  None
+                  'entry'
+                  'radius'
+               names      ('super', 'palette', 'entry_radius')
                varnames   ('self', 'dict')
-               freevars   ()
+               freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette'
-               firstlineno 357
-               lnotab
-                  0x020104011a021a021a011a021a011a011a011a011a021a011a011a011a
-                  011a0202013001120106ff08040c020c010c010c020c010c010c020c010c
-                  010cf3
+               firstlineno 366
+               lnotab 0x0401420108012aff
             (None,)
-         names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'float', 'int', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawBasicRoundEntry'
-         firstlineno 221
-         lnotab 0x0c010a0306041406061e0809080908030803080b0e06060306180618
+         firstlineno 222
+         lnotab 0x0c010a0306040806061e0809080908030803080b0e060603061c061c
       'AdwDrawBasicRoundEntry'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         400           0 RESUME                   0
+         372           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundEntry')
                        8 STORE_NAME               2 (__qualname__)
          
-         401          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 401>)
+         373          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 373>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundEntry'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               401           0 RESUME                   0
+               373           0 RESUME                   0
                
-               402           2 LOAD_FAST                0 (self)
+               374           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 401
+               firstlineno 373
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawRoundEntry'
-         firstlineno 400
+         firstlineno 372
          lnotab 0x0a01
       'AdwDrawRoundEntry'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         405           0 RESUME                   0
+         377           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkEntry')
                        8 STORE_NAME               2 (__qualname__)
          
-         406          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 406>)
+         378          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 378>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkEntry'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               406           0 RESUME                   0
+               378           0 RESUME                   0
                
-               407           2 LOAD_FAST                0 (self)
+               379           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 406
+               firstlineno 378
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawRoundDarkEntry'
-         firstlineno 405
+         firstlineno 377
          lnotab 0x0a01
       'AdwDrawRoundDarkEntry'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 4
+         stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
-            126404650565067a0700006602640584055a07640684005a086412640784
-            015a096412640884015a0a6412640984015a0b6412640a84015a0c641264
-            0b84015a0d6412640c650e6602640d84055a0f640e84005a10640f84005a
-            11641084005a126412641184015a13880078015a145300
+            0e640484015a05640584005a06640e640684015a07640e640784015a0864
+            0e640884015a09640e640984015a0a640e640a84015a0b640e640b650c66
+            02640c84055a0d640d84005a0e880078015a0f5300
                        0 MAKE_CELL                0 (__class__)
          
-         410           2 RESUME                   0
+         382           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundEntry3')
                       10 STORE_NAME               2 (__qualname__)
          
-         411          12 LOAD_CLOSURE             0 (__class__)
+         383          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\entry.py", line 411>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\entry.py", line 383>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         414          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\entry.py", line 414>)
+         386          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\entry.py", line 386>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         417          28 LOAD_CONST              18 ((None,))
-                      30 LOAD_CONST               4 ('radius')
-                      32 LOAD_NAME                5 (float)
-                      34 LOAD_NAME                6 (int)
-                      36 BINARY_OP                7 (|)
-                      40 BUILD_TUPLE              2
-                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\entry.py", line 417>)
-                      44 MAKE_FUNCTION            5 (defaults, annotations)
-                      46 STORE_NAME               7 (border_radius)
-         
-         423          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\entry.py", line 423>)
-                      50 MAKE_FUNCTION            0
-                      52 STORE_NAME               8 (_draw)
-         
-         459          54 LOAD_CONST              18 ((None,))
-                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\entry.py", line 459>)
-                      58 MAKE_FUNCTION            1 (defaults)
-                      60 STORE_NAME               9 (_focus)
-         
-         468          62 LOAD_CONST              18 ((None,))
-                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\entry.py", line 468>)
-                      66 MAKE_FUNCTION            1 (defaults)
-                      68 STORE_NAME              10 (_focusout)
-         
-         477          70 LOAD_CONST              18 ((None,))
-                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\entry.py", line 477>)
-                      74 MAKE_FUNCTION            1 (defaults)
-                      76 STORE_NAME              11 (_click)
-         
-         480          78 LOAD_CONST              18 ((None,))
-                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\entry.py", line 480>)
-                      82 MAKE_FUNCTION            1 (defaults)
-                      84 STORE_NAME              12 (_hover)
-         
-         483          86 LOAD_CONST              18 ((None,))
-                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\entry.py", line 483>)
-                      90 MAKE_FUNCTION            1 (defaults)
-                      92 STORE_NAME              13 (_hover_release)
-         
-         494          94 LOAD_CONST              18 ((None,))
-                      96 LOAD_CONST              12 ('font')
-                      98 LOAD_NAME               14 (Font)
-                     100 BUILD_TUPLE              2
-                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\entry.py", line 494>)
-                     104 MAKE_FUNCTION            5 (defaults, annotations)
-                     106 STORE_NAME              15 (font)
-         
-         500         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 500>)
-                     110 MAKE_FUNCTION            0
-                     112 STORE_NAME              16 (default_palette)
-         
-         503         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\entry.py", line 503>)
-                     116 MAKE_FUNCTION            0
-                     118 STORE_NAME              17 (palette_light)
-         
-         527         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\entry.py", line 527>)
-                     122 MAKE_FUNCTION            0
-                     124 STORE_NAME              18 (palette_dark)
-         
-         551         126 LOAD_CONST              18 ((None,))
-                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\entry.py", line 551>)
-                     130 MAKE_FUNCTION            1 (defaults)
-                     132 STORE_NAME              19 (palette)
-                     134 LOAD_CLOSURE             0 (__class__)
-                     136 COPY                     1
-                     138 STORE_NAME              20 (__classcell__)
-                     140 RETURN_VALUE
+         389          28 LOAD_CONST              14 ((None,))
+                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\canvas\entry.py", line 389>)
+                      32 MAKE_FUNCTION            1 (defaults)
+                      34 STORE_NAME               5 (border_radius)
+         
+         395          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\canvas\entry.py", line 395>)
+                      38 MAKE_FUNCTION            0
+                      40 STORE_NAME               6 (_draw)
+         
+         431          42 LOAD_CONST              14 ((None,))
+                      44 LOAD_CONST               6 (<code object _focus, file "D:\tkadw\tkadw\canvas\entry.py", line 431>)
+                      46 MAKE_FUNCTION            1 (defaults)
+                      48 STORE_NAME               7 (_focus)
+         
+         440          50 LOAD_CONST              14 ((None,))
+                      52 LOAD_CONST               7 (<code object _focusout, file "D:\tkadw\tkadw\canvas\entry.py", line 440>)
+                      54 MAKE_FUNCTION            1 (defaults)
+                      56 STORE_NAME               8 (_focusout)
+         
+         449          58 LOAD_CONST              14 ((None,))
+                      60 LOAD_CONST               8 (<code object _click, file "D:\tkadw\tkadw\canvas\entry.py", line 449>)
+                      62 MAKE_FUNCTION            1 (defaults)
+                      64 STORE_NAME               9 (_click)
+         
+         452          66 LOAD_CONST              14 ((None,))
+                      68 LOAD_CONST               9 (<code object _hover, file "D:\tkadw\tkadw\canvas\entry.py", line 452>)
+                      70 MAKE_FUNCTION            1 (defaults)
+                      72 STORE_NAME              10 (_hover)
+         
+         455          74 LOAD_CONST              14 ((None,))
+                      76 LOAD_CONST              10 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\entry.py", line 455>)
+                      78 MAKE_FUNCTION            1 (defaults)
+                      80 STORE_NAME              11 (_hover_release)
+         
+         466          82 LOAD_CONST              14 ((None,))
+                      84 LOAD_CONST              11 ('font')
+                      86 LOAD_NAME               12 (Font)
+                      88 BUILD_TUPLE              2
+                      90 LOAD_CONST              12 (<code object font, file "D:\tkadw\tkadw\canvas\entry.py", line 466>)
+                      92 MAKE_FUNCTION            5 (defaults, annotations)
+                      94 STORE_NAME              13 (font)
+         
+         472          96 LOAD_CONST              13 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 472>)
+                      98 MAKE_FUNCTION            0
+                     100 STORE_NAME              14 (default_palette)
+                     102 LOAD_CLOSURE             0 (__class__)
+                     104 COPY                     1
+                     106 STORE_NAME              15 (__classcell__)
+                     108 RETURN_VALUE
          consts
             'AdwDrawBasicRoundEntry3'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               411           2 RESUME                   0
+               383           2 RESUME                   0
                
-               412           4 PUSH_NULL
+               384           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -3134,29 +3015,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '__init__'
-               firstlineno 411
+               firstlineno 383
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               414           0 RESUME                   0
+               386           0 RESUME                   0
                
-               415           2 LOAD_FAST                0 (self)
+               387           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -3174,49 +3055,48 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_other'
-               firstlineno 414
+               firstlineno 386
                lnotab 0x0201
             None
-            'radius'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               417           0 RESUME                   0
+               389           0 RESUME                   0
                
-               418           2 LOAD_FAST                1 (radius)
+               390           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               419           6 LOAD_FAST                0 (self)
+               391           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               421     >>   20 LOAD_FAST                1 (radius)
+               393     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'border_radius'
-               firstlineno 417
+               firstlineno 389
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -3252,195 +3132,195 @@
                   00000000000000000000000000000000007c006a100000000000000000a6
                   010000ab01000000000000000001007c00a0110000000000000000000000
                   0000000000000000007c006a1000000000000000007c006a0c0000000000
                   000000a6020000ab02000000000000000001007c006a0b00000000000000
                   00a01200000000000000000000000000000000000000007c006a07000000
                   00000000007c006a1300000000000000007c006a130000000000000000ac
                   0aa6030000ab030000000000000000010064005300
-               423           0 RESUME                   0
+               395           0 RESUME                   0
                
-               424           2 LOAD_FAST                0 (self)
+               396           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               426          44 LOAD_FAST                0 (self)
+               398          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
-               427          68 LOAD_CONST               2 (0)
+               399          68 LOAD_CONST               2 (0)
                
-               428          70 LOAD_CONST               2 (0)
+               400          70 LOAD_CONST               2 (0)
                
-               429          72 LOAD_FAST                0 (self)
+               401          72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (1)
                            112 BINARY_OP               10 (-)
                
-               430         116 LOAD_FAST                0 (self)
+               402         116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (1)
                            156 BINARY_OP               10 (-)
                
-               431         160 LOAD_FAST                0 (self)
+               403         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (entry_radius)
                
-               432         172 LOAD_FAST                0 (self)
+               404         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (entry_border_width)
                
-               433         184 LOAD_FAST                0 (self)
+               405         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_entry_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_entry_back)
                
-               426         208 KW_NAMES                 4
+               398         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 POP_TOP
                
-               436         226 LOAD_CONST               5 ('button_frame')
+               408         226 LOAD_CONST               5 ('button_frame')
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (entry_frame)
                
-               438         240 LOAD_FAST                0 (self)
+               410         240 LOAD_FAST                0 (self)
                            242 LOAD_METHOD              9 (create_window)
                
-               439         264 LOAD_FAST                0 (self)
+               411         264 LOAD_FAST                0 (self)
                            266 LOAD_METHOD              2 (winfo_width)
                            288 PRECALL                  0
                            292 CALL                     0
                            302 LOAD_CONST               6 (2)
                            304 BINARY_OP               11 (/)
                            308 LOAD_FAST                0 (self)
                            310 LOAD_METHOD              3 (winfo_height)
                            332 PRECALL                  0
                            336 CALL                     0
                            346 LOAD_CONST               6 (2)
                            348 BINARY_OP               11 (/)
                
-               440         352 LOAD_FAST                0 (self)
+               412         352 LOAD_FAST                0 (self)
                            354 LOAD_METHOD              2 (winfo_width)
                            376 PRECALL                  0
                            380 CALL                     0
                            390 LOAD_FAST                0 (self)
                            392 LOAD_ATTR                5 (entry_border_width)
                            402 BINARY_OP               10 (-)
                            406 LOAD_FAST                0 (self)
                            408 LOAD_ATTR               10 (entry_padding)
                            418 LOAD_CONST               2 (0)
                            420 BINARY_SUBSCR
                            430 BINARY_OP               10 (-)
                            434 LOAD_CONST               6 (2)
                            436 BINARY_OP               10 (-)
                
-               441         440 LOAD_FAST                0 (self)
+               413         440 LOAD_FAST                0 (self)
                            442 LOAD_METHOD              3 (winfo_height)
                            464 PRECALL                  0
                            468 CALL                     0
                            478 LOAD_FAST                0 (self)
                            480 LOAD_ATTR                5 (entry_border_width)
                            490 BINARY_OP               10 (-)
                            494 LOAD_FAST                0 (self)
                            496 LOAD_ATTR               10 (entry_padding)
                            506 LOAD_CONST               3 (1)
                            508 BINARY_SUBSCR
                            518 BINARY_OP               10 (-)
                            522 LOAD_CONST               6 (2)
                            524 BINARY_OP               10 (-)
                
-               442         528 LOAD_FAST                0 (self)
+               414         528 LOAD_FAST                0 (self)
                            530 LOAD_ATTR               11 (entry)
                
-               438         540 KW_NAMES                 7
+               410         540 KW_NAMES                 7
                            542 PRECALL                  5
                            546 CALL                     5
                            556 LOAD_FAST                0 (self)
                            558 STORE_ATTR              12 (entry_text)
                
-               445         568 LOAD_FAST                0 (self)
+               417         568 LOAD_FAST                0 (self)
                            570 LOAD_METHOD             13 (create_rectangle)
                            592 LOAD_CONST               3 (1)
                            594 LOAD_FAST                0 (self)
                            596 LOAD_ATTR                4 (entry_radius)
                            606 LOAD_CONST               8 (5)
                            608 BINARY_OP               11 (/)
                            612 BINARY_OP                0 (+)
                
-               446         616 LOAD_FAST                0 (self)
+               418         616 LOAD_FAST                0 (self)
                            618 LOAD_METHOD              3 (winfo_height)
                            640 PRECALL                  0
                            644 CALL                     0
                            654 LOAD_FAST                0 (self)
                            656 LOAD_ATTR               14 (_entry_bottom_width)
                            666 BINARY_OP               10 (-)
                            670 LOAD_CONST               3 (1)
                            672 BINARY_OP               10 (-)
                
-               447         676 LOAD_FAST                0 (self)
+               419         676 LOAD_FAST                0 (self)
                            678 LOAD_METHOD              2 (winfo_width)
                            700 PRECALL                  0
                            704 CALL                     0
                            714 LOAD_CONST               3 (1)
                            716 BINARY_OP               10 (-)
                            720 LOAD_FAST                0 (self)
                            722 LOAD_ATTR                4 (entry_radius)
                            732 LOAD_CONST               8 (5)
                            734 BINARY_OP               11 (/)
                            738 BINARY_OP               10 (-)
                
-               448         742 LOAD_FAST                0 (self)
+               420         742 LOAD_FAST                0 (self)
                            744 LOAD_METHOD              3 (winfo_height)
                            766 PRECALL                  0
                            770 CALL                     0
                            780 LOAD_CONST               3 (1)
                            782 BINARY_OP               10 (-)
                
-               449         786 LOAD_FAST                0 (self)
+               421         786 LOAD_FAST                0 (self)
                            788 LOAD_ATTR               15 (_entry_bottom_line)
                            798 LOAD_FAST                0 (self)
                            800 LOAD_ATTR               15 (_entry_bottom_line)
                
-               450         810 LOAD_CONST               2 (0)
+               422         810 LOAD_CONST               2 (0)
                
-               445         812 KW_NAMES                 9
+               417         812 KW_NAMES                 9
                            814 PRECALL                  7
                            818 CALL                     7
                            828 LOAD_FAST                0 (self)
                            830 STORE_ATTR              16 (entry_bottom)
                
-               452         840 LOAD_FAST                0 (self)
+               424         840 LOAD_FAST                0 (self)
                            842 LOAD_ATTR               14 (_entry_bottom_width)
                            852 LOAD_CONST               2 (0)
                            854 COMPARE_OP               2 (==)
                            860 POP_JUMP_FORWARD_IF_FALSE    26 (to 914)
                
-               453         862 LOAD_FAST                0 (self)
+               425         862 LOAD_FAST                0 (self)
                            864 LOAD_METHOD              0 (delete)
                            886 LOAD_FAST                0 (self)
                            888 LOAD_ATTR               16 (entry_bottom)
                            898 PRECALL                  1
                            902 CALL                     1
                            912 POP_TOP
                
-               455     >>  914 LOAD_FAST                0 (self)
+               427     >>  914 LOAD_FAST                0 (self)
                            916 LOAD_METHOD             17 (tag_raise)
                            938 LOAD_FAST                0 (self)
                            940 LOAD_ATTR               16 (entry_bottom)
                            950 LOAD_FAST                0 (self)
                            952 LOAD_ATTR               12 (entry_text)
                            962 PRECALL                  2
                            966 CALL                     2
                            976 POP_TOP
                
-               457         978 LOAD_FAST                0 (self)
+               429         978 LOAD_FAST                0 (self)
                            980 LOAD_ATTR               11 (entry)
                            990 LOAD_METHOD             18 (configure)
                           1012 LOAD_FAST                0 (self)
                           1014 LOAD_ATTR                7 (_entry_back)
                           1024 LOAD_FAST                0 (self)
                           1026 LOAD_ATTR               19 (_entry_text_back)
                           1036 LOAD_FAST                0 (self)
@@ -3465,15 +3345,15 @@
                   ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_round_rect4', 'winfo_width', 'winfo_height', 'entry_radius', 'entry_border_width', '_entry_border', '_entry_back', 'entry_frame', 'create_window', 'entry_padding', 'entry', 'entry_text', 'create_rectangle', '_entry_bottom_width', '_entry_bottom_line', 'entry_bottom', 'tag_raise', 'configure', '_entry_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_draw'
-               firstlineno 423
+               firstlineno 395
                lnotab
                   0x02012a021801020102012c012c010c010c0118f9120a0e021801580158
                   0158010cfc1c0730013c0142012c01180102fb1c07160134024002
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -3481,42 +3361,42 @@
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               459           0 RESUME                   0
+               431           0 RESUME                   0
                
-               460           2 LOAD_FAST                0 (self)
+               432           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (entry_focusin_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_entry_back)
                
-               461          26 LOAD_FAST                0 (self)
+               433          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (entry_focusin_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_entry_border)
                
-               462          50 LOAD_FAST                0 (self)
+               434          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (entry_focusin_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_entry_text_back)
                
-               463          74 LOAD_FAST                0 (self)
+               435          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (entry_focusin_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_entry_bottom_line)
                
-               464          98 LOAD_FAST                0 (self)
+               436          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (entry_focusin_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_entry_bottom_width)
                
-               466         122 LOAD_FAST                0 (self)
+               438         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -3524,56 +3404,56 @@
                   None
                names      ('entry_focusin_back', '_entry_back', 'entry_focusin_border', '_entry_border', 'entry_focusin_text_back', '_entry_text_back', 'entry_focusin_bottom_line', '_entry_bottom_line', 'entry_focusin_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_focus'
-               firstlineno 459
+               firstlineno 431
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               468           0 RESUME                   0
+               440           0 RESUME                   0
                
-               469           2 LOAD_FAST                0 (self)
+               441           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (entry_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_entry_back)
                
-               470          26 LOAD_FAST                0 (self)
+               442          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (entry_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_entry_border)
                
-               471          50 LOAD_FAST                0 (self)
+               443          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (entry_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_entry_text_back)
                
-               472          74 LOAD_FAST                0 (self)
+               444          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (entry_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_entry_bottom_line)
                
-               473          98 LOAD_FAST                0 (self)
+               445          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (entry_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_entry_bottom_width)
                
-               475         122 LOAD_FAST                0 (self)
+               447         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -3581,66 +3461,66 @@
                   None
                names      ('entry_back', '_entry_back', 'entry_border', '_entry_border', 'entry_text_back', '_entry_text_back', 'entry_bottom_line', '_entry_bottom_line', 'entry_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_focusout'
-               firstlineno 468
+               firstlineno 440
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               477           0 RESUME                   0
+               449           0 RESUME                   0
                
-               478           2 LOAD_FAST                0 (self)
+               450           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_set)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('focus_set',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_click'
-               firstlineno 477
+               firstlineno 449
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064005300
-               480           0 RESUME                   0
+               452           0 RESUME                   0
                
-               481           2 LOAD_CONST               1 (True)
+               453           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                   True
                names      ('hover',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_hover'
-               firstlineno 480
+               firstlineno 452
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -3648,610 +3528,253 @@
                   00ab000000000000000000735a64017c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c006a0a00000000000000007c005f0b00000000000000007c00a0
                   0c00000000000000000000000000000000000000006400a6010000ab0100
                   0000000000000001006400530064005300
-               483           0 RESUME                   0
+               455           0 RESUME                   0
                
-               484           2 LOAD_FAST                0 (self)
+               456           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_get)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_JUMP_FORWARD_IF_TRUE    90 (to 222)
                
-               485          42 LOAD_CONST               1 (False)
+               457          42 LOAD_CONST               1 (False)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (hover)
                
-               486          56 LOAD_FAST                0 (self)
+               458          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (entry_back)
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_entry_back)
                
-               487          80 LOAD_FAST                0 (self)
+               459          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (entry_border)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               5 (_entry_border)
                
-               488         104 LOAD_FAST                0 (self)
+               460         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (entry_text_back)
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               7 (_entry_text_back)
                
-               489         128 LOAD_FAST                0 (self)
+               461         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                8 (entry_bottom_line)
                            140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               9 (_entry_bottom_line)
                
-               490         152 LOAD_FAST                0 (self)
+               462         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR               10 (entry_bottom_width)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR              11 (_entry_bottom_width)
                
-               492         176 LOAD_FAST                0 (self)
+               464         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD             12 (_draw)
                            200 LOAD_CONST               0 (None)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                
-               484     >>  222 LOAD_CONST               0 (None)
+               456     >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   False
                names      ('focus_get', 'hover', 'entry_back', '_entry_back', 'entry_border', '_entry_border', 'entry_text_back', '_entry_text_back', 'entry_bottom_line', '_entry_bottom_line', 'entry_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_hover_release'
-               firstlineno 483
+               firstlineno 455
                lnotab 0x020128010e01180118011801180118022ef8
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               494           0 RESUME                   0
+               466           0 RESUME                   0
                
-               495           2 LOAD_FAST                1 (font)
+               467           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               496           6 LOAD_FAST                0 (self)
+               468           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (entry_text_font)
                             18 RETURN_VALUE
                
-               498     >>   20 LOAD_FAST                1 (font)
+               470     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (entry_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('entry_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'font'
-               firstlineno 494
+               firstlineno 466
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               500           0 RESUME                   0
+               472           0 RESUME                   0
                
-               501           2 LOAD_FAST                0 (self)
+               473           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 500
+               firstlineno 472
                lnotab 0x0201
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 17
-               flags     : 3
-               code
-                  0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564066407640864066409640a640b640c640d640e9c0ea6
-                  010000ab010000000000000000010064005300
-               503           0 RESUME                   0
-               
-               504           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (palette)
-               
-               506          26 LOAD_CONST               1 (13)
-               
-               508          28 LOAD_CONST               2 ((6, 4))
-               
-               510          30 LOAD_CONST               3 ('#f3f3f3')
-               
-               511          32 LOAD_CONST               4 (1)
-               
-               512          34 LOAD_CONST               5 (0)
-               
-               514          36 LOAD_CONST               6 ('#eaeaea')
-               
-               515          38 LOAD_CONST               7 ('#fdfdfd')
-               
-               516          40 LOAD_CONST               8 ('#5f5f5f')
-               
-               517          42 LOAD_CONST               6 ('#eaeaea')
-               
-               519          44 LOAD_CONST               9 ('#e2e2e2')
-               
-               520          46 LOAD_CONST              10 ('#f9f9f9')
-               
-               521          48 LOAD_CONST              11 ('#1a1a1a')
-               
-               522          50 LOAD_CONST              12 ('#185fb4')
-               
-               523          52 LOAD_CONST              13 (2)
-               
-               505          54 LOAD_CONST              14 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
-                            56 BUILD_CONST_KEY_MAP     14
-               
-               504          58 PRECALL                  1
-                            62 CALL                     1
-                            72 POP_TOP
-                            74 LOAD_CONST               0 (None)
-                            76 RETURN_VALUE
-               consts
-                  None
-                  13
-                  (6, 4)
-                  '#f3f3f3'
-                  1
-                  0
-                  '#eaeaea'
-                  '#fdfdfd'
-                  '#5f5f5f'
-                  '#e2e2e2'
-                  '#f9f9f9'
-                  '#1a1a1a'
-                  '#185fb4'
-                  2
-                  ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
-               names      ('palette',)
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
-               name       'palette_light'
-               firstlineno 503
-               lnotab
-                  0x0201180202020202020102010202020102010201020202010201020102
-                  0102ee04ff
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 17
-               flags     : 3
-               code
-                  0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564066407640864096405640a6408640b640c640d9c0ea6
-                  010000ab010000000000000000010064005300
-               527           0 RESUME                   0
-               
-               528           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (palette)
-               
-               530          26 LOAD_CONST               1 (13)
-               
-               532          28 LOAD_CONST               2 ((3, 4))
-               
-               534          30 LOAD_CONST               3 ('#202020')
-               
-               535          32 LOAD_CONST               4 (1)
-               
-               537          34 LOAD_CONST               5 ('#454545')
-               
-               538          36 LOAD_CONST               6 ('#353535')
-               
-               539          38 LOAD_CONST               7 ('#cecece')
-               
-               540          40 LOAD_CONST               8 ('#ffffff')
-               
-               541          42 LOAD_CONST               9 (0)
-               
-               543          44 LOAD_CONST               5 ('#454545')
-               
-               544          46 LOAD_CONST              10 ('#2f2f2f')
-               
-               545          48 LOAD_CONST               8 ('#ffffff')
-               
-               546          50 LOAD_CONST              11 ('#4cc2ff')
-               
-               547          52 LOAD_CONST              12 (2)
-               
-               529          54 LOAD_CONST              13 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
-                            56 BUILD_CONST_KEY_MAP     14
-               
-               528          58 PRECALL                  1
-                            62 CALL                     1
-                            72 POP_TOP
-                            74 LOAD_CONST               0 (None)
-                            76 RETURN_VALUE
-               consts
-                  None
-                  13
-                  (3, 4)
-                  '#202020'
-                  1
-                  '#454545'
-                  '#353535'
-                  '#cecece'
-                  '#ffffff'
-                  0
-                  '#2f2f2f'
-                  '#4cc2ff'
-                  2
-                  ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
-               names      ('palette',)
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
-               name       'palette_dark'
-               firstlineno 527
-               lnotab
-                  0x0201180202020202020102020201020102010201020202010201020102
-                  0102ee04ff
-            code
-               argcount  : 2
-               nlocals   : 2
-               stacksize : 11
-               flags     : 3
-               code
-                  0x97007c0181df7c016401190000000000000000007c005f000000000000
-                  0000007c016402190000000000000000007c005f0100000000000000007c
-                  016403190000000000000000007c005f0200000000000000007c01640419
-                  0000000000000000007c005f0300000000000000007c0164051900000000
-                  00000000007c005f0400000000000000007c016406190000000000000000
-                  007c005f0500000000000000007c016407190000000000000000007c005f
-                  0600000000000000007c016408190000000000000000007c005f07000000
-                  00000000007c016409190000000000000000007c005f0800000000000000
-                  007c01640a190000000000000000007c005f0900000000000000007c0164
-                  0b190000000000000000007c005f0a00000000000000007c01640c190000
-                  000000000000007c005f0b00000000000000007c01640d19000000000000
-                  0000007c005f0c00000000000000007c01640e190000000000000000007c
-                  005f0d000000000000000009007c00a00e00000000000000000000000000
-                  000000000000006400a6010000ab01000000000000000001006400530023
-                  00741e000000000000000000002400720401005900640053007700780359
-                  0077017c006a0100000000000000007c006a0200000000000000007c006a
-                  0300000000000000007c006a0800000000000000007c006a040000000000
-                  0000007c006a0500000000000000007c006a0600000000000000007c006a
-                  0900000000000000007c006a0a00000000000000007c006a0b0000000000
-                  000000640f9c0a5300
-               551           0 RESUME                   0
-               
-               552           2 LOAD_FAST                1 (dict)
-                             4 POP_JUMP_FORWARD_IF_NONE   223 (to 452)
-               
-               553           6 LOAD_FAST                1 (dict)
-                             8 LOAD_CONST               1 ('entry_radius')
-                            10 BINARY_SUBSCR
-                            20 LOAD_FAST                0 (self)
-                            22 STORE_ATTR               0 (entry_radius)
-               
-               555          32 LOAD_FAST                1 (dict)
-                            34 LOAD_CONST               2 ('entry_padding')
-                            36 BINARY_SUBSCR
-                            46 LOAD_FAST                0 (self)
-                            48 STORE_ATTR               1 (entry_padding)
-               
-               557          58 LOAD_FAST                1 (dict)
-                            60 LOAD_CONST               3 ('entry_frame_back')
-                            62 BINARY_SUBSCR
-                            72 LOAD_FAST                0 (self)
-                            74 STORE_ATTR               2 (entry_frame_back)
-               
-               558          84 LOAD_FAST                1 (dict)
-                            86 LOAD_CONST               4 ('entry_border_width')
-                            88 BINARY_SUBSCR
-                            98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               3 (entry_border_width)
-               
-               560         110 LOAD_FAST                1 (dict)
-                           112 LOAD_CONST               5 ('entry_border')
-                           114 BINARY_SUBSCR
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               4 (entry_border)
-               
-               561         136 LOAD_FAST                1 (dict)
-                           138 LOAD_CONST               6 ('entry_back')
-                           140 BINARY_SUBSCR
-                           150 LOAD_FAST                0 (self)
-                           152 STORE_ATTR               5 (entry_back)
-               
-               562         162 LOAD_FAST                1 (dict)
-                           164 LOAD_CONST               7 ('entry_text_back')
-                           166 BINARY_SUBSCR
-                           176 LOAD_FAST                0 (self)
-                           178 STORE_ATTR               6 (entry_text_back)
-               
-               563         188 LOAD_FAST                1 (dict)
-                           190 LOAD_CONST               8 ('entry_bottom_line')
-                           192 BINARY_SUBSCR
-                           202 LOAD_FAST                0 (self)
-                           204 STORE_ATTR               7 (entry_bottom_line)
-               
-               564         214 LOAD_FAST                1 (dict)
-                           216 LOAD_CONST               9 ('entry_bottom_width')
-                           218 BINARY_SUBSCR
-                           228 LOAD_FAST                0 (self)
-                           230 STORE_ATTR               8 (entry_bottom_width)
-               
-               566         240 LOAD_FAST                1 (dict)
-                           242 LOAD_CONST              10 ('entry_focusin_border')
-                           244 BINARY_SUBSCR
-                           254 LOAD_FAST                0 (self)
-                           256 STORE_ATTR               9 (entry_focusin_border)
-               
-               567         266 LOAD_FAST                1 (dict)
-                           268 LOAD_CONST              11 ('entry_focusin_back')
-                           270 BINARY_SUBSCR
-                           280 LOAD_FAST                0 (self)
-                           282 STORE_ATTR              10 (entry_focusin_back)
-               
-               568         292 LOAD_FAST                1 (dict)
-                           294 LOAD_CONST              12 ('entry_focusin_text_back')
-                           296 BINARY_SUBSCR
-                           306 LOAD_FAST                0 (self)
-                           308 STORE_ATTR              11 (entry_focusin_text_back)
-               
-               569         318 LOAD_FAST                1 (dict)
-                           320 LOAD_CONST              13 ('entry_focusin_bottom_line')
-                           322 BINARY_SUBSCR
-                           332 LOAD_FAST                0 (self)
-                           334 STORE_ATTR              12 (entry_focusin_bottom_line)
-               
-               570         344 LOAD_FAST                1 (dict)
-                           346 LOAD_CONST              14 ('entry_focusin_bottom_width')
-                           348 BINARY_SUBSCR
-                           358 LOAD_FAST                0 (self)
-                           360 STORE_ATTR              13 (entry_focusin_bottom_width)
-               
-               572         370 NOP
-               
-               573         372 LOAD_FAST                0 (self)
-                           374 LOAD_METHOD             14 (_draw)
-                           396 LOAD_CONST               0 (None)
-                           398 PRECALL                  1
-                           402 CALL                     1
-                           412 POP_TOP
-                           414 LOAD_CONST               0 (None)
-                           416 RETURN_VALUE
-                       >>  418 PUSH_EXC_INFO
-               
-               574         420 LOAD_GLOBAL             30 (AttributeError)
-                           432 CHECK_EXC_MATCH
-                           434 POP_JUMP_FORWARD_IF_FALSE     4 (to 444)
-                           436 POP_TOP
-               
-               575         438 POP_EXCEPT
-                           440 LOAD_CONST               0 (None)
-                           442 RETURN_VALUE
-               
-               574     >>  444 RERAISE                  0
-                       >>  446 COPY                     3
-                           448 POP_EXCEPT
-                           450 RERAISE                  1
-               
-               578     >>  452 LOAD_FAST                0 (self)
-                           454 LOAD_ATTR                1 (entry_padding)
-               
-               580         464 LOAD_FAST                0 (self)
-                           466 LOAD_ATTR                2 (entry_frame_back)
-               
-               581         476 LOAD_FAST                0 (self)
-                           478 LOAD_ATTR                3 (entry_border_width)
-               
-               582         488 LOAD_FAST                0 (self)
-                           490 LOAD_ATTR                8 (entry_bottom_width)
-               
-               584         500 LOAD_FAST                0 (self)
-                           502 LOAD_ATTR                4 (entry_border)
-               
-               585         512 LOAD_FAST                0 (self)
-                           514 LOAD_ATTR                5 (entry_back)
-               
-               586         524 LOAD_FAST                0 (self)
-                           526 LOAD_ATTR                6 (entry_text_back)
-               
-               588         536 LOAD_FAST                0 (self)
-                           538 LOAD_ATTR                9 (entry_focusin_border)
-               
-               589         548 LOAD_FAST                0 (self)
-                           550 LOAD_ATTR               10 (entry_focusin_back)
-               
-               590         560 LOAD_FAST                0 (self)
-                           562 LOAD_ATTR               11 (entry_focusin_text_back)
-               
-               577         572 LOAD_CONST              15 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back'))
-                           574 BUILD_CONST_KEY_MAP     10
-                           576 RETURN_VALUE
-               ExceptionTable:
-                 372 to 412 -> 418 [0]
-                 418 to 436 -> 446 [1] lasti
-                 444 to 444 -> 446 [1] lasti
-               consts
-                  None
-                  'entry_radius'
-                  'entry_padding'
-                  'entry_frame_back'
-                  'entry_border_width'
-                  'entry_border'
-                  'entry_back'
-                  'entry_text_back'
-                  'entry_bottom_line'
-                  'entry_bottom_width'
-                  'entry_focusin_border'
-                  'entry_focusin_back'
-                  'entry_focusin_text_back'
-                  'entry_focusin_bottom_line'
-                  'entry_focusin_bottom_width'
-                  ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back')
-               names      ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width', '_draw', 'AttributeError')
-               varnames   ('self', 'dict')
-               freevars   ()
-               cellvars   ()
-               filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
-               name       'palette'
-               firstlineno 551
-               lnotab
-                  0x020104011a021a021a011a021a011a011a011a011a021a011a011a011a
-                  011a0202013001120106ff08040c020c010c010c020c010c010c020c010c
-                  010cf3
             (None,)
-         names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'float', 'int', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawBasicRoundEntry3'
-         firstlineno 410
-         lnotab 0x0c010a030603140606240809080908030803080b0e06060306180618
+         firstlineno 382
+         lnotab 0x0c010a030603080606240809080908030803080b0e06
       'AdwDrawBasicRoundEntry3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         594           0 RESUME                   0
+         476           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundEntry3')
                        8 STORE_NAME               2 (__qualname__)
          
-         595          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 595>)
+         477          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 477>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundEntry3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               595           0 RESUME                   0
+               477           0 RESUME                   0
                
-               596           2 LOAD_FAST                0 (self)
+               478           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 595
+               firstlineno 477
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawRoundEntry3'
-         firstlineno 594
+         firstlineno 476
          lnotab 0x0a01
       'AdwDrawRoundEntry3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         599           0 RESUME                   0
+         481           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkEntry3')
                        8 STORE_NAME               2 (__qualname__)
          
-         600          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 600>)
+         482          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 482>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkEntry3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               600           0 RESUME                   0
+               482           0 RESUME                   0
                
-               601           2 LOAD_FAST                0 (self)
+               483           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 600
+               firstlineno 482
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawRoundDarkEntry3'
-         firstlineno 599
+         firstlineno 481
          lnotab 0x0a01
       'AdwDrawRoundDarkEntry3'
       '__main__'
       ('Tk',)
       'Hello'
       ('text',)
       'x'
@@ -4262,10 +3785,10 @@
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c041c7f004d1c051c061c7f00341c051c051c7f00391c
-      051c050c010c021402180130021801300218013002180130021801300218
-      0130022ce9
+      0x00ff020110010c041c7f004e1c051c061c7f00171c051c051c5e1c051c
+      050c010c0214021801300218013002180130021801300218013002180130
+      022ce9
```

### Comparing `tkadw-0.1.5/tkadw/canvas/__pycache__/frame.cpython-311.pyc` & `tkadw-0.2.0/tkadw/canvas/__pycache__/frame.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,23 @@
 magic:    0xa70d0d0a
-moddate:  0x7f2a9564 (Fri Jun 23 05:15:43 2023 UTC)
-files sz: 8629
+moddate:  0xf04b9664 (Sat Jun 24 01:50:40 2023 UTC)
+files sz: 6326
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100020047
       006403840064046501a6030000ab0300000000000000005a040200470064
       05840064066504a6030000ab0300000000000000005a0502004700640784
       0064086504a6030000ab0300000000000000005a06020047006409840064
       0a6504a6030000ab0300000000000000005a0702004700640b8400640c65
       07a6030000ab0300000000000000005a0802004700640d8400640e6507a6
-      030000ab0300000000000000005a0902004700640f840064106504a60300
+      030000ab0300000000000000005a0902004700640f840064106507a60300
       00ab0300000000000000005a0a02004700641184006412650aa6030000ab
       0300000000000000005a0b02004700641384006414650aa6030000ab0300
       000000000000005a0c650d64156b020000000090017204640064166c026d
       0e5a0e01000200650ea6000000ab0000000000000000005a0f02006506a6
       000000ab0000000000000000005a106510a0110000000000000000000000
       00000000000000000064176418ac19a6020000ab02000000000000000001
       000200650665106a100000000000000000a6010000ab0100000000000000
@@ -57,224 +57,224 @@
                 32 MAKE_FUNCTION            0
                 34 LOAD_CONST               4 ('AdwDrawBasicFrame')
                 36 LOAD_NAME                1 (AdwDrawEngine)
                 38 PRECALL                  3
                 42 CALL                     3
                 52 STORE_NAME               4 (AdwDrawBasicFrame)
    
-    85          54 PUSH_NULL
+    82          54 PUSH_NULL
                 56 LOAD_BUILD_CLASS
-                58 LOAD_CONST               5 (<code object AdwDrawFrame, file "D:\tkadw\tkadw\canvas\frame.py", line 85>)
+                58 LOAD_CONST               5 (<code object AdwDrawFrame, file "D:\tkadw\tkadw\canvas\frame.py", line 82>)
                 60 MAKE_FUNCTION            0
                 62 LOAD_CONST               6 ('AdwDrawFrame')
                 64 LOAD_NAME                4 (AdwDrawBasicFrame)
                 66 PRECALL                  3
                 70 CALL                     3
                 80 STORE_NAME               5 (AdwDrawFrame)
    
-    90          82 PUSH_NULL
+    87          82 PUSH_NULL
                 84 LOAD_BUILD_CLASS
-                86 LOAD_CONST               7 (<code object AdwDrawDarkFrame, file "D:\tkadw\tkadw\canvas\frame.py", line 90>)
+                86 LOAD_CONST               7 (<code object AdwDrawDarkFrame, file "D:\tkadw\tkadw\canvas\frame.py", line 87>)
                 88 MAKE_FUNCTION            0
                 90 LOAD_CONST               8 ('AdwDrawDarkFrame')
                 92 LOAD_NAME                4 (AdwDrawBasicFrame)
                 94 PRECALL                  3
                 98 CALL                     3
                108 STORE_NAME               6 (AdwDrawDarkFrame)
    
-    95         110 PUSH_NULL
+    92         110 PUSH_NULL
                112 LOAD_BUILD_CLASS
-               114 LOAD_CONST               9 (<code object AdwDrawBasicRoundFrame, file "D:\tkadw\tkadw\canvas\frame.py", line 95>)
+               114 LOAD_CONST               9 (<code object AdwDrawBasicRoundFrame, file "D:\tkadw\tkadw\canvas\frame.py", line 92>)
                116 MAKE_FUNCTION            0
                118 LOAD_CONST              10 ('AdwDrawBasicRoundFrame')
                120 LOAD_NAME                4 (AdwDrawBasicFrame)
                122 PRECALL                  3
                126 CALL                     3
                136 STORE_NAME               7 (AdwDrawBasicRoundFrame)
    
-   173         138 PUSH_NULL
+   150         138 PUSH_NULL
                140 LOAD_BUILD_CLASS
-               142 LOAD_CONST              11 (<code object AdwDrawRoundFrame, file "D:\tkadw\tkadw\canvas\frame.py", line 173>)
+               142 LOAD_CONST              11 (<code object AdwDrawRoundFrame, file "D:\tkadw\tkadw\canvas\frame.py", line 150>)
                144 MAKE_FUNCTION            0
                146 LOAD_CONST              12 ('AdwDrawRoundFrame')
                148 LOAD_NAME                7 (AdwDrawBasicRoundFrame)
                150 PRECALL                  3
                154 CALL                     3
                164 STORE_NAME               8 (AdwDrawRoundFrame)
    
-   178         166 PUSH_NULL
+   155         166 PUSH_NULL
                168 LOAD_BUILD_CLASS
-               170 LOAD_CONST              13 (<code object AdwDrawDarkRoundFrame, file "D:\tkadw\tkadw\canvas\frame.py", line 178>)
+               170 LOAD_CONST              13 (<code object AdwDrawDarkRoundFrame, file "D:\tkadw\tkadw\canvas\frame.py", line 155>)
                172 MAKE_FUNCTION            0
                174 LOAD_CONST              14 ('AdwDrawDarkRoundFrame')
                176 LOAD_NAME                7 (AdwDrawBasicRoundFrame)
                178 PRECALL                  3
                182 CALL                     3
                192 STORE_NAME               9 (AdwDrawDarkRoundFrame)
    
-   183         194 PUSH_NULL
+   160         194 PUSH_NULL
                196 LOAD_BUILD_CLASS
-               198 LOAD_CONST              15 (<code object AdwDrawBasicRoundFrame3, file "D:\tkadw\tkadw\canvas\frame.py", line 183>)
+               198 LOAD_CONST              15 (<code object AdwDrawBasicRoundFrame3, file "D:\tkadw\tkadw\canvas\frame.py", line 160>)
                200 MAKE_FUNCTION            0
                202 LOAD_CONST              16 ('AdwDrawBasicRoundFrame3')
-               204 LOAD_NAME                4 (AdwDrawBasicFrame)
+               204 LOAD_NAME                7 (AdwDrawBasicRoundFrame)
                206 PRECALL                  3
                210 CALL                     3
                220 STORE_NAME              10 (AdwDrawBasicRoundFrame3)
    
-   265         222 PUSH_NULL
+   193         222 PUSH_NULL
                224 LOAD_BUILD_CLASS
-               226 LOAD_CONST              17 (<code object AdwDrawRoundFrame3, file "D:\tkadw\tkadw\canvas\frame.py", line 265>)
+               226 LOAD_CONST              17 (<code object AdwDrawRoundFrame3, file "D:\tkadw\tkadw\canvas\frame.py", line 193>)
                228 MAKE_FUNCTION            0
                230 LOAD_CONST              18 ('AdwDrawRoundFrame3')
                232 LOAD_NAME               10 (AdwDrawBasicRoundFrame3)
                234 PRECALL                  3
                238 CALL                     3
                248 STORE_NAME              11 (AdwDrawRoundFrame3)
    
-   270         250 PUSH_NULL
+   198         250 PUSH_NULL
                252 LOAD_BUILD_CLASS
-               254 LOAD_CONST              19 (<code object AdwDrawDarkRoundFrame3, file "D:\tkadw\tkadw\canvas\frame.py", line 270>)
+               254 LOAD_CONST              19 (<code object AdwDrawDarkRoundFrame3, file "D:\tkadw\tkadw\canvas\frame.py", line 198>)
                256 MAKE_FUNCTION            0
                258 LOAD_CONST              20 ('AdwDrawDarkRoundFrame3')
                260 LOAD_NAME               10 (AdwDrawBasicRoundFrame3)
                262 PRECALL                  3
                266 CALL                     3
                276 STORE_NAME              12 (AdwDrawDarkRoundFrame3)
    
-   275         278 LOAD_NAME               13 (__name__)
+   203         278 LOAD_NAME               13 (__name__)
                280 LOAD_CONST              21 ('__main__')
                282 COMPARE_OP               2 (==)
                288 EXTENDED_ARG             1
                290 POP_JUMP_FORWARD_IF_FALSE   260 (to 812)
    
-   276         292 LOAD_CONST               0 (0)
+   204         292 LOAD_CONST               0 (0)
                294 LOAD_CONST              22 (('Tk',))
                296 IMPORT_NAME              2 (tkinter)
                298 IMPORT_FROM             14 (Tk)
                300 STORE_NAME              14 (Tk)
                302 POP_TOP
    
-   277         304 PUSH_NULL
+   205         304 PUSH_NULL
                306 LOAD_NAME               14 (Tk)
                308 PRECALL                  0
                312 CALL                     0
                322 STORE_NAME              15 (root)
    
-   279         324 PUSH_NULL
+   207         324 PUSH_NULL
                326 LOAD_NAME                6 (AdwDrawDarkFrame)
                328 PRECALL                  0
                332 CALL                     0
                342 STORE_NAME              16 (frame)
    
-   280         344 LOAD_NAME               16 (frame)
+   208         344 LOAD_NAME               16 (frame)
                346 LOAD_METHOD             17 (pack)
                368 LOAD_CONST              23 ('both')
                370 LOAD_CONST              24 ('yes')
                372 KW_NAMES                25
                374 PRECALL                  2
                378 CALL                     2
                388 POP_TOP
    
-   282         390 PUSH_NULL
+   210         390 PUSH_NULL
                392 LOAD_NAME                6 (AdwDrawDarkFrame)
                394 LOAD_NAME               16 (frame)
                396 LOAD_ATTR               16 (frame)
                406 PRECALL                  1
                410 CALL                     1
                420 STORE_NAME              18 (frame2)
    
-   283         422 LOAD_NAME               18 (frame2)
+   211         422 LOAD_NAME               18 (frame2)
                424 LOAD_METHOD             17 (pack)
                446 LOAD_CONST              23 ('both')
                448 LOAD_CONST              24 ('yes')
                450 LOAD_CONST              26 (8)
                452 LOAD_CONST              26 (8)
                454 KW_NAMES                27
                456 PRECALL                  4
                460 CALL                     4
                470 POP_TOP
    
-   285         472 PUSH_NULL
+   213         472 PUSH_NULL
                474 LOAD_NAME                9 (AdwDrawDarkRoundFrame)
                476 PRECALL                  0
                480 CALL                     0
                490 STORE_NAME              19 (frame3)
    
-   286         492 LOAD_NAME               19 (frame3)
+   214         492 LOAD_NAME               19 (frame3)
                494 LOAD_METHOD             17 (pack)
                516 LOAD_CONST              23 ('both')
                518 LOAD_CONST              24 ('yes')
                520 KW_NAMES                25
                522 PRECALL                  2
                526 CALL                     2
                536 POP_TOP
    
-   288         538 PUSH_NULL
+   216         538 PUSH_NULL
                540 LOAD_NAME                9 (AdwDrawDarkRoundFrame)
                542 LOAD_NAME               19 (frame3)
                544 LOAD_ATTR               16 (frame)
                554 PRECALL                  1
                558 CALL                     1
                568 STORE_NAME              20 (frame4)
    
-   289         570 LOAD_NAME               20 (frame4)
+   217         570 LOAD_NAME               20 (frame4)
                572 LOAD_METHOD             17 (pack)
                594 LOAD_CONST              23 ('both')
                596 LOAD_CONST              24 ('yes')
                598 LOAD_CONST              26 (8)
                600 LOAD_CONST              26 (8)
                602 KW_NAMES                27
                604 PRECALL                  4
                608 CALL                     4
                618 POP_TOP
    
-   291         620 PUSH_NULL
+   219         620 PUSH_NULL
                622 LOAD_NAME               12 (AdwDrawDarkRoundFrame3)
                624 PRECALL                  0
                628 CALL                     0
                638 STORE_NAME              21 (frame5)
    
-   292         640 LOAD_NAME               21 (frame5)
+   220         640 LOAD_NAME               21 (frame5)
                642 LOAD_METHOD             17 (pack)
                664 LOAD_CONST              23 ('both')
                666 LOAD_CONST              24 ('yes')
                668 KW_NAMES                25
                670 PRECALL                  2
                674 CALL                     2
                684 POP_TOP
    
-   294         686 PUSH_NULL
+   222         686 PUSH_NULL
                688 LOAD_NAME               12 (AdwDrawDarkRoundFrame3)
                690 LOAD_NAME               21 (frame5)
                692 LOAD_ATTR               16 (frame)
                702 PRECALL                  1
                706 CALL                     1
                716 STORE_NAME              22 (frame6)
    
-   295         718 LOAD_NAME               22 (frame6)
+   223         718 LOAD_NAME               22 (frame6)
                720 LOAD_METHOD             17 (pack)
                742 LOAD_CONST              23 ('both')
                744 LOAD_CONST              24 ('yes')
                746 LOAD_CONST              26 (8)
                748 LOAD_CONST              26 (8)
                750 KW_NAMES                27
                752 PRECALL                  4
                756 CALL                     4
                766 POP_TOP
    
-   297         768 LOAD_NAME               15 (root)
+   225         768 LOAD_NAME               15 (root)
                770 LOAD_METHOD             23 (mainloop)
                792 PRECALL                  0
                796 CALL                     0
                806 POP_TOP
                808 LOAD_CONST              28 (None)
                810 RETURN_VALUE
    
-   275     >>  812 LOAD_CONST              28 (None)
+   203     >>  812 LOAD_CONST              28 (None)
                814 RETURN_VALUE
    consts
       0
       ('AdwDrawEngine',)
       ('Frame',)
       code
          argcount  : 0
@@ -315,20 +315,20 @@
                       44 MAKE_FUNCTION            0
                       46 STORE_NAME               6 (default_palette)
          
           43          48 LOAD_CONST               7 (<code object palette_light, file "D:\tkadw\tkadw\canvas\frame.py", line 43>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               7 (palette_light)
          
-          53          54 LOAD_CONST               8 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\frame.py", line 53>)
+          54          54 LOAD_CONST               8 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\frame.py", line 54>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               8 (palette_dark)
          
-          64          60 LOAD_CONST              11 ((None,))
-                      62 LOAD_CONST              10 (<code object palette, file "D:\tkadw\tkadw\canvas\frame.py", line 64>)
+          65          60 LOAD_CONST              11 ((None,))
+                      62 LOAD_CONST              10 (<code object palette, file "D:\tkadw\tkadw\canvas\frame.py", line 65>)
                       64 MAKE_FUNCTION            1 (defaults)
                       66 STORE_NAME               9 (palette)
                       68 LOAD_CLOSURE             0 (__class__)
                       70 COPY                     1
                       72 STORE_NAME              10 (__classcell__)
                       74 RETURN_VALUE
          consts
@@ -610,370 +610,372 @@
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 7
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  026403640464059c04a6010000ab010000000000000000010064005300
+                  026403640464059c036901a6010000ab0100000000000000000100640053
+                  00
                 43           0 RESUME                   0
                
                 44           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                46          26 LOAD_CONST               1 ('#f3f3f3')
+                46          26 LOAD_CONST               1 ('frame')
                
-                47          28 LOAD_CONST               2 (2)
+                47          28 LOAD_CONST               2 ('#ffffff')
                
                 48          30 LOAD_CONST               3 ('#eaeaea')
                
-                49          32 LOAD_CONST               4 ('#ffffff')
+                49          32 LOAD_CONST               4 (2)
                
-                45          34 LOAD_CONST               5 (('frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back'))
-                            36 BUILD_CONST_KEY_MAP      4
+                46          34 LOAD_CONST               5 (('back', 'border', 'border_width'))
+                            36 BUILD_CONST_KEY_MAP      3
                
-                44          38 PRECALL                  1
-                            42 CALL                     1
-                            52 POP_TOP
-                            54 LOAD_CONST               0 (None)
-                            56 RETURN_VALUE
+                45          38 BUILD_MAP                1
+               
+                44          40 PRECALL                  1
+                            44 CALL                     1
+                            54 POP_TOP
+                            56 LOAD_CONST               0 (None)
+                            58 RETURN_VALUE
                consts
                   None
-                  '#f3f3f3'
-                  2
-                  '#eaeaea'
+                  'frame'
                   '#ffffff'
-                  ('frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back')
+                  '#eaeaea'
+                  2
+                  ('back', 'border', 'border_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'palette_light'
                firstlineno 43
-               lnotab 0x0201180202010201020102fc04ff
+               lnotab 0x0201180202010201020102fd04ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 7
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  026401640364049c04a6010000ab010000000000000000010064005300
-                53           0 RESUME                   0
+                  026403640464059c036901a6010000ab0100000000000000000100640053
+                  00
+                54           0 RESUME                   0
                
-                54           2 LOAD_FAST                0 (self)
+                55           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                56          26 LOAD_CONST               1 ('#333333')
+                57          26 LOAD_CONST               1 ('frame')
                
-                57          28 LOAD_CONST               2 (2)
+                58          28 LOAD_CONST               2 ('#0f0f0f')
                
-                58          30 LOAD_CONST               1 ('#333333')
+                59          30 LOAD_CONST               3 ('#333333')
                
-                59          32 LOAD_CONST               3 ('#0f0f0f')
+                60          32 LOAD_CONST               4 (2)
                
-                55          34 LOAD_CONST               4 (('frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back'))
-                            36 BUILD_CONST_KEY_MAP      4
+                57          34 LOAD_CONST               5 (('back', 'border', 'border_width'))
+                            36 BUILD_CONST_KEY_MAP      3
                
-                54          38 PRECALL                  1
-                            42 CALL                     1
-                            52 POP_TOP
-                            54 LOAD_CONST               0 (None)
-                            56 RETURN_VALUE
+                56          38 BUILD_MAP                1
+               
+                55          40 PRECALL                  1
+                            44 CALL                     1
+                            54 POP_TOP
+                            56 LOAD_CONST               0 (None)
+                            58 RETURN_VALUE
                consts
                   None
+                  'frame'
+                  '#0f0f0f'
                   '#333333'
                   2
-                  '#0f0f0f'
-                  ('frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back')
+                  ('back', 'border', 'border_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'palette_dark'
-               firstlineno 53
-               lnotab 0x0201180202010201020102fc04ff
+               firstlineno 54
+               lnotab 0x0201180202010201020102fd04ff02ff
             None
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 5
+               stacksize : 4
                flags     : 3
                code
-                  0x97007c01815d7c016401190000000000000000007c005f000000000000
-                  0000007c016402190000000000000000007c005f0100000000000000007c
-                  016403190000000000000000007c005f0200000000000000007c01640419
-                  0000000000000000007c005f03000000000000000009007c00a004000000
-                  00000000000000000000000000000000006400a6010000ab010000000000
-                  0000000100640053002300740a0000000000000000000024007204010059
-                  006400530077007803590077017c006a0000000000000000007c006a0100
-                  000000000000007c006a0200000000000000007c006a0300000000000000
-                  0064059c045300
-                64           0 RESUME                   0
-               
-                65           2 LOAD_FAST                1 (dict)
-                             4 POP_JUMP_FORWARD_IF_NONE    93 (to 192)
-               
-                66           6 LOAD_FAST                1 (dict)
-                             8 LOAD_CONST               1 ('frame_frame_back')
-                            10 BINARY_SUBSCR
-                            20 LOAD_FAST                0 (self)
-                            22 STORE_ATTR               0 (frame_frame_back)
-               
-                67          32 LOAD_FAST                1 (dict)
-                            34 LOAD_CONST               2 ('frame_border_width')
-                            36 BINARY_SUBSCR
-                            46 LOAD_FAST                0 (self)
-                            48 STORE_ATTR               1 (frame_border_width)
-               
-                68          58 LOAD_FAST                1 (dict)
-                            60 LOAD_CONST               3 ('frame_border')
-                            62 BINARY_SUBSCR
-                            72 LOAD_FAST                0 (self)
-                            74 STORE_ATTR               2 (frame_border)
-               
-                69          84 LOAD_FAST                1 (dict)
-                            86 LOAD_CONST               4 ('frame_back')
-                            88 BINARY_SUBSCR
-                            98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               3 (frame_back)
-               
-                71         110 NOP
-               
-                72         112 LOAD_FAST                0 (self)
-                           114 LOAD_METHOD              4 (_draw)
-                           136 LOAD_CONST               0 (None)
-                           138 PRECALL                  1
-                           142 CALL                     1
-                           152 POP_TOP
-                           154 LOAD_CONST               0 (None)
-                           156 RETURN_VALUE
-                       >>  158 PUSH_EXC_INFO
-               
-                73         160 LOAD_GLOBAL             10 (AttributeError)
-                           172 CHECK_EXC_MATCH
-                           174 POP_JUMP_FORWARD_IF_FALSE     4 (to 184)
-                           176 POP_TOP
-               
-                74         178 POP_EXCEPT
-                           180 LOAD_CONST               0 (None)
-                           182 RETURN_VALUE
-               
-                73     >>  184 RERAISE                  0
-                       >>  186 COPY                     3
-                           188 POP_EXCEPT
-                           190 RERAISE                  1
-               
-                77     >>  192 LOAD_FAST                0 (self)
-                           194 LOAD_ATTR                0 (frame_frame_back)
-               
-                78         204 LOAD_FAST                0 (self)
-                           206 LOAD_ATTR                1 (frame_border_width)
-               
-                80         216 LOAD_FAST                0 (self)
-                           218 LOAD_ATTR                2 (frame_border)
-               
-                81         228 LOAD_FAST                0 (self)
-                           230 LOAD_ATTR                3 (frame_back)
-               
-                76         240 LOAD_CONST               5 (('frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back'))
-                           242 BUILD_CONST_KEY_MAP      4
-                           244 RETURN_VALUE
+                  0x97007c01816d64017c01760072397c0164011900000000000000000064
+                  02190000000000000000007c005f0000000000000000007c016401190000
+                  000000000000006403190000000000000000007c005f0100000000000000
+                  007c016401190000000000000000006404190000000000000000007c005f
+                  0200000000000000007c017c005f03000000000000000009007c00a00400
+                  000000000000000000000000000000000000006400a6010000ab01000000
+                  00000000000100640053002300740a000000000000000000002400720401
+                  0059006400530077007803590077017c006a0300000000000000005300
+                65           0 RESUME                   0
+               
+                66           2 LOAD_FAST                1 (dict)
+                             4 POP_JUMP_FORWARD_IF_NONE   109 (to 224)
+               
+                67           6 LOAD_CONST               1 ('frame')
+                             8 LOAD_FAST                1 (dict)
+                            10 CONTAINS_OP              0
+                            12 POP_JUMP_FORWARD_IF_FALSE    57 (to 128)
+               
+                68          14 LOAD_FAST                1 (dict)
+                            16 LOAD_CONST               1 ('frame')
+                            18 BINARY_SUBSCR
+                            28 LOAD_CONST               2 ('back')
+                            30 BINARY_SUBSCR
+                            40 LOAD_FAST                0 (self)
+                            42 STORE_ATTR               0 (frame_back)
+               
+                69          52 LOAD_FAST                1 (dict)
+                            54 LOAD_CONST               1 ('frame')
+                            56 BINARY_SUBSCR
+                            66 LOAD_CONST               3 ('border')
+                            68 BINARY_SUBSCR
+                            78 LOAD_FAST                0 (self)
+                            80 STORE_ATTR               1 (frame_border)
+               
+                70          90 LOAD_FAST                1 (dict)
+                            92 LOAD_CONST               1 ('frame')
+                            94 BINARY_SUBSCR
+                           104 LOAD_CONST               4 ('border_width')
+                           106 BINARY_SUBSCR
+                           116 LOAD_FAST                0 (self)
+                           118 STORE_ATTR               2 (frame_border_width)
+               
+                72     >>  128 LOAD_FAST                1 (dict)
+                           130 LOAD_FAST                0 (self)
+                           132 STORE_ATTR               3 (_palette)
+               
+                74         142 NOP
+               
+                75         144 LOAD_FAST                0 (self)
+                           146 LOAD_METHOD              4 (_draw)
+                           168 LOAD_CONST               0 (None)
+                           170 PRECALL                  1
+                           174 CALL                     1
+                           184 POP_TOP
+                           186 LOAD_CONST               0 (None)
+                           188 RETURN_VALUE
+                       >>  190 PUSH_EXC_INFO
+               
+                76         192 LOAD_GLOBAL             10 (AttributeError)
+                           204 CHECK_EXC_MATCH
+                           206 POP_JUMP_FORWARD_IF_FALSE     4 (to 216)
+                           208 POP_TOP
+               
+                77         210 POP_EXCEPT
+                           212 LOAD_CONST               0 (None)
+                           214 RETURN_VALUE
+               
+                76     >>  216 RERAISE                  0
+                       >>  218 COPY                     3
+                           220 POP_EXCEPT
+                           222 RERAISE                  1
+               
+                79     >>  224 LOAD_FAST                0 (self)
+                           226 LOAD_ATTR                3 (_palette)
+                           236 RETURN_VALUE
                ExceptionTable:
-                 112 to 152 -> 158 [0]
-                 158 to 176 -> 186 [1] lasti
-                 184 to 184 -> 186 [1] lasti
+                 144 to 184 -> 190 [0]
+                 190 to 208 -> 218 [1] lasti
+                 216 to 216 -> 218 [1] lasti
                consts
                   None
-                  'frame_frame_back'
-                  'frame_border_width'
-                  'frame_border'
-                  'frame_back'
-                  ('frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back')
-               names      ('frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back', '_draw', 'AttributeError')
+                  'frame'
+                  'back'
+                  'border'
+                  'border_width'
+               names      ('frame_back', 'frame_border', 'frame_border_width', '_palette', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'palette'
-               firstlineno 64
-               lnotab
-                  0x020104011a011a011a011a0202013001120106ff08040c010c020c010c
-                  fb
+               firstlineno 65
+               lnotab 0x0201040108012601260126020e0202013001120106ff0803
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_other', '_draw', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
          name       'AdwDrawBasicFrame'
          firstlineno 6
-         lnotab 0x0c01120d060306110603060a060b
+         lnotab 0x0c01120d060306110603060b060b
       'AdwDrawBasicFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          85           0 RESUME                   0
+          82           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawFrame')
                        8 STORE_NAME               2 (__qualname__)
          
-          86          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 86>)
+          83          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 83>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawFrame'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                86           0 RESUME                   0
+                83           0 RESUME                   0
                
-                87           2 LOAD_FAST                0 (self)
+                84           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 86
+               firstlineno 83
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
          name       'AdwDrawFrame'
-         firstlineno 85
+         firstlineno 82
          lnotab 0x0a01
       'AdwDrawFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          90           0 RESUME                   0
+          87           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkFrame')
                        8 STORE_NAME               2 (__qualname__)
          
-          91          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 91>)
+          88          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 88>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkFrame'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                91           0 RESUME                   0
+                88           0 RESUME                   0
                
-                92           2 LOAD_FAST                0 (self)
+                89           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 91
+               firstlineno 88
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
          name       'AdwDrawDarkFrame'
-         firstlineno 90
+         firstlineno 87
          lnotab 0x0a01
       'AdwDrawDarkFrame'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 2
+         stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
-            0384005a05640484005a06640584005a076408640784015a08880078015a
-            095300
+            0384005a05640484005a06640584005a07640888006601640784095a0888
+            0078015a095300
                        0 MAKE_CELL                0 (__class__)
          
-          95           2 RESUME                   0
+          92           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundFrame')
                       10 STORE_NAME               2 (__qualname__)
          
-          96          12 LOAD_CLOSURE             0 (__class__)
+          93          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\frame.py", line 96>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\frame.py", line 93>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         103          22 LOAD_CONST               2 (<code object _draw, file "D:\tkadw\tkadw\canvas\frame.py", line 103>)
+         100          22 LOAD_CONST               2 (<code object _draw, file "D:\tkadw\tkadw\canvas\frame.py", line 100>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_draw)
          
-         120          28 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 120>)
+         117          28 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 117>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               5 (default_palette)
          
-         123          34 LOAD_CONST               4 (<code object palette_light, file "D:\tkadw\tkadw\canvas\frame.py", line 123>)
+         120          34 LOAD_CONST               4 (<code object palette_light, file "D:\tkadw\tkadw\canvas\frame.py", line 120>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               6 (palette_light)
          
-         135          40 LOAD_CONST               5 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\frame.py", line 135>)
+         132          40 LOAD_CONST               5 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\frame.py", line 132>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               7 (palette_dark)
          
-         148          46 LOAD_CONST               8 ((None,))
-                      48 LOAD_CONST               7 (<code object palette, file "D:\tkadw\tkadw\canvas\frame.py", line 148>)
-                      50 MAKE_FUNCTION            1 (defaults)
-                      52 STORE_NAME               8 (palette)
-                      54 LOAD_CLOSURE             0 (__class__)
-                      56 COPY                     1
-                      58 STORE_NAME               9 (__classcell__)
-                      60 RETURN_VALUE
+         144          46 LOAD_CONST               8 ((None,))
+                      48 LOAD_CLOSURE             0 (__class__)
+                      50 BUILD_TUPLE              1
+                      52 LOAD_CONST               7 (<code object palette, file "D:\tkadw\tkadw\canvas\frame.py", line 144>)
+                      54 MAKE_FUNCTION            9 (defaults, closure)
+                      56 STORE_NAME               8 (palette)
+                      58 LOAD_CLOSURE             0 (__class__)
+                      60 COPY                     1
+                      62 STORE_NAME               9 (__classcell__)
+                      64 RETURN_VALUE
          consts
             'AdwDrawBasicRoundFrame'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
@@ -982,31 +984,31 @@
                   0000006a0100000000000000007c0169007c02a4018e01010009007c00a0
                   0200000000000000000000000000000000000000007c006a030000000000
                   000000a00400000000000000000000000000000000000000006401a60100
                   00ab010000000000000000ac02a6010000ab010000000000000000010064
                   00530023000100590064005300780359007701
                              0 COPY_FREE_VARS           1
                
-                96           2 RESUME                   0
+                93           2 RESUME                   0
                
-                97           4 PUSH_NULL
+                94           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
                             48 DICT_MERGE               1
                             50 CALL_FUNCTION_EX         1
                             52 POP_TOP
                
-                98          54 NOP
+                95          54 NOP
                
-                99          56 LOAD_FAST                0 (self)
+                96          56 LOAD_FAST                0 (self)
                             58 LOAD_METHOD              2 (configure)
                             80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                3 (master)
                             92 LOAD_METHOD              4 (cget)
                            114 LOAD_CONST               1 ('background')
                            116 PRECALL                  1
                            120 CALL                     1
@@ -1014,17 +1016,17 @@
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                            148 LOAD_CONST               0 (None)
                            150 RETURN_VALUE
                        >>  152 PUSH_EXC_INFO
                
-               100         154 POP_TOP
+                97         154 POP_TOP
                
-               101         156 POP_EXCEPT
+                98         156 POP_EXCEPT
                            158 LOAD_CONST               0 (None)
                            160 RETURN_VALUE
                        >>  162 COPY                     3
                            164 POP_EXCEPT
                            166 RERAISE                  1
                ExceptionTable:
                  56 to 146 -> 152 [0]
@@ -1035,15 +1037,15 @@
                   ('background',)
                names      ('super', '__init__', 'configure', 'master', 'cget')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       '__init__'
-               firstlineno 96
+               firstlineno 93
                lnotab 0x04013201020162010201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -1062,84 +1064,84 @@
                   00a0030000000000000000000000000000000000000000a6000000ab0000
                   0000000000000064057a0b00007c006a0900000000000000007c00a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   00000064067a0a00007c006a0500000000000000007a0a00007c00a00300
                   00000000000000000000000000000000000000a6000000ab000000000000
                   00000064067a0a00007c006a0500000000000000007a0a0000ac07a60500
                   00ab0500000000000000007c005f0c000000000000000064005300
-               103           0 RESUME                   0
+               100           0 RESUME                   0
                
-               104           2 LOAD_FAST                0 (self)
+               101           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               106          44 LOAD_FAST                0 (self)
+               103          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect2)
                
-               107          68 LOAD_CONST               2 (0)
+               104          68 LOAD_CONST               2 (0)
                             70 LOAD_CONST               2 (0)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_FAST                0 (self)
                            112 LOAD_METHOD              3 (winfo_height)
                            134 PRECALL                  0
                            138 CALL                     0
                            148 LOAD_FAST                0 (self)
                            150 LOAD_ATTR                4 (frame_radius)
                
-               108         160 LOAD_FAST                0 (self)
+               105         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                5 (frame_border_width)
                
-               109         172 LOAD_FAST                0 (self)
+               106         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                6 (frame_border)
                            184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                7 (frame_back)
                
-               106         196 KW_NAMES                 3
+               103         196 KW_NAMES                 3
                            198 PRECALL                  8
                            202 CALL                     8
                            212 LOAD_FAST                0 (self)
                            214 STORE_ATTR               8 (frame_frame)
                
-               112         224 LOAD_FAST                0 (self)
+               109         224 LOAD_FAST                0 (self)
                            226 LOAD_ATTR                9 (frame)
                            236 LOAD_METHOD             10 (configure)
                            258 LOAD_FAST                0 (self)
                            260 LOAD_ATTR                7 (frame_back)
                            270 LOAD_CONST               2 (0)
                            272 KW_NAMES                 4
                            274 PRECALL                  2
                            278 CALL                     2
                            288 POP_TOP
                
-               114         290 LOAD_FAST                0 (self)
+               111         290 LOAD_FAST                0 (self)
                            292 LOAD_METHOD             11 (create_window)
                
-               115         314 LOAD_FAST                0 (self)
+               112         314 LOAD_FAST                0 (self)
                            316 LOAD_METHOD              2 (winfo_width)
                            338 PRECALL                  0
                            342 CALL                     0
                            352 LOAD_CONST               5 (2)
                            354 BINARY_OP               11 (/)
                            358 LOAD_FAST                0 (self)
                            360 LOAD_METHOD              3 (winfo_height)
                            382 PRECALL                  0
                            386 CALL                     0
                            396 LOAD_CONST               5 (2)
                            398 BINARY_OP               11 (/)
                
-               116         402 LOAD_FAST                0 (self)
+               113         402 LOAD_FAST                0 (self)
                            404 LOAD_ATTR                9 (frame)
                
-               117         414 LOAD_FAST                0 (self)
+               114         414 LOAD_FAST                0 (self)
                            416 LOAD_METHOD              2 (winfo_width)
                            438 PRECALL                  0
                            442 CALL                     0
                            452 LOAD_CONST               6 (6)
                            454 BINARY_OP               10 (-)
                            458 LOAD_FAST                0 (self)
                            460 LOAD_ATTR                5 (frame_border_width)
@@ -1150,15 +1152,15 @@
                            502 CALL                     0
                            512 LOAD_CONST               6 (6)
                            514 BINARY_OP               10 (-)
                            518 LOAD_FAST                0 (self)
                            520 LOAD_ATTR                5 (frame_border_width)
                            530 BINARY_OP               10 (-)
                
-               114         534 KW_NAMES                 7
+               111         534 KW_NAMES                 7
                            536 PRECALL                  5
                            540 CALL                     5
                            550 LOAD_FAST                0 (self)
                            552 STORE_ATTR              12 (frame_f)
                            562 LOAD_CONST               0 (None)
                            564 RETURN_VALUE
                consts
@@ -1172,425 +1174,352 @@
                   ('window', 'width', 'height')
                names      ('delete', 'create_round_rect2', 'winfo_width', 'winfo_height', 'frame_radius', 'frame_border_width', 'frame_border', 'frame_back', 'frame_frame', 'frame', 'configure', 'create_window', 'frame_f')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       '_draw'
-               firstlineno 103
+               firstlineno 100
                lnotab 0x02012a0218015c010c0118fd1c064202180158010c0178fd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               120           0 RESUME                   0
+               117           0 RESUME                   0
                
-               121           2 LOAD_FAST                0 (self)
+               118           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 120
+               firstlineno 117
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 8
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564069c05a6010000ab0100000000000000000100640053
-                  00
-               123           0 RESUME                   0
+                  0264036404640564069c046901a6010000ab010000000000000000010064
+                  005300
+               120           0 RESUME                   0
                
-               124           2 LOAD_FAST                0 (self)
+               121           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               126          26 LOAD_CONST               1 (6)
+               123          26 LOAD_CONST               1 ('frame')
                
-               128          28 LOAD_CONST               2 ('#f3f3f3')
+               124          28 LOAD_CONST               2 (6)
                
-               129          30 LOAD_CONST               3 (2)
+               125          30 LOAD_CONST               3 ('#0f0f0f')
                
-               130          32 LOAD_CONST               4 ('#eaeaea')
+               126          32 LOAD_CONST               4 ('#333333')
                
-               131          34 LOAD_CONST               5 ('#ffffff')
+               127          34 LOAD_CONST               5 (2)
                
-               125          36 LOAD_CONST               6 (('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back'))
-                            38 BUILD_CONST_KEY_MAP      5
+               123          36 LOAD_CONST               6 (('radius', 'back', 'border', 'border_width'))
+                            38 BUILD_CONST_KEY_MAP      4
                
-               124          40 PRECALL                  1
-                            44 CALL                     1
-                            54 POP_TOP
-                            56 LOAD_CONST               0 (None)
-                            58 RETURN_VALUE
+               122          40 BUILD_MAP                1
+               
+               121          42 PRECALL                  1
+                            46 CALL                     1
+                            56 POP_TOP
+                            58 LOAD_CONST               0 (None)
+                            60 RETURN_VALUE
                consts
                   None
+                  'frame'
                   6
-                  '#f3f3f3'
+                  '#0f0f0f'
+                  '#333333'
                   2
-                  '#eaeaea'
-                  '#ffffff'
-                  ('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back')
+                  ('radius', 'back', 'border', 'border_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'palette_light'
-               firstlineno 123
-               lnotab 0x02011802020202010201020102fa04ff
+               firstlineno 120
+               lnotab 0x02011802020102010201020102fc04ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 8
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036402640464059c05a6010000ab0100000000000000000100640053
-                  00
-               135           0 RESUME                   0
+                  0264036404640564069c046901a6010000ab010000000000000000010064
+                  005300
+               132           0 RESUME                   0
                
-               136           2 LOAD_FAST                0 (self)
+               133           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               138          26 LOAD_CONST               1 (6)
+               135          26 LOAD_CONST               1 ('frame')
                
-               140          28 LOAD_CONST               2 ('#333333')
+               136          28 LOAD_CONST               2 (6)
                
-               141          30 LOAD_CONST               3 (2)
+               137          30 LOAD_CONST               3 ('#0f0f0f')
                
-               142          32 LOAD_CONST               2 ('#333333')
+               138          32 LOAD_CONST               4 ('#333333')
                
-               143          34 LOAD_CONST               4 ('#0f0f0f')
+               139          34 LOAD_CONST               5 (2)
                
-               137          36 LOAD_CONST               5 (('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back'))
-                            38 BUILD_CONST_KEY_MAP      5
+               135          36 LOAD_CONST               6 (('radius', 'back', 'border', 'border_width'))
+                            38 BUILD_CONST_KEY_MAP      4
                
-               136          40 PRECALL                  1
-                            44 CALL                     1
-                            54 POP_TOP
-                            56 LOAD_CONST               0 (None)
-                            58 RETURN_VALUE
+               134          40 BUILD_MAP                1
+               
+               133          42 PRECALL                  1
+                            46 CALL                     1
+                            56 POP_TOP
+                            58 LOAD_CONST               0 (None)
+                            60 RETURN_VALUE
                consts
                   None
+                  'frame'
                   6
+                  '#0f0f0f'
                   '#333333'
                   2
-                  '#0f0f0f'
-                  ('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back')
+                  ('radius', 'back', 'border', 'border_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'palette_dark'
-               firstlineno 135
-               lnotab 0x02011802020202010201020102fa04ff
+               firstlineno 132
+               lnotab 0x02011802020102010201020102fc04ff02ff
             None
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 6
+               stacksize : 3
                flags     : 3
                code
-                  0x97007c01816a7c016401190000000000000000007c005f000000000000
-                  0000007c016402190000000000000000007c005f0100000000000000007c
-                  016403190000000000000000007c005f0200000000000000007c01640419
-                  0000000000000000007c005f0300000000000000007c0164051900000000
-                  00000000007c005f04000000000000000009007c00a00500000000000000
-                  000000000000000000000000006400a6010000ab01000000000000000001
-                  00640053002300740c000000000000000000002400720401005900640053
-                  0077007803590077017c006a0000000000000000007c006a010000000000
-                  0000007c006a0200000000000000007c006a0300000000000000007c006a
-                  04000000000000000064069c055300
-               148           0 RESUME                   0
-               
-               149           2 LOAD_FAST                1 (dict)
-                             4 POP_JUMP_FORWARD_IF_NONE   106 (to 218)
-               
-               150           6 LOAD_FAST                1 (dict)
-                             8 LOAD_CONST               1 ('frame_radius')
-                            10 BINARY_SUBSCR
-                            20 LOAD_FAST                0 (self)
-                            22 STORE_ATTR               0 (frame_radius)
-               
-               152          32 LOAD_FAST                1 (dict)
-                            34 LOAD_CONST               2 ('frame_frame_back')
-                            36 BINARY_SUBSCR
-                            46 LOAD_FAST                0 (self)
-                            48 STORE_ATTR               1 (frame_frame_back)
-               
-               153          58 LOAD_FAST                1 (dict)
-                            60 LOAD_CONST               3 ('frame_border_width')
-                            62 BINARY_SUBSCR
-                            72 LOAD_FAST                0 (self)
-                            74 STORE_ATTR               2 (frame_border_width)
+                  0x95019700740100000000000000000000a6000000ab0000000000000000
+                  00a00100000000000000000000000000000000000000007c01a6010000ab
+                  010000000000000000010064017c01760072157c01640119000000000000
+                  0000006402190000000000000000007c005f020000000000000000640053
+                  0064005300
+                             0 COPY_FREE_VARS           1
                
-               154          84 LOAD_FAST                1 (dict)
-                            86 LOAD_CONST               4 ('frame_border')
-                            88 BINARY_SUBSCR
-                            98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               3 (frame_border)
-               
-               155         110 LOAD_FAST                1 (dict)
-                           112 LOAD_CONST               5 ('frame_back')
-                           114 BINARY_SUBSCR
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               4 (frame_back)
-               
-               157         136 NOP
-               
-               158         138 LOAD_FAST                0 (self)
-                           140 LOAD_METHOD              5 (_draw)
-                           162 LOAD_CONST               0 (None)
-                           164 PRECALL                  1
-                           168 CALL                     1
-                           178 POP_TOP
-                           180 LOAD_CONST               0 (None)
-                           182 RETURN_VALUE
-                       >>  184 PUSH_EXC_INFO
-               
-               159         186 LOAD_GLOBAL             12 (AttributeError)
-                           198 CHECK_EXC_MATCH
-                           200 POP_JUMP_FORWARD_IF_FALSE     4 (to 210)
-                           202 POP_TOP
-               
-               160         204 POP_EXCEPT
-                           206 LOAD_CONST               0 (None)
-                           208 RETURN_VALUE
-               
-               159     >>  210 RERAISE                  0
-                       >>  212 COPY                     3
-                           214 POP_EXCEPT
-                           216 RERAISE                  1
-               
-               163     >>  218 LOAD_FAST                0 (self)
-                           220 LOAD_ATTR                0 (frame_radius)
-               
-               165         230 LOAD_FAST                0 (self)
-                           232 LOAD_ATTR                1 (frame_frame_back)
-               
-               166         242 LOAD_FAST                0 (self)
-                           244 LOAD_ATTR                2 (frame_border_width)
-               
-               168         254 LOAD_FAST                0 (self)
-                           256 LOAD_ATTR                3 (frame_border)
-               
-               169         266 LOAD_FAST                0 (self)
-                           268 LOAD_ATTR                4 (frame_back)
-               
-               162         278 LOAD_CONST               6 (('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back'))
-                           280 BUILD_CONST_KEY_MAP      5
-                           282 RETURN_VALUE
-               ExceptionTable:
-                 138 to 178 -> 184 [0]
-                 184 to 202 -> 212 [1] lasti
-                 210 to 210 -> 212 [1] lasti
-               consts
-                  None
-                  'frame_radius'
-                  'frame_frame_back'
-                  'frame_border_width'
-                  'frame_border'
-                  'frame_back'
-                  ('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back')
-               names      ('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back', '_draw', 'AttributeError')
+               144           2 RESUME                   0
+               
+               145           4 LOAD_GLOBAL              1 (NULL + super)
+                            16 PRECALL                  0
+                            20 CALL                     0
+                            30 LOAD_METHOD              1 (palette)
+                            52 LOAD_FAST                1 (dict)
+                            54 PRECALL                  1
+                            58 CALL                     1
+                            68 POP_TOP
+               
+               146          70 LOAD_CONST               1 ('frame')
+                            72 LOAD_FAST                1 (dict)
+                            74 CONTAINS_OP              0
+                            76 POP_JUMP_FORWARD_IF_FALSE    21 (to 120)
+               
+               147          78 LOAD_FAST                1 (dict)
+                            80 LOAD_CONST               1 ('frame')
+                            82 BINARY_SUBSCR
+                            92 LOAD_CONST               2 ('radius')
+                            94 BINARY_SUBSCR
+                           104 LOAD_FAST                0 (self)
+                           106 STORE_ATTR               2 (frame_radius)
+                           116 LOAD_CONST               0 (None)
+                           118 RETURN_VALUE
+               
+               146     >>  120 LOAD_CONST               0 (None)
+                           122 RETURN_VALUE
+               consts
+                  None
+                  'frame'
+                  'radius'
+               names      ('super', 'palette', 'frame_radius')
                varnames   ('self', 'dict')
-               freevars   ()
+               freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'palette'
-               firstlineno 148
-               lnotab
-                  0x020104011a021a011a011a011a0202013001120106ff08040c020c010c
-                  020c010cf9
+               firstlineno 144
+               lnotab 0x0401420108012aff
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_draw', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
          name       'AdwDrawBasicRoundFrame'
-         firstlineno 95
-         lnotab 0x0c010a0706110603060c060d
+         firstlineno 92
+         lnotab 0x0c010a0706110603060c060c
       'AdwDrawBasicRoundFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         173           0 RESUME                   0
+         150           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundFrame')
                        8 STORE_NAME               2 (__qualname__)
          
-         174          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 174>)
+         151          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 151>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundFrame'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               174           0 RESUME                   0
+               151           0 RESUME                   0
                
-               175           2 LOAD_FAST                0 (self)
+               152           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 174
+               firstlineno 151
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
          name       'AdwDrawRoundFrame'
-         firstlineno 173
+         firstlineno 150
          lnotab 0x0a01
       'AdwDrawRoundFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         178           0 RESUME                   0
+         155           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkRoundFrame')
                        8 STORE_NAME               2 (__qualname__)
          
-         179          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 179>)
+         156          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 156>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkRoundFrame'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               179           0 RESUME                   0
+               156           0 RESUME                   0
                
-               180           2 LOAD_FAST                0 (self)
+               157           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 179
+               firstlineno 156
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
          name       'AdwDrawDarkRoundFrame'
-         firstlineno 178
+         firstlineno 155
          lnotab 0x0a01
       'AdwDrawDarkRoundFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
-            0384005a05640484005a06640584005a076408640784015a08880078015a
-            095300
+            0384005a05880078015a065300
                        0 MAKE_CELL                0 (__class__)
          
-         183           2 RESUME                   0
+         160           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundFrame3')
                       10 STORE_NAME               2 (__qualname__)
          
-         184          12 LOAD_CLOSURE             0 (__class__)
+         161          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\frame.py", line 184>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\frame.py", line 161>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         191          22 LOAD_CONST               2 (<code object _draw, file "D:\tkadw\tkadw\canvas\frame.py", line 191>)
+         168          22 LOAD_CONST               2 (<code object _draw, file "D:\tkadw\tkadw\canvas\frame.py", line 168>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_draw)
          
-         212          28 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 212>)
+         189          28 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 189>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               5 (default_palette)
-         
-         215          34 LOAD_CONST               4 (<code object palette_light, file "D:\tkadw\tkadw\canvas\frame.py", line 215>)
-                      36 MAKE_FUNCTION            0
-                      38 STORE_NAME               6 (palette_light)
-         
-         227          40 LOAD_CONST               5 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\frame.py", line 227>)
-                      42 MAKE_FUNCTION            0
-                      44 STORE_NAME               7 (palette_dark)
-         
-         240          46 LOAD_CONST               8 ((None,))
-                      48 LOAD_CONST               7 (<code object palette, file "D:\tkadw\tkadw\canvas\frame.py", line 240>)
-                      50 MAKE_FUNCTION            1 (defaults)
-                      52 STORE_NAME               8 (palette)
-                      54 LOAD_CLOSURE             0 (__class__)
-                      56 COPY                     1
-                      58 STORE_NAME               9 (__classcell__)
-                      60 RETURN_VALUE
+                      34 LOAD_CLOSURE             0 (__class__)
+                      36 COPY                     1
+                      38 STORE_NAME               6 (__classcell__)
+                      40 RETURN_VALUE
          consts
             'AdwDrawBasicRoundFrame3'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
@@ -1599,31 +1528,31 @@
                   0000006a0100000000000000007c0169007c02a4018e01010009007c00a0
                   0200000000000000000000000000000000000000007c006a030000000000
                   000000a00400000000000000000000000000000000000000006401a60100
                   00ab010000000000000000ac02a6010000ab010000000000000000010064
                   00530023000100590064005300780359007701
                              0 COPY_FREE_VARS           1
                
-               184           2 RESUME                   0
+               161           2 RESUME                   0
                
-               185           4 PUSH_NULL
+               162           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
                             48 DICT_MERGE               1
                             50 CALL_FUNCTION_EX         1
                             52 POP_TOP
                
-               186          54 NOP
+               163          54 NOP
                
-               187          56 LOAD_FAST                0 (self)
+               164          56 LOAD_FAST                0 (self)
                             58 LOAD_METHOD              2 (configure)
                             80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                3 (master)
                             92 LOAD_METHOD              4 (cget)
                            114 LOAD_CONST               1 ('background')
                            116 PRECALL                  1
                            120 CALL                     1
@@ -1631,17 +1560,17 @@
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                            148 LOAD_CONST               0 (None)
                            150 RETURN_VALUE
                        >>  152 PUSH_EXC_INFO
                
-               188         154 POP_TOP
+               165         154 POP_TOP
                
-               189         156 POP_EXCEPT
+               166         156 POP_EXCEPT
                            158 LOAD_CONST               0 (None)
                            160 RETURN_VALUE
                        >>  162 COPY                     3
                            164 POP_EXCEPT
                            166 RERAISE                  1
                ExceptionTable:
                  56 to 146 -> 152 [0]
@@ -1652,15 +1581,15 @@
                   ('background',)
                names      ('super', '__init__', 'configure', 'master', 'cget')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       '__init__'
-               firstlineno 184
+               firstlineno 161
                lnotab 0x04013201020162010201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -1680,89 +1609,89 @@
                   00ab00000000000000000064067a0b00007c006a0900000000000000007c
                   00a0020000000000000000000000000000000000000000a6000000ab0000
                   0000000000000064077a0a00007c006a0500000000000000007a0a00007c
                   00a0030000000000000000000000000000000000000000a6000000ab0000
                   0000000000000064077a0a00007c006a0500000000000000007a0a0000ac
                   08a6050000ab0500000000000000007c005f0c0000000000000000640053
                   00
-               191           0 RESUME                   0
+               168           0 RESUME                   0
                
-               192           2 LOAD_FAST                0 (self)
+               169           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               194          44 LOAD_FAST                0 (self)
+               171          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
-               195          68 LOAD_CONST               2 (0)
+               172          68 LOAD_CONST               2 (0)
                             70 LOAD_CONST               2 (0)
                
-               196          72 LOAD_FAST                0 (self)
+               173          72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                
-               197         110 LOAD_FAST                0 (self)
+               174         110 LOAD_FAST                0 (self)
                            112 LOAD_METHOD              3 (winfo_height)
                            134 PRECALL                  0
                            138 CALL                     0
                            148 LOAD_FAST                0 (self)
                            150 LOAD_ATTR                4 (frame_radius)
                
-               198         160 LOAD_FAST                0 (self)
+               175         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                5 (frame_border_width)
                
-               199         172 LOAD_FAST                0 (self)
+               176         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                6 (frame_border)
                            184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                7 (frame_back)
                
-               194         196 KW_NAMES                 3
+               171         196 KW_NAMES                 3
                            198 PRECALL                  8
                            202 CALL                     8
                            212 POP_TOP
                
-               202         214 LOAD_CONST               4 ('button_frame')
+               179         214 LOAD_CONST               4 ('button_frame')
                            216 LOAD_FAST                0 (self)
                            218 STORE_ATTR               8 (entry_frame)
                
-               204         228 LOAD_FAST                0 (self)
+               181         228 LOAD_FAST                0 (self)
                            230 LOAD_ATTR                9 (frame)
                            240 LOAD_METHOD             10 (configure)
                            262 LOAD_FAST                0 (self)
                            264 LOAD_ATTR                7 (frame_back)
                            274 LOAD_CONST               2 (0)
                            276 KW_NAMES                 5
                            278 PRECALL                  2
                            282 CALL                     2
                            292 POP_TOP
                
-               206         294 LOAD_FAST                0 (self)
+               183         294 LOAD_FAST                0 (self)
                            296 LOAD_METHOD             11 (create_window)
                
-               207         318 LOAD_FAST                0 (self)
+               184         318 LOAD_FAST                0 (self)
                            320 LOAD_METHOD              2 (winfo_width)
                            342 PRECALL                  0
                            346 CALL                     0
                            356 LOAD_CONST               6 (2)
                            358 BINARY_OP               11 (/)
                            362 LOAD_FAST                0 (self)
                            364 LOAD_METHOD              3 (winfo_height)
                            386 PRECALL                  0
                            390 CALL                     0
                            400 LOAD_CONST               6 (2)
                            402 BINARY_OP               11 (/)
                
-               208         406 LOAD_FAST                0 (self)
+               185         406 LOAD_FAST                0 (self)
                            408 LOAD_ATTR                9 (frame)
                
-               209         418 LOAD_FAST                0 (self)
+               186         418 LOAD_FAST                0 (self)
                            420 LOAD_METHOD              2 (winfo_width)
                            442 PRECALL                  0
                            446 CALL                     0
                            456 LOAD_CONST               7 (6)
                            458 BINARY_OP               10 (-)
                            462 LOAD_FAST                0 (self)
                            464 LOAD_ATTR                5 (frame_border_width)
@@ -1773,15 +1702,15 @@
                            506 CALL                     0
                            516 LOAD_CONST               7 (6)
                            518 BINARY_OP               10 (-)
                            522 LOAD_FAST                0 (self)
                            524 LOAD_ATTR                5 (frame_border_width)
                            534 BINARY_OP               10 (-)
                
-               206         538 KW_NAMES                 8
+               183         538 KW_NAMES                 8
                            540 PRECALL                  5
                            544 CALL                     5
                            554 LOAD_FAST                0 (self)
                            556 STORE_ATTR              12 (frame_f)
                            566 LOAD_CONST               0 (None)
                            568 RETURN_VALUE
                consts
@@ -1796,378 +1725,164 @@
                   ('window', 'width', 'height')
                names      ('delete', 'create_round_rect4', 'winfo_width', 'winfo_height', 'frame_radius', 'frame_border_width', 'frame_border', 'frame_back', 'entry_frame', 'frame', 'configure', 'create_window', 'frame_f')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       '_draw'
-               firstlineno 191
+               firstlineno 168
                lnotab
                   0x02012a0218010401260132010c0118fb12080e024202180158010c0178
                   fd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               212           0 RESUME                   0
+               189           0 RESUME                   0
                
-               213           2 LOAD_FAST                0 (self)
+               190           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 212
+               firstlineno 189
                lnotab 0x0201
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 8
-               flags     : 3
-               code
-                  0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564069c05a6010000ab0100000000000000000100640053
-                  00
-               215           0 RESUME                   0
-               
-               216           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (palette)
-               
-               218          26 LOAD_CONST               1 (13)
-               
-               220          28 LOAD_CONST               2 ('#f3f3f3')
-               
-               221          30 LOAD_CONST               3 (2)
-               
-               222          32 LOAD_CONST               4 ('#eaeaea')
-               
-               223          34 LOAD_CONST               5 ('#ffffff')
-               
-               217          36 LOAD_CONST               6 (('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back'))
-                            38 BUILD_CONST_KEY_MAP      5
-               
-               216          40 PRECALL                  1
-                            44 CALL                     1
-                            54 POP_TOP
-                            56 LOAD_CONST               0 (None)
-                            58 RETURN_VALUE
-               consts
-                  None
-                  13
-                  '#f3f3f3'
-                  2
-                  '#eaeaea'
-                  '#ffffff'
-                  ('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back')
-               names      ('palette',)
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
-               name       'palette_light'
-               firstlineno 215
-               lnotab 0x02011802020202010201020102fa04ff
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 8
-               flags     : 3
-               code
-                  0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036402640464059c05a6010000ab0100000000000000000100640053
-                  00
-               227           0 RESUME                   0
-               
-               228           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (palette)
-               
-               230          26 LOAD_CONST               1 (13)
-               
-               232          28 LOAD_CONST               2 ('#333333')
-               
-               233          30 LOAD_CONST               3 (2)
-               
-               234          32 LOAD_CONST               2 ('#333333')
-               
-               235          34 LOAD_CONST               4 ('#0f0f0f')
-               
-               229          36 LOAD_CONST               5 (('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back'))
-                            38 BUILD_CONST_KEY_MAP      5
-               
-               228          40 PRECALL                  1
-                            44 CALL                     1
-                            54 POP_TOP
-                            56 LOAD_CONST               0 (None)
-                            58 RETURN_VALUE
-               consts
-                  None
-                  13
-                  '#333333'
-                  2
-                  '#0f0f0f'
-                  ('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back')
-               names      ('palette',)
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
-               name       'palette_dark'
-               firstlineno 227
-               lnotab 0x02011802020202010201020102fa04ff
-            None
-            code
-               argcount  : 2
-               nlocals   : 2
-               stacksize : 6
-               flags     : 3
-               code
-                  0x97007c01816a7c016401190000000000000000007c005f000000000000
-                  0000007c016402190000000000000000007c005f0100000000000000007c
-                  016403190000000000000000007c005f0200000000000000007c01640419
-                  0000000000000000007c005f0300000000000000007c0164051900000000
-                  00000000007c005f04000000000000000009007c00a00500000000000000
-                  000000000000000000000000006400a6010000ab01000000000000000001
-                  00640053002300740c000000000000000000002400720401005900640053
-                  0077007803590077017c006a0000000000000000007c006a010000000000
-                  0000007c006a0200000000000000007c006a0300000000000000007c006a
-                  04000000000000000064069c055300
-               240           0 RESUME                   0
-               
-               241           2 LOAD_FAST                1 (dict)
-                             4 POP_JUMP_FORWARD_IF_NONE   106 (to 218)
-               
-               242           6 LOAD_FAST                1 (dict)
-                             8 LOAD_CONST               1 ('frame_radius')
-                            10 BINARY_SUBSCR
-                            20 LOAD_FAST                0 (self)
-                            22 STORE_ATTR               0 (frame_radius)
-               
-               244          32 LOAD_FAST                1 (dict)
-                            34 LOAD_CONST               2 ('frame_frame_back')
-                            36 BINARY_SUBSCR
-                            46 LOAD_FAST                0 (self)
-                            48 STORE_ATTR               1 (frame_frame_back)
-               
-               245          58 LOAD_FAST                1 (dict)
-                            60 LOAD_CONST               3 ('frame_border_width')
-                            62 BINARY_SUBSCR
-                            72 LOAD_FAST                0 (self)
-                            74 STORE_ATTR               2 (frame_border_width)
-               
-               246          84 LOAD_FAST                1 (dict)
-                            86 LOAD_CONST               4 ('frame_border')
-                            88 BINARY_SUBSCR
-                            98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               3 (frame_border)
-               
-               247         110 LOAD_FAST                1 (dict)
-                           112 LOAD_CONST               5 ('frame_back')
-                           114 BINARY_SUBSCR
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               4 (frame_back)
-               
-               249         136 NOP
-               
-               250         138 LOAD_FAST                0 (self)
-                           140 LOAD_METHOD              5 (_draw)
-                           162 LOAD_CONST               0 (None)
-                           164 PRECALL                  1
-                           168 CALL                     1
-                           178 POP_TOP
-                           180 LOAD_CONST               0 (None)
-                           182 RETURN_VALUE
-                       >>  184 PUSH_EXC_INFO
-               
-               251         186 LOAD_GLOBAL             12 (AttributeError)
-                           198 CHECK_EXC_MATCH
-                           200 POP_JUMP_FORWARD_IF_FALSE     4 (to 210)
-                           202 POP_TOP
-               
-               252         204 POP_EXCEPT
-                           206 LOAD_CONST               0 (None)
-                           208 RETURN_VALUE
-               
-               251     >>  210 RERAISE                  0
-                       >>  212 COPY                     3
-                           214 POP_EXCEPT
-                           216 RERAISE                  1
-               
-               255     >>  218 LOAD_FAST                0 (self)
-                           220 LOAD_ATTR                0 (frame_radius)
-               
-               257         230 LOAD_FAST                0 (self)
-                           232 LOAD_ATTR                1 (frame_frame_back)
-               
-               258         242 LOAD_FAST                0 (self)
-                           244 LOAD_ATTR                2 (frame_border_width)
-               
-               260         254 LOAD_FAST                0 (self)
-                           256 LOAD_ATTR                3 (frame_border)
-               
-               261         266 LOAD_FAST                0 (self)
-                           268 LOAD_ATTR                4 (frame_back)
-               
-               254         278 LOAD_CONST               6 (('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back'))
-                           280 BUILD_CONST_KEY_MAP      5
-                           282 RETURN_VALUE
-               ExceptionTable:
-                 138 to 178 -> 184 [0]
-                 184 to 202 -> 212 [1] lasti
-                 210 to 210 -> 212 [1] lasti
-               consts
-                  None
-                  'frame_radius'
-                  'frame_frame_back'
-                  'frame_border_width'
-                  'frame_border'
-                  'frame_back'
-                  ('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back')
-               names      ('frame_radius', 'frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back', '_draw', 'AttributeError')
-               varnames   ('self', 'dict')
-               freevars   ()
-               cellvars   ()
-               filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
-               name       'palette'
-               firstlineno 240
-               lnotab
-                  0x020104011a021a011a011a011a0202013001120106ff08040c020c010c
-                  020c010cf9
-            (None,)
-         names      ('__name__', '__module__', '__qualname__', '__init__', '_draw', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__init__', '_draw', 'default_palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
          name       'AdwDrawBasicRoundFrame3'
-         firstlineno 183
-         lnotab 0x0c010a0706150603060c060d
+         firstlineno 160
+         lnotab 0x0c010a070615
       'AdwDrawBasicRoundFrame3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         265           0 RESUME                   0
+         193           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundFrame3')
                        8 STORE_NAME               2 (__qualname__)
          
-         266          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 266>)
+         194          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 194>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundFrame3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               266           0 RESUME                   0
+               194           0 RESUME                   0
                
-               267           2 LOAD_FAST                0 (self)
+               195           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 266
+               firstlineno 194
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
          name       'AdwDrawRoundFrame3'
-         firstlineno 265
+         firstlineno 193
          lnotab 0x0a01
       'AdwDrawRoundFrame3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         270           0 RESUME                   0
+         198           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkRoundFrame3')
                        8 STORE_NAME               2 (__qualname__)
          
-         271          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 271>)
+         199          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\frame.py", line 199>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkRoundFrame3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               271           0 RESUME                   0
+               199           0 RESUME                   0
                
-               272           2 LOAD_FAST                0 (self)
+               200           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 271
+               firstlineno 199
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
          name       'AdwDrawDarkRoundFrame3'
-         firstlineno 270
+         firstlineno 198
          lnotab 0x0a01
       'AdwDrawDarkRoundFrame3'
       '__main__'
       ('Tk',)
       'both'
       'yes'
       ('fill', 'expand')
@@ -2178,9 +1893,9 @@
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\canvas\\frame.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c041c4f1c051c051c4e1c051c051c521c051c050e010c
+      0x00ff02010c010c041c4c1c051c051c3a1c051c051c211c051c050e010c
       01140214012e022001320214012e022001320214012e02200132022cea
```

### Comparing `tkadw-0.1.5/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc` & `tkadw-0.2.0/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/canvas/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.2.0/tkadw/canvas/__pycache__/textbox.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x18619564 (Fri Jun 23 09:08:40 2023 UTC)
-files sz: 23435
+moddate:  0xf34e9664 (Sat Jun 24 02:03:31 2023 UTC)
+files sz: 21800
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -58,217 +58,217 @@
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               4 ('AdwDrawBasicText')
                 40 LOAD_NAME                4 (AdwDrawEngine)
                 42 PRECALL                  3
                 46 CALL                     3
                 56 STORE_NAME               5 (AdwDrawBasicText)
    
-   254          58 PUSH_NULL
+   255          58 PUSH_NULL
                 60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               5 (<code object AdwDrawText, file "D:\tkadw\tkadw\canvas\textbox.py", line 254>)
+                62 LOAD_CONST               5 (<code object AdwDrawText, file "D:\tkadw\tkadw\canvas\textbox.py", line 255>)
                 64 MAKE_FUNCTION            0
                 66 LOAD_CONST               6 ('AdwDrawText')
                 68 LOAD_NAME                5 (AdwDrawBasicText)
                 70 PRECALL                  3
                 74 CALL                     3
                 84 STORE_NAME               6 (AdwDrawText)
    
-   259          86 PUSH_NULL
+   260          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object AdwDrawDarkText, file "D:\tkadw\tkadw\canvas\textbox.py", line 259>)
+                90 LOAD_CONST               7 (<code object AdwDrawDarkText, file "D:\tkadw\tkadw\canvas\textbox.py", line 260>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('AdwDrawDarkText')
                 96 LOAD_NAME                5 (AdwDrawBasicText)
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME               7 (AdwDrawDarkText)
    
-   265         114 PUSH_NULL
+   266         114 PUSH_NULL
                116 LOAD_BUILD_CLASS
-               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundText, file "D:\tkadw\tkadw\canvas\textbox.py", line 265>)
+               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundText, file "D:\tkadw\tkadw\canvas\textbox.py", line 266>)
                120 MAKE_FUNCTION            0
                122 LOAD_CONST              10 ('AdwDrawBasicRoundText')
                124 LOAD_NAME                5 (AdwDrawBasicText)
                126 PRECALL                  3
                130 CALL                     3
                140 STORE_NAME               8 (AdwDrawBasicRoundText)
    
-   443         142 PUSH_NULL
+   415         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object AdwDrawRoundText, file "D:\tkadw\tkadw\canvas\textbox.py", line 443>)
+               146 LOAD_CONST              11 (<code object AdwDrawRoundText, file "D:\tkadw\tkadw\canvas\textbox.py", line 415>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('AdwDrawRoundText')
                152 LOAD_NAME                8 (AdwDrawBasicRoundText)
                154 PRECALL                  3
                158 CALL                     3
                168 STORE_NAME               9 (AdwDrawRoundText)
    
-   448         170 PUSH_NULL
+   420         170 PUSH_NULL
                172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkText, file "D:\tkadw\tkadw\canvas\textbox.py", line 448>)
+               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkText, file "D:\tkadw\tkadw\canvas\textbox.py", line 420>)
                176 MAKE_FUNCTION            0
                178 LOAD_CONST              14 ('AdwDrawRoundDarkText')
                180 LOAD_NAME                8 (AdwDrawBasicRoundText)
                182 PRECALL                  3
                186 CALL                     3
                196 STORE_NAME              10 (AdwDrawRoundDarkText)
    
-   453         198 PUSH_NULL
+   425         198 PUSH_NULL
                200 LOAD_BUILD_CLASS
-               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 453>)
+               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 425>)
                204 MAKE_FUNCTION            0
                206 LOAD_CONST              16 ('AdwDrawBasicRoundText3')
                208 LOAD_NAME                5 (AdwDrawBasicText)
                210 PRECALL                  3
                214 CALL                     3
                224 STORE_NAME              11 (AdwDrawBasicRoundText3)
    
-   637         226 PUSH_NULL
+   609         226 PUSH_NULL
                228 LOAD_BUILD_CLASS
-               230 LOAD_CONST              17 (<code object AdwDrawRoundText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 637>)
+               230 LOAD_CONST              17 (<code object AdwDrawRoundText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 609>)
                232 MAKE_FUNCTION            0
                234 LOAD_CONST              18 ('AdwDrawRoundText3')
                236 LOAD_NAME               11 (AdwDrawBasicRoundText3)
                238 PRECALL                  3
                242 CALL                     3
                252 STORE_NAME              12 (AdwDrawRoundText3)
    
-   642         254 PUSH_NULL
+   614         254 PUSH_NULL
                256 LOAD_BUILD_CLASS
-               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 642>)
+               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 614>)
                260 MAKE_FUNCTION            0
                262 LOAD_CONST              20 ('AdwDrawRoundDarkText3')
                264 LOAD_NAME               11 (AdwDrawBasicRoundText3)
                266 PRECALL                  3
                270 CALL                     3
                280 STORE_NAME              13 (AdwDrawRoundDarkText3)
    
-   647         282 LOAD_NAME               14 (__name__)
+   619         282 LOAD_NAME               14 (__name__)
                284 LOAD_CONST              21 ('__main__')
                286 COMPARE_OP               2 (==)
                292 POP_JUMP_FORWARD_IF_FALSE   242 (to 778)
    
-   648         294 LOAD_CONST               0 (0)
+   620         294 LOAD_CONST               0 (0)
                296 LOAD_CONST              22 (('Tk',))
                298 IMPORT_NAME             15 (tkinter)
                300 IMPORT_FROM             16 (Tk)
                302 STORE_NAME              16 (Tk)
                304 POP_TOP
    
-   650         306 PUSH_NULL
+   622         306 PUSH_NULL
                308 LOAD_NAME               16 (Tk)
                310 PRECALL                  0
                314 CALL                     0
                324 STORE_NAME              17 (root)
    
-   652         326 PUSH_NULL
+   624         326 PUSH_NULL
                328 LOAD_NAME                6 (AdwDrawText)
                330 PRECALL                  0
                334 CALL                     0
                344 STORE_NAME              18 (text1)
    
-   653         346 LOAD_NAME               18 (text1)
+   625         346 LOAD_NAME               18 (text1)
                348 LOAD_METHOD             19 (pack)
                370 LOAD_CONST              23 ('x')
                372 LOAD_CONST              24 (5)
                374 LOAD_CONST              24 (5)
                376 KW_NAMES                25
                378 PRECALL                  3
                382 CALL                     3
                392 POP_TOP
    
-   655         394 PUSH_NULL
+   627         394 PUSH_NULL
                396 LOAD_NAME                7 (AdwDrawDarkText)
                398 PRECALL                  0
                402 CALL                     0
                412 STORE_NAME              20 (text2)
    
-   656         414 LOAD_NAME               20 (text2)
+   628         414 LOAD_NAME               20 (text2)
                416 LOAD_METHOD             19 (pack)
                438 LOAD_CONST              23 ('x')
                440 LOAD_CONST              24 (5)
                442 LOAD_CONST              24 (5)
                444 KW_NAMES                25
                446 PRECALL                  3
                450 CALL                     3
                460 POP_TOP
    
-   658         462 PUSH_NULL
+   630         462 PUSH_NULL
                464 LOAD_NAME                9 (AdwDrawRoundText)
                466 PRECALL                  0
                470 CALL                     0
                480 STORE_NAME              21 (text3)
    
-   659         482 LOAD_NAME               21 (text3)
+   631         482 LOAD_NAME               21 (text3)
                484 LOAD_METHOD             19 (pack)
                506 LOAD_CONST              23 ('x')
                508 LOAD_CONST              24 (5)
                510 LOAD_CONST              24 (5)
                512 KW_NAMES                25
                514 PRECALL                  3
                518 CALL                     3
                528 POP_TOP
    
-   661         530 PUSH_NULL
+   633         530 PUSH_NULL
                532 LOAD_NAME               10 (AdwDrawRoundDarkText)
                534 PRECALL                  0
                538 CALL                     0
                548 STORE_NAME              22 (text4)
    
-   662         550 LOAD_NAME               22 (text4)
+   634         550 LOAD_NAME               22 (text4)
                552 LOAD_METHOD             19 (pack)
                574 LOAD_CONST              23 ('x')
                576 LOAD_CONST              24 (5)
                578 LOAD_CONST              24 (5)
                580 KW_NAMES                25
                582 PRECALL                  3
                586 CALL                     3
                596 POP_TOP
    
-   664         598 PUSH_NULL
+   636         598 PUSH_NULL
                600 LOAD_NAME               12 (AdwDrawRoundText3)
                602 PRECALL                  0
                606 CALL                     0
                616 STORE_NAME              23 (text5)
    
-   665         618 LOAD_NAME               23 (text5)
+   637         618 LOAD_NAME               23 (text5)
                620 LOAD_METHOD             19 (pack)
                642 LOAD_CONST              23 ('x')
                644 LOAD_CONST              24 (5)
                646 LOAD_CONST              24 (5)
                648 KW_NAMES                25
                650 PRECALL                  3
                654 CALL                     3
                664 POP_TOP
    
-   667         666 PUSH_NULL
+   639         666 PUSH_NULL
                668 LOAD_NAME               13 (AdwDrawRoundDarkText3)
                670 PRECALL                  0
                674 CALL                     0
                684 STORE_NAME              24 (text6)
    
-   668         686 LOAD_NAME               24 (text6)
+   640         686 LOAD_NAME               24 (text6)
                688 LOAD_METHOD             19 (pack)
                710 LOAD_CONST              23 ('x')
                712 LOAD_CONST              24 (5)
                714 LOAD_CONST              24 (5)
                716 KW_NAMES                25
                718 PRECALL                  3
                722 CALL                     3
                732 POP_TOP
    
-   670         734 LOAD_NAME               17 (root)
+   642         734 LOAD_NAME               17 (root)
                736 LOAD_METHOD             25 (mainloop)
                758 PRECALL                  0
                762 CALL                     0
                772 POP_TOP
                774 LOAD_CONST              26 (None)
                776 RETURN_VALUE
    
-   647     >>  778 LOAD_CONST              26 (None)
+   619     >>  778 LOAD_CONST              26 (None)
                780 RETURN_VALUE
    consts
       0
       ('Font', 'nametofont')
       ('AdwDrawEngine',)
       code
          argcount  : 0
@@ -398,20 +398,20 @@
                      176 MAKE_FUNCTION            0
                      178 STORE_NAME              26 (default_palette)
          
          169         180 LOAD_CONST              29 (<code object palette_light, file "D:\tkadw\tkadw\canvas\textbox.py", line 169>)
                      182 MAKE_FUNCTION            0
                      184 STORE_NAME              27 (palette_light)
          
-         191         186 LOAD_CONST              30 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 191>)
+         196         186 LOAD_CONST              30 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 196>)
                      188 MAKE_FUNCTION            0
                      190 STORE_NAME              28 (palette_dark)
          
-         213         192 LOAD_CONST              32 ((None,))
-                     194 LOAD_CONST              31 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 213>)
+         223         192 LOAD_CONST              32 ((None,))
+                     194 LOAD_CONST              31 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 223>)
                      196 MAKE_FUNCTION            1 (defaults)
                      198 STORE_NAME              29 (palette)
                      200 LOAD_CLOSURE             0 (__class__)
                      202 COPY                     1
                      204 STORE_NAME              30 (__classcell__)
                      206 RETURN_VALUE
          consts
@@ -2000,589 +2000,627 @@
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
                firstlineno 166
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 16
+               stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564066407640564086409640a640b640c640d9c0da60100
-                  00ab010000000000000000010064005300
+                  0264036404640564066404640764086409640a6406640b640c640d9c0664
+                  0e9c086901a6010000ab010000000000000000010064005300
                169           0 RESUME                   0
                
                170           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               172          26 LOAD_CONST               1 ((3, 4))
+               172          26 LOAD_CONST               1 ('text')
+               
+               173          28 LOAD_CONST               2 ((3, 4))
+               
+               175          30 LOAD_CONST               3 ('#fdfdfd')
                
-               174          28 LOAD_CONST               2 ('#f3f3f3')
+               176          32 LOAD_CONST               4 ('#eaeaea')
                
-               175          30 LOAD_CONST               3 (1)
+               177          34 LOAD_CONST               5 ('#5f5f5f')
                
-               176          32 LOAD_CONST               4 (0)
+               178          36 LOAD_CONST               6 (1)
                
-               178          34 LOAD_CONST               5 ('#eaeaea')
+               180          38 LOAD_CONST               4 ('#eaeaea')
                
-               179          36 LOAD_CONST               6 ('#fdfdfd')
+               181          40 LOAD_CONST               7 (0)
                
-               180          38 LOAD_CONST               7 ('#5f5f5f')
+               184          42 LOAD_CONST               8 ('#f9f9f9')
                
-               181          40 LOAD_CONST               5 ('#eaeaea')
+               185          44 LOAD_CONST               9 ('#e2e2e2')
                
-               183          42 LOAD_CONST               8 ('#e2e2e2')
+               186          46 LOAD_CONST              10 ('#1a1a1a')
                
-               184          44 LOAD_CONST               9 ('#f9f9f9')
+               187          48 LOAD_CONST               6 (1)
                
-               185          46 LOAD_CONST              10 ('#1a1a1a')
+               189          50 LOAD_CONST              11 ('#185fb4')
                
-               186          48 LOAD_CONST              11 ('#185fb4')
+               190          52 LOAD_CONST              12 (2)
                
-               187          50 LOAD_CONST              12 (2)
+               183          54 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                            56 BUILD_CONST_KEY_MAP      6
                
-               171          52 LOAD_CONST              13 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
-                            54 BUILD_CONST_KEY_MAP     13
+               172          58 LOAD_CONST              14 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                            60 BUILD_CONST_KEY_MAP      8
                
-               170          56 PRECALL                  1
-                            60 CALL                     1
-                            70 POP_TOP
-                            72 LOAD_CONST               0 (None)
-                            74 RETURN_VALUE
+               171          62 BUILD_MAP                1
+               
+               170          64 PRECALL                  1
+                            68 CALL                     1
+                            78 POP_TOP
+                            80 LOAD_CONST               0 (None)
+                            82 RETURN_VALUE
                consts
                   None
+                  'text'
                   (3, 4)
-                  '#f3f3f3'
-                  1
-                  0
-                  '#eaeaea'
                   '#fdfdfd'
+                  '#eaeaea'
                   '#5f5f5f'
-                  '#e2e2e2'
+                  1
+                  0
                   '#f9f9f9'
+                  '#e2e2e2'
                   '#1a1a1a'
                   '#185fb4'
                   2
-                  ('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
+                  ('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width')
+                  ('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_light'
                firstlineno 169
                lnotab
-                  0x0201180202020201020102020201020102010202020102010201020102
-                  f004ff
+                  0x0201180202010202020102010201020202010203020102010201020202
+                  0102f904f504ff02ff
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 16
+               stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  02640364046405640664076408640464096407640a640b640c9c0da60100
-                  00ab010000000000000000010064005300
-               191           0 RESUME                   0
+                  026403640464056406640764086409640464076406640a640b640c9c0664
+                  0d9c086901a6010000ab010000000000000000010064005300
+               196           0 RESUME                   0
                
-               192           2 LOAD_FAST                0 (self)
+               197           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               194          26 LOAD_CONST               1 ((3, 4))
+               199          26 LOAD_CONST               1 ('text')
+               
+               200          28 LOAD_CONST               2 ((3, 4))
+               
+               202          30 LOAD_CONST               3 ('#353535')
                
-               196          28 LOAD_CONST               2 ('#202020')
+               203          32 LOAD_CONST               4 ('#454545')
                
-               197          30 LOAD_CONST               3 (1)
+               204          34 LOAD_CONST               5 ('#cecece')
                
-               199          32 LOAD_CONST               4 ('#454545')
+               205          36 LOAD_CONST               6 (1)
                
-               200          34 LOAD_CONST               5 ('#353535')
+               207          38 LOAD_CONST               7 ('#ffffff')
                
-               201          36 LOAD_CONST               6 ('#cecece')
+               208          40 LOAD_CONST               8 (0)
                
-               202          38 LOAD_CONST               7 ('#ffffff')
+               211          42 LOAD_CONST               9 ('#2f2f2f')
                
-               203          40 LOAD_CONST               8 (0)
+               212          44 LOAD_CONST               4 ('#454545')
                
-               205          42 LOAD_CONST               4 ('#454545')
+               213          46 LOAD_CONST               7 ('#ffffff')
                
-               206          44 LOAD_CONST               9 ('#2f2f2f')
+               214          48 LOAD_CONST               6 (1)
                
-               207          46 LOAD_CONST               7 ('#ffffff')
+               216          50 LOAD_CONST              10 ('#4cc2ff')
                
-               208          48 LOAD_CONST              10 ('#4cc2ff')
+               217          52 LOAD_CONST              11 (2)
                
-               209          50 LOAD_CONST              11 (2)
+               210          54 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                            56 BUILD_CONST_KEY_MAP      6
                
-               193          52 LOAD_CONST              12 (('text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
-                            54 BUILD_CONST_KEY_MAP     13
+               199          58 LOAD_CONST              13 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                            60 BUILD_CONST_KEY_MAP      8
                
-               192          56 PRECALL                  1
-                            60 CALL                     1
-                            70 POP_TOP
-                            72 LOAD_CONST               0 (None)
-                            74 RETURN_VALUE
+               198          62 BUILD_MAP                1
+               
+               197          64 PRECALL                  1
+                            68 CALL                     1
+                            78 POP_TOP
+                            80 LOAD_CONST               0 (None)
+                            82 RETURN_VALUE
                consts
                   None
+                  'text'
                   (3, 4)
-                  '#202020'
-                  1
-                  '#454545'
                   '#353535'
+                  '#454545'
                   '#cecece'
+                  1
                   '#ffffff'
                   0
                   '#2f2f2f'
                   '#4cc2ff'
                   2
-                  ('text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
+                  ('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width')
+                  ('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 191
+               firstlineno 196
                lnotab
-                  0x0201180202020201020202010201020102010202020102010201020102
-                  f004ff
+                  0x0201180202010202020102010201020202010203020102010201020202
+                  0102f904f504ff02ff
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 11
+               stacksize : 4
                flags     : 3
                code
-                  0x97007c0181d27c016401190000000000000000007c005f000000000000
-                  0000007c016402190000000000000000007c005f0100000000000000007c
-                  016403190000000000000000007c005f0200000000000000007c01640419
-                  0000000000000000007c005f0300000000000000007c0164051900000000
-                  00000000007c005f0400000000000000007c016406190000000000000000
-                  007c005f0500000000000000007c016407190000000000000000007c005f
-                  0600000000000000007c016408190000000000000000007c005f07000000
-                  00000000007c016409190000000000000000007c005f0800000000000000
-                  007c01640a190000000000000000007c005f0900000000000000007c0164
-                  0b190000000000000000007c005f0a00000000000000007c01640c190000
-                  000000000000007c005f0b00000000000000007c01640d19000000000000
-                  0000007c005f0c000000000000000009007c00a00d000000000000000000
-                  00000000000000000000006400a6010000ab010000000000000000010064
-                  0053002300741c0000000000000000000024007204010059006400530077
-                  007803590077017c006a0000000000000000007c006a0100000000000000
-                  007c006a0200000000000000007c006a0700000000000000007c006a0300
-                  000000000000007c006a0400000000000000007c006a0500000000000000
-                  007c006a0800000000000000007c006a0900000000000000007c006a0a00
-                  00000000000000640e9c0a5300
-               213           0 RESUME                   0
-               
-               214           2 LOAD_FAST                1 (dict)
-                             4 POP_JUMP_FORWARD_IF_NONE   210 (to 426)
-               
-               215           6 LOAD_FAST                1 (dict)
-                             8 LOAD_CONST               1 ('text_padding')
-                            10 BINARY_SUBSCR
-                            20 LOAD_FAST                0 (self)
-                            22 STORE_ATTR               0 (text_padding)
-               
-               217          32 LOAD_FAST                1 (dict)
-                            34 LOAD_CONST               2 ('text_frame_back')
-                            36 BINARY_SUBSCR
-                            46 LOAD_FAST                0 (self)
-                            48 STORE_ATTR               1 (text_frame_back)
-               
-               218          58 LOAD_FAST                1 (dict)
-                            60 LOAD_CONST               3 ('text_border_width')
-                            62 BINARY_SUBSCR
-                            72 LOAD_FAST                0 (self)
-                            74 STORE_ATTR               2 (text_border_width)
-               
-               220          84 LOAD_FAST                1 (dict)
-                            86 LOAD_CONST               4 ('text_border')
-                            88 BINARY_SUBSCR
-                            98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               3 (text_border)
-               
-               221         110 LOAD_FAST                1 (dict)
-                           112 LOAD_CONST               5 ('text_back')
-                           114 BINARY_SUBSCR
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               4 (text_back)
-               
-               222         136 LOAD_FAST                1 (dict)
-                           138 LOAD_CONST               6 ('text_text_back')
-                           140 BINARY_SUBSCR
-                           150 LOAD_FAST                0 (self)
-                           152 STORE_ATTR               5 (text_text_back)
-               
-               223         162 LOAD_FAST                1 (dict)
-                           164 LOAD_CONST               7 ('text_bottom_line')
-                           166 BINARY_SUBSCR
-                           176 LOAD_FAST                0 (self)
-                           178 STORE_ATTR               6 (text_bottom_line)
-               
-               224         188 LOAD_FAST                1 (dict)
-                           190 LOAD_CONST               8 ('text_bottom_width')
-                           192 BINARY_SUBSCR
-                           202 LOAD_FAST                0 (self)
-                           204 STORE_ATTR               7 (text_bottom_width)
-               
-               226         214 LOAD_FAST                1 (dict)
-                           216 LOAD_CONST               9 ('text_focusin_border')
-                           218 BINARY_SUBSCR
-                           228 LOAD_FAST                0 (self)
-                           230 STORE_ATTR               8 (text_focusin_border)
-               
-               227         240 LOAD_FAST                1 (dict)
-                           242 LOAD_CONST              10 ('text_focusin_back')
-                           244 BINARY_SUBSCR
-                           254 LOAD_FAST                0 (self)
-                           256 STORE_ATTR               9 (text_focusin_back)
-               
-               228         266 LOAD_FAST                1 (dict)
-                           268 LOAD_CONST              11 ('text_focusin_text_back')
-                           270 BINARY_SUBSCR
-                           280 LOAD_FAST                0 (self)
-                           282 STORE_ATTR              10 (text_focusin_text_back)
-               
-               229         292 LOAD_FAST                1 (dict)
-                           294 LOAD_CONST              12 ('text_focusin_bottom_line')
-                           296 BINARY_SUBSCR
-                           306 LOAD_FAST                0 (self)
-                           308 STORE_ATTR              11 (text_focusin_bottom_line)
-               
-               230         318 LOAD_FAST                1 (dict)
-                           320 LOAD_CONST              13 ('text_focusin_bottom_width')
-                           322 BINARY_SUBSCR
-                           332 LOAD_FAST                0 (self)
-                           334 STORE_ATTR              12 (text_focusin_bottom_width)
-               
-               232         344 NOP
-               
-               233         346 LOAD_FAST                0 (self)
-                           348 LOAD_METHOD             13 (_draw)
-                           370 LOAD_CONST               0 (None)
-                           372 PRECALL                  1
-                           376 CALL                     1
-                           386 POP_TOP
-                           388 LOAD_CONST               0 (None)
-                           390 RETURN_VALUE
-                       >>  392 PUSH_EXC_INFO
-               
-               234         394 LOAD_GLOBAL             28 (AttributeError)
-                           406 CHECK_EXC_MATCH
-                           408 POP_JUMP_FORWARD_IF_FALSE     4 (to 418)
-                           410 POP_TOP
-               
-               235         412 POP_EXCEPT
-                           414 LOAD_CONST               0 (None)
-                           416 RETURN_VALUE
-               
-               234     >>  418 RERAISE                  0
-                       >>  420 COPY                     3
-                           422 POP_EXCEPT
-                           424 RERAISE                  1
-               
-               238     >>  426 LOAD_FAST                0 (self)
-                           428 LOAD_ATTR                0 (text_padding)
-               
-               240         438 LOAD_FAST                0 (self)
-                           440 LOAD_ATTR                1 (text_frame_back)
-               
-               241         450 LOAD_FAST                0 (self)
-                           452 LOAD_ATTR                2 (text_border_width)
-               
-               242         462 LOAD_FAST                0 (self)
-                           464 LOAD_ATTR                7 (text_bottom_width)
-               
-               244         474 LOAD_FAST                0 (self)
-                           476 LOAD_ATTR                3 (text_border)
-               
-               245         486 LOAD_FAST                0 (self)
-                           488 LOAD_ATTR                4 (text_back)
-               
-               246         498 LOAD_FAST                0 (self)
-                           500 LOAD_ATTR                5 (text_text_back)
-               
-               248         510 LOAD_FAST                0 (self)
-                           512 LOAD_ATTR                8 (text_focusin_border)
+                  0x97007c019001815a64017c017600900172257c01640119000000000000
+                  0000006402190000000000000000007c005f0000000000000000007c0164
+                  01190000000000000000006403190000000000000000007c005f01000000
+                  00000000007c016401190000000000000000006404190000000000000000
+                  007c005f0200000000000000007c01640119000000000000000000640519
+                  0000000000000000007c005f0300000000000000007c0164011900000000
+                  00000000006406190000000000000000007c005f0400000000000000007c
+                  016401190000000000000000006407190000000000000000007c005f0500
+                  000000000000007c01640119000000000000000000640819000000000000
+                  0000007c005f06000000000000000064097c016401190000000000000000
+                  00760072967c016401190000000000000000006409190000000000000000
+                  006403190000000000000000007c005f0700000000000000007c01640119
+                  000000000000000000640919000000000000000000640419000000000000
+                  0000007c005f0800000000000000007c0164011900000000000000000064
+                  09190000000000000000006405190000000000000000007c005f09000000
+                  00000000007c016401190000000000000000006409190000000000000000
+                  006406190000000000000000007c005f0a00000000000000007c01640119
+                  000000000000000000640919000000000000000000640719000000000000
+                  0000007c005f0b00000000000000007c0164011900000000000000000064
+                  09190000000000000000006408190000000000000000007c005f0c000000
+                  00000000007c017c005f0d000000000000000009007c00a00e0000000000
+                  0000000000000000000000000000006400a6010000ab0100000000000000
+                  000100640053002300741e00000000000000000000240072040100590064
+                  00530077007803590077017c006a0d00000000000000005300
+               223           0 RESUME                   0
+               
+               224           2 LOAD_FAST                1 (dict)
+                             4 EXTENDED_ARG             1
+                             6 POP_JUMP_FORWARD_IF_NONE   346 (to 700)
+               
+               225           8 LOAD_CONST               1 ('text')
+                            10 LOAD_FAST                1 (dict)
+                            12 CONTAINS_OP              0
+                            14 EXTENDED_ARG             1
+                            16 POP_JUMP_FORWARD_IF_FALSE   293 (to 604)
+               
+               226          18 LOAD_FAST                1 (dict)
+                            20 LOAD_CONST               1 ('text')
+                            22 BINARY_SUBSCR
+                            32 LOAD_CONST               2 ('padding')
+                            34 BINARY_SUBSCR
+                            44 LOAD_FAST                0 (self)
+                            46 STORE_ATTR               0 (text_padding)
                
-               249         522 LOAD_FAST                0 (self)
-                           524 LOAD_ATTR                9 (text_focusin_back)
+               228          56 LOAD_FAST                1 (dict)
+                            58 LOAD_CONST               1 ('text')
+                            60 BINARY_SUBSCR
+                            70 LOAD_CONST               3 ('back')
+                            72 BINARY_SUBSCR
+                            82 LOAD_FAST                0 (self)
+                            84 STORE_ATTR               1 (text_back)
+               
+               229          94 LOAD_FAST                1 (dict)
+                            96 LOAD_CONST               1 ('text')
+                            98 BINARY_SUBSCR
+                           108 LOAD_CONST               4 ('border')
+                           110 BINARY_SUBSCR
+                           120 LOAD_FAST                0 (self)
+                           122 STORE_ATTR               2 (text_border)
+               
+               230         132 LOAD_FAST                1 (dict)
+                           134 LOAD_CONST               1 ('text')
+                           136 BINARY_SUBSCR
+                           146 LOAD_CONST               5 ('text_back')
+                           148 BINARY_SUBSCR
+                           158 LOAD_FAST                0 (self)
+                           160 STORE_ATTR               3 (text_text_back)
+               
+               231         170 LOAD_FAST                1 (dict)
+                           172 LOAD_CONST               1 ('text')
+                           174 BINARY_SUBSCR
+                           184 LOAD_CONST               6 ('border_width')
+                           186 BINARY_SUBSCR
+                           196 LOAD_FAST                0 (self)
+                           198 STORE_ATTR               4 (text_border_width)
                
-               250         534 LOAD_FAST                0 (self)
-                           536 LOAD_ATTR               10 (text_focusin_text_back)
+               233         208 LOAD_FAST                1 (dict)
+                           210 LOAD_CONST               1 ('text')
+                           212 BINARY_SUBSCR
+                           222 LOAD_CONST               7 ('bottom_line')
+                           224 BINARY_SUBSCR
+                           234 LOAD_FAST                0 (self)
+                           236 STORE_ATTR               5 (text_bottom_line)
+               
+               234         246 LOAD_FAST                1 (dict)
+                           248 LOAD_CONST               1 ('text')
+                           250 BINARY_SUBSCR
+                           260 LOAD_CONST               8 ('bottom_width')
+                           262 BINARY_SUBSCR
+                           272 LOAD_FAST                0 (self)
+                           274 STORE_ATTR               6 (text_bottom_width)
+               
+               236         284 LOAD_CONST               9 ('focusin')
+                           286 LOAD_FAST                1 (dict)
+                           288 LOAD_CONST               1 ('text')
+                           290 BINARY_SUBSCR
+                           300 CONTAINS_OP              0
+                           302 POP_JUMP_FORWARD_IF_FALSE   150 (to 604)
+               
+               237         304 LOAD_FAST                1 (dict)
+                           306 LOAD_CONST               1 ('text')
+                           308 BINARY_SUBSCR
+                           318 LOAD_CONST               9 ('focusin')
+                           320 BINARY_SUBSCR
+                           330 LOAD_CONST               3 ('back')
+                           332 BINARY_SUBSCR
+                           342 LOAD_FAST                0 (self)
+                           344 STORE_ATTR               7 (text_focusin_back)
+               
+               238         354 LOAD_FAST                1 (dict)
+                           356 LOAD_CONST               1 ('text')
+                           358 BINARY_SUBSCR
+                           368 LOAD_CONST               9 ('focusin')
+                           370 BINARY_SUBSCR
+                           380 LOAD_CONST               4 ('border')
+                           382 BINARY_SUBSCR
+                           392 LOAD_FAST                0 (self)
+                           394 STORE_ATTR               8 (text_focusin_border)
+               
+               239         404 LOAD_FAST                1 (dict)
+                           406 LOAD_CONST               1 ('text')
+                           408 BINARY_SUBSCR
+                           418 LOAD_CONST               9 ('focusin')
+                           420 BINARY_SUBSCR
+                           430 LOAD_CONST               5 ('text_back')
+                           432 BINARY_SUBSCR
+                           442 LOAD_FAST                0 (self)
+                           444 STORE_ATTR               9 (text_focusin_text_back)
+               
+               240         454 LOAD_FAST                1 (dict)
+                           456 LOAD_CONST               1 ('text')
+                           458 BINARY_SUBSCR
+                           468 LOAD_CONST               9 ('focusin')
+                           470 BINARY_SUBSCR
+                           480 LOAD_CONST               6 ('border_width')
+                           482 BINARY_SUBSCR
+                           492 LOAD_FAST                0 (self)
+                           494 STORE_ATTR              10 (text_focusin_border_width)
                
-               237         546 LOAD_CONST              14 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back'))
-                           548 BUILD_CONST_KEY_MAP     10
-                           550 RETURN_VALUE
+               242         504 LOAD_FAST                1 (dict)
+                           506 LOAD_CONST               1 ('text')
+                           508 BINARY_SUBSCR
+                           518 LOAD_CONST               9 ('focusin')
+                           520 BINARY_SUBSCR
+                           530 LOAD_CONST               7 ('bottom_line')
+                           532 BINARY_SUBSCR
+                           542 LOAD_FAST                0 (self)
+                           544 STORE_ATTR              11 (text_focusin_bottom_line)
+               
+               243         554 LOAD_FAST                1 (dict)
+                           556 LOAD_CONST               1 ('text')
+                           558 BINARY_SUBSCR
+                           568 LOAD_CONST               9 ('focusin')
+                           570 BINARY_SUBSCR
+                           580 LOAD_CONST               8 ('bottom_width')
+                           582 BINARY_SUBSCR
+                           592 LOAD_FAST                0 (self)
+                           594 STORE_ATTR              12 (text_focusin_bottom_width)
+               
+               245     >>  604 LOAD_FAST                1 (dict)
+                           606 LOAD_FAST                0 (self)
+                           608 STORE_ATTR              13 (_palette)
+               
+               247         618 NOP
+               
+               248         620 LOAD_FAST                0 (self)
+                           622 LOAD_METHOD             14 (_draw)
+                           644 LOAD_CONST               0 (None)
+                           646 PRECALL                  1
+                           650 CALL                     1
+                           660 POP_TOP
+                           662 LOAD_CONST               0 (None)
+                           664 RETURN_VALUE
+                       >>  666 PUSH_EXC_INFO
+               
+               249         668 LOAD_GLOBAL             30 (AttributeError)
+                           680 CHECK_EXC_MATCH
+                           682 POP_JUMP_FORWARD_IF_FALSE     4 (to 692)
+                           684 POP_TOP
+               
+               250         686 POP_EXCEPT
+                           688 LOAD_CONST               0 (None)
+                           690 RETURN_VALUE
+               
+               249     >>  692 RERAISE                  0
+                       >>  694 COPY                     3
+                           696 POP_EXCEPT
+                           698 RERAISE                  1
+               
+               252     >>  700 LOAD_FAST                0 (self)
+                           702 LOAD_ATTR               13 (_palette)
+                           712 RETURN_VALUE
                ExceptionTable:
-                 346 to 386 -> 392 [0]
-                 392 to 410 -> 420 [1] lasti
-                 418 to 418 -> 420 [1] lasti
+                 620 to 660 -> 666 [0]
+                 666 to 684 -> 694 [1] lasti
+                 692 to 692 -> 694 [1] lasti
                consts
                   None
-                  'text_padding'
-                  'text_frame_back'
-                  'text_border_width'
-                  'text_border'
+                  'text'
+                  'padding'
+                  'back'
+                  'border'
                   'text_back'
-                  'text_text_back'
-                  'text_bottom_line'
-                  'text_bottom_width'
-                  'text_focusin_border'
-                  'text_focusin_back'
-                  'text_focusin_text_back'
-                  'text_focusin_bottom_line'
-                  'text_focusin_bottom_width'
-                  ('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back')
-               names      ('text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width', '_draw', 'AttributeError')
+                  'border_width'
+                  'bottom_line'
+                  'bottom_width'
+                  'focusin'
+               names      ('text_padding', 'text_back', 'text_border', 'text_text_back', 'text_border_width', 'text_bottom_line', 'text_bottom_width', 'text_focusin_back', 'text_focusin_border', 'text_focusin_text_back', 'text_focusin_border_width', 'text_focusin_bottom_line', 'text_focusin_bottom_width', '_palette', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette'
-               firstlineno 213
+               firstlineno 223
                lnotab
-                  0x020104011a021a011a021a011a011a011a011a021a011a011a011a011a
-                  0202013001120106ff08040c020c010c010c020c010c010c020c010c010c
-                  f3
+                  0x020106010a012602260126012601260226012602140132013201320132
+                  02320132020e0202013001120106ff0803
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', 'tbbox', 'compare', 'count', 'debug', 'tdelete', 'dump', 'get', 'tindex', 'tinsert', 'search', 'see', 'undo', 'redo', '_other', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawBasicText'
          firstlineno 6
          lnotab
             0x0c01122906030603060306030603060306030603060306030603060606
-            060604061c0809080908030803080b0e06060306160616
+            060604061c0809080908030803080b0e060603061b061b
       'AdwDrawBasicText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         254           0 RESUME                   0
+         255           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawText')
                        8 STORE_NAME               2 (__qualname__)
          
-         255          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 255>)
+         256          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 256>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               255           0 RESUME                   0
+               256           0 RESUME                   0
                
-               256           2 LOAD_FAST                0 (self)
+               257           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 255
+               firstlineno 256
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawText'
-         firstlineno 254
+         firstlineno 255
          lnotab 0x0a01
       'AdwDrawText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         259           0 RESUME                   0
+         260           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkText')
                        8 STORE_NAME               2 (__qualname__)
          
-         260          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 260>)
+         261          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 261>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               260           0 RESUME                   0
+               261           0 RESUME                   0
                
-               261           2 LOAD_FAST                0 (self)
+               262           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 260
+               firstlineno 261
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawDarkText'
-         firstlineno 259
+         firstlineno 260
          lnotab 0x0a01
       'AdwDrawDarkText'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 4
+         stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
-            126404650565067a0700006602640584055a07640684005a086412640784
-            015a096412640884015a0a6412640984015a0b6412640a84015a0c641264
-            0b84015a0d6412640c650e6602640d84055a0f640e84005a10640f84005a
-            11641084005a126412641184015a13880078015a145300
+            11640484015a05640584005a066411640684015a076411640784015a0864
+            11640884015a096411640984015a0a6411640a84015a0b6411640b650c66
+            02640c84055a0d640d84005a0e640e84005a0f640f84005a106411880066
+            01641084095a11880078015a125300
                        0 MAKE_CELL                0 (__class__)
          
-         265           2 RESUME                   0
+         266           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundText')
                       10 STORE_NAME               2 (__qualname__)
          
-         266          12 LOAD_CLOSURE             0 (__class__)
+         267          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\textbox.py", line 266>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\textbox.py", line 267>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         269          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\textbox.py", line 269>)
+         270          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\textbox.py", line 270>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         272          28 LOAD_CONST              18 ((None,))
-                      30 LOAD_CONST               4 ('radius')
-                      32 LOAD_NAME                5 (float)
-                      34 LOAD_NAME                6 (int)
-                      36 BINARY_OP                7 (|)
-                      40 BUILD_TUPLE              2
-                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\textbox.py", line 272>)
-                      44 MAKE_FUNCTION            5 (defaults, annotations)
-                      46 STORE_NAME               7 (border_radius)
+         273          28 LOAD_CONST              17 ((None,))
+                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\canvas\textbox.py", line 273>)
+                      32 MAKE_FUNCTION            1 (defaults)
+                      34 STORE_NAME               5 (border_radius)
          
-         278          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\textbox.py", line 278>)
-                      50 MAKE_FUNCTION            0
-                      52 STORE_NAME               8 (_draw)
+         279          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\canvas\textbox.py", line 279>)
+                      38 MAKE_FUNCTION            0
+                      40 STORE_NAME               6 (_draw)
          
-         308          54 LOAD_CONST              18 ((None,))
-                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\textbox.py", line 308>)
-                      58 MAKE_FUNCTION            1 (defaults)
-                      60 STORE_NAME               9 (_focus)
-         
-         317          62 LOAD_CONST              18 ((None,))
-                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\textbox.py", line 317>)
-                      66 MAKE_FUNCTION            1 (defaults)
-                      68 STORE_NAME              10 (_focusout)
-         
-         326          70 LOAD_CONST              18 ((None,))
-                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\textbox.py", line 326>)
-                      74 MAKE_FUNCTION            1 (defaults)
-                      76 STORE_NAME              11 (_click)
-         
-         329          78 LOAD_CONST              18 ((None,))
-                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\textbox.py", line 329>)
-                      82 MAKE_FUNCTION            1 (defaults)
-                      84 STORE_NAME              12 (_hover)
-         
-         332          86 LOAD_CONST              18 ((None,))
-                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\textbox.py", line 332>)
-                      90 MAKE_FUNCTION            1 (defaults)
-                      92 STORE_NAME              13 (_hover_release)
-         
-         343          94 LOAD_CONST              18 ((None,))
-                      96 LOAD_CONST              12 ('font')
-                      98 LOAD_NAME               14 (Font)
-                     100 BUILD_TUPLE              2
-                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\textbox.py", line 343>)
-                     104 MAKE_FUNCTION            5 (defaults, annotations)
-                     106 STORE_NAME              15 (font)
+         309          42 LOAD_CONST              17 ((None,))
+                      44 LOAD_CONST               6 (<code object _focus, file "D:\tkadw\tkadw\canvas\textbox.py", line 309>)
+                      46 MAKE_FUNCTION            1 (defaults)
+                      48 STORE_NAME               7 (_focus)
+         
+         318          50 LOAD_CONST              17 ((None,))
+                      52 LOAD_CONST               7 (<code object _focusout, file "D:\tkadw\tkadw\canvas\textbox.py", line 318>)
+                      54 MAKE_FUNCTION            1 (defaults)
+                      56 STORE_NAME               8 (_focusout)
+         
+         327          58 LOAD_CONST              17 ((None,))
+                      60 LOAD_CONST               8 (<code object _click, file "D:\tkadw\tkadw\canvas\textbox.py", line 327>)
+                      62 MAKE_FUNCTION            1 (defaults)
+                      64 STORE_NAME               9 (_click)
+         
+         330          66 LOAD_CONST              17 ((None,))
+                      68 LOAD_CONST               9 (<code object _hover, file "D:\tkadw\tkadw\canvas\textbox.py", line 330>)
+                      70 MAKE_FUNCTION            1 (defaults)
+                      72 STORE_NAME              10 (_hover)
+         
+         333          74 LOAD_CONST              17 ((None,))
+                      76 LOAD_CONST              10 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\textbox.py", line 333>)
+                      78 MAKE_FUNCTION            1 (defaults)
+                      80 STORE_NAME              11 (_hover_release)
+         
+         344          82 LOAD_CONST              17 ((None,))
+                      84 LOAD_CONST              11 ('font')
+                      86 LOAD_NAME               12 (Font)
+                      88 BUILD_TUPLE              2
+                      90 LOAD_CONST              12 (<code object font, file "D:\tkadw\tkadw\canvas\textbox.py", line 344>)
+                      92 MAKE_FUNCTION            5 (defaults, annotations)
+                      94 STORE_NAME              13 (font)
          
-         349         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 349>)
-                     110 MAKE_FUNCTION            0
-                     112 STORE_NAME              16 (default_palette)
+         350          96 LOAD_CONST              13 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 350>)
+                      98 MAKE_FUNCTION            0
+                     100 STORE_NAME              14 (default_palette)
          
-         352         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\textbox.py", line 352>)
-                     116 MAKE_FUNCTION            0
-                     118 STORE_NAME              17 (palette_light)
+         353         102 LOAD_CONST              14 (<code object palette_light, file "D:\tkadw\tkadw\canvas\textbox.py", line 353>)
+                     104 MAKE_FUNCTION            0
+                     106 STORE_NAME              15 (palette_light)
+         
+         381         108 LOAD_CONST              15 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 381>)
+                     110 MAKE_FUNCTION            0
+                     112 STORE_NAME              16 (palette_dark)
          
-         376         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 376>)
-                     122 MAKE_FUNCTION            0
-                     124 STORE_NAME              18 (palette_dark)
-         
-         400         126 LOAD_CONST              18 ((None,))
-                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 400>)
-                     130 MAKE_FUNCTION            1 (defaults)
-                     132 STORE_NAME              19 (palette)
-                     134 LOAD_CLOSURE             0 (__class__)
-                     136 COPY                     1
-                     138 STORE_NAME              20 (__classcell__)
-                     140 RETURN_VALUE
+         409         114 LOAD_CONST              17 ((None,))
+                     116 LOAD_CLOSURE             0 (__class__)
+                     118 BUILD_TUPLE              1
+                     120 LOAD_CONST              16 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 409>)
+                     122 MAKE_FUNCTION            9 (defaults, closure)
+                     124 STORE_NAME              17 (palette)
+                     126 LOAD_CLOSURE             0 (__class__)
+                     128 COPY                     1
+                     130 STORE_NAME              18 (__classcell__)
+                     132 RETURN_VALUE
          consts
             'AdwDrawBasicRoundText'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               266           2 RESUME                   0
+               267           2 RESUME                   0
                
-               267           4 PUSH_NULL
+               268           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -2595,29 +2633,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '__init__'
-               firstlineno 266
+               firstlineno 267
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               269           0 RESUME                   0
+               270           0 RESUME                   0
                
-               270           2 LOAD_FAST                0 (self)
+               271           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -2635,49 +2673,48 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_other'
-               firstlineno 269
+               firstlineno 270
                lnotab 0x0201
             None
-            'radius'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               272           0 RESUME                   0
+               273           0 RESUME                   0
                
-               273           2 LOAD_FAST                1 (radius)
+               274           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               274           6 LOAD_FAST                0 (self)
+               275           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               276     >>   20 LOAD_FAST                1 (radius)
+               277     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'border_radius'
-               firstlineno 272
+               firstlineno 273
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -2713,27 +2750,27 @@
                   000000000000000000000000007c006a100000000000000000a6010000ab
                   01000000000000000001007c00a011000000000000000000000000000000
                   00000000007c006a1000000000000000007c006a0c0000000000000000a6
                   020000ab02000000000000000001007c006a0b0000000000000000a01200
                   000000000000000000000000000000000000007c006a0700000000000000
                   007c006a1300000000000000007c006a130000000000000000ac0ba60300
                   00ab030000000000000000010064005300
-               278           0 RESUME                   0
+               279           0 RESUME                   0
                
-               279           2 LOAD_FAST                0 (self)
+               280           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               281          44 LOAD_FAST                0 (self)
+               282          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect2)
                
-               282          68 LOAD_CONST               2 (2)
+               283          68 LOAD_CONST               2 (2)
                             70 LOAD_CONST               2 (2)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
@@ -2742,159 +2779,159 @@
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                            160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (text_radius)
                
-               283         172 LOAD_FAST                0 (self)
+               284         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (text_border_width)
                
-               284         184 LOAD_FAST                0 (self)
+               285         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_text_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_text_back)
                
-               281         208 KW_NAMES                 4
+               282         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 LOAD_FAST                0 (self)
                            226 STORE_ATTR               8 (text_frame)
                
-               287         236 LOAD_FAST                0 (self)
+               288         236 LOAD_FAST                0 (self)
                            238 LOAD_METHOD              9 (create_window)
                
-               288         260 LOAD_FAST                0 (self)
+               289         260 LOAD_FAST                0 (self)
                            262 LOAD_METHOD              2 (winfo_width)
                            284 PRECALL                  0
                            288 CALL                     0
                            298 LOAD_CONST               2 (2)
                            300 BINARY_OP               11 (/)
                            304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              3 (winfo_height)
                            328 PRECALL                  0
                            332 CALL                     0
                            342 LOAD_CONST               2 (2)
                            344 BINARY_OP               11 (/)
                
-               289         348 LOAD_FAST                0 (self)
+               290         348 LOAD_FAST                0 (self)
                            350 LOAD_METHOD              2 (winfo_width)
                            372 PRECALL                  0
                            376 CALL                     0
                            386 LOAD_FAST                0 (self)
                            388 LOAD_ATTR                5 (text_border_width)
                            398 BINARY_OP               10 (-)
                            402 LOAD_CONST               5 (5)
                            404 BINARY_OP               10 (-)
                            408 LOAD_FAST                0 (self)
                            410 LOAD_ATTR               10 (text_padding)
                            420 LOAD_CONST               6 (0)
                            422 BINARY_SUBSCR
                            432 BINARY_OP               10 (-)
                
-               290         436 LOAD_FAST                0 (self)
+               291         436 LOAD_FAST                0 (self)
                            438 LOAD_METHOD              3 (winfo_height)
                            460 PRECALL                  0
                            464 CALL                     0
                            474 LOAD_FAST                0 (self)
                            476 LOAD_ATTR                5 (text_border_width)
                            486 BINARY_OP               10 (-)
                            490 LOAD_CONST               5 (5)
                            492 BINARY_OP               10 (-)
                            496 LOAD_FAST                0 (self)
                            498 LOAD_ATTR               10 (text_padding)
                            508 LOAD_CONST               7 (1)
                            510 BINARY_SUBSCR
                            520 BINARY_OP               10 (-)
                
-               291         524 LOAD_FAST                0 (self)
+               292         524 LOAD_FAST                0 (self)
                            526 LOAD_ATTR               11 (text)
                
-               287         536 KW_NAMES                 8
+               288         536 KW_NAMES                 8
                            538 PRECALL                  5
                            542 CALL                     5
                            552 LOAD_FAST                0 (self)
                            554 STORE_ATTR              12 (text_text)
                
-               294         564 LOAD_FAST                0 (self)
+               295         564 LOAD_FAST                0 (self)
                            566 LOAD_METHOD             13 (create_rectangle)
                            588 LOAD_CONST               3 (3)
                            590 LOAD_FAST                0 (self)
                            592 LOAD_ATTR                4 (text_radius)
                            602 LOAD_CONST               2 (2)
                            604 BINARY_OP               11 (/)
                            608 BINARY_OP                0 (+)
                
-               295         612 LOAD_FAST                0 (self)
+               296         612 LOAD_FAST                0 (self)
                            614 LOAD_METHOD              3 (winfo_height)
                            636 PRECALL                  0
                            640 CALL                     0
                            650 LOAD_FAST                0 (self)
                            652 LOAD_ATTR               14 (_text_bottom_width)
                            662 BINARY_OP               10 (-)
                            666 LOAD_CONST               3 (3)
                            668 BINARY_OP               10 (-)
                
-               296         672 LOAD_FAST                0 (self)
+               297         672 LOAD_FAST                0 (self)
                            674 LOAD_METHOD              2 (winfo_width)
                            696 PRECALL                  0
                            700 CALL                     0
                            710 LOAD_CONST               3 (3)
                            712 BINARY_OP               10 (-)
                            716 LOAD_FAST                0 (self)
                            718 LOAD_ATTR                4 (text_radius)
                            728 LOAD_CONST               2 (2)
                            730 BINARY_OP               11 (/)
                            734 BINARY_OP               10 (-)
                
-               297         738 LOAD_FAST                0 (self)
+               298         738 LOAD_FAST                0 (self)
                            740 LOAD_METHOD              3 (winfo_height)
                            762 PRECALL                  0
                            766 CALL                     0
                            776 LOAD_CONST               9 (3.5)
                            778 BINARY_OP               10 (-)
                
-               298         782 LOAD_FAST                0 (self)
+               299         782 LOAD_FAST                0 (self)
                            784 LOAD_ATTR               15 (_text_bottom_line)
                            794 LOAD_FAST                0 (self)
                            796 LOAD_ATTR               15 (_text_bottom_line)
                
-               299         806 LOAD_CONST               6 (0)
+               300         806 LOAD_CONST               6 (0)
                
-               294         808 KW_NAMES                10
+               295         808 KW_NAMES                10
                            810 PRECALL                  7
                            814 CALL                     7
                            824 LOAD_FAST                0 (self)
                            826 STORE_ATTR              16 (text_bottom)
                
-               301         836 LOAD_FAST                0 (self)
+               302         836 LOAD_FAST                0 (self)
                            838 LOAD_ATTR               14 (_text_bottom_width)
                            848 LOAD_CONST               6 (0)
                            850 COMPARE_OP               2 (==)
                            856 POP_JUMP_FORWARD_IF_FALSE    26 (to 910)
                
-               302         858 LOAD_FAST                0 (self)
+               303         858 LOAD_FAST                0 (self)
                            860 LOAD_METHOD              0 (delete)
                            882 LOAD_FAST                0 (self)
                            884 LOAD_ATTR               16 (text_bottom)
                            894 PRECALL                  1
                            898 CALL                     1
                            908 POP_TOP
                
-               304     >>  910 LOAD_FAST                0 (self)
+               305     >>  910 LOAD_FAST                0 (self)
                            912 LOAD_METHOD             17 (tag_raise)
                            934 LOAD_FAST                0 (self)
                            936 LOAD_ATTR               16 (text_bottom)
                            946 LOAD_FAST                0 (self)
                            948 LOAD_ATTR               12 (text_text)
                            958 PRECALL                  2
                            962 CALL                     2
                            972 POP_TOP
                
-               306         974 LOAD_FAST                0 (self)
+               307         974 LOAD_FAST                0 (self)
                            976 LOAD_ATTR               11 (text)
                            986 LOAD_METHOD             18 (configure)
                           1008 LOAD_FAST                0 (self)
                           1010 LOAD_ATTR                7 (_text_back)
                           1020 LOAD_FAST                0 (self)
                           1022 LOAD_ATTR               19 (_text_text_back)
                           1032 LOAD_FAST                0 (self)
@@ -2920,15 +2957,15 @@
                   ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_round_rect2', 'winfo_width', 'winfo_height', 'text_radius', 'text_border_width', '_text_border', '_text_back', 'text_frame', 'create_window', 'text_padding', 'text', 'text_text', 'create_rectangle', '_text_bottom_width', '_text_bottom_line', 'text_bottom', 'tag_raise', 'configure', '_text_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_draw'
-               firstlineno 278
+               firstlineno 279
                lnotab
                   0x02012a02180168010c0118fd1c0618015801580158010cfc1c0730013c
                   0142012c01180102fb1c07160134024002
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -2936,42 +2973,42 @@
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               308           0 RESUME                   0
+               309           0 RESUME                   0
                
-               309           2 LOAD_FAST                0 (self)
+               310           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_focusin_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-               310          26 LOAD_FAST                0 (self)
+               311          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_focusin_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-               311          50 LOAD_FAST                0 (self)
+               312          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_focusin_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-               312          74 LOAD_FAST                0 (self)
+               313          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_focusin_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-               313          98 LOAD_FAST                0 (self)
+               314          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_focusin_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-               315         122 LOAD_FAST                0 (self)
+               316         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -2979,56 +3016,56 @@
                   None
                names      ('text_focusin_back', '_text_back', 'text_focusin_border', '_text_border', 'text_focusin_text_back', '_text_text_back', 'text_focusin_bottom_line', '_text_bottom_line', 'text_focusin_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_focus'
-               firstlineno 308
+               firstlineno 309
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               317           0 RESUME                   0
+               318           0 RESUME                   0
                
-               318           2 LOAD_FAST                0 (self)
+               319           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-               319          26 LOAD_FAST                0 (self)
+               320          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-               320          50 LOAD_FAST                0 (self)
+               321          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-               321          74 LOAD_FAST                0 (self)
+               322          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-               322          98 LOAD_FAST                0 (self)
+               323          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-               324         122 LOAD_FAST                0 (self)
+               325         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -3036,66 +3073,66 @@
                   None
                names      ('text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_focusout'
-               firstlineno 317
+               firstlineno 318
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               326           0 RESUME                   0
+               327           0 RESUME                   0
                
-               327           2 LOAD_FAST                0 (self)
+               328           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_set)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('focus_set',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_click'
-               firstlineno 326
+               firstlineno 327
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064005300
-               329           0 RESUME                   0
+               330           0 RESUME                   0
                
-               330           2 LOAD_CONST               1 (True)
+               331           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                   True
                names      ('hover',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_hover'
-               firstlineno 329
+               firstlineno 330
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -3103,723 +3140,581 @@
                   00ab000000000000000000735a64017c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c006a0a00000000000000007c005f0b00000000000000007c00a0
                   0c00000000000000000000000000000000000000006400a6010000ab0100
                   0000000000000001006400530064005300
-               332           0 RESUME                   0
+               333           0 RESUME                   0
                
-               333           2 LOAD_FAST                0 (self)
+               334           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_get)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_JUMP_FORWARD_IF_TRUE    90 (to 222)
                
-               334          42 LOAD_CONST               1 (False)
+               335          42 LOAD_CONST               1 (False)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (hover)
                
-               335          56 LOAD_FAST                0 (self)
+               336          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (text_back)
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_text_back)
                
-               336          80 LOAD_FAST                0 (self)
+               337          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (text_border)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               5 (_text_border)
                
-               337         104 LOAD_FAST                0 (self)
+               338         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (text_text_back)
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               7 (_text_text_back)
                
-               338         128 LOAD_FAST                0 (self)
+               339         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                8 (text_bottom_line)
                            140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               9 (_text_bottom_line)
                
-               339         152 LOAD_FAST                0 (self)
+               340         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR               10 (text_bottom_width)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR              11 (_text_bottom_width)
                
-               341         176 LOAD_FAST                0 (self)
+               342         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD             12 (_draw)
                            200 LOAD_CONST               0 (None)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                
-               333     >>  222 LOAD_CONST               0 (None)
+               334     >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   False
                names      ('focus_get', 'hover', 'text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_hover_release'
-               firstlineno 332
+               firstlineno 333
                lnotab 0x020128010e01180118011801180118022ef8
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               343           0 RESUME                   0
+               344           0 RESUME                   0
                
-               344           2 LOAD_FAST                1 (font)
+               345           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               345           6 LOAD_FAST                0 (self)
+               346           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (text_text_font)
                             18 RETURN_VALUE
                
-               347     >>   20 LOAD_FAST                1 (font)
+               348     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (text_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('text_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'font'
-               firstlineno 343
+               firstlineno 344
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               349           0 RESUME                   0
+               350           0 RESUME                   0
                
-               350           2 LOAD_FAST                0 (self)
+               351           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 349
+               firstlineno 350
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 17
+               stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564066407640864066409640a640b640c640d640e9c0ea6
-                  010000ab010000000000000000010064005300
-               352           0 RESUME                   0
+                  0264036404640564066407640564086409640a640b6407640c640d640e9c
+                  06640f9c096901a6010000ab010000000000000000010064005300
+               353           0 RESUME                   0
                
-               353           2 LOAD_FAST                0 (self)
+               354           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               355          26 LOAD_CONST               1 (6)
+               356          26 LOAD_CONST               1 ('text')
                
-               357          28 LOAD_CONST               2 ((3, 4))
+               357          28 LOAD_CONST               2 (6)
                
-               359          30 LOAD_CONST               3 ('#f3f3f3')
+               358          30 LOAD_CONST               3 ((3, 4))
                
-               360          32 LOAD_CONST               4 (1)
+               360          32 LOAD_CONST               4 ('#fdfdfd')
                
-               361          34 LOAD_CONST               5 (0)
+               361          34 LOAD_CONST               5 ('#eaeaea')
                
-               363          36 LOAD_CONST               6 ('#eaeaea')
+               362          36 LOAD_CONST               6 ('#5f5f5f')
                
-               364          38 LOAD_CONST               7 ('#fdfdfd')
+               363          38 LOAD_CONST               7 (1)
                
-               365          40 LOAD_CONST               8 ('#5f5f5f')
+               365          40 LOAD_CONST               5 ('#eaeaea')
                
-               366          42 LOAD_CONST               6 ('#eaeaea')
+               366          42 LOAD_CONST               8 (0)
                
-               368          44 LOAD_CONST               9 ('#e2e2e2')
+               369          44 LOAD_CONST               9 ('#f9f9f9')
                
-               369          46 LOAD_CONST              10 ('#f9f9f9')
+               370          46 LOAD_CONST              10 ('#e2e2e2')
                
-               370          48 LOAD_CONST              11 ('#1a1a1a')
+               371          48 LOAD_CONST              11 ('#1a1a1a')
                
-               371          50 LOAD_CONST              12 ('#185fb4')
+               372          50 LOAD_CONST               7 (1)
                
-               372          52 LOAD_CONST              13 (2)
+               374          52 LOAD_CONST              12 ('#185fb4')
                
-               354          54 LOAD_CONST              14 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
-                            56 BUILD_CONST_KEY_MAP     14
+               375          54 LOAD_CONST              13 (2)
                
-               353          58 PRECALL                  1
-                            62 CALL                     1
-                            72 POP_TOP
-                            74 LOAD_CONST               0 (None)
-                            76 RETURN_VALUE
+               368          56 LOAD_CONST              14 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                            58 BUILD_CONST_KEY_MAP      6
+               
+               356          60 LOAD_CONST              15 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                            62 BUILD_CONST_KEY_MAP      9
+               
+               355          64 BUILD_MAP                1
+               
+               354          66 PRECALL                  1
+                            70 CALL                     1
+                            80 POP_TOP
+                            82 LOAD_CONST               0 (None)
+                            84 RETURN_VALUE
                consts
                   None
+                  'text'
                   6
                   (3, 4)
-                  '#f3f3f3'
-                  1
-                  0
-                  '#eaeaea'
                   '#fdfdfd'
+                  '#eaeaea'
                   '#5f5f5f'
-                  '#e2e2e2'
+                  1
+                  0
                   '#f9f9f9'
+                  '#e2e2e2'
                   '#1a1a1a'
                   '#185fb4'
                   2
-                  ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
+                  ('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width')
+                  ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_light'
-               firstlineno 352
+               firstlineno 353
                lnotab
-                  0x0201180202020202020102010202020102010201020202010201020102
-                  0102ee04ff
+                  0x0201180202010201020202010201020102020201020302010201020102
+                  02020102f904f404ff02ff
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 17
+               stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564066407640864096405640a6408640b640c640d9c0ea6
-                  010000ab010000000000000000010064005300
-               376           0 RESUME                   0
+                  026403640464056406640764086409640a640564086407640b640c640d9c
+                  06640e9c096901a6010000ab010000000000000000010064005300
+               381           0 RESUME                   0
                
-               377           2 LOAD_FAST                0 (self)
+               382           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               379          26 LOAD_CONST               1 (6)
+               384          26 LOAD_CONST               1 ('text')
                
-               381          28 LOAD_CONST               2 ((3, 4))
+               385          28 LOAD_CONST               2 (6)
                
-               383          30 LOAD_CONST               3 ('#202020')
+               386          30 LOAD_CONST               3 ((3, 4))
                
-               384          32 LOAD_CONST               4 (1)
+               388          32 LOAD_CONST               4 ('#353535')
                
-               386          34 LOAD_CONST               5 ('#454545')
+               389          34 LOAD_CONST               5 ('#454545')
                
-               387          36 LOAD_CONST               6 ('#353535')
+               390          36 LOAD_CONST               6 ('#cecece')
                
-               388          38 LOAD_CONST               7 ('#cecece')
+               391          38 LOAD_CONST               7 (1)
                
-               389          40 LOAD_CONST               8 ('#ffffff')
+               393          40 LOAD_CONST               8 ('#ffffff')
                
-               390          42 LOAD_CONST               9 (0)
+               394          42 LOAD_CONST               9 (0)
                
-               392          44 LOAD_CONST               5 ('#454545')
+               397          44 LOAD_CONST              10 ('#2f2f2f')
                
-               393          46 LOAD_CONST              10 ('#2f2f2f')
+               398          46 LOAD_CONST               5 ('#454545')
                
-               394          48 LOAD_CONST               8 ('#ffffff')
+               399          48 LOAD_CONST               8 ('#ffffff')
                
-               395          50 LOAD_CONST              11 ('#4cc2ff')
+               400          50 LOAD_CONST               7 (1)
                
-               396          52 LOAD_CONST              12 (2)
+               402          52 LOAD_CONST              11 ('#4cc2ff')
                
-               378          54 LOAD_CONST              13 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
-                            56 BUILD_CONST_KEY_MAP     14
+               403          54 LOAD_CONST              12 (2)
                
-               377          58 PRECALL                  1
-                            62 CALL                     1
-                            72 POP_TOP
-                            74 LOAD_CONST               0 (None)
-                            76 RETURN_VALUE
+               396          56 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                            58 BUILD_CONST_KEY_MAP      6
+               
+               384          60 LOAD_CONST              14 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                            62 BUILD_CONST_KEY_MAP      9
+               
+               383          64 BUILD_MAP                1
+               
+               382          66 PRECALL                  1
+                            70 CALL                     1
+                            80 POP_TOP
+                            82 LOAD_CONST               0 (None)
+                            84 RETURN_VALUE
                consts
                   None
+                  'text'
                   6
                   (3, 4)
-                  '#202020'
-                  1
-                  '#454545'
                   '#353535'
+                  '#454545'
                   '#cecece'
+                  1
                   '#ffffff'
                   0
                   '#2f2f2f'
                   '#4cc2ff'
                   2
-                  ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
+                  ('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width')
+                  ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 376
+               firstlineno 381
                lnotab
-                  0x0201180202020202020102020201020102010201020202010201020102
-                  0102ee04ff
+                  0x0201180202010201020202010201020102020201020302010201020102
+                  02020102f904f404ff02ff
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 11
+               stacksize : 3
                flags     : 3
                code
-                  0x97007c0181df7c016401190000000000000000007c005f000000000000
-                  0000007c016402190000000000000000007c005f0100000000000000007c
-                  016403190000000000000000007c005f0200000000000000007c01640419
-                  0000000000000000007c005f0300000000000000007c0164051900000000
-                  00000000007c005f0400000000000000007c016406190000000000000000
-                  007c005f0500000000000000007c016407190000000000000000007c005f
-                  0600000000000000007c016408190000000000000000007c005f07000000
-                  00000000007c016409190000000000000000007c005f0800000000000000
-                  007c01640a190000000000000000007c005f0900000000000000007c0164
-                  0b190000000000000000007c005f0a00000000000000007c01640c190000
-                  000000000000007c005f0b00000000000000007c01640d19000000000000
-                  0000007c005f0c00000000000000007c01640e190000000000000000007c
-                  005f0d000000000000000009007c00a00e00000000000000000000000000
-                  000000000000006400a6010000ab01000000000000000001006400530023
-                  00741e000000000000000000002400720401005900640053007700780359
-                  0077017c006a0100000000000000007c006a0200000000000000007c006a
-                  0300000000000000007c006a0800000000000000007c006a040000000000
-                  0000007c006a0500000000000000007c006a0600000000000000007c006a
-                  0900000000000000007c006a0a00000000000000007c006a0b0000000000
-                  000000640f9c0a5300
-               400           0 RESUME                   0
-               
-               401           2 LOAD_FAST                1 (dict)
-                             4 POP_JUMP_FORWARD_IF_NONE   223 (to 452)
-               
-               402           6 LOAD_FAST                1 (dict)
-                             8 LOAD_CONST               1 ('text_radius')
-                            10 BINARY_SUBSCR
-                            20 LOAD_FAST                0 (self)
-                            22 STORE_ATTR               0 (text_radius)
-               
-               404          32 LOAD_FAST                1 (dict)
-                            34 LOAD_CONST               2 ('text_padding')
-                            36 BINARY_SUBSCR
-                            46 LOAD_FAST                0 (self)
-                            48 STORE_ATTR               1 (text_padding)
-               
-               406          58 LOAD_FAST                1 (dict)
-                            60 LOAD_CONST               3 ('text_frame_back')
-                            62 BINARY_SUBSCR
-                            72 LOAD_FAST                0 (self)
-                            74 STORE_ATTR               2 (text_frame_back)
-               
-               407          84 LOAD_FAST                1 (dict)
-                            86 LOAD_CONST               4 ('text_border_width')
-                            88 BINARY_SUBSCR
-                            98 LOAD_FAST                0 (self)
-                           100 STORE_ATTR               3 (text_border_width)
-               
-               409         110 LOAD_FAST                1 (dict)
-                           112 LOAD_CONST               5 ('text_border')
-                           114 BINARY_SUBSCR
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               4 (text_border)
-               
-               410         136 LOAD_FAST                1 (dict)
-                           138 LOAD_CONST               6 ('text_back')
-                           140 BINARY_SUBSCR
-                           150 LOAD_FAST                0 (self)
-                           152 STORE_ATTR               5 (text_back)
-               
-               411         162 LOAD_FAST                1 (dict)
-                           164 LOAD_CONST               7 ('text_text_back')
-                           166 BINARY_SUBSCR
-                           176 LOAD_FAST                0 (self)
-                           178 STORE_ATTR               6 (text_text_back)
-               
-               412         188 LOAD_FAST                1 (dict)
-                           190 LOAD_CONST               8 ('text_bottom_line')
-                           192 BINARY_SUBSCR
-                           202 LOAD_FAST                0 (self)
-                           204 STORE_ATTR               7 (text_bottom_line)
-               
-               413         214 LOAD_FAST                1 (dict)
-                           216 LOAD_CONST               9 ('text_bottom_width')
-                           218 BINARY_SUBSCR
-                           228 LOAD_FAST                0 (self)
-                           230 STORE_ATTR               8 (text_bottom_width)
-               
-               415         240 LOAD_FAST                1 (dict)
-                           242 LOAD_CONST              10 ('text_focusin_border')
-                           244 BINARY_SUBSCR
-                           254 LOAD_FAST                0 (self)
-                           256 STORE_ATTR               9 (text_focusin_border)
-               
-               416         266 LOAD_FAST                1 (dict)
-                           268 LOAD_CONST              11 ('text_focusin_back')
-                           270 BINARY_SUBSCR
-                           280 LOAD_FAST                0 (self)
-                           282 STORE_ATTR              10 (text_focusin_back)
-               
-               417         292 LOAD_FAST                1 (dict)
-                           294 LOAD_CONST              12 ('text_focusin_text_back')
-                           296 BINARY_SUBSCR
-                           306 LOAD_FAST                0 (self)
-                           308 STORE_ATTR              11 (text_focusin_text_back)
-               
-               418         318 LOAD_FAST                1 (dict)
-                           320 LOAD_CONST              13 ('text_focusin_bottom_line')
-                           322 BINARY_SUBSCR
-                           332 LOAD_FAST                0 (self)
-                           334 STORE_ATTR              12 (text_focusin_bottom_line)
-               
-               419         344 LOAD_FAST                1 (dict)
-                           346 LOAD_CONST              14 ('text_focusin_bottom_width')
-                           348 BINARY_SUBSCR
-                           358 LOAD_FAST                0 (self)
-                           360 STORE_ATTR              13 (text_focusin_bottom_width)
-               
-               421         370 NOP
-               
-               422         372 LOAD_FAST                0 (self)
-                           374 LOAD_METHOD             14 (_draw)
-                           396 LOAD_CONST               0 (None)
-                           398 PRECALL                  1
-                           402 CALL                     1
-                           412 POP_TOP
-                           414 LOAD_CONST               0 (None)
-                           416 RETURN_VALUE
-                       >>  418 PUSH_EXC_INFO
-               
-               423         420 LOAD_GLOBAL             30 (AttributeError)
-                           432 CHECK_EXC_MATCH
-                           434 POP_JUMP_FORWARD_IF_FALSE     4 (to 444)
-                           436 POP_TOP
-               
-               424         438 POP_EXCEPT
-                           440 LOAD_CONST               0 (None)
-                           442 RETURN_VALUE
-               
-               423     >>  444 RERAISE                  0
-                       >>  446 COPY                     3
-                           448 POP_EXCEPT
-                           450 RERAISE                  1
-               
-               427     >>  452 LOAD_FAST                0 (self)
-                           454 LOAD_ATTR                1 (text_padding)
-               
-               429         464 LOAD_FAST                0 (self)
-                           466 LOAD_ATTR                2 (text_frame_back)
-               
-               430         476 LOAD_FAST                0 (self)
-                           478 LOAD_ATTR                3 (text_border_width)
-               
-               431         488 LOAD_FAST                0 (self)
-                           490 LOAD_ATTR                8 (text_bottom_width)
-               
-               433         500 LOAD_FAST                0 (self)
-                           502 LOAD_ATTR                4 (text_border)
-               
-               434         512 LOAD_FAST                0 (self)
-                           514 LOAD_ATTR                5 (text_back)
-               
-               435         524 LOAD_FAST                0 (self)
-                           526 LOAD_ATTR                6 (text_text_back)
-               
-               437         536 LOAD_FAST                0 (self)
-                           538 LOAD_ATTR                9 (text_focusin_border)
-               
-               438         548 LOAD_FAST                0 (self)
-                           550 LOAD_ATTR               10 (text_focusin_back)
+                  0x95019700740100000000000000000000a6000000ab0000000000000000
+                  00a00100000000000000000000000000000000000000007c01a6010000ab
+                  010000000000000000010064017c01760072157c01640119000000000000
+                  0000006402190000000000000000007c005f020000000000000000640053
+                  0064005300
+                             0 COPY_FREE_VARS           1
                
-               439         560 LOAD_FAST                0 (self)
-                           562 LOAD_ATTR               11 (text_focusin_text_back)
+               409           2 RESUME                   0
                
-               426         572 LOAD_CONST              15 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back'))
-                           574 BUILD_CONST_KEY_MAP     10
-                           576 RETURN_VALUE
-               ExceptionTable:
-                 372 to 412 -> 418 [0]
-                 418 to 436 -> 446 [1] lasti
-                 444 to 444 -> 446 [1] lasti
-               consts
-                  None
-                  'text_radius'
-                  'text_padding'
-                  'text_frame_back'
-                  'text_border_width'
-                  'text_border'
-                  'text_back'
-                  'text_text_back'
-                  'text_bottom_line'
-                  'text_bottom_width'
-                  'text_focusin_border'
-                  'text_focusin_back'
-                  'text_focusin_text_back'
-                  'text_focusin_bottom_line'
-                  'text_focusin_bottom_width'
-                  ('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back')
-               names      ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width', '_draw', 'AttributeError')
+               410           4 LOAD_GLOBAL              1 (NULL + super)
+                            16 PRECALL                  0
+                            20 CALL                     0
+                            30 LOAD_METHOD              1 (palette)
+                            52 LOAD_FAST                1 (dict)
+                            54 PRECALL                  1
+                            58 CALL                     1
+                            68 POP_TOP
+               
+               411          70 LOAD_CONST               1 ('text')
+                            72 LOAD_FAST                1 (dict)
+                            74 CONTAINS_OP              0
+                            76 POP_JUMP_FORWARD_IF_FALSE    21 (to 120)
+               
+               412          78 LOAD_FAST                1 (dict)
+                            80 LOAD_CONST               1 ('text')
+                            82 BINARY_SUBSCR
+                            92 LOAD_CONST               2 ('radius')
+                            94 BINARY_SUBSCR
+                           104 LOAD_FAST                0 (self)
+                           106 STORE_ATTR               2 (text_radius)
+                           116 LOAD_CONST               0 (None)
+                           118 RETURN_VALUE
+               
+               411     >>  120 LOAD_CONST               0 (None)
+                           122 RETURN_VALUE
+               consts
+                  None
+                  'text'
+                  'radius'
+               names      ('super', 'palette', 'text_radius')
                varnames   ('self', 'dict')
-               freevars   ()
+               freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette'
-               firstlineno 400
-               lnotab
-                  0x020104011a021a021a011a021a011a011a011a011a021a011a011a011a
-                  011a0202013001120106ff08040c020c010c010c020c010c010c020c010c
-                  010cf3
+               firstlineno 409
+               lnotab 0x0401420108012aff
             (None,)
-         names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'float', 'int', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawBasicRoundText'
-         firstlineno 265
-         lnotab 0x0c010a0306031406061e0809080908030803080b0e06060306180618
+         firstlineno 266
+         lnotab 0x0c010a0306030806061e0809080908030803080b0e060603061c061c
       'AdwDrawBasicRoundText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         443           0 RESUME                   0
+         415           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundText')
                        8 STORE_NAME               2 (__qualname__)
          
-         444          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 444>)
+         416          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 416>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               444           0 RESUME                   0
+               416           0 RESUME                   0
                
-               445           2 LOAD_FAST                0 (self)
+               417           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 444
+               firstlineno 416
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawRoundText'
-         firstlineno 443
+         firstlineno 415
          lnotab 0x0a01
       'AdwDrawRoundText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         448           0 RESUME                   0
+         420           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkText')
                        8 STORE_NAME               2 (__qualname__)
          
-         449          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 449>)
+         421          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 421>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               449           0 RESUME                   0
+               421           0 RESUME                   0
                
-               450           2 LOAD_FAST                0 (self)
+               422           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 449
+               firstlineno 421
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawRoundDarkText'
-         firstlineno 448
+         firstlineno 420
          lnotab 0x0a01
       'AdwDrawRoundDarkText'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 4
+         stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
-            126404650565067a0700006602640584055a07640684005a086412640784
-            015a096412640884015a0a6412640984015a0b6412640a84015a0c641264
-            0b84015a0d6412640c650e6602640d84055a0f640e84005a10640f84005a
-            11641084005a126412641184015a13880078015a145300
+            11640484015a05640584005a066411640684015a076411640784015a0864
+            11640884015a096411640984015a0a6411640a84015a0b6411640b650c66
+            02640c84055a0d640d84005a0e640e84005a0f640f84005a106411641084
+            015a11880078015a125300
                        0 MAKE_CELL                0 (__class__)
          
-         453           2 RESUME                   0
+         425           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundText3')
                       10 STORE_NAME               2 (__qualname__)
          
-         454          12 LOAD_CLOSURE             0 (__class__)
+         426          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\textbox.py", line 454>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\textbox.py", line 426>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         457          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\textbox.py", line 457>)
+         429          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\textbox.py", line 429>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         460          28 LOAD_CONST              18 ((None,))
-                      30 LOAD_CONST               4 ('radius')
-                      32 LOAD_NAME                5 (float)
-                      34 LOAD_NAME                6 (int)
-                      36 BINARY_OP                7 (|)
-                      40 BUILD_TUPLE              2
-                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\textbox.py", line 460>)
-                      44 MAKE_FUNCTION            5 (defaults, annotations)
-                      46 STORE_NAME               7 (border_radius)
+         432          28 LOAD_CONST              17 ((None,))
+                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\canvas\textbox.py", line 432>)
+                      32 MAKE_FUNCTION            1 (defaults)
+                      34 STORE_NAME               5 (border_radius)
          
-         466          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\textbox.py", line 466>)
-                      50 MAKE_FUNCTION            0
-                      52 STORE_NAME               8 (_draw)
+         438          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\canvas\textbox.py", line 438>)
+                      38 MAKE_FUNCTION            0
+                      40 STORE_NAME               6 (_draw)
          
-         502          54 LOAD_CONST              18 ((None,))
-                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\textbox.py", line 502>)
-                      58 MAKE_FUNCTION            1 (defaults)
-                      60 STORE_NAME               9 (_focus)
-         
-         511          62 LOAD_CONST              18 ((None,))
-                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\textbox.py", line 511>)
-                      66 MAKE_FUNCTION            1 (defaults)
-                      68 STORE_NAME              10 (_focusout)
-         
-         520          70 LOAD_CONST              18 ((None,))
-                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\textbox.py", line 520>)
-                      74 MAKE_FUNCTION            1 (defaults)
-                      76 STORE_NAME              11 (_click)
-         
-         523          78 LOAD_CONST              18 ((None,))
-                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\textbox.py", line 523>)
-                      82 MAKE_FUNCTION            1 (defaults)
-                      84 STORE_NAME              12 (_hover)
-         
-         526          86 LOAD_CONST              18 ((None,))
-                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\textbox.py", line 526>)
-                      90 MAKE_FUNCTION            1 (defaults)
-                      92 STORE_NAME              13 (_hover_release)
-         
-         537          94 LOAD_CONST              18 ((None,))
-                      96 LOAD_CONST              12 ('font')
-                      98 LOAD_NAME               14 (Font)
-                     100 BUILD_TUPLE              2
-                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\textbox.py", line 537>)
-                     104 MAKE_FUNCTION            5 (defaults, annotations)
-                     106 STORE_NAME              15 (font)
+         474          42 LOAD_CONST              17 ((None,))
+                      44 LOAD_CONST               6 (<code object _focus, file "D:\tkadw\tkadw\canvas\textbox.py", line 474>)
+                      46 MAKE_FUNCTION            1 (defaults)
+                      48 STORE_NAME               7 (_focus)
+         
+         483          50 LOAD_CONST              17 ((None,))
+                      52 LOAD_CONST               7 (<code object _focusout, file "D:\tkadw\tkadw\canvas\textbox.py", line 483>)
+                      54 MAKE_FUNCTION            1 (defaults)
+                      56 STORE_NAME               8 (_focusout)
+         
+         492          58 LOAD_CONST              17 ((None,))
+                      60 LOAD_CONST               8 (<code object _click, file "D:\tkadw\tkadw\canvas\textbox.py", line 492>)
+                      62 MAKE_FUNCTION            1 (defaults)
+                      64 STORE_NAME               9 (_click)
+         
+         495          66 LOAD_CONST              17 ((None,))
+                      68 LOAD_CONST               9 (<code object _hover, file "D:\tkadw\tkadw\canvas\textbox.py", line 495>)
+                      70 MAKE_FUNCTION            1 (defaults)
+                      72 STORE_NAME              10 (_hover)
+         
+         498          74 LOAD_CONST              17 ((None,))
+                      76 LOAD_CONST              10 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\textbox.py", line 498>)
+                      78 MAKE_FUNCTION            1 (defaults)
+                      80 STORE_NAME              11 (_hover_release)
+         
+         509          82 LOAD_CONST              17 ((None,))
+                      84 LOAD_CONST              11 ('font')
+                      86 LOAD_NAME               12 (Font)
+                      88 BUILD_TUPLE              2
+                      90 LOAD_CONST              12 (<code object font, file "D:\tkadw\tkadw\canvas\textbox.py", line 509>)
+                      92 MAKE_FUNCTION            5 (defaults, annotations)
+                      94 STORE_NAME              13 (font)
          
-         543         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 543>)
-                     110 MAKE_FUNCTION            0
-                     112 STORE_NAME              16 (default_palette)
+         515          96 LOAD_CONST              13 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 515>)
+                      98 MAKE_FUNCTION            0
+                     100 STORE_NAME              14 (default_palette)
          
-         546         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\textbox.py", line 546>)
-                     116 MAKE_FUNCTION            0
-                     118 STORE_NAME              17 (palette_light)
+         518         102 LOAD_CONST              14 (<code object palette_light, file "D:\tkadw\tkadw\canvas\textbox.py", line 518>)
+                     104 MAKE_FUNCTION            0
+                     106 STORE_NAME              15 (palette_light)
+         
+         542         108 LOAD_CONST              15 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 542>)
+                     110 MAKE_FUNCTION            0
+                     112 STORE_NAME              16 (palette_dark)
          
-         570         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 570>)
-                     122 MAKE_FUNCTION            0
-                     124 STORE_NAME              18 (palette_dark)
-         
-         594         126 LOAD_CONST              18 ((None,))
-                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 594>)
-                     130 MAKE_FUNCTION            1 (defaults)
-                     132 STORE_NAME              19 (palette)
-                     134 LOAD_CLOSURE             0 (__class__)
-                     136 COPY                     1
-                     138 STORE_NAME              20 (__classcell__)
-                     140 RETURN_VALUE
+         566         114 LOAD_CONST              17 ((None,))
+                     116 LOAD_CONST              16 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 566>)
+                     118 MAKE_FUNCTION            1 (defaults)
+                     120 STORE_NAME              17 (palette)
+                     122 LOAD_CLOSURE             0 (__class__)
+                     124 COPY                     1
+                     126 STORE_NAME              18 (__classcell__)
+                     128 RETURN_VALUE
          consts
             'AdwDrawBasicRoundText3'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               454           2 RESUME                   0
+               426           2 RESUME                   0
                
-               455           4 PUSH_NULL
+               427           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -3832,29 +3727,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '__init__'
-               firstlineno 454
+               firstlineno 426
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               457           0 RESUME                   0
+               429           0 RESUME                   0
                
-               458           2 LOAD_FAST                0 (self)
+               430           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -3872,49 +3767,48 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_other'
-               firstlineno 457
+               firstlineno 429
                lnotab 0x0201
             None
-            'radius'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               460           0 RESUME                   0
+               432           0 RESUME                   0
                
-               461           2 LOAD_FAST                1 (radius)
+               433           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               462           6 LOAD_FAST                0 (self)
+               434           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               464     >>   20 LOAD_FAST                1 (radius)
+               436     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'border_radius'
-               firstlineno 460
+               firstlineno 432
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -3950,195 +3844,195 @@
                   00000000000000000000000000000000007c006a100000000000000000a6
                   010000ab01000000000000000001007c00a0110000000000000000000000
                   0000000000000000007c006a1000000000000000007c006a0c0000000000
                   000000a6020000ab02000000000000000001007c006a0b00000000000000
                   00a01200000000000000000000000000000000000000007c006a07000000
                   00000000007c006a1300000000000000007c006a130000000000000000ac
                   0aa6030000ab030000000000000000010064005300
-               466           0 RESUME                   0
+               438           0 RESUME                   0
                
-               467           2 LOAD_FAST                0 (self)
+               439           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               469          44 LOAD_FAST                0 (self)
+               441          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
-               470          68 LOAD_CONST               2 (0)
+               442          68 LOAD_CONST               2 (0)
                
-               471          70 LOAD_CONST               2 (0)
+               443          70 LOAD_CONST               2 (0)
                
-               472          72 LOAD_FAST                0 (self)
+               444          72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (1)
                            112 BINARY_OP               10 (-)
                
-               473         116 LOAD_FAST                0 (self)
+               445         116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (1)
                            156 BINARY_OP               10 (-)
                
-               474         160 LOAD_FAST                0 (self)
+               446         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (text_radius)
                
-               475         172 LOAD_FAST                0 (self)
+               447         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (text_border_width)
                
-               476         184 LOAD_FAST                0 (self)
+               448         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_text_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_text_back)
                
-               469         208 KW_NAMES                 4
+               441         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 POP_TOP
                
-               479         226 LOAD_CONST               5 ('button_frame')
+               451         226 LOAD_CONST               5 ('button_frame')
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (text_frame)
                
-               481         240 LOAD_FAST                0 (self)
+               453         240 LOAD_FAST                0 (self)
                            242 LOAD_METHOD              9 (create_window)
                
-               482         264 LOAD_FAST                0 (self)
+               454         264 LOAD_FAST                0 (self)
                            266 LOAD_METHOD              2 (winfo_width)
                            288 PRECALL                  0
                            292 CALL                     0
                            302 LOAD_CONST               6 (2)
                            304 BINARY_OP               11 (/)
                            308 LOAD_FAST                0 (self)
                            310 LOAD_METHOD              3 (winfo_height)
                            332 PRECALL                  0
                            336 CALL                     0
                            346 LOAD_CONST               6 (2)
                            348 BINARY_OP               11 (/)
                
-               483         352 LOAD_FAST                0 (self)
+               455         352 LOAD_FAST                0 (self)
                            354 LOAD_METHOD              2 (winfo_width)
                            376 PRECALL                  0
                            380 CALL                     0
                            390 LOAD_FAST                0 (self)
                            392 LOAD_ATTR                5 (text_border_width)
                            402 BINARY_OP               10 (-)
                            406 LOAD_FAST                0 (self)
                            408 LOAD_ATTR               10 (text_padding)
                            418 LOAD_CONST               2 (0)
                            420 BINARY_SUBSCR
                            430 BINARY_OP               10 (-)
                            434 LOAD_CONST               6 (2)
                            436 BINARY_OP               10 (-)
                
-               484         440 LOAD_FAST                0 (self)
+               456         440 LOAD_FAST                0 (self)
                            442 LOAD_METHOD              3 (winfo_height)
                            464 PRECALL                  0
                            468 CALL                     0
                            478 LOAD_FAST                0 (self)
                            480 LOAD_ATTR                5 (text_border_width)
                            490 BINARY_OP               10 (-)
                            494 LOAD_FAST                0 (self)
                            496 LOAD_ATTR               10 (text_padding)
                            506 LOAD_CONST               3 (1)
                            508 BINARY_SUBSCR
                            518 BINARY_OP               10 (-)
                            522 LOAD_CONST               6 (2)
                            524 BINARY_OP               10 (-)
                
-               485         528 LOAD_FAST                0 (self)
+               457         528 LOAD_FAST                0 (self)
                            530 LOAD_ATTR               11 (text)
                
-               481         540 KW_NAMES                 7
+               453         540 KW_NAMES                 7
                            542 PRECALL                  5
                            546 CALL                     5
                            556 LOAD_FAST                0 (self)
                            558 STORE_ATTR              12 (text_text)
                
-               488         568 LOAD_FAST                0 (self)
+               460         568 LOAD_FAST                0 (self)
                            570 LOAD_METHOD             13 (create_rectangle)
                            592 LOAD_CONST               3 (1)
                            594 LOAD_FAST                0 (self)
                            596 LOAD_ATTR                4 (text_radius)
                            606 LOAD_CONST               8 (5)
                            608 BINARY_OP               11 (/)
                            612 BINARY_OP                0 (+)
                
-               489         616 LOAD_FAST                0 (self)
+               461         616 LOAD_FAST                0 (self)
                            618 LOAD_METHOD              3 (winfo_height)
                            640 PRECALL                  0
                            644 CALL                     0
                            654 LOAD_FAST                0 (self)
                            656 LOAD_ATTR               14 (_text_bottom_width)
                            666 BINARY_OP               10 (-)
                            670 LOAD_CONST               3 (1)
                            672 BINARY_OP               10 (-)
                
-               490         676 LOAD_FAST                0 (self)
+               462         676 LOAD_FAST                0 (self)
                            678 LOAD_METHOD              2 (winfo_width)
                            700 PRECALL                  0
                            704 CALL                     0
                            714 LOAD_CONST               3 (1)
                            716 BINARY_OP               10 (-)
                            720 LOAD_FAST                0 (self)
                            722 LOAD_ATTR                4 (text_radius)
                            732 LOAD_CONST               8 (5)
                            734 BINARY_OP               11 (/)
                            738 BINARY_OP               10 (-)
                
-               491         742 LOAD_FAST                0 (self)
+               463         742 LOAD_FAST                0 (self)
                            744 LOAD_METHOD              3 (winfo_height)
                            766 PRECALL                  0
                            770 CALL                     0
                            780 LOAD_CONST               3 (1)
                            782 BINARY_OP               10 (-)
                
-               492         786 LOAD_FAST                0 (self)
+               464         786 LOAD_FAST                0 (self)
                            788 LOAD_ATTR               15 (_text_bottom_line)
                            798 LOAD_FAST                0 (self)
                            800 LOAD_ATTR               15 (_text_bottom_line)
                
-               493         810 LOAD_CONST               2 (0)
+               465         810 LOAD_CONST               2 (0)
                
-               488         812 KW_NAMES                 9
+               460         812 KW_NAMES                 9
                            814 PRECALL                  7
                            818 CALL                     7
                            828 LOAD_FAST                0 (self)
                            830 STORE_ATTR              16 (text_bottom)
                
-               495         840 LOAD_FAST                0 (self)
+               467         840 LOAD_FAST                0 (self)
                            842 LOAD_ATTR               14 (_text_bottom_width)
                            852 LOAD_CONST               2 (0)
                            854 COMPARE_OP               2 (==)
                            860 POP_JUMP_FORWARD_IF_FALSE    26 (to 914)
                
-               496         862 LOAD_FAST                0 (self)
+               468         862 LOAD_FAST                0 (self)
                            864 LOAD_METHOD              0 (delete)
                            886 LOAD_FAST                0 (self)
                            888 LOAD_ATTR               16 (text_bottom)
                            898 PRECALL                  1
                            902 CALL                     1
                            912 POP_TOP
                
-               498     >>  914 LOAD_FAST                0 (self)
+               470     >>  914 LOAD_FAST                0 (self)
                            916 LOAD_METHOD             17 (tag_raise)
                            938 LOAD_FAST                0 (self)
                            940 LOAD_ATTR               16 (text_bottom)
                            950 LOAD_FAST                0 (self)
                            952 LOAD_ATTR               12 (text_text)
                            962 PRECALL                  2
                            966 CALL                     2
                            976 POP_TOP
                
-               500         978 LOAD_FAST                0 (self)
+               472         978 LOAD_FAST                0 (self)
                            980 LOAD_ATTR               11 (text)
                            990 LOAD_METHOD             18 (configure)
                           1012 LOAD_FAST                0 (self)
                           1014 LOAD_ATTR                7 (_text_back)
                           1024 LOAD_FAST                0 (self)
                           1026 LOAD_ATTR               19 (_text_text_back)
                           1036 LOAD_FAST                0 (self)
@@ -4163,15 +4057,15 @@
                   ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_round_rect4', 'winfo_width', 'winfo_height', 'text_radius', 'text_border_width', '_text_border', '_text_back', 'text_frame', 'create_window', 'text_padding', 'text', 'text_text', 'create_rectangle', '_text_bottom_width', '_text_bottom_line', 'text_bottom', 'tag_raise', 'configure', '_text_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_draw'
-               firstlineno 466
+               firstlineno 438
                lnotab
                   0x02012a021801020102012c012c010c010c0118f9120a0e021801580158
                   0158010cfc1c0730013c0142012c01180102fb1c07160134024002
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -4179,42 +4073,42 @@
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               502           0 RESUME                   0
+               474           0 RESUME                   0
                
-               503           2 LOAD_FAST                0 (self)
+               475           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_focusin_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-               504          26 LOAD_FAST                0 (self)
+               476          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_focusin_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-               505          50 LOAD_FAST                0 (self)
+               477          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_focusin_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-               506          74 LOAD_FAST                0 (self)
+               478          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_focusin_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-               507          98 LOAD_FAST                0 (self)
+               479          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_focusin_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-               509         122 LOAD_FAST                0 (self)
+               481         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -4222,56 +4116,56 @@
                   None
                names      ('text_focusin_back', '_text_back', 'text_focusin_border', '_text_border', 'text_focusin_text_back', '_text_text_back', 'text_focusin_bottom_line', '_text_bottom_line', 'text_focusin_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_focus'
-               firstlineno 502
+               firstlineno 474
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               511           0 RESUME                   0
+               483           0 RESUME                   0
                
-               512           2 LOAD_FAST                0 (self)
+               484           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-               513          26 LOAD_FAST                0 (self)
+               485          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-               514          50 LOAD_FAST                0 (self)
+               486          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-               515          74 LOAD_FAST                0 (self)
+               487          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-               516          98 LOAD_FAST                0 (self)
+               488          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-               518         122 LOAD_FAST                0 (self)
+               490         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -4279,66 +4173,66 @@
                   None
                names      ('text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_focusout'
-               firstlineno 511
+               firstlineno 483
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               520           0 RESUME                   0
+               492           0 RESUME                   0
                
-               521           2 LOAD_FAST                0 (self)
+               493           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_set)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('focus_set',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_click'
-               firstlineno 520
+               firstlineno 492
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064005300
-               523           0 RESUME                   0
+               495           0 RESUME                   0
                
-               524           2 LOAD_CONST               1 (True)
+               496           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                   True
                names      ('hover',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_hover'
-               firstlineno 523
+               firstlineno 495
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -4346,179 +4240,179 @@
                   00ab000000000000000000735a64017c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c006a0a00000000000000007c005f0b00000000000000007c00a0
                   0c00000000000000000000000000000000000000006400a6010000ab0100
                   0000000000000001006400530064005300
-               526           0 RESUME                   0
+               498           0 RESUME                   0
                
-               527           2 LOAD_FAST                0 (self)
+               499           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_get)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_JUMP_FORWARD_IF_TRUE    90 (to 222)
                
-               528          42 LOAD_CONST               1 (False)
+               500          42 LOAD_CONST               1 (False)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (hover)
                
-               529          56 LOAD_FAST                0 (self)
+               501          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (text_back)
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_text_back)
                
-               530          80 LOAD_FAST                0 (self)
+               502          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (text_border)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               5 (_text_border)
                
-               531         104 LOAD_FAST                0 (self)
+               503         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (text_text_back)
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               7 (_text_text_back)
                
-               532         128 LOAD_FAST                0 (self)
+               504         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                8 (text_bottom_line)
                            140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               9 (_text_bottom_line)
                
-               533         152 LOAD_FAST                0 (self)
+               505         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR               10 (text_bottom_width)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR              11 (_text_bottom_width)
                
-               535         176 LOAD_FAST                0 (self)
+               507         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD             12 (_draw)
                            200 LOAD_CONST               0 (None)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                
-               527     >>  222 LOAD_CONST               0 (None)
+               499     >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   False
                names      ('focus_get', 'hover', 'text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_hover_release'
-               firstlineno 526
+               firstlineno 498
                lnotab 0x020128010e01180118011801180118022ef8
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               537           0 RESUME                   0
+               509           0 RESUME                   0
                
-               538           2 LOAD_FAST                1 (font)
+               510           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               539           6 LOAD_FAST                0 (self)
+               511           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (text_text_font)
                             18 RETURN_VALUE
                
-               541     >>   20 LOAD_FAST                1 (font)
+               513     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (text_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('text_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'font'
-               firstlineno 537
+               firstlineno 509
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               543           0 RESUME                   0
+               515           0 RESUME                   0
                
-               544           2 LOAD_FAST                0 (self)
+               516           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 543
+               firstlineno 515
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640864066409640a640b640c640d640e9c0ea6
                   010000ab010000000000000000010064005300
-               546           0 RESUME                   0
+               518           0 RESUME                   0
                
-               547           2 LOAD_FAST                0 (self)
+               519           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               549          26 LOAD_CONST               1 (13)
+               521          26 LOAD_CONST               1 (13)
                
-               551          28 LOAD_CONST               2 ((6, 4))
+               523          28 LOAD_CONST               2 ((6, 4))
                
-               553          30 LOAD_CONST               3 ('#f3f3f3')
+               525          30 LOAD_CONST               3 ('#f3f3f3')
                
-               554          32 LOAD_CONST               4 (1)
+               526          32 LOAD_CONST               4 (1)
                
-               555          34 LOAD_CONST               5 (0)
+               527          34 LOAD_CONST               5 (0)
                
-               557          36 LOAD_CONST               6 ('#eaeaea')
+               529          36 LOAD_CONST               6 ('#eaeaea')
                
-               558          38 LOAD_CONST               7 ('#fdfdfd')
+               530          38 LOAD_CONST               7 ('#fdfdfd')
                
-               559          40 LOAD_CONST               8 ('#5f5f5f')
+               531          40 LOAD_CONST               8 ('#5f5f5f')
                
-               560          42 LOAD_CONST               6 ('#eaeaea')
+               532          42 LOAD_CONST               6 ('#eaeaea')
                
-               562          44 LOAD_CONST               9 ('#e2e2e2')
+               534          44 LOAD_CONST               9 ('#e2e2e2')
                
-               563          46 LOAD_CONST              10 ('#f9f9f9')
+               535          46 LOAD_CONST              10 ('#f9f9f9')
                
-               564          48 LOAD_CONST              11 ('#1a1a1a')
+               536          48 LOAD_CONST              11 ('#1a1a1a')
                
-               565          50 LOAD_CONST              12 ('#185fb4')
+               537          50 LOAD_CONST              12 ('#185fb4')
                
-               566          52 LOAD_CONST              13 (2)
+               538          52 LOAD_CONST              13 (2)
                
-               548          54 LOAD_CONST              14 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
+               520          54 LOAD_CONST              14 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
                             56 BUILD_CONST_KEY_MAP     14
                
-               547          58 PRECALL                  1
+               519          58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
                   13
@@ -4537,64 +4431,64 @@
                   ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_light'
-               firstlineno 546
+               firstlineno 518
                lnotab
                   0x0201180202020202020102010202020102010201020202010201020102
                   0102ee04ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640864096405640a6408640b640c640d9c0ea6
                   010000ab010000000000000000010064005300
-               570           0 RESUME                   0
+               542           0 RESUME                   0
                
-               571           2 LOAD_FAST                0 (self)
+               543           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               573          26 LOAD_CONST               1 (13)
+               545          26 LOAD_CONST               1 (13)
                
-               575          28 LOAD_CONST               2 ((3, 4))
+               547          28 LOAD_CONST               2 ((3, 4))
                
-               577          30 LOAD_CONST               3 ('#202020')
+               549          30 LOAD_CONST               3 ('#202020')
                
-               578          32 LOAD_CONST               4 (1)
+               550          32 LOAD_CONST               4 (1)
                
-               580          34 LOAD_CONST               5 ('#454545')
+               552          34 LOAD_CONST               5 ('#454545')
                
-               581          36 LOAD_CONST               6 ('#353535')
+               553          36 LOAD_CONST               6 ('#353535')
                
-               582          38 LOAD_CONST               7 ('#cecece')
+               554          38 LOAD_CONST               7 ('#cecece')
                
-               583          40 LOAD_CONST               8 ('#ffffff')
+               555          40 LOAD_CONST               8 ('#ffffff')
                
-               584          42 LOAD_CONST               9 (0)
+               556          42 LOAD_CONST               9 (0)
                
-               586          44 LOAD_CONST               5 ('#454545')
+               558          44 LOAD_CONST               5 ('#454545')
                
-               587          46 LOAD_CONST              10 ('#2f2f2f')
+               559          46 LOAD_CONST              10 ('#2f2f2f')
                
-               588          48 LOAD_CONST               8 ('#ffffff')
+               560          48 LOAD_CONST               8 ('#ffffff')
                
-               589          50 LOAD_CONST              11 ('#4cc2ff')
+               561          50 LOAD_CONST              11 ('#4cc2ff')
                
-               590          52 LOAD_CONST              12 (2)
+               562          52 LOAD_CONST              12 (2)
                
-               572          54 LOAD_CONST              13 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
+               544          54 LOAD_CONST              13 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
                             56 BUILD_CONST_KEY_MAP     14
                
-               571          58 PRECALL                  1
+               543          58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
                   13
@@ -4612,15 +4506,15 @@
                   ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 570
+               firstlineno 542
                lnotab
                   0x0201180202020202020102020201020102010201020202010201020102
                   0102ee04ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 11
@@ -4642,160 +4536,160 @@
                   000000000000006400a6010000ab01000000000000000001006400530023
                   00741e000000000000000000002400720401005900640053007700780359
                   0077017c006a0100000000000000007c006a0200000000000000007c006a
                   0300000000000000007c006a0800000000000000007c006a040000000000
                   0000007c006a0500000000000000007c006a0600000000000000007c006a
                   0900000000000000007c006a0a00000000000000007c006a0b0000000000
                   000000640f9c0a5300
-               594           0 RESUME                   0
+               566           0 RESUME                   0
                
-               595           2 LOAD_FAST                1 (dict)
+               567           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE   223 (to 452)
                
-               596           6 LOAD_FAST                1 (dict)
+               568           6 LOAD_FAST                1 (dict)
                              8 LOAD_CONST               1 ('text_radius')
                             10 BINARY_SUBSCR
                             20 LOAD_FAST                0 (self)
                             22 STORE_ATTR               0 (text_radius)
                
-               598          32 LOAD_FAST                1 (dict)
+               570          32 LOAD_FAST                1 (dict)
                             34 LOAD_CONST               2 ('text_padding')
                             36 BINARY_SUBSCR
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               1 (text_padding)
                
-               600          58 LOAD_FAST                1 (dict)
+               572          58 LOAD_FAST                1 (dict)
                             60 LOAD_CONST               3 ('text_frame_back')
                             62 BINARY_SUBSCR
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (text_frame_back)
                
-               601          84 LOAD_FAST                1 (dict)
+               573          84 LOAD_FAST                1 (dict)
                             86 LOAD_CONST               4 ('text_border_width')
                             88 BINARY_SUBSCR
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               3 (text_border_width)
                
-               603         110 LOAD_FAST                1 (dict)
+               575         110 LOAD_FAST                1 (dict)
                            112 LOAD_CONST               5 ('text_border')
                            114 BINARY_SUBSCR
                            124 LOAD_FAST                0 (self)
                            126 STORE_ATTR               4 (text_border)
                
-               604         136 LOAD_FAST                1 (dict)
+               576         136 LOAD_FAST                1 (dict)
                            138 LOAD_CONST               6 ('text_back')
                            140 BINARY_SUBSCR
                            150 LOAD_FAST                0 (self)
                            152 STORE_ATTR               5 (text_back)
                
-               605         162 LOAD_FAST                1 (dict)
+               577         162 LOAD_FAST                1 (dict)
                            164 LOAD_CONST               7 ('text_text_back')
                            166 BINARY_SUBSCR
                            176 LOAD_FAST                0 (self)
                            178 STORE_ATTR               6 (text_text_back)
                
-               606         188 LOAD_FAST                1 (dict)
+               578         188 LOAD_FAST                1 (dict)
                            190 LOAD_CONST               8 ('text_bottom_line')
                            192 BINARY_SUBSCR
                            202 LOAD_FAST                0 (self)
                            204 STORE_ATTR               7 (text_bottom_line)
                
-               607         214 LOAD_FAST                1 (dict)
+               579         214 LOAD_FAST                1 (dict)
                            216 LOAD_CONST               9 ('text_bottom_width')
                            218 BINARY_SUBSCR
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (text_bottom_width)
                
-               609         240 LOAD_FAST                1 (dict)
+               581         240 LOAD_FAST                1 (dict)
                            242 LOAD_CONST              10 ('text_focusin_border')
                            244 BINARY_SUBSCR
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (text_focusin_border)
                
-               610         266 LOAD_FAST                1 (dict)
+               582         266 LOAD_FAST                1 (dict)
                            268 LOAD_CONST              11 ('text_focusin_back')
                            270 BINARY_SUBSCR
                            280 LOAD_FAST                0 (self)
                            282 STORE_ATTR              10 (text_focusin_back)
                
-               611         292 LOAD_FAST                1 (dict)
+               583         292 LOAD_FAST                1 (dict)
                            294 LOAD_CONST              12 ('text_focusin_text_back')
                            296 BINARY_SUBSCR
                            306 LOAD_FAST                0 (self)
                            308 STORE_ATTR              11 (text_focusin_text_back)
                
-               612         318 LOAD_FAST                1 (dict)
+               584         318 LOAD_FAST                1 (dict)
                            320 LOAD_CONST              13 ('text_focusin_bottom_line')
                            322 BINARY_SUBSCR
                            332 LOAD_FAST                0 (self)
                            334 STORE_ATTR              12 (text_focusin_bottom_line)
                
-               613         344 LOAD_FAST                1 (dict)
+               585         344 LOAD_FAST                1 (dict)
                            346 LOAD_CONST              14 ('text_focusin_bottom_width')
                            348 BINARY_SUBSCR
                            358 LOAD_FAST                0 (self)
                            360 STORE_ATTR              13 (text_focusin_bottom_width)
                
-               615         370 NOP
+               587         370 NOP
                
-               616         372 LOAD_FAST                0 (self)
+               588         372 LOAD_FAST                0 (self)
                            374 LOAD_METHOD             14 (_draw)
                            396 LOAD_CONST               0 (None)
                            398 PRECALL                  1
                            402 CALL                     1
                            412 POP_TOP
                            414 LOAD_CONST               0 (None)
                            416 RETURN_VALUE
                        >>  418 PUSH_EXC_INFO
                
-               617         420 LOAD_GLOBAL             30 (AttributeError)
+               589         420 LOAD_GLOBAL             30 (AttributeError)
                            432 CHECK_EXC_MATCH
                            434 POP_JUMP_FORWARD_IF_FALSE     4 (to 444)
                            436 POP_TOP
                
-               618         438 POP_EXCEPT
+               590         438 POP_EXCEPT
                            440 LOAD_CONST               0 (None)
                            442 RETURN_VALUE
                
-               617     >>  444 RERAISE                  0
+               589     >>  444 RERAISE                  0
                        >>  446 COPY                     3
                            448 POP_EXCEPT
                            450 RERAISE                  1
                
-               621     >>  452 LOAD_FAST                0 (self)
+               593     >>  452 LOAD_FAST                0 (self)
                            454 LOAD_ATTR                1 (text_padding)
                
-               623         464 LOAD_FAST                0 (self)
+               595         464 LOAD_FAST                0 (self)
                            466 LOAD_ATTR                2 (text_frame_back)
                
-               624         476 LOAD_FAST                0 (self)
+               596         476 LOAD_FAST                0 (self)
                            478 LOAD_ATTR                3 (text_border_width)
                
-               625         488 LOAD_FAST                0 (self)
+               597         488 LOAD_FAST                0 (self)
                            490 LOAD_ATTR                8 (text_bottom_width)
                
-               627         500 LOAD_FAST                0 (self)
+               599         500 LOAD_FAST                0 (self)
                            502 LOAD_ATTR                4 (text_border)
                
-               628         512 LOAD_FAST                0 (self)
+               600         512 LOAD_FAST                0 (self)
                            514 LOAD_ATTR                5 (text_back)
                
-               629         524 LOAD_FAST                0 (self)
+               601         524 LOAD_FAST                0 (self)
                            526 LOAD_ATTR                6 (text_text_back)
                
-               631         536 LOAD_FAST                0 (self)
+               603         536 LOAD_FAST                0 (self)
                            538 LOAD_ATTR                9 (text_focusin_border)
                
-               632         548 LOAD_FAST                0 (self)
+               604         548 LOAD_FAST                0 (self)
                            550 LOAD_ATTR               10 (text_focusin_back)
                
-               633         560 LOAD_FAST                0 (self)
+               605         560 LOAD_FAST                0 (self)
                            562 LOAD_ATTR               11 (text_focusin_text_back)
                
-               620         572 LOAD_CONST              15 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back'))
+               592         572 LOAD_CONST              15 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back'))
                            574 BUILD_CONST_KEY_MAP     10
                            576 RETURN_VALUE
                ExceptionTable:
                  372 to 412 -> 418 [0]
                  418 to 436 -> 446 [1] lasti
                  444 to 444 -> 446 [1] lasti
                consts
@@ -4817,139 +4711,139 @@
                   ('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back')
                names      ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette'
-               firstlineno 594
+               firstlineno 566
                lnotab
                   0x020104011a021a021a011a021a011a011a011a011a021a011a011a011a
                   011a0202013001120106ff08040c020c010c010c020c010c010c020c010c
                   010cf3
             (None,)
-         names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'float', 'int', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawBasicRoundText3'
-         firstlineno 453
-         lnotab 0x0c010a030603140606240809080908030803080b0e06060306180618
+         firstlineno 425
+         lnotab 0x0c010a030603080606240809080908030803080b0e06060306180618
       'AdwDrawBasicRoundText3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         637           0 RESUME                   0
+         609           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundText3')
                        8 STORE_NAME               2 (__qualname__)
          
-         638          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 638>)
+         610          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 610>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundText3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               638           0 RESUME                   0
+               610           0 RESUME                   0
                
-               639           2 LOAD_FAST                0 (self)
+               611           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 638
+               firstlineno 610
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawRoundText3'
-         firstlineno 637
+         firstlineno 609
          lnotab 0x0a01
       'AdwDrawRoundText3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         642           0 RESUME                   0
+         614           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkText3')
                        8 STORE_NAME               2 (__qualname__)
          
-         643          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 643>)
+         615          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 615>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkText3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               643           0 RESUME                   0
+               615           0 RESUME                   0
                
-               644           2 LOAD_FAST                0 (self)
+               616           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 643
+               firstlineno 615
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawRoundDarkText3'
-         firstlineno 642
+         firstlineno 614
          lnotab 0x0a01
       'AdwDrawRoundDarkText3'
       '__main__'
       ('Tk',)
       'x'
       5
       ('fill', 'padx', 'pady')
@@ -4958,10 +4852,10 @@
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c041c7f00791c051c061c7f00331c051c051c7f00391c
+      0x00ff020110010c041c7f007a1c051c061c7f00161c051c051c7f00391c
       051c050c010c021402140130021401300214013002140130021401300214
       0130022ce9
```

### Comparing `tkadw-0.1.5/tkadw/canvas/button.py` & `tkadw-0.2.0/tkadw/canvas/button.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
         self.default_palette()
 
         self.text = text
 
         self._button_back = self.button_back
         self._button_border = self.button_border
+        self._button_border_width = self.button_border_width
         self._button_text_back = self.button_text_back
 
         self.button_text_font = nametofont("TkDefaultFont")
 
         self.bind("<Configure>", self._draw, add="+")
         self.bind("<Button>", self._click, add="+")
         self.bind("<ButtonRelease>", self._unclick, add="+")
@@ -45,56 +46,60 @@
             self.configure(background=self.button_frame_back, borderwidth=0)
 
     def _draw(self, evt):
         self.delete("all")
 
         self.button_frame = self.create_rectangle(
             1.5, 1.5, self.winfo_width() - 3, self.winfo_height() - 3,
-            width=self.button_border_width,
+            width=self._button_border_width,
             outline=self._button_border, fill=self._button_back,
         )
 
         self.button_text = self.create_text(
             self.winfo_width() / 2, self.winfo_height() / 2,
             text=self.text, fill=self._button_text_back,
             font=self.button_text_font
         )
 
     def _click(self, evt=None):
         self.hover = True
         self._button_back = self.button_pressed_back
         self._button_border = self.button_pressed_border
+        self._button_border_width = self.button_pressed_border_width
         self._button_text_back = self.button_pressed_text_back
 
         self.focus_set()
 
         self._draw(None)
 
     def _unclick(self, evt=None):
         if self.hover:
             self._button_back = self.button_active_back
             self._button_border = self.button_active_border
+            self._button_border_width = self.button_active_border_width
             self._button_text_back = self.button_active_text_back
 
             self._draw(None)
 
             self.event_generate("<<Click>>")
 
     def _hover(self, evt=None):
         self.hover = True
         self._button_back = self.button_active_back
         self._button_border = self.button_active_border
+        self._button_border_width = self.button_active_border_width
         self._button_text_back = self.button_active_text_back
 
         self._draw(None)
 
     def _hover_release(self, evt=None):
         self.hover = False
         self._button_back = self.button_back
         self._button_border = self.button_border
+        self._button_border_width = self.button_border_width
         self._button_text_back = self.button_text_back
 
         self._draw(None)
 
     def font(self, font: Font = None):
         if font is None:
             return self.button_text_font
@@ -103,91 +108,91 @@
 
     def default_palette(self):
         self.palette_light()
 
     def palette_light(self):
         self.palette(
             {
-                "button_frame_back": "#f3f3f3",
-
-                "button_border_width": 1,
-
-                "button_border": "#eaeaea",
-                "button_back": "#fdfdfd",
-                "button_text_back": "#1a1a1a",
-
-                "button_active_border": "#e2e2e2",
-                "button_active_back": "#f9f9f9",
-                "button_active_text_back": "#5f5f5f",
-
-                "button_pressed_border": "#e2e2e2",
-                "button_pressed_back": "#f9f9f9",
-                "button_pressed_text_back": "#8a8a8a",
+                "button": {
+                    "back": "#fdfdfd",
+                    "border": "#eaeaea",
+                    "text_back": "#1a1a1a",
+                    "border_width": 1,
+
+                    "active": {
+                        "back": "#f9f9f9",
+                        "border": "#aaaaaa",
+                        "text_back": "#5f5f5f",
+                        "border_width": 1,
+                    },
+
+                    "pressed": {
+                        "back": "#f9f9f9",
+                        "border": "#e2e2e2",
+                        "text_back": "#8a8a8a",
+                        "border_width": 1,
+                    },
+                }
             }
         )
 
     def palette_dark(self):
         self.palette(
             {
-                "button_frame_back": "#202020",
-
-                "button_border_width": 1,
-
-                "button_border": "#454545",
-                "button_back": "#353535",
-                "button_text_back": "#ffffff",
-
-                "button_active_border": "#454545",
-                "button_active_back": "#3a3a3a",
-                "button_active_text_back": "#cecece",
-
-                "button_pressed_border": "#454545",
-                "button_pressed_back": "#2f2f2f",
-                "button_pressed_text_back": "#9a9a9a",
+                "button": {
+                    "back": "#353535",
+                    "border": "#454545",
+                    "text_back": "#ffffff",
+                    "border_width": 1,
+
+                    "active": {
+                        "back": "#3a3a3a",
+                        "border": "#454545",
+                        "text_back": "#cecece",
+                        "border_width": 1,
+                    },
+
+                    "pressed": {
+                        "back": "#2f2f2f",
+                        "border": "#454545",
+                        "text_back": "#9a9a9a",
+                        "border_width": 1,
+                    },
+                }
             }
         )
 
     def palette(self, dict=None):
         if dict is not None:
-            self.button_frame_back = dict["button_frame_back"]
-            self.button_border_width = dict["button_border_width"]
+            if "button" in dict:
+                self.button_back = dict["button"]["back"]
+                self.button_border = dict["button"]["border"]
+                self.button_text_back = dict["button"]["text_back"]
+                self.button_border_width = dict["button"]["border_width"]
+
+                if "active" in dict["button"]:
+                    self.button_active_back = dict["button"]["active"]["back"]
+                    self.button_active_border = dict["button"]["active"]["border"]
+                    self.button_active_text_back = dict["button"]["active"]["text_back"]
+                    self.button_active_border_width = dict["button"]["active"]["border_width"]
+
+                if "pressed" in dict["button"]:
+                    self.button_pressed_back = dict["button"]["pressed"]["back"]
+                    self.button_pressed_border = dict["button"]["pressed"]["border"]
+                    self.button_pressed_text_back = dict["button"]["pressed"]["text_back"]
+                    self.button_pressed_border_width = dict["button"]["pressed"]["border_width"]
 
-            self.button_border = dict["button_border"]
-            self.button_back = dict["button_back"]
-            self.button_text_back = dict["button_text_back"]
-
-            self.button_active_border = dict["button_active_border"]
-            self.button_active_back = dict["button_active_back"]
-            self.button_active_text_back = dict["button_active_text_back"]
-
-            self.button_pressed_border = dict["button_pressed_border"]
-            self.button_pressed_back = dict["button_pressed_back"]
-            self.button_pressed_text_back = dict["button_pressed_text_back"]
+            self._palette = dict
 
             try:
                 self._draw(None)
             except AttributeError:
                 pass
         else:
-            return {
-                "button_frame_back": self.button_frame_back,
-                "button_border_width": self.button_border_width,
-
-                "button_border": self.button_border,
-                "button_back": self.button_back,
-                "button_text_back": self.button_text_back,
-
-                "button_active_border": self.button_active_border,
-                "button_active_back": self.button_active_back,
-                "button_active_text_back": self.button_active_text_back,
-
-                "button_pressed_border": self.button_pressed_border,
-                "button_pressed_back": self.button_pressed_back,
-                "button_pressed_text_back": self.button_pressed_text_back,
-            }
+            return self._palette
 
 
 class AdwDrawButton(AdwDrawBasicButton):
     def default_palette(self):
         self.palette_light()
 
 
@@ -196,53 +201,52 @@
         self.palette_dark()
 
 
 class AdwDrawAccentButton(AdwDrawBasicButton):
     def default_palette(self):
         self.palette(
             {
-                "button_frame_back": "#0067c0",
-
-                "button_border_width": 1,
-
-                "button_border": "#1473c5",
-                "button_back": "#0067c0",
-                "button_text_back": "#ffffff",
-
-                "button_active_border": "#1473c5",
-                "button_active_back": "#1975c5",
-                "button_active_text_back": "#ffffff",
-
-                "button_pressed_border": "#3284cb",
-                "button_pressed_back": "#3284cb",
-                "button_pressed_text_back": "#fdfdfd",
+                "button": {
+                    "back": "#0067c0",
+                    "border": "#1473c5",
+                    "text_back": "#ffffff",
+                    "border_width": 1,
+
+                    "active": {
+                        "back": "#1975c5",
+                        "border": "#1473c5",
+                        "text_back": "#ffffff",
+                        "border_width": 1,
+                    },
+
+                    "pressed": {
+                        "back": "#3284cb",
+                        "border": "#3284cb",
+                        "text_back": "#fdfdfd",
+                        "border_width": 1,
+                    },
+                }
             }
         )
 
 
 # Round Button
 class AdwDrawBasicRoundButton(AdwDrawBasicButton):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def _other(self):
         self.configure(background=self.master.cget("bg"), borderwidth=0)
 
-    def border_radius(self, radius: float | int = None):
-        if radius is None:
-            return self.button_radius
-        else:
-            self.button_radius = radius
-
     def _draw(self, evt):
         self.delete("all")
 
         self.button_frame = self.create_round_rect2(
             2, 2, self.winfo_width()-3, self.winfo_height()-3, self.button_radius,
-            width=self.button_border_width,
+            width=self._button_border_width,
             outline=self._button_border, fill=self._button_back,
         )
 
         self.button_text = self.create_text(
             self.winfo_width() / 2, self.winfo_height() / 2,
             text=self.text, fill=self._button_text_back,
             font=self.button_text_font
@@ -250,119 +254,101 @@
 
     def default_palette(self):
         self.palette_light()
 
     def palette_light(self):
         self.palette(
             {
-                "button_radius": 8,
-
-                "button_border_width": 1,
-
-                "button_border": "#eaeaea",
-                "button_back": "#fdfdfd",
-                "button_text_back": "#1a1a1a",
-
-                "button_active_border": "#e2e2e2",
-                "button_active_back": "#f9f9f9",
-                "button_active_text_back": "#5f5f5f",
-
-                "button_pressed_border": "#e2e2e2",
-                "button_pressed_back": "#f9f9f9",
-                "button_pressed_text_back": "#8a8a8a",
+                "button": {
+                    "radius": 8,
+                    "back": "#fdfdfd",
+                    "border": "#eaeaea",
+                    "text_back": "#1a1a1a",
+                    "border_width": 1,
+
+                    "active": {
+                        "back": "#f9f9f9",
+                        "border": "#454545",
+                        "text_back": "#5f5f5f",
+                        "border_width": 1,
+                    },
+
+                    "pressed": {
+                        "back": "#f9f9f9",
+                        "border": "#e2e2e2",
+                        "text_back": "#8a8a8a",
+                        "border_width": 1,
+                    },
+                }
             }
         )
 
     def palette_dark(self):
         self.palette(
             {
-                "button_radius": 8,
-
-                "button_border_width": 1,
-
-                "button_border": "#454545",
-                "button_back": "#353535",
-                "button_text_back": "#ffffff",
-
-                "button_active_border": "#454545",
-                "button_active_back": "#3a3a3a",
-                "button_active_text_back": "#cecece",
-
-                "button_pressed_border": "#454545",
-                "button_pressed_back": "#2f2f2f",
-                "button_pressed_text_back": "#9a9a9a",
+                "button": {
+                    "radius": 8,
+                    "back": "#353535",
+                    "border": "#454545",
+                    "text_back": "#ffffff",
+                    "border_width": 1,
+
+                    "active": {
+                        "back": "#3a3a3a",
+                        "border": "#454545",
+                        "text_back": "#cecece",
+                        "border_width": 1,
+                    },
+
+                    "pressed": {
+                        "back": "#2f2f2f",
+                        "border": "#454545",
+                        "text_back": "#9a9a9a",
+                        "border_width": 1,
+                    },
+                }
             }
         )
 
     def palette(self, dict=None):
-        if dict is not None:
-            self.button_radius = dict["button_radius"]
-
-            self.button_border_width = dict["button_border_width"]
-
-            self.button_border = dict["button_border"]
-            self.button_back = dict["button_back"]
-            self.button_text_back = dict["button_text_back"]
-
-            self.button_active_border = dict["button_active_border"]
-            self.button_active_back = dict["button_active_back"]
-            self.button_active_text_back = dict["button_active_text_back"]
-
-            self.button_pressed_border = dict["button_pressed_border"]
-            self.button_pressed_back = dict["button_pressed_back"]
-            self.button_pressed_text_back = dict["button_pressed_text_back"]
-
-            try:
-                self._draw(None)
-            except AttributeError:
-                pass
-        else:
-            return {
-                "button_frame_back": self.button_frame_back,
-
-                "button_border_width": self.button_border_width,
-
-                "button_border": self.button_border,
-                "button_back": self.button_back,
-                "button_text_back": self.button_text_back,
-
-                "button_active_border": self.button_active_border,
-                "button_active_back": self.button_active_back,
-                "button_active_text_back": self.button_active_text_back,
-
-                "button_pressed_border": self.button_pressed_border,
-                "button_pressed_back": self.button_pressed_back,
-                "button_pressed_text_back": self.button_pressed_text_back,
-            }
+        super().palette(dict)
+        if "button" in dict:
+            self.button_radius = dict["button"]["radius"]
 
 
 class AdwDrawRoundButton(AdwDrawBasicRoundButton):
     def default_palette(self):
         self.palette_light()
 
 
 class AdwDrawRoundAccentButton(AdwDrawBasicRoundButton):
     def default_palette(self):
         self.palette(
             {
-                "button_radius": 8,
-
-                "button_border_width": 1,
-
-                "button_border": "#1473c5",
-                "button_back": "#0067c0",
-                "button_text_back": "#ffffff",
-
-                "button_active_border": "#1473c5",
-                "button_active_back": "#1975c5",
-                "button_active_text_back": "#ffffff",
-
-                "button_pressed_border": "#3284cb",
-                "button_pressed_back": "#3284cb",
-                "button_pressed_text_back": "#fdfdfd",
+                "button": {
+                    "radius": 8,
+                    "back": "#0067c0",
+                    "border": "#1473c5",
+                    "text_back": "#ffffff",
+                    "border_width": 1,
+
+                    "active": {
+                        "back": "#1975c5",
+                        "border": "#1473c5",
+                        "text_back": "#ffffff",
+                        "border_width": 1,
+                    },
+
+                    "pressed": {
+                        "back": "#3284cb",
+                        "border": "#3284cb",
+                        "text_back": "#fdfdfd",
+                        "border_width": 1,
+                    },
+                }
             }
         )
 
 
 class AdwDrawRoundDarkButton(AdwDrawBasicRoundButton):
     def default_palette(self):
         self.palette_dark()
@@ -390,45 +376,51 @@
         self.palette_light()
 
 
 class AdwDrawRoundAccentButton2(AdwDrawRoundButton2):
     def default_palette(self):
         self.palette(
             {
-                "button_radius": 8,
-
-                "button_border_width": 1,
-
-                "button_border": "#1473c5",
-                "button_back": "#0067c0",
-                "button_text_back": "#ffffff",
-
-                "button_active_border": "#1473c5",
-                "button_active_back": "#1975c5",
-                "button_active_text_back": "#ffffff",
-
-                "button_pressed_border": "#3284cb",
-                "button_pressed_back": "#3284cb",
-                "button_pressed_text_back": "#fdfdfd",
+                "button": {
+                    "radius": 8,
+                    "back": "#0067c0",
+                    "border": "#1473c5",
+                    "text_back": "#ffffff",
+                    "border_width": 1,
+
+                    "active": {
+                        "back": "#1975c5",
+                        "border": "#1473c5",
+                        "text_back": "#ffffff",
+                        "border_width": 1,
+                    },
+
+                    "pressed": {
+                        "back": "#3284cb",
+                        "border": "#3284cb",
+                        "text_back": "#fdfdfd",
+                        "border_width": 1,
+                    },
+                }
             }
         )
 
 
 class AdwDrawRoundDarkButton2(AdwDrawRoundButton2):
     def default_palette(self):
         self.palette_dark()
 
 
 class AdwDrawRoundButton3(AdwDrawBasicRoundButton):
     def _draw(self, evt):
         self.delete("all")
 
         self.create_round_rect4(
-            self.button_border_width + 1, self.button_border_width + 1, self.winfo_width() - self.button_border_width -2, self.winfo_height() - self.button_border_width -2, self.button_radius,
-            width=self.button_border_width,
+            1, 1, self.winfo_width() - 2, self.winfo_height() - 2, self.button_radius,
+            width=self._button_border_width,
             outline=self._button_border, fill=self._button_back,
         )
 
         self.button_frame = "button_frame"
 
         self.button_text = self.create_text(
             self.winfo_width() / 2, self.winfo_height() / 2,
@@ -440,29 +432,35 @@
         self.palette_light()
 
 
 class AdwDrawRoundAccentButton3(AdwDrawRoundButton3):
     def default_palette(self):
         self.palette(
             {
-                "button_radius": 8,
-
-                "button_border_width": 1,
-
-                "button_border": "#1473c5",
-                "button_back": "#0067c0",
-                "button_text_back": "#ffffff",
-
-                "button_active_border": "#1473c5",
-                "button_active_back": "#1975c5",
-                "button_active_text_back": "#ffffff",
-
-                "button_pressed_border": "#3284cb",
-                "button_pressed_back": "#3284cb",
-                "button_pressed_text_back": "#fdfdfd",
+                "button": {
+                    "radius": 8,
+                    "back": "#0067c0",
+                    "border": "#1473c5",
+                    "text_back": "#ffffff",
+                    "border_width": 1,
+
+                    "active": {
+                        "back": "#1975c5",
+                        "border": "#1473c5",
+                        "text_back": "#ffffff",
+                        "border_width": 1,
+                    },
+
+                    "pressed": {
+                        "back": "#3284cb",
+                        "border": "#3284cb",
+                        "text_back": "#fdfdfd",
+                        "border_width": 1,
+                    },
+                }
             }
         )
 
 
 class AdwDrawRoundDarkButton3(AdwDrawRoundButton3):
     def default_palette(self):
         self.palette_dark()
```

### Comparing `tkadw-0.1.5/tkadw/canvas/drawengine.py` & `tkadw-0.2.0/tkadw/canvas/drawengine.py`

 * *Files 2% similar despite different names*

```diff
@@ -575,14 +575,20 @@
             f.close()
         image = SvgImage(file=file)
 
         i = self.create_image(x, y, image=image, **kwargs)
 
         return i
 
+    def draw_copy_icon(self, __x, __y, size=10, padding=10, radius=18):
+        _1 = self.create_round_rect4(__x, __y, __x+size*5, __y+size*5, radius)
+        _2 = self.create_round_rect4(__x+padding, __y+padding, __x+size*5-padding, __y+size*5-padding, radius/2, fill="white")
+        _3 = self.create_round_rect4(__x+size*2, __y+size*2, __x+size*7, __y+size*7, radius)
+        _4 = self.create_round_rect4(__x+size*2+padding, __y+size*2+padding, __x+size*7-padding, __y+size*7-padding, radius/2, fill="white")
+        return _1, _2, _3, _4
 
 if __name__ == '__main__':
     from tkinter import Tk
 
     root = Tk()
 
     canvas = AdwDrawEngine()
```

### Comparing `tkadw-0.1.5/tkadw/canvas/fun.py` & `tkadw-0.2.0/tkadw/canvas/fun.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/canvas/fun2.py` & `tkadw-0.2.0/tkadw/canvas/fun2.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/canvas/fun3.py` & `tkadw-0.2.0/tkadw/canvas/fun3.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/canvas/fun4.py` & `tkadw-0.2.0/tkadw/canvas/fun4.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/canvas/fun5.py` & `tkadw-0.2.0/tkadw/canvas/fun5.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/canvas/fun6.py` & `tkadw-0.2.0/tkadw/canvas/fun6.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/canvas/poly.tcl` & `tkadw-0.2.0/tkadw/canvas/poly.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/canvas/textbox.py` & `tkadw-0.2.0/tkadw/canvas/textbox.py`

 * *Files 16% similar despite different names*

```diff
@@ -165,94 +165,95 @@
 
     def default_palette(self):
         self.palette_light()
 
     def palette_light(self):
         self.palette(
             {
-                "text_padding": (3, 4),
+                "text": {
+                    "padding": (3, 4),
 
-                "text_frame_back": "#f3f3f3",
-                "text_border_width": 1,
-                "text_bottom_width": 0,
-
-                "text_border": "#eaeaea",
-                "text_back": "#fdfdfd",
-                "text_text_back": "#5f5f5f",
-                "text_bottom_line": "#eaeaea",
-
-                "text_focusin_border": "#e2e2e2",
-                "text_focusin_back": "#f9f9f9",
-                "text_focusin_text_back": "#1a1a1a",
-                "text_focusin_bottom_line": "#185fb4",
-                "text_focusin_bottom_width": 2,
+                    "back": "#fdfdfd",
+                    "border": "#eaeaea",
+                    "text_back": "#5f5f5f",
+                    "border_width": 1,
+
+                    "bottom_line": "#eaeaea",
+                    "bottom_width": 0,
+
+                    "focusin": {
+                        "back": "#f9f9f9",
+                        "border": "#e2e2e2",
+                        "text_back": "#1a1a1a",
+                        "border_width": 1,
+
+                        "bottom_line": "#185fb4",
+                        "bottom_width": 2,
+                    }
+                },
             }
         )
 
     def palette_dark(self):
         self.palette(
             {
-                "text_padding": (3, 4),
+                "text": {
+                    "padding": (3, 4),
 
-                "text_frame_back": "#202020",
-                "text_border_width": 1,
-
-                "text_border": "#454545",
-                "text_back": "#353535",
-                "text_text_back": "#cecece",
-                "text_bottom_line": "#ffffff",
-                "text_bottom_width": 0,
-
-                "text_focusin_border": "#454545",
-                "text_focusin_back": "#2f2f2f",
-                "text_focusin_text_back": "#ffffff",
-                "text_focusin_bottom_line": "#4cc2ff",
-                "text_focusin_bottom_width": 2,
+                    "back": "#353535",
+                    "border": "#454545",
+                    "text_back": "#cecece",
+                    "border_width": 1,
+
+                    "bottom_line": "#ffffff",
+                    "bottom_width": 0,
+
+                    "focusin": {
+                        "back": "#2f2f2f",
+                        "border": "#454545",
+                        "text_back": "#ffffff",
+                        "border_width": 1,
+
+                        "bottom_line": "#4cc2ff",
+                        "bottom_width": 2,
+                    }
+                },
             }
         )
 
     def palette(self, dict=None):
         if dict is not None:
-            self.text_padding = dict["text_padding"]
+            if "text" in dict:
+                self.text_padding = dict["text"]["padding"]
+
+                self.text_back = dict["text"]["back"]
+                self.text_border = dict["text"]["border"]
+                self.text_text_back = dict["text"]["text_back"]
+                self.text_border_width = dict["text"]["border_width"]
+
+                self.text_bottom_line = dict["text"]["bottom_line"]
+                self.text_bottom_width = dict["text"]["bottom_width"]
+
+                if "focusin" in dict["text"]:
+                    self.text_focusin_back = dict["text"]["focusin"]["back"]
+                    self.text_focusin_border = dict["text"]["focusin"]["border"]
+                    self.text_focusin_text_back = dict["text"]["focusin"]["text_back"]
+                    self.text_focusin_border_width = dict["text"]["focusin"]["border_width"]
 
-            self.text_frame_back = dict["text_frame_back"]
-            self.text_border_width = dict["text_border_width"]
+                    self.text_focusin_bottom_line = dict["text"]["focusin"]["bottom_line"]
+                    self.text_focusin_bottom_width = dict["text"]["focusin"]["bottom_width"]
 
-            self.text_border = dict["text_border"]
-            self.text_back = dict["text_back"]
-            self.text_text_back = dict["text_text_back"]
-            self.text_bottom_line = dict["text_bottom_line"]
-            self.text_bottom_width = dict["text_bottom_width"]
-
-            self.text_focusin_border = dict["text_focusin_border"]
-            self.text_focusin_back = dict["text_focusin_back"]
-            self.text_focusin_text_back = dict["text_focusin_text_back"]
-            self.text_focusin_bottom_line = dict["text_focusin_bottom_line"]
-            self.text_focusin_bottom_width = dict["text_focusin_bottom_width"]
+            self._palette = dict
 
             try:
                 self._draw(None)
             except AttributeError:
                 pass
         else:
-            return {
-                "text_padding": self.text_padding,
-
-                "text_frame_back": self.text_frame_back,
-                "text_border_width": self.text_border_width,
-                "text_bottom_width": self.text_bottom_width,
-
-                "text_border": self.text_border,
-                "text_back": self.text_back,
-                "text_text_back": self.text_text_back,
-
-                "text_focusin_border": self.text_focusin_border,
-                "text_focusin_back": self.text_focusin_back,
-                "text_focusin_text_back": self.text_focusin_text_back,
-            }
+            return self._palette
 
 
 class AdwDrawText(AdwDrawBasicText):
     def default_palette(self):
         self.palette_light()
 
 
@@ -265,15 +266,15 @@
 class AdwDrawBasicRoundText(AdwDrawBasicText):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def _other(self):
         self.configure(background=self.master.cget("bg"), borderwidth=0)
 
-    def border_radius(self, radius: float | int = None):
+    def border_radius(self, radius=None):
         if radius is None:
             return self.button_radius
         else:
             self.button_radius = radius
 
     def _draw(self, evt):
         self.delete("all")
@@ -348,100 +349,71 @@
 
     def default_palette(self):
         self.palette_light()
 
     def palette_light(self):
         self.palette(
             {
-                "text_radius": 6,
-
-                "text_padding": (3, 4),
-
-                "text_frame_back": "#f3f3f3",
-                "text_border_width": 1,
-                "text_bottom_width": 0,
-
-                "text_border": "#eaeaea",
-                "text_back": "#fdfdfd",
-                "text_text_back": "#5f5f5f",
-                "text_bottom_line": "#eaeaea",
-
-                "text_focusin_border": "#e2e2e2",
-                "text_focusin_back": "#f9f9f9",
-                "text_focusin_text_back": "#1a1a1a",
-                "text_focusin_bottom_line": "#185fb4",
-                "text_focusin_bottom_width": 2,
+                "text": {
+                    "radius": 6,
+                    "padding": (3, 4),
+
+                    "back": "#fdfdfd",
+                    "border": "#eaeaea",
+                    "text_back": "#5f5f5f",
+                    "border_width": 1,
+
+                    "bottom_line": "#eaeaea",
+                    "bottom_width": 0,
+
+                    "focusin": {
+                        "back": "#f9f9f9",
+                        "border": "#e2e2e2",
+                        "text_back": "#1a1a1a",
+                        "border_width": 1,
+
+                        "bottom_line": "#185fb4",
+                        "bottom_width": 2,
+                    }
+                },
             }
         )
 
     def palette_dark(self):
         self.palette(
             {
-                "text_radius": 6,
-
-                "text_padding": (3, 4),
-
-                "text_frame_back": "#202020",
-                "text_border_width": 1,
-
-                "text_border": "#454545",
-                "text_back": "#353535",
-                "text_text_back": "#cecece",
-                "text_bottom_line": "#ffffff",
-                "text_bottom_width": 0,
-
-                "text_focusin_border": "#454545",
-                "text_focusin_back": "#2f2f2f",
-                "text_focusin_text_back": "#ffffff",
-                "text_focusin_bottom_line": "#4cc2ff",
-                "text_focusin_bottom_width": 2,
+                "text": {
+                    "radius": 6,
+                    "padding": (3, 4),
+
+                    "back": "#353535",
+                    "border": "#454545",
+                    "text_back": "#cecece",
+                    "border_width": 1,
+
+                    "bottom_line": "#ffffff",
+                    "bottom_width": 0,
+
+                    "focusin": {
+                        "back": "#2f2f2f",
+                        "border": "#454545",
+                        "text_back": "#ffffff",
+                        "border_width": 1,
+
+                        "bottom_line": "#4cc2ff",
+                        "bottom_width": 2,
+                    }
+                },
             }
         )
 
     def palette(self, dict=None):
-        if dict is not None:
-            self.text_radius = dict["text_radius"]
-
-            self.text_padding = dict["text_padding"]
-
-            self.text_frame_back = dict["text_frame_back"]
-            self.text_border_width = dict["text_border_width"]
-
-            self.text_border = dict["text_border"]
-            self.text_back = dict["text_back"]
-            self.text_text_back = dict["text_text_back"]
-            self.text_bottom_line = dict["text_bottom_line"]
-            self.text_bottom_width = dict["text_bottom_width"]
-
-            self.text_focusin_border = dict["text_focusin_border"]
-            self.text_focusin_back = dict["text_focusin_back"]
-            self.text_focusin_text_back = dict["text_focusin_text_back"]
-            self.text_focusin_bottom_line = dict["text_focusin_bottom_line"]
-            self.text_focusin_bottom_width = dict["text_focusin_bottom_width"]
-
-            try:
-                self._draw(None)
-            except AttributeError:
-                pass
-        else:
-            return {
-                "text_padding": self.text_padding,
-
-                "text_frame_back": self.text_frame_back,
-                "text_border_width": self.text_border_width,
-                "text_bottom_width": self.text_bottom_width,
-
-                "text_border": self.text_border,
-                "text_back": self.text_back,
-                "text_text_back": self.text_text_back,
-
-                "text_focusin_border": self.text_focusin_border,
-                "text_focusin_back": self.text_focusin_back,
-                "text_focusin_text_back": self.text_focusin_text_back,
-            }
+        super().palette(dict)
+        if "text" in dict:
+            self.text_radius = dict["text"]["radius"]
 
 
 class AdwDrawRoundText(AdwDrawBasicRoundText):
     def default_palette(self):
         self.palette_light()
 
 
@@ -453,15 +425,15 @@
 class AdwDrawBasicRoundText3(AdwDrawBasicText):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def _other(self):
         self.configure(background=self.master.cget("bg"), borderwidth=0)
 
-    def border_radius(self, radius: float | int = None):
+    def border_radius(self, radius=None):
         if radius is None:
             return self.button_radius
         else:
             self.button_radius = radius
 
     def _draw(self, evt):
         self.delete("all")
```

### Comparing `tkadw-0.1.5/tkadw/canvas/titlebar.py` & `tkadw-0.2.0/tkadw/canvas/titlebar.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc`

 * *Files 25% similar despite different names*

#### Python bytecode

```diff
@@ -1,70 +1,81 @@
 magic:    0xa70d0d0a
-moddate:  0x464d9564 (Fri Jun 23 07:44:06 2023 UTC)
-files sz: 283
+moddate:  0x56859564 (Fri Jun 23 11:43:18 2023 UTC)
+files sz: 341
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
-      055a056d065a066d075a070100640064036c086d095a096d0a5a0a010064
-      0064046c0b6d0c5a0c6d0d5a0d010064055300
+      055a050100640064036c066d075a076d085a086d095a096d0a5a0a010064
+      0064046c0b6d0c5a0c6d0d5a0d0100640064056c0e6d0f5a0f6d105a1001
+      0064065300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('GTkFrame', 'GTkDarkFrame'))
                  6 IMPORT_NAME              0 (tkadw.tkite.gtk.frame)
                  8 IMPORT_FROM              1 (GTkFrame)
                 10 STORE_NAME               1 (GTkFrame)
                 12 IMPORT_FROM              2 (GTkDarkFrame)
                 14 STORE_NAME               2 (GTkDarkFrame)
                 16 POP_TOP
    
      2          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               2 (('GTkButton', 'GTkDarkButton', 'GTkSuggestedButton', 'GTkDestructiveButton'))
-                22 IMPORT_NAME              3 (tkadw.tkite.gtk.button)
-                24 IMPORT_FROM              4 (GTkButton)
-                26 STORE_NAME               4 (GTkButton)
-                28 IMPORT_FROM              5 (GTkDarkButton)
-                30 STORE_NAME               5 (GTkDarkButton)
-                32 IMPORT_FROM              6 (GTkSuggestedButton)
-                34 STORE_NAME               6 (GTkSuggestedButton)
-                36 IMPORT_FROM              7 (GTkDestructiveButton)
-                38 STORE_NAME               7 (GTkDestructiveButton)
-                40 POP_TOP
+                20 LOAD_CONST               2 (('GTkLabel', 'GTkDarkLabel'))
+                22 IMPORT_NAME              3 (tkadw.tkite.gtk.label)
+                24 IMPORT_FROM              4 (GTkLabel)
+                26 STORE_NAME               4 (GTkLabel)
+                28 IMPORT_FROM              5 (GTkDarkLabel)
+                30 STORE_NAME               5 (GTkDarkLabel)
+                32 POP_TOP
    
-     3          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               3 (('GTkEntry', 'GTkDarkEntry'))
-                46 IMPORT_NAME              8 (tkadw.tkite.gtk.entry)
-                48 IMPORT_FROM              9 (GTkEntry)
-                50 STORE_NAME               9 (GTkEntry)
-                52 IMPORT_FROM             10 (GTkDarkEntry)
-                54 STORE_NAME              10 (GTkDarkEntry)
+     3          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               3 (('GTkButton', 'GTkDarkButton', 'GTkSuggestedButton', 'GTkDestructiveButton'))
+                38 IMPORT_NAME              6 (tkadw.tkite.gtk.button)
+                40 IMPORT_FROM              7 (GTkButton)
+                42 STORE_NAME               7 (GTkButton)
+                44 IMPORT_FROM              8 (GTkDarkButton)
+                46 STORE_NAME               8 (GTkDarkButton)
+                48 IMPORT_FROM              9 (GTkSuggestedButton)
+                50 STORE_NAME               9 (GTkSuggestedButton)
+                52 IMPORT_FROM             10 (GTkDestructiveButton)
+                54 STORE_NAME              10 (GTkDestructiveButton)
                 56 POP_TOP
    
      4          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               4 (('GTkTextBox', 'GTkDarkTextBox'))
-                62 IMPORT_NAME             11 (tkadw.tkite.gtk.textbox)
-                64 IMPORT_FROM             12 (GTkTextBox)
-                66 STORE_NAME              12 (GTkTextBox)
-                68 IMPORT_FROM             13 (GTkDarkTextBox)
-                70 STORE_NAME              13 (GTkDarkTextBox)
+                60 LOAD_CONST               4 (('GTkEntry', 'GTkDarkEntry'))
+                62 IMPORT_NAME             11 (tkadw.tkite.gtk.entry)
+                64 IMPORT_FROM             12 (GTkEntry)
+                66 STORE_NAME              12 (GTkEntry)
+                68 IMPORT_FROM             13 (GTkDarkEntry)
+                70 STORE_NAME              13 (GTkDarkEntry)
                 72 POP_TOP
-                74 LOAD_CONST               5 (None)
-                76 RETURN_VALUE
+   
+     5          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               5 (('GTkTextBox', 'GTkDarkTextBox'))
+                78 IMPORT_NAME             14 (tkadw.tkite.gtk.textbox)
+                80 IMPORT_FROM             15 (GTkTextBox)
+                82 STORE_NAME              15 (GTkTextBox)
+                84 IMPORT_FROM             16 (GTkDarkTextBox)
+                86 STORE_NAME              16 (GTkDarkTextBox)
+                88 POP_TOP
+                90 LOAD_CONST               6 (None)
+                92 RETURN_VALUE
    consts
       0
       ('GTkFrame', 'GTkDarkFrame')
+      ('GTkLabel', 'GTkDarkLabel')
       ('GTkButton', 'GTkDarkButton', 'GTkSuggestedButton', 'GTkDestructiveButton')
       ('GTkEntry', 'GTkDarkEntry')
       ('GTkTextBox', 'GTkDarkTextBox')
       None
-   names      ('tkadw.tkite.gtk.frame', 'GTkFrame', 'GTkDarkFrame', 'tkadw.tkite.gtk.button', 'GTkButton', 'GTkDarkButton', 'GTkSuggestedButton', 'GTkDestructiveButton', 'tkadw.tkite.gtk.entry', 'GTkEntry', 'GTkDarkEntry', 'tkadw.tkite.gtk.textbox', 'GTkTextBox', 'GTkDarkTextBox')
+   names      ('tkadw.tkite.gtk.frame', 'GTkFrame', 'GTkDarkFrame', 'tkadw.tkite.gtk.label', 'GTkLabel', 'GTkDarkLabel', 'tkadw.tkite.gtk.button', 'GTkButton', 'GTkDarkButton', 'GTkSuggestedButton', 'GTkDestructiveButton', 'tkadw.tkite.gtk.entry', 'GTkEntry', 'GTkDarkEntry', 'tkadw.tkite.gtk.textbox', 'GTkTextBox', 'GTkDarkTextBox')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201100118011001
+   lnotab 0x00ff02011001100118011001
```

### Comparing `tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc` & `tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc`

 * *Files 23% similar despite different names*

#### Python bytecode

```diff
@@ -1,36 +1,41 @@
 magic:    0xa70d0d0a
-moddate:  0x1b599564 (Fri Jun 23 08:34:35 2023 UTC)
-files sz: 3726
+moddate:  0xde469664 (Sat Jun 24 01:29:02 2023 UTC)
+files sz: 4735
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100020047006402840064036501a60300
       00ab0300000000000000005a02020047006404840064056502a6030000ab
       0300000000000000005a03020047006406840064076502a6030000ab0300
       000000000000005a04020047006408840064096502a6030000ab03000000
-      00000000005a056506640a6b020000000072e06400640b6c076d085a0801
-      006400640c6c006d095a096d0a5a0a010002006508a6000000ab00000000
-      00000000005a0b650ba00c00000000000000000000000000000000000000
-      00640dac0ea6010000ab010000000000000000010002006509650ba60100
-      00ab0100000000000000005a0d02006502650d6a0d000000000000000064
-      03ac0fa6020000ab0200000000000000005a0e650ea00f00000000000000
-      000000000000000000000000006410641164116411ac12a6040000ab0400
-      000000000000000100650da00f0000000000000000000000000000000000
-      000000641364146415ac16a6030000ab0300000000000000000100020065
-      0a650ba6010000ab0100000000000000005a100200650365106a0d000000
-      00000000006405ac0fa6020000ab0200000000000000005a116511a00f00
-      000000000000000000000000000000000000006410641164116411ac12a6
-      040000ab04000000000000000001006510a00f0000000000000000000000
-      000000000000000000641364146417ac16a6030000ab0300000000000000
-      000100650ba0120000000000000000000000000000000000000000a60000
-      00ab00000000000000000001006418530064185300
+      00000000005a056506640a6b0200000000900172206400640b6c076d085a
+      0801006400640c6c006d095a096d0a5a0a010002006508a6000000ab0000
+      000000000000005a0b02006509650ba6010000ab0100000000000000005a
+      0c02006502650c6a0c00000000000000006403ac0da6020000ab02000000
+      00000000005a0d650da00e00000000000000000000000000000000000000
+      00640e640f640f640fac10a6040000ab0400000000000000000100020065
+      05650c6a0c00000000000000006409ac0da6020000ab0200000000000000
+      005a0f650fa00e0000000000000000000000000000000000000000640e64
+      0f640f640fac10a6040000ab0400000000000000000100650ca00e000000
+      0000000000000000000000000000000000641164126413ac14a6030000ab
+      03000000000000000001000200650a650ba6010000ab0100000000000000
+      005a100200650365106a0c00000000000000006405ac0da6020000ab0200
+      000000000000005a116511a00e0000000000000000000000000000000000
+      000000640e640f640f640fac10a6040000ab040000000000000000010002
+      00650465106a0c00000000000000006407ac0da6020000ab020000000000
+      0000005a126512a00e000000000000000000000000000000000000000064
+      0e640f640f640fac10a6040000ab04000000000000000001006510a00e00
+      00000000000000000000000000000000000000641164126415ac14a60300
+      00ab0300000000000000000100650ba01300000000000000000000000000
+      00000000000000a6000000ab000000000000000000010064165300641653
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('AdwDrawRoundButton3',))
                  6 IMPORT_NAME              0 (tkadw)
                  8 IMPORT_FROM              1 (AdwDrawRoundButton3)
                 10 STORE_NAME               1 (AdwDrawRoundButton3)
@@ -42,165 +47,200 @@
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               3 ('GTkButton')
                 24 LOAD_NAME                1 (AdwDrawRoundButton3)
                 26 PRECALL                  3
                 30 CALL                     3
                 40 STORE_NAME               2 (GTkButton)
    
-    96          42 PUSH_NULL
+   120          42 PUSH_NULL
                 44 LOAD_BUILD_CLASS
-                46 LOAD_CONST               4 (<code object GTkDarkButton, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 96>)
+                46 LOAD_CONST               4 (<code object GTkDarkButton, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 120>)
                 48 MAKE_FUNCTION            0
                 50 LOAD_CONST               5 ('GTkDarkButton')
                 52 LOAD_NAME                2 (GTkButton)
                 54 PRECALL                  3
                 58 CALL                     3
                 68 STORE_NAME               3 (GTkDarkButton)
    
-   101          70 PUSH_NULL
+   125          70 PUSH_NULL
                 72 LOAD_BUILD_CLASS
-                74 LOAD_CONST               6 (<code object GTkDestructiveButton, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 101>)
+                74 LOAD_CONST               6 (<code object GTkDestructiveButton, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 125>)
                 76 MAKE_FUNCTION            0
                 78 LOAD_CONST               7 ('GTkDestructiveButton')
                 80 LOAD_NAME                2 (GTkButton)
                 82 PRECALL                  3
                 86 CALL                     3
                 96 STORE_NAME               4 (GTkDestructiveButton)
    
-   106          98 PUSH_NULL
+   130          98 PUSH_NULL
                100 LOAD_BUILD_CLASS
-               102 LOAD_CONST               8 (<code object GTkSuggestedButton, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 106>)
+               102 LOAD_CONST               8 (<code object GTkSuggestedButton, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 130>)
                104 MAKE_FUNCTION            0
                106 LOAD_CONST               9 ('GTkSuggestedButton')
                108 LOAD_NAME                2 (GTkButton)
                110 PRECALL                  3
                114 CALL                     3
                124 STORE_NAME               5 (GTkSuggestedButton)
    
-   111         126 LOAD_NAME                6 (__name__)
+   135         126 LOAD_NAME                6 (__name__)
                128 LOAD_CONST              10 ('__main__')
                130 COMPARE_OP               2 (==)
-               136 POP_JUMP_FORWARD_IF_FALSE   224 (to 586)
+               136 EXTENDED_ARG             1
+               138 POP_JUMP_FORWARD_IF_FALSE   288 (to 716)
    
-   112         138 LOAD_CONST               0 (0)
-               140 LOAD_CONST              11 (('Tk',))
-               142 IMPORT_NAME              7 (tkinter)
-               144 IMPORT_FROM              8 (Tk)
-               146 STORE_NAME               8 (Tk)
-               148 POP_TOP
-   
-   113         150 LOAD_CONST               0 (0)
-               152 LOAD_CONST              12 (('GTkFrame', 'GTkDarkFrame'))
-               154 IMPORT_NAME              0 (tkadw)
-               156 IMPORT_FROM              9 (GTkFrame)
-               158 STORE_NAME               9 (GTkFrame)
-               160 IMPORT_FROM             10 (GTkDarkFrame)
-               162 STORE_NAME              10 (GTkDarkFrame)
-               164 POP_TOP
-   
-   115         166 PUSH_NULL
-               168 LOAD_NAME                8 (Tk)
-               170 PRECALL                  0
-               174 CALL                     0
-               184 STORE_NAME              11 (root)
-   
-   116         186 LOAD_NAME               11 (root)
-               188 LOAD_METHOD             12 (configure)
-               210 LOAD_CONST              13 ('#1e1e1e')
-               212 KW_NAMES                14
-               214 PRECALL                  1
-               218 CALL                     1
-               228 POP_TOP
-   
-   118         230 PUSH_NULL
-               232 LOAD_NAME                9 (GTkFrame)
-               234 LOAD_NAME               11 (root)
-               236 PRECALL                  1
-               240 CALL                     1
-               250 STORE_NAME              13 (frame)
-   
-   120         252 PUSH_NULL
-               254 LOAD_NAME                2 (GTkButton)
-               256 LOAD_NAME               13 (frame)
-               258 LOAD_ATTR               13 (frame)
-               268 LOAD_CONST               3 ('GTkButton')
-               270 KW_NAMES                15
-               272 PRECALL                  2
-               276 CALL                     2
-               286 STORE_NAME              14 (button1)
-   
-   121         288 LOAD_NAME               14 (button1)
-               290 LOAD_METHOD             15 (pack)
-               312 LOAD_CONST              16 ('x')
-               314 LOAD_CONST              17 (5)
-               316 LOAD_CONST              17 (5)
-               318 LOAD_CONST              17 (5)
-               320 KW_NAMES                18
-               322 PRECALL                  4
-               326 CALL                     4
-               336 POP_TOP
-   
-   123         338 LOAD_NAME               13 (frame)
-               340 LOAD_METHOD             15 (pack)
-               362 LOAD_CONST              19 ('both')
-               364 LOAD_CONST              20 ('yes')
-               366 LOAD_CONST              21 ('right')
-               368 KW_NAMES                22
-               370 PRECALL                  3
-               374 CALL                     3
-               384 POP_TOP
-   
-   125         386 PUSH_NULL
-               388 LOAD_NAME               10 (GTkDarkFrame)
-               390 LOAD_NAME               11 (root)
-               392 PRECALL                  1
-               396 CALL                     1
-               406 STORE_NAME              16 (frame2)
-   
-   127         408 PUSH_NULL
-               410 LOAD_NAME                3 (GTkDarkButton)
-               412 LOAD_NAME               16 (frame2)
-               414 LOAD_ATTR               13 (frame)
-               424 LOAD_CONST               5 ('GTkDarkButton')
-               426 KW_NAMES                15
-               428 PRECALL                  2
-               432 CALL                     2
-               442 STORE_NAME              17 (button2)
-   
-   128         444 LOAD_NAME               17 (button2)
-               446 LOAD_METHOD             15 (pack)
-               468 LOAD_CONST              16 ('x')
-               470 LOAD_CONST              17 (5)
-               472 LOAD_CONST              17 (5)
-               474 LOAD_CONST              17 (5)
-               476 KW_NAMES                18
-               478 PRECALL                  4
-               482 CALL                     4
-               492 POP_TOP
-   
-   130         494 LOAD_NAME               16 (frame2)
-               496 LOAD_METHOD             15 (pack)
-               518 LOAD_CONST              19 ('both')
-               520 LOAD_CONST              20 ('yes')
-               522 LOAD_CONST              23 ('left')
-               524 KW_NAMES                22
-               526 PRECALL                  3
-               530 CALL                     3
-               540 POP_TOP
-   
-   132         542 LOAD_NAME               11 (root)
-               544 LOAD_METHOD             18 (mainloop)
-               566 PRECALL                  0
-               570 CALL                     0
-               580 POP_TOP
-               582 LOAD_CONST              24 (None)
-               584 RETURN_VALUE
+   136         140 LOAD_CONST               0 (0)
+               142 LOAD_CONST              11 (('Tk',))
+               144 IMPORT_NAME              7 (tkinter)
+               146 IMPORT_FROM              8 (Tk)
+               148 STORE_NAME               8 (Tk)
+               150 POP_TOP
+   
+   137         152 LOAD_CONST               0 (0)
+               154 LOAD_CONST              12 (('GTkFrame', 'GTkDarkFrame'))
+               156 IMPORT_NAME              0 (tkadw)
+               158 IMPORT_FROM              9 (GTkFrame)
+               160 STORE_NAME               9 (GTkFrame)
+               162 IMPORT_FROM             10 (GTkDarkFrame)
+               164 STORE_NAME              10 (GTkDarkFrame)
+               166 POP_TOP
+   
+   139         168 PUSH_NULL
+               170 LOAD_NAME                8 (Tk)
+               172 PRECALL                  0
+               176 CALL                     0
+               186 STORE_NAME              11 (root)
+   
+   141         188 PUSH_NULL
+               190 LOAD_NAME                9 (GTkFrame)
+               192 LOAD_NAME               11 (root)
+               194 PRECALL                  1
+               198 CALL                     1
+               208 STORE_NAME              12 (frame)
+   
+   143         210 PUSH_NULL
+               212 LOAD_NAME                2 (GTkButton)
+               214 LOAD_NAME               12 (frame)
+               216 LOAD_ATTR               12 (frame)
+               226 LOAD_CONST               3 ('GTkButton')
+               228 KW_NAMES                13
+               230 PRECALL                  2
+               234 CALL                     2
+               244 STORE_NAME              13 (button1)
+   
+   144         246 LOAD_NAME               13 (button1)
+               248 LOAD_METHOD             14 (pack)
+               270 LOAD_CONST              14 ('x')
+               272 LOAD_CONST              15 (5)
+               274 LOAD_CONST              15 (5)
+               276 LOAD_CONST              15 (5)
+               278 KW_NAMES                16
+               280 PRECALL                  4
+               284 CALL                     4
+               294 POP_TOP
+   
+   146         296 PUSH_NULL
+               298 LOAD_NAME                5 (GTkSuggestedButton)
+               300 LOAD_NAME               12 (frame)
+               302 LOAD_ATTR               12 (frame)
+               312 LOAD_CONST               9 ('GTkSuggestedButton')
+               314 KW_NAMES                13
+               316 PRECALL                  2
+               320 CALL                     2
+               330 STORE_NAME              15 (button3)
+   
+   147         332 LOAD_NAME               15 (button3)
+               334 LOAD_METHOD             14 (pack)
+               356 LOAD_CONST              14 ('x')
+               358 LOAD_CONST              15 (5)
+               360 LOAD_CONST              15 (5)
+               362 LOAD_CONST              15 (5)
+               364 KW_NAMES                16
+               366 PRECALL                  4
+               370 CALL                     4
+               380 POP_TOP
+   
+   149         382 LOAD_NAME               12 (frame)
+               384 LOAD_METHOD             14 (pack)
+               406 LOAD_CONST              17 ('both')
+               408 LOAD_CONST              18 ('yes')
+               410 LOAD_CONST              19 ('right')
+               412 KW_NAMES                20
+               414 PRECALL                  3
+               418 CALL                     3
+               428 POP_TOP
+   
+   151         430 PUSH_NULL
+               432 LOAD_NAME               10 (GTkDarkFrame)
+               434 LOAD_NAME               11 (root)
+               436 PRECALL                  1
+               440 CALL                     1
+               450 STORE_NAME              16 (frame2)
+   
+   153         452 PUSH_NULL
+               454 LOAD_NAME                3 (GTkDarkButton)
+               456 LOAD_NAME               16 (frame2)
+               458 LOAD_ATTR               12 (frame)
+               468 LOAD_CONST               5 ('GTkDarkButton')
+               470 KW_NAMES                13
+               472 PRECALL                  2
+               476 CALL                     2
+               486 STORE_NAME              17 (button2)
+   
+   154         488 LOAD_NAME               17 (button2)
+               490 LOAD_METHOD             14 (pack)
+               512 LOAD_CONST              14 ('x')
+               514 LOAD_CONST              15 (5)
+               516 LOAD_CONST              15 (5)
+               518 LOAD_CONST              15 (5)
+               520 KW_NAMES                16
+               522 PRECALL                  4
+               526 CALL                     4
+               536 POP_TOP
+   
+   156         538 PUSH_NULL
+               540 LOAD_NAME                4 (GTkDestructiveButton)
+               542 LOAD_NAME               16 (frame2)
+               544 LOAD_ATTR               12 (frame)
+               554 LOAD_CONST               7 ('GTkDestructiveButton')
+               556 KW_NAMES                13
+               558 PRECALL                  2
+               562 CALL                     2
+               572 STORE_NAME              18 (button4)
+   
+   157         574 LOAD_NAME               18 (button4)
+               576 LOAD_METHOD             14 (pack)
+               598 LOAD_CONST              14 ('x')
+               600 LOAD_CONST              15 (5)
+               602 LOAD_CONST              15 (5)
+               604 LOAD_CONST              15 (5)
+               606 KW_NAMES                16
+               608 PRECALL                  4
+               612 CALL                     4
+               622 POP_TOP
+   
+   159         624 LOAD_NAME               16 (frame2)
+               626 LOAD_METHOD             14 (pack)
+               648 LOAD_CONST              17 ('both')
+               650 LOAD_CONST              18 ('yes')
+               652 LOAD_CONST              21 ('left')
+               654 KW_NAMES                20
+               656 PRECALL                  3
+               660 CALL                     3
+               670 POP_TOP
+   
+   161         672 LOAD_NAME               11 (root)
+               674 LOAD_METHOD             19 (mainloop)
+               696 PRECALL                  0
+               700 CALL                     0
+               710 POP_TOP
+               712 LOAD_CONST              22 (None)
+               714 RETURN_VALUE
    
-   111     >>  586 LOAD_CONST              24 (None)
-               588 RETURN_VALUE
+   135     >>  716 LOAD_CONST              22 (None)
+               718 RETURN_VALUE
    consts
       0
       ('AdwDrawRoundButton3',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
@@ -227,23 +267,23 @@
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (default_palette)
          
           11          28 LOAD_CONST               3 (<code object palette_gtk_light, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 11>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               5 (palette_gtk_light)
          
-          32          34 LOAD_CONST               4 (<code object palette_gtk_dark, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 32>)
+          38          34 LOAD_CONST               4 (<code object palette_gtk_dark, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 38>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               6 (palette_gtk_dark)
          
-          53          40 LOAD_CONST               5 (<code object palette_gtk_red, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 53>)
+          65          40 LOAD_CONST               5 (<code object palette_gtk_red, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 65>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               7 (palette_gtk_red)
          
-          74          46 LOAD_CONST               6 (<code object palette_gtk_blue, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 74>)
+          92          46 LOAD_CONST               6 (<code object palette_gtk_blue, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 92>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (palette_gtk_blue)
                       52 LOAD_CLOSURE             0 (__class__)
                       54 COPY                     1
                       56 STORE_NAME               9 (__classcell__)
                       58 RETURN_VALUE
          consts
@@ -313,453 +353,523 @@
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564066407640564066406640564089c0ba6010000ab0100
-                  00000000000000010064005300
+                  026403640464056406640764086405640664099c04640864086405640664
+                  099c04640a9c076901a6010000ab010000000000000000010064005300
                 11           0 RESUME                   0
                
                 12           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                14          26 LOAD_CONST               1 (11)
+                14          26 LOAD_CONST               1 ('button')
                
-                16          28 LOAD_CONST               2 (1.3)
+                15          28 LOAD_CONST               2 (11)
                
-                18          30 LOAD_CONST               3 ('#ccc6c1')
+                16          30 LOAD_CONST               3 ('#f6f5f4')
                
-                19          32 LOAD_CONST               4 ('#f6f5f4')
+                17          32 LOAD_CONST               4 ('#ccc6c1')
                
-                20          34 LOAD_CONST               5 ('#2e3436')
+                18          34 LOAD_CONST               5 ('#2e3436')
                
-                22          36 LOAD_CONST               6 ('#dad6d2')
+                19          36 LOAD_CONST               6 (1.3)
                
-                23          38 LOAD_CONST               7 ('#f8f8f7')
+                22          38 LOAD_CONST               7 ('#f8f8f7')
                
-                24          40 LOAD_CONST               5 ('#2e3436')
+                23          40 LOAD_CONST               8 ('#dad6d2')
                
-                26          42 LOAD_CONST               6 ('#dad6d2')
+                24          42 LOAD_CONST               5 ('#2e3436')
                
-                27          44 LOAD_CONST               6 ('#dad6d2')
+                25          44 LOAD_CONST               6 (1.3)
                
-                28          46 LOAD_CONST               5 ('#2e3436')
+                21          46 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+                            48 BUILD_CONST_KEY_MAP      4
                
-                13          48 LOAD_CONST               8 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+                29          50 LOAD_CONST               8 ('#dad6d2')
                
-                12          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+                30          52 LOAD_CONST               8 ('#dad6d2')
+               
+                31          54 LOAD_CONST               5 ('#2e3436')
+               
+                32          56 LOAD_CONST               6 (1.3)
+               
+                28          58 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+                            60 BUILD_CONST_KEY_MAP      4
+               
+                14          62 LOAD_CONST              10 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            64 BUILD_CONST_KEY_MAP      7
+               
+                13          66 BUILD_MAP                1
+               
+                12          68 PRECALL                  1
+                            72 CALL                     1
+                            82 POP_TOP
+                            84 LOAD_CONST               0 (None)
+                            86 RETURN_VALUE
                consts
                   None
+                  'button'
                   11
-                  1.3
-                  '#ccc6c1'
                   '#f6f5f4'
+                  '#ccc6c1'
                   '#2e3436'
-                  '#dad6d2'
+                  1.3
                   '#f8f8f7'
-                  ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  '#dad6d2'
+                  ('back', 'border', 'text_back', 'border_width')
+                  ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
                name       'palette_gtk_light'
                firstlineno 11
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               lnotab
+                  0x0201180202010201020102010201020302010201020102fc0408020102
+                  01020102fc04f204ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564036406640564076408640564099c0ba6010000ab0100
-                  00000000000000010064005300
-                32           0 RESUME                   0
+                  026403640464056406640764046405640664089c046409640a6405640664
+                  089c04640b9c076901a6010000ab010000000000000000010064005300
+                38           0 RESUME                   0
                
-                33           2 LOAD_FAST                0 (self)
+                39           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                35          26 LOAD_CONST               1 (11)
+                41          26 LOAD_CONST               1 ('button')
                
-                37          28 LOAD_CONST               2 (1.3)
+                42          28 LOAD_CONST               2 (11)
                
-                39          30 LOAD_CONST               3 ('#1b1b1b')
+                43          30 LOAD_CONST               3 ('#353535')
                
-                40          32 LOAD_CONST               4 ('#353535')
+                44          32 LOAD_CONST               4 ('#1b1b1b')
                
-                41          34 LOAD_CONST               5 ('#eeeeec')
+                45          34 LOAD_CONST               5 ('#eeeeec')
                
-                43          36 LOAD_CONST               3 ('#1b1b1b')
+                46          36 LOAD_CONST               6 (1.3)
                
-                44          38 LOAD_CONST               6 ('#373737')
+                49          38 LOAD_CONST               7 ('#373737')
                
-                45          40 LOAD_CONST               5 ('#eeeeec')
+                50          40 LOAD_CONST               4 ('#1b1b1b')
                
-                47          42 LOAD_CONST               7 ('#282828')
+                51          42 LOAD_CONST               5 ('#eeeeec')
                
-                48          44 LOAD_CONST               8 ('#1e1e1e')
+                52          44 LOAD_CONST               6 (1.3)
                
-                49          46 LOAD_CONST               5 ('#eeeeec')
+                48          46 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+                            48 BUILD_CONST_KEY_MAP      4
                
-                34          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+                56          50 LOAD_CONST               9 ('#1e1e1e')
                
-                33          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+                57          52 LOAD_CONST              10 ('#282828')
+               
+                58          54 LOAD_CONST               5 ('#eeeeec')
+               
+                59          56 LOAD_CONST               6 (1.3)
+               
+                55          58 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+                            60 BUILD_CONST_KEY_MAP      4
+               
+                41          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            64 BUILD_CONST_KEY_MAP      7
+               
+                40          66 BUILD_MAP                1
+               
+                39          68 PRECALL                  1
+                            72 CALL                     1
+                            82 POP_TOP
+                            84 LOAD_CONST               0 (None)
+                            86 RETURN_VALUE
                consts
                   None
+                  'button'
                   11
-                  1.3
-                  '#1b1b1b'
                   '#353535'
+                  '#1b1b1b'
                   '#eeeeec'
+                  1.3
                   '#373737'
-                  '#282828'
+                  ('back', 'border', 'text_back', 'border_width')
                   '#1e1e1e'
-                  ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  '#282828'
+                  ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
                name       'palette_gtk_dark'
-               firstlineno 32
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               firstlineno 38
+               lnotab
+                  0x0201180202010201020102010201020302010201020102fc0408020102
+                  01020102fc04f204ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564066407640564066408640564099c0ba6010000ab0100
-                  00000000000000010064005300
-                53           0 RESUME                   0
+                  026403640464056406640764086405640664099c04640a64086405640664
+                  099c04640b9c076901a6010000ab010000000000000000010064005300
+                65           0 RESUME                   0
                
-                54           2 LOAD_FAST                0 (self)
+                66           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                56          26 LOAD_CONST               1 (11)
+                68          26 LOAD_CONST               1 ('button')
                
-                58          28 LOAD_CONST               2 (1.3)
+                69          28 LOAD_CONST               2 (11)
                
-                60          30 LOAD_CONST               3 ('#851015')
+                70          30 LOAD_CONST               3 ('#d81a23')
                
-                61          32 LOAD_CONST               4 ('#d81a23')
+                71          32 LOAD_CONST               4 ('#851015')
                
-                62          34 LOAD_CONST               5 ('#ffffff')
+                72          34 LOAD_CONST               5 ('#ffffff')
                
-                64          36 LOAD_CONST               6 ('#9c1319')
+                73          36 LOAD_CONST               6 (1.3)
                
-                65          38 LOAD_CONST               7 ('#bc171e')
+                76          38 LOAD_CONST               7 ('#bc171e')
                
-                66          40 LOAD_CONST               5 ('#ffffff')
+                77          40 LOAD_CONST               8 ('#9c1319')
                
-                68          42 LOAD_CONST               6 ('#9c1319')
+                78          42 LOAD_CONST               5 ('#ffffff')
                
-                69          44 LOAD_CONST               8 ('#a0131a')
+                79          44 LOAD_CONST               6 (1.3)
                
-                70          46 LOAD_CONST               5 ('#ffffff')
+                75          46 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+                            48 BUILD_CONST_KEY_MAP      4
                
-                55          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+                83          50 LOAD_CONST              10 ('#a0131a')
                
-                54          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+                84          52 LOAD_CONST               8 ('#9c1319')
+               
+                85          54 LOAD_CONST               5 ('#ffffff')
+               
+                86          56 LOAD_CONST               6 (1.3)
+               
+                82          58 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+                            60 BUILD_CONST_KEY_MAP      4
+               
+                68          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            64 BUILD_CONST_KEY_MAP      7
+               
+                67          66 BUILD_MAP                1
+               
+                66          68 PRECALL                  1
+                            72 CALL                     1
+                            82 POP_TOP
+                            84 LOAD_CONST               0 (None)
+                            86 RETURN_VALUE
                consts
                   None
+                  'button'
                   11
-                  1.3
-                  '#851015'
                   '#d81a23'
+                  '#851015'
                   '#ffffff'
-                  '#9c1319'
+                  1.3
                   '#bc171e'
+                  '#9c1319'
+                  ('back', 'border', 'text_back', 'border_width')
                   '#a0131a'
-                  ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
                name       'palette_gtk_red'
-               firstlineno 53
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               firstlineno 65
+               lnotab
+                  0x0201180202010201020102010201020302010201020102fc0408020102
+                  01020102fc04f204ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564066407640564066408640564099c0ba6010000ab0100
-                  00000000000000010064005300
-                74           0 RESUME                   0
+                  026403640464056406640764086405640664099c04640a64086405640664
+                  099c04640b9c076901a6010000ab010000000000000000010064005300
+                92           0 RESUME                   0
                
-                75           2 LOAD_FAST                0 (self)
+                93           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                77          26 LOAD_CONST               1 (11)
+                95          26 LOAD_CONST               1 ('button')
                
-                79          28 LOAD_CONST               2 (1.3)
+                96          28 LOAD_CONST               2 (11)
                
-                81          30 LOAD_CONST               3 ('#15539e')
+                97          30 LOAD_CONST               3 ('#2d7fe3')
                
-                82          32 LOAD_CONST               4 ('#2d7fe3')
+                98          32 LOAD_CONST               4 ('#15539e')
                
-                83          34 LOAD_CONST               5 ('#ffffff')
+                99          34 LOAD_CONST               5 ('#ffffff')
                
-                85          36 LOAD_CONST               6 ('#185fb4')
+               100          36 LOAD_CONST               6 (1.3)
                
-                86          38 LOAD_CONST               7 ('#1a65c2')
+               103          38 LOAD_CONST               7 ('#1a65c2')
                
-                87          40 LOAD_CONST               5 ('#ffffff')
+               104          40 LOAD_CONST               8 ('#185fb4')
                
-                89          42 LOAD_CONST               6 ('#185fb4')
+               105          42 LOAD_CONST               5 ('#ffffff')
                
-                90          44 LOAD_CONST               8 ('#1961b9')
+               106          44 LOAD_CONST               6 (1.3)
                
-                91          46 LOAD_CONST               5 ('#ffffff')
+               102          46 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+                            48 BUILD_CONST_KEY_MAP      4
                
-                76          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
-                            50 BUILD_CONST_KEY_MAP     11
+               110          50 LOAD_CONST              10 ('#1961b9')
                
-                75          52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               111          52 LOAD_CONST               8 ('#185fb4')
+               
+               112          54 LOAD_CONST               5 ('#ffffff')
+               
+               113          56 LOAD_CONST               6 (1.3)
+               
+               109          58 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+                            60 BUILD_CONST_KEY_MAP      4
+               
+                95          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                            64 BUILD_CONST_KEY_MAP      7
+               
+                94          66 BUILD_MAP                1
+               
+                93          68 PRECALL                  1
+                            72 CALL                     1
+                            82 POP_TOP
+                            84 LOAD_CONST               0 (None)
+                            86 RETURN_VALUE
                consts
                   None
+                  'button'
                   11
-                  1.3
-                  '#15539e'
                   '#2d7fe3'
+                  '#15539e'
                   '#ffffff'
-                  '#185fb4'
+                  1.3
                   '#1a65c2'
+                  '#185fb4'
+                  ('back', 'border', 'text_back', 'border_width')
                   '#1961b9'
-                  ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
+                  ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
                name       'palette_gtk_blue'
-               firstlineno 74
-               lnotab 0x02011802020202020201020102020201020102020201020102f104ff
+               firstlineno 92
+               lnotab
+                  0x0201180202010201020102010201020302010201020102fc0408020102
+                  01020102fc04f204ff02ff
          names      ('__name__', '__module__', '__qualname__', '__init__', 'default_palette', 'palette_gtk_light', 'palette_gtk_dark', 'palette_gtk_red', 'palette_gtk_blue', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
          name       'GTkButton'
          firstlineno 4
-         lnotab 0x0c010a030603061506150615
+         lnotab 0x0c010a030603061b061b061b
       'GTkButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          96           0 RESUME                   0
+         120           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GTkDarkButton')
                        8 STORE_NAME               2 (__qualname__)
          
-          97          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 97>)
+         121          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 121>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'GTkDarkButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                97           0 RESUME                   0
+               121           0 RESUME                   0
                
-                98           2 LOAD_FAST                0 (self)
+               122           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_gtk_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_gtk_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
                name       'default_palette'
-               firstlineno 97
+               firstlineno 121
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
          name       'GTkDarkButton'
-         firstlineno 96
+         firstlineno 120
          lnotab 0x0a01
       'GTkDarkButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         101           0 RESUME                   0
+         125           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GTkDestructiveButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         102          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 102>)
+         126          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 126>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'GTkDestructiveButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               102           0 RESUME                   0
+               126           0 RESUME                   0
                
-               103           2 LOAD_FAST                0 (self)
+               127           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_gtk_red)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_gtk_red',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
                name       'default_palette'
-               firstlineno 102
+               firstlineno 126
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
          name       'GTkDestructiveButton'
-         firstlineno 101
+         firstlineno 125
          lnotab 0x0a01
       'GTkDestructiveButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         106           0 RESUME                   0
+         130           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GTkSuggestedButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         107          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 107>)
+         131          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 131>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'GTkSuggestedButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               107           0 RESUME                   0
+               131           0 RESUME                   0
                
-               108           2 LOAD_FAST                0 (self)
+               132           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_gtk_blue)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_gtk_blue',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
                name       'default_palette'
-               firstlineno 107
+               firstlineno 131
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
          name       'GTkSuggestedButton'
-         firstlineno 106
+         firstlineno 130
          lnotab 0x0a01
       'GTkSuggestedButton'
       '__main__'
       ('Tk',)
       ('GTkFrame', 'GTkDarkFrame')
-      '#1e1e1e'
-      ('background',)
       ('text',)
       'x'
       5
       ('fill', 'ipadx', 'padx', 'pady')
       'both'
       'yes'
       'right'
       ('fill', 'expand', 'side')
       'left'
       None
-   names      ('tkadw', 'AdwDrawRoundButton3', 'GTkButton', 'GTkDarkButton', 'GTkDestructiveButton', 'GTkSuggestedButton', '__name__', 'tkinter', 'Tk', 'GTkFrame', 'GTkDarkFrame', 'root', 'configure', 'frame', 'button1', 'pack', 'frame2', 'button2', 'mainloop')
+   names      ('tkadw', 'AdwDrawRoundButton3', 'GTkButton', 'GTkDarkButton', 'GTkDestructiveButton', 'GTkSuggestedButton', '__name__', 'tkinter', 'Tk', 'GTkFrame', 'GTkDarkFrame', 'root', 'frame', 'button1', 'pack', 'button3', 'frame2', 'button2', 'button4', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c031c5c1c051c051c050c010c01100214012c021602240132
-      02300216022401320230022ceb
+      0x00ff02010c031c741c051c051c050e010c011002140216022401320224
+      01320230021602240132022401320230022ce6
```

### Comparing `tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc` & `tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x425a9564 (Fri Jun 23 08:39:30 2023 UTC)
-files sz: 2441
+moddate:  0x964a9664 (Sat Jun 24 01:44:54 2023 UTC)
+files sz: 2551
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100020047006402840064036501a60300
@@ -40,144 +40,144 @@
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               3 ('GTkEntry')
                 24 LOAD_NAME                1 (AdwDrawRoundEntry3)
                 26 PRECALL                  3
                 30 CALL                     3
                 40 STORE_NAME               2 (GTkEntry)
    
-    60          42 PUSH_NULL
+    68          42 PUSH_NULL
                 44 LOAD_BUILD_CLASS
-                46 LOAD_CONST               4 (<code object GTkDarkEntry, file "D:\tkadw\tkadw\tkite\gtk\entry.py", line 60>)
+                46 LOAD_CONST               4 (<code object GTkDarkEntry, file "D:\tkadw\tkadw\tkite\gtk\entry.py", line 68>)
                 48 MAKE_FUNCTION            0
                 50 LOAD_CONST               5 ('GTkDarkEntry')
                 52 LOAD_NAME                2 (GTkEntry)
                 54 PRECALL                  3
                 58 CALL                     3
                 68 STORE_NAME               3 (GTkDarkEntry)
    
-    65          70 LOAD_NAME                4 (__name__)
+    73          70 LOAD_NAME                4 (__name__)
                 72 LOAD_CONST               6 ('__main__')
                 74 COMPARE_OP               2 (==)
                 80 POP_JUMP_FORWARD_IF_FALSE   224 (to 530)
    
-    66          82 LOAD_CONST               0 (0)
+    74          82 LOAD_CONST               0 (0)
                 84 LOAD_CONST               7 (('Tk',))
                 86 IMPORT_NAME              5 (tkinter)
                 88 IMPORT_FROM              6 (Tk)
                 90 STORE_NAME               6 (Tk)
                 92 POP_TOP
    
-    67          94 LOAD_CONST               0 (0)
+    75          94 LOAD_CONST               0 (0)
                 96 LOAD_CONST               8 (('GTkFrame', 'GTkDarkFrame', 'GTkEntry', 'GTkDarkEntry'))
                 98 IMPORT_NAME              0 (tkadw)
                100 IMPORT_FROM              7 (GTkFrame)
                102 STORE_NAME               7 (GTkFrame)
                104 IMPORT_FROM              8 (GTkDarkFrame)
                106 STORE_NAME               8 (GTkDarkFrame)
                108 IMPORT_FROM              2 (GTkEntry)
                110 STORE_NAME               2 (GTkEntry)
                112 IMPORT_FROM              3 (GTkDarkEntry)
                114 STORE_NAME               3 (GTkDarkEntry)
                116 POP_TOP
    
-    69         118 PUSH_NULL
+    77         118 PUSH_NULL
                120 LOAD_NAME                6 (Tk)
                122 PRECALL                  0
                126 CALL                     0
                136 STORE_NAME               9 (root)
    
-    70         138 LOAD_NAME                9 (root)
+    78         138 LOAD_NAME                9 (root)
                140 LOAD_METHOD             10 (configure)
                162 LOAD_CONST               9 ('#1f1f1f')
                164 KW_NAMES                10
                166 PRECALL                  1
                170 CALL                     1
                180 POP_TOP
    
-    72         182 PUSH_NULL
+    80         182 PUSH_NULL
                184 LOAD_NAME                7 (GTkFrame)
                186 LOAD_NAME                9 (root)
                188 PRECALL                  1
                192 CALL                     1
                202 STORE_NAME              11 (frame)
    
-    74         204 PUSH_NULL
+    82         204 PUSH_NULL
                206 LOAD_NAME                2 (GTkEntry)
                208 LOAD_NAME               11 (frame)
                210 LOAD_ATTR               11 (frame)
                220 PRECALL                  1
                224 CALL                     1
                234 STORE_NAME              12 (entry1)
    
-    75         236 LOAD_NAME               12 (entry1)
+    83         236 LOAD_NAME               12 (entry1)
                238 LOAD_METHOD             13 (pack)
                260 LOAD_CONST              11 ('x')
                262 LOAD_CONST              12 (5)
                264 LOAD_CONST              12 (5)
                266 LOAD_CONST              12 (5)
                268 KW_NAMES                13
                270 PRECALL                  4
                274 CALL                     4
                284 POP_TOP
    
-    77         286 LOAD_NAME               11 (frame)
+    85         286 LOAD_NAME               11 (frame)
                288 LOAD_METHOD             13 (pack)
                310 LOAD_CONST              14 ('both')
                312 LOAD_CONST              15 ('yes')
                314 LOAD_CONST              16 ('right')
                316 KW_NAMES                17
                318 PRECALL                  3
                322 CALL                     3
                332 POP_TOP
    
-    79         334 PUSH_NULL
+    87         334 PUSH_NULL
                336 LOAD_NAME                8 (GTkDarkFrame)
                338 LOAD_NAME                9 (root)
                340 PRECALL                  1
                344 CALL                     1
                354 STORE_NAME              14 (frame2)
    
-    81         356 PUSH_NULL
+    89         356 PUSH_NULL
                358 LOAD_NAME                3 (GTkDarkEntry)
                360 LOAD_NAME               14 (frame2)
                362 LOAD_ATTR               11 (frame)
                372 PRECALL                  1
                376 CALL                     1
                386 STORE_NAME              15 (entry2)
    
-    82         388 LOAD_NAME               15 (entry2)
+    90         388 LOAD_NAME               15 (entry2)
                390 LOAD_METHOD             13 (pack)
                412 LOAD_CONST              11 ('x')
                414 LOAD_CONST              12 (5)
                416 LOAD_CONST              12 (5)
                418 LOAD_CONST              12 (5)
                420 KW_NAMES                13
                422 PRECALL                  4
                426 CALL                     4
                436 POP_TOP
    
-    84         438 LOAD_NAME               14 (frame2)
+    92         438 LOAD_NAME               14 (frame2)
                440 LOAD_METHOD             13 (pack)
                462 LOAD_CONST              14 ('both')
                464 LOAD_CONST              15 ('yes')
                466 LOAD_CONST              18 ('left')
                468 KW_NAMES                17
                470 PRECALL                  3
                474 CALL                     3
                484 POP_TOP
    
-    86         486 LOAD_NAME                9 (root)
+    94         486 LOAD_NAME                9 (root)
                488 LOAD_METHOD             16 (mainloop)
                510 PRECALL                  0
                514 CALL                     0
                524 POP_TOP
                526 LOAD_CONST              19 (None)
                528 RETURN_VALUE
    
-    65     >>  530 LOAD_CONST              19 (None)
+    73     >>  530 LOAD_CONST              19 (None)
                532 RETURN_VALUE
    consts
       0
       ('AdwDrawRoundEntry3',)
       code
          argcount  : 0
          nlocals   : 0
@@ -204,15 +204,15 @@
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (default_palette)
          
           11          28 LOAD_CONST               3 (<code object palette_gtk_light, file "D:\tkadw\tkadw\tkite\gtk\entry.py", line 11>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               5 (palette_gtk_light)
          
-          35          34 LOAD_CONST               4 (<code object palette_gtk_dark, file "D:\tkadw\tkadw\tkite\gtk\entry.py", line 35>)
+          39          34 LOAD_CONST               4 (<code object palette_gtk_dark, file "D:\tkadw\tkadw\tkite\gtk\entry.py", line 39>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               6 (palette_gtk_dark)
                       40 LOAD_CLOSURE             0 (__class__)
                       42 COPY                     1
                       44 STORE_NAME               7 (__classcell__)
                       46 RETURN_VALUE
          consts
@@ -278,220 +278,238 @@
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\entry.py'
                name       'default_palette'
                firstlineno 8
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 17
+               stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  026403640464056406640764036408640964066407640a6408640b9c0ea6
-                  010000ab010000000000000000010064005300
+                  0264036404640564066407640864096404640a64066407640b6409640c9c
+                  06640d9c096901a6010000ab010000000000000000010064005300
                 11           0 RESUME                   0
                
                 12           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                14          26 LOAD_CONST               1 (11)
+                14          26 LOAD_CONST               1 ('entry')
                
-                16          28 LOAD_CONST               2 ((5, 5))
+                15          28 LOAD_CONST               2 (11)
                
-                18          30 LOAD_CONST               3 ('#eaeaea')
+                16          30 LOAD_CONST               3 ((5, 5))
                
-                19          32 LOAD_CONST               4 (1)
+                18          32 LOAD_CONST               4 ('#ffffff')
                
-                21          34 LOAD_CONST               5 ('#cdc7c2')
+                19          34 LOAD_CONST               5 ('#cdc7c2')
                
-                22          36 LOAD_CONST               6 ('#ffffff')
+                20          36 LOAD_CONST               6 ('#000000')
                
-                23          38 LOAD_CONST               7 ('#000000')
+                21          38 LOAD_CONST               7 (1)
                
-                24          40 LOAD_CONST               3 ('#eaeaea')
+                23          40 LOAD_CONST               8 ('#eaeaea')
                
-                25          42 LOAD_CONST               8 (0)
+                24          42 LOAD_CONST               9 (0)
                
-                27          44 LOAD_CONST               9 ('#3584e4')
+                27          44 LOAD_CONST               4 ('#ffffff')
                
-                28          46 LOAD_CONST               6 ('#ffffff')
+                28          46 LOAD_CONST              10 ('#3584e4')
                
-                29          48 LOAD_CONST               7 ('#000000')
+                29          48 LOAD_CONST               6 ('#000000')
                
-                30          50 LOAD_CONST              10 ('#185fb4')
+                30          50 LOAD_CONST               7 (1)
                
-                31          52 LOAD_CONST               8 (0)
+                32          52 LOAD_CONST              11 ('#185fb4')
                
-                13          54 LOAD_CONST              11 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
-                            56 BUILD_CONST_KEY_MAP     14
+                33          54 LOAD_CONST               9 (0)
                
-                12          58 PRECALL                  1
-                            62 CALL                     1
-                            72 POP_TOP
-                            74 LOAD_CONST               0 (None)
-                            76 RETURN_VALUE
+                26          56 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                            58 BUILD_CONST_KEY_MAP      6
+               
+                14          60 LOAD_CONST              13 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                            62 BUILD_CONST_KEY_MAP      9
+               
+                13          64 BUILD_MAP                1
+               
+                12          66 PRECALL                  1
+                            70 CALL                     1
+                            80 POP_TOP
+                            82 LOAD_CONST               0 (None)
+                            84 RETURN_VALUE
                consts
                   None
+                  'entry'
                   11
                   (5, 5)
-                  '#eaeaea'
-                  1
-                  '#cdc7c2'
                   '#ffffff'
+                  '#cdc7c2'
                   '#000000'
+                  1
+                  '#eaeaea'
                   0
                   '#3584e4'
                   '#185fb4'
-                  ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
+                  ('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width')
+                  ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\entry.py'
                name       'palette_gtk_light'
                firstlineno 11
                lnotab
-                  0x0201180202020202020102020201020102010201020202010201020102
-                  0102ee04ff
+                  0x0201180202010201020202010201020102020201020302010201020102
+                  02020102f904f404ff02ff
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 17
+               stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  02640364046405640664076403640864096406640a64096408640b9c0ea6
-                  010000ab010000000000000000010064005300
-                35           0 RESUME                   0
+                  0264036404640564066407640864096404640a640b6407640a6409640c9c
+                  06640d9c096901a6010000ab010000000000000000010064005300
+                39           0 RESUME                   0
                
-                36           2 LOAD_FAST                0 (self)
+                40           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                38          26 LOAD_CONST               1 (11)
+                42          26 LOAD_CONST               1 ('entry')
                
-                40          28 LOAD_CONST               2 ((5, 5))
+                43          28 LOAD_CONST               2 (11)
                
-                42          30 LOAD_CONST               3 ('#eaeaea')
+                44          30 LOAD_CONST               3 ((5, 5))
                
-                43          32 LOAD_CONST               4 (1)
+                46          32 LOAD_CONST               4 ('#2d2d2d')
                
-                45          34 LOAD_CONST               5 ('#1f1f1f')
+                47          34 LOAD_CONST               5 ('#1f1f1f')
                
-                46          36 LOAD_CONST               6 ('#2d2d2d')
+                48          36 LOAD_CONST               6 ('#cccccc')
                
-                47          38 LOAD_CONST               7 ('#cccccc')
+                49          38 LOAD_CONST               7 (1)
                
-                48          40 LOAD_CONST               3 ('#eaeaea')
+                51          40 LOAD_CONST               8 ('#eaeaea')
                
-                49          42 LOAD_CONST               8 (0)
+                52          42 LOAD_CONST               9 (0)
                
-                51          44 LOAD_CONST               9 ('#3584e4')
+                55          44 LOAD_CONST               4 ('#2d2d2d')
                
-                52          46 LOAD_CONST               6 ('#2d2d2d')
+                56          46 LOAD_CONST              10 ('#3584e4')
                
-                53          48 LOAD_CONST              10 ('#ffffff')
+                57          48 LOAD_CONST              11 ('#ffffff')
                
-                54          50 LOAD_CONST               9 ('#3584e4')
+                58          50 LOAD_CONST               7 (1)
                
-                55          52 LOAD_CONST               8 (0)
+                60          52 LOAD_CONST              10 ('#3584e4')
                
-                37          54 LOAD_CONST              11 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
-                            56 BUILD_CONST_KEY_MAP     14
+                61          54 LOAD_CONST               9 (0)
                
-                36          58 PRECALL                  1
-                            62 CALL                     1
-                            72 POP_TOP
-                            74 LOAD_CONST               0 (None)
-                            76 RETURN_VALUE
+                54          56 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                            58 BUILD_CONST_KEY_MAP      6
+               
+                42          60 LOAD_CONST              13 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                            62 BUILD_CONST_KEY_MAP      9
+               
+                41          64 BUILD_MAP                1
+               
+                40          66 PRECALL                  1
+                            70 CALL                     1
+                            80 POP_TOP
+                            82 LOAD_CONST               0 (None)
+                            84 RETURN_VALUE
                consts
                   None
+                  'entry'
                   11
                   (5, 5)
-                  '#eaeaea'
-                  1
-                  '#1f1f1f'
                   '#2d2d2d'
+                  '#1f1f1f'
                   '#cccccc'
+                  1
+                  '#eaeaea'
                   0
                   '#3584e4'
                   '#ffffff'
-                  ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
+                  ('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width')
+                  ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\entry.py'
                name       'palette_gtk_dark'
-               firstlineno 35
+               firstlineno 39
                lnotab
-                  0x0201180202020202020102020201020102010201020202010201020102
-                  0102ee04ff
+                  0x0201180202010201020202010201020102020201020302010201020102
+                  02020102f904f404ff02ff
          names      ('__name__', '__module__', '__qualname__', '__init__', 'default_palette', 'palette_gtk_light', 'palette_gtk_dark', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\entry.py'
          name       'GTkEntry'
          firstlineno 4
-         lnotab 0x0c010a0306030618
+         lnotab 0x0c010a030603061c
       'GTkEntry'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          60           0 RESUME                   0
+          68           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GTkDarkEntry')
                        8 STORE_NAME               2 (__qualname__)
          
-          61          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\tkite\gtk\entry.py", line 61>)
+          69          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\tkite\gtk\entry.py", line 69>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'GTkDarkEntry'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                61           0 RESUME                   0
+                69           0 RESUME                   0
                
-                62           2 LOAD_FAST                0 (self)
+                70           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_gtk_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_gtk_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\entry.py'
                name       'default_palette'
-               firstlineno 61
+               firstlineno 69
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\entry.py'
          name       'GTkDarkEntry'
-         firstlineno 60
+         firstlineno 68
          lnotab 0x0a01
       'GTkDarkEntry'
       '__main__'
       ('Tk',)
       ('GTkFrame', 'GTkDarkFrame', 'GTkEntry', 'GTkDarkEntry')
       '#1f1f1f'
       ('background',)
@@ -508,9 +526,9 @@
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\entry.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c031c381c050c010c01180214012c02160220013202300216
+      0x00ff02010c031c401c050c010c01180214012c02160220013202300216
       022001320230022ceb
```

### Comparing `tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc` & `tkadw-0.2.0/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x744c9564 (Fri Jun 23 07:40:36 2023 UTC)
-files sz: 1141
+moddate:  0x234c9664 (Sat Jun 24 01:51:31 2023 UTC)
+files sz: 1125
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100020047006402840064036501a60300
@@ -33,85 +33,85 @@
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               3 ('GTkFrame')
                 24 LOAD_NAME                1 (AdwDrawFrame)
                 26 PRECALL                  3
                 30 CALL                     3
                 40 STORE_NAME               2 (GTkFrame)
    
-    33          42 PUSH_NULL
+    34          42 PUSH_NULL
                 44 LOAD_BUILD_CLASS
-                46 LOAD_CONST               4 (<code object GTkDarkFrame, file "D:\tkadw\tkadw\tkite\gtk\frame.py", line 33>)
+                46 LOAD_CONST               4 (<code object GTkDarkFrame, file "D:\tkadw\tkadw\tkite\gtk\frame.py", line 34>)
                 48 MAKE_FUNCTION            0
                 50 LOAD_CONST               5 ('GTkDarkFrame')
                 52 LOAD_NAME                2 (GTkFrame)
                 54 PRECALL                  3
                 58 CALL                     3
                 68 STORE_NAME               3 (GTkDarkFrame)
    
-    38          70 LOAD_NAME                4 (__name__)
+    39          70 LOAD_NAME                4 (__name__)
                 72 LOAD_CONST               6 ('__main__')
                 74 COMPARE_OP               2 (==)
                 80 POP_JUMP_FORWARD_IF_FALSE   108 (to 298)
    
-    39          82 LOAD_CONST               0 (0)
+    40          82 LOAD_CONST               0 (0)
                 84 LOAD_CONST               7 (('Tk',))
                 86 IMPORT_NAME              5 (tkinter)
                 88 IMPORT_FROM              6 (Tk)
                 90 STORE_NAME               6 (Tk)
                 92 POP_TOP
    
-    40          94 PUSH_NULL
+    41          94 PUSH_NULL
                 96 LOAD_NAME                6 (Tk)
                 98 PRECALL                  0
                102 CALL                     0
                112 STORE_NAME               7 (root)
    
-    41         114 PUSH_NULL
+    42         114 PUSH_NULL
                116 LOAD_NAME                2 (GTkFrame)
                118 PRECALL                  0
                122 CALL                     0
                132 STORE_NAME               8 (frame)
    
-    42         134 LOAD_NAME                8 (frame)
+    43         134 LOAD_NAME                8 (frame)
                136 LOAD_METHOD              9 (pack)
                158 LOAD_CONST               8 ('both')
                160 LOAD_CONST               9 ('yes')
                162 LOAD_CONST              10 (2)
                164 LOAD_CONST              10 (2)
                166 KW_NAMES                11
                168 PRECALL                  4
                172 CALL                     4
                182 POP_TOP
    
-    43         184 PUSH_NULL
+    44         184 PUSH_NULL
                186 LOAD_NAME                3 (GTkDarkFrame)
                188 PRECALL                  0
                192 CALL                     0
                202 STORE_NAME              10 (frame2)
    
-    44         204 LOAD_NAME               10 (frame2)
+    45         204 LOAD_NAME               10 (frame2)
                206 LOAD_METHOD              9 (pack)
                228 LOAD_CONST               8 ('both')
                230 LOAD_CONST               9 ('yes')
                232 LOAD_CONST              10 (2)
                234 LOAD_CONST              10 (2)
                236 KW_NAMES                11
                238 PRECALL                  4
                242 CALL                     4
                252 POP_TOP
    
-    45         254 LOAD_NAME                7 (root)
+    46         254 LOAD_NAME                7 (root)
                256 LOAD_METHOD             11 (mainloop)
                278 PRECALL                  0
                282 CALL                     0
                292 POP_TOP
                294 LOAD_CONST              12 (None)
                296 RETURN_VALUE
    
-    38     >>  298 LOAD_CONST              12 (None)
+    39     >>  298 LOAD_CONST              12 (None)
                300 RETURN_VALUE
    consts
       0
       ('AdwDrawFrame',)
       code
          argcount  : 0
          nlocals   : 0
@@ -138,15 +138,15 @@
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (default_palette)
          
           11          28 LOAD_CONST               3 (<code object palette_gtk_light, file "D:\tkadw\tkadw\tkite\gtk\frame.py", line 11>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               5 (palette_gtk_light)
          
-          21          34 LOAD_CONST               4 (<code object palette_gtk_dark, file "D:\tkadw\tkadw\tkite\gtk\frame.py", line 21>)
+          22          34 LOAD_CONST               4 (<code object palette_gtk_dark, file "D:\tkadw\tkadw\tkite\gtk\frame.py", line 22>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               6 (palette_gtk_dark)
                       40 LOAD_CLOSURE             0 (__class__)
                       42 COPY                     1
                       44 STORE_NAME               7 (__classcell__)
                       46 RETURN_VALUE
          consts
@@ -216,156 +216,163 @@
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 7
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  026403640164049c04a6010000ab010000000000000000010064005300
+                  026403640464059c036901a6010000ab0100000000000000000100640053
+                  00
                 11           0 RESUME                   0
                
                 12           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                14          26 LOAD_CONST               1 ('#f6f5f4')
+                14          26 LOAD_CONST               1 ('frame')
                
-                15          28 LOAD_CONST               2 (2)
+                15          28 LOAD_CONST               2 ('#f6f5f4')
                
                 16          30 LOAD_CONST               3 ('#d5d0cc')
                
-                17          32 LOAD_CONST               1 ('#f6f5f4')
+                17          32 LOAD_CONST               4 (2)
                
-                13          34 LOAD_CONST               4 (('frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back'))
-                            36 BUILD_CONST_KEY_MAP      4
+                14          34 LOAD_CONST               5 (('back', 'border', 'border_width'))
+                            36 BUILD_CONST_KEY_MAP      3
                
-                12          38 PRECALL                  1
-                            42 CALL                     1
-                            52 POP_TOP
-                            54 LOAD_CONST               0 (None)
-                            56 RETURN_VALUE
+                13          38 BUILD_MAP                1
+               
+                12          40 PRECALL                  1
+                            44 CALL                     1
+                            54 POP_TOP
+                            56 LOAD_CONST               0 (None)
+                            58 RETURN_VALUE
                consts
                   None
+                  'frame'
                   '#f6f5f4'
-                  2
                   '#d5d0cc'
-                  ('frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back')
+                  2
+                  ('back', 'border', 'border_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\frame.py'
                name       'palette_gtk_light'
                firstlineno 11
-               lnotab 0x0201180202010201020102fc04ff
+               lnotab 0x0201180202010201020102fd04ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 7
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  026403640164049c04a6010000ab010000000000000000010064005300
-                21           0 RESUME                   0
+                  026402640364049c036901a6010000ab0100000000000000000100640053
+                  00
+                22           0 RESUME                   0
                
-                22           2 LOAD_FAST                0 (self)
+                23           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                24          26 LOAD_CONST               1 ('#353535')
+                25          26 LOAD_CONST               1 ('frame')
                
-                25          28 LOAD_CONST               2 (2)
+                26          28 LOAD_CONST               2 ('#353535')
                
-                26          30 LOAD_CONST               3 ('#1b1b1b')
+                27          30 LOAD_CONST               2 ('#353535')
                
-                27          32 LOAD_CONST               1 ('#353535')
+                28          32 LOAD_CONST               3 (2)
                
-                23          34 LOAD_CONST               4 (('frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back'))
-                            36 BUILD_CONST_KEY_MAP      4
+                25          34 LOAD_CONST               4 (('back', 'border', 'border_width'))
+                            36 BUILD_CONST_KEY_MAP      3
                
-                22          38 PRECALL                  1
-                            42 CALL                     1
-                            52 POP_TOP
-                            54 LOAD_CONST               0 (None)
-                            56 RETURN_VALUE
+                24          38 BUILD_MAP                1
+               
+                23          40 PRECALL                  1
+                            44 CALL                     1
+                            54 POP_TOP
+                            56 LOAD_CONST               0 (None)
+                            58 RETURN_VALUE
                consts
                   None
+                  'frame'
                   '#353535'
                   2
-                  '#1b1b1b'
-                  ('frame_frame_back', 'frame_border_width', 'frame_border', 'frame_back')
+                  ('back', 'border', 'border_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\frame.py'
                name       'palette_gtk_dark'
-               firstlineno 21
-               lnotab 0x0201180202010201020102fc04ff
+               firstlineno 22
+               lnotab 0x0201180202010201020102fd04ff02ff
          names      ('__name__', '__module__', '__qualname__', '__init__', 'default_palette', 'palette_gtk_light', 'palette_gtk_dark', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\frame.py'
          name       'GTkFrame'
          firstlineno 4
-         lnotab 0x0c010a030603060a
+         lnotab 0x0c010a030603060b
       'GTkFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          33           0 RESUME                   0
+          34           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GTkDarkFrame')
                        8 STORE_NAME               2 (__qualname__)
          
-          34          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\tkite\gtk\frame.py", line 34>)
+          35          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\tkite\gtk\frame.py", line 35>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'GTkDarkFrame'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                34           0 RESUME                   0
+                35           0 RESUME                   0
                
-                35           2 LOAD_FAST                0 (self)
+                36           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_gtk_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_gtk_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\frame.py'
                name       'default_palette'
-               firstlineno 34
+               firstlineno 35
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\frame.py'
          name       'GTkDarkFrame'
-         firstlineno 33
+         firstlineno 34
          lnotab 0x0a01
       'GTkDarkFrame'
       '__main__'
       ('Tk',)
       'both'
       'yes'
       2
@@ -374,8 +381,8 @@
    names      ('tkadw', 'AdwDrawFrame', 'GTkFrame', 'GTkDarkFrame', '__name__', 'tkinter', 'Tk', 'root', 'frame', 'pack', 'frame2', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\frame.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c031c1d1c050c010c01140114013201140132012cf9
+   lnotab 0x00ff02010c031c1e1c050c010c01140114013201140132012cf9
```

### Comparing `tkadw-0.1.5/tkadw/tkite/gtk/textbox.py` & `tkadw-0.2.0/tkadw/tkite/gtk/textbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,88 +7,86 @@
 
     def default_palette(self):
         self.palette_gtk_light()
 
     def palette_gtk_light(self):
         self.palette(
             {
-                "text_padding": (3, 3),
+                "text": {
+                    "padding": (5, 5),
 
-                "text_frame_back": "#eaeaea",
-                "text_border_width": 1,
-
-                "text_border": "#cdc7c2",
-                "text_back": "#ffffff",
-                "text_text_back": "#000000",
-                "text_bottom_line": "#eaeaea",
-                "text_bottom_width": 0,
-
-                "text_focusin_border": "#3584e4",
-                "text_focusin_back": "#ffffff",
-                "text_focusin_text_back": "#000000",
-                "text_focusin_bottom_line": "#185fb4",
-                "text_focusin_bottom_width": 0,
+                    "back": "#ffffff",
+                    "border": "#cdc7c2",
+                    "text_back": "#000000",
+                    "border_width": 1,
+
+                    "bottom_line": "#eaeaea",
+                    "bottom_width": 0,
+
+                    "focusin": {
+                        "back": "#ffffff",
+                        "border": "#3584e4",
+                        "text_back": "#000000",
+                        "border_width": 1,
+
+                        "bottom_line": "#185fb4",
+                        "bottom_width": 0,
+                    }
+                },
             }
         )
 
     def palette_gtk_dark(self):
         self.palette(
             {
-                "text_padding": (3, 3),
-
-                "text_frame_back": "#eaeaea",
-                "text_border_width": 1,
+                "text": {
+                    "padding": (5, 5),
 
-                "text_border": "#1f1f1f",
-                "text_back": "#2d2d2d",
-                "text_text_back": "#cccccc",
-                "text_bottom_line": "#eaeaea",
-                "text_bottom_width": 0,
-
-                "text_focusin_border": "#3584e4",
-                "text_focusin_back": "#2d2d2d",
-                "text_focusin_text_back": "#ffffff",
-                "text_focusin_bottom_line": "#3584e4",
-                "text_focusin_bottom_width": 0,
+                    "back": "#2d2d2d",
+                    "border": "#1f1f1f",
+                    "text_back": "#cccccc",
+                    "border_width": 1,
+
+                    "bottom_line": "#eaeaea",
+                    "bottom_width": 0,
+
+                    "focusin": {
+                        "back": "#2d2d2d",
+                        "border": "#3584e4",
+                        "text_back": "#ffffff",
+                        "border_width": 1,
+
+                        "bottom_line": "#3584e4",
+                        "bottom_width": 0,
+                    }
+                },
             }
         )
 
 
 class GTkDarkTextBox(GTkTextBox):
     def default_palette(self):
         self.palette_gtk_dark()
 
 
 if __name__ == '__main__':
     from tkinter import Tk
-    from tkadw import GTkFrame, GTkDarkFrame, GTkButton, GTkDarkButton, GTkEntry, GTkDarkEntry
+    from tkadw import GTkFrame, GTkDarkFrame
 
     root = Tk()
     root.configure(background="#1f1f1f")
 
     frame = GTkFrame(root)
 
-    button1 = GTkButton(frame.frame, text="GTkButton")
-    button1.pack(fill="x", ipadx=5, padx=5, pady=5)
-
-    entry1 = GTkEntry(frame.frame)
-    entry1.pack(fill="x", ipadx=5, padx=5, pady=5)
-
     textbox1 = GTkTextBox(frame.frame)
     textbox1.pack(fill="x", ipadx=5, padx=5, pady=5)
 
     frame.pack(fill="both", expand="yes", side="right")
 
     frame2 = GTkDarkFrame(root)
 
-    button2 = GTkDarkButton(frame2.frame, text="GTkDarkButton")
-    button2.pack(fill="x", ipadx=5, padx=5, pady=5)
-
-    entry2 = GTkDarkEntry(frame2.frame)
-    entry2.pack(fill="x", ipadx=5, padx=5, pady=5)
-
     textbox2 = GTkDarkTextBox(frame2.frame)
     textbox2.pack(fill="x", ipadx=5, padx=5, pady=5)
 
     frame2.pack(fill="both", expand="yes", side="left")
 
     root.mainloop()
```

### Comparing `tkadw-0.1.5/PKG-INFO` & `tkadw-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tkadw
-Version: 0.1.5
-Summary: 
+Version: 0.2.0
+Summary: extra for tkinter
 Author: XiangQinxi
 Author-email: 1379773753@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

