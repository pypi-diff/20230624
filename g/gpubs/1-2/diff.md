# Comparing `tmp/gpubs-1.tar.gz` & `tmp/gpubs-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpubs-1.tar", last modified: Fri Jun 23 04:55:07 2023, max compression
+gzip compressed data, was "gpubs-2.tar", last modified: Fri Jun 23 09:33:36 2023, max compression
```

## Comparing `gpubs-1.tar` & `gpubs-2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 04:55:07.048166 gpubs-1/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       28 2023-06-23 03:40:04.000000 gpubs-1/MANIFEST.in
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-23 04:55:07.048166 gpubs-1/PKG-INFO
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 04:55:07.048166 gpubs-1/gpubs/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      129 2023-06-23 03:11:20.000000 gpubs-1/gpubs/__init__.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       18 2023-06-23 04:55:07.000000 gpubs-1/gpubs/_version.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)    14323 2023-06-21 14:30:12.000000 gpubs-1/gpubs/api.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1829 2023-06-21 14:00:14.000000 gpubs-1/gpubs/fetch.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      210 2023-06-21 02:49:51.000000 gpubs-1/gpubs/log.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     5743 2023-06-21 13:08:21.000000 gpubs-1/gpubs/models.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     3279 2023-06-21 14:09:08.000000 gpubs-1/gpubs/parse.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1292 2023-06-21 13:33:20.000000 gpubs-1/gpubs/reference.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1939 2023-06-21 02:50:26.000000 gpubs-1/gpubs/search_words.py
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 04:55:07.048166 gpubs-1/gpubs.egg-info/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-23 04:55:07.000000 gpubs-1/gpubs.egg-info/PKG-INFO
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      411 2023-06-23 04:55:07.000000 gpubs-1/gpubs.egg-info/SOURCES.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)        1 2023-06-23 04:55:07.000000 gpubs-1/gpubs.egg-info/dependency_links.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       76 2023-06-23 04:55:07.000000 gpubs-1/gpubs.egg-info/requires.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)        6 2023-06-23 04:55:07.000000 gpubs-1/gpubs.egg-info/top_level.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      359 2023-06-23 04:54:17.000000 gpubs-1/release-info.json
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 04:55:07.048166 gpubs-1/scripts/
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     4101 2023-06-21 02:46:43.000000 gpubs-1/scripts/create_search_terms_file.sh
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     5195 2023-06-21 02:46:43.000000 gpubs-1/scripts/download_pubs.sh
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     1892 2023-06-21 02:46:43.000000 gpubs-1/scripts/search.awk
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       38 2023-06-23 04:55:07.048166 gpubs-1/setup.cfg
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1164 2023-06-23 04:40:13.000000 gpubs-1/setup.py
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 09:33:36.675703 gpubs-2/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       28 2023-06-23 03:40:04.000000 gpubs-2/MANIFEST.in
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-23 09:33:36.675703 gpubs-2/PKG-INFO
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 09:33:36.675703 gpubs-2/gpubs/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      129 2023-06-23 03:11:20.000000 gpubs-2/gpubs/__init__.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       18 2023-06-23 09:33:36.000000 gpubs-2/gpubs/_version.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)    14654 2023-06-23 09:16:16.000000 gpubs-2/gpubs/api.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1829 2023-06-21 14:00:14.000000 gpubs-2/gpubs/fetch.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      210 2023-06-21 02:49:51.000000 gpubs-2/gpubs/log.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     5743 2023-06-21 13:08:21.000000 gpubs-2/gpubs/models.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     3279 2023-06-21 14:09:08.000000 gpubs-2/gpubs/parse.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1292 2023-06-21 13:33:20.000000 gpubs-2/gpubs/reference.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1939 2023-06-21 02:50:26.000000 gpubs-2/gpubs/search_words.py
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 09:33:36.675703 gpubs-2/gpubs.egg-info/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-23 09:33:36.000000 gpubs-2/gpubs.egg-info/PKG-INFO
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      411 2023-06-23 09:33:36.000000 gpubs-2/gpubs.egg-info/SOURCES.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)        1 2023-06-23 09:33:36.000000 gpubs-2/gpubs.egg-info/dependency_links.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       76 2023-06-23 09:33:36.000000 gpubs-2/gpubs.egg-info/requires.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)        6 2023-06-23 09:33:36.000000 gpubs-2/gpubs.egg-info/top_level.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      359 2023-06-23 05:04:20.000000 gpubs-2/release-info.json
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 09:33:36.675703 gpubs-2/scripts/
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     4101 2023-06-21 02:46:43.000000 gpubs-2/scripts/create_search_terms_file.sh
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     5195 2023-06-21 02:46:43.000000 gpubs-2/scripts/download_pubs.sh
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     1892 2023-06-21 02:46:43.000000 gpubs-2/scripts/search.awk
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       38 2023-06-23 09:33:36.675703 gpubs-2/setup.cfg
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1164 2023-06-23 04:40:13.000000 gpubs-2/setup.py
```

### Comparing `gpubs-1/gpubs/api.py` & `gpubs-2/gpubs/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,21 +269,26 @@
     filtered_terms_file = os.path.join(m.search_path(), m.filtered_terms_filename)
     csv_inpath = m.pub_outpath()
     csv_outpath = m.genes_outpath()
     verbose = m.verbose
     
     import glob
     import subprocess
-    awk_script = "scripts/search.awk" # xxx move this to ReferenceData
+    awk_script = "search.awk"
+    # Check if awk_script is under ./scripts - e.g., this is being run from the notebook from inside the repo
+    # otherwise awk_script should be in path - e.g. gpubs has been pip install'd
+    if os.path.isfile(os.path.join("scripts", awk_script)):
+        awk_script = os.path.join("scripts", awk_script)
     for file_name_path in glob.glob(os.path.join(csv_inpath,"pubmed*.xml.gz.csv")):
         file_name = os.path.basename(file_name_path)
         input_csv_file = os.path.join(csv_inpath, file_name)
         output_csv_file = os.path.join(csv_outpath, file_name)
         msg2(verbose, f"Creating {output_csv_file}")
         error_file = os.path.join(csv_outpath, f"{file_name}.err")
+        # xxx test this out, then run make to install version 2
         command = [awk_script, filtered_terms_file, input_csv_file]
         with open(output_csv_file, "w") as output, open(error_file, "w") as error:
             subprocess.run(command, stdout=output, stderr=error)
 
 def pipeline(m: ReferenceData):
     """ 
     Run the whole data pipeline, end to end. See QuickStart notebook for step-by-step outputs
```

### Comparing `gpubs-1/gpubs/fetch.py` & `gpubs-2/gpubs/fetch.py`

 * *Files identical despite different names*

### Comparing `gpubs-1/gpubs/models.py` & `gpubs-2/gpubs/models.py`

 * *Files identical despite different names*

### Comparing `gpubs-1/gpubs/parse.py` & `gpubs-2/gpubs/parse.py`

 * *Files identical despite different names*

### Comparing `gpubs-1/gpubs/reference.py` & `gpubs-2/gpubs/reference.py`

 * *Files identical despite different names*

### Comparing `gpubs-1/gpubs/search_words.py` & `gpubs-2/gpubs/search_words.py`

 * *Files identical despite different names*

### Comparing `gpubs-1/scripts/create_search_terms_file.sh` & `gpubs-2/scripts/create_search_terms_file.sh`

 * *Files identical despite different names*

### Comparing `gpubs-1/scripts/download_pubs.sh` & `gpubs-2/scripts/download_pubs.sh`

 * *Files identical despite different names*

### Comparing `gpubs-1/scripts/search.awk` & `gpubs-2/scripts/search.awk`

 * *Files identical despite different names*

### Comparing `gpubs-1/setup.py` & `gpubs-2/setup.py`

 * *Files identical despite different names*

