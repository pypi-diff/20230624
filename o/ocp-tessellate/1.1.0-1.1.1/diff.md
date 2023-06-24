# Comparing `tmp/ocp_tessellate-1.1.0.tar.gz` & `tmp/ocp_tessellate-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_tessellate-1.1.0.tar", last modified: Fri Jun 16 20:28:20 2023, max compression
+gzip compressed data, was "ocp_tessellate-1.1.1.tar", last modified: Sat Jun 24 13:03:12 2023, max compression
```

## Comparing `ocp_tessellate-1.1.0.tar` & `ocp_tessellate-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-16 20:28:20.584547 ocp_tessellate-1.1.0/
--rw-r--r--   0 bernhard   (501) staff       (20)      810 2023-06-16 20:28:20.584589 ocp_tessellate-1.1.0/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-02-04 10:28:52.000000 ocp_tessellate-1.1.0/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-16 20:28:20.583840 ocp_tessellate-1.1.0/ocp_tessellate/
--rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.0/ocp_tessellate/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-06-16 06:52:31.000000 ocp_tessellate-1.1.0/ocp_tessellate/_version.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13575 2023-06-15 16:29:54.000000 ocp_tessellate-1.1.0/ocp_tessellate/cad_objects.py
--rw-r--r--   0 bernhard   (501) staff       (20)    30958 2023-06-16 06:31:35.000000 ocp_tessellate-1.1.0/ocp_tessellate/convert.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10521 2023-06-16 06:30:40.000000 ocp_tessellate-1.1.0/ocp_tessellate/defaults.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.0/ocp_tessellate/mp_tess.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.0/ocp_tessellate/mp_tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)    22358 2023-06-15 21:03:54.000000 ocp_tessellate-1.1.0/ocp_tessellate/ocp_utils.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-23 10:15:07.000000 ocp_tessellate-1.1.0/ocp_tessellate/stepreader.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-23 10:15:07.000000 ocp_tessellate-1.1.0/ocp_tessellate/tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-29 10:55:18.000000 ocp_tessellate-1.1.0/ocp_tessellate/utils.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-16 20:28:20.584455 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      810 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-06-16 20:28:20.000000 ocp_tessellate-1.1.0/ocp_tessellate.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-06-16 20:28:20.584876 ocp_tessellate-1.1.0/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-06-16 06:52:31.000000 ocp_tessellate-1.1.0/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:03:12.913377 ocp_tessellate-1.1.1/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-06-24 13:03:12.913434 ocp_tessellate-1.1.1/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-02-04 10:28:52.000000 ocp_tessellate-1.1.1/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:03:12.912602 ocp_tessellate-1.1.1/ocp_tessellate/
+-rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.1/ocp_tessellate/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-06-24 13:02:34.000000 ocp_tessellate-1.1.1/ocp_tessellate/_version.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13603 2023-06-24 13:01:17.000000 ocp_tessellate-1.1.1/ocp_tessellate/cad_objects.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    30958 2023-06-16 06:31:35.000000 ocp_tessellate-1.1.1/ocp_tessellate/convert.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10521 2023-06-16 06:30:40.000000 ocp_tessellate-1.1.1/ocp_tessellate/defaults.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.1/ocp_tessellate/mp_tess.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.1/ocp_tessellate/mp_tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    22358 2023-06-15 21:03:54.000000 ocp_tessellate-1.1.1/ocp_tessellate/ocp_utils.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-23 10:15:07.000000 ocp_tessellate-1.1.1/ocp_tessellate/stepreader.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-23 10:15:07.000000 ocp_tessellate-1.1.1/ocp_tessellate/tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-29 10:55:18.000000 ocp_tessellate-1.1.1/ocp_tessellate/utils.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:03:12.913244 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-06-24 13:03:12.913691 ocp_tessellate-1.1.1/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-06-24 13:02:34.000000 ocp_tessellate-1.1.1/setup.py
```

### Comparing `ocp_tessellate-1.1.0/PKG-INFO` & `ocp_tessellate-1.1.1/ocp_tessellate.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
-Name: ocp_tessellate
-Version: 1.1.0
+Name: ocp-tessellate
+Version: 1.1.1
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
-License: UNKNOWN
 Keywords: CAD,cadquery
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Provides-Extra: dev
 
 Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs
-
```

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate/__init__.py` & `ocp_tessellate-1.1.1/ocp_tessellate/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate/_version.py` & `ocp_tessellate-1.1.1/ocp_tessellate/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     r = re.compile(
         r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\-{0,1}(?P<release>\D*)(?P<build>\d*)"
     )
     major, minor, patch, release, build = r.match(version).groups()
     return VersionInfo(major, minor, patch, release, build)
 
 
-__version__ = "1.1.0"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "1.1.1"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
```

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate/cad_objects.py` & `ocp_tessellate-1.1.1/ocp_tessellate/cad_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,18 +446,18 @@
         return make_compound(self.compounds())
 
 
 class CoordAxis(OCP_Edges):
     def __init__(self, name, origin, z_dir, size=1):
         o, x, y, z = axis_to_vecs(origin, z_dir)
         edge = line(o, o + size * z)
-        a2 = line(o + size * z, o + size * 0.9 * z - 0.025 * x)
-        a3 = line(o + size * z, o + size * 0.9 * z + 0.025 * x)
-        a4 = line(o + size * z, o + size * 0.9 * z - 0.025 * y)
-        a5 = line(o + size * z, o + size * 0.9 * z + 0.025 * y)
+        a2 = line(o + size * z, o + size * 0.9 * z - size * 0.025 * x)
+        a3 = line(o + size * z, o + size * 0.9 * z + size * 0.025 * x)
+        a4 = line(o + size * z, o + size * 0.9 * z - size * 0.025 * y)
+        a5 = line(o + size * z, o + size * 0.9 * z + size * 0.025 * y)
         # c = circle((o + size * 0.9 * z).Coord(), z_dir, 0.025)
         colors = Color("black")
         super().__init__([edge, a2, a3, a4, a5], name, colors, width=3)
 
 
 class CoordSystem(OCP_Edges):
     def __init__(self, name, origin, x_dir, z_dir, size=1):
```

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate/convert.py` & `ocp_tessellate-1.1.1/ocp_tessellate/convert.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate/defaults.py` & `ocp_tessellate-1.1.1/ocp_tessellate/defaults.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate/mp_tess.py` & `ocp_tessellate-1.1.1/ocp_tessellate/mp_tess.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate/mp_tessellator.py` & `ocp_tessellate-1.1.1/ocp_tessellate/mp_tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate/ocp_utils.py` & `ocp_tessellate-1.1.1/ocp_tessellate/ocp_utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate/stepreader.py` & `ocp_tessellate-1.1.1/ocp_tessellate/stepreader.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate/tessellator.py` & `ocp_tessellate-1.1.1/ocp_tessellate/tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate/utils.py` & `ocp_tessellate-1.1.1/ocp_tessellate/utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate.egg-info/PKG-INFO` & `ocp_tessellate-1.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
-Name: ocp-tessellate
-Version: 1.1.0
+Name: ocp_tessellate
+Version: 1.1.1
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
-License: UNKNOWN
 Keywords: CAD,cadquery
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Provides-Extra: dev
 
 Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs
-
```

### Comparing `ocp_tessellate-1.1.0/ocp_tessellate.egg-info/SOURCES.txt` & `ocp_tessellate-1.1.1/ocp_tessellate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.0/setup.cfg` & `ocp_tessellate-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.0
+current_version = 1.1.1
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_tessellate-1.1.0/setup.py` & `ocp_tessellate-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 LONG_DESCRIPTION = (
     "Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs"
 )
 
 setup_args = {
     "name": "ocp_tessellate",
-    "version": "1.1.0",
+    "version": "1.1.1",
     "description": "Tessellate OCP objects",
     "long_description": LONG_DESCRIPTION,
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "webcolors~=1.12",
         "numpy",
```

