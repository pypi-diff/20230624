# Comparing `tmp/FluidCubeGame-1.0.0.tar.gz` & `tmp/FluidCubeGame-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidCubeGame-1.0.0.tar", last modified: Fri Jun 23 18:05:58 2023, max compression
+gzip compressed data, was "FluidCubeGame-1.0.3.tar", last modified: Sat Jun 24 06:19:58 2023, max compression
```

## Comparing `FluidCubeGame-1.0.0.tar` & `FluidCubeGame-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:05:58.866193 FluidCubeGame-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:05:58.862193 FluidCubeGame-1.0.0/FluidCubeGame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-23 18:05:58.000000 FluidCubeGame-1.0.0/FluidCubeGame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-23 18:05:58.000000 FluidCubeGame-1.0.0/FluidCubeGame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:05:58.000000 FluidCubeGame-1.0.0/FluidCubeGame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 18:05:58.000000 FluidCubeGame-1.0.0/FluidCubeGame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 18:05:58.000000 FluidCubeGame-1.0.0/FluidCubeGame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-23 18:05:58.866193 FluidCubeGame-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-23 18:04:10.000000 FluidCubeGame-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:05:58.866193 FluidCubeGame-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-23 18:04:10.000000 FluidCubeGame-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:05:58.866193 FluidCubeGame-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-23 18:04:10.000000 FluidCubeGame-1.0.0/src/FluidCube.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-23 18:04:10.000000 FluidCubeGame-1.0.0/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:19:58.527349 FluidCubeGame-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:19:58.527349 FluidCubeGame-1.0.3/FluidCubeGame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-24 06:19:58.000000 FluidCubeGame-1.0.3/FluidCubeGame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-24 06:19:58.000000 FluidCubeGame-1.0.3/FluidCubeGame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 06:19:58.000000 FluidCubeGame-1.0.3/FluidCubeGame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 06:19:58.000000 FluidCubeGame-1.0.3/FluidCubeGame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-24 06:19:58.000000 FluidCubeGame-1.0.3/FluidCubeGame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-24 06:19:58.527349 FluidCubeGame-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-24 06:18:40.000000 FluidCubeGame-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 06:19:58.527349 FluidCubeGame-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-24 06:18:40.000000 FluidCubeGame-1.0.3/setup.py
```

### Comparing `FluidCubeGame-1.0.0/README.md` & `FluidCubeGame-1.0.3/README.md`

 * *Files identical despite different names*

