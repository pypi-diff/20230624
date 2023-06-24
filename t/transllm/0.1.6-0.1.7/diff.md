# Comparing `tmp/transllm-0.1.6.tar.gz` & `tmp/transllm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transllm-0.1.6.tar", last modified: Sat Jun 24 14:03:37 2023, max compression
+gzip compressed data, was "transllm-0.1.7.tar", last modified: Sat Jun 24 15:10:35 2023, max compression
```

## Comparing `transllm-0.1.6.tar` & `transllm-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 14:03:37.757740 transllm-0.1.6/
--rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     8476 2023-06-24 14:03:37.756731 transllm-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     7537 2023-06-24 14:00:52.000000 transllm-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 14:03:37.757740 transllm-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2059 2023-06-24 14:01:12.000000 transllm-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 14:03:37.739723 transllm-0.1.6/transllm/
--rw-rw-rw-   0        0        0      192 2023-06-24 14:01:17.000000 transllm-0.1.6/transllm/__init__.py
--rw-rw-rw-   0        0        0     3600 2023-06-24 13:55:20.000000 transllm-0.1.6/transllm/core.py
-drwxrwxrwx   0        0        0        0 2023-06-24 14:03:37.754730 transllm-0.1.6/transllm.egg-info/
--rw-rw-rw-   0        0        0     8476 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 15:10:35.168963 transllm-0.1.7/
+-rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     8476 2023-06-24 15:10:35.167950 transllm-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7537 2023-06-24 14:00:52.000000 transllm-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 15:10:35.168963 transllm-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     2035 2023-06-24 15:10:12.000000 transllm-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:10:35.149854 transllm-0.1.7/transllm/
+-rw-rw-rw-   0        0        0      192 2023-06-24 15:10:18.000000 transllm-0.1.7/transllm/__init__.py
+-rw-rw-rw-   0        0        0     3629 2023-06-24 15:02:32.000000 transllm-0.1.7/transllm/core.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:10:35.165277 transllm-0.1.7/transllm.egg-info/
+-rw-rw-rw-   0        0        0     8476 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      122 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 15:10:35.000000 transllm-0.1.7/transllm.egg-info/top_level.txt
```

### Comparing `transllm-0.1.6/LICENSE` & `transllm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `transllm-0.1.6/PKG-INFO` & `transllm-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.6
+Version: 0.1.7
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transllm Version: 0.1.6 Summary: LLMtranslator
+Metadata-Version: 2.1 Name: transllm Version: 0.1.7 Summary: LLMtranslator
 translates and generates text in multiple languages. Home-page: https://
 github.com/dsdanielpark/hf-transllm Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Science/Research Classifier: Natural
 Language :: English Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `transllm-0.1.6/README.md` & `transllm-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `transllm-0.1.6/setup.py` & `transllm-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="transllm",
-    version="0.1.6",
+    version="0.1.7",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="LLMtranslator translates and generates text in multiple languages.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/hf-transllm",
     packages=find_packages(exclude=[]),
@@ -38,15 +38,14 @@
         "requests",
         "deep_translator",
         "colorama",
         "httpx[http2]",
         "torch",
         "deepl",
         "transformers",
-        "googletrans",
         "bardapi",
         "openai",
         "sentencepiece",
         "accelerate",
         "translang"
     ],
     keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
```

### Comparing `transllm-0.1.6/transllm/core.py` & `transllm-0.1.7/transllm/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def __init__(
         self,
         model_path,
         target_lang="ko",
         translator="google",
         torch_dtype=torch.float16,
-        offload_folder="offload",
+        offload_folder=None,
         device_map="auto",
         deepl_api_key=None,
         bard_api_key=None,
         openai_api_key=None,
         openai_model="gpt-3.5-turbo",
     ):
         super().__init__(
@@ -42,14 +42,15 @@
         )
         self.model_path = model_path
         self.target_lang = target_lang
         self.tokenizer = LlamaTokenizer.from_pretrained(model_path)
         self.model = LlamaForCausalLM.from_pretrained(
             model_path, torch_dtype=torch_dtype, device_map=device_map, offload_folder=offload_folder
         )
+        self.model.tie_weights()
 
     def process_prompt(self, prompt: str) -> str:
         """
         Preprocesses the prompt text for translation.
 
         Args:
             prompt (str): The prompt text.
```

### Comparing `transllm-0.1.6/transllm.egg-info/PKG-INFO` & `transllm-0.1.7/transllm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.6
+Version: 0.1.7
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transllm Version: 0.1.6 Summary: LLMtranslator
+Metadata-Version: 2.1 Name: transllm Version: 0.1.7 Summary: LLMtranslator
 translates and generates text in multiple languages. Home-page: https://
 github.com/dsdanielpark/hf-transllm Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Science/Research Classifier: Natural
 Language :: English Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

