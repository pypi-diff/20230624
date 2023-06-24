# Comparing `tmp/even-dist-0.2.1.tar.gz` & `tmp/even-dist-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "even-dist-0.2.1.tar", last modified: Sat Jun 24 01:10:40 2023, max compression
+gzip compressed data, was "even-dist-0.2.2.tar", last modified: Sat Jun 24 01:18:21 2023, max compression
```

## Comparing `even-dist-0.2.1.tar` & `even-dist-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 01:10:40.622364 even-dist-0.2.1/
--rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      400 2023-06-24 01:10:40.621774 even-dist-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 01:10:40.619373 even-dist-0.2.1/even_dist.egg-info/
--rw-rw-rw-   0        0        0      400 2023-06-24 01:10:40.000000 even-dist-0.2.1/even_dist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-24 01:10:40.000000 even-dist-0.2.1/even_dist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 01:10:40.000000 even-dist-0.2.1/even_dist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-24 01:10:40.000000 even-dist-0.2.1/even_dist.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 01:10:40.000000 even-dist-0.2.1/even_dist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 01:10:40.623363 even-dist-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-06-24 01:10:37.000000 even-dist-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 01:18:21.020225 even-dist-0.2.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      400 2023-06-24 01:18:21.018230 even-dist-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 01:18:21.012246 even-dist-0.2.2/even_dist.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-06-24 01:18:20.000000 even-dist-0.2.2/even_dist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-24 01:18:20.000000 even-dist-0.2.2/even_dist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 01:18:20.000000 even-dist-0.2.2/even_dist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 01:18:20.000000 even-dist-0.2.2/even_dist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 01:18:20.000000 even-dist-0.2.2/even_dist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 01:18:21.020225 even-dist-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      688 2023-06-24 01:18:17.000000 even-dist-0.2.2/setup.py
```

### Comparing `even-dist-0.2.1/LICENSE` & `even-dist-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `even-dist-0.2.1/setup.py` & `even-dist-0.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="even-dist",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=find_packages(include=["even_dist"]),  # I only will upload this package
-    version="0.2.1",
+    packages=find_packages(include=["src"]),  # I only will upload this package
+    version="0.2.2",
     description="My first Python library",
     install_requires=["numpy", "matplotlib"],
     author="kirp",
     author_email="kirp@umich.edu",
     license="MIT",
     setup_requires=["pytest-runner"],
     test_suite="tests",
```

