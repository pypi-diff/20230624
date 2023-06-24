# Comparing `tmp/user_discord-1.2.5.tar.gz` & `tmp/user_discord-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-1.2.5.tar", last modified: Sat Jun 24 17:46:09 2023, max compression
+gzip compressed data, was "user_discord-1.2.6.tar", last modified: Sat Jun 24 18:22:53 2023, max compression
```

## Comparing `user_discord-1.2.5.tar` & `user_discord-1.2.6.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 17:46:09.329091 user_discord-1.2.5/
--rw-rw-rw-   0        0        0      443 2023-06-24 17:46:09.328091 user_discord-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3545 2023-06-24 16:52:42.000000 user_discord-1.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 17:46:09.330088 user_discord-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-24 17:45:54.000000 user_discord-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:46:09.305594 user_discord-1.2.5/user_discord/
--rw-rw-rw-   0        0        0      586 2023-06-24 17:46:02.000000 user_discord-1.2.5/user_discord/__init__.py
--rw-rw-rw-   0        0        0     5614 2023-06-24 17:45:28.000000 user_discord-1.2.5/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:46:09.326093 user_discord-1.2.5/user_discord.egg-info/
--rw-rw-rw-   0        0        0      443 2023-06-24 17:46:08.000000 user_discord-1.2.5/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-24 17:46:09.000000 user_discord-1.2.5/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 17:46:08.000000 user_discord-1.2.5/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-24 17:46:08.000000 user_discord-1.2.5/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-24 17:46:08.000000 user_discord-1.2.5/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 18:22:53.555810 user_discord-1.2.6/
+-rw-rw-rw-   0        0        0      443 2023-06-24 18:22:53.554812 user_discord-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 18:22:53.556808 user_discord-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-24 18:20:49.000000 user_discord-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:22:53.502721 user_discord-1.2.6/user_discord/
+-rw-rw-rw-   0        0        0      604 2023-06-24 18:21:02.000000 user_discord-1.2.6/user_discord/__init__.py
+-rw-rw-rw-   0        0        0     5638 2023-06-24 18:18:16.000000 user_discord-1.2.6/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:22:53.533398 user_discord-1.2.6/user_discord/utils/
+-rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.2.6/user_discord/utils/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.2.6/user_discord/utils/objects.py
+-rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.2.6/user_discord/utils/payloads.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:22:53.527398 user_discord-1.2.6/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-06-24 18:22:52.000000 user_discord-1.2.6/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-24 18:22:53.000000 user_discord-1.2.6/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:22:52.000000 user_discord-1.2.6/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-24 18:22:52.000000 user_discord-1.2.6/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-24 18:22:52.000000 user_discord-1.2.6/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-1.2.5/README.md` & `user_discord-1.2.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 - Python 3.x
 - `requests` library
 - `websocket-client` library
 
 ## Installation
 
-1. Clone the repository or download the project files.
+1. ```shell
+   pip install user-discord
+   ```
 2. Install the required libraries by running the following command:
    ```
    pip install requests websocket-client
    ```
 
 ## Usage
 
@@ -24,18 +26,16 @@
    import time
    import random
    import base64
    import requests
    import websocket
    from requests.structures import CaseInsensitiveDict
    from threading import Thread
-   from utils.payloads import StartSocket
-   from utils.objects import MessageContent
-   from client_discord import ClientDiscord
-   from socket_discord import SocketDiscord
+   from user_discord import ClientDiscord
+   from user_discord import SocketDiscord
    ```
 
 2. Create an instance of the `ClientDiscord` class:
    ```python
    client = ClientDiscord()
    ```
 
@@ -112,14 +112,10 @@
 
    # Register more event handlers as needed
 
    # Start the WebSocket connection
    socket.start_ws()
    ```
 
-   Note: The available event types are `'READY'`, `'MESSAGE_CREATE'`, and `'all'`. You can register event handlers for these types and handle the received data
-
- accordingly.
-
 ## Contributing
 
 Contributions are welcome! If you have any suggestions, improvements, or bug fixes, please open an issue or submit a pull request.
```

### Comparing `user_discord-1.2.5/setup.py` & `user_discord-1.2.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ### No work
 Join-server, login, access discord database :D"""
 
 setup(
     name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="1.2.5",
+    version="1.2.6",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

### Comparing `user_discord-1.2.5/user_discord/__init__.py` & `user_discord-1.2.6/user_discord/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 __title__ = 'user_discord'
 __author__ = 'nxSlayer'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 nxSlayer'
 
 from .user_discord import SocketDiscord
 from .user_discord import ClientDiscord
-from .utils import objects, payloads
+from .utils import objects
+from .utils import payloads
 
 from requests import get
 from json import loads
 
 __newest__ = loads(get("https://pypi.org/pypi/user-discord/json").text)["info"]["version"]
 
-if '1.2.5' != __newest__:
+if '1.2.6' != __newest__:
     print(f"(user-discord) There is a new version, please update for better results")
```

### Comparing `user_discord-1.2.5/user_discord/user_discord.py` & `user_discord-1.2.6/user_discord/user_discord.py`

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
-from .utils.payloads import StartSocket
-from .utils.objects import MessageContent
+from user_discord.utils.payloads import StartSocket
+from user_discord.utils.objects import MessageContent
 
 
 class ClientDiscord:
 
   def __init__(self):
     
     self.token = None
```

