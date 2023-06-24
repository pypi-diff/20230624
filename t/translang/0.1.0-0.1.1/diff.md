# Comparing `tmp/translang-0.1.0.tar.gz` & `tmp/translang-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translang-0.1.0.tar", last modified: Sat Jun 24 07:51:59 2023, max compression
+gzip compressed data, was "translang-0.1.1.tar", last modified: Sat Jun 24 09:33:04 2023, max compression
```

## Comparing `translang-0.1.0.tar` & `translang-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 07:51:59.964444 translang-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-06-24 07:21:53.000000 translang-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3761 2023-06-24 07:51:59.964444 translang-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2856 2023-06-24 07:47:52.000000 translang-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 07:51:59.965444 translang-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1839 2023-06-24 07:48:28.000000 translang-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:51:59.947432 translang-0.1.0/translang/
--rw-rw-rw-   0        0        0      203 2023-06-24 07:49:16.000000 translang-0.1.0/translang/__init__.py
--rw-rw-rw-   0        0        0     5249 2023-06-24 07:50:57.000000 translang-0.1.0/translang/core.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:51:59.962441 translang-0.1.0/translang.egg-info/
--rw-rw-rw-   0        0        0     3761 2023-06-24 07:51:59.000000 translang-0.1.0/translang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-24 07:51:59.000000 translang-0.1.0/translang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 07:51:59.000000 translang-0.1.0/translang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-24 07:51:59.000000 translang-0.1.0/translang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 07:51:59.000000 translang-0.1.0/translang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-24 07:51:59.000000 translang-0.1.0/translang.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 09:33:04.323889 translang-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2023-06-24 08:01:00.000000 translang-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4288 2023-06-24 09:33:04.322888 translang-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-06-24 09:24:07.000000 translang-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 09:33:04.323889 translang-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1839 2023-06-24 09:24:23.000000 translang-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:33:04.305080 translang-0.1.1/translang/
+-rw-rw-rw-   0        0        0      203 2023-06-24 09:24:27.000000 translang-0.1.1/translang/__init__.py
+-rw-rw-rw-   0        0        0     4759 2023-06-24 09:23:52.000000 translang-0.1.1/translang/core.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:33:04.321882 translang-0.1.1/translang.egg-info/
+-rw-rw-rw-   0        0        0     4288 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-24 09:33:04.000000 translang-0.1.1/translang.egg-info/top_level.txt
```

### Comparing `translang-0.1.0/README.md` & `translang-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 # translang
-Translation Service Module
+Translation Service Module for other projects. Refer to the [hf-transllm](https://github.com/dsdanielpark/hf-transllm) Project for Reference.
 
 
-# Install
+
+## Install
 ```
 pip install translang
 ```
 
-# Usage
 
-Google Translator
-```python
-translator = TranslationService(translator="google")
 
-text = "Hello, how are you?"
-destination_lang = "es"  # Spanish
-
-translated_text = asyncio.run(translator.translate(text, destination_lang))
-print(f"Translated Text (Google Translate): {translated_text}")
-```
+## Usage
+### Seamless Integration of Translation APIs through Inheritance
+You can easily extend the `TranslationService` class to integrate with popular translation API services.
 
-DeepL
 ```python
-translator = TranslationService(translator="deepl", deepl_api="YOUR_DEEPL_API_KEY")
+from translang import TranslationService
 
-text = "Hello, how are you?"
-destination_lang = "es"  # Spanish
-
-translated_text = asyncio.run(translator.translate(text, destination_lang))
-print(f"Translated Text (DeepL Translate): {translated_text}")
+class CustomTranslationService(TranslationService):
+    def __init__(self, translator="google", deepl_api_key=None, bard_api_key=None, openai_api_key=None, openai_model='gpt-3.5-turbo'):
+        super().__init__(translator, deepl_api_key, bard_api_key, openai_api_key, openai_model)
+
+    def custom_process_with_translation(self, text: str, dest_lang: str) -> str:
+        translated_text = self.translate(text, dest_lang)
+        # Perform additional customization or processing if needed
+        return translated_text
 ```
 
-Bard
 ```python
-translator = TranslationService(translator="bard", bard_api="YOUR_BARD_API_KEY")
-
-text = "Hello, how are you?"
-destination_lang = "es"  # Spanish
+translator = CustomTranslationService(translator="google")
 
-translated_text = asyncio.run(translator.translate(text, destination_lang))
-print(f"Translated Text (Bard Translate): {translated_text}")
+translated_text = translator.custom_process_with_translation("Hello", "ko")
+print(translated_text)
 ```
 
-OpenAI
+
+### Static Methods
+
+Google Translator
 ```python
-translator = TranslationService(translator="openai", openai_api="YOUR_OPENAI_API_KEY")
+fomr translang import TranslationService
 
-text = "Hello, how are you?"
-destination_lang = "es"  # Spanish
+translator = TranslationService(translator="google")                                                                         # Google
+# translator = TranslationService(translator="deepl", deepl_api_key="YOUR_DEEPL_API_KEY")                                    # DeepL
+# translator = TranslationService(translator="bard", bard_api_key="YOUR_BARD_API_KEY")                                       # Bard
+# translator = TranslationService(translator="openai", openai_api_key="YOUR_OPENAI_API_KEY", openai_model="gpt-3.5-trubo")   # Open AI
 
-translated_text = asyncio.run(translator.translate(text, destination_lang))
-print(f"Translated Text (OpenAI Translate): {translated_text}")
+translated_text = translator.translate("Hello", "ko")
+print(translated_text)
 ```
 
 
 ## License
 [MIT](https://opensource.org/license/mit/) <br>
 I hold no legal responsibility; 
 ```
@@ -77,13 +74,13 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 ```
 
-## Bugs and Issues
+### Bugs and Issues
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated.
 
-## Contacts
+### Contacts
 - Core maintainer: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
 - E-mail: parkminwoo1991@gmail.com <br>
```

### Comparing `translang-0.1.0/setup.py` & `translang-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="translang",
-    version="0.1.0",
+    version="0.1.1",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="Translation Service API Module.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/hf-transllm",
     packages=find_packages(exclude=[]),
```

### Comparing `translang-0.1.0/translang/core.py` & `translang-0.1.1/translang/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,130 +1,112 @@
-# Copyright (c) 2023 Park Minwoo MIT License
-
 import re
 import deepl
 import openai
-import asyncio
-from bardapi import Bard
+import concurrent.futures
 from googletrans import Translator
+from bardapi import Bard
+from typing import List
 
 
 class TranslationService:
-    def __init__(self, translator="google", deepl_api=None, bard_api=None, openai_api=None, openai_model='gpt-3.5-turbo'):
-        """
-        The TranslationService class provides functionality to translate text using various translation services.
+    """
+    A service for translating text using different translation engines.
 
-        :param translator: The translation service to use (default: "google")
-        :param deepl_api: DeepL API key (if required)
-        :param bard_api: Bard API key (if required)
-        :param openai_api: OpenAI API key (if required)
-        :param openai_model: OpenAI model name (default: "gpt-3.5-turbo")
-        """
+    Args:
+        translator (str, optional): The translation engine to use. Defaults to "google".
+        deepl_api_key (str, optional): API key for DeepL translator. Required if translator is "deepl".
+        bard_api_key (str, optional): API key for Bard translator. Required if translator is "bard".
+        openai_api_key (str, optional): API key for OpenAI translator. Required if translator is "openai".
+        openai_model (str, optional): The OpenAI model to use. Defaults to "gpt-3.5-turbo".
+        use_cache (bool, optional): Whether to use a translation cache. Defaults to False.
+
+    Attributes:
+        translator (str): The translation engine being used.
+        deepl_api_key (str): API key for DeepL translator.
+        bard_api_key (str): API key for Bard translator.
+        openai_api_key (str): API key for OpenAI translator.
+        openai_model (str): The OpenAI model being used.
+        use_cache (bool): Whether to use a translation cache.
+        translation_cache (dict): Cache for storing translated texts.
+        translator_engine: The translation engine object.
+
+    """
+
+    def __init__(self, translator="google", deepl_api_key=None, bard_api_key=None, openai_api_key=None, openai_model='gpt-3.5-turbo', use_cache=False):
         self.translator = translator
-        self.deepl_api = deepl_api
-        self.bard_api = bard_api
-        self.openai_api = openai_api
+        self.deepl_api_key = deepl_api_key
+        self.bard_api_key = bard_api_key
+        self.openai_api_key = openai_api_key
         self.openai_model = openai_model
+        self.use_cache = use_cache
 
         self.translation_cache = {}
-        self.translator_obj = None
-
-    async def translate(self, text: str, dest_lang: str) -> str:
-        """
-        Translates the given text to the specified destination language.
-
-        :param text: The text to be translated
-        :param dest_lang: The destination language for translation
-        :return: The translated text
-        """
-        cache_key = (text, dest_lang)
-        translated_text = self.translation_cache.get(cache_key)
-        if translated_text is not None:
-            return translated_text
-
-        if self.translator_obj is None:
-            self.translator_obj = self.create_translator()
+        self.translator_engine = None
 
         if self.translator == "google":
-            translated_text = await self.async_translate_google(text, dest_lang)
+            self.translator_engine = Translator()
         elif self.translator == "deepl":
-            translated_text = await self.async_translate_deepl(text, dest_lang)
+            self.translator_engine = deepl.Translator(auth_key=self.deepl_api_key)
         elif self.translator == "bard":
-            translated_text = await self.async_translate_bard(text, dest_lang)
+            self.translator_engine = Bard(token=self.bard_api_key)
         elif self.translator == "openai":
-            translated_text = await self.async_translate_openai(text, dest_lang)
-
-        self.translation_cache[cache_key] = translated_text
-        return translated_text
-
-    def create_translator(self):
-        """
-        Creates an instance of the translator based on the selected translation service.
+            openai.api_key = self.openai_api_key
 
-        :return: The translator object
-        """
-        if self.translator == "google":
-            return Translator()
-        elif self.translator == "deepl":
-            return deepl.Translator(self.deepl_api)
-        elif self.translator == "bard":
-            return Bard(token=self.bard_api)
+    def _refine_bard(self, text):
+        try: 
+            extracted_text = re.search(r'\*\*(.*?)\*\*', text).group(1)
+        except:
+            matches = re.findall(r'"([^"]+)"', text)
+            extracted_text=matches[1]
+        return extracted_text
 
-    async def async_translate_google(self, text, dest_lang):
+    def translate(self, text: str, dest_lang: str) -> str:
         """
-        Translates the text using Google Translate asynchronously.
+        Translate the given text to the specified destination language.
 
-        :param text: The text to be translated
-        :param dest_lang: The destination language for translation
-        :return: The translated text
-        """
-        return (await self.translator_obj.translate(text, dest=dest_lang)).text
+        Args:
+            text (str): The text to be translated.
+            dest_lang (str): The destination language code.
 
-    async def async_translate_deepl(self, text, dest_lang):
-        """
-        Translates the text using DeepL Translate asynchronously.
+        Returns:
+            str: The translated text.
 
-        :param text: The text to be translated
-        :param dest_lang: The destination language for translation
-        :return: The translated text
         """
-        return (await self.translator_obj.translate_text(text, target_lang=dest_lang)).text
+        if self.use_cache:
+            cache_key = (text, dest_lang)
+            translated_text = self.translation_cache.get(cache_key)
+            if translated_text is not None:
+                return translated_text
 
-    async def async_translate_bard(self, text, dest_lang):
-        """
-        Translates the text using Bard Translate asynchronously.
+        if self.translator == "google":
+            translated_text = self.translator_engine.translate(text, dest=dest_lang).text
+        elif self.translator == "deepl":
+            translated_text = self.translator_engine.translate_text(text, target_lang=dest_lang).text
+        elif self.translator == "bard":
+            translated = self.translator_engine.get_answer(f"translate {text} to {dest_lang} only")['content']
+            translated_text = self._refine_bard(translated)
+        elif self.translator == "openai":
+            prompt = f"Translate the following text to {dest_lang}: {text}\nLanguage: {self.openai_model}\n\nTranslation:"
+            response = openai.Completion.create(engine=self.openai_model, prompt=prompt, max_tokens=100)
+            translated_text = response.choices[0].text.strip()
+
+        if self.use_cache:
+            cache_key = (text, dest_lang)
+            self.translation_cache[cache_key] = translated_text
 
-        :param text: The text to be translated
-        :param dest_lang: The destination language for translation
-        :return: The translated text
-        """
-        translated = (await self.translator_obj.get_answer(f"translate {text} to {dest_lang} only"))['content']
-        extracted_text = re.findall(r'"([^"]*)"', translated)
-        return extracted_text[0]
+        return translated_text
 
-    async def async_translate_openai(self, text, dest_lang):
+    def translate_parallel(self, texts: List[str], dest_lang: str) -> List[str]:
         """
-        Translates the text using OpenAI Translate asynchronously.
+        Translate a list of texts to the specified destination language in parallel.
 
-        :param text: The text to be translated
-        :param dest_lang: The destination language for translation
-        :return: The translated text
-        """
-        openai.api_key = self.openai_api
-        prompt = f"Translate the following text to {dest_lang}: {text}\nLanguage: {self.openai_model}\n\nTranslation:"
-        response = await asyncio.get_event_loop().run_in_executor(None, openai.Completion.create, engine=self.openai_model, prompt=prompt, max_tokens=100)
-        translated_text = response.choices[0].text.strip()
-        return translated_text
+        Args:
+            texts (List[str]): The list of texts to be translated.
+            dest_lang (str): The destination language code.
 
-    def translate_batch(self, texts: list, dest_lang: str) -> list:
-        """
-        Translates a batch of texts to the specified destination language.
+        Returns:
+            List[str]: The list of translated texts.
 
-        :param texts: The list of texts to be translated
-        :param dest_lang: The destination language for translation
-        :return: The list of translated texts
         """
-        results = []
-        for text in texts:
-            result = self.translate(text, dest_lang)
-            results.append(result)
-        return results
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            translated_texts = list(executor.map(self.translate, texts, [dest_lang] * len(texts)))
+        return translated_texts
```

