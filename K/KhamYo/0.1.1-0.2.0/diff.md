# Comparing `tmp/KhamYo-0.1.1.tar.gz` & `tmp/KhamYo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KhamYo-0.1.1.tar", last modified: Fri Nov 26 18:52:22 2021, max compression
+gzip compressed data, was "KhamYo-0.2.0.tar", last modified: Sat Jun 24 05:13:50 2023, max compression
```

## Comparing `KhamYo-0.1.1.tar` & `KhamYo-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-26 18:52:22.667563 KhamYo-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-26 18:52:22.667563 KhamYo-0.1.1/KhamYo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3563 2021-11-26 18:52:22.000000 KhamYo-0.1.1/KhamYo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      255 2021-11-26 18:52:22.000000 KhamYo-0.1.1/KhamYo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-26 18:52:22.000000 KhamYo-0.1.1/KhamYo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-26 18:52:22.000000 KhamYo-0.1.1/KhamYo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-11-26 18:52:22.000000 KhamYo-0.1.1/KhamYo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-11-26 18:52:22.000000 KhamYo-0.1.1/KhamYo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-11-26 18:52:07.000000 KhamYo-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3563 2021-11-26 18:52:22.667563 KhamYo-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2472 2021-11-26 18:52:07.000000 KhamYo-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-26 18:52:22.667563 KhamYo-0.1.1/khamyo/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-11-26 18:52:07.000000 KhamYo-0.1.1/khamyo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2021-11-26 18:52:07.000000 KhamYo-0.1.1/khamyo/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    27343 2021-11-26 18:52:07.000000 KhamYo-0.1.1/khamyo/data.json
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-26 18:52:22.667563 KhamYo-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2021-11-26 18:52:07.000000 KhamYo-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:13:50.554971 KhamYo-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:13:50.554971 KhamYo-0.2.0/KhamYo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-24 05:13:50.000000 KhamYo-0.2.0/KhamYo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-24 05:13:50.000000 KhamYo-0.2.0/KhamYo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 05:13:50.000000 KhamYo-0.2.0/KhamYo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 05:13:50.000000 KhamYo-0.2.0/KhamYo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-24 05:13:50.000000 KhamYo-0.2.0/KhamYo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 05:13:50.000000 KhamYo-0.2.0/KhamYo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-24 05:13:38.000000 KhamYo-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-24 05:13:50.554971 KhamYo-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-24 05:13:38.000000 KhamYo-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:13:50.554971 KhamYo-0.2.0/khamyo/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-24 05:13:38.000000 KhamYo-0.2.0/khamyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-24 05:13:38.000000 KhamYo-0.2.0/khamyo/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28948 2023-06-24 05:13:38.000000 KhamYo-0.2.0/khamyo/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 05:13:50.554971 KhamYo-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-24 05:13:38.000000 KhamYo-0.2.0/setup.py
```

### Comparing `KhamYo-0.1.1/KhamYo.egg-info/PKG-INFO` & `KhamYo-0.2.0/KhamYo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: KhamYo
-Version: 0.1.1
+Version: 0.2.0
 Summary: Thai abbreviation to full text library
 Home-page: https://github.com/wannaphong/KhamYo
 Author: Wannaphong Phatthiyaphaibun
 Author-email: wannaphong@yahoo.com
 License: Apache Software License 2.0
 Project-URL: Source Code, https://github.com/wannaphong/KhamYo
 Project-URL: Bug Tracker, https://github.com/wannaphong/KhamYo/issues
 Keywords: NLP,natural language processing,text analytics,text processing,localization,computational linguistics,ThaiNLP,Thai NLP,Thai language
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Thai
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing
@@ -75,9 +74,7 @@
     title        = {{KhamYo: Thai abbreviation to full text tool}},
     month        = July,
     year         = 2021,
     publisher    = {GitHub},
     url          = {https://github.com/wannaphong/KhamYo}
 }
 ```
-
-
```

### Comparing `KhamYo-0.1.1/LICENSE` & `KhamYo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `KhamYo-0.1.1/PKG-INFO` & `KhamYo-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: KhamYo
-Version: 0.1.1
+Version: 0.2.0
 Summary: Thai abbreviation to full text library
 Home-page: https://github.com/wannaphong/KhamYo
 Author: Wannaphong Phatthiyaphaibun
 Author-email: wannaphong@yahoo.com
 License: Apache Software License 2.0
 Project-URL: Source Code, https://github.com/wannaphong/KhamYo
 Project-URL: Bug Tracker, https://github.com/wannaphong/KhamYo/issues
 Keywords: NLP,natural language processing,text analytics,text processing,localization,computational linguistics,ThaiNLP,Thai NLP,Thai language
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Thai
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing
@@ -75,9 +74,7 @@
     title        = {{KhamYo: Thai abbreviation to full text tool}},
     month        = July,
     year         = 2021,
     publisher    = {GitHub},
     url          = {https://github.com/wannaphong/KhamYo}
 }
 ```
-
-
```

### Comparing `KhamYo-0.1.1/README.md` & `KhamYo-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `KhamYo-0.1.1/khamyo/core.py` & `KhamYo-0.2.0/khamyo/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 import numpy as np
 from pythainlp.tokenize import Tokenizer
 from pythainlp.corpus import thai_words
 from khamyo import __file__ as khamyo_file
 
 path_file = os.path.join(os.path.dirname(khamyo_file),'data.json')
 
-model = SentenceTransformer('airesearch/wangchanberta-base-att-spm-uncased')
+model = SentenceTransformer('kornwtp/ConGen-WangchanBERT-Small')
 
 with open(path_file, encoding='utf-8') as fh:
     worddict = json.load(fh)
 
 list_th = list(worddict.keys())
-tokenizer = Tokenizer(list_th+list(thai_words()), engine='newmm', keep_whitespace="False")
+tokenizer = Tokenizer(list_th+list(thai_words()), engine='newmm')
 
 
 def merge(l: list) -> list:
   list_sent = []
   temp = ""
   for i in l:
     if i not in list_th:
```

### Comparing `KhamYo-0.1.1/khamyo/data.json` & `KhamYo-0.2.0/khamyo/data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9479755178907723%*

 * *Differences: {"'ตร.ม.'": "['ตารางเมตร', 'ตารางไมล์']",*

 * * "'ตร.รฟ.'": "['ตำรวจรถไฟ']",*

 * * "'ตร.ว.'": "['ตารางวา']",*

 * * "'ตร.ส.'": "['ตำรวจสันติบาล']",*

 * * "'ตร.สข.'": "['ตำรวจสุนัข']",*

 * * "'ตรอ.'": "['ตรวจสภาพรถเอกชน']",*

 * * "'ทูลเกล้าฯ'": "['ทูลเกล้าทูลกระหม่อม']",*

 * * "'ธ.ก.ส.'": "['ธนาคารเพื่อการเกษตรและสหกรณ์การเกษตร']",*

 * * "'ธ.บ.'": "['ธรรมศาสตรบัณฑิต']",*

 * * "'ธกท.'": "['ธนาคารกสิกรไทยจำกัด']",*

 * * "'ธปท.'": "['ธนาคารแห่งประเทศไทย']",*

 * * "'ธร.'": "['กรมธนารักษ์']",*

 * * "'ธสอ.'": "['ธนาคารเพื่อการส่งออกและนำเข้าแห่งประเทศไทย']",*

 * * "'น.'": "{inse […]*

```diff
@@ -224,14 +224,33 @@
     "\u0e15.\u0e0a.\u0e14.": [
         "\u0e15\u0e33\u0e23\u0e27\u0e08\u0e15\u0e23\u0e30\u0e40\u0e27\u0e19\u0e0a\u0e32\u0e22\u0e41\u0e14\u0e19"
     ],
     "\u0e15\u0e23.": [
         "\u0e15\u0e33\u0e23\u0e27\u0e08",
         "\u0e15\u0e32\u0e23\u0e32\u0e07"
     ],
+    "\u0e15\u0e23.\u0e21.": [
+        "\u0e15\u0e32\u0e23\u0e32\u0e07\u0e40\u0e21\u0e15\u0e23",
+        "\u0e15\u0e32\u0e23\u0e32\u0e07\u0e44\u0e21\u0e25\u0e4c"
+    ],
+    "\u0e15\u0e23.\u0e23\u0e1f.": [
+        "\u0e15\u0e33\u0e23\u0e27\u0e08\u0e23\u0e16\u0e44\u0e1f"
+    ],
+    "\u0e15\u0e23.\u0e27.": [
+        "\u0e15\u0e32\u0e23\u0e32\u0e07\u0e27\u0e32"
+    ],
+    "\u0e15\u0e23.\u0e2a.": [
+        "\u0e15\u0e33\u0e23\u0e27\u0e08\u0e2a\u0e31\u0e19\u0e15\u0e34\u0e1a\u0e32\u0e25"
+    ],
+    "\u0e15\u0e23.\u0e2a\u0e02.": [
+        "\u0e15\u0e33\u0e23\u0e27\u0e08\u0e2a\u0e38\u0e19\u0e31\u0e02"
+    ],
+    "\u0e15\u0e23\u0e2d.": [
+        "\u0e15\u0e23\u0e27\u0e08\u0e2a\u0e20\u0e32\u0e1e\u0e23\u0e16\u0e40\u0e2d\u0e01\u0e0a\u0e19"
+    ],
     "\u0e15\u0e25\u0e17.": [
         "\u0e15\u0e25\u0e32\u0e14\u0e2b\u0e25\u0e31\u0e01\u0e17\u0e23\u0e31\u0e1e\u0e22\u0e4c\u0e41\u0e2b\u0e48\u0e07\u0e1b\u0e23\u0e30\u0e40\u0e17\u0e28\u0e44\u0e17\u0e22"
     ],
     "\u0e16.": [
         "\u0e16\u0e19\u0e19"
     ],
     "\u0e17.\u0e0d.": [
@@ -264,32 +283,61 @@
     ],
     "\u0e17\u0e2a.": [
         "\u0e01\u0e23\u0e30\u0e17\u0e23\u0e27\u0e07\u0e17\u0e23\u0e31\u0e1e\u0e22\u0e32\u0e01\u0e23\u0e18\u0e23\u0e23\u0e21\u0e0a\u0e32\u0e15\u0e34\u0e41\u0e25\u0e30\u0e2a\u0e34\u0e48\u0e07\u0e41\u0e27\u0e14\u0e25\u0e49\u0e2d\u0e21"
     ],
     "\u0e17\u0e2d.": [
         "\u0e17\u0e2b\u0e32\u0e23\u0e2d\u0e32\u0e01\u0e32\u0e28"
     ],
+    "\u0e17\u0e39\u0e25\u0e40\u0e01\u0e25\u0e49\u0e32\u0e2f": [
+        "\u0e17\u0e39\u0e25\u0e40\u0e01\u0e25\u0e49\u0e32\u0e17\u0e39\u0e25\u0e01\u0e23\u0e30\u0e2b\u0e21\u0e48\u0e2d\u0e21"
+    ],
+    "\u0e18.\u0e01.\u0e2a.": [
+        "\u0e18\u0e19\u0e32\u0e04\u0e32\u0e23\u0e40\u0e1e\u0e37\u0e48\u0e2d\u0e01\u0e32\u0e23\u0e40\u0e01\u0e29\u0e15\u0e23\u0e41\u0e25\u0e30\u0e2a\u0e2b\u0e01\u0e23\u0e13\u0e4c\u0e01\u0e32\u0e23\u0e40\u0e01\u0e29\u0e15\u0e23"
+    ],
     "\u0e18.\u0e04.": [
         "\u0e18\u0e31\u0e19\u0e27\u0e32\u0e04\u0e21"
     ],
+    "\u0e18.\u0e1a.": [
+        "\u0e18\u0e23\u0e23\u0e21\u0e28\u0e32\u0e2a\u0e15\u0e23\u0e1a\u0e31\u0e13\u0e11\u0e34\u0e15"
+    ],
+    "\u0e18\u0e01\u0e17.": [
+        "\u0e18\u0e19\u0e32\u0e04\u0e32\u0e23\u0e01\u0e2a\u0e34\u0e01\u0e23\u0e44\u0e17\u0e22\u0e08\u0e33\u0e01\u0e31\u0e14"
+    ],
+    "\u0e18\u0e1b\u0e17.": [
+        "\u0e18\u0e19\u0e32\u0e04\u0e32\u0e23\u0e41\u0e2b\u0e48\u0e07\u0e1b\u0e23\u0e30\u0e40\u0e17\u0e28\u0e44\u0e17\u0e22"
+    ],
+    "\u0e18\u0e23.": [
+        "\u0e01\u0e23\u0e21\u0e18\u0e19\u0e32\u0e23\u0e31\u0e01\u0e29\u0e4c"
+    ],
+    "\u0e18\u0e2a\u0e2d.": [
+        "\u0e18\u0e19\u0e32\u0e04\u0e32\u0e23\u0e40\u0e1e\u0e37\u0e48\u0e2d\u0e01\u0e32\u0e23\u0e2a\u0e48\u0e07\u0e2d\u0e2d\u0e01\u0e41\u0e25\u0e30\u0e19\u0e33\u0e40\u0e02\u0e49\u0e32\u0e41\u0e2b\u0e48\u0e07\u0e1b\u0e23\u0e30\u0e40\u0e17\u0e28\u0e44\u0e17\u0e22"
+    ],
     "\u0e18\u0e2d\u0e2a.": [
         "\u0e18\u0e19\u0e32\u0e04\u0e32\u0e23\u0e2d\u0e32\u0e04\u0e32\u0e23\u0e2a\u0e07\u0e40\u0e04\u0e23\u0e32\u0e30\u0e2b\u0e4c"
     ],
     "\u0e19.": [
-        "\u0e19\u0e32\u0e2c\u0e34\u0e01\u0e32"
+        "\u0e19\u0e32\u0e2c\u0e34\u0e01\u0e32",
+        "\u0e04\u0e33\u0e19\u0e32\u0e21",
+        "\u0e17\u0e34\u0e28\u0e40\u0e2b\u0e19\u0e37\u0e2d",
+        "\u0e19\u0e34\u0e49\u0e27",
+        "\u0e41\u0e21\u0e48\u0e19\u0e49\u0e33",
+        "\u0e2b\u0e19\u0e49\u0e32"
     ],
     "\u0e19.\u0e0a.": [
         "\u0e19\u0e31\u0e01\u0e42\u0e17\u0e29\u0e0a\u0e32\u0e22"
     ],
     "\u0e19.\u0e0d.": [
         "\u0e19\u0e31\u0e01\u0e42\u0e17\u0e29\u0e2b\u0e0d\u0e34\u0e07"
     ],
     "\u0e19.\u0e19.": [
         "\u0e19\u0e49\u0e33\u0e2b\u0e19\u0e31\u0e01"
     ],
+    "\u0e19.\u0e1b.\u0e17.": [
+        "\u0e19\u0e32\u0e22\u0e44\u0e1b\u0e23\u0e29\u0e13\u0e35\u0e22\u0e4c\u0e42\u0e17\u0e23\u0e40\u0e25\u0e02"
+    ],
     "\u0e19.\u0e1e.": [
         "\u0e19\u0e32\u0e22\u0e41\u0e1e\u0e17\u0e22\u0e4c"
     ],
     "\u0e19.\u0e2a.": [
         "\u0e19\u0e32\u0e07\u0e2a\u0e32\u0e27"
     ],
     "\u0e19\u0e04\u0e1b.": [
@@ -298,14 +346,18 @@
     "\u0e19\u0e08\u0e2d.": [
         "\u0e19\u0e31\u0e01\u0e40\u0e23\u0e35\u0e22\u0e19\u0e08\u0e48\u0e32\u0e2d\u0e32\u0e01\u0e32\u0e28"
     ],
     "\u0e19\u0e19\u0e23.": [
         "\u0e19\u0e31\u0e01\u0e40\u0e23\u0e35\u0e22\u0e19\u0e19\u0e32\u0e22\u0e40\u0e23\u0e37\u0e2d",
         "\u0e19\u0e31\u0e01\u0e40\u0e23\u0e35\u0e22\u0e19\u0e19\u0e32\u0e22\u0e23\u0e49\u0e2d\u0e22"
     ],
+    "\u0e19\u0e1e\u0e17.": [
+        "\u0e19\u0e31\u0e01\u0e40\u0e23\u0e35\u0e22\u0e19\u0e41\u0e1e\u0e17\u0e22\u0e4c\u0e17\u0e2b\u0e32\u0e23",
+        "\u0e2b\u0e19\u0e48\u0e27\u0e22\u0e41\u0e1e\u0e17\u0e22\u0e4c\u0e40\u0e04\u0e25\u0e37\u0e48\u0e2d\u0e19\u0e17\u0e35\u0e48"
+    ],
     "\u0e19\u0e23": [
         "\u0e2a\u0e33\u0e19\u0e31\u0e01\u0e19\u0e32\u0e22\u0e01\u0e23\u0e31\u0e10\u0e21\u0e19\u0e15\u0e23\u0e35"
     ],
     "\u0e19\u0e23.": [
         "\u0e19\u0e31\u0e01\u0e40\u0e23\u0e35\u0e22\u0e19"
     ],
     "\u0e19\u0e28.": [
@@ -580,14 +632,17 @@
     ],
     "\u0e21.\u0e28.": [
         "\u0e21\u0e2b\u0e32\u0e28\u0e31\u0e01\u0e23\u0e32\u0e0a"
     ],
     "\u0e21\u0e02.": [
         "\u0e21\u0e2b\u0e32\u0e27\u0e34\u0e17\u0e22\u0e32\u0e25\u0e31\u0e22\u0e02\u0e2d\u0e19\u0e41\u0e01\u0e48\u0e19"
     ],
+    "\u0e21\u0e02.\u0e27\u0e19\u0e04.": [
+        "\u0e21\u0e2b\u0e32\u0e27\u0e34\u0e17\u0e22\u0e32\u0e25\u0e31\u0e22\u0e02\u0e2d\u0e19\u0e41\u0e01\u0e48\u0e19 \u0e27\u0e34\u0e17\u0e22\u0e32\u0e40\u0e02\u0e15\u0e2b\u0e19\u0e2d\u0e07\u0e04\u0e32\u0e22"
+    ],
     "\u0e21\u0e0a.": [
         "\u0e21\u0e2b\u0e32\u0e27\u0e34\u0e17\u0e22\u0e32\u0e25\u0e31\u0e22\u0e40\u0e0a\u0e35\u0e22\u0e07\u0e43\u0e2b\u0e21\u0e48"
     ],
     "\u0e21\u0e17.": [
         "\u0e01\u0e23\u0e30\u0e17\u0e23\u0e27\u0e07\u0e21\u0e2b\u0e32\u0e14\u0e44\u0e17\u0e22"
     ],
     "\u0e21\u0e17\u0e2a.": [
@@ -708,14 +763,17 @@
     ],
     "\u0e27\u0e17.\u0e1a.": [
         "\u0e27\u0e34\u0e17\u0e22\u0e32\u0e28\u0e32\u0e2a\u0e15\u0e23\u0e1a\u0e31\u0e13\u0e11\u0e34\u0e15"
     ],
     "\u0e27\u0e18.": [
         "\u0e01\u0e23\u0e30\u0e17\u0e23\u0e27\u0e07\u0e27\u0e31\u0e12\u0e19\u0e18\u0e23\u0e23\u0e21"
     ],
+    "\u0e27\u0e19\u0e04.": [
+        "\u0e27\u0e34\u0e17\u0e22\u0e32\u0e40\u0e02\u0e15\u0e2b\u0e19\u0e2d\u0e07\u0e04\u0e32\u0e22"
+    ],
     "\u0e27\u0e1b\u0e2d.": [
         "\u0e27\u0e34\u0e17\u0e22\u0e32\u0e25\u0e31\u0e22\u0e1b\u0e49\u0e2d\u0e07\u0e01\u0e31\u0e19\u0e23\u0e32\u0e0a\u0e2d\u0e32\u0e13\u0e32\u0e08\u0e31\u0e01\u0e23"
     ],
     "\u0e27\u0e27.": [
         "\u0e2a\u0e16\u0e32\u0e1a\u0e31\u0e19\u0e27\u0e34\u0e08\u0e31\u0e22\u0e27\u0e34\u0e17\u0e22\u0e32\u0e28\u0e32\u0e2a\u0e15\u0e23\u0e4c\u0e41\u0e25\u0e30\u0e40\u0e17\u0e04\u0e42\u0e19\u0e42\u0e25\u0e22\u0e35\u0e41\u0e2b\u0e48\u0e07\u0e1b\u0e23\u0e30\u0e40\u0e17\u0e28\u0e44\u0e17\u0e22"
     ],
     "\u0e27\u0e2d\u0e28.": [
@@ -981,14 +1039,17 @@
     ],
     "\u0e2d\u0e08.": [
         "\u0e2d\u0e32\u0e08\u0e32\u0e23\u0e22\u0e4c"
     ],
     "\u0e2d\u0e15.": [
         "\u0e01\u0e23\u0e21\u0e2d\u0e38\u0e15\u0e38\u0e19\u0e34\u0e22\u0e21\u0e27\u0e34\u0e17\u0e22\u0e32"
     ],
+    "\u0e2d\u0e19.": [
+        "\u0e2d\u0e07\u0e04\u0e4c\u0e01\u0e32\u0e23\u0e19\u0e31\u0e01\u0e28\u0e36\u0e01\u0e29\u0e32"
+    ],
     "\u0e2d\u0e1a\u0e08.": [
         "\u0e2d\u0e07\u0e04\u0e4c\u0e01\u0e32\u0e23\u0e1a\u0e23\u0e34\u0e2b\u0e32\u0e23\u0e2a\u0e48\u0e27\u0e19\u0e08\u0e31\u0e07\u0e2b\u0e27\u0e31\u0e14"
     ],
     "\u0e2d\u0e1a\u0e15.": [
         "\u0e2d\u0e07\u0e04\u0e4c\u0e01\u0e32\u0e23\u0e1a\u0e23\u0e34\u0e2b\u0e32\u0e23\u0e2a\u0e48\u0e27\u0e19\u0e15\u0e33\u0e1a\u0e25"
     ],
     "\u0e2d\u0e1e\u0e0a.": [
```

### Comparing `KhamYo-0.1.1/setup.py` & `KhamYo-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 requirements = [
-    "pythainlp>=2.2",
+    "pythainlp>=4.0",
     "sentence-transformers",
-    "transformers"
+    "transformers",
+    "sentencepiece"
 ]
 
 with open('README.md','r',encoding='utf-8-sig') as f:
     readme = f.read()
 
 setup(
     name="KhamYo",
-    version="0.1.1",
+    version="0.2.0",
     description="Thai abbreviation to full text library",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Wannaphong Phatthiyaphaibun",
     author_email="wannaphong@yahoo.com",
     url="https://github.com/wannaphong/KhamYo",
     packages=find_packages(exclude=["tests", "tests.*"]),
@@ -53,8 +54,8 @@
         "Topic :: Text Processing :: General",
         "Topic :: Text Processing :: Linguistic",
     ],
     project_urls={
         "Source Code": "https://github.com/wannaphong/KhamYo",
         "Bug Tracker": "https://github.com/wannaphong/KhamYo/issues",
     },
-)
+)
```

