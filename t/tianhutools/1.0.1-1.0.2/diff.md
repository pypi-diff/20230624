# Comparing `tmp/tianhutools-1.0.1.tar.gz` & `tmp/tianhutools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tianhutools-1.0.1.tar", last modified: Sat Jun  3 12:13:09 2023, max compression
+gzip compressed data, was "tianhutools-1.0.2.tar", last modified: Sat Jun 24 05:38:40 2023, max compression
```

## Comparing `tianhutools-1.0.1.tar` & `tianhutools-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 12:13:09.128363 tianhutools-1.0.1/
--rw-rw-rw-   0        0        0       29 2023-06-03 09:16:20.000000 tianhutools-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4386 2023-06-03 12:13:09.119363 tianhutools-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3937 2023-06-03 09:54:48.000000 tianhutools-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-03 12:13:09.129364 tianhutools-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1116 2023-06-03 09:54:43.000000 tianhutools-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:13:09.079361 tianhutools-1.0.1/tianhutools/
--rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 tianhutools-1.0.1/tianhutools/__init__.py
--rw-rw-rw-   0        0        0     2212 2023-05-27 05:03:59.000000 tianhutools-1.0.1/tianhutools/ip.py
--rw-rw-rw-   0        0        0     6138 2023-05-27 07:12:28.000000 tianhutools-1.0.1/tianhutools/jiami.py
--rw-rw-rw-   0        0        0     2313 2023-06-03 09:54:50.000000 tianhutools-1.0.1/tianhutools/text.py
-drwxrwxrwx   0        0        0        0 2023-06-03 12:13:09.113363 tianhutools-1.0.1/tianhutools.egg-info/
--rw-rw-rw-   0        0        0     4386 2023-06-03 12:13:08.000000 tianhutools-1.0.1/tianhutools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-03 12:13:08.000000 tianhutools-1.0.1/tianhutools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 12:13:08.000000 tianhutools-1.0.1/tianhutools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-03 12:13:08.000000 tianhutools-1.0.1/tianhutools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-03 12:13:08.000000 tianhutools-1.0.1/tianhutools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 05:38:40.025871 tianhutools-1.0.2/
+-rw-rw-rw-   0        0        0       29 2023-06-03 09:16:20.000000 tianhutools-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4576 2023-06-24 05:38:40.023871 tianhutools-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4127 2023-06-24 05:33:28.000000 tianhutools-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 05:38:40.025871 tianhutools-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1134 2023-06-24 05:33:35.000000 tianhutools-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:38:40.000870 tianhutools-1.0.2/tianhutools/
+-rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 tianhutools-1.0.2/tianhutools/__init__.py
+-rw-rw-rw-   0        0        0     2212 2023-05-27 05:03:59.000000 tianhutools-1.0.2/tianhutools/ip.py
+-rw-rw-rw-   0        0        0     6929 2023-06-24 05:31:21.000000 tianhutools-1.0.2/tianhutools/jiami.py
+-rw-rw-rw-   0        0        0     2313 2023-06-03 09:54:50.000000 tianhutools-1.0.2/tianhutools/text.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:38:40.018871 tianhutools-1.0.2/tianhutools.egg-info/
+-rw-rw-rw-   0        0        0     4576 2023-06-24 05:38:39.000000 tianhutools-1.0.2/tianhutools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-24 05:38:39.000000 tianhutools-1.0.2/tianhutools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 05:38:39.000000 tianhutools-1.0.2/tianhutools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-24 05:38:39.000000 tianhutools-1.0.2/tianhutools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-24 05:38:39.000000 tianhutools-1.0.2/tianhutools.egg-info/top_level.txt
```

### Comparing `tianhutools-1.0.1/PKG-INFO` & `tianhutools-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tianhutools
-Version: 1.0.1
+Version: 1.0.2
 Summary: 由天狐宗开发的工具，方便开发时使用,已更名为tianhutools
 Home-page: https://github.com/tianhuzong/thztools
 Author: Sen
 Author-email: tianhuzong@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,16 @@
 - - -
 >1.0.5中，修复一个命名冲突
 - - -
 >2023-6-3 +0800，正式更名为tianhutool，版本重置
 >并加入了文本缩短
 - - -
 >new 1.0.1版本中，将文本缩短修改为使用Python标准库re,math,和第三方库jieba
+- - -
+>1.0.2版本中，修复了上个版本未将jieba安装进setup，并将rsa密钥修改为pem格式，rsa的密文，明文，签名文本与aes的密文，明文都修改为base64
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install tianhutools
 ```
 安装完模块之后接下来就是引用了
```

### Comparing `tianhutools-1.0.1/README.md` & `tianhutools-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 - - -
 >1.0.5中，修复一个命名冲突
 - - -
 >2023-6-3 +0800，正式更名为tianhutool，版本重置
 >并加入了文本缩短
 - - -
 >new 1.0.1版本中，将文本缩短修改为使用Python标准库re,math,和第三方库jieba
+- - -
+>1.0.2版本中，修复了上个版本未将jieba安装进setup，并将rsa密钥修改为pem格式，rsa的密文，明文，签名文本与aes的密文，明文都修改为base64
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install tianhutools
 ```
 安装完模块之后接下来就是引用了
```

### Comparing `tianhutools-1.0.1/setup.py` & `tianhutools-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup
 with open("./README.md",mode='r',encoding='utf-8') as f:
     des = f.read()
 setup(
     name="tianhutools",      # 包名，用于安装和调用该包
-    version="1.0.1",               # 版本号
+    version="1.0.2",               # 版本号
     author="Sen",
     description="由天狐宗开发的工具，方便开发时使用,已更名为tianhutools",
     long_description=des,
     long_description_content_type='text/markdown',
     author_email="tianhuzong@qq.com",
     url="https://github.com/tianhuzong/thztools",
     license="MIT",
     packages=["tianhutools"],     # 需要打包的包，可以是单个或多个包
     package_data={"tianhutools": ["*.py"]},  # 包需要包含的数据文件（可选）
     install_requires=[           # 安装依赖，可以是单个或多个依赖项
         "rsa",
         "Crypto",
         "2ip",
-        "sumy"
+        "sumy",
+        "jieba"
     ],
     classifiers=[                # 分类标签（可选），使用 PyPI 标准分类
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
 )
```

### Comparing `tianhutools-1.0.1/tianhutools/ip.py` & `tianhutools-1.0.2/tianhutools/ip.py`

 * *Files identical despite different names*

### Comparing `tianhutools-1.0.1/tianhutools/jiami.py` & `tianhutools-1.0.2/tianhutools/jiami.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from Crypto.Cipher import AES as AESclass
 from Crypto.Random import get_random_bytes
 import rsa
+import base64
+
+def __bytes_to_b64(bytes_var : bytes) -> str:
+    return base64.b64decode(bytes_var)
+def __b64_to_bytes(b64str : str) -> bytes:
+    return base64.b64encode(b64str)
 class KaiSa:
     def jiami(self,plaintext, shift):
         """
         凯撒加密算法
         plaintext: 明文
         shift: 偏移量
         """
@@ -42,95 +48,100 @@
     def newkeys(self,length : int = 1024):
         """
         生成一个rsa密钥对，默认为1024位
         :param length : int,长度，默认为1024
         :return 公钥,私钥
         """
         (gongyao,siyao) = rsa.newkeys(length)
-        return gongyao,siyao
-    def jiami(self,gongyao,text) -> bytes:
+        gongyao_save = gongyao.save_pkcs1().decode()
+        siyao_save = siyao.save_pkcs1().decode()
+        return gongyao_save,siyao_save
+    def jiami(self,gongyao,text) -> str:
         """
         使用rsa算法进行加密
         Args:
-            gongyao : rsa 公钥
+            gongyao : rsa 公钥pem格式
             text : 欲加密文本
         Return:
-            返回密文(bytes流)
+            返回密文(base64)
         """
         message = text.encode()
-        miwen = rsa.encrypt(message, gongyao)
+        gongyao_obj = rsa.PublicKey.load_pkcs1(gongyao.encode())
+        miwen = base64.b64decode( rsa.encrypt(message, gongyao_obj) ).decode()
         return miwen
-    def jiemi(self,siyao,miwen:bytes):
+    def jiemi(self,siyao,miwen:str):
         """
         使用rsa算法进行解密
         Args:
-            siyao : rsa私钥
-            miwen : 密文（bytes字节流）
+            siyao : rsa私钥,pem格式
+            miwen : 密文（base64）
         Return:
             明文
         """
-        return rsa.decrypt(miwen, siyao).decode()
+        return rsa.decrypt(base64.b64encode(miwen), siyao).decode()
     def sign(self,siyao,text):
         """
         使用rsa算法进行数字签名
-        :param siyao:rsa私钥
+        :param siyao:rsa私钥,pem格式
         :param text:欲签名文本
         :return 返回签名文本
         """
-        qianminwenben = rsa.sign(text.encode(),siyao,'SHA-1')
+        siyao_obj = rsa.PrivateKey.load_pkcs1(siyao)
+        qianminwenben = base64.b64decode( rsa.sign(text.encode(),siyao_obj,'SHA-1') ).decode()
         return qianminwenben
     def qmyz(self,text,qmwb,gongyao):
         """
         签名验证
         :param text:被验证的文本
         :param qmwb:签名文本，sign()函数的返回值
-        :param gongyao:rsa公钥
+        :param gongyao:rsa公钥,pem格式
         :return 成功返回True，失败返回False
         """
-        res = rsa.verify(text.encode(),qmwb,gongyao)
+        res = rsa.verify(text.encode(),base64.b64encode(qmwb),rsa.PublicKey.load_pkcs1(gongyao))
         if res:
             return True
         else:
             return False
 class AES:
     def newkey(self):
         """
         自动生成32位（256位）AES秘钥
+        :return key，base64编码的key
         """
         key = get_random_bytes(32)
-        return key
+        return base64.b64decode(key).decode()
 
     def jiami(self,plaintext, key):
         """
         AES加密算法
         plaintext: 明文
-        key: 秘钥
+        key: 秘钥,base64
         Returns:
-            密文,随机数，验证标签，均为bytes类型
+            密文,随机数，验证标签，均为str类型的base64编码
         """
         # 用秘钥创建一个AES对象
-        cipher = AESclass.new(key, AESclass.MODE_EAX)
+        cipher = AESclass.new(base64.b64encode(key), AESclass.MODE_EAX)
         # 加密明文
         ciphertext, tag = cipher.encrypt_and_digest(plaintext.encode('utf-8'))
         # 返回加密后的密文和必要的参数
-        return ciphertext, cipher.nonce, tag
+        return __bytes_to_b64(ciphertext), __bytes_to_b64(cipher.nonce), __bytes_to_b64(tag)
 
     def jiemi(self,ciphertext, key, nonce, tag):
         """
         AES解密算法
         ciphertext: 密文
         key: 秘钥
         nonce: 加密时生成的随机数
         tag: 加密时生成的验证标签
         """
         # 用密钥和随机数创建一个AES对象
-        cipher = AESclass.new(key, AESclass.MODE_EAX, nonce=nonce)
+        cipher = AESclass.new(__b64_to_bytes(key), AESclass.MODE_EAX, nonce=__b64_to_bytes(nonce))
         try:
             # 解密密文
-            plaintext = cipher.decrypt_and_verify(ciphertext, tag)
+            plaintext = cipher.decrypt_and_verify(__b64_to_bytes(ciphertext), __b64_to_bytes(tag))
             return plaintext.decode('utf-8')
         except:
             return None
 class Weijiniya:
     def jiami(self,plaintext, key):
         """
         使用维吉尼亚密码加密明文字符串
```

### Comparing `tianhutools-1.0.1/tianhutools/text.py` & `tianhutools-1.0.2/tianhutools/text.py`

 * *Files identical despite different names*

### Comparing `tianhutools-1.0.1/tianhutools.egg-info/PKG-INFO` & `tianhutools-1.0.2/tianhutools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tianhutools
-Version: 1.0.1
+Version: 1.0.2
 Summary: 由天狐宗开发的工具，方便开发时使用,已更名为tianhutools
 Home-page: https://github.com/tianhuzong/thztools
 Author: Sen
 Author-email: tianhuzong@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,16 @@
 - - -
 >1.0.5中，修复一个命名冲突
 - - -
 >2023-6-3 +0800，正式更名为tianhutool，版本重置
 >并加入了文本缩短
 - - -
 >new 1.0.1版本中，将文本缩短修改为使用Python标准库re,math,和第三方库jieba
+- - -
+>1.0.2版本中，修复了上个版本未将jieba安装进setup，并将rsa密钥修改为pem格式，rsa的密文，明文，签名文本与aes的密文，明文都修改为base64
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install tianhutools
 ```
 安装完模块之后接下来就是引用了
```

