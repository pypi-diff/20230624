# Comparing `tmp/revChatGPT-6.4.3.tar.gz` & `tmp/revChatGPT-6.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.4.3.tar", last modified: Sat Jun 24 14:07:51 2023, max compression
+gzip compressed data, was "revChatGPT-6.4.4.tar", last modified: Sat Jun 24 14:53:38 2023, max compression
```

## Comparing `revChatGPT-6.4.3.tar` & `revChatGPT-6.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:07:51.229461 revChatGPT-6.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-24 14:07:13.000000 revChatGPT-6.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-24 14:07:51.229461 revChatGPT-6.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-24 14:07:50.000000 revChatGPT-6.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 14:07:51.229461 revChatGPT-6.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-24 14:07:13.000000 revChatGPT-6.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:07:51.225460 revChatGPT-6.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:07:51.229461 revChatGPT-6.4.3/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    59551 2023-06-24 14:07:13.000000 revChatGPT-6.4.3/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    24062 2023-06-24 14:07:13.000000 revChatGPT-6.4.3/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-24 14:07:13.000000 revChatGPT-6.4.3/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-24 14:07:13.000000 revChatGPT-6.4.3/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:07:51.229461 revChatGPT-6.4.3/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-24 14:07:13.000000 revChatGPT-6.4.3/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-24 14:07:13.000000 revChatGPT-6.4.3/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-24 14:07:13.000000 revChatGPT-6.4.3/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:07:51.229461 revChatGPT-6.4.3/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-24 14:07:51.000000 revChatGPT-6.4.3/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-24 14:07:51.000000 revChatGPT-6.4.3/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:07:51.000000 revChatGPT-6.4.3/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-24 14:07:51.000000 revChatGPT-6.4.3/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 14:07:51.000000 revChatGPT-6.4.3/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:07:51.229461 revChatGPT-6.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-24 14:07:13.000000 revChatGPT-6.4.3/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-24 14:53:37.000000 revChatGPT-6.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    57005 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24062 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-24 14:53:38.000000 revChatGPT-6.4.4/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-24 14:53:38.000000 revChatGPT-6.4.4/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:53:38.000000 revChatGPT-6.4.4/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-24 14:53:38.000000 revChatGPT-6.4.4/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 14:53:38.000000 revChatGPT-6.4.4/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/tests/test_recipient.py
```

### Comparing `revChatGPT-6.4.3/LICENSE` & `revChatGPT-6.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.3/PKG-INFO` & `revChatGPT-6.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.4.3
+Version: 6.4.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.4.3/README.md` & `revChatGPT-6.4.4/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.3/setup.py` & `revChatGPT-6.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.4.3",
+    version="6.4.4",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.4.3/src/revChatGPT/V1.py` & `revChatGPT-6.4.4/src/revChatGPT/V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,56 +370,27 @@
             password=self.config.get("password"),
             proxy=self.config.get("proxy"),
         )
         log.debug("Using authenticator to get access token")
 
         self.set_access_token(auth.auth())
 
-    def __arkose_token(self) -> str:
-        headers = {
-            "Accept": "application/json",
-            "Content-Type": "application/x-www-form-urlencoded",
-            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
-        }
-        form_data = {
-            "public_key": "35536E1E-65B4-4D96-9D97-6ADB7EFF8147",
-            # BDA is btoa(JSON.stringify({ ct: "", iv: "", s: "" })); in JS
-            "bda": str(base64.b64encode(b'{"ct":"","iv":"","s":""}'), "utf-8"),
-            "site": "https://chat.openai.com",
-            "userbrowser": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1823.43",
-            "capi_version": "1.5.2",
-            "capi_version": "lightbox",
-            "style_theme": "default",
-            # 17 digit random number
-            "rnd": "".join([str(random_int(0, 9)) for _ in range(17)]),
-        }
-        # URL encoded form data
-        form_data = "&".join([f"{k}={v}" for k, v in form_data.items()])
-        form_data = urllib.parse.quote(form_data, safe="=&")
-        url = "https://tcr9i.chat.openai.com/fc/gt2/public_key/35536E1E-65B4-4D96-9D97-6ADB7EFF8147"
-        response = self.session.post(url, data=form_data, headers=headers)
-        self.__check_response(response)
-        return response.json()["token"]
-
     @logger(is_timed=True)
     def __send_request(
         self,
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
         **kwargs,
     ) -> Generator[dict, None, None]:
         log.debug("Sending the payload")
 
         cid, pid = data["conversation_id"], data["parent_message_id"]
         message = ""
 
-        if data.get("model", "").startswith("gpt-4"):
-            data["arkose_token"] = self.__arkose_token()
-
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
         response = self.session.post(
             url=f"{self.base_url}conversation",
             data=json.dumps(data),
             timeout=timeout,
             stream=True,
@@ -976,39 +947,25 @@
             base_url=base_url,
             lazy_loading=lazy_loading,
         )
 
         # overwrite inherited normal session with async
         self.session = AsyncClient(headers=self.session.headers)
 
-    async def __arkose_token(self) -> str:
-        headers = {
-            "Accept": "application/json",
-            "Content-Type": "application/x-www-form-urlencoded",
-            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
-        }
-        form_data = "public_key=35536E1E-65B4-4D96-9D97-6ADB7EFF8147&site=https%3A%2F%2Fchat.openai.com&userbrowser=Mozilla%2F5.0%20(X11%3B%20Linux%20x86_64)%20AppleWebKit%2F537.36%20(KHTML%2C%20like%20Gecko)%20Chrome%2F114.0.0.0%20Safari%2F537.36&capi_version=1.5.2&capi_mode=lightbox&style_theme=default&rnd=0.3649022041957759"
-        url = "https://tcr9i.chat.openai.com/fc/gt2/public_key/35536E1E-65B4-4D96-9D97-6ADB7EFF8147"
-        response = await self.session.post(url, data=form_data, headers=headers)
-        self.__check_response(response)
-        return response.json()["token"]
-
     async def __send_request(
         self,
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
         **kwargs,
     ) -> AsyncGenerator[dict, None]:
         log.debug("Sending the payload")
 
         cid, pid = data["conversation_id"], data["parent_message_id"]
         message = ""
-        if data.get("model", "").startswith("gpt-4"):
-            data["arkose_token"] = await self.__arkose_token()
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
         async with self.session.stream(
             "POST",
             url=f"{self.base_url}conversation",
             data=json.dumps(data),
             timeout=timeout,
```

### Comparing `revChatGPT-6.4.3/src/revChatGPT/V3.py` & `revChatGPT-6.4.4/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.3/src/revChatGPT/__init__.py` & `revChatGPT-6.4.4/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.3/src/revChatGPT/__main__.py` & `revChatGPT-6.4.4/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.3/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.4.4/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.3/src/revChatGPT/typings.py` & `revChatGPT-6.4.4/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.3/src/revChatGPT/utils.py` & `revChatGPT-6.4.4/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.3/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.4.4/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.4.3
+Version: 6.4.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.4.3/tests/test_recipient.py` & `revChatGPT-6.4.4/tests/test_recipient.py`

 * *Files identical despite different names*

