# Comparing `tmp/w3bstream_client_python-0.2.1.tar.gz` & `tmp/w3bstream_client_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3bstream_client_python-0.2.1.tar", last modified: Sat Jun 24 06:21:59 2023, max compression
+gzip compressed data, was "w3bstream_client_python-0.3.0.tar", last modified: Sat Jun 24 07:21:10 2023, max compression
```

## Comparing `w3bstream_client_python-0.2.1.tar` & `w3bstream_client_python-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 06:21:59.744129 w3bstream_client_python-0.2.1/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-24 06:21:59.744129 w3bstream_client_python-0.2.1/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-06-24 06:21:59.744129 w3bstream_client_python-0.2.1/setup.cfg
--rw-r--r--   0 haaai     (1000) haaai     (1000)      205 2023-06-24 06:20:36.000000 w3bstream_client_python-0.2.1/setup.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 06:21:59.744129 w3bstream_client_python-0.2.1/w3bstream_client_python/
--rw-r--r--   0 haaai     (1000) haaai     (1000)       49 2023-06-24 01:11:11.000000 w3bstream_client_python-0.2.1/w3bstream_client_python/__init__.py
--rw-r--r--   0 haaai     (1000) haaai     (1000)      887 2023-06-24 06:21:23.000000 w3bstream_client_python-0.2.1/w3bstream_client_python/client.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 06:21:59.744129 w3bstream_client_python-0.2.1/w3bstream_client_python.egg-info/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-24 06:21:59.000000 w3bstream_client_python-0.2.1/w3bstream_client_python.egg-info/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      266 2023-06-24 06:21:59.000000 w3bstream_client_python-0.2.1/w3bstream_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-06-24 06:21:59.000000 w3bstream_client_python-0.2.1/w3bstream_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-06-24 06:21:59.000000 w3bstream_client_python-0.2.1/w3bstream_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 07:21:10.676302 w3bstream_client_python-0.3.0/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-24 07:21:10.676302 w3bstream_client_python-0.3.0/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-06-24 07:21:10.676302 w3bstream_client_python-0.3.0/setup.cfg
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      205 2023-06-24 07:21:04.000000 w3bstream_client_python-0.3.0/setup.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 07:21:10.666302 w3bstream_client_python-0.3.0/w3bstream_client_python/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       49 2023-06-24 01:11:11.000000 w3bstream_client_python-0.3.0/w3bstream_client_python/__init__.py
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     1190 2023-06-24 07:19:44.000000 w3bstream_client_python-0.3.0/w3bstream_client_python/client.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 07:21:10.676302 w3bstream_client_python-0.3.0/w3bstream_client_python.egg-info/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-24 07:21:10.000000 w3bstream_client_python-0.3.0/w3bstream_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      266 2023-06-24 07:21:10.000000 w3bstream_client_python-0.3.0/w3bstream_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-06-24 07:21:10.000000 w3bstream_client_python-0.3.0/w3bstream_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-06-24 07:21:10.000000 w3bstream_client_python-0.3.0/w3bstream_client_python.egg-info/top_level.txt
```

### Comparing `w3bstream_client_python-0.2.1/w3bstream_client_python/client.py` & `w3bstream_client_python-0.3.0/w3bstream_client_python/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,22 +7,28 @@
     def __init__(self, endpoint, api_key):
         self.endpoint = endpoint
         self.api_key = api_key
 
     # TODO: support push_data non-blocking, which can send data async in batch
     # TODO: make push_data non-panic
     def push_data(self, deviceID, data, event_type="DEFAULT"):
+        self._validate_data_format(deviceID, data, event_type)
         headers = {
             'Content-Type': 'application/json',
             'Authorization': 'Bearer ' + self.api_key,
         }
-        body = {
+        body = [{
             'device_id': deviceID,
             'event_type': event_type,
             'payload': data,
-            'timestamp':  datetime.datetime.now().isoformat(),
-        }
-        response = requests.post(
+            'timestamp':  int(round(datetime.datetime.now().timestamp())),
+        }]
+        return requests.post(
             self.endpoint, data=json.dumps(body), headers=headers)
-        print(f"Hello, {self.endpoint}, {self.api_key}, {body}!")
-        print(response)
-        return response
+
+    def _validate_data_format(self, deviceID, data, event_type):
+        if type(deviceID) != str:
+            raise ValueError("deviceID should be a string")
+        if type(data) != str:
+            raise ValueError("data should be a string")
+        if type(event_type) != str:
+            raise ValueError("event_type should be a string")
```

