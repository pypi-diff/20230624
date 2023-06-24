# Comparing `tmp/irregular-chars-0.1.2.tar.gz` & `tmp/irregular-chars-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irregular-chars-0.1.2.tar", last modified: Sat Jun 24 17:42:22 2023, max compression
+gzip compressed data, was "irregular-chars-1.0.0.tar", last modified: Sat Jun 24 18:17:46 2023, max compression
```

## Comparing `irregular-chars-0.1.2.tar` & `irregular-chars-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 17:42:22.216985 irregular-chars-0.1.2/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-24 15:34:45.000000 irregular-chars-0.1.2/LICENSE
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      487 2023-06-24 17:42:22.216985 irregular-chars-0.1.2/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-06-24 16:31:23.000000 irregular-chars-0.1.2/README.md
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 17:42:22.212985 irregular-chars-0.1.2/irregular-chars/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 15:25:21.000000 irregular-chars-0.1.2/irregular-chars/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      735 2023-06-24 16:14:52.000000 irregular-chars-0.1.2/irregular-chars/zero_width.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 17:42:22.216985 irregular-chars-0.1.2/irregular_chars.egg-info/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      487 2023-06-24 17:42:22.000000 irregular-chars-0.1.2/irregular_chars.egg-info/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      290 2023-06-24 17:42:22.000000 irregular-chars-0.1.2/irregular_chars.egg-info/SOURCES.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-24 17:42:22.000000 irregular-chars-0.1.2/irregular_chars.egg-info/dependency_links.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       22 2023-06-24 17:42:22.000000 irregular-chars-0.1.2/irregular_chars.egg-info/top_level.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-24 17:42:22.216985 irregular-chars-0.1.2/setup.cfg
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      717 2023-06-24 17:42:20.000000 irregular-chars-0.1.2/setup.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 17:42:22.216985 irregular-chars-0.1.2/tests/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 14:44:31.000000 irregular-chars-0.1.2/tests/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      725 2023-06-24 17:40:31.000000 irregular-chars-0.1.2/tests/test_zero_width_spaces.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 18:17:46.676440 irregular-chars-1.0.0/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-24 15:34:45.000000 irregular-chars-1.0.0/LICENSE
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      500 2023-06-24 18:17:46.676440 irregular-chars-1.0.0/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-06-24 16:31:23.000000 irregular-chars-1.0.0/README.md
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 18:17:46.676440 irregular-chars-1.0.0/irregular-chars/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 15:25:21.000000 irregular-chars-1.0.0/irregular-chars/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      783 2023-06-24 18:15:44.000000 irregular-chars-1.0.0/irregular-chars/zero_width.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 18:17:46.676440 irregular-chars-1.0.0/irregular_chars.egg-info/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      500 2023-06-24 18:17:46.000000 irregular-chars-1.0.0/irregular_chars.egg-info/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      290 2023-06-24 18:17:46.000000 irregular-chars-1.0.0/irregular_chars.egg-info/SOURCES.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-24 18:17:46.000000 irregular-chars-1.0.0/irregular_chars.egg-info/dependency_links.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       22 2023-06-24 18:17:46.000000 irregular-chars-1.0.0/irregular_chars.egg-info/top_level.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-24 18:17:46.676440 irregular-chars-1.0.0/setup.cfg
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      730 2023-06-24 18:17:44.000000 irregular-chars-1.0.0/setup.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 18:17:46.676440 irregular-chars-1.0.0/tests/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 14:44:31.000000 irregular-chars-1.0.0/tests/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      873 2023-06-24 18:14:35.000000 irregular-chars-1.0.0/tests/test_zero_width_spaces.py
```

### Comparing `irregular-chars-0.1.2/LICENSE` & `irregular-chars-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `irregular-chars-0.1.2/setup.py` & `irregular-chars-1.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import find_packages, setup
 
 setup(
     name="irregular-chars",
-    version="0.1.2",
+    version="1.0.0",
     description="A library for cleaning text, such as removing zero-width characters or"
     "converting full-width characters to half-width",
     packages=find_packages(),
     install_requires=[],
     classifiers=[  # パッケージのメタデータ（詳細は https://pypi.org/classifiers/ を参照）
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
     ],
     author="Masato Emata",
     url="https://github.com/masatoEmata/replace_irregular_chars",
     keywords="",
```

### Comparing `irregular-chars-0.1.2/tests/test_zero_width_spaces.py` & `irregular-chars-1.0.0/tests/test_zero_width_spaces.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,7 +15,13 @@
     assert remove_zero_width(test_str) == expected_str
 
 
 def test_remove_zero_width_no_change():
     test_str = "Hello World"
     expected_str = "Hello World"
     assert remove_zero_width(test_str) == expected_str
+
+
+def test_remove_zero_width_use_quotations():
+    origin = '"​"""⁡""­"'
+    expect = '"""""""'
+    assert expect == remove_zero_width(origin)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

