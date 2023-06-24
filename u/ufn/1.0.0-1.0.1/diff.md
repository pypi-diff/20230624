# Comparing `tmp/ufn-1.0.0.tar.gz` & `tmp/ufn-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufn-1.0.0.tar", last modified: Sat Jun 24 13:33:44 2023, max compression
+gzip compressed data, was "ufn-1.0.1.tar", last modified: Sat Jun 24 13:43:45 2023, max compression
```

## Comparing `ufn-1.0.0.tar` & `ufn-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sophgo     (501) staff       (20)        0 2023-06-24 13:33:44.940107 ufn-1.0.0/
--rw-r--r--   0 sophgo     (501) staff       (20)     1059 2023-06-22 09:55:54.000000 ufn-1.0.0/LICENSE
--rw-r--r--   0 sophgo     (501) staff       (20)      660 2023-06-24 13:33:44.939969 ufn-1.0.0/PKG-INFO
--rw-r--r--   0 sophgo     (501) staff       (20)       21 2023-06-22 09:55:54.000000 ufn-1.0.0/README.md
--rw-r--r--   0 sophgo     (501) staff       (20)       38 2023-06-24 13:33:44.940150 ufn-1.0.0/setup.cfg
--rw-r--r--   0 sophgo     (501) staff       (20)      846 2023-06-24 13:33:21.000000 ufn-1.0.0/setup.py
-drwxr-xr-x   0 sophgo     (501) staff       (20)        0 2023-06-24 13:33:44.939253 ufn-1.0.0/ufn/
--rw-r--r--   0 sophgo     (501) staff       (20)        0 2023-06-23 15:46:36.000000 ufn-1.0.0/ufn/__init__.py
--rw-r--r--   0 sophgo     (501) staff       (20)     2245 2023-06-24 13:22:52.000000 ufn-1.0.0/ufn/__main__.py
--rw-r--r--   0 sophgo     (501) staff       (20)     4161 2023-06-24 13:30:00.000000 ufn-1.0.0/ufn/utils.py
-drwxr-xr-x   0 sophgo     (501) staff       (20)        0 2023-06-24 13:33:44.939812 ufn-1.0.0/ufn.egg-info/
--rw-r--r--   0 sophgo     (501) staff       (20)      660 2023-06-24 13:33:44.000000 ufn-1.0.0/ufn.egg-info/PKG-INFO
--rw-r--r--   0 sophgo     (501) staff       (20)      205 2023-06-24 13:33:44.000000 ufn-1.0.0/ufn.egg-info/SOURCES.txt
--rw-r--r--   0 sophgo     (501) staff       (20)        1 2023-06-24 13:33:44.000000 ufn-1.0.0/ufn.egg-info/dependency_links.txt
--rw-r--r--   0 sophgo     (501) staff       (20)       32 2023-06-24 13:33:44.000000 ufn-1.0.0/ufn.egg-info/requires.txt
--rw-r--r--   0 sophgo     (501) staff       (20)        4 2023-06-24 13:33:44.000000 ufn-1.0.0/ufn.egg-info/top_level.txt
+drwxr-xr-x   0 sophgo     (501) staff       (20)        0 2023-06-24 13:43:45.073163 ufn-1.0.1/
+-rw-r--r--   0 sophgo     (501) staff       (20)     1059 2023-06-22 09:55:54.000000 ufn-1.0.1/LICENSE
+-rw-r--r--   0 sophgo     (501) staff       (20)      660 2023-06-24 13:43:45.073007 ufn-1.0.1/PKG-INFO
+-rw-r--r--   0 sophgo     (501) staff       (20)       21 2023-06-22 09:55:54.000000 ufn-1.0.1/README.md
+-rw-r--r--   0 sophgo     (501) staff       (20)       38 2023-06-24 13:43:45.073210 ufn-1.0.1/setup.cfg
+-rw-r--r--   0 sophgo     (501) staff       (20)      846 2023-06-24 13:43:20.000000 ufn-1.0.1/setup.py
+drwxr-xr-x   0 sophgo     (501) staff       (20)        0 2023-06-24 13:43:45.072089 ufn-1.0.1/ufn/
+-rw-r--r--   0 sophgo     (501) staff       (20)        0 2023-06-23 15:46:36.000000 ufn-1.0.1/ufn/__init__.py
+-rw-r--r--   0 sophgo     (501) staff       (20)     2548 2023-06-24 13:42:15.000000 ufn-1.0.1/ufn/__main__.py
+-rw-r--r--   0 sophgo     (501) staff       (20)     4161 2023-06-24 13:30:00.000000 ufn-1.0.1/ufn/utils.py
+drwxr-xr-x   0 sophgo     (501) staff       (20)        0 2023-06-24 13:43:45.072816 ufn-1.0.1/ufn.egg-info/
+-rw-r--r--   0 sophgo     (501) staff       (20)      660 2023-06-24 13:43:45.000000 ufn-1.0.1/ufn.egg-info/PKG-INFO
+-rw-r--r--   0 sophgo     (501) staff       (20)      205 2023-06-24 13:43:45.000000 ufn-1.0.1/ufn.egg-info/SOURCES.txt
+-rw-r--r--   0 sophgo     (501) staff       (20)        1 2023-06-24 13:43:45.000000 ufn-1.0.1/ufn.egg-info/dependency_links.txt
+-rw-r--r--   0 sophgo     (501) staff       (20)       32 2023-06-24 13:43:45.000000 ufn-1.0.1/ufn.egg-info/requires.txt
+-rw-r--r--   0 sophgo     (501) staff       (20)        4 2023-06-24 13:43:45.000000 ufn-1.0.1/ufn.egg-info/top_level.txt
```

### Comparing `ufn-1.0.0/LICENSE` & `ufn-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ufn-1.0.0/PKG-INFO` & `ufn-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufn
-Version: 1.0.0
+Version: 1.0.1
 Summary: upload for nas
 Home-page: https://github.com/sduwfc/ufn
 Author: kilmu
 Author-email: mail@wfc.im
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ufn-1.0.0/setup.py` & `ufn-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ufn',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     description='upload for nas',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='kilmu',
     author_email='mail@wfc.im',
     url='https://github.com/sduwfc/ufn',
```

### Comparing `ufn-1.0.0/ufn/__main__.py` & `ufn-1.0.1/ufn/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import os
 import json
 from getpass import getpass
 
-from .utils import upload_file,upload_directory
+from .utils import upload_file,upload_directory,get_sid
 
 UFN_CONFIG_DIR = 'ufn_config'  # The name of the config directory
 UFN_CONFIG_FILE = 'config.json'  # The name of the config file
 
 def main():
     parser = argparse.ArgumentParser(prog='ufn', description='Upload files or directories.')
     group = parser.add_mutually_exclusive_group(required=True)
@@ -27,14 +27,21 @@
             password = config_data.get('password')
     else:
         print(f"No existing ufn config found at {ufn_config_path}.")
         should_create_config = input("Would you like to create one to save your account and password? (y/n) ").lower() == 'y'
         account = input("Please enter your account: ")
         password = getpass("Please enter your password: ")
 
+        # Try to get sid with given account and password
+        sid = get_sid(account, password)
+        if not sid:
+            print("Failed to get sid with given account and password.")
+            print("Please check if your account and password are correct, exiting.")
+            return
+
         if should_create_config:
             # Ensure the directory exists
             os.makedirs(ufn_config_path, exist_ok=True)
             # Save the account and password
             with open(config_file_path, 'w') as config_file:
                 json.dump({'account': account, 'password': password}, config_file)
```

### Comparing `ufn-1.0.0/ufn/utils.py` & `ufn-1.0.1/ufn/utils.py`

 * *Files identical despite different names*

### Comparing `ufn-1.0.0/ufn.egg-info/PKG-INFO` & `ufn-1.0.1/ufn.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufn
-Version: 1.0.0
+Version: 1.0.1
 Summary: upload for nas
 Home-page: https://github.com/sduwfc/ufn
 Author: kilmu
 Author-email: mail@wfc.im
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

