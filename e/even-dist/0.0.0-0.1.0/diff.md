# Comparing `tmp/even_dist-0.0.0.tar.gz` & `tmp/even-dist-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "even_dist-0.0.0.tar", last modified: Fri Jun 23 21:04:30 2023, max compression
+gzip compressed data, was "even-dist-0.1.0.tar", last modified: Sat Jun 24 00:24:14 2023, max compression
```

## Comparing `even_dist-0.0.0.tar` & `even-dist-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 21:04:30.442376 even_dist-0.0.0/
--rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even_dist-0.0.0/LICENSE
--rw-rw-rw-   0        0        0       79 2023-06-23 21:04:30.441768 even_dist-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-06-23 19:46:09.000000 even_dist-0.0.0/README.md
--rw-rw-rw-   0        0        0      361 2023-06-23 21:04:18.000000 even_dist-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 21:04:30.442376 even_dist-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 21:04:30.390216 even_dist-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 21:04:30.419206 even_dist-0.0.0/src/even_dist/
--rw-rw-rw-   0        0        0       53 2023-06-23 20:53:09.000000 even_dist-0.0.0/src/even_dist/__init__.py
--rw-rw-rw-   0        0        0      601 2023-06-23 20:55:55.000000 even_dist-0.0.0/src/even_dist/even_dist.py
-drwxrwxrwx   0        0        0        0 2023-06-23 21:04:30.437323 even_dist-0.0.0/src/even_dist.egg-info/
--rw-rw-rw-   0        0        0       79 2023-06-23 21:04:30.000000 even_dist-0.0.0/src/even_dist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-06-23 21:04:30.000000 even_dist-0.0.0/src/even_dist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 21:04:30.000000 even_dist-0.0.0/src/even_dist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-23 21:04:30.000000 even_dist-0.0.0/src/even_dist.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-23 21:04:30.439311 even_dist-0.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-23 21:00:28.000000 even_dist-0.0.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-24 00:24:14.947946 even-dist-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      223 2023-06-24 00:24:14.946951 even-dist-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-06-23 19:46:09.000000 even-dist-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 00:24:14.918027 even-dist-0.1.0/even_dist/
+-rw-rw-rw-   0        0        0       53 2023-06-23 23:59:36.000000 even-dist-0.1.0/even_dist/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-06-24 00:11:48.000000 even-dist-0.1.0/even_dist/even_dist.py
+drwxrwxrwx   0        0        0        0 2023-06-24 00:24:14.943957 even-dist-0.1.0/even_dist.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-06-24 00:24:14.000000 even-dist-0.1.0/even_dist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-24 00:24:14.000000 even-dist-0.1.0/even_dist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 00:24:14.000000 even-dist-0.1.0/even_dist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 00:24:14.000000 even-dist-0.1.0/even_dist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-24 00:24:14.000000 even-dist-0.1.0/even_dist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 00:24:14.947946 even-dist-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      459 2023-06-24 00:24:11.000000 even-dist-0.1.0/setup.py
```

### Comparing `even_dist-0.0.0/LICENSE` & `even-dist-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `even_dist-0.0.0/src/even_dist/even_dist.py` & `even-dist-0.1.0/even_dist/even_dist.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 
 def add_one(number):
     return number + 1
 
 
 def fibo_sphere(n):
+    if type(n) != int:
+        raise TypeError("n must be an integer")
+    if n == 0:
+        return [], [], []
     goldenRatio = (1 + 5**0.5) / 2
     i = arange(0, n)
     theta = 2 * pi * i / goldenRatio
     phi = arccos(1 - 2 * (i + 0.5) / n)
     x, y, z = cos(theta) * sin(phi), sin(theta) * sin(phi), cos(phi)
     return x, y, z
```

