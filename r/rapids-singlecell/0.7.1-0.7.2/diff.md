# Comparing `tmp/rapids_singlecell-0.7.1.tar.gz` & `tmp/rapids_singlecell-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapids_singlecell-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rapids_singlecell-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rapids_singlecell-0.7.1.tar` & `rapids_singlecell-0.7.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1070 2023-05-31 21:28:46.364811 rapids_singlecell-0.7.1/LICENSE
--rw-r--r--   0        0        0     5987 2023-05-31 21:28:46.364811 rapids_singlecell-0.7.1/README.md
--rw-r--r--   0        0        0     1062 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/pyproject.toml
--rwxr-xr-x   0        0        0      132 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/__init__.py
--rw-r--r--   0        0        0    25027 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData/__init__.py
--rw-r--r--   0        0        0      334 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/__init__.py
--rw-r--r--   0        0        0    36773 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_hvg.py
--rw-r--r--   0        0        0    14581 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_normalize.py
--rw-r--r--   0        0        0     4544 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_pca.py
--rw-r--r--   0        0        0     2783 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_plotting.py
--rw-r--r--   0        0        0     4795 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_regress_out.py
--rw-r--r--   0        0        0     1441 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_scale.py
--rw-r--r--   0        0        0    18267 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_simple.py
--rw-r--r--   0        0        0     3351 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_utils.py
--rw-r--r--   0        0        0       29 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/dcg.py
--rw-r--r--   0        0        0       68 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/decoupler_gpu/__init__.py
--rw-r--r--   0        0        0     4609 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/decoupler_gpu/_method_mlm.py
--rw-r--r--   0        0        0     6349 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/decoupler_gpu/_method_wsum.py
--rw-r--r--   0        0        0       27 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/gr.py
--rw-r--r--   0        0        0       91 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/pl.py
--rw-r--r--   0        0        0       30 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/pp.py
--rw-r--r--   0        0        0      340 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/__init__.py
--rw-r--r--   0        0        0     5576 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_clustering.py
--rw-r--r--   0        0        0     3429 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_diffmap.py
--rw-r--r--   0        0        0     4040 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_draw_graph.py
--rw-r--r--   0        0        0     5154 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_embedding_density.py
--rw-r--r--   0        0        0    12177 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
--rw-r--r--   0        0        0     1729 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
--rw-r--r--   0        0        0     2425 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_pymde.py
--rw-r--r--   0        0        0     7928 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
--rw-r--r--   0        0        0     3241 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_tsne.py
--rw-r--r--   0        0        0       68 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/__init__.py
--rw-r--r--   0        0        0     6012 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_autocorr.py
--rw-r--r--   0        0        0     6467 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_gearysc.py
--rw-r--r--   0        0        0    29539 2023-05-31 21:28:46.628815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_ligrec.py
--rw-r--r--   0        0        0     6325 2023-05-31 21:28:46.628815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_moransi.py
--rw-r--r--   0        0        0     6227 2023-05-31 21:28:46.628815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_utils.py
--rw-r--r--   0        0        0       26 2023-05-31 21:28:46.632815 rapids_singlecell-0.7.1/rapids_singlecell/tl.py
--rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 rapids_singlecell-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-24 21:46:06.256052 rapids_singlecell-0.7.2/LICENSE
+-rw-r--r--   0        0        0     5987 2023-06-24 21:46:06.256052 rapids_singlecell-0.7.2/README.md
+-rw-r--r--   0        0        0     1062 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/pyproject.toml
+-rwxr-xr-x   0        0        0      132 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/__init__.py
+-rw-r--r--   0        0        0    24992 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/__init__.py
+-rw-r--r--   0        0        0    36773 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_hvg.py
+-rw-r--r--   0        0        0    14581 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_normalize.py
+-rw-r--r--   0        0        0     4544 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_pca.py
+-rw-r--r--   0        0        0     2783 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_plotting.py
+-rw-r--r--   0        0        0     4795 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_regress_out.py
+-rw-r--r--   0        0        0     1459 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_scale.py
+-rw-r--r--   0        0        0    18267 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_simple.py
+-rw-r--r--   0        0        0     3351 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_utils.py
+-rw-r--r--   0        0        0       29 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/dcg.py
+-rw-r--r--   0        0        0       68 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/decoupler_gpu/__init__.py
+-rw-r--r--   0        0        0     4609 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/decoupler_gpu/_method_mlm.py
+-rw-r--r--   0        0        0     6349 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/decoupler_gpu/_method_wsum.py
+-rw-r--r--   0        0        0       27 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/gr.py
+-rw-r--r--   0        0        0       91 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/pl.py
+-rw-r--r--   0        0        0       30 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/pp.py
+-rw-r--r--   0        0        0      340 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5680 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_clustering.py
+-rw-r--r--   0        0        0     3429 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_diffmap.py
+-rw-r--r--   0        0        0     4040 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_draw_graph.py
+-rw-r--r--   0        0        0     5154 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_embedding_density.py
+-rw-r--r--   0        0        0    12177 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
+-rw-r--r--   0        0        0     1729 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
+-rw-r--r--   0        0        0     2425 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_pymde.py
+-rw-r--r--   0        0        0     7928 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
+-rw-r--r--   0        0        0     3241 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_tsne.py
+-rw-r--r--   0        0        0       68 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/__init__.py
+-rw-r--r--   0        0        0     6012 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_autocorr.py
+-rw-r--r--   0        0        0     6467 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_gearysc.py
+-rw-r--r--   0        0        0    29539 2023-06-24 21:46:06.556057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_ligrec.py
+-rw-r--r--   0        0        0     6325 2023-06-24 21:46:06.556057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_moransi.py
+-rw-r--r--   0        0        0     6227 2023-06-24 21:46:06.556057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_utils.py
+-rw-r--r--   0        0        0       26 2023-06-24 21:46:06.560057 rapids_singlecell-0.7.2/rapids_singlecell/tl.py
+-rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 rapids_singlecell-0.7.2/PKG-INFO
```

### Comparing `rapids_singlecell-0.7.1/LICENSE` & `rapids_singlecell-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/README.md` & `rapids_singlecell-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/pyproject.toml` & `rapids_singlecell-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/cunnData/__init__.py` & `rapids_singlecell-0.7.2/rapids_singlecell/cunnData/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -659,15 +659,15 @@
 def _check_X(X):
     return isinstance(
         X, (cp.ndarray, cpx.scipy.sparse.csr_matrix, cpx.scipy.sparse.csc_matrix)
     )
 
 
 def _get_vector(cudata, k, coldim, idxdim, layer=None):
-    # cudata could be self if Raw and AnnData shared a parent
+    # cudata could be self
     dims = ("obs", "var")
     col = getattr(cudata, coldim).columns
     idx = getattr(cudata, f"{idxdim}_names")
 
     in_col = k in col
     in_idx = k in idx
```

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_hvg.py` & `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_hvg.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_normalize.py` & `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_normalize.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_pca.py` & `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_pca.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_plotting.py` & `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_plotting.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_regress_out.py` & `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_regress_out.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_scale.py` & `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_scale.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     mean = X.sum(axis=0).flatten() / X.shape[0]
     X -= mean
     del mean
     stddev = cp.sqrt(X.var(axis=0))
     X /= stddev
     del stddev
     if max_value:
-        X = cp.clip(X, a_max=max_value)
+        X = cp.clip(X, a_min=-max_value, a_max=max_value)
     if inplace:
         if layer:
             cudata.layers[layer] = X
         else:
             cudata.X = X
     else:
         return X
```

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_simple.py` & `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_simple.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_utils.py` & `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_utils.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/decoupler_gpu/_method_mlm.py` & `rapids_singlecell-0.7.2/rapids_singlecell/decoupler_gpu/_method_mlm.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/decoupler_gpu/_method_wsum.py` & `rapids_singlecell-0.7.2/rapids_singlecell/decoupler_gpu/_method_wsum.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_clustering.py` & `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import cupy as cp
 import cudf
-import cugraph
+from cugraph import Graph
+from cugraph import leiden as culeiden
+from cugraph import louvain as culouvain
 import numpy as np
 import pandas as pd
 from cuml.cluster import KMeans
 
 from anndata import AnnData
 
 from typing import Optional
@@ -12,15 +14,15 @@
 
 import warnings
 
 
 def leiden(
     adata: AnnData,
     resolution: float = 1.0,
-    n_iterations: int = -1,
+    n_iterations: int = 100,
     use_weights: bool = True,
     neighbors_key: Optional[int] = None,
     key_added: str = "leiden",
 ) -> None:
     """
     Performs Leiden Clustering using cuGraph
 
@@ -30,17 +32,17 @@
             annData object with 'neighbors' field.
 
         resolution
             A parameter value controlling the coarseness of the clustering.
             Higher values lead to more clusters.
 
         n_iterations
-            How many iterations of the Leiden clustering algorithm to perform.
-            Positive values above 2 define the total number of iterations to perform,
-            -1 has the algorithm run until it reaches its optimal clustering.
+            This controls the maximum number of levels/iterations of the Louvain algorithm.
+            When specified the algorithm will terminate after no more than the specified number of iterations.
+            No error occurs when the algorithm terminates early in this manner.
 
         use_weights
             If `True`, edge weights from the graph are used in the computation
             (placing more emphasis on stronger edges).
 
         neighbors_key
             If not specified, `leiden` looks at `.obsp['connectivities']` for neighbors connectivities
@@ -59,20 +61,20 @@
     offsets = cudf.Series(adjacency.indptr)
     indices = cudf.Series(adjacency.indices)
     if use_weights:
         weights = cudf.Series(adjacency.data)
     else:
         weights = None
 
-    g = cugraph.Graph()
+    g = Graph()
 
     g.from_cudf_adjlist(offsets, indices, weights)
 
     # Cluster
-    leiden_parts, _ = cugraph.leiden(g, resolution=resolution, max_iter=n_iterations)
+    leiden_parts, _ = culeiden(g, resolution=resolution, max_iter=n_iterations)
 
     # Format output
     groups = (
         leiden_parts.to_pandas().sort_values("vertex")[["partition"]].to_numpy().ravel()
     )
 
     adata.obs[key_added] = pd.Categorical(
@@ -134,20 +136,20 @@
     offsets = cudf.Series(adjacency.indptr)
     indices = cudf.Series(adjacency.indices)
     if use_weights:
         weights = cudf.Series(adjacency.data)
     else:
         weights = None
 
-    g = cugraph.Graph()
+    g = Graph()
 
     g.from_cudf_adjlist(offsets, indices, weights)
 
     # Cluster
-    louvain_parts, _ = cugraph.louvain(g, resolution=resolution, max_iter=n_iterations)
+    louvain_parts, _ = culouvain(g, resolution=resolution, max_iter=n_iterations)
 
     # Format output
     groups = (
         louvain_parts.to_pandas()
         .sort_values("vertex")[["partition"]]
         .to_numpy()
         .ravel()
```

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_diffmap.py` & `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_diffmap.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_draw_graph.py` & `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_draw_graph.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_embedding_density.py` & `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_embedding_density.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py` & `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_harmony_integrate.py` & `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_harmony_integrate.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_pymde.py` & `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_pymde.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py` & `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_tsne.py` & `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_tsne.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_autocorr.py` & `rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_autocorr.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_gearysc.py` & `rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_gearysc.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_ligrec.py` & `rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_ligrec.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_moransi.py` & `rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_moransi.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_utils.py` & `rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_utils.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.1/PKG-INFO` & `rapids_singlecell-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapids_singlecell
-Version: 0.7.1
+Version: 0.7.2
 Summary: running single cell analysis on Nvidia GPUs
 Author: Severin Dicks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anndata>=0.7.4
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: decoupler>=1.3.2
```

