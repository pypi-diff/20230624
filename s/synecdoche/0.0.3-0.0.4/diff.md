# Comparing `tmp/synecdoche-0.0.3.tar.gz` & `tmp/synecdoche-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synecdoche-0.0.3.tar", last modified: Fri Jun 23 20:15:28 2023, max compression
+gzip compressed data, was "synecdoche-0.0.4.tar", last modified: Sat Jun 24 16:29:26 2023, max compression
```

## Comparing `synecdoche-0.0.3.tar` & `synecdoche-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:15:28.887444 synecdoche-0.0.3/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-23 14:39:41.000000 synecdoche-0.0.3/LICENSE
--rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-23 20:15:28.887444 synecdoche-0.0.3/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      590 2023-06-23 20:10:30.000000 synecdoche-0.0.3/README.md
--rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-23 20:15:28.887444 synecdoche-0.0.3/setup.cfg
--rw-rw-r--   0 legion    (1000) legion    (1000)     1447 2023-06-23 20:11:13.000000 synecdoche-0.0.3/setup.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:15:28.887444 synecdoche-0.0.3/synecdoche/
--rw-rw-r--   0 legion    (1000) legion    (1000)      129 2023-06-23 17:33:17.000000 synecdoche-0.0.3/synecdoche/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:39.000000 synecdoche-0.0.3/synecdoche/_version.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1740 2023-06-23 20:07:56.000000 synecdoche-0.0.3/synecdoche/experimental.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     8460 2023-06-23 20:10:09.000000 synecdoche-0.0.3/synecdoche/hyper.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:15:28.887444 synecdoche-0.0.3/synecdoche.egg-info/
--rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-23 20:15:28.000000 synecdoche-0.0.3/synecdoche.egg-info/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      311 2023-06-23 20:15:28.000000 synecdoche-0.0.3/synecdoche.egg-info/SOURCES.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-23 20:15:28.000000 synecdoche-0.0.3/synecdoche.egg-info/dependency_links.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       34 2023-06-23 20:15:28.000000 synecdoche-0.0.3/synecdoche.egg-info/requires.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       11 2023-06-23 20:15:28.000000 synecdoche-0.0.3/synecdoche.egg-info/top_level.txt
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:15:28.887444 synecdoche-0.0.3/tests/
--rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-23 17:42:50.000000 synecdoche-0.0.3/tests/test_networks.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:29:26.308767 synecdoche-0.0.4/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-23 14:39:41.000000 synecdoche-0.0.4/LICENSE
+-rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-24 16:29:26.308767 synecdoche-0.0.4/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      639 2023-06-23 21:57:45.000000 synecdoche-0.0.4/README.md
+-rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-24 16:29:26.308767 synecdoche-0.0.4/setup.cfg
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1447 2023-06-24 16:28:55.000000 synecdoche-0.0.4/setup.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:29:26.308767 synecdoche-0.0.4/synecdoche/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      129 2023-06-23 17:33:17.000000 synecdoche-0.0.4/synecdoche/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:39.000000 synecdoche-0.0.4/synecdoche/_version.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1882 2023-06-24 15:43:56.000000 synecdoche-0.0.4/synecdoche/experimental.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     8464 2023-06-24 15:43:08.000000 synecdoche-0.0.4/synecdoche/hyper.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:29:26.308767 synecdoche-0.0.4/synecdoche.egg-info/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-24 16:29:26.000000 synecdoche-0.0.4/synecdoche.egg-info/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      311 2023-06-24 16:29:26.000000 synecdoche-0.0.4/synecdoche.egg-info/SOURCES.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-24 16:29:26.000000 synecdoche-0.0.4/synecdoche.egg-info/dependency_links.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       34 2023-06-24 16:29:26.000000 synecdoche-0.0.4/synecdoche.egg-info/requires.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       11 2023-06-24 16:29:26.000000 synecdoche-0.0.4/synecdoche.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:29:26.308767 synecdoche-0.0.4/tests/
+-rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-23 17:42:50.000000 synecdoche-0.0.4/tests/test_networks.py
```

### Comparing `synecdoche-0.0.3/LICENSE` & `synecdoche-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `synecdoche-0.0.3/PKG-INFO` & `synecdoche-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synecdoche
-Version: 0.0.3
+Version: 0.0.4
 Summary: Synecdoche: Hypernetworks for Haiku in JAX
 Home-page: https://github.com/kmheckel/synecdoche
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `synecdoche-0.0.3/README.md` & `synecdoche-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 
 🏗️ 🚧 This library is under construction!🚧
 ===========================================
 
+![brain printer](synecdoche.png "Synecdoche")
+
+
 Synecdoche: HyperNetworks in Haiku
 ===================================
 
 Hi!
 
 Synecdoche is a mini-library for JAX providing clean implementations of hypernetworks.
 
 The name Synecdoche refers to the literary device in which a part of something is substituted for the whole; fittingly, the methods implemented in this library are based around substituting the weights for a much larger network with a smaller one that is easier to manipulate!
 
 
-Creating a hypernetwork has never been so easy!
+Creating a hypernetwork has never been so easy!
```

### Comparing `synecdoche-0.0.3/setup.py` & `synecdoche-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "dm-haiku",
     ],
 )
 
 # This call to setup() does all the work
 setup(
     name="synecdoche",
-    version="0.0.3",
+    version="0.0.4",
     description="Synecdoche: Hypernetworks for Haiku in JAX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kmheckel/synecdoche",
     author="Kade Heckel",
     author_email="example@email.com",
     license="MIT",
```

### Comparing `synecdoche-0.0.3/synecdoche/experimental.py` & `synecdoche-0.0.4/synecdoche/experimental.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import jax.tree_util as tree
 import jax.numpy as jnp
 import haiku as hk
 
 class DynamicHypernetwork(hk.Module):
     """
     Hypernetwork that takes the current batch as inputs, averages the samples, and then uses that average to predict weights for the layer.
+
+    This will be modified soon such that it contains a dynamic hypernet for a single input
+    that is then vmapped over the batch axis.
     """
 
     def __init__(self, embedding_dim, latent_dim, network_params):
         super().__init__()
         # PyTree data needed to reconstruct net
         self.tgt_treedef = tree.tree_structure(network_params)
         self.tgt_sizes = tree.tree_map(jnp.size, network_params)
@@ -25,14 +28,14 @@
         layer_inputs = jnp.repeat(jnp.expand_dims(avg, 0), self.num_tgt_layers, 0)
         projections = hk.nets.MLP([self.embedding_dim, self.latent_dim, self.latent_dim])(layer_inputs)
 
         layer_projections = jnp.split(projections, self.num_tgt_layers)
                 
         rebuilt_tree = tree.tree_unflatten(self.tgt_treedef, layer_projections)
         resized_tree = tree.tree_map(lambda layer, size: jnp.pad(layer[1,:size], 
-                                                                 (0,max(0,size-layer.size)), 
+                                                                 (0,jnp.max(0,size-layer.size)), 
                                                                  mode="wrap"), 
                                      rebuilt_tree, 
                                      self.tgt_sizes
                                     )
         net = tree.tree_map(jnp.reshape, resized_tree, self.target_layer_shapes)
         return net
```

### Comparing `synecdoche-0.0.3/synecdoche/hyper.py` & `synecdoche-0.0.4/synecdoche/hyper.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,14 @@
         # tgt_layers X max_layer_size matrix
         
         layer_projections = jnp.split(projections, self.num_tgt_layers)
                 
         rebuilt_tree = tree.tree_unflatten(self.tgt_treedef, layer_projections)
         # this is ugly... sorry...
         resized_tree = tree.tree_map(lambda layer, size: jnp.pad(layer[1,:size], 
-                                                                 (0,max(0,size-layer.size)), 
+                                                                 (0,jnp.max(0,size-layer.size)), 
                                                                  mode="wrap"), 
                                      rebuilt_tree, 
                                      self.tgt_sizes
                                     )
         net = tree.tree_map(jnp.reshape, resized_tree, self.target_layer_shapes)
         return net
```

### Comparing `synecdoche-0.0.3/synecdoche.egg-info/PKG-INFO` & `synecdoche-0.0.4/synecdoche.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synecdoche
-Version: 0.0.3
+Version: 0.0.4
 Summary: Synecdoche: Hypernetworks for Haiku in JAX
 Home-page: https://github.com/kmheckel/synecdoche
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

