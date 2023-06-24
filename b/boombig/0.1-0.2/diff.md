# Comparing `tmp/boombig-0.1.tar.gz` & `tmp/boombig-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boombig-0.1.tar", last modified: Sat Jun 24 08:35:39 2023, max compression
+gzip compressed data, was "boombig-0.2.tar", last modified: Sat Jun 24 12:51:03 2023, max compression
```

## Comparing `boombig-0.1.tar` & `boombig-0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 08:35:39.447625 boombig-0.1/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 boombig-0.1/LICENSE
--rw-r--r--   0 themamad  (1000) themamad  (1000)      971 2023-06-24 08:35:39.447625 boombig-0.1/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      246 2023-06-24 08:25:45.000000 boombig-0.1/README.md
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 08:35:39.447625 boombig-0.1/boombig/
--rwxr-----   0 themamad  (1000) themamad  (1000)     3037 2023-06-24 08:34:44.000000 boombig-0.1/boombig/__init__.py
--rwxr-----   0 themamad  (1000) themamad  (1000)      513 2023-06-23 12:28:00.000000 boombig-0.1/boombig/config.py
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 08:35:39.447625 boombig-0.1/boombig.egg-info/
--rw-r--r--   0 themamad  (1000) themamad  (1000)      971 2023-06-24 08:35:39.000000 boombig-0.1/boombig.egg-info/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      188 2023-06-24 08:35:39.000000 boombig-0.1/boombig.egg-info/SOURCES.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-24 08:35:39.000000 boombig-0.1/boombig.egg-info/dependency_links.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        8 2023-06-24 08:35:39.000000 boombig-0.1/boombig.egg-info/top_level.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-24 08:35:39.447625 boombig-0.1/setup.cfg
--rw-r--r--   0 themamad  (1000) themamad  (1000)      960 2023-06-24 08:26:05.000000 boombig-0.1/setup.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 12:51:03.638144 boombig-0.2/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 boombig-0.2/LICENSE
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1103 2023-06-24 12:51:03.638144 boombig-0.2/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      372 2023-06-24 12:47:12.000000 boombig-0.2/README.md
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 12:51:03.638144 boombig-0.2/boombig/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)       34 2023-06-24 12:39:02.000000 boombig-0.2/boombig/__init__.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 12:51:03.638144 boombig-0.2/boombig/config/
+-rwxr-----   0 themamad  (1000) themamad  (1000)      513 2023-06-23 12:28:00.000000 boombig-0.2/boombig/config/__init__.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 12:51:03.638144 boombig-0.2/boombig/main/
+-rwxr-----   0 themamad  (1000) themamad  (1000)     3035 2023-06-24 12:31:34.000000 boombig-0.2/boombig/main/__init__.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-24 12:51:03.638144 boombig-0.2/boombig.egg-info/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1103 2023-06-24 12:51:03.000000 boombig-0.2/boombig.egg-info/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      222 2023-06-24 12:51:03.000000 boombig-0.2/boombig.egg-info/SOURCES.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-24 12:51:03.000000 boombig-0.2/boombig.egg-info/dependency_links.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        8 2023-06-24 12:51:03.000000 boombig-0.2/boombig.egg-info/top_level.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-24 12:51:03.638144 boombig-0.2/setup.cfg
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      969 2023-06-24 12:39:57.000000 boombig-0.2/setup.py
```

### Comparing `boombig-0.1/LICENSE` & `boombig-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `boombig-0.1/PKG-INFO` & `boombig-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: boombig
-Version: 0.1
+Version: 0.2
 Summary: boombing a Library Python
 Home-page: https://github.com/OnlyRad/Boombers
 Author: Mohammad and Amir
 Author-email: mohammadmehrabi175@gmail.com
-Keywords: bot,sms,boombers,boomber
+Keywords: bot,sms,boombers,boomber,boomb
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -26,13 +26,20 @@
 
 ```python
 pip install -U boombing
 ```
 
 => START
 
-> doc: github.com/onlyrad/boombers
+> doc: github.com/onlyrad
+
+<hr>
 
 # Social Media:
-Telegram: @OnlyRad <br>
-github: github.com/OnlyRad <br>
-rubika: rubika.ir/OnlyMamad
+## Mohammad Mehrabi Rad
+### Telegram: @OnlyRad <br>
+### github: github.com/OnlyRad <br>
+### rubika: rubika.ir/OnlyMamad <br>
+
+## Amir kamankesh <br>
+### Telegram: @paytowin_prg <br>
+### rubika: rubika.ir/paytowin
```

### Comparing `boombig-0.1/boombig/__init__.py` & `boombig-0.2/boombig/main/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import requests as re
 from time import sleep
 from random import choice , random , randint
 from config import __copyright__ , __version__ , __license__ , welcome
 from colorama import Fore as f
 
-
 welcome(f"boombig library virsion {__version__}{__copyright__}")
 
-
 class sms:
     
     def __init__(self , phonenumber:str , TimeForOnSMS:float , SMS:int):
         self.phonenumber = phonenumber
         self.timeforonsms = TimeForOnSMS
         self.sms = SMS
         self.tim = self.timeforonsms * self.sms
```

### Comparing `boombig-0.1/boombig/config.py` & `boombig-0.2/boombig/config/__init__.py`

 * *Files identical despite different names*

### Comparing `boombig-0.1/boombig.egg-info/PKG-INFO` & `boombig-0.2/boombig.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: boombig
-Version: 0.1
+Version: 0.2
 Summary: boombing a Library Python
 Home-page: https://github.com/OnlyRad/Boombers
 Author: Mohammad and Amir
 Author-email: mohammadmehrabi175@gmail.com
-Keywords: bot,sms,boombers,boomber
+Keywords: bot,sms,boombers,boomber,boomb
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -26,13 +26,20 @@
 
 ```python
 pip install -U boombing
 ```
 
 => START
 
-> doc: github.com/onlyrad/boombers
+> doc: github.com/onlyrad
+
+<hr>
 
 # Social Media:
-Telegram: @OnlyRad <br>
-github: github.com/OnlyRad <br>
-rubika: rubika.ir/OnlyMamad
+## Mohammad Mehrabi Rad
+### Telegram: @OnlyRad <br>
+### github: github.com/OnlyRad <br>
+### rubika: rubika.ir/OnlyMamad <br>
+
+## Amir kamankesh <br>
+### Telegram: @paytowin_prg <br>
+### rubika: rubika.ir/paytowin
```

### Comparing `boombig-0.1/setup.py` & `boombig-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'boombig',
-    version = '0.1',
+    version = '0.2',
     author='Mohammad and Amir',
     author_email = 'mohammadmehrabi175@gmail.com',
     description = 'boombing a Library Python',
-    keywords = ['bot' , 'sms' , 'boombers' , 'boomber'],
+    keywords = ['bot' , 'sms' , 'boombers' , 'boomber', 'boomb'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/OnlyRad/Boombers',
     packages = find_packages(),
     install_requires = [],
     classifiers = [
```

