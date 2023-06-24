# Comparing `tmp/fastapi-elasticsearch-0.6.0.tar.gz` & `tmp/fastapi-elasticsearch-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-elasticsearch-0.6.0.tar", last modified: Fri Jun  9 21:06:50 2023, max compression
+gzip compressed data, was "fastapi-elasticsearch-0.7.0.tar", last modified: Sat Jun 24 17:03:46 2023, max compression
```

## Comparing `fastapi-elasticsearch-0.6.0.tar` & `fastapi-elasticsearch-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 21:06:50.123850 fastapi-elasticsearch-0.6.0/
--rw-r--r--   0 root         (0) root         (0)     9000 2023-06-09 21:06:50.123850 fastapi-elasticsearch-0.6.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 21:06:50.123850 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch/
--rw-r--r--   0 root         (0) root         (0)       91 2023-06-09 19:32:59.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8567 2023-06-08 14:19:14.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch/api.py
--rw-r--r--   0 root         (0) root         (0)      721 2021-04-03 18:13:19.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 21:06:50.123850 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9000 2023-06-09 21:06:50.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-09 21:06:50.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 21:06:50.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-09 21:06:50.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 21:06:50.000000 fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 21:06:50.123850 fastapi-elasticsearch-0.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      582 2023-06-09 21:06:32.000000 fastapi-elasticsearch-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:03:46.190751 fastapi-elasticsearch-0.7.0/
+-rw-r--r--   0 root         (0) root         (0)     9536 2023-06-24 17:03:46.190751 fastapi-elasticsearch-0.7.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:03:46.190751 fastapi-elasticsearch-0.7.0/fastapi_elasticsearch/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-06-24 15:51:04.000000 fastapi-elasticsearch-0.7.0/fastapi_elasticsearch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8567 2023-06-08 14:19:14.000000 fastapi-elasticsearch-0.7.0/fastapi_elasticsearch/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 17:03:46.190751 fastapi-elasticsearch-0.7.0/fastapi_elasticsearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9536 2023-06-24 17:03:46.000000 fastapi-elasticsearch-0.7.0/fastapi_elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-24 17:03:46.000000 fastapi-elasticsearch-0.7.0/fastapi_elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 17:03:46.000000 fastapi-elasticsearch-0.7.0/fastapi_elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-24 17:03:46.000000 fastapi-elasticsearch-0.7.0/fastapi_elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-24 17:03:46.000000 fastapi-elasticsearch-0.7.0/fastapi_elasticsearch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 17:03:46.190751 fastapi-elasticsearch-0.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-24 16:57:29.000000 fastapi-elasticsearch-0.7.0/setup.py
```

### Comparing `fastapi-elasticsearch-0.6.0/PKG-INFO` & `fastapi-elasticsearch-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fastapi-elasticsearch
-Version: 0.6.0
+Version: 0.7.0
 Summary: Query Utility for Elasticsearch
 Home-page: https://github.com/euler-io/fastapi-elasticsearch
 License: LGPL-2.1 License
 Description-Content-Type: text/markdown
 
-# Query Helper for Elasticsearch
+# Query Helper for Elasticsearch or OpenSearch
 
 [![Pypi](https://img.shields.io/pypi/v/fastapi-elasticsearch.svg)](https://pypi.org/project/fastapi-elasticsearch/)
 
-This is a helper library for creating elasticsearch query proxies using [FastAPI](https://fastapi.tiangolo.com/).
+This is a helper library for creating elasticsearch or opensearch query proxies using [FastAPI](https://fastapi.tiangolo.com/).
 
 ```python
 
 from fastapi_elasticsearch import ElasticsearchAPIQueryBuilder
 
 # Create a new query_builder for the endpoint.
 query_builder = ElasticsearchAPIQueryBuilder()
@@ -62,14 +62,37 @@
     }
   },
   "size": 10,
   "from": 0
 }
 ```
 
+To use OpenSearch, simply change the client.
+
+```python
+from fastapi_elasticsearch import ElasticsearchAPIQueryBuilder
+from opensearchpy import OpenSearch
+
+...
+
+@app.get("/search")
+async def search(
+        os: OpenSearch = Depends(get_opensearch),
+        query_body: Dict = Depends(query_builder.build())) -> JSONResponse:
+    return os.search(
+        body=query_body,
+        index=index_name
+    )
+...
+
+# Create a new query_builder for the endpoint.
+query_builder = ElasticsearchAPIQueryBuilder()
+
+```
+
 To control the scoring use a matcher.
 
 ```python
 
 # Or decorate a function as a matcher
 # (will contribute to the query scoring).
 # Parameters can also be used.
```

### Comparing `fastapi-elasticsearch-0.6.0/fastapi_elasticsearch/api.py` & `fastapi-elasticsearch-0.7.0/fastapi_elasticsearch/api.py`

 * *Files identical despite different names*

### Comparing `fastapi-elasticsearch-0.6.0/fastapi_elasticsearch.egg-info/PKG-INFO` & `fastapi-elasticsearch-0.7.0/fastapi_elasticsearch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fastapi-elasticsearch
-Version: 0.6.0
+Version: 0.7.0
 Summary: Query Utility for Elasticsearch
 Home-page: https://github.com/euler-io/fastapi-elasticsearch
 License: LGPL-2.1 License
 Description-Content-Type: text/markdown
 
-# Query Helper for Elasticsearch
+# Query Helper for Elasticsearch or OpenSearch
 
 [![Pypi](https://img.shields.io/pypi/v/fastapi-elasticsearch.svg)](https://pypi.org/project/fastapi-elasticsearch/)
 
-This is a helper library for creating elasticsearch query proxies using [FastAPI](https://fastapi.tiangolo.com/).
+This is a helper library for creating elasticsearch or opensearch query proxies using [FastAPI](https://fastapi.tiangolo.com/).
 
 ```python
 
 from fastapi_elasticsearch import ElasticsearchAPIQueryBuilder
 
 # Create a new query_builder for the endpoint.
 query_builder = ElasticsearchAPIQueryBuilder()
@@ -62,14 +62,37 @@
     }
   },
   "size": 10,
   "from": 0
 }
 ```
 
+To use OpenSearch, simply change the client.
+
+```python
+from fastapi_elasticsearch import ElasticsearchAPIQueryBuilder
+from opensearchpy import OpenSearch
+
+...
+
+@app.get("/search")
+async def search(
+        os: OpenSearch = Depends(get_opensearch),
+        query_body: Dict = Depends(query_builder.build())) -> JSONResponse:
+    return os.search(
+        body=query_body,
+        index=index_name
+    )
+...
+
+# Create a new query_builder for the endpoint.
+query_builder = ElasticsearchAPIQueryBuilder()
+
+```
+
 To control the scoring use a matcher.
 
 ```python
 
 # Or decorate a function as a matcher
 # (will contribute to the query scoring).
 # Parameters can also be used.
```

