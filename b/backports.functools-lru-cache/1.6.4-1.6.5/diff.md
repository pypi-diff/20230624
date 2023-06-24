# Comparing `tmp/backports.functools_lru_cache-1.6.4.tar.gz` & `tmp/backports.functools_lru_cache-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backports.functools_lru_cache-1.6.4.tar", last modified: Sun Apr 11 19:31:32 2021, max compression
+gzip compressed data, was "backports.functools_lru_cache-1.6.5.tar", last modified: Sat Jun 24 00:50:52 2023, max compression
```

## Comparing `backports.functools_lru_cache-1.6.4.tar` & `backports.functools_lru_cache-1.6.5.tar`

### file list

```diff
@@ -1,40 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:31:32.244775 backports.functools_lru_cache-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:31:32.240775 backports.functools_lru_cache-1.6.4/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:31:32.240775 backports.functools_lru_cache-1.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/.github/workflows/automerge.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      793 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      825 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2021-04-11 19:31:32.244775 backports.functools_lru_cache-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:31:32.240775 backports.functools_lru_cache-1.6.4/backports/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7239 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/backports/functools_lru_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:31:32.240775 backports.functools_lru_cache-1.6.4/backports.functools_lru_cache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2021-04-11 19:31:32.000000 backports.functools_lru_cache-1.6.4/backports.functools_lru_cache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      695 2021-04-11 19:31:32.000000 backports.functools_lru_cache-1.6.4/backports.functools_lru_cache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-11 19:31:32.000000 backports.functools_lru_cache-1.6.4/backports.functools_lru_cache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      386 2021-04-11 19:31:32.000000 backports.functools_lru_cache-1.6.4/backports.functools_lru_cache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-04-11 19:31:32.000000 backports.functools_lru_cache-1.6.4/backports.functools_lru_cache.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:31:32.240775 backports.functools_lru_cache-1.6.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:31:32.240775 backports.functools_lru_cache-1.6.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/docs/_templates/tidelift-sidebar.html
--rw-r--r--   0 runner    (1001) docker     (121)      934 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      313 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-04-11 19:31:32.244775 backports.functools_lru_cache-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10139 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/skeleton.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 19:31:32.244775 backports.functools_lru_cache-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/tests/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2021-04-11 19:31:07.000000 backports.functools_lru_cache-1.6.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.427822 backports.functools_lru_cache-1.6.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.427822 backports.functools_lru_cache-1.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.427822 backports.functools_lru_cache-1.6.5/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/backports/functools_lru_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-24 00:50:52.000000 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-24 00:50:52.000000 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 00:50:52.000000 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-24 00:50:52.000000 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-24 00:50:52.000000 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/tests/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/tox.ini
```

### Comparing `backports.functools_lru_cache-1.6.4/.gitignore` & `backports.functools_lru_cache-1.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `backports.functools_lru_cache-1.6.4/CHANGES.rst` & `backports.functools_lru_cache-1.6.5/NEWS.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v1.6.5
+======
+
+No significant changes.
+
+
 v1.6.4
 ======
 
 #16: For test dependencies, when indicating Python 3, use ``>=3``
 instead of ``>3`` to satisfy
 `python-poetry/poetry#3862 <https://github.com/python-poetry/poetry/issues/3862>`_.
```

### Comparing `backports.functools_lru_cache-1.6.4/LICENSE` & `backports.functools_lru_cache-1.6.5/LICENSE`

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

### Comparing `backports.functools_lru_cache-1.6.4/PKG-INFO` & `backports.functools_lru_cache-1.6.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 Metadata-Version: 2.1
 Name: backports.functools_lru_cache
-Version: 1.6.4
+Version: 1.6.5
 Summary: Backport of functools.lru_cache
 Home-page: https://github.com/jaraco/backports.functools_lru_cache
 Author: Raymond Hettinger
 Author-email: raymond.hettinger@gmail.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/backports.functools_lru_cache.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/backports.functools_lru_cache.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/backports.functools_lru_cache
-        
-        .. image:: https://github.com/jaraco/backports.functools_lru_cache/workflows/tests/badge.svg
-           :target: https://github.com/jaraco/backports.functools_lru_cache/actions?query=workflow%3A%22tests%22
-           :alt: tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. image:: https://readthedocs.org/projects/backportsfunctools_lru_cache/badge/?version=latest
-           :target: https://backportsfunctools_lru_cache.readthedocs.io/en/latest/?badge=latest
-        
-        .. image:: https://tidelift.com/badges/package/pypi/backports.functools_lru_cache
-           :target: https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=readme
-        
-        Backport of functools.lru_cache from Python 3.3 as published at `ActiveState
-        <http://code.activestate.com/recipes/578078/>`_.
-        
-        Usage
-        =====
-        
-        Consider using this technique for importing the 'lru_cache' function::
-        
-            try:
-                from functools import lru_cache
-            except ImportError:
-                from backports.functools_lru_cache import lru_cache
-        
-        
-        For Enterprise
-        ==============
-        
-        Available as part of the Tidelift Subscription.
-        
-        This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
-        
-        `Learn more <https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=referral&utm_campaign=github>`_.
-        
-        Security Contact
-        ================
-        
-        To report a security vulnerability, please use the
-        `Tidelift security contact <https://tidelift.com/security>`_.
-        Tidelift will coordinate the fix and disclosure.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=2.6
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/backports.functools_lru_cache.svg
+   :target: https://pypi.org/project/backports.functools_lru_cache
+
+.. image:: https://img.shields.io/pypi/pyversions/backports.functools_lru_cache.svg
+
+.. image:: https://github.com/jaraco/backports.functools_lru_cache/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/backports.functools_lru_cache/actions?query=workflow%3A%22tests%22
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
+.. image:: https://readthedocs.org/projects/backportsfunctools_lru_cache/badge/?version=latest
+   :target: https://backportsfunctools_lru_cache.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
+
+.. image:: https://tidelift.com/badges/package/pypi/backports.functools_lru_cache
+   :target: https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=readme
+
+Backport of functools.lru_cache from Python 3.3 as published at `ActiveState
+<http://code.activestate.com/recipes/578078/>`_.
+
+Usage
+=====
+
+Consider using this technique for importing the 'lru_cache' function::
+
+    try:
+        from functools import lru_cache
+    except ImportError:
+        from backports.functools_lru_cache import lru_cache
+
+
+For Enterprise
+==============
+
+Available as part of the Tidelift Subscription.
+
+This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
+
+`Learn more <https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=referral&utm_campaign=github>`_.
+
+Security Contact
+================
+
+To report a security vulnerability, please use the
+`Tidelift security contact <https://tidelift.com/security>`_.
+Tidelift will coordinate the fix and disclosure.
```

### Comparing `backports.functools_lru_cache-1.6.4/README.rst` & `backports.functools_lru_cache-1.6.5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 .. image:: https://img.shields.io/pypi/v/backports.functools_lru_cache.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/backports.functools_lru_cache
 
 .. image:: https://img.shields.io/pypi/pyversions/backports.functools_lru_cache.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/backports.functools_lru_cache
 
 .. image:: https://github.com/jaraco/backports.functools_lru_cache/workflows/tests/badge.svg
    :target: https://github.com/jaraco/backports.functools_lru_cache/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/backportsfunctools_lru_cache/badge/?version=latest
    :target: https://backportsfunctools_lru_cache.readthedocs.io/en/latest/?badge=latest
 
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
+
 .. image:: https://tidelift.com/badges/package/pypi/backports.functools_lru_cache
    :target: https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=readme
 
 Backport of functools.lru_cache from Python 3.3 as published at `ActiveState
 <http://code.activestate.com/recipes/578078/>`_.
 
 Usage
```

### Comparing `backports.functools_lru_cache-1.6.4/backports/functools_lru_cache.py` & `backports.functools_lru_cache-1.6.5/backports/functools_lru_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
 
     # Users should only access the lru_cache through its public API:
     #       cache_info, cache_clear, and f.__wrapped__
     # The internals of the lru_cache are encapsulated for thread safety and
     # to allow the implementation to change (including a possible C version).
 
     def decorating_function(user_function):
-
         cache = dict()
         stats = [0, 0]  # make statistics updateable non-locally
         HITS, MISSES = 0, 1  # names for the stats fields
         make_key = _make_key
         cache_get = cache.get  # bound method to lookup key or return None
         _len = len  # localize the global len() function
         lock = RLock()  # because linkedlist updates aren't threadsafe
```

### Comparing `backports.functools_lru_cache-1.6.4/backports.functools_lru_cache.egg-info/PKG-INFO` & `backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 Metadata-Version: 2.1
 Name: backports.functools-lru-cache
-Version: 1.6.4
+Version: 1.6.5
 Summary: Backport of functools.lru_cache
 Home-page: https://github.com/jaraco/backports.functools_lru_cache
 Author: Raymond Hettinger
 Author-email: raymond.hettinger@gmail.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/backports.functools_lru_cache.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/backports.functools_lru_cache.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/backports.functools_lru_cache
-        
-        .. image:: https://github.com/jaraco/backports.functools_lru_cache/workflows/tests/badge.svg
-           :target: https://github.com/jaraco/backports.functools_lru_cache/actions?query=workflow%3A%22tests%22
-           :alt: tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. image:: https://readthedocs.org/projects/backportsfunctools_lru_cache/badge/?version=latest
-           :target: https://backportsfunctools_lru_cache.readthedocs.io/en/latest/?badge=latest
-        
-        .. image:: https://tidelift.com/badges/package/pypi/backports.functools_lru_cache
-           :target: https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=readme
-        
-        Backport of functools.lru_cache from Python 3.3 as published at `ActiveState
-        <http://code.activestate.com/recipes/578078/>`_.
-        
-        Usage
-        =====
-        
-        Consider using this technique for importing the 'lru_cache' function::
-        
-            try:
-                from functools import lru_cache
-            except ImportError:
-                from backports.functools_lru_cache import lru_cache
-        
-        
-        For Enterprise
-        ==============
-        
-        Available as part of the Tidelift Subscription.
-        
-        This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
-        
-        `Learn more <https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=referral&utm_campaign=github>`_.
-        
-        Security Contact
-        ================
-        
-        To report a security vulnerability, please use the
-        `Tidelift security contact <https://tidelift.com/security>`_.
-        Tidelift will coordinate the fix and disclosure.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=2.6
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+.. image:: https://img.shields.io/pypi/v/backports.functools_lru_cache.svg
+   :target: https://pypi.org/project/backports.functools_lru_cache
+
+.. image:: https://img.shields.io/pypi/pyversions/backports.functools_lru_cache.svg
+
+.. image:: https://github.com/jaraco/backports.functools_lru_cache/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/backports.functools_lru_cache/actions?query=workflow%3A%22tests%22
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
+.. image:: https://readthedocs.org/projects/backportsfunctools_lru_cache/badge/?version=latest
+   :target: https://backportsfunctools_lru_cache.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
+
+.. image:: https://tidelift.com/badges/package/pypi/backports.functools_lru_cache
+   :target: https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=readme
+
+Backport of functools.lru_cache from Python 3.3 as published at `ActiveState
+<http://code.activestate.com/recipes/578078/>`_.
+
+Usage
+=====
+
+Consider using this technique for importing the 'lru_cache' function::
+
+    try:
+        from functools import lru_cache
+    except ImportError:
+        from backports.functools_lru_cache import lru_cache
+
+
+For Enterprise
+==============
+
+Available as part of the Tidelift Subscription.
+
+This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
+
+`Learn more <https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=referral&utm_campaign=github>`_.
+
+Security Contact
+================
+
+To report a security vulnerability, please use the
+`Tidelift security contact <https://tidelift.com/security>`_.
+Tidelift will coordinate the fix and disclosure.
```

### Comparing `backports.functools_lru_cache-1.6.4/backports.functools_lru_cache.egg-info/SOURCES.txt` & `backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 .coveragerc
 .editorconfig
-.flake8
 .gitignore
 .pre-commit-config.yaml
-.readthedocs.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
-setup.py
-skeleton.md
+towncrier.toml
 tox.ini
 .github/FUNDING.yml
-.github/workflows/automerge.yml
+.github/dependabot.yml
 .github/workflows/main.yml
 backports/__init__.py
 backports/functools_lru_cache.py
 backports.functools_lru_cache.egg-info/PKG-INFO
 backports.functools_lru_cache.egg-info/SOURCES.txt
 backports.functools_lru_cache.egg-info/dependency_links.txt
 backports.functools_lru_cache.egg-info/requires.txt
 backports.functools_lru_cache.egg-info/top_level.txt
 docs/conf.py
 docs/history.rst
 docs/index.rst
-docs/_templates/tidelift-sidebar.html
 tests/test_lru_cache.py
```

### Comparing `backports.functools_lru_cache-1.6.4/setup.cfg` & `backports.functools_lru_cache-1.6.5/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 [metadata]
-license_files = 
-	LICENSE
 name = backports.functools_lru_cache
 author = Raymond Hettinger
 author_email = raymond.hettinger@gmail.com
 maintainer = Jason R. Coombs
 maintainer_email = jaraco@jaraco.com
 description = Backport of functools.lru_cache
 long_description = file:README.rst
@@ -18,36 +16,41 @@
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 include_package_data = true
 python_requires = >=2.6
 install_requires = 
-setup_requires = setuptools_scm[toml] >= 3.4.1
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
-	pytest >= 4.6
-	pytest-checkdocs >= 2.4; python_version >= "3.6"
-	pytest-flake8; python_version >= "3"
-	pytest-black >= 0.3.7; python_implementation != "PyPy" and python_version < "3.10" and python_version >= "3"
-	pytest-cov; python_version >= "3"
-	pytest-mypy; python_implementation != "PyPy" and python_version < "3.10" and python_version >= "3"
-	pytest-enabler >= 1.0.1; python_version >= "3.0"
+	pytest >= 6
+	pytest-checkdocs >= 2.4
+	pytest-black >= 0.3.7; \
+	python_implementation != "PyPy"
+	pytest-cov
+	pytest-mypy >= 0.9.1; \
+	python_implementation != "PyPy"
+	pytest-enabler >= 1.3
+	pytest-ruff
 docs = 
-	sphinx
-	jaraco.packaging >= 8.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
+	
+	jaraco.tidelift >= 1.4
 
 [options.entry_points]
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
```

