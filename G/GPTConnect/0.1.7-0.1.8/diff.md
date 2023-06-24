# Comparing `tmp/GPTConnect-0.1.7.tar.gz` & `tmp/GPTConnect-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTConnect-0.1.7.tar", last modified: Sat Jun 24 07:34:27 2023, max compression
+gzip compressed data, was "GPTConnect-0.1.8.tar", last modified: Sat Jun 24 07:57:52 2023, max compression
```

## Comparing `GPTConnect-0.1.7.tar` & `GPTConnect-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 07:34:27.074041 GPTConnect-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-06-24 07:34:27.064801 GPTConnect-0.1.7/GPTConnect.egg-info/
--rw-rw-rw-   0        0        0      855 2023-06-24 07:34:26.000000 GPTConnect-0.1.7/GPTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-06-24 07:34:26.000000 GPTConnect-0.1.7/GPTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 07:34:26.000000 GPTConnect-0.1.7/GPTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 07:34:26.000000 GPTConnect-0.1.7/GPTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 07:34:26.000000 GPTConnect-0.1.7/GPTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-06-24 07:34:27.073041 GPTConnect-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      669 2023-06-24 03:56:53.000000 GPTConnect-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 07:34:27.071064 GPTConnect-0.1.7/gptconnect/
--rw-rw-rw-   0        0        0       55 2023-06-24 03:57:23.000000 GPTConnect-0.1.7/gptconnect/__init__.py
--rw-rw-rw-   0        0        0     2639 2023-06-24 07:34:03.000000 GPTConnect-0.1.7/gptconnect/gptconnect.py
--rw-rw-rw-   0        0        0      807 2023-06-24 07:31:10.000000 GPTConnect-0.1.7/gptconnect/gptfunction.py
--rw-rw-rw-   0        0        0       42 2023-06-24 07:34:27.074041 GPTConnect-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      346 2023-06-24 07:34:20.000000 GPTConnect-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:57:52.477044 GPTConnect-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-06-24 07:57:52.468080 GPTConnect-0.1.8/GPTConnect.egg-info/
+-rw-rw-rw-   0        0        0     1061 2023-06-24 07:57:52.000000 GPTConnect-0.1.8/GPTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-24 07:57:52.000000 GPTConnect-0.1.8/GPTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 07:57:52.000000 GPTConnect-0.1.8/GPTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 07:57:52.000000 GPTConnect-0.1.8/GPTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 07:57:52.000000 GPTConnect-0.1.8/GPTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1061 2023-06-24 07:57:52.476043 GPTConnect-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      875 2023-06-24 07:57:09.000000 GPTConnect-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 07:57:52.474038 GPTConnect-0.1.8/gptconnect/
+-rw-rw-rw-   0        0        0       55 2023-06-24 03:57:23.000000 GPTConnect-0.1.8/gptconnect/__init__.py
+-rw-rw-rw-   0        0        0     2647 2023-06-24 07:56:11.000000 GPTConnect-0.1.8/gptconnect/gptconnect.py
+-rw-rw-rw-   0        0        0      807 2023-06-24 07:31:10.000000 GPTConnect-0.1.8/gptconnect/gptfunction.py
+-rw-rw-rw-   0        0        0       42 2023-06-24 07:57:52.477044 GPTConnect-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      364 2023-06-24 07:57:49.000000 GPTConnect-0.1.8/setup.py
```

### Comparing `GPTConnect-0.1.7/GPTConnect.egg-info/PKG-INFO` & `GPTConnect-0.1.8/GPTConnect.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 
 # GPTConnect
 
-GPTConnect is a Python package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating, defining and interacting with GPT functions, making your development process smoother and more efficient.
+GPTConnect is a Python 🐍 package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating and interacting with GPT functions, making your development process smoother and more efficient.
+
+Make sure to star this project if you find it useful! ✨
+
+If you have any ideas, bug reports or suggestions feel free to open an issue or contact me on discord at @**sleepystew**
 
 ## Features
 
-- Simplified and intuitive decorator based system to define GPT functions.
-- Function groups system that allow easy integration of multiple commands at a time
-- More feautures coming soon! This package is only in early stages of development.
+- 🎉 Simplified and intuitive decorator based system to define GPT functions.
+- 🔤 Function groups system that allow easy integration of multiple commands at a time
+- 🕐 More features coming soon! This package is only in early stages of development.
 
 ## Install
 `pip install GPTConnect`
 
-## Demo
-[demo.py](https://github.com/SleepyStew/gptconnect/blob/master/example.py)
+## Example Usage
+[example.py](https://github.com/SleepyStew/gptconnect/blob/master/example.py)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `GPTConnect-0.1.7/PKG-INFO` & `GPTConnect-0.1.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 
 # GPTConnect
 
-GPTConnect is a Python package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating, defining and interacting with GPT functions, making your development process smoother and more efficient.
+GPTConnect is a Python 🐍 package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating and interacting with GPT functions, making your development process smoother and more efficient.
+
+Make sure to star this project if you find it useful! ✨
+
+If you have any ideas, bug reports or suggestions feel free to open an issue or contact me on discord at @**sleepystew**
 
 ## Features
 
-- Simplified and intuitive decorator based system to define GPT functions.
-- Function groups system that allow easy integration of multiple commands at a time
-- More feautures coming soon! This package is only in early stages of development.
+- 🎉 Simplified and intuitive decorator based system to define GPT functions.
+- 🔤 Function groups system that allow easy integration of multiple commands at a time
+- 🕐 More features coming soon! This package is only in early stages of development.
 
 ## Install
 `pip install GPTConnect`
 
-## Demo
-[demo.py](https://github.com/SleepyStew/gptconnect/blob/master/example.py)
+## Example Usage
+[example.py](https://github.com/SleepyStew/gptconnect/blob/master/example.py)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `GPTConnect-0.1.7/gptconnect/gptconnect.py` & `GPTConnect-0.1.8/gptconnect/gptconnect.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ) -> dict:
         """
         Make a ChatGPT Completion with a prompt or list of messages, and function group
 
         :param prompt: The prompt to provide
         :param function_group: The function group to use
         :param messages: The messages to provide as context
-        :return: A dictionary containing the function if called and the response choices from OpenAI
+        :return: A dictionary containing the function if called, and the content of the response from OpenAI
         """
         if not prompt and not messages:
             raise ValueError("Prompt or messages must be provided")
 
         if not messages:
             messages = [{"role": "user", "content": prompt}]
```

### Comparing `GPTConnect-0.1.7/gptconnect/gptfunction.py` & `GPTConnect-0.1.8/gptconnect/gptfunction.py`

 * *Files identical despite different names*

