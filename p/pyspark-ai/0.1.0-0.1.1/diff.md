# Comparing `tmp/pyspark_ai-0.1.0.tar.gz` & `tmp/pyspark_ai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_ai-0.1.0.tar", max compression
+gzip compressed data, was "pyspark_ai-0.1.1.tar", max compression
```

## Comparing `pyspark_ai-0.1.0.tar` & `pyspark_ai-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.0/LICENSE
--rw-r--r--   0        0        0     3397 2023-06-23 22:14:14.463218 pyspark_ai-0.1.0/README.md
--rw-r--r--   0        0        0      978 2023-06-23 22:14:18.319337 pyspark_ai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.0/pyspark_ai/__init__.py
--rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.0/pyspark_ai/ai_utils.py
--rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.0/pyspark_ai/cache.py
--rw-r--r--   0        0        0     1905 2023-06-23 22:14:14.485144 pyspark_ai-0.1.0/pyspark_ai/code_logger.py
--rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.0/pyspark_ai/file_cache.py
--rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.0/pyspark_ai/llm_chain_with_cache.py
--rw-r--r--   0        0        0     8879 2023-06-23 22:14:14.485908 pyspark_ai-0.1.0/pyspark_ai/prompt.py
--rw-r--r--   0        0        0    15377 2023-06-23 23:11:22.993517 pyspark_ai-0.1.0/pyspark_ai/pyspark_ai.py
--rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.0/pyspark_ai/search_tool_with_cache.py
--rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 pyspark_ai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 pyspark_ai-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3397 2023-06-23 22:14:14.463218 pyspark_ai-0.1.1/README.md
+-rw-r--r--   0        0        0      978 2023-06-23 23:50:06.264450 pyspark_ai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-23 22:14:14.484356 pyspark_ai-0.1.1/pyspark_ai/__init__.py
+-rw-r--r--   0        0        0     3945 2023-06-23 22:14:14.484674 pyspark_ai-0.1.1/pyspark_ai/ai_utils.py
+-rw-r--r--   0        0        0     2718 2023-06-23 22:14:14.484982 pyspark_ai-0.1.1/pyspark_ai/cache.py
+-rw-r--r--   0        0        0     1905 2023-06-23 22:14:14.485144 pyspark_ai-0.1.1/pyspark_ai/code_logger.py
+-rw-r--r--   0        0        0     5224 2023-06-23 22:14:14.485334 pyspark_ai-0.1.1/pyspark_ai/file_cache.py
+-rw-r--r--   0        0        0     1233 2023-06-23 22:14:14.485716 pyspark_ai-0.1.1/pyspark_ai/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     8879 2023-06-23 22:14:14.485908 pyspark_ai-0.1.1/pyspark_ai/prompt.py
+-rw-r--r--   0        0        0    15941 2023-06-23 23:49:27.968706 pyspark_ai-0.1.1/pyspark_ai/pyspark_ai.py
+-rw-r--r--   0        0        0      713 2023-06-23 22:14:14.486408 pyspark_ai-0.1.1/pyspark_ai/search_tool_with_cache.py
+-rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 pyspark_ai-0.1.1/PKG-INFO
```

### Comparing `pyspark_ai-0.1.0/LICENSE` & `pyspark_ai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.0/README.md` & `pyspark_ai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.0/pyproject.toml` & `pyspark_ai-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyspark-ai"
-version = "0.1.0"
+version = "0.1.1"
 description = "English SDK for Apache Spark"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/databrickslabs/pyspark-ai"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pyspark_ai-0.1.0/pyspark_ai/ai_utils.py` & `pyspark_ai-0.1.1/pyspark_ai/ai_utils.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.0/pyspark_ai/cache.py` & `pyspark_ai-0.1.1/pyspark_ai/cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.0/pyspark_ai/code_logger.py` & `pyspark_ai-0.1.1/pyspark_ai/code_logger.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.0/pyspark_ai/file_cache.py` & `pyspark_ai-0.1.1/pyspark_ai/file_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.0/pyspark_ai/llm_chain_with_cache.py` & `pyspark_ai-0.1.1/pyspark_ai/llm_chain_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.0/pyspark_ai/prompt.py` & `pyspark_ai-0.1.1/pyspark_ai/prompt.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.0/pyspark_ai/pyspark_ai.py` & `pyspark_ai-0.1.1/pyspark_ai/pyspark_ai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import re
 import pandas as pd  # noqa: F401
 
 from typing import Callable, Optional, List
 from urllib.parse import urlparse
 
 import requests
@@ -40,15 +41,15 @@
     def __init__(
         self,
         llm: BaseLanguageModel = ChatOpenAI(model_name='gpt-4', temperature=0),
         web_search_tool: Optional[Callable[[str], str]] = None,
         spark_session: Optional[SparkSession] = None,
         enable_cache: bool = True,
         cache_file_format: str = "json",
-        cache_file_location: str = "spark_llm_cache.json",
+        cache_file_location: Optional[str] = None,
         encoding: Optional[Encoding] = None,
         max_tokens_of_web_content: int = 3000,
         verbose: bool = False,
     ) -> None:
         """
         Initialize the SparkAI object with the provided parameters.
 
@@ -61,16 +62,26 @@
         :param max_tokens_of_web_content: maximum tokens of web content after encoding
         """
         self._spark = spark_session or SparkSession.builder.getOrCreate()
         self._llm = llm
         self._web_search_tool = web_search_tool or self._default_web_search_tool
         if enable_cache:
             self._enable_cache = enable_cache
+            if cache_file_location is not None:
+                # if there is parameter setting for it, use the parameter
+                self._cache_file_location = cache_file_location
+            elif 'AI_CACHE_FILE_LOCATION' in os.environ:
+                # otherwise read from env variable AI_CACHE_FILE_LOCATION
+                self._cache_file_location = os.environ['AI_CACHE_FILE_LOCATION']
+            else:
+                # use default value "spark_ai_cache.json"
+                self._cache_file_location = "spark_ai_cache.json"
             self._cache = Cache(
-                cache_file_location=cache_file_location, file_format=cache_file_format
+                cache_file_location=self._cache_file_location,
+                file_format=cache_file_format
             )
             self._web_search_tool = SearchToolWithCache(
                 self._web_search_tool, self._cache
             ).search
         else:
             self._cache = None
         self._encoding = encoding or tiktoken.get_encoding("cl100k_base")
```

### Comparing `pyspark_ai-0.1.0/pyspark_ai/search_tool_with_cache.py` & `pyspark_ai-0.1.1/pyspark_ai/search_tool_with_cache.py`

 * *Files identical despite different names*

### Comparing `pyspark_ai-0.1.0/PKG-INFO` & `pyspark_ai-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspark-ai
-Version: 0.1.0
+Version: 0.1.1
 Summary: English SDK for Apache Spark
 Home-page: https://github.com/databrickslabs/pyspark-ai
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

