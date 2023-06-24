# Comparing `tmp/backports.unittest_mock-1.5.tar.gz` & `tmp/backports.unittest_mock-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpdfi_ra0c/tmp478ne0vv/backports.unittest_mock-1.5.tar", last modified: Thu Aug 22 20:02:53 2019, max compression
+gzip compressed data, was "backports.unittest_mock-1.5.1.tar", last modified: Sat Jun 24 01:42:46 2023, max compression
```

## Comparing `backports.unittest_mock-1.5.tar` & `backports.unittest_mock-1.5.1.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/.flake8
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/.pre-commit-config.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/.readthedocs.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      472 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      815 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2645 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1322 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      468 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/appveyor.yml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/backports/
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/backports/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/backports/unittest_mock/
--rw-rw-r--   0 travis    (2000) travis    (2000)      259 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/backports/unittest_mock/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/backports.unittest_mock.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2645 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/backports.unittest_mock.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      584 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/backports.unittest_mock.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/backports.unittest_mock.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       52 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/backports.unittest_mock.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      223 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/backports.unittest_mock.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/backports.unittest_mock.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      335 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      167 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      464 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/pytest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)     1358 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8063 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/skeleton.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-22 20:02:53.000000 backports.unittest_mock-1.5/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      251 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/tests/test_unittest_mock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      644 2019-08-22 20:02:37.000000 backports.unittest_mock-1.5/tox.ini
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 01:42:46.329410 backports.unittest_mock-1.5.1/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      133 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/.coveragerc
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      246 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/.editorconfig
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 01:42:46.327498 backports.unittest_mock-1.5.1/.github/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      148 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/.github/dependabot.yml
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 01:42:46.327629 backports.unittest_mock-1.5.1/.github/workflows/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3167 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/.github/workflows/main.yml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       81 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      188 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/.readthedocs.yaml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1023 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/LICENSE
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      856 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/NEWS.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2504 2023-06-24 01:42:46.329512 backports.unittest_mock-1.5.1/PKG-INFO
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1493 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/README.rst
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 01:42:46.327767 backports.unittest_mock-1.5.1/backports/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       65 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/backports/__init__.py
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 01:42:46.328741 backports.unittest_mock-1.5.1/backports/unittest_mock/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      259 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/backports/unittest_mock/__init__.py
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 01:42:46.328604 backports.unittest_mock-1.5.1/backports.unittest_mock.egg-info/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2504 2023-06-24 01:42:46.000000 backports.unittest_mock-1.5.1/backports.unittest_mock.egg-info/PKG-INFO
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      628 2023-06-24 01:42:46.000000 backports.unittest_mock-1.5.1/backports.unittest_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)        1 2023-06-24 01:42:46.000000 backports.unittest_mock-1.5.1/backports.unittest_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       51 2023-06-24 01:42:46.000000 backports.unittest_mock-1.5.1/backports.unittest_mock.egg-info/entry_points.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      337 2023-06-24 01:42:46.000000 backports.unittest_mock-1.5.1/backports.unittest_mock.egg-info/requires.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       10 2023-06-24 01:42:46.000000 backports.unittest_mock-1.5.1/backports.unittest_mock.egg-info/top_level.txt
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 01:42:46.329155 backports.unittest_mock-1.5.1/docs/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1122 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/docs/conf.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       78 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/docs/history.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      307 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/docs/index.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      154 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/mypy.ini
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      374 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/pyproject.toml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      842 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/pytest.ini
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1488 2023-06-24 01:42:46.329845 backports.unittest_mock-1.5.1/setup.cfg
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-06-24 01:42:46.329289 backports.unittest_mock-1.5.1/tests/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      251 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/tests/test_unittest_mock.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       44 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/towncrier.toml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      814 2023-06-24 01:42:33.000000 backports.unittest_mock-1.5.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `backports.unittest_mock-1.5/CHANGES.rst` & `backports.unittest_mock-1.5.1/NEWS.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v1.5.1
+======
+
+No significant changes.
+
+
 1.5
 ===
 
 Refresh project metadata.
 
 1.4
 ===
```

### Comparing `backports.unittest_mock-1.5/README.rst` & `backports.unittest_mock-1.5.1/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 .. image:: https://img.shields.io/pypi/v/backports.unittest_mock.svg
    :target: https://pypi.org/project/backports.unittest_mock
 
 .. image:: https://img.shields.io/pypi/pyversions/backports.unittest_mock.svg
 
-.. image:: https://img.shields.io/travis/jaraco/backports.unittest_mock/master.svg
-   :target: https://travis-ci.org/jaraco/backports.unittest_mock
+.. image:: https://github.com/jaraco/backports.unittest_mock/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/backports.unittest_mock/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/ambv/black
+   :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://img.shields.io/appveyor/ci/jaraco/backports-unittest_mock/master.svg
-..    :target: https://ci.appveyor.com/project/jaraco/backports-unittest_mock/branch/master
-
 .. image:: https://readthedocs.org/projects/backportsunittest_mock/badge/?version=latest
    :target: https://backportsunittest_mock.readthedocs.io/en/latest/?badge=latest
 
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
+
 Provides a function "install()" which makes the "mock" module
 available as "unittest.mock" on Python 3.2 and earlier.
 
 Also advertises a pytest plugin which configures unittest.mock
 automatically.
 
 Usage
```

### Comparing `backports.unittest_mock-1.5/backports.unittest_mock.egg-info/SOURCES.txt` & `backports.unittest_mock-1.5.1/backports.unittest_mock.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-.flake8
+.coveragerc
+.editorconfig
 .pre-commit-config.yaml
-.readthedocs.yml
-.travis.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
-appveyor.yml
+mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
-setup.py
-skeleton.md
+towncrier.toml
 tox.ini
+.github/dependabot.yml
+.github/workflows/main.yml
 backports/__init__.py
 backports.unittest_mock.egg-info/PKG-INFO
 backports.unittest_mock.egg-info/SOURCES.txt
 backports.unittest_mock.egg-info/dependency_links.txt
 backports.unittest_mock.egg-info/entry_points.txt
 backports.unittest_mock.egg-info/requires.txt
 backports.unittest_mock.egg-info/top_level.txt
```

### Comparing `backports.unittest_mock-1.5/docs/conf.py` & `backports.unittest_mock-1.5.1/docs/conf.py`

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
-                pattern=r'^(?m)((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n',
+                pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
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

### Comparing `backports.unittest_mock-1.5/setup.cfg` & `backports.unittest_mock-1.5.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-[bdist_wheel]
-universal = 1
-
 [metadata]
-license_file = LICENSE
 name = backports.unittest_mock
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
 description = Make unittest.mock available on older Pythons
 long_description = file:README.rst
 url = https://github.com/jaraco/backports.unittest_mock
 classifiers = 
@@ -22,31 +18,44 @@
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Framework :: Pytest
 
 [options]
-packages = find:
+packages = find_namespace:
 include_package_data = true
 python_requires = >=2.6
 install_requires = 
 	mock; python_version=="2.6" or python_version=="2.7" or python_version=="3.2"
-setup_requires = setuptools_scm >= 1.15.0
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
-	pytest-checkdocs
-	pytest-flake8
-	pytest-black-multipy
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
-	jaraco.packaging >= 3.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 pytest11 = 
 	unittest_mock = backports.unittest_mock
 
 [egg_info]
 tag_build =
```

