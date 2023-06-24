# Comparing `tmp/CONGA-3.0.5.tar.gz` & `tmp/CONGA-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CONGA-3.0.5.tar", last modified: Tue Apr 25 01:54:49 2023, max compression
+gzip compressed data, was "CONGA-3.0.6.tar", last modified: Sat Jun 24 00:45:20 2023, max compression
```

## Comparing `CONGA-3.0.5.tar` & `CONGA-3.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:49.100366 CONGA-3.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:49.100366 CONGA-3.0.5/CONGA/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-25 01:54:42.000000 CONGA-3.0.5/CONGA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61600 2023-04-25 01:54:42.000000 CONGA-3.0.5/CONGA/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:49.100366 CONGA-3.0.5/CONGA/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:42.000000 CONGA-3.0.5/CONGA/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-25 01:54:42.000000 CONGA-3.0.5/CONGA/tests/unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:49.100366 CONGA-3.0.5/CONGA/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    70087 2023-04-25 01:54:42.000000 CONGA-3.0.5/CONGA/utils/CONGA_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:42.000000 CONGA-3.0.5/CONGA/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32362 2023-04-25 01:54:42.000000 CONGA-3.0.5/CONGA/utils/peptides.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 01:54:49.100366 CONGA-3.0.5/CONGA/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:49.100366 CONGA-3.0.5/CONGA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-25 01:54:49.000000 CONGA-3.0.5/CONGA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-25 01:54:49.000000 CONGA-3.0.5/CONGA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:54:49.000000 CONGA-3.0.5/CONGA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 01:54:49.000000 CONGA-3.0.5/CONGA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 01:54:49.000000 CONGA-3.0.5/CONGA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 01:54:42.000000 CONGA-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-25 01:54:49.100366 CONGA-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-25 01:54:42.000000 CONGA-3.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 01:54:49.100366 CONGA-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-25 01:54:44.000000 CONGA-3.0.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-25 01:54:44.000000 CONGA-3.0.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:45:20.643425 CONGA-3.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:45:20.643425 CONGA-3.0.6/CONGA/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-24 00:45:15.000000 CONGA-3.0.6/CONGA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61730 2023-06-24 00:45:15.000000 CONGA-3.0.6/CONGA/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:45:20.643425 CONGA-3.0.6/CONGA/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:45:15.000000 CONGA-3.0.6/CONGA/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-06-24 00:45:15.000000 CONGA-3.0.6/CONGA/tests/unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:45:20.643425 CONGA-3.0.6/CONGA/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    70087 2023-06-24 00:45:15.000000 CONGA-3.0.6/CONGA/utils/CONGA_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:45:15.000000 CONGA-3.0.6/CONGA/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32362 2023-06-24 00:45:15.000000 CONGA-3.0.6/CONGA/utils/peptides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-24 00:45:20.643425 CONGA-3.0.6/CONGA/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:45:20.643425 CONGA-3.0.6/CONGA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-24 00:45:20.000000 CONGA-3.0.6/CONGA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-24 00:45:20.000000 CONGA-3.0.6/CONGA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 00:45:20.000000 CONGA-3.0.6/CONGA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-24 00:45:20.000000 CONGA-3.0.6/CONGA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 00:45:20.000000 CONGA-3.0.6/CONGA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-24 00:45:15.000000 CONGA-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-24 00:45:20.643425 CONGA-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-24 00:45:15.000000 CONGA-3.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-24 00:45:20.643425 CONGA-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-24 00:45:17.000000 CONGA-3.0.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-24 00:45:17.000000 CONGA-3.0.6/versioneer.py
```

### Comparing `CONGA-3.0.5/CONGA/__main__.py` & `CONGA-3.0.6/CONGA/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -912,15 +912,17 @@
     df['originally_discovered'] = True
     df['above_group_threshold'] = True
     
     logging.info("Reporting delta masses and variable modifications (if applicable) for each discovered peptide.")
     sys.stderr.write("Reporting delta masses and variable modifications (if applicable) for each discovered peptide. \n")
     
     if df.shape[0] > 0:
-        df_extra = cg.create_cluster(target_decoys_all.copy(), df['winning_peptides'].copy(), dcy_prefix, score, tops_gw, tide_used, isolation_window)
+        original_winning_peptides = df['winning_peptides'].str.replace(
+            "\\[|\\]|\\.|\\d+", "", regex=True).copy()
+        df_extra = cg.create_cluster(target_decoys_all.copy(), original_winning_peptides.copy(), dcy_prefix, score, tops_gw, tide_used, isolation_window)
         df_extra['originally_discovered'] = False
         df_extra = cg.get_thresholds(df.copy(), df_extra.copy(), df_all.copy(), delta_mass_max, precursor_bin_width, tops_gw, score)
         df = pd.concat([df, df_extra]).reset_index(drop = True)
     
     #I don't believe this will be needed in the output for users honestly
     df.pop('all_group_ids') 
     df.pop('bins')
```

### Comparing `CONGA-3.0.5/CONGA/tests/unit_test.py` & `CONGA-3.0.6/CONGA/tests/unit_test.py`

 * *Files identical despite different names*

### Comparing `CONGA-3.0.5/CONGA/utils/CONGA_functions.py` & `CONGA-3.0.6/CONGA/utils/CONGA_functions.py`

 * *Files identical despite different names*

### Comparing `CONGA-3.0.5/CONGA/utils/peptides.py` & `CONGA-3.0.6/CONGA/utils/peptides.py`

 * *Files identical despite different names*

### Comparing `CONGA-3.0.5/CONGA.egg-info/PKG-INFO` & `CONGA-3.0.6/CONGA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CONGA
-Version: 3.0.5
+Version: 3.0.6
 Summary: Combined Open and Narrow searches via Group Analysis
 Home-page: https://github.com/freejstone/CONGA
 Author: Jack Freestone
 Author-email: jfre0619@uni.sydney.edu.au
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CONGA-3.0.5/LICENSE` & `CONGA-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CONGA-3.0.5/PKG-INFO` & `CONGA-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CONGA
-Version: 3.0.5
+Version: 3.0.6
 Summary: Combined Open and Narrow searches via Group Analysis
 Home-page: https://github.com/freejstone/CONGA
 Author: Jack Freestone
 Author-email: jfre0619@uni.sydney.edu.au
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CONGA-3.0.5/README.rst` & `CONGA-3.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `CONGA-3.0.5/setup.py` & `CONGA-3.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `CONGA-3.0.5/versioneer.py` & `CONGA-3.0.6/versioneer.py`

 * *Files identical despite different names*

