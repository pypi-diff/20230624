# Comparing `tmp/sepm-api-0.0.4.tar.gz` & `tmp/sepm-api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sepm-api-0.0.4.tar", last modified: Thu May 18 19:45:44 2023, max compression
+gzip compressed data, was "sepm-api-0.0.5.tar", last modified: Fri Jun 23 23:31:38 2023, max compression
```

## Comparing `sepm-api-0.0.4.tar` & `sepm-api-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-05-18 19:45:44.100006 sepm-api-0.0.4/
--rw-r--r--   0 aalmero    (501) staff       (20)     1077 2023-01-23 20:35:31.000000 sepm-api-0.0.4/LICENSE
--rw-r--r--   0 aalmero    (501) staff       (20)     1865 2023-05-18 19:45:44.099681 sepm-api-0.0.4/PKG-INFO
--rw-r--r--   0 aalmero    (501) staff       (20)     1478 2023-05-05 16:15:17.000000 sepm-api-0.0.4/README.rst
-drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-05-18 19:45:44.065282 sepm-api-0.0.4/sepm/
--rw-r--r--   0 aalmero    (501) staff       (20)     5536 2023-04-27 18:18:13.000000 sepm-api-0.0.4/sepm/__init__.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1090 2023-04-26 19:25:54.000000 sepm-api-0.0.4/sepm/config.py
-drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-05-18 19:45:44.095510 sepm-api-0.0.4/sepm/endpoints/
--rw-r--r--   0 aalmero    (501) staff       (20)        0 2023-01-25 18:19:20.000000 sepm-api-0.0.4/sepm/endpoints/__init__.py
--rw-r--r--   0 aalmero    (501) staff       (20)    11653 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/administrators.py
--rw-r--r--   0 aalmero    (501) staff       (20)     4708 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/blacklist.py
--rw-r--r--   0 aalmero    (501) staff       (20)     4780 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/cloud.py
--rw-r--r--   0 aalmero    (501) staff       (20)    17544 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/commands.py
--rw-r--r--   0 aalmero    (501) staff       (20)     6805 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/computers.py
--rw-r--r--   0 aalmero    (501) staff       (20)      905 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/content.py
--rw-r--r--   0 aalmero    (501) staff       (20)     4591 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/domains.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1448 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/events.py
--rw-r--r--   0 aalmero    (501) staff       (20)      784 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/group_update_provider.py
--rw-r--r--   0 aalmero    (501) staff       (20)    38197 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/groups.py
--rw-r--r--   0 aalmero    (501) staff       (20)     2243 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/identity.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1054 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/notifications.py
--rw-r--r--   0 aalmero    (501) staff       (20)    25446 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/policies.py
--rw-r--r--   0 aalmero    (501) staff       (20)     2460 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/replication.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1135 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/reporting.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1267 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/requested_files.py
--rw-r--r--   0 aalmero    (501) staff       (20)     8058 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/statistics.py
--rw-r--r--   0 aalmero    (501) staff       (20)     6198 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/threat_defense_for_active_directory.py
--rw-r--r--   0 aalmero    (501) staff       (20)      800 2023-04-25 15:56:27.000000 sepm-api-0.0.4/sepm/endpoints/version.py
--rw-r--r--   0 aalmero    (501) staff       (20)     1108 2023-01-25 18:47:14.000000 sepm-api-0.0.4/sepm/exceptions.py
--rw-r--r--   0 aalmero    (501) staff       (20)     7830 2023-04-25 15:04:42.000000 sepm-api-0.0.4/sepm/rest_api_session.py
-drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-05-18 19:45:44.098446 sepm-api-0.0.4/sepm_api.egg-info/
--rw-r--r--   0 aalmero    (501) staff       (20)     1865 2023-05-18 19:45:44.000000 sepm-api-0.0.4/sepm_api.egg-info/PKG-INFO
--rw-r--r--   0 aalmero    (501) staff       (20)      848 2023-05-18 19:45:44.000000 sepm-api-0.0.4/sepm_api.egg-info/SOURCES.txt
--rw-r--r--   0 aalmero    (501) staff       (20)        1 2023-05-18 19:45:44.000000 sepm-api-0.0.4/sepm_api.egg-info/dependency_links.txt
--rw-r--r--   0 aalmero    (501) staff       (20)        5 2023-05-18 19:45:44.000000 sepm-api-0.0.4/sepm_api.egg-info/top_level.txt
--rw-r--r--   0 aalmero    (501) staff       (20)       38 2023-05-18 19:45:44.100104 sepm-api-0.0.4/setup.cfg
--rw-r--r--   0 aalmero    (501) staff       (20)      893 2023-04-27 19:16:04.000000 sepm-api-0.0.4/setup.py
-drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-05-18 19:45:44.098876 sepm-api-0.0.4/tests/
--rw-r--r--   0 aalmero    (501) staff       (20)       98 2023-01-23 20:35:31.000000 sepm-api-0.0.4/tests/test_sample.py
+drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-06-23 23:31:38.252851 sepm-api-0.0.5/
+-rw-r--r--   0 aalmero    (501) staff       (20)     1077 2023-01-23 20:35:31.000000 sepm-api-0.0.5/LICENSE
+-rw-r--r--   0 aalmero    (501) staff       (20)     1911 2023-06-23 23:31:38.252460 sepm-api-0.0.5/PKG-INFO
+-rw-r--r--   0 aalmero    (501) staff       (20)     1524 2023-06-23 22:55:18.000000 sepm-api-0.0.5/README.rst
+drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-06-23 23:31:38.211078 sepm-api-0.0.5/sepm/
+-rw-r--r--   0 aalmero    (501) staff       (20)     5536 2023-06-23 22:49:41.000000 sepm-api-0.0.5/sepm/__init__.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1090 2023-04-26 19:25:54.000000 sepm-api-0.0.5/sepm/config.py
+drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-06-23 23:31:38.247334 sepm-api-0.0.5/sepm/endpoints/
+-rw-r--r--   0 aalmero    (501) staff       (20)        0 2023-01-25 18:19:20.000000 sepm-api-0.0.5/sepm/endpoints/__init__.py
+-rw-r--r--   0 aalmero    (501) staff       (20)    11653 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/administrators.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     4708 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/blacklist.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     4780 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/cloud.py
+-rw-r--r--   0 aalmero    (501) staff       (20)    17544 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/commands.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     6805 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/computers.py
+-rw-r--r--   0 aalmero    (501) staff       (20)      905 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/content.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     4591 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/domains.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1448 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/events.py
+-rw-r--r--   0 aalmero    (501) staff       (20)      784 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/group_update_provider.py
+-rw-r--r--   0 aalmero    (501) staff       (20)    38197 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/groups.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     2243 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/identity.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1054 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/notifications.py
+-rw-r--r--   0 aalmero    (501) staff       (20)    25446 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/policies.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     2460 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/replication.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1135 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/reporting.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1267 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/requested_files.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     8058 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/statistics.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     6198 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/threat_defense_for_active_directory.py
+-rw-r--r--   0 aalmero    (501) staff       (20)      800 2023-04-25 15:56:27.000000 sepm-api-0.0.5/sepm/endpoints/version.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     1108 2023-01-25 18:47:14.000000 sepm-api-0.0.5/sepm/exceptions.py
+-rw-r--r--   0 aalmero    (501) staff       (20)     7836 2023-06-23 23:27:54.000000 sepm-api-0.0.5/sepm/rest_api_session.py
+drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-06-23 23:31:38.250637 sepm-api-0.0.5/sepm_api.egg-info/
+-rw-r--r--   0 aalmero    (501) staff       (20)     1911 2023-06-23 23:31:38.000000 sepm-api-0.0.5/sepm_api.egg-info/PKG-INFO
+-rw-r--r--   0 aalmero    (501) staff       (20)      848 2023-06-23 23:31:38.000000 sepm-api-0.0.5/sepm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 aalmero    (501) staff       (20)        1 2023-06-23 23:31:38.000000 sepm-api-0.0.5/sepm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 aalmero    (501) staff       (20)        5 2023-06-23 23:31:38.000000 sepm-api-0.0.5/sepm_api.egg-info/top_level.txt
+-rw-r--r--   0 aalmero    (501) staff       (20)       38 2023-06-23 23:31:38.252968 sepm-api-0.0.5/setup.cfg
+-rw-r--r--   0 aalmero    (501) staff       (20)      893 2023-06-23 22:49:41.000000 sepm-api-0.0.5/setup.py
+drwxr-xr-x   0 aalmero    (501) staff       (20)        0 2023-06-23 23:31:38.251142 sepm-api-0.0.5/tests/
+-rw-r--r--   0 aalmero    (501) staff       (20)       98 2023-01-23 20:35:31.000000 sepm-api-0.0.5/tests/test_sample.py
```

### Comparing `sepm-api-0.0.4/LICENSE` & `sepm-api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/PKG-INFO` & `sepm-api-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sepm-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: Symantec Endpoint Protection Manager API
 Home-page: https://github.com/aalmero/sepm-api
 Author: Alex Almero
 Author-email: aalmero@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -50,14 +50,15 @@
     API_USERNAME
     API_PASSWORD
     API_DOMAIN
     API_BASE_URL  [default: https://localhost:8446/sepm/api/v1]
 
 Compatibility
 -------------
+Symantec Endpoint Protection Manager API 14.3
 
 License
 -------
 
 This software code is license under `MIT <https://github.com/aalmero/sepm-api/blob/main/LICENSE>`_.
 
 Authors
```

### Comparing `sepm-api-0.0.4/README.rst` & `sepm-api-0.0.5/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     API_USERNAME
     API_PASSWORD
     API_DOMAIN
     API_BASE_URL  [default: https://localhost:8446/sepm/api/v1]
 
 Compatibility
 -------------
+Symantec Endpoint Protection Manager API 14.3
 
 License
 -------
 
 This software code is license under `MIT <https://github.com/aalmero/sepm-api/blob/main/LICENSE>`_.
 
 Authors
```

### Comparing `sepm-api-0.0.4/sepm/__init__.py` & `sepm-api-0.0.5/sepm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     LOG_FILE_PREFIX,
     PRINT_TO_CONSOLE,
     SUPPRESS_LOGGING,
     INHERIT_LOGGING_CONFIG,
     SIMULATE_API,
 )
 
-__version__ = '0.0.1'
+__version__ = '0.0.5'
 __author__ = 'Alex Almero <aalmero@gmail.com>'
 __all__ = []
 
 class SymantecEndpointProtectionManagerAPI(object):
     """
     create a persistent Symantec Endpoint Protection Manager API session
     ....
```

### Comparing `sepm-api-0.0.4/sepm/config.py` & `sepm-api-0.0.5/sepm/config.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/administrators.py` & `sepm-api-0.0.5/sepm/endpoints/administrators.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/blacklist.py` & `sepm-api-0.0.5/sepm/endpoints/blacklist.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/cloud.py` & `sepm-api-0.0.5/sepm/endpoints/cloud.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/commands.py` & `sepm-api-0.0.5/sepm/endpoints/commands.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/computers.py` & `sepm-api-0.0.5/sepm/endpoints/computers.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/content.py` & `sepm-api-0.0.5/sepm/endpoints/content.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/domains.py` & `sepm-api-0.0.5/sepm/endpoints/domains.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/events.py` & `sepm-api-0.0.5/sepm/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/group_update_provider.py` & `sepm-api-0.0.5/sepm/endpoints/group_update_provider.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/groups.py` & `sepm-api-0.0.5/sepm/endpoints/groups.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/identity.py` & `sepm-api-0.0.5/sepm/endpoints/identity.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/notifications.py` & `sepm-api-0.0.5/sepm/endpoints/notifications.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/policies.py` & `sepm-api-0.0.5/sepm/endpoints/policies.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/replication.py` & `sepm-api-0.0.5/sepm/endpoints/replication.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/reporting.py` & `sepm-api-0.0.5/sepm/endpoints/reporting.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/requested_files.py` & `sepm-api-0.0.5/sepm/endpoints/requested_files.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/statistics.py` & `sepm-api-0.0.5/sepm/endpoints/statistics.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/threat_defense_for_active_directory.py` & `sepm-api-0.0.5/sepm/endpoints/threat_defense_for_active_directory.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/endpoints/version.py` & `sepm-api-0.0.5/sepm/endpoints/version.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/exceptions.py` & `sepm-api-0.0.5/sepm/exceptions.py`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/sepm/rest_api_session.py` & `sepm-api-0.0.5/sepm/rest_api_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         super(RestApiSession, self).__init__()
 
         # initialize attributes and properties
         self._version = __version__
         self._username = username
         self._password = password
         self._domain = domain
-        self._api_key = "CHANGEME"
+        self._api_key = "CHANGEME" # this will be updated on authn success
         self._base_url = str(base_url)
         self._auth_url = str(auth_url)
         self._simulate = simulate
         self._retry_4xx_error = retry_4xx_error
         self._retry_4xx_error_wait_time = retry_4xx_error_wait_time
         self._maximum_retries = maximum_retries
 
@@ -46,15 +46,14 @@
         payload = {
             "username": self._username,
             "password": self._password,
             "domain": self._domain
         }
 
         auth_req = requests.post(self._auth_url,
-                    verify=False,
                     headers= {"Content-Type": "application/json"},
                     data=json.dumps(payload))
 
         isAuthenticated = False
         if auth_req.status_code == 200:
             isAuthenticated = True
```

### Comparing `sepm-api-0.0.4/sepm_api.egg-info/PKG-INFO` & `sepm-api-0.0.5/sepm_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sepm-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: Symantec Endpoint Protection Manager API
 Home-page: https://github.com/aalmero/sepm-api
 Author: Alex Almero
 Author-email: aalmero@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -50,14 +50,15 @@
     API_USERNAME
     API_PASSWORD
     API_DOMAIN
     API_BASE_URL  [default: https://localhost:8446/sepm/api/v1]
 
 Compatibility
 -------------
+Symantec Endpoint Protection Manager API 14.3
 
 License
 -------
 
 This software code is license under `MIT <https://github.com/aalmero/sepm-api/blob/main/LICENSE>`_.
 
 Authors
```

### Comparing `sepm-api-0.0.4/sepm_api.egg-info/SOURCES.txt` & `sepm-api-0.0.5/sepm_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sepm-api-0.0.4/setup.py` & `sepm-api-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding='utf-8') as fd:
         return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
 
 
 setup(
     name="sepm-api",
-    version="0.0.4",
+    version="0.0.5",
     url="https://github.com/aalmero/sepm-api",
     license='MIT',
 
     author="Alex Almero",
     author_email="aalmero@gmail.com",
 
     description="Symantec Endpoint Protection Manager API",
```

