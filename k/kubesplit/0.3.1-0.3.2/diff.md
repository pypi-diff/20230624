# Comparing `tmp/kubesplit-0.3.1.tar.gz` & `tmp/kubesplit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kubesplit-0.3.1.tar", last modified: Sun May 17 20:16:05 2020, max compression
+gzip compressed data, was "dist/kubesplit-0.3.2.tar", last modified: Sun Aug 16 15:16:59 2020, max compression
```

## Comparing `kubesplit-0.3.1.tar` & `kubesplit-0.3.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-17 20:16:05.000000 kubesplit-0.3.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2020-05-17 20:15:38.000000 kubesplit-0.3.1/AUTHORS.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2020-05-17 20:15:38.000000 kubesplit-0.3.1/HISTORY.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2020-05-17 20:15:38.000000 kubesplit-0.3.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      262 2020-05-17 20:15:38.000000 kubesplit-0.3.1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4239 2020-05-17 20:16:05.000000 kubesplit-0.3.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1899 2020-05-17 20:15:38.000000 kubesplit-0.3.1/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-17 20:16:05.000000 kubesplit-0.3.1/docs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2020-05-17 20:15:38.000000 kubesplit-0.3.1/docs/Makefile
--rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2020-05-17 20:15:38.000000 kubesplit-0.3.1/docs/authors.rst
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4917 2020-05-17 20:15:38.000000 kubesplit-0.3.1/docs/conf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2020-05-17 20:15:38.000000 kubesplit-0.3.1/docs/contributing.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2020-05-17 20:15:38.000000 kubesplit-0.3.1/docs/history.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      314 2020-05-17 20:15:38.000000 kubesplit-0.3.1/docs/index.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1126 2020-05-17 20:15:38.000000 kubesplit-0.3.1/docs/installation.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2020-05-17 20:15:38.000000 kubesplit-0.3.1/docs/readme.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2020-05-17 20:15:38.000000 kubesplit-0.3.1/docs/usage.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-17 20:16:05.000000 kubesplit-0.3.1/kubesplit/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      172 2020-05-17 20:15:38.000000 kubesplit-0.3.1/kubesplit/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      221 2020-05-17 20:15:38.000000 kubesplit-0.3.1/kubesplit/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2144 2020-05-17 20:15:38.000000 kubesplit-0.3.1/kubesplit/args.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3217 2020-05-17 20:15:38.000000 kubesplit-0.3.1/kubesplit/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5364 2020-05-17 20:15:38.000000 kubesplit-0.3.1/kubesplit/convert.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      249 2020-05-17 20:15:38.000000 kubesplit-0.3.1/kubesplit/helpers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2961 2020-05-17 20:15:38.000000 kubesplit-0.3.1/kubesplit/k8s_descriptor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1714 2020-05-17 20:15:38.000000 kubesplit-0.3.1/kubesplit/kubesplit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2020-05-17 20:15:38.000000 kubesplit-0.3.1/kubesplit/namespaces.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1539 2020-05-17 20:15:38.000000 kubesplit-0.3.1/kubesplit/output.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-17 20:16:05.000000 kubesplit-0.3.1/kubesplit.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4239 2020-05-17 20:16:05.000000 kubesplit-0.3.1/kubesplit.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2020-05-17 20:16:05.000000 kubesplit-0.3.1/kubesplit.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-05-17 20:16:05.000000 kubesplit-0.3.1/kubesplit.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2020-05-17 20:16:05.000000 kubesplit-0.3.1/kubesplit.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-05-17 20:16:05.000000 kubesplit-0.3.1/kubesplit.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2020-05-17 20:16:05.000000 kubesplit-0.3.1/kubesplit.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2020-05-17 20:16:05.000000 kubesplit-0.3.1/kubesplit.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      452 2020-05-17 20:16:05.000000 kubesplit-0.3.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1957 2020-05-17 20:15:38.000000 kubesplit-0.3.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-17 20:16:05.000000 kubesplit-0.3.1/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8277 2020-05-17 20:15:38.000000 kubesplit-0.3.1/tests/test_convert.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2712 2020-05-17 20:15:38.000000 kubesplit-0.3.1/tests/test_k8s_descriptor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1293 2020-05-17 20:15:38.000000 kubesplit-0.3.1/tests/test_namespaces.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8490 2020-05-17 20:15:38.000000 kubesplit-0.3.1/tests/test_output.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-08-16 15:16:59.000000 kubesplit-0.3.2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2020-08-16 15:16:35.000000 kubesplit-0.3.2/AUTHORS.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2020-08-16 15:16:35.000000 kubesplit-0.3.2/HISTORY.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2020-08-16 15:16:35.000000 kubesplit-0.3.2/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      262 2020-08-16 15:16:35.000000 kubesplit-0.3.2/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4371 2020-08-16 15:16:59.000000 kubesplit-0.3.2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1991 2020-08-16 15:16:35.000000 kubesplit-0.3.2/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-08-16 15:16:58.000000 kubesplit-0.3.2/docs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2020-08-16 15:16:35.000000 kubesplit-0.3.2/docs/Makefile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2020-08-16 15:16:35.000000 kubesplit-0.3.2/docs/authors.rst
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4917 2020-08-16 15:16:35.000000 kubesplit-0.3.2/docs/conf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2020-08-16 15:16:35.000000 kubesplit-0.3.2/docs/contributing.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2020-08-16 15:16:35.000000 kubesplit-0.3.2/docs/history.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      314 2020-08-16 15:16:35.000000 kubesplit-0.3.2/docs/index.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1126 2020-08-16 15:16:35.000000 kubesplit-0.3.2/docs/installation.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2020-08-16 15:16:35.000000 kubesplit-0.3.2/docs/readme.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2020-08-16 15:16:35.000000 kubesplit-0.3.2/docs/usage.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-08-16 15:16:58.000000 kubesplit-0.3.2/kubesplit/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      172 2020-08-16 15:16:35.000000 kubesplit-0.3.2/kubesplit/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      221 2020-08-16 15:16:35.000000 kubesplit-0.3.2/kubesplit/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2144 2020-08-16 15:16:35.000000 kubesplit-0.3.2/kubesplit/args.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3238 2020-08-16 15:16:35.000000 kubesplit-0.3.2/kubesplit/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5364 2020-08-16 15:16:35.000000 kubesplit-0.3.2/kubesplit/convert.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      249 2020-08-16 15:16:35.000000 kubesplit-0.3.2/kubesplit/helpers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2961 2020-08-16 15:16:35.000000 kubesplit-0.3.2/kubesplit/k8s_descriptor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1714 2020-08-16 15:16:35.000000 kubesplit-0.3.2/kubesplit/kubesplit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2020-08-16 15:16:35.000000 kubesplit-0.3.2/kubesplit/namespaces.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1539 2020-08-16 15:16:35.000000 kubesplit-0.3.2/kubesplit/output.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-08-16 15:16:59.000000 kubesplit-0.3.2/kubesplit.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4371 2020-08-16 15:16:58.000000 kubesplit-0.3.2/kubesplit.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2020-08-16 15:16:58.000000 kubesplit-0.3.2/kubesplit.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-08-16 15:16:58.000000 kubesplit-0.3.2/kubesplit.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2020-08-16 15:16:58.000000 kubesplit-0.3.2/kubesplit.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-08-16 15:16:58.000000 kubesplit-0.3.2/kubesplit.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2020-08-16 15:16:58.000000 kubesplit-0.3.2/kubesplit.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2020-08-16 15:16:58.000000 kubesplit-0.3.2/kubesplit.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      452 2020-08-16 15:16:59.000000 kubesplit-0.3.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1957 2020-08-16 15:16:35.000000 kubesplit-0.3.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-08-16 15:16:59.000000 kubesplit-0.3.2/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8277 2020-08-16 15:16:35.000000 kubesplit-0.3.2/tests/test_convert.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2712 2020-08-16 15:16:35.000000 kubesplit-0.3.2/tests/test_k8s_descriptor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1293 2020-08-16 15:16:35.000000 kubesplit-0.3.2/tests/test_namespaces.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8490 2020-08-16 15:16:35.000000 kubesplit-0.3.2/tests/test_output.py
```

### Comparing `kubesplit-0.3.1/HISTORY.rst` & `kubesplit-0.3.2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/LICENSE` & `kubesplit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/PKG-INFO` & `kubesplit-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kubesplit
-Version: 0.3.1
+Version: 0.3.2
 Summary: Split multidoc yaml formatted kubernetes descriptors to a set         of single resource files
 Home-page: https://github.com/looztra/kubesplit
 Author: Christophe Furmaniak
 Author-email: christophe.furmaniak@gmail.com
 License: Apache Software License 2.0
 Description: =========
         kubesplit
@@ -43,14 +43,19 @@
         -------
         
         This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
         
         .. _Cookiecutter: https://github.com/audreyr/cookiecutter
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         
+        Acknowledgements
+        ----------------
+        
+        - Dependencies scanned by `PyUp.io <https://pyup.io/>`_
+        
         
         =======
         History
         =======
         
         0.1.0 (2019-06-16)
         ------------------
```

### Comparing `kubesplit-0.3.1/README.rst` & `kubesplit-0.3.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -34,7 +34,12 @@
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+Acknowledgements
+----------------
+
+- Dependencies scanned by `PyUp.io <https://pyup.io/>`_
```

### Comparing `kubesplit-0.3.1/docs/Makefile` & `kubesplit-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/docs/conf.py` & `kubesplit-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/docs/installation.rst` & `kubesplit-0.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/kubesplit/args.py` & `kubesplit-0.3.2/kubesplit/args.py`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/kubesplit/config.py` & `kubesplit-0.3.2/kubesplit/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 def get_io_config_from_args(
     args: Namespace, show_version: bool
 ) -> KubesplitIOConfig:
     """Build a KubesplitIOConfig from parsed args."""
     input_display_name = "STDIN"
-    if args.input is None:
+    if args.input is None or args.input == "-":
         f_input = None
     else:
         f_input = args.input
         input_display_name = f_input
     if show_version:
         output_dir = None
     else:
```

### Comparing `kubesplit-0.3.1/kubesplit/convert.py` & `kubesplit-0.3.2/kubesplit/convert.py`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/kubesplit/k8s_descriptor.py` & `kubesplit-0.3.2/kubesplit/k8s_descriptor.py`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/kubesplit/kubesplit.py` & `kubesplit-0.3.2/kubesplit/kubesplit.py`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/kubesplit/namespaces.py` & `kubesplit-0.3.2/kubesplit/namespaces.py`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/kubesplit/output.py` & `kubesplit-0.3.2/kubesplit/output.py`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/kubesplit.egg-info/PKG-INFO` & `kubesplit-0.3.2/kubesplit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kubesplit
-Version: 0.3.1
+Version: 0.3.2
 Summary: Split multidoc yaml formatted kubernetes descriptors to a set         of single resource files
 Home-page: https://github.com/looztra/kubesplit
 Author: Christophe Furmaniak
 Author-email: christophe.furmaniak@gmail.com
 License: Apache Software License 2.0
 Description: =========
         kubesplit
@@ -43,14 +43,19 @@
         -------
         
         This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
         
         .. _Cookiecutter: https://github.com/audreyr/cookiecutter
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         
+        Acknowledgements
+        ----------------
+        
+        - Dependencies scanned by `PyUp.io <https://pyup.io/>`_
+        
         
         =======
         History
         =======
         
         0.1.0 (2019-06-16)
         ------------------
```

### Comparing `kubesplit-0.3.1/kubesplit.egg-info/SOURCES.txt` & `kubesplit-0.3.2/kubesplit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/setup.py` & `kubesplit-0.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,10 +54,10 @@
     packages=find_packages(include=["kubesplit"]),
     python_requires=">=3.6",
     entry_points={"console_scripts": ["kubesplit = kubesplit.__main__:main"]},
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/looztra/kubesplit",
-    version="0.3.1",
+    version="0.3.2",
     zip_safe=False,
 )
```

### Comparing `kubesplit-0.3.1/tests/test_convert.py` & `kubesplit-0.3.2/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/tests/test_k8s_descriptor.py` & `kubesplit-0.3.2/tests/test_k8s_descriptor.py`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/tests/test_namespaces.py` & `kubesplit-0.3.2/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `kubesplit-0.3.1/tests/test_output.py` & `kubesplit-0.3.2/tests/test_output.py`

 * *Files identical despite different names*

