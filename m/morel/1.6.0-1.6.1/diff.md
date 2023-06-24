# Comparing `tmp/morel-1.6.0.tar.gz` & `tmp/morel-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.6.0.tar", last modified: Fri Jun 23 22:13:53 2023, max compression
+gzip compressed data, was "morel-1.6.1.tar", last modified: Sat Jun 24 09:48:30 2023, max compression
```

## Comparing `morel-1.6.0.tar` & `morel-1.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-23 22:13:53.208881 morel-1.6.0/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.6.0/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-23 22:13:53.208881 morel-1.6.0/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.6.0/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-23 22:11:20.000000 morel-1.6.0/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-23 22:13:53.208881 morel-1.6.0/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-23 22:13:53.206881 morel-1.6.0/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-23 22:13:53.207881 morel-1.6.0/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.6.0/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     4012 2023-06-23 22:09:50.000000 morel-1.6.0/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.6.0/src/morel/exploit_template.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1022 2023-06-23 22:08:52.000000 morel-1.6.0/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.6.0/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.6.0/src/morel/singleton.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3927 2023-06-23 22:03:19.000000 morel-1.6.0/src/morel/target.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.6.0/src/morel/target_template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-23 22:13:53.208881 morel-1.6.0/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-23 22:13:53.000000 morel-1.6.0/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 09:48:30.153815 morel-1.6.1/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.6.1/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-24 09:48:30.153815 morel-1.6.1/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.6.1/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-24 09:48:22.000000 morel-1.6.1/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-24 09:48:30.153815 morel-1.6.1/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 09:48:30.151815 morel-1.6.1/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 09:48:30.152815 morel-1.6.1/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.6.1/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     4012 2023-06-23 22:09:50.000000 morel-1.6.1/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.6.1/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1022 2023-06-23 22:08:52.000000 morel-1.6.1/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.6.1/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-06-16 17:07:04.000000 morel-1.6.1/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     4040 2023-06-24 09:48:05.000000 morel-1.6.1/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.6.1/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-24 09:48:30.153815 morel-1.6.1/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-24 09:48:30.000000 morel-1.6.1/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-24 09:48:30.000000 morel-1.6.1/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-24 09:48:30.000000 morel-1.6.1/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-24 09:48:30.000000 morel-1.6.1/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-24 09:48:30.000000 morel-1.6.1/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-24 09:48:30.000000 morel-1.6.1/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.6.0/LICENSE` & `morel-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.6.0/PKG-INFO` & `morel-1.6.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.6.0
+Version: 1.6.1
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.6.0/pyproject.toml` & `morel-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.6.0"
+version = "1.6.1"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.6.0/src/morel/app.py` & `morel-1.6.1/src/morel/app.py`

 * *Files identical despite different names*

### Comparing `morel-1.6.0/src/morel/exploit_template.py` & `morel-1.6.1/src/morel/exploit_template.py`

 * *Files identical despite different names*

### Comparing `morel-1.6.0/src/morel/exploits.py` & `morel-1.6.1/src/morel/exploits.py`

 * *Files identical despite different names*

### Comparing `morel-1.6.0/src/morel/singleton.py` & `morel-1.6.1/src/morel/singleton.py`

 * *Files identical despite different names*

### Comparing `morel-1.6.0/src/morel/target.py` & `morel-1.6.1/src/morel/target.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,27 +90,31 @@
                     spec.loader.exec_module(module)  # type: ignore
                     targetfun = getattr(sys.modules[name], "main")
                     target_funcs.append(targetfun)
                 except Exception as e:
                     self.log.error(f"Exception while importing module {name}:\n{e}")
             self.target_functions = target_funcs
             self.log.info(f"Target functions: {self.target_functions}")
+        self.log.debug(f"loader released lock")
 
     def fetch_new_targets(self):
         with self._lock:
             if time.time() - self.last_update > 2:
                 for function in self.target_functions:
                     try:
                         target = function()
                         # self.log.debug(f"{target = }")
                         self.append(target)
                     except Exception as e:
                         self.log.warning(f"{function} raised an exception:\n{e}")
                         continue
                 self.last_update = time.time()
+        self.log.debug(f"fetcher released lock")
+
+        return
 
 
 Targets = _Targets()
 
 
 if __name__ == "__main__":
     Targets.setBaseDir("tests/targets")
```

### Comparing `morel-1.6.0/src/morel.egg-info/PKG-INFO` & `morel-1.6.1/src/morel.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.6.0
+Version: 1.6.1
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

