# Comparing `tmp/pyncm-1.6.9.0.1.tar.gz` & `tmp/pyncm-1.6.9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncm-1.6.9.0.1.tar", last modified: Wed Jun 14 05:25:35 2023, max compression
+gzip compressed data, was "pyncm-1.6.9.0.2.tar", last modified: Sat Jun 24 10:58:22 2023, max compression
```

## Comparing `pyncm-1.6.9.0.1.tar` & `pyncm-1.6.9.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.541209 pyncm-1.6.9.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.533208 pyncm-1.6.9.0.1/demos/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/二维码登录.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/云盘上传.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/手机登录.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/获取单曲下载链接.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/demos/足迹伪装.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/pyncm/
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28468 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/pyncm/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/album.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/artist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/cloudsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/difm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/sportsfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/miniprograms/zonefm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/apis/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/pyncm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/lrcparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyncm/utils/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:25:35.537208 pyncm-1.6.9.0.1/pyncm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 05:25:35.000000 pyncm-1.6.9.0.1/pyncm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 05:25:35.541209 pyncm-1.6.9.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-14 05:25:19.000000 pyncm-1.6.9.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:58:22.163691 pyncm-1.6.9.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-24 10:58:22.163691 pyncm-1.6.9.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:58:22.159691 pyncm-1.6.9.0.2/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/demos/二维码登录.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/demos/云盘上传.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/demos/手机登录.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/demos/获取单曲下载链接.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/demos/足迹伪装.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:58:22.159691 pyncm-1.6.9.0.2/pyncm/
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28446 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:58:22.163691 pyncm-1.6.9.0.2/pyncm/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/cloudsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:58:22.163691 pyncm-1.6.9.0.2/pyncm/apis/miniprograms/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/miniprograms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/miniprograms/difm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/miniprograms/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/miniprograms/sportsfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/miniprograms/zonefm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/apis/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:58:22.163691 pyncm-1.6.9.0.2/pyncm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/utils/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/utils/lrcparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyncm/utils/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:58:22.159691 pyncm-1.6.9.0.2/pyncm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-24 10:58:22.000000 pyncm-1.6.9.0.2/pyncm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-24 10:58:22.000000 pyncm-1.6.9.0.2/pyncm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:58:22.000000 pyncm-1.6.9.0.2/pyncm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-24 10:58:22.000000 pyncm-1.6.9.0.2/pyncm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 10:58:22.000000 pyncm-1.6.9.0.2/pyncm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-24 10:58:22.000000 pyncm-1.6.9.0.2/pyncm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 10:58:22.163691 pyncm-1.6.9.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-24 10:58:11.000000 pyncm-1.6.9.0.2/setup.py
```

### Comparing `pyncm-1.6.9.0.1/LICENSE` & `pyncm-1.6.9.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/PKG-INFO` & `pyncm-1.6.9.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyncm
-Version: 1.6.9.0.1
+Version: 1.6.9.0.2
 Summary: NeteaseCloudMusic APIs for Python 3.x 适用于 Python 3 的网易云音乐 API
 Home-page: https://github.com/greats3an/pyncm
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyncm-1.6.9.0.1/README.md` & `pyncm-1.6.9.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/demos/__init__.py` & `pyncm-1.6.9.0.2/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/demos/二维码登录.py` & `pyncm-1.6.9.0.2/demos/二维码登录.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/demos/云盘上传.py` & `pyncm-1.6.9.0.2/demos/云盘上传.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/demos/手机登录.py` & `pyncm-1.6.9.0.2/demos/手机登录.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/demos/足迹伪装.py` & `pyncm-1.6.9.0.2/demos/足迹伪装.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/__init__.py` & `pyncm-1.6.9.0.2/pyncm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     >>> pyncm.SetNewSession(
             pyncm.LoadSessionFromString(save)
         )
 
 # 注意事项
     - (PR#11) 海外用户可能经历 460 "Cheating" 问题，可通过添加以下 Header 解决: `X-Real-IP = 118.88.88.88`    
 """
-__version__ = "1.6.9.0.1"
+__version__ = "1.6.9.0.2"
 
 from threading import current_thread
 from typing import Text, Union
 from time import time
 from .utils.crypto import EapiEncrypt, EapiDecrypt, HexCompose
 import requests, logging, json, os
 logger = logging.getLogger("pyncm.api")
```

### Comparing `pyncm-1.6.9.0.1/pyncm/__main__.py` & `pyncm-1.6.9.0.2/pyncm/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
         for _id in ids:        
             logger.info(self.prefix + "：%s" % ArtistHelper(_id).ArtistName)
             # dList = artist.GetArtisTracks(_id,limit=self.args.count,order=self.args.sort_by)
             # This API is rather inconsistent for some reason. Sometimes 'songs' list
             # would be straight out empty
             # TODO: Fix GetArtistTracks
             # We iterate all Albums instead as this would provide a superset of what `GetArtistsTracks` gives us   
-            album_ids = [album['id'] for album in artist.GetArtistAlbums(_id,limit=self.args.count)['hotAlbums']]
+            album_ids = [album['id'] for album in artist.GetArtistAlbums(_id)['hotAlbums']]
             album_task = Album(self.args,self.put,prefix='艺术家专辑')
             album_task.forIds = self.forIds
             # All exceptions will still be handled by this subroutine
             # TODO: Try to... handle this nicer?
             queued += album_task(album_ids)                        
         return queued
```

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/__init__.py` & `pyncm-1.6.9.0.2/pyncm/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/album.py` & `pyncm-1.6.9.0.2/pyncm/apis/album.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/artist.py` & `pyncm-1.6.9.0.2/pyncm/apis/artist.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/cloud.py` & `pyncm-1.6.9.0.2/pyncm/apis/cloud.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/cloudsearch.py` & `pyncm-1.6.9.0.2/pyncm/apis/cloudsearch.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/login.py` & `pyncm-1.6.9.0.2/pyncm/apis/login.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/miniprograms/difm.py` & `pyncm-1.6.9.0.2/pyncm/apis/miniprograms/difm.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/miniprograms/radio.py` & `pyncm-1.6.9.0.2/pyncm/apis/miniprograms/radio.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/miniprograms/sportsfm.py` & `pyncm-1.6.9.0.2/pyncm/apis/miniprograms/sportsfm.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/miniprograms/zonefm.py` & `pyncm-1.6.9.0.2/pyncm/apis/miniprograms/zonefm.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/playlist.py` & `pyncm-1.6.9.0.2/pyncm/apis/playlist.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/track.py` & `pyncm-1.6.9.0.2/pyncm/apis/track.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/user.py` & `pyncm-1.6.9.0.2/pyncm/apis/user.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/apis/video.py` & `pyncm-1.6.9.0.2/pyncm/apis/video.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/utils/__init__.py` & `pyncm-1.6.9.0.2/pyncm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/utils/aes.py` & `pyncm-1.6.9.0.2/pyncm/utils/aes.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/utils/crypto.py` & `pyncm-1.6.9.0.2/pyncm/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/utils/helper.py` & `pyncm-1.6.9.0.2/pyncm/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/utils/lrcparser.py` & `pyncm-1.6.9.0.2/pyncm/utils/lrcparser.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm/utils/security.py` & `pyncm-1.6.9.0.2/pyncm/utils/security.py`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/pyncm.egg-info/PKG-INFO` & `pyncm-1.6.9.0.2/pyncm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyncm
-Version: 1.6.9.0.1
+Version: 1.6.9.0.2
 Summary: NeteaseCloudMusic APIs for Python 3.x 适用于 Python 3 的网易云音乐 API
 Home-page: https://github.com/greats3an/pyncm
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyncm-1.6.9.0.1/pyncm.egg-info/SOURCES.txt` & `pyncm-1.6.9.0.2/pyncm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyncm-1.6.9.0.1/setup.py` & `pyncm-1.6.9.0.2/setup.py`

 * *Files identical despite different names*

