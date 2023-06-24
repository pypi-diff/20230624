# Comparing `tmp/transllm-0.1.5.tar.gz` & `tmp/transllm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transllm-0.1.5.tar", last modified: Fri Jun 23 10:54:59 2023, max compression
+gzip compressed data, was "transllm-0.1.6.tar", last modified: Sat Jun 24 14:03:37 2023, max compression
```

## Comparing `transllm-0.1.5.tar` & `transllm-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 10:54:59.021558 transllm-0.1.5/
--rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     6197 2023-06-23 10:54:59.020559 transllm-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     5258 2023-06-23 10:49:39.000000 transllm-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 10:54:59.021558 transllm-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2037 2023-06-23 10:54:48.000000 transllm-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:54:58.999569 transllm-0.1.5/transllm/
--rw-rw-rw-   0        0        0      192 2023-06-23 10:54:46.000000 transllm-0.1.5/transllm/__init__.py
--rw-rw-rw-   0        0        0     5718 2023-06-23 10:54:29.000000 transllm-0.1.5/transllm/core.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:54:59.017557 transllm-0.1.5/transllm.egg-info/
--rw-rw-rw-   0        0        0     6197 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 14:03:37.757740 transllm-0.1.6/
+-rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     8476 2023-06-24 14:03:37.756731 transllm-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7537 2023-06-24 14:00:52.000000 transllm-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 14:03:37.757740 transllm-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     2059 2023-06-24 14:01:12.000000 transllm-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:03:37.739723 transllm-0.1.6/transllm/
+-rw-rw-rw-   0        0        0      192 2023-06-24 14:01:17.000000 transllm-0.1.6/transllm/__init__.py
+-rw-rw-rw-   0        0        0     3600 2023-06-24 13:55:20.000000 transllm-0.1.6/transllm/core.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:03:37.754730 transllm-0.1.6/transllm.egg-info/
+-rw-rw-rw-   0        0        0     8476 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 14:03:37.000000 transllm-0.1.6/transllm.egg-info/top_level.txt
```

### Comparing `transllm-0.1.5/LICENSE` & `transllm-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `transllm-0.1.5/PKG-INFO` & `transllm-0.1.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.5
+Version: 0.1.6
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -30,50 +30,59 @@
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
 <a href="https://pypi.org/project/transllm/"><img alt="PyPI" src="https://img.shields.io/pypi/v/transllm"></a>
 </p>
 
 
 > LLMtranslator translates and generates text in multiple languages.
 
-![](assets/hf-transllm.png)
+![](assets/transllm.png)
 
-Through the inference module of Hugging Face, you can conveniently use the results of Hugging Face's open-source large language model. However, there are limitations in retraining or evaluating the model's performance in various languages.
+### Introducing hf-transllm: Unlock the Power of Multilingual Exploration
 
-Therefore, this package allows you to explore the results of the Hugging Face inference module in multiple languages using various trnaslated_answer API services.
-
-Since the purpose of the Hugging Face inference module is more focused on checking the model weights easily rather than efficiency, this package emphasizes the ability to explore the results in various languages rather than efficiency.
+Discover the hf-transllm package, a seamless integration of Hugging Face's inference module and translation APIs. Overcome limitations in retraining and evaluating large language models in different languages. Explore diverse results effortlessly, leveraging translation API services. Emphasizing versatility over efficiency, hf-transllm enables you to delve into the outcomes of Hugging Face's models in various languages.
 
 
 <br>
 
 
 <br>
 
-## Install
+## Installation
 ```
 pip install transllm
 ```
+Or
+```
+pip install git+https://github.com/dsdanielpark/hf-trnasllm.git
+```
+
+<br>
 
 If you wish to use the various features and CLI:
 ```
 pip install git+https://github.com/dsdanielpark/hf-transllm.git
 cd hf-transllm
-python main.py
+pip install -r requirements.txt
+```
+There can be issues with various dependencies such as Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the appropriate environment by searching online.
+```bash
+python main.py --hfmodel <openlm-research/open_llama_3b> --lang <ko> --translator <google>
 ```
-
 <br>
 
 <br>
 
 ## Usage 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
+Applying LLMs to the majority of Hugging Face repositories is generally feasible. However, it can be challenging to apply them to objects that require unique tokenizers or inference processes. In such cases, it is recommended to customize the usage by incorporating a translation module for prompts.
 
-Simple Usage
+In other words, if you are familiar with the inference process or code from Hugging Face repositories, you can customize the translation object by adding a translation module before and after the known inference process or code.
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
 
-- Google Trnaslator
+Google Trnaslator
+- Support Languages: https://github.com/ssut/py-googletrans/blob/master/googletrans/constants.py
 ```python
 from transllm import LLMtranslator
 
 # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b'
 # model_path = 'openlm-research/open_llama_7b'
 # model_path = 'openlm-research/open_llama_13b'
@@ -85,15 +94,18 @@
 prompt = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 trnaslated_answer = open_llama3b_kor.generate(prompt)
 print(trnaslated_answer)
 ```
 
 <br>
 
-- DeepL, OpenAI, Bard
+DeepL
+- Support Languages: https://www.deepl.com/pro/select-country?cta=header-pro-button/#developer
+
+Open AI, Bard use pre-prompt for translation.
 ```python
 from transllm import LLMtranslator
 
 # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b'
 # model_path = 'openlm-research/open_llama_7b'
 # model_path = 'openlm-research/open_llama_13b'
@@ -107,14 +119,59 @@
 prompt = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 trnaslated_answer = open_llama3b_kor.generate(prompt)
 print(trnaslated_answer)
 ```
 
 <br>
 
+## Customized Inference
+```python
+import torch
+from trnasllm import LLMtranslator
+
+
+class MyLLMtranslator(LLMtranslator):
+    def __init__(
+        self,
+        model_path,
+        target_lang="ko",
+        translator="google",
+        torch_dtype=torch.float16,
+        device_map="auto",
+        deepl_api=None,
+        bard_api=None,
+        openai_model="gpt-3.5-turbo",
+        openai_api=None
+    ):
+        super().__init__(
+            model_path=model_path,
+            target_lang=target_lang,
+            translator=translator,
+            torch_dtype=torch_dtype,
+            device_map=device_map,
+            deepl_api=deepl_api,
+            bard_api=bard_api,
+            openai_model=openai_model,
+            openai_api=openai_api
+        )
+
+    def inference(self, prompt: str) -> str:
+        # Custom logic for inference
+        # You can override the implementation of the inference method here
+        # and provide your own logic for generating the translated answer
+        # Remember to return the translated answer as a string.
+
+        answer = customizing_process(prompt)
+        # Custom inference logic...
+        
+        return answer
+```
+
+## [FAQs](./documents/FAQs.md)
+Use `Ctrl`+`F` for help in this `FAQs.md`.
 
 ## Contributors
 
 I would like to express my sincere gratitude for the contributions made by all the contributors.
 
 <a href="https://github.com/dsdanielpark/hf-transllm/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=dsdanielpark/hf-transllm" />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transllm Version: 0.1.5 Summary: LLMtranslator
+Metadata-Version: 2.1 Name: transllm Version: 0.1.6 Summary: LLMtranslator
 translates and generates text in multiple languages. Home-page: https://
 github.com/dsdanielpark/hf-transllm Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Science/Research Classifier: Natural
 Language :: English Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
@@ -13,51 +13,77 @@
 License-File: LICENSE Development Status :: 3 - Alpha # Python Package: hf-
 transllm
 [PyPI package] [Code_style:_black] [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-
 transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 [PyPI]
 > LLMtranslator translates and generates text in multiple languages. ![]
-(assets/hf-transllm.png) Through the inference module of Hugging Face, you can
-conveniently use the results of Hugging Face's open-source large language
-model. However, there are limitations in retraining or evaluating the model's
-performance in various languages. Therefore, this package allows you to explore
-the results of the Hugging Face inference module in multiple languages using
-various trnaslated_answer API services. Since the purpose of the Hugging Face
-inference module is more focused on checking the model weights easily rather
-than efficiency, this package emphasizes the ability to explore the results in
-various languages rather than efficiency.
+(assets/transllm.png) ### Introducing hf-transllm: Unlock the Power of
+Multilingual Exploration Discover the hf-transllm package, a seamless
+integration of Hugging Face's inference module and translation APIs. Overcome
+limitations in retraining and evaluating large language models in different
+languages. Explore diverse results effortlessly, leveraging translation API
+services. Emphasizing versatility over efficiency, hf-transllm enables you to
+delve into the outcomes of Hugging Face's models in various languages.
 
-## Install ``` pip install transllm ``` If you wish to use the various features
-and CLI: ``` pip install git+https://github.com/dsdanielpark/hf-transllm.git cd
-hf-transllm python main.py ```
+## Installation ``` pip install transllm ``` Or ``` pip install git+https://
+github.com/dsdanielpark/hf-trnasllm.git ```
+If you wish to use the various features and CLI: ``` pip install git+https://
+github.com/dsdanielpark/hf-transllm.git cd hf-transllm pip install -
+r requirements.txt ``` There can be issues with various dependencies such as
+Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the
+appropriate environment by searching online. ```bash python main.py --hfmodel
+pen_llama_3b> --lang  --translator  ```
 
-## Usage [![Open In Colab](https://colab.research.google.com/assets/colab-
+## Usage Applying LLMs to the majority of Hugging Face repositories is
+generally feasible. However, it can be challenging to apply them to objects
+that require unique tokenizers or inference processes. In such cases, it is
+recommended to customize the usage by incorporating a translation module for
+prompts. In other words, if you are familiar with the inference process or code
+from Hugging Face repositories, you can customize the translation object by
+adding a translation module before and after the known inference process or
+code. [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
-1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) Simple Usage - Google Trnaslator
-```python from transllm import LLMtranslator # Set huggingface repository
-model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-research/
-open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get TransLLM
-Object open_llama3b_kor = LLMtranslator(model_path, target_lang='ko',
+1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) Google Trnaslator - Support
+Languages: https://github.com/ssut/py-googletrans/blob/master/googletrans/
+constants.py ```python from transllm import LLMtranslator # Set huggingface
+repository model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-
+research/open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get
+TransLLM Object open_llama3b_kor = LLMtranslator(model_path, target_lang='ko',
 translator='google') # Using Prompt in multi-language prompt = "ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
 trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
 ```
-- DeepL, OpenAI, Bard ```python from transllm import LLMtranslator # Set
-huggingface repository model_path = 'openlm-research/open_llama_3b' #
-model_path = 'openlm-research/open_llama_7b' # model_path = 'openlm-research/
-open_llama_13b' # Choose Translate Service API: DeepL, OpenAI, Bard
-open_llama3b_kor = LLMtranslator(model_path, target_lang='EN',
-translator='deepl', deepl_api='xxxxxxx') # open_llama3b_kor = LLMtranslator
-(model_path, target_lang='korean', translator='openai', openai_api='xxxxxxx',
-openai_model='gpt-3.5-turbo') # open_llama3b_kor = LLMtranslator(model_path,
-target_lang='korean', translator='bard', bard_api='xxxxxxx') # Using Prompt in
-multi-language prompt = "ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì
-ëí´ì ìë ¤ì¤" trnaslated_answer = open_llama3b_kor.generate(prompt)
-print(trnaslated_answer) ```
+DeepL - Support Languages: https://www.deepl.com/pro/select-country?cta=header-
+pro-button/#developer Open AI, Bard use pre-prompt for translation. ```python
+from transllm import LLMtranslator # Set huggingface repository model_path =
+'openlm-research/open_llama_3b' # model_path = 'openlm-research/open_llama_7b'
+# model_path = 'openlm-research/open_llama_13b' # Choose Translate Service API:
+DeepL, OpenAI, Bard open_llama3b_kor = LLMtranslator(model_path,
+target_lang='EN', translator='deepl', deepl_api='xxxxxxx') # open_llama3b_kor =
+LLMtranslator(model_path, target_lang='korean', translator='openai',
+openai_api='xxxxxxx', openai_model='gpt-3.5-turbo') # open_llama3b_kor =
+LLMtranslator(model_path, target_lang='korean', translator='bard',
+bard_api='xxxxxxx') # Using Prompt in multi-language prompt = "ëì ë´
+ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
+trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
+```
+## Customized Inference ```python import torch from trnasllm import
+LLMtranslator class MyLLMtranslator(LLMtranslator): def __init__( self,
+model_path, target_lang="ko", translator="google", torch_dtype=torch.float16,
+device_map="auto", deepl_api=None, bard_api=None, openai_model="gpt-3.5-turbo",
+openai_api=None ): super().__init__( model_path=model_path,
+target_lang=target_lang, translator=translator, torch_dtype=torch_dtype,
+device_map=device_map, deepl_api=deepl_api, bard_api=bard_api,
+openai_model=openai_model, openai_api=openai_api ) def inference(self, prompt:
+str) -> str: # Custom logic for inference # You can override the implementation
+of the inference method here # and provide your own logic for generating the
+translated answer # Remember to return the translated answer as a string.
+answer = customizing_process(prompt) # Custom inference logic... return answer
+``` ## [FAQs](./documents/FAQs.md) Use `Ctrl`+`F` for help in this `FAQs.md`.
 ## Contributors I would like to express my sincere gratitude for the
 contributions made by all the contributors. [https://contrib.rocks/
 image?repo=dsdanielpark/hf-transllm]
 ## License [MIT](https://opensource.org/license/mit/)
 I hold no legal responsibility; ``` The MIT License (MIT) Copyright (c) 2023
 Minwoo Park Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `transllm-0.1.5/setup.py` & `transllm-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="transllm",
-    version="0.1.5",
+    version="0.1.6",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="LLMtranslator translates and generates text in multiple languages.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/hf-transllm",
     packages=find_packages(exclude=[]),
@@ -42,15 +42,16 @@
         "torch",
         "deepl",
         "transformers",
         "googletrans",
         "bardapi",
         "openai",
         "sentencepiece",
-        "accelerate"
+        "accelerate",
+        "translang"
     ],
     keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
```

### Comparing `transllm-0.1.5/transllm.egg-info/PKG-INFO` & `transllm-0.1.6/transllm.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.5
+Version: 0.1.6
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -30,50 +30,59 @@
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
 <a href="https://pypi.org/project/transllm/"><img alt="PyPI" src="https://img.shields.io/pypi/v/transllm"></a>
 </p>
 
 
 > LLMtranslator translates and generates text in multiple languages.
 
-![](assets/hf-transllm.png)
+![](assets/transllm.png)
 
-Through the inference module of Hugging Face, you can conveniently use the results of Hugging Face's open-source large language model. However, there are limitations in retraining or evaluating the model's performance in various languages.
+### Introducing hf-transllm: Unlock the Power of Multilingual Exploration
 
-Therefore, this package allows you to explore the results of the Hugging Face inference module in multiple languages using various trnaslated_answer API services.
-
-Since the purpose of the Hugging Face inference module is more focused on checking the model weights easily rather than efficiency, this package emphasizes the ability to explore the results in various languages rather than efficiency.
+Discover the hf-transllm package, a seamless integration of Hugging Face's inference module and translation APIs. Overcome limitations in retraining and evaluating large language models in different languages. Explore diverse results effortlessly, leveraging translation API services. Emphasizing versatility over efficiency, hf-transllm enables you to delve into the outcomes of Hugging Face's models in various languages.
 
 
 <br>
 
 
 <br>
 
-## Install
+## Installation
 ```
 pip install transllm
 ```
+Or
+```
+pip install git+https://github.com/dsdanielpark/hf-trnasllm.git
+```
+
+<br>
 
 If you wish to use the various features and CLI:
 ```
 pip install git+https://github.com/dsdanielpark/hf-transllm.git
 cd hf-transllm
-python main.py
+pip install -r requirements.txt
+```
+There can be issues with various dependencies such as Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the appropriate environment by searching online.
+```bash
+python main.py --hfmodel <openlm-research/open_llama_3b> --lang <ko> --translator <google>
 ```
-
 <br>
 
 <br>
 
 ## Usage 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
+Applying LLMs to the majority of Hugging Face repositories is generally feasible. However, it can be challenging to apply them to objects that require unique tokenizers or inference processes. In such cases, it is recommended to customize the usage by incorporating a translation module for prompts.
 
-Simple Usage
+In other words, if you are familiar with the inference process or code from Hugging Face repositories, you can customize the translation object by adding a translation module before and after the known inference process or code.
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
 
-- Google Trnaslator
+Google Trnaslator
+- Support Languages: https://github.com/ssut/py-googletrans/blob/master/googletrans/constants.py
 ```python
 from transllm import LLMtranslator
 
 # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b'
 # model_path = 'openlm-research/open_llama_7b'
 # model_path = 'openlm-research/open_llama_13b'
@@ -85,15 +94,18 @@
 prompt = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 trnaslated_answer = open_llama3b_kor.generate(prompt)
 print(trnaslated_answer)
 ```
 
 <br>
 
-- DeepL, OpenAI, Bard
+DeepL
+- Support Languages: https://www.deepl.com/pro/select-country?cta=header-pro-button/#developer
+
+Open AI, Bard use pre-prompt for translation.
 ```python
 from transllm import LLMtranslator
 
 # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b'
 # model_path = 'openlm-research/open_llama_7b'
 # model_path = 'openlm-research/open_llama_13b'
@@ -107,14 +119,59 @@
 prompt = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 trnaslated_answer = open_llama3b_kor.generate(prompt)
 print(trnaslated_answer)
 ```
 
 <br>
 
+## Customized Inference
+```python
+import torch
+from trnasllm import LLMtranslator
+
+
+class MyLLMtranslator(LLMtranslator):
+    def __init__(
+        self,
+        model_path,
+        target_lang="ko",
+        translator="google",
+        torch_dtype=torch.float16,
+        device_map="auto",
+        deepl_api=None,
+        bard_api=None,
+        openai_model="gpt-3.5-turbo",
+        openai_api=None
+    ):
+        super().__init__(
+            model_path=model_path,
+            target_lang=target_lang,
+            translator=translator,
+            torch_dtype=torch_dtype,
+            device_map=device_map,
+            deepl_api=deepl_api,
+            bard_api=bard_api,
+            openai_model=openai_model,
+            openai_api=openai_api
+        )
+
+    def inference(self, prompt: str) -> str:
+        # Custom logic for inference
+        # You can override the implementation of the inference method here
+        # and provide your own logic for generating the translated answer
+        # Remember to return the translated answer as a string.
+
+        answer = customizing_process(prompt)
+        # Custom inference logic...
+        
+        return answer
+```
+
+## [FAQs](./documents/FAQs.md)
+Use `Ctrl`+`F` for help in this `FAQs.md`.
 
 ## Contributors
 
 I would like to express my sincere gratitude for the contributions made by all the contributors.
 
 <a href="https://github.com/dsdanielpark/hf-transllm/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=dsdanielpark/hf-transllm" />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transllm Version: 0.1.5 Summary: LLMtranslator
+Metadata-Version: 2.1 Name: transllm Version: 0.1.6 Summary: LLMtranslator
 translates and generates text in multiple languages. Home-page: https://
 github.com/dsdanielpark/hf-transllm Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Science/Research Classifier: Natural
 Language :: English Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
@@ -13,51 +13,77 @@
 License-File: LICENSE Development Status :: 3 - Alpha # Python Package: hf-
 transllm
 [PyPI package] [Code_style:_black] [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-
 transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 [PyPI]
 > LLMtranslator translates and generates text in multiple languages. ![]
-(assets/hf-transllm.png) Through the inference module of Hugging Face, you can
-conveniently use the results of Hugging Face's open-source large language
-model. However, there are limitations in retraining or evaluating the model's
-performance in various languages. Therefore, this package allows you to explore
-the results of the Hugging Face inference module in multiple languages using
-various trnaslated_answer API services. Since the purpose of the Hugging Face
-inference module is more focused on checking the model weights easily rather
-than efficiency, this package emphasizes the ability to explore the results in
-various languages rather than efficiency.
+(assets/transllm.png) ### Introducing hf-transllm: Unlock the Power of
+Multilingual Exploration Discover the hf-transllm package, a seamless
+integration of Hugging Face's inference module and translation APIs. Overcome
+limitations in retraining and evaluating large language models in different
+languages. Explore diverse results effortlessly, leveraging translation API
+services. Emphasizing versatility over efficiency, hf-transllm enables you to
+delve into the outcomes of Hugging Face's models in various languages.
 
-## Install ``` pip install transllm ``` If you wish to use the various features
-and CLI: ``` pip install git+https://github.com/dsdanielpark/hf-transllm.git cd
-hf-transllm python main.py ```
+## Installation ``` pip install transllm ``` Or ``` pip install git+https://
+github.com/dsdanielpark/hf-trnasllm.git ```
+If you wish to use the various features and CLI: ``` pip install git+https://
+github.com/dsdanielpark/hf-transllm.git cd hf-transllm pip install -
+r requirements.txt ``` There can be issues with various dependencies such as
+Hugging Face's Transformers, SentencePiece, Torch, and CUDA. Please set up the
+appropriate environment by searching online. ```bash python main.py --hfmodel
+pen_llama_3b> --lang  --translator  ```
 
-## Usage [![Open In Colab](https://colab.research.google.com/assets/colab-
+## Usage Applying LLMs to the majority of Hugging Face repositories is
+generally feasible. However, it can be challenging to apply them to objects
+that require unique tokenizers or inference processes. In such cases, it is
+recommended to customize the usage by incorporating a translation module for
+prompts. In other words, if you are familiar with the inference process or code
+from Hugging Face repositories, you can customize the translation object by
+adding a translation module before and after the known inference process or
+code. [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
-1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) Simple Usage - Google Trnaslator
-```python from transllm import LLMtranslator # Set huggingface repository
-model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-research/
-open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get TransLLM
-Object open_llama3b_kor = LLMtranslator(model_path, target_lang='ko',
+1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) Google Trnaslator - Support
+Languages: https://github.com/ssut/py-googletrans/blob/master/googletrans/
+constants.py ```python from transllm import LLMtranslator # Set huggingface
+repository model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-
+research/open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get
+TransLLM Object open_llama3b_kor = LLMtranslator(model_path, target_lang='ko',
 translator='google') # Using Prompt in multi-language prompt = "ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
 trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
 ```
-- DeepL, OpenAI, Bard ```python from transllm import LLMtranslator # Set
-huggingface repository model_path = 'openlm-research/open_llama_3b' #
-model_path = 'openlm-research/open_llama_7b' # model_path = 'openlm-research/
-open_llama_13b' # Choose Translate Service API: DeepL, OpenAI, Bard
-open_llama3b_kor = LLMtranslator(model_path, target_lang='EN',
-translator='deepl', deepl_api='xxxxxxx') # open_llama3b_kor = LLMtranslator
-(model_path, target_lang='korean', translator='openai', openai_api='xxxxxxx',
-openai_model='gpt-3.5-turbo') # open_llama3b_kor = LLMtranslator(model_path,
-target_lang='korean', translator='bard', bard_api='xxxxxxx') # Using Prompt in
-multi-language prompt = "ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì
-ëí´ì ìë ¤ì¤" trnaslated_answer = open_llama3b_kor.generate(prompt)
-print(trnaslated_answer) ```
+DeepL - Support Languages: https://www.deepl.com/pro/select-country?cta=header-
+pro-button/#developer Open AI, Bard use pre-prompt for translation. ```python
+from transllm import LLMtranslator # Set huggingface repository model_path =
+'openlm-research/open_llama_3b' # model_path = 'openlm-research/open_llama_7b'
+# model_path = 'openlm-research/open_llama_13b' # Choose Translate Service API:
+DeepL, OpenAI, Bard open_llama3b_kor = LLMtranslator(model_path,
+target_lang='EN', translator='deepl', deepl_api='xxxxxxx') # open_llama3b_kor =
+LLMtranslator(model_path, target_lang='korean', translator='openai',
+openai_api='xxxxxxx', openai_model='gpt-3.5-turbo') # open_llama3b_kor =
+LLMtranslator(model_path, target_lang='korean', translator='bard',
+bard_api='xxxxxxx') # Using Prompt in multi-language prompt = "ëì ë´
+ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
+trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
+```
+## Customized Inference ```python import torch from trnasllm import
+LLMtranslator class MyLLMtranslator(LLMtranslator): def __init__( self,
+model_path, target_lang="ko", translator="google", torch_dtype=torch.float16,
+device_map="auto", deepl_api=None, bard_api=None, openai_model="gpt-3.5-turbo",
+openai_api=None ): super().__init__( model_path=model_path,
+target_lang=target_lang, translator=translator, torch_dtype=torch_dtype,
+device_map=device_map, deepl_api=deepl_api, bard_api=bard_api,
+openai_model=openai_model, openai_api=openai_api ) def inference(self, prompt:
+str) -> str: # Custom logic for inference # You can override the implementation
+of the inference method here # and provide your own logic for generating the
+translated answer # Remember to return the translated answer as a string.
+answer = customizing_process(prompt) # Custom inference logic... return answer
+``` ## [FAQs](./documents/FAQs.md) Use `Ctrl`+`F` for help in this `FAQs.md`.
 ## Contributors I would like to express my sincere gratitude for the
 contributions made by all the contributors. [https://contrib.rocks/
 image?repo=dsdanielpark/hf-transllm]
 ## License [MIT](https://opensource.org/license/mit/)
 I hold no legal responsibility; ``` The MIT License (MIT) Copyright (c) 2023
 Minwoo Park Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

