# Comparing `tmp/citrusdb-0.4.0.tar.gz` & `tmp/citrusdb-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrusdb-0.4.0.tar", last modified: Thu Jun 15 19:17:20 2023, max compression
+gzip compressed data, was "citrusdb-0.5.0.tar", last modified: Sat Jun 24 14:36:20 2023, max compression
```

## Comparing `citrusdb-0.4.0.tar` & `citrusdb-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.323471 citrusdb-0.4.0/
--rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.4.0/LICENSE
--rw-r--r--   0 debabrata   (501) staff       (20)     2341 2023-06-15 19:17:20.323342 citrusdb-0.4.0/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)     1758 2023-06-15 19:08:11.000000 citrusdb-0.4.0/README.md
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.320189 citrusdb-0.4.0/citrusdb/
--rw-r--r--   0 debabrata   (501) staff       (20)      281 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.321187 citrusdb-0.4.0/citrusdb/api/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.4.0/citrusdb/api/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     3969 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/api/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)     6648 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/api/local.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.321320 citrusdb-0.4.0/citrusdb/db/
--rw-r--r--   0 debabrata   (501) staff       (20)     1039 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.321522 citrusdb-0.4.0/citrusdb/db/index/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.4.0/citrusdb/db/index/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/db/index/hnswlib.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.321890 citrusdb-0.4.0/citrusdb/db/postgres/
--rw-r--r--   0 debabrata   (501) staff       (20)     3888 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/postgres/db.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1479 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/postgres/queries.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1445 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/postgres/query_builder.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.322389 citrusdb-0.4.0/citrusdb/db/sqlite/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/db/sqlite/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     3101 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/sqlite/db.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1472 2023-06-15 19:08:11.000000 citrusdb-0.4.0/citrusdb/db/sqlite/queries.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1369 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/db/sqlite/query_builder.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.322616 citrusdb-0.4.0/citrusdb/embedding/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.4.0/citrusdb/embedding/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.4.0/citrusdb/embedding/openai.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.322952 citrusdb-0.4.0/citrusdb/utils/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/utils/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      205 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/utils/types.py
--rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-12 11:56:56.000000 citrusdb-0.4.0/citrusdb/utils/utils.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.320819 citrusdb-0.4.0/citrusdb.egg-info/
--rw-r--r--   0 debabrata   (501) staff       (20)     2341 2023-06-15 19:17:20.000000 citrusdb-0.4.0/citrusdb.egg-info/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      770 2023-06-15 19:17:20.000000 citrusdb-0.4.0/citrusdb.egg-info/SOURCES.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-15 19:17:20.000000 citrusdb-0.4.0/citrusdb.egg-info/dependency_links.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       79 2023-06-15 19:17:20.000000 citrusdb-0.4.0/citrusdb.egg-info/requires.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-06-15 19:17:20.000000 citrusdb-0.4.0/citrusdb.egg-info/top_level.txt
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-15 19:17:20.323173 citrusdb-0.4.0/cloud-temp/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.4.0/cloud-temp/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2065 2023-06-02 09:23:04.000000 citrusdb-0.4.0/cloud-temp/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)      724 2023-06-15 19:16:46.000000 citrusdb-0.4.0/pyproject.toml
--rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-15 19:17:20.323501 citrusdb-0.4.0/setup.cfg
--rw-r--r--   0 debabrata   (501) staff       (20)      964 2023-06-15 19:14:39.000000 citrusdb-0.4.0/setup.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.197616 citrusdb-0.5.0/
+-rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.5.0/LICENSE
+-rw-r--r--   0 debabrata   (501) staff       (20)     2411 2023-06-24 14:36:20.197492 citrusdb-0.5.0/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)     1828 2023-06-19 14:22:45.000000 citrusdb-0.5.0/README.md
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.193707 citrusdb-0.5.0/citrusdb/
+-rw-r--r--   0 debabrata   (501) staff       (20)      281 2023-06-16 18:28:46.000000 citrusdb-0.5.0/citrusdb/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.194869 citrusdb-0.5.0/citrusdb/api/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.0/citrusdb/api/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     4017 2023-06-19 15:43:59.000000 citrusdb-0.5.0/citrusdb/api/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     6915 2023-06-24 14:09:55.000000 citrusdb-0.5.0/citrusdb/api/local.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.195028 citrusdb-0.5.0/citrusdb/db/
+-rw-r--r--   0 debabrata   (501) staff       (20)     1252 2023-06-19 18:42:45.000000 citrusdb-0.5.0/citrusdb/db/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.195276 citrusdb-0.5.0/citrusdb/db/index/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.0/citrusdb/db/index/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-12 11:56:56.000000 citrusdb-0.5.0/citrusdb/db/index/hnswlib.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.195695 citrusdb-0.5.0/citrusdb/db/postgres/
+-rw-r--r--   0 debabrata   (501) staff       (20)     5421 2023-06-24 11:27:51.000000 citrusdb-0.5.0/citrusdb/db/postgres/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1722 2023-06-24 12:19:41.000000 citrusdb-0.5.0/citrusdb/db/postgres/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1533 2023-06-19 15:14:26.000000 citrusdb-0.5.0/citrusdb/db/postgres/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.196243 citrusdb-0.5.0/citrusdb/db/sqlite/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.0/citrusdb/db/sqlite/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     4116 2023-06-24 14:15:18.000000 citrusdb-0.5.0/citrusdb/db/sqlite/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1708 2023-06-24 13:50:46.000000 citrusdb-0.5.0/citrusdb/db/sqlite/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1382 2023-06-19 15:10:21.000000 citrusdb-0.5.0/citrusdb/db/sqlite/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.196529 citrusdb-0.5.0/citrusdb/embedding/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.0/citrusdb/embedding/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.5.0/citrusdb/embedding/openai.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.196930 citrusdb-0.5.0/citrusdb/utils/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.0/citrusdb/utils/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      236 2023-06-19 15:39:24.000000 citrusdb-0.5.0/citrusdb/utils/types.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-12 11:56:56.000000 citrusdb-0.5.0/citrusdb/utils/utils.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.194439 citrusdb-0.5.0/citrusdb.egg-info/
+-rw-r--r--   0 debabrata   (501) staff       (20)     2411 2023-06-24 14:36:20.000000 citrusdb-0.5.0/citrusdb.egg-info/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      792 2023-06-24 14:36:20.000000 citrusdb-0.5.0/citrusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-24 14:36:20.000000 citrusdb-0.5.0/citrusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       79 2023-06-24 14:36:20.000000 citrusdb-0.5.0/citrusdb.egg-info/requires.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-06-24 14:36:20.000000 citrusdb-0.5.0/citrusdb.egg-info/top_level.txt
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.197309 citrusdb-0.5.0/cloud-temp/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.5.0/cloud-temp/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2248 2023-06-16 13:03:05.000000 citrusdb-0.5.0/cloud-temp/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2826 2023-06-16 18:18:23.000000 citrusdb-0.5.0/cloud-temp/main-pg.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      724 2023-06-24 14:34:53.000000 citrusdb-0.5.0/pyproject.toml
+-rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-24 14:36:20.197646 citrusdb-0.5.0/setup.cfg
+-rw-r--r--   0 debabrata   (501) staff       (20)      964 2023-06-24 14:35:05.000000 citrusdb-0.5.0/setup.py
```

### Comparing `citrusdb-0.4.0/LICENSE` & `citrusdb-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `citrusdb-0.4.0/PKG-INFO` & `citrusdb-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.4.0
+Version: 0.5.0
 Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -70,7 +70,9 @@
 Go launch a repl on [Replit](https://replit.com) and see what result you get after running the query! `result` will contain the `ids` of the top `k` search hits.
 
 ## Example
 [pokedex search](https://replit.com/@debabratajr/pokedex-search)
 
 ## Facing issues?
 Feel free to open issues on this repository! Discord server coming soon!
+
+PS: citrus isn't distributed just yet. We're getting there though ;)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.4.0 Summary: open-source vector
+Metadata-Version: 2.1 Name: citrusdb Version: 0.5.0 Summary: open-source vector
 database. store and retrieve embeddings for your next project! Home-page:
 https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
 Debabrata Mondal
 js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
@@ -25,8 +25,9 @@
 environment. By default we use OpenAI to to generate the embeddings. Please
 reach out if you're looking for support from a different provider! #### 3.
 Search ```py result, distances = citrus.query(index="example", documents=["What
 is it like to launch a startup"], k=1) ``` Go launch a repl on [Replit](https:/
 /replit.com) and see what result you get after running the query! `result` will
 contain the `ids` of the top `k` search hits. ## Example [pokedex search]
 (https://replit.com/@debabratajr/pokedex-search) ## Facing issues? Feel free to
-open issues on this repository! Discord server coming soon!
+open issues on this repository! Discord server coming soon! PS: citrus isn't
+distributed just yet. We're getting there though ;)
```

### Comparing `citrusdb-0.4.0/README.md` & `citrusdb-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,7 +55,9 @@
 Go launch a repl on [Replit](https://replit.com) and see what result you get after running the query! `result` will contain the `ids` of the top `k` search hits.
 
 ## Example
 [pokedex search](https://replit.com/@debabratajr/pokedex-search)
 
 ## Facing issues?
 Feel free to open issues on this repository! Discord server coming soon!
+
+PS: citrus isn't distributed just yet. We're getting there though ;)
```

#### html2text {}

```diff
@@ -16,8 +16,9 @@
 environment. By default we use OpenAI to to generate the embeddings. Please
 reach out if you're looking for support from a different provider! #### 3.
 Search ```py result, distances = citrus.query(index="example", documents=["What
 is it like to launch a startup"], k=1) ``` Go launch a repl on [Replit](https:/
 /replit.com) and see what result you get after running the query! `result` will
 contain the `ids` of the top `k` search hits. ## Example [pokedex search]
 (https://replit.com/@debabratajr/pokedex-search) ## Facing issues? Feel free to
-open issues on this repository! Discord server coming soon!
+open issues on this repository! Discord server coming soon! PS: citrus isn't
+distributed just yet. We're getting there though ;)
```

### Comparing `citrusdb-0.4.0/citrusdb/api/index.py` & `citrusdb-0.5.0/citrusdb/api/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import pickle
 from typing import Any, List, Optional
 from numpy import float32
 from numpy._typing import NDArray
 from citrusdb.db.index.hnswlib import HnswIndex
+from citrusdb.utils.types import IDs
 from citrusdb.utils.utils import ensure_valid_path
 
 
 class Index:
     _db: HnswIndex
     _parameters: dict
 
@@ -57,15 +58,15 @@
                 M=M,
                 ef_construction=ef_construction,
                 allow_replace_deleted=allow_replace_deleted,
             )
 
     def add(
         self,
-        ids,
+        ids: List[int],
         embeddings: Optional[NDArray[float32]],
         replace_deleted: bool,
     ):
         self._db.add_items(embeddings, ids, replace_deleted)
         if self._parameters["persist_directory"]:
             self._save()
```

### Comparing `citrusdb-0.4.0/citrusdb/api/local.py` & `citrusdb-0.5.0/citrusdb/api/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from numpy._typing import NDArray
 import shutil
 
 from citrusdb.api.index import Index
 from citrusdb.db import BaseDB
 from citrusdb.db.postgres.db import PostgresDB
 from citrusdb.db.sqlite.db import SQLiteDB
+from citrusdb.utils.types import IDs
 
 
 class LocalAPI:
     _db: Dict[str, Index] 
     _SQLClient: BaseDB
     persist_directory: Optional[str]
     _TEMP_DIRECTORY = "citrus_temp"
@@ -60,21 +61,22 @@
             ef_construction=ef_construction,
             allow_replace_deleted=allow_replace_deleted
         )
 
     def add(
         self,
         index: str,
-        ids,
+        ids: IDs,
         documents: Optional[List[str]] = None,
         embeddings: Optional[NDArray[float32]] = None,
         metadatas: Optional[List[Dict]] = None
     ):
         """
         Insert embeddings/text documents
+
         index: Name of index
         ids: Unique ID for each element
         documents: List of strings to index
         embeddings: List of embeddings to index
         metadatas: Additional metadata for each vector
         """
 
@@ -114,48 +116,47 @@
                     index_id,
                     None if documents is None else documents[i],
                     json.dumps(embeddings[i].tolist()),
                     None if metadatas is None else json.dumps(metadatas[i])
                 )
                 data.append(row + row)
 
-            # Insert data into sqlite
-            self._SQLClient.insert_to_index(data)
+            # Insert data into DB
+            hnsw_labels = self._SQLClient.insert_to_index(data)
 
             # Index vectors
             self._db[index].add(
-                ids=ids,
+                ids=hnsw_labels,
                 embeddings=embeddings,
                 replace_deleted=replace_deleted
             )
 
     def delete_vectors(
         self,
         index: str,
-        ids: List[int],
+        ids: IDs
     ):
         index_details = self._SQLClient.get_index_details(index)
         if index_details is None:
             raise ValueError(f"Could not find index: {index}")
 
         index_id = index_details[0]
-        self._SQLClient.delete_vectors_from_index(
+        hnsw_labels = self._SQLClient.delete_vectors_from_index(
             index_id=index_id,
             ids=ids
         )
 
-        self._db[index].delete_vectors(ids)
+        self._db[index].delete_vectors(hnsw_labels)
 
     def reload_indices(self):
         """
         Load all indices from disk to memory
         """
 
         indices = self._SQLClient.get_indices()
-        print("Indices: ", indices)
         for index in indices:
             index_name = index[1]
             # Load index
             self.create_index(
                 name=index_name,
                 max_elements=index[3],
                 M=index[4],
@@ -187,20 +188,25 @@
 
         filter_function = lambda label: label in allowed_ids
 
         flag = 1
         for key in self._db.keys():
             if key == index:
                 flag = 0
-                return self._db[key].query(
+                results, distances = self._db[key].query(
                     documents=documents,
                     query_embeddings=query_embeddings,
                     k=k,
                     filter_function=None if filters is None else filter_function
                 )
+                lolo_vector_ids = self._SQLClient.get_vector_ids_of_results(
+                    name=index,
+                    results=results
+                )
+                return lolo_vector_ids, distances
 
         if flag:
             raise ValueError(f"Could not find index: {index}")
 
 
     def get_status(self, index: str):
         flag = 1
```

### Comparing `citrusdb-0.4.0/citrusdb/db/__init__.py` & `citrusdb-0.5.0/citrusdb/db/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Tuple, Optional
 
+from citrusdb.utils.types import IDs
+
 
 class BaseDB(ABC):
     @abstractmethod
     def create_index(
         self,
         name: str,
         max_elements: int,
@@ -15,16 +17,16 @@
     ):
         pass
 
     @abstractmethod
     def delete_vectors_from_index(
         self,
         index_id: int,
-        ids: List[int]
-    ):
+        ids: IDs
+    ) -> List[int]:
         pass
 
     @abstractmethod
     def filter_vectors(self, index_name: str, filters: List[Dict]) -> List:
         pass
 
     @abstractmethod
@@ -35,18 +37,26 @@
     def get_index_details(
         self,
         name: str
     ) -> Optional[Tuple[int, str, int, int, int, int, int, bool]]:
         pass
 
     @abstractmethod
+    def get_vector_ids_of_results(
+        self,
+        name: str,
+        results: List[List[int]]
+    ) -> List[IDs]:
+        pass
+
+    @abstractmethod
     def insert_to_index(
         self,
         data
-    ):
+    ) -> List[int]:
         pass
 
     @abstractmethod
     def update_ef(
         self,
         name: str,
         ef: int
```

### Comparing `citrusdb-0.4.0/citrusdb/db/index/hnswlib.py` & `citrusdb-0.5.0/citrusdb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.4.0/citrusdb/db/postgres/db.py` & `citrusdb-0.5.0/citrusdb/db/sqlite/db.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,148 @@
-from psycopg_pool import ConnectionPool
-from typing import Any, Dict, List, Optional, Tuple
+import os
+import sqlite3
+from typing import Dict, List, Optional, Tuple
+
 from citrusdb.db import BaseDB
-import citrusdb.db.postgres.queries as queries
-from citrusdb.db.postgres.query_builder import QueryBuilder
+from citrusdb.utils.types import IDs
+from citrusdb.utils.utils import ensure_valid_path
+import citrusdb.db.sqlite.queries as queries
+from citrusdb.db.sqlite.query_builder import QueryBuilder
 
 
-class PostgresDB(BaseDB):
-    _pool: ConnectionPool
+class SQLiteDB(BaseDB):
+    _con: sqlite3.Connection
 
     def __init__(
         self,
-        **kwargs: Dict[str, Any]
+        persist_directory: str,
     ):
-        # Setup connection pool
-        self._pool = ConnectionPool(kwargs=kwargs)
+        ensure_valid_path(persist_directory)
 
-        # Create index_manager and index_data table if they don't exist already
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(queries.CREATE_INDEX_MANAGER_TABLE)
-                cur.execute(queries.CREATE_INDEX_DATA_TABLE)
-                conn.commit()
+        self._con = sqlite3.connect(
+            os.path.join(
+                persist_directory, "citrus.db"
+            )
+        )
+
+        cur = self._con.cursor()
+        cur.execute("PRAGMA foreign_keys = ON")    # Enable foreign keys
+        cur.executescript(f'''
+        BEGIN;
+        {queries.CREATE_INDEX_MANAGER_TABLE}
+        {queries.CREATE_INDEX_DATA_TABLE}
+        END;
+        ''')
+        cur.close()
 
     def create_index(
         self,
         name: str,
         max_elements: int,
         M: int,
         ef_construction: int,
         allow_replace_deleted: bool,
         dimensions: Optional[int] = 1536,
     ):
+        cur = self._con.cursor()
         ef = ef_construction
         parameters = (name, dimensions, max_elements, M, ef, ef_construction, allow_replace_deleted)
-        # Create new index entry to postgres db
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(queries.INSERT_INDEX_TO_MANAGER, parameters)
-                conn.commit()
+        cur.execute(queries.INSERT_INDEX_TO_MANAGER, parameters)
+        self._con.commit()
+        cur.close()
 
     def delete_vectors_from_index(
         self,
         index_id: int,
-        ids: List[int]
+        ids: IDs
     ):
-        """
-        Delete vectors with given list of IDs from specific index
+        cur = self._con.cursor()
+        query = queries.DELETE_VECTORS_FROM_INDEX.format(", ".join("?" * len(ids)))
+        parameters = tuple(ids) + (index_id,)
+        cur.execute(query, parameters)
+
+        rows = cur.fetchall()
+        self._con.commit()
+        cur.close()
 
-        index_id: ID of index where the elements belong
-        ids: List of IDs to be deleted
-        """
-        parameters = (tuple(ids), index_id)
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(queries.DELETE_VECTORS_FROM_INDEX, parameters)
-                conn.commit()
+        vector_ids = [row[0] for row in rows]
+        return vector_ids
 
     def filter_vectors(self, index_name: str, filters: List[Dict]):
-        """
-        Get list of IDs of vectors that match filters.
-
-        index_name: Name of index where the elements belong
-        filters: List of filters to be applied
-        """
-        with self._pool.connection() as conn:
-            query_builder = QueryBuilder(conn)
-            res = query_builder.execute_query(index_name, filters)
-            allowed_ids = []
-            for row in res:
-                allowed_ids.append(row[0])
-            return allowed_ids
+        query_builder = QueryBuilder(self._con)
+        res = query_builder.execute_query(index_name, filters)
+        allowed_ids = []
+        for row in res:
+            allowed_ids.append(row[0])
+        return allowed_ids
 
     def get_indices(self):
         """
-        Get all index details
+        Fetch all index details from index_manager table.
+        Returns a list of tuples where each one corresponds to an index.
         """
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(queries.GET_ALL_INDEX_DETAILS)
-                return cur.fetchall()
+
+        cur = self._con.cursor()
+        res = cur.execute(queries.GET_ALL_INDEX_DETAILS)
+        rows = res.fetchall()
+        cur.close()
+        return rows
 
     def get_index_details(
         self,
         name: str
     ) -> Optional[Tuple[int, str, int, int, int, int, int, bool]]:
-        """
-        Get specific index details
-
-        name: Name of index to fetch
-        """
+        cur = self._con.cursor()
         parameters = (name,)
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(queries.GET_INDEX_DETAILS_BY_NAME, parameters)
-                return cur.fetchone()
+        res = cur.execute(queries.GET_INDEX_DETAILS_BY_NAME, parameters)
+        row = res.fetchone()
+        cur.close()
+        return row
+
+    def get_vector_ids_of_results(
+        self,
+        name: str,
+        results: List[List[int]]
+    ) -> List[IDs]:
+        lolo_vector_ids = []
+        index_details = self.get_index_details(name)
+        index_id = index_details[0]               # type: ignore
+
+        cur = self._con.cursor()
+        for ids in results:
+            query = queries.GET_VECTOR_IDS_OF_RESULTS.format(", ".join("?" * len(ids)))
+            parameters = ()
+            for id in ids:
+                parameters += (int(id),)
+            parameters += (index_id,)
+            res = cur.execute(query, parameters)
+            rows = res.fetchall()
+            lolo_vector_ids.append([row[0] for row in rows])
+        cur.close()
+
+        return lolo_vector_ids
 
     def insert_to_index(
         self,
         data
     ):
-        """
-        Insert vectors to index
+        cur = self._con.cursor()
+        vector_ids = []
+        for row in data:
+            res = cur.execute(queries.INSERT_DATA_TO_INDEX, row)
+            vector_ids.append(res.fetchone()[0])
 
-        data: Tuple of tuples corresponding to each row
-        """
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.executemany(queries.INSERT_DATA_TO_INDEX, data)
-                conn.commit()
+        self._con.commit()
+        cur.close()
+
+        return vector_ids
 
     def update_ef(
         self,
         name: str,
         ef: int
     ):
-        """
-        Update ef for an index
-
-        name: Name of index to be updated
-        ef: New ef value
-        """
+        cur = self._con.cursor()
         parameters = (ef, name)
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(queries.UPDATE_EF, parameters)
-                conn.commit()
+        cur.execute(queries.UPDATE_EF, parameters)
+        self._con.commit()
+        cur.close()
```

### Comparing `citrusdb-0.4.0/citrusdb/db/postgres/queries.py` & `citrusdb-0.5.0/citrusdb/db/postgres/queries.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,45 +9,55 @@
     ef_construction INTEGER NOT NULL,
     allow_replace_deleted BOOLEAN NOT NULL
 );
 '''
 
 CREATE_INDEX_DATA_TABLE = '''
 CREATE TABLE IF NOT EXISTS index_data (
-    id BIGINT,
+    vector_id BIGINT PRIMARY KEY GENERATED ALWAYS AS IDENTITY,
+    id text NOT NULL,
     index_id BIGINT,
     text TEXT,
     embedding JSONB NOT NULL,
     metadata JSONB,
-    PRIMARY KEY(id, index_id),
+    UNIQUE(id, index_id),
     FOREIGN KEY(index_id) REFERENCES index_manager(index_id) ON DELETE CASCADE
 );
 '''
 
 DELETE_VECTORS_FROM_INDEX = '''
 DELETE FROM index_data
 WHERE id IN %s AND index_id = %s
+RETURNING vector_id
 '''
 
 GET_ALL_INDEX_DETAILS = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
 FROM index_manager
 '''
 
 GET_INDEX_DETAILS_BY_NAME = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
 FROM index_manager
 WHERE name = %s
 '''
 
+GET_VECTOR_IDS_OF_RESULTS = '''
+SELECT id
+FROM index_data
+WHERE id IN %s AND index_id = %s
+'''
+
 INSERT_DATA_TO_INDEX = '''
 INSERT INTO index_data
+(id, index_id, text, embedding, metadata)
 VALUES(%s, %s, %s, %s, %s)
 ON CONFLICT(id, index_id)
 DO UPDATE SET id = %s, index_id = %s, text = %s, embedding = %s, metadata = %s
+RETURNING vector_id
 '''
 
 INSERT_INDEX_TO_MANAGER = '''
 INSERT INTO index_manager
 (name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted)
 VALUES (%s, %s, %s, %s, %s, %s, %s);
 '''
```

### Comparing `citrusdb-0.4.0/citrusdb/db/postgres/query_builder.py` & `citrusdb-0.5.0/citrusdb/db/postgres/query_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,30 @@
     _con: Connection
 
     def __init__(self, connection):
         self._con = connection
 
     def build_query(self, filters):
         # Building the base SQL query
-        sql_query = f"SELECT d.id, d.index_id, d.text FROM index_data d JOIN index_manager m ON m.index_id = d.index_id WHERE m.name = %s"
+        sql_query = f"SELECT d.vector_id, d.id, d.index_id, d.text FROM index_data d JOIN index_manager m ON m.index_id = d.index_id WHERE m.name = %s"
 
         # Adding the filter criteria to the SQL query
         if filters:
             sql_query += " AND "
             conditions = []
             for filter in filters:
                 field = filter["field"]
                 operator = filter["operator"]
                 value = filter["value"]
-                if isinstance(value, int) or isinstance(value, float):
-                    # ->> returns text in postgres
-                    condition = f"metadata ->> '{field}' {operator} '{value}'"
-                else:
-                    condition = f"metadata ->> '{field}' {operator} '{value}'"
+                # ->> returns text in postgres
+                #if isinstance(value, int) or isinstance(value, float):
+                #    condition = f"metadata ->> '{field}' {operator} '{value}'"
+                #else:
+                #    condition = f"metadata ->> '{field}' {operator} '{value}'"
+                condition = f"metadata ->> '{field}' {operator} '{value}'"
                 conditions.append(condition)
             sql_query += " AND ".join(conditions)
 
         return sql.SQL(sql_query)
 
     def execute_query(self, index_name: str, filters: List[Dict]):
         with self._con.cursor() as cur:
```

### Comparing `citrusdb-0.4.0/citrusdb/db/sqlite/queries.py` & `citrusdb-0.5.0/citrusdb/db/sqlite/queries.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,45 +9,55 @@
     ef_construction INTEGER NOT NULL,
     allow_replace_deleted INTEGER NOT NULL
 );
 '''
 
 CREATE_INDEX_DATA_TABLE = '''
 CREATE TABLE IF NOT EXISTS index_data (
-    id INTEGER,
+    vector_id INTEGER PRIMARY KEY AUTOINCREMENT,
+    id TEXT NOT NULL,
     index_id INTEGER,
     text TEXT,
     embedding BLOB NOT NULL,
     metadata TEXT,
-    PRIMARY KEY(id, index_id),
+    UNIQUE(id, index_id),
     FOREIGN KEY(index_id) REFERENCES index_manager(index_id) ON DELETE CASCADE
 );
 '''
 
 DELETE_VECTORS_FROM_INDEX = '''
 DELETE FROM index_data
 WHERE id IN ({}) AND index_id = ?
+RETURNING vector_id
 '''
 
 GET_ALL_INDEX_DETAILS = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
 FROM index_manager
 '''
 
 GET_INDEX_DETAILS_BY_NAME = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
 FROM index_manager
 WHERE name = ?
 '''
 
+GET_VECTOR_IDS_OF_RESULTS = '''
+SELECT id
+FROM index_data
+WHERE vector_id IN ({}) AND index_id = ?
+'''
+
 INSERT_DATA_TO_INDEX = '''
 INSERT INTO index_data
+(id, index_id, text, embedding, metadata)
 VALUES(?, ?, ?, ?, ?)
 ON CONFLICT(id, index_id)
 DO UPDATE SET id = ?, index_id = ?, text = ?, embedding = ?, metadata = ?
+RETURNING vector_id
 '''
 
 INSERT_INDEX_TO_MANAGER = '''
 INSERT INTO index_manager
 (name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted)
 VALUES (?, ?, ?, ?, ?, ?, ?);
 '''
```

### Comparing `citrusdb-0.4.0/citrusdb/db/sqlite/query_builder.py` & `citrusdb-0.5.0/citrusdb/db/sqlite/query_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     _con: sqlite3.Connection
 
     def __init__(self, connection):
         self._con = connection
 
     def build_query(self, index_name, filters):
         # Building the base SQL query
-        sql_query = f"SELECT d.id, d.index_id, d.text FROM index_data d JOIN index_manager m ON m.index_id = d.index_id WHERE m.name = '{index_name}'"
+        sql_query = f"SELECT d.vector_id, d.id, d.index_id, d.text FROM index_data d JOIN index_manager m ON m.index_id = d.index_id WHERE m.name = '{index_name}'"
 
         # Adding the filter criteria to the SQL query
         if filters:
             sql_query += " AND "
             conditions = []
             for filter in filters:
                 field = filter["field"]
```

### Comparing `citrusdb-0.4.0/citrusdb/utils/utils.py` & `citrusdb-0.5.0/citrusdb/utils/utils.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.4.0/citrusdb.egg-info/PKG-INFO` & `citrusdb-0.5.0/citrusdb.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.4.0
+Version: 0.5.0
 Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -70,7 +70,9 @@
 Go launch a repl on [Replit](https://replit.com) and see what result you get after running the query! `result` will contain the `ids` of the top `k` search hits.
 
 ## Example
 [pokedex search](https://replit.com/@debabratajr/pokedex-search)
 
 ## Facing issues?
 Feel free to open issues on this repository! Discord server coming soon!
+
+PS: citrus isn't distributed just yet. We're getting there though ;)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.4.0 Summary: open-source vector
+Metadata-Version: 2.1 Name: citrusdb Version: 0.5.0 Summary: open-source vector
 database. store and retrieve embeddings for your next project! Home-page:
 https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
 Debabrata Mondal
 js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
@@ -25,8 +25,9 @@
 environment. By default we use OpenAI to to generate the embeddings. Please
 reach out if you're looking for support from a different provider! #### 3.
 Search ```py result, distances = citrus.query(index="example", documents=["What
 is it like to launch a startup"], k=1) ``` Go launch a repl on [Replit](https:/
 /replit.com) and see what result you get after running the query! `result` will
 contain the `ids` of the top `k` search hits. ## Example [pokedex search]
 (https://replit.com/@debabratajr/pokedex-search) ## Facing issues? Feel free to
-open issues on this repository! Discord server coming soon!
+open issues on this repository! Discord server coming soon! PS: citrus isn't
+distributed just yet. We're getting there though ;)
```

### Comparing `citrusdb-0.4.0/citrusdb.egg-info/SOURCES.txt` & `citrusdb-0.5.0/citrusdb.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 citrusdb/db/sqlite/query_builder.py
 citrusdb/embedding/__init__.py
 citrusdb/embedding/openai.py
 citrusdb/utils/__init__.py
 citrusdb/utils/types.py
 citrusdb/utils/utils.py
 cloud-temp/__init__.py
-cloud-temp/index.py
+cloud-temp/index.py
+cloud-temp/main-pg.py
```

### Comparing `citrusdb-0.4.0/cloud-temp/index.py` & `citrusdb-0.5.0/cloud-temp/index.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-from typing import Dict, List
 import numpy as np
 from fastapi import FastAPI
 from fastapi.responses import JSONResponse
-from numpy._typing import NDArray
 from citrusdb import Client
 
 app = FastAPI()
 client = Client(persist_directory="citrus")
 
 @app.post("/index")
 def create_index(index_name: str, max_elements: int = 1000, allow_replace_deleted: bool = True, M = 64, ef_construction = 200):
     try:
         client.create_index(
             name=index_name,
-            max_elements=max_elements,
+            max_elements=int(max_elements),
             allow_replace_deleted=allow_replace_deleted,
-            M=M,
-            ef_construction=ef_construction
+            M=int(M),
+            ef_construction=int(ef_construction)
         )
         return {"message": f"Index '{index_name}' created successfully."}
     except Exception as error:
         return JSONResponse(status_code=500, content=error)
 
 @app.post("/insert")
 def insert_elements(index_name: str, elements: list[dict]):
     try:
+        embeddings = None
+        texts = None
         ids = [element["id"] for element in elements]
-        embeddings = np.asarray([element["embedding"] for element in elements], np.float32)
+
+        keys = elements[0].keys()
+        if "embedding" in keys:
+            embeddings = np.asarray([element["embedding"] for element in elements], np.float32)
+        if "text" in keys:
+            texts = [element["text"] for element in elements]
+
         metadatas = [element["metadata"] for element in elements]
 
-        client.add(index=index_name, ids=ids, embeddings=embeddings, metadatas=metadatas)
+        client.add(index=index_name, ids=ids, embeddings=embeddings, documents=texts, metadatas=metadatas)
         return {"message": f"{len(ids)} vectors indexed."}
     except Exception as error:
         return JSONResponse(status_code=500, content=error)
 
 @app.get("/search")
 def semantic_search(index_name: str, search: dict, k: int = 1):
     try:
@@ -45,10 +51,11 @@
                 for j, id in result:
                     obj = {"id": id, "similarity_score": 1 - distances[i][j]}
                     response.append(obj)  # Assuming documents is accessible here
             return {"results": response}
     except Exception as error:
         return JSONResponse(status_code=500, content=error)
 
+'''
 if __name__ == "__main__":
     uvicorn.run(app, host="0.0.0.0", port=8000)
-
+'''
```

### Comparing `citrusdb-0.4.0/pyproject.toml` & `citrusdb-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "citrusdb"
-version = "0.4.0"
+version = "0.5.0"
 
 authors = [
   { name="Debabrata Mondal", email="debabrata.js@protonmail.com" },
 ]
 description = "open-source vector database. store and retrieve embeddings for your next project!"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `citrusdb-0.4.0/setup.py` & `citrusdb-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="citrusdb",
-    version="0.4.0",
+    version="0.5.0",
     author="Debabrata Mondal",
     author_email="debabrata.js@protonmail.com",
     description="(distributed) vector database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0xDebabrata/citrus",
     packages=(
```

