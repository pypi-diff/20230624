# Comparing `tmp/fastapi_module_register-0.0.2.tar.gz` & `tmp/fastapi_module_register-0.0.3.tar.gz`

## Comparing `fastapi_module_register-0.0.2.tar` & `fastapi_module_register-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,25 @@
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/README.en.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/__init__.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/base_method.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/base_register.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/constants.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/exceptions.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/logger.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/schema.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/utils.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/tortoise/__init__.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/tortoise/tortoise_method.py
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/src/fastapi_module_register/tortoise/tortoise_register.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/LICENSE
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/README.en.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/__init__.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/base_register.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/constants.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/exceptions.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/logger.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/schema.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/utils.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/interface/method_interface.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/interface/register_interface.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/sqlmodel/__init__.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/sqlmodel/sqlmodel_method.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/sqlmodel/sqlmodel_reigster.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/sqlmodel/utils.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/tortoise/__init__.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/tortoise/tortoise_method.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/src/fastapi_module_register/tortoise/tortoise_register.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/tests/test_sqlmodel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/tests/test_tortoise.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/LICENSE
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/README.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 fastapi_module_register-0.0.3/PKG-INFO
```

### Comparing `fastapi_module_register-0.0.2/README.en.md` & `fastapi_module_register-0.0.3/README.en.md`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.2/src/fastapi_module_register/base_method.py` & `fastapi_module_register-0.0.3/src/fastapi_module_register/interface/method_interface.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from abc import abstractmethod, ABC
-from typing import Any, Callable, Optional, Tuple, Union
+from typing import Any, Callable, Optional, Tuple
 
-from tortoise.models import Model
 
-
-class BaseMethod(ABC):
+class MethodInterface(ABC):
 
     @abstractmethod
-    def get(cls, module: Union[Model, Any], *args, **kwars) -> Optional[Tuple[Callable, Any]]:
+    def get(self, *args, **kwars) -> Optional[Tuple[Callable, Any]]:
         raise NotImplementedError
 
     @abstractmethod
-    def post(cls, module: Union[Model, Any], *args, **kwars) -> Optional[Tuple[Callable, Any]]:
+    def post(self, *args, **kwars) -> Optional[Tuple[Callable, Any]]:
         raise NotImplementedError
 
     @abstractmethod
-    def put(cls, module: Union[Model, Any], *args, **kwars) -> Optional[Tuple[Callable, Any]]:
+    def put(self, *args, **kwars) -> Optional[Tuple[Callable, Any]]:
         raise NotImplementedError
 
     @abstractmethod
-    def delete(cls, module: Union[Model, Any], *args, **kwars) -> Optional[Tuple[Callable, Any]]:
+    def delete(self, *args, **kwars) -> Optional[Tuple[Callable, Any]]:
         raise NotImplementedError
```

### Comparing `fastapi_module_register-0.0.2/src/fastapi_module_register/base_register.py` & `fastapi_module_register-0.0.3/src/fastapi_module_register/interface/register_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from typing import Union, Dict, List, Any
 
 from fastapi import FastAPI
 
 from fastapi_module_register.schema import ModuleConfig
 
 
-class BaseRegister(ABC):
+class RegisterInterface(ABC):
 
-    modules: Dict[str, Union[ModuleConfig, Any]] = {}
+    modules: Dict[str, ModuleConfig] = {}
     _inited: bool = False
 
     @classmethod
     @abstractmethod
     def init(cls, app: FastAPI, module_configs: List[ModuleConfig], *args, **kwargs) -> None:
         raise NotImplementedError
```

### Comparing `fastapi_module_register-0.0.2/src/fastapi_module_register/schema.py` & `fastapi_module_register-0.0.3/src/fastapi_module_register/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
-from typing import Any, Dict, List, Generic, Optional, TypeVar
+from typing import Any, Dict, List,Type, Callable, Generic, Optional, TypeVar, Union
 
 import ujson as json
 from pydantic import BaseModel, Extra, Field
 from pydantic.generics import GenericModel
+from tortoise.models import Model
 
 
 _T = TypeVar("_T")
 
 
 class RouterConfig(BaseModel):
     api_path: str = Field(None, description="The api router path")
@@ -25,22 +26,22 @@
             }
         }
 
 
 class ModuleConfig(BaseModel):
     name: str = Field(None, description="The module name")
     module_path: str = Field(..., description="The module path")
-    module: Any = None
+    module: Union[Type["Model"], Any] = Field(None, description="The module")
     router_config: List[RouterConfig] = []
 
     class Config:
         schema_extra = {
             "example": {
                 "name": "example",
-                "module_path": ["models.example"],
+                "module_path": "models.example",
                 "router_config": [
                     {
                         "api_path": "/api/example",
                         "method": "get",
                         "parameters": {
                             "tags": ["example"]
                         }
@@ -92,14 +93,21 @@
         router_config = self.get_router_config(
             "get",
             f"/{module_name}/" + "{pk}",
             module_name
         )
         self.router_config.append(router_config)
 
+
+class Router(BaseModel):
+    path: str = Field("...", description="The router path")
+    endpoint: Callable = Field(..., description="")
+    
+
+
 class BaseApiSchema(BaseModel):
     class Config:
         extra = Extra.allow
         json_loads = json.loads
         json_dumps = json.dumps
         json_encoders = {
             datetime: lambda v: v.strftime("%Y-%m-%d %H:%M:%S"),
```

### Comparing `fastapi_module_register-0.0.2/src/fastapi_module_register/utils.py` & `fastapi_module_register-0.0.3/src/fastapi_module_register/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.2/src/fastapi_module_register/tortoise/__init__.py` & `fastapi_module_register-0.0.3/src/fastapi_module_register/tortoise/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-from typing import Any, Dict, List, Union
+from typing import Any, Callable, Dict, List, Union
 
 from fastapi import FastAPI
 
 from fastapi_module_register.logger import logger
 from fastapi_module_register.schema import ModuleConfig
 from fastapi_module_register.tortoise.tortoise_register import TortoiseRegister
 from fastapi_module_register.utils import get_module_configs
 
 
-def router_register(
+def tortoise_register(
     app: FastAPI,
+    depend_func: List[Callable],
     module_configs: Union[List[str], List[ModuleConfig], List[Dict[str, Any]]]
 ) -> None:
     """_summary_
 
     Args:
         app (FastAPI): _description_
+        depend_func (Callbale) _description_
         module_configs (Union[List[str], List[ModuleConfig], List[Dict[str, Any]]]): _description_. Defaults to None.
     """
     if not module_configs:
-        logger.info("No module register.")
+        logger.info("No module register")
         return
 
     if not isinstance(app, FastAPI):
-        raise RuntimeError("Please given fastapi object.")
+        raise RuntimeError("Please given fastapi object")
 
     module_configs = get_module_configs(module_configs)
     @app.on_event("startup")
     async def init_router() -> None:  # pylint: disable=W0612
-        modules = TortoiseRegister.init(app, module_configs)
+        modules = TortoiseRegister.init(app, depend_func, module_configs)
         logger.info("Register tortoise router started, %s", modules)
```

### Comparing `fastapi_module_register-0.0.2/src/fastapi_module_register/tortoise/tortoise_method.py` & `fastapi_module_register-0.0.3/src/fastapi_module_register/tortoise/tortoise_method.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,124 +1,106 @@
-from typing import Any, List, Optional, Callable, Type, Tuple
+from typing import Optional, Callable, Type, Tuple, Union
 
 from fastapi import Depends, HTTPException
+from fastapi_pagination import Page, Params
+from fastapi_pagination.ext.tortoise import paginate
 from tortoise.models import Model
-from tortoise.contrib.pydantic import pydantic_model_creator
 from tortoise.contrib.pydantic.base import PydanticModel
+from tortoise.contrib.pydantic.creator import pydantic_model_creator
 
-from fastapi_module_register.base_method import BaseMethod
+from fastapi_module_register.interface.method_interface import MethodInterface
 from fastapi_module_register.schema import BaseApiOut
 
 
-class TortoiseMethod(BaseMethod):
+class TortoiseMethod(MethodInterface):
 
-    def __init__(self, module: Model, depend_func: Optional[Callable] = None)-> None:
+    def __init__(self, module: Type[Model])-> None:
         """_summary_
 
         Args:
             module (Model): The tortoise model
-            depend_func (Optional[Callable], optional): _description_. Defaults to None.
         """
         self._module = module
-        self._depend_func = depend_func
         self._base_request = pydantic_model_creator(
-            module, 
-            name=f"{module.__name__}_req",
-            exclude=[module._meta.pk_attr]
+            module,
+            name=f"{module.__name__}_request",
+            exclude=(module._meta.pk_attr, ),
+            exclude_readonly=True
         )
         self._get_response = pydantic_model_creator(module, name=f"{module.__name__}_get")
-        self._base_response = pydantic_model_creator(module, name=f"{module.__name__}_res")
+        self._base_response = pydantic_model_creator(module, name=f"{module.__name__}_response")
 
-    def get(self, filter_by_pk: bool = False, *args, **kwargs) -> Tuple[Callable, Any]:
+    def get(self, filter_by_pk: bool = False, *args, **kwargs) -> Tuple[Callable, Union[Type[PydanticModel], Type[Page[PydanticModel]]]]:
         """The http get method
         Args:
             filter_by_pk (bool): Get item by pk
         Returns:
             Callable: _description_
         """
         if filter_by_pk:
-            async def wapper(pk: int):
+            async def wapper(pk: int): # type: ignore
                 result = self._module.get(pk=pk)
                 result = await self._get_response.from_queryset_single(result)
                 return result
             return wapper, self._base_response
-        async def wapper():
-            results = self._module.all()
-            results = await self._get_response.from_queryset(results)
+        async def wapper(params: Params = Depends()):
+            results = self._module.filter()
+            results = await paginate(results, params)
             return results
-        return wapper, List[self._get_response]
+        return wapper, Page[self._get_response]
 
     def post(
         self,
-        depend_func: Optional[Callable] = None,
-        request_model: Optional[Type[PydanticModel]] = None
-    ) -> Tuple[Callable, Any]:
+        request_model: Optional[Type[PydanticModel]] = None,
+    ) -> Tuple[Callable, Type[PydanticModel]]:
         """The http post method
 
         Args:
-            depend_func (Optional[Callable], optional): _description_. Defaults to None.
             request_model (Optional[Type[PydanticModel]], optional): _description_. Defaults to None.
 
         Returns:
             Callable: _description_
         """
         if not request_model:
             request_model = self._base_request
 
-        depend_func = depend_func if depend_func else self._depend_func
-        if depend_func:
-            async def wapper(req: request_model, _ = Depends(depend_func)):
-                save_item = await self._module.create(**req.dict(exclude_unset=True))
-                return await self._base_response.from_tortoise_orm(save_item)
-            return wapper, self._base_response
-        
-        async def wapper(req: request_model):
+        async def wapper(req: request_model): # type: ignore
             save_item = await self._module.create(**req.dict(exclude_unset=True))
             return await self._base_response.from_tortoise_orm(save_item)
         return wapper, self._base_response
 
     def put(
         self,
-        depend_func: Optional[Callable] = None,
         request_model: Optional[Type[PydanticModel]] = None
-    ) -> Tuple[Callable, Any]:
+    ) -> Tuple[Callable, Type[PydanticModel]]:
         """_summary_
 
         Args:
-            depend_func (Optional[Callable], optional): _description_. Defaults to None.
             request_model (Optional[Type[PydanticModel]], optional): _description_. Defaults to None.
 
         Returns:
             _type_: _description_
         """
         if not request_model:
             request_model = self._base_request
-        
-        depend_func = depend_func if depend_func else self._depend_func
-        if depend_func:
-            async def wapper(pk: int, req: request_model, _ = Depends(depend_func)):
-                await self._module.filter(pk=pk).update(**req.dict(exclude_unset=True))
-                return await self._base_response.from_queryset_single(
-                    self._module.get(pk=pk)
-                )
-            return wapper, self._base_response
 
-        async def wapper(pk: int, req: request_model):
+        async def wapper(pk: int, req: request_model): # type: ignore
             await self._module.filter(pk=pk).update(**req.dict(exclude_unset=True))
             return await self._base_response.from_queryset_single(
                 self._module.get(pk=pk)
             )
         return wapper, self._base_response
 
-    def delete(self) -> Tuple[Callable, BaseApiOut]:
+    def delete(self) -> Tuple[Callable, Type[BaseApiOut]]:
         """Delete the item by primary key
 
         Returns:
             Callable: _description_
         """
         async def wapper(pk: int):
             item = await self._module.get(pk=pk)
             if not item:
                 raise HTTPException(status_code=404, detail=f"{self._module.__name__} {pk} not found")
             await item.delete()
             return BaseApiOut()
+
         return wapper, BaseApiOut
```

### Comparing `fastapi_module_register-0.0.2/src/fastapi_module_register/tortoise/tortoise_register.py` & `fastapi_module_register-0.0.3/src/fastapi_module_register/base_register.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-from typing import Any, Dict, List, Optional, Type
+from typing import Any, Dict, List, Callable, Optional, Type
 import warnings
 
-from fastapi import FastAPI
-from tortoise.models import Model
-from tortoise.contrib.fastapi import HTTPNotFoundError
+from fastapi import FastAPI, Depends
 
-from fastapi_module_register.base_register import BaseRegister
 from fastapi_module_register.exceptions import ConfigurationError
+from fastapi_module_register.interface.register_interface import RegisterInterface
 from fastapi_module_register.schema import ModuleConfig
-from fastapi_module_register.tortoise.tortoise_method import TortoiseMethod
-from fastapi_module_register.utils import import_string 
+from fastapi_module_register.utils import import_string
 
 
-class TortoiseRegister(BaseRegister):
+class BaseRegister(RegisterInterface):
 
     @classmethod
-    def init(cls, app: FastAPI, module_configs: List[ModuleConfig]) -> None:
+    def init(cls, app: FastAPI, depend_func: Callable, module_configs: List[ModuleConfig]) -> None:
         if cls._inited or not module_configs:
             return
-        
+
+        cls.depend_func = depend_func
         cls.load_modules(module_configs)
         routers = cls.load_routers()
         cls.add_router(app, routers)
 
     @classmethod
     def load_modules(cls, module_configs: List[ModuleConfig]) -> None:
         """load modules
@@ -38,72 +36,72 @@
                 continue
             module_config.module = module
             if not module_config.name:
                 module_config.name = module.__name__
         cls.modules = {model.name: model for model in module_configs}
 
     @classmethod
-    def _discover_model(
-        cls,
-        models_path: str
-    ) -> Optional[Type["Model"]]:
+    def _discover_model(cls, module_path: str, *args, **kwargs) -> Optional[Type["Any"]]:
         """_summary_
 
         Raises:
             ConfigurationError: _description_
 
         Returns:
             _type_: _description_
         """
-        
         try:
-            module = import_string(models_path)
+            module = import_string(module_path)
         except ImportError:
-            raise ConfigurationError(f'Module "{models_path}" not found')
+            raise ConfigurationError(f'Module "{module_path}" not found')
 
-        if issubclass(module, Model) and not module._meta.abstract:
-            if not module._meta.app:
-                return None
+        if cls._check_module(module):
             return module
 
     @classmethod
+    def _discover_method(cls, module: Any, *args, **kwargs) -> Callable:
+        raise NotImplementedError
+    
+    @classmethod
+    def _check_module(cls, module: Any, *args, **kwargs) -> bool:
+        raise NotImplementedError
+
+    @classmethod
     def load_routers(cls) -> List[Any]:
         """load routers
 
         Returns:
             _type_: _description_
         """
         
         routers = []
         for _, module_config in cls.modules.items():
-            if not issubclass(module_config.module, Model):
-                warnings.warn(f"The module is not a type model")
+            if not cls._check_module(module_config.module):
                 continue
-
-            tortoise_method = TortoiseMethod(module_config.module)
             for config in module_config.router_config:
-                exec_fun = getattr(tortoise_method, config.method, None)
+                method_func = cls._discover_method(module_config.module)
+                exec_fun = getattr(method_func, config.method, None)
                 if not exec_fun:
                     warnings.warn(f"Unsupported http method: {config.method}")
                     continue
 
                 if config.method.lower() == "get":
                     filter_by_pk = True if '{pk}' in config.api_path else False
-                    exec_fun_obj, req_schema = exec_fun(filter_by_pk)
+                    exec_fun_obj, res_schema = exec_fun(filter_by_pk)
                 else:
-                    exec_fun_obj, req_schema = exec_fun()
+                    exec_fun_obj, res_schema = exec_fun()
+
                 if not callable(exec_fun_obj):
                     continue
 
                 router = {
                     "path": config.api_path,
                     "endpoint": exec_fun_obj,
                     "methods": [config.method],
-                    "response_model": req_schema,
-                    "responses": {404: {"model": HTTPNotFoundError}}
+                    "response_model": res_schema
                 }
                 router.update(config.parameters)
                 routers.append(router)
         return routers
 
     @classmethod
     def add_router(cls, app: FastAPI, routers: List[Dict]) -> None:
@@ -113,8 +111,8 @@
             app (FastAPI): _description_
             routers (List[Dict]): _description_
         """
         if not routers:
             return
         
         for router in routers:
-            app.add_api_route(**router)
+            app.add_api_route(**router, dependencies=[Depends(cls.depend_func)])
```

### Comparing `fastapi_module_register-0.0.2/.gitignore` & `fastapi_module_register-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.2/LICENSE` & `fastapi_module_register-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.2/README.md` & `fastapi_module_register-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_module_register-0.0.2/pyproject.toml` & `fastapi_module_register-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_module_register"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="stan", email="gd19920125@hotmail.com"},
 ]
 description = "通过将fastapi的模型自动注册路由"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
@@ -16,12 +16,14 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "fastapi>=0.95.1",
     "tortoise-orm>=0.19.3",
-    "ujson>=5.7.0"
+    "ujson>=5.7.0",
+    "fastapi-pagination==0.12.4",
+    "sqlmodel==0.0.8"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dcshoecousa"
```

### Comparing `fastapi_module_register-0.0.2/PKG-INFO` & `fastapi_module_register-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_module_register
-Version: 0.0.2
+Version: 0.0.3
 Summary: 通过将fastapi的模型自动注册路由
 Project-URL: Homepage, https://github.com/dcshoecousa
 Author-email: stan <gd19920125@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 dcshoecousa
         
@@ -26,15 +26,17 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: fastapi-pagination==0.12.4
 Requires-Dist: fastapi>=0.95.1
+Requires-Dist: sqlmodel==0.0.8
 Requires-Dist: tortoise-orm>=0.19.3
 Requires-Dist: ujson>=5.7.0
 Description-Content-Type: text/markdown
 
 # fastapi_module_register
 
 #### 介绍
```

