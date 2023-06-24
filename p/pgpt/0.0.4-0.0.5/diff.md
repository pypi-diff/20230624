# Comparing `tmp/pgpt-0.0.4.tar.gz` & `tmp/pgpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgpt-0.0.4.tar", last modified: Sat Jun 24 07:49:06 2023, max compression
+gzip compressed data, was "pgpt-0.0.5.tar", last modified: Sat Jun 24 08:52:30 2023, max compression
```

## Comparing `pgpt-0.0.4.tar` & `pgpt-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 brettegeary   (501) staff       (20)        0 2023-06-24 07:49:06.952013 pgpt-0.0.4/
--rw-r--r--   0 brettegeary   (501) staff       (20)    35149 2023-06-24 07:23:36.000000 pgpt-0.0.4/LICENSE
--rw-r--r--   0 brettegeary   (501) staff       (20)     6299 2023-06-24 07:49:06.951543 pgpt-0.0.4/PKG-INFO
--rw-r--r--   0 brettegeary   (501) staff       (20)     5646 2023-06-24 07:23:36.000000 pgpt-0.0.4/README.md
-drwxr-xr-x   0 brettegeary   (501) staff       (20)        0 2023-06-24 07:49:06.931000 pgpt-0.0.4/pgpt.egg-info/
--rw-r--r--   0 brettegeary   (501) staff       (20)     6299 2023-06-24 07:49:06.000000 pgpt-0.0.4/pgpt.egg-info/PKG-INFO
--rw-r--r--   0 brettegeary   (501) staff       (20)      461 2023-06-24 07:49:06.000000 pgpt-0.0.4/pgpt.egg-info/SOURCES.txt
--rw-r--r--   0 brettegeary   (501) staff       (20)        1 2023-06-24 07:49:06.000000 pgpt-0.0.4/pgpt.egg-info/dependency_links.txt
--rw-r--r--   0 brettegeary   (501) staff       (20)       53 2023-06-24 07:49:06.000000 pgpt-0.0.4/pgpt.egg-info/entry_points.txt
--rw-r--r--   0 brettegeary   (501) staff       (20)     1225 2023-06-24 07:49:06.000000 pgpt-0.0.4/pgpt.egg-info/requires.txt
--rw-r--r--   0 brettegeary   (501) staff       (20)       19 2023-06-24 07:49:06.000000 pgpt-0.0.4/pgpt.egg-info/top_level.txt
-drwxr-xr-x   0 brettegeary   (501) staff       (20)        0 2023-06-24 07:49:06.945893 pgpt-0.0.4/programengineergpt/
--rw-r--r--   0 brettegeary   (501) staff       (20)      173 2023-06-24 07:23:36.000000 pgpt-0.0.4/programengineergpt/__init__.py
--rw-r--r--   0 brettegeary   (501) staff       (20)      187 2023-06-24 07:23:36.000000 pgpt-0.0.4/programengineergpt/__main__.py
--rw-r--r--   0 brettegeary   (501) staff       (20)     2294 2023-06-24 07:23:36.000000 pgpt-0.0.4/programengineergpt/config.py
--rw-r--r--   0 brettegeary   (501) staff       (20)      270 2023-06-24 07:23:36.000000 pgpt-0.0.4/programengineergpt/main.py
--rw-r--r--   0 brettegeary   (501) staff       (20)     1101 2023-06-24 07:23:36.000000 pgpt-0.0.4/programengineergpt/program_engineer.py
--rw-r--r--   0 brettegeary   (501) staff       (20)     3309 2023-06-24 07:48:18.000000 pgpt-0.0.4/pyproject.toml
--rw-r--r--   0 brettegeary   (501) staff       (20)       38 2023-06-24 07:49:06.952220 pgpt-0.0.4/setup.cfg
-drwxr-xr-x   0 brettegeary   (501) staff       (20)        0 2023-06-24 07:49:06.950216 pgpt-0.0.4/tests/
--rw-r--r--   0 brettegeary   (501) staff       (20)        0 2023-06-24 07:23:36.000000 pgpt-0.0.4/tests/test_code_assistant.py
--rw-r--r--   0 brettegeary   (501) staff       (20)      689 2023-06-24 07:23:36.000000 pgpt-0.0.4/tests/test_config.py
--rw-r--r--   0 brettegeary   (501) staff       (20)     1286 2023-06-24 07:23:36.000000 pgpt-0.0.4/tests/test_embedder.py
--rw-r--r--   0 brettegeary   (501) staff       (20)     1486 2023-06-24 07:23:36.000000 pgpt-0.0.4/tests/test_load_and_split.py
+drwxr-xr-x   0 brettegeary   (501) staff       (20)        0 2023-06-24 08:52:30.833650 pgpt-0.0.5/
+-rw-r--r--   0 brettegeary   (501) staff       (20)    35149 2023-06-24 07:23:36.000000 pgpt-0.0.5/LICENSE
+-rw-r--r--   0 brettegeary   (501) staff       (20)     6299 2023-06-24 08:52:30.832915 pgpt-0.0.5/PKG-INFO
+-rw-r--r--   0 brettegeary   (501) staff       (20)     5646 2023-06-24 07:23:36.000000 pgpt-0.0.5/README.md
+drwxr-xr-x   0 brettegeary   (501) staff       (20)        0 2023-06-24 08:52:30.821288 pgpt-0.0.5/pgpt.egg-info/
+-rw-r--r--   0 brettegeary   (501) staff       (20)     6299 2023-06-24 08:52:30.000000 pgpt-0.0.5/pgpt.egg-info/PKG-INFO
+-rw-r--r--   0 brettegeary   (501) staff       (20)      461 2023-06-24 08:52:30.000000 pgpt-0.0.5/pgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 brettegeary   (501) staff       (20)        1 2023-06-24 08:52:30.000000 pgpt-0.0.5/pgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 brettegeary   (501) staff       (20)       53 2023-06-24 08:52:30.000000 pgpt-0.0.5/pgpt.egg-info/entry_points.txt
+-rw-r--r--   0 brettegeary   (501) staff       (20)     1225 2023-06-24 08:52:30.000000 pgpt-0.0.5/pgpt.egg-info/requires.txt
+-rw-r--r--   0 brettegeary   (501) staff       (20)       19 2023-06-24 08:52:30.000000 pgpt-0.0.5/pgpt.egg-info/top_level.txt
+drwxr-xr-x   0 brettegeary   (501) staff       (20)        0 2023-06-24 08:52:30.826763 pgpt-0.0.5/programengineergpt/
+-rw-r--r--   0 brettegeary   (501) staff       (20)      173 2023-06-24 07:23:36.000000 pgpt-0.0.5/programengineergpt/__init__.py
+-rw-r--r--   0 brettegeary   (501) staff       (20)      186 2023-06-24 08:33:48.000000 pgpt-0.0.5/programengineergpt/__main__.py
+-rw-r--r--   0 brettegeary   (501) staff       (20)     2296 2023-06-24 08:33:48.000000 pgpt-0.0.5/programengineergpt/config.py
+-rw-r--r--   0 brettegeary   (501) staff       (20)      270 2023-06-24 07:23:36.000000 pgpt-0.0.5/programengineergpt/main.py
+-rw-r--r--   0 brettegeary   (501) staff       (20)     1118 2023-06-24 08:47:54.000000 pgpt-0.0.5/programengineergpt/program_engineer.py
+-rw-r--r--   0 brettegeary   (501) staff       (20)     3309 2023-06-24 08:50:36.000000 pgpt-0.0.5/pyproject.toml
+-rw-r--r--   0 brettegeary   (501) staff       (20)       38 2023-06-24 08:52:30.833824 pgpt-0.0.5/setup.cfg
+drwxr-xr-x   0 brettegeary   (501) staff       (20)        0 2023-06-24 08:52:30.831735 pgpt-0.0.5/tests/
+-rw-r--r--   0 brettegeary   (501) staff       (20)        0 2023-06-24 07:23:36.000000 pgpt-0.0.5/tests/test_code_assistant.py
+-rw-r--r--   0 brettegeary   (501) staff       (20)      636 2023-06-24 08:33:48.000000 pgpt-0.0.5/tests/test_config.py
+-rw-r--r--   0 brettegeary   (501) staff       (20)     1274 2023-06-24 08:33:48.000000 pgpt-0.0.5/tests/test_embedder.py
+-rw-r--r--   0 brettegeary   (501) staff       (20)     1489 2023-06-24 08:33:48.000000 pgpt-0.0.5/tests/test_load_and_split.py
```

### Comparing `pgpt-0.0.4/LICENSE` & `pgpt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pgpt-0.0.4/PKG-INFO` & `pgpt-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgpt
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: pgpt Version: 0.0.4 Summary: ProgramEngineerGPT is
+Metadata-Version: 2.1 Name: pgpt Version: 0.0.5 Summary: ProgramEngineerGPT is
 an interactive command line tool that leverages the power of AI to assist
 developers with code comprehension, exploration, and generation. It serves as a
 virtual assistant that can analyze codebases, answer queries about code, and
 even help in setting up new coding projects. Author-email: Brette Geary
 outlook.com> Project-URL: Homepage, https://github.com/hackedbyagirl/
 programengineergpt Project-URL: Bug Tracker, https://github.com/hackedbyagirl/
 programengineergpt/issues Requires-Python: >=3.10 Description-Content-Type:
```

### Comparing `pgpt-0.0.4/README.md` & `pgpt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pgpt-0.0.4/pgpt.egg-info/PKG-INFO` & `pgpt-0.0.5/pgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgpt
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: pgpt Version: 0.0.4 Summary: ProgramEngineerGPT is
+Metadata-Version: 2.1 Name: pgpt Version: 0.0.5 Summary: ProgramEngineerGPT is
 an interactive command line tool that leverages the power of AI to assist
 developers with code comprehension, exploration, and generation. It serves as a
 virtual assistant that can analyze codebases, answer queries about code, and
 even help in setting up new coding projects. Author-email: Brette Geary
 outlook.com> Project-URL: Homepage, https://github.com/hackedbyagirl/
 programengineergpt Project-URL: Bug Tracker, https://github.com/hackedbyagirl/
 programengineergpt/issues Requires-Python: >=3.10 Description-Content-Type:
```

### Comparing `pgpt-0.0.4/pgpt.egg-info/requires.txt` & `pgpt-0.0.5/pgpt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pgpt-0.0.4/programengineergpt/config.py` & `pgpt-0.0.5/programengineergpt/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 
 # Imports
 import os
+
 from dotenv import load_dotenv
+
 from programengineergpt.utils.args import Arguments
 
 
 class Config(object):
     """Stores configuration variables and functions for CodeAssistantGPT"""
 
     initialized = False
```

### Comparing `pgpt-0.0.4/programengineergpt/program_engineer.py` & `pgpt-0.0.5/programengineergpt/program_engineer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/python3
 
 # imports
 from programengineergpt.config import Config
 from programengineergpt.utils.display import Display
-from programengineergpt.utils.cli import CLI
 
 
 class ProgramEngineerGPT(object):
     """
     An AI-powered tool designed to assist with a variety of coding tasks.
     This includes:
         - Understanding the structure, dependencies, and other details of a codebase.
@@ -34,9 +33,11 @@
         """
         Launches the main interactive interface.
 
         Args:
             self : Argument
 
         """
+        from programengineergpt.utils.cli import CLI
+        
         app = CLI()
         app.launc_main_cli()
```

### Comparing `pgpt-0.0.4/pyproject.toml` & `pgpt-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "pgpt"
-version = "0.0.4"
+version = "0.0.5"
 description = "ProgramEngineerGPT is an interactive command line tool that leverages the power of AI to assist developers with code comprehension, exploration, and generation. It serves as a virtual assistant that can analyze codebases, answer queries about code, and even help in setting up new coding projects."
 authors = [
     { name = "Brette Geary", email = "hackedbg@outlook.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `pgpt-0.0.4/tests/test_config.py` & `pgpt-0.0.5/tests/test_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-import os
-import pytest
-from unittest.mock import patch, MagicMock
 from src.config import Config
 
+
 def test_init():
     # Call the init method
     Config.init()
 
     # Check that the initialized attribute is set to True
-    assert Config.initialized == True
+    assert Config.initialized is True
 
     # Check that the default values are set correctly
     assert Config.verbose == 0
-    assert Config.openai_key != None
-    assert Config.activeloop_key != None
-    assert Config.activeloop_username != None
-    assert Config.repo == None
+    assert Config.openai_key is not None
+    assert Config.activeloop_key is not None
+    assert Config.activeloop_username is not None
+    assert Config.repo is None
     assert Config.model == 'gpt-3.5-turbo'
-    assert Config.question == None
+    assert Config.question is None
     assert Config.chunk_size == 1000
     assert Config.chunk_overlap == 0
-    assert Config.embedded_size == 1536
+    assert Config.embedded_size == 1536
```

### Comparing `pgpt-0.0.4/tests/test_embedder.py` & `pgpt-0.0.5/tests/test_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import pytest
-from unittest.mock import patch, MagicMock
+from unittest.mock import MagicMock, patch
+
 from src.core.embedder import CodeEmbedder
 
+
 def test_embed_code():
     # Mock the OpenAIEmbeddings and DeepLake classes
     with patch('src.core.embedder.OpenAIEmbeddings') as MockOpenAIEmbeddings, \
          patch('src.core.embedder.DeepLake') as MockDeepLake:
         # Create a CodeEmbedder object
         embedder = CodeEmbedder(["def test(): pass"])
```

### Comparing `pgpt-0.0.4/tests/test_load_and_split.py` & `pgpt-0.0.5/tests/test_load_and_split.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python3
 
 import os
+
 import pytest
+
 from src.core.loader import CodeLoader
 
+
 @pytest.fixture
 def cleanup():
     # Setup: nothing to do
     yield
     # Teardown: remove the temp_repo directory if it exists
     if os.path.exists("temp_repo"):
         os.system("rm -rf temp_repo")
```

