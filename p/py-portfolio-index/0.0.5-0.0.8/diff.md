# Comparing `tmp/py-portfolio-index-0.0.5.tar.gz` & `tmp/py-portfolio-index-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-portfolio-index-0.0.5.tar", last modified: Sat Jun 17 15:39:55 2023, max compression
+gzip compressed data, was "py-portfolio-index-0.0.8.tar", last modified: Sat Jun 24 19:17:41 2023, max compression
```

## Comparing `py-portfolio-index-0.0.5.tar` & `py-portfolio-index-0.0.8.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:39:55.370522 py-portfolio-index-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-17 15:39:55.370522 py-portfolio-index-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:39:55.366522 py-portfolio-index-0.0.5/py_portfolio_index/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:39:55.366522 py-portfolio-index-0.0.5/py_portfolio_index/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:39:55.366522 py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2020_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2021_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2022_q2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2022_q3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2022_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2023_q1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/qcln_2020_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:39:55.370522 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/coal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/cruises.csv
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/fake_meat.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/meat_poultry.csv
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/non_ethical_conduct.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-17 15:39:44.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/oil.csv
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/renewable.csv
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/semiconductor.csv
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/space.csv
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/vice.csv
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:39:55.370522 py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/alpaca.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/alpaca_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/base_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/local_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/robinhood.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/py_portfolio_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:39:55.366522 py-portfolio-index-0.0.5/py_portfolio_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-17 15:39:55.000000 py-portfolio-index-0.0.5/py_portfolio_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-17 15:39:55.000000 py-portfolio-index-0.0.5/py_portfolio_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:39:55.000000 py-portfolio-index-0.0.5/py_portfolio_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-17 15:39:55.000000 py-portfolio-index-0.0.5/py_portfolio_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 15:39:55.000000 py-portfolio-index-0.0.5/py_portfolio_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:39:55.370522 py-portfolio-index-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-17 15:39:45.000000 py-portfolio-index-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:41.001037 py-portfolio-index-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-24 19:17:41.001037 py-portfolio-index-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:40.993037 py-portfolio-index-0.0.8/py_portfolio_index/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:40.993037 py-portfolio-index-0.0.8/py_portfolio_index/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:40.997037 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2021_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2023_q1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/qcln_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/sp500_2023_q3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/yolo_gme_2023_q1.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:41.001037 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/coal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/cruises.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/fake_meat.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/meat_poultry.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/non_ethical_conduct.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/oil.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/renewable.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/semiconductor.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/space.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/vice.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:41.001037 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/alpaca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/alpaca_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/local_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/robinhood.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/py_portfolio_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:17:40.993037 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-24 19:17:40.000000 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-24 19:17:40.000000 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:17:40.000000 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-24 19:17:40.000000 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-24 19:17:40.000000 py-portfolio-index-0.0.8/py_portfolio_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:17:41.001037 py-portfolio-index-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-24 19:17:31.000000 py-portfolio-index-0.0.8/setup.py
```

### Comparing `py-portfolio-index-0.0.5/LICENSE.txt` & `py-portfolio-index-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.5/PKG-INFO` & `py-portfolio-index-0.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,56 @@
-Metadata-Version: 2.1
-Name: py-portfolio-index
-Version: 0.0.5
-Summary: Build index portfolios.
-Home-page: 
-Author: 
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: alpaca
-Provides-Extra: robinhood
-License-File: LICENSE.txt
-
 ## Py Portfolio Index
 
-`py-portfolio-index` is a python library to make it easier to mantain a broad, index-based approach to stock investing
-while following individual ESG (Environmental, Social, and Governance) or SRI (Socially Response Investing) goals.
+`py-portfolio-index` is a python library to make it easier to mantain a broad, index-based approach to stock investing while being able to layer in person preferences, such as to exclude or reweight certain kinds of stocks.
+
+ For example, a user could construct a portfolio that matches the composition of the S&P 500, but excludes oil companies and overweights semiconductor companies.
 
 To do that, it provides tools for constructing and managing portfolios that are modeled off indexes. These ideal
-portfolios can be efficiently converted into actual portfolios by API, using commission free platforms like Robinhood or
-Alpaca. Since constructing an index analogue typically requires many small stock purchases, a
-commission free platform is important to minimizing overhead. Robinhood has the additional benefit of allowing fractional
-share purchases, which allow an index to come closer to an ideal match with a smaller total portfolio size. 
+portfolios can be efficiently converted into actual portfolios by API, using commission free platforms like Robinhood or Alpaca. Since constructing an index analogue typically requires many small stock purchases, a
+commission free platform is important to minimizing overhead. For small investment sizes, the ability of the platform to support fractional shares is critical to being able to accurately map to the index.
 
 #### Install
 
 The package supports Python 3.7 plus.
 
 `pip install py-portfolio-index` [Not yet!]
 
 #### Considerations
 
 Some providers may take some time to place an order. Keep this in mind when running repeated rebalances, as the
 portfolio balance may not have updated to reflect your last order.
 
+Also remember that the stock markets are not always open!
+
 #### Basic Example
 
 This example shows a basic example using the Alpaca API in paper trading mode.
 
 It constructs an ideal portfolio based on the composition of the Vanguard ESG index fund in Q4 2020, then uses the
 Alpaca API to construct a matching portfolio based on an initial investment of 10000 dollars.
 
-Since Alpaca doesn't support fractional shares, this portfolio will approximate an index, but cannot match it exactly, 
-especially for small total portfolio sizes.
 
-```python
-from py_portfolio_index import INDEXES, STOCK_LISTS, Logger, AlpacaProvider, PurchaseStrategy, compare_portfolios,
 
-AlpacaProvider
+```python
+from py_portfolio_index import INDEXES, STOCK_LISTS, Logger, AlpacaProvider, PurchaseStrategy, generate_order_plan
 
 from logging import INFO, StreamHandler
 
 Logger.addHandler(StreamHandler())
 Logger.setLevel(INFO)
 
-API_KEY = '#########'
-
-SECRET_KEY = '##########'
 
 # The size of our paper portfolio
 TARGET_PORTFOLIO_SIZE = 10000
 
 # instantiate the Alpaca provider with identity information
 # and set it to use the paper provider
-provider = AlpacaProvider(key_id=API_KEY, secret_key=SECRET_KEY, paper=True)
+# this expects the environment variables ALPACA_API_KEY and ALPACA_API_SECRET to be set,
+# or they can be passed in directly, using AlpacaProvider(key_id=..., secret_key=...)
+provider = AlpacaProvider()
 
 # get an example index 
 # this one is the vanguard ESG index for Q4 202
 ideal_portfolio = INDEXES['esgv_2020_q4']
 
 # exclude all stocks from the oil, vice, and cruise lists
 ideal_portfolio.exclude(STOCK_LISTS['oil']).exclude(STOCK_LISTS['vice']).exclude(STOCK_LISTS['cruises'])
@@ -78,26 +59,28 @@
 ideal_portfolio.reweight(STOCK_LISTS['renewable'], weight=2.0, min_weight=.001)
 ideal_portfolio.reweight(STOCK_LISTS['semiconductor'], weight=2.0, min_weight=.001)
 
 # get actual holdings
 real_port = provider.get_holdings()
 
 # compare actual holdings to this ideal portfolio to produce a buy and sell list
-to_buy, to_sell = compare_portfolios(ideal=ideal_portfolio, real=real_port,
+planned_orders = generate_order_plan(ideal=ideal_portfolio, real=real_port,
                                      buy_order=PurchaseStrategy.LARGEST_DIFF_FIRST,
                                      target_size=TARGET_PORTFOLIO_SIZE)
+# review the orders
+for item in planned_orders.to_buy:
+    print(item)
 
 # purchase the buy list
-provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, fractional_shares=False, skip_errored_stocks=True)
+provider.purchase_order_plan(plan = planned_orders, fractional_shares=False, skip_errored_stocks=False)
 ```
 
 ### Robinhood
 
-Since robinhood supports fractional shares, it's much easier to get close to an index
-with a smaller amount of money. 
+Robinhood has a less reliable API, but it is also commission free and supports fractional shares.
 
 
 ```python
 from py_portfolio_index.bin import INDEXES, STOCK_LISTS
 from py_portfolio_index.enums import PurchaseStrategy
 from py_portfolio_index.operators import compare_portfolios
 from py_portfolio_index.portfolio_providers.robinhood import RobinhoodProvider
@@ -122,41 +105,43 @@
 
 provider = RobinhoodProvider(username='#####', password='#########')
 
 real_port = provider.get_holdings()
 
 TARGET_SIZE = 10000
 
-to_buy, to_sell = compare_portfolios(ideal=ideal_port, real=real_port, buy_order=PurchaseStrategy.CHEAPEST_FIRST,
-                                     target_size = TARGET_SIZE)
-
+planned_orders = generate_order_plan(ideal=ideal_portfolio, real=real_port,
+                                     buy_order=PurchaseStrategy.LARGEST_DIFF_FIRST,
+                                     target_size=TARGET_PORTFOLIO_SIZE)
+# review the orders
+for item in planned_orders.to_buy:
+    print(item)
 
-provider.purchase_ticker_value_dict(to_buy, purchasing_power=1000, fractional_shares=True, skip_errored_stocks=True)
+# purchase the buy list
+provider.purchase_order_plan(plan = planned_orders, fractional_shares=False, skip_errored_stocks=False)
 
 ```
 
 ### Testing
 
 To avoid actually purchasing a stock, use the plan_only option to log what trades would have occurred.
 
 ```python
 
-provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, plan_only=True, fractional_shares=False,
-                                    skip_errored_stocks=True, )
+provider.purchase_order_plan(plan = planned_orders, plan_only=True )
 
 ```
 
 ### Example Scripts
 
 Can be found in the examples folder.
 
 ### Logging
 
-To see messages, it's helpful to configure the logger to print messages. You can either configure the standard python
-logger or use the portfolio specific one using an example like the below.
+It can be helpful to configure the logger to print messages. You can either configure the standard python logger or use the portfolio specific one using an example like the below.
 
 ```python
 from py_portfolio_index.constants import Logger
 from logging import INFO, StreamHandler
 
 Logger.addHandler(StreamHandler())
 Logger.setLevel(INFO)
```

### Comparing `py-portfolio-index-0.0.5/README.md` & `py-portfolio-index-0.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,72 @@
+Metadata-Version: 2.1
+Name: py-portfolio-index
+Version: 0.0.8
+Summary: Build index portfolios.
+Home-page: 
+Author: 
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+Provides-Extra: alpaca
+Provides-Extra: robinhood
+License-File: LICENSE.txt
+
 ## Py Portfolio Index
 
-`py-portfolio-index` is a python library to make it easier to mantain a broad, index-based approach to stock investing
-while following individual ESG (Environmental, Social, and Governance) or SRI (Socially Response Investing) goals.
+`py-portfolio-index` is a python library to make it easier to mantain a broad, index-based approach to stock investing while being able to layer in person preferences, such as to exclude or reweight certain kinds of stocks.
+
+ For example, a user could construct a portfolio that matches the composition of the S&P 500, but excludes oil companies and overweights semiconductor companies.
 
 To do that, it provides tools for constructing and managing portfolios that are modeled off indexes. These ideal
-portfolios can be efficiently converted into actual portfolios by API, using commission free platforms like Robinhood or
-Alpaca. Since constructing an index analogue typically requires many small stock purchases, a
-commission free platform is important to minimizing overhead. Robinhood has the additional benefit of allowing fractional
-share purchases, which allow an index to come closer to an ideal match with a smaller total portfolio size. 
+portfolios can be efficiently converted into actual portfolios by API, using commission free platforms like Robinhood or Alpaca. Since constructing an index analogue typically requires many small stock purchases, a
+commission free platform is important to minimizing overhead. For small investment sizes, the ability of the platform to support fractional shares is critical to being able to accurately map to the index.
 
 #### Install
 
 The package supports Python 3.7 plus.
 
 `pip install py-portfolio-index` [Not yet!]
 
 #### Considerations
 
 Some providers may take some time to place an order. Keep this in mind when running repeated rebalances, as the
 portfolio balance may not have updated to reflect your last order.
 
+Also remember that the stock markets are not always open!
+
 #### Basic Example
 
 This example shows a basic example using the Alpaca API in paper trading mode.
 
 It constructs an ideal portfolio based on the composition of the Vanguard ESG index fund in Q4 2020, then uses the
 Alpaca API to construct a matching portfolio based on an initial investment of 10000 dollars.
 
-Since Alpaca doesn't support fractional shares, this portfolio will approximate an index, but cannot match it exactly, 
-especially for small total portfolio sizes.
 
-```python
-from py_portfolio_index import INDEXES, STOCK_LISTS, Logger, AlpacaProvider, PurchaseStrategy, compare_portfolios,
 
-AlpacaProvider
+```python
+from py_portfolio_index import INDEXES, STOCK_LISTS, Logger, AlpacaProvider, PurchaseStrategy, generate_order_plan
 
 from logging import INFO, StreamHandler
 
 Logger.addHandler(StreamHandler())
 Logger.setLevel(INFO)
 
-API_KEY = '#########'
-
-SECRET_KEY = '##########'
 
 # The size of our paper portfolio
 TARGET_PORTFOLIO_SIZE = 10000
 
 # instantiate the Alpaca provider with identity information
 # and set it to use the paper provider
-provider = AlpacaProvider(key_id=API_KEY, secret_key=SECRET_KEY, paper=True)
+# this expects the environment variables ALPACA_API_KEY and ALPACA_API_SECRET to be set,
+# or they can be passed in directly, using AlpacaProvider(key_id=..., secret_key=...)
+provider = AlpacaProvider()
 
 # get an example index 
 # this one is the vanguard ESG index for Q4 202
 ideal_portfolio = INDEXES['esgv_2020_q4']
 
 # exclude all stocks from the oil, vice, and cruise lists
 ideal_portfolio.exclude(STOCK_LISTS['oil']).exclude(STOCK_LISTS['vice']).exclude(STOCK_LISTS['cruises'])
@@ -62,26 +75,28 @@
 ideal_portfolio.reweight(STOCK_LISTS['renewable'], weight=2.0, min_weight=.001)
 ideal_portfolio.reweight(STOCK_LISTS['semiconductor'], weight=2.0, min_weight=.001)
 
 # get actual holdings
 real_port = provider.get_holdings()
 
 # compare actual holdings to this ideal portfolio to produce a buy and sell list
-to_buy, to_sell = compare_portfolios(ideal=ideal_portfolio, real=real_port,
+planned_orders = generate_order_plan(ideal=ideal_portfolio, real=real_port,
                                      buy_order=PurchaseStrategy.LARGEST_DIFF_FIRST,
                                      target_size=TARGET_PORTFOLIO_SIZE)
+# review the orders
+for item in planned_orders.to_buy:
+    print(item)
 
 # purchase the buy list
-provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, fractional_shares=False, skip_errored_stocks=True)
+provider.purchase_order_plan(plan = planned_orders, fractional_shares=False, skip_errored_stocks=False)
 ```
 
 ### Robinhood
 
-Since robinhood supports fractional shares, it's much easier to get close to an index
-with a smaller amount of money. 
+Robinhood has a less reliable API, but it is also commission free and supports fractional shares.
 
 
 ```python
 from py_portfolio_index.bin import INDEXES, STOCK_LISTS
 from py_portfolio_index.enums import PurchaseStrategy
 from py_portfolio_index.operators import compare_portfolios
 from py_portfolio_index.portfolio_providers.robinhood import RobinhoodProvider
@@ -106,41 +121,43 @@
 
 provider = RobinhoodProvider(username='#####', password='#########')
 
 real_port = provider.get_holdings()
 
 TARGET_SIZE = 10000
 
-to_buy, to_sell = compare_portfolios(ideal=ideal_port, real=real_port, buy_order=PurchaseStrategy.CHEAPEST_FIRST,
-                                     target_size = TARGET_SIZE)
-
+planned_orders = generate_order_plan(ideal=ideal_portfolio, real=real_port,
+                                     buy_order=PurchaseStrategy.LARGEST_DIFF_FIRST,
+                                     target_size=TARGET_PORTFOLIO_SIZE)
+# review the orders
+for item in planned_orders.to_buy:
+    print(item)
 
-provider.purchase_ticker_value_dict(to_buy, purchasing_power=1000, fractional_shares=True, skip_errored_stocks=True)
+# purchase the buy list
+provider.purchase_order_plan(plan = planned_orders, fractional_shares=False, skip_errored_stocks=False)
 
 ```
 
 ### Testing
 
 To avoid actually purchasing a stock, use the plan_only option to log what trades would have occurred.
 
 ```python
 
-provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, plan_only=True, fractional_shares=False,
-                                    skip_errored_stocks=True, )
+provider.purchase_order_plan(plan = planned_orders, plan_only=True )
 
 ```
 
 ### Example Scripts
 
 Can be found in the examples folder.
 
 ### Logging
 
-To see messages, it's helpful to configure the logger to print messages. You can either configure the standard python
-logger or use the portfolio specific one using an example like the below.
+It can be helpful to configure the logger to print messages. You can either configure the standard python logger or use the portfolio specific one using an example like the below.
 
 ```python
 from py_portfolio_index.constants import Logger
 from logging import INFO, StreamHandler
 
 Logger.addHandler(StreamHandler())
 Logger.setLevel(INFO)
```

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2020_q4.csv` & `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2021_q4.csv` & `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2021_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2022_q2.csv` & `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q2.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2022_q3.csv` & `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q3.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2022_q4.csv` & `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2022_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/esgv_2023_q1.csv` & `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/esgv_2023_q1.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/inventory.py` & `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Set
 import re
 from datetime import date
-from decimal import Decimal 
+from decimal import Decimal
 from pydantic import BaseModel, Field
 from pathlib import Path
 
 from py_portfolio_index.models import IdealPortfolioElement, IdealPortfolio
 
 QUARTER_TO_MONTH = {1: 1, 2: 4, 3: 7, 4: 10}
 
 
-def parse_date_from_name(input: str)-> date | None:
+def parse_date_from_name(input: str) -> date | None:
     components = input.lower().split("_")
     year = None
     quarter = None
     for item in components:
         if re.match("[0-9]{4}", item):
             year = int(item)
         if re.match("q[1-4]", item):
@@ -24,29 +24,29 @@
 
     return date(year=year, month=QUARTER_TO_MONTH[quarter], day=1)
 
 
 class IndexInventory(BaseModel):
     keys: Set[str] = Field(exclude=True)
     base: Path = Field(exclude=True)
-    loaded: dict[str, IdealPortfolio] = Field(default_factory = dict)
+    loaded: dict[str, IdealPortfolio] = Field(default_factory=dict)
 
     @classmethod
     def from_path(cls, path):
         path = Path(path)
         if path.is_file():
             path = path.parent
         keys = []
         for f in path.iterdir():
             try:
                 if f.suffix == ".csv":
                     keys.append(f.stem)
             except FileNotFoundError:
                 pass
-        return IndexInventory(keys = keys, base = path)
+        return IndexInventory(keys=keys, base=path)
 
     def __getitem__(self, item: str) -> IdealPortfolio:
         if item in self.keys:
             values = self.loaded.get(item, None)
             if values:
                 return values
             values = self.get_values(item)
```

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/qcln_2020_q4.csv` & `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/qcln_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv` & `py-portfolio-index-0.0.8/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/inventory.py` & `py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/inventory.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from typing import List, Set
 from pathlib import Path
 
 
 class StocklistInventory(BaseModel):
     keys: Set[str] = Field(exclude=True)
     base: Path = Field(exclude=True)
-    loaded: dict[str, List[str]] = Field(default_factory = dict)
+    loaded: dict[str, List[str]] = Field(default_factory=dict)
 
     @classmethod
     def from_path(cls, path):
         path = Path(path)
         if path.is_file():
             path = path.parent
         keys = []
         for f in path.iterdir():
             try:
                 if f.suffix == ".csv":
                     keys.append(f.stem)
             except FileNotFoundError:
                 pass
-        return StocklistInventory(keys = keys, base = path)
-    
+        return StocklistInventory(keys=keys, base=path)
+
     def __getitem__(self, item: str) -> List[str]:
         if item in self.keys:
             values = self.loaded.get(item, None)
             if values:
                 return values
             values = self.get_values(item)
             self.loaded[item] = values
```

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/bin/lists/oil.csv` & `py-portfolio-index-0.0.8/py_portfolio_index/bin/lists/oil.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/config.py` & `py-portfolio-index-0.0.8/py_portfolio_index/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from dataclasses import dataclass
 from py_portfolio_index.enums import Currency, Provider
 from typing import List
 
+
 @dataclass
 class Config:
     default_currency = Currency.USD
 
-def get_providers()->List[Provider]:
+
+def get_providers() -> List[Provider]:
     providers = []
     try:
         from alpaca.trading.client import TradingClient  # noqa: F401
+
         providers.append(Provider.ALPACA)
     except ImportError:
         pass
     try:
         import robin_stocks.robinhood as r  # noqa: F401
+
         providers.append(Provider.ROBINHOOD)
     except ImportError:
         pass
     return providers
```

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/models.py` & `py-portfolio-index-0.0.8/py_portfolio_index/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,38 @@
 from typing import List, Optional, Union, TYPE_CHECKING
 from pydantic import BaseModel, Field, validator
 from pandas import DataFrame
 from py_portfolio_index.enums import Currency
 from py_portfolio_index.constants import Logger
 from py_portfolio_index.exceptions import PriceFetchError
 from decimal import Decimal
+from enum import Enum
 
 if TYPE_CHECKING:
     from py_portfolio_index.portfolio_providers.base_portfolio import BaseProvider
 
 
 class Money(BaseModel):
     value: Union[Decimal, int, float, "Money"]
     currency: Currency = Currency.USD
 
+    @property
+    def decimal(self) -> Decimal:
+        return self.value #type: ignore
+    
     @validator("value", pre=True)
-    def coerce_to_decimal(cls, v):
-        if isinstance(v, int):
+    def coerce_to_decimal(cls, v)-> Decimal:
+        if isinstance(v, (int, float)):
             return Decimal(v)
-        if isinstance(v, Money):
+        elif isinstance(v, Money):
             # TODO convert this
-            return Decimal(v.value)
-        return v
+            return v.decimal
+        elif isinstance(v, Decimal):
+            return v
+        return Decimal(v)
 
     def __str__(self):
         return f"{self.currency.value}{self.value}"
 
     def __repr__(self):
         return str(self)
 
@@ -113,30 +120,29 @@
     holdings: List[IdealPortfolioElement]
     source_date: Optional[date] = Field(default_factory=date.today)
 
     def _reweight_portfolio(self):
         weights: Decimal = sum([item.weight for item in self.holdings])
 
         scaling_factor = Decimal(1) / weights
-
         for item in self.holdings:
             item.weight = item.weight * scaling_factor
 
     def exclude(self, exclusion_list: List[str]):
         reweighted = []
         excluded = Decimal(0.0)
         for ticker in exclusion_list:
             reweighted.append(ticker)
             for item in self.holdings:
                 if item.ticker == ticker:
                     excluded += item.weight
                     item.weight = Decimal(0.0)
 
         self.holdings = [
-            item for item in self.holdings if item.ticker not in [reweighted]
+            item for item in self.holdings if item.ticker not in reweighted
         ]
         self._reweight_portfolio()
         Logger.info(
             f"Set the following stocks to weight 0 {reweighted}. Total value excluded {excluded}."
         )
         return self
 
@@ -160,14 +166,15 @@
                     found = True
             if not found:
                 reweighted.append(ticker)
                 total_value += cmin_weight
                 self.holdings.append(
                     IdealPortfolioElement(ticker=ticker, weight=cmin_weight)
                 )
+            
         self._reweight_portfolio()
         Logger.info(
             f"modified the following by weight {cweight} {reweighted}. Total value modified {total_value}."
         )
         return self
 
     def reweight_to_present(self, provider: "BaseProvider"):
@@ -209,22 +216,24 @@
 
 
 class RealPortfolioElement(IdealPortfolioElement):
     ticker: str
     units: Decimal
     value: Money
     weight: Decimal = Decimal(0.0)
+    unsettled: bool = False
 
     @validator("value", pre=True)
     def value_coercion(cls, v) -> Money:
         return Money.parse(v)
 
 
 class RealPortfolio(IdealPortfolio):
     holdings: List[RealPortfolioElement]  # type: ignore
+    cash: None | Money = None
 
     @property
     def _index(self):
         return {val.ticker: val for val in self.holdings}
 
     def get_holding(self, ticker: str):
         return self._index.get(ticker)
@@ -253,7 +262,24 @@
             self.add_holding(other)
         elif isinstance(other, RealPortfolio):
             for item in other.holdings:
                 self.add_holding(item)
         else:
             raise ValueError
         return self
+
+
+class OrderType(Enum):
+    BUY = "BUY"
+    SELL = "SELL"
+
+
+class OrderElement(BaseModel):
+    ticker: str
+    order_type: OrderType
+    value: Money | None
+    qty: int | None
+
+
+class OrderPlan(BaseModel):
+    to_buy: List[OrderElement]
+    to_sell: List[OrderElement]
```

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/alpaca.py` & `py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/alpaca.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,32 @@
 from typing import Optional
 from datetime import date, datetime, timezone, timedelta
 from functools import lru_cache
 
 from os import environ
 
 
-
-
 class AlpacaProviderLegacy(BaseProvider):
-    def __init__(self, key_id: str | None = None, secret_key: str | None = None, paper: bool = False):
+    def __init__(
+        self,
+        key_id: str | None = None,
+        secret_key: str | None = None,
+        paper: bool = False,
+    ):
         import alpaca_trade_api as tradeapi
         from alpaca_trade_api.common import URL
+
         if not key_id:
-            key_id = environ.get('ALPACA_API_KEY', None)
+            key_id = environ.get("ALPACA_API_KEY", None)
         if not secret_key:
-            secret_key = environ.get('ALPACA_API_SECRET', None)
+            secret_key = environ.get("ALPACA_API_SECRET", None)
         if not (key_id and secret_key):
-            raise ValueError('Must provide key_id and secret_key or set environment variables ALPACA_API_KEY and ALPACA_API_SECRET ')
+            raise ValueError(
+                "Must provide key_id and secret_key or set environment variables ALPACA_API_KEY and ALPACA_API_SECRET "
+            )
         TARGET_URL = (
             "https://paper-api.alpaca.markets"
             if paper
             else "https://api.alpaca.markets"
         )
         self.api = tradeapi.REST(
             key_id=key_id, secret_key=secret_key, base_url=URL(TARGET_URL)
@@ -64,15 +70,14 @@
                     end=end.isoformat(),
                 )
                 # take the first day after target day
                 return Decimal(raw[0].h)
             return Decimal(raw.ap)
 
     def buy_instrument(self, ticker: str, qty: Decimal):
-
         qty_float = float(qty)
         self.api.submit_order(
             symbol=ticker,
             qty=qty_float,
             side="buy",
             type="market",
             time_in_force="day",
```

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/alpaca_v2.py` & `py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/alpaca_v2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from py_portfolio_index.models import RealPortfolio, RealPortfolioElement, Money
+from py_portfolio_index.exceptions import ConfigurationError, OrderError
 from .base_portfolio import BaseProvider
 from decimal import Decimal
 from typing import Optional
 from datetime import date, datetime, timezone, timedelta
 from functools import lru_cache
 
+
 from os import environ
 
 
 class AlpacaProvider(BaseProvider):
     def __init__(
         self,
         key_id: str | None = None,
@@ -19,15 +21,15 @@
         from alpaca.data.historical import StockHistoricalDataClient
 
         if not key_id:
             key_id = environ.get("ALPACA_API_KEY", None)
         if not secret_key:
             secret_key = environ.get("ALPACA_API_SECRET", None)
         if not (key_id and secret_key):
-            raise ValueError(
+            raise ConfigurationError(
                 "Must provide key_id and secret_key or set environment variables ALPACA_API_KEY and ALPACA_API_SECRET "
             )
         self.trading_client = TradingClient(
             api_key=key_id, secret_key=secret_key, paper=False
         )
         self.historical_client = StockHistoricalDataClient(
             api_key=key_id, secret_key=secret_key
@@ -94,44 +96,71 @@
                 # take the first day after target day
                 return Decimal(raw[ticker][0].high)
             return Decimal(raw[ticker].ask_price)
 
     def buy_instrument(self, ticker: str, qty: Decimal):
         from alpaca.trading.requests import MarketOrderRequest
         from alpaca.trading.enums import OrderSide, TimeInForce
+        from alpaca.common.exceptions import APIError
 
         market_order_data = MarketOrderRequest(
             symbol=ticker,
             qty=float(qty),
             side=OrderSide.BUY,
             time_in_force=TimeInForce.DAY,
         )
-        self.trading_client.submit_order(order_data=market_order_data)
-
+        try:
+            self.trading_client.submit_order(order_data=market_order_data)
+        except APIError as e:
+            import json
+            error = json.loads(e._error)
+            message = error.get('message', 'Unknown Error')
+            raise OrderError(message= f"Failed to buy {ticker} {qty} {e}: {message}")
         return True
 
     def get_unsettled_instruments(self):
         from alpaca.trading.requests import GetOrdersRequest, QueryOrderStatus
 
         open_orders = self.trading_client.get_orders(
             filter=GetOrdersRequest(status=QueryOrderStatus.OPEN)
         )
         return set([o.symbol for o in open_orders])
 
     def get_holdings(self):
         from decimal import Decimal
 
         my_stocks = self.trading_client.get_all_positions()
-
+        account = self.trading_client.get_account()
+        unsettled = self.get_unsettled_instruments()
+        unsettled_elements = [
+            RealPortfolioElement(
+                ticker=ticker,
+                units=0,
+                value=Money(value=Decimal(0)),
+                weight=Decimal(0),
+                unsettled=True,
+            )
+            for ticker in unsettled
+        ]
         if not my_stocks:
-            return RealPortfolio(holdings=[])
+            return RealPortfolio(
+                holdings=unsettled_elements, cash=Money(value=account.cash)
+            )
         total_value = sum([Decimal(item.market_value) for item in my_stocks])
         out = [
             RealPortfolioElement(
                 ticker=row.symbol,
                 units=row.qty,
                 value=Money(value=Decimal(row.market_value)),
                 weight=Decimal(row.market_value) / total_value,
+                unsettled=row.symbol in unsettled,
             )
             for row in my_stocks
         ]
-        return RealPortfolio(holdings=out)
+
+        extra_unsettled = [
+            item
+            for item in unsettled_elements
+            if item.ticker not in [x.ticker for x in out]
+        ]
+        out.extend(extra_unsettled)
+        return RealPortfolio(holdings=out, cash=Money(value=account.cash))
```

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/base_portfolio.py` & `py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/base_portfolio.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from math import floor, ceil
 from typing import Dict, Union, Optional, Set
 from decimal import Decimal
 from datetime import date
 
-from py_portfolio_index.common import print_money, print_per
+from py_portfolio_index.common import print_money, print_per, round_up_to_place
 from py_portfolio_index.constants import Logger
 from py_portfolio_index.enums import RoundingStrategy
 from py_portfolio_index.exceptions import PriceFetchError
-from py_portfolio_index.models import Money
+from py_portfolio_index.models import Money, OrderPlan
 from functools import lru_cache
 
 
 class BaseProvider(object):
+    MIN_ORDER_VALUE = Money(value=1)
+    MAX_ORDER_DECIMALS = 2
+    
     def _get_instrument_price(self, ticker: str, at_day: Optional[date] = None):
         raise NotImplementedError
 
     @lru_cache(maxsize=None)
     def get_instrument_price(
         self, ticker: str, at_day: Optional[date] = None
     ) -> Optional[Decimal]:
         try:
             return self._get_instrument_price(ticker, at_day)
         except NotImplementedError as e:
             raise e
         except Exception as e:
             raise PriceFetchError(e)
 
-    def buy_instrument(self, ticker: str, qty: Decimal)->bool:
+    def buy_instrument(self, ticker: str, qty: Decimal) -> bool:
         raise NotImplementedError
 
     def get_unsettled_instruments(self) -> Set[str]:
-
         raise NotImplementedError
 
     def purchase_ticker_value_dict(
         self,
         to_buy: Dict[str, Money],
-        purchasing_power: Union[Money, Decimal, int, float], 
+        purchasing_power: Union[Money, Decimal, int, float],
         plan_only: bool = False,
         fractional_shares: bool = True,
         skip_errored_stocks=False,
         rounding_strategy=RoundingStrategy.CLOSEST,
         ignore_unsettled: bool = True,
     ):
         purchased = Money(value=0)
@@ -56,15 +58,15 @@
             if key in unsettled:
                 Logger.info(f"Skipping {key} with unsettled orders.")
                 continue
             try:
                 raw_price = self.get_instrument_price(key)
                 if not raw_price:
                     raise ValueError(f"No price found for this instrument: {key}")
-                price:Money = Money(value=raw_price)
+                price: Money = Money(value=raw_price)
                 Logger.info(f"got price of {price} for {key}")
             except Exception as e:
                 if not skip_errored_stocks:
                     raise e
                 else:
                     continue
             if not price:
@@ -100,25 +102,74 @@
                 to_buy_units = Decimal(round(purchasing / price, 4).value)
             if to_buy_units > Decimal(0):
                 Logger.info(f"going to buy {to_buy_units} of {key}")
                 try:
                     if not plan_only:
                         successfully_purchased = self.buy_instrument(key, to_buy_units)
                     if successfully_purchased:
-                        purchasing_power_resolved = purchasing_power_resolved - purchasing
+                        purchasing_power_resolved = (
+                            purchasing_power_resolved - purchasing
+                        )
                         purchased += purchasing
                         diff += abs(value - purchasing)
                         Logger.info(
                             f"bought {to_buy_units} of {key}, {purchasing_power_resolved} left"
                         )
                 except Exception as e:
                     print(e)
                     if not skip_errored_stocks:
                         raise e
             if break_flag:
                 Logger.info(
                     f"No purchasing power left, purchased {print_money(purchased)} of {print_money(target_value)}."
-                )    
+                )
                 break
         Logger.info(
             f"$ diff from ideal for purchased stocks was {print_money(diff)}. {print_per(diff / target_value)} of total purchase goal."
         )
+
+    def purchase_order_plan(
+        self,
+        plan: OrderPlan,
+        skip_errored_stocks=False,
+        ignore_unsettled: bool = True,
+        plan_only:bool = False
+    ):
+        if ignore_unsettled:
+            unsettled = self.get_unsettled_instruments()
+        else:
+            unsettled = set()
+        for item in plan.to_buy:
+            if item.ticker in unsettled:
+                Logger.info(f"Skipping {item.ticker} with unsettled orders.")
+                continue
+
+            # round decimal units to 4 places
+            if item.qty:
+                units = Decimal(item.qty)
+            elif item.value:
+                try:
+                    raw_price = self.get_instrument_price(item.ticker)
+                    if not raw_price:
+                        raise ValueError(
+                            f"No price found for this instrument: {item.ticker}"
+                        )
+                    price: Money = Money(value=raw_price)
+                    Logger.info(f"got price of {price} for {item.ticker}")
+                except Exception as e:
+                    if not skip_errored_stocks:
+                        raise e
+                    else:
+                        continue
+                units = round_up_to_place((item.value/price).value, self.MAX_ORDER_DECIMALS)
+            else:
+                raise ValueError("Order element must have qty or value")
+            try:
+                if not plan_only:
+                    self.buy_instrument(item.ticker, units)
+                    Logger.info(f"Bought {units} of {item.ticker}")
+                else:
+                    Logger.info(f"Would have bought {units} of {item.ticker}")
+            except Exception as e:
+                print(e)
+                if not skip_errored_stocks:
+                    raise e
```

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/local_dict.py` & `py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/local_dict.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index/portfolio_providers/robinhood.py` & `py-portfolio-index-0.0.8/py_portfolio_index/portfolio_providers/robinhood.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from decimal import Decimal
 from time import sleep
 from datetime import date, datetime
 import pandas as pd
 from typing import Optional
-
+from py_portfolio_index.exceptions import ConfigurationError
 from py_portfolio_index.constants import Logger
 from py_portfolio_index.models import RealPortfolio, RealPortfolioElement
 from .base_portfolio import BaseProvider
 from py_portfolio_index.exceptions import PriceFetchError
 from functools import lru_cache
 from os import environ
 
@@ -38,15 +38,15 @@
         import robin_stocks.robinhood as r
 
         if not username:
             username = environ.get("ROBINHOOD_USERNAME", None)
         if not password:
             password = environ.get("ROBINHOOD_PASSWORD", None)
         if not (username and password):
-            raise ValueError(
+            raise ConfigurationError(
                 "Must provide username and password arguments or set environment variables ROBINHOOD_USERNAME and ROBINHOOD_PASSWORD "
             )
         self._provider = r
         BaseProvider.__init__(self)
         self._provider.login(username=username, password=password)
 
     @lru_cache(maxsize=None)
```

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index.egg-info/PKG-INFO` & `py-portfolio-index-0.0.8/py_portfolio_index.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-index
-Version: 0.0.5
+Version: 0.0.8
 Summary: Build index portfolios.
 Home-page: 
 Author: 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,64 +12,61 @@
 Description-Content-Type: text/markdown
 Provides-Extra: alpaca
 Provides-Extra: robinhood
 License-File: LICENSE.txt
 
 ## Py Portfolio Index
 
-`py-portfolio-index` is a python library to make it easier to mantain a broad, index-based approach to stock investing
-while following individual ESG (Environmental, Social, and Governance) or SRI (Socially Response Investing) goals.
+`py-portfolio-index` is a python library to make it easier to mantain a broad, index-based approach to stock investing while being able to layer in person preferences, such as to exclude or reweight certain kinds of stocks.
+
+ For example, a user could construct a portfolio that matches the composition of the S&P 500, but excludes oil companies and overweights semiconductor companies.
 
 To do that, it provides tools for constructing and managing portfolios that are modeled off indexes. These ideal
-portfolios can be efficiently converted into actual portfolios by API, using commission free platforms like Robinhood or
-Alpaca. Since constructing an index analogue typically requires many small stock purchases, a
-commission free platform is important to minimizing overhead. Robinhood has the additional benefit of allowing fractional
-share purchases, which allow an index to come closer to an ideal match with a smaller total portfolio size. 
+portfolios can be efficiently converted into actual portfolios by API, using commission free platforms like Robinhood or Alpaca. Since constructing an index analogue typically requires many small stock purchases, a
+commission free platform is important to minimizing overhead. For small investment sizes, the ability of the platform to support fractional shares is critical to being able to accurately map to the index.
 
 #### Install
 
 The package supports Python 3.7 plus.
 
 `pip install py-portfolio-index` [Not yet!]
 
 #### Considerations
 
 Some providers may take some time to place an order. Keep this in mind when running repeated rebalances, as the
 portfolio balance may not have updated to reflect your last order.
 
+Also remember that the stock markets are not always open!
+
 #### Basic Example
 
 This example shows a basic example using the Alpaca API in paper trading mode.
 
 It constructs an ideal portfolio based on the composition of the Vanguard ESG index fund in Q4 2020, then uses the
 Alpaca API to construct a matching portfolio based on an initial investment of 10000 dollars.
 
-Since Alpaca doesn't support fractional shares, this portfolio will approximate an index, but cannot match it exactly, 
-especially for small total portfolio sizes.
 
-```python
-from py_portfolio_index import INDEXES, STOCK_LISTS, Logger, AlpacaProvider, PurchaseStrategy, compare_portfolios,
 
-AlpacaProvider
+```python
+from py_portfolio_index import INDEXES, STOCK_LISTS, Logger, AlpacaProvider, PurchaseStrategy, generate_order_plan
 
 from logging import INFO, StreamHandler
 
 Logger.addHandler(StreamHandler())
 Logger.setLevel(INFO)
 
-API_KEY = '#########'
-
-SECRET_KEY = '##########'
 
 # The size of our paper portfolio
 TARGET_PORTFOLIO_SIZE = 10000
 
 # instantiate the Alpaca provider with identity information
 # and set it to use the paper provider
-provider = AlpacaProvider(key_id=API_KEY, secret_key=SECRET_KEY, paper=True)
+# this expects the environment variables ALPACA_API_KEY and ALPACA_API_SECRET to be set,
+# or they can be passed in directly, using AlpacaProvider(key_id=..., secret_key=...)
+provider = AlpacaProvider()
 
 # get an example index 
 # this one is the vanguard ESG index for Q4 202
 ideal_portfolio = INDEXES['esgv_2020_q4']
 
 # exclude all stocks from the oil, vice, and cruise lists
 ideal_portfolio.exclude(STOCK_LISTS['oil']).exclude(STOCK_LISTS['vice']).exclude(STOCK_LISTS['cruises'])
@@ -78,26 +75,28 @@
 ideal_portfolio.reweight(STOCK_LISTS['renewable'], weight=2.0, min_weight=.001)
 ideal_portfolio.reweight(STOCK_LISTS['semiconductor'], weight=2.0, min_weight=.001)
 
 # get actual holdings
 real_port = provider.get_holdings()
 
 # compare actual holdings to this ideal portfolio to produce a buy and sell list
-to_buy, to_sell = compare_portfolios(ideal=ideal_portfolio, real=real_port,
+planned_orders = generate_order_plan(ideal=ideal_portfolio, real=real_port,
                                      buy_order=PurchaseStrategy.LARGEST_DIFF_FIRST,
                                      target_size=TARGET_PORTFOLIO_SIZE)
+# review the orders
+for item in planned_orders.to_buy:
+    print(item)
 
 # purchase the buy list
-provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, fractional_shares=False, skip_errored_stocks=True)
+provider.purchase_order_plan(plan = planned_orders, fractional_shares=False, skip_errored_stocks=False)
 ```
 
 ### Robinhood
 
-Since robinhood supports fractional shares, it's much easier to get close to an index
-with a smaller amount of money. 
+Robinhood has a less reliable API, but it is also commission free and supports fractional shares.
 
 
 ```python
 from py_portfolio_index.bin import INDEXES, STOCK_LISTS
 from py_portfolio_index.enums import PurchaseStrategy
 from py_portfolio_index.operators import compare_portfolios
 from py_portfolio_index.portfolio_providers.robinhood import RobinhoodProvider
@@ -122,41 +121,43 @@
 
 provider = RobinhoodProvider(username='#####', password='#########')
 
 real_port = provider.get_holdings()
 
 TARGET_SIZE = 10000
 
-to_buy, to_sell = compare_portfolios(ideal=ideal_port, real=real_port, buy_order=PurchaseStrategy.CHEAPEST_FIRST,
-                                     target_size = TARGET_SIZE)
-
+planned_orders = generate_order_plan(ideal=ideal_portfolio, real=real_port,
+                                     buy_order=PurchaseStrategy.LARGEST_DIFF_FIRST,
+                                     target_size=TARGET_PORTFOLIO_SIZE)
+# review the orders
+for item in planned_orders.to_buy:
+    print(item)
 
-provider.purchase_ticker_value_dict(to_buy, purchasing_power=1000, fractional_shares=True, skip_errored_stocks=True)
+# purchase the buy list
+provider.purchase_order_plan(plan = planned_orders, fractional_shares=False, skip_errored_stocks=False)
 
 ```
 
 ### Testing
 
 To avoid actually purchasing a stock, use the plan_only option to log what trades would have occurred.
 
 ```python
 
-provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, plan_only=True, fractional_shares=False,
-                                    skip_errored_stocks=True, )
+provider.purchase_order_plan(plan = planned_orders, plan_only=True )
 
 ```
 
 ### Example Scripts
 
 Can be found in the examples folder.
 
 ### Logging
 
-To see messages, it's helpful to configure the logger to print messages. You can either configure the standard python
-logger or use the portfolio specific one using an example like the below.
+It can be helpful to configure the logger to print messages. You can either configure the standard python logger or use the portfolio specific one using an example like the below.
 
 ```python
 from py_portfolio_index.constants import Logger
 from logging import INFO, StreamHandler
 
 Logger.addHandler(StreamHandler())
 Logger.setLevel(INFO)
```

### Comparing `py-portfolio-index-0.0.5/py_portfolio_index.egg-info/SOURCES.txt` & `py-portfolio-index-0.0.8/py_portfolio_index.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 py_portfolio_index/bin/indexes/esgv_2021_q4.csv
 py_portfolio_index/bin/indexes/esgv_2022_q2.csv
 py_portfolio_index/bin/indexes/esgv_2022_q3.csv
 py_portfolio_index/bin/indexes/esgv_2022_q4.csv
 py_portfolio_index/bin/indexes/esgv_2023_q1.csv
 py_portfolio_index/bin/indexes/inventory.py
 py_portfolio_index/bin/indexes/qcln_2020_q4.csv
+py_portfolio_index/bin/indexes/sp500_2023_q3.csv
 py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
+py_portfolio_index/bin/indexes/yolo_gme_2023_q1.csv
 py_portfolio_index/bin/lists/__init__.py
 py_portfolio_index/bin/lists/coal.csv
 py_portfolio_index/bin/lists/cruises.csv
 py_portfolio_index/bin/lists/fake_meat.csv
 py_portfolio_index/bin/lists/inventory.py
 py_portfolio_index/bin/lists/meat_poultry.csv
 py_portfolio_index/bin/lists/non_ethical_conduct.csv
```

### Comparing `py-portfolio-index-0.0.5/setup.py` & `py-portfolio-index-0.0.8/setup.py`

 * *Files identical despite different names*

