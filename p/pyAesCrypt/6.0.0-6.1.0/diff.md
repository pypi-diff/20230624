# Comparing `tmp/pyAesCrypt-6.0.0.tar.gz` & `tmp/pyAesCrypt-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyAesCrypt-6.0.0.tar", last modified: Sun May  9 10:09:21 2021, max compression
+gzip compressed data, was "pyAesCrypt-6.1.0.tar", last modified: Sat Jun 24 11:48:55 2023, max compression
```

## Comparing `pyAesCrypt-6.0.0.tar` & `pyAesCrypt-6.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 marcomurk  (1000) marcomurk  (1000)        0 2021-05-09 10:09:21.000000 pyAesCrypt-6.0.0/
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)     1712 2021-05-09 09:42:11.000000 pyAesCrypt-6.0.0/HISTORY.rst
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)    11357 2018-12-02 12:53:22.000000 pyAesCrypt-6.0.0/LICENSE
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)       50 2018-12-02 12:53:22.000000 pyAesCrypt-6.0.0/MANIFEST.in
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)     6584 2021-05-09 10:09:21.000000 pyAesCrypt-6.0.0/PKG-INFO
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)     4770 2021-05-09 09:52:30.000000 pyAesCrypt-6.0.0/README.rst
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)      781 2021-05-09 09:42:11.000000 pyAesCrypt-6.0.0/THANKS.rst
-drwxr-xr-x   0 marcomurk  (1000) marcomurk  (1000)        0 2021-05-09 10:09:21.000000 pyAesCrypt-6.0.0/bin/
--rwxr-xr-x   0 marcomurk  (1000) marcomurk  (1000)     5203 2021-01-22 13:03:24.000000 pyAesCrypt-6.0.0/bin/pyAesCrypt
-drwxr-xr-x   0 marcomurk  (1000) marcomurk  (1000)        0 2021-05-09 10:09:21.000000 pyAesCrypt-6.0.0/pyAesCrypt/
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)       75 2018-12-02 12:53:22.000000 pyAesCrypt-6.0.0/pyAesCrypt/__init__.py
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)    14601 2021-05-09 09:42:11.000000 pyAesCrypt-6.0.0/pyAesCrypt/crypto.py
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)    13550 2021-05-09 09:42:11.000000 pyAesCrypt-6.0.0/pyAesCrypt/test_crypto.py
-drwxr-xr-x   0 marcomurk  (1000) marcomurk  (1000)        0 2021-05-09 10:09:21.000000 pyAesCrypt-6.0.0/pyAesCrypt.egg-info/
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)     6584 2021-05-09 10:09:20.000000 pyAesCrypt-6.0.0/pyAesCrypt.egg-info/PKG-INFO
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)      316 2021-05-09 10:09:20.000000 pyAesCrypt-6.0.0/pyAesCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)        1 2021-05-09 10:09:20.000000 pyAesCrypt-6.0.0/pyAesCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)       13 2021-05-09 10:09:20.000000 pyAesCrypt-6.0.0/pyAesCrypt.egg-info/requires.txt
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)       11 2021-05-09 10:09:20.000000 pyAesCrypt-6.0.0/pyAesCrypt.egg-info/top_level.txt
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)       38 2021-05-09 10:09:21.000000 pyAesCrypt-6.0.0/setup.cfg
--rw-r--r--   0 marcomurk  (1000) marcomurk  (1000)      911 2021-05-09 09:42:11.000000 pyAesCrypt-6.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 11:48:55.356089 pyAesCrypt-6.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-24 11:48:42.000000 pyAesCrypt-6.1.0/HISTORY.rst
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-24 11:48:42.000000 pyAesCrypt-6.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-24 11:48:42.000000 pyAesCrypt-6.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5189 2023-06-24 11:48:55.356089 pyAesCrypt-6.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4622 2023-06-24 11:48:42.000000 pyAesCrypt-6.1.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-24 11:48:42.000000 pyAesCrypt-6.1.0/THANKS.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 11:48:55.352089 pyAesCrypt-6.1.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     5203 2023-06-24 11:48:42.000000 pyAesCrypt-6.1.0/bin/pyAesCrypt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 11:48:55.356089 pyAesCrypt-6.1.0/pyAesCrypt/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-24 11:48:42.000000 pyAesCrypt-6.1.0/pyAesCrypt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13520 2023-06-24 11:48:42.000000 pyAesCrypt-6.1.0/pyAesCrypt/crypto.py
+-rw-r--r--   0 root         (0) root         (0)    14411 2023-06-24 11:48:42.000000 pyAesCrypt-6.1.0/pyAesCrypt/test_crypto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 11:48:55.356089 pyAesCrypt-6.1.0/pyAesCrypt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5189 2023-06-24 11:48:55.000000 pyAesCrypt-6.1.0/pyAesCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      316 2023-06-24 11:48:55.000000 pyAesCrypt-6.1.0/pyAesCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 11:48:55.000000 pyAesCrypt-6.1.0/pyAesCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-24 11:48:55.000000 pyAesCrypt-6.1.0/pyAesCrypt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-24 11:48:55.000000 pyAesCrypt-6.1.0/pyAesCrypt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 11:48:55.356089 pyAesCrypt-6.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-24 11:48:42.000000 pyAesCrypt-6.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyAesCrypt-6.0.0/HISTORY.rst` & `pyAesCrypt-6.1.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `pyAesCrypt-6.0.0/LICENSE` & `pyAesCrypt-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAesCrypt-6.0.0/PKG-INFO` & `pyAesCrypt-6.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,162 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyAesCrypt
-Version: 6.0.0
+Version: 6.1.0
 Summary: Encrypt and decrypt files and streams in AES Crypt format (version 2)
 Home-page: https://github.com/marcobellaccini/pyAesCrypt
 Author: Marco Bellaccini
-Author-email: UNKNOWN
 License: Apache License 2.0
-Description: pyAesCrypt
-        ===============
-        .. image:: https://travis-ci.com/marcobellaccini/pyAesCrypt.svg?branch=master
-            :target: https://travis-ci.com/marcobellaccini/pyAesCrypt
-        .. image:: https://pepy.tech/badge/pyaescrypt
-            :target: https://pepy.tech/project/pyaescrypt
-        
-        About pyAesCrypt
-        --------------------------
-        pyAesCrypt is a Python 3 file-encryption module and script that uses AES256-CBC to encrypt/decrypt files and binary streams.
-        
-        pyAesCrypt is compatible with the `AES Crypt`_ `file format`_ (version 2).
-        
-        It is Free Software, released under the `Apache License, Version 2.0`_.
-        
-        pyAesCrypt is brought to you by Marco Bellaccini - marco.bellaccini(at!)gmail.com.
-         
-        IMPORTANT SECURITY NOTE: version 2 of the AES Crypt file format does not authenticate the "file size modulo 16" byte. This implies that an attacker  
-        with write access to the encrypted file may alter the corresponding plaintext file size by up to 15 bytes.
-        
-        NOTE: there is no low-level memory management in Python, hence it is not possible to wipe memory areas were sensitive information was stored.
-        
-        Module usage example
-        ------------------------
-        Here is an example showing encryption and decryption of a file:
-        
-        .. code:: python
-        
-            import pyAesCrypt
-            password = "please-use-a-long-and-random-password"
-            # encrypt
-            pyAesCrypt.encryptFile("data.txt", "data.txt.aes", password)
-            # decrypt
-            pyAesCrypt.decryptFile("data.txt.aes", "dataout.txt", password)
-        
-        **This is the most straightforward way to use pyAesCrypt, and should be preferred.**
-        
-        If you need to specify a custom buffer size (default is 64KB), you can pass it as an optional argument:
-        
-        .. code:: python
-        
-            import pyAesCrypt
-            # custom encryption/decryption buffer size (default is 64KB)
-            bufferSize = 128 * 1024
-            password = "please-use-a-long-and-random-password"
-            # encrypt
-            pyAesCrypt.encryptFile("data.txt", "data.txt.aes", password, bufferSize)
-            # decrypt
-            pyAesCrypt.decryptFile("data.txt.aes", "dataout.txt", password, bufferSize)
-        
-        In case you need it, you can work with binary streams too:
-        
-        .. code:: python
-        
-            import pyAesCrypt
-            from os import stat, remove
-            # encryption/decryption buffer size - 64K
-            # with stream-oriented functions, setting buffer size is mandatory
-            bufferSize = 64 * 1024
-            password = "please-use-a-long-and-random-password"
-            
-            # encrypt
-            with open("data.txt", "rb") as fIn:
-                with open("data.txt.aes", "wb") as fOut:
-                    pyAesCrypt.encryptStream(fIn, fOut, password, bufferSize)
-            
-            # get encrypted file size
-            encFileSize = stat("data.txt.aes").st_size
-            
-            # decrypt
-            with open("data.txt.aes", "rb") as fIn:
-                try:
-                    with open("dataout.txt", "wb") as fOut:
-                        # decrypt file stream
-                        pyAesCrypt.decryptStream(fIn, fOut, password, bufferSize, encFileSize)
-                except ValueError:
-                    # remove output file on error
-                    remove("dataout.txt")
-        
-        you can also perform in-memory encryption/decryption (using BytesIO):
-        
-        .. code:: python
-        
-            import pyAesCrypt
-            import io
-            
-            bufferSize = 64 * 1024
-            password = "please-use-a-long-and-random-password"
-            
-            # binary data to be encrypted
-            pbdata = b"This is binary plaintext \x00\x01"
-            
-            # input plaintext binary stream
-            fIn = io.BytesIO(pbdata)
-            
-            # initialize ciphertext binary stream
-            fCiph = io.BytesIO()
-            
-            # initialize decrypted binary stream
-            fDec = io.BytesIO()
-            
-            # encrypt stream
-            pyAesCrypt.encryptStream(fIn, fCiph, password, bufferSize)
-            
-            # print encrypted data
-            print("This is the ciphertext:\n" + str(fCiph.getvalue()))
-            
-            # get ciphertext length
-            ctlen = len(fCiph.getvalue())
-            
-            # go back to the start of the ciphertext stream
-            fCiph.seek(0)
-            
-            # decrypt stream
-            pyAesCrypt.decryptStream(fCiph, fDec, password, bufferSize, ctlen)
-            
-            # print decrypted data
-            print("Decrypted data:\n" + str(fDec.getvalue()))
-        
-        
-        
-        Script usage examples
-        ------------------------
-        Encrypt file test.txt in test.txt.aes:
-        
-        	pyAesCrypt -e test.txt
-        
-        Decrypt file test.txt.aes in test.txt:
-        
-        	pyAesCrypt -d test.txt.aes
-        	
-        Encrypt file test.txt in test2.txt.aes:
-        
-        	pyAesCrypt -e test.txt -o test2.txt.aes
-        
-        Decrypt file test.txt.aes in test2.txt:
-        
-        	pyAesCrypt -d test.txt.aes -o test2.txt
-        
-        FAQs
-        ------------------------
-        - *Is pyAesCrypt malware?*
-        
-          **NO!** Of course it isn't!
-        
-          Nevertheless, being a module, it can be used by any other software, including malware.
-          
-          In fact, it has been reported that it is used as crypto library by some ransomware.
-        
-        .. _AES Crypt: https://www.aescrypt.com
-        .. _file format: https://www.aescrypt.com/aes_file_format.html
-        .. _Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
-        
 Keywords: AES Crypt encrypt decrypt
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+pyAesCrypt
+===============
+.. image:: https://github.com/marcobellaccini/pyaescrypt/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/marcobellaccini/pyAesCrypt/actions
+.. image:: https://pepy.tech/badge/pyaescrypt
+    :target: https://pepy.tech/project/pyaescrypt
+
+About pyAesCrypt
+--------------------------
+pyAesCrypt is a Python 3 file-encryption module and script that uses AES256-CBC to encrypt/decrypt files and binary streams.
+
+pyAesCrypt is compatible with the `AES Crypt`_ `file format`_ (version 2).
+
+It is Free Software, released under the `Apache License, Version 2.0`_.
+
+pyAesCrypt is brought to you by Marco Bellaccini - marco.bellaccini(at!)gmail.com.
+ 
+IMPORTANT SECURITY NOTE: version 2 of the AES Crypt file format does not authenticate the "file size modulo 16" byte. This implies that an attacker  
+with write access to the encrypted file may alter the corresponding plaintext file size by up to 15 bytes.
+
+NOTE: there is no low-level memory management in Python, hence it is not possible to wipe memory areas were sensitive information was stored.
+
+Module usage example
+------------------------
+Here is an example showing encryption and decryption of a file:
+
+.. code:: python
+
+    import pyAesCrypt
+    password = "please-use-a-long-and-random-password"
+    # encrypt
+    pyAesCrypt.encryptFile("data.txt", "data.txt.aes", password)
+    # decrypt
+    pyAesCrypt.decryptFile("data.txt.aes", "dataout.txt", password)
+
+**This is the most straightforward way to use pyAesCrypt, and should be preferred.**
+
+If you need to specify a custom buffer size (default is 64KB), you can pass it as an optional argument:
+
+.. code:: python
+
+    import pyAesCrypt
+    # custom encryption/decryption buffer size (default is 64KB)
+    bufferSize = 128 * 1024
+    password = "please-use-a-long-and-random-password"
+    # encrypt
+    pyAesCrypt.encryptFile("data.txt", "data.txt.aes", password, bufferSize)
+    # decrypt
+    pyAesCrypt.decryptFile("data.txt.aes", "dataout.txt", password, bufferSize)
+
+In case you need it, you can work with binary streams too:
+
+.. code:: python
+
+    import pyAesCrypt
+    from os import stat, remove
+    # encryption/decryption buffer size - 64K
+    # with stream-oriented functions, setting buffer size is mandatory
+    bufferSize = 64 * 1024
+    password = "please-use-a-long-and-random-password"
+    
+    # encrypt
+    with open("data.txt", "rb") as fIn:
+        with open("data.txt.aes", "wb") as fOut:
+            pyAesCrypt.encryptStream(fIn, fOut, password, bufferSize)
+    
+    # decrypt
+    with open("data.txt.aes", "rb") as fIn:
+        try:
+            with open("dataout.txt", "wb") as fOut:
+                # decrypt file stream
+                pyAesCrypt.decryptStream(fIn, fOut, password, bufferSize)
+        except ValueError:
+            # remove output file on error
+            remove("dataout.txt")
+
+you can also perform in-memory encryption/decryption (using BytesIO):
+
+.. code:: python
+
+    import pyAesCrypt
+    import io
+    
+    bufferSize = 64 * 1024
+    password = "please-use-a-long-and-random-password"
+    
+    # binary data to be encrypted
+    pbdata = b"This is binary plaintext \x00\x01"
+    
+    # input plaintext binary stream
+    fIn = io.BytesIO(pbdata)
+    
+    # initialize ciphertext binary stream
+    fCiph = io.BytesIO()
+    
+    # initialize decrypted binary stream
+    fDec = io.BytesIO()
+    
+    # encrypt stream
+    pyAesCrypt.encryptStream(fIn, fCiph, password, bufferSize)
+    
+    # print encrypted data
+    print("This is the ciphertext:\n" + str(fCiph.getvalue()))
+    
+    # go back to the start of the ciphertext stream
+    fCiph.seek(0)
+    
+    # decrypt stream
+    pyAesCrypt.decryptStream(fCiph, fDec, password, bufferSize)
+    
+    # print decrypted data
+    print("Decrypted data:\n" + str(fDec.getvalue()))
+
+
+
+Script usage examples
+------------------------
+Encrypt file test.txt in test.txt.aes:
+
+	pyAesCrypt -e test.txt
+
+Decrypt file test.txt.aes in test.txt:
+
+	pyAesCrypt -d test.txt.aes
+	
+Encrypt file test.txt in test2.txt.aes:
+
+	pyAesCrypt -e test.txt -o test2.txt.aes
+
+Decrypt file test.txt.aes in test2.txt:
+
+	pyAesCrypt -d test.txt.aes -o test2.txt
+
+FAQs
+------------------------
+- *Is pyAesCrypt malware?*
+
+  **NO!** Of course it isn't!
+
+  Nevertheless, being a module, it can be used by any other software, including malware.
+  
+  In fact, it has been reported that it is used as crypto library by some ransomware.
+
+.. _AES Crypt: https://www.aescrypt.com
+.. _file format: https://www.aescrypt.com/aes_file_format.html
+.. _Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyAesCrypt-6.0.0/README.rst` & `pyAesCrypt-6.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pyAesCrypt
 ===============
-.. image:: https://travis-ci.com/marcobellaccini/pyAesCrypt.svg?branch=master
-    :target: https://travis-ci.com/marcobellaccini/pyAesCrypt
+.. image:: https://github.com/marcobellaccini/pyaescrypt/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/marcobellaccini/pyAesCrypt/actions
 .. image:: https://pepy.tech/badge/pyaescrypt
     :target: https://pepy.tech/project/pyaescrypt
 
 About pyAesCrypt
 --------------------------
 pyAesCrypt is a Python 3 file-encryption module and script that uses AES256-CBC to encrypt/decrypt files and binary streams.
 
@@ -60,23 +60,20 @@
     password = "please-use-a-long-and-random-password"
     
     # encrypt
     with open("data.txt", "rb") as fIn:
         with open("data.txt.aes", "wb") as fOut:
             pyAesCrypt.encryptStream(fIn, fOut, password, bufferSize)
     
-    # get encrypted file size
-    encFileSize = stat("data.txt.aes").st_size
-    
     # decrypt
     with open("data.txt.aes", "rb") as fIn:
         try:
             with open("dataout.txt", "wb") as fOut:
                 # decrypt file stream
-                pyAesCrypt.decryptStream(fIn, fOut, password, bufferSize, encFileSize)
+                pyAesCrypt.decryptStream(fIn, fOut, password, bufferSize)
         except ValueError:
             # remove output file on error
             remove("dataout.txt")
 
 you can also perform in-memory encryption/decryption (using BytesIO):
 
 .. code:: python
@@ -101,22 +98,19 @@
     
     # encrypt stream
     pyAesCrypt.encryptStream(fIn, fCiph, password, bufferSize)
     
     # print encrypted data
     print("This is the ciphertext:\n" + str(fCiph.getvalue()))
     
-    # get ciphertext length
-    ctlen = len(fCiph.getvalue())
-    
     # go back to the start of the ciphertext stream
     fCiph.seek(0)
     
     # decrypt stream
-    pyAesCrypt.decryptStream(fCiph, fDec, password, bufferSize, ctlen)
+    pyAesCrypt.decryptStream(fCiph, fDec, password, bufferSize)
     
     # print decrypted data
     print("Decrypted data:\n" + str(fDec.getvalue()))
 
 
 
 Script usage examples
```

### Comparing `pyAesCrypt-6.0.0/THANKS.rst` & `pyAesCrypt-6.1.0/THANKS.rst`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 
 * Thanks to `sander76`_ for finding an issue affecting output file removal.
 
 * Thanks to `Dead4W`_ for improving CI.
 
 * Thanks to `MySixSenses`_ for pointing out that there was no default buffer size.
 
+* Thanks to `ddelange`_ for improving decryptStream.
+
 .. _Ben Fisher: https://downpoured.github.io/
 
 .. _Thomas O'Neill: https://github.com/toneill818
 
 .. _Harish Navnit: https://github.com/harishnavnit
 
 .. _sander76: https://github.com/sander76
 
 .. _Dead4W: https://github.com/Dead4W
 
 .. _MySixSenses: https://github.com/MySixSenses
+
+.. _ddelange: https://github.com/ddelange
```

### Comparing `pyAesCrypt-6.0.0/bin/pyAesCrypt` & `pyAesCrypt-6.1.0/bin/pyAesCrypt`

 * *Files identical despite different names*

### Comparing `pyAesCrypt-6.0.0/pyAesCrypt/crypto.py` & `pyAesCrypt-6.1.0/pyAesCrypt/crypto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,429 +1,405 @@
-#==============================================================================
+# ==============================================================================
 # Copyright 2020 Marco Bellaccini - marco.bellaccini[at!]gmail.com
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#==============================================================================
+# ==============================================================================
 
-#==============================================================================
+# ==============================================================================
 # pyAesCrypt
 #
 # pyAesCrypt is a Python file-encryption utility that uses AES256-CBC to
 # encrypt/decrypt files and binary streams.
 # pyAesCrypt is compatible with the AES Crypt (https://www.aescrypt.com/)
 # file format (version 2).
 # It uses PyCA Cryptography for crypto primitives and the operating system's
-# random number generator (/dev/urandom on UNIX platforms, CryptGenRandom 
+# random number generator (/dev/urandom on UNIX platforms, CryptGenRandom
 # on Windows).
 #
 # IMPORTANT SECURITY NOTE: version 2 of the AES Crypt file format does not
 # authenticate the "file size modulo 16" byte. This implies that an attacker
 # with write access to the encrypted file may alter the corresponding plaintext
 # file size by up to 15 bytes.
 #
 # NOTE: there is no low-level memory management in Python, hence it is
 # not possible to wipe memory areas were sensitive information was stored.
-#==============================================================================
+# ==============================================================================
 
 # pyAesCrypt module
 
+import io
+import warnings
+from os import path, remove, urandom
+
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, hmac
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
-from os import urandom
-from os import stat, remove, path
 
 # pyAesCrypt version - now semver
-version = "6.0.0"
+version = "6.1.0"
 
 # default encryption/decryption buffer size - 64KB
 bufferSizeDef = 64 * 1024
 
 # maximum password length (number of chars)
 maxPassLen = 1024
 
 # AES block size in bytes
 AESBlockSize = 16
 
 
 # password stretching function
 def stretch(passw, iv1):
-    
+
     # hash the external iv and the password 8192 times
     digest = iv1 + (16 * b"\x00")
-    
+
     for i in range(8192):
         passHash = hashes.Hash(hashes.SHA256(), backend=default_backend())
         passHash.update(digest)
         passHash.update(bytes(passw, "utf_16_le"))
         digest = passHash.finalize()
-    
+
     return digest
 
+
 # encrypt file function
 # arguments:
 # infile: plaintext file path
 # outfile: ciphertext file path
 # passw: encryption password
 # bufferSize: optional buffer size, must be a multiple of
 #             AES block size (16)
 #             using a larger buffer speeds up things when dealing
 #             with big files
 #             Default is 64KB.
-def encryptFile(infile, outfile, passw, bufferSize = bufferSizeDef):
+def encryptFile(infile, outfile, passw, bufferSize=bufferSizeDef):
     try:
         with open(infile, "rb") as fIn:
             # check that output file does not exist
             # or that, if exists, is not the same as the input file
             # (i.e.: overwrite if it seems safe)
             if path.isfile(outfile):
                 if path.samefile(infile, outfile):
-                    raise ValueError("Input and output files "
-                                     "are the same.")
+                    raise ValueError("Input and output files are the same.")
             try:
                 with open(outfile, "wb") as fOut:
                     # encrypt file stream
                     encryptStream(fIn, fOut, passw, bufferSize)
-                
+
             except IOError:
                 raise ValueError("Unable to write output file.")
-            
+
     except IOError:
         raise ValueError("Unable to read input file.")
-                
+
 
 # encrypt binary stream function
 # arguments:
 # fIn: input binary stream
 # fOut: output binary stream
 # passw: encryption password
 # bufferSize: encryption buffer size, must be a multiple of
 #             AES block size (16)
 #             using a larger buffer speeds up things when dealing
 #             with long streams
-def encryptStream(fIn, fOut, passw, bufferSize):
+def encryptStream(fIn, fOut, passw, bufferSize=bufferSizeDef):
     # validate bufferSize
     if bufferSize % AESBlockSize != 0:
         raise ValueError("Buffer size must be a multiple of AES block size.")
-    
+
     if len(passw) > maxPassLen:
         raise ValueError("Password is too long.")
 
     # generate external iv (used to encrypt the main iv and the
     # encryption key)
     iv1 = urandom(AESBlockSize)
-    
+
     # stretch password and iv
     key = stretch(passw, iv1)
-    
+
     # generate random main iv
     iv0 = urandom(AESBlockSize)
-    
+
     # generate random internal key
     intKey = urandom(32)
-    
+
     # instantiate AES cipher
-    cipher0 = Cipher(algorithms.AES(intKey), modes.CBC(iv0),
-                     backend=default_backend())
+    cipher0 = Cipher(algorithms.AES(intKey), modes.CBC(iv0), backend=default_backend())
     encryptor0 = cipher0.encryptor()
-    
+
     # instantiate HMAC-SHA256 for the ciphertext
-    hmac0 = hmac.HMAC(intKey, hashes.SHA256(),
-                      backend=default_backend())
-    
+    hmac0 = hmac.HMAC(intKey, hashes.SHA256(), backend=default_backend())
+
     # instantiate another AES cipher
-    cipher1 = Cipher(algorithms.AES(key), modes.CBC(iv1),
-                     backend=default_backend())
+    cipher1 = Cipher(algorithms.AES(key), modes.CBC(iv1), backend=default_backend())
     encryptor1 = cipher1.encryptor()
-    
+
     # encrypt main iv and key
     c_iv_key = encryptor1.update(iv0 + intKey) + encryptor1.finalize()
-    
+
     # calculate HMAC-SHA256 of the encrypted iv and key
-    hmac1 = hmac.HMAC(key, hashes.SHA256(),
-                      backend=default_backend())
+    hmac1 = hmac.HMAC(key, hashes.SHA256(), backend=default_backend())
     hmac1.update(c_iv_key)
 
     # write header
     fOut.write(bytes("AES", "utf8"))
-    
+
     # write version (AES Crypt version 2 file format -
     # see https://www.aescrypt.com/aes_file_format.html)
     fOut.write(b"\x02")
-    
+
     # reserved byte (set to zero)
     fOut.write(b"\x00")
-    
+
     # setup "CREATED-BY" extension
     cby = "pyAesCrypt " + version
-    
+
     # write "CREATED-BY" extension length
-    fOut.write(b"\x00" + bytes([1+len("CREATED_BY"+cby)]))
-    
+    fOut.write(b"\x00" + bytes([1 + len("CREATED_BY" + cby)]))
+
     # write "CREATED-BY" extension
-    fOut.write(bytes("CREATED_BY", "utf8") + b"\x00" +
-               bytes(cby, "utf8"))
-    
+    fOut.write(bytes("CREATED_BY", "utf8") + b"\x00" + bytes(cby, "utf8"))
+
     # write "container" extension length
     fOut.write(b"\x00\x80")
-    
+
     # write "container" extension
     for i in range(128):
         fOut.write(b"\x00")
-        
+
     # write end-of-extensions tag
     fOut.write(b"\x00\x00")
-    
+
     # write the iv used to encrypt the main iv and the
     # encryption key
     fOut.write(iv1)
-    
+
     # write encrypted main iv and key
     fOut.write(c_iv_key)
-    
+
     # write HMAC-SHA256 of the encrypted iv and key
     fOut.write(hmac1.finalize())
-    
+
     # encrypt file while reading it
     while True:
         # try to read bufferSize bytes
         fdata = fIn.read(bufferSize)
-        
+
         # get the real number of bytes read
         bytesRead = len(fdata)
-        
+
         # check if EOF was reached
         if bytesRead < bufferSize:
             # file size mod 16, lsb positions
             fs16 = bytes([bytesRead % AESBlockSize])
             # pad data (this is NOT PKCS#7!)
             # ...unless no bytes or a multiple of a block size
             # of bytes was read
             if bytesRead % AESBlockSize == 0:
                 padLen = 0
             else:
                 padLen = 16 - bytesRead % AESBlockSize
-            fdata += bytes([padLen])*padLen
+            fdata += bytes([padLen]) * padLen
             # encrypt data
-            cText = encryptor0.update(fdata) \
-                    + encryptor0.finalize()
+            cText = encryptor0.update(fdata) + encryptor0.finalize()
             # update HMAC
             hmac0.update(cText)
             # write encrypted file content
             fOut.write(cText)
             # break
             break
         # ...otherwise a full bufferSize was read
         else:
             # encrypt data
-            cText = encryptor0.update(fdata)                                
+            cText = encryptor0.update(fdata)
             # update HMAC
             hmac0.update(cText)
             # write encrypted file content
             fOut.write(cText)
-    
+
     # write plaintext file size mod 16 lsb positions
     fOut.write(fs16)
-    
+
     # write HMAC-SHA256 of the encrypted file
     fOut.write(hmac0.finalize())
 
+
 # decrypt file function
 # arguments:
 # infile: ciphertext file path
 # outfile: plaintext file path
 # passw: encryption password
 # bufferSize: optional buffer size, must be a multiple of AES block size (16)
 #             using a larger buffer speeds up things when dealing with
 #             big files
 #             Default is 64KB.
-def decryptFile(infile, outfile, passw, bufferSize = bufferSizeDef):
+def decryptFile(infile, outfile, passw, bufferSize=bufferSizeDef):
     try:
         with open(infile, "rb") as fIn:
             # check that output file does not exist
             # or that, if exists, is not the same as the input file
             # (i.e.: overwrite if it seems safe)
             if path.isfile(outfile):
                 if path.samefile(infile, outfile):
-                    raise ValueError("Input and output files "
-                                     "are the same.")
+                    raise ValueError("Input and output files are the same.")
             try:
                 with open(outfile, "wb") as fOut:
-                    # get input file size
-                    inputFileSize = stat(infile).st_size
                     try:
                         # decrypt file stream
-                        decryptStream(fIn, fOut, passw, bufferSize,
-                                      inputFileSize)
+                        decryptStream(fIn, fOut, passw, bufferSize)
                     except ValueError as exd:
                         # should not remove output file here because it is still in use
                         # re-raise exception
                         raise ValueError(str(exd))
-            
+
             except IOError:
                 raise ValueError("Unable to write output file.")
             except ValueError as exd:
                 # remove output file on error
                 remove(outfile)
                 # re-raise exception
                 raise ValueError(str(exd))
-                
+
     except IOError:
         raise ValueError("Unable to read input file.")
-                    
+
 
 # decrypt stream function
 # arguments:
 # fIn: input binary stream
 # fOut: output binary stream
 # passw: encryption password
 # bufferSize: decryption buffer size, must be a multiple of AES block size (16)
 #             using a larger buffer speeds up things when dealing with
 #             long streams
-# inputLength: input stream length
-def decryptStream(fIn, fOut, passw, bufferSize, inputLength):
+# inputLength: input stream length (DEPRECATED)
+def decryptStream(fIn, fOut, passw, bufferSize=bufferSizeDef, inputLength=None):
+    if inputLength is not None:
+        warnings.warn(
+            "inputLength parameter is no longer used, and might be removed in a future version",
+            DeprecationWarning,
+            stacklevel=2,
+        )
     # validate bufferSize
     if bufferSize % AESBlockSize != 0:
         raise ValueError("Buffer size must be a multiple of AES block size")
-    
+
     if len(passw) > maxPassLen:
         raise ValueError("Password is too long.")
 
+    if not hasattr(fIn, "peek"):
+        fIn = io.BufferedReader(fIn, bufferSize)
+
     fdata = fIn.read(3)
     # check if file is in AES Crypt format (also min length check)
-    if (fdata != bytes("AES", "utf8") or inputLength < 136):
-            raise ValueError("File is corrupted or not an AES Crypt "
-                             "(or pyAesCrypt) file.")
-        
+    if fdata != b"AES":
+        raise ValueError("File is corrupted or not an AES Crypt (or pyAesCrypt) file.")
+
     # check if file is in AES Crypt format, version 2
     # (the only one compatible with pyAesCrypt)
     fdata = fIn.read(1)
     if len(fdata) != 1:
         raise ValueError("File is corrupted.")
-    
+
     if fdata != b"\x02":
-        raise ValueError("pyAesCrypt is only compatible with version "
-                         "2 of the AES Crypt file format.")
-    
+        raise ValueError(
+            "pyAesCrypt is only compatible with version "
+            "2 of the AES Crypt file format."
+        )
+
     # skip reserved byte
     fIn.read(1)
-    
+
     # skip all the extensions
     while True:
         fdata = fIn.read(2)
         if len(fdata) != 2:
             raise ValueError("File is corrupted.")
         if fdata == b"\x00\x00":
             break
         fIn.read(int.from_bytes(fdata, byteorder="big"))
-        
+
     # read external iv
     iv1 = fIn.read(16)
     if len(iv1) != 16:
         raise ValueError("File is corrupted.")
-    
+
     # stretch password and iv
     key = stretch(passw, iv1)
-    
+
     # read encrypted main iv and key
     c_iv_key = fIn.read(48)
     if len(c_iv_key) != 48:
         raise ValueError("File is corrupted.")
-        
+
     # read HMAC-SHA256 of the encrypted iv and key
     hmac1 = fIn.read(32)
     if len(hmac1) != 32:
         raise ValueError("File is corrupted.")
-    
+
     # compute actual HMAC-SHA256 of the encrypted iv and key
-    hmac1Act = hmac.HMAC(key, hashes.SHA256(),
-                         backend=default_backend())
+    hmac1Act = hmac.HMAC(key, hashes.SHA256(), backend=default_backend())
     hmac1Act.update(c_iv_key)
-    
+
     # HMAC check
     if hmac1 != hmac1Act.finalize():
         raise ValueError("Wrong password (or file is corrupted).")
-    
+
     # instantiate AES cipher
-    cipher1 = Cipher(algorithms.AES(key), modes.CBC(iv1),
-                     backend=default_backend())
+    cipher1 = Cipher(algorithms.AES(key), modes.CBC(iv1), backend=default_backend())
     decryptor1 = cipher1.decryptor()
-    
+
     # decrypt main iv and key
     iv_key = decryptor1.update(c_iv_key) + decryptor1.finalize()
-    
+
     # get internal iv and key
     iv0 = iv_key[:16]
     intKey = iv_key[16:]
-    
+
     # instantiate another AES cipher
-    cipher0 = Cipher(algorithms.AES(intKey), modes.CBC(iv0),
-                     backend=default_backend())
+    cipher0 = Cipher(algorithms.AES(intKey), modes.CBC(iv0), backend=default_backend())
     decryptor0 = cipher0.decryptor()
-    
+
     # instantiate actual HMAC-SHA256 of the ciphertext
-    hmac0Act = hmac.HMAC(intKey, hashes.SHA256(),
-                         backend=default_backend())
+    hmac0Act = hmac.HMAC(intKey, hashes.SHA256(), backend=default_backend())
 
     # decrypt ciphertext, until last block is reached
-    while fIn.tell() < inputLength - 32 - 1 - AESBlockSize:
+    last_block_reached = False
+    while not last_block_reached:
         # read data
-        cText = fIn.read(
-            min(
-                bufferSize,
-                inputLength - fIn.tell() - 32 - 1 - AESBlockSize
-            )
-        )
+        cText = fIn.read(bufferSize)
+
+        # end of buffer
+        if len(fIn.peek(32 + 1)) < 32 + 1:
+            last_block_reached = True
+            cText += fIn.read()
+            fs16 = cText[-32 - 1]  # plaintext file size mod 16 lsb positions
+            hmac0 = cText[-32:]
+            cText = cText[: -32 - 1]
+
         # update HMAC
         hmac0Act.update(cText)
         # decrypt data and write it to output file
-        fOut.write(decryptor0.update(cText))
-        
-    # last block reached, remove padding if needed
-    
-    # read last block
-    
-    # this is for empty files
-    if fIn.tell() != inputLength - 32 - 1:
-        cText = fIn.read(AESBlockSize)
-        if len(cText) < AESBlockSize:
-            raise ValueError("File is corrupted.")
-    else:
-        cText = bytes()
-    
-    # update HMAC
-    hmac0Act.update(cText)
-    
-    # read plaintext file size mod 16 lsb positions
-    fs16 = fIn.read(1)
-    if len(fs16) != 1:
-        raise ValueError("File is corrupted.")
-    
-    # decrypt last block
-    pText = decryptor0.update(cText) + decryptor0.finalize()
-    
-    # remove padding
-    toremove = ((16 - fs16[0]) % 16)
-    if toremove != 0:
-        pText = pText[:-toremove]
-        
-    # write decrypted data to output file
-    fOut.write(pText)
-    
-    # read HMAC-SHA256 of the encrypted file
-    hmac0 = fIn.read(32)
-    if len(hmac0) != 32:
-        raise ValueError("File is corrupted.")
-    
+        pText = decryptor0.update(cText)
+
+        # remove padding
+        if last_block_reached:
+            toremove = (16 - fs16) % 16
+            if toremove:
+                pText = pText[:-toremove]
+
+        fOut.write(pText)
+
     # HMAC check
     if hmac0 != hmac0Act.finalize():
-        raise ValueError("Bad HMAC (file is corrupted).")   
+        raise ValueError("Bad HMAC (file is corrupted).")
```

### Comparing `pyAesCrypt-6.0.0/pyAesCrypt/test_crypto.py` & `pyAesCrypt-6.1.0/pyAesCrypt/test_crypto.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,16 +182,16 @@
         # delete test files
         os.remove(filenames[4])
         os.remove(encfilenames[4])
         os.remove(decfilenames[4])
         # delete directory for test files
         os.rmdir(tfdirname)
     
-    # quick test for binary stream functions
-    def test_bs_quick(self):
+    # quick test for binary stream functions - deprecated version with stream size
+    def test_bs_quick_deprecated(self):
         # encrypt
         with open(filenames[4], "rb") as fIn:
             with open(encfilenames[4], "wb") as fOut:
                 pyAesCrypt.encryptStream(fIn, fOut, password, bufferSize)
         
         # get encrypted file size
         encFileSize = os.stat(encfilenames[4]).st_size
@@ -202,14 +202,34 @@
                 # decrypt file stream
                 pyAesCrypt.decryptStream(fIn, fOut, password, bufferSize,
                                          encFileSize)
 
         # check that the original file and the output file are equal
         self.assertTrue(filecmp.cmp(filenames[4], decfilenames[4]))
 
+    # quick test for binary stream functions
+    def test_bs_quick(self):
+        # encrypt
+        with open(filenames[4], "rb") as fIn:
+            with open(encfilenames[4], "wb") as fOut:
+                pyAesCrypt.encryptStream(fIn, fOut, password, bufferSize)
+        
+        # get encrypted file size
+        encFileSize = os.stat(encfilenames[4]).st_size
+        
+        # decrypt
+        with open(encfilenames[4], "rb") as fIn:
+            with open(decfilenames[4], "wb") as fOut:
+                # decrypt file stream
+                pyAesCrypt.decryptStream(fIn, fOut, password, bufferSize)
+
+        # check that the original file and the output file are equal
+        self.assertTrue(filecmp.cmp(filenames[4], decfilenames[4]))
+
+
 
 # test exceptions
 class TestExceptions(unittest.TestCase):
     
     # test file path
     tfile = prefix + 'test.txt'
     
@@ -324,15 +344,16 @@
         
         # truncate hmac (i.e.: truncate end of the file)
         with open(self.tfile+'.aes', 'r+b') as ftc:
             ftc.truncate(fsize-1)
         
         # try to decrypt file
         # ...and check that ValueError is raised
-        self.assertRaisesRegex(ValueError, "File is corrupted.",
+        self.assertRaisesRegex(ValueError, ("Bad HMAC "
+                                                "\(file is corrupted\)."),
                                pyAesCrypt.decryptFile, self.tfile + '.aes',
                                self.tfile + '.decr', password, bufferSize)
                                
         # check that decrypted file was deleted
         self.assertFalse(isfile(self.tfile + '.decr'))
     
     # test same input and output file - encryption
```

### Comparing `pyAesCrypt-6.0.0/pyAesCrypt.egg-info/PKG-INFO` & `pyAesCrypt-6.1.0/pyAesCrypt.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,162 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyAesCrypt
-Version: 6.0.0
+Version: 6.1.0
 Summary: Encrypt and decrypt files and streams in AES Crypt format (version 2)
 Home-page: https://github.com/marcobellaccini/pyAesCrypt
 Author: Marco Bellaccini
-Author-email: UNKNOWN
 License: Apache License 2.0
-Description: pyAesCrypt
-        ===============
-        .. image:: https://travis-ci.com/marcobellaccini/pyAesCrypt.svg?branch=master
-            :target: https://travis-ci.com/marcobellaccini/pyAesCrypt
-        .. image:: https://pepy.tech/badge/pyaescrypt
-            :target: https://pepy.tech/project/pyaescrypt
-        
-        About pyAesCrypt
-        --------------------------
-        pyAesCrypt is a Python 3 file-encryption module and script that uses AES256-CBC to encrypt/decrypt files and binary streams.
-        
-        pyAesCrypt is compatible with the `AES Crypt`_ `file format`_ (version 2).
-        
-        It is Free Software, released under the `Apache License, Version 2.0`_.
-        
-        pyAesCrypt is brought to you by Marco Bellaccini - marco.bellaccini(at!)gmail.com.
-         
-        IMPORTANT SECURITY NOTE: version 2 of the AES Crypt file format does not authenticate the "file size modulo 16" byte. This implies that an attacker  
-        with write access to the encrypted file may alter the corresponding plaintext file size by up to 15 bytes.
-        
-        NOTE: there is no low-level memory management in Python, hence it is not possible to wipe memory areas were sensitive information was stored.
-        
-        Module usage example
-        ------------------------
-        Here is an example showing encryption and decryption of a file:
-        
-        .. code:: python
-        
-            import pyAesCrypt
-            password = "please-use-a-long-and-random-password"
-            # encrypt
-            pyAesCrypt.encryptFile("data.txt", "data.txt.aes", password)
-            # decrypt
-            pyAesCrypt.decryptFile("data.txt.aes", "dataout.txt", password)
-        
-        **This is the most straightforward way to use pyAesCrypt, and should be preferred.**
-        
-        If you need to specify a custom buffer size (default is 64KB), you can pass it as an optional argument:
-        
-        .. code:: python
-        
-            import pyAesCrypt
-            # custom encryption/decryption buffer size (default is 64KB)
-            bufferSize = 128 * 1024
-            password = "please-use-a-long-and-random-password"
-            # encrypt
-            pyAesCrypt.encryptFile("data.txt", "data.txt.aes", password, bufferSize)
-            # decrypt
-            pyAesCrypt.decryptFile("data.txt.aes", "dataout.txt", password, bufferSize)
-        
-        In case you need it, you can work with binary streams too:
-        
-        .. code:: python
-        
-            import pyAesCrypt
-            from os import stat, remove
-            # encryption/decryption buffer size - 64K
-            # with stream-oriented functions, setting buffer size is mandatory
-            bufferSize = 64 * 1024
-            password = "please-use-a-long-and-random-password"
-            
-            # encrypt
-            with open("data.txt", "rb") as fIn:
-                with open("data.txt.aes", "wb") as fOut:
-                    pyAesCrypt.encryptStream(fIn, fOut, password, bufferSize)
-            
-            # get encrypted file size
-            encFileSize = stat("data.txt.aes").st_size
-            
-            # decrypt
-            with open("data.txt.aes", "rb") as fIn:
-                try:
-                    with open("dataout.txt", "wb") as fOut:
-                        # decrypt file stream
-                        pyAesCrypt.decryptStream(fIn, fOut, password, bufferSize, encFileSize)
-                except ValueError:
-                    # remove output file on error
-                    remove("dataout.txt")
-        
-        you can also perform in-memory encryption/decryption (using BytesIO):
-        
-        .. code:: python
-        
-            import pyAesCrypt
-            import io
-            
-            bufferSize = 64 * 1024
-            password = "please-use-a-long-and-random-password"
-            
-            # binary data to be encrypted
-            pbdata = b"This is binary plaintext \x00\x01"
-            
-            # input plaintext binary stream
-            fIn = io.BytesIO(pbdata)
-            
-            # initialize ciphertext binary stream
-            fCiph = io.BytesIO()
-            
-            # initialize decrypted binary stream
-            fDec = io.BytesIO()
-            
-            # encrypt stream
-            pyAesCrypt.encryptStream(fIn, fCiph, password, bufferSize)
-            
-            # print encrypted data
-            print("This is the ciphertext:\n" + str(fCiph.getvalue()))
-            
-            # get ciphertext length
-            ctlen = len(fCiph.getvalue())
-            
-            # go back to the start of the ciphertext stream
-            fCiph.seek(0)
-            
-            # decrypt stream
-            pyAesCrypt.decryptStream(fCiph, fDec, password, bufferSize, ctlen)
-            
-            # print decrypted data
-            print("Decrypted data:\n" + str(fDec.getvalue()))
-        
-        
-        
-        Script usage examples
-        ------------------------
-        Encrypt file test.txt in test.txt.aes:
-        
-        	pyAesCrypt -e test.txt
-        
-        Decrypt file test.txt.aes in test.txt:
-        
-        	pyAesCrypt -d test.txt.aes
-        	
-        Encrypt file test.txt in test2.txt.aes:
-        
-        	pyAesCrypt -e test.txt -o test2.txt.aes
-        
-        Decrypt file test.txt.aes in test2.txt:
-        
-        	pyAesCrypt -d test.txt.aes -o test2.txt
-        
-        FAQs
-        ------------------------
-        - *Is pyAesCrypt malware?*
-        
-          **NO!** Of course it isn't!
-        
-          Nevertheless, being a module, it can be used by any other software, including malware.
-          
-          In fact, it has been reported that it is used as crypto library by some ransomware.
-        
-        .. _AES Crypt: https://www.aescrypt.com
-        .. _file format: https://www.aescrypt.com/aes_file_format.html
-        .. _Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
-        
 Keywords: AES Crypt encrypt decrypt
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+pyAesCrypt
+===============
+.. image:: https://github.com/marcobellaccini/pyaescrypt/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/marcobellaccini/pyAesCrypt/actions
+.. image:: https://pepy.tech/badge/pyaescrypt
+    :target: https://pepy.tech/project/pyaescrypt
+
+About pyAesCrypt
+--------------------------
+pyAesCrypt is a Python 3 file-encryption module and script that uses AES256-CBC to encrypt/decrypt files and binary streams.
+
+pyAesCrypt is compatible with the `AES Crypt`_ `file format`_ (version 2).
+
+It is Free Software, released under the `Apache License, Version 2.0`_.
+
+pyAesCrypt is brought to you by Marco Bellaccini - marco.bellaccini(at!)gmail.com.
+ 
+IMPORTANT SECURITY NOTE: version 2 of the AES Crypt file format does not authenticate the "file size modulo 16" byte. This implies that an attacker  
+with write access to the encrypted file may alter the corresponding plaintext file size by up to 15 bytes.
+
+NOTE: there is no low-level memory management in Python, hence it is not possible to wipe memory areas were sensitive information was stored.
+
+Module usage example
+------------------------
+Here is an example showing encryption and decryption of a file:
+
+.. code:: python
+
+    import pyAesCrypt
+    password = "please-use-a-long-and-random-password"
+    # encrypt
+    pyAesCrypt.encryptFile("data.txt", "data.txt.aes", password)
+    # decrypt
+    pyAesCrypt.decryptFile("data.txt.aes", "dataout.txt", password)
+
+**This is the most straightforward way to use pyAesCrypt, and should be preferred.**
+
+If you need to specify a custom buffer size (default is 64KB), you can pass it as an optional argument:
+
+.. code:: python
+
+    import pyAesCrypt
+    # custom encryption/decryption buffer size (default is 64KB)
+    bufferSize = 128 * 1024
+    password = "please-use-a-long-and-random-password"
+    # encrypt
+    pyAesCrypt.encryptFile("data.txt", "data.txt.aes", password, bufferSize)
+    # decrypt
+    pyAesCrypt.decryptFile("data.txt.aes", "dataout.txt", password, bufferSize)
+
+In case you need it, you can work with binary streams too:
+
+.. code:: python
+
+    import pyAesCrypt
+    from os import stat, remove
+    # encryption/decryption buffer size - 64K
+    # with stream-oriented functions, setting buffer size is mandatory
+    bufferSize = 64 * 1024
+    password = "please-use-a-long-and-random-password"
+    
+    # encrypt
+    with open("data.txt", "rb") as fIn:
+        with open("data.txt.aes", "wb") as fOut:
+            pyAesCrypt.encryptStream(fIn, fOut, password, bufferSize)
+    
+    # decrypt
+    with open("data.txt.aes", "rb") as fIn:
+        try:
+            with open("dataout.txt", "wb") as fOut:
+                # decrypt file stream
+                pyAesCrypt.decryptStream(fIn, fOut, password, bufferSize)
+        except ValueError:
+            # remove output file on error
+            remove("dataout.txt")
+
+you can also perform in-memory encryption/decryption (using BytesIO):
+
+.. code:: python
+
+    import pyAesCrypt
+    import io
+    
+    bufferSize = 64 * 1024
+    password = "please-use-a-long-and-random-password"
+    
+    # binary data to be encrypted
+    pbdata = b"This is binary plaintext \x00\x01"
+    
+    # input plaintext binary stream
+    fIn = io.BytesIO(pbdata)
+    
+    # initialize ciphertext binary stream
+    fCiph = io.BytesIO()
+    
+    # initialize decrypted binary stream
+    fDec = io.BytesIO()
+    
+    # encrypt stream
+    pyAesCrypt.encryptStream(fIn, fCiph, password, bufferSize)
+    
+    # print encrypted data
+    print("This is the ciphertext:\n" + str(fCiph.getvalue()))
+    
+    # go back to the start of the ciphertext stream
+    fCiph.seek(0)
+    
+    # decrypt stream
+    pyAesCrypt.decryptStream(fCiph, fDec, password, bufferSize)
+    
+    # print decrypted data
+    print("Decrypted data:\n" + str(fDec.getvalue()))
+
+
+
+Script usage examples
+------------------------
+Encrypt file test.txt in test.txt.aes:
+
+	pyAesCrypt -e test.txt
+
+Decrypt file test.txt.aes in test.txt:
+
+	pyAesCrypt -d test.txt.aes
+	
+Encrypt file test.txt in test2.txt.aes:
+
+	pyAesCrypt -e test.txt -o test2.txt.aes
+
+Decrypt file test.txt.aes in test2.txt:
+
+	pyAesCrypt -d test.txt.aes -o test2.txt
+
+FAQs
+------------------------
+- *Is pyAesCrypt malware?*
+
+  **NO!** Of course it isn't!
+
+  Nevertheless, being a module, it can be used by any other software, including malware.
+  
+  In fact, it has been reported that it is used as crypto library by some ransomware.
+
+.. _AES Crypt: https://www.aescrypt.com
+.. _file format: https://www.aescrypt.com/aes_file_format.html
+.. _Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyAesCrypt-6.0.0/setup.py` & `pyAesCrypt-6.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
     README = readme.read()
 
 setup(name='pyAesCrypt',
-    version='6.0.0',
+    version='6.1.0',
     packages = find_packages(),
     include_package_data=True,
     description='Encrypt and decrypt files and streams in AES Crypt format (version 2)',
     long_description = README,
     author='Marco Bellaccini',
     url='https://github.com/marcobellaccini/pyAesCrypt',
     license='Apache License 2.0',
```

