# Comparing `tmp/botocore-a-la-carte-payment-cryptography-1.29.159.tar.gz` & `tmp/botocore-a-la-carte-payment-cryptography-1.29.160.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-payment-cryptography-1.29.159.tar", last modified: Fri Jun 23 01:43:04 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-payment-cryptography-1.29.160.tar", last modified: Sat Jun 24 01:41:32 2023, max compression
```

## Comparing `botocore-a-la-carte-payment-cryptography-1.29.159.tar` & `botocore-a-la-carte-payment-cryptography-1.29.160.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:43:04.818524 botocore-a-la-carte-payment-cryptography-1.29.159/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-23 01:43:04.000000 botocore-a-la-carte-payment-cryptography-1.29.159/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-23 01:43:04.818524 botocore-a-la-carte-payment-cryptography-1.29.159/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:43:04.814524 botocore-a-la-carte-payment-cryptography-1.29.159/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:43:04.814524 botocore-a-la-carte-payment-cryptography-1.29.159/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:43:04.814524 botocore-a-la-carte-payment-cryptography-1.29.159/botocore/data/payment-cryptography/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:43:04.814524 botocore-a-la-carte-payment-cryptography-1.29.159/botocore/data/payment-cryptography/2021-09-14/
--rw-r--r--   0 runner    (1001) docker     (123)    17732 2023-06-23 01:42:24.000000 botocore-a-la-carte-payment-cryptography-1.29.159/botocore/data/payment-cryptography/2021-09-14/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-23 01:42:24.000000 botocore-a-la-carte-payment-cryptography-1.29.159/botocore/data/payment-cryptography/2021-09-14/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    87954 2023-06-23 01:42:24.000000 botocore-a-la-carte-payment-cryptography-1.29.159/botocore/data/payment-cryptography/2021-09-14/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:43:04.818524 botocore-a-la-carte-payment-cryptography-1.29.159/botocore_a_la_carte_payment_cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-23 01:43:04.000000 botocore-a-la-carte-payment-cryptography-1.29.159/botocore_a_la_carte_payment_cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-23 01:43:04.000000 botocore-a-la-carte-payment-cryptography-1.29.159/botocore_a_la_carte_payment_cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 01:43:04.000000 botocore-a-la-carte-payment-cryptography-1.29.159/botocore_a_la_carte_payment_cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 01:43:04.000000 botocore-a-la-carte-payment-cryptography-1.29.159/botocore_a_la_carte_payment_cryptography.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 01:43:04.818524 botocore-a-la-carte-payment-cryptography-1.29.159/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-23 01:43:04.000000 botocore-a-la-carte-payment-cryptography-1.29.159/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:41:32.087135 botocore-a-la-carte-payment-cryptography-1.29.160/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-24 01:41:31.000000 botocore-a-la-carte-payment-cryptography-1.29.160/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-24 01:41:32.087135 botocore-a-la-carte-payment-cryptography-1.29.160/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:41:32.087135 botocore-a-la-carte-payment-cryptography-1.29.160/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:41:32.087135 botocore-a-la-carte-payment-cryptography-1.29.160/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:41:32.087135 botocore-a-la-carte-payment-cryptography-1.29.160/botocore/data/payment-cryptography/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:41:32.087135 botocore-a-la-carte-payment-cryptography-1.29.160/botocore/data/payment-cryptography/2021-09-14/
+-rw-r--r--   0 runner    (1001) docker     (123)    17732 2023-06-24 01:40:51.000000 botocore-a-la-carte-payment-cryptography-1.29.160/botocore/data/payment-cryptography/2021-09-14/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-24 01:40:51.000000 botocore-a-la-carte-payment-cryptography-1.29.160/botocore/data/payment-cryptography/2021-09-14/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    87954 2023-06-24 01:40:51.000000 botocore-a-la-carte-payment-cryptography-1.29.160/botocore/data/payment-cryptography/2021-09-14/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:41:32.087135 botocore-a-la-carte-payment-cryptography-1.29.160/botocore_a_la_carte_payment_cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-24 01:41:32.000000 botocore-a-la-carte-payment-cryptography-1.29.160/botocore_a_la_carte_payment_cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-24 01:41:32.000000 botocore-a-la-carte-payment-cryptography-1.29.160/botocore_a_la_carte_payment_cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 01:41:32.000000 botocore-a-la-carte-payment-cryptography-1.29.160/botocore_a_la_carte_payment_cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 01:41:32.000000 botocore-a-la-carte-payment-cryptography-1.29.160/botocore_a_la_carte_payment_cryptography.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 01:41:32.087135 botocore-a-la-carte-payment-cryptography-1.29.160/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-24 01:41:31.000000 botocore-a-la-carte-payment-cryptography-1.29.160/setup.py
```

### Comparing `botocore-a-la-carte-payment-cryptography-1.29.159/LICENSE.txt` & `botocore-a-la-carte-payment-cryptography-1.29.160/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-payment-cryptography-1.29.159/PKG-INFO` & `botocore-a-la-carte-payment-cryptography-1.29.160/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-payment-cryptography
-Version: 1.29.159
+Version: 1.29.160
 Summary: payment-cryptography data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-payment-cryptography-1.29.159/botocore/data/payment-cryptography/2021-09-14/endpoint-rule-set-1.json` & `botocore-a-la-carte-payment-cryptography-1.29.160/botocore/data/payment-cryptography/2021-09-14/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-payment-cryptography-1.29.159/botocore/data/payment-cryptography/2021-09-14/service-2.json` & `botocore-a-la-carte-payment-cryptography-1.29.160/botocore/data/payment-cryptography/2021-09-14/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-payment-cryptography-1.29.159/botocore_a_la_carte_payment_cryptography.egg-info/PKG-INFO` & `botocore-a-la-carte-payment-cryptography-1.29.160/botocore_a_la_carte_payment_cryptography.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-payment-cryptography
-Version: 1.29.159
+Version: 1.29.160
 Summary: payment-cryptography data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-payment-cryptography-1.29.159/setup.py` & `botocore-a-la-carte-payment-cryptography-1.29.160/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-payment-cryptography',
-    version="1.29.159",
+    version="1.29.160",
     description='payment-cryptography data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/payment-cryptography/*/*.json'],
```

