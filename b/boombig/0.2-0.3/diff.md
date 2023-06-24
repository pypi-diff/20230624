# Comparing `tmp/boombig-0.2.tar.gz` & `tmp/boombig-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boombig-0.2.tar", last modified: Sat Jun 24 12:51:03 2023, max compression
+gzip compressed data, was "boombig-0.3.tar", last modified: Sat Jun 24 13:59:58 2023, max compression
```

## Comparing `boombig-0.2.tar` & `boombig-0.3.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 12:51:03.638144 boombig-0.2/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 boombig-0.2/LICENSE
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1103 2023-06-24 12:51:03.638144 boombig-0.2/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      372 2023-06-24 12:47:12.000000 boombig-0.2/README.md
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 12:51:03.638144 boombig-0.2/boombig/
--rw-r--r--   0 themamad  (1000) themamad  (1000)       34 2023-06-24 12:39:02.000000 boombig-0.2/boombig/__init__.py
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 12:51:03.638144 boombig-0.2/boombig/config/
--rwxr-----   0 themamad  (1000) themamad  (1000)      513 2023-06-23 12:28:00.000000 boombig-0.2/boombig/config/__init__.py
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 12:51:03.638144 boombig-0.2/boombig/main/
--rwxr-----   0 themamad  (1000) themamad  (1000)     3035 2023-06-24 12:31:34.000000 boombig-0.2/boombig/main/__init__.py
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 12:51:03.638144 boombig-0.2/boombig.egg-info/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1103 2023-06-24 12:51:03.000000 boombig-0.2/boombig.egg-info/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      222 2023-06-24 12:51:03.000000 boombig-0.2/boombig.egg-info/SOURCES.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-24 12:51:03.000000 boombig-0.2/boombig.egg-info/dependency_links.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        8 2023-06-24 12:51:03.000000 boombig-0.2/boombig.egg-info/top_level.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-24 12:51:03.638144 boombig-0.2/setup.cfg
--rw-r--r--   0 themamad  (1000) themamad  (1000)      969 2023-06-24 12:39:57.000000 boombig-0.2/setup.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 13:59:58.589549 boombig-0.3/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 boombig-0.3/LICENSE
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1108 2023-06-24 13:59:58.589549 boombig-0.3/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      377 2023-06-24 13:59:28.000000 boombig-0.3/README.md
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 13:59:58.576216 boombig-0.3/boombig/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)       71 2023-06-24 13:58:42.000000 boombig-0.3/boombig/__init__.py
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      434 2023-06-24 13:58:09.000000 boombig-0.3/boombig/config.py
+-rwxr-----   0 themamad  (1000) themamad  (1000)     2969 2023-06-24 13:57:45.000000 boombig-0.3/boombig/main.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 13:59:58.589549 boombig-0.3/boombig.egg-info/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1108 2023-06-24 13:59:58.000000 boombig-0.3/boombig.egg-info/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      204 2023-06-24 13:59:58.000000 boombig-0.3/boombig.egg-info/SOURCES.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-24 13:59:58.000000 boombig-0.3/boombig.egg-info/dependency_links.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        8 2023-06-24 13:59:58.000000 boombig-0.3/boombig.egg-info/top_level.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-24 13:59:58.589549 boombig-0.3/setup.cfg
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      969 2023-06-24 13:59:07.000000 boombig-0.3/setup.py
```

### Comparing `boombig-0.2/LICENSE` & `boombig-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `boombig-0.2/PKG-INFO` & `boombig-0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boombig
-Version: 0.2
+Version: 0.3
 Summary: boombing a Library Python
 Home-page: https://github.com/OnlyRad/Boombers
 Author: Mohammad and Amir
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,sms,boombers,boomber,boomb
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -32,14 +32,14 @@
 
 > doc: github.com/onlyrad
 
 <hr>
 
 # Social Media:
 ## Mohammad Mehrabi Rad
-### Telegram: @OnlyRad <br>
-### github: github.com/OnlyRad <br>
-### rubika: rubika.ir/OnlyMamad <br>
+#### Telegram: @OnlyRad <br>
+#### github: github.com/OnlyRad <br>
+#### rubika: rubika.ir/OnlyMamad <br>
 
 ## Amir kamankesh <br>
-### Telegram: @paytowin_prg <br>
-### rubika: rubika.ir/paytowin
+#### Telegram: @paytowin_prg <br>
+#### rubika: rubika.ir/paytowin
```

### Comparing `boombig-0.2/boombig/main/__init__.py` & `boombig-0.3/boombig/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import requests as re
 from time import sleep
 from random import choice , random , randint
 from config import __copyright__ , __version__ , __license__ , welcome
 from colorama import Fore as f
 
-welcome(f"boombig library virsion {__version__}{__copyright__}")
-
 class sms:
     
     def __init__(self , phonenumber:str , TimeForOnSMS:float , SMS:int):
         self.phonenumber = phonenumber
         self.timeforonsms = TimeForOnSMS
         self.sms = SMS
         self.tim = self.timeforonsms * self.sms
```

### Comparing `boombig-0.2/boombig.egg-info/PKG-INFO` & `boombig-0.3/boombig.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boombig
-Version: 0.2
+Version: 0.3
 Summary: boombing a Library Python
 Home-page: https://github.com/OnlyRad/Boombers
 Author: Mohammad and Amir
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,sms,boombers,boomber,boomb
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -32,14 +32,14 @@
 
 > doc: github.com/onlyrad
 
 <hr>
 
 # Social Media:
 ## Mohammad Mehrabi Rad
-### Telegram: @OnlyRad <br>
-### github: github.com/OnlyRad <br>
-### rubika: rubika.ir/OnlyMamad <br>
+#### Telegram: @OnlyRad <br>
+#### github: github.com/OnlyRad <br>
+#### rubika: rubika.ir/OnlyMamad <br>
 
 ## Amir kamankesh <br>
-### Telegram: @paytowin_prg <br>
-### rubika: rubika.ir/paytowin
+#### Telegram: @paytowin_prg <br>
+#### rubika: rubika.ir/paytowin
```

### Comparing `boombig-0.2/setup.py` & `boombig-0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'boombig',
-    version = '0.2',
+    version = '0.3',
     author='Mohammad and Amir',
     author_email = 'mohammadmehrabi175@gmail.com',
     description = 'boombing a Library Python',
     keywords = ['bot' , 'sms' , 'boombers' , 'boomber', 'boomb'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
```

