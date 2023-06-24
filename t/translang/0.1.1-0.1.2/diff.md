# Comparing `tmp/translang-0.1.1.tar.gz` & `tmp/translang-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translang-0.1.1.tar", last modified: Sat Jun 24 09:33:04 2023, max compression
+gzip compressed data, was "translang-0.1.2.tar", last modified: Sat Jun 24 13:37:56 2023, max compression
```

## Comparing `translang-0.1.1.tar` & `translang-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 09:33:04.323889 translang-0.1.1/
--rw-rw-rw-   0        0        0     1089 2023-06-24 08:01:00.000000 translang-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4288 2023-06-24 09:33:04.322888 translang-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-06-24 09:24:07.000000 translang-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 09:33:04.323889 translang-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1839 2023-06-24 09:24:23.000000 translang-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 09:33:04.305080 translang-0.1.1/translang/
--rw-rw-rw-   0        0        0      203 2023-06-24 09:24:27.000000 translang-0.1.1/translang/__init__.py
--rw-rw-rw-   0        0        0     4759 2023-06-24 09:23:52.000000 translang-0.1.1/translang/core.py
-drwxrwxrwx   0        0        0        0 2023-06-24 09:33:04.321882 translang-0.1.1/translang.egg-info/
--rw-rw-rw-   0        0        0     4288 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 13:37:56.605661 translang-0.1.2/
+-rw-rw-rw-   0        0        0     1089 2023-06-24 08:01:00.000000 translang-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4288 2023-06-24 13:37:56.604187 translang-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-06-24 09:24:07.000000 translang-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:37:56.605661 translang-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1839 2023-06-24 13:22:18.000000 translang-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:37:56.591343 translang-0.1.2/translang/
+-rw-rw-rw-   0        0        0      203 2023-06-24 13:35:58.000000 translang-0.1.2/translang/__init__.py
+-rw-rw-rw-   0        0        0     5097 2023-06-24 13:35:23.000000 translang-0.1.2/translang/core.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:37:56.602179 translang-0.1.2/translang.egg-info/
+-rw-rw-rw-   0        0        0     4288 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-24 13:37:56.000000 translang-0.1.2/translang.egg-info/top_level.txt
```

### Comparing `translang-0.1.1/LICENSE` & `translang-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `translang-0.1.1/PKG-INFO` & `translang-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translang
-Version: 0.1.1
+Version: 0.1.2
 Summary: Translation Service API Module.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `translang-0.1.1/README.md` & `translang-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `translang-0.1.1/setup.py` & `translang-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="translang",
-    version="0.1.1",
+    version="0.1.2",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="Translation Service API Module.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/hf-transllm",
     packages=find_packages(exclude=[]),
```

### Comparing `translang-0.1.1/translang/core.py` & `translang-0.1.2/translang/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,21 +47,32 @@
         elif self.translator == "deepl":
             self.translator_engine = deepl.Translator(auth_key=self.deepl_api_key)
         elif self.translator == "bard":
             self.translator_engine = Bard(token=self.bard_api_key)
         elif self.translator == "openai":
             openai.api_key = self.openai_api_key
 
-    def _refine_bard(self, text):
-        try: 
-            extracted_text = re.search(r'\*\*(.*?)\*\*', text).group(1)
-        except:
-            matches = re.findall(r'"([^"]+)"', text)
-            extracted_text=matches[1]
-        return extracted_text
+                
+    def _refine_bard_answer(self, text: str) -> str:
+        """
+        Extracts and returns refined text from the given input text using specific patterns.
+        
+        Args:
+            text (str): The input text to be refined.
+        
+        Returns:
+            str: The refined text extracted from the input text.
+        """
+        extracted_text = re.search(r'```(.*?)```|\*\*(.*?)\*\*', text, re.DOTALL)
+        
+        if extracted_text:
+            return extracted_text.group(1) or extracted_text.group(2) 
+        
+        return text
+
 
     def translate(self, text: str, dest_lang: str) -> str:
         """
         Translate the given text to the specified destination language.
 
         Args:
             text (str): The text to be translated.
@@ -74,22 +85,23 @@
         if self.use_cache:
             cache_key = (text, dest_lang)
             translated_text = self.translation_cache.get(cache_key)
             if translated_text is not None:
                 return translated_text
 
         if self.translator == "google":
-            translated_text = self.translator_engine.translate(text, dest=dest_lang).text
+            translator_obj = Translator()
+            translated_text = translator_obj.translate(text, dest=dest_lang).text
         elif self.translator == "deepl":
             translated_text = self.translator_engine.translate_text(text, target_lang=dest_lang).text
         elif self.translator == "bard":
-            translated = self.translator_engine.get_answer(f"translate {text} to {dest_lang} only")['content']
-            translated_text = self._refine_bard(translated)
+            translated = self.translator_engine.get_answer(f"Translate the following text to {dest_lang}: {text}")['content']
+            translated_text = self._refine_bard_answer(translated)
         elif self.translator == "openai":
-            prompt = f"Translate the following text to {dest_lang}: {text}\nLanguage: {self.openai_model}\n\nTranslation:"
+            prompt = f"Translate the following text to {dest_lang}: {text}"
             response = openai.Completion.create(engine=self.openai_model, prompt=prompt, max_tokens=100)
             translated_text = response.choices[0].text.strip()
 
         if self.use_cache:
             cache_key = (text, dest_lang)
             self.translation_cache[cache_key] = translated_text
```

### Comparing `translang-0.1.1/translang.egg-info/PKG-INFO` & `translang-0.1.2/translang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translang
-Version: 0.1.1
+Version: 0.1.2
 Summary: Translation Service API Module.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

