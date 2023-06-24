# Comparing `tmp/mysql_to_sqlite3-2.0.2.tar.gz` & `tmp/mysql_to_sqlite3-2.0.3.tar.gz`

## Comparing `mysql_to_sqlite3-2.0.2.tar` & `mysql_to_sqlite3-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     5870 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/requirements_dev.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/__init__.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/cli.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/click_utils.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/debug_info.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/mysql_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/py.typed
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/sqlite_utils.py
--rw-r--r--   0        0        0    28142 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/transporter.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/__init__.py
--rw-r--r--   0        0        0    10855 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/conftest.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/database.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/factories.py
--rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/func/__init__.py
--rw-r--r--   0        0        0    47509 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/func/mysql_to_sqlite3_test.py
--rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/func/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/unit/__init__.py
--rw-r--r--   0        0        0    25443 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/tests/unit/mysql_to_sqlite3_test.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/LICENSE
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/README.md
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/requirements_dev.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/__init__.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/cli.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/click_utils.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/debug_info.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/mysql_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/py.typed
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/sqlite_utils.py
+-rw-r--r--   0        0        0    28114 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/transporter.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/tests/__init__.py
+-rw-r--r--   0        0        0    10855 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/tests/database.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/tests/factories.py
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/tests/func/__init__.py
+-rw-r--r--   0        0        0    47509 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/tests/func/mysql_to_sqlite3_test.py
+-rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/tests/func/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0    25443 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/tests/unit/mysql_to_sqlite3_test.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/LICENSE
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/README.md
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.3/PKG-INFO
```

### Comparing `mysql_to_sqlite3-2.0.2/CHANGELOG.md` & `mysql_to_sqlite3-2.0.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 2.0.3
+
+* [FIX] import MySQLConnectionAbstract instead of concrete implementations
+
 # 2.0.2
 
 * [FIX] properly import CMySQLConnection
 
 # 2.0.1
 
 * [FEAT] add support for MySQL character set introducers in DEFAULT clause
```

### Comparing `mysql_to_sqlite3-2.0.2/CODE-OF-CONDUCT.md` & `mysql_to_sqlite3-2.0.3/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/cli.py` & `mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/cli.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/click_utils.py` & `mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/click_utils.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/debug_info.py` & `mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/debug_info.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/sqlite_utils.py` & `mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/transporter.py` & `mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/transporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from decimal import Decimal
 from math import ceil
 from os.path import realpath
 from sys import stdout
 
 import mysql.connector
 import typing_extensions as tx
-from mysql.connector import MySQLConnection, errorcode
-from mysql.connector.connection_cext import CMySQLConnection
+from mysql.connector import errorcode
+from mysql.connector.abstracts import MySQLConnectionAbstract
 from mysql.connector.types import ToPythonOutputTypes
 from tqdm import tqdm, trange
 
 from mysql_to_sqlite3.mysql_utils import CHARSET_INTRODUCERS
 from mysql_to_sqlite3.sqlite_utils import (
     CollatingSequences,
     adapt_decimal,
@@ -120,15 +120,15 @@
             _mysql_connection = mysql.connector.connect(
                 user=self._mysql_user,
                 password=self._mysql_password,
                 host=self._mysql_host,
                 port=self._mysql_port,
                 ssl_disabled=self._mysql_ssl_disabled,
             )
-            if isinstance(_mysql_connection, (MySQLConnection, CMySQLConnection)):
+            if isinstance(_mysql_connection, MySQLConnectionAbstract):
                 self._mysql = _mysql_connection
             else:
                 raise ConnectionError("Unable to connect to MySQL")
             if not self._mysql.is_connected():
                 raise ConnectionError("Unable to connect to MySQL")
 
             self._mysql_cur = self._mysql.cursor(buffered=self._buffered, raw=True)  # type: ignore[assignment]
```

### Comparing `mysql_to_sqlite3-2.0.2/mysql_to_sqlite3/types.py` & `mysql_to_sqlite3-2.0.3/mysql_to_sqlite3/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Types for mysql-to-sqlite3."""
 import os
 import typing as t
 from logging import Logger
 from sqlite3 import Connection, Cursor
 
 import typing_extensions as tx
-from mysql.connector import MySQLConnection
-from mysql.connector.connection_cext import CMySQLConnection
+from mysql.connector.abstracts import MySQLConnectionAbstract
 from mysql.connector.cursor import MySQLCursorDict, MySQLCursorPrepared, MySQLCursorRaw
 
 
 class MySQLtoSQLiteParams(tx.TypedDict):
     """MySQLtoSQLite parameters."""
 
     buffered: t.Optional[bool]
@@ -42,15 +41,15 @@
     _chunk_size: t.Optional[int]
     _collation: str
     _current_chunk_number: int
     _exclude_mysql_tables: t.Sequence[str]
     _json_as_text: bool
     _limit_rows: int
     _logger: Logger
-    _mysql: t.Union[MySQLConnection, CMySQLConnection]
+    _mysql: MySQLConnectionAbstract
     _mysql_cur: MySQLCursorRaw
     _mysql_cur_dict: MySQLCursorDict
     _mysql_cur_prepared: MySQLCursorPrepared
     _mysql_database: str
     _mysql_host: str
     _mysql_password: t.Optional[str]
     _mysql_port: int
```

### Comparing `mysql_to_sqlite3-2.0.2/tests/conftest.py` & `mysql_to_sqlite3-2.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/tests/database.py` & `mysql_to_sqlite3-2.0.3/tests/database.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/tests/factories.py` & `mysql_to_sqlite3-2.0.3/tests/factories.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/tests/models.py` & `mysql_to_sqlite3-2.0.3/tests/models.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/tests/func/mysql_to_sqlite3_test.py` & `mysql_to_sqlite3-2.0.3/tests/func/mysql_to_sqlite3_test.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/tests/func/test_cli.py` & `mysql_to_sqlite3-2.0.3/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/tests/unit/mysql_to_sqlite3_test.py` & `mysql_to_sqlite3-2.0.3/tests/unit/mysql_to_sqlite3_test.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/.gitignore` & `mysql_to_sqlite3-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/LICENSE` & `mysql_to_sqlite3-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/README.md` & `mysql_to_sqlite3-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/pyproject.toml` & `mysql_to_sqlite3-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.2/PKG-INFO` & `mysql_to_sqlite3-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-to-sqlite3
-Version: 2.0.2
+Version: 2.0.3
 Summary: A simple Python tool to transfer data from MySQL to SQLite 3
 Project-URL: Source, https://github.com/techouse/mysql-to-sqlite3
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: data,migrate,migration,mysql,sqlite3,transfer
 Classifier: Development Status :: 5 - Production/Stable
```

