# Comparing `tmp/cytotransform-0.1.0.tar.gz` & `tmp/cytotransform-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytotransform-0.1.0.tar", max compression
+gzip compressed data, was "cytotransform-0.1.11.tar", max compression
```

## Comparing `cytotransform-0.1.0.tar` & `cytotransform-0.1.11.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-06-24 16:39:23.106914 cytotransform-0.1.0/LICENSE
--rw-r--r--   0        0        0     3039 2023-06-24 16:39:22.994914 cytotransform-0.1.0/README.md
--rw-r--r--   0        0        0      154 2023-06-24 16:30:42.111930 cytotransform-0.1.0/cytotransform/__init__.py
--rw-r--r--   0        0        0     2282 2023-05-23 19:46:34.225604 cytotransform-0.1.0/cytotransform/asinh.py
--rw-r--r--   0        0        0     1630 2023-05-23 18:23:35.752259 cytotransform-0.1.0/cytotransform/base.py
--rw-r--r--   0        0        0     3166 2023-06-24 16:40:17.838809 cytotransform-0.1.0/cytotransform/hyperlog.py
--rw-r--r--   0        0        0     1888 2023-05-23 19:46:59.161647 cytotransform-0.1.0/cytotransform/log.py
--rw-r--r--   0        0        0     3899 2023-06-15 18:12:40.765679 cytotransform-0.1.0/cytotransform/logicle.py
--rw-r--r--   0        0        0       92 2023-05-01 17:30:50.398865 cytotransform-0.1.0/cytotransform/logicle_ext/.gitignore
--rw-r--r--   0        0        0     4216 2023-05-01 17:30:50.398865 cytotransform-0.1.0/cytotransform/logicle_ext/FastLogicle.cpp
--rw-r--r--   0        0        0     1760 2023-05-01 17:30:50.398865 cytotransform-0.1.0/cytotransform/logicle_ext/LICENSE.txt
--rw-r--r--   0        0        0     8799 2023-05-01 17:30:50.398865 cytotransform-0.1.0/cytotransform/logicle_ext/Logicle.cpp
--rw-r--r--   0        0        0     5726 2023-05-01 17:30:50.398865 cytotransform-0.1.0/cytotransform/logicle_ext/logicle.h
--rw-r--r--   0        0        0     2028 2023-06-24 16:17:37.917619 cytotransform-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3684 1970-01-01 00:00:00.000000 cytotransform-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-24 16:39:23.106914 cytotransform-0.1.11/LICENSE
+-rw-r--r--   0        0        0     3387 2023-06-24 16:59:28.492763 cytotransform-0.1.11/README.md
+-rw-r--r--   0        0        0      154 2023-06-24 16:30:42.111930 cytotransform-0.1.11/cytotransform/__init__.py
+-rw-r--r--   0        0        0     2282 2023-05-23 19:46:34.225604 cytotransform-0.1.11/cytotransform/asinh.py
+-rw-r--r--   0        0        0     1630 2023-05-23 18:23:35.752259 cytotransform-0.1.11/cytotransform/base.py
+-rw-r--r--   0        0        0     3166 2023-06-24 16:40:17.838809 cytotransform-0.1.11/cytotransform/hyperlog.py
+-rw-r--r--   0        0        0     1888 2023-05-23 19:46:59.161647 cytotransform-0.1.11/cytotransform/log.py
+-rw-r--r--   0        0        0     3899 2023-06-15 18:12:40.765679 cytotransform-0.1.11/cytotransform/logicle.py
+-rw-r--r--   0        0        0       92 2023-05-01 17:30:50.398865 cytotransform-0.1.11/cytotransform/logicle_ext/.gitignore
+-rw-r--r--   0        0        0     4216 2023-05-01 17:30:50.398865 cytotransform-0.1.11/cytotransform/logicle_ext/FastLogicle.cpp
+-rw-r--r--   0        0        0     1760 2023-05-01 17:30:50.398865 cytotransform-0.1.11/cytotransform/logicle_ext/LICENSE.txt
+-rw-r--r--   0        0        0     8799 2023-05-01 17:30:50.398865 cytotransform-0.1.11/cytotransform/logicle_ext/Logicle.cpp
+-rw-r--r--   0        0        0     5726 2023-05-01 17:30:50.398865 cytotransform-0.1.11/cytotransform/logicle_ext/logicle.h
+-rw-r--r--   0        0        0     1838 2023-06-24 17:23:44.862624 cytotransform-0.1.11/pyproject.toml
+-rw-r--r--   0        0        0     4033 1970-01-01 00:00:00.000000 cytotransform-0.1.11/PKG-INFO
```

### Comparing `cytotransform-0.1.0/LICENSE` & `cytotransform-0.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `cytotransform-0.1.0/README.md` & `cytotransform-0.1.11/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Cytotransfrom
 
-[![PyPi]()()
-[![Python]()()
-[![Wheel]()()
-[![License]()()
-[![LastCommit]()()
-[![CodeCov]()()
-[![GitHubActions]()()
+![PyPI](https://img.shields.io/pypi/v/cytotransform)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cytotransform)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/cytotransform)
+![PyPI - License](https://img.shields.io/pypi/l/cytotransform)
+![Codecov](https://img.shields.io/codecov/c/github/burtonrj/cytotransform)
+![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/burtonrj/cytotransform/build.yaml)
 
 ## Description
 
 Cytotransform is a python package for transforming flow cytometry data. It implements the following transformations
 according to the GatingML 2.0 definitions (https://flowcyt.sourceforge.net/gating/latest.pdf):
 
 - Parametrized logarithmic transformation
```

### Comparing `cytotransform-0.1.0/cytotransform/asinh.py` & `cytotransform-0.1.11/cytotransform/asinh.py`

 * *Files identical despite different names*

### Comparing `cytotransform-0.1.0/cytotransform/base.py` & `cytotransform-0.1.11/cytotransform/base.py`

 * *Files identical despite different names*

### Comparing `cytotransform-0.1.0/cytotransform/hyperlog.py` & `cytotransform-0.1.11/cytotransform/hyperlog.py`

 * *Files identical despite different names*

### Comparing `cytotransform-0.1.0/cytotransform/log.py` & `cytotransform-0.1.11/cytotransform/log.py`

 * *Files identical despite different names*

### Comparing `cytotransform-0.1.0/cytotransform/logicle.py` & `cytotransform-0.1.11/cytotransform/logicle.py`

 * *Files identical despite different names*

### Comparing `cytotransform-0.1.0/cytotransform/logicle_ext/FastLogicle.cpp` & `cytotransform-0.1.11/cytotransform/logicle_ext/FastLogicle.cpp`

 * *Files identical despite different names*

### Comparing `cytotransform-0.1.0/cytotransform/logicle_ext/LICENSE.txt` & `cytotransform-0.1.11/cytotransform/logicle_ext/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cytotransform-0.1.0/cytotransform/logicle_ext/Logicle.cpp` & `cytotransform-0.1.11/cytotransform/logicle_ext/Logicle.cpp`

 * *Files identical despite different names*

### Comparing `cytotransform-0.1.0/cytotransform/logicle_ext/logicle.h` & `cytotransform-0.1.11/cytotransform/logicle_ext/logicle.h`

 * *Files identical despite different names*

### Comparing `cytotransform-0.1.0/pyproject.toml` & `cytotransform-0.1.11/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cytotransform"
-version = "0.1.0"
+version = "0.1.11"
 description = "Rapid transformations for cytometry data"
 authors = ["Ross Burton <burtonrossj@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
@@ -42,19 +42,14 @@
 ##### isort configuration https://pycqa.github.io/isort/docs/configuration/config_files.html
 [tool.isort]
 profile = "black"
 default_section = "THIRDPARTY"
 sections = "FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 skip = "__init__.py"
 
-##### black configuration https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-via-a-file
-[tool.black]
-line-length    = 88
-target_version = ['py311']
-
 
 ##### pytest configuration: http://doc.pytest.org/en/latest/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
 python_files = [ "test_*.py" ]
 norecursedirs = [
   ".git",
```

### Comparing `cytotransform-0.1.0/PKG-INFO` & `cytotransform-0.1.11/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cytotransform
-Version: 0.1.0
+Version: 0.1.11
 Summary: Rapid transformations for cytometry data
 License: MIT
 Author: Ross Burton
 Author-email: burtonrossj@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,21 +15,20 @@
 Requires-Dist: pybind11 (>=2.10.4,<3.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: setuptools (>=67.7.1,<68.0.0)
 Description-Content-Type: text/markdown
 
 # Cytotransfrom
 
-[![PyPi]()()
-[![Python]()()
-[![Wheel]()()
-[![License]()()
-[![LastCommit]()()
-[![CodeCov]()()
-[![GitHubActions]()()
+![PyPI](https://img.shields.io/pypi/v/cytotransform)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cytotransform)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/cytotransform)
+![PyPI - License](https://img.shields.io/pypi/l/cytotransform)
+![Codecov](https://img.shields.io/codecov/c/github/burtonrj/cytotransform)
+![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/burtonrj/cytotransform/build.yaml)
 
 ## Description
 
 Cytotransform is a python package for transforming flow cytometry data. It implements the following transformations
 according to the GatingML 2.0 definitions (https://flowcyt.sourceforge.net/gating/latest.pdf):
 
 - Parametrized logarithmic transformation
```

