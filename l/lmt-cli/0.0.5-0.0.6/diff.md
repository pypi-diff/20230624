# Comparing `tmp/lmt-cli-0.0.5.tar.gz` & `tmp/lmt-cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmt-cli-0.0.5.tar", last modified: Fri Jun 23 23:51:32 2023, max compression
+gzip compressed data, was "lmt-cli-0.0.6.tar", last modified: Sat Jun 24 00:26:40 2023, max compression
```

## Comparing `lmt-cli-0.0.5.tar` & `lmt-cli-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 23:51:32.636969 lmt-cli-0.0.5/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.5/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 23:51:32.636969 lmt-cli-0.0.5/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8412 2023-06-23 18:54:04.000000 lmt-cli-0.0.5/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 23:51:32.636969 lmt-cli-0.0.5/lmt_cli/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.5/lmt_cli/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7666 2023-06-23 19:35:04.000000 lmt-cli-0.0.5/lmt_cli/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4828 2023-06-22 23:46:33.000000 lmt-cli-0.0.5/lmt_cli/gpt_integration.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9228 2023-06-23 23:48:47.000000 lmt-cli-0.0.5/lmt_cli/lib.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 23:51:32.636969 lmt-cli-0.0.5/lmt_cli.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      291 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       40 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-06-23 23:51:32.000000 lmt-cli-0.0.5/lmt_cli.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-23 23:51:32.636969 lmt-cli-0.0.5/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1174 2023-06-23 23:46:08.000000 lmt-cli-0.0.5/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 00:26:40.806964 lmt-cli-0.0.6/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.6/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9059 2023-06-24 00:26:40.806964 lmt-cli-0.0.6/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8416 2023-06-24 00:13:18.000000 lmt-cli-0.0.6/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 00:26:40.806964 lmt-cli-0.0.6/lmt_cli/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.6/lmt_cli/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7666 2023-06-23 19:35:04.000000 lmt-cli-0.0.6/lmt_cli/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4828 2023-06-22 23:46:33.000000 lmt-cli-0.0.6/lmt_cli/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9218 2023-06-24 00:24:19.000000 lmt-cli-0.0.6/lmt_cli/lib.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 00:26:40.806964 lmt-cli-0.0.6/lmt_cli.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9059 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      291 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       40 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-06-24 00:26:40.000000 lmt-cli-0.0.6/lmt_cli.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-24 00:26:40.806964 lmt-cli-0.0.6/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1174 2023-06-24 00:26:19.000000 lmt-cli-0.0.6/setup.py
```

### Comparing `lmt-cli-0.0.5/LICENSE` & `lmt-cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.5/PKG-INFO` & `lmt-cli-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmt-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
 Home-page: https://github.com/sderev/lmt
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/lmt
 Project-URL: Issues, http://github.com/sderev/lmt/issues
 Project-URL: Changelog, https://github.com/sderev/lmt/releases
@@ -56,15 +56,15 @@
 **TODO: Video Demo**: A video demo showcasing `lmt`'s features will be added here.
 
 ## Installation
 
 ### `pip`
 
 ```bash
-python3 -m pip install llm-toolbox
+python3 -m pip install lmt-cli
 ```
 
 ### `pipx`, the Easy Way
 
 To use these tools, I recommend that you first install [pipx](https://pypa.github.io/pipx/installation/). It's a package manager for Python that makes the installation and upgrade of CLI apps easy (no more hassle with virtual environments 😌).
 
 * Debian / Ubuntu
@@ -80,27 +80,27 @@
     ```
 
 ### Installing `lmt` with `pipx`
 
 To install the latest stable version of `lmt`, simply run this command:
 
 ```bash
-pipx install lmt
+pipx install lmt-cli
 ```
 
 If you want to follow the `main` branch:
 
 ```bash
 pipx install git+https://github.com/sderev/lmt
 ```
 
 To upgrade it:
 
 ```bash
-pipx upgrade lmt
+pipx upgrade lmt-cli
 ```
 
 ### Cloning the `lmt` Repository
 
 You can clone this repository with the following command:
 
 ```bash
```

### Comparing `lmt-cli-0.0.5/README.md` & `lmt-cli-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 **TODO: Video Demo**: A video demo showcasing `lmt`'s features will be added here.
 
 ## Installation
 
 ### `pip`
 
 ```bash
-python3 -m pip install llm-toolbox
+python3 -m pip install lmt-cli
 ```
 
 ### `pipx`, the Easy Way
 
 To use these tools, I recommend that you first install [pipx](https://pypa.github.io/pipx/installation/). It's a package manager for Python that makes the installation and upgrade of CLI apps easy (no more hassle with virtual environments 😌).
 
 * Debian / Ubuntu
@@ -66,27 +66,27 @@
     ```
 
 ### Installing `lmt` with `pipx`
 
 To install the latest stable version of `lmt`, simply run this command:
 
 ```bash
-pipx install lmt
+pipx install lmt-cli
 ```
 
 If you want to follow the `main` branch:
 
 ```bash
 pipx install git+https://github.com/sderev/lmt
 ```
 
 To upgrade it:
 
 ```bash
-pipx upgrade lmt
+pipx upgrade lmt-cli
 ```
 
 ### Cloning the `lmt` Repository
 
 You can clone this repository with the following command:
 
 ```bash
```

### Comparing `lmt-cli-0.0.5/lmt_cli/cli.py` & `lmt-cli-0.0.6/lmt_cli/cli.py`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.5/lmt_cli/gpt_integration.py` & `lmt-cli-0.0.6/lmt_cli/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.5/lmt_cli/lib.py` & `lmt-cli-0.0.6/lmt_cli/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,22 @@
     """
     Adds an emoji to the system message.
     """
     emoji_message = (
         "Add plenty of emojis as a colorful way to convey emotions. However, don't"
         " mention it."
     )
+    system = system.rstrip()
+
     if system == "":
         return emoji_message
-    elif system[-1] == ".":
-        return system + " " + emoji_message
-    else:
-        return system.rstrip() + ". " + emoji_message
+
+    if not system.endswith("."):
+        system += "."
+    return system + " " + emoji_message
 
 
 def generate_response(
     debug: bool = False,
     emoji: bool = False,
     model: str = "gpt-3.5-turbo",
     prompt: str = None,
```

### Comparing `lmt-cli-0.0.5/lmt_cli.egg-info/PKG-INFO` & `lmt-cli-0.0.6/lmt_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmt-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
 Home-page: https://github.com/sderev/lmt
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/lmt
 Project-URL: Issues, http://github.com/sderev/lmt/issues
 Project-URL: Changelog, https://github.com/sderev/lmt/releases
@@ -56,15 +56,15 @@
 **TODO: Video Demo**: A video demo showcasing `lmt`'s features will be added here.
 
 ## Installation
 
 ### `pip`
 
 ```bash
-python3 -m pip install llm-toolbox
+python3 -m pip install lmt-cli
 ```
 
 ### `pipx`, the Easy Way
 
 To use these tools, I recommend that you first install [pipx](https://pypa.github.io/pipx/installation/). It's a package manager for Python that makes the installation and upgrade of CLI apps easy (no more hassle with virtual environments 😌).
 
 * Debian / Ubuntu
@@ -80,27 +80,27 @@
     ```
 
 ### Installing `lmt` with `pipx`
 
 To install the latest stable version of `lmt`, simply run this command:
 
 ```bash
-pipx install lmt
+pipx install lmt-cli
 ```
 
 If you want to follow the `main` branch:
 
 ```bash
 pipx install git+https://github.com/sderev/lmt
 ```
 
 To upgrade it:
 
 ```bash
-pipx upgrade lmt
+pipx upgrade lmt-cli
 ```
 
 ### Cloning the `lmt` Repository
 
 You can clone this repository with the following command:
 
 ```bash
```

### Comparing `lmt-cli-0.0.5/setup.py` & `lmt-cli-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
```

