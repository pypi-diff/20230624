# Comparing `tmp/mini_set-0.1.0.tar.gz` & `tmp/mini_set-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_set-0.1.0.tar", max compression
+gzip compressed data, was "mini_set-0.1.1.tar", max compression
```

## Comparing `mini_set-0.1.0.tar` & `mini_set-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-04-09 08:08:56.485842 mini_set-0.1.0/LICENSE
--rw-r--r--   0        0        0      540 2023-04-09 08:08:56.485842 mini_set-0.1.0/README.md
--rw-r--r--   0        0        0      193 2023-04-09 08:08:56.489842 mini_set-0.1.0/miniset/__init__.py
--rw-r--r--   0        0        0     1246 2023-04-09 08:08:56.489842 mini_set-0.1.0/miniset/exceptions.py
--rw-r--r--   0        0        0     3049 2023-04-09 08:08:56.489842 mini_set-0.1.0/miniset/extensions.py
--rw-r--r--   0        0        0     2470 2023-04-09 08:08:56.489842 mini_set-0.1.0/miniset/filters.py
--rw-r--r--   0        0        0     4816 2023-04-09 08:08:56.489842 mini_set-0.1.0/miniset/jinja_context.py
--rw-r--r--   0        0        0      164 2023-04-09 08:08:56.489842 mini_set-0.1.0/miniset/types.py
--rw-r--r--   0        0        0     1290 2023-04-09 08:09:15.210082 mini_set-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1297 1970-01-01 00:00:00.000000 mini_set-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-24 00:44:59.163906 mini_set-0.1.1/LICENSE
+-rw-r--r--   0        0        0      540 2023-06-24 00:44:59.163906 mini_set-0.1.1/README.md
+-rw-r--r--   0        0        0      193 2023-06-24 00:44:59.163906 mini_set-0.1.1/miniset/__init__.py
+-rw-r--r--   0        0        0     1246 2023-06-24 00:44:59.163906 mini_set-0.1.1/miniset/exceptions.py
+-rw-r--r--   0        0        0     3049 2023-06-24 00:44:59.163906 mini_set-0.1.1/miniset/extensions.py
+-rw-r--r--   0        0        0     2470 2023-06-24 00:44:59.163906 mini_set-0.1.1/miniset/filters.py
+-rw-r--r--   0        0        0     4816 2023-06-24 00:44:59.163906 mini_set-0.1.1/miniset/jinja_context.py
+-rw-r--r--   0        0        0      164 2023-06-24 00:44:59.163906 mini_set-0.1.1/miniset/types.py
+-rw-r--r--   0        0        0     1234 2023-06-24 00:45:13.540121 mini_set-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 mini_set-0.1.1/PKG-INFO
```

### Comparing `mini_set-0.1.0/LICENSE` & `mini_set-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mini_set-0.1.0/README.md` & `mini_set-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mini_set-0.1.0/miniset/exceptions.py` & `mini_set-0.1.1/miniset/exceptions.py`

 * *Files identical despite different names*

### Comparing `mini_set-0.1.0/miniset/extensions.py` & `mini_set-0.1.1/miniset/extensions.py`

 * *Files identical despite different names*

### Comparing `mini_set-0.1.0/miniset/filters.py` & `mini_set-0.1.1/miniset/filters.py`

 * *Files identical despite different names*

### Comparing `mini_set-0.1.0/miniset/jinja_context.py` & `mini_set-0.1.1/miniset/jinja_context.py`

 * *Files identical despite different names*

### Comparing `mini_set-0.1.0/pyproject.toml` & `mini_set-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 [tool.poetry]
 name = "mini-set"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Jinja2 template processor for interacting with an SQL engine"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ninoseki/miniset"
 repository = "https://github.com/ninoseki/miniset"
 documentation = "https://ninoseki.github.io/miniset/"
 packages = [
     { include = "miniset" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 jinja2 = ">=3.1,<4.0"
-typing-extensions = ">=4.5,<5.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-mypy = "^1.2.0"
-pre-commit = "^3.2.2"
-pytest = "^7.2.2"
-pytest-pretty = "^1.2.0"
-pytest-randomly = "^3.12.0"
+black = "^23.3"
+mypy = "^1.4"
+pre-commit = "^3.3"
+pytest = "^7.4"
+pytest-pretty = "^1.2"
+pytest-randomly = "^3.12"
 sqlmodel = "^0.0.8"
+urllib3 = "^1.0"
 
 [tool.poetry.group.doc.dependencies]
-mkdocs = "^1.4.2"
-mkdocs-material = "^9.1.6"
-mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+mkdocs = "^1.4"
+mkdocs-material = "^9.1"
+mkdocstrings = {extras = ["python"], version = "^0.22"}
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.ruff]
 select = [
     "E",    # pycodestyle errors
     "W",    # pycodestyle warnings
     "F",    # pyflakes
-    # "I",    # isort
     "C",    # flake8-comprehensions
     "B",    # flake8-bugbear
     "T20",  # flake8-print
 ]
 ignore = [
     "E501",  # line too long, handled by black
 ]
```

### Comparing `mini_set-0.1.0/PKG-INFO` & `mini_set-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: mini-set
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Jinja2 template processor for interacting with an SQL engine
 Home-page: https://github.com/ninoseki/miniset
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (>=3.1,<4.0)
-Requires-Dist: typing-extensions (>=4.5,<5.0)
 Project-URL: Documentation, https://ninoseki.github.io/miniset/
 Project-URL: Repository, https://github.com/ninoseki/miniset
 Description-Content-Type: text/markdown
 
 # miniset
 
 [![PyPI version](https://badge.fury.io/py/mini-set.svg)](https://badge.fury.io/py/mini-set)
```

