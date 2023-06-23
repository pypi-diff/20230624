# Comparing `tmp/morel-1.5.2.tar.gz` & `tmp/morel-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.5.2.tar", last modified: Fri Jun 16 21:11:34 2023, max compression
+gzip compressed data, was "morel-1.6.0.tar", last modified: Fri Jun 23 22:13:53 2023, max compression
```

## Comparing `morel-1.5.2.tar` & `morel-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:11:34.796580 morel-1.5.2/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.5.2/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 21:11:34.796580 morel-1.5.2/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.5.2/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-16 21:11:04.000000 morel-1.5.2/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-16 21:11:34.796580 morel-1.5.2/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:11:34.794581 morel-1.5.2/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:11:34.795580 morel-1.5.2/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.5.2/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.5.2/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.5.2/src/morel/exploit_template.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.5.2/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.5.2/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.5.2/src/morel/singleton.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3684 2023-06-16 21:09:41.000000 morel-1.5.2/src/morel/target.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.5.2/src/morel/target_template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-16 21:11:34.796580 morel-1.5.2/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-16 21:11:34.000000 morel-1.5.2/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-23 22:13:53.208881 morel-1.6.0/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.6.0/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-23 22:13:53.208881 morel-1.6.0/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.6.0/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-23 22:11:20.000000 morel-1.6.0/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-23 22:13:53.208881 morel-1.6.0/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-23 22:13:53.206881 morel-1.6.0/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-23 22:13:53.207881 morel-1.6.0/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.6.0/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     4012 2023-06-23 22:09:50.000000 morel-1.6.0/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.6.0/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1022 2023-06-23 22:08:52.000000 morel-1.6.0/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.6.0/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.6.0/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3927 2023-06-23 22:03:19.000000 morel-1.6.0/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.6.0/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-23 22:13:53.208881 morel-1.6.0/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.5.2/LICENSE` & `morel-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.5.2/PKG-INFO` & `morel-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.5.2
+Version: 1.6.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.5.2/pyproject.toml` & `morel-1.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.5.2"
+version = "1.6.0"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.5.2/src/morel/app.py` & `morel-1.6.0/src/morel/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import sys
 import click
 import importlib
 
 from pathlib import Path
 from threading import Thread
 
+from morel.target import Targets
+
 from .exploits import launchAttack
 
 with open(Path(Path(__file__).parent, "exploit_template.py")) as fs:
     exploit_template = fs.read()
 
 with open(Path(Path(__file__).parent, "target_template.py")) as fs:
     target_template = fs.read()
@@ -65,22 +67,26 @@
     type=click.STRING,
     default="0.0.0.0",
     show_default=True,
     prompt="Target IP",
 )
 @click.argument("filename", required=True, type=click.Path(exists=True))
 def test(target, filename):
-    """Test your exploit against a target ip"""
+    """Test your exploit against a target ip. If you want to use the global Targets dictionary place your target functions inside a folder named 'targets' placed in the current working directory"""
     if os.system("ping -c 1 " + target + " > /dev/null") != 0:
         click.echo(f"Host {target} is unreachable")
         return
     click.echo(f"Testing {filename} on {target}")
     filename = Path(filename)
     name = filename.stem
 
+    Targets.setBaseDir("targets")
+    Targets.load_target_functions()
+    Targets.fetch_new_targets()
+
     try:
         spec = importlib.util.spec_from_file_location(name, filename.resolve())
         module = importlib.util.module_from_spec(spec)  # type: ignore
         sys.modules[name] = module
         spec.loader.exec_module(module)  # type: ignore
         exploitfun = getattr(sys.modules[name], "main")
     except Exception as e:
```

### Comparing `morel-1.5.2/src/morel/exploit_template.py` & `morel-1.6.0/src/morel/exploit_template.py`

 * *Files identical despite different names*

### Comparing `morel-1.5.2/src/morel/exploits.py` & `morel-1.6.0/src/morel/exploits.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def find_flags(flags: list[str]):
     valid_flags = []
 
     if isinstance(flags, str):
         flags = [
             flags,
         ]
-    print(os.environ["FLAG_REGEX"])
+
     if os.environ["FLAG_REGEX"] != "None":
         for flag in flags:
             m = re.finditer(pattern=os.environ["FLAG_REGEX"], string=flag)
             if m:
                 for f in m:
                     valid_flags.append(f.group())
```

### Comparing `morel-1.5.2/src/morel/singleton.py` & `morel-1.6.0/src/morel/singleton.py`

 * *Files identical despite different names*

### Comparing `morel-1.5.2/src/morel/target.py` & `morel-1.6.0/src/morel/target.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 from morel.logger import logger
 
 
 class _restrictedDict(UserDict):
     def __init__(self, initialD={}):
         super().__init__(initialD)
 
-    # def __getitem__(self, key):
-    #    return UserDict.__getitem__(self, key)
+    def __getitem__(self, key):
+        return UserDict.__getitem__(self, key)
 
-    # def __setitem__(self, key, val):
-    #    UserDict.__setitem__(self, key, val)
+    def __setitem__(self, key, val):
+        UserDict.__setitem__(self, key, val)
 
     def append(self, dict2) -> None:  # inplace
         dict2 = _restrictedDict(dict2)
         # print(dict2)
         for k, v in dict2.items():
             if k not in self:
                 self[k] = v
@@ -55,15 +55,16 @@
         super().__init__()
         self._lock = Lock()
         self.target_functions = []
         self.log = logger
         self.last_update = 0
 
     # def __getitem__(self, key):
-    #    return dict.__getitem__(self, key)
+    #    with self._lock:
+    #        return _restrictedDict.__getitem__(self, key)
 
     def setBaseDir(self, dir):
         self.p = Path(dir)
 
     def setLogger(self, logger):
         self.log = logger
 
@@ -86,25 +87,29 @@
                     spec = importlib.util.spec_from_file_location(name, targ.resolve())
                     module = importlib.util.module_from_spec(spec)  # type: ignore
                     sys.modules[name] = module
                     spec.loader.exec_module(module)  # type: ignore
                     targetfun = getattr(sys.modules[name], "main")
                     target_funcs.append(targetfun)
                 except Exception as e:
-                    self.log.error(f"Exception on module {name}:\n{e}")
+                    self.log.error(f"Exception while importing module {name}:\n{e}")
             self.target_functions = target_funcs
             self.log.info(f"Target functions: {self.target_functions}")
 
     def fetch_new_targets(self):
         with self._lock:
             if time.time() - self.last_update > 2:
                 for function in self.target_functions:
-                    target = function()
-                    # self.log.debug(f"{target = }")
-                    self.append(target)
+                    try:
+                        target = function()
+                        # self.log.debug(f"{target = }")
+                        self.append(target)
+                    except Exception as e:
+                        self.log.warning(f"{function} raised an exception:\n{e}")
+                        continue
                 self.last_update = time.time()
 
 
 Targets = _Targets()
 
 
 if __name__ == "__main__":
```

### Comparing `morel-1.5.2/src/morel.egg-info/PKG-INFO` & `morel-1.6.0/src/morel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.5.2
+Version: 1.6.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

