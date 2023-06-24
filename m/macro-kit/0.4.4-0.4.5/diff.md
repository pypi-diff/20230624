# Comparing `tmp/macro_kit-0.4.4.tar.gz` & `tmp/macro_kit-0.4.5.tar.gz`

## Comparing `macro_kit-0.4.4.tar` & `macro_kit-0.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/__init__.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/_symbol.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/_validator.py
--rw-r--r--   0        0        0    17970 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/ast.py
--rw-r--r--   0        0        0    32474 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/expression.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/head.py
--rw-r--r--   0        0        0    33105 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/macro.py
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/mock.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/py.typed
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/type_map.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/utils.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/ipython/__init__.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/ipython/magic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/julia/__init__.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/julia/translate.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 macro_kit-0.4.4/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 macro_kit-0.4.4/LICENSE
--rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 macro_kit-0.4.4/README.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 macro_kit-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 macro_kit-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/__init__.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/_symbol.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/_validator.py
+-rw-r--r--   0        0        0    17842 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/ast.py
+-rw-r--r--   0        0        0    33045 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/expression.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/head.py
+-rw-r--r--   0        0        0    33105 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/macro.py
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/mock.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/py.typed
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/type_map.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/utils.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/ipython/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/ipython/magic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/julia/__init__.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 macro_kit-0.4.5/macrokit/julia/translate.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 macro_kit-0.4.5/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 macro_kit-0.4.5/LICENSE
+-rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 macro_kit-0.4.5/README.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 macro_kit-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 macro_kit-0.4.5/PKG-INFO
```

### Comparing `macro_kit-0.4.4/macrokit/__init__.py` & `macro_kit-0.4.5/macrokit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """macro-kit is a package for macro recording and metaprogramming in Python."""
 
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 __author__ = "Hanjin Liu"
 __email__ = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp"
 
 from macrokit._symbol import Symbol
 from macrokit.expression import (
     Expr,
     Head,
```

### Comparing `macro_kit-0.4.4/macrokit/_symbol.py` & `macro_kit-0.4.5/macrokit/_symbol.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/macrokit/_validator.py` & `macro_kit-0.4.5/macrokit/_validator.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/macrokit/ast.py` & `macro_kit-0.4.5/macrokit/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,31 +585,29 @@
         ]
 
 
 def _nest_joinedstr(ast_object: ast.JoinedStr):
     strs: "list[str]" = []
     for k in ast_object.values:
         if isinstance(k, ast.FormattedValue):
-            name = k.value
-            if not isinstance(name, ast.Name):
-                raise RuntimeError(f"Unknown name type: {type(name)}")
+            _id = ast.unparse(k.value)
             if k.format_spec is None:
                 if k.conversion == -1:
-                    strs.append("{" + f"{name.id}" + "}")
+                    strs.append("{" + f"{_id}" + "}")
                 elif k.conversion == 115:
-                    strs.append("{" + f"{name.id}!s" + "}")
+                    strs.append("{" + f"{_id}!s" + "}")
                 elif k.conversion == 114:
-                    strs.append("{" + f"{name.id}!r" + "}")
+                    strs.append("{" + f"{_id}!r" + "}")
                 elif k.conversion == 97:
-                    strs.append("{" + f"{name.id}!a" + "}")
+                    strs.append("{" + f"{_id}!a" + "}")
                 else:
                     raise RuntimeError(f"Unknown conversion: {k.conversion}")
             elif isinstance(k.format_spec, ast.JoinedStr):
                 fspec = _nest_joinedstr(k.format_spec)
-                strs.append("{" + f"{name.id}:{fspec}" + "}")
+                strs.append("{" + f"{_id}:{fspec}" + "}")
             else:
                 raise RuntimeError(f"Unknown format_spec type: {type(k.format_spec)}")
         elif isinstance(k, ast.Constant):
             strs.append(k.value)
         else:
             raise RuntimeError(f"Unknown JoinedStr value type: {type(k)}")
     return "".join(strs)
```

### Comparing `macro_kit-0.4.4/macrokit/expression.py` & `macro_kit-0.4.5/macrokit/expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,22 +132,44 @@
     else:
         args = x.args
         prefix = ""
 
     return f"{_s_(i)}{prefix}import {sjoin(', ', args, i)}"
 
 
+def _only_generator(args: "list[Expr | Symbol]") -> bool:
+    return (
+        len(args) == 1 and isinstance(args[0], Expr) and args[0].head is Head.generator
+    )
+
+
+def _list_str(x: "Expr", i: int) -> str:
+    args = x.args
+    if _only_generator(args):
+        return f"{_s_(i)}[{rm_par(str_(args[0]))}]"
+    else:
+        return f"{_s_(i)}[{', '.join(str_(arg) for arg in args)}]"
+
+
+def _braces_str(x: "Expr", i: int) -> str:
+    args = x.args
+    if _only_generator(args):
+        return f"{_s_(i)}{{{rm_par(str_(args[0]))}}}"
+    else:
+        return f"{_s_(i)}{{{', '.join(str_(arg) for arg in args)}}}"
+
+
 _STR_MAP: "dict[Head, Callable[[Expr, int], str]]" = {
     Head.empty: lambda e, i: "",
     Head.getattr: lambda e, i: f"{str_(e.args[0], i)}.{str_(e.args[1])}",
     Head.getitem: lambda e, i: f"{str_(e.args[0], i)}[{rm_par(str_(e.args[1]))}]",
     Head.del_: lambda e, i: f"{_s_(i)}del {str_(e.args[0])}",
     Head.tuple: _tuple_str,
-    Head.list: lambda e, i: f"{_s_(i)}[{', '.join(str_(arg) for arg in e.args)}]",
-    Head.braces: lambda e, i: f"{_s_(i)}{{{', '.join(str_(arg) for arg in e.args)}}}",
+    Head.list: _list_str,
+    Head.braces: _braces_str,
     Head.call: lambda e, i: f"{str_(e.args[0], i)}({sjoin(', ', e.args[1:])})",
     Head.assign: lambda e, i: f"{str_(e.args[0], i)} = {e.args[1]}",
     Head.kw: lambda e, i: f"{str_(e.args[0])}={str_(e.args[1])}",
     Head.assert_: _assert_str,
     Head.comment: lambda e, i: f"{_s_(i)}# {e.args[0]}",
     Head.unop: lambda e, i: f"{_s_(i)}({str_(e.args[0])}{str_(e.args[1])})",
     Head.binop: lambda e, i: f"{_s_(i)}({str_(e.args[1])} {str_(e.args[0])} {str_(e.args[2])})",  # noqa
@@ -391,17 +413,20 @@
         ns : Dict[str, Any], optional
             Namespace used for evaluation.
         """
         if self.head is not Head.call:
             raise ValueError(f"Expected {Head.call}, got {self.head}.")
         # search for the index where keyword argument starts
         arguments = self.args[1:]
+        i = 0
         for i, arg in enumerate(arguments):
             if isinstance(arg, Expr) and arg.head is Head.kw:
                 break
+        else:
+            i += 1
 
         _args = arguments[:i]
         _kwargs = arguments[i:]
 
         # prepare namespaces
         args_ns: dict[Union[str, _Expr], Any] = ns.copy()
         args_ns[symbol(_tuple)] = _tuple
```

### Comparing `macro_kit-0.4.4/macrokit/head.py` & `macro_kit-0.4.5/macrokit/head.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/macrokit/macro.py` & `macro_kit-0.4.5/macrokit/macro.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/macrokit/mock.py` & `macro_kit-0.4.5/macrokit/mock.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/macrokit/type_map.py` & `macro_kit-0.4.5/macrokit/type_map.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/macrokit/utils.py` & `macro_kit-0.4.5/macrokit/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,16 @@
         """Error description with the causes."""
         return f"{super().__str__()} (Caused by: `{self._expr}` in `{self._line}`)"
 
 
 _BUILTIN_FUNCTION_OR_METHOD = type(print)
 
 
-def check_attributes(code: Expr, ns: dict[str, Any]) -> list[ExprCheckError]:
+# TODO: import
+def check_attributes(code: Expr, ns: dict[str, Any] = {}) -> list[ExprCheckError]:
     """Check if the given code contains undefined attributes."""
     errors = list[ExprCheckError]()
     for line in code.iter_lines():
         if isinstance(line, Symbol):
             continue
         for expr in line.iter_getattr():
             try:
@@ -35,26 +36,26 @@
                 errors.append(ExprCheckError(str(e), expr, line))
             except NameError:
                 # variables defined during the execution of the code.
                 pass
     return errors
 
 
-def check_call_args(code: Expr, ns: dict[str, Any]) -> list[ExprCheckError]:
+def check_call_args(code: Expr, ns: dict[str, Any] = {}) -> list[ExprCheckError]:
     """Check if all the function calls in the given code are valid."""
     errors = list[ExprCheckError]()
     for line in code.iter_lines():
         if isinstance(line, Symbol):
             continue
         for expr in line.iter_call():
             fexpr, args, kwargs = expr.split_call()
             _method = fexpr.eval(ns)
             if isinstance(_method, _BUILTIN_FUNCTION_OR_METHOD):
                 continue
             try:
                 inspect.signature(_method).bind(*args, **kwargs)
             except TypeError as e:
                 errors.append(ExprCheckError(str(e), expr, line))
-            except ValueError:
+            except (ValueError, NameError):
                 # builtin classes such as `range`.
                 pass
     return errors
```

### Comparing `macro_kit-0.4.4/macrokit/ipython/magic.py` & `macro_kit-0.4.5/macrokit/ipython/magic.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/macrokit/julia/translate.py` & `macro_kit-0.4.5/macrokit/julia/translate.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/.gitignore` & `macro_kit-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/LICENSE` & `macro_kit-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/README.md` & `macro_kit-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/pyproject.toml` & `macro_kit-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.4/PKG-INFO` & `macro_kit-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macro-kit
-Version: 0.4.4
+Version: 0.4.5
 Summary: Macro recording and metaprogramming in Python
 Project-URL: Download, https://github.com/hanjinliu/macro-kit
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, hanjinliu
         All rights reserved.
```

