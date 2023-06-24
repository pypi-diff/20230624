# Comparing `tmp/ConversationAgent-0.5.4.tar.gz` & `tmp/ConversationAgent-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConversationAgent-0.5.4.tar", last modified: Sun Dec 12 19:17:04 2021, max compression
+gzip compressed data, was "ConversationAgent-0.5.8.tar", last modified: Sat Jun 24 12:43:52 2023, max compression
```

## Comparing `ConversationAgent-0.5.4.tar` & `ConversationAgent-0.5.8.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2021-12-12 19:17:04.532083 ConversationAgent-0.5.4/
-drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2021-12-12 19:17:04.474767 ConversationAgent-0.5.4/ConversationAgent/
--rw-r--r--   0 thetawang   (501) staff       (20)    15504 2021-11-04 19:27:35.000000 ConversationAgent-0.5.4/ConversationAgent/LibStage.py
--rw-r--r--   0 thetawang   (501) staff       (20)     8893 2021-09-26 09:38:20.000000 ConversationAgent-0.5.4/ConversationAgent/README.md
--rw-r--r--   0 thetawang   (501) staff       (20)     4561 2021-07-07 08:26:10.000000 ConversationAgent-0.5.4/ConversationAgent/SentenceStage.py
--rw-r--r--   0 thetawang   (501) staff       (20)     4747 2021-10-25 17:27:44.000000 ConversationAgent-0.5.4/ConversationAgent/__agent__.py
--rw-r--r--   0 thetawang   (501) staff       (20)     1299 2021-08-06 02:02:28.000000 ConversationAgent-0.5.4/ConversationAgent/__init__.py
--rw-r--r--   0 thetawang   (501) staff       (20)     9541 2021-12-12 19:16:43.000000 ConversationAgent-0.5.4/ConversationAgent/__stage__.py
--rw-r--r--   0 thetawang   (501) staff       (20)      688 2021-08-06 02:36:39.000000 ConversationAgent-0.5.4/ConversationAgent/__tool__.py
-drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2021-12-12 19:17:04.477219 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/
--rw-r--r--   0 thetawang   (501) staff       (20)      285 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/README.md
--rw-r--r--   0 thetawang   (501) staff       (20)    18754 2021-07-07 08:45:22.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/__init__.py
--rw-r--r--   0 thetawang   (501) staff       (20)     2371 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/__main__.py
--rw-r--r--   0 thetawang   (501) staff       (20)     1222 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/_compat.py
-drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2021-12-12 19:17:04.504595 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/analyse/
--rwxr-xr-x   0 thetawang   (501) staff       (20)      501 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/analyse/__init__.py
--rw-r--r--   0 thetawang   (501) staff       (20)     1403 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/analyse/analyzer.py
--rw-r--r--   0 thetawang   (501) staff       (20)  6200957 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/analyse/idf.txt
--rw-r--r--   0 thetawang   (501) staff       (20)     3757 2021-07-07 07:49:20.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/analyse/textrank.py
--rwxr-xr-x   0 thetawang   (501) staff       (20)     4313 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/analyse/tfidf.py
--rw-r--r--   0 thetawang   (501) staff       (20)  4154486 2021-07-07 01:55:22.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/dict.txt
-drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2021-12-12 19:17:04.508671 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/finalseg/
--rw-r--r--   0 thetawang   (501) staff       (20)     2397 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/finalseg/__init__.py
--rw-r--r--   0 thetawang   (501) staff       (20)   864307 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/finalseg/prob_emit.py
--rw-r--r--   0 thetawang   (501) staff       (20)       92 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/finalseg/prob_start.py
--rw-r--r--   0 thetawang   (501) staff       (20)      243 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/finalseg/prob_trans.py
-drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2021-12-12 19:17:04.528991 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/
--rw-r--r--   0 thetawang   (501) staff       (20)     9007 2021-07-07 08:44:31.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/__init__.py
--rw-r--r--   0 thetawang   (501) staff       (20)  1618015 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/char_state_tab.py
--rw-r--r--   0 thetawang   (501) staff       (20)  3987090 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/prob_emit.py
--rw-r--r--   0 thetawang   (501) staff       (20)     7204 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/prob_start.py
--rw-r--r--   0 thetawang   (501) staff       (20)   247312 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/prob_trans.py
--rw-r--r--   0 thetawang   (501) staff       (20)     1610 2021-06-24 06:30:54.000000 ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/viterbi.py
--rw-r--r--   0 thetawang   (501) staff       (20)     1418 2021-08-24 05:23:38.000000 ConversationAgent-0.5.4/ConversationAgent/nlp_tool.py
-drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2021-12-12 19:17:04.531366 ConversationAgent-0.5.4/ConversationAgent/test/
--rw-r--r--   0 thetawang   (501) staff       (20)        0 2021-08-13 03:54:21.000000 ConversationAgent-0.5.4/ConversationAgent/test/__init__.py
--rw-r--r--   0 thetawang   (501) staff       (20)    16488 2021-10-24 05:11:59.000000 ConversationAgent-0.5.4/ConversationAgent/test/__test_v1__.py
--rw-r--r--   0 thetawang   (501) staff       (20)     2787 2021-08-13 05:51:09.000000 ConversationAgent-0.5.4/ConversationAgent/test/__test_v2__.py
--rw-r--r--   0 thetawang   (501) staff       (20)     8482 2021-10-24 05:06:47.000000 ConversationAgent-0.5.4/ConversationAgent/test/__test_v3__.py
--rw-r--r--   0 thetawang   (501) staff       (20)     1290 2021-08-24 02:38:09.000000 ConversationAgent-0.5.4/ConversationAgent/test/__test_v4__.py
--rw-r--r--   0 thetawang   (501) staff       (20)     2541 2021-08-24 05:34:39.000000 ConversationAgent-0.5.4/ConversationAgent/test/__test_v5__.py
--rw-r--r--   0 thetawang   (501) staff       (20)     2552 2021-10-24 10:59:09.000000 ConversationAgent-0.5.4/ConversationAgent/test/__test_v6__.py
--rw-r--r--   0 thetawang   (501) staff       (20)     1612 2021-10-24 10:47:21.000000 ConversationAgent-0.5.4/ConversationAgent/test/__test_v7__.py
-drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2021-12-12 19:17:04.475687 ConversationAgent-0.5.4/ConversationAgent.egg-info/
--rw-r--r--   0 thetawang   (501) staff       (20)    11371 2021-12-12 19:17:04.000000 ConversationAgent-0.5.4/ConversationAgent.egg-info/PKG-INFO
--rw-r--r--   0 thetawang   (501) staff       (20)     1658 2021-12-12 19:17:04.000000 ConversationAgent-0.5.4/ConversationAgent.egg-info/SOURCES.txt
--rw-r--r--   0 thetawang   (501) staff       (20)        1 2021-12-12 19:17:04.000000 ConversationAgent-0.5.4/ConversationAgent.egg-info/dependency_links.txt
--rw-r--r--   0 thetawang   (501) staff       (20)        1 2021-07-29 02:48:55.000000 ConversationAgent-0.5.4/ConversationAgent.egg-info/not-zip-safe
--rw-r--r--   0 thetawang   (501) staff       (20)       18 2021-12-12 19:17:04.000000 ConversationAgent-0.5.4/ConversationAgent.egg-info/top_level.txt
--rw-r--r--   0 thetawang   (501) staff       (20)    11371 2021-12-12 19:17:04.531869 ConversationAgent-0.5.4/PKG-INFO
--rw-r--r--   0 thetawang   (501) staff       (20)       38 2021-12-12 19:17:04.532133 ConversationAgent-0.5.4/setup.cfg
--rw-r--r--   0 thetawang   (501) staff       (20)      544 2021-12-12 19:16:59.000000 ConversationAgent-0.5.4/setup.py
+drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2023-06-24 12:43:52.649637 ConversationAgent-0.5.8/
+drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2023-06-24 12:43:52.607379 ConversationAgent-0.5.8/ConversationAgent/
+-rw-r--r--   0 thetawang   (501) staff       (20)    15504 2023-06-24 12:01:13.000000 ConversationAgent-0.5.8/ConversationAgent/LibStage.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     8893 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/README.md
+-rw-r--r--   0 thetawang   (501) staff       (20)     4561 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/SentenceStage.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     4747 2023-06-24 12:01:10.000000 ConversationAgent-0.5.8/ConversationAgent/__agent__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     1322 2023-06-24 12:26:23.000000 ConversationAgent-0.5.8/ConversationAgent/__init__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     9541 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/__stage__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)      688 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/__tool__.py
+drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2023-06-24 12:43:52.609167 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/
+-rw-r--r--   0 thetawang   (501) staff       (20)      285 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/README.md
+-rw-r--r--   0 thetawang   (501) staff       (20)    18754 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/__init__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     2371 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/__main__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     1222 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/_compat.py
+drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2023-06-24 12:43:52.627798 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/analyse/
+-rwxr-xr-x   0 thetawang   (501) staff       (20)      501 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/analyse/__init__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     1403 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/analyse/analyzer.py
+-rw-r--r--   0 thetawang   (501) staff       (20)  6200957 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/analyse/idf.txt
+-rw-r--r--   0 thetawang   (501) staff       (20)     3757 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/analyse/textrank.py
+-rwxr-xr-x   0 thetawang   (501) staff       (20)     4313 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/analyse/tfidf.py
+-rw-r--r--   0 thetawang   (501) staff       (20)  4154486 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/dict.txt
+drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2023-06-24 12:43:52.632912 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/finalseg/
+-rw-r--r--   0 thetawang   (501) staff       (20)     2397 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/finalseg/__init__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)   864307 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/finalseg/prob_emit.py
+-rw-r--r--   0 thetawang   (501) staff       (20)       92 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/finalseg/prob_start.py
+-rw-r--r--   0 thetawang   (501) staff       (20)      243 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/finalseg/prob_trans.py
+drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2023-06-24 12:43:52.646695 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/
+-rw-r--r--   0 thetawang   (501) staff       (20)     9007 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/__init__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)  1618015 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/char_state_tab.py
+-rw-r--r--   0 thetawang   (501) staff       (20)  3987090 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/prob_emit.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     7204 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/prob_start.py
+-rw-r--r--   0 thetawang   (501) staff       (20)   247312 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/prob_trans.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     1610 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/viterbi.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     1418 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/nlp_tool.py
+drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2023-06-24 12:43:52.649155 ConversationAgent-0.5.8/ConversationAgent/test/
+-rw-r--r--   0 thetawang   (501) staff       (20)        0 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/test/__init__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)    16488 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/test/__test_v1__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     2787 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/test/__test_v2__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     8482 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/test/__test_v3__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     1290 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/test/__test_v4__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     2541 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/test/__test_v5__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     2552 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/test/__test_v6__.py
+-rw-r--r--   0 thetawang   (501) staff       (20)     1612 2023-06-24 09:01:58.000000 ConversationAgent-0.5.8/ConversationAgent/test/__test_v7__.py
+drwxr-xr-x   0 thetawang   (501) staff       (20)        0 2023-06-24 12:43:52.608274 ConversationAgent-0.5.8/ConversationAgent.egg-info/
+-rw-r--r--   0 thetawang   (501) staff       (20)     9099 2023-06-24 12:43:52.000000 ConversationAgent-0.5.8/ConversationAgent.egg-info/PKG-INFO
+-rw-r--r--   0 thetawang   (501) staff       (20)     1668 2023-06-24 12:43:52.000000 ConversationAgent-0.5.8/ConversationAgent.egg-info/SOURCES.txt
+-rw-r--r--   0 thetawang   (501) staff       (20)        1 2023-06-24 12:43:52.000000 ConversationAgent-0.5.8/ConversationAgent.egg-info/dependency_links.txt
+-rw-r--r--   0 thetawang   (501) staff       (20)        1 2023-06-24 12:14:23.000000 ConversationAgent-0.5.8/ConversationAgent.egg-info/not-zip-safe
+-rw-r--r--   0 thetawang   (501) staff       (20)       18 2023-06-24 12:43:52.000000 ConversationAgent-0.5.8/ConversationAgent.egg-info/top_level.txt
+-rw-r--r--   0 thetawang   (501) staff       (20)     9099 2023-06-24 12:43:52.649474 ConversationAgent-0.5.8/PKG-INFO
+-rw-r--r--   0 thetawang   (501) staff       (20)      346 2023-06-24 12:26:23.000000 ConversationAgent-0.5.8/README.md
+-rw-r--r--   0 thetawang   (501) staff       (20)       38 2023-06-24 12:43:52.649678 ConversationAgent-0.5.8/setup.cfg
+-rw-r--r--   0 thetawang   (501) staff       (20)      544 2023-06-24 12:43:43.000000 ConversationAgent-0.5.8/setup.py
```

### Comparing `ConversationAgent-0.5.4/ConversationAgent/LibStage.py` & `ConversationAgent-0.5.8/ConversationAgent/LibStage.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/README.md` & `ConversationAgent-0.5.8/ConversationAgent/README.md`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/SentenceStage.py` & `ConversationAgent-0.5.8/ConversationAgent/SentenceStage.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/__agent__.py` & `ConversationAgent-0.5.8/ConversationAgent/__agent__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/__init__.py` & `ConversationAgent-0.5.8/ConversationAgent/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import uuid
 import re
 
 from .__agent__ import Agent
 from .__stage__ import Stage, __USER_TEXT__, __SYS_REPLY__, StageStatus, \
     __LOCAL_VAR_LABEL__, __LOCAL_VAR_VALUE__
 
+__version__ = "0.1.10"
 __MOCK_STAGES_LABEL_1__ = "__MOCK_STAGES_LABEL_1__"
 
 
 def mock_client_with_test(agent, says, tests):
     data = {}
     for s, t in zip(says, tests):
         data[__USER_TEXT__] = s
```

### Comparing `ConversationAgent-0.5.4/ConversationAgent/__stage__.py` & `ConversationAgent-0.5.8/ConversationAgent/__stage__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/__tool__.py` & `ConversationAgent-0.5.8/ConversationAgent/__tool__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/__init__.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/__init__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/__main__.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/__main__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/_compat.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/_compat.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/analyse/analyzer.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/analyse/analyzer.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/analyse/idf.txt` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/analyse/idf.txt`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/analyse/textrank.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/analyse/textrank.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/analyse/tfidf.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/analyse/tfidf.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/dict.txt` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/dict.txt`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/finalseg/__init__.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/finalseg/__init__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/finalseg/prob_emit.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/finalseg/prob_emit.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/__init__.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/__init__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/char_state_tab.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/char_state_tab.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/prob_emit.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/prob_emit.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/prob_start.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/prob_start.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/prob_trans.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/prob_trans.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/jieba_zh/posseg/viterbi.py` & `ConversationAgent-0.5.8/ConversationAgent/jieba_zh/posseg/viterbi.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/nlp_tool.py` & `ConversationAgent-0.5.8/ConversationAgent/nlp_tool.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/test/__test_v1__.py` & `ConversationAgent-0.5.8/ConversationAgent/test/__test_v1__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/test/__test_v2__.py` & `ConversationAgent-0.5.8/ConversationAgent/test/__test_v2__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/test/__test_v3__.py` & `ConversationAgent-0.5.8/ConversationAgent/test/__test_v3__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/test/__test_v4__.py` & `ConversationAgent-0.5.8/ConversationAgent/test/__test_v4__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/test/__test_v5__.py` & `ConversationAgent-0.5.8/ConversationAgent/test/__test_v5__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/test/__test_v6__.py` & `ConversationAgent-0.5.8/ConversationAgent/test/__test_v6__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent/test/__test_v7__.py` & `ConversationAgent-0.5.8/ConversationAgent/test/__test_v7__.py`

 * *Files identical despite different names*

### Comparing `ConversationAgent-0.5.4/ConversationAgent.egg-info/PKG-INFO` & `ConversationAgent-0.5.8/ConversationAgent.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,288 +1,286 @@
 Metadata-Version: 2.1
 Name: ConversationAgent
-Version: 0.5.4
+Version: 0.5.8
 Summary: ConversationAgent
 Home-page: https://github.com/Chunshan-Theta/ConversationAgent
 Author: Theta
-License: UNKNOWN
-Description: ## 說明
-        不需資料庫之對話腳本代理。
-        
-        ## agent
-        `agent`可以透過Json來產生對話核心，為此我們有一個接口可以使用
-        ```
-        from ConversationAgent.LibStage import gen_agent
-        from ConversationAgent import to_bot
-        ```
-        - 透過"ConversationAgent.LibStage.gen_agent"方法來建置機器人
-        - 透過"ConversationAgent.to_bot"方式與機器人溝通
-            - 該方法需要三個參數
-                - agent代理物件: gen_agent 產生
-                - text: 使用者輸入內容，字串內容
-                - data: 過場資訊，預設使用`{}`空字典，第二次與之後溝通應該戴上 `to_bot` 回傳的資料。
-            - 該方法會回傳機器人回應與過場資訊，下次溝通保留該過場資訊在進行溝通。
-            
-        ### Quick start
-        ```
-        from ConversationAgent.LibStage import gen_agent
-        import ConversationAgent
-        bot = {
-            "__MAIN_STAGES__": [
-                {
-                    "stage_type": "__QA_STAGE__",
-                    "qa_threshold": 1,
-                    "__STAGE_NAME__": "__開始階段__",
-                    "__SYS_QUESTION__": {
-                        "__SYS_WELCOME__": "歡迎句",
-                        "__SYS_REFUSE__": "拒絕句",
-                        "__SYS_COMPLETE__": "完成句"
-                    },
-                    "corpus": {
-                        "早安": "1",
-                        "午安": "2",
-                        "晚安": "3"
-                    },
-                    "__SAVED_NAME__": {
-                        QAStage.__QA_RESPOND__: "QA_r1",
-                        QAStage.__QA_RESPOND_THRESHOLD__: "QA_th",
-                        QAStage.__QA_RESPOND_QUESTION__: "QA_q1",
-                        QAStage.__QA_RESPOND_SCORE__: "QA_s1",
-                        QAStage.__RUNNING_CORPUS__: "QA_c1",
-                    },
-                    "__DISABLE_WELCOME__": False
-                }
-            ]
-        }
-        print(f"\n" * 5)
-        
-        agent = gen_agent(bot)
-        data = {}
-        reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
-        print(f"reply_text: {reply_text}， ")
-        reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
-        print(f"reply_text: {reply_text}， ")
-        reply_text, data = ConversationAgent.to_bot(agent, "早安", data)
-        print(f"reply_text: {reply_text}， ")
-        ```
-        
-        ## Stage 種類
-        ### RE_STAGE
-        
-        RE_STAGE 採用`stage_type`為`__RE_STAGE__`，是用於最基礎的對話階段，由兩個主要結構構成：
-        1. `__SYS_QUESTION__`: 用來設定該階段的回應句，回應句有三種類型
-           * 歡迎句: 第一次到該階段時，機器人會回應該句子。(可依需求關閉功能，`DISSABLE_WELCOME`設為`True`就關閉，預設為`False`。)
-           * 拒絕句: 當沒有滿足抓取到所有`is_fits`部分所要求的變數時，機器人會回應該句子。
-           * 完成句: 以上都完成時，機器人會回應該句子。(可透過`%%`包裹變數名稱，並以`空格`前後相隔後，調用該變數。)
-        
-        2. is_fits: 透過`正規表達式(regular expression)`從使用者的輸入句子來抓取變數，該變數會儲存起來提供給`完成句`和 `SWITCH_STAGE`使用。
-        
-        選用設定:
-        1. `__STAGE_NAME__`: 這是選用設定。 可以設定每個stage的獨特名稱，名稱不可重複。
-        2. `__SYS_WELCOME__`、`__SYS_REFUSE__`、`__SYS_COMPLETE__`的回應句可以設定成文字陣列，若設為陣列則會隨機取用。
-        ```
+Description-Content-Type: text/markdown
+
+## 說明
+不需資料庫之對話腳本代理。
+
+## agent
+`agent`可以透過Json來產生對話核心，為此我們有一個接口可以使用
+```
+from ConversationAgent.LibStage import gen_agent
+from ConversationAgent import to_bot
+```
+- 透過"ConversationAgent.LibStage.gen_agent"方法來建置機器人
+- 透過"ConversationAgent.to_bot"方式與機器人溝通
+    - 該方法需要三個參數
+        - agent代理物件: gen_agent 產生
+        - text: 使用者輸入內容，字串內容
+        - data: 過場資訊，預設使用`{}`空字典，第二次與之後溝通應該戴上 `to_bot` 回傳的資料。
+    - 該方法會回傳機器人回應與過場資訊，下次溝通保留該過場資訊在進行溝通。
+    
+### Quick start
+```
+from ConversationAgent.LibStage import gen_agent
+import ConversationAgent
+bot = {
+    "__MAIN_STAGES__": [
         {
-            "stage_type": "__RE_STAGE__",
+            "stage_type": "__QA_STAGE__",
+            "qa_threshold": 1,
             "__STAGE_NAME__": "__開始階段__",
             "__SYS_QUESTION__": {
                 "__SYS_WELCOME__": "歡迎句",
                 "__SYS_REFUSE__": "拒絕句",
                 "__SYS_COMPLETE__": "完成句"
             },
-            "is_fits": [
-                [".*", "YOUSAYS"]
-            ],
-            "__DISABLE_WELCOME__": False,
-            "__DISABLE_REFUSE__": False
-        }
-        ```
-        
-        ### SWITCH_STAGE
-        
-        SWITCH_STAGE 採用`stage_type`為`__LIB_SWITCH_STAGE__`，用於在`Agent`不同路線切換，主要結構是`stages_filter`。 stages_filter用來設定切換路線的條件，用`[]`可包含帶多種條件多路線，每一條件單位由`變數名稱`、`限定數值`和 `切換路線`三部分組成。
-        
-        以下說明主要幾種設置方式:
-        * 無條件設定:
-            ```
-            [
-                ["*",True,"_新路線1_"]
-            ]
-            ```
-        * 單一條件設定:
-            ```
-            [
-                ["_VAR_","VALUE1","_新路線1_"],
-                ["_VAR_","VALUE2","_新路線2_"]
-            ]
-            ```
-        * 多條件設定:
-            ```
-            [
-                [["_VAR1_","_VAR2_"],["VALUE1","VALUE2"],"_新路線1_"],
-                [["_VAR1_","_VAR2_"],["VALUE3","VALUE4"],"_新路線2_"],
-            ]
-            ```
-        * 混合條件設定:
-            ```
-            [
-                ["_VAR1_","VALUE1","_新路線1_"],
-                [["_VAR1_","_VAR2_"],["VALUE3","VALUE4"],"_新路線2_"],
-                ["*",True,"_新路線3_"]
-            ]
-            ```
-        * 非`=`之條件設定:
-            ```
-            [
-                ["_VAR1_",0.95,"_新路線1_",">="]
-            ]
-            ```
-          
-        * 多重非`=`之條件設定:
-            ```
-            [
-                [["_VAR1_","_VAR2_"],[0.1,0.56],"_新路線1_",[">=","<"]]
-            ]
-            ```
-          
-        **儲存變數方式是透過`RE_STAGE`的 `is_fits`來執行。
-        
-        範例：
-        ```
-        {
-            "stage_type": "__LIB_SWITCH_STAGE__",
-            "stages_filter": [
-                ["VAR","我想要的數值","_成功路線_"],,
-                ["*",True,"_失敗路線_"]
-            ]
-        
-        }
-        ```
-        
-        ### QA_STAGE
-        QA_STAGE 採用`stage_type`為`__QA_STAGE__`，是通過`相似度`來決定回應的一種階段，主要有三個部分的組成。
-        1. says: 用來設定該階段的回應句，回應句有三種類型
-           * 歡迎句: 第一次到該階段時，機器人會回應該句子。(可依需求關閉功能，`DISSABLE_WELCOME`設為`True`就關閉，預設為`False`。)
-           * 拒絕句: 當相似分數低於`qa_threshold`時，機器人會回應該句子。(可依需求關閉功能，`__DISABLE_REFUSE__`設為`True`就關閉，預設為`False`。)
-           * 完成句: 以上都完成時，機器人會回應該句子。(可透過`%%`包裹變數名稱，並以`空格`前後相隔後，調用該變數。)
-        
-        2. corpus: 使用者的輸入會與該字典的所有`key`進行比對，並儲存相關結果，相關結果包含：
-            * `__QA_RESPOND_QUESTION__`: 相似值最高的 key
-            * `__QA_RESPOND__`: 相似值最高的 key 對應之 value
-            * `__QA_RESPOND_SCORE__`: 相似值最高的數值
-            * `__RUNNING_CORPUS__`: 該次測試時使用的 corpus
-            * `__QA_RESPOND_THRESHOLD__`: 該次測試使用的 threshold
-            
-        3. `__SAVED_NAME__`: 設定儲存之變數的名稱，方便使用。
-        
-        
-        ```
-         {
-            "stage_type": "__QA_STAGE__",
-            "qa_threshold": 1,
-            "says": {
-                "sys_welcome": "歡迎句",
-                "sys_refuse": "拒絕句",
-                "sys_complete": "完成句"
-            },
             "corpus": {
                 "早安": "1",
                 "午安": "2",
                 "晚安": "3"
             },
             "__SAVED_NAME__": {
-                "__QA_RESPOND__": "QA_r1",
-                "__QA_RESPOND_THRESHOLD__": "QA_th",
-                "__QA_RESPOND_QUESTION__": "QA_q1",
-                "__QA_RESPOND_SCORE__": "QA_s1",
-                "__RUNNING_CORPUS__": "QA_c1",
+                QAStage.__QA_RESPOND__: "QA_r1",
+                QAStage.__QA_RESPOND_THRESHOLD__: "QA_th",
+                QAStage.__QA_RESPOND_QUESTION__: "QA_q1",
+                QAStage.__QA_RESPOND_SCORE__: "QA_s1",
+                QAStage.__RUNNING_CORPUS__: "QA_c1",
             },
-            "__DISABLE_WELCOME__": False,
-            "__DISABLE_REFUSE__": False,
+            "__DISABLE_WELCOME__": False
         }
-        ```
-        
-        
-        
-        ## More Examples
-        
-        # 飲料店
-        ```
-        bot = {
-            "__MAIN_STAGES__": [
-                {
-                    "stage_type": "__RE_STAGE__",
-                    "question": {
-                        "sys_welcome": "歡迎來到飲料店，請輸入您要的東西 紅茶/綠茶 少冰/去冰",
-                        "sys_refuse": "不完全輸入 %%drink_type%% %%ice_type%% ",
-                        "sys_complete": "你輸入的內容是 %%drink_type%% %%ice_type%% "
-                    },
-                    "is_fits": [
-                        ["(紅茶|綠茶)+", "drink_type"],
-                        ["(少冰|去冰)+", "ice_type"],
-        
-                    ]
-                },
-                {
-                    "stage_type": "__LIB_SWITCH_STAGE__",
-                    "stages_filter": [
-                        [["drink_type", "ice_type"], ["綠茶", "去冰"], "_新路線1_"],
-                        ["*", True, "_新路線2_"]
-                    ]
-        
-                }
-            ],
-            "_新路線1_": [
-                {
-                    "stage_type": "__RE_STAGE__",
-                    "question": {
-                        "sys_welcome": "",
-                        "sys_refuse": "",
-                        "sys_complete": "切換分之成功1"
-                    },
-                    "__DISSABLE_Q1__": True
-                },
-            ],
-            "_新路線2_": [
-                {
-                    "stage_type": "__RE_STAGE__",
-                    "question": {
-                        "sys_welcome": "",
-                        "sys_refuse": "",
-                        "sys_complete": "切換分之成功2"
-                    },
-                    "__DISSABLE_Q1__": True
-                },
+    ]
+}
+print(f"\n" * 5)
+
+agent = gen_agent(bot)
+data = {}
+reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
+print(f"reply_text: {reply_text}， ")
+reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
+print(f"reply_text: {reply_text}， ")
+reply_text, data = ConversationAgent.to_bot(agent, "早安", data)
+print(f"reply_text: {reply_text}， ")
+```
+
+## Stage 種類
+### RE_STAGE
+
+RE_STAGE 採用`stage_type`為`__RE_STAGE__`，是用於最基礎的對話階段，由兩個主要結構構成：
+1. `__SYS_QUESTION__`: 用來設定該階段的回應句，回應句有三種類型
+   * 歡迎句: 第一次到該階段時，機器人會回應該句子。(可依需求關閉功能，`DISSABLE_WELCOME`設為`True`就關閉，預設為`False`。)
+   * 拒絕句: 當沒有滿足抓取到所有`is_fits`部分所要求的變數時，機器人會回應該句子。
+   * 完成句: 以上都完成時，機器人會回應該句子。(可透過`%%`包裹變數名稱，並以`空格`前後相隔後，調用該變數。)
+
+2. is_fits: 透過`正規表達式(regular expression)`從使用者的輸入句子來抓取變數，該變數會儲存起來提供給`完成句`和 `SWITCH_STAGE`使用。
+
+選用設定:
+1. `__STAGE_NAME__`: 這是選用設定。 可以設定每個stage的獨特名稱，名稱不可重複。
+2. `__SYS_WELCOME__`、`__SYS_REFUSE__`、`__SYS_COMPLETE__`的回應句可以設定成文字陣列，若設為陣列則會隨機取用。
+```
+{
+    "stage_type": "__RE_STAGE__",
+    "__STAGE_NAME__": "__開始階段__",
+    "__SYS_QUESTION__": {
+        "__SYS_WELCOME__": "歡迎句",
+        "__SYS_REFUSE__": "拒絕句",
+        "__SYS_COMPLETE__": "完成句"
+    },
+    "is_fits": [
+        [".*", "YOUSAYS"]
+    ],
+    "__DISABLE_WELCOME__": False,
+    "__DISABLE_REFUSE__": False
+}
+```
+
+### SWITCH_STAGE
+
+SWITCH_STAGE 採用`stage_type`為`__LIB_SWITCH_STAGE__`，用於在`Agent`不同路線切換，主要結構是`stages_filter`。 stages_filter用來設定切換路線的條件，用`[]`可包含帶多種條件多路線，每一條件單位由`變數名稱`、`限定數值`和 `切換路線`三部分組成。
+
+以下說明主要幾種設置方式:
+* 無條件設定:
+    ```
+    [
+        ["*",True,"_新路線1_"]
+    ]
+    ```
+* 單一條件設定:
+    ```
+    [
+        ["_VAR_","VALUE1","_新路線1_"],
+        ["_VAR_","VALUE2","_新路線2_"]
+    ]
+    ```
+* 多條件設定:
+    ```
+    [
+        [["_VAR1_","_VAR2_"],["VALUE1","VALUE2"],"_新路線1_"],
+        [["_VAR1_","_VAR2_"],["VALUE3","VALUE4"],"_新路線2_"],
+    ]
+    ```
+* 混合條件設定:
+    ```
+    [
+        ["_VAR1_","VALUE1","_新路線1_"],
+        [["_VAR1_","_VAR2_"],["VALUE3","VALUE4"],"_新路線2_"],
+        ["*",True,"_新路線3_"]
+    ]
+    ```
+* 非`=`之條件設定:
+    ```
+    [
+        ["_VAR1_",0.95,"_新路線1_",">="]
+    ]
+    ```
+  
+* 多重非`=`之條件設定:
+    ```
+    [
+        [["_VAR1_","_VAR2_"],[0.1,0.56],"_新路線1_",[">=","<"]]
+    ]
+    ```
+  
+**儲存變數方式是透過`RE_STAGE`的 `is_fits`來執行。
+
+範例：
+```
+{
+    "stage_type": "__LIB_SWITCH_STAGE__",
+    "stages_filter": [
+        ["VAR","我想要的數值","_成功路線_"],,
+        ["*",True,"_失敗路線_"]
+    ]
+
+}
+```
+
+### QA_STAGE
+QA_STAGE 採用`stage_type`為`__QA_STAGE__`，是通過`相似度`來決定回應的一種階段，主要有三個部分的組成。
+1. says: 用來設定該階段的回應句，回應句有三種類型
+   * 歡迎句: 第一次到該階段時，機器人會回應該句子。(可依需求關閉功能，`DISSABLE_WELCOME`設為`True`就關閉，預設為`False`。)
+   * 拒絕句: 當相似分數低於`qa_threshold`時，機器人會回應該句子。(可依需求關閉功能，`__DISABLE_REFUSE__`設為`True`就關閉，預設為`False`。)
+   * 完成句: 以上都完成時，機器人會回應該句子。(可透過`%%`包裹變數名稱，並以`空格`前後相隔後，調用該變數。)
+
+2. corpus: 使用者的輸入會與該字典的所有`key`進行比對，並儲存相關結果，相關結果包含：
+    * `__QA_RESPOND_QUESTION__`: 相似值最高的 key
+    * `__QA_RESPOND__`: 相似值最高的 key 對應之 value
+    * `__QA_RESPOND_SCORE__`: 相似值最高的數值
+    * `__RUNNING_CORPUS__`: 該次測試時使用的 corpus
+    * `__QA_RESPOND_THRESHOLD__`: 該次測試使用的 threshold
+    
+3. `__SAVED_NAME__`: 設定儲存之變數的名稱，方便使用。
+
+
+```
+ {
+    "stage_type": "__QA_STAGE__",
+    "qa_threshold": 1,
+    "says": {
+        "sys_welcome": "歡迎句",
+        "sys_refuse": "拒絕句",
+        "sys_complete": "完成句"
+    },
+    "corpus": {
+        "早安": "1",
+        "午安": "2",
+        "晚安": "3"
+    },
+    "__SAVED_NAME__": {
+        "__QA_RESPOND__": "QA_r1",
+        "__QA_RESPOND_THRESHOLD__": "QA_th",
+        "__QA_RESPOND_QUESTION__": "QA_q1",
+        "__QA_RESPOND_SCORE__": "QA_s1",
+        "__RUNNING_CORPUS__": "QA_c1",
+    },
+    "__DISABLE_WELCOME__": False,
+    "__DISABLE_REFUSE__": False,
+}
+```
+
+
+
+## More Examples
+
+# 飲料店
+```
+bot = {
+    "__MAIN_STAGES__": [
+        {
+            "stage_type": "__RE_STAGE__",
+            "question": {
+                "sys_welcome": "歡迎來到飲料店，請輸入您要的東西 紅茶/綠茶 少冰/去冰",
+                "sys_refuse": "不完全輸入 %%drink_type%% %%ice_type%% ",
+                "sys_complete": "你輸入的內容是 %%drink_type%% %%ice_type%% "
+            },
+            "is_fits": [
+                ["(紅茶|綠茶)+", "drink_type"],
+                ["(少冰|去冰)+", "ice_type"],
+
+            ]
+        },
+        {
+            "stage_type": "__LIB_SWITCH_STAGE__",
+            "stages_filter": [
+                [["drink_type", "ice_type"], ["綠茶", "去冰"], "_新路線1_"],
+                ["*", True, "_新路線2_"]
             ]
+
         }
-        print(f"\n" * 5)
-        
-        agent = gen_agent(bot)
-        data = {}
-        reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
-        print(f"reply_text: {reply_text}， ")
-        reply_text, data = ConversationAgent.to_bot(agent, "紅茶", data)
-        print(f"reply_text: {reply_text}， ")
-        reply_text, data = ConversationAgent.to_bot(agent, "少冰", data)
-        print(f"reply_text: {reply_text}， ")
-        ```
-        
-        ## ToDo
-        
-        ~~* Switch除了等號以外的方法~~
-        
-        ~~* DISSABLE_WELCOME測試與勘誤名詞~~
-        
-        ~~* QAStage 停用拒絕句(無論分數都會通過)~~
-        
-        ~~* 多回應方式~~
-        
-        ~~* 設定階段名稱~~
-        
-        * 修正QAstage為相似度模型階段
-        * 分類型模型階段
-        * 繼承的範例
-        * 說明agent刪除變數的規則
-        
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+    ],
+    "_新路線1_": [
+        {
+            "stage_type": "__RE_STAGE__",
+            "question": {
+                "sys_welcome": "",
+                "sys_refuse": "",
+                "sys_complete": "切換分之成功1"
+            },
+            "__DISSABLE_Q1__": True
+        },
+    ],
+    "_新路線2_": [
+        {
+            "stage_type": "__RE_STAGE__",
+            "question": {
+                "sys_welcome": "",
+                "sys_refuse": "",
+                "sys_complete": "切換分之成功2"
+            },
+            "__DISSABLE_Q1__": True
+        },
+    ]
+}
+print(f"\n" * 5)
+
+agent = gen_agent(bot)
+data = {}
+reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
+print(f"reply_text: {reply_text}， ")
+reply_text, data = ConversationAgent.to_bot(agent, "紅茶", data)
+print(f"reply_text: {reply_text}， ")
+reply_text, data = ConversationAgent.to_bot(agent, "少冰", data)
+print(f"reply_text: {reply_text}， ")
+```
+
+## ToDo
+
+~~* Switch除了等號以外的方法~~
+
+~~* DISSABLE_WELCOME測試與勘誤名詞~~
+
+~~* QAStage 停用拒絕句(無論分數都會通過)~~
+
+~~* 多回應方式~~
+
+~~* 設定階段名稱~~
+
+* 修正QAstage為相似度模型階段
+* 分類型模型階段
+* 繼承的範例
+* 說明agent刪除變數的規則
+
+
```

### Comparing `ConversationAgent-0.5.4/ConversationAgent.egg-info/SOURCES.txt` & `ConversationAgent-0.5.8/ConversationAgent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 ConversationAgent/LibStage.py
 ConversationAgent/README.md
 ConversationAgent/SentenceStage.py
 ConversationAgent/__agent__.py
 ConversationAgent/__init__.py
 ConversationAgent/__stage__.py
```

### Comparing `ConversationAgent-0.5.4/PKG-INFO` & `ConversationAgent-0.5.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,288 +1,286 @@
 Metadata-Version: 2.1
 Name: ConversationAgent
-Version: 0.5.4
+Version: 0.5.8
 Summary: ConversationAgent
 Home-page: https://github.com/Chunshan-Theta/ConversationAgent
 Author: Theta
-License: UNKNOWN
-Description: ## 說明
-        不需資料庫之對話腳本代理。
-        
-        ## agent
-        `agent`可以透過Json來產生對話核心，為此我們有一個接口可以使用
-        ```
-        from ConversationAgent.LibStage import gen_agent
-        from ConversationAgent import to_bot
-        ```
-        - 透過"ConversationAgent.LibStage.gen_agent"方法來建置機器人
-        - 透過"ConversationAgent.to_bot"方式與機器人溝通
-            - 該方法需要三個參數
-                - agent代理物件: gen_agent 產生
-                - text: 使用者輸入內容，字串內容
-                - data: 過場資訊，預設使用`{}`空字典，第二次與之後溝通應該戴上 `to_bot` 回傳的資料。
-            - 該方法會回傳機器人回應與過場資訊，下次溝通保留該過場資訊在進行溝通。
-            
-        ### Quick start
-        ```
-        from ConversationAgent.LibStage import gen_agent
-        import ConversationAgent
-        bot = {
-            "__MAIN_STAGES__": [
-                {
-                    "stage_type": "__QA_STAGE__",
-                    "qa_threshold": 1,
-                    "__STAGE_NAME__": "__開始階段__",
-                    "__SYS_QUESTION__": {
-                        "__SYS_WELCOME__": "歡迎句",
-                        "__SYS_REFUSE__": "拒絕句",
-                        "__SYS_COMPLETE__": "完成句"
-                    },
-                    "corpus": {
-                        "早安": "1",
-                        "午安": "2",
-                        "晚安": "3"
-                    },
-                    "__SAVED_NAME__": {
-                        QAStage.__QA_RESPOND__: "QA_r1",
-                        QAStage.__QA_RESPOND_THRESHOLD__: "QA_th",
-                        QAStage.__QA_RESPOND_QUESTION__: "QA_q1",
-                        QAStage.__QA_RESPOND_SCORE__: "QA_s1",
-                        QAStage.__RUNNING_CORPUS__: "QA_c1",
-                    },
-                    "__DISABLE_WELCOME__": False
-                }
-            ]
-        }
-        print(f"\n" * 5)
-        
-        agent = gen_agent(bot)
-        data = {}
-        reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
-        print(f"reply_text: {reply_text}， ")
-        reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
-        print(f"reply_text: {reply_text}， ")
-        reply_text, data = ConversationAgent.to_bot(agent, "早安", data)
-        print(f"reply_text: {reply_text}， ")
-        ```
-        
-        ## Stage 種類
-        ### RE_STAGE
-        
-        RE_STAGE 採用`stage_type`為`__RE_STAGE__`，是用於最基礎的對話階段，由兩個主要結構構成：
-        1. `__SYS_QUESTION__`: 用來設定該階段的回應句，回應句有三種類型
-           * 歡迎句: 第一次到該階段時，機器人會回應該句子。(可依需求關閉功能，`DISSABLE_WELCOME`設為`True`就關閉，預設為`False`。)
-           * 拒絕句: 當沒有滿足抓取到所有`is_fits`部分所要求的變數時，機器人會回應該句子。
-           * 完成句: 以上都完成時，機器人會回應該句子。(可透過`%%`包裹變數名稱，並以`空格`前後相隔後，調用該變數。)
-        
-        2. is_fits: 透過`正規表達式(regular expression)`從使用者的輸入句子來抓取變數，該變數會儲存起來提供給`完成句`和 `SWITCH_STAGE`使用。
-        
-        選用設定:
-        1. `__STAGE_NAME__`: 這是選用設定。 可以設定每個stage的獨特名稱，名稱不可重複。
-        2. `__SYS_WELCOME__`、`__SYS_REFUSE__`、`__SYS_COMPLETE__`的回應句可以設定成文字陣列，若設為陣列則會隨機取用。
-        ```
+Description-Content-Type: text/markdown
+
+## 說明
+不需資料庫之對話腳本代理。
+
+## agent
+`agent`可以透過Json來產生對話核心，為此我們有一個接口可以使用
+```
+from ConversationAgent.LibStage import gen_agent
+from ConversationAgent import to_bot
+```
+- 透過"ConversationAgent.LibStage.gen_agent"方法來建置機器人
+- 透過"ConversationAgent.to_bot"方式與機器人溝通
+    - 該方法需要三個參數
+        - agent代理物件: gen_agent 產生
+        - text: 使用者輸入內容，字串內容
+        - data: 過場資訊，預設使用`{}`空字典，第二次與之後溝通應該戴上 `to_bot` 回傳的資料。
+    - 該方法會回傳機器人回應與過場資訊，下次溝通保留該過場資訊在進行溝通。
+    
+### Quick start
+```
+from ConversationAgent.LibStage import gen_agent
+import ConversationAgent
+bot = {
+    "__MAIN_STAGES__": [
         {
-            "stage_type": "__RE_STAGE__",
+            "stage_type": "__QA_STAGE__",
+            "qa_threshold": 1,
             "__STAGE_NAME__": "__開始階段__",
             "__SYS_QUESTION__": {
                 "__SYS_WELCOME__": "歡迎句",
                 "__SYS_REFUSE__": "拒絕句",
                 "__SYS_COMPLETE__": "完成句"
             },
-            "is_fits": [
-                [".*", "YOUSAYS"]
-            ],
-            "__DISABLE_WELCOME__": False,
-            "__DISABLE_REFUSE__": False
-        }
-        ```
-        
-        ### SWITCH_STAGE
-        
-        SWITCH_STAGE 採用`stage_type`為`__LIB_SWITCH_STAGE__`，用於在`Agent`不同路線切換，主要結構是`stages_filter`。 stages_filter用來設定切換路線的條件，用`[]`可包含帶多種條件多路線，每一條件單位由`變數名稱`、`限定數值`和 `切換路線`三部分組成。
-        
-        以下說明主要幾種設置方式:
-        * 無條件設定:
-            ```
-            [
-                ["*",True,"_新路線1_"]
-            ]
-            ```
-        * 單一條件設定:
-            ```
-            [
-                ["_VAR_","VALUE1","_新路線1_"],
-                ["_VAR_","VALUE2","_新路線2_"]
-            ]
-            ```
-        * 多條件設定:
-            ```
-            [
-                [["_VAR1_","_VAR2_"],["VALUE1","VALUE2"],"_新路線1_"],
-                [["_VAR1_","_VAR2_"],["VALUE3","VALUE4"],"_新路線2_"],
-            ]
-            ```
-        * 混合條件設定:
-            ```
-            [
-                ["_VAR1_","VALUE1","_新路線1_"],
-                [["_VAR1_","_VAR2_"],["VALUE3","VALUE4"],"_新路線2_"],
-                ["*",True,"_新路線3_"]
-            ]
-            ```
-        * 非`=`之條件設定:
-            ```
-            [
-                ["_VAR1_",0.95,"_新路線1_",">="]
-            ]
-            ```
-          
-        * 多重非`=`之條件設定:
-            ```
-            [
-                [["_VAR1_","_VAR2_"],[0.1,0.56],"_新路線1_",[">=","<"]]
-            ]
-            ```
-          
-        **儲存變數方式是透過`RE_STAGE`的 `is_fits`來執行。
-        
-        範例：
-        ```
-        {
-            "stage_type": "__LIB_SWITCH_STAGE__",
-            "stages_filter": [
-                ["VAR","我想要的數值","_成功路線_"],,
-                ["*",True,"_失敗路線_"]
-            ]
-        
-        }
-        ```
-        
-        ### QA_STAGE
-        QA_STAGE 採用`stage_type`為`__QA_STAGE__`，是通過`相似度`來決定回應的一種階段，主要有三個部分的組成。
-        1. says: 用來設定該階段的回應句，回應句有三種類型
-           * 歡迎句: 第一次到該階段時，機器人會回應該句子。(可依需求關閉功能，`DISSABLE_WELCOME`設為`True`就關閉，預設為`False`。)
-           * 拒絕句: 當相似分數低於`qa_threshold`時，機器人會回應該句子。(可依需求關閉功能，`__DISABLE_REFUSE__`設為`True`就關閉，預設為`False`。)
-           * 完成句: 以上都完成時，機器人會回應該句子。(可透過`%%`包裹變數名稱，並以`空格`前後相隔後，調用該變數。)
-        
-        2. corpus: 使用者的輸入會與該字典的所有`key`進行比對，並儲存相關結果，相關結果包含：
-            * `__QA_RESPOND_QUESTION__`: 相似值最高的 key
-            * `__QA_RESPOND__`: 相似值最高的 key 對應之 value
-            * `__QA_RESPOND_SCORE__`: 相似值最高的數值
-            * `__RUNNING_CORPUS__`: 該次測試時使用的 corpus
-            * `__QA_RESPOND_THRESHOLD__`: 該次測試使用的 threshold
-            
-        3. `__SAVED_NAME__`: 設定儲存之變數的名稱，方便使用。
-        
-        
-        ```
-         {
-            "stage_type": "__QA_STAGE__",
-            "qa_threshold": 1,
-            "says": {
-                "sys_welcome": "歡迎句",
-                "sys_refuse": "拒絕句",
-                "sys_complete": "完成句"
-            },
             "corpus": {
                 "早安": "1",
                 "午安": "2",
                 "晚安": "3"
             },
             "__SAVED_NAME__": {
-                "__QA_RESPOND__": "QA_r1",
-                "__QA_RESPOND_THRESHOLD__": "QA_th",
-                "__QA_RESPOND_QUESTION__": "QA_q1",
-                "__QA_RESPOND_SCORE__": "QA_s1",
-                "__RUNNING_CORPUS__": "QA_c1",
+                QAStage.__QA_RESPOND__: "QA_r1",
+                QAStage.__QA_RESPOND_THRESHOLD__: "QA_th",
+                QAStage.__QA_RESPOND_QUESTION__: "QA_q1",
+                QAStage.__QA_RESPOND_SCORE__: "QA_s1",
+                QAStage.__RUNNING_CORPUS__: "QA_c1",
             },
-            "__DISABLE_WELCOME__": False,
-            "__DISABLE_REFUSE__": False,
+            "__DISABLE_WELCOME__": False
         }
-        ```
-        
-        
-        
-        ## More Examples
-        
-        # 飲料店
-        ```
-        bot = {
-            "__MAIN_STAGES__": [
-                {
-                    "stage_type": "__RE_STAGE__",
-                    "question": {
-                        "sys_welcome": "歡迎來到飲料店，請輸入您要的東西 紅茶/綠茶 少冰/去冰",
-                        "sys_refuse": "不完全輸入 %%drink_type%% %%ice_type%% ",
-                        "sys_complete": "你輸入的內容是 %%drink_type%% %%ice_type%% "
-                    },
-                    "is_fits": [
-                        ["(紅茶|綠茶)+", "drink_type"],
-                        ["(少冰|去冰)+", "ice_type"],
-        
-                    ]
-                },
-                {
-                    "stage_type": "__LIB_SWITCH_STAGE__",
-                    "stages_filter": [
-                        [["drink_type", "ice_type"], ["綠茶", "去冰"], "_新路線1_"],
-                        ["*", True, "_新路線2_"]
-                    ]
-        
-                }
-            ],
-            "_新路線1_": [
-                {
-                    "stage_type": "__RE_STAGE__",
-                    "question": {
-                        "sys_welcome": "",
-                        "sys_refuse": "",
-                        "sys_complete": "切換分之成功1"
-                    },
-                    "__DISSABLE_Q1__": True
-                },
-            ],
-            "_新路線2_": [
-                {
-                    "stage_type": "__RE_STAGE__",
-                    "question": {
-                        "sys_welcome": "",
-                        "sys_refuse": "",
-                        "sys_complete": "切換分之成功2"
-                    },
-                    "__DISSABLE_Q1__": True
-                },
+    ]
+}
+print(f"\n" * 5)
+
+agent = gen_agent(bot)
+data = {}
+reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
+print(f"reply_text: {reply_text}， ")
+reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
+print(f"reply_text: {reply_text}， ")
+reply_text, data = ConversationAgent.to_bot(agent, "早安", data)
+print(f"reply_text: {reply_text}， ")
+```
+
+## Stage 種類
+### RE_STAGE
+
+RE_STAGE 採用`stage_type`為`__RE_STAGE__`，是用於最基礎的對話階段，由兩個主要結構構成：
+1. `__SYS_QUESTION__`: 用來設定該階段的回應句，回應句有三種類型
+   * 歡迎句: 第一次到該階段時，機器人會回應該句子。(可依需求關閉功能，`DISSABLE_WELCOME`設為`True`就關閉，預設為`False`。)
+   * 拒絕句: 當沒有滿足抓取到所有`is_fits`部分所要求的變數時，機器人會回應該句子。
+   * 完成句: 以上都完成時，機器人會回應該句子。(可透過`%%`包裹變數名稱，並以`空格`前後相隔後，調用該變數。)
+
+2. is_fits: 透過`正規表達式(regular expression)`從使用者的輸入句子來抓取變數，該變數會儲存起來提供給`完成句`和 `SWITCH_STAGE`使用。
+
+選用設定:
+1. `__STAGE_NAME__`: 這是選用設定。 可以設定每個stage的獨特名稱，名稱不可重複。
+2. `__SYS_WELCOME__`、`__SYS_REFUSE__`、`__SYS_COMPLETE__`的回應句可以設定成文字陣列，若設為陣列則會隨機取用。
+```
+{
+    "stage_type": "__RE_STAGE__",
+    "__STAGE_NAME__": "__開始階段__",
+    "__SYS_QUESTION__": {
+        "__SYS_WELCOME__": "歡迎句",
+        "__SYS_REFUSE__": "拒絕句",
+        "__SYS_COMPLETE__": "完成句"
+    },
+    "is_fits": [
+        [".*", "YOUSAYS"]
+    ],
+    "__DISABLE_WELCOME__": False,
+    "__DISABLE_REFUSE__": False
+}
+```
+
+### SWITCH_STAGE
+
+SWITCH_STAGE 採用`stage_type`為`__LIB_SWITCH_STAGE__`，用於在`Agent`不同路線切換，主要結構是`stages_filter`。 stages_filter用來設定切換路線的條件，用`[]`可包含帶多種條件多路線，每一條件單位由`變數名稱`、`限定數值`和 `切換路線`三部分組成。
+
+以下說明主要幾種設置方式:
+* 無條件設定:
+    ```
+    [
+        ["*",True,"_新路線1_"]
+    ]
+    ```
+* 單一條件設定:
+    ```
+    [
+        ["_VAR_","VALUE1","_新路線1_"],
+        ["_VAR_","VALUE2","_新路線2_"]
+    ]
+    ```
+* 多條件設定:
+    ```
+    [
+        [["_VAR1_","_VAR2_"],["VALUE1","VALUE2"],"_新路線1_"],
+        [["_VAR1_","_VAR2_"],["VALUE3","VALUE4"],"_新路線2_"],
+    ]
+    ```
+* 混合條件設定:
+    ```
+    [
+        ["_VAR1_","VALUE1","_新路線1_"],
+        [["_VAR1_","_VAR2_"],["VALUE3","VALUE4"],"_新路線2_"],
+        ["*",True,"_新路線3_"]
+    ]
+    ```
+* 非`=`之條件設定:
+    ```
+    [
+        ["_VAR1_",0.95,"_新路線1_",">="]
+    ]
+    ```
+  
+* 多重非`=`之條件設定:
+    ```
+    [
+        [["_VAR1_","_VAR2_"],[0.1,0.56],"_新路線1_",[">=","<"]]
+    ]
+    ```
+  
+**儲存變數方式是透過`RE_STAGE`的 `is_fits`來執行。
+
+範例：
+```
+{
+    "stage_type": "__LIB_SWITCH_STAGE__",
+    "stages_filter": [
+        ["VAR","我想要的數值","_成功路線_"],,
+        ["*",True,"_失敗路線_"]
+    ]
+
+}
+```
+
+### QA_STAGE
+QA_STAGE 採用`stage_type`為`__QA_STAGE__`，是通過`相似度`來決定回應的一種階段，主要有三個部分的組成。
+1. says: 用來設定該階段的回應句，回應句有三種類型
+   * 歡迎句: 第一次到該階段時，機器人會回應該句子。(可依需求關閉功能，`DISSABLE_WELCOME`設為`True`就關閉，預設為`False`。)
+   * 拒絕句: 當相似分數低於`qa_threshold`時，機器人會回應該句子。(可依需求關閉功能，`__DISABLE_REFUSE__`設為`True`就關閉，預設為`False`。)
+   * 完成句: 以上都完成時，機器人會回應該句子。(可透過`%%`包裹變數名稱，並以`空格`前後相隔後，調用該變數。)
+
+2. corpus: 使用者的輸入會與該字典的所有`key`進行比對，並儲存相關結果，相關結果包含：
+    * `__QA_RESPOND_QUESTION__`: 相似值最高的 key
+    * `__QA_RESPOND__`: 相似值最高的 key 對應之 value
+    * `__QA_RESPOND_SCORE__`: 相似值最高的數值
+    * `__RUNNING_CORPUS__`: 該次測試時使用的 corpus
+    * `__QA_RESPOND_THRESHOLD__`: 該次測試使用的 threshold
+    
+3. `__SAVED_NAME__`: 設定儲存之變數的名稱，方便使用。
+
+
+```
+ {
+    "stage_type": "__QA_STAGE__",
+    "qa_threshold": 1,
+    "says": {
+        "sys_welcome": "歡迎句",
+        "sys_refuse": "拒絕句",
+        "sys_complete": "完成句"
+    },
+    "corpus": {
+        "早安": "1",
+        "午安": "2",
+        "晚安": "3"
+    },
+    "__SAVED_NAME__": {
+        "__QA_RESPOND__": "QA_r1",
+        "__QA_RESPOND_THRESHOLD__": "QA_th",
+        "__QA_RESPOND_QUESTION__": "QA_q1",
+        "__QA_RESPOND_SCORE__": "QA_s1",
+        "__RUNNING_CORPUS__": "QA_c1",
+    },
+    "__DISABLE_WELCOME__": False,
+    "__DISABLE_REFUSE__": False,
+}
+```
+
+
+
+## More Examples
+
+# 飲料店
+```
+bot = {
+    "__MAIN_STAGES__": [
+        {
+            "stage_type": "__RE_STAGE__",
+            "question": {
+                "sys_welcome": "歡迎來到飲料店，請輸入您要的東西 紅茶/綠茶 少冰/去冰",
+                "sys_refuse": "不完全輸入 %%drink_type%% %%ice_type%% ",
+                "sys_complete": "你輸入的內容是 %%drink_type%% %%ice_type%% "
+            },
+            "is_fits": [
+                ["(紅茶|綠茶)+", "drink_type"],
+                ["(少冰|去冰)+", "ice_type"],
+
+            ]
+        },
+        {
+            "stage_type": "__LIB_SWITCH_STAGE__",
+            "stages_filter": [
+                [["drink_type", "ice_type"], ["綠茶", "去冰"], "_新路線1_"],
+                ["*", True, "_新路線2_"]
             ]
+
         }
-        print(f"\n" * 5)
-        
-        agent = gen_agent(bot)
-        data = {}
-        reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
-        print(f"reply_text: {reply_text}， ")
-        reply_text, data = ConversationAgent.to_bot(agent, "紅茶", data)
-        print(f"reply_text: {reply_text}， ")
-        reply_text, data = ConversationAgent.to_bot(agent, "少冰", data)
-        print(f"reply_text: {reply_text}， ")
-        ```
-        
-        ## ToDo
-        
-        ~~* Switch除了等號以外的方法~~
-        
-        ~~* DISSABLE_WELCOME測試與勘誤名詞~~
-        
-        ~~* QAStage 停用拒絕句(無論分數都會通過)~~
-        
-        ~~* 多回應方式~~
-        
-        ~~* 設定階段名稱~~
-        
-        * 修正QAstage為相似度模型階段
-        * 分類型模型階段
-        * 繼承的範例
-        * 說明agent刪除變數的規則
-        
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+    ],
+    "_新路線1_": [
+        {
+            "stage_type": "__RE_STAGE__",
+            "question": {
+                "sys_welcome": "",
+                "sys_refuse": "",
+                "sys_complete": "切換分之成功1"
+            },
+            "__DISSABLE_Q1__": True
+        },
+    ],
+    "_新路線2_": [
+        {
+            "stage_type": "__RE_STAGE__",
+            "question": {
+                "sys_welcome": "",
+                "sys_refuse": "",
+                "sys_complete": "切換分之成功2"
+            },
+            "__DISSABLE_Q1__": True
+        },
+    ]
+}
+print(f"\n" * 5)
+
+agent = gen_agent(bot)
+data = {}
+reply_text, data = ConversationAgent.to_bot(agent, "哈囉", data)
+print(f"reply_text: {reply_text}， ")
+reply_text, data = ConversationAgent.to_bot(agent, "紅茶", data)
+print(f"reply_text: {reply_text}， ")
+reply_text, data = ConversationAgent.to_bot(agent, "少冰", data)
+print(f"reply_text: {reply_text}， ")
+```
+
+## ToDo
+
+~~* Switch除了等號以外的方法~~
+
+~~* DISSABLE_WELCOME測試與勘誤名詞~~
+
+~~* QAStage 停用拒絕句(無論分數都會通過)~~
+
+~~* 多回應方式~~
+
+~~* 設定階段名稱~~
+
+* 修正QAstage為相似度模型階段
+* 分類型模型階段
+* 繼承的範例
+* 說明agent刪除變數的規則
+
+
```

### Comparing `ConversationAgent-0.5.4/setup.py` & `ConversationAgent-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("./ConversationAgent/README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 setuptools.setup(
     name='ConversationAgent',
-    version='0.5.4',
+    version='0.5.8',
     description='ConversationAgent',
     author='Theta',
     license='',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     package_data={
```

