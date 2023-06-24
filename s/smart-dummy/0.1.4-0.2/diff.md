# Comparing `tmp/smart_dummy-0.1.4.tar.gz` & `tmp/smart_dummy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_dummy-0.1.4.tar", last modified: Fri Jun  9 23:54:29 2023, max compression
+gzip compressed data, was "smart_dummy-0.2.tar", last modified: Sat Jun 24 15:00:16 2023, max compression
```

## Comparing `smart_dummy-0.1.4.tar` & `smart_dummy-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 23:54:29.397969 smart_dummy-0.1.4/
--rw-rw-rw-   0        0        0     1105 2023-06-09 23:14:45.000000 smart_dummy-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2634 2023-06-09 23:54:29.397969 smart_dummy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1622 2023-06-09 23:14:45.000000 smart_dummy-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 23:54:29.398970 smart_dummy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-06-09 23:54:20.000000 smart_dummy-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 23:54:29.385965 smart_dummy-0.1.4/smart_dummy/
--rw-rw-rw-   0        0        0      298 2023-06-09 23:52:06.000000 smart_dummy-0.1.4/smart_dummy/__init__.py
--rw-rw-rw-   0        0        0      661 2023-06-09 23:14:45.000000 smart_dummy-0.1.4/smart_dummy/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 23:54:29.396969 smart_dummy-0.1.4/smart_dummy.egg-info/
--rw-rw-rw-   0        0        0     2634 2023-06-09 23:54:29.000000 smart_dummy-0.1.4/smart_dummy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-09 23:54:29.000000 smart_dummy-0.1.4/smart_dummy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 23:54:29.000000 smart_dummy-0.1.4/smart_dummy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-06-09 23:54:29.000000 smart_dummy-0.1.4/smart_dummy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-09 23:54:29.000000 smart_dummy-0.1.4/smart_dummy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 15:00:16.775874 smart_dummy-0.2/
+-rw-rw-rw-   0        0        0     1105 2023-06-09 23:14:45.000000 smart_dummy-0.2/LICENSE
+-rw-rw-rw-   0        0        0     2227 2023-06-24 15:00:16.774873 smart_dummy-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1692 2023-06-24 14:50:46.000000 smart_dummy-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 15:00:16.775874 smart_dummy-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      853 2023-06-24 14:52:43.000000 smart_dummy-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:00:16.749865 smart_dummy-0.2/smart_dummy/
+-rw-rw-rw-   0        0        0      287 2023-06-24 14:51:28.000000 smart_dummy-0.2/smart_dummy/__init__.py
+-rw-rw-rw-   0        0        0     1436 2023-06-24 14:50:46.000000 smart_dummy-0.2/smart_dummy/main.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:00:16.773873 smart_dummy-0.2/smart_dummy.egg-info/
+-rw-rw-rw-   0        0        0     2227 2023-06-24 15:00:16.000000 smart_dummy-0.2/smart_dummy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-24 15:00:16.000000 smart_dummy-0.2/smart_dummy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 15:00:16.000000 smart_dummy-0.2/smart_dummy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-06-24 15:00:16.000000 smart_dummy-0.2/smart_dummy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-24 15:00:16.000000 smart_dummy-0.2/smart_dummy.egg-info/top_level.txt
```

### Comparing `smart_dummy-0.1.4/LICENSE` & `smart_dummy-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_dummy-0.1.4/setup.py` & `smart_dummy-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="smart_dummy",
-    version="0.1.4",
+    version="0.2",
     packages=find_packages(),
     install_requires=[
         'numpy>=1.24',
         'pandas>=1.0',
         'pydantic>=1.10',
         'scikit-learn>=1.0',
         'spacy>=3.5'
     ],
     author="Muriel Grobler, Emma Zhang",
     author_email="muriel.grobler@gmail.com, emma.lzhang@gmail.com",
-    description="A smart and easy replacement to pandas.get_dummies() ",
+    description="A smart and easy alternative to pandas.get_dummies() ",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/emmalzhang/smart_dummy",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

