# Comparing `tmp/pythoncryptographypackage-1.0.0.tar.gz` & `tmp/pythoncryptographypackage-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncryptographypackage-1.0.0.tar", last modified: Fri Jun 23 23:01:06 2023, max compression
+gzip compressed data, was "pythoncryptographypackage-1.1.0.tar", last modified: Fri Jun 23 23:03:13 2023, max compression
```

## Comparing `pythoncryptographypackage-1.0.0.tar` & `pythoncryptographypackage-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:06.748491 pythoncryptographypackage-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-23 23:01:06.748491 pythoncryptographypackage-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:06.744491 pythoncryptographypackage-1.0.0/pythoncryptographypackage/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-23 23:01:06.000000 pythoncryptographypackage-1.0.0/pythoncryptographypackage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:06.744491 pythoncryptographypackage-1.0.0/pythoncryptographypackage.egg-info/
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-23 23:01:06.000000 pythoncryptographypackage-1.0.0/pythoncryptographypackage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-23 23:01:06.000000 pythoncryptographypackage-1.0.0/pythoncryptographypackage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 23:01:06.000000 pythoncryptographypackage-1.0.0/pythoncryptographypackage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-23 23:01:06.000000 pythoncryptographypackage-1.0.0/pythoncryptographypackage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 23:01:06.748491 pythoncryptographypackage-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      571 2023-06-23 23:01:06.000000 pythoncryptographypackage-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:03:13.228120 pythoncryptographypackage-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-23 23:03:13.228120 pythoncryptographypackage-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:03:13.228120 pythoncryptographypackage-1.1.0/pythoncryptographypackage/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-06-23 23:03:12.000000 pythoncryptographypackage-1.1.0/pythoncryptographypackage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:03:13.228120 pythoncryptographypackage-1.1.0/pythoncryptographypackage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-23 23:03:13.000000 pythoncryptographypackage-1.1.0/pythoncryptographypackage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-23 23:03:13.000000 pythoncryptographypackage-1.1.0/pythoncryptographypackage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 23:03:13.000000 pythoncryptographypackage-1.1.0/pythoncryptographypackage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-23 23:03:13.000000 pythoncryptographypackage-1.1.0/pythoncryptographypackage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 23:03:13.228120 pythoncryptographypackage-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      571 2023-06-23 23:03:12.000000 pythoncryptographypackage-1.1.0/setup.py
```

### Comparing `pythoncryptographypackage-1.0.0/setup.py` & `pythoncryptographypackage-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythoncryptographypackage",
     version=VERSION,
```

