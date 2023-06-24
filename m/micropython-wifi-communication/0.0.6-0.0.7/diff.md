# Comparing `tmp/micropython_wifi_communication-0.0.6.tar.gz` & `tmp/micropython_wifi_communication-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_wifi_communication-0.0.6.tar", last modified: Sat Jun 24 04:21:55 2023, max compression
+gzip compressed data, was "micropython_wifi_communication-0.0.7.tar", last modified: Sat Jun 24 18:02:25 2023, max compression
```

## Comparing `micropython_wifi_communication-0.0.6.tar` & `micropython_wifi_communication-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 04:21:55.866841 micropython_wifi_communication-0.0.6/
--rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.6/LICENCE
--rw-rw-rw-   0        0        0     1179 2023-06-24 04:21:55.864466 micropython_wifi_communication-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      741 2023-06-24 04:21:10.000000 micropython_wifi_communication-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 04:21:55.822849 micropython_wifi_communication-0.0.6/comu/
--rw-rw-rw-   0        0        0       71 2023-06-16 17:37:27.000000 micropython_wifi_communication-0.0.6/comu/__init__.py
--rw-rw-rw-   0        0        0     2792 2023-06-24 04:14:24.000000 micropython_wifi_communication-0.0.6/comu/cli.py
--rw-rw-rw-   0        0        0     2694 2023-06-20 21:22:54.000000 micropython_wifi_communication-0.0.6/comu/ser.py
--rw-rw-rw-   0        0        0      386 2023-06-15 18:40:47.000000 micropython_wifi_communication-0.0.6/comu/util.py
-drwxrwxrwx   0        0        0        0 2023-06-24 04:21:55.863060 micropython_wifi_communication-0.0.6/micropython_wifi_communication.egg-info/
--rw-rw-rw-   0        0        0     1179 2023-06-24 04:21:54.000000 micropython_wifi_communication-0.0.6/micropython_wifi_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-24 04:21:55.000000 micropython_wifi_communication-0.0.6/micropython_wifi_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 04:21:54.000000 micropython_wifi_communication-0.0.6/micropython_wifi_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-24 04:21:54.000000 micropython_wifi_communication-0.0.6/micropython_wifi_communication.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 04:21:55.866841 micropython_wifi_communication-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-06-24 04:13:15.000000 micropython_wifi_communication-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:02:25.337987 micropython_wifi_communication-0.0.7/
+-rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.7/LICENCE
+-rw-rw-rw-   0        0        0     1179 2023-06-24 18:02:25.335233 micropython_wifi_communication-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-06-24 04:21:10.000000 micropython_wifi_communication-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 18:02:25.324850 micropython_wifi_communication-0.0.7/comu/
+-rw-rw-rw-   0        0        0       71 2023-06-16 17:37:27.000000 micropython_wifi_communication-0.0.7/comu/__init__.py
+-rw-rw-rw-   0        0        0     2914 2023-06-24 18:00:12.000000 micropython_wifi_communication-0.0.7/comu/cli.py
+-rw-rw-rw-   0        0        0     4209 2023-06-24 18:00:12.000000 micropython_wifi_communication-0.0.7/comu/ser.py
+-rw-rw-rw-   0        0        0     2019 2023-06-24 18:00:12.000000 micropython_wifi_communication-0.0.7/comu/util.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:02:25.335233 micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/
+-rw-rw-rw-   0        0        0     1179 2023-06-24 18:02:25.000000 micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-24 18:02:25.000000 micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:02:25.000000 micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-24 18:02:25.000000 micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 18:02:25.337987 micropython_wifi_communication-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      510 2023-06-24 18:02:07.000000 micropython_wifi_communication-0.0.7/setup.py
```

### Comparing `micropython_wifi_communication-0.0.6/LICENCE` & `micropython_wifi_communication-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.6/PKG-INFO` & `micropython_wifi_communication-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython_wifi_communication
-Version: 0.0.6
+Version: 0.0.7
 Summary: um substituto para em vez de uma comunicação RF utilizar wifi
 Home-page: UNKNOWN
 Author: issei momonge
 Author-email: mggyggf@gmail.com
 License: MIT License
 Keywords: socket communication via wifi
 Platform: UNKNOWN
```

### Comparing `micropython_wifi_communication-0.0.6/README.md` & `micropython_wifi_communication-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.6/comu/cli.py` & `micropython_wifi_communication-0.0.7/comu/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import socket
-import network
-from comu.util import validator
+netw = True
+try:
+    import network
+except:
+    netw = False
+from comu.util import validator, ip
 from time import sleep
 
 class ci:
 
     def __init__(self, net=None, Host='50.1', tr=1024):
         self.net = net
         x = None
@@ -13,26 +17,28 @@
                 self.cone()
                 x = True
             except:
                 pass
             sleep(1)
         self.trans = tr
         self.HOST = '192.168.' + Host  # Endereço IP do servidor
+        self.HOST = ip(self.HOST)[0]
         self.PORT = 1234  # Porta para comunicação
 
         # Cria o socket TCP/IP
         self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.client_socket.settimeout(None)
         # Conecta-se ao servidor
         self.client_socket.connect((self.HOST, self.PORT))
         self.client_socket.settimeout(300)
 
     def cone(self):
+        global netw
         net = self.net
-        if net:
+        if net and netw:
             if type(net) != dict:
                 net = {}
             sta_if = network.WLAN(network.STA_IF)
             if not sta_if.isconnected():
                 print('Conectando-se à rede Wi-Fi...')
                 sta_if.active(True)
                 ssid = 'MinhaRedeWiFI'
```

### Comparing `micropython_wifi_communication-0.0.6/micropython_wifi_communication.egg-info/PKG-INFO` & `micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-wifi-communication
-Version: 0.0.6
+Version: 0.0.7
 Summary: um substituto para em vez de uma comunicação RF utilizar wifi
 Home-page: UNKNOWN
 Author: issei momonge
 Author-email: mggyggf@gmail.com
 License: MIT License
 Keywords: socket communication via wifi
 Platform: UNKNOWN
```

