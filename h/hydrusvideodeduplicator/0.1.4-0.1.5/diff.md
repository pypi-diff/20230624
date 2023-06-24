# Comparing `tmp/hydrusvideodeduplicator-0.1.4.tar.gz` & `tmp/hydrusvideodeduplicator-0.1.5.tar.gz`

## Comparing `hydrusvideodeduplicator-0.1.4.tar` & `hydrusvideodeduplicator-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/README.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    10894 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/pdq_utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_faiss.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/LICENSE
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/README.md
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/README.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    11276 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/pdq_utils.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_faiss.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/README.md
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.5/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/README.md` & `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/__main__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/config.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/dedup.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,24 +113,31 @@
                     video_response = self.client.get_file(hash_=video_hash)
                     try:
                         # spooled file means it stays in RAM unless it's too big
                         with tempfile.NamedTemporaryFile(mode="w+b", dir=tmp_dir_name) as tmp_vid_file:
                             tmp_vid_file.write(video_response.content)
                             tmp_vid_file.seek(0)
                             
-                            hashdb[video_hash] = VPDQSignal.hash_from_file(tmp_vid_file.name)
-                            self.hydlog.debug(f"Perceptual hash calculated and written to DB.")
+                            # Set perceptual_hash column
+                            perceptual_hash = VPDQSignal.hash_from_file(tmp_vid_file.name)
+                            try:
+                                row = hashdb[video_hash]
+                            except KeyError:
+                                hashdb[video_hash] = {}
+
+                            row = hashdb[video_hash]
+                            row["perceptual_hash"] = perceptual_hash
+                            hashdb[video_hash] = row
+                            self.hydlog.debug(f"Perceptual hash calculated and added to DB.")
                     except KeyboardInterrupt:
                         rprint("[red] Perceptual hash generation was interrupted!\n")
                         break
-                    # TODO: Don't catch everything.
-                    except Exception as exc:
+                    except:
                         rprint("[red] Failed to calculate a perceptual hash.")
-                        self.hydlog.error(f"Bad file hash: {video_hash}")
-                        self.hydlog.error(exc)
+                        self.hydlog.error(f"Errored file hash: {video_hash}")
                     
                     if count_since_last_commit >= commit_interval:
                         hashdb.commit()
                         count_since_last_commit = 0
 
             hashdb.commit()
             
@@ -168,19 +175,20 @@
         pre_dedupe_count = self.get_potential_duplicate_count_hydrus()
 
         similar_files_found_count = 0
         
         video_counter = 0
         with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="r") as hashdb:
             # tqdm progress bar is broken for SqliteDict because len doesn't work
-            for i, video in tqdm(enumerate(hashdb.items()), desc="Finding duplicates"):
+            for i, video_hash in tqdm(enumerate(hashdb), desc="Finding duplicates"):
                 video_counter+=1
-                video_hash, video_phash = video[0], video[1]
-                for video2 in islice(hashdb.items(), i+1, None):
-                    video2_hash, video2_phash = video2[0], video2[1]
+                video_phash = hashdb[video_hash]["perceptual_hash"]
+                # TODO: Are sqlite databases ordered?
+                for video2_hash in islice(hashdb, i+1, None):
+                    video2_phash = hashdb[video2_hash]["perceptual_hash"]
                     
                     similar = HydrusVideoDeduplicator.is_similar(video_phash, video2_phash, self.threshold)
                     
                     if similar:
                         similar_files_found_count += 1
                         if self._DEBUG:
                             file_names = get_file_names_hydrus(self.client, [video_hash, video2_hash])
@@ -192,15 +200,15 @@
                             "hash_b": str(video2_hash),
                             "relationship": int(hydrus_api.DuplicateStatus.POTENTIAL_DUPLICATES),
                             "do_default_content_merge": True,
                         }
                     
                         # This throws always because set_file_relationships
                         # in the Hydrus API doesn't have a response or something.
-                        # There is a pull request for this on GitLab I should fork and merge
+                        # There is a pull request for this on the Hydrus API GitLab I should fork and merge
                         # TODO: Defer this API call to speed up processing
                         try:
                             self.client.set_file_relationships([new_relationship])
                         except json.decoder.JSONDecodeError:
                             pass
 
         # Statistics for user
```

### Comparing `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/pdq_utils.py` & `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/pdq_utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq.py` & `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_brute_matcher.py` & `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_brute_matcher.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_faiss.py` & `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_faiss.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/src/hydrusvideodeduplicator/vpdq_util.py` & `hydrusvideodeduplicator-0.1.5/src/hydrusvideodeduplicator/vpdq_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/.gitignore` & `hydrusvideodeduplicator-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/LICENSE` & `hydrusvideodeduplicator-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/README.md` & `hydrusvideodeduplicator-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/pyproject.toml` & `hydrusvideodeduplicator-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.4/PKG-INFO` & `hydrusvideodeduplicator-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.1.4
+Version: 0.1.5
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/appleappleapplenanner/hydrus-video-deduplicator
 Author: appleappleapplenanner
 License-Expression: MIT
 License-File: LICENSE
```

