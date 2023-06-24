# Comparing `tmp/openai_functions-0.5.4.tar.gz` & `tmp/openai_functions-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.5.4.tar", max compression
+gzip compressed data, was "openai_functions-0.5.5.tar", max compression
```

## Comparing `openai_functions-0.5.4.tar` & `openai_functions-0.5.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2859 2023-06-24 01:53:23.475835 openai_functions-0.5.4/README.md
--rw-r--r--   0        0        0      561 2023-06-24 01:49:09.012365 openai_functions-0.5.4/openai_functions/__init__.py
--rw-r--r--   0        0        0    10102 2023-06-24 02:01:13.116505 openai_functions-0.5.4/openai_functions/conversation.py
--rw-r--r--   0        0        0      371 2023-06-23 23:16:40.645247 openai_functions-0.5.4/openai_functions/functions/__init__.py
--rw-r--r--   0        0        0     2936 2023-06-23 23:39:48.076531 openai_functions-0.5.4/openai_functions/functions/basic_set.py
--rw-r--r--   0        0        0      356 2023-06-24 01:56:28.673664 openai_functions-0.5.4/openai_functions/functions/exceptions.py
--rw-r--r--   0        0        0     2478 2023-06-24 01:57:02.009995 openai_functions-0.5.4/openai_functions/functions/functions.py
--rw-r--r--   0        0        0     4210 2023-06-24 01:50:27.961125 openai_functions-0.5.4/openai_functions/functions/sets.py
--rw-r--r--   0        0        0     1678 2023-06-23 23:33:22.081874 openai_functions-0.5.4/openai_functions/functions/union.py
--rw-r--r--   0        0        0     6327 2023-06-24 01:44:38.621801 openai_functions-0.5.4/openai_functions/functions/wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.5.4/openai_functions/json_type.py
--rw-r--r--   0        0        0     2794 2023-06-24 01:48:05.913763 openai_functions-0.5.4/openai_functions/nlp.py
--rw-r--r--   0        0        0     6605 2023-06-24 01:58:06.858641 openai_functions-0.5.4/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.5.4/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.5.4/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      975 2023-06-24 00:28:00.470995 openai_functions-0.5.4/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.5.4/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-24 00:45:19.947754 openai_functions-0.5.4/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.5.4/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.5.4/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.5.4/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      520 2023-06-24 01:52:09.574112 openai_functions-0.5.4/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.5.4/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.5.4/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.5.4/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.5.4/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.5.4/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.5.4/openai_functions/py.typed
--rw-r--r--   0        0        0      607 2023-06-24 01:57:38.808361 openai_functions-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3511 1970-01-01 00:00:00.000000 openai_functions-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     2859 2023-06-24 01:53:23.475835 openai_functions-0.5.5/README.md
+-rw-r--r--   0        0        0      561 2023-06-24 01:49:09.012365 openai_functions-0.5.5/openai_functions/__init__.py
+-rw-r--r--   0        0        0    10102 2023-06-24 02:01:13.116505 openai_functions-0.5.5/openai_functions/conversation.py
+-rw-r--r--   0        0        0      371 2023-06-23 23:16:40.645247 openai_functions-0.5.5/openai_functions/functions/__init__.py
+-rw-r--r--   0        0        0     2936 2023-06-23 23:39:48.076531 openai_functions-0.5.5/openai_functions/functions/basic_set.py
+-rw-r--r--   0        0        0      356 2023-06-24 01:56:28.673664 openai_functions-0.5.5/openai_functions/functions/exceptions.py
+-rw-r--r--   0        0        0     2478 2023-06-24 01:57:02.009995 openai_functions-0.5.5/openai_functions/functions/functions.py
+-rw-r--r--   0        0        0     4210 2023-06-24 01:50:27.961125 openai_functions-0.5.5/openai_functions/functions/sets.py
+-rw-r--r--   0        0        0     1678 2023-06-23 23:33:22.081874 openai_functions-0.5.5/openai_functions/functions/union.py
+-rw-r--r--   0        0        0     6327 2023-06-24 01:44:38.621801 openai_functions-0.5.5/openai_functions/functions/wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.5.5/openai_functions/json_type.py
+-rw-r--r--   0        0        0     2794 2023-06-24 01:48:05.913763 openai_functions-0.5.5/openai_functions/nlp.py
+-rw-r--r--   0        0        0     6605 2023-06-24 01:58:06.858641 openai_functions-0.5.5/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.5.5/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.5.5/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      975 2023-06-24 00:28:00.470995 openai_functions-0.5.5/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.5.5/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-24 00:45:19.947754 openai_functions-0.5.5/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.5.5/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.5.5/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.5.5/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      520 2023-06-24 01:52:09.574112 openai_functions-0.5.5/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.5.5/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.5.5/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.5.5/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.5.5/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.5.5/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.5.5/openai_functions/py.typed
+-rw-r--r--   0        0        0      607 2023-06-24 02:05:04.256832 openai_functions-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3511 1970-01-01 00:00:00.000000 openai_functions-0.5.5/PKG-INFO
```

### Comparing `openai_functions-0.5.4/README.md` & `openai_functions-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/__init__.py` & `openai_functions-0.5.5/openai_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/conversation.py` & `openai_functions-0.5.5/openai_functions/conversation.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/functions/basic_set.py` & `openai_functions-0.5.5/openai_functions/functions/basic_set.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/functions/functions.py` & `openai_functions-0.5.5/openai_functions/functions/functions.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/functions/sets.py` & `openai_functions-0.5.5/openai_functions/functions/sets.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/functions/union.py` & `openai_functions-0.5.5/openai_functions/functions/union.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/functions/wrapper.py` & `openai_functions-0.5.5/openai_functions/functions/wrapper.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/nlp.py` & `openai_functions-0.5.5/openai_functions/nlp.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/openai_types.py` & `openai_functions-0.5.5/openai_functions/openai_types.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/parsers/abc.py` & `openai_functions-0.5.5/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.5.5/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.5.5/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/parsers/default.py` & `openai_functions-0.5.5/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/parsers/dict_parser.py` & `openai_functions-0.5.5/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/parsers/enum_parser.py` & `openai_functions-0.5.5/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/parsers/float_parser.py` & `openai_functions-0.5.5/openai_functions/parsers/float_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/parsers/int_parser.py` & `openai_functions-0.5.5/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/parsers/list_parser.py` & `openai_functions-0.5.5/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/parsers/none_parser.py` & `openai_functions-0.5.5/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/openai_functions/parsers/union_parser.py` & `openai_functions-0.5.5/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.4/pyproject.toml` & `openai_functions-0.5.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.5.4"
+version = "0.5.5"
 description = "Simplifies the usage of OpenAI's function calling."
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "openai_functions"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `openai_functions-0.5.4/PKG-INFO` & `openai_functions-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.5.4
+Version: 0.5.5
 Summary: Simplifies the usage of OpenAI's function calling.
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

