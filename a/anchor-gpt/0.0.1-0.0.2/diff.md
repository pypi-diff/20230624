# Comparing `tmp/anchor-gpt-0.0.1.tar.gz` & `tmp/anchor-gpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anchor-gpt-0.0.1.tar", last modified: Fri Jun 23 02:32:18 2023, max compression
+gzip compressed data, was "anchor-gpt-0.0.2.tar", last modified: Sat Jun 24 02:12:52 2023, max compression
```

## Comparing `anchor-gpt-0.0.1.tar` & `anchor-gpt-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 02:32:18.734617 anchor-gpt-0.0.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3166 2023-06-23 02:32:18.734617 anchor-gpt-0.0.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1962 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 02:32:18.734617 anchor-gpt-0.0.1/anchor_gpt/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/anchor_gpt/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/anchor_gpt/coreset.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/anchor_gpt/prompt.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/anchor_gpt/prompt_logger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2456 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/anchor_gpt/prompt_store.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-23 02:32:18.734617 anchor-gpt-0.0.1/anchor_gpt.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3166 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/anchor_gpt.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      316 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/anchor_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/anchor_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/anchor_gpt.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       11 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/anchor_gpt.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-23 02:32:18.738617 anchor-gpt-0.0.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1758 2023-06-23 02:32:18.000000 anchor-gpt-0.0.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-24 02:12:52.555305 anchor-gpt-0.0.2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6300 2023-06-24 02:12:52.555305 anchor-gpt-0.0.2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4504 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-24 02:12:52.555305 anchor-gpt-0.0.2/anchor_gpt/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/anchor_gpt/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4700 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/anchor_gpt/coreset.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1096 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/anchor_gpt/prompt.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2124 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/anchor_gpt/prompt_logger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3233 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/anchor_gpt/prompt_store.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4067 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/anchor_gpt/test_logger.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-24 02:12:52.555305 anchor-gpt-0.0.2/anchor_gpt.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6300 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/anchor_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      342 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/anchor_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/anchor_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/anchor_gpt.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       11 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/anchor_gpt.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-24 02:12:52.555305 anchor-gpt-0.0.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1758 2023-06-24 02:12:52.000000 anchor-gpt-0.0.2/setup.py
```

### Comparing `anchor-gpt-0.0.1/LICENSE` & `anchor-gpt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anchor-gpt-0.0.1/anchor_gpt/coreset.py` & `anchor-gpt-0.0.2/anchor_gpt/coreset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,26 @@
+###
+# Implementation of the Coreset Algirithm
 # Heavily inspired by https://github.com/google/active-learning
+###
+
+
 import os
 from datetime import datetime
 import numpy as np
 from tqdm import tqdm
+import random
 
 import tempfile
 
+random.seed(1234)
+np.random.seed(1234)
+
 try:
+    # Using cuML to GPU enable coreset, otherwise use sklearn
     from cuml.metrics.pairwise_distances import pairwise_distances
 except Exception as e:
     from sklearn.metrics import pairwise_distances
 
 BATCH_SIZE = int(os.environ.get('CORESET_BATCH_SIZE', '100'))
 
 class kCenterGreedy():
@@ -60,16 +70,14 @@
 
   def select_batch_(self, already_selected, N):
 
     self.update_distances(already_selected, only_new=False, reset_dist=True)
 
     new_batch = []
 
-    np.random.seed(1234)
-
     n_obs = len(self.X)
 
     for _ in tqdm(range(N), desc='calculating coreset...'):
       if self.min_distances is None:
         # Initialize centers with a randomly selected datapoint
         ind = np.random.choice(np.arange(n_obs))
       else:
@@ -83,15 +91,14 @@
 
     self.already_selected = already_selected
 
     return new_batch
 
 def coreset(vector_ids, already_selected, number_of_datapoints, transformer, distance='euclidean'):
 
-  tic = datetime.now()
   with tempfile.TemporaryDirectory() as tmpdirname:
     batch_shapes = {}
     for batch_start in range(0, len(vector_ids), BATCH_SIZE):
       features_batch = transformer(vector_ids[batch_start:batch_start + BATCH_SIZE])
       try:
         first_none_vector_idx = features_batch.index(None)
         raise ValueError(f'Cannot use None embeddings for id {vector_ids[first_none_vector_idx + batch_start]} to calculate coreset')
@@ -104,15 +111,15 @@
         fp = np.memmap(os.path.join(tmpdirname, str(uuid)), dtype='float16', mode='w+', shape=features_batch[index].shape)
         fp[:] = features_batch[index][:]
         fp.flush()
       try:
         np_features_batch = np.stack(features_batch, axis=0)
       except ValueError as e:
         raise ValueError(f'Cannot use provided embeddings to calculate coreset: {e}') from e
- 
+
       bfp = np.memmap(
         os.path.join(tmpdirname, str(batch_start)), dtype='float16', mode='w+', shape=np_features_batch.shape)
       bfp[:] = np_features_batch[:]
       bfp.flush()
       batch_shapes[batch_start] = np_features_batch.shape
 
     X = np.array(vector_ids)
```

### Comparing `anchor-gpt-0.0.1/anchor_gpt/prompt_store.py` & `anchor-gpt-0.0.2/anchor_gpt/prompt_store.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,106 @@
 import sqlite3
 import uuid
-import json
+import ast
 
 sqlite3.register_adapter(uuid.UUID, lambda u: u.bytes_le)
 
 from .prompt import Prompt
 
 class PromptStore:
+    """
+    An extensible class for prompt stores.
+    """
     def add(self, prompt):
-        '''
+        """
         Add a prompt to the store.
-        prompt: a Prompt object.
-        '''
+
+        Parameters:
+            prompt: a Prompt object.
+        """
         raise NotImplementedError
-    
+
     def update(self, prompt):
-        '''
+        """
         Update a prompt in the store.
-        prompt: a Prompt object.
-        '''
+
+        Parameters:
+            prompt: a Prompt object.
+        """
         raise NotImplementedError
-    
+
     def get_by_ids(self, ids):
-        '''
+        """
         Get a list of prompts by their ids.
-        ids: a list of UUIDs.
-        '''
+
+        Parameters:
+            ids: a list of UUIDs.
+        """
         raise NotImplementedError
-    
+
+    def purge(self):
+        """
+        Purge the store of all prompts.
+
+        """
+        raise NotImplementedError
+
 
 def prompt_to_db(prompt):
-    return (prompt.id, prompt.text, str(prompt.scores) if prompt.scores else None, str(prompt.embeddings) if prompt.embeddings else None)
+    """
+    Convert a prompt to a tuple that can be inserted into the database.
+
+    Parameters:
+        prompt: a Prompt object.
+    """
+    return (prompt.id, prompt.text, prompt.response, str(prompt.scores) if prompt.scores else None, str(prompt.embeddings) if prompt.embeddings else None)
 
 def db_to_prompt(db_prompt):
+    """
+    Convert a database row to a Prompt object.
+
+    Parameters:
+        db_prompt: a database row.
+    """
     return Prompt(
-        id=uuid.UUID(bytes_le=db_prompt['id']), 
-        text=db_prompt['text'], 
-        scores=json.loads(db_prompt['scores']), 
-        embeddings=json.loads(db_prompt['embeddings']) if db_prompt['embeddings'] else None
+        id=uuid.UUID(bytes_le=db_prompt['id']),
+        text=db_prompt['text'],
+        response=db_prompt['response'],
+        scores=ast.literal_eval(db_prompt['scores']),
+        embeddings=ast.literal_eval(db_prompt['embeddings']) if db_prompt['embeddings'] else None
     )
 
 class SQLitePromptStore(PromptStore):
-    '''
-    A prompt store that uses SQLite as a backend.
-    '''
-    def __init__(self, name="anchor.db"):
+    """
+    An impementation of a prompt store that uses a SQLite backend.
+    """
+    def __init__(self, name='anchor.db', debug=False):
         self.name = name
         self.connection = sqlite3.connect(name)
-        # self.connection.set_trace_callback(print)
+        if debug:
+            self.connection.set_trace_callback(print)
         self.connection.row_factory = sqlite3.Row
-        self.connection.execute("CREATE TABLE IF NOT EXISTS prompts (id UUID, text TEXT, scores JSON, embeddings JSON)")
+        self.connection.execute('CREATE TABLE IF NOT EXISTS prompts (id UUID, text TEXT, response TEXT, scores JSON, embeddings JSON)')
 
     def add(self, prompt):
-        self.connection.execute("INSERT INTO prompts VALUES (?, ?, ?, ?)", prompt_to_db(prompt))
+        self.connection.execute('INSERT INTO prompts VALUES (?, ?, ?, ?, ?)', prompt_to_db(prompt))
         self.connection.commit()
         return prompt
 
     def update(self, prompt):
-        (id, text, scores, embeddings) = prompt_to_db(prompt)
-        self.connection.execute("UPDATE prompts SET text=?, scores=?, embeddings=? WHERE id=?", (text, scores, embeddings, id))
+        (id, text, response, scores, embeddings) = prompt_to_db(prompt)
+        self.connection.execute('UPDATE prompts SET text=?, response=?, scores=?, embeddings=? WHERE id=?', (text, response, scores, embeddings, id))
         self.connection.commit()
         return prompt
-    
+
+    def purge(self):
+        self.connection.execute('DELETE FROM prompts')
+        self.connection.commit()
+
     def get_by_ids(self, ids):
-        result = self.connection.execute(f"SELECT * FROM prompts WHERE id IN ({','.join(['?'] * len(ids))})", ids).fetchall()
+        result = self.connection.execute(f'SELECT * FROM prompts WHERE id IN ({",".join(["?"] * len(ids))})', ids).fetchall()
 
         return [db_to_prompt(row) for row in result]
 
-    def select_prompts(self, fields='text, id, scores, embeddings', where='1=1', order_by='id', limit='-1'):
+    def select_prompts(self, fields='text, response, id, scores, embeddings', where='1=1', order_by='id', limit='-1'):
 
-        return [db_to_prompt(row) for row in self.connection.execute(f"SELECT {fields} FROM prompts WHERE {where} ORDER BY {order_by} LIMIT {limit}")]
+        return [db_to_prompt(row) for row in self.connection.execute(f'SELECT {fields} FROM prompts WHERE {where} ORDER BY {order_by} LIMIT {limit}')]
```

### Comparing `anchor-gpt-0.0.1/setup.py` & `anchor-gpt-0.0.2/setup.py`

 * *Files identical despite different names*

