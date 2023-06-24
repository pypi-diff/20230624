# Comparing `tmp/snok-0.0.7.tar.gz` & `tmp/snok-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snok-0.0.7.tar", last modified: Thu Jun 22 05:44:12 2023, max compression
+gzip compressed data, was "snok-0.0.8.tar", last modified: Sat Jun 24 19:31:23 2023, max compression
```

## Comparing `snok-0.0.7.tar` & `snok-0.0.8.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.976360 snok-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 05:43:49.000000 snok-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 05:44:12.976360 snok-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-22 05:43:49.000000 snok-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-22 05:43:49.000000 snok-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 05:44:12.976360 snok-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.968360 snok-0.0.7/snok/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 05:43:49.000000 snok-0.0.7/snok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-22 05:43:49.000000 snok-0.0.7/snok/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 05:43:49.000000 snok-0.0.7/snok/const.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.972360 snok-0.0.7/snok/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-22 05:43:49.000000 snok-0.0.7/snok/services/new.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.964360 snok-0.0.7/snok/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.972360 snok-0.0.7/snok/templates/__app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app/db.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app/gunicorn_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.972360 snok-0.0.7/snok/templates/__app/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.972360 snok-0.0.7/snok/templates/__app/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app/routers/snok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.972360 snok-0.0.7/snok/templates/__app/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app/services/snok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.976360 snok-0.0.7/snok/templates/__app_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app_templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app_templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app_templates/_base.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app_templates/_head.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app_templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.976360 snok-0.0.7/snok/templates/__app_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__app_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.976360 snok-0.0.7/snok/templates/__package/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__package/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.976360 snok-0.0.7/snok/templates/__package_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__package_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__package_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__package_tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__package_tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.976360 snok-0.0.7/snok/templates/__shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__shared/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__shared/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__shared/_.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__shared/_.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__shared/_.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__shared/_pyproject_toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__shared/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-06-22 05:43:49.000000 snok-0.0.7/snok/templates/__shared/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-22 05:43:49.000000 snok-0.0.7/snok/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.972360 snok-0.0.7/snok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 05:44:12.000000 snok-0.0.7/snok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-22 05:44:12.000000 snok-0.0.7/snok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:44:12.000000 snok-0.0.7/snok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 05:44:12.000000 snok-0.0.7/snok.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 05:44:12.000000 snok-0.0.7/snok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 05:44:12.000000 snok-0.0.7/snok.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:12.976360 snok-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-22 05:43:49.000000 snok-0.0.7/tests/test_cli_new.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 05:43:49.000000 snok-0.0.7/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-24 19:31:00.000000 snok-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-24 19:31:23.545004 snok-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-24 19:31:00.000000 snok-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-24 19:31:00.000000 snok-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:31:23.545004 snok-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-24 19:31:00.000000 snok-0.0.8/snok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-24 19:31:00.000000 snok-0.0.8/snok/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-24 19:31:00.000000 snok-0.0.8/snok/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-24 19:31:00.000000 snok-0.0.8/snok/services/new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.537005 snok-0.0.8/snok/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/templates/__app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/gunicorn_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/templates/__app/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/templates/__app/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/routers/snok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok/templates/__app/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app/services/snok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/snok/templates/__app_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_templates/_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_templates/_head.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/snok/templates/__app_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__app_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/snok/templates/__package/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/snok/templates/__package_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package_tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__package_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/snok/templates/__shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/_.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/_.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/_.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/_pyproject_toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:00.000000 snok-0.0.8/snok/templates/__shared/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-24 19:31:00.000000 snok-0.0.8/snok/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.541005 snok-0.0.8/snok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-24 19:31:23.000000 snok-0.0.8/snok.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:31:23.545004 snok-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-24 19:31:00.000000 snok-0.0.8/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-24 19:31:00.000000 snok-0.0.8/tests/test_utils.py
```

### Comparing `snok-0.0.7/LICENSE` & `snok-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `snok-0.0.7/PKG-INFO` & `snok-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.7
+Version: 0.0.8
 Summary: 🚀 A simple, modern, full-stack toolkit for Python 🐍
 Author-email: Anthony Corletti <anthcor+snok@gmail.com>
 License: MIT
 Project-URL: Home, https://github.com/anthonycorletti/snok
 Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -51,66 +51,67 @@
 With this in mind, snok is a Python toolkit for developers that focuses on making it simple and easy to build modern, full-stack applications, across web and AI frameworks.
 
 Snok is designed to leverage the best tools and packages that exist in the Python ecosystem in simple and easy to use workflows that accelerate development.
 
 ## 🎉 Featuring
 
 - Package generation
-- Task management with `invoke`
+- Built-in dependency management
 - Packaging with `setuptools`
-- Linting with `ruff` and `black`
+- Linting and formatting with `ruff` and `black`
 - Type checking with `mypy`
 - Testing with `pytest`
 
 ## 🤩 Coming Soon
 
-- Web application generation with `fastapi` and `htmx`
 - Database integration with `pydantic` and `sqlmodel`
+- Web application generation with `fastapi` and `htmx`
 - Production ready deployment stacks with `nix`, `docker`, `skaffold` and `kustomize`
 - AI framework integrations with `pytorch` and `langchain`
+- Documentation site generation with `mkdocs`
 
 Check out the latest [issues](https://github.com/anthonycorletti/snok/issues) and [pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's coming soon!
 
 ## 📝 Requirements
 
 - Python 3.11+
 - `pip`
 
 ## ⚙️ Installation
 
-After you've created your Python 3.11+ virtual environment, install Snok with:
+After you've created your Python 3.11+ virtual environment in a new directory, install Snok:
 
 ```sh
 pip install snok
 ```
 
 ## 🐍 Getting Started
 
 Create a new package with:
 
 ```sh
-snok new mypackage && cd mypackage
+snok new mypackage
 ```
 
-Snok uses `invoke` to manage tasks, like installing dependencies, running tests, and more.
+To install dependencies:
 
 ```sh
-inv --list
+snok install
 ```
 
-To install dependencies:
+To add a new dependency:
 
 ```sh
-inv add fastapi
+snok add fastapi
 ```
 
-To uninstall dependencies:
+To remove a dependency:
 
 ```sh
-inv remove fastapi
+snok remove fastapi
 ```
 
 ## 🫶 How can I help?
 
 - [⭐️ Star snok on GitHub! ⭐️](https://github.com/anthonycorletti/snok)
 - Open an [issue](https://github.com/anthonycorletti/snok/issues/new/choose) if you have a question, comment, feature request, or bug report.
 - Open a [pull request](https://github.com/anthonycorletti/snok/compare) on GitHub. Contributions are encouraged and welcome!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snok Version: 0.0.7 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.8 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
@@ -17,29 +17,28 @@
 project. ## ð Why? The Python tooling ecosystem has plenty of options, and
 often times, it's not clear whether or not you're following the "right" way to
 do things, especially when those ways are changing week to week. With this in
 mind, snok is a Python toolkit for developers that focuses on making it simple
 and easy to build modern, full-stack applications, across web and AI
 frameworks. Snok is designed to leverage the best tools and packages that exist
 in the Python ecosystem in simple and easy to use workflows that accelerate
-development. ## ð Featuring - Package generation - Task management with
-`invoke` - Packaging with `setuptools` - Linting with `ruff` and `black` - Type
-checking with `mypy` - Testing with `pytest` ## ð¤© Coming Soon - Web
-application generation with `fastapi` and `htmx` - Database integration with
-`pydantic` and `sqlmodel` - Production ready deployment stacks with `nix`,
-`docker`, `skaffold` and `kustomize` - AI framework integrations with `pytorch`
-and `langchain` Check out the latest [issues](https://github.com/
-anthonycorletti/snok/issues) and [pull requests](https://github.com/
-anthonycorletti/snok/pulls) to see what's coming soon! ## ð Requirements -
-Python 3.11+ - `pip` ## âï¸ Installation After you've created your Python
-3.11+ virtual environment, install Snok with: ```sh pip install snok ``` ##
-ð Getting Started Create a new package with: ```sh snok new mypackage && cd
-mypackage ``` Snok uses `invoke` to manage tasks, like installing dependencies,
-running tests, and more. ```sh inv --list ``` To install dependencies: ```sh
-inv add fastapi ``` To uninstall dependencies: ```sh inv remove fastapi ``` ##
-ð«¶ How can I help? - [â­ï¸ Star snok on GitHub! â­ï¸](https://github.com/
-anthonycorletti/snok) - Open an [issue](https://github.com/anthonycorletti/
-snok/issues/new/choose) if you have a question, comment, feature request, or
-bug report. - Open a [pull request](https://github.com/anthonycorletti/snok/
-compare) on GitHub. Contributions are encouraged and welcome! ## ð² Contact
-Reach out on [Twitter](https://twitter.com/anthonycorletti) if you'd like to
-get in touch!  
+development. ## ð Featuring - Package generation - Built-in dependency
+management - Packaging with `setuptools` - Linting and formatting with `ruff`
+and `black` - Type checking with `mypy` - Testing with `pytest` ## ð¤© Coming
+Soon - Database integration with `pydantic` and `sqlmodel` - Web application
+generation with `fastapi` and `htmx` - Production ready deployment stacks with
+`nix`, `docker`, `skaffold` and `kustomize` - AI framework integrations with
+`pytorch` and `langchain` - Documentation site generation with `mkdocs` Check
+out the latest [issues](https://github.com/anthonycorletti/snok/issues) and
+[pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's
+coming soon! ## ð Requirements - Python 3.11+ - `pip` ## âï¸ Installation
+After you've created your Python 3.11+ virtual environment in a new directory,
+install Snok: ```sh pip install snok ``` ## ð Getting Started Create a new
+package with: ```sh snok new mypackage ``` To install dependencies: ```sh snok
+install ``` To add a new dependency: ```sh snok add fastapi ``` To remove a
+dependency: ```sh snok remove fastapi ``` ## ð«¶ How can I help? - [â­ï¸
+Star snok on GitHub! â­ï¸](https://github.com/anthonycorletti/snok) - Open an
+[issue](https://github.com/anthonycorletti/snok/issues/new/choose) if you have
+a question, comment, feature request, or bug report. - Open a [pull request]
+(https://github.com/anthonycorletti/snok/compare) on GitHub. Contributions are
+encouraged and welcome! ## ð² Contact Reach out on [Twitter](https://
+twitter.com/anthonycorletti) if you'd like to get in touch!
```

### Comparing `snok-0.0.7/README.md` & `snok-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,66 +38,67 @@
 With this in mind, snok is a Python toolkit for developers that focuses on making it simple and easy to build modern, full-stack applications, across web and AI frameworks.
 
 Snok is designed to leverage the best tools and packages that exist in the Python ecosystem in simple and easy to use workflows that accelerate development.
 
 ## 🎉 Featuring
 
 - Package generation
-- Task management with `invoke`
+- Built-in dependency management
 - Packaging with `setuptools`
-- Linting with `ruff` and `black`
+- Linting and formatting with `ruff` and `black`
 - Type checking with `mypy`
 - Testing with `pytest`
 
 ## 🤩 Coming Soon
 
-- Web application generation with `fastapi` and `htmx`
 - Database integration with `pydantic` and `sqlmodel`
+- Web application generation with `fastapi` and `htmx`
 - Production ready deployment stacks with `nix`, `docker`, `skaffold` and `kustomize`
 - AI framework integrations with `pytorch` and `langchain`
+- Documentation site generation with `mkdocs`
 
 Check out the latest [issues](https://github.com/anthonycorletti/snok/issues) and [pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's coming soon!
 
 ## 📝 Requirements
 
 - Python 3.11+
 - `pip`
 
 ## ⚙️ Installation
 
-After you've created your Python 3.11+ virtual environment, install Snok with:
+After you've created your Python 3.11+ virtual environment in a new directory, install Snok:
 
 ```sh
 pip install snok
 ```
 
 ## 🐍 Getting Started
 
 Create a new package with:
 
 ```sh
-snok new mypackage && cd mypackage
+snok new mypackage
 ```
 
-Snok uses `invoke` to manage tasks, like installing dependencies, running tests, and more.
+To install dependencies:
 
 ```sh
-inv --list
+snok install
 ```
 
-To install dependencies:
+To add a new dependency:
 
 ```sh
-inv add fastapi
+snok add fastapi
 ```
 
-To uninstall dependencies:
+To remove a dependency:
 
 ```sh
-inv remove fastapi
+snok remove fastapi
 ```
 
 ## 🫶 How can I help?
 
 - [⭐️ Star snok on GitHub! ⭐️](https://github.com/anthonycorletti/snok)
 - Open an [issue](https://github.com/anthonycorletti/snok/issues/new/choose) if you have a question, comment, feature request, or bug report.
 - Open a [pull request](https://github.com/anthonycorletti/snok/compare) on GitHub. Contributions are encouraged and welcome!
```

#### html2text {}

```diff
@@ -11,29 +11,28 @@
 project. ## ð Why? The Python tooling ecosystem has plenty of options, and
 often times, it's not clear whether or not you're following the "right" way to
 do things, especially when those ways are changing week to week. With this in
 mind, snok is a Python toolkit for developers that focuses on making it simple
 and easy to build modern, full-stack applications, across web and AI
 frameworks. Snok is designed to leverage the best tools and packages that exist
 in the Python ecosystem in simple and easy to use workflows that accelerate
-development. ## ð Featuring - Package generation - Task management with
-`invoke` - Packaging with `setuptools` - Linting with `ruff` and `black` - Type
-checking with `mypy` - Testing with `pytest` ## ð¤© Coming Soon - Web
-application generation with `fastapi` and `htmx` - Database integration with
-`pydantic` and `sqlmodel` - Production ready deployment stacks with `nix`,
-`docker`, `skaffold` and `kustomize` - AI framework integrations with `pytorch`
-and `langchain` Check out the latest [issues](https://github.com/
-anthonycorletti/snok/issues) and [pull requests](https://github.com/
-anthonycorletti/snok/pulls) to see what's coming soon! ## ð Requirements -
-Python 3.11+ - `pip` ## âï¸ Installation After you've created your Python
-3.11+ virtual environment, install Snok with: ```sh pip install snok ``` ##
-ð Getting Started Create a new package with: ```sh snok new mypackage && cd
-mypackage ``` Snok uses `invoke` to manage tasks, like installing dependencies,
-running tests, and more. ```sh inv --list ``` To install dependencies: ```sh
-inv add fastapi ``` To uninstall dependencies: ```sh inv remove fastapi ``` ##
-ð«¶ How can I help? - [â­ï¸ Star snok on GitHub! â­ï¸](https://github.com/
-anthonycorletti/snok) - Open an [issue](https://github.com/anthonycorletti/
-snok/issues/new/choose) if you have a question, comment, feature request, or
-bug report. - Open a [pull request](https://github.com/anthonycorletti/snok/
-compare) on GitHub. Contributions are encouraged and welcome! ## ð² Contact
-Reach out on [Twitter](https://twitter.com/anthonycorletti) if you'd like to
-get in touch!  
+development. ## ð Featuring - Package generation - Built-in dependency
+management - Packaging with `setuptools` - Linting and formatting with `ruff`
+and `black` - Type checking with `mypy` - Testing with `pytest` ## ð¤© Coming
+Soon - Database integration with `pydantic` and `sqlmodel` - Web application
+generation with `fastapi` and `htmx` - Production ready deployment stacks with
+`nix`, `docker`, `skaffold` and `kustomize` - AI framework integrations with
+`pytorch` and `langchain` - Documentation site generation with `mkdocs` Check
+out the latest [issues](https://github.com/anthonycorletti/snok/issues) and
+[pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's
+coming soon! ## ð Requirements - Python 3.11+ - `pip` ## âï¸ Installation
+After you've created your Python 3.11+ virtual environment in a new directory,
+install Snok: ```sh pip install snok ``` ## ð Getting Started Create a new
+package with: ```sh snok new mypackage ``` To install dependencies: ```sh snok
+install ``` To add a new dependency: ```sh snok add fastapi ``` To remove a
+dependency: ```sh snok remove fastapi ``` ## ð«¶ How can I help? - [â­ï¸
+Star snok on GitHub! â­ï¸](https://github.com/anthonycorletti/snok) - Open an
+[issue](https://github.com/anthonycorletti/snok/issues/new/choose) if you have
+a question, comment, feature request, or bug report. - Open a [pull request]
+(https://github.com/anthonycorletti/snok/compare) on GitHub. Contributions are
+encouraged and welcome! ## ð² Contact Reach out on [Twitter](https://
+twitter.com/anthonycorletti) if you'd like to get in touch!
```

### Comparing `snok-0.0.7/pyproject.toml` & `snok-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,61 +14,61 @@
 ]
 requires-python = ">=3.11"
 dependencies = [
     "black>=21.10",
     "coverage>=6.1.1",
     "fastapi>=0.97.0",
     "gunicorn>=20.1.0",
-    "invoke>=2.0.0",
+    "httpx>=0.24.1",
     "jinja2>=3.1.2",
     "mypy>=0.910",
     "packaging>=21.0",
     "pre-commit>=2.17.0",
     "pydantic>=1.8.2",
     "pytest-cov>=3.0.0",
     "pytest-xdist>=3.3.1",
     "pytest>=6.2.5",
+    "requests>=2.26.0",
     "rich>=10.12.0",
     "ruff>=0.0.98",
     "setuptools>=67.8.0",
     "toml>=0.10.2",
     "typer>=0.7.0",
+    "types-requests>=2.26.0",
     "types-toml>=0.1.0",
     "uvicorn>=0.15.0",
     "wheel>=0.36",
 ]
 [[project.authors]]
 name = "Anthony Corletti"
 email = "anthcor+snok@gmail.com"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 dev = [
+    "invoke>=1.6.0",
     "mdx-include>=1.4.2",
-    "mkdocs>=1.4.2",
     "mkdocs-material>=9.1.5",
+    "mkdocs>=1.4.2",
 ]
 
 [project.urls]
 Home = "https://github.com/anthonycorletti/snok"
 Documentation = "https://snok.corletti.xyz"
 
 [project.scripts]
 snok = "snok.cli:app"
 
-[tool.setuptools.package-data]
-snok = ["py.typed", "templates/**/*"]
-
-[tool.setuptools.dynamic]
-version = {attr = "snok.__version__"}
-
-[tool.setuptools.packages.find]
-exclude = ["tests"]
+[tool.snok]
+sources = [
+    "snok",
+    "tests",
+]
 
 [tool.ruff]
 line-length = 88
 ignore = [
     "D10",
 ]
 include = [
@@ -125,28 +125,30 @@
     snok/templates/*
 )/
 '''
 
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_defs = true
-mypy_path = [
-    "snok",
-    "tests",
-]
 exclude = [
     "dist",
     "build",
     ".venv",
     "snok/templates/*",
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
+[tool.setuptools.package-data]
+snok = [
+    "py.typed",
+    "templates/**/*",
+]
+
 [tool.pytest.ini_options]
 addopts = [
     "-n",
     "auto",
     "-o",
     "console_output_style=progress",
     "--ignore=snok/templates",
@@ -173,7 +175,15 @@
 ]
 
 [tool.coverage.html]
 directory = "htmlcov"
 
 [tool.coverage.xml]
 output = "coverage.xml"
+
+[tool.setuptools.dynamic.version]
+attr = "snok.__version__"
+
+[tool.setuptools.packages.find]
+exclude = [
+    "tests",
+]
```

### Comparing `snok-0.0.7/snok/services/new.py` & `snok-0.0.8/snok/services/new.py`

 * *Files identical despite different names*

### Comparing `snok-0.0.7/snok/templates/__shared/CONTRIBUTING.md` & `snok-0.0.8/snok/templates/__shared/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snok-0.0.7/snok/templates/__shared/_.gitignore` & `snok-0.0.8/snok/templates/__shared/_.gitignore`

 * *Files identical despite different names*

### Comparing `snok-0.0.7/snok/templates/__shared/_.pre-commit-config.yaml` & `snok-0.0.8/snok/templates/__shared/_.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `snok-0.0.7/snok/templates/__shared/_pyproject_toml` & `snok-0.0.8/snok/templates/__shared/_pyproject_toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,24 @@
     "version",
 ]
 requires-python = ">=3.11"
 dependencies = []
 
 [project.optional-dependencies]
 dev = [
-    "black>=21.10",
-    "coverage>=6.1.1",
-    "mypy>=0.910",
-    "packaging>=21.0",
-    "pre-commit>=2.17.0",
-    "pytest-cov>=3.0.0",
-    "pytest-xdist>=3.3.1",
-    "pytest>=6.2.5",
-    "ruff>=0.0.98",
-    "setuptools>=67.8.0",
-    "wheel>=0.36",
+    "snok",
 ]
 
+[tool.snok]
+sources = [
+    "{{ __template_name }}",
+    "tests",
+]
+
+
 [tool.setuptools.package-data]
 {{ __template_name }} = ["py.typed"]
 
 [tool.setuptools.dynamic]
 version = {attr = "{{ __template_name }}.__version__"}
 
 [tool.setuptools.packages.find]
```

### Comparing `snok-0.0.7/snok.egg-info/PKG-INFO` & `snok-0.0.8/snok.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.7
+Version: 0.0.8
 Summary: 🚀 A simple, modern, full-stack toolkit for Python 🐍
 Author-email: Anthony Corletti <anthcor+snok@gmail.com>
 License: MIT
 Project-URL: Home, https://github.com/anthonycorletti/snok
 Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -51,66 +51,67 @@
 With this in mind, snok is a Python toolkit for developers that focuses on making it simple and easy to build modern, full-stack applications, across web and AI frameworks.
 
 Snok is designed to leverage the best tools and packages that exist in the Python ecosystem in simple and easy to use workflows that accelerate development.
 
 ## 🎉 Featuring
 
 - Package generation
-- Task management with `invoke`
+- Built-in dependency management
 - Packaging with `setuptools`
-- Linting with `ruff` and `black`
+- Linting and formatting with `ruff` and `black`
 - Type checking with `mypy`
 - Testing with `pytest`
 
 ## 🤩 Coming Soon
 
-- Web application generation with `fastapi` and `htmx`
 - Database integration with `pydantic` and `sqlmodel`
+- Web application generation with `fastapi` and `htmx`
 - Production ready deployment stacks with `nix`, `docker`, `skaffold` and `kustomize`
 - AI framework integrations with `pytorch` and `langchain`
+- Documentation site generation with `mkdocs`
 
 Check out the latest [issues](https://github.com/anthonycorletti/snok/issues) and [pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's coming soon!
 
 ## 📝 Requirements
 
 - Python 3.11+
 - `pip`
 
 ## ⚙️ Installation
 
-After you've created your Python 3.11+ virtual environment, install Snok with:
+After you've created your Python 3.11+ virtual environment in a new directory, install Snok:
 
 ```sh
 pip install snok
 ```
 
 ## 🐍 Getting Started
 
 Create a new package with:
 
 ```sh
-snok new mypackage && cd mypackage
+snok new mypackage
 ```
 
-Snok uses `invoke` to manage tasks, like installing dependencies, running tests, and more.
+To install dependencies:
 
 ```sh
-inv --list
+snok install
 ```
 
-To install dependencies:
+To add a new dependency:
 
 ```sh
-inv add fastapi
+snok add fastapi
 ```
 
-To uninstall dependencies:
+To remove a dependency:
 
 ```sh
-inv remove fastapi
+snok remove fastapi
 ```
 
 ## 🫶 How can I help?
 
 - [⭐️ Star snok on GitHub! ⭐️](https://github.com/anthonycorletti/snok)
 - Open an [issue](https://github.com/anthonycorletti/snok/issues/new/choose) if you have a question, comment, feature request, or bug report.
 - Open a [pull request](https://github.com/anthonycorletti/snok/compare) on GitHub. Contributions are encouraged and welcome!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snok Version: 0.0.7 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.8 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
@@ -17,29 +17,28 @@
 project. ## ð Why? The Python tooling ecosystem has plenty of options, and
 often times, it's not clear whether or not you're following the "right" way to
 do things, especially when those ways are changing week to week. With this in
 mind, snok is a Python toolkit for developers that focuses on making it simple
 and easy to build modern, full-stack applications, across web and AI
 frameworks. Snok is designed to leverage the best tools and packages that exist
 in the Python ecosystem in simple and easy to use workflows that accelerate
-development. ## ð Featuring - Package generation - Task management with
-`invoke` - Packaging with `setuptools` - Linting with `ruff` and `black` - Type
-checking with `mypy` - Testing with `pytest` ## ð¤© Coming Soon - Web
-application generation with `fastapi` and `htmx` - Database integration with
-`pydantic` and `sqlmodel` - Production ready deployment stacks with `nix`,
-`docker`, `skaffold` and `kustomize` - AI framework integrations with `pytorch`
-and `langchain` Check out the latest [issues](https://github.com/
-anthonycorletti/snok/issues) and [pull requests](https://github.com/
-anthonycorletti/snok/pulls) to see what's coming soon! ## ð Requirements -
-Python 3.11+ - `pip` ## âï¸ Installation After you've created your Python
-3.11+ virtual environment, install Snok with: ```sh pip install snok ``` ##
-ð Getting Started Create a new package with: ```sh snok new mypackage && cd
-mypackage ``` Snok uses `invoke` to manage tasks, like installing dependencies,
-running tests, and more. ```sh inv --list ``` To install dependencies: ```sh
-inv add fastapi ``` To uninstall dependencies: ```sh inv remove fastapi ``` ##
-ð«¶ How can I help? - [â­ï¸ Star snok on GitHub! â­ï¸](https://github.com/
-anthonycorletti/snok) - Open an [issue](https://github.com/anthonycorletti/
-snok/issues/new/choose) if you have a question, comment, feature request, or
-bug report. - Open a [pull request](https://github.com/anthonycorletti/snok/
-compare) on GitHub. Contributions are encouraged and welcome! ## ð² Contact
-Reach out on [Twitter](https://twitter.com/anthonycorletti) if you'd like to
-get in touch!  
+development. ## ð Featuring - Package generation - Built-in dependency
+management - Packaging with `setuptools` - Linting and formatting with `ruff`
+and `black` - Type checking with `mypy` - Testing with `pytest` ## ð¤© Coming
+Soon - Database integration with `pydantic` and `sqlmodel` - Web application
+generation with `fastapi` and `htmx` - Production ready deployment stacks with
+`nix`, `docker`, `skaffold` and `kustomize` - AI framework integrations with
+`pytorch` and `langchain` - Documentation site generation with `mkdocs` Check
+out the latest [issues](https://github.com/anthonycorletti/snok/issues) and
+[pull requests](https://github.com/anthonycorletti/snok/pulls) to see what's
+coming soon! ## ð Requirements - Python 3.11+ - `pip` ## âï¸ Installation
+After you've created your Python 3.11+ virtual environment in a new directory,
+install Snok: ```sh pip install snok ``` ## ð Getting Started Create a new
+package with: ```sh snok new mypackage ``` To install dependencies: ```sh snok
+install ``` To add a new dependency: ```sh snok add fastapi ``` To remove a
+dependency: ```sh snok remove fastapi ``` ## ð«¶ How can I help? - [â­ï¸
+Star snok on GitHub! â­ï¸](https://github.com/anthonycorletti/snok) - Open an
+[issue](https://github.com/anthonycorletti/snok/issues/new/choose) if you have
+a question, comment, feature request, or bug report. - Open a [pull request]
+(https://github.com/anthonycorletti/snok/compare) on GitHub. Contributions are
+encouraged and welcome! ## ð² Contact Reach out on [Twitter](https://
+twitter.com/anthonycorletti) if you'd like to get in touch!
```

### Comparing `snok-0.0.7/snok.egg-info/SOURCES.txt` & `snok-0.0.8/snok.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,10 +39,9 @@
 snok/templates/__shared/CONTRIBUTING.md
 snok/templates/__shared/README.md
 snok/templates/__shared/_.editorconfig
 snok/templates/__shared/_.gitignore
 snok/templates/__shared/_.pre-commit-config.yaml
 snok/templates/__shared/_pyproject_toml
 snok/templates/__shared/py.typed
-snok/templates/__shared/tasks.py
-tests/test_cli_new.py
-tests/test_version.py
+tests/test_cli.py
+tests/test_utils.py
```

### Comparing `snok-0.0.7/tests/test_cli_new.py` & `snok-0.0.8/tests/test_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,27 @@
 
 from typer.testing import CliRunner
 
 from snok import __version__
 from snok.cli import app
 
 
-def test_new_package(cli_runner: CliRunner, setup_test_project_dir: str) -> None:
+def test_version(cli_runner: CliRunner) -> None:
+    response = cli_runner.invoke(app, ["version"])
+    assert response.exit_code == 0
+    assert response.stdout == __version__
+
+
+def test_new_package_setup(cli_runner: CliRunner, setup_test_project_dir: str) -> None:
     response = cli_runner.invoke(
         app,
         ["new", "test_package", "-o", setup_test_project_dir],
     )
     assert response.exit_code == 0
-    print(os.listdir(setup_test_project_dir))
+
     # assert the output directory exists
     for path in [
         f"{setup_test_project_dir}/test_package",
         f"{setup_test_project_dir}/tests",
         f"{setup_test_project_dir}/.git",
         f"{setup_test_project_dir}/README.md",
         f"{setup_test_project_dir}/pyproject.toml",
@@ -25,13 +31,7 @@
         f"{setup_test_project_dir}/test_package/main.py",
         f"{setup_test_project_dir}/tests/__init__.py",
         f"{setup_test_project_dir}/tests/conftest.py",
         f"{setup_test_project_dir}/tests/test_main.py",
         f"{setup_test_project_dir}/tests/test_version.py",
     ]:
         assert os.path.exists(path)
-
-
-def test_version(cli_runner: CliRunner) -> None:
-    response = cli_runner.invoke(app, ["version"])
-    assert response.exit_code == 0
-    assert response.stdout == __version__
```

