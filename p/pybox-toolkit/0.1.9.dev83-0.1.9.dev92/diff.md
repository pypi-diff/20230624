# Comparing `tmp/pybox-toolkit-0.1.9.dev83.tar.gz` & `tmp/pybox-toolkit-0.1.9.dev92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybox-toolkit-0.1.9.dev83.tar", last modified: Fri Jun 23 11:53:44 2023, max compression
+gzip compressed data, was "pybox-toolkit-0.1.9.dev92.tar", last modified: Sat Jun 24 17:24:57 2023, max compression
```

## Comparing `pybox-toolkit-0.1.9.dev83.tar` & `pybox-toolkit-0.1.9.dev92.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.221078 pybox-toolkit-0.1.9.dev83/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-23 11:53:44.221078 pybox-toolkit-0.1.9.dev83/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev83/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev83/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 11:53:44.221078 pybox-toolkit-0.1.9.dev83/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.213078 pybox-toolkit-0.1.9.dev83/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.217078 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-23 11:53:44.000000 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-06-23 11:53:44.000000 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 11:53:44.000000 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-23 11:53:44.000000 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-23 11:53:44.000000 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.217078 pybox-toolkit-0.1.9.dev83/src/toolkit/
--rw-rw-rw-   0 root         (0) root         (0)    15423 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.217078 pybox-toolkit-0.1.9.dev83/src/toolkit/graphing/
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/graphing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 11:53:07.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.221078 pybox-toolkit-0.1.9.dev83/src/toolkit/test/
--rw-rw-rw-   0 root         (0) root         (0)     5113 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.221078 pybox-toolkit-0.1.9.dev83/src/toolkit/typing/
--rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/typing/si.py
--rw-rw-rw-   0 root         (0) root         (0)     8004 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-06-23 09:39:42.000000 pybox-toolkit-0.1.9.dev92/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-23 09:39:42.000000 pybox-toolkit-0.1.9.dev92/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.404097 pybox-toolkit-0.1.9.dev92/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-24 17:24:57.000000 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-24 17:24:57.000000 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 17:24:57.000000 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-24 17:24:57.000000 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-24 17:24:57.000000 pybox-toolkit-0.1.9.dev92/src/pybox_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/src/toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)    15423 2023-06-23 09:39:42.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/src/toolkit/graphing/
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-05 18:07:33.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/graphing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-24 17:24:33.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/src/toolkit/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5185 2023-06-24 15:29:00.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:24:57.408097 pybox-toolkit-0.1.9.dev92/src/toolkit/typing/
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-05 19:32:07.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-31 11:15:50.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/typing/si.py
+-rw-rw-rw-   0 root         (0) root         (0)     8004 2023-06-23 09:39:42.000000 pybox-toolkit-0.1.9.dev92/src/toolkit/utils.py
```

### Comparing `pybox-toolkit-0.1.9.dev83/pyproject.toml` & `pybox-toolkit-0.1.9.dev92/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev83/src/toolkit/__init__.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev83/src/toolkit/graphing/__init__.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/graphing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev83/src/toolkit/test/__init__.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/test/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """Testing framework for formula scripts"""
 
 from __future__ import annotations
 
 import unittest
+from math import isclose
 from sys import stdout
 from typing import TYPE_CHECKING, Any, Callable, TextIO, Union
 from unittest import TestResult
 
 from toolkit.utils import TestingException
 
 if TYPE_CHECKING:
     from toolkit import BaseFormula
 
 
-def compare_floats(first: float, second: float, epsilon: float = 0.00001) -> bool:
+def compare_floats(first: float, second: float, epsilon: float = 0.00001, rel_tol = 0.05) -> bool:
     """Compares two floats using an epsilon
 
     Args:
         first (float): first float
         second (float): second float
         epsilon (float): comparison epsilon
 
     Returns:
         bool: whether the floats are equal or not under epsilon
     """
-    return abs(first - second) < epsilon
+    return isclose(first, second, rel_tol = rel_tol, abs_tol = epsilon)
 
 
 def compare_dics(first: dict[str, float], second: dict[str, float]) -> bool:
     """Compares two dictionaries to check if they're equal in terms of floats
 
     Args:
         first (dict[str, float]): first dictionary
```

### Comparing `pybox-toolkit-0.1.9.dev83/src/toolkit/typing/__init__.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev83/src/toolkit/typing/si.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/typing/si.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev83/src/toolkit/utils.py` & `pybox-toolkit-0.1.9.dev92/src/toolkit/utils.py`

 * *Files identical despite different names*

