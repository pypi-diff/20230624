# Comparing `tmp/pwl-chat-python-1.4.9.tar.gz` & `tmp/pwl-chat-python-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.4.9.tar", last modified: Tue Jun 13 10:07:08 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.5.0.tar", last modified: Sat Jun 24 05:29:52 2023, max compression
```

## Comparing `pwl-chat-python-1.4.9.tar` & `pwl-chat-python-1.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 10:07:08.000000 pwl-chat-python-1.4.9/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 10:07:08.716922 pwl-chat-python-1.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/api/__api__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/api/chatroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/api/redpacket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/chatroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/redpacket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/core/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:08.712922 pwl-chat-python-1.4.9/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 10:06:57.000000 pwl-chat-python-1.4.9/src/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:29:52.474899 pwl-chat-python-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-24 05:29:52.474899 pwl-chat-python-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:29:52.470899 pwl-chat-python-1.5.0/pwl_chat_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-24 05:29:52.000000 pwl-chat-python-1.5.0/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-24 05:29:52.000000 pwl-chat-python-1.5.0/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 05:29:52.000000 pwl-chat-python-1.5.0/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-24 05:29:52.000000 pwl-chat-python-1.5.0/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-24 05:29:52.000000 pwl-chat-python-1.5.0/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-24 05:29:52.000000 pwl-chat-python-1.5.0/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 05:29:52.474899 pwl-chat-python-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:29:52.470899 pwl-chat-python-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:29:52.470899 pwl-chat-python-1.5.0/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/api/__api__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/api/chatroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/api/redpacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:29:52.470899 pwl-chat-python-1.5.0/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/core/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/core/chatroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/core/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/core/redpacket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/core/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/core/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:29:52.474899 pwl-chat-python-1.5.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 05:29:38.000000 pwl-chat-python-1.5.0/src/utils/version.py
```

### Comparing `pwl-chat-python-1.4.9/LICENSE` & `pwl-chat-python-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/PKG-INFO` & `pwl-chat-python-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.9
+Version: 1.5.0
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pwl-chat-python-1.4.9/README.md` & `pwl-chat-python-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.5.0/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.9
+Version: 1.5.0
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pwl-chat-python-1.4.9/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.5.0/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/setup.py` & `pwl-chat-python-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/src/api/__init__.py` & `pwl-chat-python-1.5.0/src/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/src/api/chatroom.py` & `pwl-chat-python-1.5.0/src/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/src/api/redpacket.py` & `pwl-chat-python-1.5.0/src/api/redpacket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/src/api/user.py` & `pwl-chat-python-1.5.0/src/api/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/src/core/__init__.py` & `pwl-chat-python-1.5.0/src/core/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 
 from src.api import FishPi
 from .chatroom import init_soliloquize, listener
+from .redpacket import render_redpacket
 from .config import GLOBAL_CONFIG, RedPacketConfig, AuthConfig, ChatConfig
 import configparser
 import os
 
 
 def __init__(api: FishPi, file_path: str = None):
     if file_path is None:   
@@ -27,14 +28,15 @@
         __init_default_config()
     __init_message_listener(api)
     init_soliloquize(api)
 
 
 def __init_message_listener(api :FishPi):
     api.add_listener(listener)
+    api.add_listener(render_redpacket)
 
 def __init_default_config():
     print("加载默认配置文件")
     GLOBAL_CONFIG.auth_config = AuthConfig()
     GLOBAL_CONFIG.redpacket_config = RedPacketConfig()
     GLOBAL_CONFIG.chat_config = ChatConfig()
     GLOBAL_CONFIG.cfg_path = None
```

### Comparing `pwl-chat-python-1.4.9/src/core/blacklist.py` & `pwl-chat-python-1.5.0/src/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/src/core/chatroom.py` & `pwl-chat-python-1.5.0/src/core/chatroom.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 executor = ThreadPoolExecutor(max_workers=5)
 
 def listener(api: FishPi, message :dict) -> None:
     if message['type'] == 'msg':
         if message['content'].find("redPacket") != -1:
             executor.submit(rush_redpacket, api, message)
-            #rush_redpacket(api, message)
         else:
             time = message['time']
             user = message['userName']
             user_nick_name = message['userNickname']
             if len(GLOBAL_CONFIG.chat_config.blacklist) > 0 \
                     and GLOBAL_CONFIG.chat_config.blacklist.__contains__(user):
                 return
```

### Comparing `pwl-chat-python-1.4.9/src/core/cli.py` & `pwl-chat-python-1.5.0/src/core/cli.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/src/core/config.py` & `pwl-chat-python-1.5.0/src/core/config.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/src/core/redpacket.py` & `pwl-chat-python-1.5.0/src/core/redpacket.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,26 +43,37 @@
     if code == CODE.SUCCESS:
         api.chatroom.send(RPS_SUCCESS)
     elif code == CODE.LOSED:
         api.chatroom.send(RPS_LOSED)
     elif code == CODE.ZERO:
         api.chatroom.send(RPS_ZERO)
 
+def render_redpacket(api: FishPi, message :dict) -> None:
+    if message['type'] != 'redPacketStatus':
+        return
+    sender = message['whoGive']
+    goter = message['whoGot']
+    if sender == api.current_user:
+        if goter != sender:
+            print(f"红包助手: {goter} 领取了你的红包!")
+    else:
+        return
 
 def rush_redpacket(api: FishPi, redpacket):
     sender = redpacket['userName']
+    content = json.loads(redpacket['content'])
     if sender == api.current_user:
         print('\t\t\t\t\t\t[' + redpacket['time'] + ']')
         print('\t\t\t\t\t\t发送了一个红包')
+        if content['type'] not in ['rockPaperScissors','heartbeat']:
+            open_red_packet(api, redpacket['oId'])
         return
     if (GLOBAL_CONFIG.redpacket_config.red_packet_switch == False):
         print(f'红包助手: {sender}发送了一个红包 你错过了这个红包，请开启抢红包模式！')
         return
-    sender = redpacket['userName']
-    content = json.loads(redpacket['content'])
     if content['type'] == 'heartbeat':
         if GLOBAL_CONFIG.redpacket_config.heartbeat:
             if GLOBAL_CONFIG.redpacket_config.smart_mode:
                 print(f'红包助手: {sender}发了一个心跳红包')
                 __analyzeHeartbeatRedPacket(api, redpacket['oId'])
                 return
             open_red_packet(api, redpacket['oId'])
```

### Comparing `pwl-chat-python-1.4.9/src/core/user.py` & `pwl-chat-python-1.5.0/src/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/src/core/websocket.py` & `pwl-chat-python-1.5.0/src/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/src/main.py` & `pwl-chat-python-1.5.0/src/main.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.9/src/utils/utils.py` & `pwl-chat-python-1.5.0/src/utils/utils.py`

 * *Files identical despite different names*

