# Comparing `tmp/flet_ivid_hks-1.3.tar.gz` & `tmp/flet_ivid_hks-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_ivid_hks-1.3.tar", last modified: Sat Jun 24 07:58:57 2023, max compression
+gzip compressed data, was "flet_ivid_hks-1.4.tar", last modified: Sat Jun 24 08:19:11 2023, max compression
```

## Comparing `flet_ivid_hks-1.3.tar` & `flet_ivid_hks-1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 07:58:57.756873 flet_ivid_hks-1.3/
--rw-rw-rw-   0        0        0     1081 2023-06-05 11:51:13.000000 flet_ivid_hks-1.3/LICENSE
--rw-rw-rw-   0        0        0       18 2023-06-05 11:51:13.000000 flet_ivid_hks-1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1505 2023-06-24 07:58:57.756873 flet_ivid_hks-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1062 2023-06-08 02:55:17.000000 flet_ivid_hks-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 07:58:57.746874 flet_ivid_hks-1.3/example/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:56:27.000000 flet_ivid_hks-1.3/example/__init__.py
--rw-rw-rw-   0        0        0     1231 2023-06-24 07:54:33.000000 flet_ivid_hks-1.3/example/video_ad.py
--rw-rw-rw-   0        0        0     4070 2023-06-24 07:45:46.000000 flet_ivid_hks-1.3/example/video_grid.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:58:57.749874 flet_ivid_hks-1.3/flet_ivid_hks/
--rw-rw-rw-   0        0        0       45 2023-06-05 11:51:13.000000 flet_ivid_hks-1.3/flet_ivid_hks/__init__.py
--rw-rw-rw-   0        0        0    12897 2023-06-24 07:56:16.000000 flet_ivid_hks-1.3/flet_ivid_hks/clip_container.py
--rw-rw-rw-   0        0        0    12108 2023-06-24 03:23:35.000000 flet_ivid_hks-1.3/flet_ivid_hks/video_container.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:58:57.755874 flet_ivid_hks-1.3/flet_ivid_hks.egg-info/
--rw-rw-rw-   0        0        0     1505 2023-06-24 07:58:57.000000 flet_ivid_hks-1.3/flet_ivid_hks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-06-24 07:58:57.000000 flet_ivid_hks-1.3/flet_ivid_hks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 07:58:57.000000 flet_ivid_hks-1.3/flet_ivid_hks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-24 07:58:57.000000 flet_ivid_hks-1.3/flet_ivid_hks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-24 07:58:57.000000 flet_ivid_hks-1.3/flet_ivid_hks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-05 11:51:13.000000 flet_ivid_hks-1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 07:58:57.757874 flet_ivid_hks-1.3/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-06-24 07:58:50.000000 flet_ivid_hks-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:19:11.644427 flet_ivid_hks-1.4/
+-rw-rw-rw-   0        0        0     1081 2023-06-05 11:51:13.000000 flet_ivid_hks-1.4/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-06-05 11:51:13.000000 flet_ivid_hks-1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1505 2023-06-24 08:19:11.644427 flet_ivid_hks-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1062 2023-06-08 02:55:17.000000 flet_ivid_hks-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 08:19:11.637427 flet_ivid_hks-1.4/example/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:56:27.000000 flet_ivid_hks-1.4/example/__init__.py
+-rw-rw-rw-   0        0        0     1231 2023-06-24 07:54:33.000000 flet_ivid_hks-1.4/example/video_ad.py
+-rw-rw-rw-   0        0        0     4070 2023-06-24 07:45:46.000000 flet_ivid_hks-1.4/example/video_grid.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:19:11.639427 flet_ivid_hks-1.4/flet_ivid_hks/
+-rw-rw-rw-   0        0        0       88 2023-06-24 08:18:50.000000 flet_ivid_hks-1.4/flet_ivid_hks/__init__.py
+-rw-rw-rw-   0        0        0    12897 2023-06-24 07:56:16.000000 flet_ivid_hks-1.4/flet_ivid_hks/clip_container.py
+-rw-rw-rw-   0        0        0    12108 2023-06-24 03:23:35.000000 flet_ivid_hks-1.4/flet_ivid_hks/video_container.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:19:11.643426 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/
+-rw-rw-rw-   0        0        0     1505 2023-06-24 08:19:11.000000 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-06-24 08:19:11.000000 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 08:19:11.000000 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-24 08:19:11.000000 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-24 08:19:11.000000 flet_ivid_hks-1.4/flet_ivid_hks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-05 11:51:13.000000 flet_ivid_hks-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 08:19:11.644427 flet_ivid_hks-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-06-24 08:19:09.000000 flet_ivid_hks-1.4/setup.py
```

### Comparing `flet_ivid_hks-1.3/LICENSE` & `flet_ivid_hks-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.3/PKG-INFO` & `flet_ivid_hks-1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_ivid_hks
-Version: 1.3
+Version: 1.4
 Summary: A package tool that provide basic video player and easy clip for flet.
 Home-page: https://github.com/Uni-Gal/fork-flet_ived
 Author: SKbarbon, Hocassian
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_ivid_hks-1.3/README.md` & `flet_ivid_hks-1.4/README.md`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.3/example/video_ad.py` & `flet_ivid_hks-1.4/example/video_ad.py`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.3/example/video_grid.py` & `flet_ivid_hks-1.4/example/video_grid.py`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.3/flet_ivid_hks/clip_container.py` & `flet_ivid_hks-1.4/flet_ivid_hks/clip_container.py`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.3/flet_ivid_hks/video_container.py` & `flet_ivid_hks-1.4/flet_ivid_hks/video_container.py`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.3/flet_ivid_hks.egg-info/PKG-INFO` & `flet_ivid_hks-1.4/flet_ivid_hks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-ivid-hks
-Version: 1.3
+Version: 1.4
 Summary: A package tool that provide basic video player and easy clip for flet.
 Home-page: https://github.com/Uni-Gal/fork-flet_ived
 Author: SKbarbon, Hocassian
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_ivid_hks-1.3/setup.py` & `flet_ivid_hks-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_des = str(f.read())
 
 setup(
     name='flet_ivid_hks',
-    version='1.3',
+    version='1.4',
     author='SKbarbon, Hocassian',
     description='A package tool that provide basic video player and easy clip for flet.',
     long_description=long_des,
     long_description_content_type='text/markdown',
     url='https://github.com/Uni-Gal/fork-flet_ived',
     install_requires=["flet", "opencv-python"],
     packages=find_packages(),
```

