# Comparing `tmp/even-dist-0.2.9.tar.gz` & `tmp/even-dist-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "even-dist-0.2.9.tar", last modified: Sat Jun 24 02:21:51 2023, max compression
+gzip compressed data, was "even-dist-0.3.0.tar", last modified: Sat Jun 24 02:25:40 2023, max compression
```

## Comparing `even-dist-0.2.9.tar` & `even-dist-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 02:21:51.507843 even-dist-0.2.9/
--rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.2.9/LICENSE
--rw-rw-rw-   0        0        0      400 2023-06-24 02:21:51.507216 even-dist-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 02:21:51.507843 even-dist-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-06-24 02:19:24.000000 even-dist-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:21:51.472371 even-dist-0.2.9/src/
-drwxrwxrwx   0        0        0        0 2023-06-24 02:21:51.486332 even-dist-0.2.9/src/even_dist/
--rw-rw-rw-   0        0        0       53 2023-06-24 00:32:55.000000 even-dist-0.2.9/src/even_dist/__init__.py
--rw-rw-rw-   0        0        0      713 2023-06-24 00:11:48.000000 even-dist-0.2.9/src/even_dist/even_dist.py
-drwxrwxrwx   0        0        0        0 2023-06-24 02:21:51.502858 even-dist-0.2.9/src/even_dist.egg-info/
--rw-rw-rw-   0        0        0      400 2023-06-24 02:21:51.000000 even-dist-0.2.9/src/even_dist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-06-24 02:21:51.000000 even-dist-0.2.9/src/even_dist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 02:21:51.000000 even-dist-0.2.9/src/even_dist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-24 02:21:51.000000 even-dist-0.2.9/src/even_dist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-24 02:21:51.000000 even-dist-0.2.9/src/even_dist.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-24 02:21:51.504852 even-dist-0.2.9/src/hello/
--rw-rw-rw-   0        0        0        0 2023-06-24 01:57:38.000000 even-dist-0.2.9/src/hello/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:25:40.734744 even-dist-0.3.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      400 2023-06-24 02:25:40.734308 even-dist-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 02:25:40.735743 even-dist-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-06-24 02:25:21.000000 even-dist-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:25:40.705799 even-dist-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 02:25:40.715773 even-dist-0.3.0/src/even_dist/
+-rw-rw-rw-   0        0        0       53 2023-06-24 00:32:55.000000 even-dist-0.3.0/src/even_dist/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-06-24 00:11:48.000000 even-dist-0.3.0/src/even_dist/even_dist.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:25:40.729756 even-dist-0.3.0/src/even_dist.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-06-24 02:25:40.000000 even-dist-0.3.0/src/even_dist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-06-24 02:25:40.000000 even-dist-0.3.0/src/even_dist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 02:25:40.000000 even-dist-0.3.0/src/even_dist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 02:25:40.000000 even-dist-0.3.0/src/even_dist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-24 02:25:40.000000 even-dist-0.3.0/src/even_dist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 02:25:40.732748 even-dist-0.3.0/src/hello/
+-rw-rw-rw-   0        0        0        0 2023-06-24 01:57:38.000000 even-dist-0.3.0/src/hello/__init__.py
```

### Comparing `even-dist-0.2.9/LICENSE` & `even-dist-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `even-dist-0.2.9/setup.py` & `even-dist-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     name="even-dist",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", include=["*"]),
     package_dir={"": "src"},
     package_data={"hello": ["*.txt"]},
     include_package_data=True,
-    version="0.2.9",
+    version="0.3.0",
     description="My first Python library",
     install_requires=["numpy", "matplotlib"],
     author="kirp",
     author_email="kirp@umich.edu",
     license="MIT",
     setup_requires=["pytest-runner"],
     test_suite="tests",
```

### Comparing `even-dist-0.2.9/src/even_dist/even_dist.py` & `even-dist-0.3.0/src/even_dist/even_dist.py`

 * *Files identical despite different names*

