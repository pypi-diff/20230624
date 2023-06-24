# Comparing `tmp/irregular_chars-0.1.1.tar.gz` & `tmp/irregular-chars-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irregular_chars-0.1.1.tar", last modified: Sat Jun 24 16:36:56 2023, max compression
+gzip compressed data, was "irregular-chars-0.1.2.tar", last modified: Sat Jun 24 17:42:22 2023, max compression
```

## Comparing `irregular_chars-0.1.1.tar` & `irregular-chars-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 16:36:56.915282 irregular_chars-0.1.1/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-24 15:34:45.000000 irregular_chars-0.1.1/LICENSE
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      488 2023-06-24 16:36:56.911282 irregular_chars-0.1.1/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-06-24 16:31:23.000000 irregular_chars-0.1.1/README.md
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 16:36:56.911282 irregular_chars-0.1.1/irregular_chars/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 15:25:21.000000 irregular_chars-0.1.1/irregular_chars/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      735 2023-06-24 16:14:52.000000 irregular_chars-0.1.1/irregular_chars/zero_width.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 16:36:56.911282 irregular_chars-0.1.1/irregular_chars.egg-info/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      488 2023-06-24 16:36:56.000000 irregular_chars-0.1.1/irregular_chars.egg-info/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      290 2023-06-24 16:36:56.000000 irregular_chars-0.1.1/irregular_chars.egg-info/SOURCES.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-24 16:36:56.000000 irregular_chars-0.1.1/irregular_chars.egg-info/dependency_links.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       22 2023-06-24 16:36:56.000000 irregular_chars-0.1.1/irregular_chars.egg-info/top_level.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-24 16:36:56.915282 irregular_chars-0.1.1/setup.cfg
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      711 2023-06-24 16:33:17.000000 irregular_chars-0.1.1/setup.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 16:36:56.911282 irregular_chars-0.1.1/tests/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 14:44:31.000000 irregular_chars-0.1.1/tests/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      726 2023-06-24 15:29:07.000000 irregular_chars-0.1.1/tests/test_zero_width_spaces.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 17:42:22.216985 irregular-chars-0.1.2/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-24 15:34:45.000000 irregular-chars-0.1.2/LICENSE
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      487 2023-06-24 17:42:22.216985 irregular-chars-0.1.2/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-06-24 16:31:23.000000 irregular-chars-0.1.2/README.md
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 17:42:22.212985 irregular-chars-0.1.2/irregular-chars/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 15:25:21.000000 irregular-chars-0.1.2/irregular-chars/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      735 2023-06-24 16:14:52.000000 irregular-chars-0.1.2/irregular-chars/zero_width.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 17:42:22.216985 irregular-chars-0.1.2/irregular_chars.egg-info/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      487 2023-06-24 17:42:22.000000 irregular-chars-0.1.2/irregular_chars.egg-info/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      290 2023-06-24 17:42:22.000000 irregular-chars-0.1.2/irregular_chars.egg-info/SOURCES.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-24 17:42:22.000000 irregular-chars-0.1.2/irregular_chars.egg-info/dependency_links.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       22 2023-06-24 17:42:22.000000 irregular-chars-0.1.2/irregular_chars.egg-info/top_level.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-24 17:42:22.216985 irregular-chars-0.1.2/setup.cfg
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      717 2023-06-24 17:42:20.000000 irregular-chars-0.1.2/setup.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 17:42:22.216985 irregular-chars-0.1.2/tests/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 14:44:31.000000 irregular-chars-0.1.2/tests/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      725 2023-06-24 17:40:31.000000 irregular-chars-0.1.2/tests/test_zero_width_spaces.py
```

### Comparing `irregular_chars-0.1.1/LICENSE` & `irregular-chars-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `irregular_chars-0.1.1/irregular_chars/zero_width.py` & `irregular-chars-0.1.2/irregular-chars/zero_width.py`

 * *Files identical despite different names*

### Comparing `irregular_chars-0.1.1/setup.py` & `irregular-chars-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import find_packages, setup
 
 setup(
-    name="irregular_chars",
-    version="0.1.1",
-    description="A library for cleaning text, such as removing zero-width characters or converting full-width characters to half-width",
+    name="irregular-chars",
+    version="0.1.2",
+    description="A library for cleaning text, such as removing zero-width characters or"
+    "converting full-width characters to half-width",
     packages=find_packages(),
     install_requires=[],
     classifiers=[  # パッケージのメタデータ（詳細は https://pypi.org/classifiers/ を参照）
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
```

### Comparing `irregular_chars-0.1.1/tests/test_zero_width_spaces.py` & `irregular-chars-0.1.2/tests/test_zero_width_spaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from irregular_chars.zero_width import ZERO_WIDTH_SPACES, remove_zero_width
 
 
 @pytest.mark.parametrize("name, char", ZERO_WIDTH_SPACES.items())
 def test_remove_zero_width(name, char):
     test_str = f"Hello{char}World"
     expected_str = "HelloWorld"
```

