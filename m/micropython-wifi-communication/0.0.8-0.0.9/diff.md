# Comparing `tmp/micropython_wifi_communication-0.0.8.tar.gz` & `tmp/micropython_wifi_communication-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_wifi_communication-0.0.8.tar", last modified: Sat Jun 24 20:38:37 2023, max compression
+gzip compressed data, was "micropython_wifi_communication-0.0.9.tar", last modified: Sat Jun 24 20:53:27 2023, max compression
```

## Comparing `micropython_wifi_communication-0.0.8.tar` & `micropython_wifi_communication-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 20:38:37.496570 micropython_wifi_communication-0.0.8/
--rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.8/LICENCE
--rw-rw-rw-   0        0        0     1231 2023-06-24 20:38:37.496570 micropython_wifi_communication-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      789 2023-06-24 20:38:01.000000 micropython_wifi_communication-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 20:38:37.466648 micropython_wifi_communication-0.0.8/comu/
--rw-rw-rw-   0        0        0       71 2023-06-16 17:37:27.000000 micropython_wifi_communication-0.0.8/comu/__init__.py
--rw-rw-rw-   0        0        0     3518 2023-06-24 20:37:35.000000 micropython_wifi_communication-0.0.8/comu/cli.py
--rw-rw-rw-   0        0        0     4436 2023-06-24 20:37:27.000000 micropython_wifi_communication-0.0.8/comu/ser.py
--rw-rw-rw-   0        0        0     2157 2023-06-24 20:38:14.000000 micropython_wifi_communication-0.0.8/comu/util.py
-drwxrwxrwx   0        0        0        0 2023-06-24 20:38:37.494416 micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/
--rw-rw-rw-   0        0        0     1231 2023-06-24 20:38:36.000000 micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-24 20:38:36.000000 micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 20:38:36.000000 micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-24 20:38:36.000000 micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 20:38:37.496570 micropython_wifi_communication-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-06-24 20:36:44.000000 micropython_wifi_communication-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:53:27.186893 micropython_wifi_communication-0.0.9/
+-rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.9/LICENCE
+-rw-rw-rw-   0        0        0     1231 2023-06-24 20:53:27.186893 micropython_wifi_communication-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      789 2023-06-24 20:38:01.000000 micropython_wifi_communication-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 20:53:27.160598 micropython_wifi_communication-0.0.9/comu/
+-rw-rw-rw-   0        0        0       71 2023-06-16 17:37:27.000000 micropython_wifi_communication-0.0.9/comu/__init__.py
+-rw-rw-rw-   0        0        0     3518 2023-06-24 20:37:35.000000 micropython_wifi_communication-0.0.9/comu/cli.py
+-rw-rw-rw-   0        0        0     4436 2023-06-24 20:37:27.000000 micropython_wifi_communication-0.0.9/comu/ser.py
+-rw-rw-rw-   0        0        0     1997 2023-06-24 20:52:41.000000 micropython_wifi_communication-0.0.9/comu/util.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:53:27.185778 micropython_wifi_communication-0.0.9/micropython_wifi_communication.egg-info/
+-rw-rw-rw-   0        0        0     1231 2023-06-24 20:53:27.000000 micropython_wifi_communication-0.0.9/micropython_wifi_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-24 20:53:27.000000 micropython_wifi_communication-0.0.9/micropython_wifi_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 20:53:27.000000 micropython_wifi_communication-0.0.9/micropython_wifi_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-24 20:53:27.000000 micropython_wifi_communication-0.0.9/micropython_wifi_communication.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 20:53:27.186893 micropython_wifi_communication-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      510 2023-06-24 20:53:04.000000 micropython_wifi_communication-0.0.9/setup.py
```

### Comparing `micropython_wifi_communication-0.0.8/LICENCE` & `micropython_wifi_communication-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.8/PKG-INFO` & `micropython_wifi_communication-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython_wifi_communication
-Version: 0.0.8
+Version: 0.0.9
 Summary: um substituto para em vez de uma comunicação RF utilizar wifi
 Home-page: UNKNOWN
 Author: issei momonge
 Author-email: mggyggf@gmail.com
 License: MIT License
 Keywords: socket communication via wifi
 Platform: UNKNOWN
```

### Comparing `micropython_wifi_communication-0.0.8/README.md` & `micropython_wifi_communication-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.8/comu/cli.py` & `micropython_wifi_communication-0.0.9/comu/cli.py`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.8/comu/ser.py` & `micropython_wifi_communication-0.0.9/comu/ser.py`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.8/comu/util.py` & `micropython_wifi_communication-0.0.9/comu/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,114 +22,104 @@
 00000150: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
 00000160: 2054 7275 652c 2046 616c 7365 0d0a 2020   True, False..  
 00000170: 2020 7265 7475 726e 2046 616c 7365 2c20    return False, 
 00000180: 6974 656d 0d0a 0d0a 6465 6620 6765 745f  item....def get_
 00000190: 6970 5f61 6e64 5f6e 6574 6d61 736b 5f69  ip_and_netmask_i
 000001a0: 6e5f 7769 6e64 6f73 2829 3a0d 0a20 2020  n_windos():..   
 000001b0: 2069 6d70 6f72 7420 7375 6270 726f 6365   import subproce
-000001c0: 7373 0d0a 2020 2020 696d 706f 7274 2072  ss..    import r
-000001d0: 650d 0a20 2020 2023 2045 7865 6375 7461  e..    # Executa
-000001e0: 206f 2063 6f6d 616e 646f 2069 7063 6f6e   o comando ipcon
-000001f0: 6669 670d 0a20 2020 206f 7574 7075 7420  fig..    output 
-00000200: 3d20 7375 6270 726f 6365 7373 2e63 6865  = subprocess.che
-00000210: 636b 5f6f 7574 7075 7428 2769 7063 6f6e  ck_output('ipcon
-00000220: 6669 6727 2c20 7368 656c 6c3d 5472 7565  fig', shell=True
-00000230: 292e 6465 636f 6465 2827 6c61 7469 6e2d  ).decode('latin-
-00000240: 3127 290d 0a20 2020 206f 7574 7075 7420  1')..    output 
-00000250: 3d20 6f75 7470 7574 2e73 706c 6974 2827  = output.split('
-00000260: 4164 6170 7461 646f 7220 6465 2052 6564  Adaptador de Red
-00000270: 6520 7365 6d20 4669 6f20 5769 2d46 693a  e sem Fio Wi-Fi:
-00000280: 2729 5b31 5d0d 0a0d 0a20 2020 2023 2050  ')[1]....    # P
-00000290: 726f 6375 7261 2070 656c 6f20 656e 6465  rocura pelo ende
-000002a0: 7265 c3a7 6f20 4950 2064 6120 7265 6465  re..o IP da rede
-000002b0: 2065 2070 656c 6120 6dc3 a173 6361 7261   e pela m..scara
-000002c0: 2064 6520 7265 6465 206e 6120 7361 c3ad   de rede na sa..
-000002d0: 6461 0d0a 2020 2020 6970 5f72 6567 6578  da..    ip_regex
-000002e0: 203d 2072 2249 5076 342e 202e 2b3f 3a20   = r"IPv4. .+?: 
-000002f0: 285b 5c64 2e5d 2b29 220d 0a20 2020 206d  ([\d.]+)"..    m
-00000300: 6173 6b5f 7265 6765 7820 3d20 7222 5375  ask_regex = r"Su
-00000310: 622d 7265 6465 202e 202e 2b3f 3a20 285b  b-rede . .+?: ([
-00000320: 5c64 2e5d 2b29 220d 0a0d 0a20 2020 2069  \d.]+)"....    i
-00000330: 705f 6d61 7463 6820 3d20 7265 2e73 6561  p_match = re.sea
-00000340: 7263 6828 6970 5f72 6567 6578 2c20 6f75  rch(ip_regex, ou
-00000350: 7470 7574 290d 0a20 2020 206d 6173 6b5f  tput)..    mask_
-00000360: 6d61 7463 6820 3d20 7265 2e73 6561 7263  match = re.searc
-00000370: 6828 6d61 736b 5f72 6567 6578 2c20 6f75  h(mask_regex, ou
-00000380: 7470 7574 290d 0a0d 0a20 2020 2069 6620  tput)....    if 
-00000390: 6970 5f6d 6174 6368 2061 6e64 206d 6173  ip_match and mas
-000003a0: 6b5f 6d61 7463 683a 0d0a 2020 2020 2020  k_match:..      
-000003b0: 2020 6970 5f61 6464 7265 7373 203d 2069    ip_address = i
-000003c0: 705f 6d61 7463 682e 6772 6f75 7028 3129  p_match.group(1)
-000003d0: 0d0a 2020 2020 2020 2020 6e65 746d 6173  ..        netmas
-000003e0: 6b20 3d20 6d61 736b 5f6d 6174 6368 2e67  k = mask_match.g
-000003f0: 726f 7570 2831 290d 0a0d 0a20 2020 2020  roup(1)....     
-00000400: 2020 2072 6574 7572 6e20 6970 5f61 6464     return ip_add
-00000410: 7265 7373 2c20 6e65 746d 6173 6b0d 0a0d  ress, netmask...
-00000420: 0a20 2020 2072 6574 7572 6e20 4e6f 6e65  .    return None
-00000430: 2c20 4e6f 6e65 2020 2320 5265 746f 726e  , None  # Retorn
-00000440: 6120 4e6f 6e65 2073 6520 6ec3 a36f 2065  a None se n..o e
-00000450: 6e63 6f6e 7472 6f75 2061 7320 696e 666f  ncontrou as info
-00000460: 726d 61c3 a7c3 b565 730d 0a0d 0a64 6566  rma....es....def
-00000470: 2069 7028 686f 7374 2c69 706d 736b 3d4e   ip(host,ipmsk=N
-00000480: 6f6e 652c 7365 3d4e 6f6e 6529 3a0d 0a20  one,se=None):.. 
-00000490: 2020 2068 6f73 7431 203d 204e 6f6e 650d     host1 = None.
-000004a0: 0a20 2020 206d 6173 6b31 203d 204e 6f6e  .    mask1 = Non
-000004b0: 650d 0a20 2020 2068 6f73 7432 203d 204e  e..    host2 = N
-000004c0: 6f6e 650d 0a20 2020 206d 6173 6b32 203d  one..    mask2 =
-000004d0: 204e 6f6e 650d 0a20 2020 2069 6620 6970   None..    if ip
-000004e0: 6d73 6b3a 0d0a 2020 2020 2020 2020 6966  msk:..        if
-000004f0: 2074 7970 6528 6970 6d73 6b29 203d 3d20   type(ipmsk) == 
-00000500: 7475 706c 653a 0d0a 2020 2020 2020 2020  tuple:..        
-00000510: 2020 2020 686f 7374 312c 206d 6173 6b31      host1, mask1
-00000520: 2c20 686f 7374 322c 206d 6173 6b32 203d  , host2, mask2 =
-00000530: 2069 706d 736b 0d0a 2020 2020 656c 7365   ipmsk..    else
-00000540: 3a0d 0a20 2020 2020 2020 2068 6f73 7431  :..        host1
-00000550: 2c20 6d61 736b 3120 3d20 6765 745f 6970  , mask1 = get_ip
-00000560: 5f61 6e64 5f6e 6574 6d61 736b 5f69 6e5f  _and_netmask_in_
-00000570: 7769 6e64 6f73 2829 0d0a 2020 2020 2020  windos()..      
-00000580: 2020 686f 7374 3220 3d20 686f 7374 310d    host2 = host1.
-00000590: 0a20 2020 2020 2020 206d 6173 6b32 203d  .        mask2 =
-000005a0: 206d 6173 6b31 0d0a 2020 2020 2020 2020   mask1..        
-000005b0: 6966 2073 653a 0d0a 2020 2020 2020 2020  if se:..        
-000005c0: 2020 2020 7072 696e 7428 6627 486f 7374      print(f'Host
-000005d0: 2070 6172 6120 7365 7220 6164 6963 696f   para ser adicio
-000005e0: 6e61 646f 206e 6f20 6573 7033 323a 207b  nado no esp32: {
-000005f0: 686f 7374 317d 2729 0d0a 2020 2020 2020  host1}')..      
-00000600: 2020 2020 2020 7265 7475 726e 2028 686f        return (ho
-00000610: 7374 312c 6d61 736b 312c 686f 7374 312c  st1,mask1,host1,
-00000620: 6d61 736b 3129 0d0a 2020 2020 6d61 7363  mask1)..    masc
-00000630: 6172 6120 3d20 6d61 736b 312e 7370 6c69  ara = mask1.spli
-00000640: 7428 272e 2729 0d0a 2020 2020 686f 7374  t('.')..    host
-00000650: 7061 6472 616f 203d 2068 6f73 7431 2e73  padrao = host1.s
-00000660: 706c 6974 2827 2e27 290d 0a20 2020 2069  plit('.')..    i
-00000670: 7066 696e 616c 203d 2027 270d 0a20 2020  pfinal = ''..   
-00000680: 2078 203d 2030 0d0a 2020 2020 6573 7061   x = 0..    espa
-00000690: 736f 7320 3d20 300d 0a20 2020 2066 6f72  sos = 0..    for
-000006a0: 2069 2069 6e20 6d61 7363 6172 613a 0d0a   i in mascara:..
-000006b0: 2020 2020 2020 2020 6920 3d20 696e 7428          i = int(
-000006c0: 6929 0d0a 2020 2020 2020 2020 6966 2069  i)..        if i
-000006d0: 203d 3d20 3235 353a 0d0a 2020 2020 2020   == 255:..      
-000006e0: 2020 2020 2020 6970 6669 6e61 6c2b 3d66        ipfinal+=f
-000006f0: 277b 7374 7228 686f 7374 7061 6472 616f  '{str(hostpadrao
-00000700: 5b78 5d29 7d2e 270d 0a20 2020 2020 2020  [x])}.'..       
-00000710: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00000720: 2020 2020 6573 7061 736f 732b 3d31 0d0a      espasos+=1..
-00000730: 2020 2020 2020 2020 782b 3d31 0d0a 2020          x+=1..  
-00000740: 2020 686f 7374 203d 2068 6f73 742e 7370    host = host.sp
-00000750: 6c69 7428 272e 2729 0d0a 2020 2020 666f  lit('.')..    fo
-00000760: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-00000770: 2868 6f73 7429 2d31 293a 0d0a 2020 2020  (host)-1):..    
-00000780: 2020 2020 6966 206e 6f74 2065 7370 6173      if not espas
-00000790: 6f73 203d 3d20 6c65 6e28 686f 7374 293a  os == len(host):
-000007a0: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
-000007b0: 6c20 686f 7374 5b30 5d0d 0a20 2020 2078  l host[0]..    x
-000007c0: 3d31 0d0a 2020 2020 666f 7220 6920 696e  =1..    for i in
-000007d0: 2068 6f73 743a 0d0a 2020 2020 2020 2020   host:..        
-000007e0: 6966 2078 203d 3d20 6c65 6e28 686f 7374  if x == len(host
-000007f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00000800: 6970 6669 6e61 6c2b 3d69 0d0a 2020 2020  ipfinal+=i..    
-00000810: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00000820: 2020 2020 2020 2069 7066 696e 616c 2b3d         ipfinal+=
-00000830: 692b 272e 270d 0a20 2020 2020 2020 2078  i+'.'..        x
-00000840: 2b3d 310d 0a20 2020 2072 6574 7572 6e20  +=1..    return 
-00000850: 2869 7066 696e 616c 2c6d 6173 6b31 2c69  (ipfinal,mask1,i
-00000860: 7066 696e 616c 2c6d 6173 6b31 29         pfinal,mask1)
+000001c0: 7373 0d0a 2020 2020 7265 7375 6c74 6164  ss..    resultad
+000001d0: 6f20 3d20 7375 6270 726f 6365 7373 2e72  o = subprocess.r
+000001e0: 756e 285b 2769 7063 6f6e 6669 6727 5d2c  un(['ipconfig'],
+000001f0: 2063 6170 7475 7265 5f6f 7574 7075 743d   capture_output=
+00000200: 5472 7565 2c20 7465 7874 3d54 7275 6529  True, text=True)
+00000210: 0d0a 2020 2020 6f75 7470 7574 203d 2072  ..    output = r
+00000220: 6573 756c 7461 646f 2e73 7464 6f75 740d  esultado.stdout.
+00000230: 0a0d 0a20 2020 2023 2041 6e61 6c69 7361  ...    # Analisa
+00000240: 2061 2073 61c3 ad64 6120 7061 7261 2065   a sa..da para e
+00000250: 6e63 6f6e 7472 6172 206f 2065 6e64 6572  ncontrar o ender
+00000260: 65c3 a76f 2049 500d 0a20 2020 206c 696e  e..o IP..    lin
+00000270: 6861 7320 3d20 6f75 7470 7574 2e73 706c  has = output.spl
+00000280: 6974 2827 5c6e 2729 0d0a 2020 2020 7265  it('\n')..    re
+00000290: 6970 203d 205b 5d0d 0a20 2020 2072 656d  ip = []..    rem
+000002a0: 6120 3d20 5b5d 0d0a 2020 2020 666f 7220  a = []..    for 
+000002b0: 6c69 6e68 6120 696e 206c 696e 6861 733a  linha in linhas:
+000002c0: 0d0a 2020 2020 2020 2020 6966 2027 4950  ..        if 'IP
+000002d0: 7634 2720 696e 206c 696e 6861 3a0d 0a20  v4' in linha:.. 
+000002e0: 2020 2020 2020 2020 2020 2069 7020 3d20             ip = 
+000002f0: 6c69 6e68 612e 7370 6c69 7428 273a 2729  linha.split(':')
+00000300: 5b31 5d2e 7374 7269 7028 290d 0a20 2020  [1].strip()..   
+00000310: 2020 2020 2020 2020 2072 6569 702e 6170           reip.ap
+00000320: 7065 6e64 2869 7029 0d0a 2020 2020 2020  pend(ip)..      
+00000330: 2020 656c 6966 2027 5375 622d 7265 6465    elif 'Sub-rede
+00000340: 2720 696e 206c 696e 6861 3a0d 0a20 2020  ' in linha:..   
+00000350: 2020 2020 2020 2020 206d 6120 3d20 6c69           ma = li
+00000360: 6e68 612e 7370 6c69 7428 273a 2729 5b31  nha.split(':')[1
+00000370: 5d2e 7374 7269 7028 290d 0a20 2020 2020  ].strip()..     
+00000380: 2020 2020 2020 2072 656d 612e 6170 7065         rema.appe
+00000390: 6e64 286d 6129 0d0a 2020 2020 7265 7475  nd(ma)..    retu
+000003a0: 726e 2072 6569 705b 6c65 6e28 7265 6970  rn reip[len(reip
+000003b0: 2920 2d20 315d 2c20 7265 6d61 5b6c 656e  ) - 1], rema[len
+000003c0: 2872 656d 6129 2d31 5d0d 0a0d 0a64 6566  (rema)-1]....def
+000003d0: 2069 7028 686f 7374 2c69 706d 736b 3d4e   ip(host,ipmsk=N
+000003e0: 6f6e 652c 7365 3d4e 6f6e 6529 3a0d 0a20  one,se=None):.. 
+000003f0: 2020 2068 6f73 7431 203d 204e 6f6e 650d     host1 = None.
+00000400: 0a20 2020 206d 6173 6b31 203d 204e 6f6e  .    mask1 = Non
+00000410: 650d 0a20 2020 2068 6f73 7432 203d 204e  e..    host2 = N
+00000420: 6f6e 650d 0a20 2020 206d 6173 6b32 203d  one..    mask2 =
+00000430: 204e 6f6e 650d 0a20 2020 2069 6620 6970   None..    if ip
+00000440: 6d73 6b3a 0d0a 2020 2020 2020 2020 6966  msk:..        if
+00000450: 2074 7970 6528 6970 6d73 6b29 203d 3d20   type(ipmsk) == 
+00000460: 7475 706c 653a 0d0a 2020 2020 2020 2020  tuple:..        
+00000470: 2020 2020 686f 7374 312c 206d 6173 6b31      host1, mask1
+00000480: 2c20 686f 7374 322c 206d 6173 6b32 203d  , host2, mask2 =
+00000490: 2069 706d 736b 0d0a 2020 2020 656c 7365   ipmsk..    else
+000004a0: 3a0d 0a20 2020 2020 2020 2068 6f73 7431  :..        host1
+000004b0: 2c20 6d61 736b 3120 3d20 6765 745f 6970  , mask1 = get_ip
+000004c0: 5f61 6e64 5f6e 6574 6d61 736b 5f69 6e5f  _and_netmask_in_
+000004d0: 7769 6e64 6f73 2829 0d0a 2020 2020 2020  windos()..      
+000004e0: 2020 686f 7374 3220 3d20 686f 7374 310d    host2 = host1.
+000004f0: 0a20 2020 2020 2020 206d 6173 6b32 203d  .        mask2 =
+00000500: 206d 6173 6b31 0d0a 2020 2020 2020 2020   mask1..        
+00000510: 6966 2073 653a 0d0a 2020 2020 2020 2020  if se:..        
+00000520: 2020 2020 7072 696e 7428 6627 486f 7374      print(f'Host
+00000530: 2070 6172 6120 7365 7220 6164 6963 696f   para ser adicio
+00000540: 6e61 646f 206e 6f20 6573 7033 323a 207b  nado no esp32: {
+00000550: 686f 7374 317d 2729 0d0a 2020 2020 2020  host1}')..      
+00000560: 2020 2020 2020 7265 7475 726e 2028 686f        return (ho
+00000570: 7374 312c 6d61 736b 312c 686f 7374 312c  st1,mask1,host1,
+00000580: 6d61 736b 3129 0d0a 2020 2020 6d61 7363  mask1)..    masc
+00000590: 6172 6120 3d20 6d61 736b 312e 7370 6c69  ara = mask1.spli
+000005a0: 7428 272e 2729 0d0a 2020 2020 686f 7374  t('.')..    host
+000005b0: 7061 6472 616f 203d 2068 6f73 7431 2e73  padrao = host1.s
+000005c0: 706c 6974 2827 2e27 290d 0a20 2020 2069  plit('.')..    i
+000005d0: 7066 696e 616c 203d 2027 270d 0a20 2020  pfinal = ''..   
+000005e0: 2078 203d 2030 0d0a 2020 2020 6573 7061   x = 0..    espa
+000005f0: 736f 7320 3d20 300d 0a20 2020 2066 6f72  sos = 0..    for
+00000600: 2069 2069 6e20 6d61 7363 6172 613a 0d0a   i in mascara:..
+00000610: 2020 2020 2020 2020 6920 3d20 696e 7428          i = int(
+00000620: 6929 0d0a 2020 2020 2020 2020 6966 2069  i)..        if i
+00000630: 203d 3d20 3235 353a 0d0a 2020 2020 2020   == 255:..      
+00000640: 2020 2020 2020 6970 6669 6e61 6c2b 3d66        ipfinal+=f
+00000650: 277b 7374 7228 686f 7374 7061 6472 616f  '{str(hostpadrao
+00000660: 5b78 5d29 7d2e 270d 0a20 2020 2020 2020  [x])}.'..       
+00000670: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00000680: 2020 2020 6573 7061 736f 732b 3d31 0d0a      espasos+=1..
+00000690: 2020 2020 2020 2020 782b 3d31 0d0a 2020          x+=1..  
+000006a0: 2020 686f 7374 203d 2068 6f73 742e 7370    host = host.sp
+000006b0: 6c69 7428 272e 2729 0d0a 2020 2020 666f  lit('.')..    fo
+000006c0: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+000006d0: 2868 6f73 7429 2d31 293a 0d0a 2020 2020  (host)-1):..    
+000006e0: 2020 2020 6966 206e 6f74 2065 7370 6173      if not espas
+000006f0: 6f73 203d 3d20 6c65 6e28 686f 7374 293a  os == len(host):
+00000700: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+00000710: 6c20 686f 7374 5b30 5d0d 0a20 2020 2078  l host[0]..    x
+00000720: 3d31 0d0a 2020 2020 666f 7220 6920 696e  =1..    for i in
+00000730: 2068 6f73 743a 0d0a 2020 2020 2020 2020   host:..        
+00000740: 6966 2078 203d 3d20 6c65 6e28 686f 7374  if x == len(host
+00000750: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00000760: 6970 6669 6e61 6c2b 3d69 0d0a 2020 2020  ipfinal+=i..    
+00000770: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000780: 2020 2020 2020 2069 7066 696e 616c 2b3d         ipfinal+=
+00000790: 692b 272e 270d 0a20 2020 2020 2020 2078  i+'.'..        x
+000007a0: 2b3d 310d 0a20 2020 2072 6574 7572 6e20  +=1..    return 
+000007b0: 2869 7066 696e 616c 2c6d 6173 6b31 2c69  (ipfinal,mask1,i
+000007c0: 7066 696e 616c 2c6d 6173 6b31 29         pfinal,mask1)
```

### Comparing `micropython_wifi_communication-0.0.8/micropython_wifi_communication.egg-info/PKG-INFO` & `micropython_wifi_communication-0.0.9/micropython_wifi_communication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-wifi-communication
-Version: 0.0.8
+Version: 0.0.9
 Summary: um substituto para em vez de uma comunicação RF utilizar wifi
 Home-page: UNKNOWN
 Author: issei momonge
 Author-email: mggyggf@gmail.com
 License: MIT License
 Keywords: socket communication via wifi
 Platform: UNKNOWN
```

