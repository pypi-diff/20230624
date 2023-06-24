# Comparing `tmp/aimped-0.1.51.tar.gz` & `tmp/aimped-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimped-0.1.51.tar", last modified: Tue Jun  6 20:38:23 2023, max compression
+gzip compressed data, was "dist/aimped-0.1.52.tar", last modified: Sat Jun 24 17:32:53 2023, max compression
```

## Comparing `aimped-0.1.51.tar` & `aimped-0.1.52.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.451718 aimped-0.1.51/
--rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.51/LICENSE
--rw-rw-rw-   0        0        0     1778 2023-06-06 20:38:23.452711 aimped-0.1.51/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.51/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.394163 aimped-0.1.51/aimped/
--rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.51/aimped/__init__.py
--rw-rw-rw-   0        0        0    13545 2023-06-06 20:32:24.000000 aimped-0.1.51/aimped/io_tasks.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.409188 aimped-0.1.51/aimped/model/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/model/__init__.py
--rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/model/load.py
--rw-rw-rw-   0        0        0      655 2023-06-06 20:37:28.000000 aimped-0.1.51/aimped/models.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.412190 aimped-0.1.51/aimped/nitro/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nitro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.435712 aimped-0.1.51/aimped/nlp/
--rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/assertion.py
--rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/chunker.py
--rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/deid.py
--rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/ner.py
--rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/ner_cls_report.py
--rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/pipeline.py
--rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/regex_parser.py
--rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.51/aimped/nlp/relation.py
--rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.51/aimped/nlp/relation_visualizer.py
--rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/tokenizer.py
--rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/nlp/tools.py
--rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.51/aimped/nlp/translation.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.450715 aimped-0.1.51/aimped/test/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/__init__.py
--rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_assertion.py
--rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_chunk_merger.py
--rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_deid_pipeline.py
--rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_ner_results.py
--rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_regex_parser.py
--rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_relation_pipeline.py
--rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_tokenizer.py
--rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.51/aimped/test/test_translation_pipeline.py
--rw-rw-rw-   0        0        0     2060 2023-06-05 10:53:19.000000 aimped-0.1.51/aimped/utils.py
--rw-rw-rw-   0        0        0      130 2023-06-06 20:34:20.000000 aimped-0.1.51/aimped/version.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:38:23.406189 aimped-0.1.51/aimped.egg-info/
--rw-rw-rw-   0        0        0     1778 2023-06-06 20:38:23.000000 aimped-0.1.51/aimped.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-06-06 20:38:23.000000 aimped-0.1.51/aimped.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 20:38:23.000000 aimped-0.1.51/aimped.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-06 20:38:23.000000 aimped-0.1.51/aimped.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 20:38:23.000000 aimped-0.1.51/aimped.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-06-06 20:38:23.453716 aimped-0.1.51/setup.cfg
--rw-rw-rw-   0        0        0     1163 2023-06-06 20:33:50.000000 aimped-0.1.51/setup.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/
+-rw-r--r--   0 DataScience   (501) staff       (20)     1751 2023-06-24 17:32:53.000000 aimped-0.1.52/PKG-INFO
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped/
+-rw-r--r--   0 DataScience   (501) staff       (20)    12438 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/io_tasks.py
+-rw-r--r--   0 DataScience   (501) staff       (20)      123 2023-06-24 17:32:21.000000 aimped-0.1.52/aimped/version.py
+-rw-r--r--   0 DataScience   (501) staff       (20)      502 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/models.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped/test/
+-rw-r--r--   0 DataScience   (501) staff       (20)     1313 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_chunk_merger.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     3320 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_relation_pipeline.py
+-rw-r--r--   0 DataScience   (501) staff       (20)      610 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_tokenizer.py
+-rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/__init__.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     1592 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_regex_parser.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     5585 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_translation_pipeline.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     1297 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_ner_results.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2748 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_assertion.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     1866 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_deid_pipeline.py
+-rw-r--r--   0 DataScience   (501) staff       (20)      193 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/__init__.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2060 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/utils.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped/model/
+-rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/model/__init__.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2338 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/model/load.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped/nlp/
+-rw-r--r--   0 DataScience   (501) staff       (20)    19853 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/relation_visualizer.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     4290 2023-06-24 17:02:00.000000 aimped-0.1.52/aimped/nlp/relation.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     3917 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/chunker.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2251 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/tools.py
+-rw-r--r--   0 DataScience   (501) staff       (20)      353 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/__init__.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2228 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/assertion.py
+-rw-r--r--   0 DataScience   (501) staff       (20)      803 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/tokenizer.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2629 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/ner_cls_report.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     4521 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/ner.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2825 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/deid.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     6873 2023-06-24 17:31:12.000000 aimped-0.1.52/aimped/nlp/pipeline.py
+-rwxr-xr-x   0 DataScience   (501) staff       (20)     2524 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/translation.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     3899 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/regex_parser.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped/nitro/
+-rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nitro/__init__.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     1063 2023-06-24 16:48:55.000000 aimped-0.1.52/LICENSE
+-rw-r--r--   0 DataScience   (501) staff       (20)     1157 2023-06-24 16:48:55.000000 aimped-0.1.52/README.md
+-rw-r--r--   0 DataScience   (501) staff       (20)     1163 2023-06-24 16:48:55.000000 aimped-0.1.52/setup.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/
+-rw-r--r--   0 DataScience   (501) staff       (20)     1751 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/PKG-INFO
+-rw-r--r--   0 DataScience   (501) staff       (20)      952 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/SOURCES.txt
+-rw-r--r--   0 DataScience   (501) staff       (20)       48 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/requires.txt
+-rw-r--r--   0 DataScience   (501) staff       (20)        7 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/top_level.txt
+-rw-r--r--   0 DataScience   (501) staff       (20)        1 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/dependency_links.txt
+-rw-r--r--   0 DataScience   (501) staff       (20)      103 2023-06-24 17:32:53.000000 aimped-0.1.52/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `aimped-0.1.51/LICENSE` & `aimped-0.1.52/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/PKG-INFO` & `aimped-0.1.52/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-Metadata-Version: 2.1
-Name: aimped
-Version: 0.1.51
-Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.aimped.ai/
-Author: Russell C.
-Author-email: russell@aimped.com
-Maintainer: aimped
-Maintainer-email: contact@aimped.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **aimped**
-![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
+Metadata-Version: 2.1
+Name: aimped
+Version: 0.1.52
+Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
+Home-page: https://dev.aimped.ai/
+Author: Russell C.
+Author-email: russell@aimped.com
+Maintainer: aimped
+Maintainer-email: contact@aimped.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
+
+
```

### Comparing `aimped-0.1.51/README.md` & `aimped-0.1.52/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# **aimped**
-![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
```

### Comparing `aimped-0.1.51/aimped/model/load.py` & `aimped-0.1.52/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/nlp/assertion.py` & `aimped-0.1.52/aimped/nlp/assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/nlp/chunker.py` & `aimped-0.1.52/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/nlp/deid.py` & `aimped-0.1.52/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/nlp/ner.py` & `aimped-0.1.52/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/nlp/ner_cls_report.py` & `aimped-0.1.52/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/nlp/pipeline.py` & `aimped-0.1.52/aimped/nlp/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,16 +142,15 @@
         merged_results = RegexModelOutputMerger(regex_json_files_path_list=regex_json_files_path_list,
                                                 model_results=model_results,
                                                 text=text,
                                                 white_label_list=white_label_list)
         return merged_results
 
     def relation_result(self, sentences, ner_chunk_results, relation_classifier,
-                        ner_white_label_list, relation_white_label_list, one_to_many=True,
-                        one_label=None, return_svg=False):
+                        relation_white_label_list, relation_pairs, return_svg=False):
         """It returns the relation results of a text.
         parameters:
         ----------------
         sentences: list of str
         ner_chunk_results: list of dict
         relation_classifier: str
         ner_white_label_list: list of str
@@ -163,26 +162,21 @@
         ----------------
         results: list of dict
         """
         from aimped.nlp.relation import RelationResults, RelationAnnotateSentence
         results = RelationResults(sentences=sentences,
                                   ner_chunk_results=ner_chunk_results,
                                   relation_classifier=relation_classifier,
-                                  ner_white_label_list=ner_white_label_list,
                                   relation_white_label_list=relation_white_label_list,
-                                  one_to_many=one_to_many,
-                                  one_label=one_label,
+                                  relation_pairs =relation_pairs,
                                   return_svg=return_svg)
         return results
 
  
    
 
     def __str__(self) -> str:
         """Return the string representation of the pipeline."""
         return f"Pipeline(model={self.model}, tokenizer={self.tokenizer})"
 
 
-    def __str__(self) -> str:
-        """Return the string representation of the pipeline."""
-        return f"Pipeline(model={self.model}, tokenizer={self.tokenizer})"
```

### Comparing `aimped-0.1.51/aimped/nlp/regex_parser.py` & `aimped-0.1.52/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/nlp/relation.py` & `aimped-0.1.52/aimped/nlp/relation.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,26 +30,24 @@
         df['sentence'][a2_end:]
     ])
 
     return df['new_sentence']
 
 
 def RelationResults(sentences, ner_chunk_results, relation_classifier,
-                    ner_white_label_list, relation_white_label_list, one_to_many,
-                    one_label, return_svg):
+                    relation_white_label_list, relation_pairs, return_svg):
     """It returns the relation results of a text.
     parameters:
     ----------------
     sentences: list of str
     ner_chunk_results: list of dict
     relation_classifier: str
     ner_white_label_list: list of str
     relation_white_label_list: list of str
-    one_to_many: bool
-    one_label: str
+    relation_pairs: list of tuple
     return_svg: bool
     return:
     ----------------
     results: list of dict
     """
     import itertools
     import pandas as pd
@@ -73,20 +71,16 @@
                 df['firstCharEnt2'] = df[1].apply(lambda x: x[2])
                 df['lastCharEnt2'] = df[1].apply(lambda x: x[3])
                 df['entity2'] = df[1].apply(lambda x: x[0])
                 df['chunk2'] = df[1].apply(lambda x: x[1])
                 df['sent_begin2'] = df[1].apply(lambda x: x[-2])
                 df['sent_end2'] = df[1].apply(lambda x: x[-1])
 
-                if one_to_many:
-                    df = df[((df.entity1 == one_label) | (df.entity2 == one_label))]
-                    df = df[~((df.entity1 == one_label) & (df.entity2 == one_label))]
-                else:
-                    for ner_label in ner_white_label_list:
-                        df = df[~((df.entity1 == ner_label) & (df.entity2 == ner_label))]
+                df = df[df.apply(lambda row: any((row['entity1'], row['entity2']) == item for item in relation_pairs), axis=1)]
+
 
                 if len(df) != 0:
                     df['sentID'] = i
                     df['sentence'] = sentences[i]
                     df = df.drop([0, 1], axis=1)
                     df['new_sentence'] = np.nan
                     df['new_sentence'] = df.apply(RelationAnnotateSentence, axis=1)
```

### Comparing `aimped-0.1.51/aimped/nlp/relation_visualizer.py` & `aimped-0.1.52/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/nlp/tokenizer.py` & `aimped-0.1.52/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/nlp/tools.py` & `aimped-0.1.52/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/test/test_assertion.py` & `aimped-0.1.52/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/test/test_chunk_merger.py` & `aimped-0.1.52/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/test/test_deid_pipeline.py` & `aimped-0.1.52/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/test/test_ner_results.py` & `aimped-0.1.52/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/test/test_regex_parser.py` & `aimped-0.1.52/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/test/test_relation_pipeline.py` & `aimped-0.1.52/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/test/test_tokenizer.py` & `aimped-0.1.52/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/test/test_translation_pipeline.py` & `aimped-0.1.52/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped/utils.py` & `aimped-0.1.52/aimped/utils.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/aimped.egg-info/PKG-INFO` & `aimped-0.1.52/aimped.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-Metadata-Version: 2.1
-Name: aimped
-Version: 0.1.51
-Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.aimped.ai/
-Author: Russell C.
-Author-email: russell@aimped.com
-Maintainer: aimped
-Maintainer-email: contact@aimped.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **aimped**
-![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
+Metadata-Version: 2.1
+Name: aimped
+Version: 0.1.52
+Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
+Home-page: https://dev.aimped.ai/
+Author: Russell C.
+Author-email: russell@aimped.com
+Maintainer: aimped
+Maintainer-email: contact@aimped.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
+
+
```

### Comparing `aimped-0.1.51/aimped.egg-info/SOURCES.txt` & `aimped-0.1.52/aimped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimped-0.1.51/setup.py` & `aimped-0.1.52/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,10 +28,10 @@
     url="https://dev.aimped.ai/", 
     
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
 )
```

