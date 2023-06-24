# Comparing `tmp/pandas-indexing-0.2.7.tar.gz` & `tmp/pandas-indexing-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.2.7.tar", last modified: Fri May 26 20:05:07 2023, max compression
+gzip compressed data, was "pandas-indexing-0.2.8.tar", last modified: Sat Jun 24 12:01:24 2023, max compression
```

## Comparing `pandas-indexing-0.2.7.tar` & `pandas-indexing-0.2.8.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.290772 pandas-indexing-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-26 20:05:07.290772 pandas-indexing-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.282772 pandas-indexing-0.2.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.282772 pandas-indexing-0.2.7/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   362791 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/notebooks/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:05:07.290772 pandas-indexing-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.278771 pandas-indexing-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.286772 pandas-indexing-0.2.7/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.290772 pandas-indexing-0.2.7/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-26 20:04:46.000000 pandas-indexing-0.2.7/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:05:07.290772 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-26 20:05:07.000000 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-26 20:05:07.000000 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:05:07.000000 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-26 20:05:07.000000 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 20:05:07.000000 pandas-indexing-0.2.7/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.914776 pandas-indexing-0.2.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/AUTHORS.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.914776 pandas-indexing-0.2.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.914776 pandas-indexing-0.2.8/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   362710 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.914776 pandas-indexing-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-24 12:01:24.000000 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-24 12:01:24.000000 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 12:01:24.000000 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-24 12:01:24.000000 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-24 12:01:24.000000 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.2.7/CODE_OF_CONDUCT.md` & `pandas-indexing-0.2.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.7/CONTRIBUTING.rst` & `pandas-indexing-0.2.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.7/LICENSE` & `pandas-indexing-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.7/PKG-INFO` & `pandas-indexing-0.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.7
+Version: 0.2.8
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
@@ -23,14 +23,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: units
 Provides-Extra: lint
 License-File: LICENSE
 
 pandas-indexing helper
 ======================
 
 .. image:: https://github.com/coroa/pandas-indexing/workflows/ci/badge.svg?branch=main
```

### Comparing `pandas-indexing-0.2.7/README.rst` & `pandas-indexing-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.7/docs/api.rst` & `pandas-indexing-0.2.8/docs/api.rst`

 * *Files 4% similar despite different names*

```diff
@@ -30,7 +30,14 @@
 
 
 selectors
 =========
 
 .. automodule:: pandas_indexing.selectors
     :members:
+
+
+units
+=====
+
+.. automodule:: pandas_indexing.units
+    :members:
```

### Comparing `pandas-indexing-0.2.7/docs/conf.py` & `pandas-indexing-0.2.8/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "sphinx.ext.extlinks",
     "sphinx.ext.autosectionlabel",
     # "sphinx.ext.ifconfig",
     "sphinx.ext.napoleon",
     "sphinx.ext.intersphinx",
     # "sphinx.ext.todo",
     # "sphinx.ext.viewcode",
-    "nbsphinx",
+    "myst_nb",
 ]
 
 if os.getenv("SPELLCHECK"):
     extensions += ("sphinxcontrib.spelling",)
     spelling_show_suggestions = True
     spelling_lang = "en_US"
     # https://sphinxcontrib-spelling.readthedocs.io/en/latest/customize.html
@@ -71,15 +71,15 @@
 linkcheck_ignore = [
     "https://codecov.io/gh/coroa/pandas-indexing/*",
 ]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ["html"]
+exclude_patterns = ["html", "jupyter_execute"]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # -- Options for HTML output -------------------------------------------------
 
 html_theme = "sphinx_rtd_theme"
@@ -89,14 +89,17 @@
     "display_github": False,
     "github_user": "coroa",
     "github_repo": "pandas-indexing",
     "github_version": "main",
     "conf_py_path": "/docs/source",
 }
 
+html_static_path = ["_static"]
+html_css_files = ["custom.css"]
+
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for coverage extension ------------------------------------------
 coverage_write_headline = False  # do not write headlines.
 
 # -- Options for autodoc extension -------------------------------------------
```

### Comparing `pandas-indexing-0.2.7/docs/notebooks/introduction.ipynb` & `pandas-indexing-0.2.8/docs/notebooks/introduction.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998915139826422%*

 * *Differences: {"'cells'": "{23: {'source': {insert: [(0, '````{warning}\\n'), (9, '````')], delete: [14, 13, 5, "*

 * *            '3, 2, 1, 0]}}}'}*

```diff
@@ -2241,29 +2241,24 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "7e1d4f00",
             "metadata": {},
             "source": [
-                "<div class=\"alert alert-warning\">\n",
-                "\n",
-                "WARNING\n",
-                "\n",
+                "````{warning}\n",
                 "It is currently impossible to use a pandas boolean series **in front of** a selector; ie.\n",
-                "\n",
                 "```python\n",
                 "(capacity[2030] > 250) & isin(variable=[\"Coal\", \"Gas\", \"Nuclear\"], unit=\"GW\")\n",
                 "```\n",
                 "will **fail**, it needs to be\n",
                 "```python\n",
                 "isin(variable=[\"Coal\", \"Gas\", \"Nuclear\"], unit=\"GW\") & (capacity[2030] > 250)\n",
                 "```\n",
-                "\n",
-                "</div>"
+                "````"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "id": "8b421dba",
             "metadata": {},
```

### Comparing `pandas-indexing-0.2.7/pyproject.toml` & `pandas-indexing-0.2.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -50,25 +50,30 @@
 
 [project.optional-dependencies]
 # Add dependencies for building docs and running tests
 docs = [
     "sphinx>=2.2",
     "sphinx-argparse",
     "sphinx-rtd-theme",
-    "nbsphinx",
+    "myst_nb",
     "ipython",
 ]
 
 test = [
     "coverage",
     "pytest",
     "pytest-cov",
     "hypothesis",
 ]
 
+units = [
+    "pint>=0.21",
+    "openscm-units",
+]
+
 lint = [
     "black",
     "ruff",
 ]
 
 [project.scripts]
```

### Comparing `pandas-indexing-0.2.7/src/pandas_indexing/__init__.py` & `pandas-indexing-0.2.8/src/pandas_indexing/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     formatlevel,
     index_names,
     projectlevel,
     semijoin,
     uniquelevel,
 )
 from .selectors import isin, ismatch
+from .units import convert_unit, dequantify, quantify, set_openscm_registry_as_default
 
 
 try:
     __version__ = _version("pandas-indexing")
 except Exception:
     # Local copy or not installed with setuptools.
     # Disable minimum version checks on downstream libraries.
```

### Comparing `pandas-indexing-0.2.7/src/pandas_indexing/accessors.py` & `pandas-indexing-0.2.8/src/pandas_indexing/accessors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Registers convenience accessors into the ``idx`` namespace of each pandas
 object.
 
-Usage
------
+Examples
+--------
 >>> df.idx.project(["model", "scenario"])
 
 >>> df.index.idx.assign(unit="Mt CO2")
 
 >>> df.idx.multiply(other, how="left")
 """
 
-from typing import Any, Literal, Optional, Sequence, Union
+from typing import Any, Callable, Literal, Mapping, Optional, Sequence, Union
 
 import pandas as pd
 from pandas import DataFrame, Index, MultiIndex, Series
 
 from . import arithmetics
 from .core import (
     assignlevel,
@@ -25,14 +25,15 @@
     isna,
     notna,
     projectlevel,
     semijoin,
     uniquelevel,
 )
 from .types import Axis, Data
+from .units import convert_unit, dequantify, quantify
 from .utils import doc
 
 
 class _IdxAccessor:
     """
     Convenience accessor for accessing `pandas-indexing` functions.
     """
@@ -130,14 +131,41 @@
 
     def add(self, other, **align_kwds):
         return arithmetics.add(self._obj, other, **align_kwds)
 
     def subtract(self, other, **align_kwds):
         return arithmetics.subtract(self._obj, other, **align_kwds)
 
+    @doc(quantify, data="", example_call="s.idx.quantify()")
+    def quantify(
+        self,
+        level: str = "unit",
+        unit: Optional[str] = None,
+        axis: Axis = 0,
+        copy: bool = False,
+    ):
+        return quantify(self._obj, level=level, unit=unit, axis=axis, copy=copy)
+
+    def dequantify(self, level: str = "unit", axis: Axis = 0, copy: bool = False):
+        return dequantify(self._obj, level=level, axis=axis, copy=copy)
+
+    @doc(
+        convert_unit,
+        data="",
+        convert_unit_s_km='s.idx.convert_unit("km")',
+        convert_unit_s_m_to_km='s.idx.convert_unit({"m": "km"})',
+    )
+    def convert_unit(
+        self,
+        unit: Union[str, Mapping[str, str], Callable[[str], str]],
+        level: Optional[str] = "unit",
+        axis: Axis = 0,
+    ):
+        return convert_unit(self._obj, unit=unit, level=level, axis=axis)
+
 
 @pd.api.extensions.register_dataframe_accessor("idx")
 class DataFrameIdxAccessor(_DataIdxAccessor):
     pass
 
 
 @pd.api.extensions.register_series_accessor("idx")
```

### Comparing `pandas-indexing-0.2.7/src/pandas_indexing/arithmetics.py` & `pandas-indexing-0.2.8/src/pandas_indexing/arithmetics.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.7/src/pandas_indexing/core.py` & `pandas-indexing-0.2.8/src/pandas_indexing/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -225,15 +225,17 @@
             raise ValueError(
                 "All objects need to have the same index levels, but "
                 f"{set(orderset)} != {set(ax.names)}"
             )
 
         return df_or_ser.set_axis(ax.reorder_levels(order), axis=axis, copy=False)
 
-    return pd.concat([reorder(o) for o in objs], keys=keys, copy=copy, **concat_kwds)
+    return pd.concat(
+        [reorder(o) for o in objs], keys=keys, copy=copy, axis=axis, **concat_kwds
+    )
 
 
 def _notna(
     index: Index,
     subset: Optional[Sequence[str]] = None,
     how: Literal["any", "all"] = "any",
 ) -> np.ndarray:
@@ -487,57 +489,47 @@
         if frame_or_series does not derive from DataFrame or Series
 
     See also
     --------
     pandas.Index.join
     """
 
-    if isinstance(axis, str):
-        if axis == "index":
-            axis = 0
-        elif axis == "columns":
-            axis = 1
-        else:
-            raise ValueError(
-                f"axis can only be one of 0, 1, 'index' or 'columns', not: {axis}"
-            )
+    index = get_axis(frame_or_series, axis)
 
-    axes = frame_or_series.axes
-    index = axes[axis]
     if level is None:
         index = ensure_multiindex(index)
         other = ensure_multiindex(other)
 
     new_index, left_idx, _ = index.join(
         other, how=how, level=level, return_indexers=True, sort=sort
     )
 
-    cls = frame_or_series.__class__
-    axes[axis] = new_index
-
     if left_idx is None:
-        return cls(frame_or_series.values, *axes).__finalize__(frame_or_series)
+        return frame_or_series.set_axis(new_index, axis=axis)
 
+    any_missing = not (left_idx != -1).all()
     if isinstance(frame_or_series, DataFrame):
-        if axis == 0:
-            data = np.where(
-                left_idx[:, np.newaxis] != -1,
-                frame_or_series.values[left_idx, :],
-                np.nan,
-            )
-        elif axis == 1:
-            data = np.where(left_idx != -1, frame_or_series.values[:, left_idx], np.nan)
+        if axis in (0, "index"):
+            data = frame_or_series.iloc[left_idx]
+            index = data.index
+        elif axis in (1, "columns"):
+            data = frame_or_series.iloc[:, left_idx]
+            index = data.columns
+        if any_missing:
+            data = data.where(pd.Series(left_idx != -1, index), axis=axis)
     elif isinstance(frame_or_series, Series):
-        data = np.where(left_idx != -1, frame_or_series.values[left_idx], np.nan)
+        data = frame_or_series.iloc[left_idx]
+        if any_missing:
+            data = data.where(left_idx != -1)
     else:
         raise TypeError(
             f"frame_or_series must derive from DataFrame or Series, but is {type(frame_or_series)}"
         )
 
-    return cls(data, *axes).__finalize__(frame_or_series, method="semijoin")
+    return data.set_axis(new_index, axis=axis)
 
 
 def _extractlevel(
     index: Index, template: Optional[str] = None, drop: bool = False, **templates: str
 ) -> Tuple[Index, List[str]]:
     index = ensure_multiindex(index)
     all_identifiers = set()
@@ -585,16 +577,21 @@
     template: Optional[str] = None,
     *,
     drop: bool = False,
     dropna: bool = True,
     axis: Axis = 0,
     **templates: str,
 ) -> T:
-    """Split an index ``dim`` ension into multiple ones based on a
-    ``template``.
+    """Extract new index levels with ``templates`` matched against any index
+    level.
+
+    The ``**templates`` argument defines pairs of level names and templates.
+    Given level names are matched against the template, f.ex. ``"Emi|{{gas}}|{{sector}}"``.
+    Patterns (``{{gas}}`` or ``{{sector}}``) appearing in the template are extracted
+    from the successful matches and added as new levels.
 
     Parameters
     ----------\
     {index_or_data}
     template : str, optional
         Extraction template for a single level
     drop : bool, default False
@@ -612,14 +609,53 @@
 
     Raises
     ------
     ValueError
         If ``dim`` is not a dimension of ``index_or_series``
     ValueError
         If ``template`` is given, while index has more than one level
+
+    Examples
+    --------
+    >>> s = Series(
+    ...     range(3),
+    ...     MultiIndex.from_arrays(
+    ...         [["SE|Elec|Bio", "SE|Elec|Coal", "PE|Coal"], ["GWh", "GWh", "EJ"]],
+    ...         names=["variable", "unit"],
+    ...     ),
+    ... )
+    >>> s
+    variable      unit
+    SE|Elec|Bio   GWh     0
+    SE|Elec|Coal  GWh     1
+    PE|Coal       EJ      2
+    dtype: int64
+    >>> extractlevel(s, variable="SE|{{type}}|{{fuel}}")
+    variable      unit  type  fuel
+    SE|Elec|Bio   GWh   Elec  Bio     0
+    SE|Elec|Coal  GWh   Elec  Coal    1
+    dtype: int64
+
+    >>> extractlevel(s, variable="SE|{{type}}|{{fuel}}", dropna=False)
+    variable      unit  type  fuel
+    SE|Elec|Bio   GWh   Elec  Bio     0
+    SE|Elec|Coal  GWh   Elec  Coal    1
+    PE|Coal       EJ    NaN   NaN     2
+    dtype: int64
+
+    >>> s = Series(range(3), ["SE|Elec|Bio", "SE|Elec|Coal", "PE|Coal"])
+    >>> extractlevel(s, "SE|{{type}}|{{fuel}}", drop=True)
+    type  fuel
+    Elec  Bio     0
+          Coal    1
+    dtype: int64
+
+    See also
+    --------
+    formatlevel
     """
     if isinstance(index_or_data, Index):
         index_or_data, identifiers = _extractlevel(
             index_or_data, template, drop, **templates
         )
     else:
         index, identifiers = _extractlevel(
```

### Comparing `pandas-indexing-0.2.7/src/pandas_indexing/datasets/__init__.py` & `pandas-indexing-0.2.8/src/pandas_indexing/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.7/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas-indexing-0.2.8/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.7/src/pandas_indexing/selectors.py` & `pandas-indexing-0.2.8/src/pandas_indexing/selectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     if not filters and singlefilter is not None:
         filters = {None: singlefilter}
 
     if df is None:
         return Ismatch(
             filters, regex=regex, ignore_missing_levels=ignore_missing_levels
         )
-    elif not isinstance(df, (DataFrame, Series)):
+    elif not isinstance(df, (DataFrame, Series, Index)):
         # Special case: a pattern was passed in through `df` which wants to be applied to
         # hopefully a non-MultiIndex based Series or dataframe that we get afterwards
         filters = {None: df}
         return Ismatch(filters, regex=regex)
     else:
         return Ismatch(
             filters, regex=regex, ignore_missing_levels=ignore_missing_levels
```

### Comparing `pandas-indexing-0.2.7/src/pandas_indexing/utils.py` & `pandas-indexing-0.2.8/src/pandas_indexing/utils.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.7/src/pandas_indexing.egg-info/PKG-INFO` & `pandas-indexing-0.2.8/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.7
+Version: 0.2.8
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
@@ -23,14 +23,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: units
 Provides-Extra: lint
 License-File: LICENSE
 
 pandas-indexing helper
 ======================
 
 .. image:: https://github.com/coroa/pandas-indexing/workflows/ci/badge.svg?branch=main
```

### Comparing `pandas-indexing-0.2.7/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas-indexing-0.2.8/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
 docs/spelling_wordlist.txt
 docs/usage.rst
+docs/_static/custom.css
 docs/notebooks/introduction.ipynb
 src/pandas_indexing/__init__.py
 src/pandas_indexing/accessors.py
 src/pandas_indexing/arithmetics.py
 src/pandas_indexing/core.py
 src/pandas_indexing/selectors.py
 src/pandas_indexing/types.py
+src/pandas_indexing/units.py
 src/pandas_indexing/utils.py
 src/pandas_indexing.egg-info/PKG-INFO
 src/pandas_indexing.egg-info/SOURCES.txt
 src/pandas_indexing.egg-info/dependency_links.txt
 src/pandas_indexing.egg-info/requires.txt
 src/pandas_indexing.egg-info/top_level.txt
 src/pandas_indexing/datasets/__init__.py
```

