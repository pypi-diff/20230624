# Comparing `tmp/FluidCubeGame-1.0.5.tar.gz` & `tmp/FluidCubeGame-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidCubeGame-1.0.5.tar", last modified: Sat Jun 24 06:43:22 2023, max compression
+gzip compressed data, was "FluidCubeGame-1.0.6.tar", last modified: Sat Jun 24 06:53:41 2023, max compression
```

## Comparing `FluidCubeGame-1.0.5.tar` & `FluidCubeGame-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:43:22.363051 FluidCubeGame-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:43:22.363051 FluidCubeGame-1.0.5/FluidCubeGame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-24 06:43:22.000000 FluidCubeGame-1.0.5/FluidCubeGame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-24 06:43:22.000000 FluidCubeGame-1.0.5/FluidCubeGame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 06:43:22.000000 FluidCubeGame-1.0.5/FluidCubeGame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 06:43:22.000000 FluidCubeGame-1.0.5/FluidCubeGame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-24 06:43:22.000000 FluidCubeGame-1.0.5/FluidCubeGame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-24 06:43:22.363051 FluidCubeGame-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-24 06:42:11.000000 FluidCubeGame-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 06:43:22.363051 FluidCubeGame-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-24 06:42:11.000000 FluidCubeGame-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:43:22.363051 FluidCubeGame-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:43:22.363051 FluidCubeGame-1.0.5/src/FluidCubeGame/
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-24 06:42:11.000000 FluidCubeGame-1.0.5/src/FluidCubeGame/FluidCubeGame.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-24 06:42:11.000000 FluidCubeGame-1.0.5/src/FluidCubeGame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-24 06:42:11.000000 FluidCubeGame-1.0.5/src/FluidCubeGame/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:53:41.691071 FluidCubeGame-1.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:53:41.691071 FluidCubeGame-1.0.6/FluidCubeGame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-24 06:53:41.000000 FluidCubeGame-1.0.6/FluidCubeGame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-24 06:53:41.000000 FluidCubeGame-1.0.6/FluidCubeGame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 06:53:41.000000 FluidCubeGame-1.0.6/FluidCubeGame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 06:53:41.000000 FluidCubeGame-1.0.6/FluidCubeGame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-24 06:53:41.000000 FluidCubeGame-1.0.6/FluidCubeGame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-24 06:53:41.691071 FluidCubeGame-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-24 06:51:55.000000 FluidCubeGame-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 06:53:41.691071 FluidCubeGame-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-24 06:51:55.000000 FluidCubeGame-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:53:41.691071 FluidCubeGame-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:53:41.691071 FluidCubeGame-1.0.6/src/FluidCubeGame/
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-24 06:51:55.000000 FluidCubeGame-1.0.6/src/FluidCubeGame/FluidCubeGame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-24 06:51:55.000000 FluidCubeGame-1.0.6/src/FluidCubeGame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-24 06:51:55.000000 FluidCubeGame-1.0.6/src/FluidCubeGame/main.py
```

### Comparing `FluidCubeGame-1.0.5/README.md` & `FluidCubeGame-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `FluidCubeGame-1.0.5/src/FluidCubeGame/FluidCubeGame.py` & `FluidCubeGame-1.0.6/src/FluidCubeGame/FluidCubeGame.py`

 * *Files identical despite different names*

### Comparing `FluidCubeGame-1.0.5/src/FluidCubeGame/main.py` & `FluidCubeGame-1.0.6/src/FluidCubeGame/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import FluidCube as fc
+import FluidCubeGame.FluidCubeGame as fc
 import pygame
 import sys
 import cv2
 
 N = fc.N
 SCALE = fc.SCALE
```

