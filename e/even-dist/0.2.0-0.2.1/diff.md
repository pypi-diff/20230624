# Comparing `tmp/even-dist-0.2.0.tar.gz` & `tmp/even-dist-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "even-dist-0.2.0.tar", last modified: Sat Jun 24 00:42:28 2023, max compression
+gzip compressed data, was "even-dist-0.2.1.tar", last modified: Sat Jun 24 01:10:40 2023, max compression
```

## Comparing `even-dist-0.2.0.tar` & `even-dist-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 00:42:28.336348 even-dist-0.2.0/
--rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      400 2023-06-24 00:42:28.335342 even-dist-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 00:42:28.319385 even-dist-0.2.0/even_dist/
--rw-rw-rw-   0        0        0       53 2023-06-24 00:32:55.000000 even-dist-0.2.0/even_dist/__init__.py
--rw-rw-rw-   0        0        0      713 2023-06-24 00:11:48.000000 even-dist-0.2.0/even_dist/even_dist.py
-drwxrwxrwx   0        0        0        0 2023-06-24 00:42:28.333348 even-dist-0.2.0/even_dist.egg-info/
--rw-rw-rw-   0        0        0      400 2023-06-24 00:42:28.000000 even-dist-0.2.0/even_dist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-24 00:42:28.000000 even-dist-0.2.0/even_dist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 00:42:28.000000 even-dist-0.2.0/even_dist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-24 00:42:28.000000 even-dist-0.2.0/even_dist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-24 00:42:28.000000 even-dist-0.2.0/even_dist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 00:42:28.337337 even-dist-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      732 2023-06-24 00:41:26.000000 even-dist-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 01:10:40.622364 even-dist-0.2.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      400 2023-06-24 01:10:40.621774 even-dist-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 01:10:40.619373 even-dist-0.2.1/even_dist.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-06-24 01:10:40.000000 even-dist-0.2.1/even_dist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-24 01:10:40.000000 even-dist-0.2.1/even_dist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 01:10:40.000000 even-dist-0.2.1/even_dist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 01:10:40.000000 even-dist-0.2.1/even_dist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 01:10:40.000000 even-dist-0.2.1/even_dist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 01:10:40.623363 even-dist-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-06-24 01:10:37.000000 even-dist-0.2.1/setup.py
```

### Comparing `even-dist-0.2.0/LICENSE` & `even-dist-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `even-dist-0.2.0/setup.py` & `even-dist-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="even-dist",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(include=["even_dist"]),  # I only will upload this package
-    version="0.2.0",
+    version="0.2.1",
     description="My first Python library",
     install_requires=["numpy", "matplotlib"],
     author="kirp",
     author_email="kirp@umich.edu",
     license="MIT",
     setup_requires=["pytest-runner"],
-    tests_require=["pytest==4.4.1"],
     test_suite="tests",
     url="https://github.com/tic-top/even_dist/",
 )
```

