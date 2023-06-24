# Comparing `tmp/casino-dice-1.0.0.tar.gz` & `tmp/casino-dice-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casino-dice-1.0.0.tar", last modified: Sat Jun 24 18:08:18 2023, max compression
+gzip compressed data, was "casino-dice-1.0.1.tar", last modified: Sat Jun 24 18:33:35 2023, max compression
```

## Comparing `casino-dice-1.0.0.tar` & `casino-dice-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:08:18.710665 casino-dice-1.0.0/
--rw-rw-rw-   0        0        0     1111 2023-06-01 13:44:37.000000 casino-dice-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4277 2023-06-24 18:08:18.710665 casino-dice-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3330 2023-06-24 17:43:01.000000 casino-dice-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 18:08:18.695040 casino-dice-1.0.0/casino_dice/
--rw-rw-rw-   0        0        0       51 2023-06-24 17:35:31.000000 casino-dice-1.0.0/casino_dice/__init__.py
--rw-rw-rw-   0        0        0     2998 2023-06-24 18:07:32.000000 casino-dice-1.0.0/casino_dice/casino_dice.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:08:18.695040 casino-dice-1.0.0/casino_dice.egg-info/
--rw-rw-rw-   0        0        0     4277 2023-06-24 18:08:18.000000 casino-dice-1.0.0/casino_dice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-24 18:08:18.000000 casino-dice-1.0.0/casino_dice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:08:18.000000 casino-dice-1.0.0/casino_dice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-24 18:08:18.000000 casino-dice-1.0.0/casino_dice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 18:08:18.710665 casino-dice-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1152 2023-06-24 17:44:10.000000 casino-dice-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:08:18.710665 casino-dice-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-24 17:26:00.000000 casino-dice-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2719 2023-06-24 17:35:31.000000 casino-dice-1.0.0/tests/unit_tests.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:33:35.774930 casino-dice-1.0.1/
+-rw-rw-rw-   0        0        0     1111 2023-06-01 13:44:37.000000 casino-dice-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5643 2023-06-24 18:33:35.774930 casino-dice-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4664 2023-06-24 18:29:55.000000 casino-dice-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 18:33:35.774930 casino-dice-1.0.1/casino_dice/
+-rw-rw-rw-   0        0        0       51 2023-06-24 18:31:07.000000 casino-dice-1.0.1/casino_dice/__init__.py
+-rw-rw-rw-   0        0        0     2998 2023-06-24 18:07:32.000000 casino-dice-1.0.1/casino_dice/casino_dice.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:33:35.774930 casino-dice-1.0.1/casino_dice.egg-info/
+-rw-rw-rw-   0        0        0     5643 2023-06-24 18:33:35.000000 casino-dice-1.0.1/casino_dice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-24 18:33:35.000000 casino-dice-1.0.1/casino_dice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:33:35.000000 casino-dice-1.0.1/casino_dice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-24 18:33:35.000000 casino-dice-1.0.1/casino_dice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 18:33:35.774930 casino-dice-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-06-24 18:32:59.000000 casino-dice-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:33:35.774930 casino-dice-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-24 17:26:00.000000 casino-dice-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2719 2023-06-24 17:35:31.000000 casino-dice-1.0.1/tests/unit_tests.py
```

### Comparing `casino-dice-1.0.0/LICENSE` & `casino-dice-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `casino-dice-1.0.0/casino_dice/casino_dice.py` & `casino-dice-1.0.1/casino_dice/casino_dice.py`

 * *Files identical despite different names*

### Comparing `casino-dice-1.0.0/setup.py` & `casino-dice-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="casino-dice",
-    version="1.0.0",
+    version="1.0.1",
     author="Anthony V. Ozdemir",
     author_email="anthony@anthonyozdemir.com",
     description="A library for generating byte objects from physical casino dice rolls",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/anthony-ozdemir/casino-dice",
     packages=find_packages(),
```

### Comparing `casino-dice-1.0.0/tests/unit_tests.py` & `casino-dice-1.0.1/tests/unit_tests.py`

 * *Files identical despite different names*

