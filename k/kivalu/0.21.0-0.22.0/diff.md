# Comparing `tmp/kivalu-0.21.0.tar.gz` & `tmp/kivalu-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivalu-0.21.0.tar", last modified: Fri May 12 17:59:40 2023, max compression
+gzip compressed data, was "kivalu-0.22.0.tar", last modified: Sat Jun 24 13:55:15 2023, max compression
```

## Comparing `kivalu-0.21.0.tar` & `kivalu-0.22.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 17:59:40.170964 kivalu-0.21.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-05-07 10:57:06.000000 kivalu-0.21.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-05-12 17:59:40.170964 kivalu-0.21.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 17:59:40.170964 kivalu-0.21.0/kivalu/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13449 2023-05-12 17:28:52.000000 kivalu-0.21.0/kivalu/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 17:59:40.170964 kivalu-0.21.0/kivalu.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-05-12 17:59:40.000000 kivalu-0.21.0/kivalu.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2023-05-12 17:59:40.000000 kivalu-0.21.0/kivalu.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-12 17:59:40.000000 kivalu-0.21.0/kivalu.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-05-12 17:59:40.000000 kivalu-0.21.0/kivalu.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-05-12 17:59:40.000000 kivalu-0.21.0/kivalu.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 17:59:40.170964 kivalu-0.21.0/scripts/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       52 2023-05-07 10:57:06.000000 kivalu-0.21.0/scripts/kivalu-setup
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-12 17:59:40.170964 kivalu-0.21.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-05-12 17:47:08.000000 kivalu-0.21.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 17:59:40.170964 kivalu-0.21.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1100 2023-05-12 16:53:14.000000 kivalu-0.21.0/tests/test_argumentparser.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8781 2023-05-12 17:28:52.000000 kivalu-0.21.0/tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1017 2023-05-12 16:53:14.000000 kivalu-0.21.0/tests/test_main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2203 2023-05-07 10:57:06.000000 kivalu-0.21.0/tests/test_server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 13:55:15.850455 kivalu-0.22.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-05-07 10:57:06.000000 kivalu-0.22.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-06-24 13:55:15.850455 kivalu-0.22.0/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 13:55:15.850455 kivalu-0.22.0/kivalu/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13483 2023-06-24 11:24:20.000000 kivalu-0.22.0/kivalu/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 13:55:15.850455 kivalu-0.22.0/kivalu.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-06-24 13:55:15.000000 kivalu-0.22.0/kivalu.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2023-06-24 13:55:15.000000 kivalu-0.22.0/kivalu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-24 13:55:15.000000 kivalu-0.22.0/kivalu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-06-24 13:55:15.000000 kivalu-0.22.0/kivalu.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-06-24 13:55:15.000000 kivalu-0.22.0/kivalu.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 13:55:15.850455 kivalu-0.22.0/scripts/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       52 2023-05-07 10:57:06.000000 kivalu-0.22.0/scripts/kivalu-setup
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-24 13:55:15.850455 kivalu-0.22.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-06-24 11:39:05.000000 kivalu-0.22.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 13:55:15.850455 kivalu-0.22.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1100 2023-05-12 16:53:14.000000 kivalu-0.22.0/tests/test_argumentparser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9095 2023-06-24 11:24:21.000000 kivalu-0.22.0/tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1017 2023-05-12 16:53:14.000000 kivalu-0.22.0/tests/test_main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2203 2023-05-07 10:57:06.000000 kivalu-0.22.0/tests/test_server.py
```

### Comparing `kivalu-0.21.0/LICENSE` & `kivalu-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kivalu-0.21.0/PKG-INFO` & `kivalu-0.22.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivalu
-Version: 0.21.0
+Version: 0.22.0
 Summary: Nested key-value system with built-in inheritance and templating, designed for configuration management
 Home-page: https://zebr0.io/projects/kivalu
 Download-URL: https://gitlab.com/zebr0/kivalu
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kivalu-0.21.0/kivalu/__init__.py` & `kivalu-0.22.0/kivalu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             self.extra_vars = extra_vars
         if timeout is not None:
             self.timeout = timeout
         if cache is not None:
             self.cache = cache
 
         # templating setup
-        self.jinja_environment = jinja2.Environment(keep_trailing_newline=True)
+        self.jinja_environment = jinja2.Environment(keep_trailing_newline=True, undefined=jinja2.StrictUndefined)
         self.jinja_environment.globals[URL] = self.url
         self.jinja_environment.globals[FAILOVER] = self.failover
         self.jinja_environment.globals[LEVELS] = self.levels
         self.jinja_environment.globals.update(self.extra_vars)
         self.jinja_environment.globals["configuration"] = json.dumps({URL: self.url, FAILOVER: self.failover, LEVELS: self.levels, EXTRA_VARS: self.extra_vars, TIMEOUT: self.timeout, CACHE: self.cache})
         self.jinja_environment.filters["get"] = self.get
         self.jinja_environment.filters["read"] = read
```

### Comparing `kivalu-0.21.0/kivalu.egg-info/PKG-INFO` & `kivalu-0.22.0/kivalu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivalu
-Version: 0.21.0
+Version: 0.22.0
 Summary: Nested key-value system with built-in inheritance and templating, designed for configuration management
 Home-page: https://zebr0.io/projects/kivalu
 Download-URL: https://gitlab.com/zebr0/kivalu
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kivalu-0.21.0/setup.py` & `kivalu-0.22.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="kivalu",
-    version="0.21.0",
+    version="0.22.0",
     description="Nested key-value system with built-in inheritance and templating, designed for configuration management",
     long_description="TODO",
     long_description_content_type="text/markdown",
     author="Thomas JOUANNOT",
     author_email="mazerty@gmail.com",
     url="https://zebr0.io/projects/kivalu",
     download_url="https://gitlab.com/zebr0/kivalu",
```

### Comparing `kivalu-0.21.0/tests/test_argumentparser.py` & `kivalu-0.22.0/tests/test_argumentparser.py`

 * *Files identical despite different names*

### Comparing `kivalu-0.21.0/tests/test_client.py` & `kivalu-0.22.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import http.server
 import time
 from pathlib import Path
 
+import jinja2.exceptions
 import pytest
 import requests.exceptions
 
 import kivalu
 
 
 def test_default_url():
@@ -109,22 +110,30 @@
 def test_render_with_default(server):
     server.data = {"template": "{{ 'missing_key' | get('default') }}"}
     client = kivalu.Client(url="http://127.0.0.1:8000", configuration_file=Path(""))
 
     assert client.get("template") == "default"
 
 
-def test_render_with_extra_vars(server):
+def test_render_with_extra_vars_ok(server):
     server.data = {"template": "{{ variable }}"}
     client = kivalu.Client(url="http://127.0.0.1:8000", configuration_file=Path(""), extra_vars={"variable": "lorem ipsum"})
 
     assert client.get("template") == "lorem ipsum"
     assert client.get("template", extra_vars={"variable": "dolor sit amet"}) == "dolor sit amet"
 
 
+def test_render_with_extra_vars_undefined_variable(server):
+    server.data = {"template": "{{ variable }}"}
+    client = kivalu.Client(url="http://127.0.0.1:8000", configuration_file=Path(""))
+
+    with pytest.raises(jinja2.exceptions.UndefinedError):
+        client.get("template")
+
+
 def test_read_ok(tmp_path, server):
     file = tmp_path.joinpath("file")
     file.write_text("content")
     server.data = {"template": "{{ '" + str(file) + "' | read }}"}
     client = kivalu.Client(url="http://127.0.0.1:8000", configuration_file=Path(""))
 
     assert client.get("template") == "content"
```

### Comparing `kivalu-0.21.0/tests/test_main.py` & `kivalu-0.22.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `kivalu-0.21.0/tests/test_server.py` & `kivalu-0.22.0/tests/test_server.py`

 * *Files identical despite different names*

