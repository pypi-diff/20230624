# Comparing `tmp/lycoris_lora-0.1.7.dev4.tar.gz` & `tmp/lycoris_lora-0.1.7.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-0.1.7.dev4.tar", last modified: Fri Jun 16 13:19:06 2023, max compression
+gzip compressed data, was "lycoris_lora-0.1.7.dev5.tar", last modified: Sat Jun 24 18:14:40 2023, max compression
```

## Comparing `lycoris_lora-0.1.7.dev4.tar` & `lycoris_lora-0.1.7.dev5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 13:19:06.955444 lycoris_lora-0.1.7.dev4/
--rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev4/Algo.md
--rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev4/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev4/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-06-16 13:19:06.954441 lycoris_lora-0.1.7.dev4/PKG-INFO
--rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 13:19:06.948416 lycoris_lora-0.1.7.dev4/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev4/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev4/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev4/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev4/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev4/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev4/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev4/experiments/time_test.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:19:06.951941 lycoris_lora-0.1.7.dev4/lycoris/
--rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/lycoris/__init__.py
--rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.7.dev4/lycoris/dylora.py
--rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev4/lycoris/ia3.py
--rw-rw-rw-   0        0        0    22402 2023-06-16 11:27:54.000000 lycoris_lora-0.1.7.dev4/lycoris/kohya.py
--rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev4/lycoris/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/lycoris/kohya_utils.py
--rw-rw-rw-   0        0        0     3844 2023-06-16 11:29:39.000000 lycoris_lora-0.1.7.dev4/lycoris/locon.py
--rw-rw-rw-   0        0        0     8557 2023-06-16 13:17:19.000000 lycoris_lora-0.1.7.dev4/lycoris/loha.py
--rw-rw-rw-   0        0        0    10339 2023-06-16 13:18:39.000000 lycoris_lora-0.1.7.dev4/lycoris/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev4/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:19:06.953942 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-06-16 13:19:06.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      773 2023-06-16 13:19:06.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 13:19:06.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-06-16 13:19:06.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 13:19:06.000000 lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 13:19:06.955444 lycoris_lora-0.1.7.dev4/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-06-16 13:19:05.000000 lycoris_lora-0.1.7.dev4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:19:06.954441 lycoris_lora-0.1.7.dev4/tools/
--rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev4/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev4/tools/merge.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:14:40.267951 lycoris_lora-0.1.7.dev5/
+-rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev5/Algo.md
+-rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev5/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev5/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-06-24 18:14:40.267452 lycoris_lora-0.1.7.dev5/PKG-INFO
+-rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 18:14:40.251449 lycoris_lora-0.1.7.dev5/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev5/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev5/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev5/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev5/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev5/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev5/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev5/experiments/time_test.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:14:40.254949 lycoris_lora-0.1.7.dev5/lycoris/
+-rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.7.dev5/lycoris/dylora.py
+-rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev5/lycoris/ia3.py
+-rw-rw-rw-   0        0        0    22402 2023-06-16 11:27:54.000000 lycoris_lora-0.1.7.dev5/lycoris/kohya.py
+-rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev5/lycoris/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/lycoris/kohya_utils.py
+-rw-rw-rw-   0        0        0     3844 2023-06-16 11:29:39.000000 lycoris_lora-0.1.7.dev5/lycoris/locon.py
+-rw-rw-rw-   0        0        0     8518 2023-06-24 18:13:14.000000 lycoris_lora-0.1.7.dev5/lycoris/loha.py
+-rw-rw-rw-   0        0        0    10339 2023-06-16 13:18:39.000000 lycoris_lora-0.1.7.dev5/lycoris/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev5/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:14:40.266451 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-06-24 18:14:40.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2023-06-24 18:14:40.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:14:40.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-06-24 18:14:40.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-24 18:14:40.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 18:14:40.267951 lycoris_lora-0.1.7.dev5/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-06-24 18:14:34.000000 lycoris_lora-0.1.7.dev5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:14:40.266951 lycoris_lora-0.1.7.dev5/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev5/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev5/tools/merge.py
```

### Comparing `lycoris_lora-0.1.7.dev4/.gitignore` & `lycoris_lora-0.1.7.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/Algo.md` & `lycoris_lora-0.1.7.dev5/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/Change.md` & `lycoris_lora-0.1.7.dev5/Change.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/Demo.md` & `lycoris_lora-0.1.7.dev5/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/LICENSE.md` & `lycoris_lora-0.1.7.dev5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/README.md` & `lycoris_lora-0.1.7.dev5/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/experiments/better_conv.py` & `lycoris_lora-0.1.7.dev5/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/experiments/better_conv_extract.py` & `lycoris_lora-0.1.7.dev5/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/experiments/concept_neuron.py` & `lycoris_lora-0.1.7.dev5/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/experiments/locon_extract_test.py` & `lycoris_lora-0.1.7.dev5/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/experiments/locon_merge_test.py` & `lycoris_lora-0.1.7.dev5/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/experiments/singular_value_test.py` & `lycoris_lora-0.1.7.dev5/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/experiments/sparse_bias_test.py` & `lycoris_lora-0.1.7.dev5/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/experiments/time_test.py` & `lycoris_lora-0.1.7.dev5/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/lycoris/dylora.py` & `lycoris_lora-0.1.7.dev5/lycoris/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/lycoris/ia3.py` & `lycoris_lora-0.1.7.dev5/lycoris/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/lycoris/kohya.py` & `lycoris_lora-0.1.7.dev5/lycoris/kohya.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/lycoris/kohya_model_utils.py` & `lycoris_lora-0.1.7.dev5/lycoris/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/lycoris/kohya_utils.py` & `lycoris_lora-0.1.7.dev5/lycoris/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/lycoris/locon.py` & `lycoris_lora-0.1.7.dev5/lycoris/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/lycoris/loha.py` & `lycoris_lora-0.1.7.dev5/lycoris/loha.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,20 +41,18 @@
         
         return orig_weight + rebuild1*rebuild2*scale
 
     @staticmethod
     def backward(ctx, grad_out):
         (t1, w1a, w1b, t2, w2a, w2b, scale) = ctx.saved_tensors
         
-        grad_out = grad_out*scale
-        
         temp = torch.einsum('i j k l, j r -> i r k l', t2, w2b)
         rebuild = torch.einsum('i j k l, i r -> r j k l', temp, w2a)
         
-        grad_w = rebuild*grad_out
+        grad_w = rebuild*grad_out*scale
         del rebuild
         
         grad_w1a = torch.einsum('r j k l, i j k l -> r i', temp, grad_w)
         grad_temp = torch.einsum('i j k l, i r -> r j k l', grad_w, w1a.T)
         del grad_w, temp
         
         grad_w1b = torch.einsum('i r k l, i j k l -> r j', t1, grad_temp)
```

### Comparing `lycoris_lora-0.1.7.dev4/lycoris/lokr.py` & `lycoris_lora-0.1.7.dev5/lycoris/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/lycoris/utils.py` & `lycoris_lora-0.1.7.dev5/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/setup.py` & `lycoris_lora-0.1.7.dev5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lycoris_lora',
     packages=['lycoris'],
-    version='0.1.7.dev4',
+    version='0.1.7.dev5',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-0.1.7.dev4/tools/extract_locon.py` & `lycoris_lora-0.1.7.dev5/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev4/tools/merge.py` & `lycoris_lora-0.1.7.dev5/tools/merge.py`

 * *Files identical despite different names*

