# Comparing `tmp/dsutils_ms-1.1.tar.gz` & `tmp/dsutils_ms-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsutils_ms-1.1.tar", last modified: Sun Jun  4 01:26:38 2023, max compression
+gzip compressed data, was "dsutils_ms-1.2.tar", last modified: Sat Jun 24 17:44:16 2023, max compression
```

## Comparing `dsutils_ms-1.1.tar` & `dsutils_ms-1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.521625 dsutils_ms-1.1/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    34903 2023-05-30 17:35:50.000000 dsutils_ms-1.1/LICENSE.md
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      635 2023-06-04 01:26:38.521625 dsutils_ms-1.1/PKG-INFO
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       71 2023-05-30 17:35:50.000000 dsutils_ms-1.1/README.md
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.513625 dsutils_ms-1.1/dsutils_ms/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/__init__.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.513625 dsutils_ms-1.1/dsutils_ms/adapters/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/adapters/__init__.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2206 2023-06-04 01:19:54.000000 dsutils_ms-1.1/dsutils_ms/adapters/dynamo.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     5336 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/adapters/google_sheets.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1223 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/adapters/interface.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3489 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/adapters/mysql.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3199 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/adapters/s3.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.517624 dsutils_ms-1.1/dsutils_ms/helpers/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/helpers/__init__.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     7202 2023-06-04 00:51:17.000000 dsutils_ms-1.1/dsutils_ms/helpers/cleaning.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      789 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/helpers/dataframe.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      748 2023-06-03 23:40:41.000000 dsutils_ms-1.1/dsutils_ms/helpers/datetime.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      738 2023-06-03 23:40:42.000000 dsutils_ms-1.1/dsutils_ms/helpers/dict.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      867 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/helpers/env.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      112 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/helpers/google_chat.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      776 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/helpers/log.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.513625 dsutils_ms-1.1/dsutils_ms.egg-info/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      635 2023-06-04 01:26:38.000000 dsutils_ms-1.1/dsutils_ms.egg-info/PKG-INFO
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      788 2023-06-04 01:26:38.000000 dsutils_ms-1.1/dsutils_ms.egg-info/SOURCES.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-06-04 01:26:38.000000 dsutils_ms-1.1/dsutils_ms.egg-info/dependency_links.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      191 2023-06-04 01:26:38.000000 dsutils_ms-1.1/dsutils_ms.egg-info/requires.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       11 2023-06-04 01:26:38.000000 dsutils_ms-1.1/dsutils_ms.egg-info/top_level.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-05-30 18:22:49.000000 dsutils_ms-1.1/dsutils_ms.egg-info/zip-safe
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       80 2023-05-30 17:35:50.000000 dsutils_ms-1.1/pyproject.toml
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1044 2023-06-04 01:26:38.525625 dsutils_ms-1.1/setup.cfg
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       69 2023-05-30 17:35:50.000000 dsutils_ms-1.1/setup.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.521625 dsutils_ms-1.1/tests/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    15766 2023-06-04 01:02:31.000000 dsutils_ms-1.1/tests/test_cleaning.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2980 2023-05-30 17:35:50.000000 dsutils_ms-1.1/tests/test_google_sheets.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3456 2023-05-30 17:35:50.000000 dsutils_ms-1.1/tests/test_mysql.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2342 2023-05-30 17:35:50.000000 dsutils_ms-1.1/tests/test_s3.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.905735 dsutils_ms-1.2/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    34903 2023-05-30 17:35:50.000000 dsutils_ms-1.2/LICENSE.md
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      689 2023-06-24 17:44:16.905735 dsutils_ms-1.2/PKG-INFO
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      125 2023-06-04 01:42:21.000000 dsutils_ms-1.2/README.md
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.901735 dsutils_ms-1.2/dsutils_ms/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/__init__.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.901735 dsutils_ms-1.2/dsutils_ms/adapters/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/adapters/__init__.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2206 2023-06-04 01:19:54.000000 dsutils_ms-1.2/dsutils_ms/adapters/dynamo.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     5336 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/adapters/google_sheets.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1223 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/adapters/interface.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3489 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/adapters/mysql.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3199 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/adapters/s3.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.901735 dsutils_ms-1.2/dsutils_ms/helpers/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/helpers/__init__.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     7202 2023-06-04 00:51:17.000000 dsutils_ms-1.2/dsutils_ms/helpers/cleaning.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      789 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/helpers/dataframe.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      748 2023-06-03 23:40:41.000000 dsutils_ms-1.2/dsutils_ms/helpers/datetime.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      738 2023-06-03 23:40:42.000000 dsutils_ms-1.2/dsutils_ms/helpers/dict.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1026 2023-06-24 17:43:43.000000 dsutils_ms-1.2/dsutils_ms/helpers/env.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      112 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/helpers/google_chat.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      776 2023-05-30 17:35:50.000000 dsutils_ms-1.2/dsutils_ms/helpers/log.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.901735 dsutils_ms-1.2/dsutils_ms.egg-info/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      689 2023-06-24 17:44:16.000000 dsutils_ms-1.2/dsutils_ms.egg-info/PKG-INFO
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      788 2023-06-24 17:44:16.000000 dsutils_ms-1.2/dsutils_ms.egg-info/SOURCES.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-06-24 17:44:16.000000 dsutils_ms-1.2/dsutils_ms.egg-info/dependency_links.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      191 2023-06-24 17:44:16.000000 dsutils_ms-1.2/dsutils_ms.egg-info/requires.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       11 2023-06-24 17:44:16.000000 dsutils_ms-1.2/dsutils_ms.egg-info/top_level.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-05-30 18:22:49.000000 dsutils_ms-1.2/dsutils_ms.egg-info/zip-safe
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       80 2023-05-30 17:35:50.000000 dsutils_ms-1.2/pyproject.toml
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1044 2023-06-24 17:44:16.905735 dsutils_ms-1.2/setup.cfg
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       69 2023-05-30 17:35:50.000000 dsutils_ms-1.2/setup.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 17:44:16.905735 dsutils_ms-1.2/tests/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    15766 2023-06-04 01:02:31.000000 dsutils_ms-1.2/tests/test_cleaning.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2980 2023-05-30 17:35:50.000000 dsutils_ms-1.2/tests/test_google_sheets.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3456 2023-05-30 17:35:50.000000 dsutils_ms-1.2/tests/test_mysql.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2342 2023-05-30 17:35:50.000000 dsutils_ms-1.2/tests/test_s3.py
```

### Comparing `dsutils_ms-1.1/LICENSE.md` & `dsutils_ms-1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/PKG-INFO` & `dsutils_ms-1.2/dsutils_ms.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: dsutils_ms
-Version: 1.1
+Name: dsutils-ms
+Version: 1.2
 Summary: My Data Science Utils
 Home-page: https://www.linkedin.com/in/matheusserpa/
 Author: Matheus Serpa
 Author-email: matheusserpa@gmail.com
 License: GNU General Public License v3.0
 Keywords: data science,data engineering,machine learning,data analysis,data visualization
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 python3.11 setup.py sdist
 
-twine upload dist/*
+twine upload --repository dsutils_ms dist/dsutils_ms-1.1.tar.gz --verbose
 
 
 pip3.11 install -e .
```

### Comparing `dsutils_ms-1.1/dsutils_ms/adapters/dynamo.py` & `dsutils_ms-1.2/dsutils_ms/adapters/dynamo.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/dsutils_ms/adapters/google_sheets.py` & `dsutils_ms-1.2/dsutils_ms/adapters/google_sheets.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/dsutils_ms/adapters/interface.py` & `dsutils_ms-1.2/dsutils_ms/adapters/interface.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/dsutils_ms/adapters/mysql.py` & `dsutils_ms-1.2/dsutils_ms/adapters/mysql.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/dsutils_ms/adapters/s3.py` & `dsutils_ms-1.2/dsutils_ms/adapters/s3.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/dsutils_ms/helpers/cleaning.py` & `dsutils_ms-1.2/dsutils_ms/helpers/cleaning.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/dsutils_ms/helpers/dataframe.py` & `dsutils_ms-1.2/dsutils_ms/helpers/dataframe.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/dsutils_ms/helpers/datetime.py` & `dsutils_ms-1.2/dsutils_ms/helpers/datetime.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/dsutils_ms/helpers/dict.py` & `dsutils_ms-1.2/dsutils_ms/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/dsutils_ms/helpers/env.py` & `dsutils_ms-1.2/dsutils_ms/helpers/env.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 from dotenv.main import load_dotenv
 from os.path import exists
 import json
 from pathlib import Path
 from dsutils_ms.helpers.log import log_title
 
 
-def load_env():
-    PATH = "./"
+def load_env(path_finder: str = "./"):
+    PATH = path_finder
 
+    tries = 0
     while True:
+        tries = tries + 1
         if exists(PATH + ".env"):
             load_dotenv(Path(PATH + ".env"))
             log_title("Loading .env file")
             break
         if exists(PATH + ".gitignore"):
             break
         PATH = "../" + PATH
+        if tries > 10:
+            raise Exception(".env file not found after 10 tries")
 
     if not exists(PATH + ".env"):
         raise Exception(".env file not found")
 
 
 def get_credential(key: str) -> str:
     load_env()
```

### Comparing `dsutils_ms-1.1/dsutils_ms/helpers/log.py` & `dsutils_ms-1.2/dsutils_ms/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/dsutils_ms.egg-info/PKG-INFO` & `dsutils_ms-1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: dsutils-ms
-Version: 1.1
+Name: dsutils_ms
+Version: 1.2
 Summary: My Data Science Utils
 Home-page: https://www.linkedin.com/in/matheusserpa/
 Author: Matheus Serpa
 Author-email: matheusserpa@gmail.com
 License: GNU General Public License v3.0
 Keywords: data science,data engineering,machine learning,data analysis,data visualization
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 python3.11 setup.py sdist
 
-twine upload dist/*
+twine upload --repository dsutils_ms dist/dsutils_ms-1.1.tar.gz --verbose
 
 
 pip3.11 install -e .
```

### Comparing `dsutils_ms-1.1/dsutils_ms.egg-info/SOURCES.txt` & `dsutils_ms-1.2/dsutils_ms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/setup.cfg` & `dsutils_ms-1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsutils_ms
-version = 1.1
+version = 1.2
 author = Matheus Serpa
 author_email = matheusserpa@gmail.com
 url = https://www.linkedin.com/in/matheusserpa/
 description = My Data Science Utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = data science, data engineering, machine learning, data analysis, data visualization
```

### Comparing `dsutils_ms-1.1/tests/test_cleaning.py` & `dsutils_ms-1.2/tests/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/tests/test_google_sheets.py` & `dsutils_ms-1.2/tests/test_google_sheets.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/tests/test_mysql.py` & `dsutils_ms-1.2/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.1/tests/test_s3.py` & `dsutils_ms-1.2/tests/test_s3.py`

 * *Files identical despite different names*

