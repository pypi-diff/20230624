# Comparing `tmp/user_discord-1.2.6.tar.gz` & `tmp/user_discord-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-1.2.6.tar", last modified: Sat Jun 24 18:22:53 2023, max compression
+gzip compressed data, was "user_discord-1.2.7.tar", last modified: Sat Jun 24 18:27:52 2023, max compression
```

## Comparing `user_discord-1.2.6.tar` & `user_discord-1.2.7.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:22:53.555810 user_discord-1.2.6/
--rw-rw-rw-   0        0        0      443 2023-06-24 18:22:53.554812 user_discord-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 18:22:53.556808 user_discord-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-24 18:20:49.000000 user_discord-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:22:53.502721 user_discord-1.2.6/user_discord/
--rw-rw-rw-   0        0        0      604 2023-06-24 18:21:02.000000 user_discord-1.2.6/user_discord/__init__.py
--rw-rw-rw-   0        0        0     5638 2023-06-24 18:18:16.000000 user_discord-1.2.6/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:22:53.533398 user_discord-1.2.6/user_discord/utils/
--rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.2.6/user_discord/utils/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.2.6/user_discord/utils/objects.py
--rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.2.6/user_discord/utils/payloads.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:22:53.527398 user_discord-1.2.6/user_discord.egg-info/
--rw-rw-rw-   0        0        0      443 2023-06-24 18:22:52.000000 user_discord-1.2.6/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-06-24 18:22:53.000000 user_discord-1.2.6/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:22:52.000000 user_discord-1.2.6/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-24 18:22:52.000000 user_discord-1.2.6/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-24 18:22:52.000000 user_discord-1.2.6/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 18:27:52.295783 user_discord-1.2.7/
+-rw-rw-rw-   0        0        0      443 2023-06-24 18:27:52.294783 user_discord-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 18:27:52.296784 user_discord-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-24 18:27:34.000000 user_discord-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:27:52.258082 user_discord-1.2.7/user_discord/
+-rw-rw-rw-   0        0        0      612 2023-06-24 18:27:44.000000 user_discord-1.2.7/user_discord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:27:52.286789 user_discord-1.2.7/user_discord/lib/
+-rw-rw-rw-   0        0        0        0 2023-06-24 18:26:04.000000 user_discord-1.2.7/user_discord/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:27:52.292787 user_discord-1.2.7/user_discord/lib/utils/
+-rw-rw-rw-   0        0        0       46 2023-06-24 18:25:01.000000 user_discord-1.2.7/user_discord/lib/utils/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.2.7/user_discord/lib/utils/objects.py
+-rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.2.7/user_discord/lib/utils/payloads.py
+-rw-rw-rw-   0        0        0     5622 2023-06-24 18:26:31.000000 user_discord-1.2.7/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:27:52.284785 user_discord-1.2.7/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-06-24 18:27:51.000000 user_discord-1.2.7/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-06-24 18:27:52.000000 user_discord-1.2.7/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:27:51.000000 user_discord-1.2.7/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-24 18:27:51.000000 user_discord-1.2.7/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-24 18:27:51.000000 user_discord-1.2.7/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-1.2.6/README.md` & `user_discord-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `user_discord-1.2.6/setup.py` & `user_discord-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ### No work
 Join-server, login, access discord database :D"""
 
 setup(
     name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="1.2.6",
+    version="1.2.7",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

### Comparing `user_discord-1.2.6/user_discord/__init__.py` & `user_discord-1.2.7/user_discord/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 __title__ = 'user_discord'
 __author__ = 'nxSlayer'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 nxSlayer'
 
 from .user_discord import SocketDiscord
 from .user_discord import ClientDiscord
-from .utils import objects
-from .utils import payloads
+from .lib.utils import objects
+from .lib.utils import payloads
 
 from requests import get
 from json import loads
 
 __newest__ = loads(get("https://pypi.org/pypi/user-discord/json").text)["info"]["version"]
 
-if '1.2.6' != __newest__:
+if '1.2.7' != __newest__:
     print(f"(user-discord) There is a new version, please update for better results")
```

### Comparing `user_discord-1.2.6/user_discord/user_discord.py` & `user_discord-1.2.7/user_discord/user_discord.py`

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
-from user_discord.utils.payloads import StartSocket
-from user_discord.utils.objects import MessageContent
+from .lib.utils.payloads import StartSocket
+from .lib.utils.objects import MessageContent
 
 
 class ClientDiscord:
 
   def __init__(self):
     
     self.token = None
```

### Comparing `user_discord-1.2.6/user_discord/utils/objects.py` & `user_discord-1.2.7/user_discord/lib/utils/objects.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.2.6/user_discord/utils/payloads.py` & `user_discord-1.2.7/user_discord/lib/utils/payloads.py`

 * *Files identical despite different names*

