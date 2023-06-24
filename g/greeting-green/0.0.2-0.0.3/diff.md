# Comparing `tmp/greeting_green-0.0.2.tar.gz` & `tmp/greeting_green-0.0.3.tar.gz`

## Comparing `greeting_green-0.0.2.tar` & `greeting_green-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/__about__.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/__init__.py
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/admin.py
--rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/apps.py
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/models.py
--rwxr-xr-x   0        0        0      375 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/tests.py
--rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/urls.py
--rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/views.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/migrations/__init__.py
--rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/static/greeting/style.css
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/templates/greeting/index.html
--rwxr-xr-x   0        0        0       29 2020-02-02 00:00:00.000000 greeting_green-0.0.2/.gitignore
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 greeting_green-0.0.2/LICENSE.txt
--rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 greeting_green-0.0.2/README.md
--rwxr-xr-x   0        0        0     3237 2020-02-02 00:00:00.000000 greeting_green-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 greeting_green-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/__init__.py
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/admin.py
+-rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/apps.py
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/models.py
+-rwxr-xr-x   0        0        0      381 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/tests.py
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/urls.py
+-rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/views.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/migrations/__init__.py
+-rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/static/greeting/style.css
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 greeting_green-0.0.3/greeting_green/templates/greeting/index.html
+-rwxr-xr-x   0        0        0       29 2020-02-02 00:00:00.000000 greeting_green-0.0.3/.gitignore
+-rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 greeting_green-0.0.3/LICENSE.txt
+-rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 greeting_green-0.0.3/README.md
+-rwxr-xr-x   0        0        0     3297 2020-02-02 00:00:00.000000 greeting_green-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 greeting_green-0.0.3/PKG-INFO
```

### Comparing `greeting_green-0.0.2/LICENSE.txt` & `greeting_green-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `greeting_green-0.0.2/README.md` & `greeting_green-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `greeting_green-0.0.2/pyproject.toml` & `greeting_green-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "greeting-green"
 dynamic = ["version"]
-description = 'あいさつ'
+description = '挨拶アプリ'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Kenno-Warise", email = "wariken0523@gmail.com" },
 ]
@@ -20,32 +20,30 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = [
-  "Django == 4.2.2",
-]
+dependencies = []
 
 [project.urls]
-Documentation = "https://github.com/unknown/greeting#readme"
-Issues = "https://github.com/unknown/greeting/issues"
-Source = "https://github.com/unknown/greeting"
+Documentation = "https://github.com/unknown/greeting-green#readme"
+Issues = "https://github.com/unknown/greeting-green/issues"
+Source = "https://github.com/unknown/greeting-green"
 
 [tool.hatch.build]
 include = [
-  "src/greeting/*",
-  "src/greeting/static",
-  "src/greeting/templates",
+  "greeting_green/*",
+  "greeting_green/templates",
+  "greeting_green/static",
 ]
 
 [tool.hatch.version]
-path = "src/greeting/__about__.py"
+path = "greeting_green/__init__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
 ]
 [tool.hatch.envs.default.scripts]
@@ -67,15 +65,15 @@
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
 ]
 [tool.hatch.envs.lint.scripts]
-typing = "mypy --install-types --non-interactive {args:src/greeting tests}"
+typing = "mypy --install-types --non-interactive {args:src/greeting_green tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
 fmt = [
   "black {args:.}",
   "ruff --fix {args:.}",
@@ -133,34 +131,34 @@
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
 [tool.ruff.isort]
-known-first-party = ["greeting"]
+known-first-party = ["greeting_green"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
-source_pkgs = ["greeting", "tests"]
+source_pkgs = ["greeting_green", "tests"]
 branch = true
 parallel = true
 omit = [
-  "src/greeting/__about__.py",
+  "src/greeting_green/__about__.py",
 ]
 
 [tool.coverage.paths]
-greeting = ["src/greeting", "*/greeting/src/greeting"]
-tests = ["tests", "*/greeting/tests"]
+greeting_green = ["src/greeting_green", "*/greeting-green/src/greeting_green"]
+tests = ["tests", "*/greeting-green/tests"]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
```

### Comparing `greeting_green-0.0.2/PKG-INFO` & `greeting_green-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: greeting-green
-Version: 0.0.2
-Summary: あいさつ
-Project-URL: Documentation, https://github.com/unknown/greeting#readme
-Project-URL: Issues, https://github.com/unknown/greeting/issues
-Project-URL: Source, https://github.com/unknown/greeting
+Version: 0.0.3
+Summary: 挨拶アプリ
+Project-URL: Documentation, https://github.com/unknown/greeting-green#readme
+Project-URL: Issues, https://github.com/unknown/greeting-green/issues
+Project-URL: Source, https://github.com/unknown/greeting-green
 Author-email: Kenno-Warise <wariken0523@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: django==4.2.2
 Description-Content-Type: text/markdown
 
 # django-hatch
 
 [![PyPI - Version](https://img.shields.io/pypi/v/django-hatch.svg)](https://pypi.org/project/django-hatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-hatch.svg)](https://pypi.org/project/django-hatch)
```

