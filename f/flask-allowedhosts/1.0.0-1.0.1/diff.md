# Comparing `tmp/flask-allowedhosts-1.0.0.tar.gz` & `tmp/flask-allowedhosts-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-allowedhosts-1.0.0.tar", last modified: Sat Jun 24 09:20:19 2023, max compression
+gzip compressed data, was "flask-allowedhosts-1.0.1.tar", last modified: Sat Jun 24 09:25:53 2023, max compression
```

## Comparing `flask-allowedhosts-1.0.0.tar` & `flask-allowedhosts-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 09:20:19.746533 flask-allowedhosts-1.0.0/
--rw-rw-rw-   0        0        0     1090 2023-06-24 09:14:27.000000 flask-allowedhosts-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0      844 2023-06-24 09:20:19.745533 flask-allowedhosts-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1988 2023-06-24 09:15:11.000000 flask-allowedhosts-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 09:20:19.721092 flask-allowedhosts-1.0.0/flask_allowedhosts/
--rw-rw-rw-   0        0        0       34 2023-06-24 08:29:33.000000 flask-allowedhosts-1.0.0/flask_allowedhosts/__init__.py
--rw-rw-rw-   0        0        0      486 2023-06-24 08:47:48.000000 flask-allowedhosts-1.0.0/flask_allowedhosts/decorators.py
-drwxrwxrwx   0        0        0        0 2023-06-24 09:20:19.743533 flask-allowedhosts-1.0.0/flask_allowedhosts.egg-info/
--rw-rw-rw-   0        0        0      844 2023-06-24 09:20:19.000000 flask-allowedhosts-1.0.0/flask_allowedhosts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-24 09:20:19.000000 flask-allowedhosts-1.0.0/flask_allowedhosts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 09:20:19.000000 flask-allowedhosts-1.0.0/flask_allowedhosts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-24 09:20:19.000000 flask-allowedhosts-1.0.0/flask_allowedhosts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-24 09:20:19.000000 flask-allowedhosts-1.0.0/flask_allowedhosts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 09:20:19.747534 flask-allowedhosts-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-06-24 09:19:16.000000 flask-allowedhosts-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:25:53.574751 flask-allowedhosts-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2023-06-24 09:14:27.000000 flask-allowedhosts-1.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0     2953 2023-06-24 09:25:53.573752 flask-allowedhosts-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1988 2023-06-24 09:15:11.000000 flask-allowedhosts-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 09:25:53.549752 flask-allowedhosts-1.0.1/flask_allowedhosts/
+-rw-rw-rw-   0        0        0       34 2023-06-24 08:29:33.000000 flask-allowedhosts-1.0.1/flask_allowedhosts/__init__.py
+-rw-rw-rw-   0        0        0      486 2023-06-24 08:47:48.000000 flask-allowedhosts-1.0.1/flask_allowedhosts/decorators.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:25:53.571753 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/
+-rw-rw-rw-   0        0        0     2953 2023-06-24 09:25:53.000000 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-24 09:25:53.000000 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 09:25:53.000000 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-24 09:25:53.000000 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-24 09:25:53.000000 flask-allowedhosts-1.0.1/flask_allowedhosts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 09:25:53.574751 flask-allowedhosts-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1170 2023-06-24 09:25:46.000000 flask-allowedhosts-1.0.1/setup.py
```

### Comparing `flask-allowedhosts-1.0.0/LICENSE.md` & `flask-allowedhosts-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flask-allowedhosts-1.0.0/README.md` & `flask-allowedhosts-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `flask-allowedhosts-1.0.0/setup.py` & `flask-allowedhosts-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from setuptools import setup
 
+long_description = open('README.md').read()
+long_description_content_type = 'text/markdown'
+
 setup(
     name='flask-allowedhosts',
-    version='1.0.0',
+    version='1.0.1',
     packages=['flask_allowedhosts'],
     install_requires=[
         'Flask',
     ],
     url='https://github.com/riad-azz/flask-allowedhosts',
     license='MIT',
     author='Riadh Azzoun',
     author_email='riadh.azzoun@hotmail.com',
     description='A Flask extension to limit access to your routes by using allowed hosts.',
+    long_description=long_description,
+    long_description_content_type=long_description_content_type,
     keywords=["flask", "allowed hosts", "web development", "security"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

