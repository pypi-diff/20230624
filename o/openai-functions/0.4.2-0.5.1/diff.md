# Comparing `tmp/openai_functions-0.4.2.tar.gz` & `tmp/openai_functions-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.4.2.tar", max compression
+gzip compressed data, was "openai_functions-0.5.1.tar", max compression
```

## Comparing `openai_functions-0.4.2.tar` & `openai_functions-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,29 @@
--rw-r--r--   0        0        0     2689 2023-06-23 21:23:30.745575 openai_functions-0.4.2/README.md
--rw-r--r--   0        0        0      385 2023-06-23 21:21:35.696216 openai_functions-0.4.2/openai_functions/__init__.py
--rw-r--r--   0        0        0    12813 2023-06-23 22:09:12.725627 openai_functions-0.4.2/openai_functions/conversation.py
--rw-r--r--   0        0        0     6245 2023-06-23 20:59:37.510332 openai_functions-0.4.2/openai_functions/function_wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.4.2/openai_functions/json_type.py
--rw-r--r--   0        0        0     6399 2023-06-23 22:16:16.102898 openai_functions-0.4.2/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.4.2/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.4.2/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.4.2/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.4.2/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.4.2/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.4.2/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.4.2/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.4.2/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.4.2/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.4.2/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.4.2/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.4.2/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.4.2/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.4.2/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.4.2/openai_functions/py.typed
--rw-r--r--   0        0        0      557 2023-06-23 22:18:36.452317 openai_functions-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3291 1970-01-01 00:00:00.000000 openai_functions-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     2689 2023-06-23 21:23:30.745575 openai_functions-0.5.1/README.md
+-rw-r--r--   0        0        0      529 2023-06-23 23:16:48.913340 openai_functions-0.5.1/openai_functions/__init__.py
+-rw-r--r--   0        0        0     9051 2023-06-23 23:33:40.127098 openai_functions-0.5.1/openai_functions/conversation.py
+-rw-r--r--   0        0        0      371 2023-06-23 23:16:40.645247 openai_functions-0.5.1/openai_functions/functions/__init__.py
+-rw-r--r--   0        0        0     3116 2023-06-23 23:11:05.588418 openai_functions-0.5.1/openai_functions/functions/basic_set.py
+-rw-r--r--   0        0        0      136 2023-06-23 23:09:35.721366 openai_functions-0.5.1/openai_functions/functions/exceptions.py
+-rw-r--r--   0        0        0     1369 2023-06-23 22:58:45.747092 openai_functions-0.5.1/openai_functions/functions/functions.py
+-rw-r--r--   0        0        0     3881 2023-06-23 23:10:56.953317 openai_functions-0.5.1/openai_functions/functions/sets.py
+-rw-r--r--   0        0        0     1678 2023-06-23 23:33:22.081874 openai_functions-0.5.1/openai_functions/functions/union.py
+-rw-r--r--   0        0        0     6247 2023-06-23 22:59:35.344787 openai_functions-0.5.1/openai_functions/functions/wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.5.1/openai_functions/json_type.py
+-rw-r--r--   0        0        0     6413 2023-06-23 23:30:57.813048 openai_functions-0.5.1/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.5.1/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.5.1/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.5.1/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.5.1/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.5.1/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.5.1/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.5.1/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.5.1/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.5.1/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.5.1/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.5.1/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.5.1/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.5.1/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.5.1/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.5.1/openai_functions/py.typed
+-rw-r--r--   0        0        0      557 2023-06-23 23:34:15.015530 openai_functions-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3291 1970-01-01 00:00:00.000000 openai_functions-0.5.1/PKG-INFO
```

### Comparing `openai_functions-0.4.2/README.md` & `openai_functions-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.2/openai_functions/conversation.py` & `openai_functions-0.5.1/openai_functions/conversation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,49 @@
 """A module for running OpenAI functions"""
 from __future__ import annotations
-from functools import partial
-import json
-from typing import Callable, Protocol, TYPE_CHECKING, overload, runtime_checkable
+from typing import Callable, TYPE_CHECKING, overload
 
 import openai
 
-from .function_wrapper import FunctionWrapper, WrapperConfig
+from .functions.union import UnionSkillSet
 from .openai_types import (
     FinalResponseMessage,
     FunctionMessageType,
     GenericMessage,
     Message,
     is_final_response_message,
 )
 
+
 if TYPE_CHECKING:
     from .json_type import JsonType
     from .openai_types import FunctionCall, MessageType, NonFunctionMessageType
-
-
-@runtime_checkable
-class OpenAIFunction(Protocol):
-    """A protocol for OpenAI functions"""
-
-    def __call__(self, arguments: dict[str, JsonType]) -> JsonType:
-        ...
-
-    @property
-    def schema(self) -> JsonType:
-        """Get the schema for this function"""
-
-    @property
-    def name(self) -> str:
-        """Get the name of this function"""
-        # This ellipsis is for Pyright #2758
-        ...  # pylint: disable=unnecessary-ellipsis
-
-    @property
-    def save_return(self) -> bool:
-        """Get whether to save the return value of this function"""
-        ...  # pylint: disable=unnecessary-ellipsis
-
-    @property
-    def serialize(self) -> bool:
-        """Get whether to continue running after this function"""
-        ...  # pylint: disable=unnecessary-ellipsis
-
-    @property
-    def interpret_as_response(self) -> bool:
-        """Get whether to interpret the return value of this function as a response"""
-        ...  # pylint: disable=unnecessary-ellipsis
+    from .functions.sets import FunctionResult, FunctionSet, OpenAIFunction
 
 
 class Conversation:
     """A class for running OpenAI functions"""
 
     def __init__(
         self,
-        functions: list[OpenAIFunction] | None = None,
+        skills: list[FunctionSet] | None = None,
         model: str = "gpt-3.5-turbo-0613",
     ) -> None:
         self.messages: list[GenericMessage] = []
-        self.functions = functions or []
+        self.skills = UnionSkillSet(*(skills or []))
         self.model = model
 
     @property
     def functions_schema(self) -> JsonType:
         """Get the functions schema
 
         Returns:
             JsonType: The functions schema
         """
-        return [function.schema for function in self.functions]
-
-    def run_function(self, input_data: FunctionCall) -> JsonType:
-        """Run the function
-
-        Args:
-            input_data (FunctionCall): The function call
-
-        Returns:
-            JsonType: The function output
-
-        Raises:
-            TypeError: If the input data is not a dictionary
-            ValueError: If the function is not found
-        """
-        return self.find_function(input_data["name"])(
-            json.loads(input_data["arguments"])
-        )
+        return self.skills.functions_schema
 
     def _add_message(self, message: GenericMessage) -> None:
         """Add a message
 
         Args:
             message (GenericMessage): The message
         """
@@ -144,114 +94,68 @@
             model=self.model,
             messages=[message.as_dict() for message in self.messages],
             functions=self.functions_schema,
             function_call="auto",
         )
         return response["choices"][0]["message"]  # type: ignore
 
-    def find_function(self, function_name: str) -> OpenAIFunction:
-        """Find a function
-
-        Args:
-            function_name (str): The function name
-
-        Returns:
-            OpenAIFunction: The function
-
-        Raises:
-            ValueError: If the function is not found
-        """
-        for function in self.functions:
-            if function.name == function_name:
-                return function
-        raise ValueError(f"Function {function_name} not found")
-
-    def get_function_result(
-        self, function: OpenAIFunction, arguments: dict[str, JsonType]
-    ) -> str | None:
-        """Get the result of a function
-
-        Args:
-            function (OpenAIFunction): The function
-            arguments (dict[str, JsonType]): The arguments
-
-        Raises:
-            TypeError: If the function returns a non-string value
-                while serialize is False
-
-        Returns:
-            str | None: The result
-        """
-        result = function(arguments)
-
-        if function.save_return:
-            if function.serialize:
-                return json.dumps(result)
-            if isinstance(result, str):
-                return result
-            raise TypeError(f"Function {function.name} returned a non-string value")
-        return None
-
     def substitute_last_with_function_result(self, result: str) -> None:
         """Substitute the last message with the result
 
         Args:
             result (str): The function result
         """
         self.pop_message()
         response: NonFunctionMessageType = {
             "role": "assistant",
             "content": result,
         }
         self.add_message(response)
 
-    def add_function_result(
-        self, function_name: str, function_result: str | None
-    ) -> bool:
+    def add_function_result(self, function_result: FunctionResult) -> bool:
         """Add a function result
 
         Args:
-            function_name (str): The function name
-            function_result (str | None): The function result
+            function_result (FunctionResult): The function result
 
         Returns:
             bool: Whether the function result was added
         """
-        if function_result is None:
+        if function_result.content is None:
             return False
         response: FunctionMessageType = {
             "role": "function",
-            "name": function_name,
-            "content": function_result,
+            "name": function_result.name,
+            "content": function_result.content,
         }
         self.add_message(response)
         return True
 
     def add_or_substitute_function_result(
-        self, function_name: str, function_result: str | None, substitute: bool = False
+        self, function_result: FunctionResult
     ) -> bool:
         """Add or substitute a function result
 
         Args:
-            function_name (str): The function name
-            function_result (str): The function result
-            substitute (bool): Whether to substitute the last message.
+            function_result (FunctionResult): The function result
 
         Raises:
             TypeError: If the function returns a None value
 
         Returns:
             bool: Whether the function result was added
         """
-        if substitute:
-            if function_result is None:
-                raise TypeError(f"Function {function_name} returned a None value")
-            self.substitute_last_with_function_result(function_result)
+        if function_result.substitute:
+            if function_result.content is None:
+                raise TypeError(
+                    f"Function {function_result.name} returned a None value"
+                )
+            self.substitute_last_with_function_result(function_result.content)
             return True
-        return self.add_function_result(function_name, function_result)
+        return self.add_function_result(function_result)
 
     def run_function_and_substitute(
         self,
         function_call: FunctionCall,
     ) -> bool:
         """Run a function, replacing the last message with the result if needed
 
@@ -260,21 +164,16 @@
 
         Raises:
             TypeError: If the function returns a None value
 
         Returns:
             bool: Whether the function result was added
         """
-        function = self.find_function(function_call["name"])
-        function_result = self.get_function_result(
-            function, json.loads(function_call["arguments"])
-        )
-
         return self.add_or_substitute_function_result(
-            function.name, function_result, function.interpret_as_response
+            self.skills.run_function(function_call)
         )
 
     def run_function_if_needed(self) -> bool:
         """Run a function if needed
 
         Returns:
             bool: Whether the function result was added
@@ -308,22 +207,14 @@
             FinalResponseMessage: The response
         """
         while True:
             message = self.generate_message()
             if is_final_response_message(message):
                 return message
 
-    def _add_function(self, function: OpenAIFunction) -> None:
-        """Add a function
-
-        Args:
-            function (OpenAIFunction): The function
-        """
-        self.functions.append(function)
-
     @overload
     def add_function(self, function: OpenAIFunction) -> OpenAIFunction:
         ...
 
     @overload
     def add_function(
         self,
@@ -368,61 +259,49 @@
             interpret_as_response (bool): Whether to interpret the return
                 value of this function as a response of the agent. Defaults to False.
 
         Returns:
             Callable[[Callable[..., JsonType]], Callable[..., JsonType]]: A decorator
             Callable[..., JsonType]: The original function
         """
-        if isinstance(function, OpenAIFunction):
-            self._add_function(function)
-            return function
-        if callable(function):
-            self._add_function(
-                FunctionWrapper(
-                    function,
-                    WrapperConfig(None, save_return, serialize, interpret_as_response),
-                )
+        if function is None:
+            return self.skills.add_function(
+                save_return=save_return,
+                serialize=serialize,
+                interpret_as_response=interpret_as_response,
             )
-            return function
-
-        return partial(
-            self.add_function,
+        return self.skills.add_function(
+            function,
             save_return=save_return,
             serialize=serialize,
             interpret_as_response=interpret_as_response,
         )
 
-    def _remove_function(self, function: str) -> None:
-        """Remove a function
-
-        Args:
-            function (str): The function
-        """
-        self.functions = [f for f in self.functions if f.name != function]
-
     def remove_function(
         self, function: str | OpenAIFunction | Callable[..., JsonType]
     ) -> None:
         """Remove a function
 
         Args:
             function (str | OpenAIFunction | Callable[..., JsonType]): The function
         """
-        if isinstance(function, str):
-            self._remove_function(function)
-            return
-        if isinstance(function, OpenAIFunction):
-            self._remove_function(function.name)
-            return
-        self._remove_function(function.__name__)
+        self.skills.remove_function(function)
 
     def ask(self, question: str) -> str:
         """Ask the AI a question
 
         Args:
             question (str): The question
 
         Returns:
             str: The answer to the question
         """
         self.add_message(question)
         return self.run_until_response().content
+
+    def add_skill(self, skill: FunctionSet) -> None:
+        """Add a skill
+
+        Args:
+            skill (FunctionSet): The skill to add
+        """
+        self.skills.add_skill(skill)
```

### Comparing `openai_functions-0.4.2/openai_functions/function_wrapper.py` & `openai_functions-0.5.1/openai_functions/functions/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from __future__ import annotations
 from dataclasses import dataclass
 import inspect
 from typing import Any, Callable, OrderedDict, TYPE_CHECKING, Type
 
 from docstring_parser import Docstring, parse
 
-from .parsers import ArgSchemaParser, defargparsers
+from ..parsers import ArgSchemaParser, defargparsers
 
 if TYPE_CHECKING:
-    from .json_type import JsonType
+    from ..json_type import JsonType
 
 
 @dataclass
 class WrapperConfig:
     """Configuration for a FunctionWrapper"""
 
     parsers: list[Type[ArgSchemaParser]] | None = None
```

### Comparing `openai_functions-0.4.2/openai_functions/openai_types.py` & `openai_functions-0.5.1/openai_functions/openai_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     def function_call(self) -> FunctionCall | None:
         """Get the function call
 
         Returns:
             FunctionCall | None: The function call
         """
         if self.message["role"] == "assistant":
-            if "content" in self.message:
+            if self.message.get("content") is not None:
                 return None
             return self.message.get("function_call")
         return None
 
     @property
     def is_final_response(self) -> bool:
         """Check if the message is a final response
```

### Comparing `openai_functions-0.4.2/openai_functions/parsers/abc.py` & `openai_functions-0.5.1/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.2/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.5.1/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.2/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.5.1/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.2/openai_functions/parsers/default.py` & `openai_functions-0.5.1/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.2/openai_functions/parsers/dict_parser.py` & `openai_functions-0.5.1/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.2/openai_functions/parsers/enum_parser.py` & `openai_functions-0.5.1/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.2/openai_functions/parsers/int_parser.py` & `openai_functions-0.5.1/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.2/openai_functions/parsers/list_parser.py` & `openai_functions-0.5.1/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.2/openai_functions/parsers/none_parser.py` & `openai_functions-0.5.1/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.2/openai_functions/parsers/union_parser.py` & `openai_functions-0.5.1/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.2/pyproject.toml` & `openai_functions-0.5.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.4.2"
+version = "0.5.1"
 description = ""
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "openai_functions"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `openai_functions-0.4.2/PKG-INFO` & `openai_functions-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.4.2
+Version: 0.5.1
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

