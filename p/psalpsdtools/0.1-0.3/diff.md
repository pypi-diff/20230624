# Comparing `tmp/psalpsdtools-0.1.tar.gz` & `tmp/psalpsdtools-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psalpsdtools-0.1.tar", last modified: Fri Jun 23 02:30:01 2023, max compression
+gzip compressed data, was "psalpsdtools-0.3.tar", last modified: Sat Jun 24 13:26:36 2023, max compression
```

## Comparing `psalpsdtools-0.1.tar` & `psalpsdtools-0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 02:30:01.139533 psalpsdtools-0.1/
--rw-rw-rw-   0        0        0      133 2023-06-23 02:30:01.140531 psalpsdtools-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-23 02:30:01.129569 psalpsdtools-0.1/psalpsdtools/
--rw-rw-rw-   0        0        0     4648 2018-06-19 23:16:08.000000 psalpsdtools-0.1/psalpsdtools/Binomialdistribution.py
--rw-rw-rw-   0        0        0     3631 2018-06-19 23:16:08.000000 psalpsdtools-0.1/psalpsdtools/Gaussiandistribution.py
--rw-rw-rw-   0        0        0      932 2018-06-19 23:16:08.000000 psalpsdtools-0.1/psalpsdtools/Generaldistribution.py
--rw-rw-rw-   0        0        0     2258 2023-06-22 11:00:11.000000 psalpsdtools-0.1/psalpsdtools/ProvincesOfRegions.py
--rw-rw-rw-   0        0        0      125 2023-06-22 10:35:38.000000 psalpsdtools-0.1/psalpsdtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 02:30:01.138536 psalpsdtools-0.1/psalpsdtools.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-23 02:30:00.000000 psalpsdtools-0.1/psalpsdtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-06-23 02:30:00.000000 psalpsdtools-0.1/psalpsdtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 02:30:00.000000 psalpsdtools-0.1/psalpsdtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 02:30:00.000000 psalpsdtools-0.1/psalpsdtools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-23 02:30:00.000000 psalpsdtools-0.1/psalpsdtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 02:30:01.140531 psalpsdtools-0.1/setup.cfg
--rw-rw-rw-   0        0        0      227 2023-06-23 02:23:28.000000 psalpsdtools-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:26:36.011732 psalpsdtools-0.3/
+-rw-rw-rw-   0        0        0      229 2023-06-24 13:26:36.011732 psalpsdtools-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 13:26:36.006177 psalpsdtools-0.3/psalpsdtools/
+-rw-rw-rw-   0        0        0     4648 2018-06-19 23:16:08.000000 psalpsdtools-0.3/psalpsdtools/Binomialdistribution.py
+-rw-rw-rw-   0        0        0     3631 2018-06-19 23:16:08.000000 psalpsdtools-0.3/psalpsdtools/Gaussiandistribution.py
+-rw-rw-rw-   0        0        0      932 2018-06-19 23:16:08.000000 psalpsdtools-0.3/psalpsdtools/Generaldistribution.py
+-rw-rw-rw-   0        0        0     3550 2023-06-24 12:37:30.000000 psalpsdtools-0.3/psalpsdtools/PhilippinesRegions.py
+-rw-rw-rw-   0        0        0     2258 2023-06-22 11:00:11.000000 psalpsdtools-0.3/psalpsdtools/ProvincesOfRegions.py
+-rw-rw-rw-   0        0        0      176 2023-06-24 13:09:33.000000 psalpsdtools-0.3/psalpsdtools/__init__.py
+-rw-rw-rw-   0        0        0      529 2023-06-24 12:19:00.000000 psalpsdtools-0.3/psalpsdtools/test.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:26:36.010726 psalpsdtools-0.3/psalpsdtools.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-06-24 13:26:35.000000 psalpsdtools-0.3/psalpsdtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-06-24 13:26:35.000000 psalpsdtools-0.3/psalpsdtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:26:35.000000 psalpsdtools-0.3/psalpsdtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-24 13:26:35.000000 psalpsdtools-0.3/psalpsdtools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-24 13:26:35.000000 psalpsdtools-0.3/psalpsdtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:26:36.012731 psalpsdtools-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      227 2023-06-24 13:26:12.000000 psalpsdtools-0.3/setup.py
```

### Comparing `psalpsdtools-0.1/psalpsdtools/Binomialdistribution.py` & `psalpsdtools-0.3/psalpsdtools/Binomialdistribution.py`

 * *Files identical despite different names*

### Comparing `psalpsdtools-0.1/psalpsdtools/Gaussiandistribution.py` & `psalpsdtools-0.3/psalpsdtools/Gaussiandistribution.py`

 * *Files identical despite different names*

### Comparing `psalpsdtools-0.1/psalpsdtools/Generaldistribution.py` & `psalpsdtools-0.3/psalpsdtools/Generaldistribution.py`

 * *Files identical despite different names*

### Comparing `psalpsdtools-0.1/psalpsdtools/ProvincesOfRegions.py` & `psalpsdtools-0.3/psalpsdtools/ProvincesOfRegions.py`

 * *Files identical despite different names*

