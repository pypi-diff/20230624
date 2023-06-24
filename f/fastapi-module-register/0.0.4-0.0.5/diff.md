# Comparing `tmp/fastapi_module_register-0.0.4.tar.gz` & `tmp/fastapi_module_register-0.0.5.tar.gz`

## Comparing `fastapi_module_register-0.0.4.tar` & `fastapi_module_register-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/README.en.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/__init__.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/base_register.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/constants.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/exceptions.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/logger.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/schema.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/utils.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/interface/method_interface.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/interface/register_interface.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/sqlmodel/__init__.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/sqlmodel/sqlmodel_method.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/sqlmodel/sqlmodel_reigster.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/sqlmodel/utils.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/tortoise/__init__.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/tortoise/tortoise_method.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/src/fastapi_module_register/tortoise/tortoise_register.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/tests/test_sqlmodel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/tests/test_tortoise.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/LICENSE
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/README.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/README.en.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/__init__.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/base_register.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/constants.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/exceptions.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/logger.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/schema.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/utils.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/interface/method_interface.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/interface/register_interface.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/sqlmodel/__init__.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/sqlmodel/sqlmodel_method.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/sqlmodel/sqlmodel_reigster.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/sqlmodel/utils.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/tortoise/__init__.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/tortoise/tortoise_method.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/src/fastapi_module_register/tortoise/tortoise_register.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/tests/test_sqlmodel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/tests/test_tortoise.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/LICENSE
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/README.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.5/PKG-INFO
```

### Comparing `fastapi_module_register-0.0.4/README.en.md` & `fastapi_module_register-0.0.5/README.en.md`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/base_register.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/base_register.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class BaseRegister(RegisterInterface):
 
     @classmethod
     def init(cls, app: FastAPI, depend_func: List[Callable], module_configs: List[ModuleConfig]) -> None:
         if cls._inited or not module_configs:
             return
 
-        cls.depend_func = [Depends(item) for item in depend_func if not callable(item)]
+        cls.depend_func = [Depends(item) for item in depend_func if callable(item)]
         cls.load_modules(module_configs)
         routers = cls.load_routers()
         cls.add_router(app, routers)
 
     @classmethod
     def load_modules(cls, module_configs: List[ModuleConfig]) -> None:
         """load modules
```

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/schema.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/utils.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/interface/method_interface.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/interface/method_interface.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/interface/register_interface.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/interface/register_interface.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/sqlmodel/__init__.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/sqlmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/sqlmodel/sqlmodel_method.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/sqlmodel/sqlmodel_method.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/sqlmodel/sqlmodel_reigster.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/sqlmodel/sqlmodel_reigster.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/sqlmodel/utils.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/sqlmodel/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/tortoise/__init__.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/tortoise/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/tortoise/tortoise_method.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/tortoise/tortoise_method.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/src/fastapi_module_register/tortoise/tortoise_register.py` & `fastapi_module_register-0.0.5/src/fastapi_module_register/tortoise/tortoise_register.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/.gitignore` & `fastapi_module_register-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/LICENSE` & `fastapi_module_register-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/README.md` & `fastapi_module_register-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.4/pyproject.toml` & `fastapi_module_register-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_module_register"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="stan", email="gd19920125@hotmail.com"},
 ]
 description = "通过将fastapi的模型自动注册路由"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `fastapi_module_register-0.0.4/PKG-INFO` & `fastapi_module_register-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_module_register
-Version: 0.0.4
+Version: 0.0.5
 Summary: 通过将fastapi的模型自动注册路由
 Project-URL: Homepage, https://github.com/dcshoecousa
 Author-email: stan <gd19920125@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 dcshoecousa
```

