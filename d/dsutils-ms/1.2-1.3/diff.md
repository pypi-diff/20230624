# Comparing `tmp/dsutils_ms-1.2.tar.gz` & `tmp/dsutils_ms-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsutils_ms-1.2.tar", last modified: Sat Jun 24 17:44:16 2023, max compression
+gzip compressed data, was "dsutils_ms-1.3.tar", last modified: Sat Jun 24 17:52:15 2023, max compression
```

## Comparing `dsutils_ms-1.2.tar` & `dsutils_ms-1.3.tar`

### file list

```diff
@@ -1,37 +1,42 @@
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.905735 dsutils_ms-1.2/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    34903 2023-05-30 17:35:50.000000 dsutils_ms-1.2/LICENSE.md
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      689 2023-06-24 17:44:16.905735 dsutils_ms-1.2/PKG-INFO
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      125 2023-06-04 01:42:21.000000 dsutils_ms-1.2/README.md
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.901735 dsutils_ms-1.2/dsutils_ms/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/__init__.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.901735 dsutils_ms-1.2/dsutils_ms/adapters/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/adapters/__init__.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2206 2023-06-04 01:19:54.000000 dsutils_ms-1.2/dsutils_ms/adapters/dynamo.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     5336 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/adapters/google_sheets.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1223 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/adapters/interface.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3489 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/adapters/mysql.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3199 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/adapters/s3.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.901735 dsutils_ms-1.2/dsutils_ms/helpers/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/helpers/__init__.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     7202 2023-06-04 00:51:17.000000 dsutils_ms-1.2/dsutils_ms/helpers/cleaning.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      789 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/helpers/dataframe.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      748 2023-06-03 23:40:41.000000 dsutils_ms-1.2/dsutils_ms/helpers/datetime.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      738 2023-06-03 23:40:42.000000 dsutils_ms-1.2/dsutils_ms/helpers/dict.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1026 2023-06-24 17:43:43.000000 dsutils_ms-1.2/dsutils_ms/helpers/env.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      112 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/helpers/google_chat.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      776 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/helpers/log.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.901735 dsutils_ms-1.2/dsutils_ms.egg-info/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      689 2023-06-24 17:44:16.000000 dsutils_ms-1.2/dsutils_ms.egg-info/PKG-INFO
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      788 2023-06-24 17:44:16.000000 dsutils_ms-1.2/dsutils_ms.egg-info/SOURCES.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-06-24 17:44:16.000000 dsutils_ms-1.2/dsutils_ms.egg-info/dependency_links.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      191 2023-06-24 17:44:16.000000 dsutils_ms-1.2/dsutils_ms.egg-info/requires.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       11 2023-06-24 17:44:16.000000 dsutils_ms-1.2/dsutils_ms.egg-info/top_level.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-05-30 18:22:49.000000 dsutils_ms-1.2/dsutils_ms.egg-info/zip-safe
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       80 2023-05-30 17:35:50.000000 dsutils_ms-1.2/pyproject.toml
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1044 2023-06-24 17:44:16.905735 dsutils_ms-1.2/setup.cfg
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       69 2023-05-30 17:35:50.000000 dsutils_ms-1.2/setup.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.905735 dsutils_ms-1.2/tests/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    15766 2023-06-04 01:02:31.000000 dsutils_ms-1.2/tests/test_cleaning.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2980 2023-05-30 17:35:50.000000 dsutils_ms-1.2/tests/test_google_sheets.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3456 2023-05-30 17:35:50.000000 dsutils_ms-1.2/tests/test_mysql.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2342 2023-05-30 17:35:50.000000 dsutils_ms-1.2/tests/test_s3.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:52:15.883163 dsutils_ms-1.3/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    34903 2023-05-30 17:35:50.000000 dsutils_ms-1.3/LICENSE.md
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      689 2023-06-24 17:52:15.883163 dsutils_ms-1.3/PKG-INFO
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      125 2023-06-04 01:42:21.000000 dsutils_ms-1.3/README.md
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:52:15.879163 dsutils_ms-1.3/dsutils_ms/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.3/dsutils_ms/__init__.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:52:15.883163 dsutils_ms-1.3/dsutils_ms/adapters/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.3/dsutils_ms/adapters/__init__.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2206 2023-06-04 01:19:54.000000 dsutils_ms-1.3/dsutils_ms/adapters/dynamo.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     5336 2023-05-30 17:35:50.000000 dsutils_ms-1.3/dsutils_ms/adapters/google_sheets.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1223 2023-05-30 17:35:50.000000 dsutils_ms-1.3/dsutils_ms/adapters/interface.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3489 2023-05-30 17:35:50.000000 dsutils_ms-1.3/dsutils_ms/adapters/mysql.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3199 2023-05-30 17:35:50.000000 dsutils_ms-1.3/dsutils_ms/adapters/s3.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:52:15.883163 dsutils_ms-1.3/dsutils_ms/helpers/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.3/dsutils_ms/helpers/__init__.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     7202 2023-06-04 00:51:17.000000 dsutils_ms-1.3/dsutils_ms/helpers/cleaning.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      789 2023-05-30 17:35:50.000000 dsutils_ms-1.3/dsutils_ms/helpers/dataframe.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      748 2023-06-03 23:40:41.000000 dsutils_ms-1.3/dsutils_ms/helpers/datetime.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      738 2023-06-03 23:40:42.000000 dsutils_ms-1.3/dsutils_ms/helpers/dict.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1062 2023-06-24 17:51:45.000000 dsutils_ms-1.3/dsutils_ms/helpers/env.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      112 2023-05-30 17:35:50.000000 dsutils_ms-1.3/dsutils_ms/helpers/google_chat.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      776 2023-05-30 17:35:50.000000 dsutils_ms-1.3/dsutils_ms/helpers/log.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:52:15.883163 dsutils_ms-1.3/dsutils_ms.egg-info/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      689 2023-06-24 17:52:15.000000 dsutils_ms-1.3/dsutils_ms.egg-info/PKG-INFO
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      895 2023-06-24 17:52:15.000000 dsutils_ms-1.3/dsutils_ms.egg-info/SOURCES.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-06-24 17:52:15.000000 dsutils_ms-1.3/dsutils_ms.egg-info/dependency_links.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      191 2023-06-24 17:52:15.000000 dsutils_ms-1.3/dsutils_ms.egg-info/requires.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       11 2023-06-24 17:52:15.000000 dsutils_ms-1.3/dsutils_ms.egg-info/top_level.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-05-30 18:22:49.000000 dsutils_ms-1.3/dsutils_ms.egg-info/zip-safe
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       80 2023-05-30 17:35:50.000000 dsutils_ms-1.3/pyproject.toml
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1044 2023-06-24 17:52:15.883163 dsutils_ms-1.3/setup.cfg
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       69 2023-05-30 17:35:50.000000 dsutils_ms-1.3/setup.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:52:15.883163 dsutils_ms-1.3/tests/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    15766 2023-06-04 01:02:31.000000 dsutils_ms-1.3/tests/test_cleaning.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      543 2023-06-03 23:40:41.000000 dsutils_ms-1.3/tests/test_datetime.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      832 2023-06-03 23:40:54.000000 dsutils_ms-1.3/tests/test_dict.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1816 2023-06-04 01:22:00.000000 dsutils_ms-1.3/tests/test_dynamo.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      274 2023-06-03 23:40:41.000000 dsutils_ms-1.3/tests/test_env.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      389 2023-06-03 23:40:41.000000 dsutils_ms-1.3/tests/test_google_chat.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2980 2023-05-30 17:35:50.000000 dsutils_ms-1.3/tests/test_google_sheets.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3456 2023-05-30 17:35:50.000000 dsutils_ms-1.3/tests/test_mysql.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2342 2023-05-30 17:35:50.000000 dsutils_ms-1.3/tests/test_s3.py
```

### Comparing `dsutils_ms-1.2/LICENSE.md` & `dsutils_ms-1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/PKG-INFO` & `dsutils_ms-1.3/dsutils_ms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dsutils_ms
-Version: 1.2
+Name: dsutils-ms
+Version: 1.3
 Summary: My Data Science Utils
 Home-page: https://www.linkedin.com/in/matheusserpa/
 Author: Matheus Serpa
 Author-email: matheusserpa@gmail.com
 License: GNU General Public License v3.0
 Keywords: data science,data engineering,machine learning,data analysis,data visualization
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dsutils_ms-1.2/dsutils_ms/adapters/dynamo.py` & `dsutils_ms-1.3/dsutils_ms/adapters/dynamo.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/dsutils_ms/adapters/google_sheets.py` & `dsutils_ms-1.3/dsutils_ms/adapters/google_sheets.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/dsutils_ms/adapters/interface.py` & `dsutils_ms-1.3/dsutils_ms/adapters/interface.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/dsutils_ms/adapters/mysql.py` & `dsutils_ms-1.3/dsutils_ms/adapters/mysql.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/dsutils_ms/adapters/s3.py` & `dsutils_ms-1.3/dsutils_ms/adapters/s3.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/dsutils_ms/helpers/cleaning.py` & `dsutils_ms-1.3/dsutils_ms/helpers/cleaning.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/dsutils_ms/helpers/dataframe.py` & `dsutils_ms-1.3/dsutils_ms/helpers/dataframe.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/dsutils_ms/helpers/datetime.py` & `dsutils_ms-1.3/dsutils_ms/helpers/datetime.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/dsutils_ms/helpers/dict.py` & `dsutils_ms-1.3/dsutils_ms/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/dsutils_ms/helpers/env.py` & `dsutils_ms-1.3/dsutils_ms/helpers/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         if tries > 10:
             raise Exception(".env file not found after 10 tries")
 
     if not exists(PATH + ".env"):
         raise Exception(".env file not found")
 
 
-def get_credential(key: str) -> str:
-    load_env()
+def get_credential(key: str, path_finder: str = "./") -> str:
+    load_env(path_finder)
 
     data = getenv(key)
 
     if data is None:
         raise Exception(f"Environment variable {key} not found")
 
     JSON_CREDENTIALS = ["GOOGLE_SERVICE_ACCOUNT"]
```

### Comparing `dsutils_ms-1.2/dsutils_ms/helpers/log.py` & `dsutils_ms-1.3/dsutils_ms/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/dsutils_ms.egg-info/PKG-INFO` & `dsutils_ms-1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dsutils-ms
-Version: 1.2
+Name: dsutils_ms
+Version: 1.3
 Summary: My Data Science Utils
 Home-page: https://www.linkedin.com/in/matheusserpa/
 Author: Matheus Serpa
 Author-email: matheusserpa@gmail.com
 License: GNU General Public License v3.0
 Keywords: data science,data engineering,machine learning,data analysis,data visualization
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dsutils_ms-1.2/dsutils_ms.egg-info/SOURCES.txt` & `dsutils_ms-1.3/dsutils_ms.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -21,10 +21,15 @@
 dsutils_ms/helpers/dataframe.py
 dsutils_ms/helpers/datetime.py
 dsutils_ms/helpers/dict.py
 dsutils_ms/helpers/env.py
 dsutils_ms/helpers/google_chat.py
 dsutils_ms/helpers/log.py
 tests/test_cleaning.py
+tests/test_datetime.py
+tests/test_dict.py
+tests/test_dynamo.py
+tests/test_env.py
+tests/test_google_chat.py
 tests/test_google_sheets.py
 tests/test_mysql.py
 tests/test_s3.py
```

### Comparing `dsutils_ms-1.2/setup.cfg` & `dsutils_ms-1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsutils_ms
-version = 1.2
+version = 1.3
 author = Matheus Serpa
 author_email = matheusserpa@gmail.com
 url = https://www.linkedin.com/in/matheusserpa/
 description = My Data Science Utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = data science, data engineering, machine learning, data analysis, data visualization
```

### Comparing `dsutils_ms-1.2/tests/test_cleaning.py` & `dsutils_ms-1.3/tests/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/tests/test_google_sheets.py` & `dsutils_ms-1.3/tests/test_google_sheets.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/tests/test_mysql.py` & `dsutils_ms-1.3/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.2/tests/test_s3.py` & `dsutils_ms-1.3/tests/test_s3.py`

 * *Files identical despite different names*

