# Comparing `tmp/openai_function_calling-0.2.0.tar.gz` & `tmp/openai_function_calling-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_calling-0.2.0.tar", max compression
+gzip compressed data, was "openai_function_calling-0.3.0.tar", max compression
```

## Comparing `openai_function_calling-0.2.0.tar` & `openai_function_calling-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1856 2023-06-24 18:27:02.962873 openai_function_calling-0.2.0/README.md
--rw-r--r--   0        0        0      316 2023-06-24 18:07:58.595690 openai_function_calling-0.2.0/openai_function_calling/__init__.py
--rw-r--r--   0        0        0     1402 2023-06-24 17:49:24.389161 openai_function_calling-0.2.0/openai_function_calling/function.py
--rw-r--r--   0        0        0      791 2023-06-24 17:51:44.764292 openai_function_calling-0.2.0/openai_function_calling/parameter.py
--rw-r--r--   0        0        0      571 2023-06-24 18:27:02.968464 openai_function_calling-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 openai_function_calling-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1916 2023-06-24 18:28:58.238391 openai_function_calling-0.3.0/README.md
+-rw-r--r--   0        0        0      316 2023-06-24 18:07:58.595690 openai_function_calling-0.3.0/openai_function_calling/__init__.py
+-rw-r--r--   0        0        0     1402 2023-06-24 17:49:24.389161 openai_function_calling-0.3.0/openai_function_calling/function.py
+-rw-r--r--   0        0        0      791 2023-06-24 17:51:44.764292 openai_function_calling-0.3.0/openai_function_calling/parameter.py
+-rw-r--r--   0        0        0      571 2023-06-24 18:29:31.311724 openai_function_calling-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 openai_function_calling-0.3.0/PKG-INFO
```

### Comparing `openai_function_calling-0.2.0/README.md` & `openai_function_calling-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -61,8 +61,8 @@
 export OPENAI_API_KEY=SOME_KEY_VALUE
 
 # or when running an example
 
 OPENAI_API_KEY=SOME_KEY_VALUE python examples/weather_functions.py
 ```
 
-See complete examples in the [./examples](./examples/) folder.
+See complete examples in the [./examples](https://github.com/jakecyr/openai-function-calling/tree/master/examples) folder.
```

### Comparing `openai_function_calling-0.2.0/openai_function_calling/function.py` & `openai_function_calling-0.3.0/openai_function_calling/function.py`

 * *Files identical despite different names*

### Comparing `openai_function_calling-0.2.0/openai_function_calling/parameter.py` & `openai_function_calling-0.3.0/openai_function_calling/parameter.py`

 * *Files identical despite different names*

### Comparing `openai_function_calling-0.2.0/pyproject.toml` & `openai_function_calling-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-function-calling"
-version = "0.2.0"
+version = "0.3.0"
 description = "Helper functions to generate OpenAI GPT function calling requests."
 authors = ["Jake Cyr <cyrjake@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_function_calling"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `openai_function_calling-0.2.0/PKG-INFO` & `openai_function_calling-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-function-calling
-Version: 0.2.0
+Version: 0.3.0
 Summary: Helper functions to generate OpenAI GPT function calling requests.
 Author: Jake Cyr
 Author-email: cyrjake@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -75,9 +75,9 @@
 export OPENAI_API_KEY=SOME_KEY_VALUE
 
 # or when running an example
 
 OPENAI_API_KEY=SOME_KEY_VALUE python examples/weather_functions.py
 ```
 
-See complete examples in the [./examples](./examples/) folder.
+See complete examples in the [./examples](https://github.com/jakecyr/openai-function-calling/tree/master/examples) folder.
```

