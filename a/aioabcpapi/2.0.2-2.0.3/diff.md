# Comparing `tmp/aioabcpapi-2.0.2.tar.gz` & `tmp/aioabcpapi-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioabcpapi-2.0.2.tar", last modified: Sat Jun 24 13:38:55 2023, max compression
+gzip compressed data, was "aioabcpapi-2.0.3.tar", last modified: Sat Jun 24 18:10:02 2023, max compression
```

## Comparing `aioabcpapi-2.0.2.tar` & `aioabcpapi-2.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.230650 aioabcpapi-2.0.2/
--rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     5371 2023-06-24 13:38:55.230650 aioabcpapi-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4549 2023-05-08 23:26:33.000000 aioabcpapi-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.191640 aioabcpapi-2.0.2/aioabcpapi/
--rw-rw-rw-   0        0        0      530 2023-06-24 13:38:51.000000 aioabcpapi-2.0.2/aioabcpapi/__init__.py
--rw-rw-rw-   0        0        0      653 2023-06-23 21:18:29.000000 aioabcpapi-2.0.2/aioabcpapi/abcp.py
--rw-rw-rw-   0        0        0    20198 2023-06-24 10:52:34.000000 aioabcpapi-2.0.2/aioabcpapi/api.py
--rw-rw-rw-   0        0        0     4794 2023-06-24 13:28:13.000000 aioabcpapi-2.0.2/aioabcpapi/base.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.214646 aioabcpapi-2.0.2/aioabcpapi/cp/
--rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-2.0.2/aioabcpapi/cp/__init__.py
--rw-rw-rw-   0        0        0   113820 2023-06-24 12:52:15.000000 aioabcpapi-2.0.2/aioabcpapi/cp/admin.py
--rw-rw-rw-   0        0        0      321 2023-06-23 21:51:21.000000 aioabcpapi-2.0.2/aioabcpapi/cp/base.py
--rw-rw-rw-   0        0        0    60771 2023-06-24 10:40:46.000000 aioabcpapi-2.0.2/aioabcpapi/cp/client.py
--rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-2.0.2/aioabcpapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.219647 aioabcpapi-2.0.2/aioabcpapi/ts/
--rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-2.0.2/aioabcpapi/ts/__init__.py
--rw-rw-rw-   0        0        0   123974 2023-06-24 13:18:40.000000 aioabcpapi-2.0.2/aioabcpapi/ts/admin.py
--rw-rw-rw-   0        0        0      668 2023-06-24 10:35:56.000000 aioabcpapi-2.0.2/aioabcpapi/ts/base.py
--rw-rw-rw-   0        0        0    45528 2023-06-24 13:28:13.000000 aioabcpapi-2.0.2/aioabcpapi/ts/client.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.223647 aioabcpapi-2.0.2/aioabcpapi/utils/
--rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-2.0.2/aioabcpapi/utils/__init__.py
--rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-2.0.2/aioabcpapi/utils/fields_checker.py
--rw-rw-rw-   0        0        0     9063 2023-06-24 10:35:56.000000 aioabcpapi-2.0.2/aioabcpapi/utils/payload.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.208645 aioabcpapi-2.0.2/aioabcpapi.egg-info/
--rw-rw-rw-   0        0        0     5371 2023-06-24 13:38:55.000000 aioabcpapi-2.0.2/aioabcpapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2023-06-24 13:38:55.000000 aioabcpapi-2.0.2/aioabcpapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 13:38:55.000000 aioabcpapi-2.0.2/aioabcpapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-24 13:38:55.000000 aioabcpapi-2.0.2/aioabcpapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-06-24 13:38:55.000000 aioabcpapi-2.0.2/aioabcpapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      206 2023-06-24 13:38:55.232650 aioabcpapi-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-06-24 12:54:25.000000 aioabcpapi-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.229649 aioabcpapi-2.0.2/test/
--rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-2.0.2/test/test_payload.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.149711 aioabcpapi-2.0.3/
+-rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5371 2023-06-24 18:10:02.149711 aioabcpapi-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4549 2023-05-08 23:26:33.000000 aioabcpapi-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.013440 aioabcpapi-2.0.3/aioabcpapi/
+-rw-rw-rw-   0        0        0      530 2023-06-24 18:09:53.000000 aioabcpapi-2.0.3/aioabcpapi/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 21:18:29.000000 aioabcpapi-2.0.3/aioabcpapi/abcp.py
+-rw-rw-rw-   0        0        0    20198 2023-06-24 10:52:34.000000 aioabcpapi-2.0.3/aioabcpapi/api.py
+-rw-rw-rw-   0        0        0     4794 2023-06-24 13:28:13.000000 aioabcpapi-2.0.3/aioabcpapi/base.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.078085 aioabcpapi-2.0.3/aioabcpapi/cp/
+-rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-2.0.3/aioabcpapi/cp/__init__.py
+-rw-rw-rw-   0        0        0   113820 2023-06-24 12:52:15.000000 aioabcpapi-2.0.3/aioabcpapi/cp/admin.py
+-rw-rw-rw-   0        0        0      321 2023-06-23 21:51:21.000000 aioabcpapi-2.0.3/aioabcpapi/cp/base.py
+-rw-rw-rw-   0        0        0    60771 2023-06-24 10:40:46.000000 aioabcpapi-2.0.3/aioabcpapi/cp/client.py
+-rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-2.0.3/aioabcpapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.113142 aioabcpapi-2.0.3/aioabcpapi/ts/
+-rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-2.0.3/aioabcpapi/ts/__init__.py
+-rw-rw-rw-   0        0        0   123974 2023-06-24 13:18:40.000000 aioabcpapi-2.0.3/aioabcpapi/ts/admin.py
+-rw-rw-rw-   0        0        0      668 2023-06-24 10:35:56.000000 aioabcpapi-2.0.3/aioabcpapi/ts/base.py
+-rw-rw-rw-   0        0        0    45528 2023-06-24 13:28:13.000000 aioabcpapi-2.0.3/aioabcpapi/ts/client.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.132145 aioabcpapi-2.0.3/aioabcpapi/utils/
+-rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-2.0.3/aioabcpapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-2.0.3/aioabcpapi/utils/fields_checker.py
+-rw-rw-rw-   0        0        0     9063 2023-06-24 10:35:56.000000 aioabcpapi-2.0.3/aioabcpapi/utils/payload.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.039082 aioabcpapi-2.0.3/aioabcpapi.egg-info/
+-rw-rw-rw-   0        0        0     5371 2023-06-24 18:10:01.000000 aioabcpapi-2.0.3/aioabcpapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-06-24 18:10:01.000000 aioabcpapi-2.0.3/aioabcpapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:10:01.000000 aioabcpapi-2.0.3/aioabcpapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-24 18:10:01.000000 aioabcpapi-2.0.3/aioabcpapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-06-24 18:10:01.000000 aioabcpapi-2.0.3/aioabcpapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      206 2023-06-24 18:10:02.151712 aioabcpapi-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1329 2023-06-24 18:09:53.000000 aioabcpapi-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.147711 aioabcpapi-2.0.3/test/
+-rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-2.0.3/test/test_payload.py
```

### Comparing `aioabcpapi-2.0.2/LICENSE` & `aioabcpapi-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/PKG-INFO` & `aioabcpapi-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 2.0.2
+Version: 2.0.3
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-2.0.2/README.md` & `aioabcpapi-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi/__init__.py` & `aioabcpapi-2.0.3/aioabcpapi/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,9 +5,9 @@
                          AbcpParameterRequired, TeaPot)
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 
 __author__ = 'bl4ckm45k'
-__version__ = '2.0.2'
+__version__ = '2.0.3'
 __email__ = 'nonpowa@gmail.com'
```

### Comparing `aioabcpapi-2.0.2/aioabcpapi/abcp.py` & `aioabcpapi-2.0.3/aioabcpapi/abcp.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi/api.py` & `aioabcpapi-2.0.3/aioabcpapi/api.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi/base.py` & `aioabcpapi-2.0.3/aioabcpapi/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi/cp/admin.py` & `aioabcpapi-2.0.3/aioabcpapi/cp/admin.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi/cp/client.py` & `aioabcpapi-2.0.3/aioabcpapi/cp/client.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi/exceptions.py` & `aioabcpapi-2.0.3/aioabcpapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi/ts/admin.py` & `aioabcpapi-2.0.3/aioabcpapi/ts/admin.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi/ts/base.py` & `aioabcpapi-2.0.3/aioabcpapi/ts/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi/ts/client.py` & `aioabcpapi-2.0.3/aioabcpapi/ts/client.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi/utils/fields_checker.py` & `aioabcpapi-2.0.3/aioabcpapi/utils/fields_checker.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi/utils/payload.py` & `aioabcpapi-2.0.3/aioabcpapi/utils/payload.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/aioabcpapi.egg-info/PKG-INFO` & `aioabcpapi-2.0.3/aioabcpapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 2.0.2
+Version: 2.0.3
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-2.0.2/aioabcpapi.egg-info/SOURCES.txt` & `aioabcpapi-2.0.3/aioabcpapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.2/setup.py` & `aioabcpapi-2.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import sys
-
 from setuptools import setup
-from pip._vendor.pkg_resources import parse_version
-import aioabcpapi
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 requirements = ["aiohttp>=3.8.3", "certifi>=2022.12.7", "ujson>=5.7.0", "pytz>=2022.7.1", "pyrfc3339"]
-parsed_version = parse_version(aioabcpapi.__version__)
 setup(
     name='aioabcpapi',
-    version=parsed_version,
+    version='2.0.3',
     author='bl4ckm45k',
     author_email='nonpowa@gmail.com',
     description='Async library for ABCP API',
     long_description_content_type="text/markdown",
     url="https://github.com/bl4ckm45k/aioabcpapi",
     license="MIT",
     packages=['aioabcpapi', 'aioabcpapi/cp', 'aioabcpapi/ts', 'aioabcpapi/utils'],
```

### Comparing `aioabcpapi-2.0.2/test/test_payload.py` & `aioabcpapi-2.0.3/test/test_payload.py`

 * *Files identical despite different names*

