# Comparing `tmp/micropython_wifi_communication-0.0.7.tar.gz` & `tmp/micropython_wifi_communication-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_wifi_communication-0.0.7.tar", last modified: Sat Jun 24 18:02:25 2023, max compression
+gzip compressed data, was "micropython_wifi_communication-0.0.8.tar", last modified: Sat Jun 24 20:38:37 2023, max compression
```

## Comparing `micropython_wifi_communication-0.0.7.tar` & `micropython_wifi_communication-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:02:25.337987 micropython_wifi_communication-0.0.7/
--rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.7/LICENCE
--rw-rw-rw-   0        0        0     1179 2023-06-24 18:02:25.335233 micropython_wifi_communication-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      741 2023-06-24 04:21:10.000000 micropython_wifi_communication-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 18:02:25.324850 micropython_wifi_communication-0.0.7/comu/
--rw-rw-rw-   0        0        0       71 2023-06-16 17:37:27.000000 micropython_wifi_communication-0.0.7/comu/__init__.py
--rw-rw-rw-   0        0        0     2914 2023-06-24 18:00:12.000000 micropython_wifi_communication-0.0.7/comu/cli.py
--rw-rw-rw-   0        0        0     4209 2023-06-24 18:00:12.000000 micropython_wifi_communication-0.0.7/comu/ser.py
--rw-rw-rw-   0        0        0     2019 2023-06-24 18:00:12.000000 micropython_wifi_communication-0.0.7/comu/util.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:02:25.335233 micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/
--rw-rw-rw-   0        0        0     1179 2023-06-24 18:02:25.000000 micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-24 18:02:25.000000 micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:02:25.000000 micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-24 18:02:25.000000 micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 18:02:25.337987 micropython_wifi_communication-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-06-24 18:02:07.000000 micropython_wifi_communication-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:38:37.496570 micropython_wifi_communication-0.0.8/
+-rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.8/LICENCE
+-rw-rw-rw-   0        0        0     1231 2023-06-24 20:38:37.496570 micropython_wifi_communication-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      789 2023-06-24 20:38:01.000000 micropython_wifi_communication-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 20:38:37.466648 micropython_wifi_communication-0.0.8/comu/
+-rw-rw-rw-   0        0        0       71 2023-06-16 17:37:27.000000 micropython_wifi_communication-0.0.8/comu/__init__.py
+-rw-rw-rw-   0        0        0     3518 2023-06-24 20:37:35.000000 micropython_wifi_communication-0.0.8/comu/cli.py
+-rw-rw-rw-   0        0        0     4436 2023-06-24 20:37:27.000000 micropython_wifi_communication-0.0.8/comu/ser.py
+-rw-rw-rw-   0        0        0     2157 2023-06-24 20:38:14.000000 micropython_wifi_communication-0.0.8/comu/util.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:38:37.494416 micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/
+-rw-rw-rw-   0        0        0     1231 2023-06-24 20:38:36.000000 micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-24 20:38:36.000000 micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 20:38:36.000000 micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-24 20:38:36.000000 micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 20:38:37.496570 micropython_wifi_communication-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      510 2023-06-24 20:36:44.000000 micropython_wifi_communication-0.0.8/setup.py
```

### Comparing `micropython_wifi_communication-0.0.7/LICENCE` & `micropython_wifi_communication-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.7/PKG-INFO` & `micropython_wifi_communication-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython_wifi_communication
-Version: 0.0.7
+Version: 0.0.8
 Summary: um substituto para em vez de uma comunicação RF utilizar wifi
 Home-page: UNKNOWN
 Author: issei momonge
 Author-email: mggyggf@gmail.com
 License: MIT License
 Keywords: socket communication via wifi
 Platform: UNKNOWN
@@ -68,7 +68,11 @@
     x = 0
 
     while True:
         c.send(x)
         x+=1
         sleep(1)
 
+close server
+    
+    c.close() # or s.close()
+
```

### Comparing `micropython_wifi_communication-0.0.7/README.md` & `micropython_wifi_communication-0.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -53,8 +53,12 @@
     from time import sleep
     
     x = 0
 
     while True:
         c.send(x)
         x+=1
-        sleep(1)
+        sleep(1)
+
+close server
+    
+    c.close() # or s.close()
```

### Comparing `micropython_wifi_communication-0.0.7/comu/cli.py` & `micropython_wifi_communication-0.0.8/comu/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import socket
+
 netw = True
 try:
     import network
 except:
     netw = False
 from comu.util import validator, ip
 from time import sleep
 
+
 class ci:
 
     def __init__(self, net=None, Host='50.1', tr=1024):
         self.net = net
         x = None
         while not x:
             try:
                 self.cone()
                 x = True
             except:
                 pass
             sleep(1)
         self.trans = tr
-        self.HOST = '192.168.' + Host  # Endereço IP do servidor
-        self.HOST = ip(self.HOST)[0]
-        self.PORT = 1234  # Porta para comunicação
+        self.HOST = Host  # Endereço IP do servidor
+        try:
+            self.HOST = ip(self.HOST, self.ifconfig)[0]
+        except:
+            self.HOST = ip(self.HOST)[0]
+        self.PORT = 1238  # Porta para comunicação
 
         # Cria o socket TCP/IP
         self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.client_socket.settimeout(None)
         # Conecta-se ao servidor
         self.client_socket.connect((self.HOST, self.PORT))
         self.client_socket.settimeout(300)
@@ -35,49 +40,61 @@
         global netw
         net = self.net
         if net and netw:
             if type(net) != dict:
                 net = {}
             sta_if = network.WLAN(network.STA_IF)
             if not sta_if.isconnected():
-                print('Conectando-se à rede Wi-Fi...')
                 sta_if.active(True)
                 ssid = 'MinhaRedeWiFI'
                 if 'ssid' in net:
                     ssid = net['ssid']
                 password = 'MinhaSenha123'
                 if 'password' in net:
                     password = net['password']
                 if password != '':
                     sta_if.connect(ssid, password)
                 else:
                     sta_if.connect(ssid)
                 while not sta_if.isconnected():
                     pass
+            self.ifconfig = sta_if.ifconfig()
 
     def send(self, data):
         try:
             self.client_socket.settimeout(5)
             message = str({1: 1, 'inf': data, 0: 0})
             self.client_socket.send(message.encode())
             self.client_socket.settimeout(None)
         except:
             self.ence()
 
+    def close(self):
+        self.send('jnhvcdtyGHAJHDGDHgftghjnhbftryuikjnbhgvfrtyuiokmnbvgcfrtyuikjnbhvcfrtyui75414578445445741574')
+        self.client_socket.close()
+        raise Exception("Servidor finalizado!")
+
     def recv(self):
+        x = None
         try:
             message = self.client_socket.recv(self.trans).decode()
             if not message:
                 self.ence()
             self.client_socket.settimeout(None)
             va, me = validator(message)
-            if not va:
-                return me['inf']
+            me = me['inf']
+            if me == 'jnhvcdtyGHAJHDGDHgftghjnhbftryuikjnbhgvfrtyuiokmnbvgcfrtyuikjnbhvcfrtyui75414578445445741574':
+                x = True
+            elif not va:
+                return me
         except:
             self.ence()
+        if x:
+            self.client_socket.close()
+            raise Exception("Servidor finalizado pelo server!")
 
     def ence(self):
         x = None
         self.client_socket.close()
         while not x:
             try:
                 wlan = network.WLAN(network.STA_IF)
@@ -85,8 +102,8 @@
                     self.cone()
                 self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 self.client_socket.connect((self.HOST, self.PORT))
                 self.client_socket.settimeout(300)
                 x = True
             except Exception as e:
                 pass
-            sleep(1)
+            sleep(1)
```

### Comparing `micropython_wifi_communication-0.0.7/comu/ser.py` & `micropython_wifi_communication-0.0.8/comu/ser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,124 +1,131 @@
 import socket
+
 netw = True
 try:
     import network
 except:
     netw = False
 from comu.util import validator, ip
+from time import sleep
 
 
 class se:
 
     def __init__(self, net=None, Host='50.1', tr=1024, conecao=False):
         self.trans = tr
-        self.HOST = '192.168.' + Host  # Endereço IP do servidor
-        self.PORT = 1234  # self.PORTa para comunicação
+        self.HOST = Host  # Endereço IP do servidor
+        self.PORT = 1238  # self.PORTa para comunicação
         self.net = net
         self.conecao = conecao
         x = None
         while not x:
             try:
                 self.cone()
                 x = True
-            except:
+            except Exception as e:
                 pass
+            sleep(1)
 
         # Cria o socket TCP/IP
         self.server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
         # Associa o socket ao endereço IP e self.PORTa
         self.server_socket.bind((self.HOST, self.PORT))
 
         # Aguarda por conexões
         self.server_socket.listen(1)
 
         # Aceita uma nova conexão
         self.client_socket, self.client_address = self.server_socket.accept()
         self.client_socket.settimeout(300)
-        print("cliente aceito")
 
     def cone(self):
         net = self.net
         conecao = self.conecao
         global netw
         ap_config = (self.HOST, '255.255.0.0', self.HOST, '255.255.0.0')
+        if type(net) != dict:
+            net = {}
         if net and netw:
-            if type(net) != dict:
-                net = {}
             SSID = 'MinhaRedeWiFI'  # Nome da rede Wi-Fi
             if 'SSID' in net:
                 SSID = net['SSID']
             PASSWORD = 'MinhaSenha123'  # Senha da rede Wi-Fi
             if 'PASSWORD' in net:
                 PASSWORD = net['PASSWORD']
 
             # Configura o ponto de acesso Wi-Fi
-            if conecao:
+            if not conecao:
                 ap = network.WLAN(network.AP_IF)
                 ap.active(True)
                 if PASSWORD != '':
                     ap.config(essid=SSID, authmode=network.AUTH_WPA2_PSK, password=PASSWORD)
                 else:
                     ap.config(essid=SSID)
                 network_config = ap.ifconfig()
 
                 # Atualiza o endereço IP do ponto de acesso para o valor de self.HOST
                 ap.ifconfig(ap_config)
             else:
                 sta_if = network.WLAN(network.STA_IF)
                 if not sta_if.isconnected():
-                    print('Conectando-se à rede Wi-Fi...')
                     sta_if.active(True)
-                    ssid = 'MinhaRedeWiFI'
-                    if 'ssid' in net:
-                        ssid = net['ssid']
-                    password = 'MinhaSenha123'
-                    if 'password' in net:
-                        password = net['password']
-                    if password != '':
-                        sta_if.connect(ssid, password)
+                    if PASSWORD != '':
+                        sta_if.connect(SSID, PASSWORD)
                     else:
-                        sta_if.connect(ssid)
+                        sta_if.connect(SSID)
                     while not sta_if.isconnected():
                         pass
-                    ap_config = ip(self.HOST,sta_if.ifconfig())
-                    self.HOST = ap_config[0]
-
-                    sta_if.ifconfig(ap_config)
+                ap_config = ip(self.HOST, sta_if.ifconfig(),se=True)
+                self.HOST = ap_config[0]
+                sta_if.ifconfig(ap_config)
+        else:
+            self.HOST = ip(self.HOST,se=True)[0]
 
     def send(self, data):
         try:
             self.client_socket.settimeout(5)
             message = str({1: 1, 'inf': data, 0: 0})
             self.client_socket.send(message.encode())
             self.client_socket.settimeout(None)
         except:
             self.ence()
 
+    def close(self):
+        self.send('jnhvcdtyGHAJHDGDHgftghjnhbftryuikjnbhgvfrtyuiokmnbvgcfrtyuikjnbhvcfrtyui75414578445445741574')
+        self.client_socket.close()
+        raise Exception("Servidor finalizado!")
+
     def recv(self):
+        x=None
         try:
             message = self.client_socket.recv(self.trans).decode()
             if not message:
                 self.ence()
             self.client_socket.settimeout(None)
             va, me = validator(message)
-            if not va:
-                return me['inf']
+            me = me['inf']
+            if me == 'jnhvcdtyGHAJHDGDHgftghjnhbftryuikjnbhgvfrtyuiokmnbvgcfrtyuikjnbhvcfrtyui75414578445445741574':
+                x = True
+            elif not va:
+                return me
         except:
             self.ence()
+        if x:
+            self.client_socket.close()
+            raise Exception("Servidor finalizado pelo cliente!")
 
     def ence(self):
         x = None
         while not x:
             try:
                 self.cone()
                 # self.client_socket.close()
                 self.server_socket.listen(1)
                 # Aceita uma nova conexão
                 self.client_socket, self.client_address = self.server_socket.accept()
                 self.client_socket.settimeout(300)
-                print("cliente aceito")
                 x = True
             except Exception as e:
-                print(e)
-                pass
+                pass
+            sleep(1)
```

### Comparing `micropython_wifi_communication-0.0.7/comu/util.py` & `micropython_wifi_communication-0.0.8/comu/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,127 +1,135 @@
-00000000: 6465 6620 7661 6c69 6461 746f 7228 6974  def validator(it
-00000010: 656d 293a 0d0a 2020 2020 6974 656d 203d  em):..    item =
-00000020: 2069 7465 6d2e 7370 6c69 7428 2730 3a20   item.split('0: 
-00000030: 307d 2729 0d0a 2020 2020 6974 656d 203d  0}')..    item =
-00000040: 2069 7465 6d5b 6c65 6e28 6974 656d 2920   item[len(item) 
-00000050: 2d20 325d 202b 2027 303a 2030 7d27 0d0a  - 2] + '0: 0}'..
-00000060: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00000070: 2020 6974 656d 203d 2065 7661 6c28 6974    item = eval(it
-00000080: 656d 290d 0a20 2020 2065 7863 6570 743a  em)..    except:
-00000090: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000000a0: 2054 7275 652c 2046 616c 7365 0d0a 2020   True, False..  
-000000b0: 2020 7820 3d20 4661 6c73 650d 0a20 2020    x = False..   
-000000c0: 2079 203d 2046 616c 7365 0d0a 2020 2020   y = False..    
-000000d0: 7472 793a 0d0a 2020 2020 2020 2020 6974  try:..        it
-000000e0: 656d 5b31 5d0d 0a20 2020 2065 7863 6570  em[1]..    excep
-000000f0: 743a 0d0a 2020 2020 2020 2020 7820 3d20  t:..        x = 
-00000100: 5472 7565 0d0a 2020 2020 7472 793a 0d0a  True..    try:..
-00000110: 2020 2020 2020 2020 6974 656d 5b30 5d0d          item[0].
-00000120: 0a20 2020 2065 7863 6570 743a 0d0a 2020  .    except:..  
-00000130: 2020 2020 2020 7920 3d20 5472 7565 0d0a        y = True..
-00000140: 2020 2020 6966 2078 206f 7220 793a 0d0a      if x or y:..
-00000150: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00000160: 7275 652c 2046 616c 7365 0d0a 2020 2020  rue, False..    
-00000170: 7265 7475 726e 2046 616c 7365 2c20 6974  return False, it
-00000180: 656d 0d0a 0d0a 6465 6620 6765 745f 6970  em....def get_ip
-00000190: 5f61 6e64 5f6e 6574 6d61 736b 5f69 6e5f  _and_netmask_in_
-000001a0: 7769 6e64 6f73 2829 3a0d 0a20 2020 2069  windos():..    i
-000001b0: 6d70 6f72 7420 7375 6270 726f 6365 7373  mport subprocess
-000001c0: 0d0a 2020 2020 696d 706f 7274 2072 650d  ..    import re.
-000001d0: 0a20 2020 2023 2045 7865 6375 7461 206f  .    # Executa o
-000001e0: 2063 6f6d 616e 646f 2069 7063 6f6e 6669   comando ipconfi
-000001f0: 670d 0a20 2020 206f 7574 7075 7420 3d20  g..    output = 
-00000200: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-00000210: 5f6f 7574 7075 7428 2769 7063 6f6e 6669  _output('ipconfi
-00000220: 6727 2c20 7368 656c 6c3d 5472 7565 292e  g', shell=True).
-00000230: 6465 636f 6465 2827 6c61 7469 6e2d 3127  decode('latin-1'
-00000240: 290d 0a20 2020 206f 7574 7075 7420 3d20  )..    output = 
-00000250: 6f75 7470 7574 2e73 706c 6974 2827 4164  output.split('Ad
-00000260: 6170 7461 646f 7220 6465 2052 6564 6520  aptador de Rede 
-00000270: 7365 6d20 4669 6f20 5769 2d46 693a 2729  sem Fio Wi-Fi:')
-00000280: 5b31 5d0d 0a0d 0a20 2020 2023 2050 726f  [1]....    # Pro
-00000290: 6375 7261 2070 656c 6f20 656e 6465 7265  cura pelo endere
-000002a0: c3a7 6f20 4950 2064 6120 7265 6465 2065  ..o IP da rede e
-000002b0: 2070 656c 6120 6dc3 a173 6361 7261 2064   pela m..scara d
-000002c0: 6520 7265 6465 206e 6120 7361 c3ad 6461  e rede na sa..da
-000002d0: 0d0a 2020 2020 6970 5f72 6567 6578 203d  ..    ip_regex =
-000002e0: 2072 2249 5076 342e 202e 2b3f 3a20 285b   r"IPv4. .+?: ([
-000002f0: 5c64 2e5d 2b29 220d 0a20 2020 206d 6173  \d.]+)"..    mas
-00000300: 6b5f 7265 6765 7820 3d20 7222 5375 622d  k_regex = r"Sub-
-00000310: 7265 6465 202e 202e 2b3f 3a20 285b 5c64  rede . .+?: ([\d
-00000320: 2e5d 2b29 220d 0a0d 0a20 2020 2069 705f  .]+)"....    ip_
-00000330: 6d61 7463 6820 3d20 7265 2e73 6561 7263  match = re.searc
-00000340: 6828 6970 5f72 6567 6578 2c20 6f75 7470  h(ip_regex, outp
-00000350: 7574 290d 0a20 2020 206d 6173 6b5f 6d61  ut)..    mask_ma
-00000360: 7463 6820 3d20 7265 2e73 6561 7263 6828  tch = re.search(
-00000370: 6d61 736b 5f72 6567 6578 2c20 6f75 7470  mask_regex, outp
-00000380: 7574 290d 0a0d 0a20 2020 2069 6620 6970  ut)....    if ip
-00000390: 5f6d 6174 6368 2061 6e64 206d 6173 6b5f  _match and mask_
-000003a0: 6d61 7463 683a 0d0a 2020 2020 2020 2020  match:..        
-000003b0: 6970 5f61 6464 7265 7373 203d 2069 705f  ip_address = ip_
-000003c0: 6d61 7463 682e 6772 6f75 7028 3129 0d0a  match.group(1)..
-000003d0: 2020 2020 2020 2020 6e65 746d 6173 6b20          netmask 
-000003e0: 3d20 6d61 736b 5f6d 6174 6368 2e67 726f  = mask_match.gro
-000003f0: 7570 2831 290d 0a0d 0a20 2020 2020 2020  up(1)....       
-00000400: 2072 6574 7572 6e20 6970 5f61 6464 7265   return ip_addre
-00000410: 7373 2c20 6e65 746d 6173 6b0d 0a0d 0a20  ss, netmask.... 
-00000420: 2020 2072 6574 7572 6e20 4e6f 6e65 2c20     return None, 
-00000430: 4e6f 6e65 2020 2320 5265 746f 726e 6120  None  # Retorna 
-00000440: 4e6f 6e65 2073 6520 6ec3 a36f 2065 6e63  None se n..o enc
-00000450: 6f6e 7472 6f75 2061 7320 696e 666f 726d  ontrou as inform
-00000460: 61c3 a7c3 b565 730d 0a0d 0a64 6566 2069  a....es....def i
-00000470: 7028 686f 7374 2c69 706d 736b 3d4e 6f6e  p(host,ipmsk=Non
-00000480: 6529 3a0d 0a20 2020 2068 6f73 7431 203d  e):..    host1 =
-00000490: 204e 6f6e 650d 0a20 2020 206d 6173 6b31   None..    mask1
-000004a0: 203d 204e 6f6e 650d 0a20 2020 2068 6f73   = None..    hos
-000004b0: 7432 203d 204e 6f6e 650d 0a20 2020 206d  t2 = None..    m
-000004c0: 6173 6b32 203d 204e 6f6e 650d 0a20 2020  ask2 = None..   
-000004d0: 2069 6620 6970 6d73 6b3a 0d0a 2020 2020   if ipmsk:..    
-000004e0: 2020 2020 6966 2074 7970 6528 6970 6d73      if type(ipms
-000004f0: 6b29 203d 3d20 7475 706c 653a 0d0a 2020  k) == tuple:..  
-00000500: 2020 2020 2020 2020 2020 686f 7374 312c            host1,
-00000510: 206d 6173 6b31 2c20 686f 7374 322c 206d   mask1, host2, m
-00000520: 6173 6b32 203d 2069 706d 736b 0d0a 2020  ask2 = ipmsk..  
-00000530: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00000540: 2068 6f73 7431 2c20 6d61 736b 3120 3d20   host1, mask1 = 
-00000550: 6765 745f 6970 5f61 6e64 5f6e 6574 6d61  get_ip_and_netma
-00000560: 736b 5f69 6e5f 7769 6e64 6f73 2829 0d0a  sk_in_windos()..
-00000570: 2020 2020 2020 2020 686f 7374 3220 3d20          host2 = 
-00000580: 686f 7374 310d 0a20 2020 2020 2020 206d  host1..        m
-00000590: 6173 6b32 203d 206d 6173 6b31 0d0a 2020  ask2 = mask1..  
-000005a0: 2020 6d61 7363 6172 6120 3d20 6d61 736b    mascara = mask
-000005b0: 312e 7370 6c69 7428 272e 2729 0d0a 2020  1.split('.')..  
-000005c0: 2020 686f 7374 7061 6472 616f 203d 2068    hostpadrao = h
-000005d0: 6f73 7431 2e73 706c 6974 2827 2e27 290d  ost1.split('.').
-000005e0: 0a20 2020 2069 7066 696e 616c 203d 2027  .    ipfinal = '
-000005f0: 270d 0a20 2020 2078 203d 2030 0d0a 2020  '..    x = 0..  
-00000600: 2020 6573 7061 736f 7320 3d20 300d 0a20    espasos = 0.. 
-00000610: 2020 2066 6f72 2069 2069 6e20 6d61 7363     for i in masc
-00000620: 6172 613a 0d0a 2020 2020 2020 2020 6920  ara:..        i 
-00000630: 3d20 696e 7428 6929 0d0a 2020 2020 2020  = int(i)..      
-00000640: 2020 6966 2069 203d 3d20 3235 353a 0d0a    if i == 255:..
-00000650: 2020 2020 2020 2020 2020 2020 6970 6669              ipfi
-00000660: 6e61 6c2b 3d66 277b 7374 7228 686f 7374  nal+=f'{str(host
-00000670: 7061 6472 616f 5b78 5d29 7d2e 270d 0a20  padrao[x])}.'.. 
-00000680: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00000690: 2020 2020 2020 2020 2020 6573 7061 736f            espaso
-000006a0: 732b 3d31 0d0a 2020 2020 2020 2020 782b  s+=1..        x+
-000006b0: 3d31 0d0a 2020 2020 686f 7374 203d 2068  =1..    host = h
-000006c0: 6f73 742e 7370 6c69 7428 272e 2729 0d0a  ost.split('.')..
-000006d0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-000006e0: 6765 286c 656e 2868 6f73 7429 2d31 293a  ge(len(host)-1):
-000006f0: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00000700: 2065 7370 6173 6f73 203d 3d20 6c65 6e28   espasos == len(
-00000710: 686f 7374 293a 0d0a 2020 2020 2020 2020  host):..        
-00000720: 2020 2020 6465 6c20 686f 7374 5b30 5d0d      del host[0].
-00000730: 0a20 2020 2078 3d31 0d0a 2020 2020 666f  .    x=1..    fo
-00000740: 7220 6920 696e 2068 6f73 743a 0d0a 2020  r i in host:..  
-00000750: 2020 2020 2020 6966 2078 203d 3d20 6c65        if x == le
-00000760: 6e28 686f 7374 293a 0d0a 2020 2020 2020  n(host):..      
-00000770: 2020 2020 2020 6970 6669 6e61 6c2b 3d69        ipfinal+=i
-00000780: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00000790: 0a20 2020 2020 2020 2020 2020 2069 7066  .            ipf
-000007a0: 696e 616c 2b3d 692b 272e 270d 0a20 2020  inal+=i+'.'..   
-000007b0: 2020 2020 2078 2b3d 310d 0a20 2020 2072       x+=1..    r
-000007c0: 6574 7572 6e20 2869 7066 696e 616c 2c6d  eturn (ipfinal,m
-000007d0: 6173 6b31 2c69 7066 696e 616c 2c6d 6173  ask1,ipfinal,mas
-000007e0: 6b31 29                                  k1)
+00000000: 0d0a 6465 6620 7661 6c69 6461 746f 7228  ..def validator(
+00000010: 6974 656d 293a 0d0a 2020 2020 6974 656d  item):..    item
+00000020: 203d 2069 7465 6d2e 7370 6c69 7428 2730   = item.split('0
+00000030: 3a20 307d 2729 0d0a 2020 2020 6974 656d  : 0}')..    item
+00000040: 203d 2069 7465 6d5b 6c65 6e28 6974 656d   = item[len(item
+00000050: 2920 2d20 325d 202b 2027 303a 2030 7d27  ) - 2] + '0: 0}'
+00000060: 0d0a 2020 2020 7472 793a 0d0a 2020 2020  ..    try:..    
+00000070: 2020 2020 6974 656d 203d 2065 7661 6c28      item = eval(
+00000080: 6974 656d 290d 0a20 2020 2065 7863 6570  item)..    excep
+00000090: 743a 0d0a 2020 2020 2020 2020 7265 7475  t:..        retu
+000000a0: 726e 2054 7275 652c 2046 616c 7365 0d0a  rn True, False..
+000000b0: 2020 2020 7820 3d20 4661 6c73 650d 0a20      x = False.. 
+000000c0: 2020 2079 203d 2046 616c 7365 0d0a 2020     y = False..  
+000000d0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+000000e0: 6974 656d 5b31 5d0d 0a20 2020 2065 7863  item[1]..    exc
+000000f0: 6570 743a 0d0a 2020 2020 2020 2020 7820  ept:..        x 
+00000100: 3d20 5472 7565 0d0a 2020 2020 7472 793a  = True..    try:
+00000110: 0d0a 2020 2020 2020 2020 6974 656d 5b30  ..        item[0
+00000120: 5d0d 0a20 2020 2065 7863 6570 743a 0d0a  ]..    except:..
+00000130: 2020 2020 2020 2020 7920 3d20 5472 7565          y = True
+00000140: 0d0a 2020 2020 6966 2078 206f 7220 793a  ..    if x or y:
+00000150: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000160: 2054 7275 652c 2046 616c 7365 0d0a 2020   True, False..  
+00000170: 2020 7265 7475 726e 2046 616c 7365 2c20    return False, 
+00000180: 6974 656d 0d0a 0d0a 6465 6620 6765 745f  item....def get_
+00000190: 6970 5f61 6e64 5f6e 6574 6d61 736b 5f69  ip_and_netmask_i
+000001a0: 6e5f 7769 6e64 6f73 2829 3a0d 0a20 2020  n_windos():..   
+000001b0: 2069 6d70 6f72 7420 7375 6270 726f 6365   import subproce
+000001c0: 7373 0d0a 2020 2020 696d 706f 7274 2072  ss..    import r
+000001d0: 650d 0a20 2020 2023 2045 7865 6375 7461  e..    # Executa
+000001e0: 206f 2063 6f6d 616e 646f 2069 7063 6f6e   o comando ipcon
+000001f0: 6669 670d 0a20 2020 206f 7574 7075 7420  fig..    output 
+00000200: 3d20 7375 6270 726f 6365 7373 2e63 6865  = subprocess.che
+00000210: 636b 5f6f 7574 7075 7428 2769 7063 6f6e  ck_output('ipcon
+00000220: 6669 6727 2c20 7368 656c 6c3d 5472 7565  fig', shell=True
+00000230: 292e 6465 636f 6465 2827 6c61 7469 6e2d  ).decode('latin-
+00000240: 3127 290d 0a20 2020 206f 7574 7075 7420  1')..    output 
+00000250: 3d20 6f75 7470 7574 2e73 706c 6974 2827  = output.split('
+00000260: 4164 6170 7461 646f 7220 6465 2052 6564  Adaptador de Red
+00000270: 6520 7365 6d20 4669 6f20 5769 2d46 693a  e sem Fio Wi-Fi:
+00000280: 2729 5b31 5d0d 0a0d 0a20 2020 2023 2050  ')[1]....    # P
+00000290: 726f 6375 7261 2070 656c 6f20 656e 6465  rocura pelo ende
+000002a0: 7265 c3a7 6f20 4950 2064 6120 7265 6465  re..o IP da rede
+000002b0: 2065 2070 656c 6120 6dc3 a173 6361 7261   e pela m..scara
+000002c0: 2064 6520 7265 6465 206e 6120 7361 c3ad   de rede na sa..
+000002d0: 6461 0d0a 2020 2020 6970 5f72 6567 6578  da..    ip_regex
+000002e0: 203d 2072 2249 5076 342e 202e 2b3f 3a20   = r"IPv4. .+?: 
+000002f0: 285b 5c64 2e5d 2b29 220d 0a20 2020 206d  ([\d.]+)"..    m
+00000300: 6173 6b5f 7265 6765 7820 3d20 7222 5375  ask_regex = r"Su
+00000310: 622d 7265 6465 202e 202e 2b3f 3a20 285b  b-rede . .+?: ([
+00000320: 5c64 2e5d 2b29 220d 0a0d 0a20 2020 2069  \d.]+)"....    i
+00000330: 705f 6d61 7463 6820 3d20 7265 2e73 6561  p_match = re.sea
+00000340: 7263 6828 6970 5f72 6567 6578 2c20 6f75  rch(ip_regex, ou
+00000350: 7470 7574 290d 0a20 2020 206d 6173 6b5f  tput)..    mask_
+00000360: 6d61 7463 6820 3d20 7265 2e73 6561 7263  match = re.searc
+00000370: 6828 6d61 736b 5f72 6567 6578 2c20 6f75  h(mask_regex, ou
+00000380: 7470 7574 290d 0a0d 0a20 2020 2069 6620  tput)....    if 
+00000390: 6970 5f6d 6174 6368 2061 6e64 206d 6173  ip_match and mas
+000003a0: 6b5f 6d61 7463 683a 0d0a 2020 2020 2020  k_match:..      
+000003b0: 2020 6970 5f61 6464 7265 7373 203d 2069    ip_address = i
+000003c0: 705f 6d61 7463 682e 6772 6f75 7028 3129  p_match.group(1)
+000003d0: 0d0a 2020 2020 2020 2020 6e65 746d 6173  ..        netmas
+000003e0: 6b20 3d20 6d61 736b 5f6d 6174 6368 2e67  k = mask_match.g
+000003f0: 726f 7570 2831 290d 0a0d 0a20 2020 2020  roup(1)....     
+00000400: 2020 2072 6574 7572 6e20 6970 5f61 6464     return ip_add
+00000410: 7265 7373 2c20 6e65 746d 6173 6b0d 0a0d  ress, netmask...
+00000420: 0a20 2020 2072 6574 7572 6e20 4e6f 6e65  .    return None
+00000430: 2c20 4e6f 6e65 2020 2320 5265 746f 726e  , None  # Retorn
+00000440: 6120 4e6f 6e65 2073 6520 6ec3 a36f 2065  a None se n..o e
+00000450: 6e63 6f6e 7472 6f75 2061 7320 696e 666f  ncontrou as info
+00000460: 726d 61c3 a7c3 b565 730d 0a0d 0a64 6566  rma....es....def
+00000470: 2069 7028 686f 7374 2c69 706d 736b 3d4e   ip(host,ipmsk=N
+00000480: 6f6e 652c 7365 3d4e 6f6e 6529 3a0d 0a20  one,se=None):.. 
+00000490: 2020 2068 6f73 7431 203d 204e 6f6e 650d     host1 = None.
+000004a0: 0a20 2020 206d 6173 6b31 203d 204e 6f6e  .    mask1 = Non
+000004b0: 650d 0a20 2020 2068 6f73 7432 203d 204e  e..    host2 = N
+000004c0: 6f6e 650d 0a20 2020 206d 6173 6b32 203d  one..    mask2 =
+000004d0: 204e 6f6e 650d 0a20 2020 2069 6620 6970   None..    if ip
+000004e0: 6d73 6b3a 0d0a 2020 2020 2020 2020 6966  msk:..        if
+000004f0: 2074 7970 6528 6970 6d73 6b29 203d 3d20   type(ipmsk) == 
+00000500: 7475 706c 653a 0d0a 2020 2020 2020 2020  tuple:..        
+00000510: 2020 2020 686f 7374 312c 206d 6173 6b31      host1, mask1
+00000520: 2c20 686f 7374 322c 206d 6173 6b32 203d  , host2, mask2 =
+00000530: 2069 706d 736b 0d0a 2020 2020 656c 7365   ipmsk..    else
+00000540: 3a0d 0a20 2020 2020 2020 2068 6f73 7431  :..        host1
+00000550: 2c20 6d61 736b 3120 3d20 6765 745f 6970  , mask1 = get_ip
+00000560: 5f61 6e64 5f6e 6574 6d61 736b 5f69 6e5f  _and_netmask_in_
+00000570: 7769 6e64 6f73 2829 0d0a 2020 2020 2020  windos()..      
+00000580: 2020 686f 7374 3220 3d20 686f 7374 310d    host2 = host1.
+00000590: 0a20 2020 2020 2020 206d 6173 6b32 203d  .        mask2 =
+000005a0: 206d 6173 6b31 0d0a 2020 2020 2020 2020   mask1..        
+000005b0: 6966 2073 653a 0d0a 2020 2020 2020 2020  if se:..        
+000005c0: 2020 2020 7072 696e 7428 6627 486f 7374      print(f'Host
+000005d0: 2070 6172 6120 7365 7220 6164 6963 696f   para ser adicio
+000005e0: 6e61 646f 206e 6f20 6573 7033 323a 207b  nado no esp32: {
+000005f0: 686f 7374 317d 2729 0d0a 2020 2020 2020  host1}')..      
+00000600: 2020 2020 2020 7265 7475 726e 2028 686f        return (ho
+00000610: 7374 312c 6d61 736b 312c 686f 7374 312c  st1,mask1,host1,
+00000620: 6d61 736b 3129 0d0a 2020 2020 6d61 7363  mask1)..    masc
+00000630: 6172 6120 3d20 6d61 736b 312e 7370 6c69  ara = mask1.spli
+00000640: 7428 272e 2729 0d0a 2020 2020 686f 7374  t('.')..    host
+00000650: 7061 6472 616f 203d 2068 6f73 7431 2e73  padrao = host1.s
+00000660: 706c 6974 2827 2e27 290d 0a20 2020 2069  plit('.')..    i
+00000670: 7066 696e 616c 203d 2027 270d 0a20 2020  pfinal = ''..   
+00000680: 2078 203d 2030 0d0a 2020 2020 6573 7061   x = 0..    espa
+00000690: 736f 7320 3d20 300d 0a20 2020 2066 6f72  sos = 0..    for
+000006a0: 2069 2069 6e20 6d61 7363 6172 613a 0d0a   i in mascara:..
+000006b0: 2020 2020 2020 2020 6920 3d20 696e 7428          i = int(
+000006c0: 6929 0d0a 2020 2020 2020 2020 6966 2069  i)..        if i
+000006d0: 203d 3d20 3235 353a 0d0a 2020 2020 2020   == 255:..      
+000006e0: 2020 2020 2020 6970 6669 6e61 6c2b 3d66        ipfinal+=f
+000006f0: 277b 7374 7228 686f 7374 7061 6472 616f  '{str(hostpadrao
+00000700: 5b78 5d29 7d2e 270d 0a20 2020 2020 2020  [x])}.'..       
+00000710: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00000720: 2020 2020 6573 7061 736f 732b 3d31 0d0a      espasos+=1..
+00000730: 2020 2020 2020 2020 782b 3d31 0d0a 2020          x+=1..  
+00000740: 2020 686f 7374 203d 2068 6f73 742e 7370    host = host.sp
+00000750: 6c69 7428 272e 2729 0d0a 2020 2020 666f  lit('.')..    fo
+00000760: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+00000770: 2868 6f73 7429 2d31 293a 0d0a 2020 2020  (host)-1):..    
+00000780: 2020 2020 6966 206e 6f74 2065 7370 6173      if not espas
+00000790: 6f73 203d 3d20 6c65 6e28 686f 7374 293a  os == len(host):
+000007a0: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+000007b0: 6c20 686f 7374 5b30 5d0d 0a20 2020 2078  l host[0]..    x
+000007c0: 3d31 0d0a 2020 2020 666f 7220 6920 696e  =1..    for i in
+000007d0: 2068 6f73 743a 0d0a 2020 2020 2020 2020   host:..        
+000007e0: 6966 2078 203d 3d20 6c65 6e28 686f 7374  if x == len(host
+000007f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00000800: 6970 6669 6e61 6c2b 3d69 0d0a 2020 2020  ipfinal+=i..    
+00000810: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000820: 2020 2020 2020 2069 7066 696e 616c 2b3d         ipfinal+=
+00000830: 692b 272e 270d 0a20 2020 2020 2020 2078  i+'.'..        x
+00000840: 2b3d 310d 0a20 2020 2072 6574 7572 6e20  +=1..    return 
+00000850: 2869 7066 696e 616c 2c6d 6173 6b31 2c69  (ipfinal,mask1,i
+00000860: 7066 696e 616c 2c6d 6173 6b31 29         pfinal,mask1)
```

### Comparing `micropython_wifi_communication-0.0.7/micropython_wifi_communication.egg-info/PKG-INFO` & `micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-wifi-communication
-Version: 0.0.7
+Version: 0.0.8
 Summary: um substituto para em vez de uma comunicação RF utilizar wifi
 Home-page: UNKNOWN
 Author: issei momonge
 Author-email: mggyggf@gmail.com
 License: MIT License
 Keywords: socket communication via wifi
 Platform: UNKNOWN
@@ -68,7 +68,11 @@
     x = 0
 
     while True:
         c.send(x)
         x+=1
         sleep(1)
 
+close server
+    
+    c.close() # or s.close()
+
```

