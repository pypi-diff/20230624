# Comparing `tmp/pyroe-0.9.2.tar.gz` & `tmp/pyroe-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroe-0.9.2.tar", last modified: Sun May  7 14:22:34 2023, max compression
+gzip compressed data, was "pyroe-0.9.3.tar", last modified: Fri Jun 23 22:06:14 2023, max compression
```

## Comparing `pyroe-0.9.2.tar` & `pyroe-0.9.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.415984 pyroe-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-07 14:22:18.000000 pyroe-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-07 14:22:34.415984 pyroe-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-07 14:22:18.000000 pyroe-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.411984 pyroe-0.9.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10146 2023-05-07 14:22:18.000000 pyroe-0.9.2/bin/pyroe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-07 14:22:18.000000 pyroe-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-07 14:22:34.415984 pyroe-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.411984 pyroe-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.411984 pyroe-0.9.2/src/pyroe/
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/ProcessedQuant.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.411984 pyroe-0.9.2/src/pyroe/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14989 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/data/available_datasets.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/fetch_processed_quant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/id_to_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/load_fry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/load_processed_quant.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24577 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/make_splici_txome.py
--rw-r--r--   0 runner    (1001) docker     (123)    50262 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/make_txome.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/pyroe_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.411984 pyroe-0.9.2/src/pyroe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-07 14:22:34.000000 pyroe-0.9.2/src/pyroe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-07 14:22:34.000000 pyroe-0.9.2/src/pyroe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:22:34.000000 pyroe-0.9.2/src/pyroe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-07 14:22:34.000000 pyroe-0.9.2/src/pyroe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 14:22:34.000000 pyroe-0.9.2/src/pyroe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.415984 pyroe-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-07 14:22:18.000000 pyroe-0.9.2/tests/test_ProcessedQuant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-07 14:22:18.000000 pyroe-0.9.2/tests/test_fetch_processed_quant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-07 14:22:18.000000 pyroe-0.9.2/tests/test_load_processed_quant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-07 14:22:18.000000 pyroe-0.9.2/tests/test_make_spliceu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-07 14:22:18.000000 pyroe-0.9.2/tests/test_make_splici.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:06:14.871923 pyroe-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-23 22:06:03.000000 pyroe-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-23 22:06:14.871923 pyroe-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-23 22:06:03.000000 pyroe-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:06:14.867922 pyroe-0.9.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10146 2023-06-23 22:06:03.000000 pyroe-0.9.3/bin/pyroe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 22:06:03.000000 pyroe-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-23 22:06:14.871923 pyroe-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:06:14.867922 pyroe-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:06:14.871923 pyroe-0.9.3/src/pyroe/
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-06-23 22:06:03.000000 pyroe-0.9.3/src/pyroe/ProcessedQuant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-23 22:06:03.000000 pyroe-0.9.3/src/pyroe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-23 22:06:03.000000 pyroe-0.9.3/src/pyroe/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:06:14.871923 pyroe-0.9.3/src/pyroe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14989 2023-06-23 22:06:03.000000 pyroe-0.9.3/src/pyroe/data/available_datasets.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-06-23 22:06:03.000000 pyroe-0.9.3/src/pyroe/fetch_processed_quant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-23 22:06:03.000000 pyroe-0.9.3/src/pyroe/id_to_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-06-23 22:06:03.000000 pyroe-0.9.3/src/pyroe/load_fry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-06-23 22:06:03.000000 pyroe-0.9.3/src/pyroe/load_processed_quant.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24577 2023-06-23 22:06:03.000000 pyroe-0.9.3/src/pyroe/make_splici_txome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50262 2023-06-23 22:06:03.000000 pyroe-0.9.3/src/pyroe/make_txome.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-23 22:06:03.000000 pyroe-0.9.3/src/pyroe/pyroe_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:06:14.871923 pyroe-0.9.3/src/pyroe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-23 22:06:14.000000 pyroe-0.9.3/src/pyroe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-23 22:06:14.000000 pyroe-0.9.3/src/pyroe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:06:14.000000 pyroe-0.9.3/src/pyroe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 22:06:14.000000 pyroe-0.9.3/src/pyroe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 22:06:14.000000 pyroe-0.9.3/src/pyroe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:06:14.871923 pyroe-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-23 22:06:03.000000 pyroe-0.9.3/tests/test_ProcessedQuant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-23 22:06:03.000000 pyroe-0.9.3/tests/test_fetch_processed_quant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-23 22:06:03.000000 pyroe-0.9.3/tests/test_load_processed_quant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-23 22:06:03.000000 pyroe-0.9.3/tests/test_make_spliceu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-23 22:06:03.000000 pyroe-0.9.3/tests/test_make_splici.py
```

### Comparing `pyroe-0.9.2/LICENSE` & `pyroe-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/PKG-INFO` & `pyroe-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroe
-Version: 0.9.2
+Version: 0.9.3
 Summary: utilities of alevin-fry
 Home-page: https://github.com/COMBINE-lab/pyroe
 Author: Dongze He, Rob Patro
 Author-email: dhe17@umd.edu, rob@cs.umd.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyroe-0.9.2/README.md` & `pyroe-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/bin/pyroe` & `pyroe-0.9.3/bin/pyroe`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/setup.cfg` & `pyroe-0.9.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyroe
-version = 0.9.2
+version = 0.9.3
 author = Dongze He, Rob Patro
 author_email = dhe17@umd.edu, rob@cs.umd.edu
 description = utilities of alevin-fry
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/COMBINE-lab/pyroe
 classifiers =
```

### Comparing `pyroe-0.9.2/src/pyroe/ProcessedQuant.py` & `pyroe-0.9.3/src/pyroe/ProcessedQuant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/src/pyroe/convert.py` & `pyroe-0.9.3/src/pyroe/convert.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/src/pyroe/data/available_datasets.tsv` & `pyroe-0.9.3/src/pyroe/data/available_datasets.tsv`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/src/pyroe/fetch_processed_quant.py` & `pyroe-0.9.3/src/pyroe/fetch_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/src/pyroe/id_to_name.py` & `pyroe-0.9.3/src/pyroe/id_to_name.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,39 +2,43 @@
 import logging
 import pathlib
 import sys
 
 
 def id_to_name(params):
     format_map = {
-        ".gtf": pyranges.read_gtf,
-        ".gff": pyranges.read_gff3,
-        ".gff3": pyranges.read_gff3,
+        "gtf": pyranges.read_gtf,
+        "gff": pyranges.read_gff3,
+        "gff3": pyranges.read_gff3,
     }
     annot_reader = None
     if params.format is None:
         p = pathlib.Path(params.gtf_file)
-        suffs = [z.lower() for z in p.suffixes]
+        suffs = [z.lower().strip('.') for z in p.suffixes]
 
         z = None
-        if len(suffs) == 1:
-            z = suffs[0]
-        elif len(suffs) == 2 and suffs[-1] == ".gz":
-            z = suffs[-2]
+        if len(suffs) >= 1:
+            # look at the final suffix
+            z = suffs[-1]
+            # if the final suffix is gz and there are
+            # suffixes preceding it, check the penultimate
+            # one and use that
+            if z == "gz" and len(suffs) > 1:
+                z = suffs[-2]
 
-        if z in format_map.keys():
-            annot_reader = format_map[z]
-        else:
+        if z is None or z not in format_map.keys():
             logging.error(
                 "Could not determine format of annotation file. Please provide it explicitly."
             )
             sys.exit(1)
+        else:
+            annot_reader = format_map[z]
     else:
         fmt = params.format.lower()
-        if fmt not in ["gtf", "gff3"]:
+        if fmt not in format_map.keys():
             logging.error(
                 f'Format must be either "gtf" or "gff3", but {fmt} was provided.'
             )
             sys.exit(1)
         annot_reader = format_map[fmt]
 
     a = annot_reader(params.gtf_file)
```

### Comparing `pyroe-0.9.2/src/pyroe/load_fry.py` & `pyroe-0.9.3/src/pyroe/load_fry.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/src/pyroe/load_processed_quant.py` & `pyroe-0.9.3/src/pyroe/load_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/src/pyroe/make_splici_txome.py` & `pyroe-0.9.3/src/pyroe/make_splici_txome.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/src/pyroe/make_txome.py` & `pyroe-0.9.3/src/pyroe/make_txome.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/src/pyroe/pyroe_utils.py` & `pyroe-0.9.3/src/pyroe/pyroe_utils.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/src/pyroe.egg-info/PKG-INFO` & `pyroe-0.9.3/src/pyroe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroe
-Version: 0.9.2
+Version: 0.9.3
 Summary: utilities of alevin-fry
 Home-page: https://github.com/COMBINE-lab/pyroe
 Author: Dongze He, Rob Patro
 Author-email: dhe17@umd.edu, rob@cs.umd.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyroe-0.9.2/src/pyroe.egg-info/SOURCES.txt` & `pyroe-0.9.3/src/pyroe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/tests/test_ProcessedQuant.py` & `pyroe-0.9.3/tests/test_ProcessedQuant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/tests/test_fetch_processed_quant.py` & `pyroe-0.9.3/tests/test_fetch_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/tests/test_load_processed_quant.py` & `pyroe-0.9.3/tests/test_load_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/tests/test_make_spliceu.py` & `pyroe-0.9.3/tests/test_make_spliceu.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.2/tests/test_make_splici.py` & `pyroe-0.9.3/tests/test_make_splici.py`

 * *Files identical despite different names*

