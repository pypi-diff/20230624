# Comparing `tmp/PyInstl-1.0.2.tar.gz` & `tmp/PyInstl-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyInstl-1.0.2.tar", last modified: Sat Jun 24 16:33:35 2023, max compression
+gzip compressed data, was "PyInstl-1.0.3.tar", last modified: Sat Jun 24 16:39:31 2023, max compression
```

## Comparing `PyInstl-1.0.2.tar` & `PyInstl-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 16:33:35.079960 PyInstl-1.0.2/
--rw-rw-rw-   0        0        0    35823 2023-06-24 16:29:01.000000 PyInstl-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      232 2023-06-24 16:33:35.078967 PyInstl-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 16:33:35.067993 PyInstl-1.0.2/PyInstl/
--rw-rw-rw-   0        0        0     1922 2023-06-24 16:29:01.000000 PyInstl-1.0.2/PyInstl/LoadAnim.py
--rw-rw-rw-   0        0        0     1217 2023-06-24 16:29:01.000000 PyInstl-1.0.2/PyInstl/PyInstl.py
--rw-rw-rw-   0        0        0      164 2023-06-24 16:29:01.000000 PyInstl-1.0.2/PyInstl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 16:33:35.077964 PyInstl-1.0.2/PyInstl.egg-info/
--rw-rw-rw-   0        0        0      232 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-06-24 16:29:01.000000 PyInstl-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 16:33:35.079960 PyInstl-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      559 2023-06-24 16:33:21.000000 PyInstl-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:39:31.463627 PyInstl-1.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-06-24 16:29:01.000000 PyInstl-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      232 2023-06-24 16:39:31.463627 PyInstl-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 16:39:31.451658 PyInstl-1.0.3/PyInstl/
+-rw-rw-rw-   0        0        0     1922 2023-06-24 16:29:01.000000 PyInstl-1.0.3/PyInstl/LoadAnim.py
+-rw-rw-rw-   0        0        0     1217 2023-06-24 16:29:01.000000 PyInstl-1.0.3/PyInstl/PyInstl.py
+-rw-rw-rw-   0        0        0      164 2023-06-24 16:29:01.000000 PyInstl-1.0.3/PyInstl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:39:31.461632 PyInstl-1.0.3/PyInstl.egg-info/
+-rw-rw-rw-   0        0        0      232 2023-06-24 16:39:31.000000 PyInstl-1.0.3/PyInstl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-24 16:39:31.000000 PyInstl-1.0.3/PyInstl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 16:39:31.000000 PyInstl-1.0.3/PyInstl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-24 16:39:31.000000 PyInstl-1.0.3/PyInstl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-06-24 16:39:31.000000 PyInstl-1.0.3/PyInstl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 16:39:31.000000 PyInstl-1.0.3/PyInstl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-06-24 16:29:01.000000 PyInstl-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 16:39:31.463627 PyInstl-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-06-24 16:39:05.000000 PyInstl-1.0.3/setup.py
```

### Comparing `PyInstl-1.0.2/LICENSE` & `PyInstl-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyInstl-1.0.2/PyInstl/LoadAnim.py` & `PyInstl-1.0.3/PyInstl/LoadAnim.py`

 * *Files identical despite different names*

### Comparing `PyInstl-1.0.2/PyInstl/PyInstl.py` & `PyInstl-1.0.3/PyInstl/PyInstl.py`

 * *Files identical despite different names*

### Comparing `PyInstl-1.0.2/setup.py` & `PyInstl-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, find_namespace_packages
 from setuptools import setup
 
 setup(
     name="PyInstl",
-    version="1.0.2",
+    version="1.0.3",
     description="A package installer cli for python",
     author="Muhammed Mehmood",
     author_email="ifreezeu2@gmail.com",
     url="https://github.com/Mo-Xcoder/PyInstl",
     install_requires=["argparse", "pyfiglet", "clint"],
     packages=find_namespace_packages(include=["PyInstl.*"]),
     entry_points={
```

