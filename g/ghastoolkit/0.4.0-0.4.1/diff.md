# Comparing `tmp/ghastoolkit-0.4.0.tar.gz` & `tmp/ghastoolkit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.4.0.tar", last modified: Tue Jun  6 19:45:04 2023, max compression
+gzip compressed data, was "ghastoolkit-0.4.1.tar", last modified: Sat Jun 24 09:24:28 2023, max compression
```

## Comparing `ghastoolkit-0.4.0.tar` & `ghastoolkit-0.4.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.393639 ghastoolkit-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.393639 ghastoolkit-0.4.0/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.393639 ghastoolkit-0.4.0/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.393639 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-06 19:45:04.000000 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-06 19:45:04.000000 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:45:04.000000 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-06 19:45:04.000000 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 19:45:04.000000 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:24:28.658968 ghastoolkit-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-24 09:24:28.658968 ghastoolkit-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 09:24:28.658968 ghastoolkit-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:24:28.654967 ghastoolkit-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:24:28.654967 ghastoolkit-0.4.1/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:24:28.654967 ghastoolkit-0.4.1/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/codeql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/codeql/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/codeql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:24:28.658968 ghastoolkit-0.4.1/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:24:28.658968 ghastoolkit-0.4.1/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:24:28.658968 ghastoolkit-0.4.1/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:24:28.654967 ghastoolkit-0.4.1/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-24 09:24:28.000000 ghastoolkit-0.4.1/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-24 09:24:28.000000 ghastoolkit-0.4.1/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 09:24:28.000000 ghastoolkit-0.4.1/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-24 09:24:28.000000 ghastoolkit-0.4.1/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-24 09:24:28.000000 ghastoolkit-0.4.1/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:24:28.658968 ghastoolkit-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-24 09:24:00.000000 ghastoolkit-0.4.1/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.4.0/LICENSE` & `ghastoolkit-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/PKG-INFO` & `ghastoolkit-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.0
+Version: 0.4.1
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.4.0/README.md` & `ghastoolkit-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/pyproject.toml` & `ghastoolkit-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -19,15 +19,15 @@
 dependencies = [
     "certifi==2023.5.7",
     "charset-normalizer==3.1.0",
     "idna==3.4",
     "PyYAML==6.0",
     "ratelimit==2.2.1",
     "requests==2.31.0",
-    "urllib3==2.0.2"
+    "urllib3==2.0.3"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/GeekMasher/ghastoolkit"
 "Bug Tracker" = "https://github.com/GeekMasher/ghastoolkit/issues"
 
 [build-system]
```

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/__init__.py` & `ghastoolkit-0.4.1/src/ghastoolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/__main__.py` & `ghastoolkit-0.4.1/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.4.1/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.4.1/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.4.1/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.4.1/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.4.1/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.4.1/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.4.1/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.4.1/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.4.1/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.4.1/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.4.1/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.4.1/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.4.1/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.4.1/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.4.1/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.0
+Version: 0.4.1
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.4.0/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.4.1/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/tests/test_codeqldb.py` & `ghastoolkit-0.4.1/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/tests/test_codescanning.py` & `ghastoolkit-0.4.1/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/tests/test_default.py` & `ghastoolkit-0.4.1/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/tests/test_dependencies.py` & `ghastoolkit-0.4.1/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/tests/test_depgraph.py` & `ghastoolkit-0.4.1/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/tests/test_github.py` & `ghastoolkit-0.4.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/tests/test_licenses.py` & `ghastoolkit-0.4.1/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/tests/test_octokit.py` & `ghastoolkit-0.4.1/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.0/tests/test_secretscanning.py` & `ghastoolkit-0.4.1/tests/test_secretscanning.py`

 * *Files identical despite different names*

