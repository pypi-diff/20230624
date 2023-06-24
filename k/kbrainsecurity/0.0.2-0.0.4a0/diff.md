# Comparing `tmp/kbrainsecurity-0.0.2.tar.gz` & `tmp/kbrainsecurity-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbrainsecurity-0.0.2.tar", max compression
+gzip compressed data, was "kbrainsecurity-0.0.4a0.tar", max compression
```

## Comparing `kbrainsecurity-0.0.2.tar` & `kbrainsecurity-0.0.4a0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      574 2023-06-24 00:06:42.019101 kbrainsecurity-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1004 2023-06-23 23:07:28.087580 kbrainsecurity-0.0.2/README.md
--rw-r--r--   0        0        0     1349 2023-06-23 23:07:28.095586 kbrainsecurity-0.0.2/src/azure_authentication.py
--rw-r--r--   0        0        0     1379 2023-06-23 23:07:28.097586 kbrainsecurity-0.0.2/src/bearer.py
--rw-r--r--   0        0        0     1560 1970-01-01 00:00:00.000000 kbrainsecurity-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      982 2023-06-24 00:12:31.686943 kbrainsecurity-0.0.4a0/README.md
+-rw-r--r--   0        0        0      553 2023-06-24 00:13:15.942541 kbrainsecurity-0.0.4a0/pyproject.toml
+-rw-r--r--   0        0        0     1313 2023-06-24 00:12:31.686943 kbrainsecurity-0.0.4a0/src/azure_authentication.py
+-rw-r--r--   0        0        0     1336 2023-06-24 00:12:31.686943 kbrainsecurity-0.0.4a0/src/bearer.py
+-rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 kbrainsecurity-0.0.4a0/PKG-INFO
```

### Comparing `kbrainsecurity-0.0.2/src/azure_authentication.py` & `kbrainsecurity-0.0.4a0/src/azure_authentication.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import functools
-import json
-import logging
-from typing import Callable
-
-import azure.functions as func
-from jose import JWTError
-
-from src.bearer import AuthenticationTokenException
-from src.bearer import extract_claims
-from src.bearer import validate_claims
-
-
-def authenticate_request(required_claims: dict[str, any]) -> func.HttpResponse:
-    def argument_wrapper(callback: Callable[..., any]):
-        @functools.wraps(callback)
-        def wrapper(req: func.HttpRequest, *args, **kwargs) -> func.HttpResponse:
-            try:
-                logging.info(
-                    f"KBRAIN Authentication. Required claims: {json.dumps(required_claims)}"
-                )
-                try:
-                    auth = req.headers.get("Authorization", None)
-                    token_claims = extract_claims(auth)
-                    validate_claims(token_claims, required_claims)
-                except (AuthenticationTokenException, JWTError) as ae:
-                    return func.HttpResponse(str(ae), status_code=401)
-
-                [data, status] = callback(req, *args, **kwargs)
-                return func.HttpResponse(data, status_code=status)
-            except Exception as ex:
-                return func.HttpResponse(str(ex), status_code=500)
-
-        return wrapper
-
-    return argument_wrapper
+import functools
+import json
+import logging
+from typing import Callable
+
+import azure.functions as func
+from jose import JWTError
+
+from src.bearer import AuthenticationTokenException
+from src.bearer import extract_claims
+from src.bearer import validate_claims
+
+
+def authenticate_request(required_claims: dict[str, any]) -> func.HttpResponse:
+    def argument_wrapper(callback: Callable[..., any]):
+        @functools.wraps(callback)
+        def wrapper(req: func.HttpRequest, *args, **kwargs) -> func.HttpResponse:
+            try:
+                logging.info(
+                    f"KBRAIN Authentication. Required claims: {json.dumps(required_claims)}"
+                )
+                try:
+                    auth = req.headers.get("Authorization", None)
+                    token_claims = extract_claims(auth)
+                    validate_claims(token_claims, required_claims)
+                except (AuthenticationTokenException, JWTError) as ae:
+                    return func.HttpResponse(str(ae), status_code=401)
+
+                [data, status] = callback(req, *args, **kwargs)
+                return func.HttpResponse(data, status_code=status)
+            except Exception as ex:
+                return func.HttpResponse(str(ex), status_code=500)
+
+        return wrapper
+
+    return argument_wrapper
```

### Comparing `kbrainsecurity-0.0.2/src/bearer.py` & `kbrainsecurity-0.0.4a0/src/bearer.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import json
-
-from jose import jwt
-
-
-class AuthenticationTokenException(Exception):
-    def __init__(self, error):
-        super().__init__(error)
-
-
-def extract_claims(token: str) -> list:
-    if not token:
-        raise AuthenticationTokenException(
-            "Authentication error: Authorization header is missing"
-        )
-
-    parts: list[str] = token.split()
-
-    if parts[0].lower() != "bearer":
-        raise AuthenticationTokenException(
-            "Authentication error: Authorization header must start with ' Bearer'"
-        )
-    elif len(parts) == 1:
-        raise AuthenticationTokenException("Authentication error: Token not found")
-    elif len(parts) > 2:
-        raise AuthenticationTokenException(
-            "Authentication error: Authorization header must be 'Bearer <token>'"
-        )
-
-    token_claims: dict[str, any] = jwt.get_unverified_claims(parts[1])
-    return token_claims
-
-
-def validate_claims(
-    token_claims: dict[str, any], required_claims: dict[str, any]
-) -> bool:
-    for key in required_claims:
-        if key not in token_claims or token_claims[key] != required_claims[key]:
-            raise AuthenticationTokenException(
-                "Authentication error: The token provided does not have sufficiently valid claims to authorize access to this service."
-            )
-
-    return True
+import json
+
+from jose import jwt
+
+
+class AuthenticationTokenException(Exception):
+    def __init__(self, error):
+        super().__init__(error)
+
+
+def extract_claims(token: str) -> list:
+    if not token:
+        raise AuthenticationTokenException(
+            "Authentication error: Authorization header is missing"
+        )
+
+    parts: list[str] = token.split()
+
+    if parts[0].lower() != "bearer":
+        raise AuthenticationTokenException(
+            "Authentication error: Authorization header must start with ' Bearer'"
+        )
+    elif len(parts) == 1:
+        raise AuthenticationTokenException("Authentication error: Token not found")
+    elif len(parts) > 2:
+        raise AuthenticationTokenException(
+            "Authentication error: Authorization header must be 'Bearer <token>'"
+        )
+
+    token_claims: dict[str, any] = jwt.get_unverified_claims(parts[1])
+    return token_claims
+
+
+def validate_claims(
+    token_claims: dict[str, any], required_claims: dict[str, any]
+) -> bool:
+    for key in required_claims:
+        if key not in token_claims or token_claims[key] != required_claims[key]:
+            raise AuthenticationTokenException(
+                "Authentication error: The token provided does not have sufficiently valid claims to authorize access to this service."
+            )
+
+    return True
```

### Comparing `kbrainsecurity-0.0.2/PKG-INFO` & `kbrainsecurity-0.0.4a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbrainsecurity
-Version: 0.0.2
+Version: 0.0.4a0
 Summary: Security and authentication functions for use in KBRAIN
 License: UNLICENSED
 Author: Daniel E. Fredriksen
 Author-email: daniel.fredriksen@us.kbr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

