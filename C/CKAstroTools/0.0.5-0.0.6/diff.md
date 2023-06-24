# Comparing `tmp/CKAstroTools-0.0.5.tar.gz` & `tmp/CKAstroTools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CKAstroTools-0.0.5.tar", last modified: Thu Jun 22 09:26:23 2023, max compression
+gzip compressed data, was "CKAstroTools-0.0.6.tar", last modified: Sat Jun 24 05:44:42 2023, max compression
```

## Comparing `CKAstroTools-0.0.5.tar` & `CKAstroTools-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/CKAstroTools.egg-info/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1476 2023-06-22 09:26:23.000000 CKAstroTools-0.0.5/CKAstroTools.egg-info/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      405 2023-06-22 09:26:23.000000 CKAstroTools-0.0.5/CKAstroTools.egg-info/SOURCES.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-06-22 09:26:23.000000 CKAstroTools-0.0.5/CKAstroTools.egg-info/dependency_links.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-06-22 09:26:23.000000 CKAstroTools-0.0.5/CKAstroTools.egg-info/requires.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       13 2023-06-22 09:26:23.000000 CKAstroTools-0.0.5/CKAstroTools.egg-info/top_level.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 CKAstroTools-0.0.5/LICENSE
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1476 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      874 2023-06-22 09:22:37.000000 CKAstroTools-0.0.5/README.md
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/ckastrotools/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2022-12-19 09:28:13.000000 CKAstroTools-0.0.5/ckastrotools/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 CKAstroTools-0.0.5/ckastrotools/__main__.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/ckastrotools/io/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       31 2022-12-19 10:11:43.000000 CKAstroTools-0.0.5/ckastrotools/io/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1270 2022-12-19 10:33:57.000000 CKAstroTools-0.0.5/ckastrotools/io/subcube.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/ckastrotools/milkyway/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        0 2023-06-10 14:05:04.000000 CKAstroTools-0.0.5/ckastrotools/milkyway/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)    17687 2023-06-22 09:21:02.000000 CKAstroTools-0.0.5/ckastrotools/milkyway/spiralarms.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      826 2023-06-22 09:22:53.000000 CKAstroTools-0.0.5/pyproject.toml
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/setup.cfg
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-22 09:26:23.118993 CKAstroTools-0.0.5/tests/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 CKAstroTools-0.0.5/tests/test_main.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.340756 CKAstroTools-0.0.6/
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.336757 CKAstroTools-0.0.6/CKAstroTools.egg-info/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1476 2023-06-24 05:44:42.000000 CKAstroTools-0.0.6/CKAstroTools.egg-info/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      443 2023-06-24 05:44:42.000000 CKAstroTools-0.0.6/CKAstroTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-06-24 05:44:42.000000 CKAstroTools-0.0.6/CKAstroTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-06-24 05:44:42.000000 CKAstroTools-0.0.6/CKAstroTools.egg-info/requires.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       13 2023-06-24 05:44:42.000000 CKAstroTools-0.0.6/CKAstroTools.egg-info/top_level.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 CKAstroTools-0.0.6/LICENSE
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1476 2023-06-24 05:44:42.340756 CKAstroTools-0.0.6/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      874 2023-06-22 09:22:37.000000 CKAstroTools-0.0.6/README.md
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.336757 CKAstroTools-0.0.6/ckastrotools/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       33 2023-06-23 04:41:23.000000 CKAstroTools-0.0.6/ckastrotools/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 CKAstroTools-0.0.6/ckastrotools/__main__.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.336757 CKAstroTools-0.0.6/ckastrotools/io/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       36 2023-06-23 04:40:16.000000 CKAstroTools-0.0.6/ckastrotools/io/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1319 2023-06-23 04:43:12.000000 CKAstroTools-0.0.6/ckastrotools/io/subcube.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.336757 CKAstroTools-0.0.6/ckastrotools/milkyway/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       49 2023-06-23 04:37:12.000000 CKAstroTools-0.0.6/ckastrotools/milkyway/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      835 2023-06-24 05:41:45.000000 CKAstroTools-0.0.6/ckastrotools/milkyway/galactic_bar.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)    17778 2023-06-23 04:38:15.000000 CKAstroTools-0.0.6/ckastrotools/milkyway/spiralarms.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      826 2023-06-24 05:43:35.000000 CKAstroTools-0.0.6/pyproject.toml
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-06-24 05:44:42.340756 CKAstroTools-0.0.6/setup.cfg
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-24 05:44:42.336757 CKAstroTools-0.0.6/tests/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 CKAstroTools-0.0.6/tests/test_main.py
```

### Comparing `CKAstroTools-0.0.5/CKAstroTools.egg-info/PKG-INFO` & `CKAstroTools-0.0.6/CKAstroTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CKAstroTools
-Version: 0.0.5
+Version: 0.0.6
 Summary: General toolks for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CKAstroTools-0.0.5/LICENSE` & `CKAstroTools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.5/PKG-INFO` & `CKAstroTools-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CKAstroTools
-Version: 0.0.5
+Version: 0.0.6
 Summary: General toolks for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CKAstroTools-0.0.5/README.md` & `CKAstroTools-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.5/ckastrotools/io/subcube.py` & `CKAstroTools-0.0.6/ckastrotools/io/subcube.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Working on subcubes."""
+"""Module to work on subcubes."""
 from typing import Optional
 import astropy.units as u
 from spectral_cube import SpectralCube
 
 
 def extractCutout(cube: SpectralCube,
                   glon: float, glat: float,
@@ -20,19 +20,20 @@
     glat:
         Galactic latitude of the center.
     width:
         Width in degrees.
     v_min:
         Minimum velocity in km/s (default = -49.5 km/s).
     v_max:
-        Maxiumum velocity in km/s (default = -49.5 km/s).
+        Maxiumum velocity in km/s (default = 150 km/s).
 
     Returns
     -------
-    Returns the extracted subcube.
+    subcube: spectral_cube.SpectralCube
+        Returns the extracted subcube.
     """
     glon_min = glon - width / 2
     glon_max = glon + width / 2
     glat_min = glat - width / 2
     glat_max = glat + width / 2
 
     if v_min is None:
```

### Comparing `CKAstroTools-0.0.5/ckastrotools/milkyway/spiralarms.py` & `CKAstroTools-0.0.6/ckastrotools/milkyway/spiralarms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module for spiral arm functions."""
+"""Module for the spiral arms of the Milky Way."""
 
 import numpy as np
 from astropy.coordinates import SkyCoord
 from astropy import units as u
 
 
 def _getSpiralParameters(model):
@@ -248,15 +248,16 @@
     resolution: float
         Resolution of the spiral arm model in degrees.
     R_0: float
         Galactocentric distance of the sun in kpc.
 
     Returns
     -------
-    Coordinates of the spiral arm in the galactocentric frame.
+    coordinates: astropy.coordinates.Galactocentric
+        Coordinates of the spiral arm in the galactocentric frame.
     """
     spiral_arm_params = _getSpiralParameters(model)
 
     R_ref = spiral_arm_params[name]['R_ref']
     beta_ref = spiral_arm_params[name]['beta_ref']
     pitch = spiral_arm_params[name]['pitch']
     beta_min = spiral_arm_params[name]['beta_min']
@@ -341,25 +342,27 @@
     # per_x = list(pckx) + list(pvx2) + list(px) + list(pvx)
     # per_y = list(pcky) + list(pvy2) + list(py) + list(pvy)
     perseus = getSpiralArm('perseus', model=model)
 
     return sagittarius, scutum, outer, perseus
 
 
-def getSpiralArms(model='vallee2015'):
+def getSpiralArms(model='reid2014'):
     """
     Returns the spiral arms in a dictionary.
 
     Parameters
     ----------
-    model: The model to use
+    model: str
+        The model to use
 
     Returns
     -------
-    dict: A dictionary with the spiral arms.
+    arms: dict
+        A dictionary with the spiral arms.
     """
     sagittarius, scutum, outer, perseus = getSpiralArmsDetail(model=model)
 
     return {'sagittarius': sagittarius,
             'scutum': scutum,
             'perseus': perseus,
             'outer': outer}
```

### Comparing `CKAstroTools-0.0.5/pyproject.toml` & `CKAstroTools-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
             "pytest",
             "pytest-mock"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CKAstroTools"
 description = "General toolks for astronomy I personally use regularly for data analysis."
-version = "0.0.5"
+version = "0.0.6"
 requires-python = ">=3.7"
 dependencies = ["spectral-cube"]
 keywords = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

