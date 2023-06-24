# Comparing `tmp/images-compare-0.5.0.tar.gz` & `tmp/images-compare-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "images-compare-0.5.0.tar", last modified: Thu Jun 22 18:20:10 2023, max compression
+gzip compressed data, was "images-compare-0.6.0.tar", last modified: Sat Jun 24 14:32:25 2023, max compression
```

## Comparing `images-compare-0.5.0.tar` & `images-compare-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 18:20:09.997304 images-compare-0.5.0/
--rw-rw-rw-   0        0        0     1092 2023-06-10 18:34:53.000000 images-compare-0.5.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1391 2023-06-22 18:20:09.997304 images-compare-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      797 2023-06-22 17:42:33.000000 images-compare-0.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 18:20:09.997304 images-compare-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      956 2023-06-22 18:19:58.000000 images-compare-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:20:09.948218 images-compare-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 18:20:09.972999 images-compare-0.5.0/src/images_compare/
--rw-rw-rw-   0        0        0       35 2023-06-22 18:18:37.000000 images-compare-0.5.0/src/images_compare/__init__.py
--rw-rw-rw-   0        0        0      822 2023-06-22 18:19:18.000000 images-compare-0.5.0/src/images_compare/verify.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:20:09.992529 images-compare-0.5.0/src/images_compare.egg-info/
--rw-rw-rw-   0        0        0     1391 2023-06-22 18:20:09.000000 images-compare-0.5.0/src/images_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-22 18:20:09.000000 images-compare-0.5.0/src/images_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 18:20:09.000000 images-compare-0.5.0/src/images_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-22 18:20:09.000000 images-compare-0.5.0/src/images_compare.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-22 18:20:09.000000 images-compare-0.5.0/src/images_compare.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:32:25.964463 images-compare-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-24 14:32:17.000000 images-compare-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-24 14:32:25.964463 images-compare-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-24 14:32:17.000000 images-compare-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:32:25.964463 images-compare-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-24 14:32:25.000000 images-compare-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:32:25.960463 images-compare-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:32:25.960463 images-compare-0.6.0/src/images_compare/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-24 14:32:17.000000 images-compare-0.6.0/src/images_compare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-24 14:32:17.000000 images-compare-0.6.0/src/images_compare/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:32:25.960463 images-compare-0.6.0/src/images_compare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-24 14:32:25.000000 images-compare-0.6.0/src/images_compare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-24 14:32:25.000000 images-compare-0.6.0/src/images_compare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:32:25.000000 images-compare-0.6.0/src/images_compare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:32:25.000000 images-compare-0.6.0/src/images_compare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-24 14:32:25.000000 images-compare-0.6.0/src/images_compare.egg-info/top_level.txt
```

### Comparing `images-compare-0.5.0/README.md` & `images-compare-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `images-compare-0.5.0/setup.py` & `images-compare-0.6.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup, find_packages
-
-with open("README.md", "r", encoding="utf8") as f:
-    long_description = f.read()
-
-setup(
-    name="images-compare",
-    version="0.5.0",
-    description="This Python package allows for image comparison between two provided images using a specified threshold",
-    package_dir={"": "src"},
-    packages=find_packages(where="src"),
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/denzilrdz/images-compare",
-    author="Denzil Rodrigues",
-    author_email="denzil.rdz@gmail.com",
-    license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.11",
-        "Operating System :: OS Independent",
-    ],
-    install_requires=["numpy>=1.25.0", "opencv-python>=4.7.0.72"],
-    extras_requires={"dev": ["twine>=4.0.2"]},
-    python_requires=">=3.11",
-)
+from setuptools import setup, find_packages
+
+with open("README.md", "r", encoding="utf8") as f:
+    long_description = f.read()
+
+setup(
+    name="images-compare",
+    version="0.6.0",
+    description="This Python package allows for image comparison between two provided images using a specified threshold",
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/denzilrdz/images-compare",
+    author="Denzil Rodrigues",
+    author_email="denzil.rdz@gmail.com",
+    license="MIT",
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.11",
+        "Operating System :: OS Independent",
+    ],
+    install_requires=["numpy>=1.25.0", "opencv-python>=4.7.0.72"],
+    extras_requires={"dev": []},
+    python_requires=">=3.11",
+)
```

