# Comparing `tmp/aioabcpapi-1.1.5.tar.gz` & `tmp/aioabcpapi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioabcpapi-1.1.5.tar", last modified: Mon May  8 23:13:24 2023, max compression
+gzip compressed data, was "aioabcpapi-2.0.0.tar", last modified: Sat Jun 24 12:55:08 2023, max compression
```

## Comparing `aioabcpapi-1.1.5.tar` & `aioabcpapi-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 23:13:24.097699 aioabcpapi-1.1.5/
--rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-1.1.5/LICENSE
--rw-rw-rw-   0        0        0     5341 2023-05-08 23:13:24.097699 aioabcpapi-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4519 2022-11-22 13:00:19.000000 aioabcpapi-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 23:13:23.969668 aioabcpapi-1.1.5/aioabcpapi/
--rw-rw-rw-   0        0        0      584 2023-05-08 23:12:15.000000 aioabcpapi-1.1.5/aioabcpapi/__init__.py
--rw-rw-rw-   0        0        0      680 2023-04-11 17:25:28.000000 aioabcpapi-1.1.5/aioabcpapi/abcp.py
--rw-rw-rw-   0        0        0    18959 2023-05-08 23:10:24.000000 aioabcpapi-1.1.5/aioabcpapi/api.py
--rw-rw-rw-   0        0        0     4799 2023-04-11 17:25:28.000000 aioabcpapi-1.1.5/aioabcpapi/base.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:13:24.028683 aioabcpapi-1.1.5/aioabcpapi/cp/
--rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-1.1.5/aioabcpapi/cp/__init__.py
--rw-rw-rw-   0        0        0   113231 2023-04-11 17:21:52.000000 aioabcpapi-1.1.5/aioabcpapi/cp/admin.py
--rw-rw-rw-   0        0        0      767 2023-04-11 17:25:28.000000 aioabcpapi-1.1.5/aioabcpapi/cp/base.py
--rw-rw-rw-   0        0        0    60138 2023-04-16 16:54:48.000000 aioabcpapi-1.1.5/aioabcpapi/cp/client.py
--rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-1.1.5/aioabcpapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:13:24.065691 aioabcpapi-1.1.5/aioabcpapi/ts/
--rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-1.1.5/aioabcpapi/ts/__init__.py
--rw-rw-rw-   0        0        0   113383 2023-04-11 17:37:33.000000 aioabcpapi-1.1.5/aioabcpapi/ts/admin.py
--rw-rw-rw-   0        0        0      784 2023-04-11 17:25:28.000000 aioabcpapi-1.1.5/aioabcpapi/ts/base.py
--rw-rw-rw-   0        0        0    45010 2023-04-11 16:56:32.000000 aioabcpapi-1.1.5/aioabcpapi/ts/client.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:13:24.083694 aioabcpapi-1.1.5/aioabcpapi/utils/
--rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-1.1.5/aioabcpapi/utils/__init__.py
--rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-1.1.5/aioabcpapi/utils/fields_checker.py
--rw-rw-rw-   0        0        0     9025 2023-04-11 17:30:01.000000 aioabcpapi-1.1.5/aioabcpapi/utils/payload.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:13:23.993675 aioabcpapi-1.1.5/aioabcpapi.egg-info/
--rw-rw-rw-   0        0        0     5341 2023-05-08 23:13:23.000000 aioabcpapi-1.1.5/aioabcpapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2023-05-08 23:13:23.000000 aioabcpapi-1.1.5/aioabcpapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 23:13:23.000000 aioabcpapi-1.1.5/aioabcpapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-08 23:13:23.000000 aioabcpapi-1.1.5/aioabcpapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-05-08 23:13:23.000000 aioabcpapi-1.1.5/aioabcpapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      206 2023-05-08 23:13:24.099700 aioabcpapi-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-05-08 23:12:15.000000 aioabcpapi-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:13:24.095699 aioabcpapi-1.1.5/test/
--rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-1.1.5/test/test_payload.py
+drwxrwxrwx   0        0        0        0 2023-06-24 12:55:08.442557 aioabcpapi-2.0.0/
+-rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     5371 2023-06-24 12:55:08.443557 aioabcpapi-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4549 2023-05-08 23:26:33.000000 aioabcpapi-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 12:55:08.387911 aioabcpapi-2.0.0/aioabcpapi/
+-rw-rw-rw-   0        0        0      586 2023-06-24 12:53:26.000000 aioabcpapi-2.0.0/aioabcpapi/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 21:18:29.000000 aioabcpapi-2.0.0/aioabcpapi/abcp.py
+-rw-rw-rw-   0        0        0    20198 2023-06-24 10:52:34.000000 aioabcpapi-2.0.0/aioabcpapi/api.py
+-rw-rw-rw-   0        0        0     4792 2023-06-24 10:53:50.000000 aioabcpapi-2.0.0/aioabcpapi/base.py
+drwxrwxrwx   0        0        0        0 2023-06-24 12:55:08.416919 aioabcpapi-2.0.0/aioabcpapi/cp/
+-rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-2.0.0/aioabcpapi/cp/__init__.py
+-rw-rw-rw-   0        0        0   113820 2023-06-24 12:52:15.000000 aioabcpapi-2.0.0/aioabcpapi/cp/admin.py
+-rw-rw-rw-   0        0        0      321 2023-06-23 21:51:21.000000 aioabcpapi-2.0.0/aioabcpapi/cp/base.py
+-rw-rw-rw-   0        0        0    60771 2023-06-24 10:40:46.000000 aioabcpapi-2.0.0/aioabcpapi/cp/client.py
+-rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-2.0.0/aioabcpapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-24 12:55:08.423920 aioabcpapi-2.0.0/aioabcpapi/ts/
+-rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-2.0.0/aioabcpapi/ts/__init__.py
+-rw-rw-rw-   0        0        0   123529 2023-06-24 12:52:15.000000 aioabcpapi-2.0.0/aioabcpapi/ts/admin.py
+-rw-rw-rw-   0        0        0      668 2023-06-24 10:35:56.000000 aioabcpapi-2.0.0/aioabcpapi/ts/base.py
+-rw-rw-rw-   0        0        0    45530 2023-06-24 12:52:15.000000 aioabcpapi-2.0.0/aioabcpapi/ts/client.py
+drwxrwxrwx   0        0        0        0 2023-06-24 12:55:08.427560 aioabcpapi-2.0.0/aioabcpapi/utils/
+-rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-2.0.0/aioabcpapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-2.0.0/aioabcpapi/utils/fields_checker.py
+-rw-rw-rw-   0        0        0     9063 2023-06-24 10:35:56.000000 aioabcpapi-2.0.0/aioabcpapi/utils/payload.py
+drwxrwxrwx   0        0        0        0 2023-06-24 12:55:08.410916 aioabcpapi-2.0.0/aioabcpapi.egg-info/
+-rw-rw-rw-   0        0        0     5371 2023-06-24 12:55:08.000000 aioabcpapi-2.0.0/aioabcpapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-06-24 12:55:08.000000 aioabcpapi-2.0.0/aioabcpapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 12:55:08.000000 aioabcpapi-2.0.0/aioabcpapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-24 12:55:08.000000 aioabcpapi-2.0.0/aioabcpapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-06-24 12:55:08.000000 aioabcpapi-2.0.0/aioabcpapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      206 2023-06-24 12:55:08.449557 aioabcpapi-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-06-24 12:54:25.000000 aioabcpapi-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 12:55:08.441558 aioabcpapi-2.0.0/test/
+-rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-2.0.0/test/test_payload.py
```

### Comparing `aioabcpapi-1.1.5/LICENSE` & `aioabcpapi-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.5/PKG-INFO` & `aioabcpapi-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 1.1.5
+Version: 2.0.0
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,17 +18,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## AioAbcpApi
 
-Async library for [API ABCP](https://www.abcp.ru/wiki/ABCP.API "API ABCP")
-with [asyncio](https://docs.python.org/3/library/asyncio.html "asyncio")
-and [aiohttp](https://github.com/aio-libs/aiohttp "aiohttp")
+Асинхронная библиотека для [API ABCP](https://www.abcp.ru/wiki/ABCP.API "API ABCP")
+с [asyncio](https://docs.python.org/3/library/asyncio.html "asyncio")
+и [aiohttp](https://github.com/aio-libs/aiohttp "aiohttp")
 
 ![](https://img.shields.io/github/stars/bl4ckm45k/aioabcpapi.svg)
 ![](https://img.shields.io/github/forks/bl4ckm45k/aioabcpapi.svg)
 ![](https://img.shields.io/github/issues/bl4ckm45k/aioabcpapi.svg)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/aioabcpapi.svg)](https://pypi.python.org/pypi/aioabcpapi)
 [![Downloads](https://img.shields.io/pypi/dm/aioabcpapi.svg?)](https://pypi.python.org/pypi/aioabcpapi)
 [![PyPi Package Version](https://img.shields.io/pypi/v/aioabcpapi)](https://pypi.python.org/pypi/aioabcpapi)
```

### Comparing `aioabcpapi-1.1.5/README.md` & `aioabcpapi-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## AioAbcpApi
 
-Async library for [API ABCP](https://www.abcp.ru/wiki/ABCP.API "API ABCP")
-with [asyncio](https://docs.python.org/3/library/asyncio.html "asyncio")
-and [aiohttp](https://github.com/aio-libs/aiohttp "aiohttp")
+Асинхронная библиотека для [API ABCP](https://www.abcp.ru/wiki/ABCP.API "API ABCP")
+с [asyncio](https://docs.python.org/3/library/asyncio.html "asyncio")
+и [aiohttp](https://github.com/aio-libs/aiohttp "aiohttp")
 
 ![](https://img.shields.io/github/stars/bl4ckm45k/aioabcpapi.svg)
 ![](https://img.shields.io/github/forks/bl4ckm45k/aioabcpapi.svg)
 ![](https://img.shields.io/github/issues/bl4ckm45k/aioabcpapi.svg)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/aioabcpapi.svg)](https://pypi.python.org/pypi/aioabcpapi)
 [![Downloads](https://img.shields.io/pypi/dm/aioabcpapi.svg?)](https://pypi.python.org/pypi/aioabcpapi)
 [![PyPi Package Version](https://img.shields.io/pypi/v/aioabcpapi)](https://pypi.python.org/pypi/aioabcpapi)
```

### Comparing `aioabcpapi-1.1.5/aioabcpapi/__init__.py` & `aioabcpapi-2.0.0/aioabcpapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from .base import BaseAbcp
 from .abcp import Abcp
-from .api import check_result, make_request, Methods
+# from .api import check_result, make_request, Methods
 from .exceptions import (NetworkError, UnsupportedHost, UnsupportedLogin, PasswordType, NotEnoughRights, AbcpAPIError,
                          AbcpParameterRequired, TeaPot)
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 
 __author__ = 'bl4ckm45k'
-__version__ = '1.1.5'
+__version__ = '2.0.0'
 __email__ = 'nonpowa@gmail.com'
```

### Comparing `aioabcpapi-1.1.5/aioabcpapi/abcp.py` & `aioabcpapi-2.0.0/aioabcpapi/abcp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from aioabcpapi import BaseAbcp
 from aioabcpapi.cp.base import CpApi
 from aioabcpapi.ts.base import TsApi
 
 
-class Abcp(BaseAbcp):
+class Abcp:
     def __init__(self, host: str, login: str, password: str):
         """
         Инициализация класса API
 
         api = Abcp(host, login, password)
 
         Доступные методы:
@@ -16,10 +16,10 @@
 
         ts - API TS (API 2.0)
 
         :param host: Хост
         :param login: Логин
         :param password: MD5-пароль
         """
-        super().__init__(host, login, password)
-        self.cp = CpApi(host, login, password)
-        self.ts = TsApi(host, login, password)
+        self._base = BaseAbcp(host, login, password)
+        self.cp = CpApi(self._base)
+        self.ts = TsApi(self._base)
```

### Comparing `aioabcpapi-1.1.5/aioabcpapi/api.py` & `aioabcpapi-2.0.0/aioabcpapi/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,36 +11,33 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger('api')
 
 
 def check_data(host: str, login: str, password: str):
     regex_md = re.match(r"([a-f\d]{32})", password)
-    if regex_md:
-        host_id = host.split('.')[0][2:]
-        if host_id.isdigit() and len(host_id) < 6 and host[0:2] == 'id':
-            if login[0:6] == 'api@id' and login[6:] == host_id:
-                return True
-            if login.isdigit() and 4 < len(login) < 14:
-                return False
-            if '@' in login:
-                email = re.match('^[\w.]+@([\w-]+\.)+[\w-]{2,6}$', login, flags=re.IGNORECASE)
-                if email:
-                    return False
-                else:
-                    raise UnsupportedLogin('Недопустимый логин')
-            else:
+    if not regex_md:
+        raise PasswordType('Допускаются пароли только в md5 hash')
+    host_id = host.split('.')[0]
+    if login[0:4] == 'api@':
+        return login.split('@')[1] == host_id
+    if host_id[2:].isdigit() and len(host_id) < 10 and host[0:2] == 'id':
+        if login.isdigit() and 4 < len(login) < 14:
+            return False
+        if '@' in login:
+            email = re.match('^[\w.]+@([\w-]+\.)+[\w-]{2,6}$', login, flags=re.IGNORECASE)
+            if not email:
                 raise UnsupportedLogin('Недопустимый логин')
-        elif host[:4] == 'abcp' and host.split('.')[0][4:].isdigit():
-            return True
-        else:
-            raise UnsupportedHost(f'Имя хоста {host} не поддерживается\n'
-                                  f'Допустимые имена id200.public.api.abcp.ru')
+            return False
+        raise UnsupportedLogin('Недопустимый логин')
     else:
-        raise PasswordType('Допускаются пароли только в md5 hash')
+        raise UnsupportedHost(f'Имя хоста {host} не поддерживается\n'
+                              f'Допустимые имена:\n'
+                              f'id200.public.api.abcp.ru\n'
+                              f'abcp55333.public.api.abcp.ru')
 
 
 def check_result(method_name: str, content_type: str, status_code: int, body):
     """
     Checks whether `result` is a valid API response.
     A result is considered invalid if:
     - The server returned an HTTP response code other than 200
@@ -83,17 +80,17 @@
                             data: Dict, headers,
                             **kwargs):
     url = f'https://{host}/{method}'
     try:
         async with session.post(url, json=data, headers=headers, **kwargs) as response:
             try:
                 body = await response.json()
+                return check_result(method, response.content_type, response.status, body)
             except:
-                body = response.text
-            return check_result(method, response.content_type, response.status, body)
+                raise AbcpAPIError(response.text)
     except aiohttp.ClientError as e:
         raise NetworkError(f"aiohttp client throws an error: {e.__class__.__name__}: {e}")
 
 
 async def make_request(session, host, method,
                        data: Union[Dict, aiohttp.FormData],
                        headers, post,
@@ -136,15 +133,15 @@
     def url_encoded_header(self):
         return self.__url_encoded_header
 
     def multipart_header(self):
         return self.__multipart_header
 
 
-class Methods:
+class _Methods:
     class Admin:
         @dataclass(frozen=True)
         class Orders:
             GET_ORDERS_LIST: str = 'cp/orders'
             GET_ORDER: str = 'cp/order'
             STATUS_HISTORY: str = 'cp/order/statusHistory'
             SAVE_ORDER: str = 'cp/order'
@@ -333,14 +330,15 @@
         @dataclass(frozen=True)
         class Positions:
             GET: str = 'ts/positions/get'
             GET_LIST: str = 'ts/positions/list'
             CANCEL: str = 'ts/positions/cancel'
             MASS_CANCEL: str = 'ts/positions/massCancel'
 
+    @dataclass(frozen=True)
     class TsAdmin:
         @dataclass(frozen=True)
         class OrderPickings:
             FAST_GET_OUT: str = 'cp/ts/orderPickings/fastGetOut'
             GET: str = 'cp/ts/orderPickings/get'
             GET_GOODS: str = 'cp/ts/orderPickings/getGoods'
             CREATE_BY_OLD_POS: str = 'cp/ts/orderPickings/createByOldPos'
@@ -356,14 +354,44 @@
             CREATE_POSITION: str = 'cp/ts/customerComplaints/createPosition'
             CREATE_POSITION_MULTIPLE: str = 'cp/ts/customerComplaints/createPositionMultiple'
             UPDATE_POSITION: str = 'cp/ts/customerComplaints/updatePosition'
             CHANGE_STATUS_POSITION: str = 'cp/ts/customerComplaints/changeStatusPosition'
             UPDATE: str = 'cp/ts/customerComplaints/update'
             UPDATE_CUSTOM_FILE: str = 'cp/ts/customerComplaints/updateCustomFile'
 
+        class SupplierReturns:
+            @dataclass
+            class Operations:
+                __section: str = '/cp/ts/supplierReturns/operations'
+                LIST: str = f'{__section}/list'
+                SUM: str = f'{__section}/sum'
+                GET: str = f'{__section}/get'
+                CREATE: str = f'{__section}/create'
+                UPDATE: str = f'{__section}/update'
+                DELETE: str = f'{__section}/delete'
+
+            @dataclass
+            class Positions:
+                __section: str = '/cp/ts/supplierReturns/positions'
+                LIST: str = f'{__section}/list'
+                SUM: str = f'{__section}/sum'
+                STATUS: str = f'{__section}/status'
+                GET: str = f'{__section}/get'
+                CREATE_MULTIPLE: str = f'{__section}/createMultiple'
+                SPLIT = f'{__section}/split'
+                UPDATE = f'{__section}/update'
+                CHANGE_STATUS = f'{__section}/changeStatus'
+
+            @dataclass
+            class PositionsAttr:
+                __section: str = '/cp/ts/supplierReturns/positions/attr'
+                CREATE: str = f'{__section}/create'
+                UPDATE: str = f'{__section}/update'
+                DELETE: str = f'{__section}/delete'
+
         @dataclass(frozen=True)
         class DistributorOwners:
             DISTRIBUTOR_OWNERS: str = 'cp/ts/distributorOwners'
 
         @dataclass(frozen=True)
         class Orders:
             CREATE: str = 'cp/ts/orders/create'
@@ -447,10 +475,10 @@
     class VinQu:
         pass
 
     class TecDoc:
         pass
 
 
-SEARCH_METHODS = (Methods.Client.Search.BRANDS, Methods.Client.Search.ARTICLES, Methods.Client.Search.BATCH,
-                  Methods.Client.Search.HISTORY, Methods.Client.Search.TIPS, Methods.Client.Search.ADVICES,
-                  Methods.Client.Search.ADVICES_BATCH)
+SEARCH_METHODS = (_Methods.Client.Search.BRANDS, _Methods.Client.Search.ARTICLES, _Methods.Client.Search.BATCH,
+                  _Methods.Client.Search.HISTORY, _Methods.Client.Search.TIPS, _Methods.Client.Search.ADVICES,
+                  _Methods.Client.Search.ADVICES_BATCH)
```

### Comparing `aioabcpapi-1.1.5/aioabcpapi/base.py` & `aioabcpapi-2.0.0/aioabcpapi/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import aiohttp
 import certifi
 import ujson as json
 from aiohttp import FormData
 
 from . import api
-from .api import Headers, Methods
+from .api import Headers, _Methods
 from .exceptions import NotEnoughRights
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger('base')
 
 
 class BaseAbcp:
@@ -42,20 +42,20 @@
 
         self._main_loop = loop
         # Authentication
 
         self._host = host
         self._login = login
         self._password = password
-        self._admin = api.check_data(host, login, password)
+        self.admin = api.check_data(host, login, password)
 
-        self._shipment_address = None
-        self._shipment_method = None
-        self._payment_method = None
-        self._shipment_office = None
+        self.shipment_address = None
+        self.shipment_method = None
+        self.payment_method = None
+        self.shipment_office = None
         self._ssl_context = ssl.create_default_context(cafile=certifi.where())
 
         self._session: Optional[aiohttp.ClientSession] = None
         self._connector_class: Type[aiohttp.TCPConnector] = aiohttp.TCPConnector
         self._connector_init = dict(limit=connections_limit, ssl=self._ssl_context)
         self._headers = Headers()
 
@@ -95,31 +95,31 @@
         elif isinstance(payload, FormData):
             payload.add_field('userlogin', self._login)
             payload.add_field('userpsw', self._password)
         elif payload is None:
             payload = {'userlogin': self._login, 'userpsw': self._password}
         return payload
 
-    async def _request(self, method: str,
-                       payload: Union[Dict, FormData] = None, post: bool = False, **kwargs) -> Union[List, Dict, bool]:
+    async def request(self, method: str,
+                      payload: Union[Dict, FormData] = None, post: bool = False, **kwargs) -> Union[List, Dict, bool]:
         """
         Make an request to ABCP API
 
         https://www.abcp.ru/wiki/API:Docs
 
         :param method: API method
         :type method: :obj:`str`
         :param payload: _request parameters
         :type payload: :obj:`dict`
         :param post:
         :return: result
         :rtype: Union[List, Dict]
         :raise: :obj:`utils.exceptions`
         """
-        if not self._admin and isinstance(method, (Methods.Admin, Methods.TsAdmin)):
+        if not self.admin and isinstance(method, (Methods.Admin, Methods.TsAdmin)):
             raise NotEnoughRights('Недостаточно прав для использования API администратора')
         payload = self.__payload_check(payload)
         if isinstance(payload, FormData):
             headers = self._headers.multipart_header()
         elif kwargs is not None and 'json' in kwargs.keys():
             headers = self._headers.json_header()
             return await api.make_request_json(await self._get_session(), self._host, method, payload, headers)
```

### Comparing `aioabcpapi-1.1.5/aioabcpapi/cp/admin.py` & `aioabcpapi-2.0.0/aioabcpapi/cp/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
-
-import logging
 from datetime import datetime
 from io import BufferedReader
 from typing import Dict, List, Optional, Union
 
-from .. import api
+from ..api import _Methods
 from ..base import BaseAbcp
 from ..exceptions import AbcpAPIError, AbcpParameterRequired, AbcpWrongParameterError
 from ..utils.payload import generate_payload, generate_payload_filter, generate_payload_payments, \
     generate_payload_online_order, generate_file_payload
 
-logging.basicConfig(level=logging.DEBUG)
-logger = logging.getLogger('Cp.Admin')
-
 
-class AdminApi(BaseAbcp):
-    def __init__(self, *args):
+class AdminApi:
+    def __init__(self, base: BaseAbcp):
         """
         Класс содержит методы административного интерфейса
 
         https://www.abcp.ru/wiki/API.ABCP.Admin
         """
-        super().__init__(*args)
-        self.orders = Orders(*args)
-        self.finance = Finance(*args)
-        self.users = Users(*args)
-        self.staff = Staff(*args)
-        self.statuses = Statuses(*args)
-        self.distributors = Distributors(*args)
-        self.catalog = Catalog(*args)
-        self.articles = Articles(*args)
-        self.users_catalog = UsersCatalog(*args)
-        self.payment = Payment(*args)
-
-
-class Orders(BaseAbcp):
+        self._base = base
+        self.orders = Orders(base)
+        self.finance = Finance(base)
+        self.users = Users(base)
+        self.staff = Staff(base)
+        self.statuses = Statuses(base)
+        self.distributors = Distributors(base)
+        self.catalog = Catalog(base)
+        self.articles = Articles(base)
+        self.users_catalog = UsersCatalog(base)
+        self.payment = Payment(base)
+
+
+class Orders:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
     async def get_orders_list(
             self,
             date_created_start: Union[str, datetime] = None,
             date_created_end: Union[str, datetime] = None,
             date_updated_start: Union[str, datetime] = None,
             date_updated_end: Union[str, datetime] = None,
@@ -122,16 +119,15 @@
         if isinstance(status_code, (int, str)):
             status_code = [status_code]
         if not isinstance(numbers, list) and numbers is not None:
             numbers = [numbers]
         if isinstance(user_id, str) and not user_id.isdigit():
             raise AbcpAPIError(f'Параметр user_id должен быть числом')
         payload = generate_payload(**locals())
-
-        return await self._request(api.Methods.Admin.Orders.GET_ORDERS_LIST, payload)
+        return await self._base.request(_Methods.Admin.Orders.GET_ORDERS_LIST, payload)
 
     async def get_order(
             self,
             number: Union[int, str] = None,
             internal_number: Union[int, str] = None,
             with_deleted: Union[str, bool] = None,
             format: str = None
@@ -158,15 +154,15 @@
         :type format: str
 
         """
         if number is None and internal_number is None:
             raise AbcpParameterRequired(f'Один из параметров "number" или "internal_number" должен быть указан')
         payload = generate_payload(**locals())
 
-        return await self._request(api.Methods.Admin.Orders.GET_ORDER, payload)
+        return await self._base.request(_Methods.Admin.Orders.GET_ORDER, payload)
 
     async def status_history(
             self,
             position_id: Union[int, str]
 
     ):
         """Принимает в качестве параметра id позиции заказа. Возвращает информацию об истории изменений статуса позиции заказа.
@@ -177,15 +173,15 @@
         :param position_id: Номер заказа int или str
         :type position_id int or str
 
 
         """
         payload = generate_payload(**locals())
 
-        return await self._request(api.Methods.Admin.Orders.STATUS_HISTORY, payload)
+        return await self._base.request(_Methods.Admin.Orders.STATUS_HISTORY, payload)
 
     async def create_or_edit_order(
             self,
             number: Union[int, str] = None,
             internal_number: Union[int, str] = None,
             user_id: Union[int, str] = None,
             date: Union[str, datetime] = None,
@@ -287,15 +283,15 @@
             raise AbcpParameterRequired('Недостаточно параметров')
         if note is not None and del_note is not None:
             raise AbcpAPIError('Заметку можно либо удалить либо добавить')
 
         payload = generate_payload(exclude=['client_order_number', 'order_positions', 'note', 'del_note'], order=True,
                                    **locals())
 
-        return await self._request(api.Methods.Admin.Orders.SAVE_ORDER, payload, True)
+        return await self._base.request(_Methods.Admin.Orders.SAVE_ORDER, payload, True)
 
     async def get_online_order_params(
             self,
             position_ids: Union[List, str, int]
 
     ):
         """
@@ -319,15 +315,15 @@
         :type position_ids: List of ids str or int no matter
 
         """
         if not isinstance(position_ids, list):
             position_ids = [position_ids]
         payload = generate_payload(**locals())
 
-        return await self._request(api.Methods.Admin.Orders.ONLINE_ORDER, payload)
+        return await self._base.request(_Methods.Admin.Orders.ONLINE_ORDER, payload)
 
     async def send_online_order(
             self,
             order_params: Union[List[Dict], Dict],
             positions: Union[List[Dict], Dict],
     ):
         """
@@ -360,18 +356,21 @@
         if not isinstance(positions, list):
             positions = [positions]
 
         if isinstance(order_params, dict):
             order_params = [order_params]
         payload = generate_payload_online_order(**locals())
 
-        return await self._request(api.Methods.Admin.Orders.ONLINE_ORDER, payload, True)
+        return await self._base.request(_Methods.Admin.Orders.ONLINE_ORDER, payload, True)
+
 
+class Finance:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Finance(BaseAbcp):
     async def update_balance(
             self,
             user_id: Union[int, str],
             balance: Union[float, int, str],
             in_stop_list: Union[bool, str] = None
     ):
         """
@@ -390,15 +389,15 @@
         :type user_id: int or str
         :param balance: Значение баланса в валюте сайта
         :type balance: float
         :param in_stop_list: Признак нахождения клиента в стоп-листе (необязательный параметр)
         :type in_stop_list: str or bool ('true', 'false', True, False)
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Finance.UPDATE_BALANCE, payload, True)
+        return await self._base.request(_Methods.Admin.Finance.UPDATE_BALANCE, payload, True)
 
     async def update_credit_limit(
             self,
             user_id: Union[int, str],
             credit_limit: Union[float, int, str]
 
     ):
@@ -412,15 +411,15 @@
         :param user_id: Идентификатор пользователя на сайте, для которого обновляется баланс.
         :type user_id: int or str
         :param credit_limit: Значение лимита кредита в валюте сайта
         :type credit_limit: float
         """
         payload = generate_payload(**locals())
 
-        return await self._request(api.Methods.Admin.Finance.UPDATE_CREDIT_LIMIT, payload, True)
+        return await self._base.request(_Methods.Admin.Finance.UPDATE_CREDIT_LIMIT, payload, True)
 
     async def update_finance_info(
             self,
             user_id: Union[int, str],
             balance: Union[float, int, str] = None,
             credit_limit: float = None,
             in_stop_list: Union[bool, str] = None,
@@ -445,15 +444,15 @@
         :param pay_delay: Отсрочка платежа(в днях)
         :type pay_delay: int or str
         :param overdue_saldo: Просроченный баланс
         :type overdue_saldo: float
         """
         payload = generate_payload(**locals())
 
-        return await self._request(api.Methods.Admin.Finance.UPDATE_FINANCE_INFO, payload, True)
+        return await self._base.request(_Methods.Admin.Finance.UPDATE_FINANCE_INFO, payload, True)
 
     async def get_payments_info(
             self,
             user_id: Union[int, str] = None,
             payment_number: str = None,
             create_date_time_start: Union[str, datetime] = None,
             create_date_time_end: Union[str, datetime] = None
@@ -483,15 +482,15 @@
             create_date_time_end = f'{create_date_time_end:%Y-%m-%d %H:%M:%S}'
         if all(x is None for x in [user_id, payment_number, create_date_time_start, create_date_time_end]):
             raise AbcpAPIError('Недостаточно параметров')
         if payment_number is None and any(x is None for x in [create_date_time_start, create_date_time_end]):
             raise AbcpAPIError('Недостаточно параметров')
         payload = generate_payload(**locals())
 
-        return await self._request(api.Methods.Admin.Finance.GET_PAYMENTS, payload)
+        return await self._base.request(_Methods.Admin.Finance.GET_PAYMENTS, payload)
 
     async def get_payment_links(
             self,
             payment_numbers: Union[List, str, int] = None,
             order_ids: Union[List, str, int] = None,
             user_id: Union[int, str] = None,
             date_time_start: Union[str, datetime] = None,
@@ -527,15 +526,15 @@
                     f'Недостаточно параметров, укажите user_id, date_time_start, date_time_end')
         if not isinstance(order_ids, list) and order_ids is not None:
             order_ids = [order_ids]
         if not isinstance(payment_numbers, list) and payment_numbers is not None:
             payment_numbers = [payment_numbers]
         payload = generate_payload(exclude=['date_time_start', 'date_time_end'], **locals())
 
-        return await self._request(api.Methods.Admin.Finance.GET_PAYMENTS_LINKS, payload)
+        return await self._base.request(_Methods.Admin.Finance.GET_PAYMENTS_LINKS, payload)
 
     async def get_online_payments(
             self,
             date_start: Union[str, datetime] = None,
             date_end: Union[str, datetime] = None,
             customer_ids: Union[List, int] = None,
             payment_method_id: Union[int, str] = None,
@@ -571,15 +570,15 @@
         if status_ids is not None and not isinstance(status_ids, list):
             status_ids = [status_ids]
         if customer_ids is not None and not isinstance(customer_ids, list):
             customer_ids = [customer_ids]
 
         payload = generate_payload_filter(**locals())
 
-        return await self._request(api.Methods.Admin.Finance.GET_PAYMENTS_ONLINE, payload)
+        return await self._base.request(_Methods.Admin.Finance.GET_PAYMENTS_ONLINE, payload)
 
     async def add_multiple_payments(
             self,
             payments: Union[List[Dict], Dict] = None,
             link_payments: Union[bool, int] = 0
     ):
         """
@@ -594,15 +593,15 @@
         """
         if isinstance(link_payments, bool):
             link_payments = str(link_payments)
         if type(payments) is dict:
             payments = [payments]
         payload = generate_payload_payments(single=False, **locals())
 
-        return await self._request(api.Methods.Admin.Finance.ADD_PAYMENTS, payload, True)
+        return await self._base.request(_Methods.Admin.Finance.ADD_PAYMENTS, payload, True)
 
     async def add_single_payment(
             self,
             user_id: int,
             payment_type_id: int,
             amount: Union[float, int],
             create_date_time: Union[str, datetime] = None,
@@ -637,15 +636,15 @@
         if isinstance(link_payments, bool):
             link_payments = int(link_payments)
         if isinstance(create_date_time, datetime):
             create_date_time = f'{create_date_time:%Y-%m-%d %H:%M:%S}'
 
         payload = generate_payload_payments(**locals())
 
-        return await self._request(api.Methods.Admin.Finance.ADD_PAYMENTS, payload, True)
+        return await self._base.request(_Methods.Admin.Finance.ADD_PAYMENTS, payload, True)
 
     async def delete_link_payment(
             self,
             payment_link_id: int
     ):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.A3.D0.B4.D0.B0.D0.BB.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BF.D1.80.D0.B8.D0.B2.D1.8F.D0.B7.D0.BA.D0.B8_.D0.BE.D0.BF.D0.BB.D0.B0.D1.82.D1.8B
@@ -658,15 +657,15 @@
 
         :param payment_link_id: Id привязки, которую нужно удалить.
         :type payment_link_id: int or str
         """
 
         payload = generate_payload(**locals())
 
-        return await self._request(api.Methods.Admin.Finance.DELETE_PAYMENT_LINK, payload, True)
+        return await self._base.request(_Methods.Admin.Finance.DELETE_PAYMENT_LINK, payload, True)
 
     async def link_existing_payment(
             self,
             payment_id: Union[str, int],
             order_id: Union[str, int],
             amount: Union[str, int, float]
     ):
@@ -686,15 +685,15 @@
         if all(x.isdigit() for x in [payment_id, order_id, amount] if isinstance(x, str)):
             pass
         else:
             raise AbcpAPIError('Все параметры должны являться цифрами')
 
         payload = generate_payload(**locals())
 
-        return await self._request(api.Methods.Admin.Finance.LINK_EXISTING_PLAYMENT, payload, True)
+        return await self._base.request(_Methods.Admin.Finance.LINK_EXISTING_PLAYMENT, payload, True)
 
     async def refund_payment(
             self,
             refund_payment_id: Union[str, int],
             refund_amount: Union[str, int, float]
     ):
         """
@@ -706,15 +705,15 @@
         :type refund_payment_id: int or str
         :param refund_amount: Сумма возврата.
         :type refund_amount: int or str or float
         """
         if not all(x.isdigit() for x in [refund_payment_id, refund_amount] if isinstance(x, str)):
             raise AbcpAPIError('Все параметры должны являться цифрами')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Finance.REFUND_PAYMENT, payload, True)
+        return await self._base.request(_Methods.Admin.Finance.REFUND_PAYMENT, payload, True)
 
     async def get_receipts(
             self,
             shop_id: Union[int, str] = None,
             queue_id: Union[int, str] = None,
             date_created_start: Union[str, datetime] = None,
             date_created_end: Union[str, datetime] = None,
@@ -774,15 +773,15 @@
 
         """
         if isinstance(date_created_start, datetime):
             date_created_start = f'{date_created_start:%Y-%m-%d}'
         if isinstance(date_created_end, datetime):
             date_created_end = f'{date_created_end:%Y-%m-%d}'
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Finance.GET_RECEIPTS, payload)
+        return await self._base.request(_Methods.Admin.Finance.GET_RECEIPTS, payload)
 
     async def get_payments_methods(self, only_enabled: Union[bool, str] = None,
                                    only_disabled: Union[bool, str] = None,
                                    payment_method_id: Union[int, str] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.BD.D0.B0.D1.81.D1.82.D1.80.D0.BE.D0.B5.D0.BA_.D0.BF.D0.BB.D0.B0.D1.82.D1.91.D0.B6.D0.BD.D1.8B.D1.85_.D1.81.D0.B8.D1.81.D1.82.D0.B5.D0.BC
         Возвращает настройки платёжных систем.
@@ -796,18 +795,21 @@
         :param payment_method_id: id конкретной платёжной системы для которой нужно получить настройки
         :type payment_method_id: str or int
         :return:dict
         """
         if all(x is not None for x in [only_enabled, only_disabled]):
             raise AbcpAPIError('Укажите только один параметр должен быть указан only_enabled или only_disabled')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Finance.GET_PAYMENTS_SETTINGS, payload)
+        return await self._base.request(_Methods.Admin.Finance.GET_PAYMENTS_SETTINGS, payload)
+
 
+class Users:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Users(BaseAbcp):
     async def get_users(
             self,
             date_registred_start: Union[str, datetime] = None,
             date_registred_end: Union[str, datetime] = None,
             date_updated_start: Union[str, datetime] = None,
             date_updated_end: Union[str, datetime] = None,
             state: Union[str, int] = None,
@@ -880,15 +882,15 @@
         if isinstance(format, str) and format != 'p':
             raise AbcpWrongParameterError('The parameter "format" can only take the value "p" or None')
         if not isinstance(customers_ids, list) and customers_ids is not None:
             customers_ids = [customers_ids]
         if isinstance(enable_sms, str) and (enable_sms != 'true' and enable_sms != 'false'):
             raise AbcpAPIError('Параметр "enable_sms" должен быть булевым значением, либо строкой "true" или "false"')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Users.GET_USERS_LIST, payload)
+        return await self._base.request(_Methods.Admin.Users.GET_USERS_LIST, payload)
 
     async def create(
             self,
             market_type: Union[str, int],
             name: str, password: str,
             mobile: Union[str, int],
             filial_id: Union[int, str] = None,
@@ -952,15 +954,15 @@
         """
 
         if isinstance(birth_date, datetime):
             birth_date = f'{birth_date:%Y-%m-%d}'
         if isinstance(pickup_state, bool):
             pickup_state = int(pickup_state)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Users.CREATE_USER, payload, True)
+        return await self._base.request(_Methods.Admin.Users.CREATE_USER, payload, True)
 
     async def get_profiles(
             self,
             profile_id: Union[int, str] = None,
             skip: Optional[int] = None,
             limit: Optional[int] = None,
             format: str = None
@@ -978,15 +980,15 @@
         :type format: str 'distributors' or 'brands'
         """
         format_params_check = ('brands', 'distributors')
         if isinstance(format, str) and format not in format_params_check:
             raise AbcpWrongParameterError('format parameter can take values "brands" or "distributors"')
         del format_params_check
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Users.GET_PROFILES, payload)
+        return await self._base.request(_Methods.Admin.Users.GET_PROFILES, payload)
 
     async def edit_profile(
             self,
             profile_id: Union[int, str],
             code: Union[str, int] = None,
             name: str = None,
             comment: str = None,
@@ -1030,15 +1032,15 @@
                                    matrix_price_ups, distributors_price_ups]):
             raise AbcpParameterRequired("Один из опциональных параметров должен быть передан")
         if isinstance(matrix_price_ups, dict):
             matrix_price_ups = [matrix_price_ups]
         if isinstance(distributors_price_ups, dict):
             distributors_price_ups = [distributors_price_ups]
         payload = generate_payload(exclude=['matrix_price_ups', 'distributors_price_ups'], **locals())
-        return await self._request(api.Methods.Admin.Users.EDIT_PROFILE, payload, True)
+        return await self._base.request(_Methods.Admin.Users.EDIT_PROFILE, payload, True)
 
     async def edit(
             self,
             user_id: Union[str, int], business: Union[str, int] = None,
             email: str = None, name: str = None, second_name: str = None,
             surname: str = None, password: str = None,
             birth_date: Union[str, datetime] = None, city: str = None,
@@ -1112,92 +1114,92 @@
         if isinstance(birth_date, datetime):
             birth_date = f'{birth_date:%Y-%m-%d}'
         if isinstance(pickup_state, bool):
             pickup_state = int(pickup_state)
         if isinstance(enable_sms, str) and (enable_sms != 'true' and enable_sms != 'false'):
             raise AbcpAPIError('Параметр "enable_sms" должен быть булевым значением, либо строкой "true" или "false"')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Users.EDIT_USER, payload, True)
+        return await self._base.request(_Methods.Admin.Users.EDIT_USER, payload, True)
 
     async def get_user_shipment_address(self, user_id: Union[int, str]):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.B0.D0.B4.D1.80.D0.B5.D1.81.D0.BE.D0.B2_.D0.B4.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D0.BA.D0.B8
 
         Возвращает список доступных адресов доставки. Идентификатор адреса доставки необходим при отправке заказа.
 
         :param user_id: Идентификатор клиента
         :type user_id: str or int
         """
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Users.GET_USER_SHIPMENT_ADDRESS, payload)
+        return await self._base.request(_Methods.Admin.Users.GET_USER_SHIPMENT_ADDRESS, payload)
 
     async def get_shipment_address_zones(self):
         """
         Получение списка зон адресов доставки
 
         :return: Возвращает список зон адресов доставки.
         """
-        return await self._request(api.Methods.Admin.Users.GET_USER_SHIPMENT_ADDRESS_ZONES)
+        return await self._base.request(_Methods.Admin.Users.GET_USER_SHIPMENT_ADDRESS_ZONES)
 
     async def get_shipment_address_zone(self, id: int):
         """
         Получение одной зоны адресов доставки
 
         :param id: Уникальный идентификатор зоны адресов доставки
         :return: Возвращает одну зону адресов доставки по указанному уникальному идентификатору.
         """
-        return await self._request(api.Methods.Admin.Users.GET_USER_SHIPMENT_ADDRESS_ZONE.format(id))
+        return await self._base.request(_Methods.Admin.Users.GET_USER_SHIPMENT_ADDRESS_ZONE.format(id))
 
     async def update_shipment_zones(self, zones: Union[List[Dict], Dict]):
         """
         Сохранение зон адресов доставки. Универсальный метод добавления и обновления зон адресов доставки.
 
         :param zones: Массив объектов зон адресов доставки
         :return:
         """
         if isinstance(zones, dict):
             zones = [zones]
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Users.UPDATE_SHIPMENT_ZONES, payload, True)
+        return await self._base.request(_Methods.Admin.Users.UPDATE_SHIPMENT_ZONES, payload, True)
 
     async def create_shipment_zone(self, name: str, **kwargs):
         """
         Создание новой зоны адресов доставки. Метод создания одной зоны адресов доставки.
 
         :param name: Название зоны
         :param kwargs: Аргументы isOnDay{day}: int и stopTimeDay{day}: int
         :return:
         """
         if kwargs is None:
             raise AbcpParameterRequired('Необходимо передать аргументы "isOnDay{day:int}" и "stopTimeDay{day:int}"\n\n'
                                         'Например: isOnDay1=1, stopTimeDay1="15:30"')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Users.CREATE_SHIPMENT_ZONE, payload, True, json=True)
+        return await self._base.request(_Methods.Admin.Users.CREATE_SHIPMENT_ZONE, payload, True, json=True)
 
     async def update_shipment_zone(self, id: int, name: str, **kwargs):
         """
         Метод обновления данных одной зоны адресов доставки.
 
         :param id: Идентификатор обновляемой зоны
         :param name: Название зоны
         :param kwargs: Аргументы isOnDay{day}: int и stopTimeDay{day}: int
         :return:
         """
         if kwargs is None:
             raise AbcpParameterRequired('Необходимо передать аргументы "isOnDay{day:int}" и "stopTimeDay{day:int}"\n\n'
                                         'Например: isOnDay1=1, stopTimeDay1="15:30"')
-        _method = api.Methods.Admin.Users.UPDATE_SHIPMENT_ZONE.format(id)
+        _method = _Methods.Admin.Users.UPDATE_SHIPMENT_ZONE.format(id)
         del id
         payload = generate_payload(**locals())
-        return await self._request(_method, payload, True, json=True)
+        return await self._base.request(_method, payload, True, json=True)
 
     async def delete_shipment_zone(self, id: int):
-        return await self._request(api.Methods.Admin.Users.DELETE_SHIPMENT_ZONE.format(id), None, True)
+        return await self._base.request(_Methods.Admin.Users.DELETE_SHIPMENT_ZONE.format(id), None, True)
 
     async def get_updated_cars(self, date_updated_start: str = None, date_updated_end: str = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BF.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D1.89.D0.B8.D0.BA.D0.BE.D0.B2_.D0.BE.D1.84.D0.B8.D1.81.D0.B0
         Возвращает информацию об автомобилях, в которые были внесены изменения за определённый период времени.
         Если не переданы dateUpdatedStart и dateUpdatedEnd, то будет предоставлена информация за последний месяц.
 
@@ -1210,30 +1212,33 @@
         """
         if isinstance(date_updated_start, datetime):
             date_updated_start = f'{date_updated_start:%Y-%m-%d %H:%M:%S}'
 
         if isinstance(date_updated_end, datetime):
             date_updated_end = f'{date_updated_end:%Y-%m-%d %H:%M:%S}'
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Users.GET_USERS_CARS, payload)
+        return await self._base.request(_Methods.Admin.Users.GET_USERS_CARS, payload)
 
     async def get_sms_settings(self, user_ids: Union[List, int, str]):
         if not isinstance(user_ids, list):
             user_ids = [user_ids]
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Users.SMS_SETTINGS, payload)
+        return await self._base.request(_Methods.Admin.Users.SMS_SETTINGS, payload)
 
 
-class Staff(BaseAbcp):
+class Staff:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
     async def get(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D1.81.D0.BE.D1.82.D1.80.D1.83.D0.B4.D0.BD.D0.B8.D0.BA.D0.BE.D0.B2
         Возвращает список менеджеров.
         """
-        return await self._request(api.Methods.Admin.Staff.GET_STAFF)
+        return await self._base.request(_Methods.Admin.Staff.GET_STAFF)
 
     async def update_manager(self, id: int, type_id: int = None,
                              first_name: str = None, last_name: str = None,
                              email: str = None, phone: str = None, mobile: str = None,
                              sip: Union[str, int] = None, comment: str = None, boss_id: int = None, office_id: int = None):
         """
 
@@ -1255,57 +1260,66 @@
         :param boss_id: Идентификатор руководителя
         :param office_id: Идентификатор офиса
         :return:
         """
         if isinstance(sip, str) and not sip.isdigit():
             raise AbcpWrongParameterError('Параметр "SIP" должен быть числом')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Staff.UPDATE_STAFF, payload, True)
+        return await self._base.request(_Methods.Admin.Staff.UPDATE_STAFF, payload, True)
+
 
+class Statuses:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Statuses(BaseAbcp):
     async def get(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D1.81.D1.82.D0.B0.D1.82.D1.83.D1.81.D0.BE.D0.B2
         Возвращает список всех статусов позиций заказов.
         """
-        return await self._request(api.Methods.Admin.Statuses.GET_STATUSES)
+        return await self._base.request(_Methods.Admin.Statuses.GET_STATUSES)
+
 
+class Articles:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Articles(BaseAbcp):
     async def get_brands(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D1.80.D0.B0.D0.B2.D0.BE.D1.87.D0.BD.D0.B8.D0.BA.D0.B0_.D0.B1.D1.80.D0.B5.D0.BD.D0.B4.D0.BE.D0.B2
         Возвращает список всех брендов зарегистрированных в системе с их синонимами.
         """
-        return await self._request(api.Methods.Admin.Articles.GET_BRANDS)
+        return await self._base.request(_Methods.Admin.Articles.GET_BRANDS)
 
     async def get_brand_group(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D1.80.D0.B0.D0.B2.D0.BE.D1.87.D0.BD.D0.B8.D0.BA.D0.B0_.D0.B1.D1.80.D0.B5.D0.BD.D0.B4.D0.BE.D0.B2
 
         Возвращает список всех групп брендов зарегистрированных в системе.
         """
-        return await self._request(api.Methods.Admin.Articles.GET_BRANDS_GROUP)
+        return await self._base.request(_Methods.Admin.Articles.GET_BRANDS_GROUP)
 
 
-class Distributors(BaseAbcp):
+class Distributors:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
     async def get(self, distributors4mc: Union[str, int, bool] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.BF.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D1.89.D0.B8.D0.BA.D0.BE.D0.B2
         Возвращает список всех поставщиков, подключенных в ПУ/Поставщики.
 
 
         :param distributors4mc: При передаче "1" возвращает дополнительно поставщиков 4mycar"
         :type distributors4mc: str or int
         """
         if isinstance(distributors4mc, bool):
             distributors4mc = int(distributors4mc)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Distributors.GET_DISTRIBUTORS_LIST, payload)
+        return await self._base.request(_Methods.Admin.Distributors.GET_DISTRIBUTORS_LIST, payload)
 
     async def edit_status(self, distributor_id: Union[int, str], status: Union[int, bool]):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.98.D0.B7.D0.BC.D0.B5.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D1.82.D0.B0.D1.82.D1.83.D1.81.D0.B0_.D0.BF.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D1.89.D0.B8.D0.BA.D0.B0
         Изменение статуса поставщика
 
 
@@ -1314,27 +1328,27 @@
         :param status: 	1 - Вкл. / 0 - Выкл.
         :type status: str or int
         """
         if isinstance(status, bool):
             status = int(status)
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Distributors.EDIT_DISTRIBUTORS_STATUS, payload, True)
+        return await self._base.request(_Methods.Admin.Distributors.EDIT_DISTRIBUTORS_STATUS, payload, True)
 
     async def get_routes(self, distributor_id: Union[str, int]):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.BC.D0.B0.D1.80.D1.88.D1.80.D1.83.D1.82.D0.BE.D0.B2_.D0.BF.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D1.89.D0.B8.D0.BA.D0.B0
         Возвращает список всех маршрутов поставщика.
 
 
         :param distributor_id: 	Идентификатор поставщика
         :type distributor_id: str or int
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Distributors.GET_SUPPLIER_ROUTES, payload)
+        return await self._base.request(_Methods.Admin.Distributors.GET_SUPPLIER_ROUTES, payload)
 
     async def edit_route(self,
                          route_id: Union[str, int],
                          deadline: Union[str, int] = None, deadline_replace: str = None,
                          is_deadline_replace_franch_enabled: Union[str, bool] = None,
                          deadline_max: Union[str, int] = None,
                          normal_time_start: str = None, normal_time_end: str = None,
@@ -1428,15 +1442,15 @@
         """
         if supplier_code_enabled_list is not None and not isinstance(supplier_code_enabled_list, list):
             supplier_code_enabled_list = [supplier_code_enabled_list]
         if supplier_code_disabled_list is not None and isinstance(supplier_code_disabled_list, list):
             supplier_code_disabled_list = [supplier_code_disabled_list]
         payload = generate_payload(**locals())
 
-        return await self._request(api.Methods.Admin.Distributors.UPDATE_ROUTE, payload, True)
+        return await self._base.request(_Methods.Admin.Distributors.UPDATE_ROUTE, payload, True)
 
     async def edit_route_status(self, route_id: Union[str, int], status: Union[int, bool]):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.98.D0.B7.D0.BC.D0.B5.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D1.82.D0.B0.D1.82.D1.83.D1.81.D0.B0_.D0.BC.D0.B0.D1.80.D1.88.D1.80.D1.83.D1.82.D0.B0_.D0.BF.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D1.89.D0.B8.D0.BA.D0.B0
 
         Изменяет статус маршрута поставщика
 
@@ -1446,28 +1460,28 @@
         :param status:  Значение нового статуса (1-вкл., 0-выкл.)
         :type route_id: int or str
         :return: dict
         """
         if isinstance(status, bool):
             status = int(status)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Distributors.UPDATE_ROUTE_STATUS, payload, True)
+        return await self._base.request(_Methods.Admin.Distributors.UPDATE_ROUTE_STATUS, payload, True)
 
     async def delete_route(self, route_id: Union[int, str]):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.A3.D0.B4.D0.B0.D0.BB.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BC.D0.B0.D1.80.D1.88.D1.80.D1.83.D1.82.D0.B0_.D0.BF.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D1.89.D0.B8.D0.BA.D0.B0
         Удаляет маршрут поставщика.
 
 
         :param route_id:Идентификатор маршрута поставщика
         :type route_id: int or str
         :return: dict
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Distributors.DELETE_ROUTE, payload, True)
+        return await self._base.request(_Methods.Admin.Distributors.DELETE_ROUTE, payload, True)
 
     async def connect_to_office(self, office_id: Union[str, int],
                                 distributors: Union[List[Dict], Dict] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.B4.D0.BA.D0.BB.D1.8E.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BF.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D1.89.D0.B8.D0.BA.D0.BE.D0.B2_.D0.BA_.D0.BE.D1.84.D0.B8.D1.81.D1.83
 
         Подключение/отключение поставщиков к офисам
@@ -1479,28 +1493,28 @@
         :param distributors: Массив поставщиков, если параметр не передан или содержит пустое значение - отключаются все поставщики указанного офиса.
         :type distributors List[Dict] or Dict
         :return: dict
         """
         if isinstance(distributors, dict):
             distributors = [distributors]
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Distributors.EDIT_SUPPLIER_STATUS_FOR_OFFICE, payload, True)
+        return await self._base.request(_Methods.Admin.Distributors.EDIT_SUPPLIER_STATUS_FOR_OFFICE, payload, True)
 
     async def get_office_distributors(self, office_id: Union[int, str] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BF.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D1.89.D0.B8.D0.BA.D0.BE.D0.B2_.D0.BE.D1.84.D0.B8.D1.81.D0.B0
         Возвращает информацию о подключенных к офису поставщиках
 
 
         :param office_id: Идентификатор офиса. Если параметр не указан то в ответе возвращаются данные по всем офисам
         :type office_id: str or int
         :return:dict
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Distributors.GET_OFFICE_SUPPLIERS, payload)
+        return await self._base.request(_Methods.Admin.Distributors.GET_OFFICE_SUPPLIERS, payload)
 
     async def pricelist_update(self, distributor_id: Union[str, int],
                                upload_file: Union[str, BufferedReader],
                                file_type_id: Union[int, str] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Admin#.D0.97.D0.B0.D0.B3.D1.80.D1.83.D0.B7.D0.BA.D0.B0_.D0.BF.D1.80.D0.B0.D0.B9.D1.81-.D0.BB.D0.B8.D1.81.D1.82.D0.B0_.D0.BF.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D1.89.D0.B8.D0.BA.D0.B0
         В ПУ, в разделе "Поставщики"/"Обн."/"Конфигурация прайс-листа" предварительно настраивается конфигурация
@@ -1515,27 +1529,30 @@
         :type upload_file: :obj:`str` or :obj:`BufferedReader`
         :param file_type_id: Смысла от параметра пока нет (15.05.2022)
 
         :return: dict
         """
 
         payload = generate_file_payload(exclude=['upload_file'], **locals())
-        return await self._request(api.Methods.Admin.Distributors.UPLOAD_PRICE, payload, True)
+        return await self._base.request(_Methods.Admin.Distributors.UPLOAD_PRICE, payload, True)
+
 
+class Catalog:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Catalog(BaseAbcp):
     async def info(self, goods_group: str, locale: str = 'ru_RU'):
         """
 
         :param goods_group:
         :param locale:
         :return:
         """
         payload = generate_payload(exclude=['goods_group'], **locals())
-        return await self._request(api.Methods.Admin.Catalog.INFO, payload)
+        return await self._base.request(_Methods.Admin.Catalog.INFO, payload)
 
     async def search(self, goods_group: str,
                      properties: Union[List[Dict[str, str]], Dict[str, str]],
                      skip: Optional[int] = None, limit: Optional[int] = None,
                      locale: Optional[str] = None):
         """
 
@@ -1545,24 +1562,26 @@
         :param limit:
         :param locale:
         :return:
         """
         if isinstance(properties, dict):
             properties = [properties]
         payload = generate_payload(exclude=['goods_group', 'properties'], **locals())
-        return await self._request(api.Methods.Admin.Catalog.SEARCH, payload, True)
+        return await self._base.request(_Methods.Admin.Catalog.SEARCH, payload, True)
 
     async def info_batch(self, articles_catalog: Union[List[Dict[str, str]], Dict[str, str]], locale: str = 'ru_RU'):
         if isinstance(articles_catalog, dict):
             articles_catalog = [articles_catalog]
         payload = generate_payload(exclude=['articles_catalog'], **locals())
-        return await self._request(api.Methods.Admin.Catalog.INFO_BATCH, payload, True)
+        return await self._base.request(_Methods.Admin.Catalog.INFO_BATCH, payload, True)
 
 
-class UsersCatalog(BaseAbcp):
+class UsersCatalog:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
     async def upload(self, catalog_id: Union[str, int],
                      file: Union[str, BufferedReader],
                      delete_old_mode: int = 0,
                      default_attributes_hide: Union[str, bool] = 'false',
                      article_only: Union[str, bool] = 'false',
                      image_upload_mode: int = 0,
@@ -1587,37 +1606,40 @@
         if isinstance(article_only, bool):
             article_only = str(article_only).lower()
 
         if image_upload_mode == 1 and image_archive is None:
             raise AbcpWrongParameterError('Не передан архив с изображениями')
 
         payload = generate_file_payload(exclude=['file', 'image_archive', 'catalog_id'], max_size=100, **locals())
-        return await self._request(api.Methods.Admin.UsersCatalog.UPLOAD.format(catalog_id), payload, True)
+        return await self._base.request(_Methods.Admin.UsersCatalog.UPLOAD.format(catalog_id), payload, True)
+
 
+class Payment:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Payment(BaseAbcp):
     async def token(self, number: Union[str, int]):
         """
         Получение ссылки на оплату заказа
 
         :param number: Онлайн-номер заказа
         :return:
         """
         if isinstance(number, str) and not number.isdigit():
             raise AbcpWrongParameterError('Параметр "number" должен быть числом')
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Payment.TOKEN, payload)
+        return await self._base.request(_Methods.Admin.Payment.TOKEN, payload)
 
     async def top_balance_link(self, client_id: Union[str, int], amount: Union[float, int, str]):
         """
 
         :param client_id: Идентификатор клиента
         :param amount: Сумма пополнения баланса
         :return:
         """
         if isinstance(client_id, str) and not client_id.isdigit():
             raise AbcpWrongParameterError('Параметр "client_id" должен быть числом')
         if isinstance(amount, str) and not amount.isdigit():
             raise AbcpWrongParameterError('Параметр "amount" должен быть числом')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Admin.Payment.TOP_BALANCE, payload)
+        return await self._base.request(_Methods.Admin.Payment.TOP_BALANCE, payload)
```

### Comparing `aioabcpapi-1.1.5/aioabcpapi/cp/client.py` & `aioabcpapi-2.0.0/aioabcpapi/cp/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 import logging
 from typing import Dict, List, Union, Optional
 
-from .. import api
+from ..api import _Methods
 from ..base import BaseAbcp
 from ..exceptions import NotEnoughRights, AbcpAPIError, AbcpParameterRequired, AbcpWrongParameterError
 from ..utils.payload import generate_payload
 
 logger = logging.getLogger('Cp.Client')
 
 
-class ClientApi(BaseAbcp):
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.search = Search(*args)
-        self.basket = Basket(*args)
-        self.orders = Orders(*args)
-        self.user = User(*args)
-        self.garage = Garage(*args)
-        self.car_tree = CarTree(*args)
-        self.form = Form(*args)
-        self.articles = Articles(*args)
+class ClientApi:
+    def __init__(self, base: BaseAbcp):
+        """
+        Класс содержит методы клиентского интерфейса
 
+        https://www.abcp.ru/wiki/API.ABCP.Client
+        """
+        self._base = base
+        self.search = Search(base)
+        self.basket = Basket(base)
+        self.orders = Orders(base)
+        self.user = User(base)
+        self.garage = Garage(base)
+        self.car_tree = CarTree(base)
+        self.form = Form(base)
+        self.articles = Articles(base)
+
+
+class Search:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Search(BaseAbcp):
     async def brands(self, number: Union[str, int],
                      use_online_stocks: Union[bool, int] = 0,
                      locale: Optional[str] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.B8.D1.81.D0.BA_.D0.B1.D1.80.D0.B5.D0.BD.D0.B4.D0.BE.D0.B2_.D0.BF.D0.BE_.D0.BD.D0.BE.D0.BC.D0.B5.D1.80.D1.83
         Осуществляет поиск по номеру детали и возвращает массив найденных брендов, имеющих деталь с искомым номером.
         Аналог этапа выбора бренда на сайте.
@@ -37,15 +45,15 @@
         :param locale: Локаль. Задается в формате language[_territory], например, ru_RU. По умолчанию используется локаль сайта.
         :type locale: str
         :return:
         """
         if isinstance(use_online_stocks, bool):
             use_online_stocks = int(use_online_stocks)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Search.BRANDS, payload)
+        return await self._base.request(_Methods.Client.Search.BRANDS, payload)
 
     async def articles(self,
                        number: Union[str, int],
                        brand: Union[str, int],
                        use_online_stocks: Union[bool, int] = 0,
                        disable_online_filtering: Union[bool, int] = 0,
                        with_out_analogs: Union[bool, int] = 1,
@@ -66,69 +74,69 @@
         :type disable_online_filtering: str or int
         :param with_out_analogs: Флаг "исключить поиск по аналогам". По умолчанию - 0.
         :type with_out_analogs: str or int
         :param profile_id: При передаче этого параметра, поисковая выдача api-администратора формируется как для клиента с переданным профилем. Работает только под API-администратором.
         :type profile_id: str or int
         :return:
         """
-        if not self._admin and profile_id is not None:
+        if not self._base.admin and profile_id is not None:
             raise NotEnoughRights('Только API Администор может указывать Профиль пользователя')
         if isinstance(use_online_stocks, bool):
             use_online_stocks = int(use_online_stocks)
         if isinstance(disable_online_filtering, bool):
             disable_online_filtering = int(disable_online_filtering)
         if isinstance(with_out_analogs, bool):
             with_out_analogs = int(with_out_analogs)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Search.ARTICLES, payload)
+        return await self._base.request(_Methods.Client.Search.ARTICLES, payload)
 
     async def batch(self, search: Union[List[Dict], Dict], profile_id: Union[int, str] = None):
         """
         Source https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.B0.D0.BA.D0.B5.D1.82.D0.BD.D1.8B.D0.B9_.D0.B7.D0.B0.D0.BF.D1.80.D0.BE.D1.81_.D0.B1.D0.B5.D0.B7_.D1.83.D1.87.D0.B5.D1.82.D0.B0_.D0.B0.D0.BD.D0.B0.D0.BB.D0.BE.D0.B3.D0.BE.D0.B2
         Осуществляет поиск по номеру производителя и бренду детали. Возвращает массив найденных деталей.
         Внимание! Данная операция не выполняет поиск по online-складам.
 
 
         :param search: Набор искомых деталей в формате brand - number. Максимум 100 деталей.
         :type search: dict or list of dicts ({'brand': 'LuK','number': '602000600'})
         :param profile_id: При передаче этого параметра, поисковая выдача api-администратора формируется как для клиента с переданным профилем. Работает только под API-администратором.
         :type profile_id: str or int
         :return:
         """
-        if not self._admin and profile_id is not None:
+        if not self._base.admin and profile_id is not None:
             raise NotEnoughRights('Только API Администор может указывать Профиль пользователя')
         if isinstance(search, dict):
             search = [search]
         payload = generate_payload(exclude=['search'], **locals())
         # It can work with GET and POST, but the documentation specifies POST
-        return await self._request(api.Methods.Client.Search.BATCH, payload, True)
+        return await self._base.request(_Methods.Client.Search.BATCH, payload, True)
 
     async def history(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.98.D1.81.D1.82.D0.BE.D1.80.D0.B8.D1.8F_.D0.BF.D0.BE.D0.B8.D1.81.D0.BA.D0.B0
         Возвращает массив последних (не более 50) поисковых запросов текущего пользователя.
 
 
         :return: dict
         """
-        return await self._request(api.Methods.Client.Search.HISTORY)
+        return await self._base.request(_Methods.Client.Search.HISTORY)
 
     async def tips(self, number: Union[str, int], locale: Optional[str]):
         """Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.B4.D1.81.D0.BA.D0.B0.D0.B7.D0.BA.D0.B8_.D0.BF.D0.BE_.D0.BF.D0.BE.D0.B8.D1.81.D0.BA.D1.83
         Возвращает по части номера массив подходящих пар бренд - номер
 
 
         :param number:Номер (часть номера) детали
         :type number: :obj:`str` or `int`
         :param locale: Локаль. Задается в формате language[_territory], например, ru_RU. По умолчанию используется локаль сайта.
         :type locale: :obj:`str
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Search.TIPS, payload)
+        return await self._base.request(_Methods.Client.Search.TIPS, payload)
 
     async def advices(self, brand: Union[str, int], number: Union[str, int], limit: Optional[int] = 5):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.B8.D1.81.D0.BA_.D1.81.D0.BE.D0.BF.D1.83.D1.82.D1.81.D1.82.D0.B2.D1.83.D1.8E.D1.89.D0.B8.D1.85_.D1.82.D0.BE.D0.B2.D0.B0.D1.80.D0.BE.D0.B2
         Функция реализует механизм "с этим товаром покупают" на основе статистики покупки комплектов товаров.
         Типичный пример использования функции: покупатель выбрал масляный фильтр - система рекомендует остальные товары из набора для ТО.
         Или, покупатель выбрал левый передний амортизатор, система покажет правый передний.
@@ -142,15 +150,15 @@
         :type number: :obj:`Union[str, int]`
         :param limit: необязательный параметр, ограничивающий выдачу
         :type limit :obj:`int`
         :return:
         """
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Search.ADVICES, payload)
+        return await self._base.request(_Methods.Client.Search.ADVICES, payload)
 
     async def advices_batch(self, articles: Union[List[Dict], Dict], limit: Optional[int] = 5):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9C.D0.B5.D1.85.D0.B0.D0.BD.D0.B8.D0.B7.D0.BC_.22.D0.A1_.D1.8D.D1.82.D0.B8.D0.BC_.D1.82.D0.BE.D0.B2.D0.B0.D1.80.D0.BE.D0.BC_.D0.BF.D0.BE.D0.BA.D1.83.D0.BF.D0.B0.D1.8E.D1.82.22
         Функция реализует механизм "с этим товаром покупают" по нескольким товарам.
         Дополнительно можно передать параметр limit (рекомендуется = 5), ограничивающий выдачу рекомендаций.
         Параметры товаров передаются в виде JSON-массива articles из объектов с полями 'brand' и 'number'.
@@ -159,35 +167,30 @@
         :param articles:
         :param limit:
         :return:
         """
         if isinstance(articles, dict):
             articles = [articles]
         payload = generate_payload(exclude=['articles'], **locals())
-        return await self._request(api.Methods.Client.Search.ADVICES_BATCH, payload, True, json=True)
-
+        return await self._base.request(_Methods.Client.Search.ADVICES_BATCH, payload, True, json=True)
 
-class OrderParams:
-    shipment_address = None
-    shipment_method = None
-    payment_method = None
-    shipment_office = None
 
-
-class Basket(BaseAbcp):
+class Basket:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
     async def get_baskets_list(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.BA.D0.BE.D1.80.D0.B7.D0.B8.D0.BD
         Получение списка корзин
 
 
         :return: dict
         """
-        return await self._request(api.Methods.Client.Basket.BASKETS_LIST)
+        return await self._base.request(_Methods.Client.Basket.BASKETS_LIST)
 
     async def add(self, basket_positions: Union[List[Dict], Dict], basket_id: Union[int, str] = None):
         """
         Source:https://www.abcp.ru/wiki/API.ABCP.Client#.D0.94.D0.BE.D0.B1.D0.B0.D0.B2.D0.BB.D0.B5.D0.BD.D0.B8.D0.B5_.D1.82.D0.BE.D0.B2.D0.B0.D1.80.D0.BE.D0.B2_.D0.B2_.D0.BA.D0.BE.D1.80.D0.B7.D0.B8.D0.BD.D1.83._.D0.A3.D0.B4.D0.B0.D0.BB.D0.B5.D0.BD.D0.B8.D0.B5_.D1.82.D0.BE.D0.B2.D0.B0.D1.80.D0.B0_.D0.B8.D0.B7_.D0.BA.D0.BE.D1.80.D0.B7.D0.B8.D0.BD.D1.8B
 
         Осуществляет подготовку к отправке заказа на товары по номеру производителя, бренду и коду поставки или по коду детали.
         Возвращает статус добавления товара в корзину по каждой позиции.
@@ -205,29 +208,29 @@
         :type basket_id: :obj:`str` or :obj:`int`
         :return: dict
         """
         if isinstance(basket_positions, dict):
             basket_positions = [basket_positions]
         payload = generate_payload(**locals())
 
-        return await self._request(api.Methods.Client.Basket.BASKET_ADD, payload, True)
+        return await self._base.request(_Methods.Client.Basket.BASKET_ADD, payload, True)
 
     async def clear(self, basket_id: Union[int, str] = None):
         """
         Source:https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9E.D1.87.D0.B8.D1.81.D1.82.D0.BA.D0.B0_.D0.BA.D0.BE.D1.80.D0.B7.D0.B8.D0.BD.D1.8B
 
         Удаляет все позиции из корзины.
 
 
         :param basket_id: Необязательный параметр - идентификатор корзины при использовании мультикорзины
         :type basket_id: :obj:`Union[str, int]`
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Basket.BASKET_CLEAR, payload, True)
+        return await self._base.request(_Methods.Client.Basket.BASKET_CLEAR, payload, True)
 
     async def content(self, basket_id: Union[int, str] = None):
 
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D1.82.D0.BE.D0.B2.D0.B0.D1.80.D0.BE.D0.B2_.D0.B2_.D0.BA.D0.BE.D1.80.D0.B7.D0.B8.D0.BD.D0.B5
 
         Получение списка товаров в корзине
@@ -237,47 +240,47 @@
 
 
         :param basket_id: Необязательный параметр - идентификатор корзины при использовании мультикорзины
         :type basket_id: :obj:`Union[str, int]`
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Basket.BASKET_CONTENT, payload)
+        return await self._base.request(_Methods.Client.Basket.BASKET_CONTENT, payload)
 
     async def options(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BE.D0.BF.D1.86.D0.B8.D0.B9_.D0.BA.D0.BE.D1.80.D0.B7.D0.B8.D0.BD.D1.8B
 
         Получение опций корзины
         Возвращает значение некоторых опций Корзины.
 
         :return:
         """
-        return await self._request(api.Methods.Client.Basket.BASKET_OPTIONS)
+        return await self._base.request(_Methods.Client.Basket.BASKET_OPTIONS)
 
     async def payment_method(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D1.81.D0.BF.D0.BE.D1.81.D0.BE.D0.B1.D0.BE.D0.B2_.D0.BE.D0.BF.D0.BB.D0.B0.D1.82.D1.8B
 
         Получение списка способов оплаты
         Возвращает список доступных способов оплаты.
         Идентификатор способа оплаты необходим при отправке заказа (при включенной опции "Корзина: показывать тип оплаты").
         :return:
         """
-        return await self._request(api.Methods.Client.Basket.PAYMENT_METHODS)
+        return await self._base.request(_Methods.Client.Basket.PAYMENT_METHODS)
 
     async def shipment_method(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D1.81.D0.BF.D0.BE.D1.81.D0.BE.D0.B1.D0.BE.D0.B2_.D0.B4.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D0.BA.D0.B8
 
         Получение списка способов доставки
 
         :return:
         """
-        return await self._request(api.Methods.Client.Basket.SHIPMENT_METHOD)
+        return await self._base.request(_Methods.Client.Basket.SHIPMENT_METHOD)
 
     async def shipment_offices(self, offices_type: Optional[str] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.BE.D1.84.D0.B8.D1.81.D0.BE.D0.B2_.D1.81.D0.B0.D0.BC.D0.BE.D0.B2.D1.8B.D0.B2.D0.BE.D0.B7.D0.B0
 
         Получение списка офисов самовывоза
         Возвращает список доступных офисов для самовывоза.
@@ -289,26 +292,26 @@
                             order - (используется по-умолчанию) возвращает офисы используемые для оформления заказа
                             registration - возвращает офисы используемые для регистрации пользователя при включенной опции "Офисы: включить привязку к клиентам"
         :return:
         """
         if isinstance(offices_type, str) and (offices_type != 'order' or offices_type != 'registration'):
             raise AbcpParameterRequired("offices_type может принимать значения 'order' или 'registration'")
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Basket.SHIPMENT_OFFICES, payload)
+        return await self._base.request(_Methods.Client.Basket.SHIPMENT_OFFICES, payload)
 
     async def shipment_address(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.B0.D0.B4.D1.80.D0.B5.D1.81.D0.BE.D0.B2_.D0.B4.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D0.BA.D0.B8
 
         Получение списка адресов доставки
         Возвращает список доступных адресов доставки. Идентификатор адреса доставки необходим при отправке заказа.
 
         :return:
         """
-        return await self._request(api.Methods.Client.Basket.SHIPMENT_ADDRESS)
+        return await self._base.request(_Methods.Client.Basket.SHIPMENT_ADDRESS)
 
     async def shipment_dates(self, min_deadline_time: int, max_deadline_time: int,
                              shipment_address: Union[str, int] = None):
         """
         Source:https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.B4.D0.B0.D1.82_.D0.BE.D1.82.D0.B3.D1.80.D1.83.D0.B7.D0.BA.D0.B8
 
         Получение списка дат отгрузки
@@ -323,28 +326,28 @@
         Необходимо отправлять, если заказ будет оформлен с доставкой.
         Для подготовки доставки офисам может требоваться дополнительное время на сборку.
         При отправке параметра shipmentAddress получаем актуальные даты отгрузки с учетом времени комплектации в настройках офиса.
 
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Basket.SHIPMENT_DATES)
+        return await self._base.request(_Methods.Client.Basket.SHIPMENT_DATES)
 
     async def add_shipment_address(self, address: str):
         """
         Source:https://www.abcp.ru/wiki/API.ABCP.Client#.D0.94.D0.BE.D0.B1.D0.B0.D0.B2.D0.BB.D0.B5.D0.BD.D0.B8.D0.B5_.D0.B0.D0.B4.D1.80.D0.B5.D1.81.D0.B0_.D0.B4.D0.BE.D1.81.D1.82.D0.B0.D0.B2.D0.BA.D0.B8
         Добавление адреса доставки
         Для текущего покупателя добавляет "адрес доставки" и возвращает его идентификатор используемый в методе Отправка корзины в заказ
 
 
         :param address: Обязательный, строка содержащая адрес.
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Basket.SHIPMENT_DATES, payload, True)
+        return await self._base.request(_Methods.Client.Basket.SHIPMENT_DATES, payload, True)
 
     async def set_client_params(self,
                                 payment_method_index: int,
                                 shipment_address_index: int,
                                 shipment_method_index: int = None,
                                 shipment_office_index: int = None):
         """
@@ -362,43 +365,44 @@
         :type shipment_office_index: int
         :return:
         """
         try:
             if shipment_address_index != 0 and shipment_office_index is not None:
                 raise AbcpParameterRequired('Для выбора самовывоза необходимо передать "shipment_address_index=0"')
             payment_method = await self.payment_method()  # 0
-            OrderParams.payment_method = payment_method[payment_method_index]['id']
+            self._base.payment_method = payment_method[payment_method_index]['id']
             logger.info(
                 f'Выбран тип оплаты:\nID - {payment_method[payment_method_index]["id"]}\n'
                 f'Name - {payment_method[payment_method_index]["name"]}')
             if shipment_method_index is not None and shipment_address_index is not None:
                 shipment_address = await self.shipment_address()  # 1
-                OrderParams.shipment_address = shipment_address[shipment_address_index]["id"]
+                self._base.shipment_address = shipment_address[shipment_address_index]["id"]
                 logger.info(f'\n\n\n{shipment_address}\n\n\n\n')
                 logger.info(f'Выбран адрес доставки:\nID - {shipment_address[shipment_address_index]["id"]}\n'
                             f'Name - {shipment_address[shipment_address_index]["name"]}')
 
             if shipment_office_index is not None and shipment_method_index is None:
                 shipment_office = await self.shipment_offices()
-                OrderParams.shipment_office = shipment_office[shipment_office_index]["id"]
+                self._base.shipment_office = shipment_office[shipment_office_index]["id"]
                 logger.info(f'Выбран офис самовывоза:\nID - {shipment_office[shipment_office_index]["id"]}\n'
                             f'Name - {shipment_office[shipment_office_index]["name"]}\n')
             elif shipment_method_index is not None and shipment_office_index is None:
                 shipment_method = await self.shipment_method()  # 0
-                OrderParams.shipment_method = shipment_method[shipment_method_index]['id']
+                self._base.shipment_method = shipment_method[shipment_method_index]['id']
                 logger.info(f'Выбран тип доставки:\nid - {shipment_method[shipment_method_index]["id"]}\n'
                             f'Name - {shipment_method[shipment_method_index]["name"]}\n')
         except KeyError:
             raise AbcpAPIError('Неверно передан один из индексов')
         except IndexError:
             raise AbcpAPIError('Неверно передан один из индексов')
 
 
-class Orders(BaseAbcp):
-
+class Orders:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
     async def order_by_basket(self,
                               payment_method: str = None,
                               shipment_method: str = None,
                               shipment_address: str = None,
                               shipment_office: str = None,
                               shipment_date: str = None,
@@ -426,23 +430,23 @@
         :param basket_id: Необязательный параметр - идентификатор корзины при использовании мультикорзины
         :param whole_order_only: Признак - оформить заказ целиком. Принимаемые значения - 0/1. По умолчанию - 0.
         :param position_ids: Необязательный параметр - массив с номерами позиций заказа. Номера возвращает метод basket_content
         :param client_order_number: Необязательный параметр - номер заказа в системе учета клиента
         :return:
         """
         if payment_method is None:
-            payment_method = OrderParams.payment_method
+            payment_method = self._base.payment_method
         if shipment_method is None:
-            shipment_method = OrderParams.shipment_method
+            shipment_method = self._base.shipment_method
         if shipment_address is None:
-            shipment_address = OrderParams.shipment_address
+            shipment_address = self._base.shipment_address
         if shipment_office is None:
-            shipment_office = OrderParams.shipment_office
+            shipment_office = self._base.shipment_office
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Basket.BASKET_ORDER, payload, True)
+        return await self._base.request(_Methods.Client.Basket.BASKET_ORDER, payload, True)
 
     async def order_instant(self, positions: Union[List[Dict], Dict],
                             payment_method: str = None, shipment_method: str = None,
                             shipment_address: str = None, shipment_office: str = None, shipment_date: str = None,
                             comment: str = None, basket_id: str = None, whole_order_only: int = 0,
                             client_order_number: str = None):
         """
@@ -475,37 +479,37 @@
         """
         if isinstance(positions, dict):
             basket_positions = [positions]
         else:
             basket_positions = positions
         del positions
         if payment_method is None:
-            payment_method = self._payment_method
+            payment_method = self._base.payment_method
         if shipment_method is None:
-            shipment_method = self._shipment_method
+            shipment_method = self._base.shipment_method
         if shipment_address is None:
-            shipment_address = self._shipment_address
+            shipment_address = self._base.shipment_address
         if shipment_office is None:
-            shipment_office = self._shipment_office
+            shipment_office = self._base.shipment_office
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Orders.ORDERS_INSTANT, payload, True)
+        return await self._base.request(_Methods.Client.Orders.ORDERS_INSTANT, payload, True)
 
     async def orders_list(self, orders: Union[List, str, int]):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BF.D0.BE.D0.B7.D0.B8.D1.86.D0.B8.D0.B9_.D0.B7.D0.B0.D0.BA.D0.B0.D0.B7.D0.BE.D0.B2_.D1.81.D0.BE_.D1.81.D1.82.D0.B0.D1.82.D1.83.D1.81.D0.B0.D0.BC.D0.B8
 
 
         :param orders: Список номеров заказа или один номер заказа
         :type orders: :obj:`list` or :obj:`str`
         :return:
         """
         if not isinstance(orders, list):
             orders = [orders]
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Orders.GET_ORDERS_LIST, payload)
+        return await self._base.request(_Methods.Client.Orders.GET_ORDERS_LIST, payload)
 
     async def get_orders(self, format: str = None, skip: Optional[int] = None, limit: Optional[int] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.B7.D0.B0.D0.BA.D0.B0.D0.B7.D0.BE.D0.B2
         Получение списка заказов
         Осуществляет получение списка всех заказов клиента по страницам.
         Сортировка по номеру заказа по убыванию, т.е. сначала передаются самые новые заказы.
@@ -517,31 +521,34 @@
         """
         if isinstance(format, str) and format != 'p':
             raise AbcpWrongParameterError('Параметр format может принимать только значение "p"')
         if isinstance(limit, int) and not 1 <= limit <= 1000:
             raise AbcpWrongParameterError('Параметр limit может быть в диапазоне от 1 до 1000')
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Orders.GET_ORDERS, payload)
+        return await self._base.request(_Methods.Client.Orders.GET_ORDERS, payload)
 
     async def cancel_position(self, position_id: int):
         """
         Source:https://www.abcp.ru/wiki/API.ABCP.Client#.D0.97.D0.B0.D0.BF.D1.80.D0.BE.D1.81_.D0.BD.D0.B0_.D0.BE.D1.82.D0.BC.D0.B5.D0.BD.D1.83_.D0.BF.D0.BE.D0.B7.D0.B8.D1.86.D0.B8.D0.B8
         Запрос на отмену позиции
         Выставляет позиции признак "Запрос на отмену"
 
 
         :param position_id: Идентификатор позиции заказа
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Orders.CANCEL_POSITION, payload, True)
+        return await self._base.request(_Methods.Client.Orders.CANCEL_POSITION, payload, True)
 
 
-class User(BaseAbcp):
+class User:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
     async def register(self,
                        market_type: Union[str, int],
                        name: str, second_name: str, surname: str,
                        password: str, mobile: str,
                        office: Union[str, int], email: str,
                        icq: Union[str, int] = None, skype: str = None,
                        region_id: Union[int, str] = None,
@@ -602,37 +609,37 @@
         :param send_registration_email: Необязательный, по-умолчанию - 0. 1 - отправлять клиенту, менеджеру письмо о регистрации 0 - не отправлять письмо
         :param member_of_club: Название автоклуба
         :param birth_date: Дата рождения, формат YYYY-MM-DD
         :param filial_id: Код филиала (если имеются)
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.User.REGISTER, payload, True)
+        return await self._base.request(_Methods.Client.User.REGISTER, payload, True)
 
     async def activate(self, user_code: int, activation_code: Union[str, int]):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.90.D0.BA.D1.82.D0.B8.D0.B2.D0.B0.D1.86.D0.B8.D1.8F_.D0.BF.D0.BE.D0.BB.D1.8C.D0.B7.D0.BE.D0.B2.D0.B0.D1.82.D0.B5.D0.BB.D1.8F
 
 
         :param user_code: Внутренний код пользователя
         :param activation_code: Код активации
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.User.ACTIVATION, payload, True)
+        return await self._base.request(_Methods.Client.User.ACTIVATION, payload, True)
 
     async def user_info(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.B4.D0.B0.D0.BD.D0.BD.D1.8B.D1.85_.D0.BF.D0.BE.D0.BB.D1.8C.D0.B7.D0.BE.D0.B2.D0.B0.D1.82.D0.B5.D0.BB.D1.8F_.28.D0.B0.D0.B2.D1.82.D0.BE.D1.80.D0.B8.D0.B7.D0.B0.D1.86.D0.B8.D1.8F.29
         Получение данных пользователя (авторизация)
         Возвращает данные пользователя по логину и паролю.
 
         :return:
         """
-        return await self._request(api.Methods.Client.User.USER_INFO)
+        return await self._base.request(_Methods.Client.User.USER_INFO)
 
     async def restore(self, email_or_mobile: str = None, password_new: str = None, code: str = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.92.D0.BE.D1.81.D1.81.D1.82.D0.B0.D0.BD.D0.BE.D0.B2.D0.BB.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BF.D0.B0.D1.80.D0.BE.D0.BB.D1.8F
         Операция восстановление пароля пользователя.
         Восстановление пароля состоит из двух этапов:
 
@@ -649,47 +656,50 @@
         """
         if email_or_mobile is not None and any(x is not None for x in [password_new, code]):
             raise AbcpAPIError('E-mail или мобильный используется только для первого этапа восстановления.'
                                'А password_new и code для второго')
         if email_or_mobile is None and any(x is None for x in [password_new, code]):
             raise AbcpAPIError('Для второго этапа должны быть указаны password_new и code ')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.User.USER_RESTORE, payload, True)
+        return await self._base.request(_Methods.Client.User.USER_RESTORE, payload, True)
+
 
+class Garage:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Garage(BaseAbcp):
     async def get_list(self, user_id: Union[int, str] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.B0.D0.B2.D1.82.D0.BE.D0.BC.D0.BE.D0.B1.D0.B8.D0.BB.D0.B5.D0.B9_.D0.B2_.D0.B3.D0.B0.D1.80.D0.B0.D0.B6.D0.B5
         Получение списка автомобилей в гараже
 
 
         :param user_id: Указывается API администратором
         :return:
         """
-        if user_id is not None and not self._admin:
+        if user_id is not None and not self._base.admin:
             raise AbcpAPIError('Параметр "user_id" может быть передан только API администратором')
-        return await self._request(api.Methods.Client.Garage.USER_GARAGE)
+        return await self._base.request(_Methods.Client.Garage.USER_GARAGE)
 
     async def get_car(self, car_id: int, user_id: Union[int, str] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.B8.D0.BD.D1.84.D0.BE.D1.80.D0.BC.D0.B0.D1.86.D0.B8.D0.B8_.D0.BE.D0.B1_.D0.B0.D0.B2.D1.82.D0.BE.D0.BC.D0.BE.D0.B1.D0.B8.D0.BB.D0.B5_.D0.B2_.D0.B3.D0.B0.D1.80.D0.B0.D0.B6.D0.B5
         Получение информации об автомобиле в гараже
 
         Возвращает данные по одному автомобилю гаража текущего пользователя
 
 
         :param user_id: Указывается API администратором
         :param car_id: Идентификатор автомобиля в гараже
         :return:
         """
-        if user_id is not None and not self._admin:
+        if user_id is not None and not self._base.admin:
             raise AbcpAPIError('Параметр "user_id" может быть передан только API администратором')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Garage.GARAGE_CAR, payload)
+        return await self._base.request(_Methods.Client.Garage.GARAGE_CAR, payload)
 
     async def add(self, name: str,
                   comment: str = None, year: str = None, vin: str = None,
                   frame: str = None,
                   mileage: str = None,
                   manufacturer_id: Union[int, str] = None,
                   model_id: Union[int, str] = None,
@@ -711,19 +721,19 @@
         :param manufacturer_id: Идентификатор марки автомобиля
         :param model_id: Идентификатор модели автомобиля
         :param modification_id: Идентификатор модификации автомобиля
         :param vehicle_reg_plate: Государственный номер автомобиля
         :param user_id: Указывается API администратором
         :return:
         """
-        if user_id is not None and not self._admin:
+        if user_id is not None and not self._base.admin:
             raise AbcpAPIError('Параметр "user_id" может быть передан только API администратором')
         payload = generate_payload(**locals())
 
-        return await self._request(api.Methods.Client.Garage.GARAGE_ADD, payload, True)
+        return await self._base.request(_Methods.Client.Garage.GARAGE_ADD, payload, True)
 
     async def update(self, car_id: int, name: str = None,
                      comment: str = None, year: str = None, vin: str = None,
                      frame: str = None,
                      mileage: str = None,
                      manufacturer_id: Union[int, str] = None,
                      model_id: Union[int, str] = None,
@@ -748,90 +758,96 @@
         :param manufacturer_id: Идентификатор марки автомобиля
         :param model_id: Идентификатор модели автомобиля
         :param modification_id: Идентификатор модификации автомобиля
         :param vehicle_reg_plate: Государственный номер автомобиля
         :param user_id: Указывается API администратором
         :return:
         """
-        if user_id is not None and not self._admin:
+        if user_id is not None and not self._base.admin:
             raise AbcpAPIError('Параметр "user_id" может быть передан только API администратором')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Garage.GARAGE_UPDATE, payload, True)
+        return await self._base.request(_Methods.Client.Garage.GARAGE_UPDATE, payload, True)
 
     async def delete(self, car_id: int, user_id: Union[int, str] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.A3.D0.B4.D0.B0.D0.BB.D0.B5.D0.BD.D0.B8.D0.B5_.D0.B0.D0.B2.D1.82.D0.BE.D0.BC.D0.BE.D0.B1.D0.B8.D0.BB.D1.8F_.D0.B8.D0.B7_.D0.B3.D0.B0.D1.80.D0.B0.D0.B6.D0.B0
         Удаление автомобиля из гаража
 
 
         :param car_id:
         :param user_id: Указывается API администратором
         :return:
         """
-        if user_id is not None and not self._admin:
+        if user_id is not None and not self._base.admin:
             raise AbcpAPIError('Параметр "user_id" может быть передан только API администратором')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Garage.GARAGE_DELETE, payload, True)
+        return await self._base.request(_Methods.Client.Garage.GARAGE_DELETE, payload, True)
+
 
+class CarTree:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class CarTree(BaseAbcp):
     async def years(self, manufacturer_id: Union[int, str] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.94.D0.B5.D1.80.D0.B5.D0.B2.D0.BE_.D0.B0.D0.B2.D1.82.D0.BE.D0.BC.D0.BE.D0.B1.D0.B8.D0.BB.D0.B5.D0.B9
         Получение списка годов дерева автомобилей
         Возвращает список доступных годов для дерева автомобилей
 
 
         :param manufacturer_id: Идентификатор марки для фильтрации. Необязательное.
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.CarTree.CAR_TREE_YEARS, payload)
+        return await self._base.request(_Methods.Client.CarTree.CAR_TREE_YEARS, payload)
 
     async def manufacturers(self, year: int = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.BC.D0.B0.D1.80.D0.BE.D0.BA_.D0.B4.D0.B5.D1.80.D0.B5.D0.B2.D0.B0_.D0.B0.D0.B2.D1.82.D0.BE.D0.BC.D0.BE.D0.B1.D0.B8.D0.BB.D0.B5.D0.B9
         Получение списка марок дерева автомобилей
         Возвращает список доступных марок для дерева автомобилей
 
 
         :param year: Год для фильтрации марок. Необязательное.
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.CarTree.CAR_TREE_MANUFACTURERS, payload)
+        return await self._base.request(_Methods.Client.CarTree.CAR_TREE_MANUFACTURERS, payload)
 
     async def models(self, manufacturer_id: Union[int, str] = None, year: Union[int, str] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.BC.D0.BE.D0.B4.D0.B5.D0.BB.D0.B5.D0.B9_.D0.B4.D0.B5.D1.80.D0.B5.D0.B2.D0.B0_.D0.B0.D0.B2.D1.82.D0.BE.D0.BC.D0.BE.D0.B1.D0.B8.D0.BB.D0.B5.D0.B9
 
 
         :param manufacturer_id: Идентификатор марки
         :param year: Год для фильтрации моделей. Необязательное.
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.CarTree.CAR_TREE_MODELS, payload)
+        return await self._base.request(_Methods.Client.CarTree.CAR_TREE_MODELS, payload)
 
     async def modifications(self, manufacturer_id: Union[int, str] = None, model_id: Union[int, str] = None,
                             year: Union[int, str] = None):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.BC.D0.BE.D0.B4.D0.B8.D1.84.D0.B8.D0.BA.D0.B0.D1.86.D0.B8.D0.B9_.D0.B4.D0.B5.D1.80.D0.B5.D0.B2.D0.B0_.D0.B0.D0.B2.D1.82.D0.BE.D0.BC.D0.BE.D0.B1.D0.B8.D0.BB.D0.B5.D0.B9
 
 
         :param manufacturer_id: Идентификатор марки
         :param model_id: Идентификатор модели
         :param year: Год для фильтрации моделей. Необязательное.
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.CarTree.CAR_TREE_MODIFICATIONS, payload)
+        return await self._base.request(_Methods.Client.CarTree.CAR_TREE_MODIFICATIONS, payload)
 
 
-class Form(BaseAbcp):
+class Form:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
     async def fields(self, name: str, locale: str = None):
         """
         Source:  https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.BF.D0.BE.D0.BB.D0.B5.D0.B9_.D1.84.D0.BE.D1.80.D0.BC.D1.8B
         Получение списка полей формы
 
         Возвращает список полей формы и все параметры в соответствии с установленными настройками в панели управления на странице Внешний вид и контент / Формы.
         На текущий момент доступны только формы регистрации, реализованные в API-методе user/new.
@@ -840,41 +856,44 @@
         :param locale: 	Локаль формы (по умолчанию, ru_RU)
         :return:
         """
         if name not in ['registration_wholesale', 'registration_retail']:
             raise AbcpWrongParameterError(
                 "Name parameter must be one of: 'registration_wholesale', 'registration_retail'")
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.Client.Form.FIELDS, payload)
+        return await self._base.request(_Methods.Client.Form.FIELDS, payload)
+
 
+class Articles:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Articles(BaseAbcp):
     async def brands(self):
         """
         Source: https://www.abcp.ru/wiki/API.ABCP.Client#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D1.80.D0.B0.D0.B2.D0.BE.D1.87.D0.BD.D0.B8.D0.BA.D0.B0_.D0.B1.D1.80.D0.B5.D0.BD.D0.B4.D0.BE.D0.B2
         Получение справочника брендов
         Возвращает список всех брендов зарегистрированных в системе с их синонимами.
 
 
         :return:
         """
-        return await self._request(api.Methods.Client.Articles.BRANDS)
+        return await self._base.request(_Methods.Client.Articles.BRANDS)
 
     async def info(self, brand: Union[int, str], number: Union[str, int],
                    format: str, source: Union[List, str],
                    cross_image: int = None,
                    with_original: str = None,
                    locale: str = None):
-        if not self._admin:
+        if not self._base.admin:
             raise AbcpAPIError('Операция доступна только администратору API')
         if isinstance(format, str) and format not in 'bnpchmti':
             raise AbcpWrongParameterError('Параметр "format" может содержать только символы: b, n, p, c, h, m, t, i')
         if isinstance(source, str):
             source = [source]
         if isinstance(cross_image, int) and 'i' not in format:
             raise AbcpWrongParameterError('')
         if isinstance(source, list) and not all(x in ['standard', 'common', 'common_cat'] for x in source):
             raise AbcpWrongParameterError(
                 'Параметр "source" может содержать следующие флаги: standard, common, common_cat')
 
         payload = generate_payload(exclude=['cross_image', 'with_original'], **locals())
-        return await self._request(api.Methods.Client.Articles.INFO, payload)
+        return await self._base.request(_Methods.Client.Articles.INFO, payload)
```

### Comparing `aioabcpapi-1.1.5/aioabcpapi/exceptions.py` & `aioabcpapi-2.0.0/aioabcpapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.5/aioabcpapi/ts/admin.py` & `aioabcpapi-2.0.0/aioabcpapi/ts/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,241 @@
 import base64
-import logging
 import os
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Union, List, Dict, Optional
 
 import pytz
 from pyrfc3339 import generate
 
-from .. import api
+from ..api import _Methods
 from ..base import BaseAbcp
 from ..exceptions import AbcpWrongParameterError, AbcpParameterRequired
 from ..utils.fields_checker import check_fields
 from ..utils.payload import generate_payload
 
-logger = logging.getLogger('TS.Admin')
 
+class TsAdminApi:
+    def __init__(self, base: BaseAbcp):
+        """
+        Класс содержит методы административного интерфейса
+
+        https://www.abcp.ru/wiki/API.TS.Admin
+        """
+        self._base = base
+        self.order_pickings = OrderPickings(base)
+        self.customer_complaints = CustomerComplaints(base)
+        self.supplier_returns = SupplierReturns(base)
+        self.distributor_owners = DistributorOwners(base)
+        self.orders = Orders(base)
+        self.cart = Cart(base)
+        self.positions = Positions(base)
+        self.good_receipts = GoodReceipts(base)
+        self.tags = Tags(base)
+        self.tags_relationships = TagsRelationships(base)
+        self.payments = Payments(base)
+        self.payment_methods = PaymentMethods(base)
+
+
+class SupplierReturns:
+
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+        self.operations = SupplierReturnsOperations(base)
+        self.positions = SupplierReturnsPositions(base)
+        self.positions_attr = SupplierReturnsPositionsAttr(base)
+
+
+class SupplierReturnsOperations:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class TsAdminApi(BaseAbcp):
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.order_pickings = OrderPickings(*args)
-        self.customer_complaints = CustomerComplaints(*args)
-        self.distributor_owners = DistributorOwners(*args)
-        self.orders = Orders(*args)
-        self.cart = Cart(*args)
-        self.positions = Positions(*args)
-        self.good_receipts = GoodReceipts(*args)
-        self.tags = Tags(*args)
-        self.tags_relationships = TagsRelationships(*args)
-        self.payments = Payments(*args)
-        self.payment_methods = PaymentMethods(*args)
+    class _FieldsChecker:
+        list_fields = ["goodsReceipt", "agreement", "tags", ]
 
+    async def get_list(self, creator_id: int, supplier_id: int,
+                       goods_receipt_id: int,
+                       agreement_ids: Union[List[int], int],
+                       tag_ids: Union[List[int], int],
+                       sbis_statuses: Union[List[str], str],
+                       date_start: Union[datetime, str],
+                       date_end: Union[datetime, str],
+                       skip: int, limit: int, fields: Union[List, str] = None
+                       ):
+        if isinstance(agreement_ids, list):
+            agreement_ids = ','.join(map(str, tag_ids))
+        if isinstance(tag_ids, list):
+            tag_ids = ','.join(map(str, tag_ids))
+        if isinstance(sbis_statuses, list):
+            sbis_statuses = ','.join(map(str, tag_ids))
+        if isinstance(date_start, datetime):
+            date_start = generate(date_start.replace(tzinfo=pytz.utc))
+        if isinstance(date_end, datetime):
+            date_end = generate(date_end.replace(tzinfo=pytz.utc))
+        if fields is not None:
+            fields = check_fields(fields, self._FieldsChecker.list_fields)
 
-class OrderPickings(BaseAbcp):
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Operations.LIST, payload)
+
+    async def get_sum(self, creator_id: int, supplier_id: int,
+                      goods_receipt_id: int,
+                      agreement_ids: Union[List[int], int],
+                      tag_ids: Union[List[int], int],
+                      sbis_statuses: Union[List[str], str],
+                      date_start: Union[datetime, str], date_end: Union[datetime, str],
+                      skip: int = None, limit: int = None
+                      ):
+        if isinstance(agreement_ids, list):
+            agreement_ids = ','.join(map(str, agreement_ids))
+        if isinstance(tag_ids, list):
+            tag_ids = ','.join(map(str, tag_ids))
+        if isinstance(sbis_statuses, list):
+            sbis_statuses = ','.join(map(str, sbis_statuses))
+        if isinstance(date_start, datetime):
+            date_start = generate(date_start.replace(tzinfo=pytz.utc))
+        if isinstance(date_end, datetime):
+            date_end = generate(date_end.replace(tzinfo=pytz.utc))
+
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Operations.SUM, payload)
+
+    async def get(self, id: int):
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Operations.GET, payload)
+
+    async def create(self, creator_id: int, supplier_id: int,
+                     goods_receipt_id: int, agreement_id: int):
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Operations.CREATE, payload, True)
+
+    async def update(self, id: int, number: str = None, fields: Union[List, str] = None):
+        if isinstance(fields, list):
+            fields = check_fields(fields, self._FieldsChecker.list_fields)
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Operations.UPDATE, payload, True)
+
+    async def delete(self, id: int):
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Operations.DELETE, payload, True)
+
+
+class SupplierReturnsPositions:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
+    class _FieldsChecker:
+        list_fields = ["item", "location", "operationInfo", "tags",
+                       "goodsReceiptPos", "availableQuantity", "customerComplaintPos"]
+
+    async def get_list(self, op_id: int = None, status: int = None, type: int = None,
+                       goods_receipt_pos_ids: Union[List[str], str] = None,
+                       item_ids: Union[List[str], str] = None,
+                       supplier_id: str = None,
+                       goods_receipt_ids: Union[List[str], str] = None,
+                       date_start: Union[datetime, str] = None,
+                       date_end: Union[datetime, str] = None,
+                       skip: int = None,
+                       limit: int = None,
+                       fields: Union[List[str], str] = None
+                       ):
+        if isinstance(goods_receipt_pos_ids, list):
+            goods_receipt_pos_ids = ','.join(map(str, goods_receipt_pos_ids))
+        if isinstance(item_ids, list):
+            item_ids = ','.join(map(str, item_ids))
+        if isinstance(goods_receipt_ids, list):
+            goods_receipt_ids = ','.join(map(str, goods_receipt_ids))
+        if isinstance(date_start, datetime):
+            date_start = generate(date_start.replace(tzinfo=pytz.utc))
+        if isinstance(date_end, datetime):
+            date_end = generate(date_end.replace(tzinfo=pytz.utc))
+        if isinstance(fields, list):
+            fields = check_fields(fields, self._FieldsChecker.list_fields)
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Positions.LIST, payload)
+
+    async def get_sum(self, op_id: int = None, status: int = None, type: int = None,
+                      goods_receipt_pos_ids: Union[List[str], str] = None,
+                      item_ids: Union[List[str], str] = None,
+                      supplier_id: str = None,
+                      goods_receipt_ids: Union[List[str], str] = None,
+                      date_start: Union[datetime, str] = None,
+                      date_end: Union[datetime, str] = None,
+                      skip: int = None,
+                      limit: int = None,
+                      fields: Union[List[str], str] = None):
+        if isinstance(goods_receipt_pos_ids, list):
+            goods_receipt_pos_ids = ','.join(map(str, goods_receipt_pos_ids))
+        if isinstance(item_ids, list):
+            item_ids = ','.join(map(str, item_ids))
+        if isinstance(goods_receipt_ids, list):
+            goods_receipt_ids = ','.join(map(str, goods_receipt_ids))
+        if isinstance(date_start, datetime):
+            date_start = generate(date_start.replace(tzinfo=pytz.utc))
+        if isinstance(date_end, datetime):
+            date_end = generate(date_end.replace(tzinfo=pytz.utc))
+        if isinstance(fields, list):
+            fields = check_fields(fields, self._FieldsChecker.list_fields)
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Positions.SUM, payload)
+
+    async def status(self):
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Positions.STATUS)
+
+    async def get(self, id: int):
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Positions.GET, payload)
+
+    async def create_multiple(self, op_id: int, poses_data: Union[List[Dict], Dict]):
+        # TODO: PREPARE poses_data maybe we can use dataclass constructor
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Positions.CREATE_MULTIPLE, payload, True)
+
+    async def split(self, id: int, quantity: Union[int, float],
+                    fields: Union[List[str], str] = None):
+        if isinstance(fields, list):
+            fields = check_fields(fields, self._FieldsChecker.list_fields)
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Positions.SPLIT, payload, True)
+
+    async def update(self, id: int, type: int = None, loc_id: int = None, quantity: int = None,
+                     comment: str = None, fields: Union[List[str], str] = None):
+        if isinstance(fields, list):
+            fields = check_fields(fields, self._FieldsChecker.list_fields)
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Positions.UPDATE, payload, True)
+
+    async def change_status(self, id: int, status: int, fields: Union[List[str], str] = None):
+        if isinstance(fields, list):
+            fields = check_fields(fields, self._FieldsChecker.list_fields)
+
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.Positions.CHANGE_STATUS, payload, True)
+
+
+class SupplierReturnsPositionsAttr:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
+    async def create(self, id: int, attr: Dict):
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.PositionsAttr.CREATE, payload, True)
+
+    async def update(self, id: int, old_name: str, new_name, description: str):
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.PositionsAttr.UPDATE, payload, True)
+
+    async def delete(self, id: int, name: str):
+        payload = generate_payload(**locals())
+        return await self._request(_Methods.TsAdmin.SupplierReturns.PositionsAttr.DELETE, payload, True)
+
+
+class OrderPickings:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
     async def fast_get_out(self, client_id: Union[str, int], supplier_id: Union[str, int],
                            positions: Union[List[Dict], Dict], distributor_id: Union[str, int] = None,
                            route_id: Union[str, int] = None, location_id: Union[str, int] = None,
                            order_picking_reseller_data: Dict = None,
                            number: Union[str, int] = None, date: Union[datetime, str] = None,
                            ):
@@ -59,15 +257,15 @@
         :return: None
         """
         if isinstance(date, datetime):
             date = generate(date.replace(tzinfo=pytz.utc))
         if isinstance(positions, dict):
             positions = [positions]
         payload = generate_payload(exclude=['positions'], **locals())
-        return await self._request(api.Methods.TsAdmin.OrderPickings.FAST_GET_OUT, payload, True)
+        return await self._request(_Methods.TsAdmin.OrderPickings.FAST_GET_OUT, payload, True)
 
     async def get(self, id: Union[int, str] = None, client_id: Union[int, str] = None, limit: int = None,
                   skip: int = None,
                   output: str = None, auto: str = None, creator_id: Union[int, str] = None,
                   worker_id: Union[int, str] = None,
                   agreement_id: Union[int, str] = None, statuses: Union[List, str, int] = None,
                   number: int = None, date_start: Union[str, datetime] = None, date_end: Union[str, datetime] = None,
@@ -108,15 +306,15 @@
         if isinstance(date_start, datetime):
             date_start = generate(date_start.replace(tzinfo=pytz.utc))
         if isinstance(date_end, datetime):
             date_end = generate(date_end.replace(tzinfo=pytz.utc))
         if isinstance(co_old_pos_ids, (int, str)):
             co_old_pos_ids = [co_old_pos_ids]
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.OrderPickings.GET, payload, True)
+        return await self._request(_Methods.TsAdmin.OrderPickings.GET, payload, True)
 
     async def get_goods(self, op_id: Union[str, int], limit: int = None, skip: int = None,
                         output: str = None, product_id: Union[int, str] = None, item_id: Union[int, str] = None,
                         ignore_canceled: Union[int, bool] = None):
         """
         Получение списка позиций товаров операции отгрузки
 
@@ -146,15 +344,15 @@
             if ignore_canceled:
                 ignore_canceled = int(ignore_canceled)
             else:
                 ignore_canceled = None
         if isinstance(output, str) and any(x not in ["e", "o"] for x in output):
             raise AbcpWrongParameterError(f'Параметр "output" принимает флаги "e", "o"')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.OrderPickings.GET_GOODS, payload)
+        return await self._request(_Methods.TsAdmin.OrderPickings.GET_GOODS, payload)
 
     async def create_by_old_pos(self, agreement_id: Union[str, int], account_details_id: Union[str, int],
                                 loc_id: Union[str, int],
                                 pp_ids: Union[List, str, int], op_id: Union[int, str] = None,
                                 status_id: Union[int, str] = None,
                                 done_right_away: Union[int, bool] = None, output: str = None):
         """
@@ -178,15 +376,15 @@
             raise AbcpParameterRequired(
                 'При указании параметра done_right_away, status_id является обязательным и должен иметь признак списания')
         if isinstance(pp_ids, (int, str)):
             pp_ids = [pp_ids]
         if isinstance(output, str) and any(x not in ["e", "t", "s"] for x in output):
             raise AbcpWrongParameterError('Параметр "output" принимает флаги "e", "t", "s"')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.OrderPickings.CREATE_BY_OLD_POS, payload, True)
+        return await self._request(_Methods.TsAdmin.OrderPickings.CREATE_BY_OLD_POS, payload, True)
 
     async def change_status(self, id: int, operation_status_id: Union[str, int],
                             positions_status_id: Union[int, str] = None):
         """
         Изменение статуса операции отгрузка
 
         Source:  https://www.abcp.ru/wiki/API.TS.Admin#.D0.98.D0.B7.D0.BC.D0.B5.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D1.82.D0.B0.D1.82.D1.83.D1.81.D0.B0_.D0.BE.D0.BF.D0.B5.D1.80.D0.B0.D1.86.D0.B8.D0.B8_.D0.BE.D1.82.D0.B3.D1.80.D1.83.D0.B7.D0.BA.D0.B0
@@ -198,15 +396,15 @@
         """
         if operation_status_id > 5 or operation_status_id < 1:
             raise AbcpWrongParameterError('Параметр "operation_status_id" может принимать значения от 1 до 5')
         if positions_status_id is None and operation_status_id in (3, 5):
             raise AbcpWrongParameterError(
                 f'Параметр "positions_status_id" является обязательным при смене статуса операции на {operation_status_id}')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.OrderPickings.CHANGE_STATUS, payload, True)
+        return await self._request(_Methods.TsAdmin.OrderPickings.CHANGE_STATUS, payload, True)
 
     async def update(self, id: int, number: Union[str, int] = None, creator_id: Union[int, str] = None,
                      worker_id: Union[int, str] = None,
                      client_id: Union[int, str] = None,
                      agreement_id: Union[int, str] = None, account_details_id: Union[int, str] = None,
                      loc_id: Union[int, str] = None,
                      reseller_data: Dict = None):
@@ -223,36 +421,40 @@
         :param agreement_id: Идентификатор договора
         :param account_details_id: Идентификатор реквизитов магазина
         :param loc_id: Идентификатор места хранения
         :param reseller_data: Дополнительная информация в формате dict, которая будет сохранена в операцию отгрузки.
         :return:
         """
         payload = generate_payload(exclude=['reseller_data'], **locals())
-        return await self._request(api.Methods.TsAdmin.OrderPickings.UPDATE, payload, True)
+        return await self._request(_Methods.TsAdmin.OrderPickings.UPDATE, payload, True)
 
     async def delete(self, id: int):
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.OrderPickings.DELETE_POSITION, payload, True)
+        return await self._request(_Methods.TsAdmin.OrderPickings.DELETE_POSITION, payload, True)
+
 
+class CustomerComplaints:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class CustomerComplaints(BaseAbcp):
     @dataclass
     class _FieldsChecker:
         get_fields = ["orderPicking", "agreement", "tags", "posInfo"]
         get_positions_fields = ["item", "product", "location", "orderPickingInfo", "tags", "operationInfo",
                                 "supplierReturnPos"]
         update_fields = ["orderPicking", "agreement", "posInfo"]
 
     async def get(self, id: int = None, client_id: Union[int, str] = None, creator_id: Union[int, str] = None,
                   expert_id: Union[int, str] = None,
                   auto: Union[int, str] = None,
                   number: int = None, order_picking_id: Union[int, str] = None,
                   position_statuses: Union[List, int] = None,
-                  position_type: int = None, position_auto: Union[str, int] = None, date_start: str = None,
-                  date_end: str = None,
+                  position_type: int = None, position_auto: Union[str, int] = None,
+                  date_start: Union[datetime, str] = None,
+                  date_end: Union[datetime, str] = None,
                   skip: int = None, limit: int = None, fields: Union[List, str] = None):
         """
         Получение списка возвратов покупателя
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D0.B2.D0.BE.D0.B7.D0.B2.D1.80.D0.B0.D1.82.D0.BE.D0.B2_.D0.BF.D0.BE.D0.BA.D1.83.D0.BF.D0.B0.D1.82.D0.B5.D0.BB.D1.8F
 
         :param id: Идентификатор операции. При использовании вернётся одна операция, а не список.
@@ -279,15 +481,15 @@
         if isinstance(position_type, int) and (position_type < 1 or position_type > 3):
             raise AbcpWrongParameterError('position_type parameter must be between 1 and 3')
         if isinstance(position_statuses, list):
             position_statuses = ','.join(map(str, position_statuses))
         if fields is not None:
             fields = check_fields(fields, self._FieldsChecker.get_fields)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.CustomerComplaints.GET, payload)
+        return await self._request(_Methods.TsAdmin.CustomerComplaints.GET, payload)
 
     async def get_positions(self, op_id: Union[int, str] = None, order_picking_good_id: Union[int, str] = None,
                             order_picking_good_ids: Union[List, int] = None,
                             picking_ids: Union[List, int] = None,
                             old_co_position_ids: Union[List, int] = None,
                             client_id: Union[str, int] = None, old_item_id: Union[int, str] = None,
                             item_id: Union[int, str] = None,
@@ -342,15 +544,15 @@
         if isinstance(status, int) and not 1 <= status <= 8:
             raise AbcpWrongParameterError('Параметр "status" должен быть в диапазоне от 1 до 8')
         if isinstance(type, int) and not 1 <= type <= 3:
             raise AbcpWrongParameterError('Параметр "type" должен быть в диапазоне от 1 до 3')
         if fields is not None:
             fields = check_fields(fields, self._FieldsChecker.get_positions_fields)
         payload = generate_payload(exclude=['old_item_id'], **locals())
-        return await self._request(api.Methods.TsAdmin.CustomerComplaints.GET_POSITIONS, payload)
+        return await self._request(_Methods.TsAdmin.CustomerComplaints.GET_POSITIONS, payload)
 
     async def create(self, order_picking_id: Union[str, int], positions: Union[List[Dict], Dict]):
         """
         Создание возврата покупателя
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.A1.D0.BE.D0.B7.D0.B4.D0.B0.D0.BD.D0.B8.D0.B5_.D0.B2.D0.BE.D0.B7.D0.B2.D1.80.D0.B0.D1.82.D0.B0_.D0.BF.D0.BE.D0.BA.D1.83.D0.BF.D0.B0.D1.82.D0.B5.D0.BB.D1.8F
 
@@ -358,15 +560,15 @@
         :param positions: Список позиций.
         :return:
         """
         # Прощай маржинальность :(
         if isinstance(positions, dict):
             positions = [positions]
         payload = generate_payload(exclude=['positions'], **locals())
-        return await self._request(api.Methods.TsAdmin.CustomerComplaints.CREATE, payload, True)
+        return await self._request(_Methods.TsAdmin.CustomerComplaints.CREATE, payload, True)
 
     async def create_position(self, op_id: Union[str, int], order_picking_position_id: Union[str, int], quantity: int,
                               type: int, comment: str):
         """
         Создание позиции возврата покупателя
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.A1.D0.BE.D0.B7.D0.B4.D0.B0.D0.BD.D0.B8.D0.B5_.D0.BF.D0.BE.D0.B7.D0.B8.D1.86.D0.B8.D0.B8_.D0.B2.D0.BE.D0.B7.D0.B2.D1.80.D0.B0.D1.82.D0.B0_.D0.BF.D0.BE.D0.BA.D1.83.D0.BF.D0.B0.D1.82.D0.B5.D0.BB.D1.8F
@@ -377,29 +579,29 @@
         :param type: тип возврата(1-возврат, 2-отказ, 3-брак)
         :param comment:комментарий
         :return:
         """
         if not 1 <= type <= 3:
             raise AbcpWrongParameterError('Параметр "type" может принимать значения от 1 до 3')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.CustomerComplaints.CREATE_POSITION, payload, True)
+        return await self._request(_Methods.TsAdmin.CustomerComplaints.CREATE_POSITION, payload, True)
 
     async def create_position_multiple(self, positions: Union[List[Dict], Dict],
                                        customer_complaint_id: int,
                                        customer_complaint: str,
                                        custom_complaint_file: str = None):
         with open(custom_complaint_file, "rb") as ccf:
             encoded_string = base64.b64encode(ccf.read()).decode("utf-8")
         custom_complaint_file = f"{encoded_string}"
         del ccf
         del encoded_string
         if isinstance(positions, dict):
             positions = [positions]
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.CustomerComplaints.CREATE_POSITION_MULTIPLE, payload, True)
+        return await self._request(_Methods.TsAdmin.CustomerComplaints.CREATE_POSITION_MULTIPLE, payload, True)
 
     async def update_position(self, id: int, quantity: int = None, type: int = None, comment: str = None):
         """
         Изменение позиции возврата покупателя
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.98.D0.B7.D0.BC.D0.B5.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BF.D0.BE.D0.B7.D0.B8.D1.86.D0.B8.D0.B8_.D0.B2.D0.BE.D0.B7.D0.B2.D1.80.D0.B0.D1.82.D0.B0_.D0.BF.D0.BE.D0.BA.D1.83.D0.BF.D0.B0.D1.82.D0.B5.D0.BB.D1.8F
 
@@ -410,30 +612,30 @@
         :return:
         """
         if all(x is None for x in [quantity, type, comment]):
             raise AbcpParameterRequired('Один из параметров [quantity, type, comment] должен быть указан')
         if isinstance(type, int) and not 1 <= type <= 3:
             raise AbcpWrongParameterError('Параметр "type" может принимать значения от 1 до 3')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.CustomerComplaints.UPDATE_POSITION, payload, True)
+        return await self._request(_Methods.TsAdmin.CustomerComplaints.UPDATE_POSITION, payload, True)
 
     async def change_position_status(self, id: int, status: int):
         """
         Изменение статуса позиции возврата покупателя
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.98.D0.B7.D0.BC.D0.B5.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D1.82.D0.B0.D1.82.D1.83.D1.81.D0.B0_.D0.BF.D0.BE.D0.B7.D0.B8.D1.86.D0.B8.D0.B8_.D0.B2.D0.BE.D0.B7.D0.B2.D1.80.D0.B0.D1.82.D0.B0_.D0.BF.D0.BE.D0.BA.D1.83.D0.BF.D0.B0.D1.82.D0.B5.D0.BB.D1.8F
 
         :param id:
         :param status:
         :return:
         """
         if not (1 <= status <= 8):
             raise AbcpWrongParameterError('Параметр "status" может принимать значения от 1 до 8')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.CustomerComplaints.CHANGE_STATUS_POSITION, payload, True)
+        return await self._request(_Methods.TsAdmin.CustomerComplaints.CHANGE_STATUS_POSITION, payload, True)
 
     async def update(self, id: Union[str, int], number: int = None, expert_id: Union[int, str] = None,
                      custom_complaint_file: str = '',
                      fields: Union[List, str] = None):
         """
 
         :param id: [обязательный] идентификатор операции возврата покупателя
@@ -455,15 +657,15 @@
         else:
             raise TypeError('Неверно передан путь к файлу')
         if all(x is None for x in [number, expert_id]):
             raise AbcpParameterRequired('Один из параметров "number" или "expert_id" должен быть указан')
         if fields is not None:
             fields = check_fields(fields, self._FieldsChecker.update_fields)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.CustomerComplaints.UPDATE, payload, True)
+        return await self._request(_Methods.TsAdmin.CustomerComplaints.UPDATE, payload, True)
 
     async def update_custom_file(self, id: Union[int, str], custom_complaint_file: str = '',
                                  fields: Union[List, str] = None):
         """
 
         :param id: идентификатор операции возврата покупателя
         :param custom_complaint_file: (Передавать путь к файлу) форма "Заявка на возврат", файл, передавать строкой в формате base64. Если файл не передан, то будет удалён.
@@ -478,35 +680,37 @@
             del ccf
             del encoded_string
         else:
             raise TypeError('Неверно передан путь к файлу')
         if fields is not None:
             fields = check_fields(fields, self._FieldsChecker.update_fields)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.CustomerComplaints.UPDATE_CUSTOM_FILE, payload, True)
+        return await self._request(_Methods.TsAdmin.CustomerComplaints.UPDATE_CUSTOM_FILE, payload, True)
 
 
-class DistributorOwners(BaseAbcp):
+class DistributorOwners:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
     async def distributor_owners(self, distributor_id: Union[str, int]):
         """
         Получение привязанного контрагента
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BF.D1.80.D0.B8.D0.B2.D1.8F.D0.B7.D0.B0.D0.BD.D0.BD.D0.BE.D0.B3.D0.BE_.D0.BA.D0.BE.D0.BD.D1.82.D1.80.D0.B0.D0.B3.D0.B5.D0.BD.D1.82.D0.B0
 
         :param distributor_id: Идентификатор поставщика.
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.DistributorOwners.DISTRIBUTOR_OWNERS, payload)
+        return await self._request(_Methods.TsAdmin.DistributorOwners.DISTRIBUTOR_OWNERS, payload)
 
 
-class Orders(BaseAbcp):
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.messages = Messages(*args)
+class Orders:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
     class _FieldsChecker:
         fields = ["deliveries", "agreement", "tags", "posInfo", "amounts"]
 
     async def create(self, client_id: Union[str, int], number: Union[int, str] = None,
                      agreement_id: Union[int, str] = None,
                      create_time: Union[datetime, str] = None, manager_id: Union[int, str] = None,
@@ -526,15 +730,15 @@
         """
         if isinstance(create_time, datetime):
             create_time = generate(create_time.replace(tzinfo=pytz.utc))
         if fields is not None:
             fields = check_fields(fields, self._FieldsChecker.fields)
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.CREATE, payload, True)
+        return await self._request(_Methods.TsAdmin.Orders.CREATE, payload, True)
 
     async def create_by_cart(self, client_id: Union[str, int], agreement_id: Union[str, int],
                              positions: Union[List, int, str],
                              delivery_address: str, delivery_person: str, delivery_contact: str,
                              number: Union[int, str] = None,
                              create_time: Union[datetime, str] = None, manager_id: Union[int, str] = None,
                              delivery_method_id: Union[int, str] = None,
@@ -582,15 +786,15 @@
             positions = [positions]
         payload = generate_payload(
             exclude=['delivery_address', 'delivery_person', 'delivery_contact',
                      'delivery_comment', 'delivery_method_id', 'delivery_employee_person',
                      'delivery_employee_contact', 'delivery_reseller_comment', 'delivery_start_time',
                      'delivery_end_time'],
             **locals())
-        return await self._request(api.Methods.TsAdmin.Orders.CREATE_BY_CART, payload, True)
+        return await self._request(_Methods.TsAdmin.Orders.CREATE_BY_CART, payload, True)
 
     async def orders_list(self, number: int = None,
                           agreement_id: Union[int, str] = None,
                           manager_id: Union[int, str] = None,
                           delivery_id: Union[int, str] = None,
                           message: str = None,
                           date_start: Union[datetime, str] = None, date_end: Union[datetime, str] = None,
@@ -641,39 +845,39 @@
             update_date_end = generate(update_date_end.replace(tzinfo=pytz.utc))
         if isinstance(deadline_date_start, datetime):
             deadline_date_start = generate(deadline_date_start.replace(tzinfo=pytz.utc))
         if isinstance(deadline_date_end, datetime):
             deadline_date_end = generate(deadline_date_end.replace(tzinfo=pytz.utc))
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.LIST, payload)
+        return await self._request(_Methods.TsAdmin.Orders.LIST, payload)
 
     async def get(self, order_id: Union[str, int]):
         """
         Получение одного заказа
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BE.D0.B4.D0.BD.D0.BE.D0.B3.D0.BE_.D0.B7.D0.B0.D0.BA.D0.B0.D0.B7.D0.B0
 
         :param order_id: Идентификатор заказа.
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.GET, payload)
+        return await self._request(_Methods.TsAdmin.Orders.GET, payload)
 
     async def refuse(self, order_id: Union[str, int]):
         """
         Отказ от заказа
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9E.D1.82.D0.BA.D0.B0.D0.B7_.D0.BE.D1.82_.D0.B7.D0.B0.D0.BA.D0.B0.D0.B7.D0.B0
 
         :param order_id: Идентификатор заказа.
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.REFUSE, payload, True)
+        return await self._request(_Methods.TsAdmin.Orders.REFUSE, payload, True)
 
     async def update(self, order_id: Union[str, int], number: Union[str, int] = None, client_id: Union[int, str] = None,
                      agreement_id: Union[int, str] = None,
                      manager_id: Union[int, str] = None, fields: Union[List, str] = None):
         """
         Обновление заказа
 
@@ -686,15 +890,15 @@
         :param manager_id: Идентификатор сотрудника, ответственного за заказ
         :param fields: дополнительная информация ["agreement", "tags", "posInfo", "deliveries", "amounts"]
         :return:
         """
         if fields is not None:
             fields = check_fields(fields, self._FieldsChecker.fields)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.UPDATE, payload, True)
+        return await self._request(_Methods.TsAdmin.Orders.UPDATE, payload, True)
 
     async def merge(self, main_order_id: Union[str, int], merge_orders_ids: Union[List, str, int] = None,
                     fields: Union[List, str] = None):
         """
         Объединение заказов
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9E.D0.B1.D1.8A.D0.B5.D0.B4.D0.B8.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5_.D0.B7.D0.B0.D0.BA.D0.B0.D0.B7.D0.BE.D0.B2
@@ -705,15 +909,15 @@
         :return:
         """
         if isinstance(merge_orders_ids, (int, str)):
             merge_orders_ids = [merge_orders_ids]
         if fields is not None:
             fields = check_fields(fields, self._FieldsChecker.fields)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.MERGE, payload, True)
+        return await self._request(_Methods.TsAdmin.Orders.MERGE, payload, True)
 
     async def split(self, order_id: Union[str, int], position_ids: Union[List, str, int] = None,
                     fields: Union[List, str] = None):
 
         """
         Разделение заказа (В документации описан как второй метод объединения заказов)
 
@@ -725,15 +929,15 @@
         :return:
         """
         if isinstance(position_ids, (int, str)):
             position_ids = [position_ids]
         if fields is not None:
             fields = check_fields(fields, self._FieldsChecker.fields)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.SPLIT, payload, True)
+        return await self._request(_Methods.TsAdmin.Orders.SPLIT, payload, True)
 
     async def reprice(self, order_id: Union[str, int], new_sum: Union[float, int],
                       fields: Union[List, str] = None):
         """
         Изменение суммы заказа
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.98.D0.B7.D0.BC.D0.B5.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D1.83.D0.BC.D0.BC.D1.8B_.D0.B7.D0.B0.D0.BA.D0.B0.D0.B7.D0.B0
@@ -742,88 +946,91 @@
         :param new_sum: новая сумма заказа
         :param fields: дополнительная информация ["agreement", "tags", "posInfo", "deliveries", "amounts"]
         :return:
         """
         if fields is not None:
             fields = check_fields(fields, self._FieldsChecker.fields)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.REPRICE, payload, True)
+        return await self._request(_Methods.TsAdmin.Orders.REPRICE, payload, True)
 
 
-class Messages(BaseAbcp):
-    def __init__(self, *args):
-        super().__init__(*args)
+class Messages:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
     async def create(self, order_id: Union[str, int], message: str, employee_id: Union[int, str] = None):
         """
         Создание сообщения
 
         Source:  https://www.abcp.ru/wiki/API.TS.Admin#.D0.A1.D0.BE.D0.B7.D0.B4.D0.B0.D0.BD.D0.B8.D0.B5_.D1.81.D0.BE.D0.BE.D0.B1.D1.89.D0.B5.D0.BD.D0.B8.D1.8F
 
         :param order_id: Идентификатор заказа клиента
         :param message: текст сообщения
         :param employee_id: Идентификатор сотрудника (если не указано, то будет использоваться API-администратор)
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.MESSAGES_CREATE, payload, True)
+        return await self._request(_Methods.TsAdmin.Orders.MESSAGES_CREATE, payload, True)
 
     async def get_one(self, message_id: Union[str, int]):
         """
         Получение одного сообщения
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BE.D0.B4.D0.BD.D0.BE.D0.B3.D0.BE_.D1.81.D0.BE.D0.BE.D0.B1.D1.89.D0.B5.D0.BD.D0.B8.D1.8F
 
         :param message_id: Идентификатор заказа клиента
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.MESSAGES_GET_ONE, payload)
+        return await self._request(_Methods.TsAdmin.Orders.MESSAGES_GET_ONE, payload)
 
     async def get_list(self, order_id: Union[str, int], skip: int = None, limit: int = None):
         """
         Получение списка сообщений
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D1.81.D0.BE.D0.BE.D0.B1.D1.89.D0.B5.D0.BD.D0.B8.D0.B9
 
         :param order_id: Идентификатор заказа
         :param skip: количество сообщений в ответе, которое нужно пропустить
         :param limit: максимальное количество сообщений в ответе
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.MESSAGES_LIST, payload)
+        return await self._request(_Methods.TsAdmin.Orders.MESSAGES_LIST, payload)
 
     async def update(self, message_id: Union[str, int], message: str):
         """
         Редактирование сообщения
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.A0.D0.B5.D0.B4.D0.B0.D0.BA.D1.82.D0.B8.D1.80.D0.BE.D0.B2.D0.B0.D0.BD.D0.B8.D0.B5_.D1.81.D0.BE.D0.BE.D0.B1.D1.89.D0.B5.D0.BD.D0.B8.D1.8F
 
         :param message_id: Идентификатор сообщения
         :param message: текст сообщения
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.MESSAGES_UPDATE, payload, True)
+        return await self._request(_Methods.TsAdmin.Orders.MESSAGES_UPDATE, payload, True)
 
     async def delete(self, message_id: Union[str, int]):
         """
         Удаление сообщения
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.A3.D0.B4.D0.B0.D0.BB.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BE.D0.BE.D0.B1.D1.89.D0.B5.D0.BD.D0.B8.D1.8F
 
         :param message_id: Идентификатор сообщения
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Orders.MESSAGES_DELETE, payload, True)
+        return await self._request(_Methods.TsAdmin.Orders.MESSAGES_DELETE, payload, True)
+
 
+class Cart:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Cart(BaseAbcp):
     async def create(self, client_id: Union[str, int], brand: str, number: str, number_fix: Union[str, int],
                      quantity: int,
                      distributor_route_id: Union[str, int], item_key: str, agreement_id: Union[int, str] = None,
                      item_id: Union[int, str] = None):
         """
         Добавление позиции в корзину
 
@@ -837,15 +1044,15 @@
         :param distributor_route_id: идентификатор маршрута прайс-листа
         :param item_key: Код товара, полученный поиском search/articles | await api.cp.client.search.articles(602000600, 'Luk')
         :param agreement_id:идентификатор договора, если не указан, то используется активный договор с клиентом по умолчанию
         :param item_id: идентификатор партии на складе
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Cart.CREATE, payload, True)
+        return await self._request(_Methods.TsAdmin.Cart.CREATE, payload, True)
 
     async def update(self, position_id: Union[str, int], quantity: int,
                      client_id: Union[int, str] = None, guest_id: Union[int, str] = None,
                      sell_price: Union[str, float, int] = None,
                      cl_to_res_rate: Union[str, float, int] = None, cl_sell_price: Union[str, float, int] = None,
                      availability: int = None, packing: int = None, deadline: int = None, deadline_max: int = None):
         """
@@ -866,15 +1073,15 @@
         :param deadline_max: новый максимальный срок поставки
         :return:
         """
         if (client_id is None and guest_id is None) or (client_id is not None and guest_id is not None):
             raise AbcpWrongParameterError(
                 'Один и только один из параметров должен быть определён. "client_id", "guest_id"')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Cart.UPDATE, payload, True)
+        return await self._request(_Methods.TsAdmin.Cart.UPDATE, payload, True)
 
     async def get_list(self, client_id: Union[int, str] = None, guest_id: Union[int, str] = None,
                        position_ids: Union[List, str] = None,
                        agreement_id: Union[int, str] = None, skip: int = None, limit: int = None):
         """
         Получение списка позиций в корзине
 
@@ -890,15 +1097,15 @@
         """
         if isinstance(position_ids, list):
             position_ids = ','.join(map(str, position_ids))
         if (client_id is None and guest_id is None) or (client_id is not None and guest_id is not None):
             raise AbcpWrongParameterError(
                 'Один и только один из параметров должен быть определён. "client_id", "guest_id"')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Cart.GET_LIST, payload)
+        return await self._request(_Methods.TsAdmin.Cart.GET_LIST, payload)
 
     async def exist(self, client_id: Union[str, int], agreement_id: Union[str, int], brand: Union[str, int],
                     number_fix: Union[str, int]):
         """
         Проверка наличия позиции в корзине
 
         Source:
@@ -906,15 +1113,15 @@
         :param client_id: идентификатор клиента
         :param agreement_id: идентификатор договора
         :param brand: бренд
         :param number_fix: Очищенный артикул по стандарту ABCP
         :return: quantity - количество найденных позиций в корзине
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Cart.EXIST, payload)
+        return await self._request(_Methods.TsAdmin.Cart.EXIST, payload)
 
     async def summary(self, client_id: Union[int, str] = None, guest_id: Union[int, str] = None,
                       agreement_id: Union[str, int] = None):
         """
         Получение суммарной информации по позициям корзины
 
         Source:
@@ -927,15 +1134,15 @@
         if all(x is None for x in [client_id, guest_id]):
             raise AbcpWrongParameterError(
                 'Один из параметров должен быть определён. "client_id", "guest_id"')
         if client_id is not None and guest_id is not None:
             raise AbcpWrongParameterError(
                 'Один и только один из параметров должен быть определён. "client_id", "guest_id"')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Cart.SUMMARY, payload)
+        return await self._request(_Methods.TsAdmin.Cart.SUMMARY, payload)
 
     async def clear(self, agreement_id: Union[str, int], client_id: Union[int, str] = None,
                     guest_id: Union[int, str] = None):
         """
         Очистка корзины выбранного договора
 
         Source:
@@ -948,15 +1155,15 @@
         if all(x is None for x in [client_id, guest_id]):
             raise AbcpWrongParameterError(
                 'Один из параметров должен быть определён. "client_id", "guest_id"')
         if client_id is not None and guest_id is not None:
             raise AbcpWrongParameterError(
                 'Один и только один из параметров должен быть определён. "client_id", "guest_id"')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Cart.CLEAR, payload, True)
+        return await self._request(_Methods.TsAdmin.Cart.CLEAR, payload, True)
 
     async def delete_positions(self, position_ids: Union[List, str, int],
                                client_id: Union[int, str] = None, guest_id: Union[int, str] = None):
         """
         Удаление позиций корзины
 
         Source:
@@ -969,34 +1176,33 @@
         if (client_id is None and guest_id is None) or (client_id is not None and guest_id is not None):
             raise AbcpWrongParameterError(
                 'Один и только один из параметров должен быть определён. "client_id", "guest_id"')
         if not isinstance(position_ids, list):
             position_ids = [position_ids]
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Cart.DELETE, payload, True)
+        return await self._request(_Methods.TsAdmin.Cart.DELETE, payload, True)
 
     async def transfer(self, guest_id: Union[str, int], client_id: Union[str, int]):
         """
         Передача позиций корзины гостя клиенту
 
         Source:
 
         :param guest_id: идентификатор гостя
         :param client_id: идентификатор клиента
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Cart.TRANSFER, payload, True)
+        return await self._request(_Methods.TsAdmin.Cart.TRANSFER, payload, True)
 
 
-class Positions(BaseAbcp):
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.messages = PositionsMessages(*args)
+class Positions:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
     class _FieldsChecker:
         additional_info = ["reserv", "product", "orderPicking",
                            "customerComplaintPoses", "supplierOrder", "grPosition",
                            "order", "delivery", "tags", "unpaidAmount"]
         statuses = ["prepayment", "canceled", "new",
                     "supOrder", "supOrderCanceled", "reservation",
@@ -1014,15 +1220,15 @@
                            "order", "delivery", "tags", "unpaidAmount"]
         :return:
         """
         if additional_info is not None:
             additional_info = check_fields(additional_info, self._FieldsChecker.additional_info)
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.GET, payload)
+        return await self._request(_Methods.TsAdmin.Positions.GET, payload)
 
     async def get_list(self, brand: str = None, message: str = None, agreement_id: Union[int, str] = None,
                        client_id: Union[int, str] = None,
                        manager_id: Union[int, str] = None,
                        no_manager_assigned: bool = False,
                        delivery_id: Union[int, str] = None,
                        date_start: str = None, date_end: str = None, update_date_start: str = None,
@@ -1109,15 +1315,15 @@
         if isinstance(statuses, str):
             statuses = [statuses]
         if isinstance(tag_ids, list):
             tag_ids = ','.join(map(str, tag_ids))
         if statuses is not None:
             statuses = check_fields(statuses, self._FieldsChecker.statuses)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.GET_LIST, payload)
+        return await self._request(_Methods.TsAdmin.Positions.GET_LIST, payload)
 
     async def create(self, order_id: Union[str, int], client_id: Union[str, int], route_id: Union[str, int],
                      distributor_id: Union[str, int], item_key: str,
                      quantity: Union[float, int], sell_price: Union[int, float],
                      brand: Union[str, int], number_fix: str, number: Union[int, str]):
         """
         Создание позиции
@@ -1134,15 +1340,15 @@
         :param brand: бренд
         :param number_fix: номер очищенный
         :param number: номер по формату в ответе от поставщика (из результата поиска)
 
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.CREATE, payload, True)
+        return await self._request(_Methods.TsAdmin.Positions.CREATE, payload, True)
 
     async def update(self, position_id: Union[str, int], route_id: Union[int, str] = None,
                      distributor_id: Union[int, str] = None,
                      quantity: Union[int, float] = None,
                      sell_price: Union[float, int] = None, cl_to_res_rate: Union[float, int] = None,
                      cl_sell_price: Union[float, int] = None,
                      price_data_sell_price: Union[float, int] = None,
@@ -1176,41 +1382,41 @@
         if isinstance(deadline_time, datetime):
             deadline_time = generate(deadline_time.replace(tzinfo=pytz.utc))
         if isinstance(deadline_time_max, datetime):
             deadline_time_max = generate(deadline_time_max.replace(tzinfo=pytz.utc))
         if isinstance(status, str) and all(status != x for x in ['new', 'prepayment']):
             raise AbcpWrongParameterError('Параметр "status" может принимать значения "new" или "prepayment"')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.UPDATE, payload, True)
+        return await self._request(_Methods.TsAdmin.Positions.UPDATE, payload, True)
 
     async def cancel(self, position_id: Union[str, int]):
         """
         Аннулирование позиции
 
         Source:
 
         :param position_id: идентификатор позиции заказа
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.CANCEL, payload, True)
+        return await self._request(_Methods.TsAdmin.Positions.CANCEL, payload, True)
 
     async def mass_cancel(self, position_ids: Union[List, int]):
         """
         Массовое аннулирование позиций
 
         Source:
 
         :param position_ids: идентификаторы позиций через запятую
         :return:
         """
         if isinstance(position_ids, list):
             position_ids = ','.join(map(str, position_ids))
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.MASS_CANCEL, payload, True)
+        return await self._request(_Methods.TsAdmin.Positions.MASS_CANCEL, payload, True)
 
     async def change_status(self, position_ids: Union[List, int], status: str):
         """
         Массовая смена статуса позиций
 
         Source:
 
@@ -1219,74 +1425,74 @@
         :return:
         """
         if all(status != x for x in ['new', 'prepayment']):
             raise AbcpWrongParameterError('Параметр "status" может принимать значения "new" или "prepayment"')
         if isinstance(position_ids, list):
             position_ids = ','.join(map(str, position_ids))
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.CHANGE_STATUS, payload, True)
+        return await self._request(_Methods.TsAdmin.Positions.CHANGE_STATUS, payload, True)
 
     async def split(self, position_id: Union[str, int], quantity: Union[int, float]):
         """
         Разделение позиции
 
         Source:
 
         :param position_id: числовой идентификатор позиции заказа клиента
         :param quantity: количество, которое требуется отделить
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.SPLIT, payload, True)
+        return await self._request(_Methods.TsAdmin.Positions.SPLIT, payload, True)
 
     async def merge(self, main_position_id: Union[str, int], merge_positions_ids: Union[List, int]):
         """
         Объединение позиций
 
         Source:
 
         :param main_position_id:
         :param merge_positions_ids:
         :return:
         """
         if isinstance(merge_positions_ids, list):
             merge_positions_ids = ','.join(map(str, merge_positions_ids))
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.MERGE, payload, True)
+        return await self._request(_Methods.TsAdmin.Positions.MERGE, payload, True)
 
 
-class PositionsMessages(BaseAbcp):
-    def __init__(self, *args):
-        super().__init__(*args)
+class PositionsMessages:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
     async def get_list(self, position_id: Union[str, int], skip: int = None, limit: int = None):
         """
         Получение списка сообщений
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BF.D0.B8.D1.81.D0.BA.D0.B0_.D1.81.D0.BE.D0.BE.D0.B1.D1.89.D0.B5.D0.BD.D0.B8.D0.B9_2
 
         :param position_id: числовой идентификатор позиции заказа клиента
         :param skip: количество сообщений в ответе, которое нужно пропустить
         :param limit: максимальное количество сообщений, которое должно быть возвращено в ответе
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.MESSAGES_LIST, payload)
+        return await self._request(_Methods.TsAdmin.Positions.MESSAGES_LIST, payload)
 
     async def get(self, message_id: Union[str, int]):
         """
         Получение одного сообщения
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.9F.D0.BE.D0.BB.D1.83.D1.87.D0.B5.D0.BD.D0.B8.D0.B5_.D0.BE.D0.B4.D0.BD.D0.BE.D0.B3.D0.BE_.D1.81.D0.BE.D0.BE.D0.B1.D1.89.D0.B5.D0.BD.D0.B8.D1.8F_2
 
         :param message_id: числовой идентификатор сообщения
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.MESSAGES_GET, payload)
+        return await self._request(_Methods.TsAdmin.Positions.MESSAGES_GET, payload)
 
     async def create(self, position_id: Union[str, int], message: str, employee_id: Union[int, str] = None,
                      date: Union[str, datetime] = None):
         """
         Создание сообщения
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.A1.D0.BE.D0.B7.D0.B4.D0.B0.D0.BD.D0.B8.D0.B5_.D1.81.D0.BE.D0.BE.D0.B1.D1.89.D0.B5.D0.BD.D0.B8.D1.8F_2
@@ -1296,44 +1502,47 @@
         :param employee_id: идентификатор сотрудника
         :param date: дата и время. `str` в формате %Y-%m-%d %H:%M:%S или datetime object
         :return:
         """
         if isinstance(date, datetime):
             date = f'{date:%Y-%m-%d %H:%M:%S}'
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.MESSAGES_CREATE, payload, True)
+        return await self._request(_Methods.TsAdmin.Positions.MESSAGES_CREATE, payload, True)
 
     async def update(self, message_id: Union[str, int], message: str, employee_id: Union[int, str] = None):
         """
         Редактирование сообщения
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.A0.D0.B5.D0.B4.D0.B0.D0.BA.D1.82.D0.B8.D1.80.D0.BE.D0.B2.D0.B0.D0.BD.D0.B8.D0.B5_.D1.81.D0.BE.D0.BE.D0.B1.D1.89.D0.B5.D0.BD.D0.B8.D1.8F_2
 
         :param message_id: идентификатор сообщения
         :param message: текст сообщения
         :param employee_id: идентификатор сотрудника
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.MESSAGES_UPDATE, payload, True)
+        return await self._request(_Methods.TsAdmin.Positions.MESSAGES_UPDATE, payload, True)
 
     async def delete(self, message_id: Union[str, int]):
         """
         Удаление сообщения
 
         Source: https://www.abcp.ru/wiki/API.TS.Admin#.D0.A3.D0.B4.D0.B0.D0.BB.D0.B5.D0.BD.D0.B8.D0.B5_.D1.81.D0.BE.D0.BE.D0.B1.D1.89.D0.B5.D0.BD.D0.B8.D1.8F_2
 
         :param message_id: идентификатор сообщения
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Positions.MESSAGES_DELETE, payload, True)
+        return await self._request(_Methods.TsAdmin.Positions.MESSAGES_DELETE, payload, True)
+
 
+class GoodReceipts:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class GoodReceipts(BaseAbcp):
     async def create(self,
                      supplier_id: Union[str, int],
                      positions: Union[List[Dict[str, str]], Dict[str, str]],
                      sup_number: str = None, sup_shipment_date: Union[str, datetime] = None):
         """
         Создаёт приёмку с позициями. Дата создания устанавливается текущая.
 
@@ -1348,15 +1557,15 @@
         :return: id `obj`
         """
         if isinstance(sup_shipment_date, datetime):
             sup_shipment_date = f'{sup_shipment_date:%Y-%m-%d %H:%M:%S}'
         if isinstance(positions, dict):
             positions = [positions]
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.GoodReceipts.CREATE, payload, True)
+        return await self._request(_Methods.TsAdmin.GoodReceipts.CREATE, payload, True)
 
     async def get(self, limit: int = None, skip: int = None,
                   output: str = None,
                   auto: str = None,
                   creator_id: Union[str, int] = None, worker_id: Union[str, int] = None,
                   agreement_id: str = None, statuses: Union[List, int] = None,
                   number: str = None,
@@ -1394,15 +1603,15 @@
             else:
                 raise AbcpWrongParameterError('Параметр "statuses" принимет значения от 1 до 3')
         if isinstance(date_start, datetime):
             date_start = generate(date_start.replace(tzinfo=pytz.utc))
         if isinstance(date_end, datetime):
             date_end = generate(date_end.replace(tzinfo=pytz.utc))
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.GoodReceipts.GET, payload)
+        return await self._request(_Methods.TsAdmin.GoodReceipts.GET, payload)
 
     async def get_positions(self, op_id: Union[str, int], limit: int = None, skip: int = None,
                             output: str = None, product_id: Union[int, str] = None, auto: str = None):
         """
         Получение списка позиций приёмки
 
         Source:
@@ -1417,15 +1626,15 @@
         """
 
         if isinstance(limit, int) and not 1 <= limit <= 1000:
             raise AbcpWrongParameterError('Параметр "limit" должен быть в диапазоне от 1 до 1000')
         if isinstance(output, str) and output != 'e':
             raise AbcpWrongParameterError('Параметр "output" принимает только значение "e"')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.GoodReceipts.GET_POSITIONS, payload)
+        return await self._request(_Methods.TsAdmin.GoodReceipts.GET_POSITIONS, payload)
 
     async def update(self, id: int, sup_number: Union[str, int] = None, sup_shipment_date: Union[str, datetime] = None):
         """
         Операция изменения приёмки
 
         Source:
 
@@ -1434,42 +1643,42 @@
         :param sup_shipment_date: дата и время отгрузки поставщика. `str` в формате %Y-%m-%d %H:%M:%S или datetime object
         :return:
         """
 
         if isinstance(sup_shipment_date, datetime):
             sup_shipment_date = f'{sup_shipment_date:%Y-%m-%d %H:%M:%S}'
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.GoodReceipts.UPDATE, payload, True)
+        return await self._request(_Methods.TsAdmin.GoodReceipts.UPDATE, payload, True)
 
     async def change_status(self, id: int, status: int):
         """
         Операция изменения статуса приёмки
 
         Source:
 
         :param id: Идентификатор операции приёмки
         :param status: id нового статуса приёмки
         :return:
         """
         if not 1 <= status <= 3:
             raise AbcpWrongParameterError('Параметр "status" принимает значения от 1 до 3')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.GoodReceipts.CHANGE_STATUS, payload, True)
+        return await self._request(_Methods.TsAdmin.GoodReceipts.CHANGE_STATUS, payload, True)
 
     async def delete(self, id: int):
         """
         Операция удаления приёмки
 
         Source:
 
         :param id: Идентификатор операции приёмки
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.GoodReceipts.DELETE, payload, True)
+        return await self._request(_Methods.TsAdmin.GoodReceipts.DELETE, payload, True)
 
     async def create_position(self, op_id: Union[str, int], loc_id: Union[str, int], product_id: Union[str, int],
                               brand: Union[str, int], number: Union[int, str],
                               quantity: Union[float, int], sup_buy_price: Union[float, int],
                               manufacturer_country: str = None, gtd: str = None, warranty_period: int = None,
                               return_period: int = None, barcodes: Union[List, List, str, int] = None,
                               comment: str = None,
@@ -1501,39 +1710,39 @@
         :return:
         """
         if isinstance(barcodes, list):
             barcodes = ' '.join(barcodes)
         if isinstance(manufacturer_country, str) and len(manufacturer_country) != 3:
             raise AbcpWrongParameterError('Параметр manufacturer_country должен состоять из 3 английских букв')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.GoodReceipts.CREATE_POSITION, payload, True)
+        return await self._request(_Methods.TsAdmin.GoodReceipts.CREATE_POSITION, payload, True)
 
     async def delete_position(self, id: int):
         """
         Операция удаления позиции приёмки
 
         Source:
 
         :param id: Идентификатор позиции приёмки
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.GoodReceipts.DELETE_POSITION, payload, True)
+        return await self._request(_Methods.TsAdmin.GoodReceipts.DELETE_POSITION, payload, True)
 
     async def get_position(self, id: int):
         """
         Операция получения позиции приёмки
 
         Source:
 
         :param id: Идентификатор позиции приёмки
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.GoodReceipts.GET_POSITION, payload)
+        return await self._request(_Methods.TsAdmin.GoodReceipts.GET_POSITION, payload)
 
     async def update_position(self, id: int, brand: str, number: str,
                               quantity: Union[float, int], sup_buy_price: Union[float, int],
                               manufacturer_country: str = None, gtd: str = None, warranty_period: int = None,
                               return_period: int = None, barcodes: Union[List, List, str, int] = None,
                               comment: str = None,
                               descr: str = None, expected_quantity: Union[float, int] = None,
@@ -1562,30 +1771,32 @@
         :return: dict
         """
         if isinstance(barcodes, list):
             barcodes = ' '.join(map(str, barcodes))
         if isinstance(manufacturer_country, str) and len(manufacturer_country) != 3:
             raise AbcpWrongParameterError('Параметр manufacturer_country должен состоять из 3 английских букв')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.GoodReceipts.UPDATE_POSITION, payload, True)
+        return await self._request(_Methods.TsAdmin.GoodReceipts.UPDATE_POSITION, payload, True)
 
 
-class Tags(BaseAbcp):
+class Tags:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
     async def list(self, ids: Union[str, List[str], List[int]] = None):
         """
         Операция получения списка тегов
 
         :param ids: Идентификаторы тегов через запятую
         :return: dict
         """
         if isinstance(ids, list):
             ids = ','.join(map(str, ids))
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Tags.LIST, payload)
+        return await self._request(_Methods.TsAdmin.Tags.LIST, payload)
 
     async def create(self, name: str, color: str):
         """
         Операция создания тега
 
         :param name: Имя тега
         :param color: Цвет тега
@@ -1597,31 +1808,33 @@
                 del check_hex
                 color = f'#{color}'
             except ValueError as exc:
                 raise AbcpWrongParameterError(
                     'The "color" must be a hexadecimal string. It is possible to specify both with and without "#"') from exc
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Tags.CREATE, payload, True)
+        return await self._request(_Methods.TsAdmin.Tags.CREATE, payload, True)
 
     async def delete(self, id: Union[str, int]):
         """
         Операция удаления тега
 
 
         :param id: Идентификатор удаляемого тега
         :return:
         """
         if isinstance(id, str) and not id.isdigit():
             raise AbcpWrongParameterError('Параметр "id" должен быть числом')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Tags.DELETE, payload, True)
+        return await self._request(_Methods.TsAdmin.Tags.DELETE, payload, True)
 
 
-class TagsRelationships(BaseAbcp):
+class TagsRelationships:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
     async def list(self, object_ids: Union[str, List[str], List[int]] = None,
                    object_type: Union[str, int] = None,
                    group_by_object_id: Union[bool, int] = None,
                    with_all_tags: Union[bool, int] = None,
                    tags_ids: Union[str, List[str], List[int]] = None):
 
@@ -1653,15 +1866,15 @@
             raise AbcpWrongParameterError('"with_all_tags" must be in range 0-1 or use a Boolean value')
         if with_all_tags is not None and tags_ids is None:
             raise AbcpParameterRequired('The "with_all_tags" parameter must be used with the "tags_ids" parameter')
 
         if isinstance(tags_ids, list):
             tags_ids = ','.join(map(str, tags_ids))
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.TagsRelationships.LIST, payload)
+        return await self._request(_Methods.TsAdmin.TagsRelationships.LIST, payload)
 
     async def create(self, tag_id: Union[str, int], object_id: Union[str, int], object_type: Union[str, int]):
         """
         Операция создания связи тега
 
         :param tag_id: 	Идентификатор тега
         :param object_id: Идентификатор объекта
@@ -1677,15 +1890,15 @@
         if isinstance(object_type, str) and object_type.isdigit():
             if not 1 <= int(object_type) <= 13:
                 raise AbcpWrongParameterError('"object_type" must be in range 1-13')
         if isinstance(object_type, int) and not 1 <= object_type <= 13:
             raise AbcpWrongParameterError('"object_type" must be in range 1-13')
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.TagsRelationships.CREATE, payload, True)
+        return await self._request(_Methods.TsAdmin.TagsRelationships.CREATE, payload, True)
 
     async def delete(self, tag_id: Union[str, int], object_id: Union[str, int], object_type: Union[str, int]):
         """
         Операция удаления связи тега
 
         :param tag_id: 	Идентификатор тега
         :param object_id: Идентификатор объекта
@@ -1700,18 +1913,21 @@
             raise AbcpWrongParameterError('Параметр "object_id" должен быть числом')
 
         if isinstance(object_type, str) and object_type.isdigit():
             object_type = int(object_type)
         if isinstance(object_type, int) and not 1 <= object_type <= 13:
             raise AbcpWrongParameterError('"object_type" must be in range 1-13')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.TagsRelationships.DELETE, payload, True)
+        return await self._request(_Methods.TsAdmin.TagsRelationships.DELETE, payload, True)
 
 
-class Payments(BaseAbcp):
+class Payments:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
     @dataclass(frozen=True)
     class _Status:
         status = ["new", "inProcess", "accepted", "rejected", "canceled"]
 
     async def get_list(self,
                        contractor_id: Union[str, int] = None, agreement_id: Union[str, int] = None,
                        amount_start: Union[float, int, str] = None, amount_end: Union[float, int, str] = None,
@@ -1732,32 +1948,35 @@
                     f'Неверный список статусов: {status} Допустимые статусы {self._Status.status}')
             status = ','.join(status)
         if isinstance(payment_method_ids, list):
             payment_method_ids = ','.join(map(str, payment_method_ids))
         if isinstance(payment_type, list):
             payment_type = ','.join(payment_type)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Payments.GET_LIST, payload)
+        return await self._request(_Methods.TsAdmin.Payments.GET_LIST, payload)
 
     async def create(self,
                      payment_type: str, payment_method_id: int,
                      agreement_id: int, author_id: int,
                      amount: Union[float, int, str], date: Union[datetime, str],
                      contractor_id: int = None, commission: Union[float, int] = None,
                      comment: str = None, fields: Union[List[str], str] = None):
         if isinstance(date, datetime):
             date = generate(date.replace(tzinfo=pytz.utc))
         if isinstance(fields, list):
             fields = ','.join(fields)
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.Payments.CREATE, payload)
+        return await self._request(_Methods.TsAdmin.Payments.CREATE, payload)
+
 
+class PaymentMethods:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class PaymentMethods(BaseAbcp):
     @dataclass(frozen=True)
     class _Fields:
         allow_change_param = ["yes", "no", "paymentInterfaceOnly", "editOnly"]
 
     async def get_list(self,
                        payment_type: Optional[str] = None,
                        allow_change_payment: Optional[str] = None,
@@ -1773,8 +1992,8 @@
         :return:
         """
         if isinstance(allow_change_payment, str) and allow_change_payment not in self._Fields.allow_change_param:
             raise AbcpWrongParameterError(f'Неверное значение параметра "allow_change_payment" {allow_change_payment}.'
                                           f'Допустимые значения {self._Fields.allow_change_param}')
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsAdmin.PaymentMethods.METHODS_LIST, payload)
+        return await self._request(_Methods.TsAdmin.PaymentMethods.METHODS_LIST, payload)
```

### Comparing `aioabcpapi-1.1.5/aioabcpapi/ts/client.py` & `aioabcpapi-2.0.0/aioabcpapi/ts/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 import base64
-import logging
 from datetime import datetime
 from typing import Union, List, Dict
 
 import pytz
 from pyrfc3339 import generate
 
-from .. import api
+from ..api import _Methods
 from ..base import BaseAbcp
 from ..exceptions import AbcpWrongParameterError
 from ..utils.fields_checker import check_fields
 from ..utils.payload import generate_payload
 
-logger = logging.getLogger('Ts.Client')
 
 
-class TsClientApi(BaseAbcp):
-    def __init__(self, *args):
-        super().__init__(*args)
-        self.good_receipts = GoodReceipts(*args)
-        self.order_pickings = OrderPickings(*args)
-        self.customer_complaints = CustomerComplaints(*args)
-        self.orders = Orders(*args)
-        self.cart = Cart(*args)
-        self.positions = Positions(*args)
+class TsClientApi:
+    def __init__(self, base: BaseAbcp):
+        """
+        Класс содержит методы клиентского интерфейса
+
+        https://www.abcp.ru/wiki/API.TS.Client
+        """
+        self._base = base
+        self.good_receipts = GoodReceipts(base)
+        self.order_pickings = OrderPickings(base)
+        self.customer_complaints = CustomerComplaints(base)
+        self.orders = Orders(base)
+        self.cart = Cart(base)
+        self.positions = Positions(base)
 
 
-class GoodReceipts(BaseAbcp):
+class GoodReceipts:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
     async def create(self, code: Union[str, int],
                      positions: Union[List[Dict[str, str]], Dict[str, str]],
                      sup_number: str = None, sup_shipment_date: Union[str, datetime] = None):
         """
         Операция создания приёмки
 
         Source:
@@ -41,15 +47,15 @@
         :return: id `obj`
         """
         if isinstance(positions, dict):
             positions = [positions]
         payload = generate_payload(**locals())
         if isinstance(sup_shipment_date, datetime):
             sup_shipment_date = f'{sup_shipment_date:%Y-%m-%d %H:%M:%S}'
-        return await self._request(api.Methods.TsClient.GoodReceipts.CREATE, payload, True)
+        return await self._base.request(_Methods.TsClient.GoodReceipts.CREATE, payload, True)
 
     async def get(self, limit: int = None, skip: int = None,
                   output: str = None,
                   auto: str = None,
                   creator_id: Union[int, str] = None, worker_id: Union[int, str] = None,
                   agreement_id: Union[int, str] = None, statuses: Union[List, str, int] = None,
                   number: str = None,
@@ -84,15 +90,15 @@
             raise AbcpWrongParameterError('Параметр "output" должен состоять из  ["d", "e", "s"]')
         if isinstance(statuses, list):
             if all(1 <= int(x) <= 3 for x in statuses):
                 statuses = ','.join(map(str, statuses))
             else:
                 raise AbcpWrongParameterError('Параметр "statuses" принимет значения от 1 до 3')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.GoodReceipts.GET, payload)
+        return await self._base.request(_Methods.TsClient.GoodReceipts.GET, payload)
 
     async def get_positions(self, op_id: Union[str, int], limit: int = None, skip: int = None,
                             output: str = None, product_id: Union[int, str] = None, auto: str = None):
         """
         Получение списка позиций приёмки
 
         Source:
@@ -108,18 +114,21 @@
         if isinstance(limit, int) and not 1 <= limit <= 1000:
             raise AbcpWrongParameterError('Параметр "limit" может принимать значения от 1 до 1000')
         if isinstance(output, str) and output != 'e':
             raise AbcpWrongParameterError('Параметр "output" принимает только значение "e"')
         if isinstance(auto, str) and (len(auto) < 3):
             raise AbcpWrongParameterError('Параметр "auto" должен состоять минимум из 3 символов')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.GoodReceipts.GET_POSITIONS, payload)
+        return await self._base.request(_Methods.TsClient.GoodReceipts.GET_POSITIONS, payload)
+
 
+class OrderPickings:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class OrderPickings(BaseAbcp):
     async def get(self, limit: int = None, skip: int = None,
                   output: str = None, auto: Union[str, int] = None,
                   creator_id: Union[int, str] = None, worker_id: Union[int, str] = None,
                   agreement_id: Union[int, str] = None,
                   status: Union[List, str, int] = None, number: str = None,
                   date_start: Union[str, datetime] = None, date_end: Union[str, datetime] = None,
                   co_old_pos_ids: Union[List, str, int] = None):
@@ -154,15 +163,15 @@
             if all(1 <= x <= 3 for x in status):
                 statuses = ','.join(map(str, status))
             else:
                 raise AbcpWrongParameterError('Параметр "status" принимет значения от 1 до 3')
         if isinstance(output, str) and (not all(x in 'des' for x in output) or len(output) > 3):
             raise AbcpWrongParameterError('Параметр "output" должен состоять из  ["d", "e", "s"]')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.OrderPickings.GET, payload)
+        return await self._base.request(_Methods.TsClient.OrderPickings.GET, payload)
 
     async def get_positions(self, op_id: Union[str, int], limit: int = None, skip: int = None, output: str = None,
                             product_id: Union[int, str] = None,
                             item_id: Union[int, str] = None, ignore_canceled: Union[int, bool] = None):
         """
         Получение списка позиций товаров отгрузки
 
@@ -192,18 +201,21 @@
                 ignore_canceled = None
 
         if isinstance(output, str) and (not all(x in 'oe' for x in output) or len(output) > 2):
             raise AbcpWrongParameterError('Параметр "output" должен состоять из  ["o", "e"]')
         if output is not None:
             raise AbcpWrongParameterError('output must be a string')
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.OrderPickings.GET_POSITIONS, payload)
+        return await self._base.request(_Methods.TsClient.OrderPickings.GET_POSITIONS, payload)
 
 
-class CustomerComplaints(BaseAbcp):
+class CustomerComplaints:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
     class FieldsChecker:
         get_fields = ["orderPicking", "agreement", "posInfo"]
         get_positions_fields = ["product", "orderPickingInfo", "operationInfo", "supplierReturnPos"]
 
     async def get(self, auto: Union[str, int] = None, creator_id: Union[int, str] = None,
                   expert_id: Union[int, str] = None,
                   order_picking_id: Union[int, str] = None, position_statuses: Union[List, str, int] = None,
@@ -244,15 +256,15 @@
         if isinstance(tag_ids, (int, str)):
             tag_ids = [tag_ids]
         if isinstance(position_statuses, list):
             position_statuses = ','.join(map(str, position_statuses))
         if fields is not None:
             fields = check_fields(fields, self.FieldsChecker.get_fields)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.CustomerComplaints.GET, payload)
+        return await self._base.request(_Methods.TsClient.CustomerComplaints.GET, payload)
 
     async def get_positions(self, op_id: Union[str, int],
                             order_picking_good_id: Union[int, str] = None,
                             order_picking_good_ids: Union[List, str, int] = None,
                             picking_ids: Union[List, str, int] = None,
                             old_co_position_ids: Union[List, str, int] = None,
                             old_item_id: Union[int, str] = None,
@@ -308,15 +320,15 @@
             raise AbcpWrongParameterError('Параметр "type" должен быть в диапазоне от 1 до 3')
         if isinstance(output, str) and output != 'e':
             raise AbcpWrongParameterError('Параметр "output" принимает только значение "e"')
         if fields is not None:
             fields = check_fields(fields, self.FieldsChecker.get_positions_fields)
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.CustomerComplaints.GET_POSITIONS, payload)
+        return await self._base.request(_Methods.TsClient.CustomerComplaints.GET_POSITIONS, payload)
 
     async def create(self, order_picking_id: Union[str, int], positions: Union[List[Dict], Dict]):
         """
         Создание возврата покупателя
 
         Source:
 
@@ -324,62 +336,65 @@
         :param positions: список позиций
         :return:
         """
 
         if isinstance(positions, dict):
             positions = [positions]
         payload = generate_payload(exclude=['positions'], **locals())
-        return await self._request(api.Methods.TsClient.CustomerComplaints.CREATE, payload, True)
+        return await self._base.request(_Methods.TsClient.CustomerComplaints.CREATE, payload, True)
 
     async def create_position_multiple(self, positions: Union[List[Dict], Dict],
                                        customer_complaint_id: int,
                                        customer_complaint: str,
                                        custom_complaint_file: str = None):
         with open(custom_complaint_file, "rb") as ccf:
             encoded_string = base64.b64encode(ccf.read()).decode("utf-8")
         custom_complaint_file = f"{encoded_string}"
         del ccf
         del encoded_string
         if isinstance(positions, dict):
             positions = [positions]
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.CustomerComplaints.CREATE_POSITION_MULTIPLE, payload, True)
+        return await self._base.request(_Methods.TsClient.CustomerComplaints.CREATE_POSITION_MULTIPLE, payload, True)
 
     async def update_position(self, id: int, quantity: Union[str, int]):
         """
         Изменение позиции возврата покупателя
 
         Возможно изменение только количества товара позиции. Изменение возможно только в статусе "новый".
 
         Source:
 
         :param id: идентификатор позиции возврата покупателя
         :param quantity: количество
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.CustomerComplaints.UPDATE, payload, True)
+        return await self._base.request(_Methods.TsClient.CustomerComplaints.UPDATE, payload, True)
 
     async def cancel_position(self, id: int):
         """
         Отмена позиции возврата покупателя
 
         Отмена позиции возможна только в статусе "новый". Отмена позиции происходит путём изменения статуса позиции в статус 6 - аннулировано.
 
         Source:
 
         :param id: идентификатор позиции возврата покупателя
 
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.CustomerComplaints.CANCEL, payload, True)
+        return await self._base.request(_Methods.TsClient.CustomerComplaints.CANCEL, payload, True)
+
 
+class Orders:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Orders(BaseAbcp):
     async def create_by_cart(self, delivery_address: str, delivery_person: str, delivery_contact: str,
                              delivery_comment: str = None, delivery_method_id: Union[int, str] = None,
                              number: Union[str, int] = None, create_time: Union[str, datetime] = None,
                              positions: Union[List, str, int] = None):
         """
 
         :param delivery_address: адрес доставки
@@ -396,15 +411,15 @@
             create_time = generate(create_time.replace(tzinfo=pytz.utc))
         if isinstance(positions, (int, str)):
             positions = [positions]
         payload = generate_payload(
             exclude=['delivery_address', 'delivery_person',
                      'delivery_contact', 'delivery_comment', 'delivery_method_id'],
             **locals())
-        return await self._request(api.Methods.TsClient.Orders.CREATE, payload, True)
+        return await self._base.request(_Methods.TsClient.Orders.CREATE, payload, True)
 
     async def get_list(self, number: Union[str, int] = None, agreement_id: Union[int, str] = None,
                        manager_id: Union[int, str] = None,
                        delivery_id: Union[int, str] = None, brand: str = None, message: str = None,
                        date_start: Union[str, datetime] = None, date_end: Union[str, datetime] = None,
                        update_date_start: Union[str, datetime] = None, update_date_end: Union[str, datetime] = None,
                        deadline_date_start: Union[str, datetime] = None,
@@ -449,42 +464,45 @@
         if isinstance(update_date_end, datetime):
             update_date_end = generate(update_date_end.replace(tzinfo=pytz.utc))
         if isinstance(deadline_date_start, datetime):
             deadline_date_start = generate(deadline_date_start.replace(tzinfo=pytz.utc))
         if isinstance(deadline_date_end, datetime):
             deadline_date_end = generate(deadline_date_end.replace(tzinfo=pytz.utc))
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Orders.GET_LIST, payload)
+        return await self._base.request(_Methods.TsClient.Orders.GET_LIST, payload)
 
     async def get_order(self, order_id: Union[str, int]):
         """
         Получение одного заказа
 
         Source:
 
         :param order_id: Идентификатор заказа.
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Orders.GET, payload)
+        return await self._base.request(_Methods.TsClient.Orders.GET, payload)
 
     async def refuse(self, order_id: Union[str, int]):
         """
         Отказ от заказа
 
         Source:
 
         :param order_id:
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Orders.REFUSE, payload, True)
+        return await self._base.request(_Methods.TsClient.Orders.REFUSE, payload, True)
 
 
-class Cart(BaseAbcp):
+class Cart:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
     async def create(self, brand: str, number: str, quantity: int, supplier_code: Union[str, int], item_key: str,
                      agreement_id: Union[int, str] = None):
         """
         Добавление позиции в корзину
 
         Source:
 
@@ -493,28 +511,28 @@
         :param quantity: количество товара
         :param supplier_code: идентификатор маршрута прайс-листа
         :param item_key: Код товара, полученный поиском search/articles | await api.cp.client.search.articles(602000600, 'Luk')
         :param agreement_id: идентификатор договора, если не указан, то используется активный договор с клиентом по умолчанию
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Cart.CREATE, payload, True)
+        return await self._base.request(_Methods.TsClient.Cart.CREATE, payload, True)
 
     async def update(self, position_id: Union[str, int], quantity: int):
         """
         Обновление позиции в корзине
 
         Source:
 
         :param position_id: идентификатор позиции в корзине
         :param quantity: новое количество
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Cart.UPDATE, payload, True)
+        return await self._base.request(_Methods.TsClient.Cart.UPDATE, payload, True)
 
     async def get_list(self, position_ids: Union[List, str, int] = None, agreement_id: Union[int, str] = None,
                        limit: int = None,
                        skip: int = None):
         """
         Получение списка позиций в корзине
 
@@ -524,68 +542,71 @@
         :param limit: максимальное количество позиций корзины, которое должно быть возвращено в ответе
         :param skip: количество позиций корзины в ответе, которое нужно пропустить
         :return:
         """
         if isinstance(position_ids, list):
             position_ids = ','.join(map(str, position_ids))
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Cart.GET_LIST, payload, True)
+        return await self._base.request(_Methods.TsClient.Cart.GET_LIST, payload, True)
 
     async def exist(self, agreement_id: Union[str, int], brand: str, number_fix: str):
         """
         Проверка наличия позиции в корзине
 
         Source:
 
         :param agreement_id: идентификатор договора
         :param brand: бренд
         :param number_fix: артикул по стандарту ABCP
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Cart.EXIST, payload)
+        return await self._base.request(_Methods.TsClient.Cart.EXIST, payload)
 
     async def summary(self, agreement_id: Union[int, str] = None):
         """
         Получение суммарной информации по позициям корзины
 
         Source:
         :param agreement_id: идентификатор договора, если не указан, то используется активный договор с клиентом по умолчанию
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Cart.SUMMARY, payload)
+        return await self._base.request(_Methods.TsClient.Cart.SUMMARY, payload)
 
     async def clear(self, agreement_id: Union[str, int]):
         """
         Очистка корзины выбранного договора
 
         Source:
         :param agreement_id: идентификатор договора
         :return:
         """
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Cart.CLEAR, payload, True)
+        return await self._base.request(_Methods.TsClient.Cart.CLEAR, payload, True)
 
     async def delete_positions(self, position_ids: Union[List, str, int]):
         """
         Удаление позиций корзины
 
         Source:
         :param position_ids:
         :return:
         """
         if isinstance(position_ids, (int, str)):
             position_ids = [position_ids]
 
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Cart.DELETE, payload, True)
+        return await self._base.request(_Methods.TsClient.Cart.DELETE, payload, True)
+
 
+class Positions:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
 
-class Positions(BaseAbcp):
     class FieldsChecker:
         additional_info = ["delivery", "unpaidAmount"]
         statuses = ["prepayment", "canceled", "new",
                     "supOrder", "supOrderCanceled", "reservation",
                     "orderPicking", "delivery", "finished"]
 
     async def get_position(self, position_id: Union[str, int], additional_info: Union[List, str] = None):
@@ -594,15 +615,15 @@
         :param position_id: идентификатор позиции заказа
         :param additional_info: доп. информация. Значения `str` или List ["delivery", "unpaidAmount"]
         :return:
         """
         if additional_info is not None:
             additional_info = check_fields(additional_info, self.FieldsChecker.additional_info)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Positions.GET, payload)
+        return await self._base.request(_Methods.TsClient.Positions.GET, payload)
 
     async def get_list(self, brand: str = None, message: str = None, agreement_id: Union[int, str] = None,
                        manager_id: Union[int, str] = None,
                        no_manager_assigned: bool = False,
                        date_start: Union[str, datetime] = None, date_end: Union[str, datetime] = None,
                        update_date_start: Union[str, datetime] = None, update_date_end: Union[str, datetime] = None,
                        deadline_date_start: Union[str, datetime] = None, deadline_date_end: Union[str, datetime] = None,
@@ -666,24 +687,24 @@
         if isinstance(tag_ids, list):
             tag_ids = ','.join(map(str, tag_ids))
         if statuses is not None:
             statuses = check_fields(statuses, self.FieldsChecker.statuses)
         if additional_info is not None:
             additional_info = check_fields(additional_info, self.FieldsChecker.additional_info)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Positions.GET_LIST, payload)
+        return await self._base.request(_Methods.TsClient.Positions.GET_LIST, payload)
 
     async def cancel(self, position_id: Union[str, int], additional_info: Union[List, str] = None):
         """
 
         :param position_id: идентификатор позиции заказа
         :param additional_info: доп. информация. Значения `str` или List ["delivery", "unpaidAmount"]
         :return:
         """
         if additional_info is not None:
             additional_info = check_fields(additional_info, self.FieldsChecker.additional_info)
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Positions.CANCEL, payload, True)
+        return await self._base.request(_Methods.TsClient.Positions.CANCEL, payload, True)
 
     async def mass_cancel(self, position_ids: Union[List, str, int], additional_info: Union[List, str] = None):
         payload = generate_payload(**locals())
-        return await self._request(api.Methods.TsClient.Positions.MASS_CANCEL, payload, True)
+        return await self._base.request(_Methods.TsClient.Positions.MASS_CANCEL, payload, True)
```

### Comparing `aioabcpapi-1.1.5/aioabcpapi/utils/fields_checker.py` & `aioabcpapi-2.0.0/aioabcpapi/utils/fields_checker.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.5/aioabcpapi/utils/payload.py` & `aioabcpapi-2.0.0/aioabcpapi/utils/payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,12 +212,13 @@
         if key in exclude and key != '' and value is not None:
             if isinstance(value, BufferedReader):
                 data.add_field(get_camel_case_key(key), value, filename=value.name, content_type='multipart/form-data')
             if isinstance(value, str) and not value.isdigit():
                 with open(value, 'rb') as file:
                     if max_size is not None:
                         size = file.seek(0, os.SEEK_END)
-                        if (size / 1_048_576) > max_size: raise FileSizeExceeded('Файл не может быть больше 100 Мб')
+                        if (size / 1_048_576) > max_size: raise FileSizeExceeded(
+                            f'Файл не может быть больше {max_size} Мб')
                     data.add_field(get_camel_case_key(key), file, filename=file.name,
                                    content_type='multipart/form-data')
     logger.debug(f'{data}')
     return data
```

### Comparing `aioabcpapi-1.1.5/aioabcpapi.egg-info/PKG-INFO` & `aioabcpapi-2.0.0/aioabcpapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 1.1.5
+Version: 2.0.0
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,17 +18,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## AioAbcpApi
 
-Async library for [API ABCP](https://www.abcp.ru/wiki/ABCP.API "API ABCP")
-with [asyncio](https://docs.python.org/3/library/asyncio.html "asyncio")
-and [aiohttp](https://github.com/aio-libs/aiohttp "aiohttp")
+Асинхронная библиотека для [API ABCP](https://www.abcp.ru/wiki/ABCP.API "API ABCP")
+с [asyncio](https://docs.python.org/3/library/asyncio.html "asyncio")
+и [aiohttp](https://github.com/aio-libs/aiohttp "aiohttp")
 
 ![](https://img.shields.io/github/stars/bl4ckm45k/aioabcpapi.svg)
 ![](https://img.shields.io/github/forks/bl4ckm45k/aioabcpapi.svg)
 ![](https://img.shields.io/github/issues/bl4ckm45k/aioabcpapi.svg)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/aioabcpapi.svg)](https://pypi.python.org/pypi/aioabcpapi)
 [![Downloads](https://img.shields.io/pypi/dm/aioabcpapi.svg?)](https://pypi.python.org/pypi/aioabcpapi)
 [![PyPi Package Version](https://img.shields.io/pypi/v/aioabcpapi)](https://pypi.python.org/pypi/aioabcpapi)
```

### Comparing `aioabcpapi-1.1.5/aioabcpapi.egg-info/SOURCES.txt` & `aioabcpapi-2.0.0/aioabcpapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.5/setup.py` & `aioabcpapi-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import sys
 
 from setuptools import setup
+from pip._vendor.pkg_resources import parse_version
+import aioabcpapi
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 requirements = ["aiohttp>=3.8.3", "certifi>=2022.12.7", "ujson>=5.7.0", "pytz>=2022.7.1", "pyrfc3339"]
-
+parsed_version = parse_version(aioabcpapi.__version__)
 setup(
     name='aioabcpapi',
-    version='1.1.5',
+    version=parsed_version,
     author='bl4ckm45k',
     author_email='nonpowa@gmail.com',
     description='Async library for ABCP API',
     long_description_content_type="text/markdown",
     url="https://github.com/bl4ckm45k/aioabcpapi",
     license="MIT",
     packages=['aioabcpapi', 'aioabcpapi/cp', 'aioabcpapi/ts', 'aioabcpapi/utils'],
```

### Comparing `aioabcpapi-1.1.5/test/test_payload.py` & `aioabcpapi-2.0.0/test/test_payload.py`

 * *Files identical despite different names*

