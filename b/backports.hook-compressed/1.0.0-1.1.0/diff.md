# Comparing `tmp/backports.hook_compressed-1.0.0.tar.gz` & `tmp/backports.hook_compressed-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backports.hook_compressed-1.0.0.tar", last modified: Tue May 25 02:50:41 2021, max compression
+gzip compressed data, was "backports.hook_compressed-1.1.0.tar", last modified: Sat Jun 24 01:33:00 2023, max compression
```

## Comparing `backports.hook_compressed-1.0.0.tar` & `backports.hook_compressed-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 02:50:41.164950 backports.hook_compressed-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 02:50:41.160950 backports.hook_compressed-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 02:50:41.160950 backports.hook_compressed-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2021-05-25 02:50:41.164950 backports.hook_compressed-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      878 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 02:50:41.160950 backports.hook_compressed-1.0.0/backports/
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/backports/hook_compressed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 02:50:41.164950 backports.hook_compressed-1.0.0/backports.hook_compressed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2021-05-25 02:50:41.000000 backports.hook_compressed-1.0.0/backports.hook_compressed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      535 2021-05-25 02:50:41.000000 backports.hook_compressed-1.0.0/backports.hook_compressed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-25 02:50:41.000000 backports.hook_compressed-1.0.0/backports.hook_compressed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      257 2021-05-25 02:50:41.000000 backports.hook_compressed-1.0.0/backports.hook_compressed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-05-25 02:50:41.000000 backports.hook_compressed-1.0.0/backports.hook_compressed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 02:50:41.164950 backports.hook_compressed-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      814 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      309 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2021-05-25 02:50:41.164950 backports.hook_compressed-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      723 2021-05-25 02:50:22.000000 backports.hook_compressed-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:33:00.642991 backports.hook_compressed-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:33:00.634991 backports.hook_compressed-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:33:00.634991 backports.hook_compressed-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-24 01:33:00.642991 backports.hook_compressed-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:33:00.638991 backports.hook_compressed-1.1.0/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/backports/hook_compressed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:33:00.638991 backports.hook_compressed-1.1.0/backports.hook_compressed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-24 01:33:00.000000 backports.hook_compressed-1.1.0/backports.hook_compressed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-24 01:33:00.000000 backports.hook_compressed-1.1.0/backports.hook_compressed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 01:33:00.000000 backports.hook_compressed-1.1.0/backports.hook_compressed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-24 01:33:00.000000 backports.hook_compressed-1.1.0/backports.hook_compressed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-24 01:33:00.000000 backports.hook_compressed-1.1.0/backports.hook_compressed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:33:00.642991 backports.hook_compressed-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-24 01:33:00.642991 backports.hook_compressed-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-24 01:32:40.000000 backports.hook_compressed-1.1.0/tox.ini
```

### Comparing `backports.hook_compressed-1.0.0/LICENSE` & `backports.hook_compressed-1.1.0/LICENSE`

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

### Comparing `backports.hook_compressed-1.0.0/PKG-INFO` & `backports.hook_compressed-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: backports.hook_compressed
-Version: 1.0.0
+Version: 1.1.0
 Summary: Backport of fileinput.hook_compressed from Python 3.10
 Home-page: https://github.com/jaraco/backports.hook_compressed
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
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
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/backports.hook_compressed.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/backports.hook_compressed
 
 .. image:: https://img.shields.io/pypi/pyversions/backports.hook_compressed.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/backports.hook_compressed
 
 .. image:: https://github.com/jaraco/backports.hook_compressed/workflows/tests/badge.svg
    :target: https://github.com/jaraco/backports.hook_compressed/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
-
-
```

### Comparing `backports.hook_compressed-1.0.0/README.rst` & `backports.hook_compressed-1.1.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 .. image:: https://img.shields.io/pypi/v/backports.hook_compressed.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/backports.hook_compressed
 
 .. image:: https://img.shields.io/pypi/pyversions/backports.hook_compressed.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/backports.hook_compressed
 
 .. image:: https://github.com/jaraco/backports.hook_compressed/workflows/tests/badge.svg
    :target: https://github.com/jaraco/backports.hook_compressed/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
```

### Comparing `backports.hook_compressed-1.0.0/backports/hook_compressed.py` & `backports.hook_compressed-1.1.0/backports/hook_compressed.py`

 * *Files identical despite different names*

### Comparing `backports.hook_compressed-1.0.0/backports.hook_compressed.egg-info/PKG-INFO` & `backports.hook_compressed-1.1.0/backports.hook_compressed.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: backports.hook-compressed
-Version: 1.0.0
+Version: 1.1.0
 Summary: Backport of fileinput.hook_compressed from Python 3.10
 Home-page: https://github.com/jaraco/backports.hook_compressed
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
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
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/backports.hook_compressed.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/backports.hook_compressed
 
 .. image:: https://img.shields.io/pypi/pyversions/backports.hook_compressed.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/backports.hook_compressed
 
 .. image:: https://github.com/jaraco/backports.hook_compressed/workflows/tests/badge.svg
    :target: https://github.com/jaraco/backports.hook_compressed/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
-
-
```

### Comparing `backports.hook_compressed-1.0.0/docs/conf.py` & `backports.hook_compressed-1.1.0/docs/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,42 @@
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
 
-# Be strict about any broken references:
+# Be strict about any broken references
 nitpicky = True
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

### Comparing `backports.hook_compressed-1.0.0/setup.cfg` & `backports.hook_compressed-1.1.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 [metadata]
-license_files = 
-	LICENSE
 name = backports.hook_compressed
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
 description = Backport of fileinput.hook_compressed from Python 3.10
 long_description = file:README.rst
 url = https://github.com/jaraco/backports.hook_compressed
 classifiers = 
@@ -13,38 +11,41 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
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
+	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
-	pytest-black >= 0.3.7; python_implementation != "PyPy" and python_version < "3.10"
+	pytest-black >= 0.3.7; \
+	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy; python_implementation != "PyPy" and python_version < "3.10"
-	pytest-enabler >= 1.0.1
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
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

