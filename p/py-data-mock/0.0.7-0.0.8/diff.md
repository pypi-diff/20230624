# Comparing `tmp/py-data-mock-0.0.7.tar.gz` & `tmp/py-data-mock-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-data-mock-0.0.7.tar", last modified: Thu Jun  8 05:48:22 2023, max compression
+gzip compressed data, was "py-data-mock-0.0.8.tar", last modified: Sat Jun 24 21:02:46 2023, max compression
```

## Comparing `py-data-mock-0.0.7.tar` & `py-data-mock-0.0.8.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.678570 py-data-mock-0.0.7/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-08 05:48:22.678570 py-data-mock-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.670570 py-data-mock-0.0.7/data_mock/
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/__init__.py
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.670570 py-data-mock-0.0.7/data_mock/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.670570 py-data-mock-0.0.7/data_mock/google/cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.674570 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/
--rw-r--r--   0 root         (0) root         (0)      827 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6323 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/client.py
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/dataset.py
--rw-r--r--   0 root         (0) root         (0)     1427 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/enums.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.674570 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/job/
--rw-r--r--   0 root         (0) root         (0)      329 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/job/load.py
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/job/query.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/retry.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/schema.py
--rw-r--r--   0 root         (0) root         (0)     3013 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.674570 py-data-mock-0.0.7/data_mock/google/cloud/storage/
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/storage/blob.py
--rw-r--r--   0 root         (0) root         (0)      522 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/storage/bucket.py
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.674570 py-data-mock-0.0.7/data_mock/mock_helpers/
--rw-r--r--   0 root         (0) root         (0)     8025 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/mock_helpers/generate_data.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/mock_helpers/provider.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/mock_helpers/writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.678570 py-data-mock-0.0.7/data_mock/psycopg2/
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/psycopg2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4979 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/psycopg2/connect.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/psycopg2/cursor.py
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/psycopg2/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/psycopg2/extras.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.678570 py-data-mock-0.0.7/py_data_mock.egg-info/
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-08 05:48:22.000000 py-data-mock-0.0.7/py_data_mock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1117 2023-06-08 05:48:22.000000 py-data-mock-0.0.7/py_data_mock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 05:48:22.000000 py-data-mock-0.0.7/py_data_mock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-08 05:48:22.000000 py-data-mock-0.0.7/py_data_mock.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 05:48:22.678570 py-data-mock-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      635 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.558688 py-data-mock-0.0.8/data_mock/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.554687 py-data-mock-0.0.8/data_mock/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.554687 py-data-mock-0.0.8/data_mock/google/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.558688 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/
+-rw-r--r--   0 root         (0) root         (0)      827 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6784 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/client.py
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/enums.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.558688 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/job/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/job/load.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/job/query.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/retry.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/schema.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.558688 py-data-mock-0.0.8/data_mock/google/cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/storage/blob.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/storage/bucket.py
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/data_mock/mock_helpers/
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/mock_helpers/generate_data.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/mock_helpers/provider.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/mock_helpers/writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/data_mock/psycopg2/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/psycopg2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5039 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/psycopg2/connect.py
+-rw-r--r--   0 root         (0) root         (0)     5360 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/psycopg2/cursor.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/psycopg2/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/psycopg2/extras.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/py_data_mock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-24 21:02:46.000000 py-data-mock-0.0.8/py_data_mock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-24 21:02:46.000000 py-data-mock-0.0.8/py_data_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 21:02:46.000000 py-data-mock-0.0.8/py_data_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-24 21:02:46.000000 py-data-mock-0.0.8/py_data_mock.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      635 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/setup.py
```

### Comparing `py-data-mock-0.0.7/LICENSE` & `py-data-mock-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.7/README.md` & `py-data-mock-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.7/data_mock/google/cloud/bigquery/__init__.py` & `py-data-mock-0.0.8/data_mock/google/cloud/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.7/data_mock/google/cloud/bigquery/enums.py` & `py-data-mock-0.0.8/data_mock/google/cloud/bigquery/enums.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.7/data_mock/google/cloud/bigquery/table.py` & `py-data-mock-0.0.8/data_mock/google/cloud/bigquery/table.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.7/data_mock/google/cloud/storage/blob.py` & `py-data-mock-0.0.8/data_mock/google/cloud/storage/blob.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.7/data_mock/google/cloud/storage/bucket.py` & `py-data-mock-0.0.8/data_mock/google/cloud/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.7/data_mock/mock_helpers/generate_data.py` & `py-data-mock-0.0.8/data_mock/mock_helpers/generate_data.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.7/data_mock/mock_helpers/provider.py` & `py-data-mock-0.0.8/data_mock/mock_helpers/provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import types
-from typing import Union, List
+from typing import Union, List, Iterator, Type, Tuple, TypeVar
 import data_mock.exceptions
 from data_mock.google.cloud import bigquery
 #from bigquery import SchemaField
 import types
 
+V = TypeVar('V')
+
 class EmptyGenerator:
+    #not used!
 
     def __init__(self):
         self.metadata = {}
 
     def gen_func(self):
         for i in range(0):
             yield i
 
     def query_results(self):
         return self.gen_func(), {'total_rows':0, 'schema' : None}
 
 class QueryResultsFromList:
 
-    def __init__(self, data):
+    def __init__(self, data:list):
         self.data = data
         self.make_schema()
 
-    def make_schema(self):
+    def make_schema(self) -> None :
         if len(self.data) == 0:
             self.schema = None
-            return
+            return None
         schema = []
         for i in self.data[0]:
-            schema.append(bigquery.SchemaField(name = i[0], field_type = type(i[1])))
+            schema.append(bigquery.SchemaField(name = i[0], field_type = str(type(i[1]))))
         self.schema = schema
 
-    def gen_func(self):
+    def gen_func(self) -> Iterator[List]:
         for i in self.data:
             l = []
             for j in i:
                 c = Data(name = j[0], value = j[1])
                 l.append(c)
             yield l
 
@@ -55,30 +58,28 @@
     def __init__(self):
         self.dict = {}
 
     def data_from_list(self, data:List, tag:str ):
         self._test_valid_data(data)
         self.dict[tag] = QueryResultsFromList(data = data)
 
-    def add_data(self, data:List, tag:str):
+    def add_data(self, data:Union[List, V], tag:str):
         if isinstance(data, list):
             self.data_from_list(data, tag)
         else:
             self.dict[tag] = data
 
-    def get_data(self, key:str) -> Union[None, types.GeneratorType]:
+    def get_data(self, key:str) -> Union[Tuple[None, None], Tuple[types.GeneratorType, dict]]:
         if not self.dict.get(key):
             return None, None
         if not  hasattr(self.dict[key], 'query_results'):
             raise data_mock.exceptions.InvalidMockData('object does not have query_results')
         if not isinstance(self.dict[key].query_results, types.MethodType):
             msg = '"query_results" is  not a method; did you pass the class rather than class()?'
             raise data_mock.exceptions.InvalidMockData(msg)
-
-
         return self.dict[key].query_results()
 
     def _test_valid_data(self, data):
         if not isinstance(data, list):
             raise data_mock.exceptions.InvalidMockData(f'{data} is not a list')
         errors = []
         for n, i in enumerate(data):
```

### Comparing `py-data-mock-0.0.7/data_mock/psycopg2/connect.py` & `py-data-mock-0.0.8/data_mock/psycopg2/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from data_mock.psycopg2.cursor import Cursor
 from data_mock.psycopg2.extras import RealDictCursor
 
 import data_mock.mock_helpers.provider as provider
 
-from typing import Union
+from typing import Union, Type
 
 class Connect:
 
-    def __init__(self, dsn=None, connection_factory=None, 
-            mock_data = None,  **kwargs):
+    def __init__(self, dsn:None=None, connection_factory:None=None, 
+            mock_data:Union[list, None] = None,  **kwargs):
         self.data_provider = provider.ProvideData()
         if mock_data:
             self.data_provider.add_data(data = mock_data, tag = 'default')
         self.register_initial_mock_data()
         
     def register_initial_mock_data(self):
         pass
 
     def register_mock_data(self, key:str, mock_data:list):
         self.data_provider.add_data(data = mock_data, tag = key)
 
-    def cursor(self, cursor_factory: Union[Cursor, RealDictCursor] = Cursor) -> Union[Cursor, RealDictCursor]:
+    def cursor(self, cursor_factory: Union[Type[Cursor], Type[RealDictCursor]] \
+            = Cursor) -> Union[Cursor, RealDictCursor]:
         return cursor_factory(data_provider = self.data_provider)
 
     def commit(self, *args, **kwargs):
         pass
 
     def close(self, *args, **kwargs):
         pass
```

### Comparing `py-data-mock-0.0.7/data_mock/psycopg2/cursor.py` & `py-data-mock-0.0.8/data_mock/psycopg2/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 from collections import OrderedDict
 
 import data_mock.mock_helpers.provider as provider
 from data_mock.psycopg2.exceptions import ProgrammingError
 import data_mock.exceptions as exceptions
 
 class Cursor:
@@ -18,15 +20,15 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         pass
 
-    def execute(self, query:str, vars:tuple = None):
+    def execute(self, query:str, vars:Union[tuple, None] = None):
         """
         all args ignored except query
         """
 
         key = self._get_sql_key(query)
         if key:
             self.data, self.meta_data = self.data_provider.get_data(key)
@@ -52,15 +54,15 @@
 
     def fetchmany(self, n:int)-> list:
         counter = 0
         final = []
         if not hasattr(self, 'data'):
             raise ProgrammingError('no result to fetch')
         if not self.data:
-            return
+            return []
         for counter, row in enumerate(self.data):
             new_row = self.construct_row(row)
             final.append(new_row)
             if counter + 1 == n:
                 return final
         return final
 
@@ -68,15 +70,15 @@
         return self.fetchmany(n=1)
 
     def fetchall(self)-> list:
         final = []
         if not hasattr(self, 'data'):
             raise ProgrammingError('no result to fetch')
         if not self.data:
-            return
+            return []
         for counter, row in enumerate(self.data):
             new_row = self.construct_row(row)
             final.append(new_row)
         return final
 
     def close(self, *args, **kwargs):
         pass
@@ -168,15 +170,16 @@
 
     def tzinfo_factory(self, *args, **kwargs):
          raise NotImplementedError()
 
     def withhold(self, *args, **kwargs):
          raise NotImplementedError()
 
-    def _get_sql_key(self, query:str)-> str:
+    def _get_sql_key(self, query:str)-> Union[str, None]:
         for line in query.split('\n'):
             if 'py-postgres-mock-register:' in line:
                 fields = line.split(':')
                 if len(fields) != 2:
                     raise exceptions.InvalidMockData('hint should be in format "py-postgres-mock-register: key"')
                 return fields[1].strip()
+        return None
```

### Comparing `py-data-mock-0.0.7/py_data_mock.egg-info/SOURCES.txt` & `py-data-mock-0.0.8/py_data_mock.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 data_mock/__init__.py
 data_mock/exceptions.py
+data_mock/requests.py
 data_mock/google/cloud/bigquery/__init__.py
 data_mock/google/cloud/bigquery/client.py
 data_mock/google/cloud/bigquery/dataset.py
 data_mock/google/cloud/bigquery/enums.py
 data_mock/google/cloud/bigquery/exceptions.py
 data_mock/google/cloud/bigquery/retry.py
 data_mock/google/cloud/bigquery/schema.py
```

### Comparing `py-data-mock-0.0.7/setup.py` & `py-data-mock-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='py-data-mock',
-    version='0.0.7',    
+    version='0.0.8',    
     description='Mock Data',
     url='https://github.com/paulhtremblay/py-data-mock',
     author='Henry Tremblay',
     author_email='paulhtremblay@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['data_mock/google/cloud/bigquery/job', 'data_mock/google/cloud/bigquery',
         'data_mock/google/cloud/storage','data_mock/mock_helpers', 'data_mock',
```

