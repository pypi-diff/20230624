# Comparing `tmp/bantam-2.4.4.tar.gz` & `tmp/bantam-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.4.4.tar", last modified: Wed Jun 21 04:49:35 2023, max compression
+gzip compressed data, was "bantam-2.4.5.tar", last modified: Sat Jun 24 15:08:52 2023, max compression
```

## Comparing `bantam-2.4.4.tar` & `bantam-2.4.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.310540 bantam-2.4.4/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-21 04:49:35.310540 bantam-2.4.4/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.4/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.4/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-21 04:49:35.310540 bantam-2.4.4/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-21 04:49:13.000000 bantam-2.4.4/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.306540 bantam-2.4.4/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.306540 bantam-2.4.4/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.4/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    11963 2023-06-17 16:30:44.000000 bantam-2.4.4/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.306540 bantam-2.4.4/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.4/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.4/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22978 2023-06-21 04:48:21.000000 bantam-2.4.4/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.4/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.4.4/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    50578 2023-06-21 03:43:56.000000 bantam-2.4.4/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.4/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.4.4/src/bantam/js_async.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.306540 bantam-2.4.4/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-21 04:49:35.000000 bantam-2.4.4/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 04:49:35.310540 bantam-2.4.4/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     5623 2023-06-21 04:28:06.000000 bantam-2.4.4/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.4/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.4/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.4/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.4/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.4/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.4.4/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.4.4/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-24 15:08:52.821550 bantam-2.4.5/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.5/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.5/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-24 15:08:52.821550 bantam-2.4.5/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-24 15:07:51.000000 bantam-2.4.5/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.5/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    12161 2023-06-24 14:59:54.000000 bantam-2.4.5/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.5/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.5/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22978 2023-06-21 04:48:21.000000 bantam-2.4.5/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.5/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.4.5/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    50579 2023-06-24 15:02:24.000000 bantam-2.4.5/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.5/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20416 2023-06-24 14:57:43.000000 bantam-2.4.5/src/bantam/js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-24 15:08:52.000000 bantam-2.4.5/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-24 15:08:52.821550 bantam-2.4.5/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5623 2023-06-21 04:28:06.000000 bantam-2.4.5/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.5/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.5/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.5/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.5/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.5/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3029 2023-06-24 15:07:18.000000 bantam-2.4.5/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2831 2023-06-24 14:29:42.000000 bantam-2.4.5/test/test_js_async.py
```

### Comparing `bantam-2.4.4/PKG-INFO` & `bantam-2.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.4
+Version: 2.4.5
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.4
+Download-URL: https://github.com/bantam/dist/2.4.5
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.4/setup.py` & `bantam-2.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.4.4"
+VERSION = "2.4.5"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.4.4/src/bantam/__init__.py` & `bantam-2.4.5/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/src/bantam/api.py` & `bantam-2.4.5/src/bantam/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,24 +29,28 @@
         self._is_instance_method = is_instance_method
         self._is_static = not self._is_class_method and not self._is_instance_method
         self._expire_obj = expire_on_exit
         self._func = func
         self._real_func = func
         self._method = method
         self._timeout = timeout or ClientTimeout()
+        self._vararg = None
+        self._varkwds = None
         if 'return' not in annotations:
             raise TypeError(f"No annotation for return type in {func}")
         self._arg_annotations = {name: typ for name, typ in annotations.items() if name != 'return'}
         if not func.__name__.startswith('_'):
             sig = inspect.signature(func)
             for name in self._arg_annotations:
                 if sig.parameters[name].kind == inspect.Parameter.VAR_POSITIONAL:
                     self._arg_annotations[name] = typing.Tuple[int, None]
+                    self._vararg = name
                 elif sig.parameters[name].kind == inspect.Parameter.VAR_KEYWORD:
                     self._arg_annotations[name] = typing.Dict[str, self._arg_annotations[name]]
+                    self._varkwds = name
         self._async_arg_annotations = {
             name: typ for name, typ in self._arg_annotations.items()
             if typ in (bytes, AsyncChunkIterator, AsyncLineIterator)
         }
         if len(self._async_arg_annotations) > 1:
             raise TypeError("At most one parameter can be and async iterator in a web_api request")
         self._return_type = annotations['return']
@@ -154,14 +158,16 @@
         """
         takes list of kwargs for the call and transforms as needed for any varargs  or varkwargs in call
         """
         sig = inspect.signature(self._func)
         updated = kwargs
         varargs = tuple()
         for name, param in sig.parameters.items():
+            if name not in kwargs:
+                continue
             if param.kind == inspect.Parameter.VAR_KEYWORD:
                 del updated[name]
                 updated.update(**kwargs[name])
             elif param.kind == inspect.Parameter.VAR_POSITIONAL:
                 varargs = kwargs[name]
                 del updated[name]
         return updated, varargs
```

### Comparing `bantam-2.4.4/src/bantam/autogen/main.py` & `bantam-2.4.5/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/src/bantam/client.py` & `bantam-2.4.5/src/bantam/client.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/src/bantam/conversions.py` & `bantam-2.4.5/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/src/bantam/decorators.py` & `bantam-2.4.5/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/src/bantam/http.py` & `bantam-2.4.5/src/bantam/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -939,15 +939,15 @@
                 if isinstance(api.clazz, tuple):
                     module_name, class_name = api.clazz
                     api._clazz = getattr(sys.modules.get(module_name), class_name)
                 kwargs, varargs = api.update_varargs(kwargs)
                 awaitable = api(api.clazz, *varargs, **kwargs)
             else:
                 kwargs, varargs = api.update_varargs(kwargs)
-                awaitable = api(*varags, **kwargs)
+                awaitable = api(*varargs, **kwargs)
             if inspect.isasyncgen(awaitable):
                 #################
                 #  streamed response through async generator:
                 #################
                 # underlying function has yielded a result rather than turning
                 # process the yielded value and allow execution to resume from yielding task
                 async_q = asyncio.Queue()
```

### Comparing `bantam-2.4.4/src/bantam/js.py` & `bantam-2.4.5/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/src/bantam/js_async.py` & `bantam-2.4.5/src/bantam/js_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,15 +400,15 @@
         try:
             api_doc = docs.generate(api=api,
                                     flavor=APIDoc.Flavor.JAVASCRIPT, indent=tab)
         except Exception as e:
             api_doc = f"/**\n<<Unable to generate>> {e}\n**/\n"
         out.write(b'\n')
         out.write(api_doc.encode('utf-8'))
-        argnames = list(api.arg_annotations.keys())
+        argnames = [k for k in api.arg_annotations.keys() if k not in [api._vararg, api._varkwds]]
         if api.is_constructor:
             if api.name == '_create':
                 out.write(
                     f"{tab}constructor({', '.join(argnames)}) {{\n".encode(
                         cls.ENCODING))
             else:
                 out.write(
```

### Comparing `bantam-2.4.4/src/bantam.egg-info/PKG-INFO` & `bantam-2.4.5/src/bantam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.4
+Version: 2.4.5
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.4
+Download-URL: https://github.com/bantam/dist/2.4.5
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.4/src/bantam.egg-info/SOURCES.txt` & `bantam-2.4.5/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/test/test_client_get.py` & `bantam-2.4.5/test/test_client_get.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/test/test_client_post.py` & `bantam-2.4.5/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/test/test_client_post_inherited_apis.py` & `bantam-2.4.5/test/test_client_post_inherited_apis.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/test/test_conversions.py` & `bantam-2.4.5/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/test/test_decorators.py` & `bantam-2.4.5/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.4/test/test_js.py` & `bantam-2.4.5/test/test_js.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 import pytest
 from aiohttp.web_request import Request
 from aiohttp.web_response import Response, StreamResponse
 
 from bantam.http import WebApplication
 
 
+PORT = 8089
+
+
 class TestJavascriptGenerator:
 
     @pytest.mark.asyncio
     async def test_generate_basic(self):
         def assert_preprocessor(request: Request) -> Dict[str, Any]:
             assert isinstance(request, Request), "Failed to get valid response on pre-processing"
             return {}
@@ -49,17 +52,17 @@
                 with suppress(Exception):
                     browser = webbrowser.get("firefox")
                     flags = ["-new-instance"]
             if not browser:
                 os.write(sys.stderr.fileno(),
                          b"UNABLE TO GET BROWSER SUPPORT HEADLESS CONFIGURATION. DEFAULTING TO NON_HEADLESSS")
                 browser = webbrowser.get()
-            browser.open("http://localhost:8080/static/index.html")
+            browser.open(f"http://localhost:{PORT}/static/index.html")
 
-        app_task = asyncio.create_task(app.start(modules=['class_js_test']))
+        app_task = asyncio.create_task(app.start(modules=['class_js_test'], port=PORT))
         browser_task = asyncio.create_task(launch_browser())
         try:
             result = await asyncio.wait_for(RestAPIExample.result_queue.get(), timeout=120)
             if result != 'PASSED':
                 await asyncio.sleep(2.0)
         except Exception as e:
             await asyncio.sleep(2.0)
```

### Comparing `bantam-2.4.4/test/test_js_async.py` & `bantam-2.4.5/test/test_js_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import asyncio
 import json
 import os
-import sys
 import traceback
 import webbrowser
 from contextlib import suppress
 from pathlib import Path
-from typing import AsyncIterator, Optional, Dict, Any, List
+from typing import Dict, Any
 
 import pytest
 from aiohttp.web_request import Request
 from aiohttp.web_response import Response
 from bantam.http import WebApplication
 
 
 import sys
 sys.path.insert(0, os.path.dirname(__file__))
 from class_rest_get import RestAPIExampleAsync
 
 
+PORT = 8082
+
+
 class TestJavascriptGenerator:
 
     @pytest.mark.asyncio
     async def test_generate_basic(self):
         def assert_preprocessor(request: Request) -> Dict[str, Any]:
             assert isinstance(request, Request), "Failed to get valid response on pre-processing"
             return {}
@@ -47,22 +49,22 @@
                     browser = webbrowser.get("google-chrome")
                 if not browser:
                     browser = webbrowser.get()
             if not browser:
                 os.write(sys.stderr.fileno(),
                          b"UNABLE TO GET BROWSER SUPPORT IN HEADLESS CONFIGURATION. DEFAULTING TO NON_HEADLESS")
                 browser = webbrowser.get()
-            browser.open("http://localhost:8081/static/index_async.html")
+            browser.open(f"http://localhost:{PORT}/static/index_async.html")
             result = await RestAPIExampleAsync.result_queue.get()
             await asyncio.sleep(2.0)
             await app.shutdown()
             return result
 
         try:
-            completed, _ = await asyncio.wait([app.start(modules=['class_rest_get'], port=8081),
+            completed, _ = await asyncio.wait([app.start(modules=['class_rest_get'], port=PORT),
                                                launch_browser()], timeout=100000, return_when=asyncio.FIRST_COMPLETED)
             results = [c.result() for c in completed if c is not None]
         except Exception as e:
             assert False, f"Exception processing javascript results: {traceback.format_exc()}"
         if any([isinstance(r, Exception) for r in results]):
             assert False, "At least one javascript test failed. See browser window for details"
         assert results[0] == "PASSED", \
```

