# Comparing `tmp/dsutils_ms-1.7.tar.gz` & `tmp/dsutils_ms-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsutils_ms-1.7.tar", last modified: Sat Jun 24 19:37:20 2023, max compression
+gzip compressed data, was "dsutils_ms-1.8.tar", last modified: Sat Jun 24 19:43:07 2023, max compression
```

## Comparing `dsutils_ms-1.7.tar` & `dsutils_ms-1.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:37:20.624554 dsutils_ms-1.7/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    34903 2023-05-30 17:35:50.000000 dsutils_ms-1.7/LICENSE.md
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      689 2023-06-24 19:37:20.624554 dsutils_ms-1.7/PKG-INFO
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      125 2023-06-04 01:42:21.000000 dsutils_ms-1.7/README.md
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:37:20.620554 dsutils_ms-1.7/dsutils_ms/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.7/dsutils_ms/__init__.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:37:20.624554 dsutils_ms-1.7/dsutils_ms/adapters/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.7/dsutils_ms/adapters/__init__.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2206 2023-06-04 01:19:54.000000 dsutils_ms-1.7/dsutils_ms/adapters/dynamo.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     5568 2023-06-24 19:37:08.000000 dsutils_ms-1.7/dsutils_ms/adapters/google_sheets.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1223 2023-05-30 17:35:50.000000 dsutils_ms-1.7/dsutils_ms/adapters/interface.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3489 2023-05-30 17:35:50.000000 dsutils_ms-1.7/dsutils_ms/adapters/mysql.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3211 2023-06-24 18:34:03.000000 dsutils_ms-1.7/dsutils_ms/adapters/s3.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:37:20.624554 dsutils_ms-1.7/dsutils_ms/helpers/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.7/dsutils_ms/helpers/__init__.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     7202 2023-06-04 00:51:17.000000 dsutils_ms-1.7/dsutils_ms/helpers/cleaning.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      789 2023-05-30 17:35:50.000000 dsutils_ms-1.7/dsutils_ms/helpers/dataframe.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      798 2023-06-24 18:40:45.000000 dsutils_ms-1.7/dsutils_ms/helpers/datetime.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      738 2023-06-03 23:40:42.000000 dsutils_ms-1.7/dsutils_ms/helpers/dict.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      403 2023-06-24 17:56:31.000000 dsutils_ms-1.7/dsutils_ms/helpers/env.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      112 2023-05-30 17:35:50.000000 dsutils_ms-1.7/dsutils_ms/helpers/google_chat.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      776 2023-05-30 17:35:50.000000 dsutils_ms-1.7/dsutils_ms/helpers/log.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:37:20.620554 dsutils_ms-1.7/dsutils_ms.egg-info/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      689 2023-06-24 19:37:20.000000 dsutils_ms-1.7/dsutils_ms.egg-info/PKG-INFO
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      895 2023-06-24 19:37:20.000000 dsutils_ms-1.7/dsutils_ms.egg-info/SOURCES.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-06-24 19:37:20.000000 dsutils_ms-1.7/dsutils_ms.egg-info/dependency_links.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      191 2023-06-24 19:37:20.000000 dsutils_ms-1.7/dsutils_ms.egg-info/requires.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       11 2023-06-24 19:37:20.000000 dsutils_ms-1.7/dsutils_ms.egg-info/top_level.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-05-30 18:22:49.000000 dsutils_ms-1.7/dsutils_ms.egg-info/zip-safe
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       80 2023-05-30 17:35:50.000000 dsutils_ms-1.7/pyproject.toml
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1044 2023-06-24 19:37:20.628553 dsutils_ms-1.7/setup.cfg
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       69 2023-05-30 17:35:50.000000 dsutils_ms-1.7/setup.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:37:20.624554 dsutils_ms-1.7/tests/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    15766 2023-06-04 01:02:31.000000 dsutils_ms-1.7/tests/test_cleaning.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      543 2023-06-03 23:40:41.000000 dsutils_ms-1.7/tests/test_datetime.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      832 2023-06-03 23:40:54.000000 dsutils_ms-1.7/tests/test_dict.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1816 2023-06-04 01:22:00.000000 dsutils_ms-1.7/tests/test_dynamo.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      274 2023-06-03 23:40:41.000000 dsutils_ms-1.7/tests/test_env.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      389 2023-06-03 23:40:41.000000 dsutils_ms-1.7/tests/test_google_chat.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2980 2023-05-30 17:35:50.000000 dsutils_ms-1.7/tests/test_google_sheets.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3456 2023-05-30 17:35:50.000000 dsutils_ms-1.7/tests/test_mysql.py
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2342 2023-05-30 17:35:50.000000 dsutils_ms-1.7/tests/test_s3.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:43:07.428154 dsutils_ms-1.8/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    34903 2023-05-30 17:35:50.000000 dsutils_ms-1.8/LICENSE.md
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      689 2023-06-24 19:43:07.428154 dsutils_ms-1.8/PKG-INFO
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      125 2023-06-04 01:42:21.000000 dsutils_ms-1.8/README.md
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:43:07.420154 dsutils_ms-1.8/dsutils_ms/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.8/dsutils_ms/__init__.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:43:07.424154 dsutils_ms-1.8/dsutils_ms/adapters/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.8/dsutils_ms/adapters/__init__.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2206 2023-06-04 01:19:54.000000 dsutils_ms-1.8/dsutils_ms/adapters/dynamo.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     5568 2023-06-24 19:40:27.000000 dsutils_ms-1.8/dsutils_ms/adapters/google_sheets.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1223 2023-05-30 17:35:50.000000 dsutils_ms-1.8/dsutils_ms/adapters/interface.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3489 2023-05-30 17:35:50.000000 dsutils_ms-1.8/dsutils_ms/adapters/mysql.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3211 2023-06-24 18:34:03.000000 dsutils_ms-1.8/dsutils_ms/adapters/s3.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:43:07.424154 dsutils_ms-1.8/dsutils_ms/helpers/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.8/dsutils_ms/helpers/__init__.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     7214 2023-06-24 19:43:04.000000 dsutils_ms-1.8/dsutils_ms/helpers/cleaning.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      789 2023-05-30 17:35:50.000000 dsutils_ms-1.8/dsutils_ms/helpers/dataframe.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      798 2023-06-24 18:40:45.000000 dsutils_ms-1.8/dsutils_ms/helpers/datetime.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      738 2023-06-03 23:40:42.000000 dsutils_ms-1.8/dsutils_ms/helpers/dict.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      403 2023-06-24 17:56:31.000000 dsutils_ms-1.8/dsutils_ms/helpers/env.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      112 2023-05-30 17:35:50.000000 dsutils_ms-1.8/dsutils_ms/helpers/google_chat.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      776 2023-05-30 17:35:50.000000 dsutils_ms-1.8/dsutils_ms/helpers/log.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:43:07.424154 dsutils_ms-1.8/dsutils_ms.egg-info/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      689 2023-06-24 19:43:07.000000 dsutils_ms-1.8/dsutils_ms.egg-info/PKG-INFO
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      895 2023-06-24 19:43:07.000000 dsutils_ms-1.8/dsutils_ms.egg-info/SOURCES.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-06-24 19:43:07.000000 dsutils_ms-1.8/dsutils_ms.egg-info/dependency_links.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      191 2023-06-24 19:43:07.000000 dsutils_ms-1.8/dsutils_ms.egg-info/requires.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       11 2023-06-24 19:43:07.000000 dsutils_ms-1.8/dsutils_ms.egg-info/top_level.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-05-30 18:22:49.000000 dsutils_ms-1.8/dsutils_ms.egg-info/zip-safe
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       80 2023-05-30 17:35:50.000000 dsutils_ms-1.8/pyproject.toml
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1044 2023-06-24 19:43:07.428154 dsutils_ms-1.8/setup.cfg
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       69 2023-05-30 17:35:50.000000 dsutils_ms-1.8/setup.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-24 19:43:07.428154 dsutils_ms-1.8/tests/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    15766 2023-06-04 01:02:31.000000 dsutils_ms-1.8/tests/test_cleaning.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      543 2023-06-03 23:40:41.000000 dsutils_ms-1.8/tests/test_datetime.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      832 2023-06-03 23:40:54.000000 dsutils_ms-1.8/tests/test_dict.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1816 2023-06-04 01:22:00.000000 dsutils_ms-1.8/tests/test_dynamo.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      274 2023-06-03 23:40:41.000000 dsutils_ms-1.8/tests/test_env.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      389 2023-06-03 23:40:41.000000 dsutils_ms-1.8/tests/test_google_chat.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2980 2023-05-30 17:35:50.000000 dsutils_ms-1.8/tests/test_google_sheets.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3456 2023-05-30 17:35:50.000000 dsutils_ms-1.8/tests/test_mysql.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2342 2023-05-30 17:35:50.000000 dsutils_ms-1.8/tests/test_s3.py
```

### Comparing `dsutils_ms-1.7/LICENSE.md` & `dsutils_ms-1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/PKG-INFO` & `dsutils_ms-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsutils_ms
-Version: 1.7
+Version: 1.8
 Summary: My Data Science Utils
 Home-page: https://www.linkedin.com/in/matheusserpa/
 Author: Matheus Serpa
 Author-email: matheusserpa@gmail.com
 License: GNU General Public License v3.0
 Keywords: data science,data engineering,machine learning,data analysis,data visualization
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dsutils_ms-1.7/dsutils_ms/adapters/dynamo.py` & `dsutils_ms-1.8/dsutils_ms/adapters/dynamo.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/dsutils_ms/adapters/google_sheets.py` & `dsutils_ms-1.8/dsutils_ms/adapters/google_sheets.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/dsutils_ms/adapters/interface.py` & `dsutils_ms-1.8/dsutils_ms/adapters/interface.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/dsutils_ms/adapters/mysql.py` & `dsutils_ms-1.8/dsutils_ms/adapters/mysql.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/dsutils_ms/adapters/s3.py` & `dsutils_ms-1.8/dsutils_ms/adapters/s3.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/dsutils_ms/helpers/cleaning.py` & `dsutils_ms-1.8/dsutils_ms/helpers/cleaning.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 def remove_stop_words(
     df: DataFrame, how: Literal["columns", "data"] = "data"
 ) -> DataFrame:
     """
     Function to remove stop words from DataFrame columns or data.
     """
 
-    nltk.download("stopwords")
+    nltk.download("stopwords", quiet=True)
 
     english_stop_words = stopwords.words("english")
     portuguese_stop_words = stopwords.words("portuguese")
     all_words = english_stop_words + portuguese_stop_words
 
     if how == "columns":
         cols = []
```

### Comparing `dsutils_ms-1.7/dsutils_ms/helpers/dataframe.py` & `dsutils_ms-1.8/dsutils_ms/helpers/dataframe.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/dsutils_ms/helpers/datetime.py` & `dsutils_ms-1.8/dsutils_ms/helpers/datetime.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/dsutils_ms/helpers/dict.py` & `dsutils_ms-1.8/dsutils_ms/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/dsutils_ms/helpers/log.py` & `dsutils_ms-1.8/dsutils_ms/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/dsutils_ms.egg-info/PKG-INFO` & `dsutils_ms-1.8/dsutils_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsutils-ms
-Version: 1.7
+Version: 1.8
 Summary: My Data Science Utils
 Home-page: https://www.linkedin.com/in/matheusserpa/
 Author: Matheus Serpa
 Author-email: matheusserpa@gmail.com
 License: GNU General Public License v3.0
 Keywords: data science,data engineering,machine learning,data analysis,data visualization
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dsutils_ms-1.7/dsutils_ms.egg-info/SOURCES.txt` & `dsutils_ms-1.8/dsutils_ms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/setup.cfg` & `dsutils_ms-1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsutils_ms
-version = 1.7
+version = 1.8
 author = Matheus Serpa
 author_email = matheusserpa@gmail.com
 url = https://www.linkedin.com/in/matheusserpa/
 description = My Data Science Utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = data science, data engineering, machine learning, data analysis, data visualization
```

### Comparing `dsutils_ms-1.7/tests/test_cleaning.py` & `dsutils_ms-1.8/tests/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/tests/test_datetime.py` & `dsutils_ms-1.8/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/tests/test_dict.py` & `dsutils_ms-1.8/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/tests/test_dynamo.py` & `dsutils_ms-1.8/tests/test_dynamo.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/tests/test_google_sheets.py` & `dsutils_ms-1.8/tests/test_google_sheets.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/tests/test_mysql.py` & `dsutils_ms-1.8/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.7/tests/test_s3.py` & `dsutils_ms-1.8/tests/test_s3.py`

 * *Files identical despite different names*

