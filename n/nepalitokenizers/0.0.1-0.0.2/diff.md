# Comparing `tmp/nepalitokenizers-0.0.1.tar.gz` & `tmp/nepalitokenizers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepalitokenizers-0.0.1.tar", last modified: Fri Jun 23 22:51:32 2023, max compression
+gzip compressed data, was "nepalitokenizers-0.0.2.tar", last modified: Sat Jun 24 00:06:52 2023, max compression
```

## Comparing `nepalitokenizers-0.0.1.tar` & `nepalitokenizers-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:51:32.167289 nepalitokenizers-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 22:51:22.000000 nepalitokenizers-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-06-23 22:51:32.167289 nepalitokenizers-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-06-23 22:51:22.000000 nepalitokenizers-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-23 22:51:22.000000 nepalitokenizers-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 22:51:32.167289 nepalitokenizers-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:51:32.163289 nepalitokenizers-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:51:32.167289 nepalitokenizers-0.0.1/src/nepalitokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 22:51:22.000000 nepalitokenizers-0.0.1/src/nepalitokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-23 22:51:22.000000 nepalitokenizers-0.0.1/src/nepalitokenizers/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:51:32.167289 nepalitokenizers-0.0.1/src/nepalitokenizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-06-23 22:51:32.000000 nepalitokenizers-0.0.1/src/nepalitokenizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-23 22:51:32.000000 nepalitokenizers-0.0.1/src/nepalitokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:51:32.000000 nepalitokenizers-0.0.1/src/nepalitokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 22:51:32.000000 nepalitokenizers-0.0.1/src/nepalitokenizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 22:51:32.000000 nepalitokenizers-0.0.1/src/nepalitokenizers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:51:32.167289 nepalitokenizers-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-23 22:51:22.000000 nepalitokenizers-0.0.1/tests/test_tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:06:52.910411 nepalitokenizers-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-24 00:06:37.000000 nepalitokenizers-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-24 00:06:52.910411 nepalitokenizers-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-24 00:06:37.000000 nepalitokenizers-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-24 00:06:37.000000 nepalitokenizers-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 00:06:52.910411 nepalitokenizers-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:06:52.906411 nepalitokenizers-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:06:52.906411 nepalitokenizers-0.0.2/src/nepalitokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-24 00:06:37.000000 nepalitokenizers-0.0.2/src/nepalitokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:06:52.910411 nepalitokenizers-0.0.2/src/nepalitokenizers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)  2300536 2023-06-24 00:06:37.000000 nepalitokenizers-0.0.2/src/nepalitokenizers/models/SentencePiece.json
+-rw-r--r--   0 runner    (1001) docker     (123)   892328 2023-06-24 00:06:37.000000 nepalitokenizers-0.0.2/src/nepalitokenizers/models/WordPiece.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-24 00:06:37.000000 nepalitokenizers-0.0.2/src/nepalitokenizers/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:06:52.906411 nepalitokenizers-0.0.2/src/nepalitokenizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-24 00:06:52.000000 nepalitokenizers-0.0.2/src/nepalitokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-24 00:06:52.000000 nepalitokenizers-0.0.2/src/nepalitokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 00:06:52.000000 nepalitokenizers-0.0.2/src/nepalitokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-24 00:06:52.000000 nepalitokenizers-0.0.2/src/nepalitokenizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-24 00:06:52.000000 nepalitokenizers-0.0.2/src/nepalitokenizers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:06:52.910411 nepalitokenizers-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-24 00:06:37.000000 nepalitokenizers-0.0.2/tests/test_tokenizers.py
```

### Comparing `nepalitokenizers-0.0.1/LICENSE` & `nepalitokenizers-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nepalitokenizers-0.0.1/PKG-INFO` & `nepalitokenizers-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepalitokenizers
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pre-trained Tokenizers for the Nepali language with an interface to HuggingFace's tokenizers library for customizability.
 Author-email: Soyuj Jung Basnet <bsoyuj@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/basnetsoyuj/nepali-tokenizers
 Project-URL: Bug Tracker, https://github.com/basnetsoyuj/nepali-tokenizers/issues
 Keywords: nepali,tokenizer,NLP,wordpiece,sentencepiece,huggingface,transformers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nepali Tokenizers
 
-[![LICENSE](https://img.shields.io/badge/license-Apache--2.0-blue)](./LICENSE) [![Build and Release](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml/badge.svg)](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml)
+[![Build and Release](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml/badge.svg)](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml) ![GitHub tag (latest SemVer pre-release)](https://img.shields.io/github/v/tag/basnetsoyuj/nepali-tokenizers?label=Version) [![LICENSE](https://img.shields.io/badge/License-Apache--2.0-blue)](./LICENSE) 
+
 
 This package provides access to pre-trained __WordPiece__ and __SentencePiece__ (Unigram) tokenizers for Nepali language, trained using HuggingFace's `tokenizers` library. It is a simple and short Python package tailored specifically for Nepali language with a default set of configurations for the normalizer, pre-tokenizer, post-processor, and decoder. 
 
 It delegates further customization by providing an interface to HuggingFace's `Tokenizer` pipeline, allowing users to adapt the tokenizers according to their requirements.
 
 
 ## Installation
```

### Comparing `nepalitokenizers-0.0.1/README.md` & `nepalitokenizers-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Nepali Tokenizers
 
-[![LICENSE](https://img.shields.io/badge/license-Apache--2.0-blue)](./LICENSE) [![Build and Release](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml/badge.svg)](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml)
+[![Build and Release](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml/badge.svg)](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml) ![GitHub tag (latest SemVer pre-release)](https://img.shields.io/github/v/tag/basnetsoyuj/nepali-tokenizers?label=Version) [![LICENSE](https://img.shields.io/badge/License-Apache--2.0-blue)](./LICENSE) 
+
 
 This package provides access to pre-trained __WordPiece__ and __SentencePiece__ (Unigram) tokenizers for Nepali language, trained using HuggingFace's `tokenizers` library. It is a simple and short Python package tailored specifically for Nepali language with a default set of configurations for the normalizer, pre-tokenizer, post-processor, and decoder. 
 
 It delegates further customization by providing an interface to HuggingFace's `Tokenizer` pipeline, allowing users to adapt the tokenizers according to their requirements.
 
 
 ## Installation
```

### Comparing `nepalitokenizers-0.0.1/pyproject.toml` & `nepalitokenizers-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"nepalitokenizers.models" = ["*.json"]
+
 [project]
 name = "nepalitokenizers"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Soyuj Jung Basnet", email="bsoyuj@gmail.com" },
 ]
 description = "Pre-trained Tokenizers for the Nepali language with an interface to HuggingFace's tokenizers library for customizability."
 readme = "README.md"
 license = {text = "Apache-2.0"}
 requires-python = ">=3.5"
```

### Comparing `nepalitokenizers-0.0.1/src/nepalitokenizers/tokenizers.py` & `nepalitokenizers-0.0.2/src/nepalitokenizers/tokenizers.py`

 * *Files identical despite different names*

### Comparing `nepalitokenizers-0.0.1/src/nepalitokenizers.egg-info/PKG-INFO` & `nepalitokenizers-0.0.2/src/nepalitokenizers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepalitokenizers
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pre-trained Tokenizers for the Nepali language with an interface to HuggingFace's tokenizers library for customizability.
 Author-email: Soyuj Jung Basnet <bsoyuj@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/basnetsoyuj/nepali-tokenizers
 Project-URL: Bug Tracker, https://github.com/basnetsoyuj/nepali-tokenizers/issues
 Keywords: nepali,tokenizer,NLP,wordpiece,sentencepiece,huggingface,transformers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nepali Tokenizers
 
-[![LICENSE](https://img.shields.io/badge/license-Apache--2.0-blue)](./LICENSE) [![Build and Release](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml/badge.svg)](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml)
+[![Build and Release](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml/badge.svg)](https://github.com/basnetsoyuj/nepali-tokenizers/actions/workflows/build.yml) ![GitHub tag (latest SemVer pre-release)](https://img.shields.io/github/v/tag/basnetsoyuj/nepali-tokenizers?label=Version) [![LICENSE](https://img.shields.io/badge/License-Apache--2.0-blue)](./LICENSE) 
+
 
 This package provides access to pre-trained __WordPiece__ and __SentencePiece__ (Unigram) tokenizers for Nepali language, trained using HuggingFace's `tokenizers` library. It is a simple and short Python package tailored specifically for Nepali language with a default set of configurations for the normalizer, pre-tokenizer, post-processor, and decoder. 
 
 It delegates further customization by providing an interface to HuggingFace's `Tokenizer` pipeline, allowing users to adapt the tokenizers according to their requirements.
 
 
 ## Installation
```

### Comparing `nepalitokenizers-0.0.1/tests/test_tokenizers.py` & `nepalitokenizers-0.0.2/tests/test_tokenizers.py`

 * *Files identical despite different names*

