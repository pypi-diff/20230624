# Comparing `tmp/SimpleSQLite-1.3.1.tar.gz` & `tmp/SimpleSQLite-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleSQLite-1.3.1.tar", last modified: Sun Jun  4 07:01:56 2023, max compression
+gzip compressed data, was "SimpleSQLite-1.3.2.tar", last modified: Sat Jun 24 16:56:24 2023, max compression
```

## Comparing `SimpleSQLite-1.3.1.tar` & `SimpleSQLite-1.3.2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.923955 SimpleSQLite-1.3.1/
--rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      242 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    14377 2023-06-04 07:01:56.923955 SimpleSQLite-1.3.1/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)    12565 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    14377 2023-06-04 07:01:56.000000 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     1110 2023-06-04 07:01:56.000000 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-04 07:01:56.000000 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      287 2023-06-04 07:01:56.000000 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       13 2023-06-04 07:01:56.000000 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/docs/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/docs/pages/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/docs/pages/introduction/
--rw-r--r--   0 toor      (1000) toor      (1000)      177 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/docs/pages/introduction/summary.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1336 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       29 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/requirements/docs_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      130 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      121 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-04 07:01:56.923955 SimpleSQLite-1.3.1/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     3079 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/simplesqlite/
--rw-r--r--   0 toor      (1000) toor      (1000)      590 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1025 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4870 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_func.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/simplesqlite/_logger/
--rw-r--r--   0 toor      (1000) toor      (1000)       55 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_logger/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      888 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_logger/_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1071 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_logger/_null_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6522 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_sanitizer.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4280 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_validator.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3529 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/converter.py
--rw-r--r--   0 toor      (1000) toor      (1000)    58899 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/core.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1381 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/error.py
--rw-r--r--   0 toor      (1000) toor      (1000)     8879 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/model.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/py.typed
--rw-r--r--   0 toor      (1000) toor      (1000)    13682 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/query.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2560 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/sqlquery.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.923955 SimpleSQLite-1.3.1/test/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      266 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/_common.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.923955 SimpleSQLite-1.3.1/test/data/
--rw-r--r--   0 toor      (1000) toor      (1000)    71819 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/data/python - Wiktionary.html
--rw-r--r--   0 toor      (1000) toor      (1000)     1902 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/fixture.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3123 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_convertor.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1317 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_from_file.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4169 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_func.py
--rw-r--r--   0 toor      (1000) toor      (1000)      561 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1145 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_orm.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1837 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_pandas.py
--rw-r--r--   0 toor      (1000) toor      (1000)    12906 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_query.py
--rw-r--r--   0 toor      (1000) toor      (1000)    10549 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_sanitizer.py
--rw-r--r--   0 toor      (1000) toor      (1000)    42407 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_simplesqlite.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2927 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_sqlquery.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7876 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_validator.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1498 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-24 16:56:24.946401 SimpleSQLite-1.3.2/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      242 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    14327 2023-06-24 16:56:24.946401 SimpleSQLite-1.3.2/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    12565 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-24 16:56:24.936401 SimpleSQLite-1.3.2/SimpleSQLite.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    14327 2023-06-24 16:56:24.000000 SimpleSQLite-1.3.2/SimpleSQLite.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1145 2023-06-24 16:56:24.000000 SimpleSQLite-1.3.2/SimpleSQLite.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-24 16:56:24.000000 SimpleSQLite-1.3.2/SimpleSQLite.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-24 16:56:06.000000 SimpleSQLite-1.3.2/SimpleSQLite.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      287 2023-06-24 16:56:24.000000 SimpleSQLite-1.3.2/SimpleSQLite.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       13 2023-06-24 16:56:24.000000 SimpleSQLite-1.3.2/SimpleSQLite.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-24 16:56:24.936401 SimpleSQLite-1.3.2/docs/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-24 16:56:24.936401 SimpleSQLite-1.3.2/docs/pages/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-24 16:56:24.936401 SimpleSQLite-1.3.2/docs/pages/introduction/
+-rw-r--r--   0 toor      (1000) toor      (1000)      177 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/docs/pages/introduction/summary.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1365 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-24 16:56:24.936401 SimpleSQLite-1.3.2/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       29 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/requirements/docs_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      130 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      121 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-24 16:56:24.946401 SimpleSQLite-1.3.2/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     3050 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-24 16:56:24.936401 SimpleSQLite-1.3.2/simplesqlite/
+-rw-r--r--   0 toor      (1000) toor      (1000)      982 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1025 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4870 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/_func.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-24 16:56:24.936401 SimpleSQLite-1.3.2/simplesqlite/_logger/
+-rw-r--r--   0 toor      (1000) toor      (1000)       55 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/_logger/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      888 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/_logger/_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1071 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/_logger/_null_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6937 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/_sanitizer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4280 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/_validator.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3529 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/converter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    58899 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/core.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1381 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8879 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/model.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/py.typed
+-rw-r--r--   0 toor      (1000) toor      (1000)    13682 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/query.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2560 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/simplesqlite/sqlquery.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-24 16:56:24.946401 SimpleSQLite-1.3.2/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      266 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/_common.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-24 16:56:24.946401 SimpleSQLite-1.3.2/test/data/
+-rw-r--r--   0 toor      (1000) toor      (1000)    71819 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/data/python - Wiktionary.html
+-rw-r--r--   0 toor      (1000) toor      (1000)     1902 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/fixture.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3123 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/test_convertor.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1317 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/test_from_file.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4169 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/test_func.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      561 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/test_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1145 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/test_orm.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1837 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/test_pandas.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    12906 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/test_query.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11342 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/test_sanitizer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    42407 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/test_simplesqlite.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2927 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/test_sqlquery.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7876 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/test/test_validator.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1464 2023-06-24 16:55:55.000000 SimpleSQLite-1.3.2/tox.ini
```

### Comparing `SimpleSQLite-1.3.1/LICENSE` & `SimpleSQLite-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/PKG-INFO` & `SimpleSQLite-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleSQLite
-Version: 1.3.1
+Version: 1.3.2
 Summary: SimpleSQLite is a Python library to simplify SQLite database operations: table creation, data insertion and get data as other data formats. Simple ORM functionality for SQLite.
 Home-page: https://github.com/thombashi/SimpleSQLite
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Documentation, https://SimpleSQLite.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/SimpleSQLite
@@ -14,27 +14,26 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: logging
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **SimpleSQLite**
    :backlinks: top
@@ -402,15 +401,15 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-simplesqlite
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/SimpleSQLite/network/dependencies>`__
 
 Optional Dependencies
 ----------------------------------
 - `loguru <https://github.com/Delgan/loguru>`__
     - Used for logging if the package installed
 - `pandas <https://pandas.pydata.org/>`__
```

### Comparing `SimpleSQLite-1.3.1/README.rst` & `SimpleSQLite-1.3.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-simplesqlite
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/SimpleSQLite/network/dependencies>`__
 
 Optional Dependencies
 ----------------------------------
 - `loguru <https://github.com/Delgan/loguru>`__
     - Used for logging if the package installed
 - `pandas <https://pandas.pydata.org/>`__
```

### Comparing `SimpleSQLite-1.3.1/SimpleSQLite.egg-info/PKG-INFO` & `SimpleSQLite-1.3.2/SimpleSQLite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleSQLite
-Version: 1.3.1
+Version: 1.3.2
 Summary: SimpleSQLite is a Python library to simplify SQLite database operations: table creation, data insertion and get data as other data formats. Simple ORM functionality for SQLite.
 Home-page: https://github.com/thombashi/SimpleSQLite
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Documentation, https://SimpleSQLite.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/SimpleSQLite
@@ -14,27 +14,26 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: logging
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **SimpleSQLite**
    :backlinks: top
@@ -402,15 +401,15 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-simplesqlite
 
 
 Dependencies
 ============
-- Python 3.6+
+- Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/SimpleSQLite/network/dependencies>`__
 
 Optional Dependencies
 ----------------------------------
 - `loguru <https://github.com/Delgan/loguru>`__
     - Used for logging if the package installed
 - `pandas <https://pandas.pydata.org/>`__
```

### Comparing `SimpleSQLite-1.3.1/SimpleSQLite.egg-info/SOURCES.txt` & `SimpleSQLite-1.3.2/SimpleSQLite.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.rst
 pyproject.toml
 setup.py
 tox.ini
 SimpleSQLite.egg-info/PKG-INFO
 SimpleSQLite.egg-info/SOURCES.txt
 SimpleSQLite.egg-info/dependency_links.txt
+SimpleSQLite.egg-info/not-zip-safe
 SimpleSQLite.egg-info/requires.txt
 SimpleSQLite.egg-info/top_level.txt
 docs/pages/introduction/summary.txt
 requirements/docs_requirements.txt
 requirements/requirements.txt
 requirements/test_requirements.txt
 simplesqlite/__init__.py
```

### Comparing `SimpleSQLite-1.3.1/pyproject.toml` & `SimpleSQLite-1.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
@@ -14,15 +15,15 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 | docs/conf.py
 '''
-target-version = ['py36', 'py37', 'py38', 'py39', 'py310', 'py311']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.isort]
 known_third_party = [
     'dataproperty',
     'logbook',
     'mbstrdecoder',
     'pandas',
@@ -61,15 +62,15 @@
     'abstractproperty',
     'abstractclassmethod',
     'warnings.warn',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.6
+python_version = 3.7
 
 pretty = true
 show_error_codes = true
 show_error_context = true
 warn_unused_configs = true
 
 [tool.pytest.ini_options]
```

### Comparing `SimpleSQLite-1.3.1/setup.py` & `SimpleSQLite-1.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,34 +56,34 @@
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
         "Documentation": f"https://{MODULE_NAME:s}.rtfd.io/",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
         "Changlog": f"{REPOSITORY_URL:s}/releases",
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=install_requires,
     tests_require=tests_requires,
     extras_require={"logging": ["loguru>=0.4.1,<1"], "test": tests_requires},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Database",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     cmdclass=get_release_command_class(),
+    zip_safe=False,
 )
```

### Comparing `SimpleSQLite-1.3.1/simplesqlite/_common.py` & `SimpleSQLite-1.3.2/simplesqlite/_common.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/simplesqlite/_func.py` & `SimpleSQLite-1.3.2/simplesqlite/_func.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/simplesqlite/_logger/_logger.py` & `SimpleSQLite-1.3.2/simplesqlite/_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/simplesqlite/_logger/_null_logger.py` & `SimpleSQLite-1.3.2/simplesqlite/_logger/_null_logger.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/simplesqlite/_sanitizer.py` & `SimpleSQLite-1.3.2/simplesqlite/_sanitizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 from collections import Counter
 from typing import List, Optional, Sequence, cast
 
-import dataproperty
 import pathvalidate as pv
 import typepy
 from dataproperty.typing import TypeHint
 from pathvalidate.error import ErrorReason, ValidationError
 from pathvalidate.handler import raise_error
 from tabledata import (
     DataError,
@@ -106,15 +105,15 @@
     def _normalize_table_name(self, table_name: str) -> str:
         return self.__RENAME_TEMPLATE.format(table_name)
 
     def _preprocess_header(self, col_idx: int, header: Optional[str]) -> str:
         if typepy.is_null_string(header):
             return self.__get_default_header(col_idx)
 
-        if dataproperty.is_multibyte_str(header):
+        if is_multibyte_str(header):
             return cast(str, header)
 
         return Attr.sanitize(cast(str, header))
 
     def _validate_headers(self) -> None:
         if typepy.is_empty_sequence(self._tabledata.headers):
             raise ValueError("attribute name list is empty")
@@ -187,7 +186,27 @@
         i = 0
         while True:
             header = convert_idx_to_alphabet(col_idx + i)
             if header not in self.__upper_headers:
                 return header
 
             i += 1
+
+
+def is_multibyte_str(text) -> bool:
+    from mbstrdecoder import MultiByteStrDecoder
+    from typepy import StrictLevel, String
+
+    if not String(text, strict_level=StrictLevel.MIN).is_type():
+        return False
+
+    try:
+        unicode_text = MultiByteStrDecoder(text).unicode_str
+    except ValueError:
+        return False
+
+    try:
+        unicode_text.encode("ascii")
+    except UnicodeEncodeError:
+        return True
+
+    return False
```

### Comparing `SimpleSQLite-1.3.1/simplesqlite/_validator.py` & `SimpleSQLite-1.3.2/simplesqlite/_validator.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/simplesqlite/converter.py` & `SimpleSQLite-1.3.2/simplesqlite/converter.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/simplesqlite/core.py` & `SimpleSQLite-1.3.2/simplesqlite/core.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/simplesqlite/error.py` & `SimpleSQLite-1.3.2/simplesqlite/error.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/simplesqlite/model.py` & `SimpleSQLite-1.3.2/simplesqlite/model.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/simplesqlite/query.py` & `SimpleSQLite-1.3.2/simplesqlite/query.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/simplesqlite/sqlquery.py` & `SimpleSQLite-1.3.2/simplesqlite/sqlquery.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/data/python - Wiktionary.html` & `SimpleSQLite-1.3.2/test/data/python - Wiktionary.html`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/fixture.py` & `SimpleSQLite-1.3.2/test/fixture.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/test_convertor.py` & `SimpleSQLite-1.3.2/test/test_convertor.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/test_from_file.py` & `SimpleSQLite-1.3.2/test/test_from_file.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/test_func.py` & `SimpleSQLite-1.3.2/test/test_func.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/test_logger.py` & `SimpleSQLite-1.3.2/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/test_orm.py` & `SimpleSQLite-1.3.2/test/test_orm.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/test_pandas.py` & `SimpleSQLite-1.3.2/test/test_pandas.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/test_query.py` & `SimpleSQLite-1.3.2/test/test_query.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/test_sanitizer.py` & `SimpleSQLite-1.3.2/test/test_sanitizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,46 @@
 """
 
 import pytest
 from tabledata import TableData
 from typepy import String
 
 from simplesqlite import NameValidationError, SQLiteTableDataSanitizer, connect_memdb
+from simplesqlite._sanitizer import is_multibyte_str
 
 from ._common import print_test_result
 
 
+nan = float("nan")
+inf = float("inf")
+
+
+class Test_is_multibyte_str:
+    @pytest.mark.parametrize(
+        ["value", "expected"],
+        [
+            ["吾輩は猫である", True],
+            ["abcdef", False],
+            [
+                "RKBTqn1G9HIZ9onY9mCklj3+8ye7WBmu0xKMqp3ORT3pMgR5m73VXAR/5YrTZTGer"
+                "nMYLCPYdwIMewFY+6xOZmWwCrXjfw3sO2dYLubh9EIMrc/XEvAhMFd969G2yQkyFT"
+                "Nf9M8Ag94QCuBk51yQLSbxgmxJTqEw6bdC4gNTI44=",
+                False,
+            ],
+            [None, False],
+            ["", False],
+            [True, False],
+            [[], False],
+            [1, False],
+        ],
+    )
+    def test_normal(self, value, expected):
+        assert is_multibyte_str(value) == expected
+
+
 class Test_SQLiteTableDataSanitizer:
     @pytest.mark.parametrize(
         ["table_name", "headers", "records", "expected"],
         [
             [
                 "normal",
                 ["a", "b_c"],
```

### Comparing `SimpleSQLite-1.3.1/test/test_simplesqlite.py` & `SimpleSQLite-1.3.2/test/test_simplesqlite.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/test_sqlquery.py` & `SimpleSQLite-1.3.2/test/test_sqlquery.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/test/test_validator.py` & `SimpleSQLite-1.3.2/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.1/tox.ini` & `SimpleSQLite-1.3.2/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 extras =
     test
 commands =
     pytest {posargs}
 
 [testenv:build]
 deps =
+    build>=0.10
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
+    python -m build
     twine check dist/*.whl dist/*.tar.gz
-    python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
```

