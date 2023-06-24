# Comparing `tmp/even-dist-0.2.6.tar.gz` & `tmp/even-dist-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "even-dist-0.2.6.tar", last modified: Sat Jun 24 01:55:19 2023, max compression
+gzip compressed data, was "even-dist-0.2.7.tar", last modified: Sat Jun 24 01:58:45 2023, max compression
```

## Comparing `even-dist-0.2.6.tar` & `even-dist-0.2.7.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 01:55:19.525645 even-dist-0.2.6/
--rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      400 2023-06-24 01:55:19.524649 even-dist-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 01:55:19.525645 even-dist-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-06-24 01:55:17.000000 even-dist-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 01:55:19.484753 even-dist-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-24 01:55:19.495776 even-dist-0.2.6/src/even_dist/
--rw-rw-rw-   0        0        0       53 2023-06-24 00:32:55.000000 even-dist-0.2.6/src/even_dist/__init__.py
--rw-rw-rw-   0        0        0      713 2023-06-24 00:11:48.000000 even-dist-0.2.6/src/even_dist/even_dist.py
-drwxrwxrwx   0        0        0        0 2023-06-24 01:55:19.521654 even-dist-0.2.6/src/even_dist.egg-info/
--rw-rw-rw-   0        0        0      400 2023-06-24 01:55:19.000000 even-dist-0.2.6/src/even_dist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-06-24 01:55:19.000000 even-dist-0.2.6/src/even_dist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 01:55:19.000000 even-dist-0.2.6/src/even_dist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-24 01:55:19.000000 even-dist-0.2.6/src/even_dist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-24 01:55:19.000000 even-dist-0.2.6/src/even_dist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 01:58:45.960881 even-dist-0.2.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      400 2023-06-24 01:58:45.959884 even-dist-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 01:58:45.960881 even-dist-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      726 2023-06-24 01:58:42.000000 even-dist-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 01:58:45.913738 even-dist-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 01:58:45.924708 even-dist-0.2.7/src/even_dist/
+-rw-rw-rw-   0        0        0       53 2023-06-24 00:32:55.000000 even-dist-0.2.7/src/even_dist/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-06-24 00:11:48.000000 even-dist-0.2.7/src/even_dist/even_dist.py
+drwxrwxrwx   0        0        0        0 2023-06-24 01:58:45.955896 even-dist-0.2.7/src/even_dist.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-06-24 01:58:45.000000 even-dist-0.2.7/src/even_dist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-06-24 01:58:45.000000 even-dist-0.2.7/src/even_dist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 01:58:45.000000 even-dist-0.2.7/src/even_dist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 01:58:45.000000 even-dist-0.2.7/src/even_dist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-24 01:58:45.000000 even-dist-0.2.7/src/even_dist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 01:58:45.957890 even-dist-0.2.7/src/hello/
+-rw-rw-rw-   0        0        0        0 2023-06-24 01:57:38.000000 even-dist-0.2.7/src/hello/__init__.py
```

### Comparing `even-dist-0.2.6/LICENSE` & `even-dist-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `even-dist-0.2.6/setup.py` & `even-dist-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup(
     name="even-dist",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", include=["*"]),
     package_dir={"": "src"},
     include_package_data=True,
-    version="0.2.6",
+    version="0.2.7",
     description="My first Python library",
     install_requires=["numpy", "matplotlib"],
     author="kirp",
     author_email="kirp@umich.edu",
     license="MIT",
     setup_requires=["pytest-runner"],
     test_suite="tests",
```

### Comparing `even-dist-0.2.6/src/even_dist/even_dist.py` & `even-dist-0.2.7/src/even_dist/even_dist.py`

 * *Files identical despite different names*

