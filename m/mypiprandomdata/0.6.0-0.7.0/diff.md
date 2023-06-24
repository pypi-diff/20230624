# Comparing `tmp/mypiprandomdata-0.6.0.tar.gz` & `tmp/mypiprandomdata-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypiprandomdata-0.6.0.tar", last modified: Sat Jun 24 00:18:45 2023, max compression
+gzip compressed data, was "mypiprandomdata-0.7.0.tar", last modified: Sat Jun 24 00:30:22 2023, max compression
```

## Comparing `mypiprandomdata-0.6.0.tar` & `mypiprandomdata-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 00:18:45.223422 mypiprandomdata-0.6.0/
--rw-rw-rw-   0        0        0      250 2023-06-24 00:18:45.221428 mypiprandomdata-0.6.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 00:18:45.063031 mypiprandomdata-0.6.0/mypiprandomdata/
--rw-rw-rw-   0        0        0        0 2023-06-23 22:27:10.000000 mypiprandomdata-0.6.0/mypiprandomdata/__init__.py
--rw-rw-rw-   0        0        0     2448 2023-06-23 23:34:28.000000 mypiprandomdata-0.6.0/mypiprandomdata/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-24 00:18:45.109724 mypiprandomdata-0.6.0/mypiprandomdata/data/
--rw-rw-rw-   0        0        0     3817 2023-06-18 04:52:48.000000 mypiprandomdata-0.6.0/mypiprandomdata/data/Cities.txt
--rw-rw-rw-   0        0        0    10204 2023-06-18 04:53:08.000000 mypiprandomdata-0.6.0/mypiprandomdata/data/FirstName.txt
--rw-rw-rw-   0        0        0    12825 2023-06-18 04:53:22.000000 mypiprandomdata-0.6.0/mypiprandomdata/data/LastName.txt
--rw-rw-rw-   0        0        0        0 2023-06-23 23:17:05.000000 mypiprandomdata-0.6.0/mypiprandomdata/data/Real_Address.txt
--rw-rw-rw-   0        0        0      839 2023-06-23 23:05:29.000000 mypiprandomdata-0.6.0/mypiprandomdata/data/States.txt
--rw-rw-rw-   0        0        0    11708 2023-06-18 04:54:13.000000 mypiprandomdata-0.6.0/mypiprandomdata/data/UserAgent.txt
--rw-rw-rw-   0        0        0     8764 2023-06-18 04:53:50.000000 mypiprandomdata-0.6.0/mypiprandomdata/data/ZipCode.txt
--rw-rw-rw-   0        0        0   488475 2023-06-23 23:25:47.000000 mypiprandomdata-0.6.0/mypiprandomdata/data/data.json
-drwxrwxrwx   0        0        0        0 2023-06-24 00:18:45.071828 mypiprandomdata-0.6.0/mypiprandomdata.egg-info/
--rw-rw-rw-   0        0        0      250 2023-06-24 00:18:44.000000 mypiprandomdata-0.6.0/mypiprandomdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2023-06-24 00:18:45.000000 mypiprandomdata-0.6.0/mypiprandomdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 00:18:44.000000 mypiprandomdata-0.6.0/mypiprandomdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-24 00:18:44.000000 mypiprandomdata-0.6.0/mypiprandomdata.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-06-24 00:18:44.000000 mypiprandomdata-0.6.0/mypiprandomdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 00:18:45.223422 mypiprandomdata-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      568 2023-06-24 00:18:31.000000 mypiprandomdata-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 00:30:22.671161 mypiprandomdata-0.7.0/
+-rw-rw-rw-   0        0        0      250 2023-06-24 00:30:22.670132 mypiprandomdata-0.7.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 00:30:22.515440 mypiprandomdata-0.7.0/mypiprandomdata/
+-rw-rw-rw-   0        0        0        0 2023-06-23 22:27:10.000000 mypiprandomdata-0.7.0/mypiprandomdata/__init__.py
+-rw-rw-rw-   0        0        0     2658 2023-06-24 00:29:11.000000 mypiprandomdata-0.7.0/mypiprandomdata/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-24 00:30:22.562418 mypiprandomdata-0.7.0/mypiprandomdata/data/
+-rw-rw-rw-   0        0        0     3817 2023-06-18 04:52:48.000000 mypiprandomdata-0.7.0/mypiprandomdata/data/Cities.txt
+-rw-rw-rw-   0        0        0    10204 2023-06-18 04:53:08.000000 mypiprandomdata-0.7.0/mypiprandomdata/data/FirstName.txt
+-rw-rw-rw-   0        0        0    12825 2023-06-18 04:53:22.000000 mypiprandomdata-0.7.0/mypiprandomdata/data/LastName.txt
+-rw-rw-rw-   0        0        0        0 2023-06-23 23:17:05.000000 mypiprandomdata-0.7.0/mypiprandomdata/data/Real_Address.txt
+-rw-rw-rw-   0        0        0      839 2023-06-23 23:05:29.000000 mypiprandomdata-0.7.0/mypiprandomdata/data/States.txt
+-rw-rw-rw-   0        0        0    11708 2023-06-18 04:54:13.000000 mypiprandomdata-0.7.0/mypiprandomdata/data/UserAgent.txt
+-rw-rw-rw-   0        0        0     8764 2023-06-18 04:53:50.000000 mypiprandomdata-0.7.0/mypiprandomdata/data/ZipCode.txt
+-rw-rw-rw-   0        0        0   488475 2023-06-23 23:25:47.000000 mypiprandomdata-0.7.0/mypiprandomdata/data/data.json
+drwxrwxrwx   0        0        0        0 2023-06-24 00:30:22.524416 mypiprandomdata-0.7.0/mypiprandomdata.egg-info/
+-rw-rw-rw-   0        0        0      250 2023-06-24 00:30:22.000000 mypiprandomdata-0.7.0/mypiprandomdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2023-06-24 00:30:22.000000 mypiprandomdata-0.7.0/mypiprandomdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 00:30:22.000000 mypiprandomdata-0.7.0/mypiprandomdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-24 00:30:22.000000 mypiprandomdata-0.7.0/mypiprandomdata.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-06-24 00:30:22.000000 mypiprandomdata-0.7.0/mypiprandomdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 00:30:22.671161 mypiprandomdata-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      568 2023-06-24 00:29:11.000000 mypiprandomdata-0.7.0/setup.py
```

### Comparing `mypiprandomdata-0.6.0/mypiprandomdata/cli.py` & `mypiprandomdata-0.7.0/mypiprandomdata/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import random
 import json
 import pkg_resources
 
 class RandomData:
-    def __init__(self, first_name, last_name, address, city, state, zip_code, phone_number, user_agent):
+    def __init__(self, first_name, last_name, address, city, state, zip_code, phone_number, user_agent, email):
         self.first_name = first_name
         self.last_name = last_name
         self.address = address
         self.city = city
         self.state = state
         self.zip_code = zip_code
         self.phone_number = phone_number
         self.user_agent = user_agent
+        self.email = email
 
 def get_random_data():
     data_dir = pkg_resources.resource_filename('mypiprandomdata', 'data')
 
     with open(data_dir + '/data.json', 'r') as file:
         data = json.load(file)
 
@@ -31,31 +32,33 @@
         "zip_code": addresses[random_generator2]['zipcode'],
         "phone_number": addresses[random_generator2]['phone_number']
     }
 
     first_name = get_random_name_from_file(data_dir, 'FirstName.txt', split_by=',')
     last_name = get_random_name_from_file(data_dir, 'LastName.txt', split_by=',')
     user_agent = get_random_name_from_file(data_dir, 'UserAgent.txt', split_by='\n')
+    email = f"{first_name.lower()}{last_name.lower()}{random.randint(999, 9999)}{random.choice(['@gmail.com', '@yahoo.com'])}"
 
     random_data = RandomData(first_name, last_name, random_data['address'], random_data['city'],
-                             random_data['state'], random_data['zip_code'], random_data['phone_number'], user_agent)
+                             random_data['state'], random_data['zip_code'], random_data['phone_number'], user_agent, email)
 
     return random_data
 
 def get_random_name_from_file(directory, filename, split_by=None):
     file_path = directory + '/' + filename
     with open(file_path, 'r') as file:
         names = file.read().strip().split(split_by) if split_by else file.readlines()
     return random.choice(names).strip().strip('",')
 
 def main():
     random_data = get_random_data()
     print("Randomly Generated Data:")
     print("First Name:", random_data.first_name)
     print("Last Name:", random_data.last_name)
+    print("Email:", random_data.email)
     print("Address:", random_data.address)
     print("City:", random_data.city)
     print("State:", random_data.state)
     print("Zip Code:", random_data.zip_code)
     print("Phone Number:", random_data.phone_number)
     print("User Agent:", random_data.user_agent)
```

### Comparing `mypiprandomdata-0.6.0/mypiprandomdata/data/Cities.txt` & `mypiprandomdata-0.7.0/mypiprandomdata/data/Cities.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.6.0/mypiprandomdata/data/FirstName.txt` & `mypiprandomdata-0.7.0/mypiprandomdata/data/FirstName.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.6.0/mypiprandomdata/data/LastName.txt` & `mypiprandomdata-0.7.0/mypiprandomdata/data/LastName.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.6.0/mypiprandomdata/data/States.txt` & `mypiprandomdata-0.7.0/mypiprandomdata/data/States.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.6.0/mypiprandomdata/data/UserAgent.txt` & `mypiprandomdata-0.7.0/mypiprandomdata/data/UserAgent.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.6.0/mypiprandomdata/data/ZipCode.txt` & `mypiprandomdata-0.7.0/mypiprandomdata/data/ZipCode.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.6.0/mypiprandomdata/data/data.json` & `mypiprandomdata-0.7.0/mypiprandomdata/data/data.json`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.6.0/mypiprandomdata.egg-info/SOURCES.txt` & `mypiprandomdata-0.7.0/mypiprandomdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypiprandomdata-0.6.0/setup.py` & `mypiprandomdata-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='mypiprandomdata',
-    version='0.6.0',
+    version='0.7.0',
     packages=['mypiprandomdata'],
     package_data={'mypiprandomdata': ['data/*.txt', 'data/*.json']},
     entry_points={
         'console_scripts': [
             'mypiprandomdata = mypiprandomdata.cli:main'
         ]
     },
```

