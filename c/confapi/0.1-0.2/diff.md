# Comparing `tmp/confapi-0.1.tar.gz` & `tmp/confapi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confapi-0.1.tar", last modified: Wed Jun 21 03:23:24 2023, max compression
+gzip compressed data, was "confapi-0.2.tar", last modified: Fri Jun 23 23:02:12 2023, max compression
```

## Comparing `confapi-0.1.tar` & `confapi-0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:23:24.494293 confapi-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 03:23:09.000000 confapi-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-21 03:23:24.490293 confapi-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 03:23:09.000000 confapi-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:23:24.490293 confapi-0.1/confapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-21 03:23:24.000000 confapi-0.1/confapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 03:23:24.000000 confapi-0.1/confapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:23:24.000000 confapi-0.1/confapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 03:23:24.000000 confapi-0.1/confapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 03:23:24.000000 confapi-0.1/confapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:23:24.490293 confapi-0.1/confclient/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-21 03:23:09.000000 confapi-0.1/confclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-21 03:23:09.000000 confapi-0.1/confclient/confexcept.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-21 03:23:09.000000 confapi-0.1/confclient/restclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-21 03:23:09.000000 confapi-0.1/confclient/rpcclient.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 03:23:24.494293 confapi-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-21 03:23:09.000000 confapi-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:23:24.490293 confapi-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-21 03:23:09.000000 confapi-0.1/tests/test_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:02:12.376821 confapi-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 23:01:57.000000 confapi-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-23 23:02:12.372821 confapi-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-23 23:01:57.000000 confapi-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:02:12.372821 confapi-0.2/confapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-23 23:02:12.000000 confapi-0.2/confapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-23 23:02:12.000000 confapi-0.2/confapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:02:12.000000 confapi-0.2/confapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 23:02:12.000000 confapi-0.2/confapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 23:02:12.000000 confapi-0.2/confapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:02:12.372821 confapi-0.2/confclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-23 23:01:57.000000 confapi-0.2/confclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-23 23:01:57.000000 confapi-0.2/confclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-23 23:01:57.000000 confapi-0.2/confclient/confexcept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-23 23:01:57.000000 confapi-0.2/confclient/restclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-06-23 23:01:57.000000 confapi-0.2/confclient/rpcclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:02:12.376821 confapi-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-23 23:01:57.000000 confapi-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:02:12.372821 confapi-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-23 23:01:57.000000 confapi-0.2/tests/test_conf_client.py
```

### Comparing `confapi-0.1/LICENSE` & `confapi-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `confapi-0.1/confclient/confexcept.py` & `confapi-0.2/confclient/confexcept.py`

 * *Files identical despite different names*

### Comparing `confapi-0.1/confclient/rpcclient.py` & `confapi-0.2/confclient/rpcclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,31 +27,31 @@
 # ----------------- Class Definitions -------------------
 
 
 class RPCClient:
     """RPCClient for interacting with Confluence
 
     Attributes:
-        url: str = Base Url of Confluence server, E.G https://my.confluence.server.com
+        url: str = Base Url of Confluence server, e.g. https://my.confluence.server.com
         username: str = Username of Confluence user with administrator privelege
         password: str = Password of Confluence user with administrator privelege
                 NOTE: Many functionalities will fail without administrator privelege!
     """
 
     def __init__(self, url: str, username: str, password: str, version="2.0"):
         """Stores attributes needed for API calls
 
         See argument explanations above
         """
-        self.url = url + RPC_ENDPOINT
+        self.url = url
         self.username = username
         self.password = password
         self.version = version
 
-    def _execute(
+    def _execute_rpc(
         self, method: str, params: list[str | dict | bool]
     ) -> requests.Response:
         """Preform API call to endpoint
 
         Args:
             method: str = The RPC method to be called
             params: list = The arguments you would like to
@@ -65,25 +65,26 @@
             "jsonrpc": self.version,
             "method": method,
             "params": params,
             "id": random.randint(1000, 2000),
         }
 
         response = requests.post(
-            self.url,
+            self.url + RPC_ENDPOINT,
             json=data,
             auth=requests.auth.HTTPBasicAuth(self.username, self.password),
             timeout=10,
         )
 
         # Ensure non-failed request, fail hard and fast
-        if response.status_code != 200:
-            raise BadRPCRequestException(
-                f"Error: Status Code {response.status_code} Encountered,\n{response.text}"
-            )
+        # UPDATE: RPC always returns 200 status code
+        # if response.status_code != 200:
+        #     raise BadRPCRequestException(
+        #         f"Error: Status Code {response.status_code} Encountered,\n{response.text}"
+        #     )
 
         if "error" in response.json():
             error = response.json()["error"]
             raise BadRPCRequestException(f"Error ({error['code']}): {error['message']}")
 
         return response
 
@@ -112,15 +113,15 @@
             notify_user: bool = flag to indicate whether or not to send users an email
                                 notifying them of account creation
 
         Returns:
             RPC API request response
         """
 
-        return self._execute(
+        return self._execute_rpc(
             "addUser",
             [
                 {"name": username, "fullname": fullname, "email": email},
                 password,
                 notify_user,
             ],
         )
@@ -137,15 +138,15 @@
         Args:
             username: str = Confluence username of user to create
 
         Returns:
             RPC API request response
         """
 
-        return self._execute("removeUser", [username])
+        return self._execute_rpc("removeUser", [username])
 
     def add_user_to_group(self, username: str, group: str) -> requests.Response:
         """Invoke RPC endpoint for adding user to a group in Confluence
 
         RPC documentation here:
             https://developer.atlassian.com/server/confluence/remote-confluence-methods/#user-management
                 - addUserToGroup
@@ -154,15 +155,15 @@
             username: str = Confluence username of user to add to group
             group: str = name of the group to add the user to
 
         Returns:
             RPC API request response
         """
 
-        return self._execute("addUserToGroup", [username, group])
+        return self._execute_rpc("addUserToGroup", [username, group])
 
     def remove_user_from_group(self, username: str, group: str) -> requests.Response:
         """Invoke RPC endpoint for removing a user form a group in Confluence
 
         RPC documentation here:
             https://developer.atlassian.com/server/confluence/remote-confluence-methods/#user-management
                 - removeUserFromGroup
@@ -171,15 +172,15 @@
             username: str = Confluence username of user to remove from the group
             group: str = name of the group to remove the user from
 
         Returns:
             RPC API request response
         """
 
-        return self._execute("removeUserFromGroup", [username, group])
+        return self._execute_rpc("removeUserFromGroup", [username, group])
 
     def add_group(self, group):
         """Invoke RPC endpoint for creating a new group in Confluence
 
         RPC documentation here:
             https://developer.atlassian.com/server/confluence/remote-confluence-methods/#user-management
                 - addGroup
@@ -187,15 +188,15 @@
         Args:
             group: str = name of the group to create
 
         Returns:
             RPC API request response
         """
 
-        return self._execute("addGroup", [group])
+        return self._execute_rpc("addGroup", [group])
 
     def remove_group(self, group):
         """Invoke RPC endpoint for removing group in Confluence
 
         RPC documentation here:
             https://developer.atlassian.com/server/confluence/remote-confluence-methods/#user-management
                 - removeGroup
@@ -203,8 +204,8 @@
         Args:
             group: str = name of the group to remove
 
         Returns:
             RPC API request response
         """
 
-        return self._execute("removeGroup", [group])
+        return self._execute_rpc("removeGroup", [group, ""])
```

