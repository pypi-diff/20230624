# Comparing `tmp/even-dist-0.2.3.tar.gz` & `tmp/even-dist-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "even-dist-0.2.3.tar", last modified: Sat Jun 24 01:23:54 2023, max compression
+gzip compressed data, was "even-dist-0.2.5.tar", last modified: Sat Jun 24 01:47:53 2023, max compression
```

## Comparing `even-dist-0.2.3.tar` & `even-dist-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 01:23:54.277581 even-dist-0.2.3/
--rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      400 2023-06-24 01:23:54.276584 even-dist-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 01:23:54.278580 even-dist-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-06-24 01:23:50.000000 even-dist-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 01:23:54.239684 even-dist-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-24 01:23:54.249658 even-dist-0.2.3/src/even_dist/
--rw-rw-rw-   0        0        0       53 2023-06-24 00:32:55.000000 even-dist-0.2.3/src/even_dist/__init__.py
--rw-rw-rw-   0        0        0      713 2023-06-24 00:11:48.000000 even-dist-0.2.3/src/even_dist/even_dist.py
-drwxrwxrwx   0        0        0        0 2023-06-24 01:23:54.273594 even-dist-0.2.3/src/even_dist.egg-info/
--rw-rw-rw-   0        0        0      400 2023-06-24 01:23:54.000000 even-dist-0.2.3/src/even_dist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-06-24 01:23:54.000000 even-dist-0.2.3/src/even_dist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 01:23:54.000000 even-dist-0.2.3/src/even_dist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-24 01:23:54.000000 even-dist-0.2.3/src/even_dist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-24 01:23:54.000000 even-dist-0.2.3/src/even_dist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 01:47:53.626813 even-dist-0.2.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      400 2023-06-24 01:47:53.625769 even-dist-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 01:47:53.626813 even-dist-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      668 2023-06-24 01:47:51.000000 even-dist-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 01:47:53.585155 even-dist-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 01:47:53.596127 even-dist-0.2.5/src/even_dist/
+-rw-rw-rw-   0        0        0       53 2023-06-24 00:32:55.000000 even-dist-0.2.5/src/even_dist/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-06-24 00:11:48.000000 even-dist-0.2.5/src/even_dist/even_dist.py
+drwxrwxrwx   0        0        0        0 2023-06-24 01:47:53.623774 even-dist-0.2.5/src/even_dist.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-06-24 01:47:53.000000 even-dist-0.2.5/src/even_dist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-06-24 01:47:53.000000 even-dist-0.2.5/src/even_dist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 01:47:53.000000 even-dist-0.2.5/src/even_dist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 01:47:53.000000 even-dist-0.2.5/src/even_dist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 01:47:53.000000 even-dist-0.2.5/src/even_dist.egg-info/top_level.txt
```

### Comparing `even-dist-0.2.3/LICENSE` & `even-dist-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `even-dist-0.2.3/setup.py` & `even-dist-0.2.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="even-dist",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=find_packages(
-        where="src", include=["*"]
-    ),  # I only will upload this package
+    packages=find_packages(),
     package_dir={"": "src"},
-    version="0.2.3",
+    version="0.2.5",
     description="My first Python library",
     install_requires=["numpy", "matplotlib"],
     author="kirp",
     author_email="kirp@umich.edu",
     license="MIT",
     setup_requires=["pytest-runner"],
     test_suite="tests",
```

### Comparing `even-dist-0.2.3/src/even_dist/even_dist.py` & `even-dist-0.2.5/src/even_dist/even_dist.py`

 * *Files identical despite different names*

