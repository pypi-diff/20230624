# Comparing `tmp/customgpt_client-1.0.6-py3-none-any.whl.zip` & `tmp/customgpt_client-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 305221 bytes, number of entries: 376
+Zip file size: 305215 bytes, number of entries: 376
 -rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 custom_gpt_client/__init__.py
 -rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 custom_gpt_client/api/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 custom_gpt_client/api/citations/__init__.py
 -rw-r--r--  2.0 unx     6513 b- defN 80-Jan-01 00:00 custom_gpt_client/api/citations/get_open_graph_data_for_citation.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 custom_gpt_client/api/conversations/__init__.py
 -rw-r--r--  2.0 unx     7370 b- defN 80-Jan-01 00:00 custom_gpt_client/api/conversations/create_project_conversation.py
 -rw-r--r--  2.0 unx     6970 b- defN 80-Jan-01 00:00 custom_gpt_client/api/conversations/delete_project_conversation.py
@@ -368,11 +368,11 @@
 -rw-r--r--  2.0 unx     3189 b- defN 80-Jan-01 00:00 custom_gpt_client/models/update_user_profile_response_500.py
 -rw-r--r--  2.0 unx     2351 b- defN 80-Jan-01 00:00 custom_gpt_client/models/update_user_profile_response_500_data.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 custom_gpt_client/models/update_user_profile_response_500_data_code.py
 -rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 custom_gpt_client/models/update_user_profile_response_500_status.py
 -rw-r--r--  2.0 unx     3791 b- defN 80-Jan-01 00:00 custom_gpt_client/models/user.py
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 custom_gpt_client/py.typed
 -rw-r--r--  2.0 unx      993 b- defN 80-Jan-01 00:00 custom_gpt_client/types.py
--rw-r--r--  2.0 unx     1228 b- defN 80-Jan-01 00:00 customgpt_client-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 customgpt_client-1.0.6.dist-info/WHEEL
-?rw-r--r--  2.0 unx    44882 b- defN 16-Jan-01 00:00 customgpt_client-1.0.6.dist-info/RECORD
-376 files, 879962 bytes uncompressed, 229239 bytes compressed:  73.9%
+-rw-r--r--  2.0 unx     1227 b- defN 80-Jan-01 00:00 customgpt_client-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 customgpt_client-1.0.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx    44882 b- defN 16-Jan-01 00:00 customgpt_client-1.0.7.dist-info/RECORD
+376 files, 879961 bytes uncompressed, 229233 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -1113,17 +1113,17 @@
 
 Filename: custom_gpt_client/py.typed
 Comment: 
 
 Filename: custom_gpt_client/types.py
 Comment: 
 
-Filename: customgpt_client-1.0.6.dist-info/METADATA
+Filename: customgpt_client-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: customgpt_client-1.0.6.dist-info/WHEEL
+Filename: customgpt_client-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: customgpt_client-1.0.6.dist-info/RECORD
+Filename: customgpt_client-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `customgpt_client-1.0.6.dist-info/METADATA` & `customgpt_client-1.0.7.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customgpt-client
-Version: 1.0.6
+Version: 1.0.7
 Summary: A client library for accessing CustomGPT
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,15 +15,15 @@
 
 # CustomGPT SDK
 
 ## Usage
 First, create a client:
 
 ```python
-from {{ package_name }} import CustomGPT
+from custom_gpt_client import CustomGPT
 
 CustomGPT.api_key="SuperSecretToken"
 ```
 
 Now you can access to all of our Models:
 Example Request will be like this:
```

## Comparing `customgpt_client-1.0.6.dist-info/RECORD` & `customgpt_client-1.0.7.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -367,10 +367,10 @@
 custom_gpt_client/models/update_user_profile_response_500.py,sha256=vE_fP4yX8UVMMbO-96_tctsZ8YsdS1D2AF7q5mFsRNk,3189
 custom_gpt_client/models/update_user_profile_response_500_data.py,sha256=MAg1i8t243owgdIi0NdEPNLAPxypRLrVIiWb_iuSpBc,2351
 custom_gpt_client/models/update_user_profile_response_500_data_code.py,sha256=o-GDpigGzvI3qFGG1HstdR5Lx5p508fuGNvkauwP9s8,262
 custom_gpt_client/models/update_user_profile_response_500_status.py,sha256=sX5mpQWL7wNrEpdCiSpvQgsm1f6kaNvLlPmfSkzW-I8,183
 custom_gpt_client/models/user.py,sha256=Wlz5CcnbrVuJswNviFnkEthU9gCAV8GvPfnEE5DTKhI,3791
 custom_gpt_client/py.typed,sha256=8ZJUsxZiuOy1oJeVhsTWQhTG_6pTVHVXk5hJL79ebTk,25
 custom_gpt_client/types.py,sha256=4xaUIOliefW-5jz_p-JT2LO7-V0wKWaniHGtjPBQfvQ,993
-customgpt_client-1.0.6.dist-info/METADATA,sha256=usGaKAe1MDsPv9wLQlJ33ZT4XlwV0ZYFcsbnMyxU5GY,1228
-customgpt_client-1.0.6.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-customgpt_client-1.0.6.dist-info/RECORD,,
+customgpt_client-1.0.7.dist-info/METADATA,sha256=EWfzMHd7gD2l5RGdai9lMz74bsgtiAxFK9tmH0dylUQ,1227
+customgpt_client-1.0.7.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+customgpt_client-1.0.7.dist-info/RECORD,,
```

