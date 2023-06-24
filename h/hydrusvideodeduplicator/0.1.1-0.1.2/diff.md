# Comparing `tmp/hydrusvideodeduplicator-0.1.1.tar.gz` & `tmp/hydrusvideodeduplicator-0.1.2.tar.gz`

## Comparing `hydrusvideodeduplicator-0.1.1.tar` & `hydrusvideodeduplicator-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/README.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/pdq_utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/vpdq.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/vpdq_faiss.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/vpdq_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/LICENSE
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/README.md
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/README.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/pdq_utils.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_faiss.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/README.md
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/README.md` & `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/__main__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/dedup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+import os
 from io import IOBase
 import logging
 import tempfile
 from itertools import islice
 import json
 import shelve
 
 import hydrus_api
 import hydrus_api.utils
-from numpy import base_repr, binary_repr, bitwise_xor
 from tqdm import tqdm
 from rich import print as rprint
 
-from .config import DEDUP_DATABASE_NAME
+from .config import DEDUP_DATABASE_FILE, DEDUP_DATABASE_DIR, DEDUP_DATABASE_NAME
 from .dedup_util import find_tag_in_tags, get_file_names_hydrus
 from .vpdq import VPDQSignal
 
 from .vpdq_util import (
     VPDQ_QUERY_MATCH_THRESHOLD_PERCENT,
 )
 
@@ -70,26 +70,37 @@
         self._find_potential_duplicates()
         self.hydlog.info("Deduplication done.")
 
     # Update perceptual hash for videos
     # By default only adds missing phashes
     # TODO: Allow batching, where if a video is already in the DB get another until no videos left or count is 0
     def _add_perceptual_hash_to_videos(self, overwrite: bool, custom_query: list | None = None) -> None:
+
+        # Create database folder if it doesn't already exist
+        if os.path.exists(DEDUP_DATABASE_FILE):
+            with shelve.open(str(DEDUP_DATABASE_FILE)) as hashdb:
+                rprint(f"[green] Database found with {len(hashdb)} videos already hashed.")
+                self.hydlog.info(f"Found existing DB of length {len(hashdb)}, size {os.path.getsize(DEDUP_DATABASE_FILE)}")
+        else:
+            rprint(f"[yellow] Database not found. Creating one at {DEDUP_DATABASE_FILE}")
+            os.makedirs(DEDUP_DATABASE_DIR, exist_ok=True)
+            self.hydlog.info(f"Created DB dir {DEDUP_DATABASE_DIR}")
+
         search_tags = ["system:filetype=video"]
         if custom_query is not None:
             custom_query = [x for x in custom_query if x.strip()] # Remove whitespace and empty strings
             search_tags.extend(custom_query)
         
         # GET video files SHA256 with no perceptual hash tag and store for later
         print(f"Retrieving video file hashes from {self.client.api_url}")
         percep_tagged_video_hashes = self.client.search_files(search_tags, return_hashes=True)["hashes"]
         
         print("Calculating perceptual hashes:")
         
-        with shelve.open(DEDUP_DATABASE_NAME) as hashdb:
+        with shelve.open(str(DEDUP_DATABASE_FILE)) as hashdb:
             with tempfile.TemporaryDirectory() as tmp_dir_name:
                 for video_hash in tqdm(percep_tagged_video_hashes):
                     # don't calc new value unless overwrite is true
                     if not overwrite and video_hash in hashdb:
                         continue
 
                     # TODO: Check for valid request?
@@ -130,15 +141,15 @@
         # TODO: Add support for query where it will get a list of the hashes from
         # the query and iterate over them instead of the entire hashdb
 
         # Number of potential duplicates before adding more. Just for user info.
         pre_dedupe_count = self.get_potential_duplicate_count_hydrus()
 
         similar_files_found_count = 0
-        with shelve.open(DEDUP_DATABASE_NAME) as hashdb:
+        with shelve.open(str(DEDUP_DATABASE_FILE)) as hashdb:
             video_count = len(hashdb)
             for i, video in enumerate(tqdm(hashdb.items(), desc="Finding duplicates")):
                 video_hash, video_phash = video[0], video[1]
                 for video2 in islice(hashdb.items(), i+1, None):
                     video2_hash, video2_phash = video2[0], video2[1]
```

### Comparing `hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/pdq_utils.py` & `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/pdq_utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/vpdq.py` & `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/vpdq_brute_matcher.py` & `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_brute_matcher.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/vpdq_faiss.py` & `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_faiss.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.1/src/hydrusvideodeduplicator/vpdq_util.py` & `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.1/.gitignore` & `hydrusvideodeduplicator-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.1/LICENSE` & `hydrusvideodeduplicator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.1/README.md` & `hydrusvideodeduplicator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.1/pyproject.toml` & `hydrusvideodeduplicator-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
+    "appdirs",
     "hydrus-api",
     "rich",
     "numpy",
     "tqdm",
     "python-dotenv",
     "typer",
     "vpdq",
@@ -157,8 +158,8 @@
 tests = ["tests", "*/hydrus-video-deduplicator/tests"]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
-]
+]
```

### Comparing `hydrusvideodeduplicator-0.1.1/PKG-INFO` & `hydrusvideodeduplicator-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/appleappleapplenanner/hydrus-video-deduplicator
 Author: appleappleapplenanner
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
+Requires-Dist: appdirs
 Requires-Dist: hydrus-api
 Requires-Dist: numpy
 Requires-Dist: python-dotenv
 Requires-Dist: rich
 Requires-Dist: tqdm
 Requires-Dist: typer
 Requires-Dist: vpdq
```

