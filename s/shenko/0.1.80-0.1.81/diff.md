# Comparing `tmp/shenko-0.1.80-py2.py3-none-any.whl.zip` & `tmp/shenko-0.1.81-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 26620 bytes, number of entries: 30
--rw-rw-r--  2.0 unx      171 b- defN 23-May-29 02:14 shenko/__init__.py
+Zip file size: 27907 bytes, number of entries: 33
+-rw-rw-r--  2.0 unx      171 b- defN 23-Jun-24 18:05 shenko/__init__.py
 -rw-rw-r--  2.0 unx      299 b- defN 20-Sep-12 04:15 shenko/cli.py
 -rw-rw-r--  2.0 unx     4390 b- defN 21-Sep-04 18:29 shenko/click.ogg
 -rw-rw-r--  2.0 unx     9877 b- defN 21-Sep-04 18:29 shenko/logo.png
--rw-rw-r--  2.0 unx     1931 b- defN 23-May-29 02:08 shenko/shenko.py
+-rw-rw-r--  2.0 unx     2978 b- defN 23-Jun-24 17:57 shenko/shenko.py
 -rw-rw-r--  2.0 unx     2643 b- defN 22-Jan-03 10:55 shenko/S01_HOME/HOME.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Sep-05 02:30 shenko/S01_HOME/__init__.py
 -rw-rw-r--  2.0 unx      518 b- defN 20-Mar-28 22:03 shenko/S02_FILESYSTEM/FILESYSTEM.py
 -rw-rw-r--  2.0 unx       34 b- defN 20-Mar-28 22:03 shenko/S02_FILESYSTEM/__init__.py
 -rw-rw-r--  2.0 unx      515 b- defN 20-Mar-28 22:03 shenko/S03_TEMPORARY/TEMPORARY.py
 -rw-rw-r--  2.0 unx       32 b- defN 20-Mar-28 22:03 shenko/S03_TEMPORARY/__init__.py
 -rw-rw-r--  2.0 unx     2984 b- defN 20-Nov-27 17:11 shenko/S04_INPUTS/INPUTS.py
@@ -18,15 +18,18 @@
 -rw-rw-r--  2.0 unx       26 b- defN 20-Mar-28 22:03 shenko/S06_OUTPUT/__init__.py
 -rw-rw-r--  2.0 unx      514 b- defN 20-Mar-28 22:03 shenko/S07_ROBOT_HOME/ROBOT_HOME.py
 -rw-rw-r--  2.0 unx       33 b- defN 20-Mar-28 22:03 shenko/S07_ROBOT_HOME/__init__.py
 -rw-rw-r--  2.0 unx      509 b- defN 20-Mar-28 22:03 shenko/S08_NETWORK/NETWORK.py
 -rw-rw-r--  2.0 unx       28 b- defN 20-Mar-28 22:03 shenko/S08_NETWORK/__init__.py
 -rw-rw-r--  2.0 unx      513 b- defN 20-Mar-28 22:03 shenko/S09_EXTERNAL/EXTERNAL.py
 -rw-rw-r--  2.0 unx       30 b- defN 20-Mar-28 22:03 shenko/S09_EXTERNAL/__init__.py
--rw-r--r--  2.0 unx      163 b- defN 23-May-29 02:15 shenko-0.1.80.dist-info/AUTHORS.rst
--rw-r--r--  2.0 unx     1544 b- defN 23-May-29 02:15 shenko-0.1.80.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2374 b- defN 23-May-29 02:15 shenko-0.1.80.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-29 02:15 shenko-0.1.80.dist-info/WHEEL
--rw-rw-r--  2.0 unx       47 b- defN 23-May-29 02:15 shenko-0.1.80.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-May-29 02:15 shenko-0.1.80.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2475 b- defN 23-May-29 02:15 shenko-0.1.80.dist-info/RECORD
-30 files, 32979 bytes uncompressed, 22608 bytes compressed:  31.4%
+-rw-rw-r--  2.0 unx       54 b- defN 23-Jun-24 17:57 shenko/s00_init/__init__.py
+-rw-rw-r--  2.0 unx      226 b- defN 23-Jun-24 17:57 shenko/s00_init/configurator.py
+-rw-rw-r--  2.0 unx      159 b- defN 23-Jun-24 17:57 shenko/s00_init/platformer.py
+-rw-rw-r--  2.0 unx      206 b- defN 23-Jun-24 18:05 shenko-0.1.81.dist-info/AUTHORS.rst
+-rw-r--r--  2.0 unx     1544 b- defN 23-Jun-24 18:05 shenko-0.1.81.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2380 b- defN 23-Jun-24 18:05 shenko-0.1.81.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-24 18:05 shenko-0.1.81.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       47 b- defN 23-Jun-24 18:05 shenko-0.1.81.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-24 18:05 shenko-0.1.81.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2729 b- defN 23-Jun-24 18:05 shenko-0.1.81.dist-info/RECORD
+33 files, 34768 bytes uncompressed, 23493 bytes compressed:  32.4%
```

## zipnote {}

```diff
@@ -63,29 +63,38 @@
 
 Filename: shenko/S09_EXTERNAL/EXTERNAL.py
 Comment: 
 
 Filename: shenko/S09_EXTERNAL/__init__.py
 Comment: 
 
-Filename: shenko-0.1.80.dist-info/AUTHORS.rst
+Filename: shenko/s00_init/__init__.py
 Comment: 
 
-Filename: shenko-0.1.80.dist-info/LICENSE
+Filename: shenko/s00_init/configurator.py
 Comment: 
 
-Filename: shenko-0.1.80.dist-info/METADATA
+Filename: shenko/s00_init/platformer.py
 Comment: 
 
-Filename: shenko-0.1.80.dist-info/WHEEL
+Filename: shenko-0.1.81.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: shenko-0.1.80.dist-info/entry_points.txt
+Filename: shenko-0.1.81.dist-info/LICENSE
 Comment: 
 
-Filename: shenko-0.1.80.dist-info/top_level.txt
+Filename: shenko-0.1.81.dist-info/METADATA
 Comment: 
 
-Filename: shenko-0.1.80.dist-info/RECORD
+Filename: shenko-0.1.81.dist-info/WHEEL
+Comment: 
+
+Filename: shenko-0.1.81.dist-info/entry_points.txt
+Comment: 
+
+Filename: shenko-0.1.81.dist-info/top_level.txt
+Comment: 
+
+Filename: shenko-0.1.81.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shenko/__init__.py

```diff
@@ -1,8 +1,8 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for shenko."""
 
 __author__ = """Danny Dowshenko"""
 __email__ = 'dowshenko225@gmail.com'
-__version__ = '0.1.80'
+__version__ = '0.1.81'
 import shenko
```

## shenko/shenko.py

```diff
@@ -6,30 +6,45 @@
 ===================
 
 Shenko is a open source platform that uses the Panda3d game engine.
 You can visit us on our website www.shenko.org
 or find this code on github/shenko:
     https://github.com/shenko/shenko/blob/master/shenko/shenko.py
 
-Author:
-    Your Name <your@email.com>
+Authors:
+    SHENKO Development Team
 
 License:
-    The license information for your code.
+    # Copyright 2018 SHENKO
+    #
+    # This program is free software: you can redistribute it and/or modify
+    # it under the terms of the GNU General Public License as published by
+    # the Free Software Foundation, either version 3 of the License, or
+    # (at your option) any later version.
+    #
+    # This program is distributed in the hope that it will be useful,
+    # but WITHOUT ANY WARRANTY; without even the implied warranty of
+    # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    # GNU General Public License for more details.
+    #
+    # You should have received a copy of the GNU General Public License
+    # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 
 __author__      = "Shenko Development Team"
 __email__       = "shenko.org@gmail.com"
 __copyright__   = "http://creativecommons.org/licenses/by/3.0/legalcode"
 
 # Standard library imports
 import os
 import sys
 
+from s00_init import platformer, configurator
+
 # Third-party imports
 from direct.showbase.ShowBase import ShowBase
 
 # Local imports
 
 
 #--------------VARIABLES---------------/
@@ -49,14 +64,24 @@
         base.setBackgroundColor(0,0,0)
 
         # Main Menu
         if mainMenuState == True:
             print("Main Menu showing")
             # show mouse cursor
 
+        # Access functions from platformer module
+        platformer.start_platformer()
+        platformer.jump()
+        platformer.move("right")
+
+        # Access functions from configurator module
+        configurator.configure_settings()
+        configurator.set_resolution(1920, 1080)
+        configurator.set_volume(0.8)
+
         # Input
         self.accept('escape', self.quit)
         self.accept('m', self.menuToggle)
         #self.accept('arrow_down-repeat', self.moveCam)
 
     def menuToggle(self):
         global mainMenuState
```

## Comparing `shenko-0.1.80.dist-info/LICENSE` & `shenko-0.1.81.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `shenko-0.1.80.dist-info/METADATA` & `shenko-0.1.81.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: shenko
-Version: 0.1.80
+Version: 0.1.81
 Summary: visit us at www.shenko.org
 Home-page: https://github.com/shenko/shenko
-Author: Danny Dowshenko
-Author-email: dowshenko225@gmail.com
+Author: Shenko Development Team
+Author-email: shenko.org@gmail.com
 License: GNU General Public License v3
 Keywords: shenko
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
```

## Comparing `shenko-0.1.80.dist-info/RECORD` & `shenko-0.1.81.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-shenko/__init__.py,sha256=qFBVQz4-SMOsToea5pTienRbV39j7vKba0YKmAJa1sU,171
+shenko/__init__.py,sha256=96oIouaS8ZOQ_hdEMYYabmzHIfnNm_cEcIBnXBBszyo,171
 shenko/cli.py,sha256=J1oDDAhQ1hD5SDtG18TirBg0zG0_gCQA9m8Q8Jo_JRw,299
 shenko/click.ogg,sha256=wnU0YNNIrSfiLHdPfpC44PDwzOoVqn18gb01przl68E,4390
 shenko/logo.png,sha256=4ChGYJc8BsbKyye9pV5VQg-ly3IiGPXD_fz313Kgs1U,9877
-shenko/shenko.py,sha256=cEnaoW5WwOjjDQQYWQ4wETTLkzgpbw-4QPnnayRjWtw,1931
+shenko/shenko.py,sha256=O3S1j0qov2XFxV1GNAVHyN86FNa_2HOLWrQRgcYucwY,2978
 shenko/S01_HOME/HOME.py,sha256=jBs535SBJDCvSNWqpYDIQSVcGwvyf5I4zoKhpVZ3kiw,2643
 shenko/S01_HOME/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 shenko/S02_FILESYSTEM/FILESYSTEM.py,sha256=bsZK16xchZBZREPX-4nNnVRzQjsEcAMbri3IzKnsnXY,518
 shenko/S02_FILESYSTEM/__init__.py,sha256=ij30J3f0R-n33HOhglleb66lqmsq0UbNtejkrM4Pnhw,34
 shenko/S03_TEMPORARY/TEMPORARY.py,sha256=SvWFoSwrwIoCjUMPbvXEgUmg5KArNQeubTLDAxSsa-U,515
 shenko/S03_TEMPORARY/__init__.py,sha256=eXpCFZ3y8yz6u7DN86lWbuncuKG61gF8BUQf6GymSsQ,32
 shenko/S04_INPUTS/INPUTS.py,sha256=8Aa1_2Rx_ethmiOpMVXrhtCG1EhFdIBQACl1tAUjvYc,2984
@@ -17,14 +17,17 @@
 shenko/S06_OUTPUT/__init__.py,sha256=sv_n4tv61KFtb0L85KA9-_un8Ed8OQMh_Xl_EMh_kxI,26
 shenko/S07_ROBOT_HOME/ROBOT_HOME.py,sha256=OG1p1FeTWVPEK8neYsyhzHBippBC9ugFND7T8UoQ9SE,514
 shenko/S07_ROBOT_HOME/__init__.py,sha256=uwwyJ2LIqc0flvpcUECbxYvXJZXL4g6BvQur2pkiJ10,33
 shenko/S08_NETWORK/NETWORK.py,sha256=zWfV5SpN4MtYtVP7iMwsED_cyOJ70z9BGdR8YCIV1To,509
 shenko/S08_NETWORK/__init__.py,sha256=rhZflP5Ygt-R4TmWnyFKasu24tN_N_dcPmh95UdhyiU,28
 shenko/S09_EXTERNAL/EXTERNAL.py,sha256=pYrOjGd2vFbcKpnGFJ310JHHrXR-20lq-4rAloyn3f8,513
 shenko/S09_EXTERNAL/__init__.py,sha256=l5RG-UNGyQiwHtLatKTMtKM9d4S51EXoQiKSUBvuuzM,30
-shenko-0.1.80.dist-info/AUTHORS.rst,sha256=a5KR6XxEAzVsZGfI__INBjmQC-93SkI8uiJDtJVjB7o,163
-shenko-0.1.80.dist-info/LICENSE,sha256=_62wb61LFQ1ZJmqfnHle0byVnwTI9qAG42ty8Jw37qU,1544
-shenko-0.1.80.dist-info/METADATA,sha256=5_LVljrO726O_dkKhqlME_gZaA5Vs7joe3dr9TlqJek,2374
-shenko-0.1.80.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-shenko-0.1.80.dist-info/entry_points.txt,sha256=p_ULA8DSdV--tsN9bTiGrsU4ETN2lWiN5UdVLCyfcis,47
-shenko-0.1.80.dist-info/top_level.txt,sha256=AjQhm7_LeWUnzn8TGLK45F0sCMxVQ94QqVYpojvHx2M,7
-shenko-0.1.80.dist-info/RECORD,,
+shenko/s00_init/__init__.py,sha256=P9aDMDHLT6jDp1GShCYd_mb4Qmgz6mUCNkUNna6-CrU,54
+shenko/s00_init/configurator.py,sha256=hjufTWRkqwxgLBcPx649jIG8HwaJ2wrKyxukIGyFhpQ,226
+shenko/s00_init/platformer.py,sha256=3WXQ0ukWtquDlu-cCPXIi1Oa77mLYFxsatsa8SRKBoM,159
+shenko-0.1.81.dist-info/AUTHORS.rst,sha256=4MR7p_KB7M0Wh9-FBpQ072MJy5nDlgR-RfXKRtKGrmg,206
+shenko-0.1.81.dist-info/LICENSE,sha256=_62wb61LFQ1ZJmqfnHle0byVnwTI9qAG42ty8Jw37qU,1544
+shenko-0.1.81.dist-info/METADATA,sha256=Z0INbMdd4u2V_V6qblpxwn2EPviuoVaRtPzXvW8l_x4,2380
+shenko-0.1.81.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+shenko-0.1.81.dist-info/entry_points.txt,sha256=p_ULA8DSdV--tsN9bTiGrsU4ETN2lWiN5UdVLCyfcis,47
+shenko-0.1.81.dist-info/top_level.txt,sha256=AjQhm7_LeWUnzn8TGLK45F0sCMxVQ94QqVYpojvHx2M,7
+shenko-0.1.81.dist-info/RECORD,,
```

