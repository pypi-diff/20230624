# Comparing `tmp/micropython_wifi_communication-0.0.5.tar.gz` & `tmp/micropython_wifi_communication-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_wifi_communication-0.0.5.tar", last modified: Tue Jun 20 21:23:55 2023, max compression
+gzip compressed data, was "micropython_wifi_communication-0.0.6.tar", last modified: Sat Jun 24 04:21:55 2023, max compression
```

## Comparing `micropython_wifi_communication-0.0.5.tar` & `micropython_wifi_communication-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 21:23:55.740391 micropython_wifi_communication-0.0.5/
--rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.5/LICENCE
--rw-rw-rw-   0        0        0      409 2023-06-20 21:23:55.740391 micropython_wifi_communication-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-16 00:29:04.000000 micropython_wifi_communication-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 21:23:55.727124 micropython_wifi_communication-0.0.5/comu/
--rw-rw-rw-   0        0        0       71 2023-06-16 17:37:27.000000 micropython_wifi_communication-0.0.5/comu/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-20 21:22:54.000000 micropython_wifi_communication-0.0.5/comu/cli.py
--rw-rw-rw-   0        0        0     2694 2023-06-20 21:22:54.000000 micropython_wifi_communication-0.0.5/comu/ser.py
--rw-rw-rw-   0        0        0      386 2023-06-15 18:40:47.000000 micropython_wifi_communication-0.0.5/comu/util.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:23:55.738958 micropython_wifi_communication-0.0.5/micropython_wifi_communication.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-20 21:23:54.000000 micropython_wifi_communication-0.0.5/micropython_wifi_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-20 21:23:54.000000 micropython_wifi_communication-0.0.5/micropython_wifi_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 21:23:54.000000 micropython_wifi_communication-0.0.5/micropython_wifi_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-20 21:23:54.000000 micropython_wifi_communication-0.0.5/micropython_wifi_communication.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 21:23:55.740391 micropython_wifi_communication-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-06-20 21:23:14.000000 micropython_wifi_communication-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 04:21:55.866841 micropython_wifi_communication-0.0.6/
+-rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.6/LICENCE
+-rw-rw-rw-   0        0        0     1179 2023-06-24 04:21:55.864466 micropython_wifi_communication-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-06-24 04:21:10.000000 micropython_wifi_communication-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 04:21:55.822849 micropython_wifi_communication-0.0.6/comu/
+-rw-rw-rw-   0        0        0       71 2023-06-16 17:37:27.000000 micropython_wifi_communication-0.0.6/comu/__init__.py
+-rw-rw-rw-   0        0        0     2792 2023-06-24 04:14:24.000000 micropython_wifi_communication-0.0.6/comu/cli.py
+-rw-rw-rw-   0        0        0     2694 2023-06-20 21:22:54.000000 micropython_wifi_communication-0.0.6/comu/ser.py
+-rw-rw-rw-   0        0        0      386 2023-06-15 18:40:47.000000 micropython_wifi_communication-0.0.6/comu/util.py
+drwxrwxrwx   0        0        0        0 2023-06-24 04:21:55.863060 micropython_wifi_communication-0.0.6/micropython_wifi_communication.egg-info/
+-rw-rw-rw-   0        0        0     1179 2023-06-24 04:21:54.000000 micropython_wifi_communication-0.0.6/micropython_wifi_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-24 04:21:55.000000 micropython_wifi_communication-0.0.6/micropython_wifi_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 04:21:54.000000 micropython_wifi_communication-0.0.6/micropython_wifi_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-24 04:21:54.000000 micropython_wifi_communication-0.0.6/micropython_wifi_communication.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 04:21:55.866841 micropython_wifi_communication-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      510 2023-06-24 04:13:15.000000 micropython_wifi_communication-0.0.6/setup.py
```

### Comparing `micropython_wifi_communication-0.0.5/LICENCE` & `micropython_wifi_communication-0.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.5/comu/cli.py` & `micropython_wifi_communication-0.0.6/comu/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,22 @@
 from comu.util import validator
 from time import sleep
 
 class ci:
 
     def __init__(self, net=None, Host='50.1', tr=1024):
         self.net = net
-        self.cone()
+        x = None
+        while not x:
+            try:
+                self.cone()
+                x = True
+            except:
+                pass
+            sleep(1)
         self.trans = tr
         self.HOST = '192.168.' + Host  # Endereço IP do servidor
         self.PORT = 1234  # Porta para comunicação
 
         # Cria o socket TCP/IP
         self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.client_socket.settimeout(None)
@@ -24,18 +31,18 @@
         if net:
             if type(net) != dict:
                 net = {}
             sta_if = network.WLAN(network.STA_IF)
             if not sta_if.isconnected():
                 print('Conectando-se à rede Wi-Fi...')
                 sta_if.active(True)
-                ssid = ''
+                ssid = 'MinhaRedeWiFI'
                 if 'ssid' in net:
                     ssid = net['ssid']
-                password = ''
+                password = 'MinhaSenha123'
                 if 'password' in net:
                     password = net['password']
                 if password != '':
                     sta_if.connect(ssid, password)
                 else:
                     sta_if.connect(ssid)
                 while not sta_if.isconnected():
```

### Comparing `micropython_wifi_communication-0.0.5/comu/ser.py` & `micropython_wifi_communication-0.0.6/comu/ser.py`

 * *Files identical despite different names*

