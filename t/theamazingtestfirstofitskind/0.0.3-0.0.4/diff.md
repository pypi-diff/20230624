# Comparing `tmp/theamazingtestfirstofitskind-0.0.3.tar.gz` & `tmp/theamazingtestfirstofitskind-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theamazingtestfirstofitskind-0.0.3.tar", last modified: Tue Jun 20 13:00:38 2023, max compression
+gzip compressed data, was "theamazingtestfirstofitskind-0.0.4.tar", last modified: Sat Jun 24 17:11:49 2023, max compression
```

## Comparing `theamazingtestfirstofitskind-0.0.3.tar` & `theamazingtestfirstofitskind-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:00:38.779417 theamazingtestfirstofitskind-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-20 13:00:38.779417 theamazingtestfirstofitskind-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:00:38.779417 theamazingtestfirstofitskind-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-20 13:00:26.000000 theamazingtestfirstofitskind-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:00:38.779417 theamazingtestfirstofitskind-0.0.3/testops/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 13:00:26.000000 theamazingtestfirstofitskind-0.0.3/testops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 13:00:26.000000 theamazingtestfirstofitskind-0.0.3/testops/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:00:38.779417 theamazingtestfirstofitskind-0.0.3/theamazingtestfirstofitskind.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-20 13:00:38.000000 theamazingtestfirstofitskind-0.0.3/theamazingtestfirstofitskind.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-20 13:00:38.000000 theamazingtestfirstofitskind-0.0.3/theamazingtestfirstofitskind.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:00:38.000000 theamazingtestfirstofitskind-0.0.3/theamazingtestfirstofitskind.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 13:00:38.000000 theamazingtestfirstofitskind-0.0.3/theamazingtestfirstofitskind.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:11:49.744360 theamazingtestfirstofitskind-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-24 17:11:49.744360 theamazingtestfirstofitskind-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 17:11:49.744360 theamazingtestfirstofitskind-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-24 17:11:38.000000 theamazingtestfirstofitskind-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:11:49.744360 theamazingtestfirstofitskind-0.0.4/testops/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-24 17:11:38.000000 theamazingtestfirstofitskind-0.0.4/testops/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-24 17:11:38.000000 theamazingtestfirstofitskind-0.0.4/testops/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:11:49.744360 theamazingtestfirstofitskind-0.0.4/theamazingtestfirstofitskind.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-24 17:11:49.000000 theamazingtestfirstofitskind-0.0.4/theamazingtestfirstofitskind.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-24 17:11:49.000000 theamazingtestfirstofitskind-0.0.4/theamazingtestfirstofitskind.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 17:11:49.000000 theamazingtestfirstofitskind-0.0.4/theamazingtestfirstofitskind.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-24 17:11:49.000000 theamazingtestfirstofitskind-0.0.4/theamazingtestfirstofitskind.egg-info/top_level.txt
```

### Comparing `theamazingtestfirstofitskind-0.0.3/setup.py` & `theamazingtestfirstofitskind-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'basic test2'
 LONG_DESCRIPTION = 'second dev test'
 
 # Setting up
 setup(
     name="theamazingtestfirstofitskind",
     version=VERSION,
```

