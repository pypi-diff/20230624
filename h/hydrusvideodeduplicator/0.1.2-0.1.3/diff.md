# Comparing `tmp/hydrusvideodeduplicator-0.1.2.tar.gz` & `tmp/hydrusvideodeduplicator-0.1.3.tar.gz`

## Comparing `hydrusvideodeduplicator-0.1.2.tar` & `hydrusvideodeduplicator-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/README.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/pdq_utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_faiss.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/LICENSE
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/README.md
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/README.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/pdq_utils.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_faiss.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/README.md
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.3/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/README.md` & `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 - threshold is the min % matching to be considered similar. 100% is identical.
 - verbose turns on logging
 - debug turns on logging and sets the logging level to debug
 """
 rprint(f"[blue] Hydrus Video Deduplicator {__version__} [/]")
 
 def main(api_key: Annotated[Optional[str], typer.Option(help="Hydrus API Key")] = None,
-        api_url: Annotated[Optional[str], typer.Option(help="Hydrus API URL")] = None,
+        api_url: Annotated[Optional[str], typer.Option(help="Hydrus API URL")] = HYDRUS_API_URL,
         overwrite:  Annotated[Optional[bool], typer.Option(help="Overwrite existing perceptual hashes")] = False,
         query: Annotated[Optional[List[str]], typer.Option(help="Custom Hydrus tag query")] = None,
         threshold: Annotated[Optional[float], typer.Option(help="Similarity threshold for a pair of videos where 100 is identical")] = VPDQ_QUERY_MATCH_THRESHOLD_PERCENT,
         skip_hashing: Annotated[Optional[bool], typer.Option(help="Skip perceptual hashing and just search for duplicates")] = False,
         verbose:  Annotated[Optional[bool], typer.Option(hidden=True)] = False,
         debug: Annotated[Optional[bool], typer.Option(hidden=True)] = False,
         ):
@@ -62,15 +62,17 @@
         print("API key not set. Exiting...")
         raise typer.Exit(code=1)
     # This should not happen because there's a default val in secret.py
     if not api_url:
         print("Hydrus URL not set. Exiting...")
         raise typer.Exit(code=1)
 
+    print(f"Connecting to {api_url}")
     # Client connection
+    # TODO: Try to connect with https first and then fallback to http with a strong warning
     _client = hydrus_api.Client(api_url=api_url,
                                 access_key=api_key)
 
     error_connecting = True
     error_connecting_exception_msg = ""
     error_connecting_exception = ""
     try:
```

### Comparing `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/dedup.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/pdq_utils.py` & `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/pdq_utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq.py` & `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_brute_matcher.py` & `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_brute_matcher.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_faiss.py` & `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_faiss.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/src/hydrusvideodeduplicator/vpdq_util.py` & `hydrusvideodeduplicator-0.1.3/src/hydrusvideodeduplicator/vpdq_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/.gitignore` & `hydrusvideodeduplicator-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/LICENSE` & `hydrusvideodeduplicator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/README.md` & `hydrusvideodeduplicator-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/pyproject.toml` & `hydrusvideodeduplicator-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.2/PKG-INFO` & `hydrusvideodeduplicator-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/appleappleapplenanner/hydrus-video-deduplicator
 Author: appleappleapplenanner
 License-Expression: MIT
 License-File: LICENSE
```

