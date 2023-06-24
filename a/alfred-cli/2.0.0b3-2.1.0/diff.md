# Comparing `tmp/alfred_cli-2.0.0b3.tar.gz` & `tmp/alfred_cli-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred_cli-2.0.0b3.tar", max compression
+gzip compressed data, was "alfred_cli-2.1.0.tar", max compression
```

## Comparing `alfred_cli-2.0.0b3.tar` & `alfred_cli-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-05-21 09:38:29.925030 alfred_cli-2.0.0b3/LICENSE
--rw-r--r--   0        0        0    10857 2023-05-21 09:38:29.925030 alfred_cli-2.0.0b3/README.md
--rw-r--r--   0        0        0     1584 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/pyproject.toml
--rw-r--r--   0        0        0      284 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/__init__.py
--rw-r--r--   0        0        0     1483 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/alfred_command.py
--rw-r--r--   0        0        0     5527 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/cli.py
--rw-r--r--   0        0        0     5614 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/commands.py
--rw-r--r--   0        0        0     3486 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/ctx.py
--rw-r--r--   0        0        0      682 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/decorator.py
--rw-r--r--   0        0        0        0 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/domain/__init__.py
--rw-r--r--   0        0        0     2404 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/domain/command.py
--rw-r--r--   0        0        0     1470 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/domain/manifest.py
--rw-r--r--   0        0        0      605 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/echo.py
--rw-r--r--   0        0        0      645 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/exceptions.py
--rw-r--r--   0        0        0     2978 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/interpreter.py
--rw-r--r--   0        0        0     2605 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/lib.py
--rw-r--r--   0        0        0      208 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/logger.py
--rw-r--r--   0        0        0     9465 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/main.py
--rw-r--r--   0        0        0     7872 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/manifest.py
--rw-r--r--   0        0        0      619 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/os.py
--rw-r--r--   0        0        0      432 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/resources/.alfred.toml
--rw-r--r--   0        0        0        0 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/resources/__init__.py
--rw-r--r--   0        0        0      168 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/resources/cmd.py
--rw-r--r--   0        0        0    12199 1970-01-01 00:00:00.000000 alfred_cli-2.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-24 05:13:29.562518 alfred_cli-2.1.0/LICENSE
+-rw-r--r--   0        0        0    10971 2023-06-24 05:13:29.562518 alfred_cli-2.1.0/README.md
+-rw-r--r--   0        0        0     1582 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/__init__.py
+-rw-r--r--   0        0        0     1483 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/alfred_command.py
+-rw-r--r--   0        0        0     5994 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/cli.py
+-rw-r--r--   0        0        0     5614 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/commands.py
+-rw-r--r--   0        0        0     3486 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/ctx.py
+-rw-r--r--   0        0        0     2666 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/decorator.py
+-rw-r--r--   0        0        0        0 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/domain/__init__.py
+-rw-r--r--   0        0        0     2404 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/domain/command.py
+-rw-r--r--   0        0        0     1470 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/domain/manifest.py
+-rw-r--r--   0        0        0      605 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/echo.py
+-rw-r--r--   0        0        0      645 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/exceptions.py
+-rw-r--r--   0        0        0     2978 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/interpreter.py
+-rw-r--r--   0        0        0     2638 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/lib.py
+-rw-r--r--   0        0        0      208 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/logger.py
+-rw-r--r--   0        0        0     9465 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/main.py
+-rw-r--r--   0        0        0     9168 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/manifest.py
+-rw-r--r--   0        0        0      619 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/os.py
+-rw-r--r--   0        0        0      432 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/resources/.alfred.toml
+-rw-r--r--   0        0        0        0 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/resources/__init__.py
+-rw-r--r--   0        0        0     1367 2023-06-24 05:13:29.570518 alfred_cli-2.1.0/src/alfred/resources/cmd.py
+-rw-r--r--   0        0        0    12311 1970-01-01 00:00:00.000000 alfred_cli-2.1.0/PKG-INFO
```

### Comparing `alfred_cli-2.0.0b3/LICENSE` & `alfred_cli-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b3/README.md` & `alfred_cli-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ## Alfred
 
-Alfred is an extensible building tool that can replace a Makefile or Fabric.
+Alfred is an extensible automation tool. It allows you to build your **continuous integration scripts** in python, and much more. You can replace any scripts using **the best of both worlds, shell and python**.
 
-It allows you to build your **continuous integration scripts** in python, and much more. You can replace any scripts using the best of both worlds, shell and python.
+[![asciicast](https://asciinema.org/a/i7YVDmQBRYVKAq1k74n9oYp0x.svg)](https://asciinema.org/a/i7YVDmQBRYVKAq1k74n9oYp0x)
+**introductory video on using alfred**
 
 Want to try and look for inspiration, here are examples of commands that I implement in my projects :
 
 ```bash
 alfred ci # run your own continuous integration process
 alfred publish # publish a package on pypi
 alfred run # run your app
@@ -46,25 +47,30 @@
 <!-- TOC end -->
 
 ## Getting started
 
 To configure a python project to use alfred, here is the procedure:
 
 ```bash
-pip3 install alfred-cli
+pip install alfred-cli
 alfred init
 ```
 
-Une première commande a été crée pour vous. Elle vous permet de tester alfred.
+You can run alfred to see the available commands.
 
 ```bash
-alfred hello_world --name "Fabien"
+alfred
 ```
 
-A file `.alfred.toml` will be initialized at the root of the repository.
+The "hello_world" command is created automatically during initialization. It serves as an introduction to Alfred.
+
+
+```bash
+alfred hello_world
+```
 
 ## Links
 
 * Documentation : https://alfred-cli.readthedocs.io/en/latest
 * PyPI Release : https://pypi.org/project/alfred-cli
 * Source code: https://github.com/FabienArcellier/alfred-cli
 * Chat: https://discord.gg/nMn9YPRGSY
@@ -78,16 +84,16 @@
 
 *alfred/lint.py*
 ```python
 import alfred
 
 @alfred.command('lint', help="validate your product using mypy")
 def lint():
-    pylint = alfred.sh('mypy', "mypy is not installed")
-    alfred.run(pylint, ["src/alfred"])
+    mypy = alfred.sh('mypy', "mypy is not installed")
+    alfred.run(mypy, ["src/alfred"])
 ```
 
 ### Write your first workflow
 
 *alfred/ci.py*
 ```python
 import alfred
@@ -100,15 +106,15 @@
 
 ## Benefits
 
 ### Alfred scales with your team
 
 Alfred grows with your team. You can start with one command and then add more. When you feel that your command file is too crowded, you can restructure it into several files, or even separate it into several subfolders. Alfred is able to search all your orders by scanning a folder and its subfolders. It's all configurable.
 
-### Alfred likes mono-repository
+### Alfred loves mono-repository
 
 Alfred is built with the idea of being usable in a mono-repository which brings together several python, react, node projects in the same code repository. You can create several alfred sub-projects. At the root of the project, you will have access to all the commands of all the subprojects using the subproject name ``alfred project1 ci``.
 
 ## Behind the scene
 
 Alfred rely heavily on click and plumblum :
 
@@ -123,31 +129,31 @@
 
 Alfred allows you to mix shell code with python instructions. In some cases, it allows you to perform efficient processing on API calls. You can use either the cli (for git, ...) or pythons libraries depending on the nature of the treatment you want to perform.
 
 In our development process, we frequently need to operate on application with several process (frontend in react, server in flask, two external service in flask). To mount those process, we use `honcho` with alfred to load `Procfile` that will manage those process.
 
 ## Why not using alfred
 
-If you want to create a cli you will distribute, alfred is not designed for that. I won't recommand as well to use it to build a data application even if you can use python and many library.
+Alfred is not designed to build a cli you will distribute on pypi. You should use [click](https://click.palletsprojects.com/en/8.0.x/) for that.
 
-Alfred command can import only installed library. You can't use relative import. That makes difficult to share code between your commands.
+Alfred command can import only installed library. You can't use relative import in command module. You have to extend python path to share function between commands.
 
 ## The latest version
 
 You can find the latest version to ...
 
 ```bash
 git clone https://github.com/FabienArcellier/alfred-cli.git
 ```
 
 ## Cookbook
 
-### Display the commands really executed
+### Use debug mode
 
-You can display the commands really executed, either to debug the arguments,
+You can display the shell commands really executed, either to debug the arguments,
 either to run in your terminal again with other attributes.
 
 The option `d` / `--debug` display all the shell commands that are executed by
 `alfred.run()` in your alfred command.
 
 ```bash
 $ alfred -d ci
@@ -188,27 +194,15 @@
     with alfred.env(SCREEN="display"):
         bash = alfred.sh("bash")
         bash.run("-c" "echo $SCREEN")
 ```
 
 #### Add directories into pythonpath
 
-Adding a folder in the pythonpath variable allows you to expose packages without declaring them in the manifest.
-
-This pattern is useful with poetry to be able to reuse the code of the package tests in this one for example.
-
-The ``alfred.pythonpath`` decorator adds the project root. You can save specific folders here.
-
-```python
-@alfred.command('ci', help="execute continuous integration process of alfred")
-@alfred.pythonpath()
-def ci():
-    bash = alfred.sh("bash")
-    alfred.run(bash, ["-c" "echo $SCREEN"])
-```
+Adding a folder in the pythonpath variable allows you to expose packages without declaring them in ``pyproject.toml``.
 
 ```python
 @alfred.command('ci', help="execute continuous integration process of alfred")
 @alfred.pythonpath(['tests'], append_project=False)
 def ci():
     bash = alfred.sh("bash")
     alfred.run(bash, ["-c", "echo $SCREEN"])
@@ -218,14 +212,23 @@
 @alfred.command('ci', help="execute continuous integration process of alfred")
 def ci():
     with alfred.pythonpath():
         bash = alfred.sh("bash")
         alfred.run(bash, ["-c", "echo $SCREEN"])
 ```
 
+The ``alfred.pythonpath`` decorator adds the project root. You can save specific folders here. It's useful if you have deactivate ``python_path_project_root`` in ``.alfred.toml``, otherwise, it's already imported.
+
+```python
+@alfred.command('ci', help="execute continuous integration process of alfred")
+@alfred.pythonpath()
+def ci():
+    bash = alfred.sh("bash")
+    alfred.run(bash, ["-c" "echo $SCREEN"])
+```
 
 ## Developper guideline
 
 ```bash
 poetry install
 poetry shell
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alfred_cli-2.0.0b3/pyproject.toml` & `alfred_cli-2.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alfred-cli"
-version = "2.0.0b3"
+version = "2.1.0"
 description = "alfred is an extensible building tool that can replace a Makefile or Fabric. Writing commands in python is done in minutes."
 authors = ["Fabien Arcellier <fabien.arcellier@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "alfred", from = "src"}]
 include = [
     { path = "alfred/resources/*" }
```

### Comparing `alfred_cli-2.0.0b3/src/alfred/alfred_command.py` & `alfred_cli-2.1.0/src/alfred/alfred_command.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b3/src/alfred/cli.py` & `alfred_cli-2.1.0/src/alfred/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,20 +148,33 @@
 
 @contextlib.contextmanager
 def _context_middleware() -> Generator[None, None, None]:
     """
     the context code is executed before executing
     the user's target command.
     """
+    pathsep = os.pathsep
     pythonpath = os.environ.get("PYTHONPATH", "")
-    if manifest.python_path_project_root():
-        _pythonpath = pythonpath.split(':')
+    if manifest.pythonpath_project_root():
+        _pythonpath = pythonpath.split(pathsep)
         root_directory = project_directory()
         _pythonpath.append(root_directory)
-        pythonpath = ":".join(_pythonpath)
+        pythonpath = pathsep.join(_pythonpath)
+
+    extensions = manifest.pythonpath_extends()
+    if len(extensions) > 0:
+        _pythonpath = pythonpath.split(pathsep)
+        root_directory = project_directory()
+        for extension in extensions:
+            if os.path.isabs(extension):
+                _pythonpath.append(extension)
+            else:
+                _pythonpath.append(os.path.join(root_directory, extension))
+
+        pythonpath = pathsep.join(_pythonpath)
 
     with override_pythonpath(pythonpath):
         yield
 
 
 if __name__ == '__main__':
     cli()  # pylint: disable=no-value-for-parameter
```

### Comparing `alfred_cli-2.0.0b3/src/alfred/commands.py` & `alfred_cli-2.1.0/src/alfred/commands.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b3/src/alfred/ctx.py` & `alfred_cli-2.1.0/src/alfred/ctx.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b3/src/alfred/domain/command.py` & `alfred_cli-2.1.0/src/alfred/domain/command.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b3/src/alfred/domain/manifest.py` & `alfred_cli-2.1.0/src/alfred/domain/manifest.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b3/src/alfred/echo.py` & `alfred_cli-2.1.0/src/alfred/echo.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b3/src/alfred/exceptions.py` & `alfred_cli-2.1.0/src/alfred/exceptions.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b3/src/alfred/interpreter.py` & `alfred_cli-2.1.0/src/alfred/interpreter.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b3/src/alfred/lib.py` & `alfred_cli-2.1.0/src/alfred/lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,19 +64,20 @@
     """
     Override the pythonpath variable in a generalized way
 
     * override the environment variable in python
     * override pythonpath environment variable in plumbum
     * override sys.path
     """
+    pathsep = os.pathsep
     logger = get_logger()
     logger.debug(f"override PYTHONPATH: {pythonpath}")
 
     previous_pythonpath = os.getenv('PYTHONPATH', '')
     with local.env(PYTHONPATH=pythonpath):
         os.environ['PYTHONPATH'] = pythonpath
-        sys.path = pythonpath.split(':')
+        sys.path = pythonpath.split(pathsep)
         try:
             yield
         finally:
             os.environ['PYTHONPATH'] = previous_pythonpath
-            sys.path = previous_pythonpath.split(':')
+            sys.path = previous_pythonpath.split(pathsep)
```

### Comparing `alfred_cli-2.0.0b3/src/alfred/main.py` & `alfred_cli-2.1.0/src/alfred/main.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b3/src/alfred/manifest.py` & `alfred_cli-2.1.0/src/alfred/manifest.py`

 * *Files 11% similar despite different names*

```diff
@@ -186,29 +186,61 @@
 
     if 'prefix' not in configuration['alfred']:
         return _default
 
     return configuration['alfred']['prefix']
 
 
-def python_path_project_root(project_dir: Optional[str] = None) -> Optional[bool]:
+def pythonpath_project_root(project_dir: Optional[str] = None) -> Optional[bool]:
     alfred_manifest = lookup(project_dir)
     configuration = alfred_manifest.configuration
 
     _default = True
     if 'alfred' not in configuration:
         return _default
 
     if 'project' not in configuration['alfred']:
         return _default
 
-    if 'python_path_project_root' not in configuration['alfred']['project']:
+    official_parameter = 'pythonpath_project_root'
+    if official_parameter in configuration['alfred']['project']:
+        return configuration['alfred']['project'][official_parameter]
+
+    legacy_parameters = ['python_path_project_root']
+    for legacy_parameter in legacy_parameters:
+        if legacy_parameter in configuration['alfred']['project']:
+            logger.warning(f"project parameter {legacy_parameter} is deprecated in {project_dir}, use {official_parameter} instead")
+            return configuration['alfred']['project'][legacy_parameter]
+
+    return _default
+
+
+def pythonpath_extends(project_dir: Optional[str] = None) -> List[str]:
+    alfred_manifest = lookup(project_dir)
+    configuration = alfred_manifest.configuration
+
+    _default = []
+    if 'alfred' not in configuration:
+        return _default
+
+    if 'project' not in configuration['alfred']:
         return _default
 
-    return configuration['alfred']['project']['python_path_project_root']
+    official_parameter = 'pythonpath_extends'
+    if official_parameter in configuration['alfred']['project']:
+        return configuration['alfred']['project'][official_parameter]
+
+
+    legacy_parameters = ['python_path_extends']
+    for legacy_parameter in legacy_parameters:
+        if legacy_parameter in configuration['alfred']['project']:
+            logger.warning(f"project parameter {legacy_parameter} is deprecated in {project_dir}, use {official_parameter} instead")
+            return configuration['alfred']['project'][legacy_parameter]
+
+    return _default
 
 
 def name(project_dir: Optional[str] = None) -> Optional[str]:
     """
     Récupère le nom du projet depuis le manifest ``.alfred.toml``.
 
     >>> project_name = manifest.name()
```

### Comparing `alfred_cli-2.0.0b3/src/alfred/os.py` & `alfred_cli-2.1.0/src/alfred/os.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b3/PKG-INFO` & `alfred_cli-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-cli
-Version: 2.0.0b3
+Version: 2.1.0
 Summary: alfred is an extensible building tool that can replace a Makefile or Fabric. Writing commands in python is done in minutes.
 Home-page: https://github.com/FabienArcellier/alfred-cli#alfred
 License: MIT
 Keywords: building tool,makefile,productivity,automation,continuous integration,developper friendly
 Author: Fabien Arcellier
 Author-email: fabien.arcellier@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -25,17 +25,18 @@
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://alfred-cli.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/FabienArcellier/alfred-cli
 Description-Content-Type: text/markdown
 
 ## Alfred
 
-Alfred is an extensible building tool that can replace a Makefile or Fabric.
+Alfred is an extensible automation tool. It allows you to build your **continuous integration scripts** in python, and much more. You can replace any scripts using **the best of both worlds, shell and python**.
 
-It allows you to build your **continuous integration scripts** in python, and much more. You can replace any scripts using the best of both worlds, shell and python.
+[![asciicast](https://asciinema.org/a/i7YVDmQBRYVKAq1k74n9oYp0x.svg)](https://asciinema.org/a/i7YVDmQBRYVKAq1k74n9oYp0x)
+**introductory video on using alfred**
 
 Want to try and look for inspiration, here are examples of commands that I implement in my projects :
 
 ```bash
 alfred ci # run your own continuous integration process
 alfred publish # publish a package on pypi
 alfred run # run your app
@@ -75,25 +76,30 @@
 <!-- TOC end -->
 
 ## Getting started
 
 To configure a python project to use alfred, here is the procedure:
 
 ```bash
-pip3 install alfred-cli
+pip install alfred-cli
 alfred init
 ```
 
-Une première commande a été crée pour vous. Elle vous permet de tester alfred.
+You can run alfred to see the available commands.
 
 ```bash
-alfred hello_world --name "Fabien"
+alfred
 ```
 
-A file `.alfred.toml` will be initialized at the root of the repository.
+The "hello_world" command is created automatically during initialization. It serves as an introduction to Alfred.
+
+
+```bash
+alfred hello_world
+```
 
 ## Links
 
 * Documentation : https://alfred-cli.readthedocs.io/en/latest
 * PyPI Release : https://pypi.org/project/alfred-cli
 * Source code: https://github.com/FabienArcellier/alfred-cli
 * Chat: https://discord.gg/nMn9YPRGSY
@@ -107,16 +113,16 @@
 
 *alfred/lint.py*
 ```python
 import alfred
 
 @alfred.command('lint', help="validate your product using mypy")
 def lint():
-    pylint = alfred.sh('mypy', "mypy is not installed")
-    alfred.run(pylint, ["src/alfred"])
+    mypy = alfred.sh('mypy', "mypy is not installed")
+    alfred.run(mypy, ["src/alfred"])
 ```
 
 ### Write your first workflow
 
 *alfred/ci.py*
 ```python
 import alfred
@@ -129,15 +135,15 @@
 
 ## Benefits
 
 ### Alfred scales with your team
 
 Alfred grows with your team. You can start with one command and then add more. When you feel that your command file is too crowded, you can restructure it into several files, or even separate it into several subfolders. Alfred is able to search all your orders by scanning a folder and its subfolders. It's all configurable.
 
-### Alfred likes mono-repository
+### Alfred loves mono-repository
 
 Alfred is built with the idea of being usable in a mono-repository which brings together several python, react, node projects in the same code repository. You can create several alfred sub-projects. At the root of the project, you will have access to all the commands of all the subprojects using the subproject name ``alfred project1 ci``.
 
 ## Behind the scene
 
 Alfred rely heavily on click and plumblum :
 
@@ -152,31 +158,31 @@
 
 Alfred allows you to mix shell code with python instructions. In some cases, it allows you to perform efficient processing on API calls. You can use either the cli (for git, ...) or pythons libraries depending on the nature of the treatment you want to perform.
 
 In our development process, we frequently need to operate on application with several process (frontend in react, server in flask, two external service in flask). To mount those process, we use `honcho` with alfred to load `Procfile` that will manage those process.
 
 ## Why not using alfred
 
-If you want to create a cli you will distribute, alfred is not designed for that. I won't recommand as well to use it to build a data application even if you can use python and many library.
+Alfred is not designed to build a cli you will distribute on pypi. You should use [click](https://click.palletsprojects.com/en/8.0.x/) for that.
 
-Alfred command can import only installed library. You can't use relative import. That makes difficult to share code between your commands.
+Alfred command can import only installed library. You can't use relative import in command module. You have to extend python path to share function between commands.
 
 ## The latest version
 
 You can find the latest version to ...
 
 ```bash
 git clone https://github.com/FabienArcellier/alfred-cli.git
 ```
 
 ## Cookbook
 
-### Display the commands really executed
+### Use debug mode
 
-You can display the commands really executed, either to debug the arguments,
+You can display the shell commands really executed, either to debug the arguments,
 either to run in your terminal again with other attributes.
 
 The option `d` / `--debug` display all the shell commands that are executed by
 `alfred.run()` in your alfred command.
 
 ```bash
 $ alfred -d ci
@@ -217,27 +223,15 @@
     with alfred.env(SCREEN="display"):
         bash = alfred.sh("bash")
         bash.run("-c" "echo $SCREEN")
 ```
 
 #### Add directories into pythonpath
 
-Adding a folder in the pythonpath variable allows you to expose packages without declaring them in the manifest.
-
-This pattern is useful with poetry to be able to reuse the code of the package tests in this one for example.
-
-The ``alfred.pythonpath`` decorator adds the project root. You can save specific folders here.
-
-```python
-@alfred.command('ci', help="execute continuous integration process of alfred")
-@alfred.pythonpath()
-def ci():
-    bash = alfred.sh("bash")
-    alfred.run(bash, ["-c" "echo $SCREEN"])
-```
+Adding a folder in the pythonpath variable allows you to expose packages without declaring them in ``pyproject.toml``.
 
 ```python
 @alfred.command('ci', help="execute continuous integration process of alfred")
 @alfred.pythonpath(['tests'], append_project=False)
 def ci():
     bash = alfred.sh("bash")
     alfred.run(bash, ["-c", "echo $SCREEN"])
@@ -247,14 +241,23 @@
 @alfred.command('ci', help="execute continuous integration process of alfred")
 def ci():
     with alfred.pythonpath():
         bash = alfred.sh("bash")
         alfred.run(bash, ["-c", "echo $SCREEN"])
 ```
 
+The ``alfred.pythonpath`` decorator adds the project root. You can save specific folders here. It's useful if you have deactivate ``python_path_project_root`` in ``.alfred.toml``, otherwise, it's already imported.
+
+```python
+@alfred.command('ci', help="execute continuous integration process of alfred")
+@alfred.pythonpath()
+def ci():
+    bash = alfred.sh("bash")
+    alfred.run(bash, ["-c" "echo $SCREEN"])
+```
 
 ## Developper guideline
 
 ```bash
 poetry install
 poetry shell
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

