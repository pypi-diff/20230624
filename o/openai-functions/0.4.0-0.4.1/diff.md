# Comparing `tmp/openai_functions-0.4.0.tar.gz` & `tmp/openai_functions-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.4.0.tar", max compression
+gzip compressed data, was "openai_functions-0.4.1.tar", max compression
```

## Comparing `openai_functions-0.4.0.tar` & `openai_functions-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2689 2023-06-23 21:23:30.745575 openai_functions-0.4.0/README.md
--rw-r--r--   0        0        0      385 2023-06-23 21:21:35.696216 openai_functions-0.4.0/openai_functions/__init__.py
--rw-r--r--   0        0        0    12507 2023-06-23 21:20:40.873554 openai_functions-0.4.0/openai_functions/conversation.py
--rw-r--r--   0        0        0     6245 2023-06-23 20:59:37.510332 openai_functions-0.4.0/openai_functions/function_wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.4.0/openai_functions/json_type.py
--rw-r--r--   0        0        0     4042 2023-06-23 21:18:19.040787 openai_functions-0.4.0/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.4.0/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.4.0/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.4.0/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.4.0/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.4.0/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.4.0/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.4.0/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.4.0/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.4.0/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.4.0/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.4.0/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.4.0/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.4.0/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.4.0/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.4.0/openai_functions/py.typed
--rw-r--r--   0        0        0      557 2023-06-23 21:28:18.697839 openai_functions-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3291 1970-01-01 00:00:00.000000 openai_functions-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2689 2023-06-23 21:23:30.745575 openai_functions-0.4.1/README.md
+-rw-r--r--   0        0        0      385 2023-06-23 21:21:35.696216 openai_functions-0.4.1/openai_functions/__init__.py
+-rw-r--r--   0        0        0    12813 2023-06-23 22:09:12.725627 openai_functions-0.4.1/openai_functions/conversation.py
+-rw-r--r--   0        0        0     6245 2023-06-23 20:59:37.510332 openai_functions-0.4.1/openai_functions/function_wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.4.1/openai_functions/json_type.py
+-rw-r--r--   0        0        0     6376 2023-06-23 22:09:07.677576 openai_functions-0.4.1/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.4.1/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.4.1/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.4.1/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.4.1/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.4.1/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.4.1/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.4.1/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.4.1/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.4.1/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.4.1/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.4.1/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.4.1/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.4.1/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.4.1/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.4.1/openai_functions/py.typed
+-rw-r--r--   0        0        0      557 2023-06-23 22:10:29.877403 openai_functions-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3291 1970-01-01 00:00:00.000000 openai_functions-0.4.1/PKG-INFO
```

### Comparing `openai_functions-0.4.0/README.md` & `openai_functions-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/openai_functions/conversation.py` & `openai_functions-0.4.1/openai_functions/conversation.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import openai
 
 from .function_wrapper import FunctionWrapper, WrapperConfig
 from .openai_types import (
     FinalResponseMessage,
     FunctionMessageType,
+    GenericMessage,
     Message,
     is_final_response_message,
 )
 
 if TYPE_CHECKING:
     from .json_type import JsonType
     from .openai_types import FunctionCall, MessageType, NonFunctionMessageType
@@ -27,39 +28,44 @@
         ...
 
     @property
     def schema(self) -> JsonType:
         """Get the schema for this function"""
 
     @property
-    def name(self) -> str:  # type: ignore
+    def name(self) -> str:
         """Get the name of this function"""
+        # This ellipsis is for Pyright #2758
+        ...  # pylint: disable=unnecessary-ellipsis
 
     @property
-    def save_return(self) -> bool:  # type: ignore
+    def save_return(self) -> bool:
         """Get whether to save the return value of this function"""
+        ...  # pylint: disable=unnecessary-ellipsis
 
     @property
-    def serialize(self) -> bool:  # type: ignore
+    def serialize(self) -> bool:
         """Get whether to continue running after this function"""
+        ...  # pylint: disable=unnecessary-ellipsis
 
     @property
-    def interpret_as_response(self) -> bool:  # type: ignore
+    def interpret_as_response(self) -> bool:
         """Get whether to interpret the return value of this function as a response"""
+        ...  # pylint: disable=unnecessary-ellipsis
 
 
 class Conversation:
     """A class for running OpenAI functions"""
 
     def __init__(
         self,
         functions: list[OpenAIFunction] | None = None,
         model: str = "gpt-3.5-turbo-0613",
     ) -> None:
-        self.messages: list[Message] = []
+        self.messages: list[GenericMessage] = []
         self.functions = functions or []
         self.model = model
 
     @property
     def functions_schema(self) -> JsonType:
         """Get the functions schema
 
@@ -81,50 +87,50 @@
             TypeError: If the input data is not a dictionary
             ValueError: If the function is not found
         """
         return self.find_function(input_data["name"])(
             json.loads(input_data["arguments"])
         )
 
-    def _add_message(self, message: Message) -> None:
+    def _add_message(self, message: GenericMessage) -> None:
         """Add a message
 
         Args:
-            message (Message): The message
+            message (GenericMessage): The message
         """
         self.messages.append(message)
 
-    def add_message(self, message: Message | MessageType | str) -> None:
+    def add_message(self, message: GenericMessage | MessageType | str) -> None:
         """Add a message
 
         Args:
-            message (Message | MessageType | str): The message
+            message (GenericMessage | MessageType | str): The message
         """
-        if isinstance(message, Message):
+        if isinstance(message, GenericMessage):
             self._add_message(message)
         else:
             self._add_message(Message(message))
 
-    def add_messages(self, messages: list[Message | MessageType]) -> None:
+    def add_messages(self, messages: list[GenericMessage | MessageType]) -> None:
         """Add messages
 
         Args:
-            messages (list[Message | MessageType]): The messages
+            messages (list[GenericMessage | MessageType]): The messages
         """
         for message in messages:
             self.add_message(message)
 
-    def pop_message(self, index: int = -1) -> Message:
+    def pop_message(self, index: int = -1) -> GenericMessage:
         """Pop a message
 
         Args:
             index (int): The index. Defaults to -1.
 
         Returns:
-            Message: The message
+            GenericMessage: The message
         """
         return self.messages.pop(index)
 
     def clear_messages(self) -> None:
         """Clear the messages"""
         self.messages = []
 
@@ -278,32 +284,32 @@
 
         function_call = self.messages[-1].function_call
         if not function_call:
             return False
 
         return self.run_function_and_substitute(function_call)
 
-    def generate_message(self) -> Message:
+    def generate_message(self) -> GenericMessage:
         """Generate the next message
 
         Returns:
-            Message: The response
+            GenericMessage: The response
         """
         if self.run_function_if_needed():
             return self.messages[-1]
 
         message = self._generate_message()
         self.add_message(message)
         return Message(message)
 
     def run_until_response(self) -> FinalResponseMessage:
         """Run until a response is generated
 
         Returns:
-            Message: The response
+            FinalResponseMessage: The response
         """
         while True:
             message = self.generate_message()
             if is_final_response_message(message):
                 return message
 
     def _add_function(self, function: OpenAIFunction) -> None:
```

### Comparing `openai_functions-0.4.0/openai_functions/function_wrapper.py` & `openai_functions-0.4.1/openai_functions/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/openai_functions/parsers/abc.py` & `openai_functions-0.4.1/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.4.1/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.4.1/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/openai_functions/parsers/default.py` & `openai_functions-0.4.1/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/openai_functions/parsers/dict_parser.py` & `openai_functions-0.4.1/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/openai_functions/parsers/enum_parser.py` & `openai_functions-0.4.1/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/openai_functions/parsers/int_parser.py` & `openai_functions-0.4.1/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/openai_functions/parsers/list_parser.py` & `openai_functions-0.4.1/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/openai_functions/parsers/none_parser.py` & `openai_functions-0.4.1/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/openai_functions/parsers/union_parser.py` & `openai_functions-0.4.1/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.4.0/pyproject.toml` & `openai_functions-0.4.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "openai_functions"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `openai_functions-0.4.0/PKG-INFO` & `openai_functions-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

