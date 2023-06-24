# Comparing `tmp/datawise-0.0.19.tar.gz` & `tmp/datawise-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.19.tar", max compression
+gzip compressed data, was "datawise-0.0.20.tar", max compression
```

## Comparing `datawise-0.0.19.tar` & `datawise-0.0.20.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.19/LICENSE
--rw-r--r--   0        0        0     6760 2023-06-21 02:15:36.811589 datawise-0.0.19/README.md
--rw-r--r--   0        0        0     5600 2023-06-20 11:36:16.459385 datawise-0.0.19/datawise/__init__.py
--rw-r--r--   0        0        0      636 2023-06-20 11:29:08.510434 datawise-0.0.19/datawise/exceptions.py
--rw-r--r--   0        0        0      599 2023-06-21 02:16:17.039692 datawise-0.0.19/pyproject.toml
--rw-r--r--   0        0        0     7328 1970-01-01 00:00:00.000000 datawise-0.0.19/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.20/LICENSE
+-rw-r--r--   0        0        0     6750 2023-06-24 02:47:18.454410 datawise-0.0.20/README.md
+-rw-r--r--   0        0        0     5600 2023-06-20 11:36:16.459385 datawise-0.0.20/datawise/__init__.py
+-rw-r--r--   0        0        0      636 2023-06-20 11:29:08.510434 datawise-0.0.20/datawise/exceptions.py
+-rw-r--r--   0        0        0      589 2023-06-24 02:47:02.780550 datawise-0.0.20/pyproject.toml
+-rw-r--r--   0        0        0     7308 1970-01-01 00:00:00.000000 datawise-0.0.20/PKG-INFO
```

### Comparing `datawise-0.0.19/LICENSE` & `datawise-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.19/README.md` & `datawise-0.0.20/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DataWise
 
-### AI Assistant for data analysis and visualization
+### AI Assistant for Python Data Analytics
 | Capabilities                                      | Limitations                                 |
 |---------------------------------------------------|---------------------------------------------|
 | Use SQL to transform Pandas dataframes            | May occasionally generate incorrect results |
 | Use English to visualize Pandas dataframes (beta) |                                             |
 
 [Get your API Key](https://datawise.vercel.app/)
```

### Comparing `datawise-0.0.19/datawise/__init__.py` & `datawise-0.0.20/datawise/__init__.py`

 * *Files identical despite different names*

### Comparing `datawise-0.0.19/datawise/exceptions.py` & `datawise-0.0.20/datawise/exceptions.py`

 * *Files identical despite different names*

### Comparing `datawise-0.0.19/pyproject.toml` & `datawise-0.0.20/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "datawise"
-version = "0.0.19"
-description = "AI Assistant for data analysis and visualization"
+version = "0.0.20"
+description = "AI Assistant for Python Data Analytics"
 authors = ["DataWise Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
 requests = "2.31.0"
```

### Comparing `datawise-0.0.19/PKG-INFO` & `datawise-0.0.20/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: datawise
-Version: 0.0.19
-Summary: AI Assistant for data analysis and visualization
+Version: 0.0.20
+Summary: AI Assistant for Python Data Analytics
 Author: DataWise Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: urllib3 (>=1.26.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # DataWise
 
-### AI Assistant for data analysis and visualization
+### AI Assistant for Python Data Analytics
 | Capabilities                                      | Limitations                                 |
 |---------------------------------------------------|---------------------------------------------|
 | Use SQL to transform Pandas dataframes            | May occasionally generate incorrect results |
 | Use English to visualize Pandas dataframes (beta) |                                             |
 
 [Get your API Key](https://datawise.vercel.app/)
```

