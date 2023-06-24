# Comparing `tmp/kerasfuse-0.0.1.tar.gz` & `tmp/kerasfuse-0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerasfuse-0.0.1.tar", max compression
+gzip compressed data, was "kerasfuse-0.1a0.tar", max compression
```

## Comparing `kerasfuse-0.0.1.tar` & `kerasfuse-0.1a0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/LICENSE
--rw-r--r--   0        0        0     2355 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/README.md
--rw-r--r--   0        0        0      697 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/__init__.py
--rw-r--r--   0        0        0     4238 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/dataset/data_augmentation.py
--rw-r--r--   0        0        0     3015 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/dataset/generate_class_weights.py
--rw-r--r--   0        0        0     1781 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/dataset/load_images.py
--rw-r--r--   0        0        0     1192 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/evaluate.py
--rw-r--r--   0        0        0        0 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/losses/__init__.py
--rw-r--r--   0        0        0      502 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/losses/dice_loss.py
--rw-r--r--   0        0        0      697 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/losses/focal_loss.py
--rw-r--r--   0        0        0      973 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/losses/loss_functions.py
--rw-r--r--   0        0        0     3337 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/models/blocks/__init__.py
--rw-r--r--   0        0        0     7097 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/models/blocks/autoencoder.py
--rw-r--r--   0        0        0     2538 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/models/blocks/mlp.py
--rw-r--r--   0        0        0     2914 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/models/dense_net.py
--rw-r--r--   0        0        0    11069 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/models/layers/convutils.py
--rw-r--r--   0        0        0        6 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/models/layers/readme.md
--rw-r--r--   0        0        0     3776 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/models/mobile_net.py
--rw-r--r--   0        0        0     1785 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/models/res_net.py
--rw-r--r--   0        0        0     3070 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/models/u_net.py
--rw-r--r--   0        0        0     2476 2023-06-20 17:53:41.052036 kerasfuse-0.0.1/kerasfuse/models/v-net.py
--rw-r--r--   0        0        0     2654 2023-06-20 17:53:41.056036 kerasfuse-0.0.1/kerasfuse/train.py
--rw-r--r--   0        0        0     3182 2023-06-20 17:53:41.056036 kerasfuse-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3758 1970-01-01 00:00:00.000000 kerasfuse-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/LICENSE
+-rw-r--r--   0        0        0     2026 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/README.md
+-rw-r--r--   0        0        0      697 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/kerasfuse/__init__.py
+-rw-r--r--   0        0        0     4238 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/kerasfuse/dataset/data_augmentation.py
+-rw-r--r--   0        0        0     3015 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/kerasfuse/dataset/generate_class_weights.py
+-rw-r--r--   0        0        0     1781 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/kerasfuse/dataset/load_images.py
+-rw-r--r--   0        0        0     1192 2023-06-24 11:53:30.310712 kerasfuse-0.1a0/kerasfuse/evaluate.py
+-rw-r--r--   0        0        0        0 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/losses/__init__.py
+-rw-r--r--   0        0        0      502 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/losses/dice_loss.py
+-rw-r--r--   0        0        0      697 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/losses/focal_loss.py
+-rw-r--r--   0        0        0      973 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/losses/loss_functions.py
+-rw-r--r--   0        0        0     3337 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/blocks/__init__.py
+-rw-r--r--   0        0        0     7097 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/blocks/autoencoder.py
+-rw-r--r--   0        0        0     2538 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/blocks/mlp.py
+-rw-r--r--   0        0        0     2914 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/dense_net.py
+-rw-r--r--   0        0        0    11069 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/layers/convutils.py
+-rw-r--r--   0        0        0        6 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/layers/readme.md
+-rw-r--r--   0        0        0     3776 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/mobile_net.py
+-rw-r--r--   0        0        0     1785 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/res_net.py
+-rw-r--r--   0        0        0     3070 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/u_net.py
+-rw-r--r--   0        0        0     2476 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/models/v-net.py
+-rw-r--r--   0        0        0     2654 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/kerasfuse/train.py
+-rw-r--r--   0        0        0     3182 2023-06-24 11:53:30.314712 kerasfuse-0.1a0/pyproject.toml
+-rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 kerasfuse-0.1a0/PKG-INFO
```

### Comparing `kerasfuse-0.0.1/LICENSE` & `kerasfuse-0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/README.md` & `kerasfuse-0.1a0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,148 +1,127 @@
 00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000010: 223e 0a3c 7069 6374 7572 653e 0a20 203c  ">.<picture>.  <
-00000020: 736f 7572 6365 206d 6564 6961 3d22 2870  source media="(p
-00000030: 7265 6665 7273 2d63 6f6c 6f72 2d73 6368  refers-color-sch
-00000040: 656d 653a 2064 6172 6b29 2220 7372 6373  eme: dark)" srcs
-00000050: 6574 3d22 6874 7470 733a 2f2f 6769 7468  et="https://gith
-00000060: 7562 2e63 6f6d 2f61 7979 7563 6564 656d  ub.com/ayyucedem
-00000070: 6972 6261 732f 4b65 7261 7346 7573 652f  irbas/KerasFuse/
-00000080: 6173 7365 7473 2f38 3032 3331 3530 2f34  assets/8023150/4
-00000090: 3164 3838 3830 642d 3831 3137 2d34 3438  1d8880d-8117-448
-000000a0: 622d 6137 3235 2d32 6237 3264 3264 3038  b-a725-2b72d2d08
-000000b0: 6265 6222 3e0a 2020 3c73 6f75 7263 6520  beb">.  <source 
-000000c0: 6d65 6469 613d 2228 7072 6566 6572 732d  media="(prefers-
-000000d0: 636f 6c6f 722d 7363 6865 6d65 3a20 6c69  color-scheme: li
-000000e0: 6768 7429 2220 7372 6373 6574 3d22 6874  ght)" srcset="ht
-000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000100: 2f61 7979 7563 6564 656d 6972 6261 732f  /ayyucedemirbas/
-00000110: 4b65 7261 7346 7573 652f 6173 7365 7473  KerasFuse/assets
-00000120: 2f38 3032 3331 3530 2f34 3164 3838 3830  /8023150/41d8880
-00000130: 642d 3831 3137 2d34 3438 622d 6137 3235  d-8117-448b-a725
-00000140: 2d32 6237 3264 3264 3038 6265 6222 3e0a  -2b72d2d08beb">.
-00000150: 2020 3c69 6d67 2061 6c74 3d22 4b65 7261    <img alt="Kera
-00000160: 7346 7573 6522 2073 7263 3d22 6874 7470  sFuse" src="http
-00000170: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00000180: 7979 7563 6564 656d 6972 6261 732f 4b65  yyucedemirbas/Ke
-00000190: 7261 7346 7573 6522 3e0a 3c2f 7069 6374  rasFuse">.</pict
-000001a0: 7572 653e 0a3c 2f70 3e0a 0a3c 6831 2061  ure>.</p>..<h1 a
-000001b0: 6c69 676e 3d22 6365 6e74 6572 223e 4b65  lign="center">Ke
-000001c0: 7261 7346 7573 653c 2f68 313e 0a0a 3c70  rasFuse</h1>..<p
-000001d0: 3e0a 2020 3c69 6d67 2061 6c74 3d22 4769  >.  <img alt="Gi
-000001e0: 7448 7562 2220 7372 633d 2268 7474 7073  tHub" src="https
-000001f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000200: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
-00000210: 2f61 7979 7563 6564 656d 6972 6261 732f  /ayyucedemirbas/
-00000220: 4b65 7261 7366 7573 6522 3e0a 2020 3c69  Kerasfuse">.  <i
-00000230: 6d67 2061 6c74 3d22 5079 7468 6f6e 3322  mg alt="Python3"
-00000240: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000250: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000260: 6765 2f50 7974 686f 6e2d 332e 382e 3120  ge/Python-3.8.1 
-00000270: 7c20 332e 3920 7c20 332e 3130 207c 2033  | 3.9 | 3.10 | 3
-00000280: 2e31 312d 3337 3736 4142 2e73 7667 3f6c  .11-3776AB.svg?l
-00000290: 6f67 6f3d 5079 7468 6f6e 266c 6f67 6f43  ogo=Python&logoC
-000002a0: 6f6c 6f72 3d77 6869 7465 222f 3e0a 2020  olor=white"/>.  
-000002b0: 3c69 6d67 2061 6c74 3d22 5465 6e73 6f72  <img alt="Tensor
-000002c0: 666c 6f77 2220 7372 633d 2268 7474 7073  flow" src="https
-000002d0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000002e0: 6f2f 6261 6467 652f 5465 6e73 6f72 666c  o/badge/Tensorfl
-000002f0: 6f77 2d76 322e 3132 2e30 2d25 3233 4646  ow-v2.12.0-%23FF
-00000300: 3646 3030 2e73 7667 3f6c 6f67 6f3d 5465  6F00.svg?logo=Te
-00000310: 6e73 6f72 666c 6f77 266c 6f67 6f43 6f6c  nsorflow&logoCol
-00000320: 6f72 3d77 6869 7465 222f 3e0a 2020 3c69  or=white"/>.  <i
-00000330: 6d67 2061 6c74 3d22 4b65 7261 7322 2073  mg alt="Keras" s
-00000340: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000350: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000360: 2f4b 6572 6173 2d76 322e 3132 2e30 2d25  /Keras-v2.12.0-%
-00000370: 3233 4430 3030 3030 2e73 7667 3f6c 6f67  23D00000.svg?log
-00000380: 6f3d 4b65 7261 7326 6c6f 676f 436f 6c6f  o=Keras&logoColo
-00000390: 723d 7768 6974 6522 2f3e 0a20 203c 696d  r=white"/>.  <im
-000003a0: 6720 616c 743d 2242 6c61 636b 2220 7372  g alt="Black" sr
-000003b0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-000003c0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-000003d0: 636f 6465 2532 3073 7479 6c65 2d62 6c61  code%20style-bla
-000003e0: 636b 2d62 6c61 636b 222f 3e0a 2020 3c69  ck-black"/>.  <i
-000003f0: 6d67 2061 6c74 3d22 6973 6f72 7422 2073  mg alt="isort" s
-00000400: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000410: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000420: 2f69 736f 7274 2d63 6865 636b 6564 2d79  /isort-checked-y
-00000430: 656c 6c6f 7722 2f3e 0a3c 2f70 3e0a 0a3c  ellow"/>.</p>..<
-00000440: 6834 2061 6c69 676e 3d22 6365 6e74 6572  h4 align="center
-00000450: 223e f09f 9aa7 2057 6172 6e69 6e67 2074  ">.... Warning t
-00000460: 6869 7320 7072 6f6a 6563 7420 6973 2075  his project is u
-00000470: 6e64 6572 2068 6561 7679 2064 6576 656c  nder heavy devel
-00000480: 6f70 6d65 6e74 2061 6e64 206e 6f74 2072  opment and not r
-00000490: 6561 6479 2066 6f72 2070 726f 6475 6374  eady for product
-000004a0: 696f 6e2e 2041 4249 2063 6861 6e67 6573  ion. ABI changes
-000004b0: 2063 616e 2068 6170 7065 6e20 6672 6571   can happen freq
-000004c0: 7565 6e74 6c79 2075 6e74 696c 2072 6561  uently until rea
-000004d0: 6368 2073 7461 626c 6520 7665 7273 696f  ch stable versio
-000004e0: 6e20 f09f 9aa7 203c 2f68 343e 0a0a 0a4b  n .... </h4>...K
-000004f0: 6572 6173 4675 7365 2069 7320 6120 5079  erasFuse is a Py
-00000500: 7468 6f6e 206c 6962 7261 7279 2074 6861  thon library tha
-00000510: 7420 636f 6d62 696e 6573 2074 6865 2070  t combines the p
-00000520: 6f77 6572 206f 6620 5465 6e73 6f72 466c  ower of TensorFl
-00000530: 6f77 2061 6e64 204b 6572 6173 2077 6974  ow and Keras wit
-00000540: 6820 7661 7269 6f75 7320 636f 6d70 7574  h various comput
-00000550: 6572 2076 6973 696f 6e20 7465 6368 6e69  er vision techni
-00000560: 7175 6573 2066 6f72 206d 6564 6963 616c  ques for medical
-00000570: 2069 6d61 6765 2061 6e61 6c79 7369 7320   image analysis 
-00000580: 7461 736b 732e 2049 7420 7072 6f76 6964  tasks. It provid
-00000590: 6573 2061 2063 6f6c 6c65 6374 696f 6e20  es a collection 
-000005a0: 6f66 206d 6f64 756c 6573 2061 6e64 2066  of modules and f
-000005b0: 756e 6374 696f 6e73 2074 6f20 6661 6369  unctions to faci
-000005c0: 6c69 7461 7465 2074 6865 2064 6576 656c  litate the devel
-000005d0: 6f70 6d65 6e74 206f 6620 6465 6570 206c  opment of deep l
-000005e0: 6561 726e 696e 6720 6d6f 6465 6c73 2069  earning models i
-000005f0: 6e20 5465 6e73 6f72 466c 6f77 204b 6572  n TensorFlow Ker
-00000600: 6173 2066 6f72 2074 6173 6b73 2073 7563  as for tasks suc
-00000610: 6820 6173 2069 6d61 6765 2073 6567 6d65  h as image segme
-00000620: 6e74 6174 696f 6e2c 2063 6c61 7373 6966  ntation, classif
-00000630: 6963 6174 696f 6e2c 2061 6e64 206d 6f72  ication, and mor
-00000640: 652e 0a0a 0a0a 2323 2047 6574 7469 6e67  e.....## Getting
-00000650: 2053 7461 7274 6564 0a0a 2323 2320 496e   Started..### In
-00000660: 7374 616c 6c61 7469 6f6e 0a0a 2323 2323  stallation..####
-00000670: 2050 6f65 7472 7920 496e 7374 616c 6c61   Poetry Installa
-00000680: 7469 6f6e 0a0a 6060 6062 6173 680a 706f  tion..```bash.po
-00000690: 6574 7279 2069 6e73 7461 6c6c 0a70 6f65  etry install.poe
-000006a0: 7472 7920 7368 656c 6c0a 6060 600a 0a23  try shell.```..#
-000006b0: 2323 2320 5469 700a 0a49 6620 796f 7520  ### Tip..If you 
-000006c0: 6861 7665 206d 756c 7469 706c 6520 5079  have multiple Py
-000006d0: 7468 6f6e 2076 6572 7369 6f6e 7320 6f6e  thon versions on
-000006e0: 2079 6f75 7220 7379 7374 656d 2c20 796f   your system, yo
-000006f0: 7520 6361 6e20 7365 7420 796f 7572 2050  u can set your P
-00000700: 7974 686f 6e20 7665 7273 696f 6e20 6279  ython version by
-00000710: 2075 7369 6e67 2060 706f 6574 7279 2065   using `poetry e
-00000720: 6e76 6020 2e20 4865 7265 2773 2061 6e20  nv` . Here's an 
-00000730: 6578 616d 706c 6520 6f66 2068 6f77 2074  example of how t
-00000740: 6f20 7573 6520 6974 3a0a 0a60 6060 6261  o use it:..```ba
-00000750: 7368 0a70 6f65 7472 7920 656e 7620 7573  sh.poetry env us
-00000760: 6520 7079 7468 6f6e 332e 3130 0a60 6060  e python3.10.```
-00000770: 0a0a 4d6f 7265 2064 6574 6169 6c73 2061  ..More details a
-00000780: 740a 5b70 6f65 7472 792d 7377 6974 6368  t.[poetry-switch
-00000790: 696e 672d 6265 7477 6565 6e2d 656e 7669  ing-between-envi
-000007a0: 726f 6e6d 656e 7473 5d28 6874 7470 733a  ronments](https:
-000007b0: 2f2f 7079 7468 6f6e 2d70 6f65 7472 792e  //python-poetry.
-000007c0: 6f72 672f 646f 6373 2f6d 616e 6167 696e  org/docs/managin
-000007d0: 672d 656e 7669 726f 6e6d 656e 7473 2f23  g-environments/#
-000007e0: 7377 6974 6368 696e 672d 6265 7477 6565  switching-betwee
-000007f0: 6e2d 656e 7669 726f 6e6d 656e 7473 290a  n-environments).
-00000800: 0a23 2323 2320 5069 7020 496e 7374 616c  .#### Pip Instal
-00000810: 6c61 7469 6f6e 730a 0a60 6060 6261 7368  lations..```bash
-00000820: 0a70 7974 686f 6e33 202d 6d20 7665 6e76  .python3 -m venv
-00000830: 202e 7665 6e76 0a73 6f75 7263 6520 2e76   .venv.source .v
-00000840: 656e 762f 6269 6e2f 6163 7469 7661 7465  env/bin/activate
-00000850: 0a70 6970 3320 696e 7374 616c 6c20 2d72  .pip3 install -r
-00000860: 2072 6571 7569 7265 6d65 6e74 732e 7478   requirements.tx
-00000870: 740a 6060 600a 0a46 6f72 204d 6163 4f53  t.```..For MacOS
-00000880: 0a0a 6060 6062 6173 680a 7079 7468 6f6e  ..```bash.python
-00000890: 3320 2d6d 2076 656e 7620 2e76 656e 760a  3 -m venv .venv.
-000008a0: 736f 7572 6365 202e 7665 6e76 2f62 696e  source .venv/bin
-000008b0: 2f61 6374 6976 6174 650a 7069 7033 2069  /activate.pip3 i
-000008c0: 6e73 7461 6c6c 202d 7220 7265 7175 6972  nstall -r requir
-000008d0: 656d 656e 7473 2d6d 6163 6f73 2e74 7874  ements-macos.txt
-000008e0: 0a60 6060 0a0a 2323 204c 6963 656e 7365  .```..## License
-000008f0: 0a0a 5468 6973 2070 726f 6a65 6374 2069  ..This project i
-00000900: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
-00000910: 2074 6865 2074 6572 6d73 206f 6620 7468   the terms of th
-00000920: 6520 4750 4c2d 332e 3020 6c69 6365 6e73  e GPL-3.0 licens
-00000930: 652e 0a                                  e..
+00000010: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+00000020: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000030: 2f61 7979 7563 6564 656d 6972 6261 732f  /ayyucedemirbas/
+00000040: 4b65 7261 7346 7573 6522 3e3c 696d 6720  KerasFuse"><img 
+00000050: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00000060: 6875 622e 636f 6d2f 6179 7975 6365 6465  hub.com/ayyucede
+00000070: 6d69 7262 6173 2f4b 6572 6173 4675 7365  mirbas/KerasFuse
+00000080: 2f61 7373 6574 732f 3830 3233 3135 302f  /assets/8023150/
+00000090: 3431 6438 3838 3064 2d38 3131 372d 3434  41d8880d-8117-44
+000000a0: 3862 2d61 3732 352d 3262 3732 6432 6430  8b-a725-2b72d2d0
+000000b0: 3862 6562 2220 616c 743d 224b 6572 6173  8beb" alt="Keras
+000000c0: 4675 7365 223e 3c2f 613e 0a3c 2f70 3e0a  Fuse"></a>.</p>.
+000000d0: 0a3c 6831 2061 6c69 676e 3d22 6365 6e74  .<h1 align="cent
+000000e0: 6572 223e 4b65 7261 7346 7573 653c 2f68  er">KerasFuse</h
+000000f0: 313e 0a0a 3c70 3e0a 2020 3c69 6d67 2061  1>..<p>.  <img a
+00000100: 6c74 3d22 4769 7448 7562 2220 7372 633d  lt="GitHub" src=
+00000110: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000120: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+00000130: 6963 656e 7365 2f61 7979 7563 6564 656d  icense/ayyucedem
+00000140: 6972 6261 732f 4b65 7261 7366 7573 6522  irbas/Kerasfuse"
+00000150: 3e0a 2020 3c69 6d67 2061 6c74 3d22 5079  >.  <img alt="Py
+00000160: 7468 6f6e 3322 2073 7263 3d22 6874 7470  thon3" src="http
+00000170: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000180: 696f 2f62 6164 6765 2f50 7974 686f 6e2d  io/badge/Python-
+00000190: 332e 382e 3120 7c20 332e 3920 7c20 332e  3.8.1 | 3.9 | 3.
+000001a0: 3130 207c 2033 2e31 312d 3337 3736 4142  10 | 3.11-3776AB
+000001b0: 2e73 7667 3f6c 6f67 6f3d 5079 7468 6f6e  .svg?logo=Python
+000001c0: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
+000001d0: 222f 3e0a 2020 3c69 6d67 2061 6c74 3d22  "/>.  <img alt="
+000001e0: 5465 6e73 6f72 666c 6f77 2220 7372 633d  Tensorflow" src=
+000001f0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000200: 656c 6473 2e69 6f2f 6261 6467 652f 5465  elds.io/badge/Te
+00000210: 6e73 6f72 666c 6f77 2d76 322e 3132 2e30  nsorflow-v2.12.0
+00000220: 2d25 3233 4646 3646 3030 2e73 7667 3f6c  -%23FF6F00.svg?l
+00000230: 6f67 6f3d 5465 6e73 6f72 666c 6f77 266c  ogo=Tensorflow&l
+00000240: 6f67 6f43 6f6c 6f72 3d77 6869 7465 222f  ogoColor=white"/
+00000250: 3e0a 2020 3c69 6d67 2061 6c74 3d22 4b65  >.  <img alt="Ke
+00000260: 7261 7322 2073 7263 3d22 6874 7470 733a  ras" src="https:
+00000270: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000280: 2f62 6164 6765 2f4b 6572 6173 2d76 322e  /badge/Keras-v2.
+00000290: 3132 2e30 2d25 3233 4430 3030 3030 2e73  12.0-%23D00000.s
+000002a0: 7667 3f6c 6f67 6f3d 4b65 7261 7326 6c6f  vg?logo=Keras&lo
+000002b0: 676f 436f 6c6f 723d 7768 6974 6522 2f3e  goColor=white"/>
+000002c0: 0a20 203c 696d 6720 616c 743d 2242 6c61  .  <img alt="Bla
+000002d0: 636b 2220 7372 633d 2268 7474 7073 3a2f  ck" src="https:/
+000002e0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000002f0: 6261 6467 652f 636f 6465 2532 3073 7479  badge/code%20sty
+00000300: 6c65 2d62 6c61 636b 2d62 6c61 636b 222f  le-black-black"/
+00000310: 3e0a 2020 3c69 6d67 2061 6c74 3d22 6973  >.  <img alt="is
+00000320: 6f72 7422 2073 7263 3d22 6874 7470 733a  ort" src="https:
+00000330: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000340: 2f62 6164 6765 2f69 736f 7274 2d63 6865  /badge/isort-che
+00000350: 636b 6564 2d79 656c 6c6f 7722 2f3e 0a3c  cked-yellow"/>.<
+00000360: 2f70 3e0a 0a3c 6834 2061 6c69 676e 3d22  /p>..<h4 align="
+00000370: 6365 6e74 6572 223e f09f 9aa7 2057 6172  center">.... War
+00000380: 6e69 6e67 2074 6869 7320 7072 6f6a 6563  ning this projec
+00000390: 7420 6973 2075 6e64 6572 2068 6561 7679  t is under heavy
+000003a0: 2064 6576 656c 6f70 6d65 6e74 2061 6e64   development and
+000003b0: 206e 6f74 2072 6561 6479 2066 6f72 2070   not ready for p
+000003c0: 726f 6475 6374 696f 6e2e 2041 4249 2063  roduction. ABI c
+000003d0: 6861 6e67 6573 2063 616e 2068 6170 7065  hanges can happe
+000003e0: 6e20 6672 6571 7565 6e74 6c79 2075 6e74  n frequently unt
+000003f0: 696c 2072 6561 6368 2073 7461 626c 6520  il reach stable 
+00000400: 7665 7273 696f 6e20 f09f 9aa7 203c 2f68  version .... </h
+00000410: 343e 0a0a 0a4b 6572 6173 4675 7365 2069  4>...KerasFuse i
+00000420: 7320 6120 5079 7468 6f6e 206c 6962 7261  s a Python libra
+00000430: 7279 2074 6861 7420 636f 6d62 696e 6573  ry that combines
+00000440: 2074 6865 2070 6f77 6572 206f 6620 5465   the power of Te
+00000450: 6e73 6f72 466c 6f77 2061 6e64 204b 6572  nsorFlow and Ker
+00000460: 6173 2077 6974 6820 7661 7269 6f75 7320  as with various 
+00000470: 636f 6d70 7574 6572 2076 6973 696f 6e20  computer vision 
+00000480: 7465 6368 6e69 7175 6573 2066 6f72 206d  techniques for m
+00000490: 6564 6963 616c 2069 6d61 6765 2061 6e61  edical image ana
+000004a0: 6c79 7369 7320 7461 736b 732e 2049 7420  lysis tasks. It 
+000004b0: 7072 6f76 6964 6573 2061 2063 6f6c 6c65  provides a colle
+000004c0: 6374 696f 6e20 6f66 206d 6f64 756c 6573  ction of modules
+000004d0: 2061 6e64 2066 756e 6374 696f 6e73 2074   and functions t
+000004e0: 6f20 6661 6369 6c69 7461 7465 2074 6865  o facilitate the
+000004f0: 2064 6576 656c 6f70 6d65 6e74 206f 6620   development of 
+00000500: 6465 6570 206c 6561 726e 696e 6720 6d6f  deep learning mo
+00000510: 6465 6c73 2069 6e20 5465 6e73 6f72 466c  dels in TensorFl
+00000520: 6f77 204b 6572 6173 2066 6f72 2074 6173  ow Keras for tas
+00000530: 6b73 2073 7563 6820 6173 2069 6d61 6765  ks such as image
+00000540: 2073 6567 6d65 6e74 6174 696f 6e2c 2063   segmentation, c
+00000550: 6c61 7373 6966 6963 6174 696f 6e2c 2061  lassification, a
+00000560: 6e64 206d 6f72 652e 0a0a 0a0a 2323 2047  nd more.....## G
+00000570: 6574 7469 6e67 2053 7461 7274 6564 0a0a  etting Started..
+00000580: 2323 2320 496e 7374 616c 6c61 7469 6f6e  ### Installation
+00000590: 0a0a 2323 2323 2050 6f65 7472 7920 496e  ..#### Poetry In
+000005a0: 7374 616c 6c61 7469 6f6e 0a0a 6060 6062  stallation..```b
+000005b0: 6173 680a 706f 6574 7279 2069 6e73 7461  ash.poetry insta
+000005c0: 6c6c 0a70 6f65 7472 7920 7368 656c 6c0a  ll.poetry shell.
+000005d0: 6060 600a 0a23 2323 2320 5469 700a 0a49  ```..#### Tip..I
+000005e0: 6620 796f 7520 6861 7665 206d 756c 7469  f you have multi
+000005f0: 706c 6520 5079 7468 6f6e 2076 6572 7369  ple Python versi
+00000600: 6f6e 7320 6f6e 2079 6f75 7220 7379 7374  ons on your syst
+00000610: 656d 2c20 796f 7520 6361 6e20 7365 7420  em, you can set 
+00000620: 796f 7572 2050 7974 686f 6e20 7665 7273  your Python vers
+00000630: 696f 6e20 6279 2075 7369 6e67 2060 706f  ion by using `po
+00000640: 6574 7279 2065 6e76 6020 2e20 4865 7265  etry env` . Here
+00000650: 2773 2061 6e20 6578 616d 706c 6520 6f66  's an example of
+00000660: 2068 6f77 2074 6f20 7573 6520 6974 3a0a   how to use it:.
+00000670: 0a60 6060 6261 7368 0a70 6f65 7472 7920  .```bash.poetry 
+00000680: 656e 7620 7573 6520 7079 7468 6f6e 332e  env use python3.
+00000690: 3130 0a60 6060 0a0a 4d6f 7265 2064 6574  10.```..More det
+000006a0: 6169 6c73 2061 740a 5b70 6f65 7472 792d  ails at.[poetry-
+000006b0: 7377 6974 6368 696e 672d 6265 7477 6565  switching-betwee
+000006c0: 6e2d 656e 7669 726f 6e6d 656e 7473 5d28  n-environments](
+000006d0: 6874 7470 733a 2f2f 7079 7468 6f6e 2d70  https://python-p
+000006e0: 6f65 7472 792e 6f72 672f 646f 6373 2f6d  oetry.org/docs/m
+000006f0: 616e 6167 696e 672d 656e 7669 726f 6e6d  anaging-environm
+00000700: 656e 7473 2f23 7377 6974 6368 696e 672d  ents/#switching-
+00000710: 6265 7477 6565 6e2d 656e 7669 726f 6e6d  between-environm
+00000720: 656e 7473 290a 0a23 2323 2320 5069 7020  ents)..#### Pip 
+00000730: 496e 7374 616c 6c61 7469 6f6e 730a 0a60  Installations..`
+00000740: 6060 6261 7368 0a70 7974 686f 6e33 202d  ``bash.python3 -
+00000750: 6d20 7665 6e76 202e 7665 6e76 0a73 6f75  m venv .venv.sou
+00000760: 7263 6520 2e76 656e 762f 6269 6e2f 6163  rce .venv/bin/ac
+00000770: 7469 7661 7465 0a70 6970 3320 696e 7374  tivate.pip3 inst
+00000780: 616c 6c20 2d72 2072 6571 7569 7265 6d65  all -r requireme
+00000790: 6e74 732e 7478 740a 6060 600a 0a23 2320  nts.txt.```..## 
+000007a0: 4c69 6365 6e73 650a 0a54 6869 7320 7072  License..This pr
+000007b0: 6f6a 6563 7420 6973 206c 6963 656e 7365  oject is license
+000007c0: 6420 756e 6465 7220 7468 6520 7465 726d  d under the term
+000007d0: 7320 6f66 2074 6865 2047 504c 2d33 2e30  s of the GPL-3.0
+000007e0: 206c 6963 656e 7365 2e0a                  license..
```

### Comparing `kerasfuse-0.0.1/kerasfuse/__init__.py` & `kerasfuse-0.1a0/kerasfuse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-__version__ = "0.0.1"
+__version__ = "0.1a0"
```

### Comparing `kerasfuse-0.0.1/kerasfuse/dataset/data_augmentation.py` & `kerasfuse-0.1a0/kerasfuse/dataset/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/dataset/generate_class_weights.py` & `kerasfuse-0.1a0/kerasfuse/dataset/generate_class_weights.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/dataset/load_images.py` & `kerasfuse-0.1a0/kerasfuse/dataset/load_images.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/evaluate.py` & `kerasfuse-0.1a0/kerasfuse/evaluate.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/losses/focal_loss.py` & `kerasfuse-0.1a0/kerasfuse/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/losses/loss_functions.py` & `kerasfuse-0.1a0/kerasfuse/losses/loss_functions.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/metrics/metrics.py` & `kerasfuse-0.1a0/kerasfuse/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/models/blocks/autoencoder.py` & `kerasfuse-0.1a0/kerasfuse/models/blocks/autoencoder.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/models/blocks/mlp.py` & `kerasfuse-0.1a0/kerasfuse/models/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/models/dense_net.py` & `kerasfuse-0.1a0/kerasfuse/models/dense_net.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/models/layers/convutils.py` & `kerasfuse-0.1a0/kerasfuse/models/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/models/mobile_net.py` & `kerasfuse-0.1a0/kerasfuse/models/mobile_net.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/models/res_net.py` & `kerasfuse-0.1a0/kerasfuse/models/res_net.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/models/u_net.py` & `kerasfuse-0.1a0/kerasfuse/models/u_net.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/models/v-net.py` & `kerasfuse-0.1a0/kerasfuse/models/v-net.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/kerasfuse/train.py` & `kerasfuse-0.1a0/kerasfuse/train.py`

 * *Files identical despite different names*

### Comparing `kerasfuse-0.0.1/pyproject.toml` & `kerasfuse-0.1a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "KerasFuse"
-version = "0.0.1"
+version = "0.1a0"
 description = "KerasFuse is a Python library that combines the power of TensorFlow and Keras with various computer vision techniques for medical image analysis tasks."
 authors = ["Ayyuce Demirbas <a.ayyuced@gmail.com>"]
 maintainers = ["Ayyuce Demirbas <a.ayyuced@gmail.com>"]
 readme = "README.md"
 packages = [{include = "kerasfuse"}]
 homepage = "https://github.com/ayyucedemirbas/KerasFuse"
 repository = "https://github.com/ayyucedemirbas/KerasFuse"
```

### Comparing `kerasfuse-0.0.1/PKG-INFO` & `kerasfuse-0.1a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6b65 7261  : 2.1.Name: kera
 00000020: 7366 7573 650a 5665 7273 696f 6e3a 2030  sfuse.Version: 0
-00000030: 2e30 2e31 0a53 756d 6d61 7279 3a20 4b65  .0.1.Summary: Ke
+00000030: 2e31 6130 0a53 756d 6d61 7279 3a20 4b65  .1a0.Summary: Ke
 00000040: 7261 7346 7573 6520 6973 2061 2050 7974  rasFuse is a Pyt
 00000050: 686f 6e20 6c69 6272 6172 7920 7468 6174  hon library that
 00000060: 2063 6f6d 6269 6e65 7320 7468 6520 706f   combines the po
 00000070: 7765 7220 6f66 2054 656e 736f 7246 6c6f  wer of TensorFlo
 00000080: 7720 616e 6420 4b65 7261 7320 7769 7468  w and Keras with
 00000090: 2076 6172 696f 7573 2063 6f6d 7075 7465   various compute
 000000a0: 7220 7669 7369 6f6e 2074 6563 686e 6971  r vision techniq
@@ -82,154 +82,134 @@
 00000510: 6563 742d 5552 4c3a 2052 6570 6f73 6974  ect-URL: Reposit
 00000520: 6f72 792c 2068 7474 7073 3a2f 2f67 6974  ory, https://git
 00000530: 6875 622e 636f 6d2f 6179 7975 6365 6465  hub.com/ayyucede
 00000540: 6d69 7262 6173 2f4b 6572 6173 4675 7365  mirbas/KerasFuse
 00000550: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
 00000560: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 00000570: 6d61 726b 646f 776e 0a0a 3c70 2061 6c69  markdown..<p ali
-00000580: 676e 3d22 6365 6e74 6572 223e 0a3c 7069  gn="center">.<pi
-00000590: 6374 7572 653e 0a20 203c 736f 7572 6365  cture>.  <source
-000005a0: 206d 6564 6961 3d22 2870 7265 6665 7273   media="(prefers
-000005b0: 2d63 6f6c 6f72 2d73 6368 656d 653a 2064  -color-scheme: d
-000005c0: 6172 6b29 2220 7372 6373 6574 3d22 6874  ark)" srcset="ht
-000005d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000005e0: 2f61 7979 7563 6564 656d 6972 6261 732f  /ayyucedemirbas/
-000005f0: 4b65 7261 7346 7573 652f 6173 7365 7473  KerasFuse/assets
-00000600: 2f38 3032 3331 3530 2f34 3164 3838 3830  /8023150/41d8880
-00000610: 642d 3831 3137 2d34 3438 622d 6137 3235  d-8117-448b-a725
-00000620: 2d32 6237 3264 3264 3038 6265 6222 3e0a  -2b72d2d08beb">.
-00000630: 2020 3c73 6f75 7263 6520 6d65 6469 613d    <source media=
-00000640: 2228 7072 6566 6572 732d 636f 6c6f 722d  "(prefers-color-
-00000650: 7363 6865 6d65 3a20 6c69 6768 7429 2220  scheme: light)" 
-00000660: 7372 6373 6574 3d22 6874 7470 733a 2f2f  srcset="https://
-00000670: 6769 7468 7562 2e63 6f6d 2f61 7979 7563  github.com/ayyuc
-00000680: 6564 656d 6972 6261 732f 4b65 7261 7346  edemirbas/KerasF
-00000690: 7573 652f 6173 7365 7473 2f38 3032 3331  use/assets/80231
-000006a0: 3530 2f34 3164 3838 3830 642d 3831 3137  50/41d8880d-8117
-000006b0: 2d34 3438 622d 6137 3235 2d32 6237 3264  -448b-a725-2b72d
-000006c0: 3264 3038 6265 6222 3e0a 2020 3c69 6d67  2d08beb">.  <img
-000006d0: 2061 6c74 3d22 4b65 7261 7346 7573 6522   alt="KerasFuse"
-000006e0: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-000006f0: 7468 7562 2e63 6f6d 2f61 7979 7563 6564  thub.com/ayyuced
-00000700: 656d 6972 6261 732f 4b65 7261 7346 7573  emirbas/KerasFus
-00000710: 6522 3e0a 3c2f 7069 6374 7572 653e 0a3c  e">.</picture>.<
-00000720: 2f70 3e0a 0a3c 6831 2061 6c69 676e 3d22  /p>..<h1 align="
-00000730: 6365 6e74 6572 223e 4b65 7261 7346 7573  center">KerasFus
-00000740: 653c 2f68 313e 0a0a 3c70 3e0a 2020 3c69  e</h1>..<p>.  <i
-00000750: 6d67 2061 6c74 3d22 4769 7448 7562 2220  mg alt="GitHub" 
-00000760: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000770: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00000780: 7562 2f6c 6963 656e 7365 2f61 7979 7563  ub/license/ayyuc
-00000790: 6564 656d 6972 6261 732f 4b65 7261 7366  edemirbas/Kerasf
-000007a0: 7573 6522 3e0a 2020 3c69 6d67 2061 6c74  use">.  <img alt
-000007b0: 3d22 5079 7468 6f6e 3322 2073 7263 3d22  ="Python3" src="
-000007c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000007d0: 6c64 732e 696f 2f62 6164 6765 2f50 7974  lds.io/badge/Pyt
-000007e0: 686f 6e2d 332e 382e 3120 7c20 332e 3920  hon-3.8.1 | 3.9 
-000007f0: 7c20 332e 3130 207c 2033 2e31 312d 3337  | 3.10 | 3.11-37
-00000800: 3736 4142 2e73 7667 3f6c 6f67 6f3d 5079  76AB.svg?logo=Py
-00000810: 7468 6f6e 266c 6f67 6f43 6f6c 6f72 3d77  thon&logoColor=w
-00000820: 6869 7465 222f 3e0a 2020 3c69 6d67 2061  hite"/>.  <img a
-00000830: 6c74 3d22 5465 6e73 6f72 666c 6f77 2220  lt="Tensorflow" 
-00000840: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000850: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000860: 652f 5465 6e73 6f72 666c 6f77 2d76 322e  e/Tensorflow-v2.
-00000870: 3132 2e30 2d25 3233 4646 3646 3030 2e73  12.0-%23FF6F00.s
-00000880: 7667 3f6c 6f67 6f3d 5465 6e73 6f72 666c  vg?logo=Tensorfl
-00000890: 6f77 266c 6f67 6f43 6f6c 6f72 3d77 6869  ow&logoColor=whi
-000008a0: 7465 222f 3e0a 2020 3c69 6d67 2061 6c74  te"/>.  <img alt
-000008b0: 3d22 4b65 7261 7322 2073 7263 3d22 6874  ="Keras" src="ht
-000008c0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000008d0: 732e 696f 2f62 6164 6765 2f4b 6572 6173  s.io/badge/Keras
-000008e0: 2d76 322e 3132 2e30 2d25 3233 4430 3030  -v2.12.0-%23D000
-000008f0: 3030 2e73 7667 3f6c 6f67 6f3d 4b65 7261  00.svg?logo=Kera
-00000900: 7326 6c6f 676f 436f 6c6f 723d 7768 6974  s&logoColor=whit
-00000910: 6522 2f3e 0a20 203c 696d 6720 616c 743d  e"/>.  <img alt=
-00000920: 2242 6c61 636b 2220 7372 633d 2268 7474  "Black" src="htt
-00000930: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000940: 2e69 6f2f 6261 6467 652f 636f 6465 2532  .io/badge/code%2
-00000950: 3073 7479 6c65 2d62 6c61 636b 2d62 6c61  0style-black-bla
-00000960: 636b 222f 3e0a 2020 3c69 6d67 2061 6c74  ck"/>.  <img alt
-00000970: 3d22 6973 6f72 7422 2073 7263 3d22 6874  ="isort" src="ht
-00000980: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000990: 732e 696f 2f62 6164 6765 2f69 736f 7274  s.io/badge/isort
-000009a0: 2d63 6865 636b 6564 2d79 656c 6c6f 7722  -checked-yellow"
-000009b0: 2f3e 0a3c 2f70 3e0a 0a3c 6834 2061 6c69  />.</p>..<h4 ali
-000009c0: 676e 3d22 6365 6e74 6572 223e f09f 9aa7  gn="center">....
-000009d0: 2057 6172 6e69 6e67 2074 6869 7320 7072   Warning this pr
-000009e0: 6f6a 6563 7420 6973 2075 6e64 6572 2068  oject is under h
-000009f0: 6561 7679 2064 6576 656c 6f70 6d65 6e74  eavy development
-00000a00: 2061 6e64 206e 6f74 2072 6561 6479 2066   and not ready f
-00000a10: 6f72 2070 726f 6475 6374 696f 6e2e 2041  or production. A
-00000a20: 4249 2063 6861 6e67 6573 2063 616e 2068  BI changes can h
-00000a30: 6170 7065 6e20 6672 6571 7565 6e74 6c79  appen frequently
-00000a40: 2075 6e74 696c 2072 6561 6368 2073 7461   until reach sta
-00000a50: 626c 6520 7665 7273 696f 6e20 f09f 9aa7  ble version ....
-00000a60: 203c 2f68 343e 0a0a 0a4b 6572 6173 4675   </h4>...KerasFu
-00000a70: 7365 2069 7320 6120 5079 7468 6f6e 206c  se is a Python l
-00000a80: 6962 7261 7279 2074 6861 7420 636f 6d62  ibrary that comb
-00000a90: 696e 6573 2074 6865 2070 6f77 6572 206f  ines the power o
-00000aa0: 6620 5465 6e73 6f72 466c 6f77 2061 6e64  f TensorFlow and
-00000ab0: 204b 6572 6173 2077 6974 6820 7661 7269   Keras with vari
-00000ac0: 6f75 7320 636f 6d70 7574 6572 2076 6973  ous computer vis
-00000ad0: 696f 6e20 7465 6368 6e69 7175 6573 2066  ion techniques f
-00000ae0: 6f72 206d 6564 6963 616c 2069 6d61 6765  or medical image
-00000af0: 2061 6e61 6c79 7369 7320 7461 736b 732e   analysis tasks.
-00000b00: 2049 7420 7072 6f76 6964 6573 2061 2063   It provides a c
-00000b10: 6f6c 6c65 6374 696f 6e20 6f66 206d 6f64  ollection of mod
-00000b20: 756c 6573 2061 6e64 2066 756e 6374 696f  ules and functio
-00000b30: 6e73 2074 6f20 6661 6369 6c69 7461 7465  ns to facilitate
-00000b40: 2074 6865 2064 6576 656c 6f70 6d65 6e74   the development
-00000b50: 206f 6620 6465 6570 206c 6561 726e 696e   of deep learnin
-00000b60: 6720 6d6f 6465 6c73 2069 6e20 5465 6e73  g models in Tens
-00000b70: 6f72 466c 6f77 204b 6572 6173 2066 6f72  orFlow Keras for
-00000b80: 2074 6173 6b73 2073 7563 6820 6173 2069   tasks such as i
-00000b90: 6d61 6765 2073 6567 6d65 6e74 6174 696f  mage segmentatio
-00000ba0: 6e2c 2063 6c61 7373 6966 6963 6174 696f  n, classificatio
-00000bb0: 6e2c 2061 6e64 206d 6f72 652e 0a0a 0a0a  n, and more.....
-00000bc0: 2323 2047 6574 7469 6e67 2053 7461 7274  ## Getting Start
-00000bd0: 6564 0a0a 2323 2320 496e 7374 616c 6c61  ed..### Installa
-00000be0: 7469 6f6e 0a0a 2323 2323 2050 6f65 7472  tion..#### Poetr
-00000bf0: 7920 496e 7374 616c 6c61 7469 6f6e 0a0a  y Installation..
-00000c00: 6060 6062 6173 680a 706f 6574 7279 2069  ```bash.poetry i
-00000c10: 6e73 7461 6c6c 0a70 6f65 7472 7920 7368  nstall.poetry sh
-00000c20: 656c 6c0a 6060 600a 0a23 2323 2320 5469  ell.```..#### Ti
-00000c30: 700a 0a49 6620 796f 7520 6861 7665 206d  p..If you have m
-00000c40: 756c 7469 706c 6520 5079 7468 6f6e 2076  ultiple Python v
-00000c50: 6572 7369 6f6e 7320 6f6e 2079 6f75 7220  ersions on your 
-00000c60: 7379 7374 656d 2c20 796f 7520 6361 6e20  system, you can 
-00000c70: 7365 7420 796f 7572 2050 7974 686f 6e20  set your Python 
-00000c80: 7665 7273 696f 6e20 6279 2075 7369 6e67  version by using
-00000c90: 2060 706f 6574 7279 2065 6e76 6020 2e20   `poetry env` . 
-00000ca0: 4865 7265 2773 2061 6e20 6578 616d 706c  Here's an exampl
-00000cb0: 6520 6f66 2068 6f77 2074 6f20 7573 6520  e of how to use 
-00000cc0: 6974 3a0a 0a60 6060 6261 7368 0a70 6f65  it:..```bash.poe
-00000cd0: 7472 7920 656e 7620 7573 6520 7079 7468  try env use pyth
-00000ce0: 6f6e 332e 3130 0a60 6060 0a0a 4d6f 7265  on3.10.```..More
-00000cf0: 2064 6574 6169 6c73 2061 740a 5b70 6f65   details at.[poe
-00000d00: 7472 792d 7377 6974 6368 696e 672d 6265  try-switching-be
-00000d10: 7477 6565 6e2d 656e 7669 726f 6e6d 656e  tween-environmen
-00000d20: 7473 5d28 6874 7470 733a 2f2f 7079 7468  ts](https://pyth
-00000d30: 6f6e 2d70 6f65 7472 792e 6f72 672f 646f  on-poetry.org/do
-00000d40: 6373 2f6d 616e 6167 696e 672d 656e 7669  cs/managing-envi
-00000d50: 726f 6e6d 656e 7473 2f23 7377 6974 6368  ronments/#switch
-00000d60: 696e 672d 6265 7477 6565 6e2d 656e 7669  ing-between-envi
-00000d70: 726f 6e6d 656e 7473 290a 0a23 2323 2320  ronments)..#### 
-00000d80: 5069 7020 496e 7374 616c 6c61 7469 6f6e  Pip Installation
-00000d90: 730a 0a60 6060 6261 7368 0a70 7974 686f  s..```bash.pytho
-00000da0: 6e33 202d 6d20 7665 6e76 202e 7665 6e76  n3 -m venv .venv
-00000db0: 0a73 6f75 7263 6520 2e76 656e 762f 6269  .source .venv/bi
-00000dc0: 6e2f 6163 7469 7661 7465 0a70 6970 3320  n/activate.pip3 
-00000dd0: 696e 7374 616c 6c20 2d72 2072 6571 7569  install -r requi
-00000de0: 7265 6d65 6e74 732e 7478 740a 6060 600a  rements.txt.```.
-00000df0: 0a46 6f72 204d 6163 4f53 0a0a 6060 6062  .For MacOS..```b
-00000e00: 6173 680a 7079 7468 6f6e 3320 2d6d 2076  ash.python3 -m v
-00000e10: 656e 7620 2e76 656e 760a 736f 7572 6365  env .venv.source
-00000e20: 202e 7665 6e76 2f62 696e 2f61 6374 6976   .venv/bin/activ
-00000e30: 6174 650a 7069 7033 2069 6e73 7461 6c6c  ate.pip3 install
-00000e40: 202d 7220 7265 7175 6972 656d 656e 7473   -r requirements
-00000e50: 2d6d 6163 6f73 2e74 7874 0a60 6060 0a0a  -macos.txt.```..
-00000e60: 2323 204c 6963 656e 7365 0a0a 5468 6973  ## License..This
-00000e70: 2070 726f 6a65 6374 2069 7320 6c69 6365   project is lice
-00000e80: 6e73 6564 2075 6e64 6572 2074 6865 2074  nsed under the t
-00000e90: 6572 6d73 206f 6620 7468 6520 4750 4c2d  erms of the GPL-
-00000ea0: 332e 3020 6c69 6365 6e73 652e 0a0a       3.0 license...
+00000580: 676e 3d22 6365 6e74 6572 223e 0a20 203c  gn="center">.  <
+00000590: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000005a0: 6769 7468 7562 2e63 6f6d 2f61 7979 7563  github.com/ayyuc
+000005b0: 6564 656d 6972 6261 732f 4b65 7261 7346  edemirbas/KerasF
+000005c0: 7573 6522 3e3c 696d 6720 7372 633d 2268  use"><img src="h
+000005d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000005e0: 6d2f 6179 7975 6365 6465 6d69 7262 6173  m/ayyucedemirbas
+000005f0: 2f4b 6572 6173 4675 7365 2f61 7373 6574  /KerasFuse/asset
+00000600: 732f 3830 3233 3135 302f 3431 6438 3838  s/8023150/41d888
+00000610: 3064 2d38 3131 372d 3434 3862 2d61 3732  0d-8117-448b-a72
+00000620: 352d 3262 3732 6432 6430 3862 6562 2220  5-2b72d2d08beb" 
+00000630: 616c 743d 224b 6572 6173 4675 7365 223e  alt="KerasFuse">
+00000640: 3c2f 613e 0a3c 2f70 3e0a 0a3c 6831 2061  </a>.</p>..<h1 a
+00000650: 6c69 676e 3d22 6365 6e74 6572 223e 4b65  lign="center">Ke
+00000660: 7261 7346 7573 653c 2f68 313e 0a0a 3c70  rasFuse</h1>..<p
+00000670: 3e0a 2020 3c69 6d67 2061 6c74 3d22 4769  >.  <img alt="Gi
+00000680: 7448 7562 2220 7372 633d 2268 7474 7073  tHub" src="https
+00000690: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000006a0: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
+000006b0: 2f61 7979 7563 6564 656d 6972 6261 732f  /ayyucedemirbas/
+000006c0: 4b65 7261 7366 7573 6522 3e0a 2020 3c69  Kerasfuse">.  <i
+000006d0: 6d67 2061 6c74 3d22 5079 7468 6f6e 3322  mg alt="Python3"
+000006e0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+000006f0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000700: 6765 2f50 7974 686f 6e2d 332e 382e 3120  ge/Python-3.8.1 
+00000710: 7c20 332e 3920 7c20 332e 3130 207c 2033  | 3.9 | 3.10 | 3
+00000720: 2e31 312d 3337 3736 4142 2e73 7667 3f6c  .11-3776AB.svg?l
+00000730: 6f67 6f3d 5079 7468 6f6e 266c 6f67 6f43  ogo=Python&logoC
+00000740: 6f6c 6f72 3d77 6869 7465 222f 3e0a 2020  olor=white"/>.  
+00000750: 3c69 6d67 2061 6c74 3d22 5465 6e73 6f72  <img alt="Tensor
+00000760: 666c 6f77 2220 7372 633d 2268 7474 7073  flow" src="https
+00000770: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000780: 6f2f 6261 6467 652f 5465 6e73 6f72 666c  o/badge/Tensorfl
+00000790: 6f77 2d76 322e 3132 2e30 2d25 3233 4646  ow-v2.12.0-%23FF
+000007a0: 3646 3030 2e73 7667 3f6c 6f67 6f3d 5465  6F00.svg?logo=Te
+000007b0: 6e73 6f72 666c 6f77 266c 6f67 6f43 6f6c  nsorflow&logoCol
+000007c0: 6f72 3d77 6869 7465 222f 3e0a 2020 3c69  or=white"/>.  <i
+000007d0: 6d67 2061 6c74 3d22 4b65 7261 7322 2073  mg alt="Keras" s
+000007e0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000007f0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000800: 2f4b 6572 6173 2d76 322e 3132 2e30 2d25  /Keras-v2.12.0-%
+00000810: 3233 4430 3030 3030 2e73 7667 3f6c 6f67  23D00000.svg?log
+00000820: 6f3d 4b65 7261 7326 6c6f 676f 436f 6c6f  o=Keras&logoColo
+00000830: 723d 7768 6974 6522 2f3e 0a20 203c 696d  r=white"/>.  <im
+00000840: 6720 616c 743d 2242 6c61 636b 2220 7372  g alt="Black" sr
+00000850: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000860: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000870: 636f 6465 2532 3073 7479 6c65 2d62 6c61  code%20style-bla
+00000880: 636b 2d62 6c61 636b 222f 3e0a 2020 3c69  ck-black"/>.  <i
+00000890: 6d67 2061 6c74 3d22 6973 6f72 7422 2073  mg alt="isort" s
+000008a0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000008b0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000008c0: 2f69 736f 7274 2d63 6865 636b 6564 2d79  /isort-checked-y
+000008d0: 656c 6c6f 7722 2f3e 0a3c 2f70 3e0a 0a3c  ellow"/>.</p>..<
+000008e0: 6834 2061 6c69 676e 3d22 6365 6e74 6572  h4 align="center
+000008f0: 223e f09f 9aa7 2057 6172 6e69 6e67 2074  ">.... Warning t
+00000900: 6869 7320 7072 6f6a 6563 7420 6973 2075  his project is u
+00000910: 6e64 6572 2068 6561 7679 2064 6576 656c  nder heavy devel
+00000920: 6f70 6d65 6e74 2061 6e64 206e 6f74 2072  opment and not r
+00000930: 6561 6479 2066 6f72 2070 726f 6475 6374  eady for product
+00000940: 696f 6e2e 2041 4249 2063 6861 6e67 6573  ion. ABI changes
+00000950: 2063 616e 2068 6170 7065 6e20 6672 6571   can happen freq
+00000960: 7565 6e74 6c79 2075 6e74 696c 2072 6561  uently until rea
+00000970: 6368 2073 7461 626c 6520 7665 7273 696f  ch stable versio
+00000980: 6e20 f09f 9aa7 203c 2f68 343e 0a0a 0a4b  n .... </h4>...K
+00000990: 6572 6173 4675 7365 2069 7320 6120 5079  erasFuse is a Py
+000009a0: 7468 6f6e 206c 6962 7261 7279 2074 6861  thon library tha
+000009b0: 7420 636f 6d62 696e 6573 2074 6865 2070  t combines the p
+000009c0: 6f77 6572 206f 6620 5465 6e73 6f72 466c  ower of TensorFl
+000009d0: 6f77 2061 6e64 204b 6572 6173 2077 6974  ow and Keras wit
+000009e0: 6820 7661 7269 6f75 7320 636f 6d70 7574  h various comput
+000009f0: 6572 2076 6973 696f 6e20 7465 6368 6e69  er vision techni
+00000a00: 7175 6573 2066 6f72 206d 6564 6963 616c  ques for medical
+00000a10: 2069 6d61 6765 2061 6e61 6c79 7369 7320   image analysis 
+00000a20: 7461 736b 732e 2049 7420 7072 6f76 6964  tasks. It provid
+00000a30: 6573 2061 2063 6f6c 6c65 6374 696f 6e20  es a collection 
+00000a40: 6f66 206d 6f64 756c 6573 2061 6e64 2066  of modules and f
+00000a50: 756e 6374 696f 6e73 2074 6f20 6661 6369  unctions to faci
+00000a60: 6c69 7461 7465 2074 6865 2064 6576 656c  litate the devel
+00000a70: 6f70 6d65 6e74 206f 6620 6465 6570 206c  opment of deep l
+00000a80: 6561 726e 696e 6720 6d6f 6465 6c73 2069  earning models i
+00000a90: 6e20 5465 6e73 6f72 466c 6f77 204b 6572  n TensorFlow Ker
+00000aa0: 6173 2066 6f72 2074 6173 6b73 2073 7563  as for tasks suc
+00000ab0: 6820 6173 2069 6d61 6765 2073 6567 6d65  h as image segme
+00000ac0: 6e74 6174 696f 6e2c 2063 6c61 7373 6966  ntation, classif
+00000ad0: 6963 6174 696f 6e2c 2061 6e64 206d 6f72  ication, and mor
+00000ae0: 652e 0a0a 0a0a 2323 2047 6574 7469 6e67  e.....## Getting
+00000af0: 2053 7461 7274 6564 0a0a 2323 2320 496e   Started..### In
+00000b00: 7374 616c 6c61 7469 6f6e 0a0a 2323 2323  stallation..####
+00000b10: 2050 6f65 7472 7920 496e 7374 616c 6c61   Poetry Installa
+00000b20: 7469 6f6e 0a0a 6060 6062 6173 680a 706f  tion..```bash.po
+00000b30: 6574 7279 2069 6e73 7461 6c6c 0a70 6f65  etry install.poe
+00000b40: 7472 7920 7368 656c 6c0a 6060 600a 0a23  try shell.```..#
+00000b50: 2323 2320 5469 700a 0a49 6620 796f 7520  ### Tip..If you 
+00000b60: 6861 7665 206d 756c 7469 706c 6520 5079  have multiple Py
+00000b70: 7468 6f6e 2076 6572 7369 6f6e 7320 6f6e  thon versions on
+00000b80: 2079 6f75 7220 7379 7374 656d 2c20 796f   your system, yo
+00000b90: 7520 6361 6e20 7365 7420 796f 7572 2050  u can set your P
+00000ba0: 7974 686f 6e20 7665 7273 696f 6e20 6279  ython version by
+00000bb0: 2075 7369 6e67 2060 706f 6574 7279 2065   using `poetry e
+00000bc0: 6e76 6020 2e20 4865 7265 2773 2061 6e20  nv` . Here's an 
+00000bd0: 6578 616d 706c 6520 6f66 2068 6f77 2074  example of how t
+00000be0: 6f20 7573 6520 6974 3a0a 0a60 6060 6261  o use it:..```ba
+00000bf0: 7368 0a70 6f65 7472 7920 656e 7620 7573  sh.poetry env us
+00000c00: 6520 7079 7468 6f6e 332e 3130 0a60 6060  e python3.10.```
+00000c10: 0a0a 4d6f 7265 2064 6574 6169 6c73 2061  ..More details a
+00000c20: 740a 5b70 6f65 7472 792d 7377 6974 6368  t.[poetry-switch
+00000c30: 696e 672d 6265 7477 6565 6e2d 656e 7669  ing-between-envi
+00000c40: 726f 6e6d 656e 7473 5d28 6874 7470 733a  ronments](https:
+00000c50: 2f2f 7079 7468 6f6e 2d70 6f65 7472 792e  //python-poetry.
+00000c60: 6f72 672f 646f 6373 2f6d 616e 6167 696e  org/docs/managin
+00000c70: 672d 656e 7669 726f 6e6d 656e 7473 2f23  g-environments/#
+00000c80: 7377 6974 6368 696e 672d 6265 7477 6565  switching-betwee
+00000c90: 6e2d 656e 7669 726f 6e6d 656e 7473 290a  n-environments).
+00000ca0: 0a23 2323 2320 5069 7020 496e 7374 616c  .#### Pip Instal
+00000cb0: 6c61 7469 6f6e 730a 0a60 6060 6261 7368  lations..```bash
+00000cc0: 0a70 7974 686f 6e33 202d 6d20 7665 6e76  .python3 -m venv
+00000cd0: 202e 7665 6e76 0a73 6f75 7263 6520 2e76   .venv.source .v
+00000ce0: 656e 762f 6269 6e2f 6163 7469 7661 7465  env/bin/activate
+00000cf0: 0a70 6970 3320 696e 7374 616c 6c20 2d72  .pip3 install -r
+00000d00: 2072 6571 7569 7265 6d65 6e74 732e 7478   requirements.tx
+00000d10: 740a 6060 600a 0a23 2320 4c69 6365 6e73  t.```..## Licens
+00000d20: 650a 0a54 6869 7320 7072 6f6a 6563 7420  e..This project 
+00000d30: 6973 206c 6963 656e 7365 6420 756e 6465  is licensed unde
+00000d40: 7220 7468 6520 7465 726d 7320 6f66 2074  r the terms of t
+00000d50: 6865 2047 504c 2d33 2e30 206c 6963 656e  he GPL-3.0 licen
+00000d60: 7365 2e0a 0a                             se...
```

