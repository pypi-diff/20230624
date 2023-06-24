# Comparing `tmp/openai_function_calling-0.4.0.tar.gz` & `tmp/openai_function_calling-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_calling-0.4.0.tar", max compression
+gzip compressed data, was "openai_function_calling-0.5.0.tar", max compression
```

## Comparing `openai_function_calling-0.4.0.tar` & `openai_function_calling-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1938 2023-06-24 18:51:48.732222 openai_function_calling-0.4.0/README.md
--rw-r--r--   0        0        0      316 2023-06-24 18:07:58.595690 openai_function_calling-0.4.0/openai_function_calling/__init__.py
--rw-r--r--   0        0        0     1756 2023-06-24 18:47:36.891394 openai_function_calling-0.4.0/openai_function_calling/function.py
--rw-r--r--   0        0        0      848 2023-06-24 18:35:53.411122 openai_function_calling-0.4.0/openai_function_calling/parameter.py
--rw-r--r--   0        0        0      571 2023-06-24 18:51:14.516718 openai_function_calling-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2442 1970-01-01 00:00:00.000000 openai_function_calling-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2161 2023-06-24 18:57:10.088869 openai_function_calling-0.5.0/README.md
+-rw-r--r--   0        0        0      316 2023-06-24 18:07:58.595690 openai_function_calling-0.5.0/openai_function_calling/__init__.py
+-rw-r--r--   0        0        0     1756 2023-06-24 18:47:36.891394 openai_function_calling-0.5.0/openai_function_calling/function.py
+-rw-r--r--   0        0        0      848 2023-06-24 18:35:53.411122 openai_function_calling-0.5.0/openai_function_calling/parameter.py
+-rw-r--r--   0        0        0      571 2023-06-24 18:57:40.974266 openai_function_calling-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 openai_function_calling-0.5.0/PKG-INFO
```

### Comparing `openai_function_calling-0.4.0/README.md` & `openai_function_calling-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 Install from PyPi with:
 
 ```bash
 pip install openai-function-calling
 ```
 
+**The openai-function-calling package does come with the openai package. It must be installed separately with `pip install openai`**
+
 ## Usage
 
 ```python
 from openai_function_calling import Function, FunctionDict, Parameter
 
 def get_current_weather(location: str, unit: str) -> str:
   # Do some stuff here...
@@ -61,8 +63,10 @@
 export OPENAI_API_KEY=SOME_KEY_VALUE
 
 # or when running an example
 
 OPENAI_API_KEY=SOME_KEY_VALUE python examples/weather_functions.py
 ```
 
+Make sure to also follow all instructions in the [Installation section](#installation).
+
 See complete examples in the [./examples](https://github.com/jakecyr/openai-function-calling/tree/master/examples) folder.
```

### Comparing `openai_function_calling-0.4.0/openai_function_calling/function.py` & `openai_function_calling-0.5.0/openai_function_calling/function.py`

 * *Files identical despite different names*

### Comparing `openai_function_calling-0.4.0/openai_function_calling/parameter.py` & `openai_function_calling-0.5.0/openai_function_calling/parameter.py`

 * *Files identical despite different names*

### Comparing `openai_function_calling-0.4.0/pyproject.toml` & `openai_function_calling-0.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "openai-function-calling"
-version = "0.4.0"
+version = "0.5.0"
 description = "Helper functions to generate OpenAI GPT function calling requests."
 authors = ["Jake Cyr <cyrjake@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_function_calling"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-openai = "^0.27.8"
 typing-extensions = "^4.6.3"
 
 [tool.poetry.group.dev.dependencies]
+openai = "^0.27.8"
 black = "^23.3.0"
 pytest = "^7.4.0"
 ruff = "^0.0.275"
 coverage = "^7.2.7"
 build = "^0.10.0"
 
 [build-system]
```

### Comparing `openai_function_calling-0.4.0/PKG-INFO` & `openai_function_calling-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: openai-function-calling
-Version: 0.4.0
+Version: 0.5.0
 Summary: Helper functions to generate OpenAI GPT function calling requests.
 Author: Jake Cyr
 Author-email: cyrjake@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # OpenAI Function Calling
 
 ![GitHub Actions Build Status](https://github.com/jakecyr/openai-function-calling/actions/workflows/test-application.yml/badge.svg)
 
@@ -22,14 +21,16 @@
 
 Install from PyPi with:
 
 ```bash
 pip install openai-function-calling
 ```
 
+**The openai-function-calling package does come with the openai package. It must be installed separately with `pip install openai`**
+
 ## Usage
 
 ```python
 from openai_function_calling import Function, FunctionDict, Parameter
 
 def get_current_weather(location: str, unit: str) -> str:
   # Do some stuff here...
@@ -75,9 +76,11 @@
 export OPENAI_API_KEY=SOME_KEY_VALUE
 
 # or when running an example
 
 OPENAI_API_KEY=SOME_KEY_VALUE python examples/weather_functions.py
 ```
 
+Make sure to also follow all instructions in the [Installation section](#installation).
+
 See complete examples in the [./examples](https://github.com/jakecyr/openai-function-calling/tree/master/examples) folder.
```

