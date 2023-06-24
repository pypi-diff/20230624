# Comparing `tmp/GPTConnect-0.1.5.tar.gz` & `tmp/GPTConnect-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTConnect-0.1.5.tar", last modified: Fri Jun 23 14:30:51 2023, max compression
+gzip compressed data, was "GPTConnect-0.1.6.tar", last modified: Sat Jun 24 03:59:26 2023, max compression
```

## Comparing `GPTConnect-0.1.5.tar` & `GPTConnect-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 14:30:51.118877 GPTConnect-0.1.5/
-drwxrwxrwx   0        0        0        0 2023-06-23 14:30:51.111906 GPTConnect-0.1.5/GPTConnect.egg-info/
--rw-rw-rw-   0        0        0      852 2023-06-23 14:30:50.000000 GPTConnect-0.1.5/GPTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-23 14:30:51.000000 GPTConnect-0.1.5/GPTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 14:30:50.000000 GPTConnect-0.1.5/GPTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 14:30:50.000000 GPTConnect-0.1.5/GPTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-23 14:30:50.000000 GPTConnect-0.1.5/GPTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      852 2023-06-23 14:30:51.117877 GPTConnect-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      666 2023-06-23 14:20:28.000000 GPTConnect-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 14:30:51.115879 GPTConnect-0.1.5/gptconnect/
--rw-rw-rw-   0        0        0       27 2023-06-23 13:36:18.000000 GPTConnect-0.1.5/gptconnect/__init__.py
--rw-rw-rw-   0        0        0     2605 2023-06-23 14:19:13.000000 GPTConnect-0.1.5/gptconnect/gptconnect.py
--rw-rw-rw-   0        0        0       42 2023-06-23 14:30:51.119878 GPTConnect-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      346 2023-06-23 14:30:44.000000 GPTConnect-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 03:59:26.749956 GPTConnect-0.1.6/
+drwxrwxrwx   0        0        0        0 2023-06-24 03:59:26.741429 GPTConnect-0.1.6/GPTConnect.egg-info/
+-rw-rw-rw-   0        0        0      855 2023-06-24 03:59:26.000000 GPTConnect-0.1.6/GPTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-24 03:59:26.000000 GPTConnect-0.1.6/GPTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 03:59:26.000000 GPTConnect-0.1.6/GPTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 03:59:26.000000 GPTConnect-0.1.6/GPTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 03:59:26.000000 GPTConnect-0.1.6/GPTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-06-24 03:59:26.749415 GPTConnect-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      669 2023-06-24 03:56:53.000000 GPTConnect-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 03:59:26.747412 GPTConnect-0.1.6/gptconnect/
+-rw-rw-rw-   0        0        0       55 2023-06-24 03:57:23.000000 GPTConnect-0.1.6/gptconnect/__init__.py
+-rw-rw-rw-   0        0        0     2104 2023-06-24 03:57:20.000000 GPTConnect-0.1.6/gptconnect/gptconnect.py
+-rw-rw-rw-   0        0        0      535 2023-06-24 03:57:20.000000 GPTConnect-0.1.6/gptconnect/gptfunction.py
+-rw-rw-rw-   0        0        0       42 2023-06-24 03:59:26.749956 GPTConnect-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      346 2023-06-24 03:57:39.000000 GPTConnect-0.1.6/setup.py
```

### Comparing `GPTConnect-0.1.5/GPTConnect.egg-info/PKG-INFO` & `GPTConnect-0.1.6/GPTConnect.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 
 # GPTConnect
 
 GPTConnect is a Python package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating, defining and interacting with GPT functions, making your development process smoother and more efficient.
@@ -15,8 +15,8 @@
 - Function groups system that allow easy integration of multiple commands at a time
 - More feautures coming soon! This package is only in early stages of development.
 
 ## Install
 `pip install GPTConnect`
 
 ## Demo
-[demo.py](https://github.com/SleepyStew/gptconnect/blob/master/demo.py)
+[demo.py](https://github.com/SleepyStew/gptconnect/blob/master/example.py)
```

### Comparing `GPTConnect-0.1.5/PKG-INFO` & `GPTConnect-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 
 # GPTConnect
 
 GPTConnect is a Python package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating, defining and interacting with GPT functions, making your development process smoother and more efficient.
@@ -15,8 +15,8 @@
 - Function groups system that allow easy integration of multiple commands at a time
 - More feautures coming soon! This package is only in early stages of development.
 
 ## Install
 `pip install GPTConnect`
 
 ## Demo
-[demo.py](https://github.com/SleepyStew/gptconnect/blob/master/demo.py)
+[demo.py](https://github.com/SleepyStew/gptconnect/blob/master/example.py)
```

### Comparing `GPTConnect-0.1.5/README.md` & `GPTConnect-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 - Function groups system that allow easy integration of multiple commands at a time
 - More feautures coming soon! This package is only in early stages of development.
 
 ## Install
 `pip install GPTConnect`
 
 ## Demo
-[demo.py](https://github.com/SleepyStew/gptconnect/blob/master/demo.py)
+[demo.py](https://github.com/SleepyStew/gptconnect/blob/master/example.py)
```

### Comparing `GPTConnect-0.1.5/gptconnect/gptconnect.py` & `GPTConnect-0.1.6/gptconnect/gptconnect.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,26 +62,7 @@
                 model=self._model, messages=messages, functions=function_details
             )
 
         return {
             "content": response.choices[-1].message.content,
             "function_called": function_call.name if function_call else None,
         }
-
-
-def GPTFunction(description: str = None, params: dict = None, group: str = None):
-    def decorator(function):
-        def wrapper(*args, **kwargs):
-            return function(*args, **kwargs)
-
-        details = {
-            "function": function,
-            "group": group,
-            "name": function.__name__,
-            "description": description,
-            "parameters": params,
-        }
-        functions.append(details)
-
-        return wrapper
-
-    return decorator
```

