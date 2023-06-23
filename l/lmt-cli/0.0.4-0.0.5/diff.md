# Comparing `tmp/lmt-cli-0.0.4.tar.gz` & `tmp/lmt-cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmt-cli-0.0.4.tar", last modified: Fri Jun 23 19:36:50 2023, max compression
+gzip compressed data, was "lmt-cli-0.0.5.tar", last modified: Fri Jun 23 23:51:32 2023, max compression
```

## Comparing `lmt-cli-0.0.4.tar` & `lmt-cli-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:36:50.244373 lmt-cli-0.0.4/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.4/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 19:36:50.244373 lmt-cli-0.0.4/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8412 2023-06-23 18:54:04.000000 lmt-cli-0.0.4/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:36:50.244373 lmt-cli-0.0.4/lmt/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.4/lmt/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7666 2023-06-23 19:35:04.000000 lmt-cli-0.0.4/lmt/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4828 2023-06-22 23:46:33.000000 lmt-cli-0.0.4/lmt/gpt_integration.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9224 2023-06-23 18:44:29.000000 lmt-cli-0.0.4/lmt/lib.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:36:50.244373 lmt-cli-0.0.4/lmt_cli.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      275 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       36 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        4 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-23 19:36:50.244373 lmt-cli-0.0.4/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1170 2023-06-23 19:36:19.000000 lmt-cli-0.0.4/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 23:51:32.636969 lmt-cli-0.0.5/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.5/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 23:51:32.636969 lmt-cli-0.0.5/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8412 2023-06-23 18:54:04.000000 lmt-cli-0.0.5/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 23:51:32.636969 lmt-cli-0.0.5/lmt_cli/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.5/lmt_cli/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7666 2023-06-23 19:35:04.000000 lmt-cli-0.0.5/lmt_cli/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4828 2023-06-22 23:46:33.000000 lmt-cli-0.0.5/lmt_cli/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9228 2023-06-23 23:48:47.000000 lmt-cli-0.0.5/lmt_cli/lib.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 23:51:32.636969 lmt-cli-0.0.5/lmt_cli.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      291 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       40 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-23 23:51:32.636969 lmt-cli-0.0.5/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1174 2023-06-23 23:46:08.000000 lmt-cli-0.0.5/setup.py
```

### Comparing `lmt-cli-0.0.4/LICENSE` & `lmt-cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.4/PKG-INFO` & `lmt-cli-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmt-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
 Home-page: https://github.com/sderev/lmt
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/lmt
 Project-URL: Issues, http://github.com/sderev/lmt/issues
 Project-URL: Changelog, https://github.com/sderev/lmt/releases
```

### Comparing `lmt-cli-0.0.4/README.md` & `lmt-cli-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.4/lmt/cli.py` & `lmt-cli-0.0.5/lmt_cli/cli.py`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.4/lmt/gpt_integration.py` & `lmt-cli-0.0.5/lmt_cli/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.4/lmt/lib.py` & `lmt-cli-0.0.5/lmt_cli/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import click
 import openai
 import yaml
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 
-from lmt import gpt_integration as openai_utils
+from lmt_cli import gpt_integration as openai_utils
 
 RED = "\x1b[91m"
 RESET = "\x1b[0m"
 
 
 def prepare_and_generate_response(
     system: str,
```

### Comparing `lmt-cli-0.0.4/lmt_cli.egg-info/PKG-INFO` & `lmt-cli-0.0.5/lmt_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmt-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
 Home-page: https://github.com/sderev/lmt
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/lmt
 Project-URL: Issues, http://github.com/sderev/lmt/issues
 Project-URL: Changelog, https://github.com/sderev/lmt/releases
```

### Comparing `lmt-cli-0.0.4/setup.py` & `lmt-cli-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
 
 
@@ -28,13 +28,13 @@
     },
     license="Apache Licence, Version 2.0",
     version=VERSION,
     packages=find_packages(),
     install_requires=read_requirements(),
     entry_points={
         "console_scripts": [
-            "lmt=lmt.cli:lmt",
+            "lmt=lmt_cli.cli:lmt",
         ]
     },
     python_requires=">=3.8",
 )
```

