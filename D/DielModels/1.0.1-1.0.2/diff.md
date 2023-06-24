# Comparing `tmp/DielModels-1.0.1.tar.gz` & `tmp/DielModels-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DielModels-1.0.1.tar", last modified: Fri Jun 23 10:24:06 2023, max compression
+gzip compressed data, was "dist\DielModels-1.0.2.tar", last modified: Sat Jun 24 09:52:09 2023, max compression
```

## Comparing `DielModels-1.0.1.tar` & `DielModels-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 10:24:06.326083 DielModels-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-03-20 16:26:03.000000 DielModels-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      647 2023-06-23 10:24:06.326083 DielModels-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      117 2023-06-23 10:22:45.000000 DielModels-1.0.1/README.md
--rw-rw-rw-   0        0        0      556 2023-03-20 16:26:03.000000 DielModels-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      919 2023-06-23 10:24:06.328302 DielModels-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-03-20 16:26:03.000000 DielModels-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:24:06.199869 DielModels-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 10:24:06.251439 DielModels-1.0.1/src/DielModels.egg-info/
--rw-rw-rw-   0        0        0      647 2023-06-23 10:24:05.000000 DielModels-1.0.1/src/DielModels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2023-06-23 10:24:05.000000 DielModels-1.0.1/src/DielModels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 10:24:05.000000 DielModels-1.0.1/src/DielModels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 09:19:08.000000 DielModels-1.0.1/src/DielModels.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      100 2023-06-23 10:24:05.000000 DielModels-1.0.1/src/DielModels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-23 10:24:05.000000 DielModels-1.0.1/src/DielModels.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-23 10:24:06.315524 DielModels-1.0.1/src/diel_models/
--rw-rw-rw-   0        0        0        0 2023-03-20 16:26:03.000000 DielModels-1.0.1/src/diel_models/__init__.py
--rw-rw-rw-   0        0        0     2572 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/biomass_adjuster.py
--rw-rw-rw-   0        0        0     3954 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/day_night_creator.py
--rw-rw-rw-   0        0        0     2125 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/diel_models_creator.py
--rw-rw-rw-   0        0        0     2096 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/nitrate_uptake_ratio.py
--rw-rw-rw-   0        0        0     2245 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/photon_reaction_inhibitor.py
--rw-rw-rw-   0        0        0      952 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/pipeline.py
--rw-rw-rw-   0        0        0     7077 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/storage_pool_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:52:09.718384 DielModels-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-03-20 16:26:03.000000 DielModels-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2679 2023-06-24 09:52:09.719386 DielModels-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2106 2023-06-24 09:50:32.000000 DielModels-1.0.2/README.md
+-rw-rw-rw-   0        0        0      556 2023-03-20 16:26:03.000000 DielModels-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      966 2023-06-24 09:52:09.725898 DielModels-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-03-20 16:26:03.000000 DielModels-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:52:09.652555 DielModels-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 09:52:09.702343 DielModels-1.0.2/src/DielModels.egg-info/
+-rw-rw-rw-   0        0        0     2679 2023-06-24 09:52:09.000000 DielModels-1.0.2/src/DielModels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2023-06-24 09:52:09.000000 DielModels-1.0.2/src/DielModels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 09:52:09.000000 DielModels-1.0.2/src/DielModels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-24 09:33:35.000000 DielModels-1.0.2/src/DielModels.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      100 2023-06-24 09:52:09.000000 DielModels-1.0.2/src/DielModels.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-24 09:52:09.000000 DielModels-1.0.2/src/DielModels.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 09:52:09.716379 DielModels-1.0.2/src/diel_models/
+-rw-rw-rw-   0        0        0        0 2023-03-20 16:26:03.000000 DielModels-1.0.2/src/diel_models/__init__.py
+-rw-rw-rw-   0        0        0     2572 2023-06-22 12:47:14.000000 DielModels-1.0.2/src/diel_models/biomass_adjuster.py
+-rw-rw-rw-   0        0        0     3954 2023-06-22 12:47:14.000000 DielModels-1.0.2/src/diel_models/day_night_creator.py
+-rw-rw-rw-   0        0        0     2125 2023-06-22 12:47:14.000000 DielModels-1.0.2/src/diel_models/diel_models_creator.py
+-rw-rw-rw-   0        0        0     2096 2023-06-22 12:47:14.000000 DielModels-1.0.2/src/diel_models/nitrate_uptake_ratio.py
+-rw-rw-rw-   0        0        0     2245 2023-06-22 12:47:14.000000 DielModels-1.0.2/src/diel_models/photon_reaction_inhibitor.py
+-rw-rw-rw-   0        0        0      952 2023-06-22 12:47:14.000000 DielModels-1.0.2/src/diel_models/pipeline.py
+-rw-rw-rw-   0        0        0     7197 2023-06-24 09:31:27.000000 DielModels-1.0.2/src/diel_models/storage_pool_generator.py
```

### Comparing `DielModels-1.0.1/LICENSE` & `DielModels-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DielModels-1.0.1/pyproject.toml` & `DielModels-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `DielModels-1.0.1/setup.cfg` & `DielModels-1.0.2/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2044 6965 6c4d 6f64 656c 730d 0a76   = DielModels..v
-00000020: 6572 7369 6f6e 203d 2031 2e30 2e31 0d0a  ersion = 1.0.1..
+00000020: 6572 7369 6f6e 203d 2031 2e30 2e32 0d0a  ersion = 1.0.2..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 4469  description = Di
 00000040: 656c 4d6f 6465 6c73 3a0d 0a6c 6f6e 675f  elModels:..long_
 00000050: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-00000060: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6b  le: README.md..k
-00000070: 6579 776f 7264 7320 3d20 706c 616e 7473  eywords = plants
-00000080: 2c20 6469 656c 206d 6f64 656c 730d 0a61  , diel models..a
-00000090: 7574 686f 7220 3d20 4c75 6369 616e 6120  uthor = Luciana 
-000000a0: 4d61 7274 696e 7320 616e 6420 4a6f c3a3  Martins and Jo..
-000000b0: 6f20 4361 7065 6c61 0d0a 6c69 6365 6e73  o Capela..licens
-000000c0: 6520 3d20 4d49 540d 0a6c 6963 656e 7365  e = MIT..license
-000000d0: 5f66 696c 6520 3d20 4c49 4345 4e53 450d  _file = LICENSE.
-000000e0: 0a70 6c61 7466 6f72 6d73 203d 2075 6e69  .platforms = uni
-000000f0: 782c 206c 696e 7578 2c20 6f73 782c 2063  x, linux, osx, c
-00000100: 7967 7769 6e2c 2077 696e 3332 0d0a 636c  ygwin, win32..cl
-00000110: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
-00000120: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000130: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000140: 2033 0d0a 0950 726f 6772 616d 6d69 6e67   3...Programming
-00000150: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000160: 686f 6e20 3a3a 2033 203a 3a20 4f6e 6c79  hon :: 3 :: Only
-00000170: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000180: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000190: 6e20 3a3a 2033 2e38 0d0a 0950 726f 6772  n :: 3.8...Progr
-000001a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-000001c0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-000001d0: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
-000001e0: 3d73 7263 0d0a 7061 636b 6167 6573 203d  =src..packages =
-000001f0: 2066 696e 645f 6e61 6d65 7370 6163 653a   find_namespace:
-00000200: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-00000210: 7320 3d20 3e3d 332e 380d 0a7a 6970 5f73  s = >=3.8..zip_s
-00000220: 6166 6520 3d20 4661 6c73 650d 0a69 6e63  afe = False..inc
-00000230: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-00000240: 6120 3d20 5472 7565 0d0a 696e 7374 616c  a = True..instal
-00000250: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
-00000260: 636f 6272 610d 0a09 6e75 6d70 790d 0a09  cobra...numpy...
-00000270: 7061 6e64 6173 0d0a 0d0a 5b6f 7074 696f  pandas....[optio
-00000280: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-00000290: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
-000002a0: 0d0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
-000002b0: 735f 7265 7175 6972 655d 0d0a 7465 7374  s_require]..test
-000002c0: 696e 6720 3d20 0d0a 0970 7974 6573 743e  ing = ...pytest>
-000002d0: 3d37 2e31 2e31 0d0a 0970 7974 6573 742d  =7.1.1...pytest-
-000002e0: 636f 763e 3d33 2e30 2e30 0d0a 096d 7970  cov>=3.0.0...myp
-000002f0: 793e 3d30 2e39 3432 0d0a 0966 6c61 6b65  y>=0.942...flake
-00000300: 383e 3d34 2e30 2e31 0d0a 0974 6f78 3e3d  8>=4.0.1...tox>=
-00000310: 332e 3235 2e30 0d0a 0d0a 5b6f 7074 696f  3.25.0....[optio
-00000320: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
-00000330: 0d0a 706c 616e 7473 5f73 6d20 3d20 7079  ..plants_sm = py
-00000340: 2e74 7970 6564 0d0a 0d0a 5b66 6c61 6b65  .typed....[flake
-00000350: 385d 0d0a 6d61 782d 6c69 6e65 2d6c 656e  8]..max-line-len
-00000360: 6774 6820 3d20 3136 300d 0a0d 0a5b 6567  gth = 160....[eg
-00000370: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000380: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000390: 3d20 300d 0a0d 0a                        = 0....
+00000060: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
+00000070: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+00000080: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
+00000090: 6578 742f 6d61 726b 646f 776e 0d0a 6b65  ext/markdown..ke
+000000a0: 7977 6f72 6473 203d 2070 6c61 6e74 732c  ywords = plants,
+000000b0: 2064 6965 6c20 6d6f 6465 6c73 0d0a 6175   diel models..au
+000000c0: 7468 6f72 203d 204c 7563 6961 6e61 204d  thor = Luciana M
+000000d0: 6172 7469 6e73 2061 6e64 204a 6fc3 a36f  artins and Jo..o
+000000e0: 2043 6170 656c 610d 0a6c 6963 656e 7365   Capela..license
+000000f0: 203d 204d 4954 0d0a 6c69 6365 6e73 655f   = MIT..license_
+00000100: 6669 6c65 203d 204c 4943 454e 5345 0d0a  file = LICENSE..
+00000110: 706c 6174 666f 726d 7320 3d20 756e 6978  platforms = unix
+00000120: 2c20 6c69 6e75 782c 206f 7378 2c20 6379  , linux, osx, cy
+00000130: 6777 696e 2c20 7769 6e33 320d 0a63 6c61  gwin, win32..cla
+00000140: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
+00000150: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000160: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000170: 330d 0a09 5072 6f67 7261 6d6d 696e 6720  3...Programming 
+00000180: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000190: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790d  on :: 3 :: Only.
+000001a0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000001b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001c0: 203a 3a20 332e 380d 0a09 5072 6f67 7261   :: 3.8...Progra
+000001d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001e0: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
+000001f0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
+00000200: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
+00000210: 7372 630d 0a70 6163 6b61 6765 7320 3d20  src..packages = 
+00000220: 6669 6e64 5f6e 616d 6573 7061 6365 3a0d  find_namespace:.
+00000230: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+00000240: 203d 203e 3d33 2e38 0d0a 7a69 705f 7361   = >=3.8..zip_sa
+00000250: 6665 203d 2046 616c 7365 0d0a 696e 636c  fe = False..incl
+00000260: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+00000270: 203d 2054 7275 650d 0a69 6e73 7461 6c6c   = True..install
+00000280: 5f72 6571 7569 7265 7320 3d20 0d0a 0963  _requires = ...c
+00000290: 6f62 7261 0d0a 096e 756d 7079 0d0a 0970  obra...numpy...p
+000002a0: 616e 6461 730d 0a0d 0a5b 6f70 7469 6f6e  andas....[option
+000002b0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+000002c0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+000002d0: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+000002e0: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
+000002f0: 6e67 203d 200d 0a09 7079 7465 7374 3e3d  ng = ...pytest>=
+00000300: 372e 312e 310d 0a09 7079 7465 7374 2d63  7.1.1...pytest-c
+00000310: 6f76 3e3d 332e 302e 300d 0a09 6d79 7079  ov>=3.0.0...mypy
+00000320: 3e3d 302e 3934 320d 0a09 666c 616b 6538  >=0.942...flake8
+00000330: 3e3d 342e 302e 310d 0a09 746f 783e 3d33  >=4.0.1...tox>=3
+00000340: 2e32 352e 300d 0a0d 0a5b 6f70 7469 6f6e  .25.0....[option
+00000350: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
+00000360: 0a70 6c61 6e74 735f 736d 203d 2070 792e  .plants_sm = py.
+00000370: 7479 7065 640d 0a0d 0a5b 666c 616b 6538  typed....[flake8
+00000380: 5d0d 0a6d 6178 2d6c 696e 652d 6c65 6e67  ]..max-line-leng
+00000390: 7468 203d 2031 3630 0d0a 0d0a 5b65 6767  th = 160....[egg
+000003a0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000003b0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+000003c0: 2030 0d0a 0d0a                            0....
```

### Comparing `DielModels-1.0.1/src/DielModels.egg-info/SOURCES.txt` & `DielModels-1.0.2/src/DielModels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DielModels-1.0.1/src/diel_models/biomass_adjuster.py` & `DielModels-1.0.2/src/diel_models/biomass_adjuster.py`

 * *Files identical despite different names*

### Comparing `DielModels-1.0.1/src/diel_models/day_night_creator.py` & `DielModels-1.0.2/src/diel_models/day_night_creator.py`

 * *Files identical despite different names*

### Comparing `DielModels-1.0.1/src/diel_models/diel_models_creator.py` & `DielModels-1.0.2/src/diel_models/diel_models_creator.py`

 * *Files identical despite different names*

### Comparing `DielModels-1.0.1/src/diel_models/nitrate_uptake_ratio.py` & `DielModels-1.0.2/src/diel_models/nitrate_uptake_ratio.py`

 * *Files identical despite different names*

### Comparing `DielModels-1.0.1/src/diel_models/photon_reaction_inhibitor.py` & `DielModels-1.0.2/src/diel_models/photon_reaction_inhibitor.py`

 * *Files identical despite different names*

### Comparing `DielModels-1.0.1/src/diel_models/pipeline.py` & `DielModels-1.0.2/src/diel_models/pipeline.py`

 * *Files identical despite different names*

### Comparing `DielModels-1.0.1/src/diel_models/storage_pool_generator.py` & `DielModels-1.0.2/src/diel_models/storage_pool_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,20 @@
     def create_exchange_reaction(self, metabolite_id: str, metabolite_sp_id: str, direction: str) -> Reaction:
         """
         It creates a Reaction object representing an exchange reaction
         for the specified metabolite in the specified direction.
 
         Parameters
         ----------
-        metabolite_id
-        metabolite_sp_id
-        direction
+        metabolite_id: str
+            ID from original metabolite
+        metabolite_sp_id: str
+            ID from metabolite in sp
+        direction: str
+            Day or Night
 
         Returns
         -------
         Reaction object
         """
 
         met = self.model.metabolites.get_by_id(metabolite_sp_id)
```

