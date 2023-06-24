# Comparing `tmp/flask_jeroboam-0.1.0b2.tar.gz` & `tmp/flask_jeroboam-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_jeroboam-0.1.0b2.tar", max compression
+gzip compressed data, was "flask_jeroboam-0.1.0b3.tar", max compression
```

## Comparing `flask_jeroboam-0.1.0b2.tar` & `flask_jeroboam-0.1.0b3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1078 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/LICENSE
--rw-r--r--   0        0        0     8198 2023-03-09 16:16:16.686637 flask_jeroboam-0.1.0b2/README.md
--rw-r--r--   0        0        0      638 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/__init__.py
--rw-r--r--   0        0        0     1002 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/_config.py
--rw-r--r--   0        0        0     1506 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/_constants.py
--rw-r--r--   0        0        0    12586 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/_inboundhandler.py
--rw-r--r--   0        0        0       62 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/_logger.py
--rw-r--r--   0        0        0    12996 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/_outboundhandler.py
--rw-r--r--   0        0        0     6262 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/_utils.py
--rw-r--r--   0        0        0      789 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/blueprint.py
--rw-r--r--   0        0        0     1011 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/blueprint.pyi
--rw-r--r--   0        0        0      966 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/datastructures.py
--rw-r--r--   0        0        0     3685 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/exceptions.py
--rw-r--r--   0        0        0     2278 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/jeroboam.py
--rw-r--r--   0        0        0      679 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/jeroboam.pyi
--rw-r--r--   0        0        0     1872 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/models.py
--rw-r--r--   0        0        0        0 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/__init__.py
--rw-r--r--   0        0        0     9294 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/_utils.py
--rw-r--r--   0        0        0     1336 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/blueprint.py
--rw-r--r--   0        0        0     3678 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/builder.py
--rw-r--r--   0        0        0    12893 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/models/openapi.py
--rw-r--r--   0        0        0      633 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/models/ui_context.py
--rw-r--r--   0        0        0     1054 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/templates/swagger-ui.jinja
--rw-r--r--   0        0        0        0 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/py.typed
--rw-r--r--   0        0        0      459 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/responses.py
--rw-r--r--   0        0        0     2143 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/rule.py
--rw-r--r--   0        0        0     2224 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/scaffold.py
--rw-r--r--   0        0        0     1064 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/scaffold.pyi
--rw-r--r--   0        0        0     1870 2023-03-09 16:15:56.766634 flask_jeroboam-0.1.0b2/flask_jeroboam/typing.py
--rw-r--r--   0        0        0     4632 2023-03-09 16:15:56.770634 flask_jeroboam-0.1.0b2/flask_jeroboam/view.py
--rw-r--r--   0        0        0        0 2023-03-09 16:15:56.770634 flask_jeroboam-0.1.0b2/flask_jeroboam/view_arguments/__init__.py
--rw-r--r--   0        0        0     2283 2023-03-09 16:15:56.770634 flask_jeroboam-0.1.0b2/flask_jeroboam/view_arguments/_utils.py
--rw-r--r--   0        0        0     4595 2023-03-09 16:15:56.770634 flask_jeroboam-0.1.0b2/flask_jeroboam/view_arguments/arguments.py
--rw-r--r--   0        0        0     2276 2023-03-09 16:15:56.770634 flask_jeroboam-0.1.0b2/flask_jeroboam/view_arguments/functions.py
--rw-r--r--   0        0        0     4728 2023-03-09 16:15:56.770634 flask_jeroboam-0.1.0b2/flask_jeroboam/view_arguments/functions.pyi
--rw-r--r--   0        0        0     7437 2023-03-09 16:15:56.770634 flask_jeroboam-0.1.0b2/flask_jeroboam/view_arguments/solved.py
--rw-r--r--   0        0        0       98 2023-03-09 16:15:56.770634 flask_jeroboam-0.1.0b2/flask_jeroboam/wrapper.py
--rw-r--r--   0        0        0      153 2023-03-09 16:15:56.770634 flask_jeroboam-0.1.0b2/flask_jeroboam/wrapper.pyi
--rw-r--r--   0        0        0     3564 2023-03-09 16:16:16.686637 flask_jeroboam-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0    10037 1970-01-01 00:00:00.000000 flask_jeroboam-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-24 13:36:16.677633 flask_jeroboam-0.1.0b3/LICENSE
+-rw-r--r--   0        0        0     8198 2023-06-24 13:36:16.677633 flask_jeroboam-0.1.0b3/README.md
+-rw-r--r--   0        0        0      638 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/__init__.py
+-rw-r--r--   0        0        0     1002 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/_config.py
+-rw-r--r--   0        0        0     1506 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/_constants.py
+-rw-r--r--   0        0        0    12586 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/_inboundhandler.py
+-rw-r--r--   0        0        0       62 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/_logger.py
+-rw-r--r--   0        0        0    13030 2023-06-24 13:36:36.453725 flask_jeroboam-0.1.0b3/flask_jeroboam/_outboundhandler.py
+-rw-r--r--   0        0        0     6262 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/_utils.py
+-rw-r--r--   0        0        0      789 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/blueprint.py
+-rw-r--r--   0        0        0     1011 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/blueprint.pyi
+-rw-r--r--   0        0        0      966 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/datastructures.py
+-rw-r--r--   0        0        0     3685 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/exceptions.py
+-rw-r--r--   0        0        0     2278 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/jeroboam.py
+-rw-r--r--   0        0        0      679 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/jeroboam.pyi
+-rw-r--r--   0        0        0     1872 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/models.py
+-rw-r--r--   0        0        0        0 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/__init__.py
+-rw-r--r--   0        0        0     9294 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/_utils.py
+-rw-r--r--   0        0        0     1336 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/blueprint.py
+-rw-r--r--   0        0        0     3768 2023-06-24 13:36:36.453725 flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/builder.py
+-rw-r--r--   0        0        0    12893 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/models/openapi.py
+-rw-r--r--   0        0        0      633 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/models/ui_context.py
+-rw-r--r--   0        0        0     1054 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/templates/swagger-ui.jinja
+-rw-r--r--   0        0        0        0 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/py.typed
+-rw-r--r--   0        0        0      459 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/responses.py
+-rw-r--r--   0        0        0     2143 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/rule.py
+-rw-r--r--   0        0        0     2224 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/scaffold.py
+-rw-r--r--   0        0        0     1064 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/scaffold.pyi
+-rw-r--r--   0        0        0     1870 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/typing.py
+-rw-r--r--   0        0        0     4632 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/view.py
+-rw-r--r--   0        0        0        0 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/view_arguments/__init__.py
+-rw-r--r--   0        0        0     2283 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/view_arguments/_utils.py
+-rw-r--r--   0        0        0     4595 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/view_arguments/arguments.py
+-rw-r--r--   0        0        0     2276 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/view_arguments/functions.py
+-rw-r--r--   0        0        0     4728 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/view_arguments/functions.pyi
+-rw-r--r--   0        0        0     7437 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/view_arguments/solved.py
+-rw-r--r--   0        0        0       98 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/wrapper.py
+-rw-r--r--   0        0        0      153 2023-06-24 13:36:16.681633 flask_jeroboam-0.1.0b3/flask_jeroboam/wrapper.pyi
+-rw-r--r--   0        0        0     3560 2023-06-24 13:36:36.457725 flask_jeroboam-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     9837 1970-01-01 00:00:00.000000 flask_jeroboam-0.1.0b3/PKG-INFO
```

### Comparing `flask_jeroboam-0.1.0b2/LICENSE` & `flask_jeroboam-0.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/README.md` & `flask_jeroboam-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/__init__.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/_config.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/_config.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/_constants.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/_constants.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/_inboundhandler.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/_inboundhandler.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/_outboundhandler.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/_outboundhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
             return content
         elif isinstance(content, BaseModel):
             return content.dict()
         elif isinstance(content, list):
             return {
                 "__root__": [self._adapt_datastructure_of(item) for item in content]
             }
-        elif dataclasses.is_dataclass(content):
+        elif dataclasses.is_dataclass(content) and not isinstance(content, type):
             return dataclasses.asdict(content)
 
         raise ValueError("Content must be a list, a dict, a dataclass, or a BaseModel.")
 
     def _build_response(
         self,
         content: Optional[str] = None,
```

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/_utils.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/_utils.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/blueprint.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/blueprint.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/blueprint.pyi` & `flask_jeroboam-0.1.0b3/flask_jeroboam/blueprint.pyi`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/datastructures.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/datastructures.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/exceptions.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/jeroboam.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/jeroboam.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/jeroboam.pyi` & `flask_jeroboam-0.1.0b3/flask_jeroboam/jeroboam.pyi`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/models.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/models.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/_utils.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/_utils.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/blueprint.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/blueprint.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/builder.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Main builder function for OPENAPI schema."""
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
+from typing import Union
 
 from pydantic.schema import get_model_name_map
 
 from flask_jeroboam._utils import _memoized_update_if_value
 from flask_jeroboam.openapi._utils import _build_openapi_path_item
 from flask_jeroboam.openapi._utils import _get_flat_models_from_jeroboam_views
 from flask_jeroboam.openapi._utils import _get_model_definitions
 from flask_jeroboam.openapi.models.openapi import Components
 from flask_jeroboam.openapi.models.openapi import Info
 from flask_jeroboam.openapi.models.openapi import OpenAPI
+from flask_jeroboam.openapi.models.openapi import PathItem
 from flask_jeroboam.openapi.models.openapi import Tag
 
 
 if TYPE_CHECKING:  # pragma: no cover
     from flask_jeroboam.jeroboam import Jeroboam
     from flask_jeroboam.rule import JeroboamRule
     from flask_jeroboam.view import JeroboamView
@@ -46,15 +48,15 @@
             "contact": app.config.get("JEROBOAM_CONTACT", None),
             "license": app.config.get("JEROBOAM_LICENCE_INFO", None),
         }
     )
     servers = app.config.get("JEROBOAM_SERVERS", None)
 
     # Préparation
-    paths: Dict[str, Dict[str, Any]] = {}
+    paths: Dict[str, Union[Any, PathItem]] = {}
     components: Dict[str, Dict[str, Any]] = {}
     operation_ids: Set[str] = set()
 
     # Les jerobomas views, probablement à déléguer à l'app
     jeroboam_views: List[Optional["JeroboamView"]] = [
         getattr(app.view_functions[rule.endpoint], "__jeroboam_view__", None)
         for rule in rules
```

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/models/openapi.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/models/openapi.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/models/ui_context.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/models/ui_context.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/openapi/templates/swagger-ui.jinja` & `flask_jeroboam-0.1.0b3/flask_jeroboam/openapi/templates/swagger-ui.jinja`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/rule.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/rule.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/scaffold.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/scaffold.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/scaffold.pyi` & `flask_jeroboam-0.1.0b3/flask_jeroboam/scaffold.pyi`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/typing.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/typing.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/view.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/view.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/view_arguments/_utils.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/view_arguments/_utils.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/view_arguments/arguments.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/view_arguments/arguments.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/view_arguments/functions.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/view_arguments/functions.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/view_arguments/functions.pyi` & `flask_jeroboam-0.1.0b3/flask_jeroboam/view_arguments/functions.pyi`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/flask_jeroboam/view_arguments/solved.py` & `flask_jeroboam-0.1.0b3/flask_jeroboam/view_arguments/solved.py`

 * *Files identical despite different names*

### Comparing `flask_jeroboam-0.1.0b2/pyproject.toml` & `flask_jeroboam-0.1.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "A Flask extension, inspired by FastAPI that uses Pydantic to provide easy-to-configure data validation for request parsing and response serialization."
 documentation = "https://flask-jeroboam.readthedocs.io"
 homepage = "https://github.com/jcbianic/flask-jeroboam"
 license = "MIT"
 name = "flask-jeroboam"
 readme = "README.md"
 repository = "https://github.com/jcbianic/flask-jeroboam"
-version = "0.1.0.beta2"
+version = "0.1.0b3"
 
 [tool.poetry.urls]
 Changelog = "https://github.com/jcbianic/flask-jeroboam/releases"
 
 [tool.poetry.dependencies]
 Flask = "^2.1.3"
 pydantic = "^1.10.2"
```

### Comparing `flask_jeroboam-0.1.0b2/PKG-INFO` & `flask_jeroboam-0.1.0b3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-jeroboam
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: A Flask extension, inspired by FastAPI that uses Pydantic to provide easy-to-configure data validation for request parsing and response serialization.
 Home-page: https://github.com/jcbianic/flask-jeroboam
 License: MIT
 Author: Jean-Christophe Bianic
 Author-email: jc.bianic@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -15,20 +15,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Typing :: Typed
 Requires-Dist: Flask (>=2.1.3,<3.0.0)
```

