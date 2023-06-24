# Comparing `tmp/lmt-cli-0.0.6.tar.gz` & `tmp/lmt-cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmt-cli-0.0.6.tar", last modified: Sat Jun 24 00:26:40 2023, max compression
+gzip compressed data, was "lmt-cli-0.0.7.tar", last modified: Sat Jun 24 01:03:00 2023, max compression
```

## Comparing `lmt-cli-0.0.6.tar` & `lmt-cli-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 00:26:40.806964 lmt-cli-0.0.6/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.6/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9059 2023-06-24 00:26:40.806964 lmt-cli-0.0.6/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8416 2023-06-24 00:13:18.000000 lmt-cli-0.0.6/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 00:26:40.806964 lmt-cli-0.0.6/lmt_cli/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.6/lmt_cli/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7666 2023-06-23 19:35:04.000000 lmt-cli-0.0.6/lmt_cli/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4828 2023-06-22 23:46:33.000000 lmt-cli-0.0.6/lmt_cli/gpt_integration.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9218 2023-06-24 00:24:19.000000 lmt-cli-0.0.6/lmt_cli/lib.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 00:26:40.806964 lmt-cli-0.0.6/lmt_cli.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9059 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      291 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       40 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-24 00:26:40.806964 lmt-cli-0.0.6/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1174 2023-06-24 00:26:19.000000 lmt-cli-0.0.6/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 01:03:00.346960 lmt-cli-0.0.7/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.7/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9059 2023-06-24 01:03:00.346960 lmt-cli-0.0.7/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8416 2023-06-24 00:13:18.000000 lmt-cli-0.0.7/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 01:03:00.346960 lmt-cli-0.0.7/lmt_cli/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.7/lmt_cli/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7666 2023-06-23 19:35:04.000000 lmt-cli-0.0.7/lmt_cli/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4828 2023-06-22 23:46:33.000000 lmt-cli-0.0.7/lmt_cli/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9209 2023-06-24 01:01:26.000000 lmt-cli-0.0.7/lmt_cli/lib.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 01:03:00.346960 lmt-cli-0.0.7/lmt_cli.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9059 2023-06-24 01:03:00.000000 lmt-cli-0.0.7/lmt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      291 2023-06-24 01:03:00.000000 lmt-cli-0.0.7/lmt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-24 01:03:00.000000 lmt-cli-0.0.7/lmt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       40 2023-06-24 01:03:00.000000 lmt-cli-0.0.7/lmt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-24 01:03:00.000000 lmt-cli-0.0.7/lmt_cli.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-06-24 01:03:00.000000 lmt-cli-0.0.7/lmt_cli.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-24 01:03:00.346960 lmt-cli-0.0.7/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1174 2023-06-24 01:01:53.000000 lmt-cli-0.0.7/setup.py
```

### Comparing `lmt-cli-0.0.6/LICENSE` & `lmt-cli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.6/PKG-INFO` & `lmt-cli-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmt-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
 Home-page: https://github.com/sderev/lmt
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/lmt
 Project-URL: Issues, http://github.com/sderev/lmt/issues
 Project-URL: Changelog, https://github.com/sderev/lmt/releases
```

### Comparing `lmt-cli-0.0.6/README.md` & `lmt-cli-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.6/lmt_cli/cli.py` & `lmt-cli-0.0.7/lmt_cli/cli.py`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.6/lmt_cli/gpt_integration.py` & `lmt-cli-0.0.7/lmt_cli/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.6/lmt_cli/lib.py` & `lmt-cli-0.0.7/lmt_cli/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     """
     Updates the value of a key from a template.
     """
     existing_value = template_content.setdefault(key, "")
     if existing_value is None:
         template_content[key] = existing_value = ""
 
-    return template_content.get(key, value) + (value or "")
+    return existing_value.rstrip() + (value or "")
 
 
 def add_emoji(system: str) -> str:
     """
     Adds an emoji to the system message.
     """
     emoji_message = (
```

### Comparing `lmt-cli-0.0.6/lmt_cli.egg-info/PKG-INFO` & `lmt-cli-0.0.7/lmt_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmt-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
 Home-page: https://github.com/sderev/lmt
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/lmt
 Project-URL: Issues, http://github.com/sderev/lmt/issues
 Project-URL: Changelog, https://github.com/sderev/lmt/releases
```

### Comparing `lmt-cli-0.0.6/setup.py` & `lmt-cli-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
```

