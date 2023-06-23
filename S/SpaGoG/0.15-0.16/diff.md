# Comparing `tmp/SpaGoG-0.15.tar.gz` & `tmp/SpaGoG-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpaGoG-0.15.tar", last modified: Fri Jun 23 22:12:40 2023, max compression
+gzip compressed data, was "dist/SpaGoG-0.16.tar", last modified: Fri Jun 23 22:48:39 2023, max compression
```

## Comparing `SpaGoG-0.15.tar` & `SpaGoG-0.16.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:12:40.000000 SpaGoG-0.15/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1342 2023-06-23 22:11:22.000000 SpaGoG-0.15/setup.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       39 2023-05-12 23:49:44.000000 SpaGoG-0.15/setup.cfg
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:43:34.000000 SpaGoG-0.15/README
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      486 2023-06-23 22:12:40.000000 SpaGoG-0.15/PKG-INFO
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:12:40.000000 SpaGoG-0.15/spagog/
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:12:40.000000 SpaGoG-0.15/spagog/default_params/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      236 2023-05-12 23:49:43.000000 SpaGoG-0.15/spagog/default_params/gc.json
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      594 2023-05-12 23:49:43.000000 SpaGoG-0.15/spagog/default_params/gnc.json
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      595 2023-05-12 23:49:43.000000 SpaGoG-0.15/spagog/default_params/gc+nc.json
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     8354 2023-06-22 20:21:02.000000 SpaGoG-0.15/spagog/main.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:40.000000 SpaGoG-0.15/spagog/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    11750 2023-06-22 20:14:46.000000 SpaGoG-0.15/spagog/experiments.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:48:39.000000 SpaGoG-0.16/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1342 2023-06-23 22:48:35.000000 SpaGoG-0.16/setup.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       39 2023-05-12 23:49:44.000000 SpaGoG-0.16/setup.cfg
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:43:34.000000 SpaGoG-0.16/README
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      486 2023-06-23 22:48:39.000000 SpaGoG-0.16/PKG-INFO
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:48:39.000000 SpaGoG-0.16/spagog/
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:48:39.000000 SpaGoG-0.16/spagog/default_params/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      236 2023-05-12 23:49:43.000000 SpaGoG-0.16/spagog/default_params/gc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      594 2023-05-12 23:49:43.000000 SpaGoG-0.16/spagog/default_params/gnc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      595 2023-05-12 23:49:43.000000 SpaGoG-0.16/spagog/default_params/gc+nc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     5201 2023-06-23 22:45:43.000000 SpaGoG-0.16/spagog/main.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.16/spagog/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    11778 2023-06-23 22:45:43.000000 SpaGoG-0.16/spagog/experiments.py
```

### Comparing `SpaGoG-0.15/setup.py` & `SpaGoG-0.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
     name='SpaGoG',  # How you named your package folder (MyLib)
     packages=['spagog'],  # Chose the same as "name"
-    version='0.15',  # Start with a small number and increase it with every change you make
+    version='0.16',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Sparse data classification using Graph of Graphs',  # Give a short description about your library
     author='Shachar Hananya',  # Type in your name
     author_email='shacharhananya@gmail.com',  # Type in your E-Mail
     url='https://github.com/HananyaS/SpaGoG',  # Provide either the link to your github or to your website
-    download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.15.tar.gz',  # I explain this later on
+    download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.16.tar.gz',  # I explain this later on
     keywords=['GoG', 'Missing values', 'Graphs'],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
         'pandas==2.0.1',
         'torch==2.0.1',
         'torch-geometric==2.3.1',
         'matplotlib==3.7.1',
     ],
```

### Comparing `SpaGoG-0.15/spagog/default_params/gnc.json` & `SpaGoG-0.16/spagog/default_params/gnc.json`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.15/spagog/default_params/gc+nc.json` & `SpaGoG-0.16/spagog/default_params/gc+nc.json`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.15/spagog/experiments.py` & `SpaGoG-0.16/spagog/experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 import torch
 
-from datasets.tabDataset import TabDataset
-from datasets.graphsDataset import GraphsDataset
+from .datasets.tabDataset import TabDataset
+from .datasets.graphsDataset import GraphsDataset
 
-from models.graphClassification import ValuesAndGraphStructure as GC
-from models.graphNodeClassification import GraphNodeClassification as GNC
-from models.nodeClassification import NodeClassification
+from .models.graphClassification import ValuesAndGraphStructure as GC
+from .models.graphNodeClassification import GraphNodeClassification as GNC
+from .models.nodeClassification import NodeClassification
 
 PROJECT_DIR = "."
 
 
 def run_gc(
         tab_dataset: TabDataset,
         params: dict,
@@ -165,36 +165,34 @@
 
     cache, all_graphs_loader = model.fit(
         graphs_dataset,
         inter_samples_edges,
         train_mask,
         val_mask,
         test_mask,
-        n_epochs=600,
+        n_epochs=10000,
         gc_lr=params["gc_lr"],
         nc_lr=params["nc_lr"],
         gc_weight_decay=params["gc_weight_decay"],
         nc_weight_decay=params["nc_weight_decay"],
         alpha=params["alpha"],
         batch_size=params.get("batch_size", 10),
         early_stopping_patience=early_stopping,
         verbose=verbose,
         clf_from=params["clf_from"]  # clf_from
     )
 
-    y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"],
-                           probs=False,
+    y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"], probs=False,
                            to_numpy=to_numpy)
 
     if evaluate_metrics and verbose == 1:
         print(f"Test accuracy: {(test_loader.dataset.gdp.Y.flatten() == y_test).float().mean():.4f}")
 
     if probs:
-        y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"],
-                               probs=True,
+        y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"], probs=True,
                                to_numpy=to_numpy)
 
     return y_test, cache
 
 
 def run_gc_nc(
         tab_dataset: TabDataset,
@@ -344,14 +342,17 @@
 
     if probs:
         y_test = nc_model.predict(test_graph, probs=True, to_numpy=to_numpy)
 
     return y_test, cache
 
 
+def get_default_params_file(model):
+    return f"default_params/{model}.json"
+
 
 def get_tab_data(
         train_X: pd.DataFrame,
         train_Y: pd.DataFrame,
         test_X: pd.DataFrame,
         test_Y: pd.DataFrame = None,
         val_X: pd.DataFrame = None,
```

