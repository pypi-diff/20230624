# Comparing `tmp/user_discord-1.2.7.tar.gz` & `tmp/user_discord-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-1.2.7.tar", last modified: Sat Jun 24 18:27:52 2023, max compression
+gzip compressed data, was "user_discord-1.2.9.tar", last modified: Sat Jun 24 18:39:48 2023, max compression
```

## Comparing `user_discord-1.2.7.tar` & `user_discord-1.2.9.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:27:52.295783 user_discord-1.2.7/
--rw-rw-rw-   0        0        0      443 2023-06-24 18:27:52.294783 user_discord-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 18:27:52.296784 user_discord-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-24 18:27:34.000000 user_discord-1.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:27:52.258082 user_discord-1.2.7/user_discord/
--rw-rw-rw-   0        0        0      612 2023-06-24 18:27:44.000000 user_discord-1.2.7/user_discord/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:27:52.286789 user_discord-1.2.7/user_discord/lib/
--rw-rw-rw-   0        0        0        0 2023-06-24 18:26:04.000000 user_discord-1.2.7/user_discord/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:27:52.292787 user_discord-1.2.7/user_discord/lib/utils/
--rw-rw-rw-   0        0        0       46 2023-06-24 18:25:01.000000 user_discord-1.2.7/user_discord/lib/utils/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.2.7/user_discord/lib/utils/objects.py
--rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.2.7/user_discord/lib/utils/payloads.py
--rw-rw-rw-   0        0        0     5622 2023-06-24 18:26:31.000000 user_discord-1.2.7/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:27:52.284785 user_discord-1.2.7/user_discord.egg-info/
--rw-rw-rw-   0        0        0      443 2023-06-24 18:27:51.000000 user_discord-1.2.7/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-06-24 18:27:52.000000 user_discord-1.2.7/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:27:51.000000 user_discord-1.2.7/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-24 18:27:51.000000 user_discord-1.2.7/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-24 18:27:51.000000 user_discord-1.2.7/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 18:39:48.346453 user_discord-1.2.9/
+-rw-rw-rw-   0        0        0      443 2023-06-24 18:39:48.346453 user_discord-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 18:39:48.348450 user_discord-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-24 18:39:09.000000 user_discord-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:39:48.307203 user_discord-1.2.9/user_discord/
+-rw-rw-rw-   0        0        0      604 2023-06-24 18:39:18.000000 user_discord-1.2.9/user_discord/__init__.py
+-rw-rw-rw-   0        0        0     5638 2023-06-24 18:18:16.000000 user_discord-1.2.9/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:39:48.344448 user_discord-1.2.9/user_discord/utils/
+-rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.2.9/user_discord/utils/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.2.9/user_discord/utils/objects.py
+-rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.2.9/user_discord/utils/payloads.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:39:48.337519 user_discord-1.2.9/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-06-24 18:39:47.000000 user_discord-1.2.9/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-06-24 18:39:48.000000 user_discord-1.2.9/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:39:47.000000 user_discord-1.2.9/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-24 18:39:47.000000 user_discord-1.2.9/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-24 18:39:47.000000 user_discord-1.2.9/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-1.2.7/README.md` & `user_discord-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `user_discord-1.2.7/setup.py` & `user_discord-1.2.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ### No work
 Join-server, login, access discord database :D"""
 
 setup(
     name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="1.2.7",
+    version="1.2.9",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

### Comparing `user_discord-1.2.7/user_discord/lib/utils/objects.py` & `user_discord-1.2.9/user_discord/utils/objects.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.2.7/user_discord/lib/utils/payloads.py` & `user_discord-1.2.9/user_discord/utils/payloads.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.2.7/user_discord/user_discord.py` & `user_discord-1.2.9/user_discord/user_discord.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import time
 import random
 import base64
 import requests
 import websocket
 from requests.structures import CaseInsensitiveDict
 from threading import Thread
-from .lib.utils.payloads import StartSocket
-from .lib.utils.objects import MessageContent
+from user_discord.utils.payloads import StartSocket
+from user_discord.utils.objects import MessageContent
 
 
 class ClientDiscord:
 
   def __init__(self):
     
     self.token = None
```

