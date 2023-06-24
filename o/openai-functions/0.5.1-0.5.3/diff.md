# Comparing `tmp/openai_functions-0.5.1.tar.gz` & `tmp/openai_functions-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.5.1.tar", max compression
+gzip compressed data, was "openai_functions-0.5.3.tar", max compression
```

## Comparing `openai_functions-0.5.1.tar` & `openai_functions-0.5.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     2689 2023-06-23 21:23:30.745575 openai_functions-0.5.1/README.md
--rw-r--r--   0        0        0      529 2023-06-23 23:16:48.913340 openai_functions-0.5.1/openai_functions/__init__.py
--rw-r--r--   0        0        0     9051 2023-06-23 23:33:40.127098 openai_functions-0.5.1/openai_functions/conversation.py
--rw-r--r--   0        0        0      371 2023-06-23 23:16:40.645247 openai_functions-0.5.1/openai_functions/functions/__init__.py
--rw-r--r--   0        0        0     3116 2023-06-23 23:11:05.588418 openai_functions-0.5.1/openai_functions/functions/basic_set.py
--rw-r--r--   0        0        0      136 2023-06-23 23:09:35.721366 openai_functions-0.5.1/openai_functions/functions/exceptions.py
--rw-r--r--   0        0        0     1369 2023-06-23 22:58:45.747092 openai_functions-0.5.1/openai_functions/functions/functions.py
--rw-r--r--   0        0        0     3881 2023-06-23 23:10:56.953317 openai_functions-0.5.1/openai_functions/functions/sets.py
--rw-r--r--   0        0        0     1678 2023-06-23 23:33:22.081874 openai_functions-0.5.1/openai_functions/functions/union.py
--rw-r--r--   0        0        0     6247 2023-06-23 22:59:35.344787 openai_functions-0.5.1/openai_functions/functions/wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.5.1/openai_functions/json_type.py
--rw-r--r--   0        0        0     6413 2023-06-23 23:30:57.813048 openai_functions-0.5.1/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.5.1/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.5.1/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.5.1/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.5.1/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.5.1/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.5.1/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.5.1/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.5.1/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.5.1/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.5.1/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.5.1/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.5.1/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.5.1/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.5.1/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.5.1/openai_functions/py.typed
--rw-r--r--   0        0        0      557 2023-06-23 23:34:15.015530 openai_functions-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3291 1970-01-01 00:00:00.000000 openai_functions-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2859 2023-06-24 01:53:23.475835 openai_functions-0.5.3/README.md
+-rw-r--r--   0        0        0      561 2023-06-24 01:49:09.012365 openai_functions-0.5.3/openai_functions/__init__.py
+-rw-r--r--   0        0        0    10102 2023-06-24 01:51:13.190563 openai_functions-0.5.3/openai_functions/conversation.py
+-rw-r--r--   0        0        0      371 2023-06-23 23:16:40.645247 openai_functions-0.5.3/openai_functions/functions/__init__.py
+-rw-r--r--   0        0        0     2936 2023-06-23 23:39:48.076531 openai_functions-0.5.3/openai_functions/functions/basic_set.py
+-rw-r--r--   0        0        0      136 2023-06-23 23:09:35.721366 openai_functions-0.5.3/openai_functions/functions/exceptions.py
+-rw-r--r--   0        0        0     2577 2023-06-24 01:50:53.906376 openai_functions-0.5.3/openai_functions/functions/functions.py
+-rw-r--r--   0        0        0     4210 2023-06-24 01:50:27.961125 openai_functions-0.5.3/openai_functions/functions/sets.py
+-rw-r--r--   0        0        0     1678 2023-06-23 23:33:22.081874 openai_functions-0.5.3/openai_functions/functions/union.py
+-rw-r--r--   0        0        0     6327 2023-06-24 01:44:38.621801 openai_functions-0.5.3/openai_functions/functions/wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.5.3/openai_functions/json_type.py
+-rw-r--r--   0        0        0     2794 2023-06-24 01:48:05.913763 openai_functions-0.5.3/openai_functions/nlp.py
+-rw-r--r--   0        0        0     6605 2023-06-24 01:45:16.200173 openai_functions-0.5.3/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.5.3/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.5.3/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      975 2023-06-24 00:28:00.470995 openai_functions-0.5.3/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.5.3/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-24 00:45:19.947754 openai_functions-0.5.3/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.5.3/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.5.3/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.5.3/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      520 2023-06-24 01:52:09.574112 openai_functions-0.5.3/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.5.3/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.5.3/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.5.3/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.5.3/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.5.3/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.5.3/openai_functions/py.typed
+-rw-r--r--   0        0        0      557 2023-06-24 00:54:39.693088 openai_functions-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 openai_functions-0.5.3/PKG-INFO
```

### Comparing `openai_functions-0.5.1/README.md` & `openai_functions-0.5.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -52,29 +52,46 @@
         "temperature": "72",
         "unit": unit.value,
         "forecast": ["sunny", "windy"],
     }
     return weather_info
 ```
 
-4. Add user messages using the `conversation.add_message` method:
+4. Ask the AI a question:
 
 ```python
-conversation.add_message(
-    {
-        "role": "user",
-        "content": "What's the weather in San Francisco?",
-    }
-)
+conversation.ask("What's the weather in San Francisco?")
+```
+
+## Another usecase: data extraction
+
+1. Import the necessary modules:
+
+```python
+from dataclasses import dataclass
+import openai
+from openai_functions import nlp
+```
+
+3. Define your data container using the `@nlp` decorator:
+
+```python
+@nlp
+@dataclass
+class Person:
+    """Extract personal info"""
+
+    name: str
+    age: int
 ```
 
-5. Call the `conversation.run_until_response()` method to trigger the conversation and retrieve the response:
+4. Ask the AI for a summary of the data:
 
 ```python
-print(conversation.run_until_response())
+Person.nlp("I'm Jack and I'm 20 years old.", "Person")
 ```
 
 ## How it Works
 
 `openai-functions` takes care of the following tasks:
 
 - Parsing the function signatures and docstrings.
```

### Comparing `openai_functions-0.5.1/openai_functions/__init__.py` & `openai_functions-0.5.3/openai_functions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 from .functions import (
     BasicFunctionSet,
     FunctionNotFoundError,
     FunctionSet,
     FunctionWrapper,
     WrapperConfig,
 )
+from .nlp import nlp
 from .openai_types import Message
 from .parsers import ArgSchemaParser, defargparsers
 
 __all__ = [
     "Conversation",
     "BasicFunctionSet",
     "FunctionNotFoundError",
     "FunctionSet",
     "defargparsers",
     "ArgSchemaParser",
     "FunctionWrapper",
+    "nlp",
     "Message",
     "WrapperConfig",
 ]
```

### Comparing `openai_functions-0.5.1/openai_functions/conversation.py` & `openai_functions-0.5.3/openai_functions/conversation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 """A module for running OpenAI functions"""
 from __future__ import annotations
-from typing import Callable, TYPE_CHECKING, overload
+from typing import Any, Callable, TYPE_CHECKING, overload
 
 import openai
 
 from .functions.union import UnionSkillSet
 from .openai_types import (
     FinalResponseMessage,
     FunctionMessageType,
     GenericMessage,
+    IntermediateResponseMessageType,
     Message,
     is_final_response_message,
 )
 
 
 if TYPE_CHECKING:
     from .json_type import JsonType
-    from .openai_types import FunctionCall, MessageType, NonFunctionMessageType
-    from .functions.sets import FunctionResult, FunctionSet, OpenAIFunction
+    from .openai_types import (
+        FunctionCall,
+        MessageType,
+        NonFunctionMessageType,
+        OpenAIFunctionCallInput,
+    )
+    from .functions.functions import OpenAIFunction
+    from .functions.sets import FunctionResult, FunctionSet
 
 
 class Conversation:
     """A class for running OpenAI functions"""
 
     def __init__(
         self,
@@ -80,25 +87,30 @@
         """
         return self.messages.pop(index)
 
     def clear_messages(self) -> None:
         """Clear the messages"""
         self.messages = []
 
-    def _generate_message(self) -> NonFunctionMessageType:
+    def _generate_message(
+        self, function_call: OpenAIFunctionCallInput = "auto"
+    ) -> NonFunctionMessageType:
         """Generate a response
 
+        Args:
+            function_call (OpenAIFunctionCallInput): The function call.
+
         Returns:
             NonFunctionMessageType: The response
         """
         response = openai.ChatCompletion.create(
             model=self.model,
             messages=[message.as_dict() for message in self.messages],
             functions=self.functions_schema,
-            function_call="auto",
+            function_call=function_call,
         )
         return response["choices"][0]["message"]  # type: ignore
 
     def substitute_last_with_function_result(self, result: str) -> None:
         """Substitute the last message with the result
 
         Args:
@@ -183,24 +195,29 @@
 
         function_call = self.messages[-1].function_call
         if not function_call:
             return False
 
         return self.run_function_and_substitute(function_call)
 
-    def generate_message(self) -> GenericMessage:
+    def generate_message(
+        self, function_call: OpenAIFunctionCallInput = "auto"
+    ) -> GenericMessage:
         """Generate the next message
 
+        Args:
+            function_call (OpenAIFunctionCallInput): The function call
+
         Returns:
             GenericMessage: The response
         """
         if self.run_function_if_needed():
             return self.messages[-1]
 
-        message = self._generate_message()
+        message = self._generate_message(function_call)
         self.add_message(message)
         return Message(message)
 
     def run_until_response(self) -> FinalResponseMessage:
         """Run until a response is generated
 
         Returns:
@@ -301,7 +318,23 @@
     def add_skill(self, skill: FunctionSet) -> None:
         """Add a skill
 
         Args:
             skill (FunctionSet): The skill to add
         """
         self.skills.add_skill(skill)
+
+    def run(self, function: str, prompt: str) -> Any:
+        """Run a specified function and return the raw function result
+
+        Args:
+            prompt (str): The prompt to use
+            function (str): The function to run
+
+        Returns:
+            The raw function result
+        """
+        self.add_message(prompt)
+        # We can do type: ignore as we know we're forcing a function call
+        response: IntermediateResponseMessageType
+        response = self._generate_message({"name": function})  # type: ignore
+        return self.skills(response["function_call"])
```

### Comparing `openai_functions-0.5.1/openai_functions/functions/basic_set.py` & `openai_functions-0.5.3/openai_functions/functions/basic_set.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A module for running OpenAI functions"""
 from __future__ import annotations
 import json
 from typing import TYPE_CHECKING
 
 from .exceptions import FunctionNotFoundError
-from .functions import FunctionResult, OpenAIFunction
+from .functions import FunctionResult, OpenAIFunction, RawFunctionResult
 from .sets import FunctionSet
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
     from ..openai_types import FunctionCall
 
 
@@ -61,36 +61,30 @@
         for function in self.functions:
             if function.name == function_name:
                 return function
         raise FunctionNotFoundError(f"Function {function_name} not found")
 
     def get_function_result(
         self, function: OpenAIFunction, arguments: dict[str, JsonType]
-    ) -> str | None:
+    ) -> RawFunctionResult | None:
         """Get the result of a function
 
         Args:
             function (OpenAIFunction): The function
             arguments (dict[str, JsonType]): The arguments
 
-        Raises:
-            TypeError: If the function returns a non-string value
-                while serialize is False
-
         Returns:
-            str | None: The result
+            RawFunctionResult | None: The result
         """
         result = function(arguments)
 
         if function.save_return:
             if function.serialize:
-                return json.dumps(result)
-            if isinstance(result, str):
-                return result
-            raise TypeError(f"Function {function.name} returned a non-string value")
+                return RawFunctionResult(result)
+            return RawFunctionResult(result)
         return None
 
     def _add_function(self, function: OpenAIFunction) -> None:
         """Add a function
 
         Args:
             function (OpenAIFunction): The function
```

### Comparing `openai_functions-0.5.1/openai_functions/functions/functions.py` & `openai_functions-0.5.3/openai_functions/functions/functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """A module for running OpenAI functions"""
 from __future__ import annotations
 from dataclasses import dataclass
-from typing import Protocol, TYPE_CHECKING, runtime_checkable
+import json
+from typing import Any, Protocol, TYPE_CHECKING, runtime_checkable
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 
 @runtime_checkable
 class OpenAIFunction(Protocol):
@@ -37,13 +38,60 @@
     @property
     def interpret_as_response(self) -> bool:
         """Get whether to interpret the return value of this function as a response"""
         ...  # pylint: disable=unnecessary-ellipsis
 
 
 @dataclass
+class RawFunctionResult:
+    """A raw function result"""
+
+    result: Any
+    serialize: bool = True
+
+    @property
+    def serialized(self) -> str:
+        """Get the serialized result
+
+        Raises:
+            ValueError: If the result is not a string
+
+        Returns:
+            str: The serialized result
+        """
+        if self.serialize:
+            return json.dumps(self.result)
+        if isinstance(self.result, str):
+            return self.result
+        raise ValueError("Function did not return a string")
+
+
+@dataclass
 class FunctionResult:
     """A result of a function's execution"""
 
     name: str
-    content: str | None
+    raw_result: RawFunctionResult | None
     substitute: bool = False
+
+    @property
+    def content(self) -> str | None:
+        """Get the content of this result
+
+        Returns:
+            str | None: The content
+        """
+        return self.raw_result.serialized if self.raw_result else None
+
+    @property
+    def result(self) -> JsonType | None:
+        """Get the result of this function call
+
+        Raises:
+            ValueError: If the function was not expected to return a value
+
+        Returns:
+            JsonType: The result
+        """
+        if self.raw_result:
+            return self.raw_result.result
+        raise ValueError("Function was not expected to return a value")
```

### Comparing `openai_functions-0.5.1/openai_functions/functions/sets.py` & `openai_functions-0.5.3/openai_functions/functions/sets.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,7 +121,18 @@
         if isinstance(function, str):
             self._remove_function(function)
             return
         if isinstance(function, OpenAIFunction):
             self._remove_function(function.name)
             return
         self._remove_function(function.__name__)
+
+    def __call__(self, input_data: FunctionCall) -> JsonType:
+        """Run the function with the given input data
+
+        Args:
+            input_data (FunctionCall): The input data from OpenAI
+
+        Returns:
+            JsonType: Your function's raw result
+        """
+        return self.run_function(input_data).result
```

### Comparing `openai_functions-0.5.1/openai_functions/functions/union.py` & `openai_functions-0.5.3/openai_functions/functions/union.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.1/openai_functions/functions/wrapper.py` & `openai_functions-0.5.3/openai_functions/functions/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class FunctionWrapper:
     """Wraps a function for jsonschema io"""
 
     def __init__(
         self,
-        func: Callable[..., JsonType],
+        func: Callable[..., Any],
         config: WrapperConfig | None = None,
     ) -> None:
         """Initialize a FunctionWrapper
 
         Args:
             func (Callable[..., JsonType]): The function to wrap
             config (WrapperConfig | None, optional): The configuration for the wrapper.
@@ -155,23 +155,25 @@
     @property
     def schema(self) -> dict[str, JsonType]:
         """Get the schema for this function
 
         Returns:
             dict[str, JsonType]: The schema
         """
-        return {
+        schema: dict[str, JsonType] = {
             "name": self.name,
-            "description": self.parsed_docs.short_description,
             "parameters": {
                 "type": "object",
                 "properties": self.arguments_schema,
                 "required": self.required_arguments,
             },
         }
+        if self.parsed_docs.short_description:
+            schema["description"] = self.parsed_docs.short_description
+        return schema
 
     def parse_argument(self, argument: inspect.Parameter) -> ArgSchemaParser:
         """Parse an argument
 
         Args:
             argument (inspect.Parameter): The argument to parse
 
@@ -199,17 +201,17 @@
             OrderedDict[str, Any]: The parsed arguments
         """
         return OrderedDict(
             (name, self.argument_parsers[name].parse_value(value))
             for name, value in arguments.items()
         )
 
-    def __call__(self, arguments: dict[str, JsonType]) -> JsonType:
+    def __call__(self, arguments: dict[str, JsonType]) -> Any:
         """Call the wrapped function
 
         Args:
             arguments (dict[str, JsonType]): The arguments to call the function with
 
         Returns:
-            JsonType: The result of the function
+            The result of the function
         """
         return self.func(**self.parse_arguments(arguments))
```

### Comparing `openai_functions-0.5.1/openai_functions/openai_types.py` & `openai_functions-0.5.3/openai_functions/openai_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
         Returns:
             FunctionCall | None: The function call
         """
         if self.message["role"] == "assistant":
             if self.message.get("content") is not None:
                 return None
-            return self.message.get("function_call")
+            return self.message.get("function_call")  # type: ignore
         return None
 
     @property
     def is_final_response(self) -> bool:
         """Check if the message is a final response
 
         Returns:
@@ -244,7 +244,16 @@
     Args:
         message (GenericMessage): The message to check
 
     Returns:
         TypeGuard[FinalResponseMessage]: Whether the message is a final response message
     """
     return message.is_final_response
+
+
+class ForcedFunctionCall(TypedDict):
+    """A type for forced function calls"""
+
+    name: str
+
+
+OpenAIFunctionCallInput = Union[ForcedFunctionCall, Literal["auto", "none"]]
```

### Comparing `openai_functions-0.5.1/openai_functions/parsers/abc.py` & `openai_functions-0.5.3/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.1/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.5.3/openai_functions/parsers/atomic_type_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,9 +30,9 @@
     def argument_schema(self) -> dict[str, JsonType]:
         return {
             "type": self.schema_type_name,
         }
 
     def parse_value(self, value: JsonType) -> T:
         if not isinstance(value, self._type):
-            raise TypeError(f"Expected {self._type()}, got {type(value)}")
+            raise TypeError(f"Expected {self._type}, got {type(value)}")
         return value
```

### Comparing `openai_functions-0.5.1/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.5.3/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.1/openai_functions/parsers/default.py` & `openai_functions-0.5.3/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.1/openai_functions/parsers/dict_parser.py` & `openai_functions-0.5.3/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.1/openai_functions/parsers/enum_parser.py` & `openai_functions-0.5.3/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.1/openai_functions/parsers/int_parser.py` & `openai_functions-0.5.3/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.1/openai_functions/parsers/list_parser.py` & `openai_functions-0.5.3/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.1/openai_functions/parsers/none_parser.py` & `openai_functions-0.5.3/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.1/openai_functions/parsers/union_parser.py` & `openai_functions-0.5.3/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.1/pyproject.toml` & `openai_functions-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.5.1"
+version = "0.5.3"
 description = ""
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "openai_functions"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `openai_functions-0.5.1/PKG-INFO` & `openai_functions-0.5.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.5.1
+Version: 0.5.3
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -69,29 +69,46 @@
         "temperature": "72",
         "unit": unit.value,
         "forecast": ["sunny", "windy"],
     }
     return weather_info
 ```
 
-4. Add user messages using the `conversation.add_message` method:
+4. Ask the AI a question:
 
 ```python
-conversation.add_message(
-    {
-        "role": "user",
-        "content": "What's the weather in San Francisco?",
-    }
-)
+conversation.ask("What's the weather in San Francisco?")
+```
+
+## Another usecase: data extraction
+
+1. Import the necessary modules:
+
+```python
+from dataclasses import dataclass
+import openai
+from openai_functions import nlp
+```
+
+3. Define your data container using the `@nlp` decorator:
+
+```python
+@nlp
+@dataclass
+class Person:
+    """Extract personal info"""
+
+    name: str
+    age: int
 ```
 
-5. Call the `conversation.run_until_response()` method to trigger the conversation and retrieve the response:
+4. Ask the AI for a summary of the data:
 
 ```python
-print(conversation.run_until_response())
+Person.nlp("I'm Jack and I'm 20 years old.", "Person")
 ```
 
 ## How it Works
 
 `openai-functions` takes care of the following tasks:
 
 - Parsing the function signatures and docstrings.
```

