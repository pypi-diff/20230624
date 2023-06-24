# Comparing `tmp/jam_ai-0.1.5.tar.gz` & `tmp/jam_ai-0.1.6.tar.gz`

## Comparing `jam_ai-0.1.5.tar` & `jam_ai-0.1.6.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/cmd/__init__.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.1.5/cmd/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/personnel/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/personnel/albert-einstein.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/personnel/homer-simpson.json
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/personnel/marie-curie.json
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/personnel/walter-white.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/base.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/core.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/version.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/instrument/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/instrument/base.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/instrument/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/instrument/text.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/interface/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/interface/base.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/interface/openai.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/interface/stability_ai.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/persistence/__init__.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/persistence/base.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/persistence/memory.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/persistence/model.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/persistence/sqlite.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/personnel/__init__.py
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/personnel/base.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/personnel/personnel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/util/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/util/generate.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/util/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/tests/instrument/__init__.py
--rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.1.5/tests/instrument/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/tests/interface/__init__.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.1.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.1.5/LICENSE
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 jam_ai-0.1.5/README.md
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jam_ai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 jam_ai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/cmd/__init__.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.1.6/cmd/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/personnel/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/personnel/albert-einstein.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/personnel/homer-simpson.json
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/personnel/marie-curie.json
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/personnel/walter-white.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/base.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/core.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/version.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/instrument/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/instrument/base.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/instrument/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/instrument/text.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/interface/__init__.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/interface/base.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/interface/openai.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/interface/stability_ai.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/interface/writesonic.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/persistence/__init__.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/persistence/base.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/persistence/memory.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/persistence/model.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/persistence/sqlite.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/personnel/__init__.py
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/personnel/base.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/personnel/personnel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/util/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/util/generate.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/util/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/tests/instrument/__init__.py
+-rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.1.6/tests/instrument/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/tests/interface/__init__.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 jam_ai-0.1.6/tests/interface/test_base.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.1.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 jam_ai-0.1.6/README.md
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jam_ai-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 jam_ai-0.1.6/PKG-INFO
```

### Comparing `jam_ai-0.1.5/cmd/main.py` & `jam_ai-0.1.6/cmd/main.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/example/personnel/albert-einstein.json` & `jam_ai-0.1.6/example/personnel/albert-einstein.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/example/personnel/homer-simpson.json` & `jam_ai-0.1.6/example/personnel/homer-simpson.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/example/personnel/marie-curie.json` & `jam_ai-0.1.6/example/personnel/marie-curie.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/example/personnel/walter-white.json` & `jam_ai-0.1.6/example/personnel/walter-white.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/jam/base.py` & `jam_ai-0.1.6/jam/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/jam/core.py` & `jam_ai-0.1.6/jam/core.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/jam/instrument/base.py` & `jam_ai-0.1.6/jam/instrument/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/jam/instrument/image.py` & `jam_ai-0.1.6/jam/instrument/image.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/jam/interface/openai.py` & `jam_ai-0.1.6/jam/interface/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,19 +83,19 @@
                  samples: int = 1,
                  dimension: Tuple[int, int] = (512, 512)):
         super(OpenAIImageGen, self).__init__(token, model)
 
         self.samples = samples
         self.width, self.height = dimension
 
-    def call(self, prompt: AnyStr = None) -> JIOutput:
+    def call(self, x: AnyStr = None) -> JIOutput:
         try:
             filenames = []
             response = openai.Image.create(
-                prompt=prompt,
+                prompt=x,
                 n=self.samples,
                 size=f'{self.width}x{self.height}'
             )
 
             for resp in response.get('data', []):
                 filename = f'DALLE_{generate_id(8)}.png'
                 img_url = resp.get('url', '')
```

### Comparing `jam_ai-0.1.5/jam/interface/stability_ai.py` & `jam_ai-0.1.6/jam/interface/stability_ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     def __init__(self,
                  engine: str = 'stable-diffusion-v1',
                  api_key: str = None,
                  host: str = 'grpc.stability.ai:443',
                  verbose: bool = True):
         super(StabilityText2Image, self).__init__(engine, api_key, host, verbose)
 
-    def call(self, x: AnyStr = None):
+    def call(self, x: AnyStr = None) -> JIOutput:
         filenames = []
         response = self.stability_api.generate(
             prompt=x,
             steps=self.step,
             cfg_scale=self.cfg_scale,
             width=self.width,
             height=self.height,
```

### Comparing `jam_ai-0.1.5/jam/persistence/base.py` & `jam_ai-0.1.6/jam/persistence/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/jam/persistence/memory.py` & `jam_ai-0.1.6/jam/persistence/memory.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/jam/persistence/model.py` & `jam_ai-0.1.6/jam/persistence/model.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/jam/persistence/sqlite.py` & `jam_ai-0.1.6/jam/persistence/sqlite.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/jam/personnel/base.py` & `jam_ai-0.1.6/jam/personnel/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/tests/instrument/test_base.py` & `jam_ai-0.1.6/tests/instrument/test_base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/.gitignore` & `jam_ai-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/LICENSE` & `jam_ai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/README.md` & `jam_ai-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.5/pyproject.toml` & `jam_ai-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jam-ai"
-version = "0.1.5"
+version = "0.1.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 authors = [
   { name="Abhishta Gatya", email="abhishtagatya@yahoo.com" },
 ]
 description = "Experimental collaboration tool to use multiple AI personnel together equipped with instructed function calls."
 keywords = ["openai", "multi agent", "chat engine", "collaboration", "machine learning", "data science"]
 readme = "README.md"
```

### Comparing `jam_ai-0.1.5/PKG-INFO` & `jam_ai-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jam-ai
-Version: 0.1.5
+Version: 0.1.6
 Summary: Experimental collaboration tool to use multiple AI personnel together equipped with instructed function calls.
 Project-URL: homepage, https://github.com/abhishtagatya/jam
 Project-URL: documentation, https://github.com/abhishtagatya/jam
 Project-URL: changelog, https://github.com/abhishtagatya/jam/blob/master/CHANGELOG.md
 Author-email: Abhishta Gatya <abhishtagatya@yahoo.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
```

