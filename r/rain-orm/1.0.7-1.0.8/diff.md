# Comparing `tmp/rain_orm-1.0.7.tar.gz` & `tmp/rain_orm-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rain_orm-1.0.7.tar", last modified: Sat Jun 24 05:27:50 2023, max compression
+gzip compressed data, was "rain_orm-1.0.8.tar", last modified: Sat Jun 24 08:53:03 2023, max compression
```

## Comparing `rain_orm-1.0.7.tar` & `rain_orm-1.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.339259 rain_orm-1.0.7/
--rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     3514 2023-06-24 05:27:50.339259 rain_orm-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3233 2023-06-22 02:02:54.000000 rain_orm-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.306703 rain_orm-1.0.7/rain_orm/
--rw-rw-rw-   0        0        0      139 2023-06-24 05:13:16.000000 rain_orm-1.0.7/rain_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.324256 rain_orm-1.0.7/rain_orm/column/
--rw-rw-rw-   0        0        0      153 2023-06-05 03:57:35.000000 rain_orm-1.0.7/rain_orm/column/__init__.py
--rw-rw-rw-   0        0        0     1661 2023-06-24 04:49:52.000000 rain_orm-1.0.7/rain_orm/column/base.py
--rw-rw-rw-   0        0        0      271 2023-06-05 03:57:35.000000 rain_orm-1.0.7/rain_orm/column/date.py
--rw-rw-rw-   0        0        0      400 2023-06-05 03:57:35.000000 rain_orm-1.0.7/rain_orm/column/number.py
--rw-rw-rw-   0        0        0      688 2023-06-05 10:24:07.000000 rain_orm-1.0.7/rain_orm/column/string.py
--rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.7/rain_orm/common.py
--rw-rw-rw-   0        0        0      781 2023-06-05 00:52:45.000000 rain_orm-1.0.7/rain_orm/db.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.327258 rain_orm-1.0.7/rain_orm/error/
--rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.7/rain_orm/error/__init__.py
--rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.7/rain_orm/error/error.py
--rw-rw-rw-   0        0        0     1304 2023-06-24 04:57:30.000000 rain_orm-1.0.7/rain_orm/metatable.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.333261 rain_orm-1.0.7/rain_orm/sql_builder/
--rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.7/rain_orm/sql_builder/__init__.py
--rw-rw-rw-   0        0        0     1536 2023-06-24 04:49:52.000000 rain_orm-1.0.7/rain_orm/sql_builder/ddl_builder.py
--rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.7/rain_orm/sql_builder/dmldql_builder.py
--rw-rw-rw-   0        0        0     6992 2023-06-24 04:49:52.000000 rain_orm-1.0.7/rain_orm/table.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.314744 rain_orm-1.0.7/rain_orm.egg-info/
--rw-rw-rw-   0        0        0     3514 2023-06-24 05:27:50.000000 rain_orm-1.0.7/rain_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-06-24 05:27:50.000000 rain_orm-1.0.7/rain_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 05:27:50.000000 rain_orm-1.0.7/rain_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-24 05:27:50.000000 rain_orm-1.0.7/rain_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-24 05:27:50.000000 rain_orm-1.0.7/rain_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-24 05:27:50.340264 rain_orm-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      474 2023-06-24 05:13:16.000000 rain_orm-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:27:50.337257 rain_orm-1.0.7/tests/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.7/tests/__init__.py
--rw-rw-rw-   0        0        0      749 2023-06-24 05:12:49.000000 rain_orm-1.0.7/tests/t.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.536193 rain_orm-1.0.8/
+-rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3514 2023-06-24 08:53:03.536193 rain_orm-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3233 2023-06-22 02:02:54.000000 rain_orm-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.496285 rain_orm-1.0.8/rain_orm/
+-rw-rw-rw-   0        0        0      139 2023-06-24 08:52:02.000000 rain_orm-1.0.8/rain_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.517614 rain_orm-1.0.8/rain_orm/column/
+-rw-rw-rw-   0        0        0      189 2023-06-24 08:52:02.000000 rain_orm-1.0.8/rain_orm/column/__init__.py
+-rw-rw-rw-   0        0        0     1776 2023-06-24 08:45:30.000000 rain_orm-1.0.8/rain_orm/column/base.py
+-rw-rw-rw-   0        0        0      238 2023-06-24 08:45:30.000000 rain_orm-1.0.8/rain_orm/column/date.py
+-rw-rw-rw-   0        0        0      400 2023-06-05 03:57:35.000000 rain_orm-1.0.8/rain_orm/column/number.py
+-rw-rw-rw-   0        0        0      688 2023-06-05 10:24:07.000000 rain_orm-1.0.8/rain_orm/column/string.py
+-rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.8/rain_orm/common.py
+-rw-rw-rw-   0        0        0      781 2023-06-05 00:52:45.000000 rain_orm-1.0.8/rain_orm/db.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.521181 rain_orm-1.0.8/rain_orm/error/
+-rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.8/rain_orm/error/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.8/rain_orm/error/error.py
+-rw-rw-rw-   0        0        0     1304 2023-06-24 04:57:30.000000 rain_orm-1.0.8/rain_orm/metatable.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.530194 rain_orm-1.0.8/rain_orm/sql_builder/
+-rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.8/rain_orm/sql_builder/__init__.py
+-rw-rw-rw-   0        0        0     1536 2023-06-24 04:49:52.000000 rain_orm-1.0.8/rain_orm/sql_builder/ddl_builder.py
+-rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.8/rain_orm/sql_builder/dmldql_builder.py
+-rw-rw-rw-   0        0        0     7034 2023-06-24 08:52:02.000000 rain_orm-1.0.8/rain_orm/table.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.507366 rain_orm-1.0.8/rain_orm.egg-info/
+-rw-rw-rw-   0        0        0     3514 2023-06-24 08:53:03.000000 rain_orm-1.0.8/rain_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-06-24 08:53:03.000000 rain_orm-1.0.8/rain_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 08:53:03.000000 rain_orm-1.0.8/rain_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-24 08:53:03.000000 rain_orm-1.0.8/rain_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-24 08:53:03.000000 rain_orm-1.0.8/rain_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-24 08:53:03.538191 rain_orm-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      474 2023-06-24 08:52:02.000000 rain_orm-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:53:03.534193 rain_orm-1.0.8/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.8/tests/__init__.py
+-rw-rw-rw-   0        0        0      749 2023-06-24 05:12:49.000000 rain_orm-1.0.8/tests/t.py
```

### Comparing `rain_orm-1.0.7/LICENSE` & `rain_orm-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.7/PKG-INFO` & `rain_orm-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rain_orm
-Version: 1.0.7
+Version: 1.0.8
 Summary: a tiny orm frame
 Home-page: https://github.com/cgynb/rain-orm
 Author: rain
 Author-email: 948628463@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `rain_orm-1.0.7/README.md` & `rain_orm-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.7/rain_orm/column/base.py` & `rain_orm-1.0.8/rain_orm/column/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import warnings
 
 
 class Type(object):
     type_name = None
 
     def __new__(cls, *args, **kwargs):
@@ -53,8 +54,11 @@
         return isinstance(val, int) or isinstance(val, float) or val is None
 
 
 class String(Type):
     def check(self, val):
         return isinstance(val, str) or val is None
 
-# class Date()
+
+class Date(Type):
+    def check(self, val):
+        return isinstance(val, datetime.datetime) or val is None
```

### Comparing `rain_orm-1.0.7/rain_orm/column/string.py` & `rain_orm-1.0.8/rain_orm/column/string.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.7/rain_orm/db.py` & `rain_orm-1.0.8/rain_orm/db.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.7/rain_orm/metatable.py` & `rain_orm-1.0.8/rain_orm/metatable.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.7/rain_orm/sql_builder/ddl_builder.py` & `rain_orm-1.0.8/rain_orm/sql_builder/ddl_builder.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.7/rain_orm/sql_builder/dmldql_builder.py` & `rain_orm-1.0.8/rain_orm/sql_builder/dmldql_builder.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.7/rain_orm/table.py` & `rain_orm-1.0.8/rain_orm/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def __str__(self):
         if self.is_none is True:
             return "None"
         table = self.__table__
         fields = list(self.__fields__.keys())
         instance = "{\n"
         for k, v in self.__instance.items():
-            if isinstance(v.value, str):
+            if isinstance(v.value, (str, datetime.datetime)):
                 v = f"'{v.value}'"
             instance += f"\t\t{k}: {v},\n"
         instance += "\t}"
         return f"\033[0;36m<< {self.__class__.__name__} {id(self)}\033[0m\n" \
                f"\t\033[0;32m.table\033[0m = {table}\n" \
                f"\t\033[0;32m.fields\033[0m = {fields}\n" \
                f"\t\033[0;32m.instance\033[0m = {instance}\n" \
@@ -172,15 +172,15 @@
                     self.__instance[key].value = value
                     return True
 
     # delete
     def delete(self):
         self.__dmldql_builder.clear_where()
         for field, val in self.__instance.items():
-            if isinstance(val.value, str):
+            if isinstance(val.value, (str, datetime.datetime)):
                 self.__dmldql_builder.where(f"{field} = '{val.value}'")
             elif val.value is None:
                 self.__dmldql_builder.where(f"{field} is null")
             else:
                 self.__dmldql_builder.where(f"{field} = {val.value}")
         with self.__lock:
             try:
```

### Comparing `rain_orm-1.0.7/rain_orm.egg-info/PKG-INFO` & `rain_orm-1.0.8/rain_orm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rain-orm
-Version: 1.0.7
+Version: 1.0.8
 Summary: a tiny orm frame
 Home-page: https://github.com/cgynb/rain-orm
 Author: rain
 Author-email: 948628463@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `rain_orm-1.0.7/rain_orm.egg-info/SOURCES.txt` & `rain_orm-1.0.8/rain_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.7/tests/t.py` & `rain_orm-1.0.8/tests/t.py`

 * *Files identical despite different names*

