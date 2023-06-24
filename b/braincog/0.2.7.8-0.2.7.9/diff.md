# Comparing `tmp/braincog-0.2.7.8-py3-none-any.whl.zip` & `tmp/braincog-0.2.7.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 72380 bytes, number of entries: 55
+Zip file size: 72371 bytes, number of entries: 55
 -rw-rw-r--  2.0 unx      136 b- defN 22-Aug-01 03:28 braincog/__init__.py
 -rw-rw-r--  2.0 unx     4202 b- defN 22-Aug-01 03:28 braincog/utils.py
 -rw-rw-r--  2.0 unx      227 b- defN 22-Aug-01 03:28 braincog/base/__init__.py
 -rw-rw-r--  2.0 unx     4060 b- defN 22-Aug-01 03:28 braincog/base/brainarea/BrainArea.py
 -rw-rw-r--  2.0 unx     2848 b- defN 22-Aug-01 03:28 braincog/base/brainarea/IPL.py
 -rw-rw-r--  2.0 unx     2284 b- defN 22-Aug-01 03:28 braincog/base/brainarea/Insula.py
 -rw-rw-r--  2.0 unx     1329 b- defN 22-Aug-01 03:28 braincog/base/brainarea/PFC.py
@@ -46,12 +46,12 @@
 -rw-rw-r--  2.0 unx     6797 b- defN 22-Aug-01 03:28 braincog/model_zoo/bdmsnn.py
 -rw-rw-r--  2.0 unx    11030 b- defN 22-Aug-01 03:28 braincog/model_zoo/convnet.py
 -rw-rw-r--  2.0 unx     4042 b- defN 22-Aug-01 03:28 braincog/model_zoo/glsnn.py
 -rw-rw-r--  2.0 unx     2554 b- defN 22-Aug-01 03:28 braincog/model_zoo/linearNet.py
 -rw-rw-r--  2.0 unx     3229 b- defN 22-Aug-01 03:28 braincog/model_zoo/nonlinearNet.py
 -rw-rw-r--  2.0 unx     9434 b- defN 22-Aug-01 03:28 braincog/model_zoo/qsnn.py
 -rw-rw-r--  2.0 unx    17166 b- defN 22-Aug-01 03:28 braincog/model_zoo/resnet.py
--rw-rw-r--  2.0 unx     5158 b- defN 22-Aug-05 03:19 braincog-0.2.7.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Aug-05 03:19 braincog-0.2.7.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 22-Aug-05 03:19 braincog-0.2.7.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4903 b- defN 22-Aug-05 03:19 braincog-0.2.7.8.dist-info/RECORD
-55 files, 253663 bytes uncompressed, 64498 bytes compressed:  74.6%
+-rw-rw-r--  2.0 unx     5180 b- defN 22-Aug-05 03:25 braincog-0.2.7.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Aug-05 03:25 braincog-0.2.7.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 22-Aug-05 03:25 braincog-0.2.7.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4903 b- defN 22-Aug-05 03:25 braincog-0.2.7.9.dist-info/RECORD
+55 files, 253685 bytes uncompressed, 64489 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -147,20 +147,20 @@
 
 Filename: braincog/model_zoo/qsnn.py
 Comment: 
 
 Filename: braincog/model_zoo/resnet.py
 Comment: 
 
-Filename: braincog-0.2.7.8.dist-info/METADATA
+Filename: braincog-0.2.7.9.dist-info/METADATA
 Comment: 
 
-Filename: braincog-0.2.7.8.dist-info/WHEEL
+Filename: braincog-0.2.7.9.dist-info/WHEEL
 Comment: 
 
-Filename: braincog-0.2.7.8.dist-info/top_level.txt
+Filename: braincog-0.2.7.9.dist-info/top_level.txt
 Comment: 
 
-Filename: braincog-0.2.7.8.dist-info/RECORD
+Filename: braincog-0.2.7.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `braincog-0.2.7.8.dist-info/METADATA` & `braincog-0.2.7.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincog
-Version: 0.2.7.8
+Version: 0.2.7.9
 Summary: BrainCog is an open source spiking neural network based brain-inspired cognitive intelligence engine for Brain-inspired Artificial Intelligence and brain simulation. More information on braincog can be found on its homepage http://www.brain-cog.network/
 Home-page: UNKNOWN
 Author: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
@@ -67,30 +67,41 @@
 .. figure:: http://www.brain-cog.network/static/image/github_readme/braincog.png
    :alt: image
 
 Brain-Inspired AI
 -----------------
 
 braincog currently provides cognitive functions components that can be
-classified into five categories: \* Perception and Learning \* Decision
-Making \* Motor Control \* Knowledge Representation and Reasoning \*
-Social Cognition
+classified into five categories: 
+
+\* Perception and Learning 
+
+\* Decision Making 
+
+\* Motor Control 
+
+\* Knowledge Representation and Reasoning 
+
+\* Social Cognition
 
 
 .. figure:: https://raw.githubusercontent.com/BrainCog-X/Brain-Cog/main/figures/mirror-test.gif
    :alt: image
    
 .. figure:: https://raw.githubusercontent.com/BrainCog-X/Brain-Cog/main/figures/joy.gif
    :alt: image
 
 Brain Simulation
 ----------------
 
-braincog currently include two parts for brain simulation: \* Brain
-Cognitive Function Simulation \* Multi-scale Brain Structure Simulation
+braincog currently include two parts for brain simulation: 
+
+\* BrainCognitive Function Simulation 
+
+\* Multi-scale Brain Structure Simulation
 
 The anatomical and imaging data is used to support our simulation from
 various aspects.
 
 .. figure:: https://raw.githubusercontent.com/BrainCog-X/Brain-Cog/main/figures/braincog-mouse-brain-model-10s.gif
    :alt: image
 
@@ -158,16 +169,16 @@
    .. code:: shell
 
        cd ./examples/Perception_and_Learning/img_cls/bp 
        python main.py --model cifar_convnet --dataset cifar10 --node-type LIFNode --step 8 --device 0
 
 2. Examples for Event Classification
 
-.. code:: shell
+   .. code:: shell
 
-    cd ./examples/Perception_and_Learning/img_cls/bp 
-    python main.py --model dvs_convnet --node-type LIFNode --dataset dvsc10 --step 10 --batch-size 128 --act-fun QGateGrad --device 0 
+       cd ./examples/Perception_and_Learning/img_cls/bp 
+       python main.py --model dvs_convnet --node-type LIFNode --dataset dvsc10 --step 10 --batch-size 128 --act-fun QGateGrad --device 0 
 
 Other braincog features and tutorials can be found at
 http://www.brain-cog.network/docs/
```

## Comparing `braincog-0.2.7.8.dist-info/RECORD` & `braincog-0.2.7.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -45,11 +45,11 @@
 braincog/model_zoo/bdmsnn.py,sha256=_RMu7L2MdoLnCV6pspol3Vm9kNgVf3PHv7mN0qlKSuY,6797
 braincog/model_zoo/convnet.py,sha256=gn502vbsosv6ZXakhqQeW_xkYAAbyXntXG3nrFJD8j0,11030
 braincog/model_zoo/glsnn.py,sha256=cS4khVMpCnOCT-cz42Vo1-1fL4qt_b5PCmhP6OBrs4s,4042
 braincog/model_zoo/linearNet.py,sha256=hLj-BaS2GQCcua_P-gS4vkBdHqEOAZvZxkQt5PTMlM8,2554
 braincog/model_zoo/nonlinearNet.py,sha256=ZF-Zb8Vks0iiR1tHkgJt4IWKlHBQPW5IsQnOxQJhro8,3229
 braincog/model_zoo/qsnn.py,sha256=43y3PjQLY7zdB_OvEaCxOdSCLs9VYHNKVte3hftSHK8,9434
 braincog/model_zoo/resnet.py,sha256=n4a5AB5Pf1ynAKb6Fk8ey4owauudVSjDMbKKauQQrfM,17166
-braincog-0.2.7.8.dist-info/METADATA,sha256=0WYH6wLniY51vf2wwDcPublImCd3jfnx5rHRec3Zlpw,5158
-braincog-0.2.7.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-braincog-0.2.7.8.dist-info/top_level.txt,sha256=tOjr8b9fZm_bGSw3z1D_dMy88-24IiMzIKVEAvOwF38,9
-braincog-0.2.7.8.dist-info/RECORD,,
+braincog-0.2.7.9.dist-info/METADATA,sha256=j1FWGsJPwihPGvFF0iZRn2GGvdDMP5N3ZZZpHpko02I,5180
+braincog-0.2.7.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+braincog-0.2.7.9.dist-info/top_level.txt,sha256=tOjr8b9fZm_bGSw3z1D_dMy88-24IiMzIKVEAvOwF38,9
+braincog-0.2.7.9.dist-info/RECORD,,
```

