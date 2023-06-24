# Comparing `tmp/GPTConnect-0.1.8.tar.gz` & `tmp/GPTConnect-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTConnect-0.1.8.tar", last modified: Sat Jun 24 07:57:52 2023, max compression
+gzip compressed data, was "GPTConnect-0.1.9.tar", last modified: Sat Jun 24 09:36:49 2023, max compression
```

## Comparing `GPTConnect-0.1.8.tar` & `GPTConnect-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 07:57:52.477044 GPTConnect-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-06-24 07:57:52.468080 GPTConnect-0.1.8/GPTConnect.egg-info/
--rw-rw-rw-   0        0        0     1061 2023-06-24 07:57:52.000000 GPTConnect-0.1.8/GPTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-06-24 07:57:52.000000 GPTConnect-0.1.8/GPTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 07:57:52.000000 GPTConnect-0.1.8/GPTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 07:57:52.000000 GPTConnect-0.1.8/GPTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 07:57:52.000000 GPTConnect-0.1.8/GPTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1061 2023-06-24 07:57:52.476043 GPTConnect-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      875 2023-06-24 07:57:09.000000 GPTConnect-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 07:57:52.474038 GPTConnect-0.1.8/gptconnect/
--rw-rw-rw-   0        0        0       55 2023-06-24 03:57:23.000000 GPTConnect-0.1.8/gptconnect/__init__.py
--rw-rw-rw-   0        0        0     2647 2023-06-24 07:56:11.000000 GPTConnect-0.1.8/gptconnect/gptconnect.py
--rw-rw-rw-   0        0        0      807 2023-06-24 07:31:10.000000 GPTConnect-0.1.8/gptconnect/gptfunction.py
--rw-rw-rw-   0        0        0       42 2023-06-24 07:57:52.477044 GPTConnect-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      364 2023-06-24 07:57:49.000000 GPTConnect-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:36:49.137951 GPTConnect-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-06-24 09:36:49.126908 GPTConnect-0.1.9/GPTConnect.egg-info/
+-rw-rw-rw-   0        0        0     1061 2023-06-24 09:36:48.000000 GPTConnect-0.1.9/GPTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-24 09:36:49.000000 GPTConnect-0.1.9/GPTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 09:36:48.000000 GPTConnect-0.1.9/GPTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 09:36:48.000000 GPTConnect-0.1.9/GPTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 09:36:49.000000 GPTConnect-0.1.9/GPTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1061 2023-06-24 09:36:49.136950 GPTConnect-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      875 2023-06-24 07:57:09.000000 GPTConnect-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 09:36:49.134945 GPTConnect-0.1.9/gptconnect/
+-rw-rw-rw-   0        0        0       90 2023-06-24 09:26:23.000000 GPTConnect-0.1.9/gptconnect/__init__.py
+-rw-rw-rw-   0        0        0     2830 2023-06-24 09:31:52.000000 GPTConnect-0.1.9/gptconnect/gptconnect.py
+-rw-rw-rw-   0        0        0      807 2023-06-24 07:31:10.000000 GPTConnect-0.1.9/gptconnect/gptfunction.py
+-rw-rw-rw-   0        0        0      453 2023-06-24 09:33:05.000000 GPTConnect-0.1.9/gptconnect/gptfunctionhandler.py
+-rw-rw-rw-   0        0        0       42 2023-06-24 09:36:49.137951 GPTConnect-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      364 2023-06-24 09:34:31.000000 GPTConnect-0.1.9/setup.py
```

### Comparing `GPTConnect-0.1.8/GPTConnect.egg-info/PKG-INFO` & `GPTConnect-0.1.9/GPTConnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 
 # GPTConnect
 
 GPTConnect is a Python 🐍 package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating and interacting with GPT functions, making your development process smoother and more efficient.
```

### Comparing `GPTConnect-0.1.8/PKG-INFO` & `GPTConnect-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 
 # GPTConnect
 
 GPTConnect is a Python 🐍 package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating and interacting with GPT functions, making your development process smoother and more efficient.
```

### Comparing `GPTConnect-0.1.8/README.md` & `GPTConnect-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `GPTConnect-0.1.8/gptconnect/gptconnect.py` & `GPTConnect-0.1.9/gptconnect/gptconnect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from typing import Union
 import openai
 import copy
 
+
 valid_models = ["gpt-3.5-turbo-0613", "gpt-4-0613", "gpt-4-32k-0613"]
 functions = []
 
 
 class GPTConnect:
     """
     The main class for working with GPTConnect
@@ -63,15 +64,20 @@
 
         if function_call:
             function = [
                 f["function"] for f in functions if f.get("name") == function_call.name
             ][0]
             context = json.loads(function_call.arguments)
 
-            call = function(context)
+            from .gptfunctionhandler import function_handler
+
+            if function_handler:
+                call = function_handler(function, context)
+            else:
+                call = function(context)
 
             messages.append(
                 {"role": "function", "name": function_call.name, "content": str(call)}
             )
 
             response = openai.ChatCompletion.create(
                 model=self._model, messages=messages, functions=function_details
```

### Comparing `GPTConnect-0.1.8/gptconnect/gptfunction.py` & `GPTConnect-0.1.9/gptconnect/gptfunction.py`

 * *Files identical despite different names*

