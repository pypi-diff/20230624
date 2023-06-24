# Comparing `tmp/Optimo API Testing-1.0.0.tar.gz` & `tmp/Optimo API Testing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Optimo API Testing-1.0.0.tar", last modified: Thu Jun 22 22:58:59 2023, max compression
+gzip compressed data, was "Optimo API Testing-1.0.1.tar", last modified: Sat Jun 24 13:04:08 2023, max compression
```

## Comparing `Optimo API Testing-1.0.0.tar` & `Optimo API Testing-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 ambri     (1000) ambri     (1000)        0 2023-06-22 22:58:59.005260 Optimo API Testing-1.0.0/
-drwxr-xr-x   0 ambri     (1000) ambri     (1000)        0 2023-06-22 22:58:59.001260 Optimo API Testing-1.0.0/Optimo/
--rw-r--r--   0 ambri     (1000) ambri     (1000)        0 2023-06-22 21:48:13.000000 Optimo API Testing-1.0.0/Optimo/__init__.py
-drwxr-xr-x   0 ambri     (1000) ambri     (1000)        0 2023-06-22 22:58:59.005260 Optimo API Testing-1.0.0/Optimo_API_Testing.egg-info/
--rw-r--r--   0 ambri     (1000) ambri     (1000)      227 2023-06-22 22:58:58.000000 Optimo API Testing-1.0.0/Optimo_API_Testing.egg-info/PKG-INFO
--rw-r--r--   0 ambri     (1000) ambri     (1000)      236 2023-06-22 22:58:58.000000 Optimo API Testing-1.0.0/Optimo_API_Testing.egg-info/SOURCES.txt
--rw-r--r--   0 ambri     (1000) ambri     (1000)        1 2023-06-22 22:58:58.000000 Optimo API Testing-1.0.0/Optimo_API_Testing.egg-info/dependency_links.txt
--rw-r--r--   0 ambri     (1000) ambri     (1000)      619 2023-06-22 22:58:58.000000 Optimo API Testing-1.0.0/Optimo_API_Testing.egg-info/requires.txt
--rw-r--r--   0 ambri     (1000) ambri     (1000)        7 2023-06-22 22:58:58.000000 Optimo API Testing-1.0.0/Optimo_API_Testing.egg-info/top_level.txt
--rw-r--r--   0 ambri     (1000) ambri     (1000)      227 2023-06-22 22:58:59.005260 Optimo API Testing-1.0.0/PKG-INFO
--rw-r--r--   0 ambri     (1000) ambri     (1000)       38 2023-06-22 22:58:59.005260 Optimo API Testing-1.0.0/setup.cfg
--rw-r--r--   0 ambri     (1000) ambri     (1000)      350 2023-06-22 22:58:58.000000 Optimo API Testing-1.0.0/setup.py
+drwxr-xr-x   0 ambri     (1000) ambri     (1000)        0 2023-06-24 13:04:08.185367 Optimo API Testing-1.0.1/
+drwxr-xr-x   0 ambri     (1000) ambri     (1000)        0 2023-06-24 13:04:08.185367 Optimo API Testing-1.0.1/Optimo/
+-rw-r--r--   0 ambri     (1000) ambri     (1000)        0 2023-06-22 21:48:13.000000 Optimo API Testing-1.0.1/Optimo/__init__.py
+drwxr-xr-x   0 ambri     (1000) ambri     (1000)        0 2023-06-24 13:04:08.185367 Optimo API Testing-1.0.1/Optimo_API_Testing.egg-info/
+-rw-r--r--   0 ambri     (1000) ambri     (1000)      227 2023-06-24 13:04:08.000000 Optimo API Testing-1.0.1/Optimo_API_Testing.egg-info/PKG-INFO
+-rw-r--r--   0 ambri     (1000) ambri     (1000)      307 2023-06-24 13:04:08.000000 Optimo API Testing-1.0.1/Optimo_API_Testing.egg-info/SOURCES.txt
+-rw-r--r--   0 ambri     (1000) ambri     (1000)        1 2023-06-24 13:04:08.000000 Optimo API Testing-1.0.1/Optimo_API_Testing.egg-info/dependency_links.txt
+-rw-r--r--   0 ambri     (1000) ambri     (1000)     1127 2023-06-24 13:04:08.000000 Optimo API Testing-1.0.1/Optimo_API_Testing.egg-info/requires.txt
+-rw-r--r--   0 ambri     (1000) ambri     (1000)       31 2023-06-24 13:04:08.000000 Optimo API Testing-1.0.1/Optimo_API_Testing.egg-info/top_level.txt
+drwxr-xr-x   0 ambri     (1000) ambri     (1000)        0 2023-06-24 13:04:08.185367 Optimo API Testing-1.0.1/Optimo_Instance_Manager/
+-rw-r--r--   0 ambri     (1000) ambri     (1000)        0 2023-06-23 14:56:24.000000 Optimo API Testing-1.0.1/Optimo_Instance_Manager/__init__.py
+-rw-r--r--   0 ambri     (1000) ambri     (1000)     3037 2023-06-24 12:51:44.000000 Optimo API Testing-1.0.1/Optimo_Instance_Manager/manager.py
+-rw-r--r--   0 ambri     (1000) ambri     (1000)      227 2023-06-24 13:04:08.185367 Optimo API Testing-1.0.1/PKG-INFO
+-rw-r--r--   0 ambri     (1000) ambri     (1000)       38 2023-06-24 13:04:08.185367 Optimo API Testing-1.0.1/setup.cfg
+-rw-r--r--   0 ambri     (1000) ambri     (1000)      376 2023-06-24 13:04:00.000000 Optimo API Testing-1.0.1/setup.py
```

