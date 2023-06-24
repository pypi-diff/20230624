# Comparing `tmp/fakesnow-0.1.0.tar.gz` & `tmp/fakesnow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakesnow-0.1.0.tar", last modified: Wed Jun 21 02:35:59 2023, max compression
+gzip compressed data, was "fakesnow-0.2.0.tar", last modified: Sat Jun 24 05:20:28 2023, max compression
```

## Comparing `fakesnow-0.1.0.tar` & `fakesnow-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:35:59.426805 fakesnow-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-21 02:35:51.000000 fakesnow-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 02:35:51.000000 fakesnow-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-21 02:35:59.422805 fakesnow-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-21 02:35:51.000000 fakesnow-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:35:59.422805 fakesnow-0.1.0/fakesnow/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19240 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-06-21 02:35:51.000000 fakesnow-0.1.0/fakesnow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:35:59.422805 fakesnow-0.1.0/fakesnow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-21 02:35:59.000000 fakesnow-0.1.0/fakesnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-21 02:35:59.000000 fakesnow-0.1.0/fakesnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 02:35:59.000000 fakesnow-0.1.0/fakesnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 02:35:59.000000 fakesnow-0.1.0/fakesnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 02:35:59.000000 fakesnow-0.1.0/fakesnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-21 02:35:51.000000 fakesnow-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 02:35:59.426805 fakesnow-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 02:35:51.000000 fakesnow-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:35:59.422805 fakesnow-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-21 02:35:51.000000 fakesnow-0.1.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-21 02:35:51.000000 fakesnow-0.1.0/tests/test_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    22920 2023-06-21 02:35:51.000000 fakesnow-0.1.0/tests/test_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-21 02:35:51.000000 fakesnow-0.1.0/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-21 02:35:51.000000 fakesnow-0.1.0/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:20:28.764951 fakesnow-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-24 05:20:18.000000 fakesnow-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-24 05:20:18.000000 fakesnow-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-24 05:20:28.764951 fakesnow-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-24 05:20:18.000000 fakesnow-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:20:28.764951 fakesnow-0.2.0/fakesnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19502 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:20:28.764951 fakesnow-0.2.0/fakesnow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-24 05:20:28.000000 fakesnow-0.2.0/fakesnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-24 05:20:28.000000 fakesnow-0.2.0/fakesnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 05:20:28.000000 fakesnow-0.2.0/fakesnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-24 05:20:28.000000 fakesnow-0.2.0/fakesnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 05:20:28.000000 fakesnow-0.2.0/fakesnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-24 05:20:18.000000 fakesnow-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 05:20:28.764951 fakesnow-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 05:20:18.000000 fakesnow-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:20:28.764951 fakesnow-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-24 05:20:18.000000 fakesnow-0.2.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-24 05:20:18.000000 fakesnow-0.2.0/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25787 2023-06-24 05:20:18.000000 fakesnow-0.2.0/tests/test_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-24 05:20:18.000000 fakesnow-0.2.0/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-24 05:20:18.000000 fakesnow-0.2.0/tests/test_transforms.py
```

### Comparing `fakesnow-0.1.0/LICENSE` & `fakesnow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fakesnow-0.1.0/PKG-INFO` & `fakesnow-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.1.0
+Version: 0.2.0
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `fakesnow-0.1.0/README.md` & `fakesnow-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fakesnow-0.1.0/fakesnow/__init__.py` & `fakesnow-0.2.0/fakesnow/__init__.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.1.0/fakesnow/checks.py` & `fakesnow-0.2.0/fakesnow/checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.1.0/fakesnow/expr.py` & `fakesnow-0.2.0/fakesnow/expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.1.0/fakesnow/fakes.py` & `fakesnow-0.2.0/fakesnow/fakes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import re
 from string import Template
 from types import TracebackType
-from typing import Any, Iterable, Iterator, Literal, Optional, Sequence, Type, Union, cast
+from typing import TYPE_CHECKING, Any, Iterable, Iterator, Literal, Optional, Sequence, Type, Union, cast
 
 import duckdb
-import pandas as pd
+
+if TYPE_CHECKING:
+    import pandas as pd
+    import pyarrow.lib
 import pyarrow
-import pyarrow.lib
-import pyarrow.types
 import snowflake.connector.errors
 import sqlglot
 from duckdb import DuckDBPyConnection
 from snowflake.connector.cursor import DictCursor, ResultMetadata, SnowflakeCursor
 from snowflake.connector.result_batch import ResultBatch
 from sqlglot import exp, parse_one
 from typing_extensions import Self
@@ -53,14 +54,15 @@
             use_dict_result (bool, optional): If true rows are returned as dicts otherwise they
                 are returned as tuples. Defaults to False.
         """
         self._conn = conn
         self._duck_conn = duck_conn
         self._use_dict_result = use_dict_result
         self._last_sql = None
+        self._last_params = None
 
     def __enter__(self) -> Self:
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]] = ...,
@@ -87,15 +89,15 @@
         # use a cursor to avoid destroying an unfetched result on the main connection
         with self._duck_conn.cursor() as cur:
             assert self._conn.database, "Not implemented when database is None"
             assert self._conn.schema, "Not implemented when database is None"
 
             # match database and schema used on the main connection
             cur.execute(f"SET SCHEMA = '{self._conn.database}.{self._conn.schema}'")
-            cur.execute(f"DESCRIBE {self._last_sql}")
+            cur.execute(f"DESCRIBE {self._last_sql}", self._last_params)
             meta = FakeSnowflakeCursor._describe_as_result_metadata(cur.fetchall())  # noqa: SLF001
 
         return meta  # type: ignore see https://github.com/duckdb/duckdb/issues/7816
 
     def execute(
         self,
         command: str | exp.Expression,
@@ -146,14 +148,15 @@
         )
 
         sql = transformed.sql(dialect="duckdb")
 
         if cmd != "COMMENT TABLE":
             try:
                 self._last_sql = sql
+                self._last_params = params
                 self._duck_conn.execute(sql, params)
             except duckdb.BinderException as e:
                 msg = e.args[0]
                 raise snowflake.connector.errors.ProgrammingError(msg=msg, errno=2043, sqlstate="02000") from None
             except duckdb.CatalogException as e:
                 # minimal processing to make it look like a snowflake exception, message content may differ
                 msg = cast(str, e.args[0]).split("\n")[0]
@@ -389,14 +392,17 @@
         self,
         exc_type: Optional[Type[BaseException]] = ...,
         exc_value: Optional[BaseException] = ...,
         traceback: Optional[TracebackType] = ...,
     ) -> bool:
         return False
 
+    def commit(self) -> None:
+        self.cursor().execute("COMMIT")
+
     def cursor(self, cursor_class: Type[SnowflakeCursor] = SnowflakeCursor) -> FakeSnowflakeCursor:
         return FakeSnowflakeCursor(conn=self, duck_conn=self._duck_conn, use_dict_result=cursor_class == DictCursor)
 
     def execute_string(
         self,
         sql_text: str,
         remove_comments: bool = False,
@@ -407,14 +413,17 @@
         cursors = [
             self.cursor(cursor_class).execute(e.sql(dialect="snowflake"))
             for e in sqlglot.parse(sql_text, read="snowflake")
             if e
         ]
         return cursors if return_cursors else []
 
+    def rollback(self) -> None:
+        self.cursor().execute("ROLLBACK")
+
     def _insert_df(
         self, df: pd.DataFrame, table_name: str, database: str | None = None, schema: str | None = None
     ) -> int:
         # dicts in dataframes are written as parquet structs, and snowflake loads parquet structs as json strings
         # whereas duckdb loads them as a struct, so we convert them to json here
         cols = [f"TO_JSON({c})" if isinstance(df[c][0], dict) else c for c in df.columns]
         cols = ",".join(cols)
```

### Comparing `fakesnow-0.1.0/fakesnow/transforms.py` & `fakesnow-0.2.0/fakesnow/transforms.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.1.0/fakesnow.egg-info/PKG-INFO` & `fakesnow-0.2.0/fakesnow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.1.0
+Version: 0.2.0
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `fakesnow-0.1.0/pyproject.toml` & `fakesnow-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [project]
 name = "fakesnow"
 description = "Fake Snowflake Connector for Python. Run Snowflake DB locally."
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 keywords = ["snowflake", "snowflakedb", "fake", "local", "mock", "testing"]
 requires-python = ">=3.9"
 dependencies = [
     "duckdb~=0.8.0",
-    # include the pandas extra to get compatible version of pyarrow
-    "snowflake-connector-python[pandas]",
-    "sqlglot~=15.0.0",
+    "pyarrow",
+    "snowflake-connector-python",
+    "sqlglot~=16.4.2",
 ]
 
 [project.urls]
 homepage = "https://github.com/tekumara/fakesnow"
 
 [project.optional-dependencies]
 dev = [
     "black~=23.3",
     "build~=0.10",
-    # include the secure-local-storage extra for token caching
-    "snowflake-connector-python[secure-local-storage]",
+    # include compatible version of pandas, and secure-local-storage for token caching
+    "snowflake-connector-python[pandas, secure-local-storage]",
     "pre-commit~=3.2",
     "pytest~=7.3",
     "ruff~=0.0.263",
     "twine~=4.0",
 ]
 # for debugging, see https://duckdb.org/docs/guides/python/jupyter.html
 notebook = ["duckdb-engine", "ipykernel", "jupysql", "snowflake-sqlalchemy"]
```

### Comparing `fakesnow-0.1.0/tests/test_checks.py` & `fakesnow-0.2.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.1.0/tests/test_expr.py` & `fakesnow-0.2.0/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.1.0/tests/test_fakes.py` & `fakesnow-0.2.0/tests/test_fakes.py`

 * *Files 8% similar despite different names*

```diff
@@ -214,14 +214,58 @@
 
     assert cur.describe("select * from customers") == expected_metadata
 
     cur.execute("select * from customers")
     assert cur.description == expected_metadata
 
 
+def test_describe_with_params(cur: snowflake.connector.cursor.SnowflakeCursor):
+    cur.execute(
+        """
+        create table customers (
+            ID int, CNAME varchar, AMOUNT decimal(10,2), PCT real, ACTIVE boolean,
+            UPDATE_AT timestamp, UPDATE_AT_NTZ timestamp_ntz(9), INSERTIONDATE DATE
+        )
+        """
+    )
+    # fmt: off
+    expected_metadata = [
+        snowflake.connector.cursor.ResultMetadata(
+            name="ID", type_code=0, display_size=None, internal_size=None, precision=38, scale=0, is_nullable=True                  # type: ignore # noqa: E501
+        ),
+        snowflake.connector.cursor.ResultMetadata(
+            name="CNAME", type_code=2, display_size=None, internal_size=16777216, precision=None, scale=None, is_nullable=True,     # type: ignore # noqa: E501
+        ),
+        snowflake.connector.cursor.ResultMetadata(
+            name="AMOUNT", type_code=0, display_size=None, internal_size=None, precision=10, scale=2, is_nullable=True,             # type: ignore # noqa: E501
+        ),
+        snowflake.connector.cursor.ResultMetadata(
+            name="PCT", type_code=1, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True,           # type: ignore # noqa: E501
+        ),
+        snowflake.connector.cursor.ResultMetadata(
+            name="ACTIVE", type_code=13, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True,       # type: ignore # noqa: E501
+        ),
+        snowflake.connector.cursor.ResultMetadata(
+            name='UPDATE_AT', type_code=8, display_size=None, internal_size=None, precision=0, scale=9, is_nullable=True            # type: ignore # noqa: E501
+        ),
+        snowflake.connector.cursor.ResultMetadata(
+            name='UPDATE_AT_NTZ', type_code=8, display_size=None, internal_size=None, precision=0, scale=9, is_nullable=True        # type: ignore # noqa: E501
+        ),
+        snowflake.connector.cursor.ResultMetadata(
+            name='INSERTIONDATE', type_code=3, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True  # type: ignore # noqa: E501
+        ),
+    ]
+    # fmt: on
+
+    assert cur.describe("select * from customers where id = ?", (1,)) == expected_metadata
+
+    cur.execute("select * from customers where id = ?", (1,))
+    assert cur.description == expected_metadata
+
+
 def test_executemany(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
 
     customers = [(1, "Jenny", "P"), (2, "Jasper", "M")]
     cur.executemany("insert into customers (id, first_name, last_name) values (%s,%s,%s)", customers)
 
     cur.execute("select id, first_name, last_name from customers")
@@ -414,14 +458,31 @@
 
 
 def test_timestamp_to_date(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("SELECT to_date(to_timestamp(0)), to_date(cast(to_timestamp(0) as timestamp(9)))")
     assert cur.fetchall() == [(datetime.date(1970, 1, 1), datetime.date(1970, 1, 1))]
 
 
+def test_transactions(conn: snowflake.connector.SnowflakeConnection):
+    conn.execute_string(
+        """CREATE TABLE table1 (i int);
+            BEGIN TRANSACTION;
+            INSERT INTO table1 (i) VALUES (1);"""
+    )
+    conn.rollback()
+    conn.execute_string(
+        """BEGIN TRANSACTION;
+            INSERT INTO table1 (i) VALUES (2);"""
+    )
+    conn.commit()
+    with conn.cursor() as cur:
+        cur.execute("SELECT * FROM table1")
+        assert cur.fetchall() == [(2,)]
+
+
 def test_unquoted_identifiers_are_upper_cased(conn: snowflake.connector.SnowflakeConnection):
     with conn.cursor(snowflake.connector.cursor.DictCursor) as cur:
         cur.execute("create table customers (id int, first_name varchar, last_name varchar)")
         cur.execute("insert into customers values (1, 'Jenny', 'P')")
         cur.execute("select first_name, first_name as fname from customers")
 
         assert cur.fetchall() == [
```

### Comparing `fakesnow-0.1.0/tests/test_patch.py` & `fakesnow-0.2.0/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.1.0/tests/test_transforms.py` & `fakesnow-0.2.0/tests/test_transforms.py`

 * *Files identical despite different names*

