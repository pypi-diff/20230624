# Comparing `tmp/rain_orm-1.0.6.tar.gz` & `tmp/rain_orm-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rain_orm-1.0.6.tar", last modified: Thu Jun 22 07:35:35 2023, max compression
+gzip compressed data, was "rain_orm-1.0.7.tar", last modified: Sat Jun 24 05:27:50 2023, max compression
```

## Comparing `rain_orm-1.0.6.tar` & `rain_orm-1.0.7.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:35:35.000582 rain_orm-1.0.6/
--rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     3514 2023-06-22 07:35:35.000582 rain_orm-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3233 2023-06-22 02:02:54.000000 rain_orm-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 07:35:34.976947 rain_orm-1.0.6/rain_orm/
--rw-rw-rw-   0        0        0      139 2023-06-22 03:13:13.000000 rain_orm-1.0.6/rain_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:35:34.991542 rain_orm-1.0.6/rain_orm/column/
--rw-rw-rw-   0        0        0      153 2023-06-05 03:57:35.000000 rain_orm-1.0.6/rain_orm/column/__init__.py
--rw-rw-rw-   0        0        0     1602 2023-06-22 02:02:54.000000 rain_orm-1.0.6/rain_orm/column/base.py
--rw-rw-rw-   0        0        0      271 2023-06-05 03:57:35.000000 rain_orm-1.0.6/rain_orm/column/date.py
--rw-rw-rw-   0        0        0      400 2023-06-05 03:57:35.000000 rain_orm-1.0.6/rain_orm/column/number.py
--rw-rw-rw-   0        0        0      688 2023-06-05 10:24:07.000000 rain_orm-1.0.6/rain_orm/column/string.py
--rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.6/rain_orm/common.py
--rw-rw-rw-   0        0        0      781 2023-06-05 00:52:45.000000 rain_orm-1.0.6/rain_orm/db.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:35:34.993564 rain_orm-1.0.6/rain_orm/error/
--rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.6/rain_orm/error/__init__.py
--rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.6/rain_orm/error/error.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:35:34.997559 rain_orm-1.0.6/rain_orm/sql_builder/
--rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.6/rain_orm/sql_builder/__init__.py
--rw-rw-rw-   0        0        0     1280 2023-06-08 12:04:47.000000 rain_orm-1.0.6/rain_orm/sql_builder/ddl_builder.py
--rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.6/rain_orm/sql_builder/dmldql_builder.py
--rw-rw-rw-   0        0        0     7333 2023-06-22 04:00:38.000000 rain_orm-1.0.6/rain_orm/table.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:35:34.983459 rain_orm-1.0.6/rain_orm.egg-info/
--rw-rw-rw-   0        0        0     3514 2023-06-22 07:35:34.000000 rain_orm-1.0.6/rain_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      573 2023-06-22 07:35:34.000000 rain_orm-1.0.6/rain_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:35:34.000000 rain_orm-1.0.6/rain_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-22 07:35:34.000000 rain_orm-1.0.6/rain_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-22 07:35:34.000000 rain_orm-1.0.6/rain_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-22 07:35:35.001581 rain_orm-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      474 2023-06-22 03:13:13.000000 rain_orm-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:35:34.999542 rain_orm-1.0.6/tests/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.339259 rain_orm-1.0.7/
+-rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3514 2023-06-24 05:27:50.339259 rain_orm-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3233 2023-06-22 02:02:54.000000 rain_orm-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.306703 rain_orm-1.0.7/rain_orm/
+-rw-rw-rw-   0        0        0      139 2023-06-24 05:13:16.000000 rain_orm-1.0.7/rain_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.324256 rain_orm-1.0.7/rain_orm/column/
+-rw-rw-rw-   0        0        0      153 2023-06-05 03:57:35.000000 rain_orm-1.0.7/rain_orm/column/__init__.py
+-rw-rw-rw-   0        0        0     1661 2023-06-24 04:49:52.000000 rain_orm-1.0.7/rain_orm/column/base.py
+-rw-rw-rw-   0        0        0      271 2023-06-05 03:57:35.000000 rain_orm-1.0.7/rain_orm/column/date.py
+-rw-rw-rw-   0        0        0      400 2023-06-05 03:57:35.000000 rain_orm-1.0.7/rain_orm/column/number.py
+-rw-rw-rw-   0        0        0      688 2023-06-05 10:24:07.000000 rain_orm-1.0.7/rain_orm/column/string.py
+-rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.7/rain_orm/common.py
+-rw-rw-rw-   0        0        0      781 2023-06-05 00:52:45.000000 rain_orm-1.0.7/rain_orm/db.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.327258 rain_orm-1.0.7/rain_orm/error/
+-rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.7/rain_orm/error/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.7/rain_orm/error/error.py
+-rw-rw-rw-   0        0        0     1304 2023-06-24 04:57:30.000000 rain_orm-1.0.7/rain_orm/metatable.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.333261 rain_orm-1.0.7/rain_orm/sql_builder/
+-rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.7/rain_orm/sql_builder/__init__.py
+-rw-rw-rw-   0        0        0     1536 2023-06-24 04:49:52.000000 rain_orm-1.0.7/rain_orm/sql_builder/ddl_builder.py
+-rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.7/rain_orm/sql_builder/dmldql_builder.py
+-rw-rw-rw-   0        0        0     6992 2023-06-24 04:49:52.000000 rain_orm-1.0.7/rain_orm/table.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.314744 rain_orm-1.0.7/rain_orm.egg-info/
+-rw-rw-rw-   0        0        0     3514 2023-06-24 05:27:50.000000 rain_orm-1.0.7/rain_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-06-24 05:27:50.000000 rain_orm-1.0.7/rain_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 05:27:50.000000 rain_orm-1.0.7/rain_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-24 05:27:50.000000 rain_orm-1.0.7/rain_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-24 05:27:50.000000 rain_orm-1.0.7/rain_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-24 05:27:50.340264 rain_orm-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      474 2023-06-24 05:13:16.000000 rain_orm-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.337257 rain_orm-1.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      749 2023-06-24 05:12:49.000000 rain_orm-1.0.7/tests/t.py
```

### Comparing `rain_orm-1.0.6/LICENSE` & `rain_orm-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.6/PKG-INFO` & `rain_orm-1.0.7/rain_orm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rain_orm
-Version: 1.0.6
+Name: rain-orm
+Version: 1.0.7
 Summary: a tiny orm frame
 Home-page: https://github.com/cgynb/rain-orm
 Author: rain
 Author-email: 948628463@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `rain_orm-1.0.6/README.md` & `rain_orm-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.6/rain_orm/column/base.py` & `rain_orm-1.0.7/rain_orm/column/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 class Type(object):
     type_name = None
 
     def __new__(cls, *args, **kwargs):
         cls.type_name = cls.__name__.casefold()
         return object.__new__(cls)
 
-    def __init__(self, primary_key=False, unique=False, not_null=False, auto_increment=False,  default=None):
+    def __init__(self, primary_key=False, unique=False, not_null=False, auto_increment=False, foreign_key=None,  default=None):
         self.__value = None
         self.default = default
         self.constraint = {
             "primary_key": primary_key,
             "auto_increment": auto_increment,
             "unique": unique,
-            "not_null": not_null
+            "not_null": not_null,
+            "foreign_key": foreign_key
         }
 
     def __str__(self):
         return str(self.__value)
 
     def __repr__(self):
         return str(self)
```

### Comparing `rain_orm-1.0.6/rain_orm/column/string.py` & `rain_orm-1.0.7/rain_orm/column/string.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.6/rain_orm/db.py` & `rain_orm-1.0.7/rain_orm/db.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.6/rain_orm/sql_builder/ddl_builder.py` & `rain_orm-1.0.7/rain_orm/sql_builder/ddl_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 class DDLBuilder:
     def __init__(self, table):
         self.table = table
         self.__sql_str = None
         self.__fields = []
+        self.__foreign_keys = []
 
     def add_field(self, field_name, field_type, *, primary_key=False, unique=False, not_null=False,
-                  auto_increment=False):
+                  auto_increment=False, foreign_key=None):
         self.__fields.append({
             "field_name": field_name,
             "field_type": field_type,
             "constraint": {
                 "primary key": primary_key,
                 "unique": unique,
                 "not null": not_null,
                 "auto_increment": auto_increment
             }
         })
+        if foreign_key is not None:
+            self.__foreign_keys.append({
+                "field_name": field_name,
+                "reference": foreign_key
+            })
 
     @property
     def create_sql(self):
+        # TODO: 外鍵
         sql = f"create table if not exists {self.table}"
         sql += "("
         for field in self.__fields:
             sql += f"{field['field_name']} {field['field_type']}"
             for k, v in field['constraint'].items():
                 if v is not False:
                     sql += f" {k}"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rain_orm-1.0.6/rain_orm/sql_builder/dmldql_builder.py` & `rain_orm-1.0.7/rain_orm/sql_builder/dmldql_builder.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.6/rain_orm/table.py` & `rain_orm-1.0.7/rain_orm/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import datetime
 
 try:
     from rain_orm.error import DefineError, SqlBuildError, UpdateError
     from rain_orm.sql_builder import DMLDQLBuilder, DDLBuilder
     from rain_orm.column import Type
     from rain_orm.db import DB
+    from rain_orm.metatable import MetaTable
 except ImportError as e:
     print(e)
     from error import DefineError, SqlBuildError, UpdateError
     from sql_builder import DMLDQLBuilder, DDLBuilder
     from column import Type
     from db import DB
+    from metatable import MetaTable
 import pymysql
 import threading
 import copy
 
 
-class Table(object):
+class Table(metaclass=MetaTable):
     __db = None
     __lock = threading.Lock()
+    __table__ = ""
+    __fields__ = {}
 
     @classmethod
     def set_db(cls, db):
         cls.__db = db
 
     @classmethod
     def auto_migrate(cls, *classes):
@@ -35,21 +39,14 @@
             ddls.append(ddl_builder.create_sql)
         with cls.__lock:
             for ddl in ddls:
                 cls.__db.cursor.execute(ddl)
             cls.__db.commit()
 
     def __init__(self, **kwargs):
-        if not isinstance(self.__table__, str):
-            raise ValueError(f"type(__table__) should be str, but is {type(self.__table__)}")
-        if not isinstance(self.__fields__, dict):
-            raise ValueError(f"type(__fields__) should be dict, but is {type(self.__fields__)}")
-        if not all([isinstance(item, Type) for _, item in self.__fields__.items()]):
-            raise ValueError(f"items of __fields__ should be instance of rain_orm.column.Type")
-
         self.__instance = copy.deepcopy(self.__fields__)
         self.__dmldql_builder = DMLDQLBuilder(self.__table__)
         for k, v in kwargs.items():
             self.__instance[k].value = v
         self.is_none = False
 
     def __str__(self):
```

### Comparing `rain_orm-1.0.6/rain_orm.egg-info/PKG-INFO` & `rain_orm-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rain-orm
-Version: 1.0.6
+Name: rain_orm
+Version: 1.0.7
 Summary: a tiny orm frame
 Home-page: https://github.com/cgynb/rain-orm
 Author: rain
 Author-email: 948628463@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `rain_orm-1.0.6/rain_orm.egg-info/SOURCES.txt` & `rain_orm-1.0.7/rain_orm.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 rain_orm/__init__.py
 rain_orm/common.py
 rain_orm/db.py
+rain_orm/metatable.py
 rain_orm/table.py
 rain_orm.egg-info/PKG-INFO
 rain_orm.egg-info/SOURCES.txt
 rain_orm.egg-info/dependency_links.txt
 rain_orm.egg-info/requires.txt
 rain_orm.egg-info/top_level.txt
 rain_orm/column/__init__.py
@@ -17,8 +18,9 @@
 rain_orm/column/number.py
 rain_orm/column/string.py
 rain_orm/error/__init__.py
 rain_orm/error/error.py
 rain_orm/sql_builder/__init__.py
 rain_orm/sql_builder/ddl_builder.py
 rain_orm/sql_builder/dmldql_builder.py
-tests/__init__.py
+tests/__init__.py
+tests/t.py
```

