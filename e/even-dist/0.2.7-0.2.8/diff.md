# Comparing `tmp/even-dist-0.2.7.tar.gz` & `tmp/even-dist-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "even-dist-0.2.7.tar", last modified: Sat Jun 24 01:58:45 2023, max compression
+gzip compressed data, was "even-dist-0.2.8.tar", last modified: Sat Jun 24 02:16:33 2023, max compression
```

## Comparing `even-dist-0.2.7.tar` & `even-dist-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 01:58:45.960881 even-dist-0.2.7/
--rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.2.7/LICENSE
--rw-rw-rw-   0        0        0      400 2023-06-24 01:58:45.959884 even-dist-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 01:58:45.960881 even-dist-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-06-24 01:58:42.000000 even-dist-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 01:58:45.913738 even-dist-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-24 01:58:45.924708 even-dist-0.2.7/src/even_dist/
--rw-rw-rw-   0        0        0       53 2023-06-24 00:32:55.000000 even-dist-0.2.7/src/even_dist/__init__.py
--rw-rw-rw-   0        0        0      713 2023-06-24 00:11:48.000000 even-dist-0.2.7/src/even_dist/even_dist.py
-drwxrwxrwx   0        0        0        0 2023-06-24 01:58:45.955896 even-dist-0.2.7/src/even_dist.egg-info/
--rw-rw-rw-   0        0        0      400 2023-06-24 01:58:45.000000 even-dist-0.2.7/src/even_dist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-06-24 01:58:45.000000 even-dist-0.2.7/src/even_dist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 01:58:45.000000 even-dist-0.2.7/src/even_dist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-24 01:58:45.000000 even-dist-0.2.7/src/even_dist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-24 01:58:45.000000 even-dist-0.2.7/src/even_dist.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-24 01:58:45.957890 even-dist-0.2.7/src/hello/
--rw-rw-rw-   0        0        0        0 2023-06-24 01:57:38.000000 even-dist-0.2.7/src/hello/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:16:33.932144 even-dist-0.2.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 19:59:19.000000 even-dist-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0      400 2023-06-24 02:16:33.929560 even-dist-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2023-06-24 00:32:52.000000 even-dist-0.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 02:16:33.932144 even-dist-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-06-24 02:16:31.000000 even-dist-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:16:33.884205 even-dist-0.2.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 02:16:33.894175 even-dist-0.2.8/src/even_dist/
+-rw-rw-rw-   0        0        0       53 2023-06-24 00:32:55.000000 even-dist-0.2.8/src/even_dist/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-06-24 00:11:48.000000 even-dist-0.2.8/src/even_dist/even_dist.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:16:33.922158 even-dist-0.2.8/src/even_dist.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-06-24 02:16:33.000000 even-dist-0.2.8/src/even_dist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-24 02:16:33.000000 even-dist-0.2.8/src/even_dist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 02:16:33.000000 even-dist-0.2.8/src/even_dist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 02:16:33.000000 even-dist-0.2.8/src/even_dist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-24 02:16:33.000000 even-dist-0.2.8/src/even_dist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 02:16:33.927145 even-dist-0.2.8/src/hello/
+-rw-rw-rw-   0        0        0        0 2023-06-24 01:57:38.000000 even-dist-0.2.8/src/hello/__init__.py
+-rw-rw-rw-   0        0        0        8 2023-06-24 02:02:01.000000 even-dist-0.2.8/src/hello/fadf.py
```

### Comparing `even-dist-0.2.7/LICENSE` & `even-dist-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `even-dist-0.2.7/setup.py` & `even-dist-0.2.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 
 setup(
     name="even-dist",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", include=["*"]),
     package_dir={"": "src"},
-    include_package_data=True,
-    version="0.2.7",
+    # package_data={"hello": ["*"]},
+    # include_package_data=True,
+    version="0.2.8",
     description="My first Python library",
     install_requires=["numpy", "matplotlib"],
     author="kirp",
     author_email="kirp@umich.edu",
     license="MIT",
     setup_requires=["pytest-runner"],
     test_suite="tests",
```

### Comparing `even-dist-0.2.7/src/even_dist/even_dist.py` & `even-dist-0.2.8/src/even_dist/even_dist.py`

 * *Files identical despite different names*

