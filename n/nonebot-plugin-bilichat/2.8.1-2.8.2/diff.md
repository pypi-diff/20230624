# Comparing `tmp/nonebot_plugin_bilichat-2.8.1.tar.gz` & `tmp/nonebot_plugin_bilichat-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.8.1.tar", last modified: Thu Jun 22 14:45:47 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.8.2.tar", last modified: Sat Jun 24 11:10:42 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.8.1.tar` & `nonebot_plugin_bilichat-2.8.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    34523 2023-06-22 14:45:34.022725 nonebot_plugin_bilichat-2.8.1/LICENSE
--rw-r--r--   0        0        0    12397 2023-06-22 14:45:34.022725 nonebot_plugin_bilichat-2.8.1/README.md
--rw-r--r--   0        0        0     9690 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     5472 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      844 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      871 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6502 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    16355 2023-06-22 14:45:34.038725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     2773 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1187 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7534 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     2017 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    27644 2023-06-22 14:45:34.042725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/newbing.png
--rw-r--r--   0        0        0    59199 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     1363 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     6710 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2200 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     3082 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-22 14:45:34.046725 nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1583 2023-06-22 14:45:47.622857 nonebot_plugin_bilichat-2.8.1/pyproject.toml
--rw-r--r--   0        0        0    13972 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-24 11:10:33.094688 nonebot_plugin_bilichat-2.8.2/LICENSE
+-rw-r--r--   0        0        0    12397 2023-06-24 11:10:33.094688 nonebot_plugin_bilichat-2.8.2/README.md
+-rw-r--r--   0        0        0     9690 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     5767 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      844 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      871 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6502 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    16355 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     2773 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-24 11:10:33.114688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1187 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7534 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     2098 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    27644 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/newbing.png
+-rw-r--r--   0        0        0    59199 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     1363 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     6710 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4932 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2200 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     3133 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-24 11:10:33.118688 nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1583 2023-06-24 11:10:42.206816 nonebot_plugin_bilichat-2.8.2/pyproject.toml
+-rw-r--r--   0        0        0    13972 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.8.2/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.8.1/LICENSE` & `nonebot_plugin_bilichat-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/README.md` & `nonebot_plugin_bilichat-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,37 +48,50 @@
 
     # AI Summary
     bilichat_newbing_cookie: Optional[str]
     bilichat_newbing_token_limit: int = 0
     bilichat_newbing_preprocess: bool = True
     bilichat_openai_token: Optional[str]
     bilichat_openai_proxy: Optional[str]
-    bilichat_openai_model: Literal["gpt-3.5-turbo-0301", "gpt-4-0314", "gpt-4-32k-0314"] = "gpt-3.5-turbo-0301"
+    bilichat_openai_model: Literal[
+        "gpt-3.5-turbo",
+        "gpt-3.5-turbo-0301",
+        "gpt-3.5-turbo-0613",
+        "gpt-3.5-turbo-16k",
+        "gpt-3.5-turbo-16k-0613",
+        "gpt-4",
+        "gpt-4-0314",
+        "gpt-4-0613",
+        "gpt-4-32k-0314",
+    ] = "gpt-3.5-turbo-0301"
     bilichat_openai_token_limit: int = 3500
 
-    @validator("bilichat_openai_proxy",always=True,pre=True)
+    @validator("bilichat_openai_proxy", always=True, pre=True)
     def check_openai_proxy(cls, v, values):
         if not (values["bilichat_openai_token"] or values["bilichat_newbing_cookie"]):
             return v
         if v is None:
-            logger.warning("you have enabled openai or newbing summary without a proxy, this may cause request failure.")
+            logger.warning(
+                "you have enabled openai or newbing summary without a proxy, this may cause request failure."
+            )
         return v
 
     @validator("bilichat_openai_token_limit")
     def check_token_limit(cls, v, values):
         if values["bilichat_openai_token"] is None:
             return v
         if not isinstance(v, int):
             v = int(v)
-        model = values["bilichat_openai_model"]
-        max_limit = {
-            "gpt-3.5-turbo-0301": 3500,
-            "gpt-4-0314": 7600,
-            "gpt-4-32k-0314": 32200,
-        }.get(model, 3500)
+        model: str = values["bilichat_openai_model"]
+        if model.startswith("gpt-3.5"):
+            max_limit = 15000 if "16k" in model else 3500
+        elif model.startswith("gpt-4"):
+            max_limit = 32200 if "32k" in model else 7600
+        else:
+            max_limit = 3500
         if v > max_limit:
             logger.error(
                 f"Model {model} has a token cap of {max_limit} instead of {v}, token will be replaced with {max_limit}"
             )
             v = max_limit
         return v
 
@@ -108,43 +121,42 @@
                 raise ValueError("Config bilichat_newbing_cookie got a problem occurred") from e
 
         elif Path(v).is_dir():
             raise ValueError(f"Config bilichat_newbing_cookie requires a file, but {v} is a folder")
 
         elif v == "no_login":
             logger.info("Using newbing summary without a cookie")
-        
+
         else:
             raise ValueError(f"Path {v} is not recognized")
 
         return v
 
     @validator("bilichat_word_cloud", always=True)
     def check_pypackage_wordcloud(cls, v):
         if (importlib.util.find_spec("wordcloud") and importlib.util.find_spec("jieba")) or not v:
             return v
         else:
             raise RuntimeError(
                 "Package(s) of fuction wordcloud not installed, use **pip install nonebot-plugin-bilichat[wordcloud]** to install required dependencies"
             )
-    
-    @validator("bilichat_basic_info_style",always=True)
-    def check_htmlrender(cls,v):
+
+    @validator("bilichat_basic_info_style", always=True)
+    def check_htmlrender(cls, v):
         if v == "bbot_default":
             return v
         else:
             try:
                 require("nonebot_plugin_htmlrender")
                 return v
             except Exception as e:
                 raise RuntimeError(
                     "Package(s) of fuction styles not installed, use **pip install nonebot-plugin-bilichat[extra]** to install required dependencies"
                 ) from e
 
-
     def verify_permission(self, uid: Union[str, int]):
         if self.bilichat_whitelist:
             return str(uid) in self.bilichat_whitelist
         elif self.bilichat_blacklist:
             return str(uid) not in self.bilichat_blacklist
         else:
             return True
```

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -6,29 +6,36 @@
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>AI视频总结</title>
     <style>
       @font-face {
         font-family: "base";
         src: url("https://fonts.bbot?name=HarmonyOS_Sans_SC_Medium.ttf");
       }
+      
       @font-face {
         font-family: "emoji";
         src: url("https://fonts.bbot?name=nte.ttf");
       }
+      
       * {
         box-sizing: border-box;
         font-family: "base", "emoji", sans-serif;
       }
+      
       body,
       html {
         height: 100%;
         margin: 0;
         background-color: #fcf4dc; /* 浅黄色背景 */
       }
-
+      
+      .main {
+        padding: 16px 0;
+      }
+      
       .container {
         max-width: 720px;
         margin: 0 auto;
         position: relative;
         font-size: 32px;
       }
```

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/newbing.png` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/newbing.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import random
 from collections import OrderedDict
-from typing import Dict, List, Optional,Literal
+from typing import Dict, List, Optional, Literal
 
 import httpx
 import tiktoken_async
 from loguru import logger
 
 from ..config import plugin_config
 from ..model.openai import OpenAI, TokenUsage
@@ -32,18 +32,18 @@
         )
     )
 
 
 def count_tokens(prompts: List[Dict[str, str]]):
     """根据内容计算 token 数"""
 
-    if plugin_config.bilichat_openai_model == "gpt-3.5-turbo-0301":
+    if plugin_config.bilichat_openai_model.startswith("gpt-3.5"):
         tokens_per_message = 4
         tokens_per_name = -1
-    elif plugin_config.bilichat_openai_model == "gpt-4":
+    elif plugin_config.bilichat_openai_model.startswith("gpt-4"):
         tokens_per_message = 3
         tokens_per_name = 1
     else:
         raise ValueError(f"Unknown model name {plugin_config.bilichat_openai_model}")
 
     num_tokens = 0
     for message in prompts:
@@ -52,15 +52,17 @@
             num_tokens += len(tiktoken_enc.encode(value))
             if key == "name":
                 num_tokens += tokens_per_name
     num_tokens += 3
     return num_tokens
 
 
-def get_small_size_transcripts(title:str,text_data: List[str], token_limit: int = plugin_config.bilichat_openai_token_limit):
+def get_small_size_transcripts(
+    title: str, text_data: List[str], token_limit: int = plugin_config.bilichat_openai_token_limit
+):
     unique_texts = list(OrderedDict.fromkeys(text_data))
     while count_tokens(get_summarise_prompt(title, " ".join(unique_texts))) > token_limit:
         unique_texts.pop(random.randint(0, len(unique_texts) - 1))
     return " ".join(unique_texts)
 
 
 def get_full_prompt(prompt: Optional[str] = None, system: Optional[str] = None, language: Optional[str] = None):
```

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,13 +75,15 @@
             type="png",
         )
     return img_raw
 
 
 async def t2i(data: str, src: str):
     try:
+        if len(data) < 30:
+            return data
         if plugin_config.bilichat_basic_info_style != "bbot_default":
             return await pw_text2image(data, src)
         return await rich_text2image(data, src)
     except Exception as e:
         logger.exception(e)
         return f"总结图片生成失败 {e}\n {data}"
```

### Comparing `nonebot_plugin_bilichat-2.8.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.8.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.8.1/pyproject.toml` & `nonebot_plugin_bilichat-2.8.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.8.1"
+version = "2.8.2"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.8.1/PKG-INFO` & `nonebot_plugin_bilichat-2.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.8.1
+Version: 2.8.2
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.8.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.8.2 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
```

