# Comparing `tmp/free_pygpt-1.3.0.tar.gz` & `tmp/free_pygpt-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "free_pygpt-1.3.0.tar", last modified: Sat Jun 24 20:14:42 2023, max compression
+gzip compressed data, was "free_pygpt-1.3.1.tar", last modified: Sat Jun 24 20:17:32 2023, max compression
```

## Comparing `free_pygpt-1.3.0.tar` & `free_pygpt-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 20:14:42.883284 free_pygpt-1.3.0/
--rw-rw-rw-   0        0        0      426 2023-06-24 20:14:42.884280 free_pygpt-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1065 2023-06-24 20:14:06.000000 free_pygpt-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 20:14:42.817320 free_pygpt-1.3.0/free-gpt/
--rw-rw-rw-   0        0        0      461 2023-06-24 20:14:25.000000 free_pygpt-1.3.0/free-gpt/__init__.py
--rw-rw-rw-   0        0        0      643 2023-06-24 19:43:10.000000 free_pygpt-1.3.0/free-gpt/free_gpt.py
-drwxrwxrwx   0        0        0        0 2023-06-24 20:14:42.879280 free_pygpt-1.3.0/free_pygpt.egg-info/
--rw-rw-rw-   0        0        0      426 2023-06-24 20:14:41.000000 free_pygpt-1.3.0/free_pygpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-06-24 20:14:42.000000 free_pygpt-1.3.0/free_pygpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 20:14:41.000000 free_pygpt-1.3.0/free_pygpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 20:14:41.000000 free_pygpt-1.3.0/free_pygpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 20:14:41.000000 free_pygpt-1.3.0/free_pygpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 20:14:42.886277 free_pygpt-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      747 2023-06-24 20:13:36.000000 free_pygpt-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:17:32.773027 free_pygpt-1.3.1/
+-rw-rw-rw-   0        0        0      426 2023-06-24 20:17:32.774026 free_pygpt-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1065 2023-06-24 20:14:06.000000 free_pygpt-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 20:17:32.704586 free_pygpt-1.3.1/free_pygpt/
+-rw-rw-rw-   0        0        0      461 2023-06-24 20:16:42.000000 free_pygpt-1.3.1/free_pygpt/__init__.py
+-rw-rw-rw-   0        0        0      643 2023-06-24 19:43:10.000000 free_pygpt-1.3.1/free_pygpt/free_pygpt.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:17:32.771030 free_pygpt-1.3.1/free_pygpt.egg-info/
+-rw-rw-rw-   0        0        0      426 2023-06-24 20:17:32.000000 free_pygpt-1.3.1/free_pygpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-24 20:17:32.000000 free_pygpt-1.3.1/free_pygpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 20:17:32.000000 free_pygpt-1.3.1/free_pygpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 20:17:32.000000 free_pygpt-1.3.1/free_pygpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 20:17:32.000000 free_pygpt-1.3.1/free_pygpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 20:17:32.776026 free_pygpt-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      747 2023-06-24 20:17:27.000000 free_pygpt-1.3.1/setup.py
```

### Comparing `free_pygpt-1.3.0/README.md` & `free_pygpt-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `free_pygpt-1.3.0/free-gpt/free_gpt.py` & `free_pygpt-1.3.1/free_pygpt/free_pygpt.py`

 * *Files identical despite different names*

### Comparing `free_pygpt-1.3.0/setup.py` & `free_pygpt-1.3.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 `pip install free_gpt.py`
 ### How Workd"""
 
 setup(
     name="free_pygpt",
     license="MIT",
     author="nxSlayer",
-    version="1.3.0",
+    version="1.3.1",
     author_email="princediscordslay@gmail.com",
     description="Library for use free gpt 3.5 in python",
     url="https://github.com/nxSlayer/free_gpt",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

