# Comparing `tmp/PyInstl-1.0.1.tar.gz` & `tmp/PyInstl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyInstl-1.0.1.tar", last modified: Mon Jun 27 19:32:33 2022, max compression
+gzip compressed data, was "PyInstl-1.0.2.tar", last modified: Sat Jun 24 16:33:35 2023, max compression
```

## Comparing `PyInstl-1.0.1.tar` & `PyInstl-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-06-27 19:32:33.958534 PyInstl-1.0.1/
--rw-rw-rw-   0        0        0      259 2022-06-27 19:32:33.959538 PyInstl-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-06-27 19:32:33.941533 PyInstl-1.0.1/PyInstl/
--rw-rw-rw-   0        0        0     1922 2021-10-28 14:01:33.000000 PyInstl-1.0.1/PyInstl/LoadAnim.py
--rw-rw-rw-   0        0        0     3117 2022-06-27 19:24:47.000000 PyInstl-1.0.1/PyInstl/PyInstl.py
--rw-rw-rw-   0        0        0      147 2022-06-27 19:27:28.000000 PyInstl-1.0.1/PyInstl/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-27 19:32:33.957534 PyInstl-1.0.1/PyInstl.egg-info/
--rw-rw-rw-   0        0        0      259 2022-06-27 19:32:33.000000 PyInstl-1.0.1/PyInstl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2022-06-27 19:32:33.000000 PyInstl-1.0.1/PyInstl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-27 19:32:33.000000 PyInstl-1.0.1/PyInstl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2022-06-27 19:32:33.000000 PyInstl-1.0.1/PyInstl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2022-06-27 19:32:33.000000 PyInstl-1.0.1/PyInstl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-27 19:32:33.962533 PyInstl-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      444 2022-06-27 19:32:29.000000 PyInstl-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:33:35.079960 PyInstl-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-06-24 16:29:01.000000 PyInstl-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      232 2023-06-24 16:33:35.078967 PyInstl-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 16:33:35.067993 PyInstl-1.0.2/PyInstl/
+-rw-rw-rw-   0        0        0     1922 2023-06-24 16:29:01.000000 PyInstl-1.0.2/PyInstl/LoadAnim.py
+-rw-rw-rw-   0        0        0     1217 2023-06-24 16:29:01.000000 PyInstl-1.0.2/PyInstl/PyInstl.py
+-rw-rw-rw-   0        0        0      164 2023-06-24 16:29:01.000000 PyInstl-1.0.2/PyInstl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:33:35.077964 PyInstl-1.0.2/PyInstl.egg-info/
+-rw-rw-rw-   0        0        0      232 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 16:33:35.000000 PyInstl-1.0.2/PyInstl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-06-24 16:29:01.000000 PyInstl-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 16:33:35.079960 PyInstl-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-06-24 16:33:21.000000 PyInstl-1.0.2/setup.py
```

### Comparing `PyInstl-1.0.1/PyInstl/LoadAnim.py` & `PyInstl-1.0.2/PyInstl/LoadAnim.py`

 * *Files identical despite different names*

