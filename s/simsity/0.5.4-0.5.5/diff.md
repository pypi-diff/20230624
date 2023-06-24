# Comparing `tmp/simsity-0.5.4.tar.gz` & `tmp/simsity-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simsity-0.5.4.tar", last modified: Sat Apr 15 12:14:53 2023, max compression
+gzip compressed data, was "simsity-0.5.5.tar", last modified: Sat Jun 24 19:34:37 2023, max compression
```

## Comparing `simsity-0.5.4.tar` & `simsity-0.5.5.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:14:53.726307 simsity-0.5.4/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3235 2023-04-15 12:14:53.726307 simsity-0.5.4/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1827 2023-04-11 13:48:43.000000 simsity-0.5.4/README.md
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-04-15 12:14:53.726307 simsity-0.5.4/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1399 2023-04-15 12:10:27.000000 simsity-0.5.4/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:14:53.726307 simsity-0.5.4/simsity/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4240 2023-04-15 12:09:09.000000 simsity-0.5.4/simsity/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1015 2023-03-28 14:20:47.000000 simsity-0.5.4/simsity/datasets.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2022-12-20 12:12:03.000000 simsity-0.5.4/simsity/error.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-15 12:14:53.726307 simsity-0.5.4/simsity.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3235 2023-04-15 12:14:53.000000 simsity-0.5.4/simsity.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      229 2023-04-15 12:14:53.000000 simsity-0.5.4/simsity.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-15 12:14:53.000000 simsity-0.5.4/simsity.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      150 2023-04-15 12:14:53.000000 simsity-0.5.4/simsity.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        8 2023-04-15 12:14:53.000000 simsity-0.5.4/simsity.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 19:34:37.170989 simsity-0.5.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1077 2023-06-24 19:33:01.000000 simsity-0.5.5/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2689 2023-06-24 19:34:37.170989 simsity-0.5.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1827 2023-06-24 19:33:01.000000 simsity-0.5.5/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-24 19:34:37.170989 simsity-0.5.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1399 2023-06-24 19:33:44.000000 simsity-0.5.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 19:34:37.170989 simsity-0.5.5/simsity/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4609 2023-06-24 19:33:01.000000 simsity-0.5.5/simsity/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1015 2023-06-24 19:33:01.000000 simsity-0.5.5/simsity/datasets.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      730 2023-06-24 19:33:01.000000 simsity-0.5.5/simsity/error.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 19:34:37.170989 simsity-0.5.5/simsity.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2689 2023-06-24 19:34:37.000000 simsity-0.5.5/simsity.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      274 2023-06-24 19:34:37.000000 simsity-0.5.5/simsity.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-24 19:34:37.000000 simsity-0.5.5/simsity.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      150 2023-06-24 19:34:37.000000 simsity-0.5.5/simsity.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2023-06-24 19:34:37.000000 simsity-0.5.5/simsity.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-24 19:34:37.170989 simsity-0.5.5/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-24 19:33:29.000000 simsity-0.5.5/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1084 2023-06-24 19:33:01.000000 simsity-0.5.5/tests/test_base.py
```

### Comparing `simsity-0.5.4/PKG-INFO` & `simsity-0.5.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,86 @@
 Metadata-Version: 2.1
 Name: simsity
-Version: 0.5.4
+Version: 0.5.5
 Summary: Super Simple Similarity Service
 Home-page: https://github.com/koaning/simsity/
 Author: Vincent D. Warmerdam
-License: UNKNOWN
 Project-URL: Documentation, https://github.com/koaning/simsity/
 Project-URL: Source Code, https://github.com/koaning/simsity/
 Project-URL: Issue Tracker, https://github.com/koaning/simsity/issues
-Description: 
-        ![landing](https://user-images.githubusercontent.com/1019791/222645884-fd88cd66-3dd0-4b6e-98f4-65586040e538.png)
-        
-        # simsity
-        
-        > Simsity is a Super Simple Similarities Service[tm]. <br>
-        > It's all about building a neighborhood. Literally! <br>
-        
-        <br>
-        
-        This repository contains simple tools to help in similarity retrieval scenarios
-        by making a convenient wrapper around [hnswlib](https://github.com/nmslib/hnswlib/blob/master/examples/python/EXAMPLES.md).
-        Typical usecases include early stage bulk labelling and duplication discovery.
-        
-        ## Install
-        
-        You can install simsity via pip.
-        
-        ```
-        python -m pip install simsity
-        ```
-        
-        The goal of simsity is to be minimal, to make rapid prototyping very easy and to be "just enough" for medium sized datasets. You will mainly interact with these two functions. 
-        
-        ```python
-        from simsity import create_index, load_index
-        ```
-        
-        As their names imply, you can use these to create an index or to load one from disk. 
-        
-        ## Quickstart
-        
-        ```python
-        from simsity import create_index, load_index
-        
-        # Let's fetch some demo data
-        from simsity.datasets import fetch_recipes
-        df_recipes = fetch_recipes()
-        recipes = df_recipes["text"]
-        
-        # Let's use embetter for embeddings 
-        from embetter.text import SentenceEncoder
-        encoder = SentenceEncoder()
-        
-        # Populate the ANN vector index and use it. 
-        index = create_index(recipes, encoder)
-        texts, dists = index.query("pork")
-        
-        # You can also query using vectors
-        v_pork = encoder.transform(["pork"])[0]
-        texts, dists = index.query_vector(v_pork)
-        ```
-        
-        You can also provide a path and then you'll be able to store/load everything.
-        
-        ```python
-        # Make an index with a path
-        index = create_index(recipes, encoder, path="demo")
-        
-        # Load an index from a path
-        reloaded_index = load_index(path="demo", encoder=encoder)
-        texts, dists = reloaded_index.query("pork")
-        ```
-        
-        That's it! Happy hacking!
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+
+![landing](https://user-images.githubusercontent.com/1019791/222645884-fd88cd66-3dd0-4b6e-98f4-65586040e538.png)
+
+# simsity
+
+> Simsity is a Super Simple Similarities Service[tm]. <br>
+> It's all about building a neighborhood. Literally! <br>
+
+<br>
+
+This repository contains simple tools to help in similarity retrieval scenarios
+by making a convenient wrapper around [hnswlib](https://github.com/nmslib/hnswlib/blob/master/examples/python/EXAMPLES.md).
+Typical usecases include early stage bulk labelling and duplication discovery.
+
+## Install
+
+You can install simsity via pip.
+
+```
+python -m pip install simsity
+```
+
+The goal of simsity is to be minimal, to make rapid prototyping very easy and to be "just enough" for medium sized datasets. You will mainly interact with these two functions. 
+
+```python
+from simsity import create_index, load_index
+```
+
+As their names imply, you can use these to create an index or to load one from disk. 
+
+## Quickstart
+
+```python
+from simsity import create_index, load_index
+
+# Let's fetch some demo data
+from simsity.datasets import fetch_recipes
+df_recipes = fetch_recipes()
+recipes = df_recipes["text"]
+
+# Let's use embetter for embeddings 
+from embetter.text import SentenceEncoder
+encoder = SentenceEncoder()
+
+# Populate the ANN vector index and use it. 
+index = create_index(recipes, encoder)
+texts, dists = index.query("pork")
+
+# You can also query using vectors
+v_pork = encoder.transform(["pork"])[0]
+texts, dists = index.query_vector(v_pork)
+```
+
+You can also provide a path and then you'll be able to store/load everything.
+
+```python
+# Make an index with a path
+index = create_index(recipes, encoder, path="demo")
+
+# Load an index from a path
+reloaded_index = load_index(path="demo", encoder=encoder)
+texts, dists = reloaded_index.query("pork")
+```
+
+That's it! Happy hacking!
```

### Comparing `simsity-0.5.4/README.md` & `simsity-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `simsity-0.5.4/setup.py` & `simsity-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 all_packages = base_packages
 dev_packages = all_packages + test_packages
 
 
 setup(
     name="simsity",
-    version="0.5.4",
+    version="0.5.5",
     author="Vincent D. Warmerdam",
     packages=find_packages(exclude=["notebooks", "docs"]),
     description="Super Simple Similarity Service",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/koaning/simsity/",
     project_urls={
```

### Comparing `simsity-0.5.4/simsity/__init__.py` & `simsity-0.5.5/simsity/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from queue import LifoQueue
 import datetime as dt
 import itertools as it
 from pathlib import Path
-from typing import Iterable, Protocol, Callable, Union
+from typing import Iterable, Protocol, Callable, Union, Any, Dict, Optional
 
 import srsly
 from hnswlib import Index
 from tqdm import tqdm
 
 DB_NAME = "db.gz.json"
 INDEX_NAME = "index.bin"
@@ -14,38 +14,41 @@
 
 
 class Transformer(Protocol):
     def transform(self):
         pass
 
 
+EncType = Union[Callable, Transformer]
+
+
 class SimSityIndex:
     """Object for easy querying."""
 
-    def __init__(self, index, encoder, db) -> None:
+    def __init__(self, index: Index, encoder: EncType, db: Dict[int, Any]) -> None:
         self.index = index
         self.encoder = encoder
         self.db = db
 
-    def query(self, query, n=10):
+    def query(self, query: Union[str, Dict], n: int = 10):
         """
         Query using approximate nearest neighbors
 
         The object handles the encoder/data from disk.
         """
         arr = encode_data(self.encoder, query)
         return self.query_vector(query=arr, n=n)
 
-    def query_vector(self, query, n=10):
+    def query_vector(self, query: Union[str, Dict], n: int = 10):
         """Query using a vector."""
         labels, distances = self.index.knn_query(query, k=n)
-        out = [self.db[int(label)] for label in labels[0]]
+        out = [self.db[label] for label in labels[0]]
         return out, list(distances[0])
 
-    def walk(index, *args, n=10, depth=3, uniq_id=lambda d: d):
+    def walk(self, *args, n=10, depth=3, uniq_id=lambda d: d):
         """Walk through the index, finding nearest neighbors of nearest neighbors.
 
         Arguments:
 
         - args: the queries to start the walk off with
         - n : number of items to return per query
         - depth: how deep should the search go
@@ -54,15 +57,15 @@
         q = LifoQueue()
         seen = {}
 
         for i in range(depth):
             new_args = []
 
             for arg in args:
-                res, dists = index.query(arg, n=n)
+                res, dists = self.index.query(arg, n=n)
                 for item in res:
                     q.put(item)
 
             if depth != 0:
                 while not q.empty():
                     item = q.get()
                     if uniq_id(item) not in seen:
@@ -82,38 +85,43 @@
     if callable(encoder):
         return encoder(data)
     else:
         return encoder.transform(data)
 
 
 def create_index(
-    data: Iterable,
+    data: list,
     encoder: Union[Transformer, Callable],
-    path: Path = None,
-    space="cosine",
-    pbar=True,
-    batch_size=500,
+    path: Optional[Union[Path, str]] = None,
+    space: str = "cosine",
+    pbar: bool = True,
+    batch_size: int = 500,
 ):
     """
     Creates a simple ANN index. Uses hnswlib under the hood.
     You need to provide a scikit-learn compatible encoder for the data manually.
     """
     index = None
+    dim = 0
     batches = batch(data, batch_size)
     if pbar:
         batches, batches_copy = it.tee(batches)
         total = sum(1 for _ in batches_copy)
         batches = tqdm(batches, desc="indexing", total=total)
     for b in batches:
         encoded = encode_data(encoder, b)
         if not index:
             dim = encoded.shape[1]
             index = Index(space=space, dim=dim)
             index.init_index(max_elements=len(data))
         index.add_items(encoded)
+    if not index:
+        raise RuntimeError(
+            "Something has gone terrible wrong. There is no index. Did you supply data?"
+        )
     if path:
         path = Path(path)
         path.mkdir(parents=True, exist_ok=True)
         if (path / DB_NAME).exists():
             (path / DB_NAME).unlink()
         srsly.write_gzip_json(path / DB_NAME, {i: item for i, item in enumerate(data)})
         index.save_index(str(path / INDEX_NAME))
@@ -128,15 +136,15 @@
             path / METADATA_NAME,
             metadata,
         )
     db = {i: k for i, k in enumerate(data)}
     return SimSityIndex(index=index, encoder=encoder, db=db)
 
 
-def load_index(path, encoder):
+def load_index(path: Union[str, Path], encoder: EncType):
     """Load in a simsity index from a path. Must supply same encoder."""
     path = Path(path)
     metadata = srsly.read_json(path / METADATA_NAME)
     index = Index(space=metadata["space"], dim=metadata["dim"])
     index.load_index(str(path / INDEX_NAME))
-    db = {i: k for i, k in enumerate(srsly.read_gzip_json(path / DB_NAME))}
+    db = {int(i): k for i, k in srsly.read_gzip_json(path / DB_NAME).items()}
     return SimSityIndex(index=index, encoder=encoder, db=db)
```

### Comparing `simsity-0.5.4/simsity/datasets.py` & `simsity-0.5.5/simsity/datasets.py`

 * *Files identical despite different names*

### Comparing `simsity-0.5.4/simsity/error.py` & `simsity-0.5.5/simsity/error.py`

 * *Files identical despite different names*

### Comparing `simsity-0.5.4/simsity.egg-info/PKG-INFO` & `simsity-0.5.5/simsity.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,86 @@
 Metadata-Version: 2.1
 Name: simsity
-Version: 0.5.4
+Version: 0.5.5
 Summary: Super Simple Similarity Service
 Home-page: https://github.com/koaning/simsity/
 Author: Vincent D. Warmerdam
-License: UNKNOWN
 Project-URL: Documentation, https://github.com/koaning/simsity/
 Project-URL: Source Code, https://github.com/koaning/simsity/
 Project-URL: Issue Tracker, https://github.com/koaning/simsity/issues
-Description: 
-        ![landing](https://user-images.githubusercontent.com/1019791/222645884-fd88cd66-3dd0-4b6e-98f4-65586040e538.png)
-        
-        # simsity
-        
-        > Simsity is a Super Simple Similarities Service[tm]. <br>
-        > It's all about building a neighborhood. Literally! <br>
-        
-        <br>
-        
-        This repository contains simple tools to help in similarity retrieval scenarios
-        by making a convenient wrapper around [hnswlib](https://github.com/nmslib/hnswlib/blob/master/examples/python/EXAMPLES.md).
-        Typical usecases include early stage bulk labelling and duplication discovery.
-        
-        ## Install
-        
-        You can install simsity via pip.
-        
-        ```
-        python -m pip install simsity
-        ```
-        
-        The goal of simsity is to be minimal, to make rapid prototyping very easy and to be "just enough" for medium sized datasets. You will mainly interact with these two functions. 
-        
-        ```python
-        from simsity import create_index, load_index
-        ```
-        
-        As their names imply, you can use these to create an index or to load one from disk. 
-        
-        ## Quickstart
-        
-        ```python
-        from simsity import create_index, load_index
-        
-        # Let's fetch some demo data
-        from simsity.datasets import fetch_recipes
-        df_recipes = fetch_recipes()
-        recipes = df_recipes["text"]
-        
-        # Let's use embetter for embeddings 
-        from embetter.text import SentenceEncoder
-        encoder = SentenceEncoder()
-        
-        # Populate the ANN vector index and use it. 
-        index = create_index(recipes, encoder)
-        texts, dists = index.query("pork")
-        
-        # You can also query using vectors
-        v_pork = encoder.transform(["pork"])[0]
-        texts, dists = index.query_vector(v_pork)
-        ```
-        
-        You can also provide a path and then you'll be able to store/load everything.
-        
-        ```python
-        # Make an index with a path
-        index = create_index(recipes, encoder, path="demo")
-        
-        # Load an index from a path
-        reloaded_index = load_index(path="demo", encoder=encoder)
-        texts, dists = reloaded_index.query("pork")
-        ```
-        
-        That's it! Happy hacking!
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+
+![landing](https://user-images.githubusercontent.com/1019791/222645884-fd88cd66-3dd0-4b6e-98f4-65586040e538.png)
+
+# simsity
+
+> Simsity is a Super Simple Similarities Service[tm]. <br>
+> It's all about building a neighborhood. Literally! <br>
+
+<br>
+
+This repository contains simple tools to help in similarity retrieval scenarios
+by making a convenient wrapper around [hnswlib](https://github.com/nmslib/hnswlib/blob/master/examples/python/EXAMPLES.md).
+Typical usecases include early stage bulk labelling and duplication discovery.
+
+## Install
+
+You can install simsity via pip.
+
+```
+python -m pip install simsity
+```
+
+The goal of simsity is to be minimal, to make rapid prototyping very easy and to be "just enough" for medium sized datasets. You will mainly interact with these two functions. 
+
+```python
+from simsity import create_index, load_index
+```
+
+As their names imply, you can use these to create an index or to load one from disk. 
+
+## Quickstart
+
+```python
+from simsity import create_index, load_index
+
+# Let's fetch some demo data
+from simsity.datasets import fetch_recipes
+df_recipes = fetch_recipes()
+recipes = df_recipes["text"]
+
+# Let's use embetter for embeddings 
+from embetter.text import SentenceEncoder
+encoder = SentenceEncoder()
+
+# Populate the ANN vector index and use it. 
+index = create_index(recipes, encoder)
+texts, dists = index.query("pork")
+
+# You can also query using vectors
+v_pork = encoder.transform(["pork"])[0]
+texts, dists = index.query_vector(v_pork)
+```
+
+You can also provide a path and then you'll be able to store/load everything.
+
+```python
+# Make an index with a path
+index = create_index(recipes, encoder, path="demo")
+
+# Load an index from a path
+reloaded_index = load_index(path="demo", encoder=encoder)
+texts, dists = reloaded_index.query("pork")
+```
+
+That's it! Happy hacking!
```

