# Comparing `tmp/alfred_cli-2.1.0.tar.gz` & `tmp/alfred_cli-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred_cli-2.1.0.tar", max compression
+gzip compressed data, was "alfred_cli-2.1.1.tar", max compression
```

## Comparing `alfred_cli-2.1.0.tar` & `alfred_cli-2.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-06-24 05:13:29.562518 alfred_cli-2.1.0/LICENSE
--rw-r--r--   0        0        0    10971 2023-06-24 05:13:29.562518 alfred_cli-2.1.0/README.md
--rw-r--r--   0        0        0     1582 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      282 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/__init__.py
--rw-r--r--   0        0        0     1483 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/alfred_command.py
--rw-r--r--   0        0        0     5994 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/cli.py
--rw-r--r--   0        0        0     5614 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/commands.py
--rw-r--r--   0        0        0     3486 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/ctx.py
--rw-r--r--   0        0        0     2666 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/decorator.py
--rw-r--r--   0        0        0        0 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/domain/__init__.py
--rw-r--r--   0        0        0     2404 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/domain/command.py
--rw-r--r--   0        0        0     1470 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/domain/manifest.py
--rw-r--r--   0        0        0      605 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/echo.py
--rw-r--r--   0        0        0      645 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/exceptions.py
--rw-r--r--   0        0        0     2978 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/interpreter.py
--rw-r--r--   0        0        0     2638 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/lib.py
--rw-r--r--   0        0        0      208 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/logger.py
--rw-r--r--   0        0        0     9465 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/main.py
--rw-r--r--   0        0        0     9168 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/manifest.py
--rw-r--r--   0        0        0      619 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/os.py
--rw-r--r--   0        0        0      432 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/resources/.alfred.toml
--rw-r--r--   0        0        0        0 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/resources/__init__.py
--rw-r--r--   0        0        0     1367 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/resources/cmd.py
--rw-r--r--   0        0        0    12311 1970-01-01 00:00:00.000000 alfred_cli-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-24 06:03:42.256612 alfred_cli-2.1.1/LICENSE
+-rw-r--r--   0        0        0    10971 2023-06-24 06:03:42.256612 alfred_cli-2.1.1/README.md
+-rw-r--r--   0        0        0     1582 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/__init__.py
+-rw-r--r--   0        0        0     1483 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/alfred_command.py
+-rw-r--r--   0        0        0     5994 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/cli.py
+-rw-r--r--   0        0        0     5618 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/commands.py
+-rw-r--r--   0        0        0     3486 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/ctx.py
+-rw-r--r--   0        0        0     2666 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/decorator.py
+-rw-r--r--   0        0        0        0 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/domain/__init__.py
+-rw-r--r--   0        0        0     2404 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/domain/command.py
+-rw-r--r--   0        0        0     1470 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/domain/manifest.py
+-rw-r--r--   0        0        0      605 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/echo.py
+-rw-r--r--   0        0        0      645 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/exceptions.py
+-rw-r--r--   0        0        0     2990 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/interpreter.py
+-rw-r--r--   0        0        0     2638 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/lib.py
+-rw-r--r--   0        0        0      208 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/logger.py
+-rw-r--r--   0        0        0     9465 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/main.py
+-rw-r--r--   0        0        0     9168 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/manifest.py
+-rw-r--r--   0        0        0      619 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/os.py
+-rw-r--r--   0        0        0      432 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/resources/.alfred.toml
+-rw-r--r--   0        0        0        0 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/resources/__init__.py
+-rw-r--r--   0        0        0     1367 2023-06-24 06:03:42.260612 alfred_cli-2.1.1/src/alfred/resources/cmd.py
+-rw-r--r--   0        0        0    12311 1970-01-01 00:00:00.000000 alfred_cli-2.1.1/PKG-INFO
```

### Comparing `alfred_cli-2.1.0/LICENSE` & `alfred_cli-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/README.md` & `alfred_cli-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/pyproject.toml` & `alfred_cli-2.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alfred-cli"
-version = "2.1.0"
+version = "2.1.1"
 description = "alfred is an extensible building tool that can replace a Makefile or Fabric. Writing commands in python is done in minutes."
 authors = ["Fabien Arcellier <fabien.arcellier@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "alfred", from = "src"}]
 include = [
     { path = "alfred/resources/*" }
@@ -36,15 +36,15 @@
 [tool.poetry.group.dev.dependencies]
 build = "^0.10.0"
 coverage = "^7.2.2"
 fixtup = "^0.1.5"
 pylint = "^2.17.1"
 pytest = "^7.2.2"
 twine = "^4.0.2"
-sphinx = "^6.1.3"
+sphinx = "^5.0.0"
 sphinx-rtd-theme = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `alfred_cli-2.1.0/src/alfred/alfred_command.py` & `alfred_cli-2.1.1/src/alfred/alfred_command.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/cli.py` & `alfred_cli-2.1.1/src/alfred/cli.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/commands.py` & `alfred_cli-2.1.1/src/alfred/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     return commands
 
 
 def _load_subproject(commands: list, directory: str) -> list:
     _subproject_manifest = manifest.lookup(directory)
     name = manifest.name(directory)
     if ' ' in name:
-        echo.error(f"Subproject ignored: project name from {directory} cannot contain spaces, {name=}")
+        echo.error(f"Subproject ignored: project name from {directory} cannot contain spaces, name={name}")
     else:
         command = AlfredCommand()
         command.command = AlfredSubprojectCommand(name=name,
                                                   help=manifest.description(directory),
                                                   path=os.path.realpath(directory))
         command.path = os.path.realpath(directory)
         command.project_dir = os.path.realpath(directory)
```

### Comparing `alfred_cli-2.1.0/src/alfred/ctx.py` & `alfred_cli-2.1.1/src/alfred/ctx.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/decorator.py` & `alfred_cli-2.1.1/src/alfred/decorator.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/domain/command.py` & `alfred_cli-2.1.1/src/alfred/domain/command.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/domain/manifest.py` & `alfred_cli-2.1.1/src/alfred/domain/manifest.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/echo.py` & `alfred_cli-2.1.1/src/alfred/echo.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/exceptions.py` & `alfred_cli-2.1.1/src/alfred/exceptions.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/interpreter.py` & `alfred_cli-2.1.1/src/alfred/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,18 @@
     bin_path = venv_bin_path(venv)
     global_path = format_path_variable(global_path, bin_path)
 
     if not os.path.isfile(python_path):
         raise AlfredException(f"python interpreter not found in venv: {venv}")
 
     if not os.path.isdir(bin_path):
-        raise AlfredException(f"bin folder not found in venv: {venv}, {bin_path=}")
+        raise AlfredException(f"bin folder not found in venv: {venv}, bin_path={bin_path}")
 
     python = plumbum.local[python_path]
-    logger.debug(f"alfred interpreter - switch to python: {python_path} : {args=}")
+    logger.debug(f"alfred interpreter - switch to python: {python_path} : args={args}")
 
     with local.env(VIRTUAL_ENV=venv, PATH=global_path):
         python_args = ['-m', module] + args
         if is_windows():
             # windows does not support streaming through plumbum.
             # the publication is done at the end of the call.
             #
```

### Comparing `alfred_cli-2.1.0/src/alfred/lib.py` & `alfred_cli-2.1.1/src/alfred/lib.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/main.py` & `alfred_cli-2.1.1/src/alfred/main.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/manifest.py` & `alfred_cli-2.1.1/src/alfred/manifest.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/os.py` & `alfred_cli-2.1.1/src/alfred/os.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/src/alfred/resources/cmd.py` & `alfred_cli-2.1.1/src/alfred/resources/cmd.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.1.0/PKG-INFO` & `alfred_cli-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-cli
-Version: 2.1.0
+Version: 2.1.1
 Summary: alfred is an extensible building tool that can replace a Makefile or Fabric. Writing commands in python is done in minutes.
 Home-page: https://github.com/FabienArcellier/alfred-cli#alfred
 License: MIT
 Keywords: building tool,makefile,productivity,automation,continuous integration,developper friendly
 Author: Fabien Arcellier
 Author-email: fabien.arcellier@gmail.com
 Requires-Python: >=3.8,<4.0
```

