# Comparing `tmp/rain_orm-1.0.8.tar.gz` & `tmp/rain_orm-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rain_orm-1.0.8.tar", last modified: Sat Jun 24 08:53:03 2023, max compression
+gzip compressed data, was "rain_orm-1.0.9.tar", last modified: Sat Jun 24 18:56:50 2023, max compression
```

## Comparing `rain_orm-1.0.8.tar` & `rain_orm-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.536193 rain_orm-1.0.8/
--rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     3514 2023-06-24 08:53:03.536193 rain_orm-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3233 2023-06-22 02:02:54.000000 rain_orm-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.496285 rain_orm-1.0.8/rain_orm/
--rw-rw-rw-   0        0        0      139 2023-06-24 08:52:02.000000 rain_orm-1.0.8/rain_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.517614 rain_orm-1.0.8/rain_orm/column/
--rw-rw-rw-   0        0        0      189 2023-06-24 08:52:02.000000 rain_orm-1.0.8/rain_orm/column/__init__.py
--rw-rw-rw-   0        0        0     1776 2023-06-24 08:45:30.000000 rain_orm-1.0.8/rain_orm/column/base.py
--rw-rw-rw-   0        0        0      238 2023-06-24 08:45:30.000000 rain_orm-1.0.8/rain_orm/column/date.py
--rw-rw-rw-   0        0        0      400 2023-06-05 03:57:35.000000 rain_orm-1.0.8/rain_orm/column/number.py
--rw-rw-rw-   0        0        0      688 2023-06-05 10:24:07.000000 rain_orm-1.0.8/rain_orm/column/string.py
--rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.8/rain_orm/common.py
--rw-rw-rw-   0        0        0      781 2023-06-05 00:52:45.000000 rain_orm-1.0.8/rain_orm/db.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.521181 rain_orm-1.0.8/rain_orm/error/
--rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.8/rain_orm/error/__init__.py
--rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.8/rain_orm/error/error.py
--rw-rw-rw-   0        0        0     1304 2023-06-24 04:57:30.000000 rain_orm-1.0.8/rain_orm/metatable.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.530194 rain_orm-1.0.8/rain_orm/sql_builder/
--rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.8/rain_orm/sql_builder/__init__.py
--rw-rw-rw-   0        0        0     1536 2023-06-24 04:49:52.000000 rain_orm-1.0.8/rain_orm/sql_builder/ddl_builder.py
--rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.8/rain_orm/sql_builder/dmldql_builder.py
--rw-rw-rw-   0        0        0     7034 2023-06-24 08:52:02.000000 rain_orm-1.0.8/rain_orm/table.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.507366 rain_orm-1.0.8/rain_orm.egg-info/
--rw-rw-rw-   0        0        0     3514 2023-06-24 08:53:03.000000 rain_orm-1.0.8/rain_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-06-24 08:53:03.000000 rain_orm-1.0.8/rain_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 08:53:03.000000 rain_orm-1.0.8/rain_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-24 08:53:03.000000 rain_orm-1.0.8/rain_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-24 08:53:03.000000 rain_orm-1.0.8/rain_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-24 08:53:03.538191 rain_orm-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      474 2023-06-24 08:52:02.000000 rain_orm-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.534193 rain_orm-1.0.8/tests/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0      749 2023-06-24 05:12:49.000000 rain_orm-1.0.8/tests/t.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:56:50.366369 rain_orm-1.0.9/
+-rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3672 2023-06-24 18:56:50.366369 rain_orm-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3391 2023-06-24 18:54:54.000000 rain_orm-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 18:56:50.336109 rain_orm-1.0.9/rain_orm/
+-rw-rw-rw-   0        0        0      139 2023-06-24 18:54:54.000000 rain_orm-1.0.9/rain_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:56:50.353305 rain_orm-1.0.9/rain_orm/column/
+-rw-rw-rw-   0        0        0      189 2023-06-24 08:52:02.000000 rain_orm-1.0.9/rain_orm/column/__init__.py
+-rw-rw-rw-   0        0        0     1776 2023-06-24 08:45:30.000000 rain_orm-1.0.9/rain_orm/column/base.py
+-rw-rw-rw-   0        0        0      238 2023-06-24 08:45:30.000000 rain_orm-1.0.9/rain_orm/column/date.py
+-rw-rw-rw-   0        0        0      400 2023-06-05 03:57:35.000000 rain_orm-1.0.9/rain_orm/column/number.py
+-rw-rw-rw-   0        0        0      688 2023-06-05 10:24:07.000000 rain_orm-1.0.9/rain_orm/column/string.py
+-rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.9/rain_orm/common.py
+-rw-rw-rw-   0        0        0      781 2023-06-05 00:52:45.000000 rain_orm-1.0.9/rain_orm/db.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:56:50.356296 rain_orm-1.0.9/rain_orm/error/
+-rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.9/rain_orm/error/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.9/rain_orm/error/error.py
+-rw-rw-rw-   0        0        0     1363 2023-06-24 18:43:08.000000 rain_orm-1.0.9/rain_orm/metatable.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:56:50.360364 rain_orm-1.0.9/rain_orm/sql_builder/
+-rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.9/rain_orm/sql_builder/__init__.py
+-rw-rw-rw-   0        0        0     1879 2023-06-24 18:49:31.000000 rain_orm-1.0.9/rain_orm/sql_builder/ddl_builder.py
+-rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.9/rain_orm/sql_builder/dmldql_builder.py
+-rw-rw-rw-   0        0        0     7034 2023-06-24 08:52:02.000000 rain_orm-1.0.9/rain_orm/table.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:56:50.345296 rain_orm-1.0.9/rain_orm.egg-info/
+-rw-rw-rw-   0        0        0     3672 2023-06-24 18:56:50.000000 rain_orm-1.0.9/rain_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-06-24 18:56:50.000000 rain_orm-1.0.9/rain_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:56:50.000000 rain_orm-1.0.9/rain_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-24 18:56:50.000000 rain_orm-1.0.9/rain_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-24 18:56:50.000000 rain_orm-1.0.9/rain_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-24 18:56:50.367369 rain_orm-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      474 2023-06-24 18:54:54.000000 rain_orm-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:56:50.363369 rain_orm-1.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-06-24 18:52:30.000000 rain_orm-1.0.9/tests/t.py
```

### Comparing `rain_orm-1.0.8/LICENSE` & `rain_orm-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.8/PKG-INFO` & `rain_orm-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rain_orm
-Version: 1.0.8
+Version: 1.0.9
 Summary: a tiny orm frame
 Home-page: https://github.com/cgynb/rain-orm
 Author: rain
 Author-email: 948628463@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -91,26 +91,33 @@
 rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
 ```
 
 ## Define Model
 
 each data must have a unique "id"
 ```python
-import rain_orm
+from rain_orm import Table
 from rain_orm.column import Int, VarChar
 
-class StudentModel(rain_orm.Table):
-    __table__ = "students"
+
+class ClassModel(Table):
+    __table__ = "classes"
     __fields__ = {
-        "id": Int(auto_increment=True, primary_key=True),
-        "name": VarChar(30, unique=True),
-        "password": VarChar(30),
-        "class_id": Int(default=1)
+        "id": Int(primary_key=True, auto_increment=True),
+        "name": VarChar(30)
     }
 
+
+class StudentModel(Table):
+    __table__ = "students"
+    __fields__ = {
+        "id": Int(primary_key=True, auto_increment=True),
+        "name": VarChar(30, not_null=True),
+        "class_id": Int(foreign_key=ClassModel.id)
+    }
 ```
 ## Auto Migrate
 
 ```python
 # all subclasses that inherit rain_orm.Table
 rain_orm.Table.auto_migrate() 
 # create StudentModel
```

### Comparing `rain_orm-1.0.8/README.md` & `rain_orm-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -79,26 +79,33 @@
 rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
 ```
 
 ## Define Model
 
 each data must have a unique "id"
 ```python
-import rain_orm
+from rain_orm import Table
 from rain_orm.column import Int, VarChar
 
-class StudentModel(rain_orm.Table):
-    __table__ = "students"
+
+class ClassModel(Table):
+    __table__ = "classes"
     __fields__ = {
-        "id": Int(auto_increment=True, primary_key=True),
-        "name": VarChar(30, unique=True),
-        "password": VarChar(30),
-        "class_id": Int(default=1)
+        "id": Int(primary_key=True, auto_increment=True),
+        "name": VarChar(30)
     }
 
+
+class StudentModel(Table):
+    __table__ = "students"
+    __fields__ = {
+        "id": Int(primary_key=True, auto_increment=True),
+        "name": VarChar(30, not_null=True),
+        "class_id": Int(foreign_key=ClassModel.id)
+    }
 ```
 ## Auto Migrate
 
 ```python
 # all subclasses that inherit rain_orm.Table
 rain_orm.Table.auto_migrate() 
 # create StudentModel
```

### Comparing `rain_orm-1.0.8/rain_orm/column/base.py` & `rain_orm-1.0.9/rain_orm/column/base.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.8/rain_orm/column/string.py` & `rain_orm-1.0.9/rain_orm/column/string.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.8/rain_orm/db.py` & `rain_orm-1.0.9/rain_orm/db.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.8/rain_orm/metatable.py` & `rain_orm-1.0.9/rain_orm/metatable.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,10 +20,13 @@
         if not all([isinstance(item, Type) for _, item in namespace.get('__fields__').items()]):
             raise ValueError(f"items of __fields__ should be instance of rain_orm.column.Type")
         return type.__new__(mcs, name, bases, namespace)
 
     def __getattr__(cls, item):
         if item not in cls.__fields__.keys():
             raise ValueError(f"there's no field <{item}> in table {cls.__table__}")
-        return f"{cls.__table__}.{item}"
+        return {
+            "ref_table": cls.__table__,
+            "ref_field": item
+        }
```

### Comparing `rain_orm-1.0.8/rain_orm/sql_builder/dmldql_builder.py` & `rain_orm-1.0.9/rain_orm/sql_builder/dmldql_builder.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.8/rain_orm/table.py` & `rain_orm-1.0.9/rain_orm/table.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.8/rain_orm.egg-info/PKG-INFO` & `rain_orm-1.0.9/rain_orm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rain-orm
-Version: 1.0.8
+Version: 1.0.9
 Summary: a tiny orm frame
 Home-page: https://github.com/cgynb/rain-orm
 Author: rain
 Author-email: 948628463@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -91,26 +91,33 @@
 rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
 ```
 
 ## Define Model
 
 each data must have a unique "id"
 ```python
-import rain_orm
+from rain_orm import Table
 from rain_orm.column import Int, VarChar
 
-class StudentModel(rain_orm.Table):
-    __table__ = "students"
+
+class ClassModel(Table):
+    __table__ = "classes"
     __fields__ = {
-        "id": Int(auto_increment=True, primary_key=True),
-        "name": VarChar(30, unique=True),
-        "password": VarChar(30),
-        "class_id": Int(default=1)
+        "id": Int(primary_key=True, auto_increment=True),
+        "name": VarChar(30)
     }
 
+
+class StudentModel(Table):
+    __table__ = "students"
+    __fields__ = {
+        "id": Int(primary_key=True, auto_increment=True),
+        "name": VarChar(30, not_null=True),
+        "class_id": Int(foreign_key=ClassModel.id)
+    }
 ```
 ## Auto Migrate
 
 ```python
 # all subclasses that inherit rain_orm.Table
 rain_orm.Table.auto_migrate() 
 # create StudentModel
```

### Comparing `rain_orm-1.0.8/rain_orm.egg-info/SOURCES.txt` & `rain_orm-1.0.9/rain_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

