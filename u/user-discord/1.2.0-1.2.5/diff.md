# Comparing `tmp/user_discord-1.2.0.tar.gz` & `tmp/user_discord-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-1.2.0.tar", last modified: Sat Jun 24 17:43:28 2023, max compression
+gzip compressed data, was "user_discord-1.2.5.tar", last modified: Sat Jun 24 17:46:09 2023, max compression
```

## Comparing `user_discord-1.2.0.tar` & `user_discord-1.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 17:43:28.867998 user_discord-1.2.0/
--rw-rw-rw-   0        0        0      443 2023-06-24 17:43:28.866999 user_discord-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3545 2023-06-24 16:52:42.000000 user_discord-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 17:43:28.867998 user_discord-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-24 17:43:08.000000 user_discord-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:43:28.843675 user_discord-1.2.0/user_discord/
--rw-rw-rw-   0        0        0      586 2023-06-24 17:42:54.000000 user_discord-1.2.0/user_discord/__init__.py
--rw-rw-rw-   0        0        0     5612 2023-06-24 16:38:07.000000 user_discord-1.2.0/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:43:28.864000 user_discord-1.2.0/user_discord.egg-info/
--rw-rw-rw-   0        0        0      443 2023-06-24 17:43:28.000000 user_discord-1.2.0/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-24 17:43:28.000000 user_discord-1.2.0/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 17:43:28.000000 user_discord-1.2.0/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-24 17:43:28.000000 user_discord-1.2.0/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-24 17:43:28.000000 user_discord-1.2.0/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 17:46:09.329091 user_discord-1.2.5/
+-rw-rw-rw-   0        0        0      443 2023-06-24 17:46:09.328091 user_discord-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3545 2023-06-24 16:52:42.000000 user_discord-1.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 17:46:09.330088 user_discord-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-24 17:45:54.000000 user_discord-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:46:09.305594 user_discord-1.2.5/user_discord/
+-rw-rw-rw-   0        0        0      586 2023-06-24 17:46:02.000000 user_discord-1.2.5/user_discord/__init__.py
+-rw-rw-rw-   0        0        0     5614 2023-06-24 17:45:28.000000 user_discord-1.2.5/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:46:09.326093 user_discord-1.2.5/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-06-24 17:46:08.000000 user_discord-1.2.5/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-24 17:46:09.000000 user_discord-1.2.5/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 17:46:08.000000 user_discord-1.2.5/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-24 17:46:08.000000 user_discord-1.2.5/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-24 17:46:08.000000 user_discord-1.2.5/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-1.2.0/README.md` & `user_discord-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `user_discord-1.2.0/setup.py` & `user_discord-1.2.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ### No work
 Join-server, login, access discord database :D"""
 
 setup(
     name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="1.2.0",
+    version="1.2.5",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

### Comparing `user_discord-1.2.0/user_discord/__init__.py` & `user_discord-1.2.5/user_discord/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 from .utils import objects, payloads
 
 from requests import get
 from json import loads
 
 __newest__ = loads(get("https://pypi.org/pypi/user-discord/json").text)["info"]["version"]
 
-if '1.1.0' != __newest__:
+if '1.2.5' != __newest__:
     print(f"(user-discord) There is a new version, please update for better results")
```

### Comparing `user_discord-1.2.0/user_discord/user_discord.py` & `user_discord-1.2.5/user_discord/user_discord.py`

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
-from utils.payloads import StartSocket
-from utils.objects import MessageContent
+from .utils.payloads import StartSocket
+from .utils.objects import MessageContent
 
 
 class ClientDiscord:
 
   def __init__(self):
     
     self.token = None
```

