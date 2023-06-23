# Comparing `tmp/pytest-idem-3.1.0.tar.gz` & `tmp/pytest-idem-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-idem-3.1.0.tar", last modified: Wed Sep  7 00:18:58 2022, max compression
+gzip compressed data, was "pytest-idem-4.0.0.tar", last modified: Fri Jun 23 22:22:26 2023, max compression
```

## Comparing `pytest-idem-3.1.0.tar` & `pytest-idem-4.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 00:18:58.501143 pytest-idem-3.1.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2022-09-07 00:18:41.000000 pytest-idem-3.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1762 2022-09-07 00:18:58.501143 pytest-idem-3.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      935 2022-09-07 00:18:41.000000 pytest-idem-3.1.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      255 2022-09-07 00:18:41.000000 pytest-idem-3.1.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 00:18:58.500142 pytest-idem-3.1.0/pytest_idem/
--rw-r--r--   0 root         (0) root         (0)     3445 2022-09-07 00:18:41.000000 pytest-idem-3.1.0/pytest_idem/plugin.py
--rw-r--r--   0 root         (0) root         (0)       95 2022-09-07 00:18:41.000000 pytest-idem-3.1.0/pytest_idem/run.py
--rw-r--r--   0 root         (0) root         (0)    13795 2022-09-07 00:18:41.000000 pytest-idem-3.1.0/pytest_idem/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-07 00:18:58.501143 pytest-idem-3.1.0/pytest_idem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1762 2022-09-07 00:18:58.000000 pytest-idem-3.1.0/pytest_idem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      317 2022-09-07 00:18:58.000000 pytest-idem-3.1.0/pytest_idem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-07 00:18:58.000000 pytest-idem-3.1.0/pytest_idem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2022-09-07 00:18:58.000000 pytest-idem-3.1.0/pytest_idem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-09-07 00:18:58.000000 pytest-idem-3.1.0/pytest_idem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-09-07 00:18:58.000000 pytest-idem-3.1.0/pytest_idem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-07 00:18:58.501143 pytest-idem-3.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2782 2022-09-07 00:18:41.000000 pytest-idem-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 22:22:26.380953 pytest-idem-4.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-23 22:22:12.000000 pytest-idem-4.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-06-23 22:22:26.380953 pytest-idem-4.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-23 22:22:12.000000 pytest-idem-4.0.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-23 22:22:12.000000 pytest-idem-4.0.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 22:22:26.380953 pytest-idem-4.0.0/pytest_idem/
+-rw-r--r--   0 root         (0) root         (0)     3444 2023-06-23 22:22:12.000000 pytest-idem-4.0.0/pytest_idem/plugin.py
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-23 22:22:12.000000 pytest-idem-4.0.0/pytest_idem/run.py
+-rw-r--r--   0 root         (0) root         (0)    13795 2023-06-23 22:22:12.000000 pytest-idem-4.0.0/pytest_idem/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 22:22:26.380953 pytest-idem-4.0.0/pytest_idem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-06-23 22:22:26.000000 pytest-idem-4.0.0/pytest_idem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-23 22:22:26.000000 pytest-idem-4.0.0/pytest_idem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 22:22:26.000000 pytest-idem-4.0.0/pytest_idem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-23 22:22:26.000000 pytest-idem-4.0.0/pytest_idem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-23 22:22:26.000000 pytest-idem-4.0.0/pytest_idem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-23 22:22:26.000000 pytest-idem-4.0.0/pytest_idem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 22:22:26.380953 pytest-idem-4.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-06-23 22:22:12.000000 pytest-idem-4.0.0/setup.py
```

### Comparing `pytest-idem-3.1.0/LICENSE` & `pytest-idem-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-idem-3.1.0/PKG-INFO` & `pytest-idem-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pytest-idem
-Version: 3.1.0
+Version: 4.0.0
 Summary: A pytest plugin to help with testing idem projects
 Home-page: https://gitlab.com/saltstack/idem/pytest-idem
 Author: Tyler Johnson
 Author-email: tjohnson@saltstack.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ***********
 PYTEST-IDEM
 ***********
 **A pytest plugin to help with testing idem projects**
```

### Comparing `pytest-idem-3.1.0/README.rst` & `pytest-idem-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-idem-3.1.0/pytest_idem/plugin.py` & `pytest-idem-4.0.0/pytest_idem/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     ctx = data.NamespaceDict(
         {"run_name": "test", "test": False, "acct": data.NamespaceDict()}
     )
 
     old_opts = hub.OPT
 
     if acct_subs and acct_profile:
-
         if not (
             hub.OPT.get("acct")
             and hub.OPT.acct.get("acct_file")
             and hub.OPT.acct.get("acct_key")
         ):
             if not hasattr(hub, "acct"):
                 hub.pop.sub.add(dyne_name="acct")
```

### Comparing `pytest-idem-3.1.0/pytest_idem/runner.py` & `pytest-idem-4.0.0/pytest_idem/runner.py`

 * *Files identical despite different names*

### Comparing `pytest-idem-3.1.0/pytest_idem.egg-info/PKG-INFO` & `pytest-idem-4.0.0/pytest_idem.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pytest-idem
-Version: 3.1.0
+Version: 4.0.0
 Summary: A pytest plugin to help with testing idem projects
 Home-page: https://gitlab.com/saltstack/idem/pytest-idem
 Author: Tyler Johnson
 Author-email: tjohnson@saltstack.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ***********
 PYTEST-IDEM
 ***********
 **A pytest plugin to help with testing idem projects**
```

### Comparing `pytest-idem-3.1.0/setup.py` & `pytest-idem-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import Command
 from setuptools import setup
 
 NAME = "pytest_idem"
 DESC = "A pytest plugin to help with testing idem projects"
 
 # Version info -- read without importing
-VERSION = "3.1.0"
+VERSION = "4.0.0"
 
 SETUP_DIRNAME = os.path.dirname(__file__)
 if not SETUP_DIRNAME:
     SETUP_DIRNAME = os.getcwd()
 
 with open("README.rst", encoding="utf-8") as f:
     LONG_DESC = f.read()
@@ -72,24 +72,24 @@
     author_email="tjohnson@saltstack.com",
     url="https://gitlab.com/saltstack/idem/pytest-idem",
     version=VERSION,
     install_requires=REQUIREMENTS,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
     entry_points={"pytest11": ["pytest-idem = pytest_idem.plugin"]},
     cmdclass={"clean": Clean},
 )
```

