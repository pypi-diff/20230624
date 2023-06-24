# Comparing `tmp/aioabcpapi-2.0.1.tar.gz` & `tmp/aioabcpapi-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioabcpapi-2.0.1.tar", last modified: Sat Jun 24 13:19:41 2023, max compression
+gzip compressed data, was "aioabcpapi-2.0.2.tar", last modified: Sat Jun 24 13:38:55 2023, max compression
```

## Comparing `aioabcpapi-2.0.1.tar` & `aioabcpapi-2.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 13:19:41.328375 aioabcpapi-2.0.1/
--rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     5371 2023-06-24 13:19:41.329379 aioabcpapi-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4549 2023-05-08 23:26:33.000000 aioabcpapi-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 13:19:41.277512 aioabcpapi-2.0.1/aioabcpapi/
--rw-rw-rw-   0        0        0      586 2023-06-24 13:19:39.000000 aioabcpapi-2.0.1/aioabcpapi/__init__.py
--rw-rw-rw-   0        0        0      653 2023-06-23 21:18:29.000000 aioabcpapi-2.0.1/aioabcpapi/abcp.py
--rw-rw-rw-   0        0        0    20198 2023-06-24 10:52:34.000000 aioabcpapi-2.0.1/aioabcpapi/api.py
--rw-rw-rw-   0        0        0     4792 2023-06-24 10:53:50.000000 aioabcpapi-2.0.1/aioabcpapi/base.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:19:41.310374 aioabcpapi-2.0.1/aioabcpapi/cp/
--rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-2.0.1/aioabcpapi/cp/__init__.py
--rw-rw-rw-   0        0        0   113820 2023-06-24 12:52:15.000000 aioabcpapi-2.0.1/aioabcpapi/cp/admin.py
--rw-rw-rw-   0        0        0      321 2023-06-23 21:51:21.000000 aioabcpapi-2.0.1/aioabcpapi/cp/base.py
--rw-rw-rw-   0        0        0    60771 2023-06-24 10:40:46.000000 aioabcpapi-2.0.1/aioabcpapi/cp/client.py
--rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-2.0.1/aioabcpapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:19:41.316374 aioabcpapi-2.0.1/aioabcpapi/ts/
--rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-2.0.1/aioabcpapi/ts/__init__.py
--rw-rw-rw-   0        0        0   123974 2023-06-24 13:18:40.000000 aioabcpapi-2.0.1/aioabcpapi/ts/admin.py
--rw-rw-rw-   0        0        0      668 2023-06-24 10:35:56.000000 aioabcpapi-2.0.1/aioabcpapi/ts/base.py
--rw-rw-rw-   0        0        0    45530 2023-06-24 12:52:15.000000 aioabcpapi-2.0.1/aioabcpapi/ts/client.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:19:41.321373 aioabcpapi-2.0.1/aioabcpapi/utils/
--rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-2.0.1/aioabcpapi/utils/__init__.py
--rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-2.0.1/aioabcpapi/utils/fields_checker.py
--rw-rw-rw-   0        0        0     9063 2023-06-24 10:35:56.000000 aioabcpapi-2.0.1/aioabcpapi/utils/payload.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:19:41.304790 aioabcpapi-2.0.1/aioabcpapi.egg-info/
--rw-rw-rw-   0        0        0     5371 2023-06-24 13:19:41.000000 aioabcpapi-2.0.1/aioabcpapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2023-06-24 13:19:41.000000 aioabcpapi-2.0.1/aioabcpapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 13:19:41.000000 aioabcpapi-2.0.1/aioabcpapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-24 13:19:41.000000 aioabcpapi-2.0.1/aioabcpapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-06-24 13:19:41.000000 aioabcpapi-2.0.1/aioabcpapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      206 2023-06-24 13:19:41.331374 aioabcpapi-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-06-24 12:54:25.000000 aioabcpapi-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:19:41.327374 aioabcpapi-2.0.1/test/
--rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-2.0.1/test/test_payload.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.230650 aioabcpapi-2.0.2/
+-rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5371 2023-06-24 13:38:55.230650 aioabcpapi-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4549 2023-05-08 23:26:33.000000 aioabcpapi-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.191640 aioabcpapi-2.0.2/aioabcpapi/
+-rw-rw-rw-   0        0        0      530 2023-06-24 13:38:51.000000 aioabcpapi-2.0.2/aioabcpapi/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 21:18:29.000000 aioabcpapi-2.0.2/aioabcpapi/abcp.py
+-rw-rw-rw-   0        0        0    20198 2023-06-24 10:52:34.000000 aioabcpapi-2.0.2/aioabcpapi/api.py
+-rw-rw-rw-   0        0        0     4794 2023-06-24 13:28:13.000000 aioabcpapi-2.0.2/aioabcpapi/base.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.214646 aioabcpapi-2.0.2/aioabcpapi/cp/
+-rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-2.0.2/aioabcpapi/cp/__init__.py
+-rw-rw-rw-   0        0        0   113820 2023-06-24 12:52:15.000000 aioabcpapi-2.0.2/aioabcpapi/cp/admin.py
+-rw-rw-rw-   0        0        0      321 2023-06-23 21:51:21.000000 aioabcpapi-2.0.2/aioabcpapi/cp/base.py
+-rw-rw-rw-   0        0        0    60771 2023-06-24 10:40:46.000000 aioabcpapi-2.0.2/aioabcpapi/cp/client.py
+-rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-2.0.2/aioabcpapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.219647 aioabcpapi-2.0.2/aioabcpapi/ts/
+-rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-2.0.2/aioabcpapi/ts/__init__.py
+-rw-rw-rw-   0        0        0   123974 2023-06-24 13:18:40.000000 aioabcpapi-2.0.2/aioabcpapi/ts/admin.py
+-rw-rw-rw-   0        0        0      668 2023-06-24 10:35:56.000000 aioabcpapi-2.0.2/aioabcpapi/ts/base.py
+-rw-rw-rw-   0        0        0    45528 2023-06-24 13:28:13.000000 aioabcpapi-2.0.2/aioabcpapi/ts/client.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.223647 aioabcpapi-2.0.2/aioabcpapi/utils/
+-rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-2.0.2/aioabcpapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-2.0.2/aioabcpapi/utils/fields_checker.py
+-rw-rw-rw-   0        0        0     9063 2023-06-24 10:35:56.000000 aioabcpapi-2.0.2/aioabcpapi/utils/payload.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.208645 aioabcpapi-2.0.2/aioabcpapi.egg-info/
+-rw-rw-rw-   0        0        0     5371 2023-06-24 13:38:55.000000 aioabcpapi-2.0.2/aioabcpapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-06-24 13:38:55.000000 aioabcpapi-2.0.2/aioabcpapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:38:55.000000 aioabcpapi-2.0.2/aioabcpapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-24 13:38:55.000000 aioabcpapi-2.0.2/aioabcpapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-06-24 13:38:55.000000 aioabcpapi-2.0.2/aioabcpapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      206 2023-06-24 13:38:55.232650 aioabcpapi-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-06-24 12:54:25.000000 aioabcpapi-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:38:55.229649 aioabcpapi-2.0.2/test/
+-rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-2.0.2/test/test_payload.py
```

### Comparing `aioabcpapi-2.0.1/LICENSE` & `aioabcpapi-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/PKG-INFO` & `aioabcpapi-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 2.0.1
+Version: 2.0.2
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-2.0.1/README.md` & `aioabcpapi-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/aioabcpapi/abcp.py` & `aioabcpapi-2.0.2/aioabcpapi/abcp.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/aioabcpapi/api.py` & `aioabcpapi-2.0.2/aioabcpapi/api.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/aioabcpapi/base.py` & `aioabcpapi-2.0.2/aioabcpapi/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         :param payload: _request parameters
         :type payload: :obj:`dict`
         :param post:
         :return: result
         :rtype: Union[List, Dict]
         :raise: :obj:`utils.exceptions`
         """
-        if not self.admin and isinstance(method, (Methods.Admin, Methods.TsAdmin)):
+        if not self.admin and isinstance(method, (_Methods.Admin, _Methods.TsAdmin)):
             raise NotEnoughRights('Недостаточно прав для использования API администратора')
         payload = self.__payload_check(payload)
         if isinstance(payload, FormData):
             headers = self._headers.multipart_header()
         elif kwargs is not None and 'json' in kwargs.keys():
             headers = self._headers.json_header()
             return await api.make_request_json(await self._get_session(), self._host, method, payload, headers)
```

### Comparing `aioabcpapi-2.0.1/aioabcpapi/cp/admin.py` & `aioabcpapi-2.0.2/aioabcpapi/cp/admin.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/aioabcpapi/cp/client.py` & `aioabcpapi-2.0.2/aioabcpapi/cp/client.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/aioabcpapi/exceptions.py` & `aioabcpapi-2.0.2/aioabcpapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/aioabcpapi/ts/admin.py` & `aioabcpapi-2.0.2/aioabcpapi/ts/admin.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/aioabcpapi/ts/base.py` & `aioabcpapi-2.0.2/aioabcpapi/ts/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/aioabcpapi/ts/client.py` & `aioabcpapi-2.0.2/aioabcpapi/ts/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from ..api import _Methods
 from ..base import BaseAbcp
 from ..exceptions import AbcpWrongParameterError
 from ..utils.fields_checker import check_fields
 from ..utils.payload import generate_payload
 
 
-
 class TsClientApi:
     def __init__(self, base: BaseAbcp):
         """
         Класс содержит методы клиентского интерфейса
 
         https://www.abcp.ru/wiki/API.TS.Client
         """
```

### Comparing `aioabcpapi-2.0.1/aioabcpapi/utils/fields_checker.py` & `aioabcpapi-2.0.2/aioabcpapi/utils/fields_checker.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/aioabcpapi/utils/payload.py` & `aioabcpapi-2.0.2/aioabcpapi/utils/payload.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/aioabcpapi.egg-info/PKG-INFO` & `aioabcpapi-2.0.2/aioabcpapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 2.0.1
+Version: 2.0.2
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-2.0.1/aioabcpapi.egg-info/SOURCES.txt` & `aioabcpapi-2.0.2/aioabcpapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/setup.py` & `aioabcpapi-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.1/test/test_payload.py` & `aioabcpapi-2.0.2/test/test_payload.py`

 * *Files identical despite different names*

