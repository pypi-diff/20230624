# Comparing `tmp/translang-0.1.2.tar.gz` & `tmp/translang-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translang-0.1.2.tar", last modified: Sat Jun 24 13:37:56 2023, max compression
+gzip compressed data, was "translang-0.1.3.tar", last modified: Sat Jun 24 13:50:07 2023, max compression
```

## Comparing `translang-0.1.2.tar` & `translang-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 13:37:56.605661 translang-0.1.2/
--rw-rw-rw-   0        0        0     1089 2023-06-24 08:01:00.000000 translang-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4288 2023-06-24 13:37:56.604187 translang-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-06-24 09:24:07.000000 translang-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 13:37:56.605661 translang-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1839 2023-06-24 13:22:18.000000 translang-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:37:56.591343 translang-0.1.2/translang/
--rw-rw-rw-   0        0        0      203 2023-06-24 13:35:58.000000 translang-0.1.2/translang/__init__.py
--rw-rw-rw-   0        0        0     5097 2023-06-24 13:35:23.000000 translang-0.1.2/translang/core.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:37:56.602179 translang-0.1.2/translang.egg-info/
--rw-rw-rw-   0        0        0     4288 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 13:50:07.715774 translang-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-06-24 08:01:00.000000 translang-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4288 2023-06-24 13:50:07.714773 translang-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-06-24 09:24:07.000000 translang-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:50:07.715774 translang-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1843 2023-06-24 13:49:05.000000 translang-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:50:07.699080 translang-0.1.3/translang/
+-rw-rw-rw-   0        0        0      203 2023-06-24 13:49:10.000000 translang-0.1.3/translang/__init__.py
+-rw-rw-rw-   0        0        0     5106 2023-06-24 13:48:19.000000 translang-0.1.3/translang/core.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:50:07.712777 translang-0.1.3/translang.egg-info/
+-rw-rw-rw-   0        0        0     4288 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       46 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/top_level.txt
```

### Comparing `translang-0.1.2/LICENSE` & `translang-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `translang-0.1.2/PKG-INFO` & `translang-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translang
-Version: 0.1.2
+Version: 0.1.3
 Summary: Translation Service API Module.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `translang-0.1.2/README.md` & `translang-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `translang-0.1.2/setup.py` & `translang-0.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 
 
 version = get_version()
 
 
 setup(
     name="translang",
-    version="0.1.2",
+    version="0.1.3",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="Translation Service API Module.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/hf-transllm",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
     install_requires=[
         "requests",
         "deepl",
-        "googletrans",
+        "deep_translator",
         "bardapi",
         "openai",
     ],
     keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
```

### Comparing `translang-0.1.2/translang/core.py` & `translang-0.1.3/translang/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import deepl
 import openai
 import concurrent.futures
-from googletrans import Translator
+from deep_translator import GoogleTranslator
 from bardapi import Bard
 from typing import List
 
 
 class TranslationService:
     """
     A service for translating text using different translation engines.
@@ -39,15 +39,15 @@
         self.openai_model = openai_model
         self.use_cache = use_cache
 
         self.translation_cache = {}
         self.translator_engine = None
 
         if self.translator == "google":
-            self.translator_engine = Translator()
+            pass
         elif self.translator == "deepl":
             self.translator_engine = deepl.Translator(auth_key=self.deepl_api_key)
         elif self.translator == "bard":
             self.translator_engine = Bard(token=self.bard_api_key)
         elif self.translator == "openai":
             openai.api_key = self.openai_api_key
 
@@ -85,16 +85,16 @@
         if self.use_cache:
             cache_key = (text, dest_lang)
             translated_text = self.translation_cache.get(cache_key)
             if translated_text is not None:
                 return translated_text
 
         if self.translator == "google":
-            translator_obj = Translator()
-            translated_text = translator_obj.translate(text, dest=dest_lang).text
+            self.translator_engine = GoogleTranslator(source="auto", target=dest_lang)
+            translated_text = self.translator_engine.translate(text)
         elif self.translator == "deepl":
             translated_text = self.translator_engine.translate_text(text, target_lang=dest_lang).text
         elif self.translator == "bard":
             translated = self.translator_engine.get_answer(f"Translate the following text to {dest_lang}: {text}")['content']
             translated_text = self._refine_bard_answer(translated)
         elif self.translator == "openai":
             prompt = f"Translate the following text to {dest_lang}: {text}"
```

### Comparing `translang-0.1.2/translang.egg-info/PKG-INFO` & `translang-0.1.3/translang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translang
-Version: 0.1.2
+Version: 0.1.3
 Summary: Translation Service API Module.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

