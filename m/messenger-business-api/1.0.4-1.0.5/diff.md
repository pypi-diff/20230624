# Comparing `tmp/messenger-business-api-1.0.4.tar.gz` & `tmp/messenger-business-api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messenger-business-api-1.0.4.tar", last modified: Fri Jun 23 22:37:51 2023, max compression
+gzip compressed data, was "messenger-business-api-1.0.5.tar", last modified: Fri Jun 23 22:43:29 2023, max compression
```

## Comparing `messenger-business-api-1.0.4.tar` & `messenger-business-api-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:37:51.529623 messenger-business-api-1.0.4/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1066 2023-05-22 21:38:39.000000 messenger-business-api-1.0.4/LICENSE
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:37:51.529623 messenger-business-api-1.0.4/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1039 2023-06-23 22:11:44.000000 messenger-business-api-1.0.4/README.rst
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:37:51.529623 messenger-business-api-1.0.4/messenger_business_api/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       82 2023-06-23 22:08:52.000000 messenger-business-api-1.0.4/messenger_business_api/__init__.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1098 2023-06-23 22:37:40.000000 messenger-business-api-1.0.4/messenger_business_api/api.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      342 2023-06-19 22:14:04.000000 messenger-business-api-1.0.4/messenger_business_api/execeptions.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      193 2023-06-23 22:37:23.000000 messenger-business-api-1.0.4/messenger_business_api/types.py
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:37:51.529623 messenger-business-api-1.0.4/messenger_business_api.egg-info/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:37:51.000000 messenger-business-api-1.0.4/messenger_business_api.egg-info/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      406 2023-06-23 22:37:51.000000 messenger-business-api-1.0.4/messenger_business_api.egg-info/SOURCES.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-06-23 22:37:51.000000 messenger-business-api-1.0.4/messenger_business_api.egg-info/dependency_links.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       18 2023-06-23 22:37:51.000000 messenger-business-api-1.0.4/messenger_business_api.egg-info/requires.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       23 2023-06-23 22:37:51.000000 messenger-business-api-1.0.4/messenger_business_api.egg-info/top_level.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      392 2023-06-19 22:14:04.000000 messenger-business-api-1.0.4/pyproject.toml
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-06-23 22:37:51.529623 messenger-business-api-1.0.4/setup.cfg
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      684 2023-06-23 22:37:46.000000 messenger-business-api-1.0.4/setup.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:43:29.472182 messenger-business-api-1.0.5/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1066 2023-05-22 21:38:39.000000 messenger-business-api-1.0.5/LICENSE
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:43:29.472182 messenger-business-api-1.0.5/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1039 2023-06-23 22:11:44.000000 messenger-business-api-1.0.5/README.rst
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:43:29.472182 messenger-business-api-1.0.5/messenger_business_api/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       82 2023-06-23 22:43:25.000000 messenger-business-api-1.0.5/messenger_business_api/__init__.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1091 2023-06-23 22:42:25.000000 messenger-business-api-1.0.5/messenger_business_api/api.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      342 2023-06-19 22:14:04.000000 messenger-business-api-1.0.5/messenger_business_api/execeptions.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      193 2023-06-23 22:37:23.000000 messenger-business-api-1.0.5/messenger_business_api/types.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:43:29.472182 messenger-business-api-1.0.5/messenger_business_api.egg-info/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:43:29.000000 messenger-business-api-1.0.5/messenger_business_api.egg-info/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      406 2023-06-23 22:43:29.000000 messenger-business-api-1.0.5/messenger_business_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-06-23 22:43:29.000000 messenger-business-api-1.0.5/messenger_business_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       18 2023-06-23 22:43:29.000000 messenger-business-api-1.0.5/messenger_business_api.egg-info/requires.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       23 2023-06-23 22:43:29.000000 messenger-business-api-1.0.5/messenger_business_api.egg-info/top_level.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      392 2023-06-19 22:14:04.000000 messenger-business-api-1.0.5/pyproject.toml
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-06-23 22:43:29.472182 messenger-business-api-1.0.5/setup.cfg
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      684 2023-06-23 22:43:18.000000 messenger-business-api-1.0.5/setup.py
```

### Comparing `messenger-business-api-1.0.4/LICENSE` & `messenger-business-api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `messenger-business-api-1.0.4/PKG-INFO` & `messenger-business-api-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messenger-business-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: This repository is a wrapper for Meta messenger api for Messenger and Instagram
 Author: Yuri Ramos Lima
 Author-email: yurilima93@hotmail.com
 License: MIT License
 Keywords: python,Meta,Facebook,Instagram,message,chat-bot
 License-File: LICENSE
```

### Comparing `messenger-business-api-1.0.4/README.rst` & `messenger-business-api-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `messenger-business-api-1.0.4/messenger_business_api/api.py` & `messenger-business-api-1.0.5/messenger_business_api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, Optional
-from requests import Response
+from requests import Response, post, get
 from .execeptions import SendingMessageFailedException
 from .types import ApiRequestPayload
 
 
 class MessengerAPI:
 
     def __init__(self,  access_token: str, page_id: str, api_version: str = 'v16.0'):
@@ -13,17 +13,17 @@
             'Content-Type': 'application/json',
         }
 
     def send_text_message(self, user_id: str, message):
         payload = ApiRequestPayload(
             recipient={"id": user_id}, message={"text": str(message)})
         url = f"{self.base_url}/messages?access_token={self.access_token}"
-        result = requests.post(url, headers=self.headers, data=payload.json())
+        result = post(url, headers=self.headers, data=payload.json())
 
         if result.status_code != 200:
             raise SendingMessageFailedException(result.status_code)
         return result
 
     def get_media(self, uri: str) -> Optional[Response]:
-        response = requests.get(uri, stream=True)
+        response = get(uri, stream=True)
         response.raise_for_status()
         return response
```

### Comparing `messenger-business-api-1.0.4/messenger_business_api.egg-info/PKG-INFO` & `messenger-business-api-1.0.5/messenger_business_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messenger-business-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: This repository is a wrapper for Meta messenger api for Messenger and Instagram
 Author: Yuri Ramos Lima
 Author-email: yurilima93@hotmail.com
 License: MIT License
 Keywords: python,Meta,Facebook,Instagram,message,chat-bot
 License-File: LICENSE
```

### Comparing `messenger-business-api-1.0.4/setup.py` & `messenger-business-api-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.rst') as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="messenger-business-api",
-    version="1.0.4",
+    version="1.0.5",
     author="Yuri Ramos Lima",
     author_email="yurilima93@hotmail.com",
     description="This repository is a wrapper for Meta messenger api for Messenger and Instagram",
     packages=find_packages(),
     include_package_data=True,
     long_description=README,
     install_requires=[ "pydantic", "requests"],
```

