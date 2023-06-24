# Comparing `tmp/atro-pylog-0.0.7.tar.gz` & `tmp/atro-pylog-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pylog-0.0.7.tar", last modified: Sat Jun 24 12:30:29 2023, max compression
+gzip compressed data, was "atro-pylog-0.0.8.tar", last modified: Sat Jun 24 12:32:22 2023, max compression
```

## Comparing `atro-pylog-0.0.7.tar` & `atro-pylog-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 12:30:29.259336 atro-pylog-0.0.7/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-24 12:30:29.259336 atro-pylog-0.0.7/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.0.7/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 12:30:29.259336 atro-pylog-0.0.7/atro_pylog.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-24 12:30:29.000000 atro-pylog-0.0.7/atro_pylog.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      308 2023-06-24 12:30:29.000000 atro-pylog-0.0.7/atro_pylog.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-24 12:30:29.000000 atro-pylog-0.0.7/atro_pylog.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)      105 2023-06-24 12:30:29.000000 atro-pylog-0.0.7/atro_pylog.egg-info/requires.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-24 12:30:29.000000 atro-pylog-0.0.7/atro_pylog.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 12:30:29.259336 atro-pylog-0.0.7/pylog/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      935 2023-06-24 12:19:22.000000 atro-pylog-0.0.7/pylog/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1083 2023-06-24 12:30:18.000000 atro-pylog-0.0.7/pylog/level.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      362 2023-06-24 12:14:57.000000 atro-pylog-0.0.7/pylog/logger_type.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1387 2023-06-24 12:19:06.000000 atro-pylog-0.0.7/pylog/opentelemetry_setup.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      399 2023-06-24 12:13:37.000000 atro-pylog-0.0.7/pylog/rich_setup.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      695 2023-06-24 12:24:45.000000 atro-pylog-0.0.7/pylog/settings.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-24 12:30:29.259336 atro-pylog-0.0.7/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1088 2023-06-24 12:30:26.000000 atro-pylog-0.0.7/setup.py
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 12:32:22.671743 atro-pylog-0.0.8/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-24 12:32:22.671743 atro-pylog-0.0.8/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.0.8/README.md
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 12:32:22.671743 atro-pylog-0.0.8/atro_pylog.egg-info/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-24 12:32:22.000000 atro-pylog-0.0.8/atro_pylog.egg-info/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      308 2023-06-24 12:32:22.000000 atro-pylog-0.0.8/atro_pylog.egg-info/SOURCES.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-24 12:32:22.000000 atro-pylog-0.0.8/atro_pylog.egg-info/dependency_links.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      105 2023-06-24 12:32:22.000000 atro-pylog-0.0.8/atro_pylog.egg-info/requires.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-24 12:32:22.000000 atro-pylog-0.0.8/atro_pylog.egg-info/top_level.txt
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 12:32:22.671743 atro-pylog-0.0.8/pylog/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      935 2023-06-24 12:19:22.000000 atro-pylog-0.0.8/pylog/__init__.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1083 2023-06-24 12:30:18.000000 atro-pylog-0.0.8/pylog/level.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      362 2023-06-24 12:14:57.000000 atro-pylog-0.0.8/pylog/logger_type.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1387 2023-06-24 12:19:06.000000 atro-pylog-0.0.8/pylog/opentelemetry_setup.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      399 2023-06-24 12:13:37.000000 atro-pylog-0.0.8/pylog/rich_setup.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      680 2023-06-24 12:32:00.000000 atro-pylog-0.0.8/pylog/settings.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-24 12:32:22.671743 atro-pylog-0.0.8/setup.cfg
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1088 2023-06-24 12:32:13.000000 atro-pylog-0.0.8/setup.py
```

### Comparing `atro-pylog-0.0.7/PKG-INFO` & `atro-pylog-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.0.7/atro_pylog.egg-info/PKG-INFO` & `atro-pylog-0.0.8/atro_pylog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.0.7/pylog/__init__.py` & `atro-pylog-0.0.8/pylog/__init__.py`

 * *Files identical despite different names*

### Comparing `atro-pylog-0.0.7/pylog/level.py` & `atro-pylog-0.0.8/pylog/level.py`

 * *Files identical despite different names*

### Comparing `atro-pylog-0.0.7/pylog/opentelemetry_setup.py` & `atro-pylog-0.0.8/pylog/opentelemetry_setup.py`

 * *Files identical despite different names*

### Comparing `atro-pylog-0.0.7/pylog/settings.py` & `atro-pylog-0.0.8/pylog/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class BaseLoggerSettings(BaseSettings):
     name: str = "pylog"
     type: LoggerType  = LoggerType.RICH
     level: int | str  = logging.DEBUG
     msg_format: str = "%(message)s"
-    date_format: str = "%Y-%m-%d %H:%M:%S"
+    date_format: str = "%X"
     
     class Config:
         env_prefix = "ATRO_PYLOG_"
         env_file = ".env"
         env_file_encoding = "utf-8"
```

### Comparing `atro-pylog-0.0.7/setup.py` & `atro-pylog-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="atro-pylog",
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(),
     author="Atropos",
     author_email="pypi.rising@atro.xyz",
     description="A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atropos/atro-pylog",
```

