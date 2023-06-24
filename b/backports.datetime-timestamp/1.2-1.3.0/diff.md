# Comparing `tmp/backports.datetime_timestamp-1.2.tar.gz` & `tmp/backports.datetime_timestamp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpe_j4lz0k/backports.datetime_timestamp-1.2.tar", last modified: Wed Feb  6 15:04:06 2019, max compression
+gzip compressed data, was "backports.datetime_timestamp-1.3.0.tar", last modified: Sat Jun 24 00:33:02 2023, max compression
```

## Comparing `backports.datetime_timestamp-1.2.tar` & `backports.datetime_timestamp-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      286 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/.flake8
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/.readthedocs.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1299 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      454 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/appveyor.yml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/backports/
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/backports/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/backports/datetime_timestamp/
--rw-rw-r--   0 travis    (2000) travis    (2000)      603 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/backports/datetime_timestamp/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/backports.datetime_timestamp.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/backports.datetime_timestamp.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      512 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/backports.datetime_timestamp.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/backports.datetime_timestamp.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/backports.datetime_timestamp.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/backports.datetime_timestamp.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      296 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      456 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/pytest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      884 2019-02-06 15:04:06.000000 backports.datetime_timestamp-1.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7408 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/skeleton.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      553 2019-02-06 15:03:46.000000 backports.datetime_timestamp-1.2/tox.ini
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 00:33:02.749691 backports.datetime_timestamp-1.3.0/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      133 2023-06-24 00:13:16.000000 backports.datetime_timestamp-1.3.0/.coveragerc
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      246 2022-09-11 16:31:46.000000 backports.datetime_timestamp-1.3.0/.editorconfig
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 00:33:02.747363 backports.datetime_timestamp-1.3.0/.github/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      148 2022-09-11 16:31:46.000000 backports.datetime_timestamp-1.3.0/.github/dependabot.yml
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 00:33:02.747561 backports.datetime_timestamp-1.3.0/.github/workflows/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3167 2023-06-24 00:13:16.000000 backports.datetime_timestamp-1.3.0/.github/workflows/main.yml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       81 2022-09-11 16:31:46.000000 backports.datetime_timestamp-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      188 2023-06-24 00:13:16.000000 backports.datetime_timestamp-1.3.0/.readthedocs.yaml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1023 2023-06-24 00:13:16.000000 backports.datetime_timestamp-1.3.0/LICENSE
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      251 2023-06-24 00:22:28.000000 backports.datetime_timestamp-1.3.0/NEWS.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1959 2023-06-24 00:33:02.749792 backports.datetime_timestamp-1.3.0/PKG-INFO
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1361 2023-06-24 00:21:53.000000 backports.datetime_timestamp-1.3.0/README.rst
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 00:33:02.747785 backports.datetime_timestamp-1.3.0/backports/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       65 2022-09-11 16:31:46.000000 backports.datetime_timestamp-1.3.0/backports/__init__.py
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 00:33:02.748782 backports.datetime_timestamp-1.3.0/backports/datetime_timestamp/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      783 2023-06-24 00:14:32.000000 backports.datetime_timestamp-1.3.0/backports/datetime_timestamp/__init__.py
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 00:33:02.748643 backports.datetime_timestamp-1.3.0/backports.datetime_timestamp.egg-info/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1959 2023-06-24 00:33:02.000000 backports.datetime_timestamp-1.3.0/backports.datetime_timestamp.egg-info/PKG-INFO
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      580 2023-06-24 00:33:02.000000 backports.datetime_timestamp-1.3.0/backports.datetime_timestamp.egg-info/SOURCES.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)        1 2023-06-24 00:33:02.000000 backports.datetime_timestamp-1.3.0/backports.datetime_timestamp.egg-info/dependency_links.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      250 2023-06-24 00:33:02.000000 backports.datetime_timestamp-1.3.0/backports.datetime_timestamp.egg-info/requires.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       10 2023-06-24 00:33:02.000000 backports.datetime_timestamp-1.3.0/backports.datetime_timestamp.egg-info/top_level.txt
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 00:33:02.749469 backports.datetime_timestamp-1.3.0/docs/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1122 2023-06-24 00:13:16.000000 backports.datetime_timestamp-1.3.0/docs/conf.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       78 2023-06-24 00:13:16.000000 backports.datetime_timestamp-1.3.0/docs/history.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      312 2023-06-24 00:24:55.000000 backports.datetime_timestamp-1.3.0/docs/index.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      154 2023-06-24 00:13:16.000000 backports.datetime_timestamp-1.3.0/mypy.ini
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      374 2023-06-24 00:13:16.000000 backports.datetime_timestamp-1.3.0/pyproject.toml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      842 2023-06-24 00:13:16.000000 backports.datetime_timestamp-1.3.0/pytest.ini
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1042 2023-06-24 00:33:02.750134 backports.datetime_timestamp-1.3.0/setup.cfg
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       44 2023-06-24 00:13:16.000000 backports.datetime_timestamp-1.3.0/towncrier.toml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      814 2023-06-24 00:22:20.000000 backports.datetime_timestamp-1.3.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `backports.datetime_timestamp-1.2/README.rst` & `backports.datetime_timestamp-1.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,51 @@
+Metadata-Version: 2.1
+Name: backports.datetime_timestamp
+Version: 1.3.0
+Summary: Backport of the timestamp method from Python 3.3
+Home-page: https://github.com/jaraco/backports.datetime_timestamp
+Author: Jason R. Coombs
+Author-email: jaraco@jaraco.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Provides-Extra: testing
+Provides-Extra: docs
+License-File: LICENSE
+
 .. image:: https://img.shields.io/pypi/v/backports.datetime_timestamp.svg
    :target: https://pypi.org/project/backports.datetime_timestamp
 
 .. image:: https://img.shields.io/pypi/pyversions/backports.datetime_timestamp.svg
 
-.. image:: https://img.shields.io/travis/jaraco/backports.datetime_timestamp/master.svg
-   :target: http://travis-ci.org/jaraco/backports.datetime_timestamp
-
-.. .. image:: https://img.shields.io/appveyor/ci/jaraco/backports.datetime_timestamp/master.svg
-..    :target: https://ci.appveyor.com/project/jaraco/backports.datetime_timestamp/branch/master
+.. image:: https://github.com/jaraco/backports.datetime_timestamp/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/backports.datetime_timestamp/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/backportsdatetime_timestamp/badge/?version=latest
-..    :target: https://backportsdatetime_timestamp.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
 
 Backport of the `datetime.timestamp()
 <http://docs.python.org/3.3/library/datetime.html#datetime.datetime.timestamp>`_ method added in Python 3.3.
 
+Used as::
+
     from backports.datetime_timestamp import timestamp
     import datetime
 
     dt = datetime.datetime.utcnow()
     # instead of dt.timestamp(), use
     timestamp(dt)
```

### Comparing `backports.datetime_timestamp-1.2/docs/conf.py` & `backports.datetime_timestamp-1.3.0/docs/conf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ["sphinx.ext.autodoc", "jaraco.packaging.sphinx", "rst.linker"]
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    "../CHANGES.rst": dict(
-        using=dict(GH="https://github.com"),
+    '../NEWS.rst': dict(
+        using=dict(GH='https://github.com'),
         replace=[
             dict(
-                pattern=r"(Issue #|\B#)(?P<issue>\d+)",
-                url="{package_url}/issues/{issue}",
+                pattern=r'(Issue #|\B#)(?P<issue>\d+)',
+                url='{package_url}/issues/{issue}',
             ),
             dict(
-                pattern=r"^(?m)((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n",
-                with_scm="{text}\n{rev[timestamp]:%d %b %Y}\n",
+                pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
+                with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
-                pattern=r"PEP[- ](?P<pep_number>\d+)",
-                url="https://www.python.org/dev/peps/pep-{pep_number:0>4}/",
+                pattern=r'PEP[- ](?P<pep_number>\d+)',
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

