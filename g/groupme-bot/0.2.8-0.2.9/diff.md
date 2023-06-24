# Comparing `tmp/groupme-bot-0.2.8.tar.gz` & `tmp/groupme-bot-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/groupme-bot-0.2.8.tar", last modified: Mon Jan  4 17:35:34 2021, max compression
+gzip compressed data, was "groupme-bot-0.2.9.tar", last modified: Wed Jun  2 20:11:46 2021, max compression
```

## Comparing `groupme-bot-0.2.8.tar` & `groupme-bot-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 brandenc   (501) staff       (20)        0 2021-01-04 17:35:34.546480 groupme-bot-0.2.8/
--rw-r--r--   0 brandenc   (501) staff       (20)     5101 2021-01-04 17:35:34.546210 groupme-bot-0.2.8/PKG-INFO
--rw-r--r--   0 brandenc   (501) staff       (20)     3648 2020-12-30 21:01:39.000000 groupme-bot-0.2.8/README.md
-drwxr-xr-x   0 brandenc   (501) staff       (20)        0 2021-01-04 17:35:34.544321 groupme-bot-0.2.8/groupme_bot/
--rw-r--r--   0 brandenc   (501) staff       (20)      607 2021-01-04 17:34:52.000000 groupme-bot-0.2.8/groupme_bot/__init__.py
--rw-r--r--   0 brandenc   (501) staff       (20)     4811 2021-01-04 17:34:18.000000 groupme-bot-0.2.8/groupme_bot/application.py
--rw-r--r--   0 brandenc   (501) staff       (20)     3200 2021-01-04 17:34:18.000000 groupme-bot-0.2.8/groupme_bot/attachment.py
--rw-r--r--   0 brandenc   (501) staff       (20)     7284 2021-01-04 17:34:42.000000 groupme-bot-0.2.8/groupme_bot/bot.py
--rw-r--r--   0 brandenc   (501) staff       (20)     1901 2021-01-04 17:34:18.000000 groupme-bot-0.2.8/groupme_bot/callback.py
--rw-r--r--   0 brandenc   (501) staff       (20)     2655 2021-01-04 17:34:18.000000 groupme-bot-0.2.8/groupme_bot/groupme.py
-drwxr-xr-x   0 brandenc   (501) staff       (20)        0 2021-01-04 17:35:34.545796 groupme-bot-0.2.8/groupme_bot.egg-info/
--rw-r--r--   0 brandenc   (501) staff       (20)     5101 2021-01-04 17:35:34.000000 groupme-bot-0.2.8/groupme_bot.egg-info/PKG-INFO
--rw-r--r--   0 brandenc   (501) staff       (20)      335 2021-01-04 17:35:34.000000 groupme-bot-0.2.8/groupme_bot.egg-info/SOURCES.txt
--rw-r--r--   0 brandenc   (501) staff       (20)        1 2021-01-04 17:35:34.000000 groupme-bot-0.2.8/groupme_bot.egg-info/dependency_links.txt
--rw-r--r--   0 brandenc   (501) staff       (20)       76 2021-01-04 17:35:34.000000 groupme-bot-0.2.8/groupme_bot.egg-info/requires.txt
--rw-r--r--   0 brandenc   (501) staff       (20)       12 2021-01-04 17:35:34.000000 groupme-bot-0.2.8/groupme_bot.egg-info/top_level.txt
--rw-r--r--   0 brandenc   (501) staff       (20)       38 2021-01-04 17:35:34.546578 groupme-bot-0.2.8/setup.cfg
--rw-r--r--   0 brandenc   (501) staff       (20)     1143 2021-01-04 17:34:18.000000 groupme-bot-0.2.8/setup.py
+drwxr-xr-x   0 brandencolen   (501) staff       (20)        0 2021-06-02 20:11:46.949494 groupme-bot-0.2.9/
+-rw-r--r--   0 brandencolen   (501) staff       (20)     5101 2021-06-02 20:11:46.949364 groupme-bot-0.2.9/PKG-INFO
+-rw-r--r--   0 brandencolen   (501) staff       (20)     3648 2021-02-25 22:13:35.000000 groupme-bot-0.2.9/README.md
+drwxr-xr-x   0 brandencolen   (501) staff       (20)        0 2021-06-02 20:11:46.947334 groupme-bot-0.2.9/groupme_bot/
+-rw-r--r--   0 brandencolen   (501) staff       (20)      607 2021-06-02 20:06:16.000000 groupme-bot-0.2.9/groupme_bot/__init__.py
+-rw-r--r--   0 brandencolen   (501) staff       (20)     4811 2021-02-25 22:13:35.000000 groupme-bot-0.2.9/groupme_bot/application.py
+-rw-r--r--   0 brandencolen   (501) staff       (20)     3200 2021-02-25 22:13:35.000000 groupme-bot-0.2.9/groupme_bot/attachment.py
+-rw-r--r--   0 brandencolen   (501) staff       (20)     7332 2021-06-02 20:05:09.000000 groupme-bot-0.2.9/groupme_bot/bot.py
+-rw-r--r--   0 brandencolen   (501) staff       (20)     1901 2021-02-25 22:13:35.000000 groupme-bot-0.2.9/groupme_bot/callback.py
+-rw-r--r--   0 brandencolen   (501) staff       (20)     2655 2021-02-25 22:13:35.000000 groupme-bot-0.2.9/groupme_bot/groupme.py
+drwxr-xr-x   0 brandencolen   (501) staff       (20)        0 2021-06-02 20:11:46.949186 groupme-bot-0.2.9/groupme_bot.egg-info/
+-rw-r--r--   0 brandencolen   (501) staff       (20)     5101 2021-06-02 20:11:46.000000 groupme-bot-0.2.9/groupme_bot.egg-info/PKG-INFO
+-rw-r--r--   0 brandencolen   (501) staff       (20)      335 2021-06-02 20:11:46.000000 groupme-bot-0.2.9/groupme_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 brandencolen   (501) staff       (20)        1 2021-06-02 20:11:46.000000 groupme-bot-0.2.9/groupme_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 brandencolen   (501) staff       (20)       76 2021-06-02 20:11:46.000000 groupme-bot-0.2.9/groupme_bot.egg-info/requires.txt
+-rw-r--r--   0 brandencolen   (501) staff       (20)       12 2021-06-02 20:11:46.000000 groupme-bot-0.2.9/groupme_bot.egg-info/top_level.txt
+-rw-r--r--   0 brandencolen   (501) staff       (20)       38 2021-06-02 20:11:46.949533 groupme-bot-0.2.9/setup.cfg
+-rw-r--r--   0 brandencolen   (501) staff       (20)     1143 2021-02-25 22:13:35.000000 groupme-bot-0.2.9/setup.py
```

### Comparing `groupme-bot-0.2.8/PKG-INFO` & `groupme-bot-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupme-bot
-Version: 0.2.8
+Version: 0.2.9
 Summary: A simple bot builder for GroupMe
 Home-page: https://github.com/brandenc40/groupme-bot
 Author: Branden Colen
 Author-email: brandencolen@gmail.com
 License: MIT
 Description: # GroupMe Bot Builder
```

### Comparing `groupme-bot-0.2.8/README.md` & `groupme-bot-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `groupme-bot-0.2.8/groupme_bot/__init__.py` & `groupme-bot-0.2.9/groupme_bot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .attachment import (
     ImageAttachment, LocationAttachment, SplitAttachment, EmojiAttachment, MentionsAttachment, parse_attachment
 )
 from .bot import Bot, Context
 from .callback import Callback
 from .groupme import GroupMe
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 __author__ = "Branden Colen"
 __all__ = [
     "Application",
     "Bot",
     "Callback",
     "Context",
     "EmojiAttachment",
```

### Comparing `groupme-bot-0.2.8/groupme_bot/application.py` & `groupme-bot-0.2.9/groupme_bot/application.py`

 * *Files identical despite different names*

### Comparing `groupme-bot-0.2.8/groupme_bot/attachment.py` & `groupme-bot-0.2.9/groupme_bot/attachment.py`

 * *Files identical despite different names*

### Comparing `groupme-bot-0.2.8/groupme_bot/bot.py` & `groupme-bot-0.2.9/groupme_bot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-import json
 import re
+from collections import OrderedDict
 from json.decoder import JSONDecodeError
 from typing import Any, List, Callable, Optional
 
 import httpx
 from starlette.requests import Request
 from starlette.responses import PlainTextResponse
 from starlette.types import Scope, Receive, Send
@@ -58,15 +58,15 @@
         """
         super().__init__(groupme_api_token)
         self.bot_name = bot_name
         self.bot_id = bot_id
         self.groupme_api_token = groupme_api_token
         self.group_id = group_id
 
-        self._handler_functions = {}
+        self._handler_functions: OrderedDict = OrderedDict()
         self._jobs = []
 
     @property
     def cron_jobs(self) -> List[dict]:
         """
         All list of cron jobs associated with this bot.
         :return List[dict]:
```

### Comparing `groupme-bot-0.2.8/groupme_bot/callback.py` & `groupme-bot-0.2.9/groupme_bot/callback.py`

 * *Files identical despite different names*

### Comparing `groupme-bot-0.2.8/groupme_bot/groupme.py` & `groupme-bot-0.2.9/groupme_bot/groupme.py`

 * *Files identical despite different names*

### Comparing `groupme-bot-0.2.8/groupme_bot.egg-info/PKG-INFO` & `groupme-bot-0.2.9/groupme_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupme-bot
-Version: 0.2.8
+Version: 0.2.9
 Summary: A simple bot builder for GroupMe
 Home-page: https://github.com/brandenc40/groupme-bot
 Author: Branden Colen
 Author-email: brandencolen@gmail.com
 License: MIT
 Description: # GroupMe Bot Builder
```

### Comparing `groupme-bot-0.2.8/setup.py` & `groupme-bot-0.2.9/setup.py`

 * *Files identical despite different names*

