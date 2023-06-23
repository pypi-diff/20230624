# Comparing `tmp/housekeeping-1.0.tar.gz` & `tmp/housekeeping-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "housekeeping-1.0.tar", last modified: Fri May 12 23:42:31 2023, max compression
+gzip compressed data, was "housekeeping-1.1.tar", last modified: Fri Jun 23 23:20:42 2023, max compression
```

## Comparing `housekeeping-1.0.tar` & `housekeeping-1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-12 23:42:31.476071 housekeeping-1.0/
--rw-r--r--   0 chipx86    (501) staff       (20)     1057 2023-05-12 23:42:27.000000 housekeeping-1.0/LICENSE
--rw-r--r--   0 chipx86    (501) staff       (20)     8064 2023-05-12 23:42:31.475958 housekeeping-1.0/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)     6785 2023-05-12 23:42:27.000000 housekeeping-1.0/README.md
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-12 23:42:31.474761 housekeeping-1.0/housekeeping/
--rw-r--r--   0 chipx86    (501) staff       (20)     2231 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1550 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/_version.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3099 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/base.py
--rw-r--r--   0 chipx86    (501) staff       (20)    14494 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/classes.py
--rw-r--r--   0 chipx86    (501) staff       (20)    18612 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/functions.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6652 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/helpers.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3857 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/modules.py
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/py.typed
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-12 23:42:31.475814 housekeeping-1.0/housekeeping/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    13254 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/tests/test_classes.py
--rw-r--r--   0 chipx86    (501) staff       (20)    13738 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/tests/test_functions.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3961 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/tests/test_modules.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2289 2023-05-12 23:42:27.000000 housekeeping-1.0/housekeeping/tests/testcases.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-12 23:42:31.475281 housekeeping-1.0/housekeeping.egg-info/
--rw-r--r--   0 chipx86    (501) staff       (20)     8064 2023-05-12 23:42:31.000000 housekeeping-1.0/housekeeping.egg-info/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)      572 2023-05-12 23:42:31.000000 housekeeping-1.0/housekeeping.egg-info/SOURCES.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        1 2023-05-12 23:42:31.000000 housekeeping-1.0/housekeeping.egg-info/dependency_links.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       23 2023-05-12 23:42:31.000000 housekeeping-1.0/housekeeping.egg-info/requires.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       13 2023-05-12 23:42:31.000000 housekeeping-1.0/housekeeping.egg-info/top_level.txt
--rw-r--r--   0 chipx86    (501) staff       (20)     1529 2023-05-12 23:42:27.000000 housekeeping-1.0/pyproject.toml
--rw-r--r--   0 chipx86    (501) staff       (20)       38 2023-05-12 23:42:31.476106 housekeeping-1.0/setup.cfg
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-06-23 23:20:42.820284 housekeeping-1.1/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1057 2023-06-23 23:20:39.000000 housekeeping-1.1/LICENSE
+-rw-r--r--   0 chipx86    (501) staff       (20)     8064 2023-06-23 23:20:42.820160 housekeeping-1.1/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)     6785 2023-06-23 23:20:39.000000 housekeeping-1.1/README.md
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-06-23 23:20:42.818960 housekeeping-1.1/housekeeping/
+-rw-r--r--   0 chipx86    (501) staff       (20)     2231 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1550 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/_version.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3345 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/base.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    15276 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/classes.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    19637 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/functions.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6982 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/helpers.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4418 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/modules.py
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/py.typed
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-06-23 23:20:42.820019 housekeeping-1.1/housekeeping/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    14747 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/tests/test_classes.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    16382 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/tests/test_functions.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5024 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/tests/test_modules.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2289 2023-06-23 23:20:39.000000 housekeeping-1.1/housekeeping/tests/testcases.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-06-23 23:20:42.819472 housekeeping-1.1/housekeeping.egg-info/
+-rw-r--r--   0 chipx86    (501) staff       (20)     8064 2023-06-23 23:20:42.000000 housekeeping-1.1/housekeeping.egg-info/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)      572 2023-06-23 23:20:42.000000 housekeeping-1.1/housekeeping.egg-info/SOURCES.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)        1 2023-06-23 23:20:42.000000 housekeeping-1.1/housekeeping.egg-info/dependency_links.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       23 2023-06-23 23:20:42.000000 housekeeping-1.1/housekeeping.egg-info/requires.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       13 2023-06-23 23:20:42.000000 housekeeping-1.1/housekeeping.egg-info/top_level.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)     1529 2023-06-23 23:20:39.000000 housekeeping-1.1/pyproject.toml
+-rw-r--r--   0 chipx86    (501) staff       (20)       38 2023-06-23 23:20:42.820317 housekeeping-1.1/setup.cfg
```

### Comparing `housekeeping-1.0/LICENSE` & `housekeeping-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `housekeeping-1.0/PKG-INFO` & `housekeeping-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeping
-Version: 1.0
+Version: 1.1
 Summary: Python utilities for helping deprecate and remove code.
 Author-email: "Beanbag, Inc." <questions@beanbaginc.com>
 License: MIT
 Project-URL: homepage, https://github.com/beanbaginc/housekeeping
 Project-URL: documentation, https://github.com/beanbaginc/housekeeping
 Project-URL: repository, https://github.com/beanbaginc/housekeeping
 Keywords: deprecation,cleanup,code quality
```

### Comparing `housekeeping-1.0/README.md` & `housekeeping-1.1/README.md`

 * *Files identical despite different names*

### Comparing `housekeeping-1.0/housekeeping/__init__.py` & `housekeeping-1.1/housekeeping/__init__.py`

 * *Files identical despite different names*

### Comparing `housekeeping-1.0/housekeeping/_version.py` & `housekeeping-1.1/housekeeping/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # The version of housekeeping.
 #
 # This is in the format of:
 #
 #   (Major, Minor, Micro, alpha/beta/rc/final, Release Number, Released)
 #
-VERSION = (1, 0, 0, 'final', 0, True)
+VERSION = (1, 1, 0, 'final', 0, True)
 
 
 def get_version_string() -> str:
     """Return the display version of Housekeeping.
 
     Returns:
         str:
```

### Comparing `housekeeping-1.0/housekeeping/base.py` & `housekeeping-1.1/housekeeping/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base support for housekeeping warnings and types."""
 
 from __future__ import annotations
 
 import warnings
-from typing import Type, TYPE_CHECKING
+from typing import Callable, Type, TYPE_CHECKING, Union
 
 from typing_extensions import TypeAlias
 
 if TYPE_CHECKING:
     _BaseDeprecationWarningMixinClass = DeprecationWarning
     _BasePendingDeprecationWarningMixinClass = PendingDeprecationWarning
 else:
@@ -93,7 +93,17 @@
     It's recommended that projects subclass this to create their own
     base class.
     """
 
 
 #: An alias for representing a BaseDeprecationWarningMixin subclass.
 DeprecationWarningType: TypeAlias = Type[BaseDeprecationWarningMixin]
+
+
+#: An alias for a DeprecationWarningType or a callable returning one.
+#:
+#: Version Added:
+#:     1.1
+DeprecationWarningTypeOrCallable: TypeAlias = Union[
+    DeprecationWarningType,
+    Callable[[], DeprecationWarningType],
+]
```

### Comparing `housekeeping-1.0/housekeeping/classes.py` & `housekeeping-1.1/housekeeping/classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utilities to deprecate classes."""
 
 from __future__ import annotations
 
 from typing import Optional, Type
 
-from housekeeping.base import DeprecationWarningType
+from housekeeping.base import DeprecationWarningTypeOrCallable
 from housekeeping.helpers import emit_warning, format_display_name
 
 
 class ClassDeprecatedMixin:
     """Mixin for classes that are deprecated.
 
     This will emit a deprecation warning when the class is first subclassed.
@@ -84,22 +84,23 @@
                             init_deprecation_msg='...'):
                ...
     """
 
     _housekeeping_base_cls: Optional[Type] = None
     _housekeeping_subclass_deprecation_msg: Optional[str] = None
     _housekeeping_init_deprecation_msg: Optional[str] = None
-    _housekeeping_warning_cls: Optional[DeprecationWarningType] = None
+    _housekeeping_warning_cls: Optional[DeprecationWarningTypeOrCallable] = \
+        None
 
     def __init_subclass__(
         cls,
         *,
         init_deprecation_msg: Optional[str] = None,
         subclass_deprecation_msg: Optional[str] = None,
-        warning_cls: Optional[DeprecationWarningType] = None,
+        warning_cls: Optional[DeprecationWarningTypeOrCallable] = None,
         **kwargs,
     ) -> None:
         """Initialize a subclass.
 
         If this is a direct subclass of a deprecated class, a deprecation
         warning will be emitted.
 
@@ -108,20 +109,27 @@
                 A custom deprecation message to use when initializing the
                 class directly.
 
             subclass_deprecation_msg (str, optional):
                 A custom deprecation message to use when subclassing the
                 class directly.
 
-            warning_cls (type, optional):
-                The type of warning class to use.
+            warning_cls (type or callable, optional):
+                The type of warning class to use, or a callable returning one.
 
                 This must be provided for the class using this mixin. It
                 will be ignored for subclasses.
 
+                A callable can be used to avoid circular references.
+
+                Version Changed:
+                    1.1:
+                    This can now be either a warning class or a function
+                    that returns one.
+
             **kwargs (dict):
                 Additional keyword arguments to pass to the parent.
         """
         if ClassDeprecatedMixin in cls.__bases__:
             # This class is deprecated, so store information for immediate
             # subclasses to reference.
             if warning_cls is None:
@@ -142,15 +150,16 @@
             warning_cls = cls._housekeeping_warning_cls
 
             assert deprecated_base_cls is not None
             assert warning_cls is not None
 
             message = cls._housekeeping_subclass_deprecation_msg
 
-            if cls._housekeeping_base_cls in cls.__bases__:
+            if (cls._housekeeping_base_cls in cls.__bases__ and
+                not getattr(cls, 'housekeeping_skip_warning', False)):
                 emit_warning(
                     warning_cls,
                     deprecation_msg=message or (
                         '`%(subclass_name)s` subclasses `%(class_name)s`, '
                         'which is deprecated and will be removed in '
                         '%(product)s %(version)s.'
                     ),
@@ -271,23 +280,24 @@
                ...
     """
 
     _housekeeping_base_cls: Optional[Type] = None
     _housekeeping_init_deprecation_msg: Optional[str] = None
     _housekeeping_new_base_cls: Optional[Type] = None
     _housekeeping_subclass_deprecation_msg: Optional[str] = None
-    _housekeeping_warning_cls: Optional[DeprecationWarningType] = None
+    _housekeeping_warning_cls: Optional[DeprecationWarningTypeOrCallable] = \
+        None
 
     def __init_subclass__(
         cls,
         *,
         init_deprecation_msg: Optional[str] = None,
         subclass_deprecation_msg: Optional[str] = None,
         new_base_cls: Optional[Type] = None,
-        warning_cls: Optional[DeprecationWarningType] = None,
+        warning_cls: Optional[DeprecationWarningTypeOrCallable] = None,
         **kwargs,
     ) -> None:
         """Initialize a subclass.
 
         If this is a direct subclass of a deprecated class, a deprecation
         warning will be emitted.
 
@@ -296,20 +306,27 @@
                 A custom deprecation message to use when initializing the
                 class directly.
 
             subclass_deprecation_msg (str, optional):
                 A custom deprecation message to use when subclassing the
                 class directly.
 
-            warning_cls (type, optional):
-                The type of warning class to use.
+            warning_cls (type or callable, optional):
+                The type of warning class to use, or a callable returning one.
 
                 This must be provided for the class using this mixin. It
                 will be ignored for subclasses.
 
+                A callable can be used to avoid circular references.
+
+                Version Changed:
+                    1.1:
+                    This can now be either a warning class or a function
+                    that returns one.
+
             **kwargs (dict):
                 Additional keyword arguments to pass to the parent.
         """
         if ClassMovedMixin in cls.__bases__:
             # This class is deprecated, so store information for immediate
             # subclasses to reference.
             if warning_cls is None:
@@ -333,15 +350,16 @@
 
             assert deprecated_base_cls is not None
             assert new_base_cls is not None
             assert warning_cls is not None
 
             message = cls._housekeeping_subclass_deprecation_msg
 
-            if cls._housekeeping_base_cls in cls.__bases__:
+            if (cls._housekeeping_base_cls in cls.__bases__ and
+                not getattr(cls, 'housekeeping_skip_warning', False)):
                 emit_warning(
                     warning_cls,
                     deprecation_msg=message or (
                         '`%(subclass_name)s` subclasses `%(old_class_name)s`, '
                         'which is deprecated and will be removed in '
                         '%(product)s %(version)s. You will need to subclass '
                         '`%(new_class_name)s` instead.'
```

### Comparing `housekeeping-1.0/housekeeping/functions.py` & `housekeeping-1.1/housekeeping/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from __future__ import annotations
 
 import inspect
 from functools import wraps
 from typing import (Any, Callable, Dict, List, Optional, Tuple, TypeVar,
                     Union, cast)
 
-from housekeeping.base import DEFAULT_STACK_LEVEL, DeprecationWarningType
+from housekeeping.base import (DEFAULT_STACK_LEVEL,
+                               DeprecationWarningTypeOrCallable)
 from housekeeping.helpers import LazyObject, emit_warning, format_display_name
 
 
 _FuncT = TypeVar('_FuncT', bound=Callable[..., Any])
 _ValueT = TypeVar('_ValueT')
 
 
 def deprecated_arg_value(
-    warning_cls: DeprecationWarningType,
+    warning_cls: DeprecationWarningTypeOrCallable,
     *,
     owner_name: str,
     value: _ValueT,
     old_name: str,
     new_name: Optional[str] = None,
     message: Optional[str] = None,
     stacklevel: int = DEFAULT_STACK_LEVEL,
@@ -42,16 +43,23 @@
         instead.]
 
     The variations are based on whether ``new_name`` is provided.
 
     Custom messages can also be provided.
 
     Args:
-        warning_cls (type, optional):
-            The class to use for the warning.
+        warning_cls (type or callable):
+            The type of warning class to use, or a callable returning one.
+
+            A callable can be used to avoid circular references.
+
+            Version Changed:
+                1.1:
+                This can now be either a warning class or a function
+                that returns one.
 
         owner_name (str):
             The name of the owner of this argument.
 
         value (object):
             The argument value.
 
@@ -132,15 +140,15 @@
     # NOTE: We do NOT want to use typing here (`LazyObject[...]`), or we'll
     #       trigger some typing logic that stores state on the instance, and
     #       that will load the backed object.
     return LazyObject(_warn_on_use)
 
 
 def deprecate_non_keyword_only_args(
-    warning_cls: DeprecationWarningType,
+    warning_cls: DeprecationWarningTypeOrCallable,
     *,
     message: Optional[str] = None,
     stacklevel: int = DEFAULT_STACK_LEVEL,
 ) -> Callable[[_FuncT], _FuncT]:
     """Deprecate calls passing keyword-only arguments as positional arguments.
 
     This decorator allows code transitioning to keyword-only arguments to
@@ -163,17 +171,23 @@
         arguments when calling `<func_name>()`. Passing as positional
         arguments is scheduled to be deprecated in a future version of
         <product>.
 
     Custom messages can also be provided.
 
     Args:
-        warning_cls (type):
-            The specific deprecation warning class to use. This must be a
-            subclass of :py:exc:`DeprecationWarning`.
+        warning_cls (type or callable):
+            The type of warning class to use, or a callable returning one.
+
+            A callable can be used to avoid circular references.
+
+            Version Changed:
+                1.1:
+                This can now be either a warning class or a function
+                that returns one.
 
         message (str, optional):
             An optional message to use instead of the default.
 
         stacklevel (int, optional):
             A level to use for stack trace.
 
@@ -398,15 +412,15 @@
 
         return cast(_FuncT, _call)
 
     return _dec
 
 
 def func_deprecated(
-    warning_cls: DeprecationWarningType,
+    warning_cls: DeprecationWarningTypeOrCallable,
     *,
     message: Optional[str] = None,
     stacklevel: int = DEFAULT_STACK_LEVEL,
 ) -> Callable[[_FuncT], _FuncT]:
     """Decorator to mark an old function as deprecated or pending deprecation.
 
     This will emit a deprecation warning when called, advising against using
@@ -420,16 +434,23 @@
 
         `<func_name>` is scheduled to be deprecated in a future version of
         <product>.
 
     Custom messages can also be provided.
 
     Args:
-        warning_cls (type):
-            The deprecation warning class to emit.
+        warning_cls (type or callable):
+            The type of warning class to use, or a callable returning one.
+
+            A callable can be used to avoid circular references.
+
+            Version Changed:
+                1.1:
+                This can now be either a warning class or a function
+                that returns one.
 
         message (str, optional):
             A custom message to display for the deprecation message.
 
         stacklevel (int, optional):
             A level to use for stack trace.
 
@@ -473,15 +494,15 @@
 
         return cast(_FuncT, _call)
 
     return _dec
 
 
 def func_moved(
-    warning_cls: DeprecationWarningType,
+    warning_cls: DeprecationWarningTypeOrCallable,
     new_func: Union[str, Callable],
     *,
     message: Optional[str] = None,
     stacklevel: int = DEFAULT_STACK_LEVEL,
 ) -> Callable[[_FuncT], _FuncT]:
     """Decorator to mark an old function as having moved.
 
@@ -497,16 +518,23 @@
 
         `<old_func_name>` has moved to `<new_func_name>`. The old function
         is scheduled to be deprecated in a future version of <product>.
 
     Custom messages can also be provided.
 
     Args:
-        warning_cls (type):
-            The deprecation warning class to emit.
+        warning_cls (type or callable):
+            The type of warning class to use, or a callable returning one.
+
+            A callable can be used to avoid circular references.
+
+            Version Changed:
+                1.1:
+                This can now be either a warning class or a function
+                that returns one.
 
         new_func (str):
             The new function, or a descriptive string referencing the new
             function.
 
         message (str, optional):
             A custom message to display for the deprecation message.
```

### Comparing `housekeeping-1.0/housekeeping/helpers.py` & `housekeeping-1.1/housekeeping/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 This module is not public API, and may change.
 """
 
 from __future__ import annotations
 
 import inspect
 import operator
+from types import FunctionType
 from typing import Any, Callable, Generic, Type, TypeVar, Union, cast
 
-from housekeeping.base import DEFAULT_STACK_LEVEL, DeprecationWarningType
+from housekeeping.base import (DEFAULT_STACK_LEVEL,
+                               DeprecationWarningTypeOrCallable)
 
 
 _T = TypeVar('_T')
 
 
 # NOTE: This must be defined before LazyObject.
 def _new_method_proxy(
@@ -185,29 +187,29 @@
     if inspect.isfunction(entity):
         display_name = f'{display_name}()'
 
     return display_name
 
 
 def emit_warning(
-    warning_cls: DeprecationWarningType,
+    warning_cls: DeprecationWarningTypeOrCallable,
     *,
     deprecation_msg: str,
     pending_deprecation_msg: str,
     stacklevel: int = DEFAULT_STACK_LEVEL,
     **kwargs,
 ) -> None:
     """Emit a warning with a message dependent on the warning type.
 
     This takes in a deprecation message and a pending deprecation message
     and emits a warning with the correct message for the type of warning
     class.
 
     Args:
-        warning_cls (type):
+        warning_cls (type or callable):
             The deprecation warning class.
 
         deprecation_msg (str):
             The message to use for deprecation warnings.
 
         pending_deprecation_msg (str):
             The message to use for pending deprecation warnings.
@@ -219,14 +221,21 @@
 
         **kwargs (dict):
             Additional keyword arguments to pass to
             :py:meth:`~housekeeping.base.BaseDeprecationWarningMixin.warn`.
     """
     message: str
 
+    if isinstance(warning_cls, FunctionType):
+        warning_cls = warning_cls()
+
+    if not inspect.isclass(warning_cls):
+        raise TypeError('Expected a deprecation warning class for %r'
+                        % warning_cls)
+
     if issubclass(warning_cls, DeprecationWarning):
         message = deprecation_msg
     elif issubclass(warning_cls, PendingDeprecationWarning):
         message = pending_deprecation_msg
     else:
         raise TypeError('Invalid deprecation class %r' % warning_cls)
```

### Comparing `housekeeping-1.0/housekeeping/modules.py` & `housekeeping-1.1/housekeeping/modules.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Utilities to deprecate modules."""
 
 from __future__ import annotations
 
 from typing import Optional
 
-from housekeeping.base import DEFAULT_STACK_LEVEL, DeprecationWarningType
+from housekeeping.base import (DEFAULT_STACK_LEVEL,
+                               DeprecationWarningTypeOrCallable)
 from housekeeping.helpers import emit_warning
 
 
 def module_deprecated(
-    warning_cls: DeprecationWarningType,
+    warning_cls: DeprecationWarningTypeOrCallable,
     module_name: str,
     *,
     message: Optional[str] = None,
     stacklevel: int = DEFAULT_STACK_LEVEL,
 ) -> None:
     """Mark a module as deprecated.
 
@@ -28,15 +29,22 @@
     Pending deprecation notices will show a variation of:
 
         `<module_name>` is scheduled to be deprecated in a future version of
         <product>.
 
     Args:
         warning_cls (type, optional):
-            The type of warning class to use.
+            The type of warning class to use, or a callable returning one.
+
+            A callable can be used to avoid circular references.
+
+            Version Changed:
+                1.1:
+                This can now be either a warning class or a function
+                that returns one.
 
         module_name (str):
             The name of the deprecated module.
 
             Callers can pass ``__name__`` to get the current module name.
 
         message (str, optional):
@@ -58,15 +66,15 @@
             'version of %(product)s.'
         ),
         module_name=module_name,
         stacklevel=stacklevel + 1)  # Factor in this function.
 
 
 def module_moved(
-    warning_cls: DeprecationWarningType,
+    warning_cls: DeprecationWarningTypeOrCallable,
     old_module_name: str,
     new_module_name: str,
     *,
     message: Optional[str] = None,
     stacklevel: int = DEFAULT_STACK_LEVEL,
 ) -> None:
     """Mark a module as having moved to another location.
@@ -82,15 +90,22 @@
     Pending deprecation notices will show a variation of:
 
         `<old_module_name>` is scheduled to be deprecated in a future version
         of <product>. To prepare, import `<new_module_name>` instead.
 
     Args:
         warning_cls (type, optional):
-            The type of warning class to use.
+            The type of warning class to use, or a callable returning one.
+
+            A callable can be used to avoid circular references.
+
+            Version Changed:
+                1.1:
+                This can now be either a warning class or a function
+                that returns one.
 
         old_module_name (str):
             The name of the deprecated module.
 
             Callers can pass ``__name__`` to get the current module name.
 
         new_module_name (str):
```

### Comparing `housekeeping-1.0/housekeeping/tests/test_classes.py` & `housekeeping-1.1/housekeeping/tests/test_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,33 @@
         )
         line = 'class MySubclass(MyOldClass):'
 
         with self.assertWarning(MyPendingRemovalWarning, message, line):
             class MySubclass(MyOldClass):
                 pass
 
+    def test_subclass_with_warning_cls_callable(self) -> None:
+        """Testing ClassDeprecatedMixin subclassing with warning_cls as
+        callable
+        """
+        class MyOldClass(ClassDeprecatedMixin,
+                         warning_cls=lambda: MyRemovedInWarning):
+            pass
+
+        prefix = self.locals_prefix
+        message = (
+            f'`{prefix}.MySubclass` subclasses `{prefix}.MyOldClass`, which '
+            f'is deprecated and will be removed in My Product 1.0.'
+        )
+        line = 'class MySubclass(MyOldClass):'
+
+        with self.assertWarning(MyRemovedInWarning, message, line):
+            class MySubclass(MyOldClass):
+                pass
+
     def test_subclass_with_deprecation_msg(self) -> None:
         """Testing ClassDeprecatedMixin subclassing with deprecation and
         subclass_deprecation_msg=
         """
         class MyOldClass(ClassDeprecatedMixin,
                          warning_cls=MyRemovedInWarning,
                          subclass_deprecation_msg=(
@@ -200,14 +219,35 @@
             pass
 
         prefix = self.locals_prefix
         message = (
             f'`{prefix}.MySubclass` subclasses `{prefix}.MyOldClass`, which '
             f'is scheduled to be deprecated in a future version of My '
             f'Product. To prepare, subclass `{prefix}.MyNewClass` instead.'
+        )
+        line = 'class MySubclass(MyOldClass):'
+
+        with self.assertWarning(MyPendingRemovalWarning, message, line):
+            class MySubclass(MyOldClass):
+                pass
+
+    def test_subclass_with_warning_cls_callable(self) -> None:
+        """Testing ClassMovedMixin subclassing with warning_cls as callable"""
+        class MyNewClass:
+            pass
+
+        class MyOldClass(ClassMovedMixin, MyNewClass,
+                         warning_cls=lambda: MyPendingRemovalWarning):
+            pass
+
+        prefix = self.locals_prefix
+        message = (
+            f'`{prefix}.MySubclass` subclasses `{prefix}.MyOldClass`, which '
+            f'is scheduled to be deprecated in a future version of My '
+            f'Product. To prepare, subclass `{prefix}.MyNewClass` instead.'
         )
         line = 'class MySubclass(MyOldClass):'
 
         with self.assertWarning(MyPendingRemovalWarning, message, line):
             class MySubclass(MyOldClass):
                 pass
```

### Comparing `housekeeping-1.0/housekeeping/tests/test_functions.py` & `housekeeping-1.1/housekeeping/tests/test_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,33 @@
         line = 'result = 1 + value'
 
         with self.assertWarning(MyRemovedInWarning, message, line):
             result = 1 + value
 
         self.assertEqual(result, 124)
 
+    def test_with_warning_cls_as_callable(self) -> None:
+        """Testing deprecated_arg_value with warning_cls as callable"""
+        value = deprecated_arg_value(
+            lambda: MyRemovedInWarning,
+            owner_name='my_func()',
+            value=123,
+            old_name='old_arg')
+
+        message = (
+            '`old_arg` for `my_func()` has been deprecated and will be '
+            'removed in My Product 1.0.'
+        )
+        line = 'result = 1 + value'
+
+        with self.assertWarning(MyRemovedInWarning, message, line):
+            result = 1 + value
+
+        self.assertEqual(result, 124)
+
 
 class DeprecateNonKeywordOnlyArgsTests(TestCase):
     """Unit tests for @deprecate_non_keyword_only_args."""
 
     def test_decorated_state(self) -> None:
         """Testing @deprecate_non_keyword_only_args preserves decorated
         function state
@@ -168,14 +187,35 @@
         line = 'result = my_func(1, 2, 3)  # type: ignore'
 
         with self.assertWarning(MyPendingRemovalWarning, message, line):
             result = my_func(1, 2, 3)  # type: ignore
 
         self.assertEqual(result, 6)
 
+    def test_with_warning_cls_callable(self) -> None:
+        """Testing @deprecate_non_keyword_only_args with warning_cls as
+        callable
+        """
+        @deprecate_non_keyword_only_args(lambda: MyRemovedInWarning)
+        def my_func(a, *, b, c=1):
+            return a + b + c
+
+        prefix = self.locals_prefix
+        message = (
+            f'Positional argument `b` must be passed as a keyword argument '
+            f'when calling `{prefix}.my_func()`. Passing as a positional '
+            f'argument will be required in My Product 1.0.'
+        )
+        line = 'result = my_func(1, 2, c=3)  # type: ignore'
+
+        with self.assertWarning(MyRemovedInWarning, message, line):
+            result = my_func(1, 2, c=3)  # type: ignore
+
+        self.assertEqual(result, 6)
+
 
 class FuncDeprecatedTests(TestCase):
     """Unit tests for func_deprecated."""
 
     def test_decorated_state(self) -> None:
         """Testing @func_deprecated preserves decorated function state"""
         @func_deprecated(MyRemovedInWarning)
@@ -258,14 +298,32 @@
         line = 'result = my_func(1, 2)'
 
         with self.assertWarning(MyPendingRemovalWarning, message, line):
             result = my_func(1, 2)
 
         self.assertEqual(result, 3)
 
+    def test_with_warning_cls_callable(self) -> None:
+        """Testing @func_deprecated with warning_cls as callable"""
+        @func_deprecated(lambda: MyRemovedInWarning)
+        def my_func(a, b):
+            return a + b
+
+        prefix = self.locals_prefix
+        message = (
+            f'`{prefix}.my_func()` is deprecated and will be removed in My '
+            f'Product 1.0.'
+        )
+        line = 'result = my_func(1, 2)'
+
+        with self.assertWarning(MyRemovedInWarning, message, line):
+            result = my_func(1, 2)
+
+        self.assertEqual(result, 3)
+
 
 class FuncMovedTests(TestCase):
     """Unit tests for func_moved."""
 
     def test_decorated_state(self) -> None:
         """Testing @func_moved preserves decorated function state"""
         @func_moved(MyRemovedInWarning, 'new_func')
@@ -397,7 +455,26 @@
         )
         line = 'result = my_func(1, 2)'
 
         with self.assertWarning(MyPendingRemovalWarning, message, line):
             result = my_func(1, 2)
 
         self.assertEqual(result, 3)
+
+    def test_with_warning_cls_callable(self) -> None:
+        """Testing @func_moved with warning_cls as callable"""
+        @func_moved(lambda: MyRemovedInWarning,
+                    'my_new_func')
+        def my_func(a, b):
+            return a + b
+
+        prefix = self.locals_prefix
+        message = (
+            f'`{prefix}.my_func()` has moved to `my_new_func()`. The old '
+            f'function is deprecated and will be removed in My Product 1.0.'
+        )
+        line = 'result = my_func(1, 2)'
+
+        with self.assertWarning(MyRemovedInWarning, message, line):
+            result = my_func(1, 2)
+
+        self.assertEqual(result, 3)
```

### Comparing `housekeeping-1.0/housekeeping/tests/test_modules.py` & `housekeeping-1.1/housekeeping/tests/test_modules.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,28 @@
             'Custom message: housekeeping.tests.test_modules; My Product; 1.0'
         )
 
         with self.assertWarning(MyRemovedInWarning, message,
                                 '_import_module()'):
             _import_module()
 
+    def test_with_warning_cls_callable(self) -> None:
+        """Testing module_deprecated and warning_cls as callable"""
+        def _import_module():
+            module_deprecated(lambda: MyRemovedInWarning, __name__)
+
+        message = (
+            '`housekeeping.tests.test_modules` is deprecated and will be '
+            'removed in My Product 1.0.'
+        )
+
+        with self.assertWarning(MyRemovedInWarning, message,
+                                '_import_module()'):
+            _import_module()
+
 
 class ModuleMovedTests(TestCase):
     """Unit tests for module_moved."""
 
     def test_with_deprecation_warning(self) -> None:
         """Testing module_moved and deprecation"""
         def _import_module():
@@ -107,7 +121,21 @@
             'Custom message: housekeeping.tests.test_modules; my.new.module; '
             'My Product; 1.0'
         )
 
         with self.assertWarning(MyRemovedInWarning, message,
                                 '_import_module()'):
             _import_module()
+
+    def test_with_warning_cls_callable(self) -> None:
+        """Testing module_moved and warning_cls as callable"""
+        def _import_module():
+            module_moved(lambda: MyRemovedInWarning, __name__, 'my.new.module')
+
+        message = (
+            '`housekeeping.tests.test_modules` is deprecated and will be '
+            'removed in My Product 1.0. Import `my.new.module` instead.'
+        )
+
+        with self.assertWarning(MyRemovedInWarning, message,
+                                '_import_module()'):
+            _import_module()
```

### Comparing `housekeeping-1.0/housekeeping/tests/testcases.py` & `housekeeping-1.1/housekeeping/tests/testcases.py`

 * *Files identical despite different names*

### Comparing `housekeeping-1.0/housekeeping.egg-info/PKG-INFO` & `housekeeping-1.1/housekeeping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeping
-Version: 1.0
+Version: 1.1
 Summary: Python utilities for helping deprecate and remove code.
 Author-email: "Beanbag, Inc." <questions@beanbaginc.com>
 License: MIT
 Project-URL: homepage, https://github.com/beanbaginc/housekeeping
 Project-URL: documentation, https://github.com/beanbaginc/housekeeping
 Project-URL: repository, https://github.com/beanbaginc/housekeeping
 Keywords: deprecation,cleanup,code quality
```

### Comparing `housekeeping-1.0/housekeeping.egg-info/SOURCES.txt` & `housekeeping-1.1/housekeeping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `housekeeping-1.0/pyproject.toml` & `housekeeping-1.1/pyproject.toml`

 * *Files identical despite different names*

