# Comparing `tmp/morp-5.2.1.tar.gz` & `tmp/morp-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morp-5.2.1.tar", last modified: Sat May 13 22:41:32 2023, max compression
+gzip compressed data, was "morp-5.2.2.tar", last modified: Sat Jun 24 21:16:44 2023, max compression
```

## Comparing `morp-5.2.1.tar` & `morp-5.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-13 22:41:32.211141 morp-5.2.1/
--rw-r--r--   0 jaymon     (501) staff       (20)     1079 2017-07-29 01:05:20.000000 morp-5.2.1/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-05-13 22:41:32.211027 morp-5.2.1/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)     3021 2023-03-03 20:29:34.000000 morp-5.2.1/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-13 22:41:32.209605 morp-5.2.1/morp/
--rw-r--r--   0 jaymon     (501) staff       (20)      347 2023-05-13 22:41:10.000000 morp-5.2.1/morp/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     6756 2023-02-05 20:04:47.000000 morp-5.2.1/morp/__main__.py
--rw-r--r--   0 jaymon     (501) staff       (20)       97 2023-02-07 07:17:53.000000 morp-5.2.1/morp/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4714 2023-03-31 06:52:48.000000 morp-5.2.1/morp/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     1022 2023-03-03 09:33:58.000000 morp-5.2.1/morp/exception.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-13 22:41:32.210851 morp-5.2.1/morp/interface/
--rw-r--r--   0 jaymon     (501) staff       (20)     2944 2023-02-07 07:11:11.000000 morp-5.2.1/morp/interface/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    11735 2023-03-03 09:01:56.000000 morp-5.2.1/morp/interface/base.py
--rw-r--r--   0 jaymon     (501) staff       (20)     5069 2023-05-13 22:39:43.000000 morp-5.2.1/morp/interface/dropfile.py
--rw-r--r--   0 jaymon     (501) staff       (20)    13543 2023-05-13 22:35:50.000000 morp-5.2.1/morp/interface/sqs.py
--rw-r--r--   0 jaymon     (501) staff       (20)    10354 2023-05-13 22:20:12.000000 morp-5.2.1/morp/message.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-13 22:41:32.210381 morp-5.2.1/morp.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      397 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       47 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/entry_points.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/requires.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-05-13 22:41:32.000000 morp-5.2.1/morp.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-05-13 22:41:32.211175 morp-5.2.1/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     1815 2023-02-05 21:01:52.000000 morp-5.2.1/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-24 21:16:44.752397 morp-5.2.2/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1079 2017-07-29 01:05:20.000000 morp-5.2.2/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-06-24 21:16:44.752291 morp-5.2.2/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)     3021 2023-03-03 20:29:34.000000 morp-5.2.2/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-24 21:16:44.750800 morp-5.2.2/morp/
+-rw-r--r--   0 jaymon     (501) staff       (20)      347 2023-06-24 21:15:51.000000 morp-5.2.2/morp/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     6756 2023-02-05 20:04:47.000000 morp-5.2.2/morp/__main__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)       97 2023-02-07 07:17:53.000000 morp-5.2.2/morp/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4714 2023-03-31 06:52:48.000000 morp-5.2.2/morp/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     1022 2023-03-03 09:33:58.000000 morp-5.2.2/morp/exception.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-24 21:16:44.752140 morp-5.2.2/morp/interface/
+-rw-r--r--   0 jaymon     (501) staff       (20)     2944 2023-02-07 07:11:11.000000 morp-5.2.2/morp/interface/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    11734 2023-06-24 21:16:36.000000 morp-5.2.2/morp/interface/base.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     5069 2023-05-13 22:39:43.000000 morp-5.2.2/morp/interface/dropfile.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    13540 2023-06-24 21:11:11.000000 morp-5.2.2/morp/interface/sqs.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    10354 2023-05-13 22:20:12.000000 morp-5.2.2/morp/message.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-24 21:16:44.751404 morp-5.2.2/morp.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     3744 2023-06-24 21:16:44.000000 morp-5.2.2/morp.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      397 2023-06-24 21:16:44.000000 morp-5.2.2/morp.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-06-24 21:16:44.000000 morp-5.2.2/morp.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       47 2023-06-24 21:16:44.000000 morp-5.2.2/morp.egg-info/entry_points.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-06-24 21:16:44.000000 morp-5.2.2/morp.egg-info/requires.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-06-24 21:16:44.000000 morp-5.2.2/morp.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-06-24 21:16:44.752434 morp-5.2.2/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     1815 2023-02-05 21:01:52.000000 morp-5.2.2/setup.py
```

### Comparing `morp-5.2.1/LICENSE.txt` & `morp-5.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morp-5.2.1/PKG-INFO` & `morp-5.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morp
-Version: 5.2.1
+Version: 5.2.2
 Summary: Send and receive messages without thinking about it
 Home-page: http://github.com/Jaymon/morp
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Keywords: Amazon AWS SQS messages message-passing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `morp-5.2.1/README.md` & `morp-5.2.2/README.md`

 * *Files identical despite different names*

### Comparing `morp-5.2.1/morp/__main__.py` & `morp-5.2.2/morp/__main__.py`

 * *Files identical despite different names*

### Comparing `morp-5.2.1/morp/config.py` & `morp-5.2.2/morp/config.py`

 * *Files identical despite different names*

### Comparing `morp-5.2.1/morp/exception.py` & `morp-5.2.2/morp/exception.py`

 * *Files identical despite different names*

### Comparing `morp-5.2.1/morp/interface/__init__.py` & `morp-5.2.2/morp/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `morp-5.2.1/morp/interface/base.py` & `morp-5.2.2/morp/interface/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         self.connection_config = connection_config
 
     def connect(self, connection_config=None):
         """connect to the interface
 
         this will set the raw db connection to self.connection
         """
-
         if self.connected: return self.connected
         if connection_config: self.connection_config = connection_config
 
         try:
             self.connected = False
             self._connect(self.connection_config)
             self.connected = True
```

### Comparing `morp-5.2.1/morp/interface/dropfile.py` & `morp-5.2.2/morp/interface/dropfile.py`

 * *Files identical despite different names*

### Comparing `morp-5.2.1/morp/interface/sqs.py` & `morp-5.2.2/morp/interface/sqs.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,22 +79,23 @@
         region = self.connection_config.options["region"]
 
         session = boto3.Session(
             region_name=region,
             profile_name=self.connection_config.options.get("profile_name", None),
         )
 
+        session_ttl = self.connection_config.options.get("session_ttl", 3600)
+
         # if an sts arn is given, get credential by assuming given role
         if arn := self.connection_config.options.get("arn", ""):
             sts_client = session.client(
                 service_name="sts",
                 region_name=region,
             )
 
-            session_ttl = self.connection_config.options.get("session_ttl", 3600)
             response = sts_client.assume_role(
                 RoleArn=arn,
                 RoleSessionName=self.connection_config.options.get(
                     "session_name",
                     "morp"
                 ),
                 DurationSeconds=session_ttl,
```

### Comparing `morp-5.2.1/morp/message.py` & `morp-5.2.2/morp/message.py`

 * *Files identical despite different names*

### Comparing `morp-5.2.1/morp.egg-info/PKG-INFO` & `morp-5.2.2/morp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morp
-Version: 5.2.1
+Version: 5.2.2
 Summary: Send and receive messages without thinking about it
 Home-page: http://github.com/Jaymon/morp
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Keywords: Amazon AWS SQS messages message-passing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `morp-5.2.1/setup.py` & `morp-5.2.2/setup.py`

 * *Files identical despite different names*

