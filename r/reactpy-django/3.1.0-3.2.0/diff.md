# Comparing `tmp/reactpy_django-3.1.0.tar.gz` & `tmp/reactpy_django-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactpy_django-3.1.0.tar", last modified: Sun May  7 04:47:31 2023, max compression
+gzip compressed data, was "reactpy_django-3.2.0.tar", last modified: Fri Jun 23 22:41:39 2023, max compression
```

## Comparing `reactpy_django-3.1.0.tar` & `reactpy_django-3.2.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.828732 reactpy_django-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.832732 reactpy_django-3.1.0/src/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.832732 reactpy_django-3.1.0/src/reactpy_django/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/http/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/http/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.832732 reactpy_django-3.1.0/src/reactpy_django/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.828732 reactpy_django-3.1.0/src/reactpy_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/src/reactpy_django/static/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (123)   166388 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django/static/reactpy_django/client.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.828732 reactpy_django-3.1.0/src/reactpy_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/src/reactpy_django/templates/reactpy/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/templates/reactpy/component.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/src/reactpy_django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/templatetags/reactpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13388 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.836732 reactpy_django-3.1.0/src/reactpy_django/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/websocket/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-07 04:46:52.000000 reactpy_django-3.1.0/src/reactpy_django/websocket/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:31.832732 reactpy_django-3.1.0/src/reactpy_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:47:24.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 04:47:31.000000 reactpy_django-3.1.0/src/reactpy_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-23 22:41:39.994863 reactpy_django-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.986863 reactpy_django-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/http/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/http/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.986863 reactpy_django-3.2.0/src/reactpy_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/static/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (123)   166388 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django/static/reactpy_django/client.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.986863 reactpy_django-3.2.0/src/reactpy_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/templates/reactpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/templates/reactpy/component.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/templatetags/reactpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13908 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/websocket/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/websocket/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:41:33.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/top_level.txt
```

### Comparing `reactpy_django-3.1.0/LICENSE` & `reactpy_django-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/PKG-INFO` & `reactpy_django-3.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy_django
-Version: 3.1.0
+Version: 3.2.0
 Summary: Control the web with Python
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
@@ -24,15 +24,31 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <img src="https://raw.githubusercontent.com/reactive-python/reactpy/main/branding/svg/reactpy-logo-square.svg" align="left" height="45"/> ReactPy Django
 
 <!--badge-start-->
 
-[![Tests](https://github.com/reactive-python/reactpy-django/workflows/Test/badge.svg?event=push)](https://github.com/reactive-python/reactpy-django/actions?query=workflow%3ATest) [![PyPI Version](https://img.shields.io/pypi/v/reactpy-django.svg?label=PyPI)](https://pypi.python.org/pypi/reactpy-django) [![License](https://img.shields.io/badge/License-MIT-purple.svg)](https://github.com/reactive-python/reactpy-django/blob/main/LICENSE) [![Docs](https://img.shields.io/website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-python.github.io%2Freactpy-django%2F)](https://reactive-python.github.io/reactpy-django/)
+<p>
+    <a href="https://github.com/reactive-python/reactpy-django/actions?query=workflow%3ATest">
+        <img src="https://github.com/reactive-python/reactpy-django/workflows/Test/badge.svg?event=push">
+    </a>
+    <a href="https://pypi.python.org/pypi/reactpy-django">
+        <img src="https://img.shields.io/pypi/v/reactpy-django.svg?label=PyPI">
+    </a>
+    <a href="https://github.com/reactive-python/reactpy/blob/main/LICENSE">
+        <img src="https://img.shields.io/badge/License-MIT-purple.svg">
+    </a>
+    <a href="https://reactive-python.github.io/reactpy-django/">
+        <img src="https://img.shields.io/website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-python.github.io%2Freactpy-django%2F">
+    </a>
+    <a href="https://discord.gg/uNb5P4hA9X">
+        <img src="https://img.shields.io/discord/1111078259854168116?label=Discord&logo=discord">
+    </a>
+</p>
 
 <!--badge-end-->
 <!--intro-start-->
 
 [ReactPy](https://reactpy.dev/) is a library for building user interfaces in Python without Javascript. ReactPy interfaces are made from components that look and behave similar to those found in [ReactJS](https://reactjs.org/). Designed with simplicity in mind, ReactPy can be used by those without web development experience while also being powerful enough to grow with your ambitions.
 
 <table align="center">
@@ -108,14 +124,15 @@
 
 # Resources
 
 <!--resources-start-->
 
 Follow the links below to find out more about this project.
 
--   [Try it Now](https://mybinder.org/v2/gh/reactive-python/reactpy-jupyter/main?urlpath=lab/tree/notebooks/introduction.ipynb) - check out ReactPy in a Jupyter Notebook.
--   [Documentation](https://reactive-python.github.io/reactpy-django) - learn how to install, run, and use ReactPy.
--   [Community Forum](https://github.com/reactive-python/reactpy/discussions) - ask questions, share ideas, and show off projects.
--   [Contributor Guide](https://reactive-python.github.io/reactpy-django/contribute/code/) - see how you can help develop this project.
--   [Code of Conduct](https://github.com/reactive-python/reactpy-django/blob/main/CODE_OF_CONDUCT.md) - standards for interacting with this community.
+-   [Try ReactPy (Jupyter Notebook)](https://mybinder.org/v2/gh/reactive-python/reactpy-jupyter/main?urlpath=lab/tree/notebooks/introduction.ipynb)
+-   [Documentation](https://reactive-python.github.io/reactpy-django)
+-   [GitHub Discussions](https://github.com/reactive-python/reactpy-django/discussions)
+-   [Discord](https://discord.gg/uNb5P4hA9X)
+-   [Contributor Guide](https://reactive-python.github.io/reactpy-django/contribute/code/)
+-   [Code of Conduct](https://github.com/reactive-python/reactpy-django/blob/main/CODE_OF_CONDUCT.md)
 
 <!--resources-end-->
```

#### html2text {}

```diff
@@ -1,35 +1,33 @@
-Metadata-Version: 2.1 Name: reactpy_django Version: 3.1.0 Summary: Control the
+Metadata-Version: 2.1 Name: reactpy_django Version: 3.2.0 Summary: Control the
 web with Python Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead Author-email: ryan.morshead@gmail.com License: MIT
 Keywords: interactive,widgets,DOM,React Platform: Linux Platform: Mac OS X
 Platform: Windows Classifier: Framework :: Django Classifier: Framework ::
 Django :: 4.0 Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Multimedia :: Graphics Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Environment ::
 Web Environment Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE # [https://raw.githubusercontent.com/reactive-python/
-reactpy/main/branding/svg/reactpy-logo-square.svg] ReactPy Django  [![Tests]
-(https://github.com/reactive-python/reactpy-django/workflows/Test/
-badge.svg?event=push)](https://github.com/reactive-python/reactpy-django/
-actions?query=workflow%3ATest) [![PyPI Version](https://img.shields.io/pypi/v/
-reactpy-django.svg?label=PyPI)](https://pypi.python.org/pypi/reactpy-django) [!
-[License](https://img.shields.io/badge/License-MIT-purple.svg)](https://
-github.com/reactive-python/reactpy-django/blob/main/LICENSE) [![Docs](https://
-img.shields.io/
+reactpy/main/branding/svg/reactpy-logo-square.svg] ReactPy Django
+[https://github.com/reactive-python/reactpy-django/workflows/Test/
+badge.svg?event=push] [https://img.shields.io/pypi/v/reactpy-
+django.svg?label=PyPI] [https://img.shields.io/badge/License-MIT-purple.svg]
+[https://img.shields.io/
 website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-
-python.github.io%2Freactpy-django%2F)](https://reactive-python.github.io/
-reactpy-django/)   [ReactPy](https://reactpy.dev/) is a library for building
-user interfaces in Python without Javascript. ReactPy interfaces are made from
-components that look and behave similar to those found in [ReactJS](https://
-reactjs.org/). Designed with simplicity in mind, ReactPy can be used by those
-without web development experience while also being powerful enough to grow
-with your ambitions.
+python.github.io%2Freactpy-django%2F] [https://img.shields.io/discord/
+1111078259854168116?label=Discord&logo=discord]
+  [ReactPy](https://reactpy.dev/) is a library for building user interfaces in
+Python without Javascript. ReactPy interfaces are made from components that
+look and behave similar to those found in [ReactJS](https://reactjs.org/).
+Designed with simplicity in mind, ReactPy can be used by those without web
+development experience while also being powerful enough to grow with your
+ambitions.
           Supported Backends
           Built-in                       External
           Flask,_FastAPI,_Sanic,_Tornado Django, Jupyter, Plotly-Dash
  # At a Glance ## `my_app/components.py`  You will need a file to define your
 [ReactPy](https://github.com/reactive-python/reactpy) components. We recommend
 creating a `components.py` file within your chosen **Django app** to start out.
 Within this file, we will create a simple `hello_world` component.   ```python
@@ -42,17 +40,15 @@
 you can pass in `args` and `kwargs` into your component function. For example,
 after reading the code below, pay attention to how the function definition for
 `hello_world` (_in the previous example_) accepts a `recipient` argument.
 ```jinja {% load reactpy %}
 {% component "example_project.my_app.components.hello_world" recipient="World"
 %}
 ```  # Resources  Follow the links below to find out more about this project. -
-[Try it Now](https://mybinder.org/v2/gh/reactive-python/reactpy-jupyter/
-main?urlpath=lab/tree/notebooks/introduction.ipynb) - check out ReactPy in a
-Jupyter Notebook. - [Documentation](https://reactive-python.github.io/reactpy-
-django) - learn how to install, run, and use ReactPy. - [Community Forum]
-(https://github.com/reactive-python/reactpy/discussions) - ask questions, share
-ideas, and show off projects. - [Contributor Guide](https://reactive-
-python.github.io/reactpy-django/contribute/code/) - see how you can help
-develop this project. - [Code of Conduct](https://github.com/reactive-python/
-reactpy-django/blob/main/CODE_OF_CONDUCT.md) - standards for interacting with
-this community.
+[Try ReactPy (Jupyter Notebook)](https://mybinder.org/v2/gh/reactive-python/
+reactpy-jupyter/main?urlpath=lab/tree/notebooks/introduction.ipynb) -
+[Documentation](https://reactive-python.github.io/reactpy-django) - [GitHub
+Discussions](https://github.com/reactive-python/reactpy-django/discussions) -
+[Discord](https://discord.gg/uNb5P4hA9X) - [Contributor Guide](https://
+reactive-python.github.io/reactpy-django/contribute/code/) - [Code of Conduct]
+(https://github.com/reactive-python/reactpy-django/blob/main/
+CODE_OF_CONDUCT.md)
```

### Comparing `reactpy_django-3.1.0/README.md` & `reactpy_django-3.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 # <img src="https://raw.githubusercontent.com/reactive-python/reactpy/main/branding/svg/reactpy-logo-square.svg" align="left" height="45"/> ReactPy Django
 
 <!--badge-start-->
 
-[![Tests](https://github.com/reactive-python/reactpy-django/workflows/Test/badge.svg?event=push)](https://github.com/reactive-python/reactpy-django/actions?query=workflow%3ATest) [![PyPI Version](https://img.shields.io/pypi/v/reactpy-django.svg?label=PyPI)](https://pypi.python.org/pypi/reactpy-django) [![License](https://img.shields.io/badge/License-MIT-purple.svg)](https://github.com/reactive-python/reactpy-django/blob/main/LICENSE) [![Docs](https://img.shields.io/website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-python.github.io%2Freactpy-django%2F)](https://reactive-python.github.io/reactpy-django/)
+<p>
+    <a href="https://github.com/reactive-python/reactpy-django/actions?query=workflow%3ATest">
+        <img src="https://github.com/reactive-python/reactpy-django/workflows/Test/badge.svg?event=push">
+    </a>
+    <a href="https://pypi.python.org/pypi/reactpy-django">
+        <img src="https://img.shields.io/pypi/v/reactpy-django.svg?label=PyPI">
+    </a>
+    <a href="https://github.com/reactive-python/reactpy/blob/main/LICENSE">
+        <img src="https://img.shields.io/badge/License-MIT-purple.svg">
+    </a>
+    <a href="https://reactive-python.github.io/reactpy-django/">
+        <img src="https://img.shields.io/website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-python.github.io%2Freactpy-django%2F">
+    </a>
+    <a href="https://discord.gg/uNb5P4hA9X">
+        <img src="https://img.shields.io/discord/1111078259854168116?label=Discord&logo=discord">
+    </a>
+</p>
 
 <!--badge-end-->
 <!--intro-start-->
 
 [ReactPy](https://reactpy.dev/) is a library for building user interfaces in Python without Javascript. ReactPy interfaces are made from components that look and behave similar to those found in [ReactJS](https://reactjs.org/). Designed with simplicity in mind, ReactPy can be used by those without web development experience while also being powerful enough to grow with your ambitions.
 
 <table align="center">
@@ -82,14 +98,15 @@
 
 # Resources
 
 <!--resources-start-->
 
 Follow the links below to find out more about this project.
 
--   [Try it Now](https://mybinder.org/v2/gh/reactive-python/reactpy-jupyter/main?urlpath=lab/tree/notebooks/introduction.ipynb) - check out ReactPy in a Jupyter Notebook.
--   [Documentation](https://reactive-python.github.io/reactpy-django) - learn how to install, run, and use ReactPy.
--   [Community Forum](https://github.com/reactive-python/reactpy/discussions) - ask questions, share ideas, and show off projects.
--   [Contributor Guide](https://reactive-python.github.io/reactpy-django/contribute/code/) - see how you can help develop this project.
--   [Code of Conduct](https://github.com/reactive-python/reactpy-django/blob/main/CODE_OF_CONDUCT.md) - standards for interacting with this community.
+-   [Try ReactPy (Jupyter Notebook)](https://mybinder.org/v2/gh/reactive-python/reactpy-jupyter/main?urlpath=lab/tree/notebooks/introduction.ipynb)
+-   [Documentation](https://reactive-python.github.io/reactpy-django)
+-   [GitHub Discussions](https://github.com/reactive-python/reactpy-django/discussions)
+-   [Discord](https://discord.gg/uNb5P4hA9X)
+-   [Contributor Guide](https://reactive-python.github.io/reactpy-django/contribute/code/)
+-   [Code of Conduct](https://github.com/reactive-python/reactpy-django/blob/main/CODE_OF_CONDUCT.md)
 
 <!--resources-end-->
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
 # [https://raw.githubusercontent.com/reactive-python/reactpy/main/branding/svg/
-reactpy-logo-square.svg] ReactPy Django  [![Tests](https://github.com/reactive-
-python/reactpy-django/workflows/Test/badge.svg?event=push)](https://github.com/
-reactive-python/reactpy-django/actions?query=workflow%3ATest) [![PyPI Version]
-(https://img.shields.io/pypi/v/reactpy-django.svg?label=PyPI)](https://
-pypi.python.org/pypi/reactpy-django) [![License](https://img.shields.io/badge/
-License-MIT-purple.svg)](https://github.com/reactive-python/reactpy-django/
-blob/main/LICENSE) [![Docs](https://img.shields.io/
+reactpy-logo-square.svg] ReactPy Django
+[https://github.com/reactive-python/reactpy-django/workflows/Test/
+badge.svg?event=push] [https://img.shields.io/pypi/v/reactpy-
+django.svg?label=PyPI] [https://img.shields.io/badge/License-MIT-purple.svg]
+[https://img.shields.io/
 website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-
-python.github.io%2Freactpy-django%2F)](https://reactive-python.github.io/
-reactpy-django/)   [ReactPy](https://reactpy.dev/) is a library for building
-user interfaces in Python without Javascript. ReactPy interfaces are made from
-components that look and behave similar to those found in [ReactJS](https://
-reactjs.org/). Designed with simplicity in mind, ReactPy can be used by those
-without web development experience while also being powerful enough to grow
-with your ambitions.
+python.github.io%2Freactpy-django%2F] [https://img.shields.io/discord/
+1111078259854168116?label=Discord&logo=discord]
+  [ReactPy](https://reactpy.dev/) is a library for building user interfaces in
+Python without Javascript. ReactPy interfaces are made from components that
+look and behave similar to those found in [ReactJS](https://reactjs.org/).
+Designed with simplicity in mind, ReactPy can be used by those without web
+development experience while also being powerful enough to grow with your
+ambitions.
           Supported Backends
           Built-in                       External
           Flask,_FastAPI,_Sanic,_Tornado Django, Jupyter, Plotly-Dash
  # At a Glance ## `my_app/components.py`  You will need a file to define your
 [ReactPy](https://github.com/reactive-python/reactpy) components. We recommend
 creating a `components.py` file within your chosen **Django app** to start out.
 Within this file, we will create a simple `hello_world` component.   ```python
@@ -30,17 +29,15 @@
 you can pass in `args` and `kwargs` into your component function. For example,
 after reading the code below, pay attention to how the function definition for
 `hello_world` (_in the previous example_) accepts a `recipient` argument.
 ```jinja {% load reactpy %}
 {% component "example_project.my_app.components.hello_world" recipient="World"
 %}
 ```  # Resources  Follow the links below to find out more about this project. -
-[Try it Now](https://mybinder.org/v2/gh/reactive-python/reactpy-jupyter/
-main?urlpath=lab/tree/notebooks/introduction.ipynb) - check out ReactPy in a
-Jupyter Notebook. - [Documentation](https://reactive-python.github.io/reactpy-
-django) - learn how to install, run, and use ReactPy. - [Community Forum]
-(https://github.com/reactive-python/reactpy/discussions) - ask questions, share
-ideas, and show off projects. - [Contributor Guide](https://reactive-
-python.github.io/reactpy-django/contribute/code/) - see how you can help
-develop this project. - [Code of Conduct](https://github.com/reactive-python/
-reactpy-django/blob/main/CODE_OF_CONDUCT.md) - standards for interacting with
-this community.
+[Try ReactPy (Jupyter Notebook)](https://mybinder.org/v2/gh/reactive-python/
+reactpy-jupyter/main?urlpath=lab/tree/notebooks/introduction.ipynb) -
+[Documentation](https://reactive-python.github.io/reactpy-django) - [GitHub
+Discussions](https://github.com/reactive-python/reactpy-django/discussions) -
+[Discord](https://discord.gg/uNb5P4hA9X) - [Contributor Guide](https://
+reactive-python.github.io/reactpy-django/contribute/code/) - [Code of Conduct]
+(https://github.com/reactive-python/reactpy-django/blob/main/
+CODE_OF_CONDUCT.md)
```

### Comparing `reactpy_django-3.1.0/pyproject.toml` & `reactpy_django-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/setup.py` & `reactpy_django-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/src/reactpy_django/components.py` & `reactpy_django-3.2.0/src/reactpy_django/components.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/src/reactpy_django/config.py` & `reactpy_django-3.2.0/src/reactpy_django/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,7 +46,12 @@
         getattr(
             settings,
             "REACTPY_DEFAULT_QUERY_POSTPROCESSOR",
             "reactpy_django.utils.django_query_postprocessor",
         )
     )
 )
+REACTPY_AUTH_BACKEND: str | None = getattr(
+    settings,
+    "REACTPY_AUTH_BACKEND",
+    None,
+)
```

### Comparing `reactpy_django-3.1.0/src/reactpy_django/decorators.py` & `reactpy_django-3.2.0/src/reactpy_django/decorators.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/src/reactpy_django/hooks.py` & `reactpy_django-3.2.0/src/reactpy_django/hooks.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/src/reactpy_django/http/views.py` & `reactpy_django-3.2.0/src/reactpy_django/http/views.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/src/reactpy_django/migrations/0001_initial.py` & `reactpy_django-3.2.0/src/reactpy_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py` & `reactpy_django-3.2.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/src/reactpy_django/static/reactpy_django/client.js` & `reactpy_django-3.2.0/src/reactpy_django/static/reactpy_django/client.js`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/src/reactpy_django/templatetags/reactpy.py` & `reactpy_django-3.2.0/src/reactpy_django/templatetags/reactpy.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/src/reactpy_django/types.py` & `reactpy_django-3.2.0/src/reactpy_django/types.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.1.0/src/reactpy_django/utils.py` & `reactpy_django-3.2.0/src/reactpy_django/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,17 +309,23 @@
 
     return f"reactpy_django:{':'.join(str(arg) for arg in args)}"
 
 
 def db_cleanup(immediate: bool = False):
     """Deletes expired component sessions from the database.
     This function may be expanded in the future to include additional cleanup tasks."""
-    from .config import REACTPY_CACHE, REACTPY_DATABASE, REACTPY_RECONNECT_MAX
+    from .config import (
+        REACTPY_CACHE,
+        REACTPY_DATABASE,
+        REACTPY_DEBUG_MODE,
+        REACTPY_RECONNECT_MAX,
+    )
     from .models import ComponentSession
 
+    clean_started_at = datetime.now()
     cache_key: str = create_cache_key("last_cleaned")
     now_str: str = datetime.strftime(timezone.now(), DATE_FORMAT)
     cleaned_at_str: str = caches[REACTPY_CACHE].get(cache_key)
     cleaned_at: datetime = timezone.make_aware(
         datetime.strptime(cleaned_at_str or now_str, DATE_FORMAT)
     )
     clean_needed_by = cleaned_at + timedelta(seconds=REACTPY_RECONNECT_MAX)
@@ -336,7 +342,16 @@
     # Delete expired component parameters
     # Use timestamps in cache (`cleaned_at_str`) as a no-dependency rate limiter
     if immediate or not cleaned_at_str or timezone.now() >= clean_needed_by:
         ComponentSession.objects.using(REACTPY_DATABASE).filter(
             last_accessed__lte=expires_by
         ).delete()
         caches[REACTPY_CACHE].set(cache_key, now_str, timeout=None)
+
+    # Check if cleaning took abnormally long
+    clean_duration = datetime.now() - clean_started_at
+    if REACTPY_DEBUG_MODE and clean_duration.total_seconds() > 1:
+        _logger.warning(
+            "ReactPy has taken %s seconds to clean up expired component sessions. "
+            "This may indicate a performance issue with your system, cache, or database.",
+            clean_duration.total_seconds(),
+        )
```

### Comparing `reactpy_django-3.1.0/src/reactpy_django/websocket/consumer.py` & `reactpy_django-3.2.0/src/reactpy_django/websocket/consumer.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,43 +23,63 @@
 _logger = logging.getLogger(__name__)
 
 
 class ReactpyAsyncWebsocketConsumer(AsyncJsonWebsocketConsumer):
     """Communicates with the browser to perform actions on-demand."""
 
     async def connect(self) -> None:
-        from django.contrib.auth.models import AbstractBaseUser
-
+        """The browser has connected."""
         await super().connect()
 
-        user: AbstractBaseUser = self.scope.get("user")
+        # Authenticate the user, if possible
+        from reactpy_django.config import REACTPY_AUTH_BACKEND
+
+        user: Any = self.scope.get("user")
         if user and user.is_authenticated:
             try:
-                await login(self.scope, user)
-                await database_sync_to_async(self.scope["session"].save)()
+                await login(self.scope, user, backend=REACTPY_AUTH_BACKEND)
             except Exception:
                 _logger.exception("ReactPy websocket authentication has failed!")
         elif user is None:
-            _logger.warning("ReactPy websocket is missing AuthMiddlewareStack!")
+            _logger.debug(
+                "ReactPy websocket is missing AuthMiddlewareStack! "
+                "Users will not be accessible within `use_scope` or `use_websocket`!"
+            )
+
+        # Save the session, if possible
+        if self.scope.get("session"):
+            try:
+                await database_sync_to_async(self.scope["session"].save)()
+            except Exception:
+                _logger.exception("ReactPy has failed to save scope['session']!")
+        else:
+            _logger.debug(
+                "ReactPy websocket is missing SessionMiddlewareStack! "
+                "Sessions will not be accessible within `use_scope` or `use_websocket`!"
+            )
 
+        # Start allowing component renders
         self._reactpy_dispatcher_future = asyncio.ensure_future(
             self._run_dispatch_loop()
         )
 
     async def disconnect(self, code: int) -> None:
+        """The browser has disconnected."""
         if self._reactpy_dispatcher_future.done():
             await self._reactpy_dispatcher_future
         else:
             self._reactpy_dispatcher_future.cancel()
         await super().disconnect(code)
 
     async def receive_json(self, content: Any, **_) -> None:
+        """Receive a message from the browser. Typically messages are event signals."""
         await self._reactpy_recv_queue.put(content)
 
     async def _run_dispatch_loop(self):
+        """Runs the main loop that performs component rendering tasks."""
         from reactpy_django import models
         from reactpy_django.config import (
             REACTPY_DATABASE,
             REACTPY_RECONNECT_MAX,
             REACTPY_REGISTERED_COMPONENTS,
         )
 
@@ -73,15 +93,15 @@
             location=Location(
                 pathname=scope["path"],
                 search=f"?{search}" if (search and (search != "undefined")) else "",
             ),
             carrier=ComponentWebsocket(self.close, self.disconnect, dotted_path),
         )
         now = timezone.now()
-        component_args: Sequence[Any] = tuple()
+        component_args: Sequence[Any] = ()
         component_kwargs: MutableMapping[str, Any] = {}
 
         # Verify the component has already been registered
         try:
             component_constructor = REACTPY_REGISTERED_COMPONENTS[dotted_path]
         except KeyError:
             _logger.warning(
@@ -126,15 +146,15 @@
         except Exception:
             _logger.exception(
                 f"Failed to construct component {component_constructor} "
                 f"with parameters {component_kwargs}"
             )
             return
 
-        # Begin serving the ReactPy component
+        # Start the ReactPy component rendering loop
         try:
             await serve_layout(
                 Layout(ConnectionContext(component_instance, value=connection)),
                 self.send_json,
                 self._reactpy_recv_queue.get,
             )
         except Exception:
```

### Comparing `reactpy_django-3.1.0/src/reactpy_django.egg-info/PKG-INFO` & `reactpy_django-3.2.0/src/reactpy_django.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy-django
-Version: 3.1.0
+Version: 3.2.0
 Summary: Control the web with Python
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
@@ -24,15 +24,31 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <img src="https://raw.githubusercontent.com/reactive-python/reactpy/main/branding/svg/reactpy-logo-square.svg" align="left" height="45"/> ReactPy Django
 
 <!--badge-start-->
 
-[![Tests](https://github.com/reactive-python/reactpy-django/workflows/Test/badge.svg?event=push)](https://github.com/reactive-python/reactpy-django/actions?query=workflow%3ATest) [![PyPI Version](https://img.shields.io/pypi/v/reactpy-django.svg?label=PyPI)](https://pypi.python.org/pypi/reactpy-django) [![License](https://img.shields.io/badge/License-MIT-purple.svg)](https://github.com/reactive-python/reactpy-django/blob/main/LICENSE) [![Docs](https://img.shields.io/website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-python.github.io%2Freactpy-django%2F)](https://reactive-python.github.io/reactpy-django/)
+<p>
+    <a href="https://github.com/reactive-python/reactpy-django/actions?query=workflow%3ATest">
+        <img src="https://github.com/reactive-python/reactpy-django/workflows/Test/badge.svg?event=push">
+    </a>
+    <a href="https://pypi.python.org/pypi/reactpy-django">
+        <img src="https://img.shields.io/pypi/v/reactpy-django.svg?label=PyPI">
+    </a>
+    <a href="https://github.com/reactive-python/reactpy/blob/main/LICENSE">
+        <img src="https://img.shields.io/badge/License-MIT-purple.svg">
+    </a>
+    <a href="https://reactive-python.github.io/reactpy-django/">
+        <img src="https://img.shields.io/website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-python.github.io%2Freactpy-django%2F">
+    </a>
+    <a href="https://discord.gg/uNb5P4hA9X">
+        <img src="https://img.shields.io/discord/1111078259854168116?label=Discord&logo=discord">
+    </a>
+</p>
 
 <!--badge-end-->
 <!--intro-start-->
 
 [ReactPy](https://reactpy.dev/) is a library for building user interfaces in Python without Javascript. ReactPy interfaces are made from components that look and behave similar to those found in [ReactJS](https://reactjs.org/). Designed with simplicity in mind, ReactPy can be used by those without web development experience while also being powerful enough to grow with your ambitions.
 
 <table align="center">
@@ -108,14 +124,15 @@
 
 # Resources
 
 <!--resources-start-->
 
 Follow the links below to find out more about this project.
 
--   [Try it Now](https://mybinder.org/v2/gh/reactive-python/reactpy-jupyter/main?urlpath=lab/tree/notebooks/introduction.ipynb) - check out ReactPy in a Jupyter Notebook.
--   [Documentation](https://reactive-python.github.io/reactpy-django) - learn how to install, run, and use ReactPy.
--   [Community Forum](https://github.com/reactive-python/reactpy/discussions) - ask questions, share ideas, and show off projects.
--   [Contributor Guide](https://reactive-python.github.io/reactpy-django/contribute/code/) - see how you can help develop this project.
--   [Code of Conduct](https://github.com/reactive-python/reactpy-django/blob/main/CODE_OF_CONDUCT.md) - standards for interacting with this community.
+-   [Try ReactPy (Jupyter Notebook)](https://mybinder.org/v2/gh/reactive-python/reactpy-jupyter/main?urlpath=lab/tree/notebooks/introduction.ipynb)
+-   [Documentation](https://reactive-python.github.io/reactpy-django)
+-   [GitHub Discussions](https://github.com/reactive-python/reactpy-django/discussions)
+-   [Discord](https://discord.gg/uNb5P4hA9X)
+-   [Contributor Guide](https://reactive-python.github.io/reactpy-django/contribute/code/)
+-   [Code of Conduct](https://github.com/reactive-python/reactpy-django/blob/main/CODE_OF_CONDUCT.md)
 
 <!--resources-end-->
```

#### html2text {}

```diff
@@ -1,35 +1,33 @@
-Metadata-Version: 2.1 Name: reactpy-django Version: 3.1.0 Summary: Control the
+Metadata-Version: 2.1 Name: reactpy-django Version: 3.2.0 Summary: Control the
 web with Python Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead Author-email: ryan.morshead@gmail.com License: MIT
 Keywords: interactive,widgets,DOM,React Platform: Linux Platform: Mac OS X
 Platform: Windows Classifier: Framework :: Django Classifier: Framework ::
 Django :: 4.0 Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Multimedia :: Graphics Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Environment ::
 Web Environment Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE # [https://raw.githubusercontent.com/reactive-python/
-reactpy/main/branding/svg/reactpy-logo-square.svg] ReactPy Django  [![Tests]
-(https://github.com/reactive-python/reactpy-django/workflows/Test/
-badge.svg?event=push)](https://github.com/reactive-python/reactpy-django/
-actions?query=workflow%3ATest) [![PyPI Version](https://img.shields.io/pypi/v/
-reactpy-django.svg?label=PyPI)](https://pypi.python.org/pypi/reactpy-django) [!
-[License](https://img.shields.io/badge/License-MIT-purple.svg)](https://
-github.com/reactive-python/reactpy-django/blob/main/LICENSE) [![Docs](https://
-img.shields.io/
+reactpy/main/branding/svg/reactpy-logo-square.svg] ReactPy Django
+[https://github.com/reactive-python/reactpy-django/workflows/Test/
+badge.svg?event=push] [https://img.shields.io/pypi/v/reactpy-
+django.svg?label=PyPI] [https://img.shields.io/badge/License-MIT-purple.svg]
+[https://img.shields.io/
 website?down_message=offline&label=Docs&logo=read%20the%20docs&logoColor=white&up_message=online&url=https%3A%2F%2Freactive-
-python.github.io%2Freactpy-django%2F)](https://reactive-python.github.io/
-reactpy-django/)   [ReactPy](https://reactpy.dev/) is a library for building
-user interfaces in Python without Javascript. ReactPy interfaces are made from
-components that look and behave similar to those found in [ReactJS](https://
-reactjs.org/). Designed with simplicity in mind, ReactPy can be used by those
-without web development experience while also being powerful enough to grow
-with your ambitions.
+python.github.io%2Freactpy-django%2F] [https://img.shields.io/discord/
+1111078259854168116?label=Discord&logo=discord]
+  [ReactPy](https://reactpy.dev/) is a library for building user interfaces in
+Python without Javascript. ReactPy interfaces are made from components that
+look and behave similar to those found in [ReactJS](https://reactjs.org/).
+Designed with simplicity in mind, ReactPy can be used by those without web
+development experience while also being powerful enough to grow with your
+ambitions.
           Supported Backends
           Built-in                       External
           Flask,_FastAPI,_Sanic,_Tornado Django, Jupyter, Plotly-Dash
  # At a Glance ## `my_app/components.py`  You will need a file to define your
 [ReactPy](https://github.com/reactive-python/reactpy) components. We recommend
 creating a `components.py` file within your chosen **Django app** to start out.
 Within this file, we will create a simple `hello_world` component.   ```python
@@ -42,17 +40,15 @@
 you can pass in `args` and `kwargs` into your component function. For example,
 after reading the code below, pay attention to how the function definition for
 `hello_world` (_in the previous example_) accepts a `recipient` argument.
 ```jinja {% load reactpy %}
 {% component "example_project.my_app.components.hello_world" recipient="World"
 %}
 ```  # Resources  Follow the links below to find out more about this project. -
-[Try it Now](https://mybinder.org/v2/gh/reactive-python/reactpy-jupyter/
-main?urlpath=lab/tree/notebooks/introduction.ipynb) - check out ReactPy in a
-Jupyter Notebook. - [Documentation](https://reactive-python.github.io/reactpy-
-django) - learn how to install, run, and use ReactPy. - [Community Forum]
-(https://github.com/reactive-python/reactpy/discussions) - ask questions, share
-ideas, and show off projects. - [Contributor Guide](https://reactive-
-python.github.io/reactpy-django/contribute/code/) - see how you can help
-develop this project. - [Code of Conduct](https://github.com/reactive-python/
-reactpy-django/blob/main/CODE_OF_CONDUCT.md) - standards for interacting with
-this community.
+[Try ReactPy (Jupyter Notebook)](https://mybinder.org/v2/gh/reactive-python/
+reactpy-jupyter/main?urlpath=lab/tree/notebooks/introduction.ipynb) -
+[Documentation](https://reactive-python.github.io/reactpy-django) - [GitHub
+Discussions](https://github.com/reactive-python/reactpy-django/discussions) -
+[Discord](https://discord.gg/uNb5P4hA9X) - [Contributor Guide](https://
+reactive-python.github.io/reactpy-django/contribute/code/) - [Code of Conduct]
+(https://github.com/reactive-python/reactpy-django/blob/main/
+CODE_OF_CONDUCT.md)
```

### Comparing `reactpy_django-3.1.0/src/reactpy_django.egg-info/SOURCES.txt` & `reactpy_django-3.2.0/src/reactpy_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

