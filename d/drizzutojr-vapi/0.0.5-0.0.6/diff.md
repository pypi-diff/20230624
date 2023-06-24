# Comparing `tmp/drizzutojr_vapi-0.0.5-py3-none-any.whl.zip` & `tmp/drizzutojr_vapi-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4061 bytes, number of entries: 8
--rw-r--r--  2.0 unx       49 b- defN 23-Jun-20 04:01 vapi/__init__.py
--rw-r--r--  2.0 unx     1344 b- defN 23-Jun-20 04:01 vapi/exceptions.py
--rw-r--r--  2.0 unx     5798 b- defN 23-Jun-20 04:01 vapi/vapi.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-20 04:03 drizzutojr_vapi-0.0.5.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      200 b- defN 23-Jun-20 04:03 drizzutojr_vapi-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 04:03 drizzutojr_vapi-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-20 04:03 drizzutojr_vapi-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      642 b- defN 23-Jun-20 04:03 drizzutojr_vapi-0.0.5.dist-info/RECORD
-8 files, 9191 bytes uncompressed, 2935 bytes compressed:  68.1%
+Zip file size: 4279 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-24 21:03 vapi/__init__.py
+-rw-r--r--  2.0 unx     1344 b- defN 23-Jun-24 21:03 vapi/exceptions.py
+-rw-r--r--  2.0 unx     6867 b- defN 23-Jun-24 21:03 vapi/vapi.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-24 21:05 drizzutojr_vapi-0.0.6.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-24 21:05 drizzutojr_vapi-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 21:05 drizzutojr_vapi-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-24 21:05 drizzutojr_vapi-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      642 b- defN 23-Jun-24 21:05 drizzutojr_vapi-0.0.6.dist-info/RECORD
+8 files, 10260 bytes uncompressed, 3153 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: vapi/exceptions.py
 Comment: 
 
 Filename: vapi/vapi.py
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.5.dist-info/LICENSE.md
+Filename: drizzutojr_vapi-0.0.6.dist-info/LICENSE.md
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.5.dist-info/METADATA
+Filename: drizzutojr_vapi-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.5.dist-info/WHEEL
+Filename: drizzutojr_vapi-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.5.dist-info/top_level.txt
+Filename: drizzutojr_vapi-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.5.dist-info/RECORD
+Filename: drizzutojr_vapi-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vapi/vapi.py

```diff
@@ -49,21 +49,48 @@
             )
 
         self.api_version = "v1"
         self.current_path = ""
 
         token_test = self.token_lookup()
 
-    def _set_headers(self):
-        return {
+    def _validate_wrap_value(self, wrap_response):
+        error_message = f"Wrap Response value {wrap_response} is not in valid VAPI format XXs, XXm, or XXh"
+
+        try:
+            number = int(wrap_response[:-1])
+        except ValueError:
+            raise VAPIConfigError(error_message)
+
+        if (
+            wrap_response.endswith("s")
+            or wrap_response.endswith("m")
+            or wrap_response.endswith("h")
+        ):
+            pass
+        else:
+            raise VAPIConfigError(error_message)
+
+        return wrap_response
+
+    def _set_headers(self, wrap_response):
+        headers = {
             "Content-type": "application/json",
             "X-Vault-Token": self.token,
             "X-Vault-Namespace": self.namespace,
         }
 
+        if wrap_response:
+            try:
+                headers["X-Vault-Wrap-Ttl"] = self._validate_wrap_value(wrap_response)
+            except VAPIConfigError as e:
+                raise
+
+        return headers
+
     def _format_url(self, path):
         self.current_path = path
         url = f"{self.api_version}/{path}".replace("//", "/")
         url = f"{self.addr.rstrip('/')}/{url}"
         return url
 
     def _format_response(self, response, accepted_status_codes):
@@ -104,55 +131,74 @@
 
         try:
             return response.json()
         except ValueError:
             return {}
 
     def token_lookup(self, raw=False, accepted_status_codes=[204, 200]):
-        headers = self._set_headers()
+        headers = self._set_headers(None)
         url = self._format_url("/auth/token/lookup-self")
         response = requests.get(url, headers=headers, verify=self.cacert)
 
         if raw:
             return response
         else:
             return self._format_response(response, accepted_status_codes)
 
-    def get(self, path, raw=False, accepted_status_codes=[204, 200]):
-        headers = self._set_headers()
+    def get(
+        self,
+        path,
+        raw=False,
+        accepted_status_codes=[204, 200],
+        wrap_response: str = None,
+    ):
+        headers = self._set_headers(wrap_response)
         url = self._format_url(path)
         response = requests.get(url, headers=headers, verify=self.cacert)
 
         if raw:
             return response
         else:
             return self._format_response(response, accepted_status_codes)
 
-    def list(self, path, raw=False, accepted_status_codes=[204, 200]):
-        headers = self._set_headers()
+    def list(
+        self,
+        path,
+        raw=False,
+        accepted_status_codes=[204, 200],
+        wrap_response: str = None,
+    ):
+        headers = self._set_headers(wrap_response)
         url = f"{self._format_url(path)}?list=true"
         response = requests.get(url, headers=headers, verify=self.cacert)
 
         if raw:
             return response
         else:
             return self._format_response(response, accepted_status_codes)
 
-    def post(self, path, data={}, raw=False, accepted_status_codes=[204, 200]):
-        headers = self._set_headers()
+    def post(
+        self,
+        path,
+        data={},
+        raw=False,
+        accepted_status_codes=[204, 200],
+        wrap_response: str = None,
+    ):
+        headers = self._set_headers(wrap_response)
         url = self._format_url(path)
         response = requests.post(url, json=data, headers=headers, verify=self.cacert)
 
         if raw:
             return response
         else:
             return self._format_response(response, accepted_status_codes)
 
     def delete(self, path, raw=False, accepted_status_codes=[204, 200]):
-        headers = self._set_headers()
+        headers = self._set_headers(None)
         url = self._format_url(path)
         response = requests.delete(url, headers=headers, verify=self.cacert)
 
         if raw:
             return response
         else:
             return self._format_response(response, accepted_status_codes)
```

## Comparing `drizzutojr_vapi-0.0.5.dist-info/LICENSE.md` & `drizzutojr_vapi-0.0.6.dist-info/LICENSE.md`

 * *Files identical despite different names*

