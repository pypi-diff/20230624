# Comparing `tmp/mmodel-0.6.1.tar.gz` & `tmp/mmodel-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmodel-0.6.1.tar", max compression
+gzip compressed data, was "mmodel-0.6.2.tar", max compression
```

## Comparing `mmodel-0.6.1.tar` & `mmodel-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1718 2022-08-01 16:13:58.303654 mmodel-0.6.1/LICENSE
--rw-r--r--   0        0        0     5682 2023-04-18 17:17:51.785026 mmodel-0.6.1/README.rst
--rw-r--r--   0        0        0       83 2023-04-18 17:17:51.787413 mmodel-0.6.1/mmodel/__init__.py
--rw-r--r--   0        0        0     2574 2023-04-19 16:44:58.026268 mmodel-0.6.1/mmodel/draw.py
--rw-r--r--   0        0        0     1260 2023-03-30 19:59:00.773890 mmodel-0.6.1/mmodel/filter.py
--rw-r--r--   0        0        0     8399 2023-04-18 17:17:51.787590 mmodel-0.6.1/mmodel/graph.py
--rw-r--r--   0        0        0     6475 2023-04-18 17:17:51.787955 mmodel-0.6.1/mmodel/handler.py
--rw-r--r--   0        0        0     7064 2023-04-18 17:17:51.788305 mmodel-0.6.1/mmodel/metadata.py
--rw-r--r--   0        0        0     5789 2023-04-18 17:17:51.788620 mmodel-0.6.1/mmodel/model.py
--rw-r--r--   0        0        0     6428 2023-04-18 17:17:51.788770 mmodel-0.6.1/mmodel/modifier.py
--rw-r--r--   0        0        0     6009 2023-04-18 17:17:51.788896 mmodel-0.6.1/mmodel/parser.py
--rw-r--r--   0        0        0      391 2023-04-18 17:17:51.788972 mmodel-0.6.1/mmodel/shortcut.py
--rw-r--r--   0        0        0     9239 2023-04-18 17:17:51.789182 mmodel-0.6.1/mmodel/utility.py
--rw-r--r--   0        0        0     2485 2023-04-19 16:44:58.026540 mmodel-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     7280 1970-01-01 00:00:00.000000 mmodel-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1718 2022-08-01 16:13:58.303654 mmodel-0.6.2/LICENSE
+-rw-r--r--   0        0        0     5924 2023-06-24 02:21:00.546647 mmodel-0.6.2/README.rst
+-rw-r--r--   0        0        0       83 2023-04-18 17:17:51.787413 mmodel-0.6.2/mmodel/__init__.py
+-rw-r--r--   0        0        0     2574 2023-04-19 16:44:58.026268 mmodel-0.6.2/mmodel/draw.py
+-rw-r--r--   0        0        0     1260 2023-06-22 17:24:00.292747 mmodel-0.6.2/mmodel/filter.py
+-rw-r--r--   0        0        0     8409 2023-06-21 14:18:42.943596 mmodel-0.6.2/mmodel/graph.py
+-rw-r--r--   0        0        0     6475 2023-04-18 17:17:51.787955 mmodel-0.6.2/mmodel/handler.py
+-rw-r--r--   0        0        0     7069 2023-06-22 02:24:35.466189 mmodel-0.6.2/mmodel/metadata.py
+-rw-r--r--   0        0        0     5785 2023-06-09 16:19:05.226977 mmodel-0.6.2/mmodel/model.py
+-rw-r--r--   0        0        0     6428 2023-06-21 21:02:09.593628 mmodel-0.6.2/mmodel/modifier.py
+-rw-r--r--   0        0        0     6240 2023-06-21 14:18:42.944126 mmodel-0.6.2/mmodel/parser.py
+-rw-r--r--   0        0        0      476 2023-06-22 18:53:17.670892 mmodel-0.6.2/mmodel/shortcut.py
+-rw-r--r--   0        0        0     9239 2023-04-18 17:17:51.789182 mmodel-0.6.2/mmodel/utility.py
+-rw-r--r--   0        0        0     2484 2023-06-24 15:18:26.949018 mmodel-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     7521 1970-01-01 00:00:00.000000 mmodel-0.6.2/PKG-INFO
```

### Comparing `mmodel-0.6.1/LICENSE` & `mmodel-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mmodel-0.6.1/README.rst` & `mmodel-0.6.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 |Docs|
 
 MModel is a lightweight and modular model-building framework
 for small-scale and nonlinear models. The package aims to solve
 scientific program prototyping and distribution difficulties, making
 it easier to create modular, fast, and user-friendly packages.
 
+For using mmodel in a complex scientific workflow, please refer to
+the `mrfmsim <https://marohn-group.github.io/mrfmsim-docs/overview.html>`__
+on how mmodel improves the development of magnetic resonance force
+microscopy (MRFM) experiments.
+
 Quickstart
 ----------
 
 To create a nonlinear model that has the result of
 `(x + y)log(x + y, base)`:
 
 .. code-block:: python
```

### Comparing `mmodel-0.6.1/mmodel/draw.py` & `mmodel-0.6.2/mmodel/draw.py`

 * *Files identical despite different names*

### Comparing `mmodel-0.6.1/mmodel/filter.py` & `mmodel-0.6.2/mmodel/filter.py`

 * *Files identical despite different names*

### Comparing `mmodel-0.6.1/mmodel/graph.py` & `mmodel-0.6.2/mmodel/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         _func, functype, doc.
         """
 
         node_dict = self.nodes[node]
         parser = self.graph["parser"]
 
         modifiers = modifiers or list()
-        attr_dict = parser(node, func, output, inputs, modifiers)
+        attr_dict = parser(node, func, output, inputs, modifiers, **kwargs)
         node_dict.update(attr_dict)
         node_dict.update(kwargs)
 
         self.update_graph()
 
     def set_node_objects_from(self, node_objects: list):
         """Update the functions of existing nodes.
```

### Comparing `mmodel-0.6.1/mmodel/handler.py` & `mmodel-0.6.2/mmodel/handler.py`

 * *Files identical despite different names*

### Comparing `mmodel-0.6.1/mmodel/metadata.py` & `mmodel-0.6.2/mmodel/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         return metadata_str_list
 
 
 def format_func(key, value):
     """Format the metadata value that has a function.
 
     The key name is not shown in the string output.
-    The result is func(args1, args2, ...)"""
+    The result is func(args1, args2, ...)."""
 
     return [f"{value.__name__}{inspect.signature(value)}"]
 
 
 def format_list(key, value):
     """Format the metadata value that is a list."""
 
@@ -157,15 +157,15 @@
     else:
         returns_str = f"({', '.join(value)})"
 
     return [f"{key}: {returns_str}"]
 
 
 def format_value(key, value):
-    """Format the metadata without displaying key."""
+    """Format the metadata without displaying the key."""
     if value:
         return [value]
     else:
         return []
 
 
 def format_obj(key, value):
```

### Comparing `mmodel-0.6.1/mmodel/model.py` & `mmodel-0.6.2/mmodel/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,13 +160,13 @@
 
         return draw_graph(self._graph, str(self), style, export)
 
     def edit(self, **kwargs):
         """Edit components of the model to create a new model.
 
         It is not recommended to edit the graph component of the model.
-        Although it does create a new model, but "edit" is for creating
+        Although it does create a new model, "edit" is for creating
         a new model with the same graph.
         """
 
         model_dict = {key: getattr(self, key) for key in self._model_keys}
         return self.__class__(**{**model_dict, **kwargs})
```

### Comparing `mmodel-0.6.1/mmodel/modifier.py` & `mmodel-0.6.2/mmodel/modifier.py`

 * *Files identical despite different names*

### Comparing `mmodel-0.6.1/mmodel/parser.py` & `mmodel-0.6.2/mmodel/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,41 +16,53 @@
 
     To add additional function types, subclass this class.
     """
 
     def __init__(self, parser_dict):
         self._parser_dict = parser_dict
 
-    def __call__(self, node, func, output, inputs, modifiers):
+    def __call__(self, node, func, output, inputs, modifiers, **kwargs):
         """Check if the function belongs to the correct type.
 
         Returns customized dictionary if that is true. It is possible
         that some of the function options overlap when the list goes
         long, the order of the parser is important.
         """
+
+        if "doc" in kwargs:
+            doc = kwargs["doc"]
+        else:
+            doc = ""
         for parser in self._parser_dict.values():
             attr_dict = parser(
-                node=node, func=func, output=output, inputs=inputs, modifiers=modifiers
+                node=node,
+                func=func,
+                output=output,
+                inputs=inputs,
+                modifiers=modifiers,
+                **kwargs,
             )
             if attr_dict:
                 func = attr_dict["_func"]
                 # apply the modifiers
                 for mdf in modifiers:
                     func = mdf(func)
 
                 sig = inspect.signature(func)
+
                 base_dict = {
                     "func": func,
                     "sig": sig,
                     "output": output,
                     "modifiers": modifiers,
+                    "doc": doc,
                 }
                 # attr dict can overwrite the base dict
-                attr_dict.update(base_dict)
-                return attr_dict
+                base_dict.update(attr_dict)
+                return base_dict
 
 
 def grab_docstring(docstring):
     """Parse docstring from built-in function and numpy.ufunc.
 
     The built-in and ufunc type docstring location is not consistent
     some module/function has the repr at the first line, and some don't.
@@ -69,14 +81,15 @@
 
 def parse_default(node, func, inputs, **kwargs):
     """Return the default function dictionary.
 
     The function needs to have the start uppercase and end period style of
     docstring.
     """
+
     if callable(func):
         func_dict = {}
 
         doc = ""
         if hasattr(func, "__doc__") and func.__doc__:
             doc = grab_docstring(func.__doc__)
```

### Comparing `mmodel-0.6.1/mmodel/utility.py` & `mmodel-0.6.2/mmodel/utility.py`

 * *Files identical despite different names*

### Comparing `mmodel-0.6.1/pyproject.toml` & `mmodel-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "mmodel"
-version = "0.6.1"
+version = "0.6.2"
 description = "Modular modeling framework for scientific modeling and prototyping."
 readme = "README.rst"
 license = "BSD-3-Clause"
 authors = ["Peter Sun <hs859@cornell.edu>"]
 maintainers = ["Peter Sun <hs859@cornell.edu>"]
 repository = "https://github.com/peterhs73/MModel"
 packages = [{ include = "mmodel" }]
 homepage = "https://peterhs73.github.io/mmodel-docs/"
 documentation = "https://peterhs73.github.io/mmodel-docs/"
 keywords = ["python", "scientific-modeling", "prototyping"]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 
 [build-system]
```

### Comparing `mmodel-0.6.1/PKG-INFO` & `mmodel-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mmodel
-Version: 0.6.1
+Version: 0.6.2
 Summary: Modular modeling framework for scientific modeling and prototyping.
 Home-page: https://peterhs73.github.io/mmodel-docs/
 License: BSD-3-Clause
 Keywords: python,scientific-modeling,prototyping
 Author: Peter Sun
 Author-email: hs859@cornell.edu
 Maintainer: Peter Sun
 Maintainer-email: hs859@cornell.edu
 Requires-Python: >=3.8
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -44,14 +44,19 @@
 |Docs|
 
 MModel is a lightweight and modular model-building framework
 for small-scale and nonlinear models. The package aims to solve
 scientific program prototyping and distribution difficulties, making
 it easier to create modular, fast, and user-friendly packages.
 
+For using mmodel in a complex scientific workflow, please refer to
+the `mrfmsim <https://marohn-group.github.io/mrfmsim-docs/overview.html>`__
+on how mmodel improves the development of magnetic resonance force
+microscopy (MRFM) experiments.
+
 Quickstart
 ----------
 
 To create a nonlinear model that has the result of
 `(x + y)log(x + y, base)`:
 
 .. code-block:: python
```

