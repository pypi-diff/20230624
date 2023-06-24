# Comparing `tmp/snok-0.0.8.tar.gz` & `tmp/snok-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snok-0.0.8.tar", last modified: Sat Jun 24 19:31:23 2023, max compression
+gzip compressed data, was "snok-0.0.9.tar", last modified: Sat Jun 24 19:40:45 2023, max compression
```

## Comparing `snok-0.0.8.tar` & `snok-0.0.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-24 19:31:00.000000 snok-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-24 19:31:23.545004 snok-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-24 19:31:00.000000 snok-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-24 19:31:00.000000 snok-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:31:23.545004 snok-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-24 19:31:00.000000 snok-0.0.8/snok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-24 19:31:00.000000 snok-0.0.8/snok/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-24 19:31:00.000000 snok-0.0.8/snok/const.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-24 19:31:00.000000 snok-0.0.8/snok/services/new.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.537005 snok-0.0.8/snok/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/templates/__app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/db.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/gunicorn_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/templates/__app/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/templates/__app/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/routers/snok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/templates/__app/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/services/snok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/snok/templates/__app_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_templates/_base.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_templates/_head.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/snok/templates/__app_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/snok/templates/__package/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/snok/templates/__package_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package_tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package_tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/snok/templates/__shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/_.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/_.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/_.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/_pyproject_toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-24 19:31:00.000000 snok-0.0.8/snok/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-24 19:31:00.000000 snok-0.0.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-24 19:31:00.000000 snok-0.0.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.709835 snok-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-24 19:40:23.000000 snok-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-06-24 19:40:45.709835 snok-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-24 19:40:23.000000 snok-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-24 19:40:23.000000 snok-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:40:45.709835 snok-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.701835 snok-0.0.9/snok/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-24 19:40:23.000000 snok-0.0.9/snok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-24 19:40:23.000000 snok-0.0.9/snok/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-24 19:40:23.000000 snok-0.0.9/snok/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.705835 snok-0.0.9/snok/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-24 19:40:23.000000 snok-0.0.9/snok/services/new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.701835 snok-0.0.9/snok/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.705835 snok-0.0.9/snok/templates/__app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app/gunicorn_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.705835 snok-0.0.9/snok/templates/__app/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.705835 snok-0.0.9/snok/templates/__app/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app/routers/snok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.705835 snok-0.0.9/snok/templates/__app/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app/services/snok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.705835 snok-0.0.9/snok/templates/__app_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app_templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app_templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app_templates/_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app_templates/_head.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app_templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.705835 snok-0.0.9/snok/templates/__app_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__app_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.709835 snok-0.0.9/snok/templates/__package/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__package/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.709835 snok-0.0.9/snok/templates/__package_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__package_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__package_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__package_tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__package_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.709835 snok-0.0.9/snok/templates/__shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__shared/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__shared/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__shared/_.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__shared/_.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__shared/_.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__shared/_pyproject_toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:23.000000 snok-0.0.9/snok/templates/__shared/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-24 19:40:23.000000 snok-0.0.9/snok/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.705835 snok-0.0.9/snok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-06-24 19:40:45.000000 snok-0.0.9/snok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-24 19:40:45.000000 snok-0.0.9/snok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:40:45.000000 snok-0.0.9/snok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:40:45.000000 snok-0.0.9/snok.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-24 19:40:45.000000 snok-0.0.9/snok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-24 19:40:45.000000 snok-0.0.9/snok.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:40:45.709835 snok-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-24 19:40:23.000000 snok-0.0.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-24 19:40:23.000000 snok-0.0.9/tests/test_utils.py
```

### Comparing `snok-0.0.8/LICENSE` & `snok-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `snok-0.0.8/PKG-INFO` & `snok-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.8
+Version: 0.0.9
 Summary: 🚀 A simple, modern, full-stack toolkit for Python 🐍
 Author-email: Anthony Corletti <anthcor+snok@gmail.com>
 License: MIT
 Project-URL: Home, https://github.com/anthonycorletti/snok
 Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -59,15 +59,15 @@
 - Packaging with `setuptools`
 - Linting and formatting with `ruff` and `black`
 - Type checking with `mypy`
 - Testing with `pytest`
 
 ## 🤩 Coming Soon
 
-- Database integration with `pydantic` and `sqlmodel`
+- Database integration with `pydantic`, `sqlmodel`, and `alembic`
 - Web application generation with `fastapi` and `htmx`
 - Production ready deployment stacks with `nix`, `docker`, `skaffold` and `kustomize`
 - AI framework integrations with `pytorch` and `langchain`
 - Documentation site generation with `mkdocs`
 
 Check out the latest [issues](https://github.com/anthonycorletti/snok/issues) and [pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's coming soon!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snok Version: 0.0.8 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.9 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
@@ -20,25 +20,26 @@
 mind, snok is a Python toolkit for developers that focuses on making it simple
 and easy to build modern, full-stack applications, across web and AI
 frameworks. Snok is designed to leverage the best tools and packages that exist
 in the Python ecosystem in simple and easy to use workflows that accelerate
 development. ## ð Featuring - Package generation - Built-in dependency
 management - Packaging with `setuptools` - Linting and formatting with `ruff`
 and `black` - Type checking with `mypy` - Testing with `pytest` ## ð¤© Coming
-Soon - Database integration with `pydantic` and `sqlmodel` - Web application
-generation with `fastapi` and `htmx` - Production ready deployment stacks with
-`nix`, `docker`, `skaffold` and `kustomize` - AI framework integrations with
-`pytorch` and `langchain` - Documentation site generation with `mkdocs` Check
-out the latest [issues](https://github.com/anthonycorletti/snok/issues) and
-[pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's
-coming soon! ## ð Requirements - Python 3.11+ - `pip` ## âï¸ Installation
-After you've created your Python 3.11+ virtual environment in a new directory,
-install Snok: ```sh pip install snok ``` ## ð Getting Started Create a new
-package with: ```sh snok new mypackage ``` To install dependencies: ```sh snok
-install ``` To add a new dependency: ```sh snok add fastapi ``` To remove a
-dependency: ```sh snok remove fastapi ``` ## ð«¶ How can I help? - [â­ï¸
-Star snok on GitHub! â­ï¸](https://github.com/anthonycorletti/snok) - Open an
-[issue](https://github.com/anthonycorletti/snok/issues/new/choose) if you have
-a question, comment, feature request, or bug report. - Open a [pull request]
-(https://github.com/anthonycorletti/snok/compare) on GitHub. Contributions are
-encouraged and welcome! ## ð² Contact Reach out on [Twitter](https://
-twitter.com/anthonycorletti) if you'd like to get in touch!  
+Soon - Database integration with `pydantic`, `sqlmodel`, and `alembic` - Web
+application generation with `fastapi` and `htmx` - Production ready deployment
+stacks with `nix`, `docker`, `skaffold` and `kustomize` - AI framework
+integrations with `pytorch` and `langchain` - Documentation site generation
+with `mkdocs` Check out the latest [issues](https://github.com/anthonycorletti/
+snok/issues) and [pull requests](https://github.com/anthonycorletti/snok/pulls)
+to see what's coming soon! ## ð Requirements - Python 3.11+ - `pip` ##
+âï¸ Installation After you've created your Python 3.11+ virtual environment
+in a new directory, install Snok: ```sh pip install snok ``` ## ð Getting
+Started Create a new package with: ```sh snok new mypackage ``` To install
+dependencies: ```sh snok install ``` To add a new dependency: ```sh snok add
+fastapi ``` To remove a dependency: ```sh snok remove fastapi ``` ## ð«¶ How
+can I help? - [â­ï¸ Star snok on GitHub! â­ï¸](https://github.com/
+anthonycorletti/snok) - Open an [issue](https://github.com/anthonycorletti/
+snok/issues/new/choose) if you have a question, comment, feature request, or
+bug report. - Open a [pull request](https://github.com/anthonycorletti/snok/
+compare) on GitHub. Contributions are encouraged and welcome! ## ð² Contact
+Reach out on [Twitter](https://twitter.com/anthonycorletti) if you'd like to
+get in touch!
```

### Comparing `snok-0.0.8/README.md` & `snok-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 - Packaging with `setuptools`
 - Linting and formatting with `ruff` and `black`
 - Type checking with `mypy`
 - Testing with `pytest`
 
 ## 🤩 Coming Soon
 
-- Database integration with `pydantic` and `sqlmodel`
+- Database integration with `pydantic`, `sqlmodel`, and `alembic`
 - Web application generation with `fastapi` and `htmx`
 - Production ready deployment stacks with `nix`, `docker`, `skaffold` and `kustomize`
 - AI framework integrations with `pytorch` and `langchain`
 - Documentation site generation with `mkdocs`
 
 Check out the latest [issues](https://github.com/anthonycorletti/snok/issues) and [pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's coming soon!
```

#### html2text {}

```diff
@@ -14,25 +14,26 @@
 mind, snok is a Python toolkit for developers that focuses on making it simple
 and easy to build modern, full-stack applications, across web and AI
 frameworks. Snok is designed to leverage the best tools and packages that exist
 in the Python ecosystem in simple and easy to use workflows that accelerate
 development. ## ð Featuring - Package generation - Built-in dependency
 management - Packaging with `setuptools` - Linting and formatting with `ruff`
 and `black` - Type checking with `mypy` - Testing with `pytest` ## ð¤© Coming
-Soon - Database integration with `pydantic` and `sqlmodel` - Web application
-generation with `fastapi` and `htmx` - Production ready deployment stacks with
-`nix`, `docker`, `skaffold` and `kustomize` - AI framework integrations with
-`pytorch` and `langchain` - Documentation site generation with `mkdocs` Check
-out the latest [issues](https://github.com/anthonycorletti/snok/issues) and
-[pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's
-coming soon! ## ð Requirements - Python 3.11+ - `pip` ## âï¸ Installation
-After you've created your Python 3.11+ virtual environment in a new directory,
-install Snok: ```sh pip install snok ``` ## ð Getting Started Create a new
-package with: ```sh snok new mypackage ``` To install dependencies: ```sh snok
-install ``` To add a new dependency: ```sh snok add fastapi ``` To remove a
-dependency: ```sh snok remove fastapi ``` ## ð«¶ How can I help? - [â­ï¸
-Star snok on GitHub! â­ï¸](https://github.com/anthonycorletti/snok) - Open an
-[issue](https://github.com/anthonycorletti/snok/issues/new/choose) if you have
-a question, comment, feature request, or bug report. - Open a [pull request]
-(https://github.com/anthonycorletti/snok/compare) on GitHub. Contributions are
-encouraged and welcome! ## ð² Contact Reach out on [Twitter](https://
-twitter.com/anthonycorletti) if you'd like to get in touch!  
+Soon - Database integration with `pydantic`, `sqlmodel`, and `alembic` - Web
+application generation with `fastapi` and `htmx` - Production ready deployment
+stacks with `nix`, `docker`, `skaffold` and `kustomize` - AI framework
+integrations with `pytorch` and `langchain` - Documentation site generation
+with `mkdocs` Check out the latest [issues](https://github.com/anthonycorletti/
+snok/issues) and [pull requests](https://github.com/anthonycorletti/snok/pulls)
+to see what's coming soon! ## ð Requirements - Python 3.11+ - `pip` ##
+âï¸ Installation After you've created your Python 3.11+ virtual environment
+in a new directory, install Snok: ```sh pip install snok ``` ## ð Getting
+Started Create a new package with: ```sh snok new mypackage ``` To install
+dependencies: ```sh snok install ``` To add a new dependency: ```sh snok add
+fastapi ``` To remove a dependency: ```sh snok remove fastapi ``` ## ð«¶ How
+can I help? - [â­ï¸ Star snok on GitHub! â­ï¸](https://github.com/
+anthonycorletti/snok) - Open an [issue](https://github.com/anthonycorletti/
+snok/issues/new/choose) if you have a question, comment, feature request, or
+bug report. - Open a [pull request](https://github.com/anthonycorletti/snok/
+compare) on GitHub. Contributions are encouraged and welcome! ## ð² Contact
+Reach out on [Twitter](https://twitter.com/anthonycorletti) if you'd like to
+get in touch!
```

### Comparing `snok-0.0.8/pyproject.toml` & `snok-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snok-0.0.8/snok/cli.py` & `snok-0.0.9/snok/cli.py`

 * *Files identical despite different names*

### Comparing `snok-0.0.8/snok/services/new.py` & `snok-0.0.9/snok/services/new.py`

 * *Files identical despite different names*

### Comparing `snok-0.0.8/snok/templates/__shared/CONTRIBUTING.md` & `snok-0.0.9/snok/templates/__shared/CONTRIBUTING.md`

 * *Files 27% similar despite different names*

```diff
@@ -30,56 +30,44 @@
 which python pip
 ```
 
 You should see paths that use `.venv/bin` in your current working directory.
 
 ## Dependencies
 
-This project uses `invoke` to manage dependencies.
+This project uses `snok` to manage dependencies.
 
-In your virtual environment, install `invoke` by running;
+In your virtual environment, install your dependencies by running;
 
 ```sh
-pip install --upgrade pip && pip install invoke
-```
-
-Then to install the project's dependencies, run;
-
-```sh
-inv install
+snok install
 ```
 
 To add a specific dependency, run;
 
 ```sh
-inv add <PACKAGE>
+snok add <PACKAGE>
 ```
 
 To remove a specific dependency, run;
 
 ```sh
-inv rm <PACKAGE>
+snok remove <PACKAGE>
 ```
 
-## Tasks
-
-All tasks are managed with `invoke`.
-
-Invoke is a python package that allows you to define tasks in a python file and run them from the command line, similar to `make` and `rake`, but with a pythonic syntax. All tasks are located in the `tasks.py` file.
-
-### Linting
+## Linting
 
 ```sh
-inv lint
+snok lint
 ```
 
-### Formatting
+## Formatting
 
 ```sh
-inv format
+snok format
 ```
 
-### Tests
+## Tests
 
 ```sh
-inv test
+snok test
 ```
```

### Comparing `snok-0.0.8/snok/templates/__shared/_.gitignore` & `snok-0.0.9/snok/templates/__shared/_.gitignore`

 * *Files identical despite different names*

### Comparing `snok-0.0.8/snok/templates/__shared/_.pre-commit-config.yaml` & `snok-0.0.9/snok/templates/__shared/_.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `snok-0.0.8/snok/templates/__shared/_pyproject_toml` & `snok-0.0.9/snok/templates/__shared/_pyproject_toml`

 * *Files identical despite different names*

### Comparing `snok-0.0.8/snok/utils.py` & `snok-0.0.9/snok/utils.py`

 * *Files identical despite different names*

### Comparing `snok-0.0.8/snok.egg-info/PKG-INFO` & `snok-0.0.9/snok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.8
+Version: 0.0.9
 Summary: 🚀 A simple, modern, full-stack toolkit for Python 🐍
 Author-email: Anthony Corletti <anthcor+snok@gmail.com>
 License: MIT
 Project-URL: Home, https://github.com/anthonycorletti/snok
 Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -59,15 +59,15 @@
 - Packaging with `setuptools`
 - Linting and formatting with `ruff` and `black`
 - Type checking with `mypy`
 - Testing with `pytest`
 
 ## 🤩 Coming Soon
 
-- Database integration with `pydantic` and `sqlmodel`
+- Database integration with `pydantic`, `sqlmodel`, and `alembic`
 - Web application generation with `fastapi` and `htmx`
 - Production ready deployment stacks with `nix`, `docker`, `skaffold` and `kustomize`
 - AI framework integrations with `pytorch` and `langchain`
 - Documentation site generation with `mkdocs`
 
 Check out the latest [issues](https://github.com/anthonycorletti/snok/issues) and [pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's coming soon!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snok Version: 0.0.8 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.9 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
@@ -20,25 +20,26 @@
 mind, snok is a Python toolkit for developers that focuses on making it simple
 and easy to build modern, full-stack applications, across web and AI
 frameworks. Snok is designed to leverage the best tools and packages that exist
 in the Python ecosystem in simple and easy to use workflows that accelerate
 development. ## ð Featuring - Package generation - Built-in dependency
 management - Packaging with `setuptools` - Linting and formatting with `ruff`
 and `black` - Type checking with `mypy` - Testing with `pytest` ## ð¤© Coming
-Soon - Database integration with `pydantic` and `sqlmodel` - Web application
-generation with `fastapi` and `htmx` - Production ready deployment stacks with
-`nix`, `docker`, `skaffold` and `kustomize` - AI framework integrations with
-`pytorch` and `langchain` - Documentation site generation with `mkdocs` Check
-out the latest [issues](https://github.com/anthonycorletti/snok/issues) and
-[pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's
-coming soon! ## ð Requirements - Python 3.11+ - `pip` ## âï¸ Installation
-After you've created your Python 3.11+ virtual environment in a new directory,
-install Snok: ```sh pip install snok ``` ## ð Getting Started Create a new
-package with: ```sh snok new mypackage ``` To install dependencies: ```sh snok
-install ``` To add a new dependency: ```sh snok add fastapi ``` To remove a
-dependency: ```sh snok remove fastapi ``` ## ð«¶ How can I help? - [â­ï¸
-Star snok on GitHub! â­ï¸](https://github.com/anthonycorletti/snok) - Open an
-[issue](https://github.com/anthonycorletti/snok/issues/new/choose) if you have
-a question, comment, feature request, or bug report. - Open a [pull request]
-(https://github.com/anthonycorletti/snok/compare) on GitHub. Contributions are
-encouraged and welcome! ## ð² Contact Reach out on [Twitter](https://
-twitter.com/anthonycorletti) if you'd like to get in touch!  
+Soon - Database integration with `pydantic`, `sqlmodel`, and `alembic` - Web
+application generation with `fastapi` and `htmx` - Production ready deployment
+stacks with `nix`, `docker`, `skaffold` and `kustomize` - AI framework
+integrations with `pytorch` and `langchain` - Documentation site generation
+with `mkdocs` Check out the latest [issues](https://github.com/anthonycorletti/
+snok/issues) and [pull requests](https://github.com/anthonycorletti/snok/pulls)
+to see what's coming soon! ## ð Requirements - Python 3.11+ - `pip` ##
+âï¸ Installation After you've created your Python 3.11+ virtual environment
+in a new directory, install Snok: ```sh pip install snok ``` ## ð Getting
+Started Create a new package with: ```sh snok new mypackage ``` To install
+dependencies: ```sh snok install ``` To add a new dependency: ```sh snok add
+fastapi ``` To remove a dependency: ```sh snok remove fastapi ``` ## ð«¶ How
+can I help? - [â­ï¸ Star snok on GitHub! â­ï¸](https://github.com/
+anthonycorletti/snok) - Open an [issue](https://github.com/anthonycorletti/
+snok/issues/new/choose) if you have a question, comment, feature request, or
+bug report. - Open a [pull request](https://github.com/anthonycorletti/snok/
+compare) on GitHub. Contributions are encouraged and welcome! ## ð² Contact
+Reach out on [Twitter](https://twitter.com/anthonycorletti) if you'd like to
+get in touch!
```

### Comparing `snok-0.0.8/snok.egg-info/SOURCES.txt` & `snok-0.0.9/snok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snok-0.0.8/tests/test_cli.py` & `snok-0.0.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `snok-0.0.8/tests/test_utils.py` & `snok-0.0.9/tests/test_utils.py`

 * *Files identical despite different names*

