# Comparing `tmp/caltechdata_api-1.4.1.tar.gz` & `tmp/caltechdata_api-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caltechdata_api-1.4.1.tar", last modified: Fri Jun  9 19:41:43 2023, max compression
+gzip compressed data, was "caltechdata_api-1.4.2.tar", last modified: Fri Jun 23 23:16:05 2023, max compression
```

## Comparing `caltechdata_api-1.4.1.tar` & `caltechdata_api-1.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-06-09 19:41:43.286577 caltechdata_api-1.4.1/
--rw-r--r--   0 tmorrell   (502) staff       (20)     1523 2017-11-22 17:15:19.000000 caltechdata_api-1.4.1/LICENSE
--rw-r--r--   0 tmorrell   (502) staff       (20)     2514 2023-06-09 19:41:43.285760 caltechdata_api-1.4.1/PKG-INFO
--rw-r--r--   0 tmorrell   (502) staff       (20)     1825 2022-12-06 00:24:56.000000 caltechdata_api-1.4.1/README.md
-drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-06-09 19:41:43.254795 caltechdata_api-1.4.1/caltechdata_api/
--rw-r--r--   0 tmorrell   (502) staff       (20)      400 2022-12-01 21:58:52.000000 caltechdata_api-1.4.1/caltechdata_api/__init__.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     8107 2023-05-23 22:56:57.000000 caltechdata_api-1.4.1/caltechdata_api/caltechdata_edit.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     9315 2023-06-09 18:28:13.000000 caltechdata_api-1.4.1/caltechdata_api/caltechdata_write.py
--rw-r--r--   0 tmorrell   (502) staff       (20)    15913 2023-05-02 22:03:31.000000 caltechdata_api-1.4.1/caltechdata_api/customize_schema.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     1983 2022-10-28 23:31:55.000000 caltechdata_api-1.4.1/caltechdata_api/download_file.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     1304 2023-05-08 16:21:06.000000 caltechdata_api-1.4.1/caltechdata_api/get_files.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     2489 2022-10-28 18:19:39.000000 caltechdata_api-1.4.1/caltechdata_api/get_metadata.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     2742 2022-12-06 16:41:11.000000 caltechdata_api-1.4.1/caltechdata_api/utils.py
-drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-06-09 19:41:43.276479 caltechdata_api-1.4.1/caltechdata_api/vocabularies/
--rw-r--r--   0 tmorrell   (502) staff       (20)      794 2021-09-15 17:27:24.000000 caltechdata_api-1.4.1/caltechdata_api/vocabularies/date_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)      614 2023-05-11 18:15:35.000000 caltechdata_api-1.4.1/caltechdata_api/vocabularies/description_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)     1396 2022-12-06 16:41:11.000000 caltechdata_api-1.4.1/caltechdata_api/vocabularies/identifier_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)    51301 2021-09-15 17:27:24.000000 caltechdata_api-1.4.1/caltechdata_api/vocabularies/licenses.csv
--rw-r--r--   0 tmorrell   (502) staff       (20)     2682 2021-09-15 17:27:24.000000 caltechdata_api-1.4.1/caltechdata_api/vocabularies/relation_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)    16372 2022-11-18 19:12:39.000000 caltechdata_api-1.4.1/caltechdata_api/vocabularies/resource_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)     1815 2021-09-15 17:27:24.000000 caltechdata_api-1.4.1/caltechdata_api/vocabularies/roles.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)      332 2021-09-15 17:27:24.000000 caltechdata_api-1.4.1/caltechdata_api/vocabularies/title_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)      601 2021-09-21 20:43:40.000000 caltechdata_api-1.4.1/caltechdata_api/vocabularies.yaml
-drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-06-09 19:41:43.262872 caltechdata_api-1.4.1/caltechdata_api.egg-info/
--rw-r--r--   0 tmorrell   (502) staff       (20)     2514 2023-06-09 19:41:42.000000 caltechdata_api-1.4.1/caltechdata_api.egg-info/PKG-INFO
--rw-r--r--   0 tmorrell   (502) staff       (20)      950 2023-06-09 19:41:42.000000 caltechdata_api-1.4.1/caltechdata_api.egg-info/SOURCES.txt
--rw-r--r--   0 tmorrell   (502) staff       (20)        1 2023-06-09 19:41:42.000000 caltechdata_api-1.4.1/caltechdata_api.egg-info/dependency_links.txt
--rw-r--r--   0 tmorrell   (502) staff       (20)       49 2023-06-09 19:41:42.000000 caltechdata_api-1.4.1/caltechdata_api.egg-info/requires.txt
--rw-r--r--   0 tmorrell   (502) staff       (20)       16 2023-06-09 19:41:42.000000 caltechdata_api-1.4.1/caltechdata_api.egg-info/top_level.txt
--rw-r--r--   0 tmorrell   (502) staff       (20)       38 2023-06-09 19:41:43.286782 caltechdata_api-1.4.1/setup.cfg
--rwxr-xr-x   0 tmorrell   (502) staff       (20)     4595 2023-04-06 20:14:24.000000 caltechdata_api-1.4.1/setup.py
-drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-06-09 19:41:43.284604 caltechdata_api-1.4.1/tests/
--rw-r--r--   0 tmorrell   (502) staff       (20)     2046 2021-05-26 23:04:00.000000 caltechdata_api-1.4.1/tests/test_conversion.py
--rw-r--r--   0 tmorrell   (502) staff       (20)      818 2021-09-28 21:03:28.000000 caltechdata_api-1.4.1/tests/test_download.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     1668 2021-10-07 20:58:02.000000 caltechdata_api-1.4.1/tests/test_rdm.py
+drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-06-23 23:16:05.589753 caltechdata_api-1.4.2/
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1523 2017-11-22 17:15:19.000000 caltechdata_api-1.4.2/LICENSE
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2514 2023-06-23 23:16:05.588536 caltechdata_api-1.4.2/PKG-INFO
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1825 2022-12-06 00:24:56.000000 caltechdata_api-1.4.2/README.md
+drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-06-23 23:16:05.416557 caltechdata_api-1.4.2/caltechdata_api/
+-rw-r--r--   0 tmorrell   (502) staff       (20)      400 2022-12-01 21:58:52.000000 caltechdata_api-1.4.2/caltechdata_api/__init__.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     8107 2023-05-23 22:56:57.000000 caltechdata_api-1.4.2/caltechdata_api/caltechdata_edit.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     9327 2023-06-23 23:14:46.000000 caltechdata_api-1.4.2/caltechdata_api/caltechdata_write.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)    15913 2023-05-02 22:03:31.000000 caltechdata_api-1.4.2/caltechdata_api/customize_schema.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1983 2022-10-28 23:31:55.000000 caltechdata_api-1.4.2/caltechdata_api/download_file.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1304 2023-05-08 16:21:06.000000 caltechdata_api-1.4.2/caltechdata_api/get_files.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2489 2022-10-28 18:19:39.000000 caltechdata_api-1.4.2/caltechdata_api/get_metadata.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2742 2022-12-06 16:41:11.000000 caltechdata_api-1.4.2/caltechdata_api/utils.py
+drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-06-23 23:16:05.537558 caltechdata_api-1.4.2/caltechdata_api/vocabularies/
+-rw-r--r--   0 tmorrell   (502) staff       (20)      794 2021-09-15 17:27:24.000000 caltechdata_api-1.4.2/caltechdata_api/vocabularies/date_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)      614 2023-05-11 18:15:35.000000 caltechdata_api-1.4.2/caltechdata_api/vocabularies/description_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1396 2022-12-06 16:41:11.000000 caltechdata_api-1.4.2/caltechdata_api/vocabularies/identifier_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)    51301 2021-09-15 17:27:24.000000 caltechdata_api-1.4.2/caltechdata_api/vocabularies/licenses.csv
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2682 2021-09-15 17:27:24.000000 caltechdata_api-1.4.2/caltechdata_api/vocabularies/relation_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)    16372 2022-11-18 19:12:39.000000 caltechdata_api-1.4.2/caltechdata_api/vocabularies/resource_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1815 2021-09-15 17:27:24.000000 caltechdata_api-1.4.2/caltechdata_api/vocabularies/roles.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)      332 2021-09-15 17:27:24.000000 caltechdata_api-1.4.2/caltechdata_api/vocabularies/title_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)      601 2021-09-21 20:43:40.000000 caltechdata_api-1.4.2/caltechdata_api/vocabularies.yaml
+drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-06-23 23:16:05.443848 caltechdata_api-1.4.2/caltechdata_api.egg-info/
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2514 2023-06-23 23:16:04.000000 caltechdata_api-1.4.2/caltechdata_api.egg-info/PKG-INFO
+-rw-r--r--   0 tmorrell   (502) staff       (20)      950 2023-06-23 23:16:04.000000 caltechdata_api-1.4.2/caltechdata_api.egg-info/SOURCES.txt
+-rw-r--r--   0 tmorrell   (502) staff       (20)        1 2023-06-23 23:16:04.000000 caltechdata_api-1.4.2/caltechdata_api.egg-info/dependency_links.txt
+-rw-r--r--   0 tmorrell   (502) staff       (20)       49 2023-06-23 23:16:04.000000 caltechdata_api-1.4.2/caltechdata_api.egg-info/requires.txt
+-rw-r--r--   0 tmorrell   (502) staff       (20)       16 2023-06-23 23:16:04.000000 caltechdata_api-1.4.2/caltechdata_api.egg-info/top_level.txt
+-rw-r--r--   0 tmorrell   (502) staff       (20)       38 2023-06-23 23:16:05.590061 caltechdata_api-1.4.2/setup.cfg
+-rwxr-xr-x   0 tmorrell   (502) staff       (20)     4595 2023-04-06 20:14:24.000000 caltechdata_api-1.4.2/setup.py
+drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-06-23 23:16:05.586444 caltechdata_api-1.4.2/tests/
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2046 2021-05-26 23:04:00.000000 caltechdata_api-1.4.2/tests/test_conversion.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)      818 2021-09-28 21:03:28.000000 caltechdata_api-1.4.2/tests/test_download.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1668 2021-10-07 20:58:02.000000 caltechdata_api-1.4.2/tests/test_rdm.py
```

### Comparing `caltechdata_api-1.4.1/LICENSE` & `caltechdata_api-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/PKG-INFO` & `caltechdata_api-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caltechdata_api
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python wrapper for CaltechDATA API.
 Home-page: https://github.com/caltechlibrary/caltechdata_api
 Author: Thomas E Morrell
 Author-email: tmorrell@caltech.edu
 License: https://data.caltech.edu/license
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `caltechdata_api-1.4.1/README.md` & `caltechdata_api-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/caltechdata_edit.py` & `caltechdata_api-1.4.2/caltechdata_api/caltechdata_edit.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/caltechdata_write.py` & `caltechdata_api-1.4.2/caltechdata_api/caltechdata_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,23 +109,23 @@
     data = {
         "receiver": {"community": community},
         "type": "community-submission",
     }
     result = requests.put(review_link, json=data, headers=headers)
     if result.status_code != 200:
         raise Exception(result.text)
-    submit_link = result.json()["links"]["actions"]["submit"]
+    submit_link = review_link.replace('/review','/actions/submit-review')
     data = comment = {
         "payload": {
             "content": message,
             "format": "html",
         }
     }
     result = requests.post(submit_link, json=data, headers=headers)
-    if result.status_code != 200:
+    if result.status_code != 202:
         raise Exception(result.text)
     if publish:
         accept_link = result.json()["links"]["actions"]["accept"]
         data = comment = {
             "payload": {
                 "content": "This record is accepted automatically with the CaltechDATA API",
                 "format": "html",
```

### Comparing `caltechdata_api-1.4.1/caltechdata_api/customize_schema.py` & `caltechdata_api-1.4.2/caltechdata_api/customize_schema.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/download_file.py` & `caltechdata_api-1.4.2/caltechdata_api/download_file.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/get_files.py` & `caltechdata_api-1.4.2/caltechdata_api/get_files.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/get_metadata.py` & `caltechdata_api-1.4.2/caltechdata_api/get_metadata.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/utils.py` & `caltechdata_api-1.4.2/caltechdata_api/utils.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/vocabularies/date_types.yaml` & `caltechdata_api-1.4.2/caltechdata_api/vocabularies/date_types.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/vocabularies/description_types.yaml` & `caltechdata_api-1.4.2/caltechdata_api/vocabularies/description_types.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/vocabularies/identifier_types.yaml` & `caltechdata_api-1.4.2/caltechdata_api/vocabularies/identifier_types.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/vocabularies/licenses.csv` & `caltechdata_api-1.4.2/caltechdata_api/vocabularies/licenses.csv`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/vocabularies/relation_types.yaml` & `caltechdata_api-1.4.2/caltechdata_api/vocabularies/relation_types.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/vocabularies/resource_types.yaml` & `caltechdata_api-1.4.2/caltechdata_api/vocabularies/resource_types.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/vocabularies/roles.yaml` & `caltechdata_api-1.4.2/caltechdata_api/vocabularies/roles.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api/vocabularies.yaml` & `caltechdata_api-1.4.2/caltechdata_api/vocabularies.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/caltechdata_api.egg-info/PKG-INFO` & `caltechdata_api-1.4.2/caltechdata_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caltechdata-api
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python wrapper for CaltechDATA API.
 Home-page: https://github.com/caltechlibrary/caltechdata_api
 Author: Thomas E Morrell
 Author-email: tmorrell@caltech.edu
 License: https://data.caltech.edu/license
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `caltechdata_api-1.4.1/caltechdata_api.egg-info/SOURCES.txt` & `caltechdata_api-1.4.2/caltechdata_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/setup.py` & `caltechdata_api-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/tests/test_conversion.py` & `caltechdata_api-1.4.2/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/tests/test_download.py` & `caltechdata_api-1.4.2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.4.1/tests/test_rdm.py` & `caltechdata_api-1.4.2/tests/test_rdm.py`

 * *Files identical despite different names*

