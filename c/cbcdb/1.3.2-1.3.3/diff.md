# Comparing `tmp/cbcdb-1.3.2.tar.gz` & `tmp/cbcdb-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cbcdb-1.3.2.tar", last modified: Thu Jun 22 19:48:53 2023, max compression
+gzip compressed data, was "dist/cbcdb-1.3.3.tar", last modified: Sat Jun 24 00:28:02 2023, max compression
```

## Comparing `cbcdb-1.3.2.tar` & `cbcdb-1.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:48:53.000000 cbcdb-1.3.2/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     1857 2022-04-14 18:33:01.000000 cbcdb-1.3.2/.gitignore
--rw-r--r--   0 craiglathrop   (501) staff       (20)     1090 2022-02-11 18:43:22.000000 cbcdb-1.3.2/LICENSE
--rw-r--r--   0 craiglathrop   (501) staff       (20)      885 2023-06-22 19:48:53.000000 cbcdb-1.3.2/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      723 2023-06-22 19:33:07.000000 cbcdb-1.3.2/README.md
--rwxrwx---   0 craiglathrop   (501) staff       (20)       64 2021-06-28 01:32:34.000000 cbcdb-1.3.2/build-deploy.sh
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:48:53.000000 cbcdb-1.3.2/cbcdb/
--rw-r--r--   0 craiglathrop   (501) staff       (20)       32 2022-04-14 18:33:01.000000 cbcdb-1.3.2/cbcdb/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    24175 2023-06-22 19:48:49.000000 cbcdb-1.3.2/cbcdb/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)      143 2021-06-11 22:18:24.000000 cbcdb-1.3.2/cbcdb/test.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:48:53.000000 cbcdb-1.3.2/cbcdb.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      885 2023-06-22 19:48:52.000000 cbcdb-1.3.2/cbcdb.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      408 2023-06-22 19:48:52.000000 cbcdb-1.3.2/cbcdb.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2023-06-22 19:48:52.000000 cbcdb-1.3.2/cbcdb.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2021-03-10 01:30:10.000000 cbcdb-1.3.2/cbcdb.egg-info/not-zip-safe
--rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2023-06-22 19:48:52.000000 cbcdb-1.3.2/cbcdb.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2023-06-22 19:48:52.000000 cbcdb-1.3.2/cbcdb.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)      103 2021-03-10 01:30:59.000000 cbcdb-1.3.2/pyproject.toml
--rw-r--r--   0 craiglathrop   (501) staff       (20)      160 2023-06-22 19:27:40.000000 cbcdb-1.3.2/requirements.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)      993 2023-06-22 19:48:53.000000 cbcdb-1.3.2/setup.cfg
--rw-r--r--   0 craiglathrop   (501) staff       (20)       80 2021-03-16 00:52:46.000000 cbcdb-1.3.2/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-22 19:48:53.000000 cbcdb-1.3.2/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2021-03-04 23:20:27.000000 cbcdb-1.3.2/tests/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)      400 2021-04-16 03:37:29.000000 cbcdb-1.3.2/tests/docker-compose.yml
--rw-r--r--   0 craiglathrop   (501) staff       (20)     1813 2021-06-24 23:04:32.000000 cbcdb-1.3.2/tests/docker_test_setup.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    14888 2022-08-24 01:14:33.000000 cbcdb-1.3.2/tests/test_db_manager.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-24 00:28:02.000000 cbcdb-1.3.3/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     1857 2022-04-14 18:33:01.000000 cbcdb-1.3.3/.gitignore
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     1090 2022-02-11 18:43:22.000000 cbcdb-1.3.3/LICENSE
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      885 2023-06-24 00:28:02.000000 cbcdb-1.3.3/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      723 2023-06-22 19:33:07.000000 cbcdb-1.3.3/README.md
+-rwxrwx---   0 craiglathrop   (501) staff       (20)       64 2021-06-28 01:32:34.000000 cbcdb-1.3.3/build-deploy.sh
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-24 00:28:02.000000 cbcdb-1.3.3/cbcdb/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       32 2022-04-14 18:33:01.000000 cbcdb-1.3.3/cbcdb/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    24183 2023-06-24 00:27:50.000000 cbcdb-1.3.3/cbcdb/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      143 2021-06-11 22:18:24.000000 cbcdb-1.3.3/cbcdb/test.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-24 00:28:02.000000 cbcdb-1.3.3/cbcdb.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      885 2023-06-24 00:28:01.000000 cbcdb-1.3.3/cbcdb.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      408 2023-06-24 00:28:01.000000 cbcdb-1.3.3/cbcdb.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2023-06-24 00:28:01.000000 cbcdb-1.3.3/cbcdb.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2021-03-10 01:30:10.000000 cbcdb-1.3.3/cbcdb.egg-info/not-zip-safe
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2023-06-24 00:28:01.000000 cbcdb-1.3.3/cbcdb.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2023-06-24 00:28:01.000000 cbcdb-1.3.3/cbcdb.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      103 2021-03-10 01:30:59.000000 cbcdb-1.3.3/pyproject.toml
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      160 2023-06-22 19:27:40.000000 cbcdb-1.3.3/requirements.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      993 2023-06-24 00:28:02.000000 cbcdb-1.3.3/setup.cfg
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       80 2021-03-16 00:52:46.000000 cbcdb-1.3.3/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2023-06-24 00:28:02.000000 cbcdb-1.3.3/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2021-03-04 23:20:27.000000 cbcdb-1.3.3/tests/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      400 2021-04-16 03:37:29.000000 cbcdb-1.3.3/tests/docker-compose.yml
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     1813 2021-06-24 23:04:32.000000 cbcdb-1.3.3/tests/docker_test_setup.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    14888 2022-08-24 01:14:33.000000 cbcdb-1.3.3/tests/test_db_manager.py
```

### Comparing `cbcdb-1.3.2/.gitignore` & `cbcdb-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cbcdb-1.3.2/LICENSE` & `cbcdb-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cbcdb-1.3.2/PKG-INFO` & `cbcdb-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcdb
-Version: 1.3.2
+Version: 1.3.3
 Summary: A package to help facilitate postgres and Redshift database communication over SSH.
 Home-page: https://github.com/Cold-Bore-Capital/cbc-dbmanager
 Author: Cold Bore Capital
 Author-email: it-group@coldborecapital.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `cbcdb-1.3.2/README.md` & `cbcdb-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cbcdb-1.3.2/cbcdb/main.py` & `cbcdb-1.3.3/cbcdb/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import random
 import socket
 import time
 from datetime import datetime, date
 from typing import List, Any, Dict, Tuple
 
 from configservice.config import Config
-from numpy import inf
 from psycopg2 import connect
 from psycopg2.extras import execute_values
 
 
 class DBManager:
     """
     DBManager handled the read and write information to the DB.
@@ -534,14 +533,15 @@
 
         Args:
             params: A list of parameters
 
         Returns: A list of parameters with pd.nan's converted to None
         """
         import pandas as pd
+        from numpy import inf
         row_counter = 0
         for row in params:
             value_counter = 0
             if isinstance(row, list):
                 for v in row:
                     # A note on inf. inf, or np.inf shows up sometimes. It can be positive or negative (oddly).
                     # It's important to remove this or SQL Server will throw an error about floating point precision.
```

### Comparing `cbcdb-1.3.2/cbcdb.egg-info/PKG-INFO` & `cbcdb-1.3.3/cbcdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcdb
-Version: 1.3.2
+Version: 1.3.3
 Summary: A package to help facilitate postgres and Redshift database communication over SSH.
 Home-page: https://github.com/Cold-Bore-Capital/cbc-dbmanager
 Author: Cold Bore Capital
 Author-email: it-group@coldborecapital.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `cbcdb-1.3.2/setup.cfg` & `cbcdb-1.3.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cbcdb
-version = 1.3.2
+version = 1.3.3
 author = Cold Bore Capital
 author_email = it-group@coldborecapital.com
 home_page = https://github.com/Cold-Bore-Capital/cbc-dbmanager
 description = A package to help facilitate postgres and Redshift database communication over SSH.
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3
```

### Comparing `cbcdb-1.3.2/tests/docker_test_setup.py` & `cbcdb-1.3.3/tests/docker_test_setup.py`

 * *Files identical despite different names*

### Comparing `cbcdb-1.3.2/tests/test_db_manager.py` & `cbcdb-1.3.3/tests/test_db_manager.py`

 * *Files identical despite different names*

