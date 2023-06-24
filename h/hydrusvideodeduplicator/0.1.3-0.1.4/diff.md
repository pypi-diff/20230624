# Comparing `tmp/hydrusvideodeduplicator-0.1.3.tar.gz` & `tmp/hydrusvideodeduplicator-0.1.4.tar.gz`

## Comparing `hydrusvideodeduplicator-0.1.3.tar` & `hydrusvideodeduplicator-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/README.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/pdq_utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_faiss.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/LICENSE
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/README.md
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/README.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    10894 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/pdq_utils.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_faiss.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/README.md
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/README.md` & `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/__main__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 HYDRUS_LOCAL_TAG_SERVICE_NAME=os.getenv("HYDRUS_LOCAL_TAG_SERVICE_NAME", "my tags")
 
 # ~/.local/share/hydrusvideodeduplicator/ on Linux
 DEDUP_DATABASE_DIR=AppDirs("hydrusvideodeduplicator").user_data_dir
 DEDUP_DATABASE_DIR=os.getenv("DEDUP_DATABASE_DIR", DEDUP_DATABASE_DIR)
 DEDUP_DATABASE_DIR=Path(DEDUP_DATABASE_DIR)
 
-DEDUP_DATABASE_NAME=os.getenv("DEDUP_DATABASE_NAME", "hashdb")
-DEDUP_DATABASE_FILE=Path(DEDUP_DATABASE_DIR, DEDUP_DATABASE_NAME)
+DEDUP_DATABASE_NAME=os.getenv("DEDUP_DATABASE_NAME", "videohashes")
+DEDUP_DATABASE_FILE=Path(DEDUP_DATABASE_DIR, f"{DEDUP_DATABASE_NAME}.sqlite")
```

### Comparing `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/dedup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from io import IOBase
 import logging
 import tempfile
 from itertools import islice
 import json
-import shelve
+from sqlitedict import SqliteDict
 
 import hydrus_api
 import hydrus_api.utils
 from tqdm import tqdm
 from rich import print as rprint
 
 from .config import DEDUP_DATABASE_FILE, DEDUP_DATABASE_DIR, DEDUP_DATABASE_NAME
@@ -38,15 +38,15 @@
     def __init__(self, client: hydrus_api.Client,
                  verify_connection: bool = True):
         self.client = client
         if verify_connection:
             self.verify_api_connection()
         self.hydlog.setLevel(logging.WARNING)
         
-        # Commonly used things from the database
+        # Commonly used things from the Hydrus database
         # If any of these are large they should probably be lazily loaded
         self.all_services = self.client.get_services()
 
     # Verify client connection and permissions
     # Will throw a hydrus_api.APIError if something is wrong
     def verify_api_connection(self):
         self.hydlog.info(f"Client API version: v{self.client.VERSION} | Endpoint API version: v{self.client.get_api_version()['version']}")
@@ -73,90 +73,115 @@
     # Update perceptual hash for videos
     # By default only adds missing phashes
     # TODO: Allow batching, where if a video is already in the DB get another until no videos left or count is 0
     def _add_perceptual_hash_to_videos(self, overwrite: bool, custom_query: list | None = None) -> None:
 
         # Create database folder if it doesn't already exist
         if os.path.exists(DEDUP_DATABASE_FILE):
-            with shelve.open(str(DEDUP_DATABASE_FILE)) as hashdb:
+            with SqliteDict(str(DEDUP_DATABASE_FILE), tablename = "videos") as hashdb:
                 rprint(f"[green] Database found with {len(hashdb)} videos already hashed.")
                 self.hydlog.info(f"Found existing DB of length {len(hashdb)}, size {os.path.getsize(DEDUP_DATABASE_FILE)}")
         else:
             rprint(f"[yellow] Database not found. Creating one at {DEDUP_DATABASE_FILE}")
             os.makedirs(DEDUP_DATABASE_DIR, exist_ok=True)
             self.hydlog.info(f"Created DB dir {DEDUP_DATABASE_DIR}")
 
         search_tags = ["system:filetype=video"]
         if custom_query is not None:
             custom_query = [x for x in custom_query if x.strip()] # Remove whitespace and empty strings
             search_tags.extend(custom_query)
         
         # GET video files SHA256 with no perceptual hash tag and store for later
         print(f"Retrieving video file hashes from {self.client.api_url}")
+        # TODO: This could be absolutely massive. Chunk it somehow. Maybe with a query where hashes must not equal previous hashes processed?
         percep_tagged_video_hashes = self.client.search_files(search_tags, return_hashes=True)["hashes"]
         
         print("Calculating perceptual hashes:")
-        
-        with shelve.open(str(DEDUP_DATABASE_FILE)) as hashdb:
+
+        with SqliteDict(str(DEDUP_DATABASE_FILE), tablename = "videos") as hashdb:
             with tempfile.TemporaryDirectory() as tmp_dir_name:
+                # Commit every n videos to avoid excessive writes
+                commit_interval = 8    
+                count_since_last_commit = 0
                 for video_hash in tqdm(percep_tagged_video_hashes):
                     # don't calc new value unless overwrite is true
                     if not overwrite and video_hash in hashdb:
                         continue
+                    
+                    count_since_last_commit+=1
 
                     # TODO: Check for valid request?
                     video_response = self.client.get_file(hash_=video_hash)
                     try:
                         # spooled file means it stays in RAM unless it's too big
                         with tempfile.NamedTemporaryFile(mode="w+b", dir=tmp_dir_name) as tmp_vid_file:
                             tmp_vid_file.write(video_response.content)
                             tmp_vid_file.seek(0)
                             
                             hashdb[video_hash] = VPDQSignal.hash_from_file(tmp_vid_file.name)
                             self.hydlog.debug(f"Perceptual hash calculated and written to DB.")
                     except KeyboardInterrupt:
                         rprint("[red] Perceptual hash generation was interrupted!\n")
-                        return None
+                        break
                     # TODO: Don't catch everything.
                     except Exception as exc:
                         rprint("[red] Failed to calculate a perceptual hash.")
                         self.hydlog.error(f"Bad file hash: {video_hash}")
                         self.hydlog.error(exc)
-                        continue
+                    
+                    if count_since_last_commit >= commit_interval:
+                        hashdb.commit()
+                        count_since_last_commit = 0
 
+            hashdb.commit()
+            
         rprint("[green]All perceptual hash tags have been added to video files.\n")
     
     def get_potential_duplicate_count_hydrus(self) -> int:
         return self.client.get_potentials_count(file_service_keys=[self.all_services["all_local_files"][0]["service_key"]])["potential_duplicates_count"]
     
     # Return similarity of two bitstrings given a threshold
     @staticmethod
     def is_similar(a: str, b: str, min_percent_similarity: float = 0.8) -> bool:
         return VPDQSignal.compare_hash(a, b, min_percent_similarity, min_percent_similarity)
 
     # Sliding window duplicate comparisons
     # Alternatively, I could scan duplicates while adding and never do it again. I should do that instead.
     # Or, since dictionaries are ordered, store the index per hash where it ended its last search. If it's not the end, keep going until the end.
     def _find_potential_duplicates(self): 
+        # Check if table and DB exists before iterating over it since it's in read mode not the "c" r/w create mode
+        try:
+            with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="r") as hashdb:
+                pass
+        except OSError:
+            rprint(f"[red] Database does not exist. Cannot search for duplicates.")
+            return None
+        except RuntimeError: # SqliteDict error when trying to create a table for a DB in read-only mode
+            rprint(f"[red] Database does not exist. Cannot search for duplicates.")
+            return None
 
         # TODO: Add support for query where it will get a list of the hashes from
         # the query and iterate over them instead of the entire hashdb
 
+        # TODO: This can be multithreaded
+
         # Number of potential duplicates before adding more. Just for user info.
         pre_dedupe_count = self.get_potential_duplicate_count_hydrus()
 
         similar_files_found_count = 0
-        with shelve.open(str(DEDUP_DATABASE_FILE)) as hashdb:
-            video_count = len(hashdb)
-            for i, video in enumerate(tqdm(hashdb.items(), desc="Finding duplicates")):
+        
+        video_counter = 0
+        with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="r") as hashdb:
+            # tqdm progress bar is broken for SqliteDict because len doesn't work
+            for i, video in tqdm(enumerate(hashdb.items()), desc="Finding duplicates"):
+                video_counter+=1
                 video_hash, video_phash = video[0], video[1]
                 for video2 in islice(hashdb.items(), i+1, None):
                     video2_hash, video2_phash = video2[0], video2[1]
                     
-                    
                     similar = HydrusVideoDeduplicator.is_similar(video_phash, video2_phash, self.threshold)
                     
                     if similar:
                         similar_files_found_count += 1
                         if self._DEBUG:
                             file_names = get_file_names_hydrus(self.client, [video_hash, video2_hash])
                             self.hydlog.info(f"Duplicates filenames: {file_names}")
@@ -167,25 +192,26 @@
                             "hash_b": str(video2_hash),
                             "relationship": int(hydrus_api.DuplicateStatus.POTENTIAL_DUPLICATES),
                             "do_default_content_merge": True,
                         }
                     
                         # This throws always because set_file_relationships
                         # in the Hydrus API doesn't have a response or something.
+                        # There is a pull request for this on GitLab I should fork and merge
                         # TODO: Defer this API call to speed up processing
                         try:
                             self.client.set_file_relationships([new_relationship])
                         except json.decoder.JSONDecodeError:
                             pass
 
         # Statistics for user
         # if user does duplicates processing while the script is running this count will be wrong.
         if similar_files_found_count > 0:
-            rprint(f"[blue] {similar_files_found_count}/{video_count} total similar videos found")
+            rprint(f"[blue] {similar_files_found_count}/{video_counter} similar videos found")
             post_dedupe_count = self.get_potential_duplicate_count_hydrus()
             new_dedupes_count = post_dedupe_count-pre_dedupe_count
             if new_dedupes_count > 0:
                 rprint(f"[green] {new_dedupes_count} new potential duplicates marked for processing!")
             else:
                 rprint("[green] No new potential duplicates")
         else:
-            rprint(f"[yellow] No potential duplicates found out of {video_count} videos")
+            rprint(f"[yellow] No potential duplicates found out of {video_counter} videos")
```

### Comparing `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/pdq_utils.py` & `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/pdq_utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq.py` & `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_brute_matcher.py` & `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_brute_matcher.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_faiss.py` & `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_faiss.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_util.py` & `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.3/.gitignore` & `hydrusvideodeduplicator-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.3/LICENSE` & `hydrusvideodeduplicator-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.3/README.md` & `hydrusvideodeduplicator-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.3/pyproject.toml` & `hydrusvideodeduplicator-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "hydrus-api",
     "rich",
     "numpy",
     "tqdm",
     "python-dotenv",
     "typer",
     "vpdq",
+    "sqlitedict",
 ]
 
 [project.urls]
 Documentation = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme"
 Issues = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues"
 Source = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator"
```

### Comparing `hydrusvideodeduplicator-0.1.3/PKG-INFO` & `hydrusvideodeduplicator-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.1.3
+Version: 0.1.4
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/appleappleapplenanner/hydrus-video-deduplicator
 Author: appleappleapplenanner
 License-Expression: MIT
 License-File: LICENSE
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: appdirs
 Requires-Dist: hydrus-api
 Requires-Dist: numpy
 Requires-Dist: python-dotenv
 Requires-Dist: rich
+Requires-Dist: sqlitedict
 Requires-Dist: tqdm
 Requires-Dist: typer
 Requires-Dist: vpdq
 Description-Content-Type: text/markdown
 
 <div align="center">
```

