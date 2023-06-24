# Comparing `tmp/wififtp-0.1.0.tar.gz` & `tmp/wififtp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wififtp-0.1.0.tar", max compression
+gzip compressed data, was "wififtp-0.1.1.tar", max compression
```

## Comparing `wififtp-0.1.0.tar` & `wififtp-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2023-06-23 11:09:47.850427 wififtp-0.1.0/LICENSE
--rw-r--r--   0        0        0     2560 2023-06-23 11:09:47.850427 wififtp-0.1.0/README.md
--rw-r--r--   0        0        0      629 2023-06-23 11:09:47.850427 wififtp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8767 2023-06-23 11:09:47.854427 wififtp-0.1.0/wififtp.py
--rw-r--r--   0        0        0     3236 1970-01-01 00:00:00.000000 wififtp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-24 01:45:46.330988 wififtp-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2506 2023-06-24 01:45:46.330988 wififtp-0.1.1/README.md
+-rw-r--r--   0        0        0      628 2023-06-24 01:45:46.330988 wififtp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8827 2023-06-24 01:45:46.330988 wififtp-0.1.1/wififtp.py
+-rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 wififtp-0.1.1/PKG-INFO
```

### Comparing `wififtp-0.1.0/LICENSE` & `wififtp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wififtp-0.1.0/README.md` & `wififtp-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # WiFi-FTP
 
 ### [+] Description :
 ***WiFi-FTP is a tool to create a simple ftp server in local network. Anyone under same wifi/router can read/write/modify the folder you shared.***
-<h2 align="center">Share files under same Wi-Fi!</h2>
+
 
 ### [-] Installation
 
 ```apt install python3 python3-pip -y```
 
 ```pip3 install pyftpdlib --break-system-packages```
 
@@ -43,15 +43,15 @@
 
 ```
 ## [+] Caution:
 
 ### You must need "Python" installed in your operating system. If you use firewall you also have to enable python from "Windows Firewall". If you can't enable python from firewall, you may need to disable firewall while using ftp!
 ### Your sharing link will be like "ftp://192.168.0.105:2121". Make sure you are connected to same router/Wi-Fi to access folder from other device!
 ## [+] Screenshot:
-<img src="https://github.com/KasRoudra/wififtp/blob/main/ss.jpg">
+![preview](https://github.com/KasRoudra/wififtp/raw/main/ss.jpg)
 
 ## [~] Find Me on :
 
 - [![Github](https://img.shields.io/badge/Github-KasRoudra-green?style=for-the-badge&logo=github)](https://github.com/KasRoudra)
 
 - [![Gmail](https://img.shields.io/badge/Gmail-KasRoudra-green?style=for-the-badge&logo=gmail)](mailto:kasroudrakrd@gmail.com)
```

### Comparing `wififtp-0.1.0/pyproject.toml` & `wififtp-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
     "setuptools>=58.0.4",
     "wheel>=0.37.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "WiFiFTP"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 license = "MIT"
-repository = "https://github.com/KasRoudra/WiFi-FTP/"
+repository = "https://github.com/KasRoudra/WiFiFTP/"
 include = ["README.md", "LICENSE"]
 description = "Share files between devices connected to same wlan/wifi/hotspot/router"
 authors = ["KasRoudra <kasroudrakrd@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyftpdlib = "^1.5.0"
```

### Comparing `wififtp-0.1.0/wififtp.py` & `wififtp-0.1.1/wififtp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: UTF-8 -*-
 # ToolName   : WiFiFTP
 # Author     : KasRoudra
 # License    : MIT
-# Copyright  : KasRoudra (2021-2022)
+# Copyright  : KasRoudra (2021-2023)
 # Github     : https://github.com/KasRoudra
 # Contact    : https://t.me/KasRoudra
 # Description: Share files between devices connected to same wlan/wifi/hotspot/router""
 # Tags       : ftp, wififtp, share-files
 # 1st Commit : 18/08/2021
 # Language   : Python
 # Portable file/script
@@ -82,15 +82,18 @@
 purple = "\033[0;35m"
 bpurple = "\033[1;35m"
 cyan = "\033[0;36m"
 bcyan = "\033[1;36m"
 white = "\033[0;37m"
 nc = "\033[00m"
 
-version = "1.0"
+version = "0.1.1"
+
+# Major Minor version ignoring patch
+mm_ver = version[:3]
 
 # Regular Snippets
 ask = f"{green}[{white}?{green}] {yellow}"
 success = f"{yellow}[{white}√{yellow}] {green}"
 error = f"{blue}[{white}!{blue}] {red}"
 info = f"{yellow}[{white}+{yellow}] {cyan}"
 info2 = f"{green}[{white}•{green}] {purple}"
@@ -100,15 +103,15 @@
 
 banner = f"""
 {red}__        ___ _____ _  _____ _____ ____  
 {blue}\ \      / (_)  ___(_)|  ___|_   _|  _ \  
 {green} \ \ /\ / /| | |_  | || |_    | | | |_) |
 {cyan}  \ V  V / | |  _| | ||  _|   | | |  __/ 
 {purple}   \_/\_/  |_|_|   |_||_|     |_| |_| 
-{blue}{" "*31}[{green}v{cyan}{version}{blue}]   
+{blue}{" "*31}[{green}v{cyan}{mm_ver}{blue}]   
 {cyan}{" "*23}[{blue}By {green}KasRoudra{cyan}]{nc}
 """
 
 argparser = ArgumentParser()
 
 argparser.add_argument("-p", "--port", type=int, help=f"WiFiFTP's server port [Default: {default_port}]")
 argparser.add_argument("-d", "--directory", help=f"Directory where server will start [Default: {default_dir}]")
```

### Comparing `wififtp-0.1.0/PKG-INFO` & `wififtp-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: wififtp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Share files between devices connected to same wlan/wifi/hotspot/router
-Home-page: https://github.com/KasRoudra/WiFi-FTP/
+Home-page: https://github.com/KasRoudra/WiFiFTP/
 License: MIT
 Author: KasRoudra
 Author-email: kasroudrakrd@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyftpdlib (>=1.5.0,<2.0.0)
-Project-URL: Repository, https://github.com/KasRoudra/WiFi-FTP/
+Project-URL: Repository, https://github.com/KasRoudra/WiFiFTP/
 Description-Content-Type: text/markdown
 
 # WiFi-FTP
 
 ### [+] Description :
 ***WiFi-FTP is a tool to create a simple ftp server in local network. Anyone under same wifi/router can read/write/modify the folder you shared.***
-<h2 align="center">Share files under same Wi-Fi!</h2>
+
 
 ### [-] Installation
 
 ```apt install python3 python3-pip -y```
 
 ```pip3 install pyftpdlib --break-system-packages```
 
@@ -61,15 +61,15 @@
 
 ```
 ## [+] Caution:
 
 ### You must need "Python" installed in your operating system. If you use firewall you also have to enable python from "Windows Firewall". If you can't enable python from firewall, you may need to disable firewall while using ftp!
 ### Your sharing link will be like "ftp://192.168.0.105:2121". Make sure you are connected to same router/Wi-Fi to access folder from other device!
 ## [+] Screenshot:
-<img src="https://github.com/KasRoudra/wififtp/blob/main/ss.jpg">
+![preview](https://github.com/KasRoudra/wififtp/raw/main/ss.jpg)
 
 ## [~] Find Me on :
 
 - [![Github](https://img.shields.io/badge/Github-KasRoudra-green?style=for-the-badge&logo=github)](https://github.com/KasRoudra)
 
 - [![Gmail](https://img.shields.io/badge/Gmail-KasRoudra-green?style=for-the-badge&logo=gmail)](mailto:kasroudrakrd@gmail.com)
```

