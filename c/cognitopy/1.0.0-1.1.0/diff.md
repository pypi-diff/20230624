# Comparing `tmp/cognitopy-1.0.0.tar.gz` & `tmp/cognitopy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognitopy-1.0.0.tar", last modified: Thu Jun 15 23:08:14 2023, max compression
+gzip compressed data, was "cognitopy-1.1.0.tar", last modified: Sat Jun 24 19:51:17 2023, max compression
```

## Comparing `cognitopy-1.0.0.tar` & `cognitopy-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:08:14.747016 cognitopy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-15 23:08:05.000000 cognitopy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-15 23:08:14.747016 cognitopy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-15 23:08:05.000000 cognitopy-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-15 23:08:05.000000 cognitopy-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 23:08:14.747016 cognitopy-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:08:14.747016 cognitopy-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 23:08:05.000000 cognitopy-1.0.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:08:14.747016 cognitopy-1.0.0/src/cognitopy/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 23:08:05.000000 cognitopy-1.0.0/src/cognitopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-06-15 23:08:05.000000 cognitopy-1.0.0/src/cognitopy/cognitopy.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-15 23:08:05.000000 cognitopy-1.0.0/src/cognitopy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:08:14.747016 cognitopy-1.0.0/src/cognitopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-15 23:08:14.000000 cognitopy-1.0.0/src/cognitopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-15 23:08:14.000000 cognitopy-1.0.0/src/cognitopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:08:14.000000 cognitopy-1.0.0/src/cognitopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 23:08:14.000000 cognitopy-1.0.0/src/cognitopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:51:17.768737 cognitopy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-24 19:51:06.000000 cognitopy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-24 19:51:17.768737 cognitopy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-24 19:51:06.000000 cognitopy-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-24 19:51:06.000000 cognitopy-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:51:17.768737 cognitopy-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:51:17.768737 cognitopy-1.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:51:06.000000 cognitopy-1.1.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:51:17.768737 cognitopy-1.1.0/src/cognitopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 19:51:06.000000 cognitopy-1.1.0/src/cognitopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24001 2023-06-24 19:51:06.000000 cognitopy-1.1.0/src/cognitopy/cognitopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-24 19:51:06.000000 cognitopy-1.1.0/src/cognitopy/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-24 19:51:06.000000 cognitopy-1.1.0/src/cognitopy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:51:17.768737 cognitopy-1.1.0/src/cognitopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-24 19:51:17.000000 cognitopy-1.1.0/src/cognitopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-24 19:51:17.000000 cognitopy-1.1.0/src/cognitopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:51:17.000000 cognitopy-1.1.0/src/cognitopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-24 19:51:17.000000 cognitopy-1.1.0/src/cognitopy.egg-info/top_level.txt
```

### Comparing `cognitopy-1.0.0/LICENSE` & `cognitopy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognitopy-1.0.0/PKG-INFO` & `cognitopy-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,9 @@
-Metadata-Version: 2.1
-Name: cognitopy
-Version: 1.0.0
-Summary: Python package to use aws cognito in a simple way
-Author-email: Daniel Muñoz Gonzalez <dani16595@gmail.com>
-Project-URL: Homepage, https://github.com/DaniMG95/cognitopy
-Project-URL: Bug Tracker, https://github.com/DaniMG95/cognitopy/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[![PyPI version](https://img.shields.io/pypi/v/cognitopy.svg?style=plastic)](https://pypi.org/project/cognitopy/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/cognitopy?style=plastic)
 
 # cognitopy
 This is a package that will allow you to use the aws Cognito technology, so for now we are going to allow the management of users, authentication and creation of groups by Roles.  
 The potential of this package is the ease of management of all these functionalities and only creating an object with 3 parameters.
 
 ## Installation
 ```bash
@@ -29,124 +18,225 @@
 import os
 
 os.environ["AWS_ACCESS_KEY_ID"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
 os.environ["AWS_SECRET_ACCESS_KEY"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
 ```
 
 ## Usage
-To define the cognitopy object it is necessary to give it the userpool_id, the client_id and the client_secret information.
+To define the cognitopy object it is necessary to give it the userpool_id, the client_id and the client_secret information.  
+The secret_hash parameter is set to False by default and indicates that for requests it is necessary to provide the secret_hash.
 ```python
 from cognitopy import CognitoPy
 
 COGNITO_USERPOOL_ID = 'XXX-XXX-XXXXXX'
 COGNITO_APP_CLIENT_ID = 'XXXXXXXXXXXXXXXXXXXXXXXX'
 COGNITO_APP_CLIENTE_SECRET = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'
 
-cognito = CognitoPy(userpool_id=COGNITO_USERPOOL_ID, client_id=COGNITO_APP_CLIENT_ID, client_secret=COGNITO_APP_CLIENTE_SECRET)
+cognitopy = CognitoPy(
+    userpool_id=COGNITO_USERPOOL_ID, client_id=COGNITO_APP_CLIENT_ID, client_secret=COGNITO_APP_CLIENTE_SECRET,
+    secret_hash=True
+)
 ```
 
 Now I will explain the different functions that we can use in this version, with an example.  
-All these examples are in the directory example
+All these examples are in the directory example.
+
+### Using context manager
+It will allow us to use the cognitopy object in a context manager, so that we do not have to worry about closing the connection.
+```python
+with CognitoPy(userpool_id=COGNITO_USERPOOL_ID, client_id=COGNITO_APP_CLIENT_ID,
+               client_secret=COGNITO_APP_CLIENTE_SECRET) as cognito:
+    cognito.register(username="XXXXX@mail.to", password="XXXXXXX8", user_attributes={})
+```
 
 ### Register a new user
 It will register a user in our cognito service and send us a confirmation message.
 ```python
-cognitopy.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
+cognito.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
 ```
 
 ### Confirm a new user
 It is responsible for confirming the user from the number received by mail.
 ```python
-cognitopy.confirm_sing_up(username='XXXXX@mail.to', confirmation_code='820850')
+cognito.confirm_register(username='XXXXX@mail.to', confirmation_code='820850')
 ```
 
 ### Resend confirm code
 It allows us to receive a confirmation code again, when we have previously requested to change password or register.
 ```python
-cognitopy.resend_confirmation_code(username='XXXXX@mail.to')
+cognito.resend_confirmation_code(username='XXXXX@mail.to')
 ```
 
 ### Login a user
 It will return the access token and refresh token of a confirmed user.
 ```python
-tokens = cognitopy.login(username='XXXXX@mail.to', password='XXXXXXX')
+tokens = cognito.login(username='XXXXX@mail.to', password='XXXXXXX')
 print(tokens['access_token'], tokens['refresh_token'])
 ```
 
 ### Refresh access token
-It will renew the user's access token
+It will renew the user's access token.
 ```python
-access_token = cognitopy.renew_access_token(access_token='XXXXXXXXX', refresh_token='XXXXXXXXX')
+access_token = cognito.renew_access_token(access_token='XXXXXXXXX', refresh_token='XXXXXXXXX')
 print(access_token)
 ```
 
 ### Check if access token is expired
-Check if the access token has expired
+Check if the access token has expired.
 ```python
-is_expired = cognitopy.check_expired_token(access_token='XXXXXXXXX')
+is_expired = cognito.check_expired_token(access_token='XXXXXXXXX')
 print(is_expired)
 ```
 
 ### Forgot password
 Allows us to change our password by sending us a confirmation code.
 ```python
-cognitopy.initiate_forgot_password(username='XXXXX@mail.to')
+cognito.initiate_forgot_password(username='XXXXX@mail.to')
 ```
 
 ### Confirm forgot password
 Change the password of a user from the confirmation code received.
 ```python
-cognitopy.confirm_forgot_password(username='XXXXX@mail.to', confirmation_code='YYYYY', password='XXXXXXX')
+cognito.confirm_forgot_password(username='XXXXX@mail.to', confirmation_code='YYYYY', password='XXXXXXX')
 ```
 
 ### Delete user
-Delete the user from his access token
+Delete the user from his access token.
 ```python
-cognitopy.delete_user(access_token='XXXXXXXXX')
+cognito.delete_user(access_token='XXXXXXXXX')
 ```
 
 ### Change password
-Change the password from your access token
+Change the password from your access token.
 ```python
-cognitopy.change_password(access_token='XXXXXXXXX', previous_password='XXXXXXX', proposed_password="XXXXXXX")
+cognito.change_password(access_token='XXXXXXXXX', previous_password='XXXXXXX', proposed_password="XXXXXXX")
 ```
 
 ### Get user information
 We obtain basic user information from the user's access token.
 ```python
-data_user = cognitopy.get_info_user_by_token(access_token='XXXXXXXXX')
+data_user = cognito.get_info_user_by_token(access_token='XXXXXXXXX')
 print(data_user['username'], data_user['groups'])
 ```
 
 ### Admin delete user
-We remove a user from our service from the administrator credentials
+We remove a user from our service from the administrator credentials.
 ```python
-cognitopy.admin_delete_user(username='XXXXX@mail.to')
+cognito.admin_delete_user(username='XXXXX@mail.to')
 ```
 
 ### Admin create group
-We create a group from our service from the administrator credentials
+We create a group from our service from the administrator credentials.
 precedence: A non-negative integer value that specifies the precedence of this group relative to the other groups that a user can belong to in the user pool. Zero is the highest precedence value. Groups with lower Precedence values take precedence over groups with higher or null Precedence values.
 role_arn: The role Amazon Resource Name (ARN) for the group.
 ```python
-cognitopy.admin_create_group(group_name='test_group', description='test group', precedence=1)
+cognito.admin_create_group(group_name='test_group', description='test group', precedence=1)
 ```
 
 ### Admin delete group
-We remove a group from our service from the administrator credentials
+We remove a group from our service from the administrator credentials.
 ```python
-cognitopy.admin_delete_group(group_name='test_group')
+cognito.admin_delete_group(group_name='test_group')
 ```
 
 ### Admin add user to group
-We add a user to group from our service from the administrator credentials
+We add a user to group from our service from the administrator credentials.
 ```python
-cognitopy.admin_add_user_to_group(username='XXXXX@mail.to', group_name='test_group')
+cognito.admin_add_user_to_group(username='XXXXX@mail.to', group_name='test_group')
 ```
 
 ### Admin remove user from group
-We remove a user to group from our service from the administrator credentials
+We remove a user to group from our service from the administrator credentials.
+```python
+cognito.admin_remove_user_from_group(username='XXXXX@mail.to', group_name='test_group')
+```
+
+
+### Admin confirm user registration
+We confirm a user register from the administrator credentials.
+```python
+cognito.admin_confirm_register(username="XXXXX@mail.to")
+```
+
+
+### Admin create user
+We create a user from the administrator credentials.  
+message_action = MessageAction.SUPPRESS | MessageAction.RESEND  
+Set to RESEND to resend the invitation message to a user that already exists and reset the expiration limit on the user’s account. Set to SUPPRESS to suppress sending the message.  
+desired_delivery = [DesiredDelivery.EMAIL | DesiredDelivery.SMS] or [DesiredDelivery.EMAIL, DesiredDelivery.SMS]  
+Specify EMAIL if email will be used to send the welcome message. Specify SMS if the phone number will be used.  
+optional temporary_password  
 ```python
-cognitopy.admin_remove_user_from_group(username='XXXXX@mail.to', group_name='test_group')
+cognito.admin_create_user(username="XXXXX@mail.to", force_alias=True, user_attributes={},
+                          message_action=MessageAction.SUPPRESS, desired_delivery=[DesiredDelivery.EMAIL],
+                          temporary_password="XXXXXXX")
 ```
 
+### Admin disable user
+We disable a user from the administrator credentials.
+```python
+cognito.admin_disable_user(username="XXXXX@mail.to")
+```
+
+
+### Admin enable user
+We enabled a user from the administrator credentials.
+```python
+cognito.admin_enable_user(username="XXXXX@mail.to")
+```
 
+### Admin get user
+We get info about a user from the administrator credentials.
+```python
+data_user = cognito.admin_get_user(username="XXXXX@mail.to")
+print(data_user)
+```
+
+
+### Admin login
+We login a user from the administrator credentials.
+```python
+tokens = cognito.admin_login(username="XXXXX@mail.to", password="XXXXXXX")
+print(tokens)
+```
+
+
+### Admin renew access token
+We renew access token a user from the administrator credentials.
+```python
+token = cognito.admin_renew_access_token(access_token="XXXXX", refresh_token="XXXXXXX")
+print(token)
+```
+
+
+### Admin list groups for user
+We list groups for user from the administrator credentials.
+```python
+groups = cognito.admin_list_groups_for_user(username="XXXXX@mail.to", limit=10)
+print(groups)
+groups = cognito.admin_list_groups_for_user(username="XXXXX@mail.to", limit=10, next_token=groups["NextToken"])
+print(groups)
+```
+
+
+### Admin reset password
+We reset password from the administrator credentials.  
+After applying this function it will be necessary to launch the initiate_forgot_password function, since the user's password will be disabled.
+```python
+cognito.admin_reset_password(username="XXXXX@mail.to")
+```
+
+
+### Resolve challenge sms mfa
+We resolve challenge sms mfa.
+```python
+tokens = cognito.resolve_challenge_challenge_sms_mfa(username="XXXXX@mail.to", session="XXXXXX", sms_mfa_code="XXXXXX")
+print(tokens)
+```
+
+
+### Resolve challenge new password required
+We resolve challenge new password required.
+```python
+tokens = cognito.resolve_challenge_new_password(username="XXXXX@mail.to", session="XXXXXX", new_password="XXXXXX")
+print(tokens)
+```
```

### Comparing `cognitopy-1.0.0/pyproject.toml` & `cognitopy-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "cognitopy"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Daniel Muñoz Gonzalez", email="dani16595@gmail.com" },
 ]
 description = "Python package to use aws cognito in a simple way"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

