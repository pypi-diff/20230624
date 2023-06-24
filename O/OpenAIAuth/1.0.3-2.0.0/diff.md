# Comparing `tmp/OpenAIAuth-1.0.3.tar.gz` & `tmp/OpenAIAuth-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenAIAuth-1.0.3.tar", last modified: Mon Jun 19 08:27:42 2023, max compression
+gzip compressed data, was "OpenAIAuth-2.0.0.tar", last modified: Sat Jun 24 14:02:20 2023, max compression
```

## Comparing `OpenAIAuth-1.0.3.tar` & `OpenAIAuth-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:27:42.662939 OpenAIAuth-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-19 08:27:19.000000 OpenAIAuth-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-19 08:27:42.662939 OpenAIAuth-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-19 08:27:19.000000 OpenAIAuth-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:27:42.662939 OpenAIAuth-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-19 08:27:19.000000 OpenAIAuth-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:27:42.662939 OpenAIAuth-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:27:42.662939 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-19 08:27:42.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-19 08:27:42.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:27:42.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 08:27:42.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 08:27:42.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-19 08:27:19.000000 OpenAIAuth-1.0.3/src/OpenAIAuth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:02:20.794830 OpenAIAuth-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-24 14:01:51.000000 OpenAIAuth-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-24 14:02:20.794830 OpenAIAuth-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-24 14:01:51.000000 OpenAIAuth-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:02:20.794830 OpenAIAuth-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-24 14:01:51.000000 OpenAIAuth-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:02:20.794830 OpenAIAuth-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:02:20.794830 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-24 14:02:20.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-24 14:02:20.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:02:20.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 14:02:20.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 14:02:20.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-06-24 14:01:51.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.py
```

### Comparing `OpenAIAuth-1.0.3/LICENSE` & `OpenAIAuth-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenAIAuth-1.0.3/PKG-INFO` & `OpenAIAuth-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAIAuth
-Version: 1.0.3
+Version: 2.0.0
 Summary: OpenAI Authentication Reverse Engineered
 Home-page: https://github.com/acheong08/OpenAIAuth
 Author: pengzhile
 Author-email: acheong@student.dalat.org
 License: MIT
 Project-URL: Bug Report, https://github.com/acheong08/OpenAIAuth/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OpenAIAuth-1.0.3/README.md` & `OpenAIAuth-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `OpenAIAuth-1.0.3/setup.py` & `OpenAIAuth-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="OpenAIAuth",
-    version="1.0.3",
+    version="2.0.0",
     license="MIT",
     author="pengzhile",
     author_email="acheong@student.dalat.org",
     description="OpenAI Authentication Reverse Engineered",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=["OpenAIAuth"],
```

### Comparing `OpenAIAuth-1.0.3/src/OpenAIAuth.egg-info/PKG-INFO` & `OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAIAuth
-Version: 1.0.3
+Version: 2.0.0
 Summary: OpenAI Authentication Reverse Engineered
 Home-page: https://github.com/acheong08/OpenAIAuth
 Author: pengzhile
 Author-email: acheong@student.dalat.org
 License: MIT
 Project-URL: Bug Report, https://github.com/acheong08/OpenAIAuth/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OpenAIAuth-1.0.3/src/OpenAIAuth.py` & `OpenAIAuth-2.0.0/src/OpenAIAuth.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,31 +13,28 @@
 
 class Auth0:
     def __init__(
         self,
         email: str,
         password: str,
         proxy: str = None,
-        use_cache: bool = True,
         mfa: str = None,
     ):
         """
         Initializes an instance of the Auth0 class.
 
         Args:
         - email (str): The email address of the user.
         - password (str): The password of the user.
         - proxy (str, optional): The proxy server to use for requests. Defaults to None.
-        - use_cache (bool, optional): Flag indicating whether to use cache for access token. Defaults to True.
         - mfa (str, optional): The multi-factor authentication method. Defaults to None.
         """
         self.session_token = None
         self.email = email
         self.password = password
-        self.use_cache = use_cache
         self.mfa = mfa
         self.session = requests.Session()
         self.req_kwargs = {
             "proxies": {
                 "http": proxy,
                 "https": proxy,
             }
@@ -54,30 +51,22 @@
         )
 
     @staticmethod
     def __check_email(email: str):
         regex = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b"
         return re.fullmatch(regex, email)
 
-    def auth(self) -> str:
+    def get_access_token(self) -> str:
         """
         Authenticates the user and returns the access token.
 
         Returns:
         - str: The access token.
         """
 
-        if (
-            self.use_cache
-            and self.access_token
-            and self.expires
-            and self.expires > dt.now()
-        ):
-            return self.access_token
-
         if not self.__check_email(self.email) or not self.password:
             raise Exception("invalid email or password.")
 
         return self.__part_two()
 
     def __part_two(self) -> str:
         code_challenge = "w6n3Ix420Xhhu-Q5-mOOEyuPZmAsJHUbBpO8Ub7xBCY"
@@ -183,15 +172,15 @@
                 return self.__part_seven(code_verifier, location)
 
             if not location.startswith(
                 "com.openai.chat://auth0.openai.com/ios/com.openai.chat/callback?"
             ):
                 raise Exception("Login callback failed.")
 
-            return self.get_access_token(code_verifier, resp.headers["Location"])
+            return self.__get_access_token(code_verifier, resp.headers["Location"])
 
         raise Exception("Error login.")
 
     def __part_seven(self, code_verifier: str, location: str) -> str:
         url = "https://auth0.openai.com" + location
         data = {
             "state": parse_qs(urlparse(url).query)["state"][0],
@@ -215,15 +204,15 @@
             return self.__part_six(code_verifier, location, url)
 
         if resp.status_code == 400:
             raise Exception("Wrong MFA code.")
         else:
             raise Exception("Error login.")
 
-    def get_access_token(self, code_verifier: str, callback_url: str) -> str:
+    def __get_access_token(self, code_verifier: str, callback_url: str) -> str:
         url_params = parse_qs(urlparse(callback_url).query)
 
         if "error" in url_params:
             error = url_params["error"][0]
             error_description = (
                 url_params["error_description"][0]
                 if "error_description" in url_params
@@ -259,7 +248,34 @@
                 dt.utcnow()
                 + datetime.timedelta(seconds=json["expires_in"])
                 - datetime.timedelta(minutes=5)
             )
             return self.access_token
         else:
             raise Exception(resp.text)
+
+    def get_puid(self) -> str:
+        url = "https://bypass.churchless.tech/models"
+        headers = {
+            "Authorization": "Bearer " + self.access_token,
+        }
+        resp = self.session.get(url, headers=headers, **self.req_kwargs)
+        if resp.status_code == 200:
+            # Get _puid cookie
+            puid = resp.headers.get("set-cookie", "")
+            if not puid:
+                raise Exception("Get _puid cookie failed.")
+            self.puid = puid.split("_puid=")[1].split(";")[0]
+            return self.puid
+        else:
+            raise Exception(resp.text)
+
+
+if __name__ == "__main__":
+    import os
+
+    email = os.getenv("OPENAI_EMAIL")
+    password = os.getenv("OPENAI_PASSWORD")
+    openai = Auth0(email, password)
+    print(openai.get_access_token())
+
+    print(openai.get_puid())
```

