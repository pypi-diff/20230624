# Comparing `tmp/Slpapy-0.4.1.tar.gz` & `tmp/Slpapy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.4.1.tar", last modified: Fri Jun 16 08:36:57 2023, max compression
+gzip compressed data, was "Slpapy-0.4.2.tar", last modified: Sat Jun 24 01:55:27 2023, max compression
```

## Comparing `Slpapy-0.4.1.tar` & `Slpapy-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 08:36:57.645781 Slpapy-0.4.1/
--rw-rw-rw-   0        0        0      159 2023-06-16 08:36:57.644785 Slpapy-0.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 08:36:57.600205 Slpapy-0.4.1/Slpapy/
--rw-rw-rw-   0        0        0     3581 2023-06-16 07:08:20.000000 Slpapy-0.4.1/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.4.1/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:36:57.642790 Slpapy-0.4.1/Slpapy/Spatial_map_pic/
--rw-rw-rw-   0        0        0      645 2023-05-24 03:09:50.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/Spatial_map.py
--rw-rw-rw-   0        0        0       52 2023-05-10 02:09:04.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:24.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:24.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:24.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:24.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:24.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/readwrite.py
--rw-rw-rw-   0        0        0    43450 2023-05-24 03:01:38.000000 Slpapy-0.4.1/Slpapy/Spatial_map_pic/scatterplots.py
--rw-rw-rw-   0        0        0      263 2023-05-10 02:17:28.000000 Slpapy-0.4.1/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     6763 2023-06-16 08:36:38.000000 Slpapy-0.4.1/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:36:57.610179 Slpapy-0.4.1/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-06-16 08:36:57.000000 Slpapy-0.4.1/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-06-16 08:36:57.000000 Slpapy-0.4.1/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 08:36:57.000000 Slpapy-0.4.1/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-06-16 08:36:57.000000 Slpapy-0.4.1/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-16 08:36:57.000000 Slpapy-0.4.1/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 08:36:57.645781 Slpapy-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-16 08:36:38.000000 Slpapy-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 01:55:27.004376 Slpapy-0.4.2/
+-rw-rw-rw-   0        0        0      159 2023-06-24 01:55:27.002384 Slpapy-0.4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 01:55:26.955508 Slpapy-0.4.2/Slpapy/
+-rw-rw-rw-   0        0        0     3581 2023-06-16 07:08:20.000000 Slpapy-0.4.2/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.4.2/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-06-24 01:55:26.999391 Slpapy-0.4.2/Slpapy/Spatial_map_pic/
+-rw-rw-rw-   0        0        0      645 2023-05-24 03:09:50.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/Spatial_map.py
+-rw-rw-rw-   0        0        0       52 2023-05-10 02:09:04.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:24.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:24.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:24.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:24.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:24.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/readwrite.py
+-rw-rw-rw-   0        0        0    43450 2023-05-24 03:01:38.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/scatterplots.py
+-rw-rw-rw-   0        0        0      263 2023-05-10 02:17:28.000000 Slpapy-0.4.2/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     6764 2023-06-24 01:54:46.000000 Slpapy-0.4.2/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-06-24 01:55:26.967476 Slpapy-0.4.2/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-06-24 01:55:26.000000 Slpapy-0.4.2/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-06-24 01:55:26.000000 Slpapy-0.4.2/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 01:55:26.000000 Slpapy-0.4.2/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-06-24 01:55:26.000000 Slpapy-0.4.2/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 01:55:26.000000 Slpapy-0.4.2/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 01:55:27.004376 Slpapy-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-06-24 01:54:18.000000 Slpapy-0.4.2/setup.py
```

### Comparing `Slpapy-0.4.1/Slpapy/Data_reconstruction.py` & `Slpapy-0.4.2/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/MZ_ppm_match.py` & `Slpapy-0.4.2/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/Spatial_map.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/Spatial_map.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/_compat.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/_docs.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/_rcmod.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/_settings.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/_utils.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/beats.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/is_constant.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/logging.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/palettes.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/readwrite.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/Spatial_map_pic/scatterplots.py` & `Slpapy-0.4.2/Slpapy/Spatial_map_pic/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.1/Slpapy/processing_analyze.py` & `Slpapy-0.4.2/Slpapy/processing_analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     adata.var['mt'] = adata.var_names.str.startswith('zouyilongLab')  # 将线粒体基因标记为 mt
     sc.pp.calculate_qc_metrics(adata, qc_vars=['mt'], percent_top=None,
                                log1p=False, inplace=True)
     sc.pl.violin(adata, 'total_counts', jitter=0.4, multi_panel=True,
                  save='_total_counts.png')
     adata = adata[adata.obs['total_counts'] != 0, :]
     # 归一化，使得不同细胞样本间可比
-    sc.pp.normalize_total(adata, target_sum=1e4)
+    #sc.pp.normalize_total(adata, target_sum=1e4)
     sc.pp.log1p(adata)
     # 存储数据
     adata.raw = adata
     # 选择高变异基因
     if onlyhighly == True:
         sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
         sc.pl.highly_variable_genes(adata, save='_highly_variable_lipid.png')
@@ -77,15 +77,15 @@
     sc.pl.umap(adata, color=['leiden'], save='_spacial.png')
     sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
     result = adata.uns['rank_genes_groups']
     groups = result['names'].dtype.names
     res = pd.DataFrame({group + '_' + key: result[key][group] for group in groups for key in
                         ['names', 'pvals', 'logfoldchanges', 'pvals_adj', 'scores']})
     res.to_csv("dif.csv")
-    sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_Wilcoxon.png')
+    sc.pl.rank_genes_groups(adata, n_genes=20, sharey=False, save='_Wilcoxon.png')
     sc.pl.rank_genes_groups_dotplot(adata, n_genes=10, save='_dotplot_Wilcoxon.png')
     return adata
 
 
 
 
 def Basic_processing_flow(
@@ -111,15 +111,15 @@
         estimator = KMeans(n_clusters=adata.obs['leiden'].values.codes.max() + 1)  # 构造聚类器
         estimator.fit(
             np.c_[adata.X, preprocessing.normalize(np.c_[np.array(adata.obs['X']), np.array(adata.obs['Y'])])])
         label_pred = estimator.labels_  # 获取聚类标签
         adata.obs['KNNlableXY'] = label_pred.T
         adata.obs['KNNlableXY'] = adata.obs['KNNlableXY'].astype('category')
         sc.tl.rank_genes_groups(adata, 'KNNlableXY', method='wilcoxon')
-        sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_KXY_Wilcoxon.png')
+        sc.pl.rank_genes_groups(adata, n_genes=10, sharey=False, save='_KXY_Wilcoxon.png')
         sc.pl.rank_genes_groups_dotplot(adata, n_genes=10, save='_dotplot_Wilcoxon.png')
         result = adata.uns['rank_genes_groups']
         groups = result['names'].dtype.names
         res = pd.DataFrame({group + '_' + key: result[key][group] for group in groups for key in
                             ['names', 'pvals', 'logfoldchanges', 'pvals_adj', 'scores']})
         res.to_csv("dif.csv")
         sc.pl.pca_variance_ratio(adata, log=True, save='_KXY.png')
```

### Comparing `Slpapy-0.4.1/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.4.2/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

