# Comparing `tmp/ocp_vscode-1.1.2.tar.gz` & `tmp/ocp_vscode-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-1.1.2.tar", last modified: Wed Jun 21 19:02:24 2023, max compression
+gzip compressed data, was "ocp_vscode-1.1.3.tar", last modified: Sat Jun 24 13:20:12 2023, max compression
```

## Comparing `ocp_vscode-1.1.2.tar` & `ocp_vscode-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-21 19:02:24.718201 ocp_vscode-1.1.2/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-1.1.2/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-21 19:02:24.718261 ocp_vscode-1.1.2/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)     5588 2023-06-21 18:27:01.000000 ocp_vscode-1.1.2/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-21 19:02:24.716998 ocp_vscode-1.1.2/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)      702 2023-06-17 10:13:52.000000 ocp_vscode-1.1.2/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4759 2023-06-17 10:13:52.000000 ocp_vscode-1.1.2/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)    18168 2023-06-19 07:30:58.000000 ocp_vscode-1.1.2/ocp_vscode/colors.py
--rw-r--r--   0 bernhard   (501) staff       (20)     2800 2023-06-17 10:13:52.000000 ocp_vscode-1.1.2/ocp_vscode/comms.py
--rw-r--r--   0 bernhard   (501) staff       (20)     9869 2023-06-17 10:13:52.000000 ocp_vscode-1.1.2/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4409 2023-06-17 10:13:52.000000 ocp_vscode-1.1.2/ocp_vscode/finder.py
--rw-r--r--   0 bernhard   (501) staff       (20)    24578 2023-06-19 06:30:51.000000 ocp_vscode-1.1.2/ocp_vscode/show.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-21 19:02:24.718079 ocp_vscode-1.1.2/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-21 19:02:24.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      387 2023-06-21 19:02:24.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-21 19:02:24.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-21 18:25:16.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       78 2023-06-21 19:02:24.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-06-21 19:02:24.000000 ocp_vscode-1.1.2/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-06-21 19:02:24.718533 ocp_vscode-1.1.2/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1229 2023-06-21 18:17:17.000000 ocp_vscode-1.1.2/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:20:12.407458 ocp_vscode-1.1.3/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2023-04-23 10:16:29.000000 ocp_vscode-1.1.3/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-24 13:20:12.407521 ocp_vscode-1.1.3/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)     8749 2023-06-24 13:08:20.000000 ocp_vscode-1.1.3/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:20:12.406628 ocp_vscode-1.1.3/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)      702 2023-06-07 07:17:54.000000 ocp_vscode-1.1.3/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4759 2023-06-07 07:17:54.000000 ocp_vscode-1.1.3/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    18168 2023-06-19 20:31:17.000000 ocp_vscode-1.1.3/ocp_vscode/colors.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     2800 2023-06-07 07:17:54.000000 ocp_vscode-1.1.3/ocp_vscode/comms.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     9869 2023-06-16 06:38:23.000000 ocp_vscode-1.1.3/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4409 2023-06-08 06:20:47.000000 ocp_vscode-1.1.3/ocp_vscode/finder.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    24578 2023-06-19 20:31:17.000000 ocp_vscode-1.1.3/ocp_vscode/show.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:20:12.407345 ocp_vscode-1.1.3/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      387 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       78 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-06-24 13:20:12.407790 ocp_vscode-1.1.3/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1229 2023-06-24 13:07:12.000000 ocp_vscode-1.1.3/setup.py
```

### Comparing `ocp_vscode-1.1.2/LICENSE` & `ocp_vscode-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.2/PKG-INFO` & `ocp_vscode-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 1.1.2
+Version: 1.1.3
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.1.2/ocp_vscode/__init__.py` & `ocp_vscode-1.1.3/ocp_vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.2/ocp_vscode/animation.py` & `ocp_vscode-1.1.3/ocp_vscode/animation.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.2/ocp_vscode/colors.py` & `ocp_vscode-1.1.3/ocp_vscode/colors.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.2/ocp_vscode/comms.py` & `ocp_vscode-1.1.3/ocp_vscode/comms.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.2/ocp_vscode/config.py` & `ocp_vscode-1.1.3/ocp_vscode/config.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.2/ocp_vscode/finder.py` & `ocp_vscode-1.1.3/ocp_vscode/finder.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.2/ocp_vscode/show.py` & `ocp_vscode-1.1.3/ocp_vscode/show.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.2/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-1.1.3/ocp_vscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-vscode
-Version: 1.1.2
+Version: 1.1.3
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.1.2/setup.cfg` & `ocp_vscode-1.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.2
+current_version = 1.1.3
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-1.1.2/setup.py` & `ocp_vscode-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "1.1.2",
+    "version": "1.1.3",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via pythreejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
-        "ocp-tessellate>=1.1.0,<1.2.0",
+        "ocp-tessellate>=1.1.1,<1.2.0",
         "requests",
         "ipykernel",
         "orjson",
         "websockets>=11.0,<11.1",
     ],
     "packages": find_packages(),
     "zip_safe": False,
```

