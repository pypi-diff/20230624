# Comparing `tmp/phuego-0.1.0.dev1.tar.gz` & `tmp/phuego-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phuego-0.1.0.dev1.tar", max compression
+gzip compressed data, was "phuego-0.1.0.dev2.tar", max compression
```

## Comparing `phuego-0.1.0.dev1.tar` & `phuego-0.1.0.dev2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35148 2023-06-24 00:39:29.939522 phuego-0.1.0.dev1/LICENSE
--rw-r--r--   0        0        0     3233 2023-06-24 00:40:11.395414 phuego-0.1.0.dev1/README.md
--rw-r--r--   0        0        0      347 2023-06-24 00:37:50.857573 phuego-0.1.0.dev1/phuego/__init__.py
--rw-r--r--   0        0        0      138 2023-06-24 00:37:50.866412 phuego-0.1.0.dev1/phuego/__main__.py
--rw-r--r--   0        0        0     3978 2023-06-24 00:37:50.843201 phuego-0.1.0.dev1/phuego/data/EGF_vs_Untreated_@min_15_63_240.txt
--rw-r--r--   0        0        0     2937 2023-06-24 00:37:50.846224 phuego-0.1.0.dev1/phuego/dataprep.py
--rw-r--r--   0        0        0     8219 2023-06-24 00:37:50.852012 phuego-0.1.0.dev1/phuego/ego.py
--rw-r--r--   0        0        0     5433 2023-06-24 00:37:50.848975 phuego-0.1.0.dev1/phuego/ego2module.py
--rw-r--r--   0        0        0     4349 2023-06-24 00:37:50.854855 phuego-0.1.0.dev1/phuego/fishertest.py
--rw-r--r--   0        0        0      260 2023-06-24 00:37:50.860554 phuego-0.1.0.dev1/phuego/load_example.py
--rw-r--r--   0        0        0     2588 2023-06-24 00:37:50.863509 phuego-0.1.0.dev1/phuego/load_seeds.py
--rw-r--r--   0        0        0     6183 2023-06-24 00:53:13.654309 phuego-0.1.0.dev1/phuego/main.py
--rw-r--r--   0        0        0     6383 2023-06-24 00:37:50.874949 phuego-0.1.0.dev1/phuego/phuego.py
--rw-r--r--   0        0        0    12678 2023-06-24 00:37:50.872063 phuego-0.1.0.dev1/phuego/phuego_mock.py
--rw-r--r--   0        0        0     1736 2023-06-24 00:37:50.877779 phuego-0.1.0.dev1/phuego/pvalue_splitting.py
--rw-r--r--   0        0        0     4684 2023-06-24 00:37:50.934942 phuego-0.1.0.dev1/phuego/rwr_values.py
--rw-r--r--   0        0        0     1451 2023-06-24 00:37:51.016618 phuego-0.1.0.dev1/phuego/utils.py
--rw-r--r--   0        0        0      966 2023-06-24 00:42:08.289016 phuego-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     4272 1970-01-01 00:00:00.000000 phuego-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-24 00:39:29.939522 phuego-0.1.0.dev2/LICENSE
+-rw-r--r--   0        0        0     3233 2023-06-24 00:40:11.395414 phuego-0.1.0.dev2/README.md
+-rw-r--r--   0        0        0      347 2023-06-24 00:37:50.857573 phuego-0.1.0.dev2/phuego/__init__.py
+-rw-r--r--   0        0        0      138 2023-06-24 00:37:50.866412 phuego-0.1.0.dev2/phuego/__main__.py
+-rw-r--r--   0        0        0     3978 2023-06-24 00:37:50.843201 phuego-0.1.0.dev2/phuego/data/EGF_vs_Untreated_@min_15_63_240.txt
+-rw-r--r--   0        0        0     2937 2023-06-24 00:37:50.846224 phuego-0.1.0.dev2/phuego/dataprep.py
+-rw-r--r--   0        0        0     8219 2023-06-24 00:37:50.852012 phuego-0.1.0.dev2/phuego/ego.py
+-rw-r--r--   0        0        0     5433 2023-06-24 00:37:50.848975 phuego-0.1.0.dev2/phuego/ego2module.py
+-rw-r--r--   0        0        0     4349 2023-06-24 00:37:50.854855 phuego-0.1.0.dev2/phuego/fishertest.py
+-rw-r--r--   0        0        0      260 2023-06-24 00:37:50.860554 phuego-0.1.0.dev2/phuego/load_example.py
+-rw-r--r--   0        0        0     2588 2023-06-24 00:37:50.863509 phuego-0.1.0.dev2/phuego/load_seeds.py
+-rw-r--r--   0        0        0     6136 2023-06-24 17:21:28.830382 phuego-0.1.0.dev2/phuego/main.py
+-rw-r--r--   0        0        0     6383 2023-06-24 00:37:50.874949 phuego-0.1.0.dev2/phuego/phuego.py
+-rw-r--r--   0        0        0    12678 2023-06-24 00:37:50.872063 phuego-0.1.0.dev2/phuego/phuego_mock.py
+-rw-r--r--   0        0        0     1736 2023-06-24 00:37:50.877779 phuego-0.1.0.dev2/phuego/pvalue_splitting.py
+-rw-r--r--   0        0        0     4684 2023-06-24 00:37:50.934942 phuego-0.1.0.dev2/phuego/rwr_values.py
+-rw-r--r--   0        0        0     1451 2023-06-24 00:37:51.016618 phuego-0.1.0.dev2/phuego/utils.py
+-rw-r--r--   0        0        0      962 2023-06-24 17:24:23.216180 phuego-0.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     4264 1970-01-01 00:00:00.000000 phuego-0.1.0.dev2/PKG-INFO
```

### Comparing `phuego-0.1.0.dev1/LICENSE` & `phuego-0.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/README.md` & `phuego-0.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/phuego/data/EGF_vs_Untreated_@min_15_63_240.txt` & `phuego-0.1.0.dev2/phuego/data/EGF_vs_Untreated_@min_15_63_240.txt`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/phuego/dataprep.py` & `phuego-0.1.0.dev2/phuego/dataprep.py`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/phuego/ego.py` & `phuego-0.1.0.dev2/phuego/ego.py`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/phuego/ego2module.py` & `phuego-0.1.0.dev2/phuego/ego2module.py`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/phuego/fishertest.py` & `phuego-0.1.0.dev2/phuego/fishertest.py`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/phuego/load_seeds.py` & `phuego-0.1.0.dev2/phuego/load_seeds.py`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/phuego/main.py` & `phuego-0.1.0.dev2/phuego/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
               ini_pos=ini_pos,
               ini_neg=ini_neg,
               damping=damping,
               kde_cutoff=kde_cutoff,
               use_existing_rwr=use_existing_rwr,
               )
     elif(test_path):
-           print("Run phuego with user input dataset, whose first few lines are: \n", test_df.head())
+           print("Run phuego with user input dataset")
            number_of_nodes, number_of_genes = phuego(
               support_data_folder=support_data_folder,
               res_folder=res_folder,
               test_path=test_path,
               fisher_geneset=fisher_geneset,
               fisher_threshold=fisher_threshold,
               ini_pos=ini_pos,
```

### Comparing `phuego-0.1.0.dev1/phuego/phuego.py` & `phuego-0.1.0.dev2/phuego/phuego.py`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/phuego/phuego_mock.py` & `phuego-0.1.0.dev2/phuego/phuego_mock.py`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/phuego/pvalue_splitting.py` & `phuego-0.1.0.dev2/phuego/pvalue_splitting.py`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/phuego/rwr_values.py` & `phuego-0.1.0.dev2/phuego/rwr_values.py`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/phuego/utils.py` & `phuego-0.1.0.dev2/phuego/utils.py`

 * *Files identical despite different names*

### Comparing `phuego-0.1.0.dev1/pyproject.toml` & `phuego-0.1.0.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "phuego"
-version = "0.1.0.dev1"
+version = "0.1.0.dev2"
 description = "Propagation of phosphoproteomics signals"
 authors = [
     "Girolamo Giudice <Girolamo.Giudice@gmail.com>",
     "Haoqi Chen <haoqichen20@gmail.com>",
     "Evangelia Petsalaki <petsalaki@ebi.ac.uk>"
 ]
 readme = "README.md"
 license = "GPL-3.0-only"
 maintainers = [
     "Haoqi Chen <haoqichen20@gmail.com>",
     "Girolamo Giudice <Girolamo.Giudice@gmail.com>",
 ]
-repository = "https://github.com/haoqichen20/phuego_dev"
+repository = "https://github.com/haoqichen20/phuego"
 keywords = ["Phosphoproteomics", "network propagation"]
 packages = [{include = "phuego"},]
 include = [{path = "phuego/data/*.txt"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 igraph = ">=0.10.2"
```

### Comparing `phuego-0.1.0.dev1/PKG-INFO` & `phuego-0.1.0.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: phuego
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: Propagation of phosphoproteomics signals
-Home-page: https://github.com/haoqichen20/phuego_dev
+Home-page: https://github.com/haoqichen20/phuego
 License: GPL-3.0-only
 Keywords: Phosphoproteomics,network propagation
 Author: Girolamo Giudice
 Author-email: Girolamo.Giudice@gmail.com
 Maintainer: Haoqi Chen
 Maintainer-email: haoqichen20@gmail.com
 Requires-Python: >=3.9,<3.13
@@ -19,15 +19,15 @@
 Requires-Dist: igraph (>=0.10.2)
 Requires-Dist: leidenalg (>=0.9.0)
 Requires-Dist: numpy (>=1.24.3)
 Requires-Dist: pandas (>=2.0.1)
 Requires-Dist: requests (>2.29.0)
 Requires-Dist: scikit-learn (>=1.2.2)
 Requires-Dist: scipy (>=1.10.1)
-Project-URL: Repository, https://github.com/haoqichen20/phuego_dev
+Project-URL: Repository, https://github.com/haoqichen20/phuego
 Description-Content-Type: text/markdown
 
 
 
 ### phuEGO: a network-based method to reconstruct active signalling pathways from phosphoproteomics datasets
 ---
```

