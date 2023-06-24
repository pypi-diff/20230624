# Comparing `tmp/fastapi_azure_auth-4.1.2.tar.gz` & `tmp/fastapi_azure_auth-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_azure_auth-4.1.2.tar", max compression
+gzip compressed data, was "fastapi_azure_auth-4.1.3.tar", max compression
```

## Comparing `fastapi_azure_auth-4.1.2.tar` & `fastapi_azure_auth-4.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-06-23 13:06:56.105428 fastapi_azure_auth-4.1.2/LICENSE
--rw-r--r--   0        0        0     6468 2023-06-23 13:06:56.105428 fastapi_azure_auth-4.1.2/README.md
--rw-r--r--   0        0        0      339 2023-06-23 13:06:56.125428 fastapi_azure_auth-4.1.2/fastapi_azure_auth/__init__.py
--rw-r--r--   0        0        0    19735 2023-06-23 13:06:56.125428 fastapi_azure_auth-4.1.2/fastapi_azure_auth/auth.py
--rw-r--r--   0        0        0      337 2023-06-23 13:06:56.125428 fastapi_azure_auth-4.1.2/fastapi_azure_auth/exceptions.py
--rw-r--r--   0        0        0     4451 2023-06-23 13:06:56.125428 fastapi_azure_auth-4.1.2/fastapi_azure_auth/openid_config.py
--rw-r--r--   0        0        0        0 2023-06-23 13:06:56.125428 fastapi_azure_auth-4.1.2/fastapi_azure_auth/py.typed
--rw-r--r--   0        0        0     9367 2023-06-23 13:06:56.125428 fastapi_azure_auth-4.1.2/fastapi_azure_auth/user.py
--rw-r--r--   0        0        0      457 2023-06-23 13:06:56.125428 fastapi_azure_auth-4.1.2/fastapi_azure_auth/utils.py
--rw-r--r--   0        0        0     2365 2023-06-23 13:06:56.125428 fastapi_azure_auth-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     8033 1970-01-01 00:00:00.000000 fastapi_azure_auth-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-24 11:26:18.686779 fastapi_azure_auth-4.1.3/LICENSE
+-rw-r--r--   0        0        0     6468 2023-06-24 11:26:18.686779 fastapi_azure_auth-4.1.3/README.md
+-rw-r--r--   0        0        0      339 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/__init__.py
+-rw-r--r--   0        0        0    19735 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/auth.py
+-rw-r--r--   0        0        0      337 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/exceptions.py
+-rw-r--r--   0        0        0     4451 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/openid_config.py
+-rw-r--r--   0        0        0        0 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/py.typed
+-rw-r--r--   0        0        0     9424 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/user.py
+-rw-r--r--   0        0        0      457 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/utils.py
+-rw-r--r--   0        0        0     2365 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8033 1970-01-01 00:00:00.000000 fastapi_azure_auth-4.1.3/PKG-INFO
```

### Comparing `fastapi_azure_auth-4.1.2/LICENSE` & `fastapi_azure_auth-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.1.2/README.md` & `fastapi_azure_auth-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.1.2/fastapi_azure_auth/auth.py` & `fastapi_azure_auth-4.1.3/fastapi_azure_auth/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.1.2/fastapi_azure_auth/openid_config.py` & `fastapi_azure_auth-4.1.3/fastapi_azure_auth/openid_config.py`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.1.2/fastapi_azure_auth/user.py` & `fastapi_azure_auth-4.1.3/fastapi_azure_auth/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         description='Specifies the time after which the JWT can be processed.',
     )
     exp: int = Field(
         ...,
         description='Specifies the expiration time before which the JWT can be accepted for processing.',
     )
     aio: Optional[str] = Field(
-        ...,
+        default=None,
         description='An internal claim used by Azure AD to record data for token reuse. Resources should not use this claim.',
     )
     name: Optional[str] = Field(
         default=None,
         description='Provides a human-readable value that identifies the subject of the token.',
     )
     scp: List[str] = Field(
@@ -70,20 +70,20 @@
         description='The immutable identifier for the requestor, which is the verified identity of the user or service principal',
     )
     tid: str = Field(
         ...,
         description='Represents the tenant that the user is signing in to',
     )
     uti: Optional[str] = Field(
-        ...,
+        default=None,
         description='Token identifier claim, equivalent to jti in the JWT specification. Unique, per-token identifier that is case-sensitive.',
     )
     rh: Optional[str] = Field(
-        ...,
-        description='An internal claim used by Azure to revalidate tokens. Resources should not use this claim.',
+        default=None,
+        description='Token identifier claim, equivalent to jti in the JWT specification. Unique, per-token identifier that is case-sensitive.',
     )
     ver: Literal['1.0', '2.0'] = Field(
         ...,
         description='Indicates the version of the access token.',
     )
 
     # Optional claims, configured in Azure AD
```

### Comparing `fastapi_azure_auth-4.1.2/pyproject.toml` & `fastapi_azure_auth-4.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-azure-auth"
-version = "4.1.2"  # Remember to change in __init__.py as well
+version = "4.1.3"  # Remember to change in __init__.py as well
 description = "Easy and secure implementation of Azure AD for your FastAPI APIs"
 authors = ["Jonas Krüger Svensson <jonas.svensson@intility.no>"]
 readme = "README.md"
 homepage = "https://github.com/intility/fastapi-azure-auth"
 repository = "https://github.com/intility/fastapi-azure-auth"
 documentation = "https://github.com/intility/fastapi-azure-auth"
 keywords = [
```

### Comparing `fastapi_azure_auth-4.1.2/PKG-INFO` & `fastapi_azure_auth-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-azure-auth
-Version: 4.1.2
+Version: 4.1.3
 Summary: Easy and secure implementation of Azure AD for your FastAPI APIs
 Home-page: https://github.com/intility/fastapi-azure-auth
 Keywords: ad,async,asyncio,authentication,azure,azure ad,azuread,fastapi,multi tenant,oauth2,oidc,security,single tenant,starlette,trio
 Author: Jonas Krüger Svensson
 Author-email: jonas.svensson@intility.no
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-azure-auth Version: 4.1.2 Summary: Easy and
+Metadata-Version: 2.1 Name: fastapi-azure-auth Version: 4.1.3 Summary: Easy and
 secure implementation of Azure AD for your FastAPI APIs Home-page: https://
 github.com/intility/fastapi-azure-auth Keywords:
 ad,async,asyncio,authentication,azure,azure ad,azuread,fastapi,multi
 tenant,oauth2,oidc,security,single tenant,starlette,trio Author: Jonas KrÃ¼ger
 Svensson Author-email: jonas.svensson@intility.no Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Intended Audience :: Developers Classifier:
```

