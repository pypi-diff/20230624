# Comparing `tmp/backports.pdb-2.0.1.tar.gz` & `tmp/backports.pdb-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmps3bj54z3/tmpomg70z5b/backports.pdb-2.0.1.tar", last modified: Fri Nov 27 18:29:04 2020, max compression
+gzip compressed data, was "backports.pdb-2.2.0.tar", last modified: Sat Jun 24 01:53:31 2023, max compression
```

## Comparing `backports.pdb-2.0.1.tar` & `backports.pdb-2.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-27 18:29:04.398989 backports.pdb-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)       50 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (116)      246 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-27 18:29:04.398989 backports.pdb-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-27 18:29:04.398989 backports.pdb-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1040 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (116)      175 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       79 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      404 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1050 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1763 2020-11-27 18:29:04.398989 backports.pdb-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      962 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-27 18:29:04.398989 backports.pdb-2.0.1/backports/
--rw-r--r--   0 runner    (1001) docker     (116)       81 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/backports/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    62693 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/backports/pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-27 18:29:04.398989 backports.pdb-2.0.1/backports.pdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1763 2020-11-27 18:29:04.000000 backports.pdb-2.0.1/backports.pdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      472 2020-11-27 18:29:04.000000 backports.pdb-2.0.1/backports.pdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-27 18:29:04.000000 backports.pdb-2.0.1/backports.pdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      236 2020-11-27 18:29:04.000000 backports.pdb-2.0.1/backports.pdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2020-11-27 18:29:04.000000 backports.pdb-2.0.1/backports.pdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-27 18:29:04.398989 backports.pdb-2.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      756 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       81 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (116)      296 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       37 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (116)      457 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      333 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (116)      964 2020-11-27 18:29:04.402989 backports.pdb-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       92 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     8511 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/skeleton.md
--rw-r--r--   0 runner    (1001) docker     (116)      798 2020-11-27 18:28:47.000000 backports.pdb-2.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:53:31.566483 backports.pdb-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:53:31.566483 backports.pdb-2.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:53:31.566483 backports.pdb-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-24 01:53:31.566483 backports.pdb-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:53:31.566483 backports.pdb-2.2.0/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/backports/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68099 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/backports/pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:53:31.566483 backports.pdb-2.2.0/backports.pdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-24 01:53:31.000000 backports.pdb-2.2.0/backports.pdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-24 01:53:31.000000 backports.pdb-2.2.0/backports.pdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 01:53:31.000000 backports.pdb-2.2.0/backports.pdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-24 01:53:31.000000 backports.pdb-2.2.0/backports.pdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-24 01:53:31.000000 backports.pdb-2.2.0/backports.pdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:53:31.566483 backports.pdb-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-24 01:53:31.566483 backports.pdb-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-24 01:53:11.000000 backports.pdb-2.2.0/tox.ini
```

### Comparing `backports.pdb-2.0.1/LICENSE` & `backports.pdb-2.2.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `backports.pdb-2.0.1/PKG-INFO` & `backports.pdb-2.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 Metadata-Version: 2.1
 Name: backports.pdb
-Version: 2.0.1
+Version: 2.2.0
 Summary: Backport of pdb from Python 3.7
 Home-page: https://github.com/jaraco/backports.pdb
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/backports.pdb.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/backports.pdb.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/backports.pdb
-        
-        .. image:: https://github.com/jaraco/backports.pdb/workflows/Automated%20Tests/badge.svg
-           :target: https://github.com/jaraco/backports.pdb/actions?query=workflow%3A%22Automated+Tests%22
-           :alt: Automated Tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-        ..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
-        
-        
-        Backport of `pdb <https://docs.python.org/3/library/pdb.html>`_ from
-        later Python versions to older ones::
-        
-            from backports import pdb
-        
-        Including support for the ``-m`` option::
-        
-            $ python -m backports.pdb -m mymodule
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/backports.pdb.svg
+   :target: https://pypi.org/project/backports.pdb
+
+.. image:: https://img.shields.io/pypi/pyversions/backports.pdb.svg
+
+.. image:: https://github.com/jaraco/backports.pdb/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/backports.pdb/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: Black
+
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
+
+Backport of `pdb <https://docs.python.org/3/library/pdb.html>`_ from
+later Python versions to older ones::
+
+    from backports import pdb
+
+Including support for the ``-m`` option::
+
+    $ python -m backports.pdb -m mymodule
```

### Comparing `backports.pdb-2.0.1/README.rst` & `backports.pdb-2.2.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 .. image:: https://img.shields.io/pypi/v/backports.pdb.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/backports.pdb
 
 .. image:: https://img.shields.io/pypi/pyversions/backports.pdb.svg
-   :target: `PyPI link`_
 
-.. _PyPI link: https://pypi.org/project/backports.pdb
-
-.. image:: https://github.com/jaraco/backports.pdb/workflows/Automated%20Tests/badge.svg
-   :target: https://github.com/jaraco/backports.pdb/actions?query=workflow%3A%22Automated+Tests%22
-   :alt: Automated Tests
+.. image:: https://github.com/jaraco/backports.pdb/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/backports.pdb/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
 
 Backport of `pdb <https://docs.python.org/3/library/pdb.html>`_ from
 later Python versions to older ones::
 
     from backports import pdb
 
 Including support for the ``-m`` option::
```

### Comparing `backports.pdb-2.0.1/backports/pdb.py` & `backports.pdb-2.2.0/backports/pdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,17 +76,20 @@
 import dis
 import code
 import glob
 import pprint
 import signal
 import inspect
 import tokenize
+import functools
 import traceback
 import linecache
 
+from typing import Union
+
 
 class Restart(Exception):
     """Causes a debugger to be restarted for the debugged python program."""
     pass
 
 __all__ = ["run", "pm", "Pdb", "runeval", "runctx", "runcall", "set_trace",
            "post_mortem", "help"]
@@ -100,23 +103,14 @@
     # consumer of this info expects the first line to be 1
     with fp:
         for lineno, line in enumerate(fp, start=1):
             if cre.match(line):
                 return funcname, filename, lineno
     return None
 
-def getsourcelines(obj):
-    lines, lineno = inspect.findsource(obj)
-    if inspect.isframe(obj) and obj.f_globals is obj.f_locals:
-        # must be a module frame: do not try to cut a block out of it
-        return lines, 1
-    elif inspect.ismodule(obj):
-        return lines, 1
-    return inspect.getblock(lines[lineno:]), lineno+1
-
 def lasti2lineno(code, lasti):
     linestarts = list(dis.findlinestarts(code))
     linestarts.reverse()
     for i, lineno in linestarts:
         if lasti >= i:
             return lineno
     return 0
@@ -124,14 +118,89 @@
 
 class _rstr(str):
     """String that doesn't quote its repr."""
     def __repr__(self):
         return self
 
 
+class _ScriptTarget(str):
+    def __new__(cls, val):
+        # Mutate self to be the "real path".
+        res = super().__new__(cls, os.path.realpath(val))
+
+        # Store the original path for error reporting.
+        res.orig = val
+
+        return res
+
+    def check(self):
+        if not os.path.exists(self):
+            print('Error:', self.orig, 'does not exist')
+            sys.exit(1)
+
+        # Replace pdb's dir with script's dir in front of module search path.
+        sys.path[0] = os.path.dirname(self)
+
+    @property
+    def filename(self):
+        return self
+
+    @property
+    def namespace(self):
+        return dict(
+            __name__='__main__',
+            __file__=self,
+            __builtins__=__builtins__,
+        )
+
+    @property
+    def code(self):
+        with io.open_code(self) as fp:
+            return f"exec(compile({fp.read()!r}, {self!r}, 'exec'))"
+
+
+class _ModuleTarget(str):
+    def check(self):
+        try:
+            self._details
+        except Exception:
+            traceback.print_exc()
+            sys.exit(1)
+
+    @functools.cached_property
+    def _details(self):
+        import runpy
+        return runpy._get_module_details(self)
+
+    @property
+    def filename(self):
+        return self.code.co_filename
+
+    @property
+    def code(self):
+        name, spec, code = self._details
+        return code
+
+    @property
+    def _spec(self):
+        name, spec, code = self._details
+        return spec
+
+    @property
+    def namespace(self):
+        return dict(
+            __name__='__main__',
+            __file__=os.path.normcase(os.path.abspath(self.filename)),
+            __package__=self._spec.parent,
+            __loader__=self._spec.loader,
+            __spec__=self._spec,
+            __builtins__=__builtins__,
+        )
+
+
 # Interaction prompt line will separate file and call info from code
 # text using value of line_prefix string.  A newline and arrow may
 # be to your liking.  You can set it once pdb is imported using the
 # command "pdb.line_prefix = '\n% '".
 # line_prefix = ': '    # Use this to get the old situation back
 line_prefix = '\n-> '   # Probably a better default
 
@@ -162,20 +231,20 @@
         self.allow_kbdint = False
         self.nosigint = nosigint
 
         # Read ~/.pdbrc and ./.pdbrc
         self.rcLines = []
         if readrc:
             try:
-                with open(os.path.expanduser('~/.pdbrc')) as rcFile:
+                with open(os.path.expanduser('~/.pdbrc'), encoding='utf-8') as rcFile:
                     self.rcLines.extend(rcFile)
             except OSError:
                 pass
             try:
-                with open(".pdbrc") as rcFile:
+                with open(".pdbrc", encoding='utf-8') as rcFile:
                     self.rcLines.extend(rcFile)
             except OSError:
                 pass
 
         self.commands = {} # associates a command list to breakpoint numbers
         self.commands_doprompt = {} # for each bp num, tells if the prompt
                                     # must be disp. after execing the cmd list
@@ -197,14 +266,16 @@
         bdb.Bdb.reset(self)
         self.forget()
 
     def forget(self):
         self.lineno = None
         self.stack = []
         self.curindex = 0
+        if hasattr(self, 'curframe') and self.curframe:
+            self.curframe.f_globals.pop('__pdb_convenience_variables', None)
         self.curframe = None
         self.tb_lineno.clear()
 
     def setup(self, f, tb):
         self.forget()
         self.stack, self.curindex = self.get_stack(f, tb)
         while tb:
@@ -215,14 +286,15 @@
             self.tb_lineno[tb.tb_frame] = lineno
             tb = tb.tb_next
         self.curframe = self.stack[self.curindex][0]
         # The f_locals dictionary is updated from the actual frame
         # locals whenever the .f_locals accessor is called, so we
         # cache it here to ensure that modifications are not overwritten.
         self.curframe_locals = self.curframe.f_locals
+        self.set_convenience_variable(self.curframe, '_frame', self.curframe)
         return self.execRcLines()
 
     # Can be executed earlier than 'setup' if desired
     def execRcLines(self):
         if not self.rcLines:
             return
         # local copy because of recursion
@@ -286,34 +358,35 @@
         return 1
 
     def user_return(self, frame, return_value):
         """This function is called when a return trap is set here."""
         if self._wait_for_mainpyfile:
             return
         frame.f_locals['__return__'] = return_value
+        self.set_convenience_variable(frame, '_retval', return_value)
         self.message('--Return--')
         self.interaction(frame, None)
 
     def user_exception(self, frame, exc_info):
         """This function is called if an exception occurs,
         but only if we are to stop at or just below this level."""
         if self._wait_for_mainpyfile:
             return
         exc_type, exc_value, exc_traceback = exc_info
         frame.f_locals['__exception__'] = exc_type, exc_value
+        self.set_convenience_variable(frame, '_exception', exc_value)
 
         # An 'Internal StopIteration' exception is an exception debug event
         # issued by the interpreter when handling a subgenerator run with
         # 'yield from' or a generator controlled by a for loop. No exception has
         # actually occurred in this case. The debugger uses this debug event to
         # stop when the debuggee is returning from such generators.
         prefix = 'Internal ' if (not exc_traceback
                                     and exc_type is StopIteration) else ''
-        self.message('%s%s' % (prefix,
-            traceback.format_exception_only(exc_type, exc_value)[-1].strip()))
+        self.message('%s%s' % (prefix, self._format_exc(exc_value)))
         self.interaction(frame, exc_traceback)
 
     # General interaction function
     def _cmdloop(self):
         while True:
             try:
                 # keyboard interrupts allow for an easy way to cancel
@@ -322,14 +395,15 @@
                 self.cmdloop()
                 self.allow_kbdint = False
                 break
             except KeyboardInterrupt:
                 self.message('--KeyboardInterrupt--')
 
     # Called before loop, handles display expressions
+    # Set up convenience variable containers
     def preloop(self):
         displaying = self.displaying.get(self.curframe)
         if displaying:
             for expr, oldvalue in displaying.items():
                 newvalue = self._getval_except(expr)
                 # check for identity first; this prevents custom __eq__ to
                 # be called at every loop, and also prevents instances whose
@@ -362,15 +436,15 @@
         assignment of the _ variable in the builtins.
         """
         # reproduce the behavior of the standard displayhook, not printing None
         if obj is not None:
             self.message(repr(obj))
 
     def default(self, line):
-        if line[:1] == '!': line = line[1:]
+        if line[:1] == '!': line = line[1:].strip()
         locals = self.curframe_locals
         globals = self.curframe.f_globals
         try:
             code = compile(line + '\n', '<stdin>', 'single')
             save_stdout = sys.stdout
             save_stdin = sys.stdin
             save_displayhook = sys.displayhook
@@ -380,16 +454,15 @@
                 sys.displayhook = self.displayhook
                 exec(code, globals, locals)
             finally:
                 sys.stdout = save_stdout
                 sys.stdin = save_stdin
                 sys.displayhook = save_displayhook
         except:
-            exc_info = sys.exc_info()[:2]
-            self.error(traceback.format_exception_only(*exc_info)[-1].strip())
+            self._error_exc()
 
     def precmd(self, line):
         """Handle alias expansion and ';;' separator."""
         if not line.strip():
             return line
         args = line.split()
         while args[0] in self.aliases:
@@ -406,14 +479,17 @@
         if args[0] != 'alias':
             marker = line.find(';;')
             if marker >= 0:
                 # queue up everything after marker
                 next = line[marker+2:].lstrip()
                 self.cmdqueue.append(next)
                 line = line[:marker].rstrip()
+
+        # Replace all the convenience variables
+        line = re.sub(r'\$([a-zA-Z_][a-zA-Z0-9_]*)', r'__pdb_convenience_variables["\1"]', line)
         return line
 
     def onecmd(self, line):
         """Interpret the argument as though it had been typed in response
         to the prompt.
 
         Checks whether this line is typed at the normal prompt or in
@@ -456,14 +532,21 @@
 
     def message(self, msg):
         print(msg, file=self.stdout)
 
     def error(self, msg):
         print('***', msg, file=self.stdout)
 
+    # convenience variables
+
+    def set_convenience_variable(self, frame, name, value):
+        if '__pdb_convenience_variables' not in frame.f_globals:
+            frame.f_globals['__pdb_convenience_variables'] = {}
+        frame.f_globals['__pdb_convenience_variables'][name] = value
+
     # Generic completion functions.  Individual complete_foo methods can be
     # assigned below to one of these functions.
 
     def _complete_location(self, text, line, begidx, endidx):
         # Complete a file/module/function location for break/tbreak/clear.
         if line.strip().endswith((':', ',')):
             # Here comes a line number or a condition which we can't complete.
@@ -515,15 +598,15 @@
             return [n for n in ns.keys() if n.startswith(text)]
 
     # Command definitions, called by cmdloop()
     # The argument is the remaining string on the command line
     # Return true to exit from the command loop
 
     def do_commands(self, arg):
-        """commands [bpnumber]
+        """(Pdb) commands [bpnumber]
         (com) ...
         (com) end
         (Pdb)
 
         Specify a list of commands for breakpoint number bpnumber.
         The commands themselves are entered on the following lines.
         Type a line containing just 'end' to terminate the commands.
@@ -559,14 +642,20 @@
             bnum = len(bdb.Breakpoint.bpbynumber) - 1
         else:
             try:
                 bnum = int(arg)
             except:
                 self.error("Usage: commands [bnum]\n        ...\n        end")
                 return
+        try:
+            self.get_bpbynumber(bnum)
+        except ValueError as err:
+            self.error('cannot set commands: %s' % err)
+            return
+
         self.commands_bnum = bnum
         # Save old definitions for the case of a keyboard interrupt.
         if bnum in self.commands:
             old_command_defs = (self.commands[bnum],
                                 self.commands_doprompt[bnum],
                                 self.commands_silent[bnum])
         else:
@@ -595,14 +684,15 @@
             self.commands_defining = False
             self.prompt = prompt_back
 
     complete_commands = _complete_bpnumber
 
     def do_break(self, arg, temporary = 0):
         """b(reak) [ ([filename:]lineno | function) [, condition] ]
+
         Without argument, list all breaks.
 
         With a line number argument, set a break at this line in the
         current file.  With a function name, set a break at the first
         executable line of that function.  If a second argument is
         present, it is a string specifying an expression which must
         evaluate to true before the breakpoint is honored.
@@ -624,14 +714,17 @@
         filename = None
         lineno = None
         cond = None
         comma = arg.find(',')
         if comma > 0:
             # parse stuff after comma: "condition"
             cond = arg[comma+1:].lstrip()
+            if err := self._compile_error_message(cond):
+                self.error('Invalid condition %s: %r' % (cond, err))
+                return
             arg = arg[:comma].rstrip()
         # parse stuff before comma: [filename:]lineno | function
         colon = arg.rfind(':')
         funcname = None
         if colon >= 0:
             filename = arg[:colon].rstrip()
             f = self.lookupmodule(filename)
@@ -700,14 +793,15 @@
     do_b = do_break
 
     complete_break = _complete_location
     complete_b = _complete_location
 
     def do_tbreak(self, arg):
         """tbreak [ ([filename:]lineno | function) [, condition] ]
+
         Same arguments as break, but sets a temporary breakpoint: it
         is automatically deleted when first hit.
         """
         self.do_break(arg, 1)
 
     complete_tbreak = _complete_location
 
@@ -748,29 +842,31 @@
         """Check whether specified line seems to be executable.
 
         Return `lineno` if it is, 0 if not (e.g. a docstring, comment, blank
         line or EOF). Warning: testing is not comprehensive.
         """
         # this method should be callable before starting debugging, so default
         # to "no globals" if there is no current frame
-        globs = self.curframe.f_globals if hasattr(self, 'curframe') else None
+        frame = getattr(self, 'curframe', None)
+        globs = frame.f_globals if frame else None
         line = linecache.getline(filename, lineno, globs)
         if not line:
             self.message('End of file')
             return 0
         line = line.strip()
         # Don't allow setting breakpoint at a blank line
         if (not line or (line[0] == '#') or
              (line[:3] == '"""') or line[:3] == "'''"):
             self.error('Blank or comment')
             return 0
         return lineno
 
     def do_enable(self, arg):
         """enable bpnumber [bpnumber ...]
+
         Enables the breakpoints given as a space separated list of
         breakpoint numbers.
         """
         args = arg.split()
         for i in args:
             try:
                 bp = self.get_bpbynumber(i)
@@ -780,14 +876,15 @@
                 bp.enable()
                 self.message('Enabled %s' % bp)
 
     complete_enable = _complete_bpnumber
 
     def do_disable(self, arg):
         """disable bpnumber [bpnumber ...]
+
         Disables the breakpoints given as a space separated list of
         breakpoint numbers.  Disabling a breakpoint means it cannot
         cause the program to stop execution, but unlike clearing a
         breakpoint, it remains in the list of breakpoints and can be
         (re-)enabled.
         """
         args = arg.split()
@@ -800,22 +897,26 @@
                 bp.disable()
                 self.message('Disabled %s' % bp)
 
     complete_disable = _complete_bpnumber
 
     def do_condition(self, arg):
         """condition bpnumber [condition]
+
         Set a new condition for the breakpoint, an expression which
         must evaluate to true before the breakpoint is honored.  If
         condition is absent, any existing condition is removed; i.e.,
         the breakpoint is made unconditional.
         """
         args = arg.split(' ', 1)
         try:
             cond = args[1]
+            if err := self._compile_error_message(cond):
+                self.error('Invalid condition %s: %r' % (cond, err))
+                return
         except IndexError:
             cond = None
         try:
             bp = self.get_bpbynumber(args[0].strip())
         except IndexError:
             self.error('Breakpoint number expected')
         except ValueError as err:
@@ -827,14 +928,15 @@
             else:
                 self.message('New condition set for breakpoint %d.' % bp.number)
 
     complete_condition = _complete_bpnumber
 
     def do_ignore(self, arg):
         """ignore bpnumber [count]
+
         Set the ignore count for the given breakpoint number.  If
         count is omitted, the ignore count is set to 0.  A breakpoint
         becomes active when the ignore count is zero.  When non-zero,
         the count is decremented each time the breakpoint is reached
         and the breakpoint is not disabled and any associated
         condition evaluates to true.
         """
@@ -861,15 +963,16 @@
             else:
                 self.message('Will stop next time breakpoint %d is reached.'
                              % bp.number)
 
     complete_ignore = _complete_bpnumber
 
     def do_clear(self, arg):
-        """cl(ear) filename:lineno\ncl(ear) [bpnumber [bpnumber...]]
+        """cl(ear) [filename:lineno | bpnumber ...]
+
         With a space separated list of breakpoint numbers, clear
         those breakpoints.  Without argument, clear all breaks (but
         first ask confirmation).  With a filename:lineno argument,
         clear all breaks at that line in that file.
         """
         if not arg:
             try:
@@ -889,15 +992,15 @@
             filename = arg[:i]
             arg = arg[i+1:]
             try:
                 lineno = int(arg)
             except ValueError:
                 err = "Invalid line number (%s)" % arg
             else:
-                bplist = self.get_breaks(filename, lineno)
+                bplist = self.get_breaks(filename, lineno)[:]
                 err = self.clear_break(filename, lineno)
             if err:
                 self.error(err)
             else:
                 for bp in bplist:
                     self.message('Deleted %s' % bp)
             return
@@ -913,32 +1016,35 @@
     do_cl = do_clear # 'c' is already an abbreviation for 'continue'
 
     complete_clear = _complete_location
     complete_cl = _complete_location
 
     def do_where(self, arg):
         """w(here)
+
         Print a stack trace, with the most recent frame at the bottom.
         An arrow indicates the "current frame", which determines the
         context of most commands.  'bt' is an alias for this command.
         """
         self.print_stack_trace()
     do_w = do_where
     do_bt = do_where
 
     def _select_frame(self, number):
         assert 0 <= number < len(self.stack)
         self.curindex = number
         self.curframe = self.stack[self.curindex][0]
         self.curframe_locals = self.curframe.f_locals
+        self.set_convenience_variable(self.curframe, '_frame', self.curframe)
         self.print_stack_entry(self.stack[self.curindex])
         self.lineno = None
 
     def do_up(self, arg):
         """u(p) [count]
+
         Move the current frame count (default one) levels up in the
         stack trace (to an older frame).
         """
         if self.curindex == 0:
             self.error('Oldest frame')
             return
         try:
@@ -951,14 +1057,15 @@
         else:
             newframe = max(0, self.curindex - count)
         self._select_frame(newframe)
     do_u = do_up
 
     def do_down(self, arg):
         """d(own) [count]
+
         Move the current frame count (default one) levels down in the
         stack trace (to a newer frame).
         """
         if self.curindex + 1 == len(self.stack):
             self.error('Newest frame')
             return
         try:
@@ -971,14 +1078,15 @@
         else:
             newframe = min(len(self.stack) - 1, self.curindex + count)
         self._select_frame(newframe)
     do_d = do_down
 
     def do_until(self, arg):
         """unt(il) [lineno]
+
         Without argument, continue execution until the line with a
         number greater than the current one is reached.  With a line
         number, continue execution until a line with a number greater
         or equal to that is reached.  In both cases, also stop when
         the current frame returns.
         """
         if arg:
@@ -995,58 +1103,67 @@
             lineno = None
         self.set_until(self.curframe, lineno)
         return 1
     do_unt = do_until
 
     def do_step(self, arg):
         """s(tep)
+
         Execute the current line, stop at the first possible occasion
         (either in a function that is called or in the current
         function).
         """
         self.set_step()
         return 1
     do_s = do_step
 
     def do_next(self, arg):
         """n(ext)
+
         Continue execution until the next line in the current function
         is reached or it returns.
         """
         self.set_next(self.curframe)
         return 1
     do_n = do_next
 
     def do_run(self, arg):
         """run [args...]
+
         Restart the debugged python program. If a string is supplied
         it is split with "shlex", and the result is used as the new
         sys.argv.  History, breakpoints, actions and debugger options
         are preserved.  "restart" is an alias for "run".
         """
         if arg:
             import shlex
             argv0 = sys.argv[0:1]
-            sys.argv = shlex.split(arg)
+            try:
+                sys.argv = shlex.split(arg)
+            except ValueError as e:
+                self.error('Cannot run %s: %s' % (arg, e))
+                return
             sys.argv[:0] = argv0
         # this is caught in the main debugger loop
         raise Restart
 
     do_restart = do_run
 
     def do_return(self, arg):
         """r(eturn)
+
         Continue execution until the current function returns.
         """
         self.set_return(self.curframe)
         return 1
     do_r = do_return
 
     def do_continue(self, arg):
         """c(ont(inue))
+
         Continue execution, only stop when a breakpoint is encountered.
         """
         if not self.nosigint:
             try:
                 Pdb._previous_sigint_handler = \
                     signal.signal(signal.SIGINT, self.sigint_handler)
             except ValueError:
@@ -1057,14 +1174,15 @@
                 pass
         self.set_continue()
         return 1
     do_c = do_cont = do_continue
 
     def do_jump(self, arg):
         """j(ump) lineno
+
         Set the next line that will be executed.  Only available in
         the bottom-most frame.  This lets you jump back and execute
         code again, or jump forward to skip code that you don't want
         to run.
 
         It should be noted that not all jumps are allowed -- for
         instance it is not possible to jump into the middle of a
@@ -1086,57 +1204,60 @@
                 self.print_stack_entry(self.stack[self.curindex])
             except ValueError as e:
                 self.error('Jump failed: %s' % e)
     do_j = do_jump
 
     def do_debug(self, arg):
         """debug code
+
         Enter a recursive debugger that steps through the code
         argument (which is an arbitrary expression or statement to be
         executed in the current environment).
         """
         sys.settrace(None)
         globals = self.curframe.f_globals
         locals = self.curframe_locals
         p = Pdb(self.completekey, self.stdin, self.stdout)
         p.prompt = "(%s) " % self.prompt.strip()
         self.message("ENTERING RECURSIVE DEBUGGER")
         try:
             sys.call_tracing(p.run, (arg, globals, locals))
         except Exception:
-            exc_info = sys.exc_info()[:2]
-            self.error(traceback.format_exception_only(*exc_info)[-1].strip())
+            self._error_exc()
         self.message("LEAVING RECURSIVE DEBUGGER")
         sys.settrace(self.trace_dispatch)
         self.lastcmd = p.lastcmd
 
     complete_debug = _complete_expression
 
     def do_quit(self, arg):
-        """q(uit)\nexit
+        """q(uit) | exit
+
         Quit from the debugger. The program being executed is aborted.
         """
         self._user_requested_quit = True
         self.set_quit()
         return 1
 
     do_q = do_quit
     do_exit = do_quit
 
     def do_EOF(self, arg):
         """EOF
+
         Handles the receipt of EOF as a command.
         """
         self.message('')
         self._user_requested_quit = True
         self.set_quit()
         return 1
 
     def do_args(self, arg):
         """a(rgs)
+
         Print the argument list of the current function.
         """
         co = self.curframe.f_code
         dict = self.curframe_locals
         n = co.co_argcount + co.co_kwonlyargcount
         if co.co_flags & inspect.CO_VARARGS: n = n+1
         if co.co_flags & inspect.CO_VARKEYWORDS: n = n+1
@@ -1146,65 +1267,73 @@
                 self.message('%s = %r' % (name, dict[name]))
             else:
                 self.message('%s = *** undefined ***' % (name,))
     do_a = do_args
 
     def do_retval(self, arg):
         """retval
+
         Print the return value for the last return of a function.
         """
         if '__return__' in self.curframe_locals:
             self.message(repr(self.curframe_locals['__return__']))
         else:
             self.error('Not yet returned!')
     do_rv = do_retval
 
     def _getval(self, arg):
         try:
             return eval(arg, self.curframe.f_globals, self.curframe_locals)
         except:
-            exc_info = sys.exc_info()[:2]
-            self.error(traceback.format_exception_only(*exc_info)[-1].strip())
+            self._error_exc()
             raise
 
     def _getval_except(self, arg, frame=None):
         try:
             if frame is None:
                 return eval(arg, self.curframe.f_globals, self.curframe_locals)
             else:
                 return eval(arg, frame.f_globals, frame.f_locals)
+        except BaseException as exc:
+            return _rstr('** raised %s **' % self._format_exc(exc))
+
+    def _error_exc(self):
+        exc = sys.exception()
+        self.error(self._format_exc(exc))
+
+    def _msg_val_func(self, arg, func):
+        try:
+            val = self._getval(arg)
+        except:
+            return  # _getval() has displayed the error
+        try:
+            self.message(func(val))
         except:
-            exc_info = sys.exc_info()[:2]
-            err = traceback.format_exception_only(*exc_info)[-1].strip()
-            return _rstr('** raised %s **' % err)
+            self._error_exc()
 
     def do_p(self, arg):
         """p expression
+
         Print the value of the expression.
         """
-        try:
-            self.message(repr(self._getval(arg)))
-        except:
-            pass
+        self._msg_val_func(arg, repr)
 
     def do_pp(self, arg):
         """pp expression
+
         Pretty-print the value of the expression.
         """
-        try:
-            self.message(pprint.pformat(self._getval(arg)))
-        except:
-            pass
+        self._msg_val_func(arg, pprint.pformat)
 
     complete_print = _complete_expression
     complete_p = _complete_expression
     complete_pp = _complete_expression
 
     def do_list(self, arg):
-        """l(ist) [first [,last] | .]
+        """l(ist) [first[, last] | .]
 
         List source code for the current file.  Without arguments,
         list 11 lines around the current line or continue the previous
         listing.  With . as argument, list 11 lines around the current
         line.  With one argument, list 11 lines starting at that line.
         With two arguments, list the given range; if the second
         argument is less than the first, it is a count.
@@ -1234,50 +1363,58 @@
         elif self.lineno is None or arg == '.':
             first = max(1, self.curframe.f_lineno - 5)
         else:
             first = self.lineno + 1
         if last is None:
             last = first + 10
         filename = self.curframe.f_code.co_filename
+        # gh-93696: stdlib frozen modules provide a useful __file__
+        # this workaround can be removed with the closure of gh-89815
+        if filename.startswith("<frozen"):
+            tmp = self.curframe.f_globals.get("__file__")
+            if isinstance(tmp, str):
+                filename = tmp
         breaklist = self.get_file_breaks(filename)
         try:
             lines = linecache.getlines(filename, self.curframe.f_globals)
             self._print_lines(lines[first-1:last], first, breaklist,
                               self.curframe)
             self.lineno = min(last, len(lines))
             if len(lines) < last:
                 self.message('[EOF]')
         except KeyboardInterrupt:
             pass
     do_l = do_list
 
     def do_longlist(self, arg):
-        """longlist | ll
+        """ll | longlist
+
         List the whole source code for the current function or frame.
         """
         filename = self.curframe.f_code.co_filename
         breaklist = self.get_file_breaks(filename)
         try:
-            lines, lineno = getsourcelines(self.curframe)
+            lines, lineno = self._getsourcelines(self.curframe)
         except OSError as err:
             self.error(err)
             return
         self._print_lines(lines, lineno, breaklist, self.curframe)
     do_ll = do_longlist
 
     def do_source(self, arg):
         """source expression
+
         Try to get source code for the given object and display it.
         """
         try:
             obj = self._getval(arg)
         except:
             return
         try:
-            lines, lineno = getsourcelines(obj)
+            lines, lineno = self._getsourcelines(obj)
         except (OSError, TypeError) as err:
             self.error(err)
             return
         self._print_lines(lines, lineno)
 
     complete_source = _complete_expression
 
@@ -1299,15 +1436,16 @@
             if lineno == current_lineno:
                 s += '->'
             elif lineno == exc_lineno:
                 s += '>>'
             self.message(s + '\t' + line.rstrip())
 
     def do_whatis(self, arg):
-        """whatis arg
+        """whatis expression
+
         Print the type of the argument.
         """
         try:
             value = self._getval(arg)
         except:
             # _getval() already printed the error
             return
@@ -1342,21 +1480,27 @@
 
         Display the value of the expression if it changed, each time execution
         stops in the current frame.
 
         Without expression, list all display expressions for the current frame.
         """
         if not arg:
-            self.message('Currently displaying:')
-            for item in self.displaying.get(self.curframe, {}).items():
-                self.message('%s: %r' % item)
-        else:
-            val = self._getval_except(arg)
-            self.displaying.setdefault(self.curframe, {})[arg] = val
-            self.message('display %s: %r' % (arg, val))
+            if self.displaying:
+                self.message('Currently displaying:')
+                for item in self.displaying.get(self.curframe, {}).items():
+                    self.message('%s: %r' % item)
+            else:
+                self.message('No expression is being displayed')
+        else:
+            if err := self._compile_error_message(arg):
+                self.error('Unable to display %s: %r' % (arg, err))
+            else:
+                val = self._getval_except(arg)
+                self.displaying.setdefault(self.curframe, {})[arg] = val
+                self.message('display %s: %r' % (arg, val))
 
     complete_display = _complete_expression
 
     def do_undisplay(self, arg):
         """undisplay [expression]
 
         Do not display the expression any more in the current frame.
@@ -1381,15 +1525,16 @@
         Start an interactive interpreter whose global namespace
         contains all the (global and local) names found in the current scope.
         """
         ns = {**self.curframe.f_globals, **self.curframe_locals}
         code.interact("*interactive*", local=ns)
 
     def do_alias(self, arg):
-        """alias [name [command [parameter parameter ...] ]]
+        """alias [name [command]]
+
         Create an alias called 'name' that executes 'command'.  The
         command must *not* be enclosed in quotes.  Replaceable
         parameters can be indicated by %1, %2, and so on, while %* is
         replaced by all the parameters.  If no command is given, the
         current alias for name is shown. If no name is given, all
         aliases are listed.
 
@@ -1417,14 +1562,15 @@
         if args[0] in self.aliases and len(args) == 1:
             self.message("%s = %s" % (args[0], self.aliases[args[0]]))
         else:
             self.aliases[args[0]] = ' '.join(args[1:])
 
     def do_unalias(self, arg):
         """unalias name
+
         Delete the specified alias.
         """
         args = arg.split()
         if len(args) == 0: return
         if args[0] in self.aliases:
             del self.aliases[args[0]]
 
@@ -1459,14 +1605,15 @@
         self.message(prefix +
                      self.format_stack_entry(frame_lineno, prompt_prefix))
 
     # Provide help
 
     def do_help(self, arg):
         """h(elp)
+
         Without argument, print the list of available commands.
         With a command name as argument, print help about that command.
         "help pdb" shows the full pdb documentation.
         "help exec" gives help on the ! command.
         """
         if not arg:
             return cmd.Cmd.do_help(self, arg)
@@ -1479,25 +1626,32 @@
         except AttributeError:
             self.error('No help for %r' % arg)
         else:
             if sys.flags.optimize >= 2:
                 self.error('No help for %r; please do not run Python with -OO '
                            'if you need command help' % arg)
                 return
-            self.message(command.__doc__.rstrip())
+            if command.__doc__ is None:
+                self.error('No help for %r; __doc__ string missing' % arg)
+                return
+            self.message(self._help_message_from_doc(command.__doc__))
 
     do_h = do_help
 
     def help_exec(self):
         """(!) statement
+
         Execute the (one-line) statement in the context of the current
         stack frame.  The exclamation point can be omitted unless the
-        first word of the statement resembles a debugger command.  To
-        assign to a global variable you must always prefix the command
-        with a 'global' command, e.g.:
+        first word of the statement resembles a debugger command, e.g.:
+        (Pdb) ! n=42
+        (Pdb)
+
+        To assign to a global variable you must always prefix the command with
+        a 'global' command, e.g.:
         (Pdb) global list_options; list_options = ['-l']
         (Pdb)
         """
         self.message((self.help_exec.__doc__ or '').strip())
 
     def help_pdb(self):
         help()
@@ -1524,57 +1678,74 @@
             while os.path.islink(dirname):
                 dirname = os.readlink(dirname)
             fullname = os.path.join(dirname, filename)
             if os.path.exists(fullname):
                 return fullname
         return None
 
-    def _runmodule(self, module_name):
+    def _run(self, target: Union[_ModuleTarget, _ScriptTarget]):
+        # When bdb sets tracing, a number of call and line events happen
+        # BEFORE debugger even reaches user's code (and the exact sequence of
+        # events depends on python version). Take special measures to
+        # avoid stopping before reaching the main script (see user_line and
+        # user_call for details).
         self._wait_for_mainpyfile = True
         self._user_requested_quit = False
-        import runpy
-        mod_name, mod_spec, code = runpy._get_module_details(module_name)
-        self.mainpyfile = self.canonic(code.co_filename)
-        import __main__
-        __main__.__dict__.clear()
-        __main__.__dict__.update({
-            "__name__": "__main__",
-            "__file__": self.mainpyfile,
-            "__package__": mod_spec.parent,
-            "__loader__": mod_spec.loader,
-            "__spec__": mod_spec,
-            "__builtins__": __builtins__,
-        })
-        self.run(code)
-
-    def _runscript(self, filename):
-        # The script has to run in __main__ namespace (or imports from
-        # __main__ will break).
-        #
-        # So we clear up the __main__ and set several special variables
-        # (this gets rid of pdb's globals and cleans old variables on restarts).
+
+        self.mainpyfile = self.canonic(target.filename)
+
+        # The target has to run in __main__ namespace (or imports from
+        # __main__ will break). Clear __main__ and replace with
+        # the target namespace.
         import __main__
         __main__.__dict__.clear()
-        __main__.__dict__.update({"__name__"    : "__main__",
-                                  "__file__"    : filename,
-                                  "__builtins__": __builtins__,
-                                 })
+        __main__.__dict__.update(target.namespace)
 
-        # When bdb sets tracing, a number of call and line events happens
-        # BEFORE debugger even reaches user's code (and the exact sequence of
-        # events depends on python version). So we take special measures to
-        # avoid stopping before we reach the main script (see user_line and
-        # user_call for details).
-        self._wait_for_mainpyfile = True
-        self.mainpyfile = self.canonic(filename)
-        self._user_requested_quit = False
-        with io.open_code(filename) as fp:
-            statement = "exec(compile(%r, %r, 'exec'))" % \
-                        (fp.read(), self.mainpyfile)
-        self.run(statement)
+        self.run(target.code)
+
+    def _format_exc(self, exc: BaseException):
+        return traceback.format_exception_only(exc)[-1].strip()
+
+    def _compile_error_message(self, expr):
+        """Return the error message as string if compiling `expr` fails."""
+        try:
+            compile(expr, "<stdin>", "eval")
+        except SyntaxError as exc:
+            return _rstr(self._format_exc(exc))
+        return ""
+
+    def _getsourcelines(self, obj):
+        # GH-103319
+        # inspect.getsourcelines() returns lineno = 0 for
+        # module-level frame which breaks our code print line number
+        # This method should be replaced by inspect.getsourcelines(obj)
+        # once this bug is fixed in inspect
+        lines, lineno = inspect.getsourcelines(obj)
+        lineno = max(1, lineno)
+        return lines, lineno
+
+    def _help_message_from_doc(self, doc):
+        lines = [line.strip() for line in doc.rstrip().splitlines()]
+        if not lines:
+            return "No help message found."
+        if "" in lines:
+            usage_end = lines.index("")
+        else:
+            usage_end = 1
+        formatted = []
+        indent = " " * len(self.prompt)
+        for i, line in enumerate(lines):
+            if i == 0:
+                prefix = "Usage: "
+            elif i < usage_end:
+                prefix = "       "
+            else:
+                prefix = ""
+            formatted.append(indent + prefix + line)
+        return "\n".join(formatted)
 
 # Collect all command help into docstring, if not run with -OO
 
 if __doc__ is not None:
     # unfortunately we can't guess this order from the class definition
     _help_order = [
         'help', 'where', 'down', 'up', 'break', 'tbreak', 'clear', 'disable',
@@ -1590,50 +1761,94 @@
 
     del _help_order, _command
 
 
 # Simplified interface
 
 def run(statement, globals=None, locals=None):
+    """Execute the *statement* (given as a string or a code object)
+    under debugger control.
+
+    The debugger prompt appears before any code is executed; you can set
+    breakpoints and type continue, or you can step through the statement
+    using step or next.
+
+    The optional *globals* and *locals* arguments specify the
+    environment in which the code is executed; by default the
+    dictionary of the module __main__ is used (see the explanation of
+    the built-in exec() or eval() functions.).
+    """
     Pdb().run(statement, globals, locals)
 
 def runeval(expression, globals=None, locals=None):
+    """Evaluate the *expression* (given as a string or a code object)
+    under debugger control.
+
+    When runeval() returns, it returns the value of the expression.
+    Otherwise this function is similar to run().
+    """
     return Pdb().runeval(expression, globals, locals)
 
 def runctx(statement, globals, locals):
     # B/W compatibility
     run(statement, globals, locals)
 
 def runcall(*args, **kwds):
+    """Call the function (a function or method object, not a string)
+    with the given arguments.
+
+    When runcall() returns, it returns whatever the function call
+    returned. The debugger prompt appears as soon as the function is
+    entered.
+    """
     return Pdb().runcall(*args, **kwds)
 
 def set_trace(*, header=None):
+    """Enter the debugger at the calling stack frame.
+
+    This is useful to hard-code a breakpoint at a given point in a
+    program, even if the code is not otherwise being debugged (e.g. when
+    an assertion fails). If given, *header* is printed to the console
+    just before debugging begins.
+    """
     pdb = Pdb()
     if header is not None:
         pdb.message(header)
     pdb.set_trace(sys._getframe().f_back)
 
 # Post-Mortem interface
 
 def post_mortem(t=None):
+    """Enter post-mortem debugging of the given *traceback* object.
+
+    If no traceback is given, it uses the one of the exception that is
+    currently being handled (an exception must be being handled if the
+    default is to be used).
+    """
     # handling the default
     if t is None:
-        # sys.exc_info() returns (type, value, traceback) if an exception is
-        # being handled, otherwise it returns None
-        t = sys.exc_info()[2]
+        exc = sys.exception()
+        if exc is not None:
+            t = exc.__traceback__
+
     if t is None:
         raise ValueError("A valid traceback must be passed if no "
                          "exception is being handled")
 
     p = Pdb()
     p.reset()
     p.interaction(None, t)
 
 def pm():
-    post_mortem(sys.last_traceback)
+    """Enter post-mortem debugging of the traceback found in sys.last_traceback."""
+    if hasattr(sys, 'last_exc'):
+        tb = sys.last_exc.__traceback__
+    else:
+        tb = sys.last_traceback
+    post_mortem(tb)
 
 
 # Main program for testing
 
 TESTCMD = 'import x; x.main()'
 
 def test():
@@ -1655,77 +1870,67 @@
 and in the current directory, if they exist.  Commands supplied with
 -c are executed after commands from .pdbrc files.
 
 To let the script run until an exception occurs, use "-c continue".
 To let the script run up to a given line X in the debugged file, use
 "-c 'until X'"."""
 
+
 def main():
     import getopt
 
     opts, args = getopt.getopt(sys.argv[1:], 'mhc:', ['help', 'command='])
 
     if not args:
         print(_usage)
         sys.exit(2)
 
-    commands = []
-    run_as_module = False
-    for opt, optarg in opts:
-        if opt in ['-h', '--help']:
-            print(_usage)
-            sys.exit()
-        elif opt in ['-c', '--command']:
-            commands.append(optarg)
-        elif opt in ['-m']:
-            run_as_module = True
-
-    mainpyfile = args[0]     # Get script filename
-    if not run_as_module and not os.path.exists(mainpyfile):
-        print('Error:', mainpyfile, 'does not exist')
-        sys.exit(1)
+    if any(opt in ['-h', '--help'] for opt, optarg in opts):
+        print(_usage)
+        sys.exit()
 
-    sys.argv[:] = args      # Hide "pdb.py" and pdb options from argument list
+    commands = [optarg for opt, optarg in opts if opt in ['-c', '--command']]
+
+    module_indicated = any(opt in ['-m'] for opt, optarg in opts)
+    cls = _ModuleTarget if module_indicated else _ScriptTarget
+    target = cls(args[0])
+
+    target.check()
 
-    # Replace pdb's dir with script's dir in front of module search path.
-    if not run_as_module:
-        sys.path[0] = os.path.dirname(mainpyfile)
+    sys.argv[:] = args      # Hide "pdb.py" and pdb options from argument list
 
     # Note on saving/restoring sys.argv: it's a good idea when sys.argv was
     # modified by the script being debugged. It's a bad idea when it was
     # changed by the user from the command line. There is a "restart" command
     # which allows explicit specification of command line arguments.
     pdb = Pdb()
     pdb.rcLines.extend(commands)
     while True:
         try:
-            if run_as_module:
-                pdb._runmodule(mainpyfile)
-            else:
-                pdb._runscript(mainpyfile)
+            pdb._run(target)
             if pdb._user_requested_quit:
                 break
             print("The program finished and will be restarted")
         except Restart:
-            print("Restarting", mainpyfile, "with arguments:")
-            print("\t" + " ".join(args))
-        except SystemExit:
+            print("Restarting", target, "with arguments:")
+            print("\t" + " ".join(sys.argv[1:]))
+        except SystemExit as e:
             # In most cases SystemExit does not warrant a post-mortem session.
             print("The program exited via sys.exit(). Exit status:", end=' ')
-            print(sys.exc_info()[1])
+            print(e)
         except SyntaxError:
             traceback.print_exc()
             sys.exit(1)
-        except:
+        except BaseException as e:
             traceback.print_exc()
             print("Uncaught exception. Entering post mortem debugging")
             print("Running 'cont' or 'step' will restart the program")
-            t = sys.exc_info()[2]
+            t = e.__traceback__
             pdb.interaction(None, t)
-            print("Post mortem debugger finished. The " + mainpyfile +
+            print("Post mortem debugger finished. The " + target +
                   " will be restarted")
 
 
 # When invoked as main program, invoke the debugger on a script
 if __name__ == '__main__':
-    from backports import pdb
+    import pdb
     pdb.main()
```

### Comparing `backports.pdb-2.0.1/backports.pdb.egg-info/PKG-INFO` & `backports.pdb-2.2.0/backports.pdb.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 Metadata-Version: 2.1
 Name: backports.pdb
-Version: 2.0.1
+Version: 2.2.0
 Summary: Backport of pdb from Python 3.7
 Home-page: https://github.com/jaraco/backports.pdb
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/backports.pdb.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/backports.pdb.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/backports.pdb
-        
-        .. image:: https://github.com/jaraco/backports.pdb/workflows/Automated%20Tests/badge.svg
-           :target: https://github.com/jaraco/backports.pdb/actions?query=workflow%3A%22Automated+Tests%22
-           :alt: Automated Tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-        ..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
-        
-        
-        Backport of `pdb <https://docs.python.org/3/library/pdb.html>`_ from
-        later Python versions to older ones::
-        
-            from backports import pdb
-        
-        Including support for the ``-m`` option::
-        
-            $ python -m backports.pdb -m mymodule
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/backports.pdb.svg
+   :target: https://pypi.org/project/backports.pdb
+
+.. image:: https://img.shields.io/pypi/pyversions/backports.pdb.svg
+
+.. image:: https://github.com/jaraco/backports.pdb/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/backports.pdb/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: Black
+
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
+
+Backport of `pdb <https://docs.python.org/3/library/pdb.html>`_ from
+later Python versions to older ones::
+
+    from backports import pdb
+
+Including support for the ``-m`` option::
+
+    $ python -m backports.pdb -m mymodule
```

### Comparing `backports.pdb-2.0.1/docs/conf.py` & `backports.pdb-2.2.0/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
                 pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
-                url='https://www.python.org/dev/peps/pep-{pep_number:0>4}/',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
+
+# Be strict about any broken references
+nitpicky = True
+
+# Include Python intersphinx mapping to prevent failures
+# jaraco/skeleton#51
+extensions += ['sphinx.ext.intersphinx']
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+}
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `backports.pdb-2.0.1/setup.cfg` & `backports.pdb-2.2.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 [metadata]
-license_file = LICENSE
 name = backports.pdb
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
 description = Backport of pdb from Python 3.7
 long_description = file:README.rst
 url = https://github.com/jaraco/backports.pdb
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-packages = find:
+packages = find_namespace:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
-setup_requires = setuptools_scm[toml] >= 3.4.1
+
+[options.packages.find]
+exclude = 
+	build*
+	dist*
+	docs*
+	tests*
 
 [options.extras_require]
 testing = 
-	pytest >= 3.5, !=3.7.3
-	pytest-checkdocs >= 1.2.3
-	pytest-flake8
-	pytest-black >= 0.3.7; python_implementation != "PyPy"
+	pytest >= 6
+	pytest-checkdocs >= 2.4
+	pytest-black >= 0.3.7; \
+	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy; python_implementation != "PyPy"
-	jaraco.test >= 3.2.0
+	pytest-mypy >= 0.9.1; \
+	python_implementation != "PyPy"
+	pytest-enabler >= 1.3
+	pytest-ruff
 docs = 
-	sphinx
-	jaraco.packaging >= 3.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

