# Comparing `tmp/messenger-business-api-1.0.1.tar.gz` & `tmp/messenger-business-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messenger-business-api-1.0.1.tar", last modified: Fri Jun 23 22:12:26 2023, max compression
+gzip compressed data, was "messenger-business-api-1.0.2.tar", last modified: Fri Jun 23 22:24:08 2023, max compression
```

## Comparing `messenger-business-api-1.0.1.tar` & `messenger-business-api-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:12:26.964405 messenger-business-api-1.0.1/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1066 2023-05-22 21:38:39.000000 messenger-business-api-1.0.1/LICENSE
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:12:26.964405 messenger-business-api-1.0.1/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1039 2023-06-23 22:11:44.000000 messenger-business-api-1.0.1/README.rst
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:12:26.960405 messenger-business-api-1.0.1/messenger-business-api/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       82 2023-06-23 22:08:52.000000 messenger-business-api-1.0.1/messenger-business-api/__init__.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1093 2023-06-19 22:33:14.000000 messenger-business-api-1.0.1/messenger-business-api/api.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      342 2023-06-19 22:14:04.000000 messenger-business-api-1.0.1/messenger-business-api/execeptions.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      202 2023-06-19 22:14:04.000000 messenger-business-api-1.0.1/messenger-business-api/types.py
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:12:26.964405 messenger-business-api-1.0.1/messenger_business_api.egg-info/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:12:26.000000 messenger-business-api-1.0.1/messenger_business_api.egg-info/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      406 2023-06-23 22:12:26.000000 messenger-business-api-1.0.1/messenger_business_api.egg-info/SOURCES.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-06-23 22:12:26.000000 messenger-business-api-1.0.1/messenger_business_api.egg-info/dependency_links.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       18 2023-06-23 22:12:26.000000 messenger-business-api-1.0.1/messenger_business_api.egg-info/requires.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       23 2023-06-23 22:12:26.000000 messenger-business-api-1.0.1/messenger_business_api.egg-info/top_level.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      392 2023-06-19 22:14:04.000000 messenger-business-api-1.0.1/pyproject.toml
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-06-23 22:12:26.964405 messenger-business-api-1.0.1/setup.cfg
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      684 2023-06-23 22:12:03.000000 messenger-business-api-1.0.1/setup.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:24:08.438342 messenger-business-api-1.0.2/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1066 2023-05-22 21:38:39.000000 messenger-business-api-1.0.2/LICENSE
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:24:08.438342 messenger-business-api-1.0.2/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1039 2023-06-23 22:11:44.000000 messenger-business-api-1.0.2/README.rst
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:24:08.438342 messenger-business-api-1.0.2/messenger_business_api/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       82 2023-06-23 22:08:52.000000 messenger-business-api-1.0.2/messenger_business_api/__init__.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1093 2023-06-19 22:33:14.000000 messenger-business-api-1.0.2/messenger_business_api/api.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      342 2023-06-19 22:14:04.000000 messenger-business-api-1.0.2/messenger_business_api/execeptions.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      202 2023-06-19 22:14:04.000000 messenger-business-api-1.0.2/messenger_business_api/types.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-06-23 22:24:08.438342 messenger-business-api-1.0.2/messenger_business_api.egg-info/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1357 2023-06-23 22:24:08.000000 messenger-business-api-1.0.2/messenger_business_api.egg-info/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      406 2023-06-23 22:24:08.000000 messenger-business-api-1.0.2/messenger_business_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-06-23 22:24:08.000000 messenger-business-api-1.0.2/messenger_business_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       18 2023-06-23 22:24:08.000000 messenger-business-api-1.0.2/messenger_business_api.egg-info/requires.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       23 2023-06-23 22:24:08.000000 messenger-business-api-1.0.2/messenger_business_api.egg-info/top_level.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      392 2023-06-19 22:14:04.000000 messenger-business-api-1.0.2/pyproject.toml
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-06-23 22:24:08.438342 messenger-business-api-1.0.2/setup.cfg
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      684 2023-06-23 22:24:02.000000 messenger-business-api-1.0.2/setup.py
```

### Comparing `messenger-business-api-1.0.1/LICENSE` & `messenger-business-api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `messenger-business-api-1.0.1/PKG-INFO` & `messenger-business-api-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messenger-business-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: This repository is a wrapper for Meta messenger api for Messenger and Instagram
 Author: Yuri Ramos Lima
 Author-email: yurilima93@hotmail.com
 License: MIT License
 Keywords: python,Meta,Facebook,Instagram,message,chat-bot
 License-File: LICENSE
```

### Comparing `messenger-business-api-1.0.1/README.rst` & `messenger-business-api-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `messenger-business-api-1.0.1/messenger-business-api/api.py` & `messenger-business-api-1.0.2/messenger_business_api/api.py`

 * *Files identical despite different names*

### Comparing `messenger-business-api-1.0.1/messenger_business_api.egg-info/PKG-INFO` & `messenger-business-api-1.0.2/messenger_business_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messenger-business-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: This repository is a wrapper for Meta messenger api for Messenger and Instagram
 Author: Yuri Ramos Lima
 Author-email: yurilima93@hotmail.com
 License: MIT License
 Keywords: python,Meta,Facebook,Instagram,message,chat-bot
 License-File: LICENSE
```

### Comparing `messenger-business-api-1.0.1/setup.py` & `messenger-business-api-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.rst') as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="messenger-business-api",
-    version="1.0.1",
+    version="1.0.2",
     author="Yuri Ramos Lima",
     author_email="yurilima93@hotmail.com",
     description="This repository is a wrapper for Meta messenger api for Messenger and Instagram",
     packages=find_packages(),
     include_package_data=True,
     long_description=README,
     install_requires=[ "pydantic", "requests"],
```

