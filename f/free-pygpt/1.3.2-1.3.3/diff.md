# Comparing `tmp/free_pygpt-1.3.2.tar.gz` & `tmp/free_pygpt-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "free_pygpt-1.3.2.tar", last modified: Sat Jun 24 20:26:26 2023, max compression
+gzip compressed data, was "free_pygpt-1.3.3.tar", last modified: Sat Jun 24 20:40:54 2023, max compression
```

## Comparing `free_pygpt-1.3.2.tar` & `free_pygpt-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 20:26:26.367969 free_pygpt-1.3.2/
--rw-rw-rw-   0        0        0      426 2023-06-24 20:26:26.367969 free_pygpt-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1065 2023-06-24 20:14:06.000000 free_pygpt-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 20:26:26.345982 free_pygpt-1.3.2/free_pygpt/
--rw-rw-rw-   0        0        0      493 2023-06-24 20:26:08.000000 free_pygpt-1.3.2/free_pygpt/__init__.py
--rw-rw-rw-   0        0        0      643 2023-06-24 19:43:10.000000 free_pygpt-1.3.2/free_pygpt/free_pygpt.py
-drwxrwxrwx   0        0        0        0 2023-06-24 20:26:26.365972 free_pygpt-1.3.2/free_pygpt.egg-info/
--rw-rw-rw-   0        0        0      426 2023-06-24 20:26:25.000000 free_pygpt-1.3.2/free_pygpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-24 20:26:26.000000 free_pygpt-1.3.2/free_pygpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 20:26:25.000000 free_pygpt-1.3.2/free_pygpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 20:26:25.000000 free_pygpt-1.3.2/free_pygpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 20:26:25.000000 free_pygpt-1.3.2/free_pygpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 20:26:26.369969 free_pygpt-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      747 2023-06-24 20:26:17.000000 free_pygpt-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:40:54.337166 free_pygpt-1.3.3/
+-rw-rw-rw-   0        0        0      426 2023-06-24 20:40:54.337166 free_pygpt-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1065 2023-06-24 20:14:06.000000 free_pygpt-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 20:40:54.317566 free_pygpt-1.3.3/free_pygpt/
+-rw-rw-rw-   0        0        0      494 2023-06-24 20:40:02.000000 free_pygpt-1.3.3/free_pygpt/__init__.py
+-rw-rw-rw-   0        0        0      643 2023-06-24 19:43:10.000000 free_pygpt-1.3.3/free_pygpt/free_pygpt.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:40:54.335167 free_pygpt-1.3.3/free_pygpt.egg-info/
+-rw-rw-rw-   0        0        0      426 2023-06-24 20:40:53.000000 free_pygpt-1.3.3/free_pygpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-24 20:40:54.000000 free_pygpt-1.3.3/free_pygpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 20:40:53.000000 free_pygpt-1.3.3/free_pygpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 20:40:53.000000 free_pygpt-1.3.3/free_pygpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 20:40:53.000000 free_pygpt-1.3.3/free_pygpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 20:40:54.339165 free_pygpt-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      747 2023-06-24 20:40:31.000000 free_pygpt-1.3.3/setup.py
```

### Comparing `free_pygpt-1.3.2/README.md` & `free_pygpt-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `free_pygpt-1.3.2/free_pygpt/free_pygpt.py` & `free_pygpt-1.3.3/free_pygpt/free_pygpt.py`

 * *Files identical despite different names*

### Comparing `free_pygpt-1.3.2/setup.py` & `free_pygpt-1.3.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 `pip install free_gpt.py`
 ### How Workd"""
 
 setup(
     name="free_pygpt",
     license="MIT",
     author="nxSlayer",
-    version="1.3.2",
+    version="1.3.3",
     author_email="princediscordslay@gmail.com",
     description="Library for use free gpt 3.5 in python",
     url="https://github.com/nxSlayer/free_gpt",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

