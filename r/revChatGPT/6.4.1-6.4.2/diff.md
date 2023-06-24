# Comparing `tmp/revChatGPT-6.4.1.tar.gz` & `tmp/revChatGPT-6.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.4.1.tar", last modified: Thu Jun 22 03:55:44 2023, max compression
+gzip compressed data, was "revChatGPT-6.4.2.tar", last modified: Sat Jun 24 10:52:59 2023, max compression
```

## Comparing `revChatGPT-6.4.1.tar` & `revChatGPT-6.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.744142 revChatGPT-6.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    58782 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 03:55:44.000000 revChatGPT-6.4.1/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:55:44.752142 revChatGPT-6.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-22 03:55:09.000000 revChatGPT-6.4.1/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:52:59.681569 revChatGPT-6.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-24 10:52:24.000000 revChatGPT-6.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-24 10:52:59.681569 revChatGPT-6.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-24 10:52:59.000000 revChatGPT-6.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 10:52:59.681569 revChatGPT-6.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-24 10:52:24.000000 revChatGPT-6.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:52:59.677569 revChatGPT-6.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:52:59.677569 revChatGPT-6.4.2/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    59317 2023-06-24 10:52:24.000000 revChatGPT-6.4.2/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24062 2023-06-24 10:52:24.000000 revChatGPT-6.4.2/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-24 10:52:24.000000 revChatGPT-6.4.2/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-24 10:52:24.000000 revChatGPT-6.4.2/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:52:59.681569 revChatGPT-6.4.2/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-24 10:52:24.000000 revChatGPT-6.4.2/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-24 10:52:24.000000 revChatGPT-6.4.2/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-24 10:52:24.000000 revChatGPT-6.4.2/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:52:59.677569 revChatGPT-6.4.2/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-24 10:52:59.000000 revChatGPT-6.4.2/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-24 10:52:59.000000 revChatGPT-6.4.2/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:52:59.000000 revChatGPT-6.4.2/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-24 10:52:59.000000 revChatGPT-6.4.2/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 10:52:59.000000 revChatGPT-6.4.2/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:52:59.681569 revChatGPT-6.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-24 10:52:24.000000 revChatGPT-6.4.2/tests/test_recipient.py
```

### Comparing `revChatGPT-6.4.1/LICENSE` & `revChatGPT-6.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.1/PKG-INFO` & `revChatGPT-6.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.4.1
+Version: 6.4.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.4.1/README.md` & `revChatGPT-6.4.2/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.1/setup.py` & `revChatGPT-6.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.4.1",
+    version="6.4.2",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.4.1/src/revChatGPT/V1.py` & `revChatGPT-6.4.2/src/revChatGPT/V1.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pathlib import Path
 from typing import AsyncGenerator
 from typing import Generator
 from typing import NoReturn
 
 import httpx
 import requests
+import urllib
 from httpx import AsyncClient
 from OpenAIAuth import Auth0 as Authenticator
 from rich.live import Live
 from rich.markdown import Markdown
 
 from . import __version__
 from . import typings as t
@@ -369,15 +370,29 @@
 
     def __arkose_token(self) -> str:
         headers = {
             "Accept": "application/json",
             "Content-Type": "application/x-www-form-urlencoded",
             "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
         }
-        form_data = "public_key=35536E1E-65B4-4D96-9D97-6ADB7EFF8147&site=https%3A%2F%2Fchat.openai.com&userbrowser=Mozilla%2F5.0%20(X11%3B%20Linux%20x86_64)%20AppleWebKit%2F537.36%20(KHTML%2C%20like%20Gecko)%20Chrome%2F114.0.0.0%20Safari%2F537.36&capi_version=1.5.2&capi_mode=lightbox&style_theme=default&rnd=0.3649022041957759"
+        form_data = {
+            "public_key": "35536E1E-65B4-4D96-9D97-6ADB7EFF8147",
+            # BDA is btoa(JSON.stringify({ ct: "", iv: "", s: "" })); in JS
+            "bda": str(base64.b64encode(b'{"ct":"","iv":"","s":""}'), "utf-8"),
+            "site": "https://chat.openai.com",
+            "userbrowser": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1823.43",
+            "capi_version": "1.5.2",
+            "capi_version": "lightbox",
+            "style_theme": "default",
+            # 17 digit random number
+            "rnd": "".join([str(random_int(0, 9)) for _ in range(17)]),
+        }
+        # URL encoded form data
+        form_data = "&".join([f"{k}={v}" for k, v in form_data.items()])
+        form_data = urllib.parse.quote(form_data, safe="=&")
         url = "https://tcr9i.chat.openai.com/fc/gt2/public_key/35536E1E-65B4-4D96-9D97-6ADB7EFF8147"
         response = self.session.post(url, data=form_data, headers=headers)
         self.__check_response(response)
         return response.json()["token"]
 
     @logger(is_timed=True)
     def __send_request(
```

### Comparing `revChatGPT-6.4.1/src/revChatGPT/V3.py` & `revChatGPT-6.4.2/src/revChatGPT/V3.py`

 * *Files 2% similar despite different names*

```diff
@@ -683,16 +683,17 @@
             )
         except KeyboardInterrupt:
             print("\nExiting...")
             sys.exit()
         if prompt.startswith("!"):
             try:
                 chatbot.handle_commands(prompt)
-            except Exception as err:
+            except (requests.exceptions.Timeout, requests.exceptions.ConnectionError) as err:
                 print(f"Error: {err}")
+                continue
             continue
         print()
         print("ChatGPT: ", flush=True)
         if args.enable_internet:
             query = chatbot.ask(
                 f'This is a prompt from a user to a chatbot: "{prompt}". Respond with "none" if it is directed at the chatbot or cannot be answered by an internet search. Otherwise, respond with a possible search query to a search engine. Do not write any additional text. Make it as minimal as possible',
                 convo_id="search",
```

### Comparing `revChatGPT-6.4.1/src/revChatGPT/__init__.py` & `revChatGPT-6.4.2/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.1/src/revChatGPT/__main__.py` & `revChatGPT-6.4.2/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.1/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.4.2/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.1/src/revChatGPT/typings.py` & `revChatGPT-6.4.2/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.1/src/revChatGPT/utils.py` & `revChatGPT-6.4.2/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.1/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.4.2/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.4.1
+Version: 6.4.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.4.1/tests/test_recipient.py` & `revChatGPT-6.4.2/tests/test_recipient.py`

 * *Files identical despite different names*

