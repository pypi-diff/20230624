# Comparing `tmp/openai_function_calling-0.3.0.tar.gz` & `tmp/openai_function_calling-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_calling-0.3.0.tar", max compression
+gzip compressed data, was "openai_function_calling-0.4.0.tar", max compression
```

## Comparing `openai_function_calling-0.3.0.tar` & `openai_function_calling-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1916 2023-06-24 18:28:58.238391 openai_function_calling-0.3.0/README.md
--rw-r--r--   0        0        0      316 2023-06-24 18:07:58.595690 openai_function_calling-0.3.0/openai_function_calling/__init__.py
--rw-r--r--   0        0        0     1402 2023-06-24 17:49:24.389161 openai_function_calling-0.3.0/openai_function_calling/function.py
--rw-r--r--   0        0        0      791 2023-06-24 17:51:44.764292 openai_function_calling-0.3.0/openai_function_calling/parameter.py
--rw-r--r--   0        0        0      571 2023-06-24 18:29:31.311724 openai_function_calling-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 openai_function_calling-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1938 2023-06-24 18:51:48.732222 openai_function_calling-0.4.0/README.md
+-rw-r--r--   0        0        0      316 2023-06-24 18:07:58.595690 openai_function_calling-0.4.0/openai_function_calling/__init__.py
+-rw-r--r--   0        0        0     1756 2023-06-24 18:47:36.891394 openai_function_calling-0.4.0/openai_function_calling/function.py
+-rw-r--r--   0        0        0      848 2023-06-24 18:35:53.411122 openai_function_calling-0.4.0/openai_function_calling/parameter.py
+-rw-r--r--   0        0        0      571 2023-06-24 18:51:14.516718 openai_function_calling-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2442 1970-01-01 00:00:00.000000 openai_function_calling-0.4.0/PKG-INFO
```

### Comparing `openai_function_calling-0.3.0/README.md` & `openai_function_calling-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # OpenAI Function Calling
 
 ![GitHub Actions Build Status](https://github.com/jakecyr/openai-function-calling/actions/workflows/test-application.yml/badge.svg)
 
-Helper functions to generate OpenAI ChatGPT function calling requests. See the [official Function Calling reference](https://platform.openai.com/docs/guides/gpt/function-calling) for more information.
+Helper functions to generate JSON schema dicts for OpenAI ChatGPT function calling requests. See the [official Function Calling reference](https://platform.openai.com/docs/guides/gpt/function-calling) for more information.
 
 ## Installation
 
 Install from PyPi with:
 
 ```bash
 pip install openai-function-calling
```

### Comparing `openai_function_calling-0.3.0/openai_function_calling/function.py` & `openai_function_calling-0.4.0/openai_function_calling/function.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     required: NotRequired[list[str]]
 
 
 class FunctionDict(TypedDict):
     name: str
     description: str
     parameters: ParametersDict
-    required: NotRequired[list[str]]
 
 
 class Function:
     def __init__(
         self,
         name: str,
         description: str,
@@ -31,19 +30,29 @@
 
     def to_dict(self) -> FunctionDict:
         parameters_dict: dict[str, ParameterDict] = {}
 
         for parameter in self.parameters or []:
             parameters_dict[parameter.name] = parameter.to_dict()
 
-        if self.required_parameters:
-            parameters_dict["required"]
-
-        return {
+        output_dict: FunctionDict = {
             "name": self.name,
             "description": self.description,
             "parameters": {
                 "type": "object",
                 "properties": parameters_dict,
-                "required": ["location"],
             },
         }
+
+        if self.required_parameters is None or len(self.required_parameters) == 0:
+            return output_dict
+
+        for parameter in self.required_parameters:
+            if parameter not in parameters_dict:
+                raise ValueError(
+                    "Cannot require a parameter that does not have a "
+                    f"definition: '{parameter}'"
+                )
+
+        output_dict["parameters"]["required"] = self.required_parameters
+
+        return output_dict
```

### Comparing `openai_function_calling-0.3.0/openai_function_calling/parameter.py` & `openai_function_calling-0.4.0/openai_function_calling/parameter.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,23 @@
     type: str
     description: NotRequired[str]
     enum: NotRequired[list[Any]]
 
 
 class Parameter:
     def __init__(
-        self, name: str, type: str, description: str, enum: Optional[list[Any]] = None
+        self,
+        name: str,
+        type: str,
+        description: Optional[str] = None,
+        enum: Optional[list[Any]] = None,
     ) -> None:
         self.name: str = name
         self.type: str = type
-        self.description: str = description
+        self.description: str | None = description
         self.enum: list[Any] | None = enum
 
     def to_dict(self) -> ParameterDict:
         output_dict: ParameterDict = {
             "type": self.type,
         }
```

### Comparing `openai_function_calling-0.3.0/pyproject.toml` & `openai_function_calling-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-function-calling"
-version = "0.3.0"
+version = "0.4.0"
 description = "Helper functions to generate OpenAI GPT function calling requests."
 authors = ["Jake Cyr <cyrjake@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openai_function_calling"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `openai_function_calling-0.3.0/PKG-INFO` & `openai_function_calling-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-function-calling
-Version: 0.3.0
+Version: 0.4.0
 Summary: Helper functions to generate OpenAI GPT function calling requests.
 Author: Jake Cyr
 Author-email: cyrjake@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,15 +12,15 @@
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # OpenAI Function Calling
 
 ![GitHub Actions Build Status](https://github.com/jakecyr/openai-function-calling/actions/workflows/test-application.yml/badge.svg)
 
-Helper functions to generate OpenAI ChatGPT function calling requests. See the [official Function Calling reference](https://platform.openai.com/docs/guides/gpt/function-calling) for more information.
+Helper functions to generate JSON schema dicts for OpenAI ChatGPT function calling requests. See the [official Function Calling reference](https://platform.openai.com/docs/guides/gpt/function-calling) for more information.
 
 ## Installation
 
 Install from PyPi with:
 
 ```bash
 pip install openai-function-calling
```

