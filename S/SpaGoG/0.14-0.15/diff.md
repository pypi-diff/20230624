# Comparing `tmp/SpaGoG-0.14.tar.gz` & `tmp/SpaGoG-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpaGoG-0.14.tar", last modified: Thu Jun 22 20:46:02 2023, max compression
+gzip compressed data, was "dist/SpaGoG-0.15.tar", last modified: Fri Jun 23 22:12:40 2023, max compression
```

## Comparing `SpaGoG-0.14.tar` & `SpaGoG-0.15.tar`

### file list

```diff
@@ -1,9 +1,13 @@
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:46:02.000000 SpaGoG-0.14/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1224 2023-06-22 20:38:39.000000 SpaGoG-0.14/setup.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       39 2023-05-12 23:49:44.000000 SpaGoG-0.14/setup.cfg
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:43:34.000000 SpaGoG-0.14/README
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      486 2023-06-22 20:46:02.000000 SpaGoG-0.14/PKG-INFO
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:46:02.000000 SpaGoG-0.14/spagog/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     8354 2023-06-22 20:21:02.000000 SpaGoG-0.14/spagog/main.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:40.000000 SpaGoG-0.14/spagog/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    11750 2023-06-22 20:14:46.000000 SpaGoG-0.14/spagog/experiments.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:12:40.000000 SpaGoG-0.15/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1342 2023-06-23 22:11:22.000000 SpaGoG-0.15/setup.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       39 2023-05-12 23:49:44.000000 SpaGoG-0.15/setup.cfg
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:43:34.000000 SpaGoG-0.15/README
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      486 2023-06-23 22:12:40.000000 SpaGoG-0.15/PKG-INFO
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:12:40.000000 SpaGoG-0.15/spagog/
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:12:40.000000 SpaGoG-0.15/spagog/default_params/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      236 2023-05-12 23:49:43.000000 SpaGoG-0.15/spagog/default_params/gc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      594 2023-05-12 23:49:43.000000 SpaGoG-0.15/spagog/default_params/gnc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      595 2023-05-12 23:49:43.000000 SpaGoG-0.15/spagog/default_params/gc+nc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     8354 2023-06-22 20:21:02.000000 SpaGoG-0.15/spagog/main.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:40.000000 SpaGoG-0.15/spagog/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    11750 2023-06-22 20:14:46.000000 SpaGoG-0.15/spagog/experiments.py
```

### Comparing `SpaGoG-0.14/setup.py` & `SpaGoG-0.15/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from distutils.core import setup
 
 setup(
     name='SpaGoG',  # How you named your package folder (MyLib)
     packages=['spagog'],  # Chose the same as "name"
-    version='0.14',  # Start with a small number and increase it with every change you make
+    version='0.15',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Sparse data classification using Graph of Graphs',  # Give a short description about your library
     author='Shachar Hananya',  # Type in your name
     author_email='shacharhananya@gmail.com',  # Type in your E-Mail
     url='https://github.com/HananyaS/SpaGoG',  # Provide either the link to your github or to your website
-    download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.14.tar.gz',  # I explain this later on
+    download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.15.tar.gz',  # I explain this later on
     keywords=['GoG', 'Missing values', 'Graphs'],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
         'pandas==2.0.1',
         'torch==2.0.1',
         'torch-geometric==2.3.1',
         'matplotlib==3.7.1',
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',  # Again, pick a license
         'Programming Language :: Python :: 3.8',
     ],
+    # add the json files that appear in default_params folder
+    package_data={'spagog': ['default_params/*.json']},
 )
```

### Comparing `SpaGoG-0.14/spagog/main.py` & `SpaGoG-0.15/spagog/main.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.14/spagog/experiments.py` & `SpaGoG-0.15/spagog/experiments.py`

 * *Files identical despite different names*

