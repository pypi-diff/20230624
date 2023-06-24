# Comparing `tmp/Kinho-1.0.0.tar.gz` & `tmp/Kinho-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kinho-1.0.0.tar", last modified: Sat Jun 24 05:08:47 2023, max compression
+gzip compressed data, was "Kinho-1.0.1.tar", last modified: Sat Jun 24 10:36:35 2023, max compression
```

## Comparing `Kinho-1.0.0.tar` & `Kinho-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 05:08:47.102654 Kinho-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-24 05:08:46.996767 Kinho-1.0.0/Kinho/
--rw-rw-rw-   0        0        0      117 2023-06-24 05:07:25.000000 Kinho-1.0.0/Kinho/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:08:47.023061 Kinho-1.0.0/Kinho/brain/
--rw-rw-rw-   0        0        0       58 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/__init__.py
--rw-rw-rw-   0        0        0     4355 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/builder.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:08:47.033062 Kinho-1.0.0/Kinho/brain/decoder/
--rw-rw-rw-   0        0        0       86 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/decoder/__init__.py
--rw-rw-rw-   0        0        0       76 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/decoder/d_float.py
--rw-rw-rw-   0        0        0       66 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/decoder/d_int.py
--rw-rw-rw-   0        0        0       52 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/decoder/d_string.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:08:47.045060 Kinho-1.0.0/Kinho/brain/encoder/
--rw-rw-rw-   0        0        0      135 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/encoder/__init__.py
--rw-rw-rw-   0        0        0       73 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/encoder/e_float.py
--rw-rw-rw-   0        0        0       64 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/encoder/e_int.py
--rw-rw-rw-   0        0        0       54 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/encoder/e_string.py
--rw-rw-rw-   0        0        0      127 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/encoder/e_xor.py
--rw-rw-rw-   0        0        0     2414 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/brain/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:08:47.080638 Kinho-1.0.0/Kinho/kernel/
--rw-rw-rw-   0        0        0      347 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/__init__.py
--rw-rw-rw-   0        0        0      386 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/activation.py
--rw-rw-rw-   0        0        0      433 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/dactivation.py
--rw-rw-rw-   0        0        0      555 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/dlayer.py
--rw-rw-rw-   0        0        0      466 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/dloss.py
--rw-rw-rw-   0        0        0      596 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/dselector.py
--rw-rw-rw-   0        0        0      572 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/layer.py
--rw-rw-rw-   0        0        0      443 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/loss.py
--rw-rw-rw-   0        0        0      559 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/selector.py
--rw-rw-rw-   0        0        0      466 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/transpose.py
--rw-rw-rw-   0        0        0      481 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/updateWeights.py
--rw-rw-rw-   0        0        0      233 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/kernel/vars.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:08:47.082637 Kinho-1.0.0/Kinho/lib/
-drwxrwxrwx   0        0        0        0 2023-06-24 05:08:47.092602 Kinho-1.0.0/Kinho/lib/GPU/
--rw-rw-rw-   0        0        0      899 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/lib/GPU/CPU_version.py
--rw-rw-rw-   0        0        0     3509 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/lib/GPU/Function.py
--rw-rw-rw-   0        0        0       73 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/lib/GPU/__init__.py
--rw-rw-rw-   0        0        0     1650 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/lib/GPU/utils.py
--rw-rw-rw-   0        0        0       17 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/lib/__init__.py
--rw-rw-rw-   0        0        0    11697 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/neural.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:08:47.097670 Kinho-1.0.0/Kinho/transfer/
--rw-rw-rw-   0        0        0       26 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/transfer/__init__.py
--rw-rw-rw-   0        0        0      498 2023-06-23 19:27:21.000000 Kinho-1.0.0/Kinho/transfer/loader.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:08:47.014042 Kinho-1.0.0/Kinho.egg-info/
--rw-rw-rw-   0        0        0     1352 2023-06-24 05:08:46.000000 Kinho-1.0.0/Kinho.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2023-06-24 05:08:46.000000 Kinho-1.0.0/Kinho.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 05:08:46.000000 Kinho-1.0.0/Kinho.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-24 05:08:46.000000 Kinho-1.0.0/Kinho.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2022-11-07 19:10:33.000000 Kinho-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1352 2023-06-24 05:08:47.100632 Kinho-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5310 2023-06-23 19:27:21.000000 Kinho-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 05:08:47.103602 Kinho-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2030 2023-06-23 19:27:21.000000 Kinho-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.669499 Kinho-1.0.1/Kinho/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.669499 Kinho-1.0.1/Kinho/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.669499 Kinho-1.0.1/Kinho/brain/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/decoder/d_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/decoder/d_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/decoder/d_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.669499 Kinho-1.0.1/Kinho/brain/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/encoder/e_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/encoder/e_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/encoder/e_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/encoder/e_xor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/brain/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/Kinho/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/dactivation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/dlayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/dloss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/dselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/updateWeights.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/kernel/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/Kinho/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/Kinho/lib/GPU/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/lib/GPU/CPU_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/lib/GPU/Function.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/lib/GPU/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/lib/GPU/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/neural.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/Kinho/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-24 10:36:18.000000 Kinho-1.0.1/Kinho/transfer/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.669499 Kinho-1.0.1/Kinho.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-24 10:36:35.000000 Kinho-1.0.1/Kinho.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-24 10:36:35.000000 Kinho-1.0.1/Kinho.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:36:35.000000 Kinho-1.0.1/Kinho.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 10:36:35.000000 Kinho-1.0.1/Kinho.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 10:36:18.000000 Kinho-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-24 10:36:35.673499 Kinho-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-24 10:36:18.000000 Kinho-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 10:36:35.673499 Kinho-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-24 10:36:19.000000 Kinho-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:36:35.673499 Kinho-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-24 10:36:19.000000 Kinho-1.0.1/tests/test_learn_rate.py
```

### Comparing `Kinho-1.0.0/Kinho/brain/builder.py` & `Kinho-1.0.1/Kinho/brain/builder.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-import numpy as np
-from . import decoder, encoder
-
-MINIMUM_SIZE = 12
-SIGNATURE_SIZE = 7
-INT_SIZE = 4
-LAYER_HEADER_SIZE = 9
-FLOAT_SIZE = 8
-
-class Builder(object): 
-    def __init__(self, path):
-        self.__size = None
-        self.__architecture = []
-        self.__biases = []
-        self.__weights = []
-        self.__error = {
-            0: 'type `brain` has an invalid size',
-            1: 'type `brain` has not valid signature',
-            2: 'data is corrupted. The general security code not match',
-            3: 'layer header has no sufficient size',
-            4: 'layer target has no match',
-            5: 'weight has no sufficient size',
-            6: 'weitght target has no match',
-            7: 'biase has no sufficient size',
-            8: 'biase target has no match',
-            9: 'layers are not connect, shapes should be (x, y), (y, z)',
-        }
-        
-        data = self.__read(path)
-        self.__build(data)
-    
-    def __read(self, path):
-        data = b''
-        with open(path, 'rb') as file:
-            data = file.read()
-        
-        return data
-    
-    def __build(self, data):
-        if len(data) < MINIMUM_SIZE:
-            self.__raise(0)
-        
-        magic_number = decoder.toInt(encoder.securityCode(data[0:-1]))
-        if magic_number != data[-1]:
-            self.__raise(2)
-        
-        prefix = 0
-        signature = decoder.toString(data[prefix:prefix+SIGNATURE_SIZE])
-        if signature != 'kinhosz':
-            self.__raise(1)
-        
-        prefix += SIGNATURE_SIZE
-        
-        self.__size = decoder.toInt(data[prefix:prefix + INT_SIZE])
-        prefix += INT_SIZE
-        
-        for _ in range(1, self.__size):
-            prefix = self.__buildLayer(data, prefix)
-        
-        for i in range(1, self.__size - 1):
-            if self.__weights[i].shape[0] != self.__weights[i-1].shape[1]:
-                self.__raise(9)
-        
-        for i in range(self.__size - 1):
-            self.__architecture.append(self.__weights[i].shape[0])
-        self.__architecture.append(self.__weights[-1].shape[1])
-    
-    def __buildLayer(self, data, offset):
-        if len(data) < offset + LAYER_HEADER_SIZE:
-            self.__raise(3)
-        
-        target = chr(data[offset])
-        if target != 'L':
-            self.__raise(4)
-        
-        offset += 1
-        
-        dim1 = decoder.toInt(data[offset:offset+INT_SIZE])
-        offset += INT_SIZE
-        dim2 = decoder.toInt(data[offset:offset+INT_SIZE])
-        offset +=  INT_SIZE
-        
-        offset = self.__buildWeight(data, dim1, dim2, offset)
-        offset = self.__buildBiase(data, dim2, offset)
-        
-        return offset
-    
-    def __buildWeight(self, data, dim1, dim2, offset):
-        REQUIRED_LEN = offset + FLOAT_SIZE * (dim1 * dim2) + 1
-        
-        if len(data) < REQUIRED_LEN:
-            self.__raise(5)
-        
-        target = chr(data[offset])
-        if target != 'W':
-            self.__raise(6)
-        
-        offset += 1
-        
-        weight = np.empty((dim1, dim2))
-        
-        for i in range(dim1):
-            for j in range(dim2):
-                weight[i, j] = decoder.toFloat(data[offset:offset+FLOAT_SIZE])
-                offset += FLOAT_SIZE
-        
-        self.__weights.append(weight)
-        
-        return offset
-    
-    def __buildBiase(self, data, dim, offset):
-        REQUIRED_LEN = offset + FLOAT_SIZE * dim + 1
-        
-        if len(data) < REQUIRED_LEN:
-            self.__raise(7)
-        
-        target = chr(data[offset])
-        if target != 'B':
-            self.__raise(8)
-        
-        offset += 1
-        
-        biase = np.empty((1, dim))
-        
-        for i in range(dim):
-            biase[0, i] = decoder.toFloat(data[offset:offset+FLOAT_SIZE])
-            offset += FLOAT_SIZE
-        
-        self.__biases.append(biase)
-        
-        return offset
-    
-    def __raise(self, flag):
-        raise TypeError(self.__error[flag])
-    
-    def size(self):
-        return self.__size
-    
-    def architecture(self):
-        return self.__architecture
-    
-    def biases(self):
-        return self.__biases
-    
-    def weights(self):
+import numpy as np
+from . import decoder, encoder
+
+MINIMUM_SIZE = 12
+SIGNATURE_SIZE = 7
+INT_SIZE = 4
+LAYER_HEADER_SIZE = 9
+FLOAT_SIZE = 8
+
+class Builder(object): 
+    def __init__(self, path):
+        self.__size = None
+        self.__architecture = []
+        self.__biases = []
+        self.__weights = []
+        self.__error = {
+            0: 'type `brain` has an invalid size',
+            1: 'type `brain` has not valid signature',
+            2: 'data is corrupted. The general security code not match',
+            3: 'layer header has no sufficient size',
+            4: 'layer target has no match',
+            5: 'weight has no sufficient size',
+            6: 'weitght target has no match',
+            7: 'biase has no sufficient size',
+            8: 'biase target has no match',
+            9: 'layers are not connect, shapes should be (x, y), (y, z)',
+        }
+        
+        data = self.__read(path)
+        self.__build(data)
+    
+    def __read(self, path):
+        data = b''
+        with open(path, 'rb') as file:
+            data = file.read()
+        
+        return data
+    
+    def __build(self, data):
+        if len(data) < MINIMUM_SIZE:
+            self.__raise(0)
+        
+        magic_number = decoder.toInt(encoder.securityCode(data[0:-1]))
+        if magic_number != data[-1]:
+            self.__raise(2)
+        
+        prefix = 0
+        signature = decoder.toString(data[prefix:prefix+SIGNATURE_SIZE])
+        if signature != 'kinhosz':
+            self.__raise(1)
+        
+        prefix += SIGNATURE_SIZE
+        
+        self.__size = decoder.toInt(data[prefix:prefix + INT_SIZE])
+        prefix += INT_SIZE
+        
+        for _ in range(1, self.__size):
+            prefix = self.__buildLayer(data, prefix)
+        
+        for i in range(1, self.__size - 1):
+            if self.__weights[i].shape[0] != self.__weights[i-1].shape[1]:
+                self.__raise(9)
+        
+        for i in range(self.__size - 1):
+            self.__architecture.append(self.__weights[i].shape[0])
+        self.__architecture.append(self.__weights[-1].shape[1])
+    
+    def __buildLayer(self, data, offset):
+        if len(data) < offset + LAYER_HEADER_SIZE:
+            self.__raise(3)
+        
+        target = chr(data[offset])
+        if target != 'L':
+            self.__raise(4)
+        
+        offset += 1
+        
+        dim1 = decoder.toInt(data[offset:offset+INT_SIZE])
+        offset += INT_SIZE
+        dim2 = decoder.toInt(data[offset:offset+INT_SIZE])
+        offset +=  INT_SIZE
+        
+        offset = self.__buildWeight(data, dim1, dim2, offset)
+        offset = self.__buildBiase(data, dim2, offset)
+        
+        return offset
+    
+    def __buildWeight(self, data, dim1, dim2, offset):
+        REQUIRED_LEN = offset + FLOAT_SIZE * (dim1 * dim2) + 1
+        
+        if len(data) < REQUIRED_LEN:
+            self.__raise(5)
+        
+        target = chr(data[offset])
+        if target != 'W':
+            self.__raise(6)
+        
+        offset += 1
+        
+        weight = np.empty((dim1, dim2))
+        
+        for i in range(dim1):
+            for j in range(dim2):
+                weight[i, j] = decoder.toFloat(data[offset:offset+FLOAT_SIZE])
+                offset += FLOAT_SIZE
+        
+        self.__weights.append(weight)
+        
+        return offset
+    
+    def __buildBiase(self, data, dim, offset):
+        REQUIRED_LEN = offset + FLOAT_SIZE * dim + 1
+        
+        if len(data) < REQUIRED_LEN:
+            self.__raise(7)
+        
+        target = chr(data[offset])
+        if target != 'B':
+            self.__raise(8)
+        
+        offset += 1
+        
+        biase = np.empty((1, dim))
+        
+        for i in range(dim):
+            biase[0, i] = decoder.toFloat(data[offset:offset+FLOAT_SIZE])
+            offset += FLOAT_SIZE
+        
+        self.__biases.append(biase)
+        
+        return offset
+    
+    def __raise(self, flag):
+        raise TypeError(self.__error[flag])
+    
+    def size(self):
+        return self.__size
+    
+    def architecture(self):
+        return self.__architecture
+    
+    def biases(self):
+        return self.__biases
+    
+    def weights(self):
         return self.__weights
```

### Comparing `Kinho-1.0.0/Kinho/brain/wrapper.py` & `Kinho-1.0.1/Kinho/brain/wrapper.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from . import encoder
-
-class Wrapper(object):
-    def __init__(self, layers):
-        self.__data = b''
-        self.__error = {
-            0: 'weight has shape different of (x, y)',
-            1: 'biase has shape different of (1, x)',
-            2: 'weight has second dimension different of biase. Should be: (x, y), (1, y)',
-            3: 'values in weight are not float',
-            4: 'values in biase are not float',
-            5: 'layers dimensions are not connected. Should be: (x, y), (y, z)',
-        }
-        
-        self.__checkType(layers)
-        self.__buildData(layers)
-    
-    def __raise(self, flag):
-        raise TypeError(self.__error[flag])
-    
-    def __checkType(self, layers):
-        for w, b in layers:
-            if len(w.shape) != 2:
-                self.__raise(0)
-            if len(b.shape) != 2:
-                self.__raise(1)
-            
-            if w.shape[1] != b.shape[1]:
-                self.__raise(2)
-            
-            for w_x in w:
-                for w_x_y in w_x:
-                    if not isinstance(w_x_y, float):
-                        self.__raise(3)
-            
-            for b_x in b[0]:
-                if not isinstance(b_x, float):
-                    self.__raise(4)
-        
-        for i in range(1, len(layers)):
-            if layers[i][0].shape[0] != layers[i-1][0].shape[1]:
-                self.__raise(5)
-    
-    def __buildData(self, layers):
-        header = b''
-        header += encoder.fromString('kinhosz')
-        header += encoder.fromInt(len(layers) + 1)
-        
-        body = b''
-        
-        for w, b in layers:
-            layer = b''
-            layer += encoder.fromString('L')
-            layer += encoder.fromInt(w.shape[0])
-            layer += encoder.fromInt(w.shape[1])
-
-            layer += encoder.fromString('W')
-            for w_x in w:
-                for w_x_y in w_x:
-                    layer += encoder.fromFloat(w_x_y)
-            
-            layer += encoder.fromString('B')
-            for b_x in b[0]:
-                layer += encoder.fromFloat(b_x)
-            
-            body += layer
-        
-        data = header + body
-        
-        security_code = encoder.securityCode(data)
-        
-        data += security_code
-        self.__data = data
-    
-    def data(self):
-        return self.__data
-
+from . import encoder
+
+class Wrapper(object):
+    def __init__(self, layers):
+        self.__data = b''
+        self.__error = {
+            0: 'weight has shape different of (x, y)',
+            1: 'biase has shape different of (1, x)',
+            2: 'weight has second dimension different of biase. Should be: (x, y), (1, y)',
+            3: 'values in weight are not float',
+            4: 'values in biase are not float',
+            5: 'layers dimensions are not connected. Should be: (x, y), (y, z)',
+        }
+        
+        self.__checkType(layers)
+        self.__buildData(layers)
+    
+    def __raise(self, flag):
+        raise TypeError(self.__error[flag])
+    
+    def __checkType(self, layers):
+        for w, b in layers:
+            if len(w.shape) != 2:
+                self.__raise(0)
+            if len(b.shape) != 2:
+                self.__raise(1)
+            
+            if w.shape[1] != b.shape[1]:
+                self.__raise(2)
+            
+            for w_x in w:
+                for w_x_y in w_x:
+                    if not isinstance(w_x_y, float):
+                        self.__raise(3)
+            
+            for b_x in b[0]:
+                if not isinstance(b_x, float):
+                    self.__raise(4)
+        
+        for i in range(1, len(layers)):
+            if layers[i][0].shape[0] != layers[i-1][0].shape[1]:
+                self.__raise(5)
+    
+    def __buildData(self, layers):
+        header = b''
+        header += encoder.fromString('kinhosz')
+        header += encoder.fromInt(len(layers) + 1)
+        
+        body = b''
+        
+        for w, b in layers:
+            layer = b''
+            layer += encoder.fromString('L')
+            layer += encoder.fromInt(w.shape[0])
+            layer += encoder.fromInt(w.shape[1])
+
+            layer += encoder.fromString('W')
+            for w_x in w:
+                for w_x_y in w_x:
+                    layer += encoder.fromFloat(w_x_y)
+            
+            layer += encoder.fromString('B')
+            for b_x in b[0]:
+                layer += encoder.fromFloat(b_x)
+            
+            body += layer
+        
+        data = header + body
+        
+        security_code = encoder.securityCode(data)
+        
+        data += security_code
+        self.__data = data
+    
+    def data(self):
+        return self.__data
+
```

### Comparing `Kinho-1.0.0/Kinho/kernel/dselector.py` & `Kinho-1.0.1/Kinho/kernel/dselector.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from numba import cuda
-from ..lib.GPU import *
-from timeit import default_timer as timer
-from .vars import add
-from ..transfer.loader import loadTo
-
-def dselector(z, alpha, buffer):
-    LEN = z.shape[1]
-
-    t = timer()
-    z_dvc, alpha_dvc, ss_dvc, st_dvc = loadTo(z, alpha, np.zeros(1), np.zeros(1), mode='GPU')
-    t = timer() - t
-    add(t)
-
-    softmax_sum_derivate[kernelConfig1D(LEN)](buffer, z_dvc, alpha_dvc, ss_dvc, st_dvc)
-    cuda.synchronize()
-    softmax_derivate[kernelConfig1D(LEN)](buffer, alpha_dvc, ss_dvc, st_dvc)
-    cuda.synchronize()
-
-    return buffer
+from numba import cuda
+from ..lib.GPU import *
+from timeit import default_timer as timer
+from .vars import add
+from ..transfer.loader import loadTo
+
+def dselector(z, alpha, buffer):
+    LEN = z.shape[1]
+
+    t = timer()
+    z_dvc, alpha_dvc, ss_dvc, st_dvc = loadTo(z, alpha, np.zeros(1), np.zeros(1), mode='GPU')
+    t = timer() - t
+    add(t)
+
+    softmax_sum_derivate[kernelConfig1D(LEN)](buffer, z_dvc, alpha_dvc, ss_dvc, st_dvc)
+    cuda.synchronize()
+    softmax_derivate[kernelConfig1D(LEN)](buffer, alpha_dvc, ss_dvc, st_dvc)
+    cuda.synchronize()
+
+    return buffer
```

### Comparing `Kinho-1.0.0/Kinho/kernel/selector.py` & `Kinho-1.0.1/Kinho/kernel/selector.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from numba import cuda
-from ..lib.GPU import *
-from timeit import default_timer as timer
-from .vars import add
-from ..transfer.loader import loadTo
-
-def selector(z, res, buffer):
-    LEN = z.shape[1]
-
-    t = timer()
-    z_dvc, res_dvc = loadTo(z, res, mode='GPU')
-    memset[kernelConfig1D(1)](res_dvc)
-    cuda.synchronize()
-    t = timer() - t
-    add(t)
-
-    softmax_p1[kernelConfig1D(LEN)](buffer, z_dvc, res_dvc)
-    cuda.synchronize()
-
-    softmax_p2[kernelConfig1D(LEN)](buffer, res_dvc)
-    cuda.synchronize()
-
+from numba import cuda
+from ..lib.GPU import *
+from timeit import default_timer as timer
+from .vars import add
+from ..transfer.loader import loadTo
+
+def selector(z, res, buffer):
+    LEN = z.shape[1]
+
+    t = timer()
+    z_dvc, res_dvc = loadTo(z, res, mode='GPU')
+    memset[kernelConfig1D(1)](res_dvc)
+    cuda.synchronize()
+    t = timer() - t
+    add(t)
+
+    softmax_p1[kernelConfig1D(LEN)](buffer, z_dvc, res_dvc)
+    cuda.synchronize()
+
+    softmax_p2[kernelConfig1D(LEN)](buffer, res_dvc)
+    cuda.synchronize()
+
     return buffer
```

### Comparing `Kinho-1.0.0/Kinho/lib/GPU/Function.py` & `Kinho-1.0.1/Kinho/lib/GPU/Function.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-import math
-from numba import cuda, float64, float32, int64
-
-DIM1 = (1024, )
-DIM2 = (4, 256)
-
-@cuda.jit
-def copy(arr, A):
-	x = cuda.grid(1)
-
-	if x < arr.shape[1]:
-		arr[0, x] = A[0, x]
-
-@cuda.jit
-def memset(arr):
-	x = cuda.grid(1)
-
-	if x < arr.shape[0]:
-		arr[x] = float64(0.)
-
-@cuda.jit
-def memset2(arr):
-	x, y = cuda.grid(2)
-
-	if x < arr.shape[0] and y < arr.shape[1]:
-		arr[x, y] = float64(0.)
-
-@cuda.jit
-def mse(result, predicted, target):
-    pos = cuda.grid(1)
-
-    if pos < predicted.shape[0]:
-        diff = predicted[pos] - target[pos]
-        diff = (diff * diff) / 2.0
-        cuda.atomic.add(result, 0, diff)
-
-@cuda.jit
-def mse_derivate(result, predicted, target):
-    pos = cuda.grid(1)
-
-    if pos < predicted.shape[1]:
-        result[0, pos] = predicted[0, pos] - target[0, pos]
-
-@cuda.jit
-def softmax_p1(arr, z, res):
-	local_sum = cuda.shared.array(shape=DIM1, dtype=float64)
-
-	x = cuda.grid(1)
-	tx = cuda.threadIdx.x
-	local_sum[tx] = float64(.0)
-
-	if x >= arr.shape[1]:
-		return
-
-	val = math.exp(z[0, x])
-	arr[0, x] = val
-	local_sum[tx] = val
-	cuda.syncthreads()
-
-	if tx != 0:
-		return
-	
-	for i in range(1, cuda.blockDim.x):
-		local_sum[0] += local_sum[i]
-
-	cuda.atomic.add(res, 0, local_sum[0])
-
-@cuda.jit
-def softmax_p2(arr, sumT):
-	x = cuda.grid(1)
-
-	if x < arr.shape[1]:
-		arr[0, x] = arr[0, x] / sumT[0]
-
-@cuda.jit
-def softmax_sum_derivate(arr, z, alpha, simple_sum, sum_times_alpha):
-	x = cuda.grid(1)
-
-	if x < arr.shape[1]:
-		value = z[0, x]
-		value = math.exp(value)
-		arr[0, x] = value
-		cuda.atomic.add(simple_sum, 0, value)
-		cuda.atomic.add(sum_times_alpha, 0, value * alpha[0, x])
-
-@cuda.jit
-def softmax_derivate(arr, alpha, simple_sum, sum_times_alpha):
-	x = cuda.grid(1)
- 
-	if x < arr.shape[1]:
-		value = arr[0, x]
-		arr[0, x] = (value * (alpha[0, x] - (sum_times_alpha[0] / simple_sum[0]))) / simple_sum[0]
-
-@cuda.jit
-def sigmoid2(arr, A):
-	x = cuda.grid(1)
-
-	if x < arr.shape[1]:
-		arr[0, x] = 2.0 * (1.0 / (1.0 + math.exp(-A[0, x]))) - 1.0
-
-@cuda.jit
-def sigmoid2_derivate(arr, A, alpha):
-	x = cuda.grid(1)
-
-	if x < A.shape[1]:
-		value = A[0, x]
-		arr[0, x] = alpha[0, x] * (2.0 * math.exp(-value) / ( (1.0 + math.exp(-value)) * (1.0 + math.exp(-value))))
-
-@cuda.jit
-def sum(arr, C):
-	x, y = cuda.grid(2)
-
-	if x >= arr.shape[0] or y >= arr.shape[1]:
-		return
-
-	arr[x, y] += C[x, y]
-
-@cuda.jit
-def dotMatrix(arr, A, B):
-	x, y = cuda.grid(2)
-	
-	temp = cuda.shared.array(shape=DIM2, dtype=float64)
-	sA = cuda.shared.array(shape=(1, DIM2[0]), dtype=float64)
-
-	tx = cuda.threadIdx.x
-	ty = cuda.threadIdx.y
-	temp[tx, ty] = float64(.0)
-
-	if x >= B.shape[0] or y >= B.shape[1]:
-		return
-	
-	if ty == 0:
-		sA[0, tx] = A[0, x]
-	cuda.syncthreads()
-
-	temp[tx, ty] = sA[0, tx] * B[x, y]
-	cuda.syncthreads()
-
-	if tx != 0:
-		return
-	
-	for i in range(1, cuda.blockDim.x):
-		temp[0, ty] += temp[i, ty]
-	cuda.atomic.add(arr, (0, y), temp[0, ty])
-
-@cuda.jit
-def dotMatrix_derivate(arr, w, alpha):
-	x, y, z = cuda.grid(3)
-
-	if x >= arr.shape[0] or y >= arr.shape[1] or z >= alpha.shape[1]:
-		return
-
-	cuda.atomic.add(arr, (x, y), alpha[x, z] * w[y, z])
-
-@cuda.jit
-def transposeDot(arr, A, B):
-	x, y = cuda.grid(2)
-
-	if x < arr.shape[0] and y < arr.shape[1]:
-		arr[x, y] = A[0, x] * B[0, y]
-
-@cuda.jit
-def updateWeights(w, eta, nabla):
-	x, y = cuda.grid(2)
-
-	if x < w.shape[0] and y < w.shape[1]:
+import math
+from numba import cuda, float64, float32, int64
+
+DIM1 = (1024, )
+DIM2 = (4, 256)
+
+@cuda.jit
+def copy(arr, A):
+	x = cuda.grid(1)
+
+	if x < arr.shape[1]:
+		arr[0, x] = A[0, x]
+
+@cuda.jit
+def memset(arr):
+	x = cuda.grid(1)
+
+	if x < arr.shape[0]:
+		arr[x] = float64(0.)
+
+@cuda.jit
+def memset2(arr):
+	x, y = cuda.grid(2)
+
+	if x < arr.shape[0] and y < arr.shape[1]:
+		arr[x, y] = float64(0.)
+
+@cuda.jit
+def mse(result, predicted, target):
+    pos = cuda.grid(1)
+
+    if pos < predicted.shape[0]:
+        diff = predicted[pos] - target[pos]
+        diff = (diff * diff) / 2.0
+        cuda.atomic.add(result, 0, diff)
+
+@cuda.jit
+def mse_derivate(result, predicted, target):
+    pos = cuda.grid(1)
+
+    if pos < predicted.shape[1]:
+        result[0, pos] = predicted[0, pos] - target[0, pos]
+
+@cuda.jit
+def softmax_p1(arr, z, res):
+	local_sum = cuda.shared.array(shape=DIM1, dtype=float64)
+
+	x = cuda.grid(1)
+	tx = cuda.threadIdx.x
+	local_sum[tx] = float64(.0)
+
+	if x >= arr.shape[1]:
+		return
+
+	val = math.exp(z[0, x])
+	arr[0, x] = val
+	local_sum[tx] = val
+	cuda.syncthreads()
+
+	if tx != 0:
+		return
+	
+	for i in range(1, cuda.blockDim.x):
+		local_sum[0] += local_sum[i]
+
+	cuda.atomic.add(res, 0, local_sum[0])
+
+@cuda.jit
+def softmax_p2(arr, sumT):
+	x = cuda.grid(1)
+
+	if x < arr.shape[1]:
+		arr[0, x] = arr[0, x] / sumT[0]
+
+@cuda.jit
+def softmax_sum_derivate(arr, z, alpha, simple_sum, sum_times_alpha):
+	x = cuda.grid(1)
+
+	if x < arr.shape[1]:
+		value = z[0, x]
+		value = math.exp(value)
+		arr[0, x] = value
+		cuda.atomic.add(simple_sum, 0, value)
+		cuda.atomic.add(sum_times_alpha, 0, value * alpha[0, x])
+
+@cuda.jit
+def softmax_derivate(arr, alpha, simple_sum, sum_times_alpha):
+	x = cuda.grid(1)
+ 
+	if x < arr.shape[1]:
+		value = arr[0, x]
+		arr[0, x] = (value * (alpha[0, x] - (sum_times_alpha[0] / simple_sum[0]))) / simple_sum[0]
+
+@cuda.jit
+def sigmoid2(arr, A):
+	x = cuda.grid(1)
+
+	if x < arr.shape[1]:
+		arr[0, x] = 2.0 * (1.0 / (1.0 + math.exp(-A[0, x]))) - 1.0
+
+@cuda.jit
+def sigmoid2_derivate(arr, A, alpha):
+	x = cuda.grid(1)
+
+	if x < A.shape[1]:
+		value = A[0, x]
+		arr[0, x] = alpha[0, x] * (2.0 * math.exp(-value) / ( (1.0 + math.exp(-value)) * (1.0 + math.exp(-value))))
+
+@cuda.jit
+def sum(arr, C):
+	x, y = cuda.grid(2)
+
+	if x >= arr.shape[0] or y >= arr.shape[1]:
+		return
+
+	arr[x, y] += C[x, y]
+
+@cuda.jit
+def dotMatrix(arr, A, B):
+	x, y = cuda.grid(2)
+	
+	temp = cuda.shared.array(shape=DIM2, dtype=float64)
+	sA = cuda.shared.array(shape=(1, DIM2[0]), dtype=float64)
+
+	tx = cuda.threadIdx.x
+	ty = cuda.threadIdx.y
+	temp[tx, ty] = float64(.0)
+
+	if x >= B.shape[0] or y >= B.shape[1]:
+		return
+	
+	if ty == 0:
+		sA[0, tx] = A[0, x]
+	cuda.syncthreads()
+
+	temp[tx, ty] = sA[0, tx] * B[x, y]
+	cuda.syncthreads()
+
+	if tx != 0:
+		return
+	
+	for i in range(1, cuda.blockDim.x):
+		temp[0, ty] += temp[i, ty]
+	cuda.atomic.add(arr, (0, y), temp[0, ty])
+
+@cuda.jit
+def dotMatrix_derivate(arr, w, alpha):
+	x, y, z = cuda.grid(3)
+
+	if x >= arr.shape[0] or y >= arr.shape[1] or z >= alpha.shape[1]:
+		return
+
+	cuda.atomic.add(arr, (x, y), alpha[x, z] * w[y, z])
+
+@cuda.jit
+def transposeDot(arr, A, B):
+	x, y = cuda.grid(2)
+
+	if x < arr.shape[0] and y < arr.shape[1]:
+		arr[x, y] = A[0, x] * B[0, y]
+
+@cuda.jit
+def updateWeights(w, eta, nabla):
+	x, y = cuda.grid(2)
+
+	if x < w.shape[0] and y < w.shape[1]:
 		w[x, y] -= eta[0] * nabla[x, y]
```

### Comparing `Kinho-1.0.0/Kinho/lib/GPU/utils.py` & `Kinho-1.0.1/Kinho/lib/GPU/utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-MINIMUMBLOCKSIZE = 28
-EPS = 1e-10
-THREADSPERBLOCK = 1024
-
-def ceil(A, B):
-	return (A + B - 1) // B
-
-def kernelConfig1D(size_x):
-	threads_x = THREADSPERBLOCK
-	blockspergrid_x = max(ceil(size_x, threads_x), MINIMUMBLOCKSIZE)
-
-	return (blockspergrid_x, threads_x)
-
-def kernelConfig2D(size_x, size_y, shape=None):
-	threads = THREADSPERBLOCK
-
-	sz = [size_x, size_y]
-	t = [1, 1]
-
-	t[0] = 32
-	t[1] = 32
-
-	if shape:
-		t[0] = shape[0]
-		t[1] = shape[1]
-	
-	blockspergrid_x = ceil(size_x, t[0])
-	blockspergrid_y = ceil(size_y, t[1])
-
-	blocks = blockspergrid_x * blockspergrid_y
-	if blocks < MINIMUMBLOCKSIZE:
-		add = MINIMUMBLOCKSIZE - blocks
-		blocks //= blockspergrid_y
-		blockspergrid_y += ceil(add, blocks)
-	
-	blockspergrid = (blockspergrid_x, blockspergrid_y)
-	threadsperblock = (t[0], t[1])
-
-	return (blockspergrid, threadsperblock)
-
-def kernelConfig3D(size_x, size_y, size_z):
-	threads = THREADSPERBLOCK
-
-	sz = [size_x, size_y, size_z]
-	t = [1, 1, 1]
-
-	upd = True
-	while threads > 1 and upd:
-		upd = False
-		for i in range(3):
-			if t[i] >= sz[i] or threads == 1:
-				continue
-			threads //= 2
-			t[i] *= 2
-			upd = True
-	
-	blockspergrid_x = ceil(size_x, t[0])
-	blockspergrid_y = ceil(size_y, t[1])
-	blockspergrid_z = ceil(size_z, t[2])
-
-	blocks = blockspergrid_x * blockspergrid_y * blockspergrid_z
-	if blocks < MINIMUMBLOCKSIZE:
-		add = MINIMUMBLOCKSIZE - blocks
-		blocks //= blockspergrid_z
-		blockspergrid_z += ceil(add, blocks)
-	
-	blockspergrid = (blockspergrid_x, blockspergrid_y, blockspergrid_z)
-	threadsperblock = (t[0], t[1], t[2])
-
-	return (blockspergrid, threadsperblock)
+MINIMUMBLOCKSIZE = 28
+EPS = 1e-10
+THREADSPERBLOCK = 1024
+
+def ceil(A, B):
+	return (A + B - 1) // B
+
+def kernelConfig1D(size_x):
+	threads_x = THREADSPERBLOCK
+	blockspergrid_x = max(ceil(size_x, threads_x), MINIMUMBLOCKSIZE)
+
+	return (blockspergrid_x, threads_x)
+
+def kernelConfig2D(size_x, size_y, shape=None):
+	threads = THREADSPERBLOCK
+
+	sz = [size_x, size_y]
+	t = [1, 1]
+
+	t[0] = 32
+	t[1] = 32
+
+	if shape:
+		t[0] = shape[0]
+		t[1] = shape[1]
+	
+	blockspergrid_x = ceil(size_x, t[0])
+	blockspergrid_y = ceil(size_y, t[1])
+
+	blocks = blockspergrid_x * blockspergrid_y
+	if blocks < MINIMUMBLOCKSIZE:
+		add = MINIMUMBLOCKSIZE - blocks
+		blocks //= blockspergrid_y
+		blockspergrid_y += ceil(add, blocks)
+	
+	blockspergrid = (blockspergrid_x, blockspergrid_y)
+	threadsperblock = (t[0], t[1])
+
+	return (blockspergrid, threadsperblock)
+
+def kernelConfig3D(size_x, size_y, size_z):
+	threads = THREADSPERBLOCK
+
+	sz = [size_x, size_y, size_z]
+	t = [1, 1, 1]
+
+	upd = True
+	while threads > 1 and upd:
+		upd = False
+		for i in range(3):
+			if t[i] >= sz[i] or threads == 1:
+				continue
+			threads //= 2
+			t[i] *= 2
+			upd = True
+	
+	blockspergrid_x = ceil(size_x, t[0])
+	blockspergrid_y = ceil(size_y, t[1])
+	blockspergrid_z = ceil(size_z, t[2])
+
+	blocks = blockspergrid_x * blockspergrid_y * blockspergrid_z
+	if blocks < MINIMUMBLOCKSIZE:
+		add = MINIMUMBLOCKSIZE - blocks
+		blocks //= blockspergrid_z
+		blockspergrid_z += ceil(add, blocks)
+	
+	blockspergrid = (blockspergrid_x, blockspergrid_y, blockspergrid_z)
+	threadsperblock = (t[0], t[1], t[2])
+
+	return (blockspergrid, threadsperblock)
```

### Comparing `Kinho-1.0.0/Kinho/neural.py` & `Kinho-1.0.1/Kinho/neural.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,346 +1,346 @@
-import numpy as np
-from .lib.GPU import *
-from timeit import default_timer as timer
-from colorama import Fore, init
-from .kernel import *
-from .transfer import loadTo
-from .brain import Wrapper, Builder
-
-init()
-MINIMUMBLOCKSIZE = 28
-
-def ceil(A, B):
-    return (A + B - 1) // B
-
-class Neural(object):
-
-    def __init__(self, sizes=None, brain_path=None, eta=0.01, gpu=False):
-        if not sizes and not brain_path:
-            raise TypeError('Should set `sizes` or `brain_path` params')
-        
-        self.__eta = np.array([eta])
-        self.__num_layers = None
-        self.__architecture = None
-        self.__weights = None
-        self.__biases = None
-        self.__gpuMode = gpu
-        self.__logs = {}
-        self.__mapper = {}
-
-        t = timer()
-        self.__setBrain(Builder(brain_path) if brain_path else None, sizes)
-        self.__reserveMemo()
-        t = timer() - t
-    
-    def __setBrain(self, brain, sizes):
-        if brain:
-            self.__num_layers = brain.size()
-            self.__architecture = brain.architecture()
-            self.__biases = brain.biases()
-            self.__weights = brain.weights()
-        else:
-            self.__num_layers = len(sizes)
-            self.__architecture = sizes
-            self.__biases = [np.random.uniform(0, -1, x).reshape((1,x)) for x in self.__architecture[1:]]
-            self.__weights = [np.random.uniform(-2,2,x*y).reshape((x, y)) for x,y in zip(self.__architecture[:-1], self.__architecture[1:])]
-
-        if not self.__gpuMode:
-            return None
-
-        self.__eta = cuda.to_device(self.__eta)
-        cuda_biases = [cuda.to_device(bias) for bias in self.__biases]
-        self.__biases = cuda_biases
-
-        cuda_weights = [cuda.to_device(weight) for weight in self.__weights]
-        self.__weights = cuda_weights
-    
-    def __getReserve(self, kernel, pos):
-        if self.__gpuMode == False:
-            return None
-        
-        return self.__buffer[kernel][pos]
-    
-    def __reserveArr(self, module_name, shape, streams):
-        arr = cuda.device_array(shape, dtype=np.float64)
-
-        stream = cuda.stream()
-        self.__buffer[module_name].append(cuda.to_device(arr, stream=stream))
-        streams.append(stream)
-
-    def __reserveActivation(self, streams):
-        for size in self.__architecture:
-            self.__reserveArr('activation', (1, size), streams)
-    
-    def __reserveLayer(self, streams):
-        for size in self.__architecture[1:]:
-            self.__reserveArr('layer', (1, size), streams)
-    
-    def __reserveSelector(self, streams):
-        self.__reserveArr('selector', (1, self.__architecture[-1]), streams)
-    
-    def __reserveDLoss(self, streams):
-        self.__reserveArr('d_loss', (1, self.__architecture[-1]), streams)
-    
-    def __reserveDSelector(self, streams):
-        self.__reserveArr('d_selector', (1, self.__architecture[-1]), streams)
-
-    def __reserveDActivation(self, streams):
-        LEN = len(self.__architecture)
-
-        for i in range(LEN-1, -1, -1):
-            self.__reserveArr('d_activation', (1, self.__architecture[i]), streams)
-    
-    def __reserveTranspose(self, streams):
-        LEN = len(self.__architecture)
-
-        for i in range(LEN-2, -1, -1):
-            self.__reserveArr('transpose', (self.__architecture[i], self.__architecture[i+1]), streams)
-    
-    def __reserveDLayer(self, streams):
-        LEN = len(self.__architecture)
-
-        for i in range(LEN-2, -1, -1):
-            self.__reserveArr('d_layer', (1, self.__architecture[i]), streams)
-
-    def __reserveExtra(self, streams):
-        self.__reserveArr('extra', (1, ), streams)
-
-    def __reserveMemo(self):
-        if self.__gpuMode == False:
-            return None
-
-        self.__buffer = {
-            'activation': [],
-            'layer': [],
-            'selector': [],
-            'd_loss': [],
-            'd_selector': [],
-            'd_activation': [],
-            'transpose': [],
-            'd_layer': [],
-            'extra': [],
-        }
-
-        streams = []
-        self.__reserveActivation(streams)
-        self.__reserveLayer(streams)
-        self.__reserveSelector(streams)
-        self.__reserveDLoss(streams)
-        self.__reserveDSelector(streams)
-        self.__reserveDActivation(streams)
-        self.__reserveTranspose(streams)
-        self.__reserveDLayer(streams)
-        self.__reserveExtra(streams)
-
-        for stream in streams:
-            stream.synchronize()
-
-    def logs(self):
-        return self.__logs
-
-    def __logger(self, method, delta, dbg=False):
-        delta = round(delta * 1000, 3)
-
-        mode = '[GPU] ' if self.__gpuMode else '[CPU] '
-        name = mode + method
-
-        if name not in self.__logs.keys():
-            self.__logs[name] = []
-        self.__logs[name].append(delta)
-
-        color = Fore.GREEN
-        if delta >= 1.0:
-            color = Fore.YELLOW
-        if delta >= 5.0:
-            color = Fore.RED
-        
-        if dbg:
-            print(color + "{}: {}ms".format(method, delta))
-
-    def __swapper(self, *args, buffer, GPURunner, CPURunner):
-        arr = None
-        t = timer()
-
-        name = GPURunner.__name__
-        dbg = True if GPURunner.__name__ == 'transpose' else False
-
-        if self.__gpuMode == False:
-            arr = CPURunner(*args)
-        else:
-            mapped_args = []
-            for arg in args:
-                if cuda.is_cuda_array(arg):
-                    mapped_args.append(arg)
-                else:
-                    arg_dvc = cuda.to_device(arg)
-                    mapped_args.append(arg_dvc)
-                    self.__mapper[id(arg)] = arg_dvc
-                    print("register")
-                    assert False
-
-            arr = GPURunner(*mapped_args, buffer)
-
-        t = timer() - t
-        self.__logger(name, t, dbg=False)
-
-        return arr
-
-    def __loss(self, predicted, target, buffer=None):
-        return self.__swapper(predicted, target, buffer=buffer, GPURunner=loss, CPURunner=mse_cpu)
-
-    def __d_loss(self, predicted, target, buffer=None):
-        return self.__swapper(predicted, target, buffer=buffer, GPURunner=dloss, CPURunner=mse_derivate_cpu)
-
-    def __selector(self, z, buffer=None):
-        return self.__swapper(z, self.__getReserve('extra', 0), buffer=buffer, GPURunner=selector, CPURunner=softmax_cpu)
-
-    def __d_selector(self, z, alpha, buffer=None):
-        return self.__swapper(z, alpha, buffer=buffer, GPURunner=dselector, CPURunner=softmax_derivate_cpu)
-
-    def __activation(self, z, buffer=None):
-       return self.__swapper(z, buffer=buffer, GPURunner=activation, CPURunner=sigmoid2_cpu)
-
-    def __d_activation(self, z, alpha, buffer=None):
-        return self.__swapper(z, alpha, buffer=buffer, GPURunner=dactivation, CPURunner=sigmoid2_derivate_cpu)
-    
-    def __layer(self, x, w, b, buffer=None):
-        return self.__swapper(x, w, b, buffer=buffer, GPURunner=layer, CPURunner=dotMatrix_cpu)
-
-    def __d_layer(self, _, w, alpha, buffer=None):
-        return self.__swapper(w, alpha, buffer=buffer, GPURunner=dlayer, CPURunner=dotMatrix_derivate_cpu)
-    
-    def __updateWeight(self, weights, eta, nabla_w, buffer=None):
-        return self.__swapper(weights, eta, nabla_w, buffer=buffer, GPURunner=updateWeight, CPURunner=updateWeights_cpu)
-    
-    def __transpose(self, z, derror, buffer=None):
-        return self.__swapper(z, derror, buffer=buffer, GPURunner=transpose, CPURunner=transposeDot_cpu)
-
-    def __feedForward(self, x):
-        t = timer()
-
-        activation_pointer = 0
-        layer_pointer = 0
-
-        for w, b in zip(self.__weights,self.__biases):
-            arr = self.__activation(x, buffer=self.__getReserve('activation', activation_pointer))
-
-            x = self.__layer(arr, w, b, buffer=self.__getReserve('layer', layer_pointer))
-
-            activation_pointer += 1
-            layer_pointer += 1
-
-        y = self.__selector(x, buffer=self.__getReserve('selector', 0))
-
-        t = timer() - t
-        self.__logger("feedForward", t)
-        return y
-
-    def __backPropagation(self, x, target):
-        t = timer()
-
-        # feedForward
-        z = [x] # save all Zs
-        activations = [] # save all activations
-
-        activation_pointer = 1
-        layer_pointer = 0
-
-        for w, b in zip(self.__weights, self.__biases):
-            x = self.__layer(x, w, b, buffer=self.__getReserve('layer', layer_pointer))
-            layer_pointer += 1
-
-            activations.append(x)
-            x = self.__activation(x, buffer=self.__getReserve('activation', activation_pointer))
-            activation_pointer += 1
-
-            z.append(x)
-
-        y = self.__selector(x, buffer=self.__getReserve('selector', 0))
-
-        derror = self.__d_loss(y, target, buffer=self.__getReserve('d_loss', 0))
-
-        derror = self.__d_selector(z[self.__num_layers - 1], derror, buffer=self.__getReserve('d_selector', 0))
-
-        d_activation_pointer = 0
-        d_layer_pointer = 0
-        transpose_pointer = 0
-
-        for l in range(1, self.__num_layers):
-            w = self.__weights[-l]
-            b = self.__biases[-l]
-
-            derror = self.__d_activation(activations[-l], derror, buffer=self.__getReserve('d_activation', d_activation_pointer))
-
-            d_activation_pointer += 1
-            
-            nabla_w = self.__transpose(z[-l-1], derror, buffer=self.__getReserve('transpose', transpose_pointer))
-            transpose_pointer += 1
-
-            nabla_b = derror # error for each bias
-
-            derror =  self.__d_layer(z[-l-1], w, derror, buffer=self.__getReserve('d_layer', d_layer_pointer))
-
-            d_layer_pointer += 1
-
-            self.__weights[-l] = self.__updateWeight(self.__weights[-l], self.__eta, nabla_w)
-
-            self.__biases[-l] = self.__updateWeight(self.__biases[-l], self.__eta, nabla_b)
-
-        t = timer() - t
-        prefix = '[GPU] ' if self.__gpuMode else '[CPU] '
-        self.__logger(prefix + "backpropagation", t, dbg=False)
-    
-    def __buildMsg(self, x):
-        if self.__gpuMode:
-            return cuda.to_device(x)
-        return x
-
-    def send(self, l):
-        t = timer()
-
-        x =  self.__buildMsg(np.array([l]))
-        arr = self.__feedForward(x)
-
-        hst, = loadTo(arr, mode='CPU')
-        y = hst[0]
-
-        t = timer() - t
-        self.__logger("send", t)
-
-        return y
-
-    def learn(self, x, y):
-        t = timer()
-
-        x = self.__activation(self.__buildMsg(np.array([x])), buffer=self.__getReserve('activation', 0))
-        y = self.__buildMsg(np.array([y]))
-
-        self.__backPropagation(x, y)
-
-        t = timer() - t
-        self.__logger("learn", t)
-
-    def cost(self, x, y):
-        t = timer()
-
-        np_x = self.__buildMsg(np.array([x]))
-        np_y = self.__buildMsg(np.array([y]))
-        np_x = self.__activation(np_x, buffer=self.__getReserve('activation', 0))
-
-        ret = self.__loss(self.__feedForward(np_x),np_y)
-
-        t = timer() - t
-        self.__logger("cost", t)
-        return ret
-    
-    def export(self, filename, path):
-        layers = []
-
-        for w, b in zip(self.__weights, self.__biases):
-            w_host, b_host = loadTo(w, b, mode='CPU')
-            layers.append((w_host, b_host))
-        
-        wrapper = Wrapper(layers)
-
-        with open(path + filename + '.brain', 'wb') as file:
-            file.write(wrapper.data())
+import numpy as np
+from .lib.GPU import *
+from timeit import default_timer as timer
+from colorama import Fore, init
+from .kernel import *
+from .transfer import loadTo
+from .brain import Wrapper, Builder
+
+init()
+MINIMUMBLOCKSIZE = 28
+
+def ceil(A, B):
+    return (A + B - 1) // B
+
+class Neural(object):
+
+    def __init__(self, sizes=None, brain_path=None, eta=0.01, gpu=False):
+        if not sizes and not brain_path:
+            raise TypeError('Should set `sizes` or `brain_path` params')
+        
+        self.__eta = np.array([eta])
+        self.__num_layers = None
+        self.__architecture = None
+        self.__weights = None
+        self.__biases = None
+        self.__gpuMode = gpu
+        self.__logs = {}
+        self.__mapper = {}
+
+        t = timer()
+        self.__setBrain(Builder(brain_path) if brain_path else None, sizes)
+        self.__reserveMemo()
+        t = timer() - t
+    
+    def __setBrain(self, brain, sizes):
+        if brain:
+            self.__num_layers = brain.size()
+            self.__architecture = brain.architecture()
+            self.__biases = brain.biases()
+            self.__weights = brain.weights()
+        else:
+            self.__num_layers = len(sizes)
+            self.__architecture = sizes
+            self.__biases = [np.random.uniform(0, -1, x).reshape((1,x)) for x in self.__architecture[1:]]
+            self.__weights = [np.random.uniform(-2,2,x*y).reshape((x, y)) for x,y in zip(self.__architecture[:-1], self.__architecture[1:])]
+
+        if not self.__gpuMode:
+            return None
+
+        self.__eta = cuda.to_device(self.__eta)
+        cuda_biases = [cuda.to_device(bias) for bias in self.__biases]
+        self.__biases = cuda_biases
+
+        cuda_weights = [cuda.to_device(weight) for weight in self.__weights]
+        self.__weights = cuda_weights
+    
+    def __getReserve(self, kernel, pos):
+        if self.__gpuMode == False:
+            return None
+        
+        return self.__buffer[kernel][pos]
+    
+    def __reserveArr(self, module_name, shape, streams):
+        arr = cuda.device_array(shape, dtype=np.float64)
+
+        stream = cuda.stream()
+        self.__buffer[module_name].append(cuda.to_device(arr, stream=stream))
+        streams.append(stream)
+
+    def __reserveActivation(self, streams):
+        for size in self.__architecture:
+            self.__reserveArr('activation', (1, size), streams)
+    
+    def __reserveLayer(self, streams):
+        for size in self.__architecture[1:]:
+            self.__reserveArr('layer', (1, size), streams)
+    
+    def __reserveSelector(self, streams):
+        self.__reserveArr('selector', (1, self.__architecture[-1]), streams)
+    
+    def __reserveDLoss(self, streams):
+        self.__reserveArr('d_loss', (1, self.__architecture[-1]), streams)
+    
+    def __reserveDSelector(self, streams):
+        self.__reserveArr('d_selector', (1, self.__architecture[-1]), streams)
+
+    def __reserveDActivation(self, streams):
+        LEN = len(self.__architecture)
+
+        for i in range(LEN-1, -1, -1):
+            self.__reserveArr('d_activation', (1, self.__architecture[i]), streams)
+    
+    def __reserveTranspose(self, streams):
+        LEN = len(self.__architecture)
+
+        for i in range(LEN-2, -1, -1):
+            self.__reserveArr('transpose', (self.__architecture[i], self.__architecture[i+1]), streams)
+    
+    def __reserveDLayer(self, streams):
+        LEN = len(self.__architecture)
+
+        for i in range(LEN-2, -1, -1):
+            self.__reserveArr('d_layer', (1, self.__architecture[i]), streams)
+
+    def __reserveExtra(self, streams):
+        self.__reserveArr('extra', (1, ), streams)
+
+    def __reserveMemo(self):
+        if self.__gpuMode == False:
+            return None
+
+        self.__buffer = {
+            'activation': [],
+            'layer': [],
+            'selector': [],
+            'd_loss': [],
+            'd_selector': [],
+            'd_activation': [],
+            'transpose': [],
+            'd_layer': [],
+            'extra': [],
+        }
+
+        streams = []
+        self.__reserveActivation(streams)
+        self.__reserveLayer(streams)
+        self.__reserveSelector(streams)
+        self.__reserveDLoss(streams)
+        self.__reserveDSelector(streams)
+        self.__reserveDActivation(streams)
+        self.__reserveTranspose(streams)
+        self.__reserveDLayer(streams)
+        self.__reserveExtra(streams)
+
+        for stream in streams:
+            stream.synchronize()
+
+    def logs(self):
+        return self.__logs
+
+    def __logger(self, method, delta, dbg=False):
+        delta = round(delta * 1000, 3)
+
+        mode = '[GPU] ' if self.__gpuMode else '[CPU] '
+        name = mode + method
+
+        if name not in self.__logs.keys():
+            self.__logs[name] = []
+        self.__logs[name].append(delta)
+
+        color = Fore.GREEN
+        if delta >= 1.0:
+            color = Fore.YELLOW
+        if delta >= 5.0:
+            color = Fore.RED
+        
+        if dbg:
+            print(color + "{}: {}ms".format(method, delta))
+
+    def __swapper(self, *args, buffer, GPURunner, CPURunner):
+        arr = None
+        t = timer()
+
+        name = GPURunner.__name__
+        dbg = True if GPURunner.__name__ == 'transpose' else False
+
+        if self.__gpuMode == False:
+            arr = CPURunner(*args)
+        else:
+            mapped_args = []
+            for arg in args:
+                if cuda.is_cuda_array(arg):
+                    mapped_args.append(arg)
+                else:
+                    arg_dvc = cuda.to_device(arg)
+                    mapped_args.append(arg_dvc)
+                    self.__mapper[id(arg)] = arg_dvc
+                    print("register")
+                    assert False
+
+            arr = GPURunner(*mapped_args, buffer)
+
+        t = timer() - t
+        self.__logger(name, t, dbg=False)
+
+        return arr
+
+    def __loss(self, predicted, target, buffer=None):
+        return self.__swapper(predicted, target, buffer=buffer, GPURunner=loss, CPURunner=mse_cpu)
+
+    def __d_loss(self, predicted, target, buffer=None):
+        return self.__swapper(predicted, target, buffer=buffer, GPURunner=dloss, CPURunner=mse_derivate_cpu)
+
+    def __selector(self, z, buffer=None):
+        return self.__swapper(z, self.__getReserve('extra', 0), buffer=buffer, GPURunner=selector, CPURunner=softmax_cpu)
+
+    def __d_selector(self, z, alpha, buffer=None):
+        return self.__swapper(z, alpha, buffer=buffer, GPURunner=dselector, CPURunner=softmax_derivate_cpu)
+
+    def __activation(self, z, buffer=None):
+       return self.__swapper(z, buffer=buffer, GPURunner=activation, CPURunner=sigmoid2_cpu)
+
+    def __d_activation(self, z, alpha, buffer=None):
+        return self.__swapper(z, alpha, buffer=buffer, GPURunner=dactivation, CPURunner=sigmoid2_derivate_cpu)
+    
+    def __layer(self, x, w, b, buffer=None):
+        return self.__swapper(x, w, b, buffer=buffer, GPURunner=layer, CPURunner=dotMatrix_cpu)
+
+    def __d_layer(self, _, w, alpha, buffer=None):
+        return self.__swapper(w, alpha, buffer=buffer, GPURunner=dlayer, CPURunner=dotMatrix_derivate_cpu)
+    
+    def __updateWeight(self, weights, eta, nabla_w, buffer=None):
+        return self.__swapper(weights, eta, nabla_w, buffer=buffer, GPURunner=updateWeight, CPURunner=updateWeights_cpu)
+    
+    def __transpose(self, z, derror, buffer=None):
+        return self.__swapper(z, derror, buffer=buffer, GPURunner=transpose, CPURunner=transposeDot_cpu)
+
+    def __feedForward(self, x):
+        t = timer()
+
+        activation_pointer = 0
+        layer_pointer = 0
+
+        for w, b in zip(self.__weights,self.__biases):
+            arr = self.__activation(x, buffer=self.__getReserve('activation', activation_pointer))
+
+            x = self.__layer(arr, w, b, buffer=self.__getReserve('layer', layer_pointer))
+
+            activation_pointer += 1
+            layer_pointer += 1
+
+        y = self.__selector(x, buffer=self.__getReserve('selector', 0))
+
+        t = timer() - t
+        self.__logger("feedForward", t)
+        return y
+
+    def __backPropagation(self, x, target):
+        t = timer()
+
+        # feedForward
+        z = [x] # save all Zs
+        activations = [] # save all activations
+
+        activation_pointer = 1
+        layer_pointer = 0
+
+        for w, b in zip(self.__weights, self.__biases):
+            x = self.__layer(x, w, b, buffer=self.__getReserve('layer', layer_pointer))
+            layer_pointer += 1
+
+            activations.append(x)
+            x = self.__activation(x, buffer=self.__getReserve('activation', activation_pointer))
+            activation_pointer += 1
+
+            z.append(x)
+
+        y = self.__selector(x, buffer=self.__getReserve('selector', 0))
+
+        derror = self.__d_loss(y, target, buffer=self.__getReserve('d_loss', 0))
+
+        derror = self.__d_selector(z[self.__num_layers - 1], derror, buffer=self.__getReserve('d_selector', 0))
+
+        d_activation_pointer = 0
+        d_layer_pointer = 0
+        transpose_pointer = 0
+
+        for l in range(1, self.__num_layers):
+            w = self.__weights[-l]
+            b = self.__biases[-l]
+
+            derror = self.__d_activation(activations[-l], derror, buffer=self.__getReserve('d_activation', d_activation_pointer))
+
+            d_activation_pointer += 1
+            
+            nabla_w = self.__transpose(z[-l-1], derror, buffer=self.__getReserve('transpose', transpose_pointer))
+            transpose_pointer += 1
+
+            nabla_b = derror # error for each bias
+
+            derror =  self.__d_layer(z[-l-1], w, derror, buffer=self.__getReserve('d_layer', d_layer_pointer))
+
+            d_layer_pointer += 1
+
+            self.__weights[-l] = self.__updateWeight(self.__weights[-l], self.__eta, nabla_w)
+
+            self.__biases[-l] = self.__updateWeight(self.__biases[-l], self.__eta, nabla_b)
+
+        t = timer() - t
+        prefix = '[GPU] ' if self.__gpuMode else '[CPU] '
+        self.__logger(prefix + "backpropagation", t, dbg=False)
+    
+    def __buildMsg(self, x):
+        if self.__gpuMode:
+            return cuda.to_device(x)
+        return x
+
+    def send(self, l):
+        t = timer()
+
+        x =  self.__buildMsg(np.array([l]))
+        arr = self.__feedForward(x)
+
+        hst, = loadTo(arr, mode='CPU')
+        y = hst[0]
+
+        t = timer() - t
+        self.__logger("send", t)
+
+        return y
+
+    def learn(self, x, y):
+        t = timer()
+
+        x = self.__activation(self.__buildMsg(np.array([x])), buffer=self.__getReserve('activation', 0))
+        y = self.__buildMsg(np.array([y]))
+
+        self.__backPropagation(x, y)
+
+        t = timer() - t
+        self.__logger("learn", t)
+
+    def cost(self, x, y):
+        t = timer()
+
+        np_x = self.__buildMsg(np.array([x]))
+        np_y = self.__buildMsg(np.array([y]))
+        np_x = self.__activation(np_x, buffer=self.__getReserve('activation', 0))
+
+        ret = self.__loss(self.__feedForward(np_x),np_y)
+
+        t = timer() - t
+        self.__logger("cost", t)
+        return ret
+    
+    def export(self, filename, path):
+        layers = []
+
+        for w, b in zip(self.__weights, self.__biases):
+            w_host, b_host = loadTo(w, b, mode='CPU')
+            layers.append((w_host, b_host))
+        
+        wrapper = Wrapper(layers)
+
+        with open(path + filename + '.brain', 'wb') as file:
+            file.write(wrapper.data())
```

### Comparing `Kinho-1.0.0/Kinho.egg-info/PKG-INFO` & `Kinho-1.0.1/Kinho.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: Kinho
-Version: 1.0.0
-Summary: A library to classify images with deep learning.
-Home-page: https://github.com/kinhosz/Neural
-Author: Kinhosz
-Author-email: scruz.josecarlos@gmail.com
-License: MIT
-Keywords: dev,web
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: GPU
-Classifier: Environment :: GPU :: NVIDIA CUDA
-Classifier: Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Portuguese (Brazilian)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-License-File: LICENSE
-
-The library features the "Neural" model, which is a Convolutional Neural Network (CNN) for image classification. It supports both CPU and GPU, providing excellent performance for large networks. You can also export and import Deep models and continue training on other machines. The exported file is generated in the ".brain" format, which is a proprietary data type of this project. For more information, please visit our repository.
+Metadata-Version: 2.1
+Name: Kinho
+Version: 1.0.1
+Summary: A library to classify images with deep learning.
+Home-page: https://github.com/kinhosz/Neural
+Author: Kinhosz
+Author-email: scruz.josecarlos@gmail.com
+License: MIT
+Keywords: dev,web
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: GPU
+Classifier: Environment :: GPU :: NVIDIA CUDA
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Portuguese (Brazilian)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+License-File: LICENSE
+
+The library features the "Neural" model, which is a Convolutional Neural Network (CNN) for image classification. It supports both CPU and GPU, providing excellent performance for large networks. You can also export and import Deep models and continue training on other machines. The exported file is generated in the ".brain" format, which is a proprietary data type of this project. For more information, please visit our repository.
```

### Comparing `Kinho-1.0.0/Kinho.egg-info/SOURCES.txt` & `Kinho-1.0.1/Kinho.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -33,8 +33,9 @@
 Kinho/kernel/vars.py
 Kinho/lib/__init__.py
 Kinho/lib/GPU/CPU_version.py
 Kinho/lib/GPU/Function.py
 Kinho/lib/GPU/__init__.py
 Kinho/lib/GPU/utils.py
 Kinho/transfer/__init__.py
-Kinho/transfer/loader.py
+Kinho/transfer/loader.py
+tests/test_learn_rate.py
```

### Comparing `Kinho-1.0.0/LICENSE` & `Kinho-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 José Carlos
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 José Carlos
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `Kinho-1.0.0/PKG-INFO` & `Kinho-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: Kinho
-Version: 1.0.0
-Summary: A library to classify images with deep learning.
-Home-page: https://github.com/kinhosz/Neural
-Author: Kinhosz
-Author-email: scruz.josecarlos@gmail.com
-License: MIT
-Keywords: dev,web
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: GPU
-Classifier: Environment :: GPU :: NVIDIA CUDA
-Classifier: Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Portuguese (Brazilian)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-License-File: LICENSE
-
-The library features the "Neural" model, which is a Convolutional Neural Network (CNN) for image classification. It supports both CPU and GPU, providing excellent performance for large networks. You can also export and import Deep models and continue training on other machines. The exported file is generated in the ".brain" format, which is a proprietary data type of this project. For more information, please visit our repository.
+Metadata-Version: 2.1
+Name: Kinho
+Version: 1.0.1
+Summary: A library to classify images with deep learning.
+Home-page: https://github.com/kinhosz/Neural
+Author: Kinhosz
+Author-email: scruz.josecarlos@gmail.com
+License: MIT
+Keywords: dev,web
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: GPU
+Classifier: Environment :: GPU :: NVIDIA CUDA
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Portuguese (Brazilian)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+License-File: LICENSE
+
+The library features the "Neural" model, which is a Convolutional Neural Network (CNN) for image classification. It supports both CPU and GPU, providing excellent performance for large networks. You can also export and import Deep models and continue training on other machines. The exported file is generated in the ".brain" format, which is a proprietary data type of this project. For more information, please visit our repository.
```

### Comparing `Kinho-1.0.0/README.md` & `Kinho-1.0.1/README.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-# Rede Neural V2
-Classe para uma rede neural feedforward com uma camada de entrada, camadas ocultas e uma camada de saída.
-
-A rede é chamada `Neural`, uma `CNN` que você pode importar do package `Kinho`.
-
-## Como instalar
-```
-pip install Kinho
-```
-
-## Métodos:
-```py
-def __init__(sizes=None, brain_path=None, eta=0.01, gpu=False):
-    pass
-
-def send(input):
-    pass
-
-def learn(input, output):
-    pass
-
-def export(filename, path):
-    pass
-
-def cost(input, output):
-    pass
-```
-
-### Neural (constructor)
-
-#### Parâmetros:
-- `sizes (list of floats)`: lista com o número de neurônios em cada camada da rede, onde o primeiro elemento da lista é a quantidade de neurônios na camada de entrada, o último é a quantidade de neurônios na camada de saída e os elementos intermediários são as quantidades de neurônios nas camadas ocultas.
-- `brain_path(string)`: caminho de um arquivo `x.brain`, de um modelo pré-treinado que você já tenha salvo em seu diretório.
-- `eta (float)`: taxa de aprendizado. Caso não seja definida, assumimos uma taxa padrão de __0.01__.
-- `gpu (bool)`: se __True__, permite que a rede neural automaticamente mude o contexto para utilização da GPU para melhoria de performance.
-
-Exemplo:
-```py
-from Kinho import Neural
-
-net_without_imported_model = Neural(sizes=[10, 200, 300, 50, 5], eta=0.1, gpu=True)
-'''
-    Uma rede com 3 camadas ocultas (200, 300, 50). Uma camada de input com 10 entradas e,
-    uma camada de output com 5 saídas. Taxa de aprendizado 0.1 e todos os pesos sinápticos
-    aleatórios.
-'''
-
-net_with_imported_model = Neural(brain_path='./pre-trained/mnist_model.brain', eta=0.1, gpu=True)
-'''
-    Uma rede com a arquitetura e todos os pesos e biases importados de um modelo previamente treinado dentro do caminho <brain_path>.
-'''
-
-invalid_network = Neural(eta=0.1, gpu=True)
-'''
-    Um erro será gerado, pois é necessária a presença da arquitetura (sizes) ou modelo pré-treinado (brain_path).
-'''
-```
-
-É __obrigatório__ passar o `sizes` ou o `brain_path`, caso contrário, um erro de tipo será gerado. Caso o usuário passe os dois, a rede irá priorizar o modelo importado, ou seja, o `brain_path`.
-
-### send
-
-#### Parâmetros:
-- `input (list of floats)`: Os valores de entrada que serão enviados para a rede.
-
-#### Retorno:
-`list[float]`: uma lista com o mesmo tamanho da camada de saída da rede. Para posição(rótulo), existirá um float informando a probabilidade da entrada corresponder com cada rótulo. Deve-se considerar como predição o rótulo no qual tiver maior probabilidade.
-
-Exemplo:
-```py
-input = [10, 2, 4, 4, 100, 90, 3, -1, 9, 10]
-output = net.send(input)
-print(output)
-# [0.2, 0.05, 0.7, 0.05, 0.0]
-'''
-    A rede atribuiu a probabilidade para cada rótulo. Logo, há 20% de chance do rótulo
-    relacionado a posição 0 ser a resposta, e há 70% de chance do rótulo relacionado a
-    posição 2 ser a a resposta da entrada cedida à rede.
-'''
-```
-
-### learn
-
-#### Parâmetros:
-- `input (list of floats)`: Os valores de entrada que serão enviados para a rede.
-- `output (list of floats)`: A probabilidade esperada de cada rótulo estar relacionado com o input. Note que a soma de todas as probabilidades deverá ser igual a __1.0__.
-
-#### Retorno:
-Não há retorno, a rede apenas aprende utilizando __backpropagation__ e atualiza seus pesos e biases.
-
-Exemplo:
-```py
-input = [10, 2, 4, 4, 100, 90, 3, -1, 9, 10]
-output = [0.0, 0.0, 1.0, 0.0, 0.0]
-
-net.learn(input, output)
-'''
-    A resposta para o input dado deve ser 2. Logo, a rede recebe
-    o output esperado do mar de probabilidades e aprende a diminuir o erro.
-'''
-```
-
-### export
-
-#### Parâmetros:
-- `filename (string)`: O nome do arquivo que você deseja dar para o novo arquivo de dados exportado.
-- `path (string)`: caminho onde você deseja salvar seu arquivo. Coloque o diretório dentro da pasta de destino.
-
-ex.: você poderá encontrar o arquivo neste diretório: `<path><filename>.brain`
-
-#### Retorno:
-Não há um retorno, mas você pode verificar se o arquivo se encontra no caminho especificado. Se sim, você já poderá compartilhar com outras aplicações e reutilizar os dados da sua rede e continuar o seu trabalho de onde parou.
-
-### cost
-
-#### Parâmetros:
-- `input (list of floats)`: Os valores de entrada que serão enviados para a rede.
-- `output (list of floats)`: A probabilidade esperada de cada rótulo estar relacionado com o input. Note que a soma de todas as probabilidades deverá ser igual a __1.0__.
-
-#### Retorno:
-`float`: o valor da média do quadrado das diferenças entre o output esperado pelo usuário e o output gerado pela rede.
-
-Exemplo:
-```py
-input = [10, 2, 4, 4, 100, 90, 3, -1, 9, 10]
-output = [0.0, 0.0, 1.0, 0.0, 0.0]
-
-mse = net.cost(input, output)
-print(mse)
-# 0.027
-```
-
-> O tipo de dado `.brain` é um formato totalmente autoral deste projeto, suas especificações no momento não apresentam documentações, mas você pode conferir manualmente dentro da pasta `Kinho/brain`. Em breve, se necessário, haverá uma documentação mais explícita de como ler/criar este tipo de dado e quais especificações devem-se seguir para ser considerado um formato válido.
+# Rede Neural V2
+Classe para uma rede neural feedforward com uma camada de entrada, camadas ocultas e uma camada de saída.
+
+A rede é chamada `Neural`, uma `CNN` que você pode importar do package `Kinho`.
+
+## Como instalar
+```
+pip install Kinho
+```
+
+## Métodos:
+```py
+def __init__(sizes=None, brain_path=None, eta=0.01, gpu=False):
+    pass
+
+def send(input):
+    pass
+
+def learn(input, output):
+    pass
+
+def export(filename, path):
+    pass
+
+def cost(input, output):
+    pass
+```
+
+### Neural (constructor)
+
+#### Parâmetros:
+- `sizes (list of floats)`: lista com o número de neurônios em cada camada da rede, onde o primeiro elemento da lista é a quantidade de neurônios na camada de entrada, o último é a quantidade de neurônios na camada de saída e os elementos intermediários são as quantidades de neurônios nas camadas ocultas.
+- `brain_path(string)`: caminho de um arquivo `x.brain`, de um modelo pré-treinado que você já tenha salvo em seu diretório.
+- `eta (float)`: taxa de aprendizado. Caso não seja definida, assumimos uma taxa padrão de __0.01__.
+- `gpu (bool)`: se __True__, permite que a rede neural automaticamente mude o contexto para utilização da GPU para melhoria de performance.
+
+Exemplo:
+```py
+from Kinho import Neural
+
+net_without_imported_model = Neural(sizes=[10, 200, 300, 50, 5], eta=0.1, gpu=True)
+'''
+    Uma rede com 3 camadas ocultas (200, 300, 50). Uma camada de input com 10 entradas e,
+    uma camada de output com 5 saídas. Taxa de aprendizado 0.1 e todos os pesos sinápticos
+    aleatórios.
+'''
+
+net_with_imported_model = Neural(brain_path='./pre-trained/mnist_model.brain', eta=0.1, gpu=True)
+'''
+    Uma rede com a arquitetura e todos os pesos e biases importados de um modelo previamente treinado dentro do caminho <brain_path>.
+'''
+
+invalid_network = Neural(eta=0.1, gpu=True)
+'''
+    Um erro será gerado, pois é necessária a presença da arquitetura (sizes) ou modelo pré-treinado (brain_path).
+'''
+```
+
+É __obrigatório__ passar o `sizes` ou o `brain_path`, caso contrário, um erro de tipo será gerado. Caso o usuário passe os dois, a rede irá priorizar o modelo importado, ou seja, o `brain_path`.
+
+### send
+
+#### Parâmetros:
+- `input (list of floats)`: Os valores de entrada que serão enviados para a rede.
+
+#### Retorno:
+`list[float]`: uma lista com o mesmo tamanho da camada de saída da rede. Para posição(rótulo), existirá um float informando a probabilidade da entrada corresponder com cada rótulo. Deve-se considerar como predição o rótulo no qual tiver maior probabilidade.
+
+Exemplo:
+```py
+input = [10, 2, 4, 4, 100, 90, 3, -1, 9, 10]
+output = net.send(input)
+print(output)
+# [0.2, 0.05, 0.7, 0.05, 0.0]
+'''
+    A rede atribuiu a probabilidade para cada rótulo. Logo, há 20% de chance do rótulo
+    relacionado a posição 0 ser a resposta, e há 70% de chance do rótulo relacionado a
+    posição 2 ser a a resposta da entrada cedida à rede.
+'''
+```
+
+### learn
+
+#### Parâmetros:
+- `input (list of floats)`: Os valores de entrada que serão enviados para a rede.
+- `output (list of floats)`: A probabilidade esperada de cada rótulo estar relacionado com o input. Note que a soma de todas as probabilidades deverá ser igual a __1.0__.
+
+#### Retorno:
+Não há retorno, a rede apenas aprende utilizando __backpropagation__ e atualiza seus pesos e biases.
+
+Exemplo:
+```py
+input = [10, 2, 4, 4, 100, 90, 3, -1, 9, 10]
+output = [0.0, 0.0, 1.0, 0.0, 0.0]
+
+net.learn(input, output)
+'''
+    A resposta para o input dado deve ser 2. Logo, a rede recebe
+    o output esperado do mar de probabilidades e aprende a diminuir o erro.
+'''
+```
+
+### export
+
+#### Parâmetros:
+- `filename (string)`: O nome do arquivo que você deseja dar para o novo arquivo de dados exportado.
+- `path (string)`: caminho onde você deseja salvar seu arquivo. Coloque o diretório dentro da pasta de destino.
+
+ex.: você poderá encontrar o arquivo neste diretório: `<path><filename>.brain`
+
+#### Retorno:
+Não há um retorno, mas você pode verificar se o arquivo se encontra no caminho especificado. Se sim, você já poderá compartilhar com outras aplicações e reutilizar os dados da sua rede e continuar o seu trabalho de onde parou.
+
+### cost
+
+#### Parâmetros:
+- `input (list of floats)`: Os valores de entrada que serão enviados para a rede.
+- `output (list of floats)`: A probabilidade esperada de cada rótulo estar relacionado com o input. Note que a soma de todas as probabilidades deverá ser igual a __1.0__.
+
+#### Retorno:
+`float`: o valor da média do quadrado das diferenças entre o output esperado pelo usuário e o output gerado pela rede.
+
+Exemplo:
+```py
+input = [10, 2, 4, 4, 100, 90, 3, -1, 9, 10]
+output = [0.0, 0.0, 1.0, 0.0, 0.0]
+
+mse = net.cost(input, output)
+print(mse)
+# 0.027
+```
+
+> O tipo de dado `.brain` é um formato totalmente autoral deste projeto, suas especificações no momento não apresentam documentações, mas você pode conferir manualmente dentro da pasta `Kinho/brain`. Em breve, se necessário, haverá uma documentação mais explícita de como ler/criar este tipo de dado e quais especificações devem-se seguir para ser considerado um formato válido.
```

### Comparing `Kinho-1.0.0/setup.py` & `Kinho-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,56 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import os
-import re
-from setuptools import find_packages, setup
-
-package = 'Kinho'
-
-with open(os.path.join(package, '__init__.py'), 'rb') as f:
-    init_py = f.read().decode('utf-8')
-
-version = re.search(
-    '^__version__ = [\'\"]([^\'\"]+)[\'\"]', init_py, re.MULTILINE
-).group(1)
-author = re.search(
-    '^__author__ = [\'\"]([^\'\"]+)[\'\"]', init_py, re.MULTILINE
-).group(1)
-email = re.search(
-    '^__email__ = [\'\"]([^\'\"]+)[\'\"]', init_py, re.MULTILINE
-).group(1)
-
-setup(
-    name='Kinho',
-    packages=find_packages(),
-    version=version,
-    description='A library to classify images with deep learning.',
-    long_description='The library features the "Neural" model, which is a Convolutional Neural ' \
-        + 'Network (CNN) for image classification. It supports both CPU and GPU, providing excellent performance ' \
-        + 'for large networks. You can also export and import Deep models and continue training on other machines. ' \
-        + 'The exported file is generated in the ".brain" format, which is a proprietary data type of this project. '\
-        + 'For more information, please visit our repository.',
-    author=author,
-    author_email=email,
-    url='https://github.com/kinhosz/Neural',
-    install_requires=[],
-    license='MIT',
-    keywords=['dev', 'web'],
-    classifiers=[
-       'Development Status :: 5 - Production/Stable',
-       'Environment :: GPU',
-       'Environment :: GPU :: NVIDIA CUDA',
-       'Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.0',
-       'License :: OSI Approved :: MIT License',
-       'Natural Language :: Portuguese (Brazilian)',
-       'Natural Language :: English',
-       'Programming Language :: Python',
-       'Programming Language :: Python :: 3',
-       'Topic :: Scientific/Engineering :: Artificial Intelligence',
-       'Topic :: Scientific/Engineering :: Image Processing',
-       'Topic :: Scientific/Engineering :: Image Recognition',
-    ],
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import os
+import re
+from setuptools import find_packages, setup
+
+package = 'Kinho'
+
+with open(os.path.join(package, '__init__.py'), 'rb') as f:
+    init_py = f.read().decode('utf-8')
+
+version = re.search(
+    '^__version__ = [\'\"]([^\'\"]+)[\'\"]', init_py, re.MULTILINE
+).group(1)
+author = re.search(
+    '^__author__ = [\'\"]([^\'\"]+)[\'\"]', init_py, re.MULTILINE
+).group(1)
+email = re.search(
+    '^__email__ = [\'\"]([^\'\"]+)[\'\"]', init_py, re.MULTILINE
+).group(1)
+
+packages = find_packages()
+packages.remove('tests')
+
+setup(
+    name='Kinho',
+    packages=packages,
+    version=version,
+    description='A library to classify images with deep learning.',
+    long_description='The library features the "Neural" model, which is a Convolutional Neural ' \
+        + 'Network (CNN) for image classification. It supports both CPU and GPU, providing excellent performance ' \
+        + 'for large networks. You can also export and import Deep models and continue training on other machines. ' \
+        + 'The exported file is generated in the ".brain" format, which is a proprietary data type of this project. '\
+        + 'For more information, please visit our repository.',
+    author=author,
+    author_email=email,
+    url='https://github.com/kinhosz/Neural',
+    install_requires=[],
+    license='MIT',
+    keywords=['dev', 'web'],
+    classifiers=[
+       'Development Status :: 5 - Production/Stable',
+       'Environment :: GPU',
+       'Environment :: GPU :: NVIDIA CUDA',
+       'Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.0',
+       'License :: OSI Approved :: MIT License',
+       'Natural Language :: Portuguese (Brazilian)',
+       'Natural Language :: English',
+       'Programming Language :: Python',
+       'Programming Language :: Python :: 3',
+       'Topic :: Scientific/Engineering :: Artificial Intelligence',
+       'Topic :: Scientific/Engineering :: Image Processing',
+       'Topic :: Scientific/Engineering :: Image Recognition',
+    ],
 )
```

