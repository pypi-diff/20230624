# Comparing `tmp/im_openai-0.1.1.tar.gz` & `tmp/im_openai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im_openai-0.1.1.tar", last modified: Fri Jun 23 21:34:05 2023, max compression
+gzip compressed data, was "im_openai-0.1.2.tar", last modified: Fri Jun 23 21:57:33 2023, max compression
```

## Comparing `im_openai-0.1.1.tar` & `im_openai-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:34:05.370837 im_openai-0.1.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.1.1/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       89 2023-06-20 23:30:14.000000 im_openai-0.1.1/HISTORY.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.1.1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.1.1/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2420 2023-06-23 21:34:05.371521 im_openai-0.1.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1560 2023-06-21 23:37:53.000000 im_openai-0.1.1/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:34:05.307278 im_openai-0.1.1/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/authors.rst
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/history.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/installation.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.1.1/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/usage.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:34:05.330614 im_openai-0.1.1/im_openai/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-06-23 16:59:08.000000 im_openai-0.1.1/im_openai/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1610 2023-06-23 21:03:40.000000 im_openai-0.1.1/im_openai/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1755 2023-06-21 23:21:08.000000 im_openai-0.1.1/im_openai/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      390 2023-06-23 16:58:54.000000 im_openai-0.1.1/im_openai/template.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:34:05.361307 im_openai-0.1.1/im_openai.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2420 2023-06-23 21:34:05.000000 im_openai-0.1.1/im_openai.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      543 2023-06-23 21:34:05.000000 im_openai-0.1.1/im_openai.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-23 21:34:05.000000 im_openai-0.1.1/im_openai.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-23 21:34:05.000000 im_openai-0.1.1/im_openai.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-06-23 21:34:05.000000 im_openai-0.1.1/im_openai.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-06-23 21:34:05.376457 im_openai-0.1.1/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1351 2023-06-23 21:33:09.000000 im_openai-0.1.1/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:34:05.368318 im_openai-0.1.1/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.1.1/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.1.1/tests/test_im_openai.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:57:33.822033 im_openai-0.1.2/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.1.2/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.1.2/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.1.2/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2555 2023-06-23 21:57:33.823740 im_openai-0.1.2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1560 2023-06-21 23:37:53.000000 im_openai-0.1.2/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:57:33.784705 im_openai-0.1.2/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.1.2/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.1.2/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.1.2/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.1.2/docs/history.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.1.2/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.1.2/docs/installation.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.1.2/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.1.2/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.1.2/docs/usage.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:57:33.797818 im_openai-0.1.2/im_openai/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-06-23 16:59:08.000000 im_openai-0.1.2/im_openai/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1799 2023-06-23 21:48:36.000000 im_openai-0.1.2/im_openai/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1755 2023-06-21 23:21:08.000000 im_openai-0.1.2/im_openai/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.1.2/im_openai/template.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:57:33.814635 im_openai-0.1.2/im_openai.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2555 2023-06-23 21:57:33.000000 im_openai-0.1.2/im_openai.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      531 2023-06-23 21:57:33.000000 im_openai-0.1.2/im_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-23 21:57:33.000000 im_openai-0.1.2/im_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-23 21:57:33.000000 im_openai-0.1.2/im_openai.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-06-23 21:57:33.000000 im_openai-0.1.2/im_openai.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-06-23 21:57:33.826054 im_openai-0.1.2/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-06-23 21:57:20.000000 im_openai-0.1.2/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:57:33.819989 im_openai-0.1.2/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.1.2/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.1.2/tests/test_im_openai.py
```

### Comparing `im_openai-0.1.1/CONTRIBUTING.rst` & `im_openai-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.1/LICENSE` & `im_openai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.1/PKG-INFO` & `im_openai-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im_openai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -75,15 +75,20 @@
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
-=======
-History
-=======
+======= History =======
 
-0.1.0 (2023-06-20)
-------------------
+## 0.1.0 (2023-06-20)
 
-* First release on PyPI.
+-   First release on PyPI.
+
+## 0.1.1 (2023-06-23)
+
+-   add TemplateString helper and support for data / params
+
+## 0.1.2(2023-06-23)
+
+-   add support for original template too
```

### Comparing `im_openai-0.1.1/README.md` & `im_openai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.1/docs/Makefile` & `im_openai-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.1/docs/conf.py` & `im_openai-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.1/docs/installation.rst` & `im_openai-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.1/docs/make.bat` & `im_openai-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.1/im_openai/client.py` & `im_openai-0.1.2/im_openai/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,19 +19,23 @@
     event = {
         "params": {},
         "prompt": {},
         "projectKey": project_key,
         "promptEventId": prompt_event_id,
     }
     if prompt_text is not None:
-        event["prompt"]["text"] = prompt_text
-        if hasattr(prompt_text, "params"):
+        event["prompt"]["prompt_text"] = prompt_text
+        if getattr(prompt_text, "params", None):
             # Can be TemplateString or any other
             event["params"] = prompt_text.params
 
+        # If the original template is available, send it too
+        if getattr(prompt_text, "template", None):
+            event["prompt"]["template"] = prompt_text.template
+
     if response is not None:
         event["response"] = response
     if response_time is not None:
         event["responseTime"] = response_time
 
     response = requests.post(PROMPT_REPORTING_URL, json=event)
     response.raise_for_status()
```

### Comparing `im_openai-0.1.1/im_openai/patch.py` & `im_openai-0.1.2/im_openai/patch.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.1/im_openai.egg-info/PKG-INFO` & `im_openai-0.1.2/im_openai.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-openai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -75,15 +75,20 @@
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
-=======
-History
-=======
+======= History =======
 
-0.1.0 (2023-06-20)
-------------------
+## 0.1.0 (2023-06-20)
 
-* First release on PyPI.
+-   First release on PyPI.
+
+## 0.1.1 (2023-06-23)
+
+-   add TemplateString helper and support for data / params
+
+## 0.1.2(2023-06-23)
+
+-   add support for original template too
```

### Comparing `im_openai-0.1.1/im_openai.egg-info/SOURCES.txt` & `im_openai-0.1.2/im_openai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 AUTHORS.rst
 CONTRIBUTING.rst
-HISTORY.rst
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
```

### Comparing `im_openai-0.1.1/setup.py` & `im_openai-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-with open("HISTORY.rst") as history_file:
+with open("HISTORY.md") as history_file:
     history = history_file.read()
 
 requirements = []
 
 test_requirements = [
     "pytest>=3",
 ]
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="im_openai",
     name="im_openai",
     packages=find_packages(include=["im_openai", "im_openai.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/alecf/im_openai",
-    version="0.1.1",
+    version="0.1.2",
     zip_safe=False,
 )
```

### Comparing `im_openai-0.1.1/tests/test_im_openai.py` & `im_openai-0.1.2/tests/test_im_openai.py`

 * *Files identical despite different names*

