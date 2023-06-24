# Comparing `tmp/python_simpleconf-0.5.8.tar.gz` & `tmp/python_simpleconf-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_simpleconf-0.5.8.tar", max compression
+gzip compressed data, was "python_simpleconf-0.5.9.tar", max compression
```

## Comparing `python_simpleconf-0.5.8.tar` & `python_simpleconf-0.5.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1056 2023-06-24 05:58:42.152358 python_simpleconf-0.5.8/LICENSE
--rw-r--r--   0        0        0     5173 2023-06-24 05:58:42.152358 python_simpleconf-0.5.8/README.md
--rw-r--r--   0        0        0     1218 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/pyproject.toml
--rw-r--r--   0        0        0       65 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/__init__.py
--rw-r--r--   0        0        0     2319 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/caster.py
--rw-r--r--   0        0        0     7558 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/config.py
--rw-r--r--   0        0        0      172 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/exceptions.py
--rw-r--r--   0        0        0     1164 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/__init__.py
--rw-r--r--   0        0        0      258 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/dict.py
--rw-r--r--   0        0        0     1525 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/env.py
--rw-r--r--   0        0        0     1991 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/ini.py
--rw-r--r--   0        0        0      401 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/json.py
--rw-r--r--   0        0        0     1602 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/osenv.py
--rw-r--r--   0        0        0      593 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/toml.py
--rw-r--r--   0        0        0      490 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/loaders/yaml.py
--rw-r--r--   0        0        0     1750 2023-06-24 05:58:42.156358 python_simpleconf-0.5.8/simpleconf/utils.py
--rw-r--r--   0        0        0     6303 1970-01-01 00:00:00.000000 python_simpleconf-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/LICENSE
+-rw-r--r--   0        0        0     5173 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/README.md
+-rw-r--r--   0        0        0     1220 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/simpleconf/__init__.py
+-rw-r--r--   0        0        0     2319 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/simpleconf/caster.py
+-rw-r--r--   0        0        0     7642 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/simpleconf/config.py
+-rw-r--r--   0        0        0      172 2023-06-24 16:51:31.450085 python_simpleconf-0.5.9/simpleconf/exceptions.py
+-rw-r--r--   0        0        0     1164 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/__init__.py
+-rw-r--r--   0        0        0      258 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/dict.py
+-rw-r--r--   0        0        0     1525 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/env.py
+-rw-r--r--   0        0        0     1991 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/ini.py
+-rw-r--r--   0        0        0      401 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/json.py
+-rw-r--r--   0        0        0     1602 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/osenv.py
+-rw-r--r--   0        0        0      593 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/toml.py
+-rw-r--r--   0        0        0      490 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/loaders/yaml.py
+-rw-r--r--   0        0        0     1750 2023-06-24 16:51:31.454085 python_simpleconf-0.5.9/simpleconf/utils.py
+-rw-r--r--   0        0        0     6307 1970-01-01 00:00:00.000000 python_simpleconf-0.5.9/PKG-INFO
```

### Comparing `python_simpleconf-0.5.8/LICENSE` & `python_simpleconf-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.8/README.md` & `python_simpleconf-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.8/pyproject.toml` & `python_simpleconf-0.5.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "python-simpleconf"
-version = "0.5.8"
+version = "0.5.9"
 description = "Simple configuration management with python."
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/simpleconf"
 repository = "https://github.com/pwwang/simpleconf"
 packages = [
     {include = "simpleconf"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-diot = "^0.2"
+diot = "^0.2.1"
 python-dotenv = { version="^0.21", optional = true}
 pyyaml = { version="^6", optional = true}
 rtoml = {version = "^0.8", optional = true}
 iniconfig = {version = "^2.0", optional = true}
 
 [tool.poetry.extras]
 ini = [ "iniconfig" ]
```

### Comparing `python_simpleconf-0.5.8/simpleconf/caster.py` & `python_simpleconf-0.5.9/simpleconf/caster.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.8/simpleconf/config.py` & `python_simpleconf-0.5.9/simpleconf/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             A Diot object with the loaded configurations
         """
         out = Diot()
         for conf in configs:
             ext = config_to_ext(conf)
             loader = get_loader(ext)
             loaded = loader.load(conf, ignore_nonexist)
-            out.update(loaded)
+            out.update_recursively(loaded)
 
         return out
 
     @staticmethod
     def load_one(
         config, loader: str = None, ignore_nonexist: bool = False
     ) -> Diot:
@@ -79,15 +79,15 @@
         for conf in configs:
             ext = config_to_ext(conf)
             loader = get_loader(ext)
             loaded = loader.load_with_profiles(conf, ignore_nonexist)
             for profile, value in loaded.items():
                 profile = profile.lower()
                 pool.setdefault(profile, Diot())
-                pool[profile].update(value)
+                pool[profile].update_recursively(value)
 
         ProfileConfig.use_profile(out, "default")
         return out
 
     @staticmethod
     def load_one(
         conf: Any, loader: str = None, ignore_nonexist: bool = False
@@ -117,15 +117,15 @@
         else:
             loader = get_loader(loader)
 
         loaded = loader.load_with_profiles(conf, ignore_nonexist)
         for profile, value in loaded.items():
             profile = profile.lower()
             pool.setdefault(profile, Diot())
-            pool[profile].update(value)
+            pool[profile].update_recursively(value)
 
         ProfileConfig.use_profile(out, "default")
         return out
 
     @staticmethod
     def use_profile(
         conf: Diot,
@@ -145,29 +145,29 @@
             The configuration object with the switched profile if copy is True
             Otherwise None (updated in-place)
         """
         pool = conf[POOL_KEY]
         if copy:
             out = Diot({POOL_KEY: pool, META_KEY: conf[META_KEY].copy()})
             if base is not None:
-                out.update(pool[base])
+                out.update_recursively(pool[base])
             out[META_KEY]["current_profile"] = profile
             out[META_KEY]["base_profile"] = base
-            out.update(pool[profile])
+            out.update_recursively(pool[profile])
             return out
 
         # copy = False
         for key in list(conf):
             if key in (POOL_KEY, META_KEY):
                 continue
             del conf[key]
 
         if base is not None:
-            conf.update(pool[base])
-        conf.update(pool[profile])
+            conf.update_recursively(pool[base])
+        conf.update_recursively(pool[profile])
         conf[META_KEY]["current_profile"] = profile
         conf[META_KEY]["base_profile"] = base
 
     @staticmethod
     def current_profile(conf: Diot) -> str:
         """Get the current profile"""
         return conf[META_KEY]["current_profile"]
```

### Comparing `python_simpleconf-0.5.8/simpleconf/loaders/__init__.py` & `python_simpleconf-0.5.9/simpleconf/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.8/simpleconf/loaders/env.py` & `python_simpleconf-0.5.9/simpleconf/loaders/env.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.8/simpleconf/loaders/ini.py` & `python_simpleconf-0.5.9/simpleconf/loaders/ini.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.8/simpleconf/loaders/osenv.py` & `python_simpleconf-0.5.9/simpleconf/loaders/osenv.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.8/simpleconf/loaders/toml.py` & `python_simpleconf-0.5.9/simpleconf/loaders/toml.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.8/simpleconf/utils.py` & `python_simpleconf-0.5.9/simpleconf/utils.py`

 * *Files identical despite different names*

### Comparing `python_simpleconf-0.5.8/PKG-INFO` & `python_simpleconf-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-simpleconf
-Version: 0.5.8
+Version: 0.5.9
 Summary: Simple configuration management with python.
 Home-page: https://github.com/pwwang/simpleconf
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: env
 Provides-Extra: ini
 Provides-Extra: toml
 Provides-Extra: yaml
-Requires-Dist: diot (>=0.2,<0.3)
+Requires-Dist: diot (>=0.2.1,<0.3.0)
 Requires-Dist: iniconfig (>=2.0,<3.0) ; extra == "ini" or extra == "all"
 Requires-Dist: python-dotenv (>=0.21,<0.22) ; extra == "env" or extra == "all"
 Requires-Dist: pyyaml (>=6,<7) ; extra == "yaml" or extra == "all"
 Requires-Dist: rtoml (>=0.8,<0.9) ; extra == "toml" or extra == "all"
 Project-URL: Repository, https://github.com/pwwang/simpleconf
 Description-Content-Type: text/markdown
```

