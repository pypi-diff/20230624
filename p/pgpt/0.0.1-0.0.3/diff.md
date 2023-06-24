# Comparing `tmp/pgpt-0.0.1.tar.gz` & `tmp/pgpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgpt-0.0.1.tar", last modified: Sat Jun 24 05:46:29 2023, max compression
+gzip compressed data, was "pgpt-0.0.3.tar", last modified: Sat Jun 24 06:47:28 2023, max compression
```

## Comparing `pgpt-0.0.1.tar` & `pgpt-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 05:46:29.554312 pgpt-0.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-06-23 21:51:52.000000 pgpt-0.0.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5561 2023-06-24 05:46:29.554312 pgpt-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4908 2023-06-24 05:08:08.000000 pgpt-0.0.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 05:46:29.550312 pgpt-0.0.1/pgpt.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5561 2023-06-24 05:46:29.000000 pgpt-0.0.1/pgpt.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      461 2023-06-24 05:46:29.000000 pgpt-0.0.1/pgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-24 05:46:29.000000 pgpt-0.0.1/pgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       48 2023-06-24 05:46:29.000000 pgpt-0.0.1/pgpt.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3449 2023-06-24 05:46:29.000000 pgpt-0.0.1/pgpt.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       19 2023-06-24 05:46:29.000000 pgpt-0.0.1/pgpt.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 05:46:29.550312 pgpt-0.0.1/programengineergpt/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      166 2023-06-24 05:08:08.000000 pgpt-0.0.1/programengineergpt/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      302 2023-06-24 05:08:08.000000 pgpt-0.0.1/programengineergpt/__main__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2269 2023-06-24 05:08:08.000000 pgpt-0.0.1/programengineergpt/config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      302 2023-06-24 05:41:53.000000 pgpt-0.0.1/programengineergpt/main.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1113 2023-06-24 05:08:08.000000 pgpt-0.0.1/programengineergpt/program_engineer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6353 2023-06-24 05:46:25.000000 pgpt-0.0.1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-24 05:46:29.554312 pgpt-0.0.1/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 05:46:29.550312 pgpt-0.0.1/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-23 21:55:45.000000 pgpt-0.0.1/tests/test_code_assistant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      689 2023-06-23 21:51:52.000000 pgpt-0.0.1/tests/test_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1286 2023-06-23 21:51:52.000000 pgpt-0.0.1/tests/test_embedder.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1486 2023-06-23 21:51:52.000000 pgpt-0.0.1/tests/test_load_and_split.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 06:47:28.646312 pgpt-0.0.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-06-23 21:51:52.000000 pgpt-0.0.3/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5561 2023-06-24 06:47:28.646312 pgpt-0.0.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4908 2023-06-24 05:08:08.000000 pgpt-0.0.3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 06:47:28.646312 pgpt-0.0.3/pgpt.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5561 2023-06-24 06:47:28.000000 pgpt-0.0.3/pgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      461 2023-06-24 06:47:28.000000 pgpt-0.0.3/pgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-24 06:47:28.000000 pgpt-0.0.3/pgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-06-24 06:47:28.000000 pgpt-0.0.3/pgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3449 2023-06-24 06:47:28.000000 pgpt-0.0.3/pgpt.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       19 2023-06-24 06:47:28.000000 pgpt-0.0.3/pgpt.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 06:47:28.646312 pgpt-0.0.3/programengineergpt/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      150 2023-06-24 06:20:10.000000 pgpt-0.0.3/programengineergpt/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      186 2023-06-24 06:43:47.000000 pgpt-0.0.3/programengineergpt/__main__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2270 2023-06-24 06:23:15.000000 pgpt-0.0.3/programengineergpt/config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      270 2023-06-24 06:43:43.000000 pgpt-0.0.3/programengineergpt/main.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1116 2023-06-24 06:17:25.000000 pgpt-0.0.3/programengineergpt/program_engineer.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6358 2023-06-24 06:46:27.000000 pgpt-0.0.3/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-24 06:47:28.646312 pgpt-0.0.3/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 06:47:28.646312 pgpt-0.0.3/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-23 21:55:45.000000 pgpt-0.0.3/tests/test_code_assistant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      689 2023-06-23 21:51:52.000000 pgpt-0.0.3/tests/test_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1286 2023-06-23 21:51:52.000000 pgpt-0.0.3/tests/test_embedder.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1486 2023-06-23 21:51:52.000000 pgpt-0.0.3/tests/test_load_and_split.py
```

### Comparing `pgpt-0.0.1/LICENSE` & `pgpt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pgpt-0.0.1/PKG-INFO` & `pgpt-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgpt
-Version: 0.0.1
+Version: 0.0.3
 Summary: ProgramEngineerGPT is an interactive command line tool that leverages the power of AI to assist developers with code comprehension, exploration, and generation. It serves as a virtual assistant that can analyze codebases, answer queries about code, and even help in setting up new coding projects.
 Author-email: Brette Geary <hackedbg@outlook.com>
 Project-URL: Homepage, https://github.com/hackedbyagirl/programengineergpt
 Project-URL: Bug Tracker, https://github.com/hackedbyagirl/programengineergpt/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgpt Version: 0.0.1 Summary: ProgramEngineerGPT is
+Metadata-Version: 2.1 Name: pgpt Version: 0.0.3 Summary: ProgramEngineerGPT is
 an interactive command line tool that leverages the power of AI to assist
 developers with code comprehension, exploration, and generation. It serves as a
 virtual assistant that can analyze codebases, answer queries about code, and
 even help in setting up new coding projects. Author-email: Brette Geary
 outlook.com> Project-URL: Homepage, https://github.com/hackedbyagirl/
 programengineergpt Project-URL: Bug Tracker, https://github.com/hackedbyagirl/
 programengineergpt/issues Requires-Python: >=3.10 Description-Content-Type:
```

### Comparing `pgpt-0.0.1/README.md` & `pgpt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pgpt-0.0.1/pgpt.egg-info/PKG-INFO` & `pgpt-0.0.3/pgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgpt
-Version: 0.0.1
+Version: 0.0.3
 Summary: ProgramEngineerGPT is an interactive command line tool that leverages the power of AI to assist developers with code comprehension, exploration, and generation. It serves as a virtual assistant that can analyze codebases, answer queries about code, and even help in setting up new coding projects.
 Author-email: Brette Geary <hackedbg@outlook.com>
 Project-URL: Homepage, https://github.com/hackedbyagirl/programengineergpt
 Project-URL: Bug Tracker, https://github.com/hackedbyagirl/programengineergpt/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgpt Version: 0.0.1 Summary: ProgramEngineerGPT is
+Metadata-Version: 2.1 Name: pgpt Version: 0.0.3 Summary: ProgramEngineerGPT is
 an interactive command line tool that leverages the power of AI to assist
 developers with code comprehension, exploration, and generation. It serves as a
 virtual assistant that can analyze codebases, answer queries about code, and
 even help in setting up new coding projects. Author-email: Brette Geary
 outlook.com> Project-URL: Homepage, https://github.com/hackedbyagirl/
 programengineergpt Project-URL: Bug Tracker, https://github.com/hackedbyagirl/
 programengineergpt/issues Requires-Python: >=3.10 Description-Content-Type:
```

### Comparing `pgpt-0.0.1/pgpt.egg-info/requires.txt` & `pgpt-0.0.3/pgpt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pgpt-0.0.1/programengineergpt/config.py` & `pgpt-0.0.3/programengineergpt/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 # Imports
 import os
 from dotenv import load_dotenv
+
 from programengineergpt.utils.args import Arguments
 
 
 class Config(object):
     '''Stores configuration variables and functions for CodeAssistantGPT'''
 
     initialized = False
```

### Comparing `pgpt-0.0.1/programengineergpt/program_engineer.py` & `pgpt-0.0.3/programengineergpt/program_engineer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # imports
 from programengineergpt.config import Config
 from programengineergpt.utils.display import Display
 from programengineergpt.utils.cli import CLI
 
 
-class CodeEngineerGPT(object):
+class ProgramEngineerGPT(object):
     """
     An AI-powered tool designed to assist with a variety of coding tasks.
     This includes:
         - Understanding the structure, dependencies, and other details of a codebase.
         - Getting assistance in setting up a new coding project, including planning and setup.
         - Having the AI generate code snippets based on your requirements.
         - Getting help in debugging your code and suggestions for improvements.
```

### Comparing `pgpt-0.0.1/pyproject.toml` & `pgpt-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "pgpt"
-version = "0.0.1"
+version = "0.0.3"
 description = "ProgramEngineerGPT is an interactive command line tool that leverages the power of AI to assist developers with code comprehension, exploration, and generation. It serves as a virtual assistant that can analyze codebases, answer queries about code, and even help in setting up new coding projects."
 authors = [
     { name = "Brette Geary", email = "hackedbg@outlook.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
@@ -198,24 +198,24 @@
     'webcolors==1.13',
     'webencodings==0.5.1',
     'websocket-client==1.5.2',
     'wrapt==1.15.0',
     'yarl==1.9.2'
 ]
 
+[tool.setuptools]
+packages = ["programengineergpt"]
+
 [project.scripts]
-pgpt = 'programengineergpt:run'
+pgpt = 'programengineergpt.main:run'
 
 [project.urls]
 "Homepage" = "https://github.com/hackedbyagirl/programengineergpt"
 "Bug Tracker" = "https://github.com/hackedbyagirl/programengineergpt/issues"
 
-[tool.setuptools]
-packages = ["programengineergpt"]
-
 [tool.ruff]
 select = ["F", "E", "W", "I001"]
 line-length = 90
 show-fixes = false
 target-version = "py311"
 task-tags = ["TODO", "FIXME"]
 exclude = [
```

### Comparing `pgpt-0.0.1/tests/test_config.py` & `pgpt-0.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pgpt-0.0.1/tests/test_embedder.py` & `pgpt-0.0.3/tests/test_embedder.py`

 * *Files identical despite different names*

### Comparing `pgpt-0.0.1/tests/test_load_and_split.py` & `pgpt-0.0.3/tests/test_load_and_split.py`

 * *Files identical despite different names*

