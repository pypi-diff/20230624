# Comparing `tmp/mysql_to_sqlite3-2.0.1.tar.gz` & `tmp/mysql_to_sqlite3-2.0.2.tar.gz`

## Comparing `mysql_to_sqlite3-2.0.1.tar` & `mysql_to_sqlite3-2.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/requirements_dev.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/__init__.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/cli.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/click_utils.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/debug_info.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/mysql_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/py.typed
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/sqlite_utils.py
--rw-r--r--   0        0        0    28099 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/transporter.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/__init__.py
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/database.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/factories.py
--rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/func/__init__.py
--rw-r--r--   0        0        0    47466 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/func/mysql_to_sqlite3_test.py
--rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/func/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/unit/__init__.py
--rw-r--r--   0        0        0    25443 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/unit/mysql_to_sqlite3_test.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/LICENSE
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/README.md
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5870 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/requirements_dev.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/__init__.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/cli.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/click_utils.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/debug_info.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/mysql_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/py.typed
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/sqlite_utils.py
+-rw-r--r--   0        0        0    28142 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/transporter.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/__init__.py
+-rw-r--r--   0        0        0    10855 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/database.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/factories.py
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/func/__init__.py
+-rw-r--r--   0        0        0    47509 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/func/mysql_to_sqlite3_test.py
+-rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/func/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0    25443 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/unit/mysql_to_sqlite3_test.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/LICENSE
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/README.md
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/PKG-INFO
```

### Comparing `mysql_to_sqlite3-2.0.1/CODE-OF-CONDUCT.md` & `mysql_to_sqlite3-2.0.2/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/cli.py` & `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/cli.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/click_utils.py` & `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/click_utils.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/debug_info.py` & `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/debug_info.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/sqlite_utils.py` & `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/transporter.py` & `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/transporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from decimal import Decimal
 from math import ceil
 from os.path import realpath
 from sys import stdout
 
 import mysql.connector
 import typing_extensions as tx
-from mysql.connector import CMySQLConnection, MySQLConnection, errorcode
+from mysql.connector import MySQLConnection, errorcode
+from mysql.connector.connection_cext import CMySQLConnection
 from mysql.connector.types import ToPythonOutputTypes
 from tqdm import tqdm, trange
 
 from mysql_to_sqlite3.mysql_utils import CHARSET_INTRODUCERS
 from mysql_to_sqlite3.sqlite_utils import (
     CollatingSequences,
     adapt_decimal,
```

### Comparing `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/types.py` & `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Types for mysql-to-sqlite3."""
 import os
 import typing as t
 from logging import Logger
 from sqlite3 import Connection, Cursor
 
 import typing_extensions as tx
-from mysql.connector import CMySQLConnection, MySQLConnection
+from mysql.connector import MySQLConnection
+from mysql.connector.connection_cext import CMySQLConnection
 from mysql.connector.cursor import MySQLCursorDict, MySQLCursorPrepared, MySQLCursorRaw
 
 
 class MySQLtoSQLiteParams(tx.TypedDict):
     """MySQLtoSQLite parameters."""
 
     buffered: t.Optional[bool]
```

### Comparing `mysql_to_sqlite3-2.0.1/tests/conftest.py` & `mysql_to_sqlite3-2.0.2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from _pytest.config.argparsing import Parser
 from _pytest.legacypath import TempdirFactory
 from click.testing import CliRunner
 from docker import DockerClient
 from docker.errors import NotFound
 from docker.models.containers import Container
 from faker import Faker
-from mysql.connector import CMySQLConnection, MySQLConnection, errorcode
+from mysql.connector import MySQLConnection, errorcode
+from mysql.connector.connection_cext import CMySQLConnection
 from mysql.connector.pooling import PooledMySQLConnection
 from requests import HTTPError
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm import Session
 from sqlalchemy_utils import database_exists, drop_database
 
 from . import database, factories, models
```

### Comparing `mysql_to_sqlite3-2.0.1/tests/database.py` & `mysql_to_sqlite3-2.0.2/tests/database.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/tests/factories.py` & `mysql_to_sqlite3-2.0.2/tests/factories.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/tests/models.py` & `mysql_to_sqlite3-2.0.2/tests/models.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/tests/func/mysql_to_sqlite3_test.py` & `mysql_to_sqlite3-2.0.2/tests/func/mysql_to_sqlite3_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 import mysql.connector
 import pytest
 import simplejson as json
 from _pytest._py.path import LocalPath
 from _pytest.logging import LogCaptureFixture
 from faker import Faker
-from mysql.connector import CMySQLConnection, MySQLConnection, errorcode
+from mysql.connector import MySQLConnection, errorcode
+from mysql.connector.connection_cext import CMySQLConnection
 from mysql.connector.cursor import MySQLCursor
 from mysql.connector.pooling import PooledMySQLConnection
 from pytest_mock import MockFixture
 from sqlalchemy import (
     Connection,
     CursorResult,
     Engine,
```

### Comparing `mysql_to_sqlite3-2.0.1/tests/func/test_cli.py` & `mysql_to_sqlite3-2.0.2/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/tests/unit/mysql_to_sqlite3_test.py` & `mysql_to_sqlite3-2.0.2/tests/unit/mysql_to_sqlite3_test.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/.gitignore` & `mysql_to_sqlite3-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/LICENSE` & `mysql_to_sqlite3-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/README.md` & `mysql_to_sqlite3-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.1/pyproject.toml` & `mysql_to_sqlite3-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Database",
 ]
 dependencies = [
     "Click>=8.1.3",
-    "mysql-connector-python>=8.0.18,!=8.0.30,!=8.0.31",
+    "mysql-connector-python>=8.0.33",
     "pytimeparse2",
     "python-slugify>=7.0.0",
     "simplejson>=3.19.0",
     "tqdm>=4.65.0",
     "tabulate",
     "typing_extensions",
 ]
@@ -54,14 +54,15 @@
 path = "mysql_to_sqlite3/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "mysql_to_sqlite3",
     "tests",
     "README.md",
+    "CHANGELOG.md",
     "CODE-OF-CONDUCT.md",
     "LICENSE",
     "requirements_dev.txt",
 ]
 
 [project.scripts]
 mysql2sqlite = "mysql_to_sqlite3.cli:cli"
```

### Comparing `mysql_to_sqlite3-2.0.1/PKG-INFO` & `mysql_to_sqlite3-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-to-sqlite3
-Version: 2.0.1
+Version: 2.0.2
 Summary: A simple Python tool to transfer data from MySQL to SQLite 3
 Project-URL: Source, https://github.com/techouse/mysql-to-sqlite3
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: data,migrate,migration,mysql,sqlite3,transfer
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Requires-Python: >=3.7
 Requires-Dist: click>=8.1.3
-Requires-Dist: mysql-connector-python!=8.0.30,!=8.0.31,>=8.0.18
+Requires-Dist: mysql-connector-python>=8.0.33
 Requires-Dist: python-slugify>=7.0.0
 Requires-Dist: pytimeparse2
 Requires-Dist: simplejson>=3.19.0
 Requires-Dist: tabulate
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
```

