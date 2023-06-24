# Comparing `tmp/EncroX-1.0.2.tar.gz` & `tmp/EncroX-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EncroX-1.0.2.tar", last modified: Sat Jun 24 04:36:09 2023, max compression
+gzip compressed data, was "EncroX-1.0.3.tar", last modified: Sat Jun 24 05:32:48 2023, max compression
```

## Comparing `EncroX-1.0.2.tar` & `EncroX-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 04:36:09.688291 EncroX-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-24 04:36:09.672972 EncroX-1.0.2/EncroX/
--rw-rw-rw-   0        0        0       48 2023-06-23 18:24:36.000000 EncroX-1.0.2/EncroX/__init__.py
--rw-rw-rw-   0        0        0     2975 2023-06-23 18:24:36.000000 EncroX-1.0.2/EncroX/aes.py
--rw-rw-rw-   0        0        0      861 2023-06-23 18:24:36.000000 EncroX-1.0.2/EncroX/aes.pyi
--rw-rw-rw-   0        0        0     4671 2023-06-23 18:24:36.000000 EncroX-1.0.2/EncroX/ecc.py
--rw-rw-rw-   0        0        0     1445 2023-06-23 18:24:36.000000 EncroX-1.0.2/EncroX/ecc.pyi
--rw-rw-rw-   0        0        0     4995 2023-06-23 18:24:36.000000 EncroX-1.0.2/EncroX/rsa.py
--rw-rw-rw-   0        0        0     1389 2023-06-23 18:24:36.000000 EncroX-1.0.2/EncroX/rsa.pyi
-drwxrwxrwx   0        0        0        0 2023-06-24 04:36:09.684273 EncroX-1.0.2/EncroX.egg-info/
--rw-rw-rw-   0        0        0     7733 2023-06-24 04:36:09.000000 EncroX-1.0.2/EncroX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-06-24 04:36:09.000000 EncroX-1.0.2/EncroX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 04:36:09.000000 EncroX-1.0.2/EncroX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-24 04:36:09.000000 EncroX-1.0.2/EncroX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 04:36:09.000000 EncroX-1.0.2/EncroX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35184 2023-06-23 18:04:53.000000 EncroX-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     7733 2023-06-24 04:36:09.687286 EncroX-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6977 2023-06-23 17:54:25.000000 EncroX-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 04:36:09.688291 EncroX-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      751 2023-06-24 04:36:08.000000 EncroX-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:32:48.267385 EncroX-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-24 05:32:48.243294 EncroX-1.0.3/EncroX/
+-rw-rw-rw-   0        0        0       48 2023-06-23 18:24:36.000000 EncroX-1.0.3/EncroX/__init__.py
+-rw-rw-rw-   0        0        0     2975 2023-06-23 18:24:36.000000 EncroX-1.0.3/EncroX/aes.py
+-rw-rw-rw-   0        0        0      861 2023-06-23 18:24:36.000000 EncroX-1.0.3/EncroX/aes.pyi
+-rw-rw-rw-   0        0        0     4671 2023-06-23 18:24:36.000000 EncroX-1.0.3/EncroX/ecc.py
+-rw-rw-rw-   0        0        0     1445 2023-06-23 18:24:36.000000 EncroX-1.0.3/EncroX/ecc.pyi
+-rw-rw-rw-   0        0        0     4995 2023-06-23 18:24:36.000000 EncroX-1.0.3/EncroX/rsa.py
+-rw-rw-rw-   0        0        0     1389 2023-06-23 18:24:36.000000 EncroX-1.0.3/EncroX/rsa.pyi
+drwxrwxrwx   0        0        0        0 2023-06-24 05:32:48.267385 EncroX-1.0.3/EncroX.egg-info/
+-rw-rw-rw-   0        0        0     7726 2023-06-24 05:32:48.000000 EncroX-1.0.3/EncroX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-06-24 05:32:48.000000 EncroX-1.0.3/EncroX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 05:32:48.000000 EncroX-1.0.3/EncroX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-24 05:32:48.000000 EncroX-1.0.3/EncroX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 05:32:48.000000 EncroX-1.0.3/EncroX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35184 2023-06-23 18:04:53.000000 EncroX-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     7726 2023-06-24 05:32:48.267385 EncroX-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6970 2023-06-24 05:25:29.000000 EncroX-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 05:32:48.267385 EncroX-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      751 2023-06-24 05:31:57.000000 EncroX-1.0.3/setup.py
```

### Comparing `EncroX-1.0.2/EncroX/aes.py` & `EncroX-1.0.3/EncroX/aes.py`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.2/EncroX/aes.pyi` & `EncroX-1.0.3/EncroX/aes.pyi`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.2/EncroX/ecc.py` & `EncroX-1.0.3/EncroX/ecc.py`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.2/EncroX/ecc.pyi` & `EncroX-1.0.3/EncroX/ecc.pyi`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.2/EncroX/rsa.py` & `EncroX-1.0.3/EncroX/rsa.py`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.2/EncroX/rsa.pyi` & `EncroX-1.0.3/EncroX/rsa.pyi`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.2/EncroX.egg-info/PKG-INFO` & `EncroX-1.0.3/EncroX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EncroX
-Version: 1.0.2
+Version: 1.0.3
 Summary: EncroX是一个强大的加密拓展工具，旨在为您的应用程序和系统提供可靠的加密和解密功能。通过集成各种密码学算法和密钥管理方法，EncroX使您能够轻松地进行数据加密、解密和安全通信。
 Home-page: https://github.com/KindLittleTurtle/EncroX
 Author: 核善的小兲
 Author-email: hsdxt@mwtour.cn
 License: AGPL3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -81,15 +81,15 @@
     """
     ...
 ```
 
 ### 使用 RSA 公钥加密数据
 
 ```python
-from EncroX.rsa import encrypted_data
+from EncroX.rsa import rsa_encrypt
 encrypted_data = rsa_encrypt(data, public_key)
 ```
 
 使用 RSA 公钥对数据进行加密，并返回加密后的数据。
 
 #### 函数签名
 
@@ -216,15 +216,15 @@
     ...
 ```
 
 ### 使用 AES 解密数据
 
 ```python
 from EncroX.aes import aes_decrypt
-decrypted_data = aes.aes_decrypt(key, encrypted_data)
+decrypted_data = aes_decrypt(key, encrypted_data)
 ```
 
 使用 AES 密钥解密数据，并返回解密后的原始数据。
 
 #### 函数签名
 
 ```python
```

### Comparing `EncroX-1.0.2/LICENSE` & `EncroX-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.2/PKG-INFO` & `EncroX-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EncroX
-Version: 1.0.2
+Version: 1.0.3
 Summary: EncroX是一个强大的加密拓展工具，旨在为您的应用程序和系统提供可靠的加密和解密功能。通过集成各种密码学算法和密钥管理方法，EncroX使您能够轻松地进行数据加密、解密和安全通信。
 Home-page: https://github.com/KindLittleTurtle/EncroX
 Author: 核善的小兲
 Author-email: hsdxt@mwtour.cn
 License: AGPL3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -81,15 +81,15 @@
     """
     ...
 ```
 
 ### 使用 RSA 公钥加密数据
 
 ```python
-from EncroX.rsa import encrypted_data
+from EncroX.rsa import rsa_encrypt
 encrypted_data = rsa_encrypt(data, public_key)
 ```
 
 使用 RSA 公钥对数据进行加密，并返回加密后的数据。
 
 #### 函数签名
 
@@ -216,15 +216,15 @@
     ...
 ```
 
 ### 使用 AES 解密数据
 
 ```python
 from EncroX.aes import aes_decrypt
-decrypted_data = aes.aes_decrypt(key, encrypted_data)
+decrypted_data = aes_decrypt(key, encrypted_data)
 ```
 
 使用 AES 密钥解密数据，并返回解密后的原始数据。
 
 #### 函数签名
 
 ```python
```

### Comparing `EncroX-1.0.2/README.md` & `EncroX-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     """
     ...
 ```
 
 ### 使用 RSA 公钥加密数据
 
 ```python
-from EncroX.rsa import encrypted_data
+from EncroX.rsa import rsa_encrypt
 encrypted_data = rsa_encrypt(data, public_key)
 ```
 
 使用 RSA 公钥对数据进行加密，并返回加密后的数据。
 
 #### 函数签名
 
@@ -205,15 +205,15 @@
     ...
 ```
 
 ### 使用 AES 解密数据
 
 ```python
 from EncroX.aes import aes_decrypt
-decrypted_data = aes.aes_decrypt(key, encrypted_data)
+decrypted_data = aes_decrypt(key, encrypted_data)
 ```
 
 使用 AES 密钥解密数据，并返回解密后的原始数据。
 
 #### 函数签名
 
 ```python
```

### Comparing `EncroX-1.0.2/setup.py` & `EncroX-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='EncroX',
-    version='1.0.2',
+    version='1.0.3',
     packages=['EncroX'],
     url='https://github.com/KindLittleTurtle/EncroX',
     license='AGPL3.0',
     author='核善的小兲',
     author_email='hsdxt@mwtour.cn',
     description='EncroX是一个强大的加密拓展工具，旨在为您的应用程序和系统提供可靠的加密和解密功能。通过集成各种密码学算法和密钥管理方法，EncroX使您能够轻松地进行数据加密、解密和安全通信。',
     install_requires=['cryptography'],
```

