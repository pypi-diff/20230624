# Comparing `tmp/scrapy_db-0.0.1.tar.gz` & `tmp/scrapy_db-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_db-0.0.1.tar", max compression
+gzip compressed data, was "scrapy_db-0.0.2.tar", max compression
```

## Comparing `scrapy_db-0.0.1.tar` & `scrapy_db-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-06-07 10:34:22.421846 scrapy_db-0.0.1/LICENSE
--rw-r--r--   0        0        0     1547 2023-06-24 10:48:36.684160 scrapy_db-0.0.1/README.md
--rw-r--r--   0        0        0     1215 2023-06-24 10:48:36.684944 scrapy_db-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      107 2023-06-22 16:25:04.738354 scrapy_db-0.0.1/scrapy_db/__init__.py
--rw-r--r--   0        0        0     5350 2023-06-14 03:38:46.820214 scrapy_db-0.0.1/scrapy_db/db.py
--rw-r--r--   0        0        0      475 2023-06-13 15:04:25.223531 scrapy_db-0.0.1/scrapy_db/defaults.py
--rw-r--r--   0        0        0     3256 2023-06-15 02:02:42.898109 scrapy_db-0.0.1/scrapy_db/dupefilter.py
--rw-r--r--   0        0        0     2473 2023-06-14 03:15:23.908321 scrapy_db-0.0.1/scrapy_db/queue.py
--rw-r--r--   0        0        0     4381 2023-06-13 15:04:25.224164 scrapy_db-0.0.1/scrapy_db/scheduler.py
--rw-r--r--   0        0        0     4705 2023-06-13 15:04:25.224356 scrapy_db-0.0.1/scrapy_db/spiders.py
--rw-r--r--   0        0        0     1089 2023-06-13 15:04:25.224584 scrapy_db-0.0.1/scrapy_db/utils.py
--rw-r--r--   0        0        0     2632 1970-01-01 00:00:00.000000 scrapy_db-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-07 10:34:22.421846 scrapy_db-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1547 2023-06-24 10:48:36.684160 scrapy_db-0.0.2/README.md
+-rw-r--r--   0        0        0     1216 2023-06-24 11:35:28.967379 scrapy_db-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-06-24 11:35:44.984063 scrapy_db-0.0.2/scrapy_db/__init__.py
+-rw-r--r--   0        0        0     5350 2023-06-14 03:38:46.820214 scrapy_db-0.0.2/scrapy_db/db.py
+-rw-r--r--   0        0        0      475 2023-06-13 15:04:25.223531 scrapy_db-0.0.2/scrapy_db/defaults.py
+-rw-r--r--   0        0        0     3256 2023-06-15 02:02:42.898109 scrapy_db-0.0.2/scrapy_db/dupefilter.py
+-rw-r--r--   0        0        0     2473 2023-06-14 03:15:23.908321 scrapy_db-0.0.2/scrapy_db/queue.py
+-rw-r--r--   0        0        0     4381 2023-06-13 15:04:25.224164 scrapy_db-0.0.2/scrapy_db/scheduler.py
+-rw-r--r--   0        0        0     4705 2023-06-13 15:04:25.224356 scrapy_db-0.0.2/scrapy_db/spiders.py
+-rw-r--r--   0        0        0     1089 2023-06-13 15:04:25.224584 scrapy_db-0.0.2/scrapy_db/utils.py
+-rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 scrapy_db-0.0.2/PKG-INFO
```

### Comparing `scrapy_db-0.0.1/LICENSE` & `scrapy_db-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.1/README.md` & `scrapy_db-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.1/pyproject.toml` & `scrapy_db-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapy-db"
-version = "0.0.1"
+version = "0.0.2"
 description = "Similar to [scrapy-redis](https://github.com/rmax/scrapy-redis), using the database as a queue, database-based scrapy components."
 authors = ["libra146 <shumeipai146@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "scrapy_db" }]
 license = "GPL-3.0-only"
 homepage = "https://github.com/libra146/scrapy-db/blob/main/README.md"
 repository = "https://github.com/libra146/scrapy-db"
@@ -16,15 +16,15 @@
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-scrapy = "2.7.0"
+scrapy = "^2.7.0"
 peewee = "^3.16.0"
 pymysql = "^1.0.3"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.2"
 pytest-mock = "^3.10.0"
 codecov = "^2.1.13"
```

### Comparing `scrapy_db-0.0.1/scrapy_db/db.py` & `scrapy_db-0.0.2/scrapy_db/db.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.1/scrapy_db/dupefilter.py` & `scrapy_db-0.0.2/scrapy_db/dupefilter.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.1/scrapy_db/queue.py` & `scrapy_db-0.0.2/scrapy_db/queue.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.1/scrapy_db/scheduler.py` & `scrapy_db-0.0.2/scrapy_db/scheduler.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.1/scrapy_db/spiders.py` & `scrapy_db-0.0.2/scrapy_db/spiders.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.1/scrapy_db/utils.py` & `scrapy_db-0.0.2/scrapy_db/utils.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.1/PKG-INFO` & `scrapy_db-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-db
-Version: 0.0.1
+Version: 0.0.2
 Summary: Similar to [scrapy-redis](https://github.com/rmax/scrapy-redis), using the database as a queue, database-based scrapy components.
 Home-page: https://github.com/libra146/scrapy-db/blob/main/README.md
 License: GPL-3.0-only
 Author: libra146
 Author-email: shumeipai146@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: peewee (>=3.16.0,<4.0.0)
 Requires-Dist: pymysql (>=1.0.3,<2.0.0)
-Requires-Dist: scrapy (==2.7.0)
+Requires-Dist: scrapy (>=2.7.0,<3.0.0)
 Project-URL: Documentation, https://github.com/libra146/scrapy-db/blob/main/README.md
 Project-URL: Repository, https://github.com/libra146/scrapy-db
 Description-Content-Type: text/markdown
 
 # scrapy-db
 
 [![codecov](https://codecov.io/github/libra146/scrapy-db/branch/main/graph/badge.svg?token=O9L0DVI0BR)](https://codecov.io/github/libra146/scrapy-db) [![build](https://github.com/libra146/scrapy-db/actions/workflows/codecov.yaml/badge.svg?branch=main)](https://github.com/libra146/scrapy-db/actions/workflows/codecov.yaml)
```

