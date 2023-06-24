# Comparing `tmp/sqlite3_to_mysql-2.0.1.tar.gz` & `tmp/sqlite3_to_mysql-2.0.2.tar.gz`

## Comparing `sqlite3_to_mysql-2.0.1.tar` & `sqlite3_to_mysql-2.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/requirements_dev.txt
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/__init__.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/cli.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/click_utils.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/debug_info.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/mysql_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/py.typed
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/sqlite_utils.py
--rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/transporter.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/__init__.py
--rw-r--r--   0        0        0    11192 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/database.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/factories.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/func/__init__.py
--rw-r--r--   0        0        0    24132 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/func/sqlite3_to_mysql_test.py
--rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/func/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/unit/__init__.py
--rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/tests/unit/sqlite3_to_mysql_test.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/LICENSE
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/README.md
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/requirements_dev.txt
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/__init__.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/cli.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/click_utils.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/debug_info.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/mysql_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/py.typed
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/sqlite_utils.py
+-rw-r--r--   0        0        0    30707 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/transporter.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/__init__.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/database.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/factories.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/func/__init__.py
+-rw-r--r--   0        0        0    24175 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/func/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/func/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/tests/unit/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/LICENSE
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/README.md
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.0.2/PKG-INFO
```

### Comparing `sqlite3_to_mysql-2.0.1/CODE-OF-CONDUCT.md` & `sqlite3_to_mysql-2.0.2/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/cli.py` & `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/cli.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/click_utils.py` & `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/click_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/debug_info.py` & `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/debug_info.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/mysql_utils.py` & `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/mysql_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/sqlite_utils.py` & `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/transporter.py` & `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/transporter.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/sqlite3_to_mysql/types.py` & `sqlite3_to_mysql-2.0.2/sqlite3_to_mysql/types.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/tests/conftest.py` & `sqlite3_to_mysql-2.0.2/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,16 @@
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
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm import Session
 from sqlalchemy_utils import database_exists, drop_database
```

### Comparing `sqlite3_to_mysql-2.0.1/tests/database.py` & `sqlite3_to_mysql-2.0.2/tests/database.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/tests/factories.py` & `sqlite3_to_mysql-2.0.2/tests/factories.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/tests/models.py` & `sqlite3_to_mysql-2.0.2/tests/models.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/tests/func/sqlite3_to_mysql_test.py` & `sqlite3_to_mysql-2.0.2/tests/func/sqlite3_to_mysql_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import mysql.connector
 import pytest
 import simplejson as json
 from _pytest._py.path import LocalPath
 from _pytest.capture import CaptureFixture
 from _pytest.logging import LogCaptureFixture
 from faker import Faker
-from mysql.connector import CMySQLConnection, MySQLConnection, errorcode
+from mysql.connector import MySQLConnection, errorcode
+from mysql.connector.connection_cext import CMySQLConnection
 from mysql.connector.pooling import PooledMySQLConnection
 from pytest_mock import MockFixture
 from sqlalchemy import MetaData, Table, create_engine, inspect, select, text
 from sqlalchemy.engine import Connection, CursorResult, Engine, Inspector, Row
 from sqlalchemy.engine.interfaces import ReflectedIndex
 from sqlalchemy.sql import Select
 from sqlalchemy.sql.elements import TextClause
```

### Comparing `sqlite3_to_mysql-2.0.1/tests/func/test_cli.py` & `sqlite3_to_mysql-2.0.2/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/tests/unit/sqlite3_to_mysql_test.py` & `sqlite3_to_mysql-2.0.2/tests/unit/sqlite3_to_mysql_test.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/.gitignore` & `sqlite3_to_mysql-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/LICENSE` & `sqlite3_to_mysql-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/README.md` & `sqlite3_to_mysql-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.0.1/pyproject.toml` & `sqlite3_to_mysql-2.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 path = "sqlite3_to_mysql/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "sqlite3_to_mysql",
     "tests",
     "README.md",
+    "CHANGELOG.md",
     "CODE-OF-CONDUCT.md",
     "LICENSE",
     "requirements_dev.txt",
 ]
 
 [project.scripts]
 sqlite3mysql = "sqlite3_to_mysql.cli:cli"
```

### Comparing `sqlite3_to_mysql-2.0.1/PKG-INFO` & `sqlite3_to_mysql-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite3-to-mysql
-Version: 2.0.1
+Version: 2.0.2
 Summary: A simple Python tool to transfer data from SQLite 3 to MySQL
 Project-URL: Source, https://github.com/techouse/sqlite3-to-mysql
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: data,migrate,migration,mysql,sqlite3,transfer
 Classifier: Development Status :: 5 - Production/Stable
```

