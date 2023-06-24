# Comparing `tmp/GPTConnect-0.1.6.tar.gz` & `tmp/GPTConnect-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTConnect-0.1.6.tar", last modified: Sat Jun 24 03:59:26 2023, max compression
+gzip compressed data, was "GPTConnect-0.1.7.tar", last modified: Sat Jun 24 07:34:27 2023, max compression
```

## Comparing `GPTConnect-0.1.6.tar` & `GPTConnect-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 03:59:26.749956 GPTConnect-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-06-24 03:59:26.741429 GPTConnect-0.1.6/GPTConnect.egg-info/
--rw-rw-rw-   0        0        0      855 2023-06-24 03:59:26.000000 GPTConnect-0.1.6/GPTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-06-24 03:59:26.000000 GPTConnect-0.1.6/GPTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 03:59:26.000000 GPTConnect-0.1.6/GPTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 03:59:26.000000 GPTConnect-0.1.6/GPTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 03:59:26.000000 GPTConnect-0.1.6/GPTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-06-24 03:59:26.749415 GPTConnect-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      669 2023-06-24 03:56:53.000000 GPTConnect-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 03:59:26.747412 GPTConnect-0.1.6/gptconnect/
--rw-rw-rw-   0        0        0       55 2023-06-24 03:57:23.000000 GPTConnect-0.1.6/gptconnect/__init__.py
--rw-rw-rw-   0        0        0     2104 2023-06-24 03:57:20.000000 GPTConnect-0.1.6/gptconnect/gptconnect.py
--rw-rw-rw-   0        0        0      535 2023-06-24 03:57:20.000000 GPTConnect-0.1.6/gptconnect/gptfunction.py
--rw-rw-rw-   0        0        0       42 2023-06-24 03:59:26.749956 GPTConnect-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      346 2023-06-24 03:57:39.000000 GPTConnect-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:34:27.074041 GPTConnect-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-06-24 07:34:27.064801 GPTConnect-0.1.7/GPTConnect.egg-info/
+-rw-rw-rw-   0        0        0      855 2023-06-24 07:34:26.000000 GPTConnect-0.1.7/GPTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-24 07:34:26.000000 GPTConnect-0.1.7/GPTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 07:34:26.000000 GPTConnect-0.1.7/GPTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 07:34:26.000000 GPTConnect-0.1.7/GPTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 07:34:26.000000 GPTConnect-0.1.7/GPTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-06-24 07:34:27.073041 GPTConnect-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      669 2023-06-24 03:56:53.000000 GPTConnect-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 07:34:27.071064 GPTConnect-0.1.7/gptconnect/
+-rw-rw-rw-   0        0        0       55 2023-06-24 03:57:23.000000 GPTConnect-0.1.7/gptconnect/__init__.py
+-rw-rw-rw-   0        0        0     2639 2023-06-24 07:34:03.000000 GPTConnect-0.1.7/gptconnect/gptconnect.py
+-rw-rw-rw-   0        0        0      807 2023-06-24 07:31:10.000000 GPTConnect-0.1.7/gptconnect/gptfunction.py
+-rw-rw-rw-   0        0        0       42 2023-06-24 07:34:27.074041 GPTConnect-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      346 2023-06-24 07:34:20.000000 GPTConnect-0.1.7/setup.py
```

### Comparing `GPTConnect-0.1.6/GPTConnect.egg-info/PKG-INFO` & `GPTConnect-0.1.7/GPTConnect.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 
 # GPTConnect
 
 GPTConnect is a Python package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating, defining and interacting with GPT functions, making your development process smoother and more efficient.
```

### Comparing `GPTConnect-0.1.6/PKG-INFO` & `GPTConnect-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 
 # GPTConnect
 
 GPTConnect is a Python package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating, defining and interacting with GPT functions, making your development process smoother and more efficient.
```

### Comparing `GPTConnect-0.1.6/README.md` & `GPTConnect-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `GPTConnect-0.1.6/gptconnect/gptfunction.py` & `GPTConnect-0.1.7/gptconnect/gptfunction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 from gptconnect import functions
 
 
-def GPTFunction(description: str = None, params: dict = None, group: str = None):
+def GPTFunction(
+    group: str = None, description: str = None, params: dict = None
+) -> callable:
+    """
+    Decorator for creating a GPT function
+
+    :param group: The group of the function
+    :param description: The description of the function
+    :param params: The parameters of the function, in OpenAI's standard JSON format
+    """
+
     def decorator(function):
         def wrapper(*args, **kwargs):
             return function(*args, **kwargs)
 
         details = {
             "function": function,
             "group": group,
```

