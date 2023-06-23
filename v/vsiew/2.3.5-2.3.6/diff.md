# Comparing `tmp/vsiew-2.3.5.tar.gz` & `tmp/vsiew-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsiew-2.3.5.tar", last modified: Tue Jun 20 23:06:58 2023, max compression
+gzip compressed data, was "vsiew-2.3.6.tar", last modified: Fri Jun 23 22:50:03 2023, max compression
```

## Comparing `vsiew-2.3.5.tar` & `vsiew-2.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:06:58.292692 vsiew-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 23:06:32.000000 vsiew-2.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 23:06:58.292692 vsiew-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 23:06:32.000000 vsiew-2.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:06:58.292692 vsiew-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-20 23:06:32.000000 vsiew-2.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:06:58.288692 vsiew-2.3.5/vsiew/
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-20 23:06:32.000000 vsiew-2.3.5/vsiew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 23:06:32.000000 vsiew-2.3.5/vsiew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 23:06:32.000000 vsiew-2.3.5/vsiew/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-20 23:06:32.000000 vsiew-2.3.5/vsiew/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:06:58.288692 vsiew-2.3.5/vsiew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:06:58.000000 vsiew-2.3.5/vsiew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:50:03.338345 vsiew-2.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 22:49:38.000000 vsiew-2.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-23 22:50:03.338345 vsiew-2.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-23 22:49:38.000000 vsiew-2.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 22:50:03.338345 vsiew-2.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-23 22:49:38.000000 vsiew-2.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:50:03.334345 vsiew-2.3.6/vsiew/
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-23 22:49:38.000000 vsiew-2.3.6/vsiew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 22:49:38.000000 vsiew-2.3.6/vsiew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-23 22:49:38.000000 vsiew-2.3.6/vsiew/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-23 22:49:38.000000 vsiew-2.3.6/vsiew/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:50:03.338345 vsiew-2.3.6/vsiew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 22:50:03.000000 vsiew-2.3.6/vsiew.egg-info/top_level.txt
```

### Comparing `vsiew-2.3.5/LICENSE` & `vsiew-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.5/PKG-INFO` & `vsiew-2.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.5
+Version: 2.3.6
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

### Comparing `vsiew-2.3.5/setup.py` & `vsiew-2.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.5/vsiew/__init__.py` & `vsiew-2.3.6/vsiew/__init__.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.5/vsiew/init.py` & `vsiew-2.3.6/vsiew/init.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.5/vsiew.egg-info/PKG-INFO` & `vsiew-2.3.6/vsiew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.5
+Version: 2.3.6
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

