# Comparing `tmp/fcutil-0.0.1.tar.gz` & `tmp/fcutil-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcutil-0.0.1.tar", last modified: Wed Jun 21 15:52:45 2023, max compression
+gzip compressed data, was "fcutil-0.0.2.tar", last modified: Sat Jun 24 09:23:08 2023, max compression
```

## Comparing `fcutil-0.0.1.tar` & `fcutil-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 15:52:45.292934 fcutil-0.0.1/
--rw-rw-rw-   0        0        0      150 2023-06-21 15:52:45.291384 fcutil-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-21 15:52:45.293938 fcutil-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      466 2023-06-21 15:25:12.000000 fcutil-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 15:52:45.193126 fcutil-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 15:52:45.287697 fcutil-0.0.1/src/fcutil.egg-info/
--rw-rw-rw-   0        0        0      150 2023-06-21 15:52:44.000000 fcutil-0.0.1/src/fcutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      144 2023-06-21 15:52:45.000000 fcutil-0.0.1/src/fcutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 15:52:44.000000 fcutil-0.0.1/src/fcutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 15:52:44.000000 fcutil-0.0.1/src/fcutil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 09:23:08.566767 fcutil-0.0.2/
+-rw-rw-rw-   0        0        0      150 2023-06-24 09:23:08.566767 fcutil-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-24 09:23:08.566767 fcutil-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      466 2023-06-24 09:21:18.000000 fcutil-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:23:08.551143 fcutil-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 09:23:08.551143 fcutil-0.0.2/src/fcutil/
+-rw-rw-rw-   0        0        0        0 2023-06-24 09:17:18.000000 fcutil-0.0.2/src/fcutil/__init__.py
+-rw-rw-rw-   0        0        0      535 2023-06-24 09:17:18.000000 fcutil-0.0.2/src/fcutil/fuProfiler.py
+-rw-rw-rw-   0        0        0      530 2023-06-24 09:17:18.000000 fcutil-0.0.2/src/fcutil/searchList.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:23:08.566767 fcutil-0.0.2/src/fcutil.egg-info/
+-rw-rw-rw-   0        0        0      150 2023-06-24 09:23:08.000000 fcutil-0.0.2/src/fcutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-06-24 09:23:08.000000 fcutil-0.0.2/src/fcutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 09:23:08.000000 fcutil-0.0.2/src/fcutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 09:23:08.000000 fcutil-0.0.2/src/fcutil.egg-info/top_level.txt
```

