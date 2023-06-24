# Comparing `tmp/LLM-Toolbox-0.0.2.tar.gz` & `tmp/LLM-Toolbox-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLM-Toolbox-0.0.2.tar", last modified: Sun Jun 18 19:23:17 2023, max compression
+gzip compressed data, was "LLM-Toolbox-0.1.0.tar", last modified: Sat Jun 24 03:24:00 2023, max compression
```

## Comparing `LLM-Toolbox-0.0.2.tar` & `LLM-Toolbox-0.1.0.tar`

### file list

```diff
@@ -1,53 +1,32 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.0.2/LICENSE
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11013 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1547 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      670 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1026 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11013 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10475 2023-06-18 18:54:17.000000 LLM-Toolbox-0.0.2/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/llm_toolbox/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10678 2023-06-18 19:17:13.000000 LLM-Toolbox-0.0.2/llm_toolbox/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/llm_toolbox/tools/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/common.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      368 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/cheermeup.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      594 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/codereview.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      854 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/commitgen.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      576 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/critique.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      270 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/define.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      332 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/explain.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      748 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/lessonize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      533 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/pathlearner.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      423 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/proofread.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      453 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/study.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      393 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/summarize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      818 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/teachlib.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      248 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/thesaurus.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      364 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/translate.yaml
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/llm_toolbox/tools/user_defined/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/user_defined/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/user_defined/example_tool.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/prompt_templates/
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/prompt_templates/tools/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      368 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/cheermeup.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      594 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/codereview.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      854 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/commitgen.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      576 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/critique.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      270 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/define.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      332 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/explain.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      748 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/lessonize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      533 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/pathlearner.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      423 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/proofread.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      453 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/study.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      393 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/summarize.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      818 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/teachlib.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      248 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/thesaurus.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      364 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/translate.yaml
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2924 2023-06-18 19:21:47.000000 LLM-Toolbox-0.0.2/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 03:24:00.386939 LLM-Toolbox-0.1.0/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.1.0/LICENSE
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 03:24:00.376939 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15779 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      875 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      674 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       88 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-24 03:24:00.000000 LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15779 2023-06-24 03:24:00.386939 LLM-Toolbox-0.1.0/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15241 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 03:24:00.376939 LLM-Toolbox-0.1.0/llm_toolbox/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.1.0/llm_toolbox/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    12492 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 03:24:00.376939 LLM-Toolbox-0.1.0/llm_toolbox/tools/
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 03:24:00.386939 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      367 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/cheermeup.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      593 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/codereview.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      853 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/commitgen.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1372 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/critique.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      269 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/define.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      331 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/explain.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      747 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/lessonize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      532 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/pathlearner.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      422 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/proofread.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      452 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/study.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      424 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/summarize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      817 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/teachlib.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      247 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/thesaurus.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      363 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/translate.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-24 03:24:00.386939 LLM-Toolbox-0.1.0/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2915 2023-06-24 03:22:18.000000 LLM-Toolbox-0.1.0/setup.py
```

### Comparing `LLM-Toolbox-0.0.2/LICENSE` & `LLM-Toolbox-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/PKG-INFO` & `LLM-Toolbox-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-Metadata-Version: 2.1
-Name: LLM-Toolbox
-Version: 0.0.2
-Summary: A versatile collection of CLI tools leveraging large language models
-Home-page: https://github.com/sderev/llm-toolbox
-Author: Sébastien De Revière
-License: Apache Licence, Version 2.0
-Project-URL: Documentation, https://github.com/sderev/llm-toolbox
-Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
-Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # LLM-Toolbox
 
-LLM-Toolbox is a collection of command-line tools that harness the power of large language models to perform various tasks. This repository houses scripts and tools that utilize OpenAI's ChatGPT for tasks such as automatic commit messages, dictionary and thesaurus queries, text translation, proofreading, enriching language learning, automating shell commands, and more.
+**Development Status**: 
+
+LLM-Toolbox is currently under active development. Your feedback is crucial for this ongoing journey of refinement. Please share your thoughts, experiences, and suggestions. If you find this project beneficial, consider expression your support by giving it a star ⭐😊.
+
+---
 
-Additionally, the toolbox provides a selection of [prompt templates](#prompt-templates) to help you get the most out of your interactions with the language models. Whether you're new to scripting with language models or an experienced developer, these templates can serve as an invaluable resource.
+LLM-Toolbox is an ensemble of AI-powered command-line tools designed to modernize your workflow in the terminal. Built using OpenAI's ChatGPT, the tools in this toolbox can generate automatic commit messages, perform dictionary and thesaurus quesries, translate text, proofread content, enrich language learning, and automate shell commands, among others.
 
-Given the wide-ranging capabilities of the LLM-Toolbox, it can be helpful to see it in action first. Therefore, I strongly suggest you check out the video demos of the tools to gain a hands-on understanding of their potential. After viewing the demos, you can return here for a deeper dive into the specific applications and benefits. So, go ahead, watch the demos! 😊
+Additionally, the toolbox provides an array of [prompt templates](#prompt-templates) that can serve as a valuable resource, whether you're new to using languages models or you're an experienced user.
+
+I've created video demos to help you see the LLM-Toolbox in action and understand its wide-ranging capabilities. Therefore, I strongly recommend you check out the video demos of the tools to gain a hands-on understanding of their potential. After watching the demos, you can return here for a deeper dive into the specific applications and benefits. So, go ahead, watch the demos! 😊
 
 <!-- TOC -->
 ## Table of Contents
 
 1. [Prompt Templates](#prompt-templates)
 1. [Isn't the OpenAI API expensive?](#isnt-the-openai-api-expensive)
 1. [The Value of Investing in LLM-Toolbox](#the-value-of-investing-in-llm-toolbox)
@@ -32,52 +24,64 @@
     1. [pip](#pip)
     1. [`pipx`, the Easy Way](#pipx-the-easy-way)
     1. [Installing the LLM-Toolbox](#installing-the-llm-toolbox)
     1. [Cloning the LLM-Toolbox Repository](#cloning-the-llm-toolbox-repository)
 1. [Getting Started](#getting-started)
     1. [Set your OpenAI API key](#set-your-openai-api-key)
 1. [Tools](#tools)
+    1. [LMT](#lmt)
     1. [ShellGenius](#shellgenius)
+    1. [Commitgen](#commitgen)
+    1. [Codereview](#codereview)
     1. [VocabMaster](#vocabmaster)
     1. [Thesaurus](#thesaurus)
     1. [Define](#define)
     1. [Proofread](#proofread)
     1. [Translate](#translate)
-1. [Prompt Templates](#prompt-templates)
+    1. [Cheermeup](#cheermeup)
+    1. [Critique](#critique)
+    1. [Explain](#explain)
+    1. [Lessonize](#lessonize)
+    1. [Pathlearner](#pathlearner)
+    1. [Study](#study)
+    1. [Summarize](#summarize)
+    1. [Teachlib](#teachlib)
 1. [License](#license)
 <!-- /TOC -->
 
-## Prompt Templates
+## Prompt Templates 
+
+If you're less familiar with terminal interfaces, or if you simply prefer the convenience of a web interface, you'll find our [ChatGPT web interface templates](https://github.com/sderev/llm-toolbox/prompt-templates) quite helpful. Particularly for longer chat interactions with GPT-4, the web interface is advantageous, although it does necessitate a ChatGPT Plus subscription.
 
-If you're not a terminal-centric person, or if you prefer the web interface anyway, note that I prepared [templates for ChatGPT web interface](https://github.com/sderev/llm-toolbox/prompt-templates).
+The LLM-Toolbox goes beyond just tools; it also offers a comprehensive collection of prompt templates located in the [`prompt-templates/`](https://github.com/sderev/llm-toolbox/tree/main/prompt-templates) directory. These templates cater to a broad range of situations and are crafted to enhance your engagement with language models. If you're unsure about prompt structuring or want to boost the efficacy of your existing prompts, these templates serve as a great starting point.
 
-It's better to use the web interface if you plan on having very long chat interactions with GPT-4 (requires a ChatGPT Plus subscription, though). Otherwise it will cost you too much.
+You're encouraged to browse these templates and modify them to fit your unique requirements.
 
 ## Isn't the OpenAI API expensive?
 
-A lot of people are afraid that these tools will cost them too much. But the truth is, as long as you're not sending too many requests to GPT-4, you won't have exorbitant bills. On the contrary, this may surprise you, but I'm pretty confident that the majority of people won't exceed a cost of $3 per month, as long as they continue to use GPT-3.5, even if they use these tools more than a hundred times a day.
+A lot of people are afraid that these tools will cost them too much. But the truth is, as long as you're not sending too many requests to GPT-4, you won't have exorbitant bills. On the contrary, this may surprise you, but I'm pretty confident that the majority of people won't exceed a cost of $3 to $5 per month, as long as they continue to use GPT-3.5, even if they use these tools more than a hundred times a day.
 
 Also, there's a safeguard: **you can configure a soft and a hard usage limit on your OpenAI account**. This ensures that you won't ever be taken by surprise.
 
 * Soft limit: You receive a notification email.
 * Hard limit: Subsequent requests will be rejected.
 
 ## The Value of Investing in LLM-Toolbox
 
 Well... in giving your money to OpenAI, actually.
 
-Even if you have a monthly expense of more than a dollar, it's well worth looking at looking at the huge benefits you'll receive from utilizing the tools in the LLM-Toolbox. These innovative solutions provide users with powerful capabilities that can **significantly streamline tasks, improve productivity, and foster creativity**.
+Even if you have a monthly expense of more than a dollar, it's well worth looking at the huge benefits you'll receive from utilizing the tools in the LLM-Toolbox. These innovative solutions provide users with powerful capabilities that can **significantly streamline tasks, improve productivity, and foster creativity**.
 
-Particularly, let's consider [ShellGenius](#shellgenius), a remarkable tool within the LLM-Toolbox. It enhances the command-line experience by translating task descriptions into efficient shell commands, a feat that not only saves time but also reduces the possibility of human error. This tool is extremely beneficial for both beginners, who may not be fluent in shell commands, and experienced users who can streamline their command-line tasks by simply describing what they wish to accomplish, and [ShellGenius](#shellgenius) provides the correct shell command to achieve it.
+Particularly, let's consider [ShellGenius](#shellgenius), a remarkable tool within the LLM-Toolbox. It enhances the command-line experience by translating task descriptions into efficient shell commands, a feat that not only saves time but also reduces the possibility of human error. This tool is extremely beneficial for both beginners, who may not be fluent in shell commands, and experienced users who can streamline their command-line tasks by simply describing what they wish to accomplish.
 
 Therefore, when considering the cost, it's essential to look beyond the immediate dollar value and evaluate the considerable time, effort, and resources you stand to save. The utility and value derived from such tools often outweigh the minimal monthly cost. The price of these tools should not be a deterrent but rather seen as an investment in enhancing your efficiency and productivity.
 
 ### Is GPT-3.5 Sufficient for Those Tools?
 
-GPT-3.5 is an excellent model for these tools, offering cost-effective solution that consistently delivers appropriate responses. I take great care in crafting my prompts and the tools to generate the best results that cater to my daily needs.
+GPT-3.5 is an excellent model for these tools, offering a cost-effective solution that consistently delivers appropriate responses. I take great care in crafting my prompts and the tools to generate the best results that cater to my own daily needs.
 
 I will continue refining them, if necessary, as time goes on. So stay tuned to this repo and consider giving it a star ⭐!
 
 You'll also be able to update the LLM-Toolbox directly from the CLI 😊.
 
 ### Current Costs
 
@@ -96,15 +100,15 @@
 
 ```bash
 python3 -m pip install llm-toolbox
 ```
 
 ### `pipx`, the Easy Way
 
-To use these tools, I recommend that you first install [pipx](https://pypa.github.io/pipx/installation/). It's a package manager for Python that makes the installation and upgrade of CLI apps easy (no more hassle with virtual environment 😌).
+To use these tools, I recommend that you first install [pipx](https://pypa.github.io/pipx/installation/). It's a package manager for Python that makes the installation and upgrade of CLI apps easy (no more hassle with virtual environments 😌).
 
 * Debian / Ubuntu
 
     ```bash
     sudo apt install pipx
     ```
 
@@ -178,65 +182,130 @@
   setx OPENAI_API_KEY your_key
   ```
 
 ## Tools
 
 Instructions on how to use each of the tools are included in the individual directories under [tools/](https://github.com/sderev/llm-toolbox/tree/main/tools). This is also where I give some tricks and tips on their usage 💡👀💭.
 
-Here's a brief overview:
+Note that LMT is the main tool in the LLM-Toolbox. All of its options apply to (almost) all of the other tools. For instance, you change the model to GPT-4 with `-m 4` or add emojis with `--emoji`. Refer to the [LMT's documentation](https://github.com/sderev/lmt) for more information. 
+
+* **Reading from `stdin`**: Almost all of the tools can read from `stdin`. For instance: `cat my_text.md | summarize`.
+
+* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique --raw > critique_of_my_text.md`
+
+Here's a brief overview of the tools:
+
+### LMT
+
+[LMT](https://github.com/sderev/lmt) empowers you to interact directly with ChatGPT from the comfort of your terminal. One of the core features of `lmt` is its ability to facilitate the creation of custom templates, enabling you to design your personalized toolbox of CLI applications. You can easily install its standalone version from [the project's repository](https://github.com/sderev/lmt).
 
 ### ShellGenius
 
 [ShellGenius](https://github.com/sderev/shellgenius) is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands. Check out the project on [its dedicated repository](https://github.com/sderev/shellgenius).
 
 ![shellgenius](https://github.com/sderev/llm-toolbox/assets/24412384/688d9a1a-f351-42d0-9f4d-06a9a6d1909a)
 
+### Commitgen
+
+The [`commitgen`](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen) tool is designed to streamline your `git` workflow by automatically generating meaningful commit messages for your code changes.
+
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/d41985d5-d8a2-4622-9ef7-643176cdc741)
+___
+
+### Codereview
+
+The [`Codereview`](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview) tool accepts a file or a piece of text as input and provides an in-depth analysis of the code. It can identify potential issues, suggest improvements, and even detect security vulnerabilities. The Codereview tool is capable of handling a variety of programming languages, and its feedback can serve as an invaluable resource for developers seeking to enhance the quality of their code. 
+
 ___
 
 ### VocabMaster
 
 Master new languages with [VocabMaster](https://github.com/sderev/vocabmaster), a CLI tool designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience. Check out the project on [its dedicated repository](https://github.com/sderev/vocabmaster).
 
 ![vocabmaster_translate_japanese](https://github.com/sderev/llm-toolbox/assets/24412384/5f5612fe-f1fb-4d4c-bb25-68f07961e66b)
 
 ___
 
 ### Thesaurus
 
-The [`thesaurus`](https://github.com/sderev/llm-toolbox/tree/main/tools/thesaurus) script takes a word or a phrase as input and provides a list of synonyms and antonyms.
+The [`thesaurus`](https://github.com/sderev/llm-toolbox/tree/main/tools/thesaurus) tool takes a word or a phrase as input and provides a list of synonyms and antonyms.
 
 ![thesaurus](https://github.com/sderev/llm-toolbox/assets/24412384/dca6bf42-2545-4b56-bb20-4c8e6c872529)
 
 ___
 
 ### Define
 
-The [`define`](https://github.com/sderev/llm-toolbox/tree/main/tools/define) script takes a word as input and provides its definition along with an example sentence using the word.
+The [`define`](https://github.com/sderev/llm-toolbox/tree/main/tools/define) tool takes a word as input and provides its definition along with an example sentence using the word.
 
 ![define](https://github.com/sderev/llm-toolbox/assets/24412384/1e813b80-6896-483b-b31a-65ad7cb81173)
 
 ___
 
 ### Proofread
 
-The [`proofread`](https://github.com/sderev/llm-toolbox/tree/main/tools/proofread) script takes a sentence as input and provides a corrected version of it, if needed, along with an explanation of the corrections.
+The [`proofread`](https://github.com/sderev/llm-toolbox/tree/main/tools/proofread) tool takes a sentence as input and provides a corrected version of it, if needed, along with an explanation of the corrections.
 
 ![proofread_english](https://github.com/sderev/llm-toolbox/assets/24412384/e84ce7cd-68e9-4d6d-8c56-55b93c7e4fee)
 
 ___
 
 ### Translate
 
-The [`translate`](https://github.com/sderev/llm-toolbox/tree/main/tools/translate) script takes a sentence and a target language as input and provides the translated sentence in the target language.
+The [`translate`](https://github.com/sderev/llm-toolbox/tree/main/tools/translate) tool takes a sentence and a target language as input and provides the translated sentence in the target language.
 
 ![translate](https://github.com/sderev/llm-toolbox/assets/24412384/505237c9-7735-4db6-aa4a-63c3ed2867a7)
 
-## Prompt Templates
+___
+
+### Cheermeup
+
+The [`cheermeup`](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup) tool is designed to uplift your spirits based on your current mood. Whether you're feeling down or just need a little pick-me-up, this tool uses a variety of methods to bring a smile to your face and brighten your day.
+
+___
+
+### Critique
+
+The [`critique`](https://github.com/sderev/llm-toolbox/tree/main/tools/critique) tool is your personal constructive text critic, designed to analyze a given piece of text and provide detailed, insightful feedback. It enables users to enhance their writing by addressing potential shortcomings and improving the overall quality.
 
-In addition to the various tools provided, the LLM-Toolbox includes a collection of prompt templates in the [`prompts/`](https://github.com/sderev/llm-toolbox/tree/main/prompts) directory. These templates cover a wide range of scenarios and are designed to optimize your interaction with language models. They are an excellent starting point if you're not sure how to structure your prompts or if you're seeking to improve the effectiveness of your current prompts.
+___
+
+### Explain
+
+The [`explain`](https://github.com/sderev/llm-toolbox/tree/main/tools/explain) tool helps to clarify complex concepts. When given a concept, it presents a comprehensive and straightforward explanation, aiding in understanding and knowledge retention.
+
+___
+
+### Lessonize
+
+The [`lessonize`](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize) tool transforms any piece of text into an informative lesson. Whether you're a teacher looking for instructional material or a student looking to further understand a subject, this tool makes learning more accessible.
+
+___
+
+### Pathlearner
+
+The [`pathlearner`](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner) tool provides a comprehensive study plan for a given topic. Whether you're studying for an exam or learning a new subject, this tool creates a structured, step-by-step plan that aids in understanding and mastering the material.
+
+___
+
+### Study
+
+The [`study`](https://github.com/sderev/llm-toolbox/tree/main/tools/study) tool is a comprehensive guide that generates study material for a particular topic or content. It helps students to better prepare for exams, giving them access to tailored study material designed to enhance their learning experience.
+
+___
+
+### Summarize
 
-Please feel free to explore these templates and adapt them to suit your specific needs.
+The [`summarize`](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize) tool provides succinct summaries of a web page, lengthy texts, or the content of given files. It's perfect for extracting key points and crucial information from vast amounts of data, saving users time and effort.
+
+___
+
+### Teachlib
+
+The [`teachlib`](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib) tool is designed to provide comprehensive lessons on various libraries. By simplifying complex aspects and focusing on the core functionalities, this tool helps users to understand and effectively utilize different libraries.
+
+___
 
 ## License
 
 This project is licensed under the terms of the Apache License 2.0.
```

### Comparing `LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/entry_points.txt` & `LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/entry_points.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 cheermeup = llm_toolbox.cli:cheermeup
 codereview = llm_toolbox.cli:codereview
 commitgen = llm_toolbox.cli:commitgen
 critique = llm_toolbox.cli:critique
 define = llm_toolbox.cli:define
 explain = llm_toolbox.cli:explain
 lessonize = llm_toolbox.cli:lessonize
-llm = llm.cli:cli
 llm-toolbox = llm_toolbox.cli:cli
+lmt = lmt_cli.cli:lmt
 pathlearner = llm_toolbox.cli:pathlearner
 proofread = llm_toolbox.cli:proofread
 shellgenius = shellgenius.cli:shellgenius
 study = llm_toolbox.cli:study
 summarize = llm_toolbox.cli:summarize
 teachlib = llm_toolbox.cli:teachlib
 thesaurus = llm_toolbox.cli:thesaurus
```

### Comparing `LLM-Toolbox-0.0.2/PKG-INFO` & `LLM-Toolbox-0.1.0/LLM_Toolbox.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: LLM-Toolbox
-Version: 0.0.2
+Version: 0.1.0
 Summary: A versatile collection of CLI tools leveraging large language models
 Home-page: https://github.com/sderev/llm-toolbox
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/llm-toolbox
 Project-URL: Issues, http://github.com/sderev/llm-toolbox/issues
 Project-URL: Changelog, https://github.com/sderev/llm-toolbox/releases
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LLM-Toolbox
 
-LLM-Toolbox is a collection of command-line tools that harness the power of large language models to perform various tasks. This repository houses scripts and tools that utilize OpenAI's ChatGPT for tasks such as automatic commit messages, dictionary and thesaurus queries, text translation, proofreading, enriching language learning, automating shell commands, and more.
+**Development Status**: 
 
-Additionally, the toolbox provides a selection of [prompt templates](#prompt-templates) to help you get the most out of your interactions with the language models. Whether you're new to scripting with language models or an experienced developer, these templates can serve as an invaluable resource.
+LLM-Toolbox is currently under active development. Your feedback is crucial for this ongoing journey of refinement. Please share your thoughts, experiences, and suggestions. If you find this project beneficial, consider expression your support by giving it a star ⭐😊.
 
-Given the wide-ranging capabilities of the LLM-Toolbox, it can be helpful to see it in action first. Therefore, I strongly suggest you check out the video demos of the tools to gain a hands-on understanding of their potential. After viewing the demos, you can return here for a deeper dive into the specific applications and benefits. So, go ahead, watch the demos! 😊
+---
+
+LLM-Toolbox is an ensemble of AI-powered command-line tools designed to modernize your workflow in the terminal. Built using OpenAI's ChatGPT, the tools in this toolbox can generate automatic commit messages, perform dictionary and thesaurus quesries, translate text, proofread content, enrich language learning, and automate shell commands, among others.
+
+Additionally, the toolbox provides an array of [prompt templates](#prompt-templates) that can serve as a valuable resource, whether you're new to using languages models or you're an experienced user.
+
+I've created video demos to help you see the LLM-Toolbox in action and understand its wide-ranging capabilities. Therefore, I strongly recommend you check out the video demos of the tools to gain a hands-on understanding of their potential. After watching the demos, you can return here for a deeper dive into the specific applications and benefits. So, go ahead, watch the demos! 😊
 
 <!-- TOC -->
 ## Table of Contents
 
 1. [Prompt Templates](#prompt-templates)
 1. [Isn't the OpenAI API expensive?](#isnt-the-openai-api-expensive)
 1. [The Value of Investing in LLM-Toolbox](#the-value-of-investing-in-llm-toolbox)
@@ -32,52 +38,64 @@
     1. [pip](#pip)
     1. [`pipx`, the Easy Way](#pipx-the-easy-way)
     1. [Installing the LLM-Toolbox](#installing-the-llm-toolbox)
     1. [Cloning the LLM-Toolbox Repository](#cloning-the-llm-toolbox-repository)
 1. [Getting Started](#getting-started)
     1. [Set your OpenAI API key](#set-your-openai-api-key)
 1. [Tools](#tools)
+    1. [LMT](#lmt)
     1. [ShellGenius](#shellgenius)
+    1. [Commitgen](#commitgen)
+    1. [Codereview](#codereview)
     1. [VocabMaster](#vocabmaster)
     1. [Thesaurus](#thesaurus)
     1. [Define](#define)
     1. [Proofread](#proofread)
     1. [Translate](#translate)
-1. [Prompt Templates](#prompt-templates)
+    1. [Cheermeup](#cheermeup)
+    1. [Critique](#critique)
+    1. [Explain](#explain)
+    1. [Lessonize](#lessonize)
+    1. [Pathlearner](#pathlearner)
+    1. [Study](#study)
+    1. [Summarize](#summarize)
+    1. [Teachlib](#teachlib)
 1. [License](#license)
 <!-- /TOC -->
 
-## Prompt Templates
+## Prompt Templates 
+
+If you're less familiar with terminal interfaces, or if you simply prefer the convenience of a web interface, you'll find our [ChatGPT web interface templates](https://github.com/sderev/llm-toolbox/prompt-templates) quite helpful. Particularly for longer chat interactions with GPT-4, the web interface is advantageous, although it does necessitate a ChatGPT Plus subscription.
 
-If you're not a terminal-centric person, or if you prefer the web interface anyway, note that I prepared [templates for ChatGPT web interface](https://github.com/sderev/llm-toolbox/prompt-templates).
+The LLM-Toolbox goes beyond just tools; it also offers a comprehensive collection of prompt templates located in the [`prompt-templates/`](https://github.com/sderev/llm-toolbox/tree/main/prompt-templates) directory. These templates cater to a broad range of situations and are crafted to enhance your engagement with language models. If you're unsure about prompt structuring or want to boost the efficacy of your existing prompts, these templates serve as a great starting point.
 
-It's better to use the web interface if you plan on having very long chat interactions with GPT-4 (requires a ChatGPT Plus subscription, though). Otherwise it will cost you too much.
+You're encouraged to browse these templates and modify them to fit your unique requirements.
 
 ## Isn't the OpenAI API expensive?
 
-A lot of people are afraid that these tools will cost them too much. But the truth is, as long as you're not sending too many requests to GPT-4, you won't have exorbitant bills. On the contrary, this may surprise you, but I'm pretty confident that the majority of people won't exceed a cost of $3 per month, as long as they continue to use GPT-3.5, even if they use these tools more than a hundred times a day.
+A lot of people are afraid that these tools will cost them too much. But the truth is, as long as you're not sending too many requests to GPT-4, you won't have exorbitant bills. On the contrary, this may surprise you, but I'm pretty confident that the majority of people won't exceed a cost of $3 to $5 per month, as long as they continue to use GPT-3.5, even if they use these tools more than a hundred times a day.
 
 Also, there's a safeguard: **you can configure a soft and a hard usage limit on your OpenAI account**. This ensures that you won't ever be taken by surprise.
 
 * Soft limit: You receive a notification email.
 * Hard limit: Subsequent requests will be rejected.
 
 ## The Value of Investing in LLM-Toolbox
 
 Well... in giving your money to OpenAI, actually.
 
-Even if you have a monthly expense of more than a dollar, it's well worth looking at looking at the huge benefits you'll receive from utilizing the tools in the LLM-Toolbox. These innovative solutions provide users with powerful capabilities that can **significantly streamline tasks, improve productivity, and foster creativity**.
+Even if you have a monthly expense of more than a dollar, it's well worth looking at the huge benefits you'll receive from utilizing the tools in the LLM-Toolbox. These innovative solutions provide users with powerful capabilities that can **significantly streamline tasks, improve productivity, and foster creativity**.
 
-Particularly, let's consider [ShellGenius](#shellgenius), a remarkable tool within the LLM-Toolbox. It enhances the command-line experience by translating task descriptions into efficient shell commands, a feat that not only saves time but also reduces the possibility of human error. This tool is extremely beneficial for both beginners, who may not be fluent in shell commands, and experienced users who can streamline their command-line tasks by simply describing what they wish to accomplish, and [ShellGenius](#shellgenius) provides the correct shell command to achieve it.
+Particularly, let's consider [ShellGenius](#shellgenius), a remarkable tool within the LLM-Toolbox. It enhances the command-line experience by translating task descriptions into efficient shell commands, a feat that not only saves time but also reduces the possibility of human error. This tool is extremely beneficial for both beginners, who may not be fluent in shell commands, and experienced users who can streamline their command-line tasks by simply describing what they wish to accomplish.
 
 Therefore, when considering the cost, it's essential to look beyond the immediate dollar value and evaluate the considerable time, effort, and resources you stand to save. The utility and value derived from such tools often outweigh the minimal monthly cost. The price of these tools should not be a deterrent but rather seen as an investment in enhancing your efficiency and productivity.
 
 ### Is GPT-3.5 Sufficient for Those Tools?
 
-GPT-3.5 is an excellent model for these tools, offering cost-effective solution that consistently delivers appropriate responses. I take great care in crafting my prompts and the tools to generate the best results that cater to my daily needs.
+GPT-3.5 is an excellent model for these tools, offering a cost-effective solution that consistently delivers appropriate responses. I take great care in crafting my prompts and the tools to generate the best results that cater to my own daily needs.
 
 I will continue refining them, if necessary, as time goes on. So stay tuned to this repo and consider giving it a star ⭐!
 
 You'll also be able to update the LLM-Toolbox directly from the CLI 😊.
 
 ### Current Costs
 
@@ -96,15 +114,15 @@
 
 ```bash
 python3 -m pip install llm-toolbox
 ```
 
 ### `pipx`, the Easy Way
 
-To use these tools, I recommend that you first install [pipx](https://pypa.github.io/pipx/installation/). It's a package manager for Python that makes the installation and upgrade of CLI apps easy (no more hassle with virtual environment 😌).
+To use these tools, I recommend that you first install [pipx](https://pypa.github.io/pipx/installation/). It's a package manager for Python that makes the installation and upgrade of CLI apps easy (no more hassle with virtual environments 😌).
 
 * Debian / Ubuntu
 
     ```bash
     sudo apt install pipx
     ```
 
@@ -178,65 +196,130 @@
   setx OPENAI_API_KEY your_key
   ```
 
 ## Tools
 
 Instructions on how to use each of the tools are included in the individual directories under [tools/](https://github.com/sderev/llm-toolbox/tree/main/tools). This is also where I give some tricks and tips on their usage 💡👀💭.
 
-Here's a brief overview:
+Note that LMT is the main tool in the LLM-Toolbox. All of its options apply to (almost) all of the other tools. For instance, you change the model to GPT-4 with `-m 4` or add emojis with `--emoji`. Refer to the [LMT's documentation](https://github.com/sderev/lmt) for more information. 
+
+* **Reading from `stdin`**: Almost all of the tools can read from `stdin`. For instance: `cat my_text.md | summarize`.
+
+* **Output Redirection**: You can use output redirections with the tools. For instance: `cat my_text.md | critique --raw > critique_of_my_text.md`
+
+Here's a brief overview of the tools:
+
+### LMT
+
+[LMT](https://github.com/sderev/lmt) empowers you to interact directly with ChatGPT from the comfort of your terminal. One of the core features of `lmt` is its ability to facilitate the creation of custom templates, enabling you to design your personalized toolbox of CLI applications. You can easily install its standalone version from [the project's repository](https://github.com/sderev/lmt).
 
 ### ShellGenius
 
 [ShellGenius](https://github.com/sderev/shellgenius) is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands. Check out the project on [its dedicated repository](https://github.com/sderev/shellgenius).
 
 ![shellgenius](https://github.com/sderev/llm-toolbox/assets/24412384/688d9a1a-f351-42d0-9f4d-06a9a6d1909a)
 
+### Commitgen
+
+The [`commitgen`](https://github.com/sderev/llm-toolbox/tree/main/tools/commitgen) tool is designed to streamline your `git` workflow by automatically generating meaningful commit messages for your code changes.
+
+![demo_0](https://github.com/sderev/llm-toolbox/assets/24412384/d41985d5-d8a2-4622-9ef7-643176cdc741)
+___
+
+### Codereview
+
+The [`Codereview`](https://github.com/sderev/llm-toolbox/tree/main/tools/codereview) tool accepts a file or a piece of text as input and provides an in-depth analysis of the code. It can identify potential issues, suggest improvements, and even detect security vulnerabilities. The Codereview tool is capable of handling a variety of programming languages, and its feedback can serve as an invaluable resource for developers seeking to enhance the quality of their code. 
+
 ___
 
 ### VocabMaster
 
 Master new languages with [VocabMaster](https://github.com/sderev/vocabmaster), a CLI tool designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience. Check out the project on [its dedicated repository](https://github.com/sderev/vocabmaster).
 
 ![vocabmaster_translate_japanese](https://github.com/sderev/llm-toolbox/assets/24412384/5f5612fe-f1fb-4d4c-bb25-68f07961e66b)
 
 ___
 
 ### Thesaurus
 
-The [`thesaurus`](https://github.com/sderev/llm-toolbox/tree/main/tools/thesaurus) script takes a word or a phrase as input and provides a list of synonyms and antonyms.
+The [`thesaurus`](https://github.com/sderev/llm-toolbox/tree/main/tools/thesaurus) tool takes a word or a phrase as input and provides a list of synonyms and antonyms.
 
 ![thesaurus](https://github.com/sderev/llm-toolbox/assets/24412384/dca6bf42-2545-4b56-bb20-4c8e6c872529)
 
 ___
 
 ### Define
 
-The [`define`](https://github.com/sderev/llm-toolbox/tree/main/tools/define) script takes a word as input and provides its definition along with an example sentence using the word.
+The [`define`](https://github.com/sderev/llm-toolbox/tree/main/tools/define) tool takes a word as input and provides its definition along with an example sentence using the word.
 
 ![define](https://github.com/sderev/llm-toolbox/assets/24412384/1e813b80-6896-483b-b31a-65ad7cb81173)
 
 ___
 
 ### Proofread
 
-The [`proofread`](https://github.com/sderev/llm-toolbox/tree/main/tools/proofread) script takes a sentence as input and provides a corrected version of it, if needed, along with an explanation of the corrections.
+The [`proofread`](https://github.com/sderev/llm-toolbox/tree/main/tools/proofread) tool takes a sentence as input and provides a corrected version of it, if needed, along with an explanation of the corrections.
 
 ![proofread_english](https://github.com/sderev/llm-toolbox/assets/24412384/e84ce7cd-68e9-4d6d-8c56-55b93c7e4fee)
 
 ___
 
 ### Translate
 
-The [`translate`](https://github.com/sderev/llm-toolbox/tree/main/tools/translate) script takes a sentence and a target language as input and provides the translated sentence in the target language.
+The [`translate`](https://github.com/sderev/llm-toolbox/tree/main/tools/translate) tool takes a sentence and a target language as input and provides the translated sentence in the target language.
 
 ![translate](https://github.com/sderev/llm-toolbox/assets/24412384/505237c9-7735-4db6-aa4a-63c3ed2867a7)
 
-## Prompt Templates
+___
+
+### Cheermeup
 
-In addition to the various tools provided, the LLM-Toolbox includes a collection of prompt templates in the [`prompts/`](https://github.com/sderev/llm-toolbox/tree/main/prompts) directory. These templates cover a wide range of scenarios and are designed to optimize your interaction with language models. They are an excellent starting point if you're not sure how to structure your prompts or if you're seeking to improve the effectiveness of your current prompts.
+The [`cheermeup`](https://github.com/sderev/llm-toolbox/tree/main/tools/cheermeup) tool is designed to uplift your spirits based on your current mood. Whether you're feeling down or just need a little pick-me-up, this tool uses a variety of methods to bring a smile to your face and brighten your day.
+
+___
+
+### Critique
+
+The [`critique`](https://github.com/sderev/llm-toolbox/tree/main/tools/critique) tool is your personal constructive text critic, designed to analyze a given piece of text and provide detailed, insightful feedback. It enables users to enhance their writing by addressing potential shortcomings and improving the overall quality.
+
+___
 
-Please feel free to explore these templates and adapt them to suit your specific needs.
+### Explain
+
+The [`explain`](https://github.com/sderev/llm-toolbox/tree/main/tools/explain) tool helps to clarify complex concepts. When given a concept, it presents a comprehensive and straightforward explanation, aiding in understanding and knowledge retention.
+
+___
+
+### Lessonize
+
+The [`lessonize`](https://github.com/sderev/llm-toolbox/tree/main/tools/lessonize) tool transforms any piece of text into an informative lesson. Whether you're a teacher looking for instructional material or a student looking to further understand a subject, this tool makes learning more accessible.
+
+___
+
+### Pathlearner
+
+The [`pathlearner`](https://github.com/sderev/llm-toolbox/tree/main/tools/pathlearner) tool provides a comprehensive study plan for a given topic. Whether you're studying for an exam or learning a new subject, this tool creates a structured, step-by-step plan that aids in understanding and mastering the material.
+
+___
+
+### Study
+
+The [`study`](https://github.com/sderev/llm-toolbox/tree/main/tools/study) tool is a comprehensive guide that generates study material for a particular topic or content. It helps students to better prepare for exams, giving them access to tailored study material designed to enhance their learning experience.
+
+___
+
+### Summarize
+
+The [`summarize`](https://github.com/sderev/llm-toolbox/tree/main/tools/summarize) tool provides succinct summaries of a web page, lengthy texts, or the content of given files. It's perfect for extracting key points and crucial information from vast amounts of data, saving users time and effort.
+
+___
+
+### Teachlib
+
+The [`teachlib`](https://github.com/sderev/llm-toolbox/tree/main/tools/teachlib) tool is designed to provide comprehensive lessons on various libraries. By simplifying complex aspects and focusing on the core functionalities, this tool helps users to understand and effectively utilize different libraries.
+
+___
 
 ## License
 
 This project is licensed under the terms of the Apache License 2.0.
```

### Comparing `LLM-Toolbox-0.0.2/llm_toolbox/cli.py` & `LLM-Toolbox-0.1.0/llm_toolbox/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,150 +1,256 @@
-import click
 from functools import wraps
-import os
 from pathlib import Path
+import os
+import re
+import requests
 import subprocess
-import pty
 import sys
 import tempfile
-import re
 
+import click
+import validators
+from strip_tags.lib import strip_tags
 
-EMOJI = (
-    "Add plenty of emojis as a colorful way to convey emotions in your response 😊."
-    " However, don't mention that you use emojis."
-)
+from lmt_cli.lib import *
+from lmt_cli.cli import VALID_MODELS
+
+
+def validate_model_name(ctx, param, value):
+    """
+    Validates the model name parameter.
+    """
+    model_name = value.lower()
+    if model_name in VALID_MODELS:
+        return VALID_MODELS[model_name]
+    elif model_name in VALID_MODELS.values():
+        return model_name
+    else:
+        raise click.BadParameter(f"Invalid model: {model_name}")
+
+
+def validate_temperature(ctx, param, value):
+    """
+    Validates the temperature parameter.
+    """
+    if 0 <= value <= 2:
+        return value
+    else:
+        raise click.BadParameter("Temperature must be between 0 and 2.")
 
 
 @click.group()
 @click.pass_context
+@click.version_option()
 def cli():
     pass
 
 
 def common_options(f):
     @wraps(f)
     @click.option("--emoji", is_flag=True, help="Add emotions and emojis.")
     @click.option(
         "-m",
         "--model",
-        type=click.STRING,
         default="gpt-3.5-turbo",
-        help="Choose a model.",
+        help="The model to use for the requests.",
+        callback=validate_model_name,
+    )
+    @click.option(
+        "--temperature",
+        callback=validate_temperature,
+        default=1,
+        type=float,
+        help="The temperature to use for the requests.",
+        show_default=True,
+    )
+    @click.option(
+        "--tokens",
+        is_flag=True,
+        help=(
+            "Count the number of tokens in the prompt, and display the cost of the"
+            " request."
+        ),
+    )
+    @click.option(
+        "--no-stream",
+        is_flag=True,
+        default=False,
+        help="Disable the streaming of the response.",
+    )
+    @click.option(
+        "--raw",
+        "-r",
+        is_flag=True,
+        default=False,
+        help="Disable colors and formatting, and print the raw response.",
+    )
+    @click.option(
+        "--debug",
+        is_flag=True,
+        default=False,
+        help="Print debug information.",
     )
     def wrapper(*args, **kwargs):
         return f(*args, **kwargs)
 
     return wrapper
 
 
 @cli.command()
 @click.argument("words", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def thesaurus(ctx, model, words, emoji):
+def thesaurus(ctx, model, emoji, words, temperature, tokens, no_stream, raw, debug):
     """
     This is the thesaurus command. It requires a word as input, either as an argument or from stdin.
     The command will use the given word to find synonyms and antonyms.
 
     Example usage: thesaurus [word]
     """
-    process_command(ctx, "thesaurus", model, words, emoji)
+    process_command(
+        ctx,
+        "thesaurus",
+        model,
+        emoji,
+        words,
+        temperature,
+        tokens,
+        no_stream,
+        raw,
+        debug,
+    )
 
 
 @cli.command()
 @click.argument("sentence", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def translate(ctx, model, sentence, emoji):
+def translate(ctx, model, emoji, sentence, temperature, tokens, no_stream, raw, debug):
     """
     Translate a word or sentence.
     """
-    process_command(ctx, "translate", model, sentence, emoji)
+    process_command(
+        ctx,
+        "translate",
+        model,
+        emoji,
+        sentence,
+        temperature,
+        tokens,
+        no_stream,
+        raw,
+        debug,
+    )
 
 
 @cli.command()
 @click.argument("word", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def define(ctx, model, word, emoji):
+def define(ctx, model, emoji, word, temperature, tokens, no_stream, raw, debug):
     """
     Get a definition for a word.
     """
-    process_command(ctx, "define", model, word, emoji)
+    process_command(
+        ctx, "define", model, emoji, word, temperature, tokens, no_stream, raw, debug
+    )
 
 
 @cli.command()
 @click.argument("text", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def proofread(ctx, model, text, emoji):
+def proofread(ctx, model, emoji, text, temperature, tokens, no_stream, raw, debug):
     """
     Proofread a piece of text.
     """
-    process_command(ctx, "proofread", model, text, emoji)
+    process_command(
+        ctx, "proofread", model, emoji, text, temperature, tokens, no_stream, raw, debug
+    )
 
 
 @cli.command()
 @click.argument("topic", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def lessonize(ctx, model, topic, emoji):
+def lessonize(ctx, model, emoji, topic, temperature, tokens, no_stream, raw, debug):
     """
     Create a lesson from a piece of text.
     """
-    process_command(ctx, "lessonize", model, topic, emoji)
+    process_command(
+        ctx,
+        "lessonize",
+        model,
+        emoji,
+        topic,
+        temperature,
+        tokens,
+        no_stream,
+        raw,
+        debug,
+    )
 
 
 @cli.command()
 @click.argument("file", type=click.File("r"), required=False)
 @click.pass_context
 @common_options
-def commitgen(ctx, model, file, emoji):
+def commitgen(ctx, model, emoji, file, temperature, tokens, no_stream, raw, debug):
     """
     This is the commitgen command. It is used in a git repository.
 
     The command will generate a detailed commit message based on the changes detected by 'git diff --staged'.
 
     Optionally, it can take entire files to provide more context.
 
     Example usage: commitgen myfile.py
     """
     # Check if we are in a git repository
     try:
         subprocess.check_output(["git", "rev-parse", "--is-inside-work-tree"])
     except subprocess.CalledProcessError as error:
-        # click.echo(f"Error occurred: {error}", err=True)
+        click.echo(f"{click.style('Error occurred: {error}', fg='red')}", err=True)
         return
 
     # Check if there are staged changes
     try:
-        diff_output = subprocess.check_output(["git", "diff", "--staged"]).decode()
+        diff_output = subprocess.check_output(["git", "diff", "--staged"])
     except subprocess.CalledProcessError as error:
-        click.echo(f"Error occurred: {error}", err=True)
-        # There are no staged changes
+        click.echo(f"{click.style('Error occurred: {error}', fg='red')}", err=True)
         return
 
     if file:
         file_content = file.read()
-        prompt = diff_output + "\n---\n" + file_content
+        prompt_input = diff_output + "\n---\n" + file_content
     else:
-        prompt = diff_output
+        prompt_input = str(diff_output)
 
-    if emoji:
-        prompt += f"\n---\n{EMOJI}"
+    click.echo("Generating commit message...\n---\n\n")
 
-    command = ["llm", "--template", "commitgen", prompt.encode("utf-8")]
-    if model:
-        command.extend(["--model", str(model)])
+    commit_message = process_command(
+        ctx,
+        template="commitgen",
+        emoji=emoji,
+        model=model,
+        prompt_input=prompt_input,
+        temperature=temperature,
+        tokens=tokens,
+        no_stream=no_stream,
+        raw=raw,
+        debug=debug,
+    )
 
-    click.echo("Generating commit message...\n---\n\n")
+    # Get only the content of the ChatGPT request
+    commit_message = commit_message[0].strip()
 
-    commit_message = execute(command)
-    click.echo(commit_message)
+    # Clean `^M` characters
+    commit_message = commit_message.replace("\r", "")
+
+    # click.echo(commit_message) #TODO: delete?
     click.echo("\n---\n")
 
     choice = click.prompt(
         "Do you want to use this commit message? (yes/edit/no)",
         type=str,
         default="edit",
     )
@@ -175,216 +281,249 @@
             subprocess.run(["git", "commit", "-F", temp_path])
         elif choice == "edit":
             subprocess.run(["git", "commit", "-e", "-t", temp_path])
     finally:
         os.remove(temp_path)
 
 
-def codereview(ctx, model, file_to_review, emoji):
+@cli.command()
+@click.argument("file_to_review", type=click.File("r"), required=False)
+@click.pass_context
+@common_options
+def codereview(
+    ctx, model, emoji, file_to_review, temperature, tokens, no_stream, raw, debug
+):
     """
     Generate a code review for a given file.
 
     Example usage: cat file.py | codereview --emoji
     """
-    process_command(ctx, "codereview", model, file_to_review, emoji)
+    process_command(
+        ctx,
+        "codereview",
+        model,
+        emoji,
+        file_to_review,
+        temperature,
+        tokens,
+        no_stream,
+        raw,
+        debug,
+    )
 
 
 @cli.command()
 @click.argument("source", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def summarize(ctx, model, source, emoji):
+def summarize(ctx, model, emoji, source, temperature, tokens, no_stream, raw, debug):
     """
     Summarize the text, the content of a given file, or a webpage (provided as URL).
     """
-    # No input from pipe and no argument
-    if not source and sys.stdin.isatty():
-        with click.Context(summarize) as ctx:
-            click.echo(summarize.get_help(ctx), err=True)
-        return
-
     source_str = " ".join(source)
 
-    command = ["llm", "--template", "summarize"]
-    if model:
-        command.extend(["--model", str(model)])
-
-    prompt = "".encode("utf-8")
-    if emoji:
-        prompt = f"{EMOJI}\n---\n".encode("utf-8")
+    prompt_input = ""
 
     if is_valid_url(source_str):
-        curl_cmd = ["curl", "-s", source_str]
-        strip_tags_cmd = ["strip-tags", "-m"]
-
-        curl_proc = subprocess.Popen(curl_cmd, stdout=subprocess.PIPE)
-        strip_tags_proc = subprocess.Popen(
-            strip_tags_cmd, stdin=curl_proc.stdout, stdout=subprocess.PIPE
-        )
-        llm_proc = subprocess.Popen(
-            command, stdin=strip_tags_proc.stdout, stdout=subprocess.PIPE
-        )
-
-        # Allow curl_proc to receive a SIGPIPE if strip_tags_proc exits.
-        curl_proc.stdout.close()
-        # Allow strip_tags_proc to receive a SIGPIPE if llm_proc exits.
-        strip_tags_proc.stdout.close()
-
+        source_content = requests.get(source_str).text
+        prompt_input = strip_tags(input=source_content, minify=True)
     else:
         if source:
-            content = "".join(source).encode("utf-8")
-            prompt += content
-            command.append(prompt)
+            content = "".join(source)
+            prompt_input += content
 
-    execute(command)
+    process_command(
+        ctx,
+        "summarize",
+        model,
+        emoji,
+        prompt_input,
+        temperature,
+        tokens,
+        no_stream,
+        raw,
+        debug,
+    )
 
 
 @cli.command()
 @click.argument("work_to_critique", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def critique(ctx, model, work_to_critique, emoji):
+def critique(
+    ctx, model, emoji, work_to_critique, temperature, tokens, no_stream, raw, debug
+):
     """
     Generate a critique for a given piece of work.
     """
-    process_command(ctx, "critique", model, work_to_critique, emoji)
+    process_command(
+        ctx,
+        "critique",
+        model,
+        emoji,
+        work_to_critique,
+        temperature,
+        tokens,
+        no_stream,
+        raw,
+        debug,
+    )
 
 
 @cli.command()
 @click.argument("topic", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def pathlearner(ctx, model, topic, emoji):
+def pathlearner(ctx, model, emoji, topic, temperature, tokens, no_stream, raw, debug):
     """
     Provide a study plan for a given topic.
     """
-    process_command(ctx, "pathlearner", model, topic, emoji)
+    process_command(
+        ctx,
+        "pathlearner",
+        model,
+        emoji,
+        topic,
+        temperature,
+        tokens,
+        no_stream,
+        raw,
+        debug,
+    )
 
 
 @cli.command()
 @click.argument("concept", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def explain(ctx, model, concept, emoji):
+def explain(ctx, model, emoji, concept, temperature, tokens, no_stream, raw, debug):
     """
     Explain a concept.
     """
-    process_command(ctx, "explain", model, concept, emoji)
+    process_command(
+        ctx,
+        "explain",
+        model,
+        emoji,
+        concept,
+        temperature,
+        tokens,
+        no_stream,
+        raw,
+        debug,
+    )
 
 
 @cli.command()
 @click.argument("mood", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def cheermeup(ctx, model, mood, emoji):
+def cheermeup(ctx, model, emoji, mood, temperature, tokens, no_stream, raw, debug):
     """
     Cheer you up based on your mood.
     """
-    process_command(ctx, "cheermeup", model, mood, emoji)
+    process_command(
+        ctx, "cheermeup", model, emoji, mood, temperature, tokens, no_stream, raw, debug
+    )
 
 
 @cli.command()
 @click.argument("study_material", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def study(ctx, model, study_material, emoji):
+def study(
+    ctx, model, emoji, study_material, temperature, tokens, no_stream, raw, debug
+):
     """
     Generate study material for a topic or from the content of the content of a file.
     """
-    process_command(ctx, "study", model, study_material, emoji)
+    process_command(
+        ctx,
+        "study",
+        model,
+        emoji,
+        study_material,
+        temperature,
+        tokens,
+        no_stream,
+        raw,
+        debug,
+    )
 
 
 @cli.command()
 @click.argument("library_name", nargs=-1, required=False)
 @click.pass_context
 @common_options
-def teachlib(ctx, model, library_name, emoji):
+def teachlib(
+    ctx, model, emoji, library_name, temperature, tokens, no_stream, raw, debug
+):
     """
     Teach a library.
     """
-    process_command(ctx, "teachlib", model, library_name, emoji)
+    process_command(
+        ctx,
+        "teachlib",
+        model,
+        emoji,
+        library_name,
+        temperature,
+        tokens,
+        no_stream,
+        raw,
+        debug,
+    )
 
 
-def process_command(ctx, command_name, model, prompt, emoji):
+def process_command(
+    ctx,
+    template: str,
+    model: str,
+    emoji: bool,
+    prompt_input: str,
+    temperature: float,
+    tokens: bool,
+    no_stream: bool,
+    raw: bool,
+    debug: bool,
+):
     """
     Process a given command using a specific template and optional lines.
-
-    This function forms a command for the Language Learning Model (LLM) using
-    a specified command name and optionally lines. The formed command is then executed.
-    If no lines are provided, the function attempts to read from the standard input.
-    """
-    if not prompt and sys.stdin.isatty():
-        with click.Context(ctx.command) as ctx:
-            click.echo(ctx.command.get_help(ctx), err=True)
-        return
-
-    if not prompt:
-        prompt = sys.stdin.read().splitlines()
-
-    command = ["llm", "--template", command_name]
-
-    if model:
-        command.extend(["--model", str(model)])
-
-    if prompt:
-        prompt = "\n".join(prompt)
-
-        if emoji:
-            prompt += EMOJI
-        command.append(prompt.encode("utf-8"))
-
-    execute(command)
-
-
-def execute(command):
     """
-    Execute a subprocess and print the output in real-time.
-    """
-    output_str = ""
-
-    try:
-        # Open a pseudo-terminal to interact with the subprocess
-        master, slave = pty.openpty()
-
-        process = subprocess.Popen(command, stdout=slave, stderr=subprocess.STDOUT)
-
-        os.close(slave)  # Close the slave pty, otherwise we won't get EOF
-
-        while True:
-            try:
-                output = os.read(master, 8)  # Read chunks of 8 bytes
-                if not output:
-                    break
-                try:
-                    decoded_output = output.decode("utf-8")
-                except UnicodeDecodeError as error:
-                    decoded_output = output.decode("utf-8", errors="replace")
-                    click.echo(f"Error decoding output: {error}", err=True)
-
-                print(decoded_output, end="")
-                output_str += decoded_output
-                sys.stdout.flush()
-            except OSError:
-                break  # Probably the process has ended
-
-        os.close(master)  # Close the master pty too when we're done.
-
-        exit_status = process.wait()
-        if exit_status != 0:
-            click.echo(f"'{command}' exited with status {exit_status}", err=True)
-
-    except Exception as error:
-        click.echo(
-            f"Error occurred while executing command:\n{str(error)}",
-            err=True,
-        )
-
-    return output_str
+    if not prompt_input:
+        if not sys.stdin.isatty():
+            prompt_input = sys.stdin.read()
+        elif sys.stdin.isatty():
+            click.echo(
+                click.style(
+                    (
+                        "You can paste your prompt below. Press <Enter> to"
+                        " validate.\nOnce you've done, press Ctrl+D to send it."
+                    ),
+                    fg="yellow",
+                )
+                + "\n---"
+            )
+            prompt_input = sys.stdin.read()
+            click.echo()
+    prompt_input = "".join(prompt_input).rstrip()
+
+    return prepare_and_generate_response(
+        system=None,
+        template=template,
+        model=model,
+        prompt_input=prompt_input,
+        emoji=emoji,
+        temperature=temperature,
+        tokens=tokens,
+        no_stream=no_stream,
+        raw=raw,
+        debug=debug,
+    )
 
 
 def is_valid_url(url):
-    pattern = r"^((http|https)://)[-a-zA-Z0-9@:%._\\+~#?&//=]{2,256}\\.[a-z]{2,6}\\b([-a-zA-Z0-9@:%._\\+~#?&//=]*)$"
-    return re.match(pattern, url)
+    return validators.url(url)
 
 
 if __name__ == "__main__":
     cli()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/codereview.yaml` & `LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/codereview.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,5 @@
 system: >
   As an AI with a deep understanding of code structure and programming best practices, you scrutinize every aspect of the provided code.
   Your focus encompasses potential bugs, appropriateness of variable and function names, time and space complexity, comments, and other elements crucial to efficient code writing.
   You identify areas for improvement and provide clear, detailed explanations for your recommended changes.
   Always polite and constructive, your goal is to assist the coder in honing their skills and enhancing their understanding of clean, efficient code writing.
-
```

### Comparing `LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/commitgen.yaml` & `LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/commitgen.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
 system: >
   As an AI with extensive knowledge of code and version control best practices, your task is to generate a detailed and meaningful git commit message based on the output of a `git diff` command.
   You will carefully read the diff to understand what changes have been made, and then construct a concise, informative commit message that captures the essence of the modifications.
   In cases where entire files are provided, you will use the context of the full code to ensure your commit message is as accurate and helpful as possible.
   Maintain a profesionnal tone.
   It's crucial that the first line of your generated commit message must be a summary of the commit message and never exceed 50 characters. Follow with a detailed, but compact, explanation.
   Do not talk. Just write a detailed commit message following professional guidelines.
-
```

### Comparing `LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/lessonize.yaml` & `LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/lessonize.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,8 +2,7 @@
   As an AI with extensive knowledge and excellent pedagogical skills, your task is to transform the given concept or topic into a comprehensive lesson.
   Start by providing an engaging introduction that hooks the learner's interest.
   Define clear learning objectives that outline what the learner will gain from the lesson.
   Then, break down the topic into manageable sections or steps, explaining each one in an understandable manner.
   Incorporate practical examples, activities or exercises where possible to reinforce learning.
   Finally, provide a summary and potential follow-up activities or resources for further study.
   You ensure that your lesson is structured, detailed and catered to the learner's level of understanding.
-
```

### Comparing `LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/pathlearner.yaml` & `LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/pathlearner.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,5 @@
 system: >
   Assuming the role of an AI guidance counselor, you bring to bear your extensive knowledge of various educational and career paths.
   Your task is to guide and recommend the best paths based on the individual's interests, skills, and aspirations.
   Beyond suggestions, you also develop a concrete and actionable plan to help the individual achieve their goals.
   Your advice is empathetic, clear, and practical, aimed at enabling individuals to make informed decisions and follow a tangible roadmap towards their future.
-
```

### Comparing `LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/teachlib.yaml` & `LLM-Toolbox-0.1.0/llm_toolbox/tools/templates/teachlib.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,7 @@
   As an expert in programming language, your mission is to impart knowledge on the provided library.
   Start by introducing the library to a newcomer who has never used it, with a focus on making your explanations understandable and engaging.
   Your examples should be clear and elegantly crafted to aid understanding.
   After this introductory phase, guide your student through the basic functionalities of the library.
   Progress to more advanced features of the library, ensuring your student comprehends each level before moving on.
   Once the basics and advanced features are well understood, implement a project-based lesson to provide practical, hands-on experience with the library.
   You are not only an expert but also a pedagogue, ensuring your student's understanding at each stage of learning.
-
```

### Comparing `LLM-Toolbox-0.0.2/setup.py` & `LLM-Toolbox-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 from pathlib import Path
 import shutil
 
-VERSION = "0.0.2"
+VERSION = "0.1.0"
 
 
 class PostDevelopCommand(develop):
     """Post-installation for development mode."""
 
     def run(self):
         develop.run(self)
         self.execute(self.copy_files, (), {})
 
     def copy_files(self):
-        dest_path = Path.home() / ".config/io.datasette.llm/templates"
+        dest_path = Path.home() / ".config/lmt/templates"
         dest_path.mkdir(parents=True, exist_ok=True)
 
         src_path = Path(__file__).parent / "llm_toolbox/tools/templates"
         for file in src_path.glob("*.yaml"):
             shutil.copy2(file, dest_path)
 
 
@@ -61,29 +61,29 @@
     package_data={
         "llm_toolbox": ["tools/templates/*.yaml"],
     },
     cmdclass={"develop": PostDevelopCommand, "install": PostInstallCommand},
     install_requires=read_requirements(),
     entry_points={
         "console_scripts": [
-            "llm-toolbox=llm_toolbox.cli:cli",
-            "thesaurus=llm_toolbox.cli:thesaurus",
-            "llm=llm.cli:cli",
-            "translate=llm_toolbox.cli:translate",
-            "define=llm_toolbox.cli:define",
-            "proofread=llm_toolbox.cli:proofread",
-            "lessonize=llm_toolbox.cli:lessonize",
-            "commitgen=llm_toolbox.cli:commitgen",
+            "cheermeup=llm_toolbox.cli:cheermeup",
             "codereview=llm_toolbox.cli:codereview",
-            "summarize=llm_toolbox.cli:summarize",
+            "commitgen=llm_toolbox.cli:commitgen",
             "critique=llm_toolbox.cli:critique",
-            "pathlearner=llm_toolbox.cli:pathlearner",
+            "define=llm_toolbox.cli:define",
             "explain=llm_toolbox.cli:explain",
-            "cheermeup=llm_toolbox.cli:cheermeup",
+            "lessonize=llm_toolbox.cli:lessonize",
+            "llm-toolbox=llm_toolbox.cli:cli",
+            "lmt=lmt_cli.cli:lmt",
+            "pathlearner=llm_toolbox.cli:pathlearner",
+            "proofread=llm_toolbox.cli:proofread",
             "shellgenius=shellgenius.cli:shellgenius",
             "study=llm_toolbox.cli:study",
+            "summarize=llm_toolbox.cli:summarize",
             "teachlib=llm_toolbox.cli:teachlib",
+            "thesaurus=llm_toolbox.cli:thesaurus",
+            "translate=llm_toolbox.cli:translate",
             "vocabmaster=vocabmaster.cli:vocabmaster",
         ]
     },
     python_requires=">=3.8",
 )
```

