# Comparing `tmp/dalpha-0.1.1.tar.gz` & `tmp/dalpha-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.1.1.tar", max compression
+gzip compressed data, was "dalpha-0.1.2.tar", max compression
```

## Comparing `dalpha-0.1.1.tar` & `dalpha-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      459 2023-05-28 23:48:43.785059 dalpha-0.1.1/README.md
--rw-r--r--   0        0        0     6363 2023-06-19 14:20:53.477797 dalpha-0.1.1/dalpha/__init__.py
--rw-r--r--   0        0        0      745 2023-06-19 14:22:28.764937 dalpha-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 dalpha-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      459 2023-05-28 23:48:43.785059 dalpha-0.1.2/README.md
+-rw-r--r--   0        0        0     6431 2023-06-24 02:59:46.421105 dalpha-0.1.2/dalpha/__init__.py
+-rw-r--r--   0        0        0      745 2023-06-24 04:10:36.493493 dalpha-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 dalpha-0.1.2/PKG-INFO
```

### Comparing `dalpha-0.1.1/dalpha/__init__.py` & `dalpha-0.1.2/dalpha/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import requests, json, boto3, io, logging, sys, os
 class Agent:
-    def __init__(self, api_id, mock, use_sqs = False):
+    def __init__(self, api_id, use_sqs = False, dev_server=False):
         self.cfg_path = os.path.join(sys.path[0],'.dalphacfg')
         self.__load_config(self.cfg_path)
         self.token = os.environ['TOKEN']
-        self.base_url = os.environ['BASE_URL']
+        if dev_server:
+            self.base_url = os.environ['DEV_BASE_URL']
+        else:
+            self.base_url = os.environ['BASE_URL']
         self.queue_url = os.environ['QUEUE_URL']
         self.evaluate_url = os.path.join(self.base_url, f"inferences/{api_id}/evaluate")
         self.api_id = api_id
-        self.mock = mock
+        self.mock = {}
         self.s3 = boto3.client('s3')
         self.sqs = boto3.client('sqs', region_name='ap-northeast-2')
         self.evaluates = {}
         self.use_sqs = use_sqs
         
     def __load_config(self,file_path):
         if not os.path.isfile(file_path):
@@ -24,23 +27,25 @@
         
         for line in lines:
             line = line.strip()
             if line and not line.startswith("#"):
                 key, value = line.split("=")
                 os.environ[key] = value
 
+    def set_mock(self, mock):
+        self.mock = mock
+
     def poll(self, max_number_of_messages = 1, mock=True):
         if mock:
             return self.mock
         
         if self.use_sqs:
             response = self.sqs.receive_message(
                 QueueUrl = self.queue_url,
                 MaxNumberOfMessages = max_number_of_messages,  # 가져올 메시지의 최대 수 (1개 이상 설정 가능)
-                VisibilityTimeout = 15,   # 메시지의 가시성 제한 시간 (초 단위)
                 WaitTimeSeconds = 0       # 긴 폴링을 위한 대기 시간 (초 단위)
             )
             ret = []
             messages = response.get('Messages', [])
             for message in messages:
                 message_body = message['Body']
                 try:
```

### Comparing `dalpha-0.1.1/pyproject.toml` & `dalpha-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.26.137"
 requests = "^2.30.0"
 build = "^0.10.0"
 
 [project]
 name = "dalpha"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Beomseok", email="beomseok.lee@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dalpha-0.1.1/PKG-INFO` & `dalpha-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

