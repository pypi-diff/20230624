# Comparing `tmp/geocat.comp-2023.6.0.tar.gz` & `tmp/geocat.comp-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocat.comp-2023.6.0.tar", last modified: Fri Jun 23 21:03:47 2023, max compression
+gzip compressed data, was "geocat.comp-2023.6.1.tar", last modified: Sat Jun 24 04:09:32 2023, max compression
```

## Comparing `geocat.comp-2023.6.0.tar` & `geocat.comp-2023.6.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:03:47.725020 geocat.comp-2023.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-23 21:03:47.725020 geocat.comp-2023.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:03:47.721020 geocat.comp-2023.6.0/build_envs/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/build_envs/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/build_envs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/build_envs/upstream-dev-environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:03:47.721020 geocat.comp-2023.6.0/geocat/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:03:47.725020 geocat.comp-2023.6.0/geocat/comp/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/climatologies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/fourier_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/gc_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    26716 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    54706 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/meteorology.py
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/spherical.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:03:47.721020 geocat.comp-2023.6.0/geocat.comp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-23 21:03:47.725020 geocat.comp-2023.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:09:32.224064 geocat.comp-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-24 04:09:32.228064 geocat.comp-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:09:32.224064 geocat.comp-2023.6.1/build_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/build_envs/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/build_envs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/build_envs/upstream-dev-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:09:32.224064 geocat.comp-2023.6.1/geocat/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/geocat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:09:32.224064 geocat.comp-2023.6.1/geocat/comp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/geocat/comp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/geocat/comp/climatologies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/geocat/comp/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/geocat/comp/fourier_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/geocat/comp/gc_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/geocat/comp/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26716 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/geocat/comp/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54706 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/geocat/comp/meteorology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/geocat/comp/spherical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/geocat/comp/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 04:09:32.224064 geocat.comp-2023.6.1/geocat.comp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-24 04:09:31.000000 geocat.comp-2023.6.1/geocat.comp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-24 04:09:32.000000 geocat.comp-2023.6.1/geocat.comp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 04:09:31.000000 geocat.comp-2023.6.1/geocat.comp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 04:09:31.000000 geocat.comp-2023.6.1/geocat.comp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-24 04:09:31.000000 geocat.comp-2023.6.1/geocat.comp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 04:09:31.000000 geocat.comp-2023.6.1/geocat.comp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-24 04:09:32.228064 geocat.comp-2023.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 04:09:18.000000 geocat.comp-2023.6.1/setup.py
```

### Comparing `geocat.comp-2023.6.0/.gitignore` & `geocat.comp-2023.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/.pre-commit-config.yaml` & `geocat.comp-2023.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/CONTRIBUTING.md` & `geocat.comp-2023.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/LICENSE` & `geocat.comp-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/PKG-INFO` & `geocat.comp-2023.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: geocat.comp
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: GeoCAT-comp is computational component of the GeoCAT project and
 Home-page: https://geocat-comp.readthedocs.io
 Author: GeoCAT Team
 Author-email: geocat@ucar.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: <=3.11,>=3.9
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 | CI           | [![GitHub Workflow Status][github-ci-badge]][github-ci-link] [![GitHub Workflow Status][github-upstream-ci-badge]][github-upstream-ci-link] [![Code Coverage Status][codecov-badge]][codecov-link] |
 | :----------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
 | **Docs**     |                                                                    [![Documentation Status][rtd-badge]][rtd-link]                                                                    |
 | **Package**  |                                                         [![Conda][conda-badge]][conda-link] [![PyPI][pypi-badge]][pypi-link]                                                         |
```

### Comparing `geocat.comp-2023.6.0/README.md` & `geocat.comp-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/build_envs/environment.yml` & `geocat.comp-2023.6.1/build_envs/environment.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name: geocat_comp_build
 channels:
   - conda-forge
 dependencies:
-  - python>=3.9, <=3.11  # minimum support 3.9
+  - python>=3.9, <3.12  # minimum support 3.9
   - cf_xarray>=0.3.1    # min version 0.3.1 for dependencies
   - cftime
   - dask
   - distributed
   - eofs
   - metpy
   - numba
```

### Comparing `geocat.comp-2023.6.0/geocat/comp/__init__.py` & `geocat.comp-2023.6.1/geocat/comp/__init__.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/geocat/comp/climatologies.py` & `geocat.comp-2023.6.1/geocat/comp/climatologies.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/geocat/comp/deprecated.py` & `geocat.comp-2023.6.1/geocat/comp/deprecated.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/geocat/comp/fourier_filters.py` & `geocat.comp-2023.6.1/geocat/comp/fourier_filters.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/geocat/comp/gc_util.py` & `geocat.comp-2023.6.1/geocat/comp/gc_util.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/geocat/comp/gradient.py` & `geocat.comp-2023.6.1/geocat/comp/gradient.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/geocat/comp/interpolation.py` & `geocat.comp-2023.6.1/geocat/comp/interpolation.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/geocat/comp/meteorology.py` & `geocat.comp-2023.6.1/geocat/comp/meteorology.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/geocat/comp/spherical.py` & `geocat.comp-2023.6.1/geocat/comp/spherical.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/geocat/comp/stats.py` & `geocat.comp-2023.6.1/geocat/comp/stats.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/geocat.comp.egg-info/PKG-INFO` & `geocat.comp-2023.6.1/geocat.comp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: geocat.comp
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: GeoCAT-comp is computational component of the GeoCAT project and
 Home-page: https://geocat-comp.readthedocs.io
 Author: GeoCAT Team
 Author-email: geocat@ucar.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: <=3.11,>=3.9
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 | CI           | [![GitHub Workflow Status][github-ci-badge]][github-ci-link] [![GitHub Workflow Status][github-upstream-ci-badge]][github-upstream-ci-link] [![Code Coverage Status][codecov-badge]][codecov-link] |
 | :----------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
 | **Docs**     |                                                                    [![Documentation Status][rtd-badge]][rtd-link]                                                                    |
 | **Package**  |                                                         [![Conda][conda-badge]][conda-link] [![PyPI][pypi-badge]][pypi-link]                                                         |
```

### Comparing `geocat.comp-2023.6.0/geocat.comp.egg-info/SOURCES.txt` & `geocat.comp-2023.6.1/geocat.comp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.6.0/setup.cfg` & `geocat.comp-2023.6.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 
 [options]
 zip_safe = False
 include_package_data = True
-python_requires = >=3.9, <=3.11
+python_requires = >=3.9, <3.12
 packages = 
 	geocat
 	geocat.comp
 setup_requires = 
 	setuptools_scm
 	setuptools
 	pip
```

