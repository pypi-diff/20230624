# Comparing `tmp/onion_network-1.0.1.tar.gz` & `tmp/onion_network-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion_network-1.0.1.tar", last modified: Fri Jun 23 22:23:32 2023, max compression
+gzip compressed data, was "onion_network-1.0.2.tar", last modified: Sat Jun 24 12:08:48 2023, max compression
```

## Comparing `onion_network-1.0.1.tar` & `onion_network-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:23:32.468529 onion_network-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-23 22:23:22.000000 onion_network-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 22:23:22.000000 onion_network-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-23 22:23:32.468529 onion_network-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-06-23 22:23:22.000000 onion_network-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:23:32.468529 onion_network-1.0.1/onion_network/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-23 22:23:22.000000 onion_network-1.0.1/onion_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-23 22:23:22.000000 onion_network-1.0.1/onion_network/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-23 22:23:22.000000 onion_network-1.0.1/onion_network/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:23:32.468529 onion_network-1.0.1/onion_network.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-23 22:23:32.000000 onion_network-1.0.1/onion_network.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-23 22:23:32.000000 onion_network-1.0.1/onion_network.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:23:32.000000 onion_network-1.0.1/onion_network.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 22:23:32.000000 onion_network-1.0.1/onion_network.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 22:23:32.000000 onion_network-1.0.1/onion_network.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 22:23:22.000000 onion_network-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 22:23:32.468529 onion_network-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-23 22:23:22.000000 onion_network-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:23:32.468529 onion_network-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-23 22:23:22.000000 onion_network-1.0.1/tests/test_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:08:48.757016 onion_network-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-24 12:08:39.000000 onion_network-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-24 12:08:39.000000 onion_network-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-24 12:08:48.757016 onion_network-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-06-24 12:08:39.000000 onion_network-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:08:48.757016 onion_network-1.0.2/onion_network/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-24 12:08:39.000000 onion_network-1.0.2/onion_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-24 12:08:39.000000 onion_network-1.0.2/onion_network/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-24 12:08:39.000000 onion_network-1.0.2/onion_network/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:08:48.757016 onion_network-1.0.2/onion_network.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-24 12:08:48.000000 onion_network-1.0.2/onion_network.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-24 12:08:48.000000 onion_network-1.0.2/onion_network.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 12:08:48.000000 onion_network-1.0.2/onion_network.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 12:08:48.000000 onion_network-1.0.2/onion_network.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 12:08:48.000000 onion_network-1.0.2/onion_network.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-24 12:08:39.000000 onion_network-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 12:08:48.757016 onion_network-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-24 12:08:39.000000 onion_network-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:08:48.757016 onion_network-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-24 12:08:39.000000 onion_network-1.0.2/tests/test_generation.py
```

### Comparing `onion_network-1.0.1/LICENSE` & `onion_network-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onion_network-1.0.1/PKG-INFO` & `onion_network-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: onion_network
-Version: 1.0.1
+Version: 1.0.2
 Summary: A module for generating and visualizing onion-structured networks!
 Home-page: https://github.com/SimonPop/onion_network
 Author: Simon Popelier
 Author-email: simon.popelier@gmail.com
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1  align="center">🧅 Onion Network </h1>
 
 <img src="imgs/illustration.png" alt="banner" width="100%">
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: onion_network Version: 1.0.1 Summary: A module for
+Metadata-Version: 2.1 Name: onion_network Version: 1.0.2 Summary: A module for
 generating and visualizing onion-structured networks! Home-page: https://
 github.com/SimonPop/onion_network Author: Simon Popelier Author-email:
-simon.popelier@gmail.com License-File: LICENSE
+simon.popelier@gmail.com Description-Content-Type: text/markdown License-File:
+LICENSE
                        ****** ð§ Onion Network ******
 [banner]
 [Project_Version] [Python_Version_3.8] [License:_MIT] [Code_style:_black] [PyPI
                                    version]
 Onion-structured networks are special kinds of scale-free networks with special
 topologies. They tend to possess a high degree [assortativity](https://
 en.wikipedia.org/wiki/Assortativity). It makes it possible to decompose them
```

### Comparing `onion_network-1.0.1/README.md` & `onion_network-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `onion_network-1.0.1/onion_network/generation.py` & `onion_network-1.0.2/onion_network/generation.py`

 * *Files identical despite different names*

### Comparing `onion_network-1.0.1/onion_network/visualization.py` & `onion_network-1.0.2/onion_network/visualization.py`

 * *Files identical despite different names*

### Comparing `onion_network-1.0.1/onion_network.egg-info/PKG-INFO` & `onion_network-1.0.2/onion_network.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: onion-network
-Version: 1.0.1
+Version: 1.0.2
 Summary: A module for generating and visualizing onion-structured networks!
 Home-page: https://github.com/SimonPop/onion_network
 Author: Simon Popelier
 Author-email: simon.popelier@gmail.com
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1  align="center">🧅 Onion Network </h1>
 
 <img src="imgs/illustration.png" alt="banner" width="100%">
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: onion-network Version: 1.0.1 Summary: A module for
+Metadata-Version: 2.1 Name: onion-network Version: 1.0.2 Summary: A module for
 generating and visualizing onion-structured networks! Home-page: https://
 github.com/SimonPop/onion_network Author: Simon Popelier Author-email:
-simon.popelier@gmail.com License-File: LICENSE
+simon.popelier@gmail.com Description-Content-Type: text/markdown License-File:
+LICENSE
                        ****** ð§ Onion Network ******
 [banner]
 [Project_Version] [Python_Version_3.8] [License:_MIT] [Code_style:_black] [PyPI
                                    version]
 Onion-structured networks are special kinds of scale-free networks with special
 topologies. They tend to possess a high degree [assortativity](https://
 en.wikipedia.org/wiki/Assortativity). It makes it possible to decompose them
```

### Comparing `onion_network-1.0.1/setup.py` & `onion_network-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 with open("requirements.txt") as f:
     tests_require = f.readlines()
 install_requires = [t.strip() for t in tests_require]
 
 setup(
     name="onion_network",
-    version="1.0.1",
+    version="1.0.2",
     description="A module for generating and visualizing onion-structured networks!",
     long_description=long_description,
+    long_description_content_type='text/markdown',
     author="Simon Popelier",
     author_email="simon.popelier@gmail.com",
     packages=["onion_network"],
     install_requires=install_requires,
     url='https://github.com/SimonPop/onion_network'
 )
```

### Comparing `onion_network-1.0.1/tests/test_generation.py` & `onion_network-1.0.2/tests/test_generation.py`

 * *Files identical despite different names*

