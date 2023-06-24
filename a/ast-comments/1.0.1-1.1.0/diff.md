# Comparing `tmp/ast_comments-1.0.1.tar.gz` & `tmp/ast_comments-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ast_comments-1.0.1.tar", max compression
+gzip compressed data, was "ast_comments-1.1.0.tar", max compression
```

## Comparing `ast_comments-1.0.1.tar` & `ast_comments-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-02-18 16:12:05.559648 ast_comments-1.0.1/LICENSE
--rw-r--r--   0        0        0     1643 2023-03-06 08:16:19.791946 ast_comments-1.0.1/README.md
--rw-r--r--   0        0        0     4696 2023-03-13 10:06:53.977036 ast_comments-1.0.1/ast_comments.py
--rw-r--r--   0        0        0      545 2023-03-13 10:10:05.322919 ast_comments-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2200 1970-01-01 00:00:00.000000 ast_comments-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-02-18 16:12:05.559648 ast_comments-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1187 2023-05-09 07:25:08.794505 ast_comments-1.1.0/README.md
+-rw-r--r--   0        0        0     5823 2023-06-24 14:37:59.947225 ast_comments-1.1.0/ast_comments.py
+-rw-r--r--   0        0        0      545 2023-06-24 14:40:05.866049 ast_comments-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 ast_comments-1.1.0/setup.py
+-rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 ast_comments-1.1.0/PKG-INFO
```

### Comparing `ast_comments-1.0.1/LICENSE` & `ast_comments-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_comments-1.0.1/README.md` & `ast_comments-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: ast-comments
+Version: 1.1.0
+Summary: 
+Home-page: https://github.com/t3rn0/ast-comments
+Author: Dmitry Makarov
+Author-email: dmtern0vnik@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/t3rn0/ast-comments
+Description-Content-Type: text/markdown
+
 # ast-comments
 
 An extension to the built-in `ast` module. 
 Finds comments in source code and adds them to the parsed tree.
 
 ## Installation
 ```
@@ -21,35 +37,19 @@
 >>> tree
 <_ast.Module object at 0x7ffba52322e0>
 >>> tree.body
 [<ast_comments.Comment object at 0x10c1b6160>, <_ast.Assign object at 0x10bd217c0>]
 >>> tree.body[0].value
 '# comment to hello'
 >>> dump(tree)
-"Module(body=[Comment(value='# comment to hello'), Assign(targets=[Name(id='hello', ctx=Store())], value=Constant(value='hello', kind=None), type_comment=None)], type_ignores=[])"
+"Module(body=[Assign(targets=[Name(id='hello', ctx=Store())], value=Constant(value='hello', kind=None), type_comment=None), Comment(value='# comment to hello', inline=True)], type_ignores=[])"
 ```
 If you have python3.9 or above it's also possible to unparse the tree object with its comments preserved.
 ```
 >>> print(unparse(tree))
 # comment to hello
 hello = 'hello'
 ```
 More examples can be found in test_parse.py and test_unparse.py.
 
-## Notes
-1. Right now it is assumed that there is no difference between inlined comments and regular. 
-All inlined comments become regular after the tree object is unparsed.
-
-2. Inlined comments for class- (def-, if-, ...) block shift "inside" body of the corresponding block:
-    ```
-    >>> source = """class Foo: # c1
-    ...     pass
-    ... """
-    >>> unparse(parse(source))
-    >>> print(unparse(parse(source)))
-    class Foo:
-        # c1
-        pass
-    ```
-
 ## Contributing
-You are welcome to open an issue or create a pull request
+You are welcome to open an issue or create a pull request
```

### Comparing `ast_comments-1.0.1/ast_comments.py` & `ast_comments-1.1.0/ast_comments.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from ast import *  # noqa: F401,F403
 from collections.abc import Iterable
 from typing import Dict, List, Tuple, Union
 
 
 class Comment(ast.AST):
     value: str
-    _fields = ("value",)
+    inline: bool
+    _fields = (
+        "value",
+        "inline",
+    )
 
 
 _CONTAINER_ATTRS = ["body", "handlers", "orelse", "finalbody"]
 
 
 def parse(source: Union[str, bytes, ast.AST], *args, **kwargs) -> ast.AST:
     tree = ast.parse(source, *args, **kwargs)
@@ -31,14 +35,15 @@
     for t in tokens:
         if t.type != tokenize.COMMENT:
             continue
         lineno, col_offset = t.start
         end_lineno, end_col_offset = t.end
         c = Comment(
             value=t.string,
+            inline=t.string != t.line.strip("\n").strip(" "),
             lineno=lineno,
             col_offset=col_offset,
             end_lineno=end_lineno,
             end_col_offset=end_col_offset,
         )
         comment_nodes.append(c)
 
@@ -68,15 +73,36 @@
             *_, target_attr = sub_intervals[loc]
         else:
             target_node = tree
             target_attr = "body"
 
         attr = getattr(target_node, target_attr)
         attr.append(c_node)
-        attr.sort(key=lambda x: (x.end_lineno, not isinstance(x, Comment)))
+        attr.sort(key=lambda x: (x.end_lineno, isinstance(x, Comment)))
+
+        # NOTE:
+        # Due to some issues it's possible for comment nodes to go outside of their initial place
+        # after the parse-unparse roundtip:
+        #   before parse/unparse:
+        #   ```
+        #   # comment 0
+        #   some_code  # comment 1
+        #   ```
+        #   after parse/unparse:
+        #   ```
+        #   # comment 0  # comment 1
+        #   some_code
+        #   ```
+        # As temporary workaround I decided to correct inline attributes here so they don't
+        # overlap with each other. This place should be revisited after solving following issues:
+        # - https://github.com/t3rn0/ast-comments/issues/10
+        # - https://github.com/t3rn0/ast-comments/issues/13
+        for left, right in zip(attr[:-1], attr[1:]):
+            if isinstance(left, Comment) and isinstance(right, Comment):
+                right.inline = False
 
 
 def _get_tree_intervals(
     node: ast.AST,
 ) -> Dict[Tuple[int, int], Dict[str, Union[List[Tuple[int, int]], ast.AST]]]:
     res = {}
     for node in ast.walk(node):
@@ -86,35 +112,39 @@
                 if not isinstance(items, Iterable):
                     continue
                 attr_intervals.append((*_get_interval(items), attr))
         if attr_intervals:
             low = node.lineno if hasattr(node, "lineno") else min(attr_intervals)[0]
             high = (
                 node.end_lineno
-                if hasattr(node, "endlineno")
+                if hasattr(node, "end_lineno")
                 else max(attr_intervals)[1]
             )
             res[(low, high)] = {"intervals": attr_intervals, "node": node}
     return res
 
 
+# get min and max line from a source tree
 def _get_interval(items: List[ast.AST]) -> Tuple[int, int]:
     linenos, end_linenos = [], []
     for item in items:
         linenos.append(item.lineno)
         end_linenos.append(item.end_lineno)
     return min(linenos), max(end_linenos)
 
 
 # `unparse` has been introduced in Python 3.9
 if sys.version_info >= (3, 9):
 
     class _Unparser(ast._Unparser):
         def visit_Comment(self, node: Comment) -> None:
-            self.fill(node.value)
+            if node.inline:
+                self.write(f"  {node.value}")
+            else:
+                self.fill(node.value)
 
         def visit_If(self, node: ast.If) -> None:
             def _get_first_not_comment_idx(orelse: list[ast.stmt]) -> int:
                 i = 0
                 while i < len(orelse) and isinstance(orelse[i], Comment):
                     i += 1
                 return i
```

### Comparing `ast_comments-1.0.1/pyproject.toml` & `ast_comments-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ast-comments"
-version = "1.0.1"
+version = "1.1.0"
 description = ""
 readme = "README.md"
 repository = "https://github.com/t3rn0/ast-comments"
 homepage = "https://github.com/t3rn0/ast-comments"
 authors = ["Dmitry Makarov <dmtern0vnik@gmail.com>"]
 
 [tool.poetry.dependencies]
```

