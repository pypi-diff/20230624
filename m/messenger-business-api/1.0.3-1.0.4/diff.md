# Comparing `tmp/messenger-business-api-1.0.3.tar.gz` & `tmp/messenger-business-api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messenger-business-api-1.0.3.tar", last modified: Fri Jun 23 22:33:39 2023, max compression
+gzip compressed data, was "messenger-business-api-1.0.4.tar", last modified: Fri Jun 23 22:37:51 2023, max compression
```

## Comparing `messenger-business-api-1.0.3.tar` & `messenger-business-api-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:33:39.156364 messenger-business-api-1.0.3/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1066 2023-05-22 21:38:39.000000 messenger-business-api-1.0.3/LICENSE
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:33:39.152364 messenger-business-api-1.0.3/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1039 2023-06-23 22:11:44.000000 messenger-business-api-1.0.3/README.rst
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:33:39.152364 messenger-business-api-1.0.3/messenger_business_api/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       82 2023-06-23 22:08:52.000000 messenger-business-api-1.0.3/messenger_business_api/__init__.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1098 2023-06-23 22:31:47.000000 messenger-business-api-1.0.3/messenger_business_api/api.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      342 2023-06-19 22:14:04.000000 messenger-business-api-1.0.3/messenger_business_api/execeptions.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      202 2023-06-19 22:14:04.000000 messenger-business-api-1.0.3/messenger_business_api/types.py
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:33:39.152364 messenger-business-api-1.0.3/messenger_business_api.egg-info/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:33:39.000000 messenger-business-api-1.0.3/messenger_business_api.egg-info/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      406 2023-06-23 22:33:39.000000 messenger-business-api-1.0.3/messenger_business_api.egg-info/SOURCES.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-06-23 22:33:39.000000 messenger-business-api-1.0.3/messenger_business_api.egg-info/dependency_links.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       18 2023-06-23 22:33:39.000000 messenger-business-api-1.0.3/messenger_business_api.egg-info/requires.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       23 2023-06-23 22:33:39.000000 messenger-business-api-1.0.3/messenger_business_api.egg-info/top_level.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      392 2023-06-19 22:14:04.000000 messenger-business-api-1.0.3/pyproject.toml
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-06-23 22:33:39.156364 messenger-business-api-1.0.3/setup.cfg
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      684 2023-06-23 22:33:16.000000 messenger-business-api-1.0.3/setup.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:37:51.529623 messenger-business-api-1.0.4/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1066 2023-05-22 21:38:39.000000 messenger-business-api-1.0.4/LICENSE
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:37:51.529623 messenger-business-api-1.0.4/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1039 2023-06-23 22:11:44.000000 messenger-business-api-1.0.4/README.rst
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:37:51.529623 messenger-business-api-1.0.4/messenger_business_api/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       82 2023-06-23 22:08:52.000000 messenger-business-api-1.0.4/messenger_business_api/__init__.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1098 2023-06-23 22:37:40.000000 messenger-business-api-1.0.4/messenger_business_api/api.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      342 2023-06-19 22:14:04.000000 messenger-business-api-1.0.4/messenger_business_api/execeptions.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      193 2023-06-23 22:37:23.000000 messenger-business-api-1.0.4/messenger_business_api/types.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:37:51.529623 messenger-business-api-1.0.4/messenger_business_api.egg-info/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:37:51.000000 messenger-business-api-1.0.4/messenger_business_api.egg-info/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      406 2023-06-23 22:37:51.000000 messenger-business-api-1.0.4/messenger_business_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-06-23 22:37:51.000000 messenger-business-api-1.0.4/messenger_business_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       18 2023-06-23 22:37:51.000000 messenger-business-api-1.0.4/messenger_business_api.egg-info/requires.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       23 2023-06-23 22:37:51.000000 messenger-business-api-1.0.4/messenger_business_api.egg-info/top_level.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      392 2023-06-19 22:14:04.000000 messenger-business-api-1.0.4/pyproject.toml
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-06-23 22:37:51.529623 messenger-business-api-1.0.4/setup.cfg
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      684 2023-06-23 22:37:46.000000 messenger-business-api-1.0.4/setup.py
```

### Comparing `messenger-business-api-1.0.3/LICENSE` & `messenger-business-api-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `messenger-business-api-1.0.3/PKG-INFO` & `messenger-business-api-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messenger-business-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: This repository is a wrapper for Meta messenger api for Messenger and Instagram
 Author: Yuri Ramos Lima
 Author-email: yurilima93@hotmail.com
 License: MIT License
 Keywords: python,Meta,Facebook,Instagram,message,chat-bot
 License-File: LICENSE
```

### Comparing `messenger-business-api-1.0.3/README.rst` & `messenger-business-api-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `messenger-business-api-1.0.3/messenger_business_api/api.py` & `messenger-business-api-1.0.4/messenger_business_api/api.py`

 * *Files identical despite different names*

### Comparing `messenger-business-api-1.0.3/messenger_business_api.egg-info/PKG-INFO` & `messenger-business-api-1.0.4/messenger_business_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messenger-business-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: This repository is a wrapper for Meta messenger api for Messenger and Instagram
 Author: Yuri Ramos Lima
 Author-email: yurilima93@hotmail.com
 License: MIT License
 Keywords: python,Meta,Facebook,Instagram,message,chat-bot
 License-File: LICENSE
```

### Comparing `messenger-business-api-1.0.3/setup.py` & `messenger-business-api-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.rst') as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="messenger-business-api",
-    version="1.0.3",
+    version="1.0.4",
     author="Yuri Ramos Lima",
     author_email="yurilima93@hotmail.com",
     description="This repository is a wrapper for Meta messenger api for Messenger and Instagram",
     packages=find_packages(),
     include_package_data=True,
     long_description=README,
     install_requires=[ "pydantic", "requests"],
```

