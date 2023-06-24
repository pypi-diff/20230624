# Comparing `tmp/selis-3.4.4.tar.gz` & `tmp/selis-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-3.4.4.tar", last modified: Sat Jun 24 11:48:04 2023, max compression
+gzip compressed data, was "selis-3.4.5.tar", last modified: Sat Jun 24 11:52:44 2023, max compression
```

## Comparing `selis-3.4.4.tar` & `selis-3.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-24 11:48:04.034254 selis-3.4.4/
--rw-r--r--   0 client     (501) staff       (20)      130 2023-06-24 11:48:04.034112 selis-3.4.4/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-24 11:48:04.032028 selis-3.4.4/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-17 14:59:11.000000 selis-3.4.4/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     3835 2023-06-20 05:09:46.000000 selis-3.4.4/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)      638 2023-06-20 05:08:34.000000 selis-3.4.4/selis/computerinfo.py
--rw-r--r--   0 client     (501) staff       (20)     1137 2023-06-24 11:47:50.000000 selis-3.4.4/selis/selis.py
--rw-r--r--   0 client     (501) staff       (20)      410 2023-06-19 15:00:37.000000 selis-3.4.4/selis/utils.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-24 11:48:04.033687 selis-3.4.4/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      130 2023-06-24 11:48:04.000000 selis-3.4.4/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      270 2023-06-24 11:48:04.000000 selis-3.4.4/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-24 11:48:04.000000 selis-3.4.4/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-24 11:48:04.000000 selis-3.4.4/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)       24 2023-06-24 11:48:04.000000 selis-3.4.4/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-24 11:48:04.000000 selis-3.4.4/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-24 11:48:04.034302 selis-3.4.4/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      281 2023-06-24 11:47:47.000000 selis-3.4.4/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-24 11:52:44.465815 selis-3.4.5/
+-rw-r--r--   0 client     (501) staff       (20)      130 2023-06-24 11:52:44.465702 selis-3.4.5/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-24 11:52:44.464092 selis-3.4.5/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-17 14:59:11.000000 selis-3.4.5/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     3861 2023-06-24 11:52:26.000000 selis-3.4.5/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)      786 2023-06-24 11:52:24.000000 selis-3.4.5/selis/computerinfo.py
+-rw-r--r--   0 client     (501) staff       (20)     1137 2023-06-24 11:52:33.000000 selis-3.4.5/selis/selis.py
+-rw-r--r--   0 client     (501) staff       (20)      410 2023-06-24 11:51:57.000000 selis-3.4.5/selis/utils.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-24 11:52:44.465481 selis-3.4.5/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      130 2023-06-24 11:52:44.000000 selis-3.4.5/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      270 2023-06-24 11:52:44.000000 selis-3.4.5/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-24 11:52:44.000000 selis-3.4.5/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-24 11:52:44.000000 selis-3.4.5/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)       24 2023-06-24 11:52:44.000000 selis-3.4.5/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-24 11:52:44.000000 selis-3.4.5/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-24 11:52:44.465856 selis-3.4.5/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      281 2023-06-24 11:51:33.000000 selis-3.4.5/setup.py
```

### Comparing `selis-3.4.4/selis/client.py` & `selis-3.4.5/selis/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import socket
 import threading
 import sys
 import getpass
 
-import computerinfo
+from selis.computerinfo import ComputerInfo
 from selis.utils import convert_color, guide_to_exit, clear_screen, open_url
 
 
 class ChatClient:
     def __init__(self, ip, port, nickname):
         self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
@@ -18,15 +18,15 @@
 
         self.nickname = nickname
         self.send_client_info_to_sever()
         self.is_running = True
 
 
     def send_client_info_to_sever(self):
-        client_computer = computerinfo.get()
+        client_computer = ComputerInfo().get()
         msg = self.nickname + "/" + client_computer
         self.send_message(msg)
 
 
     def send_message(self, message):
         self.connection.send(message.encode())
```

### Comparing `selis-3.4.4/selis/computerinfo.py` & `selis-3.4.5/selis/computerinfo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import requests
 import platform
 
 from bs4 import BeautifulSoup
 
 
-def get_public_ip():
-    response = requests.get("https://www.iplocation.net/find-ip-address")
-    soup = BeautifulSoup(response.content, "html.parser")
-    ip = soup.find("span", style="font-weight: bold; color:green;").get_text()
-    return ip
+class ComputerInfo:
+    def __init__(self):
+        self.url = "https://www.iplocation.net/find-ip-address"
 
 
-def get_system_info():
-    return platform.machine() + "/" + platform.node() + "/" + platform.platform() + "/" + platform.processor() + "/" + \
-        platform.release() + "/" + platform.system() + "/" + platform.version()
+    def get_public_ip(self):
+        response = requests.get(self.url)
+        soup = BeautifulSoup(response.content, "html.parser")
+        ip = soup.find("span", style="font-weight: bold; color:green;").get_text()
+        return ip
 
 
-def get():
-    ip = get_public_ip()
-    os_info = get_system_info()
+    def get_system_info(self):
+        return platform.machine() + "/" + platform.node() + "/" + platform.platform() + "/" + platform.processor() + "/" + \
+            platform.release() + "/" + platform.system() + "/" + platform.version()
 
-    return ip + "/" + os_info
+
+    def get(self):
+        ip = self.get_public_ip()
+        os_info = self.get_system_info()
+
+        return ip + "/" + os_info
+
```

### Comparing `selis-3.4.4/selis/selis.py` & `selis-3.4.5/selis/selis.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     parser = OptionParser()
     parser.add_option("-v", "--version", dest="version", action="store_true", help="show version and exit")
     parser.add_option("-p", "--port", dest="port", help="connect to sever through this port")
     parser.add_option("-n", "--nickname", dest="nickname", help="choose a nickname")
     (options, arguments) = parser.parse_args()
 
     if options.version:
-        print("selis 3.4.4")
+        print("selis 3.4.5")
         sys.exit()
         
     return_error(parser, options)
     return options
 
 
 def return_error(parser, options):
```

