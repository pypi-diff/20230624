# Comparing `tmp/nonebot_plugin_maimai-0.2.2.tar.gz` & `tmp/nonebot_plugin_maimai-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_maimai-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_maimai-0.2.3.tar", max compression
```

## Comparing `nonebot_plugin_maimai-0.2.2.tar` & `nonebot_plugin_maimai-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-06-24 10:34:15.763557 nonebot_plugin_maimai-0.2.2/LICENSE
--rw-r--r--   0        0        0     3492 2023-06-24 10:34:15.763557 nonebot_plugin_maimai-0.2.2/README.md
--rw-r--r--   0        0        0    15374 2023-06-24 10:34:15.763557 nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 10:34:15.763557 nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/libraries/__init__.py
--rw-r--r--   0        0        0     1556 2023-06-24 10:34:15.763557 nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/libraries/image.py
--rw-r--r--   0        0        0    17432 2023-06-24 10:34:15.763557 nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/libraries/maimai_best_40.py
--rw-r--r--   0        0        0    17520 2023-06-24 10:34:15.763557 nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/libraries/maimai_best_50.py
--rw-r--r--   0        0        0     5353 2023-06-24 10:34:15.763557 nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/libraries/maimaidx_music.py
--rw-r--r--   0        0        0      385 2023-06-24 10:34:15.763557 nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/libraries/tool.py
--rw-r--r--   0        0        0     7312 2023-06-24 10:34:15.763557 nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/public.py
--rw-r--r--   0        0        0     1059 2023-06-24 10:34:15.763557 nonebot_plugin_maimai-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4525 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3492 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/README.md
+-rw-r--r--   0        0        0    15374 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/__init__.py
+-rw-r--r--   0        0        0     1556 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/image.py
+-rw-r--r--   0        0        0    17432 2023-06-24 14:36:40.711175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimai_best_40.py
+-rw-r--r--   0        0        0    17520 2023-06-24 14:36:40.715175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimai_best_50.py
+-rw-r--r--   0        0        0     5353 2023-06-24 14:36:40.715175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimaidx_music.py
+-rw-r--r--   0        0        0      385 2023-06-24 14:36:40.715175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/tool.py
+-rw-r--r--   0        0        0     7312 2023-06-24 14:36:40.715175 nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/public.py
+-rw-r--r--   0        0        0     1098 2023-06-24 14:36:40.715175 nonebot_plugin_maimai-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4587 1970-01-01 00:00:00.000000 nonebot_plugin_maimai-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_maimai-0.2.2/LICENSE` & `nonebot_plugin_maimai-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.2/README.md` & `nonebot_plugin_maimai-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/__init__.py` & `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     ...... .^...,.=O=@...OO@\      ,[O\=.    ./`.*.*OOOOO..OOO*..OO.,OOO
     ....../O....../^=O@`..O@@@@@]`    .* .,/@@/..../OOOOO*.,OOO..,OO`=OO
     @OO\ooO....,*/@^,@@@\..@^[\@@@@@@O]*]//[`@^*^*=OOOOOO^..=OO\...\^.\@
     OOooo^..`./oOO@/ =^\/^.^\\....=]......,/@@^O^*O.... .,][],OO\....\`.
     @Oooo\/]OOOOOO/  .  \.=^....,..........[.,OO^=^.    /    ,`\OO`.....
     """
 
-__version__ = "0.1.3"
+__version__ = "0.2.3"
 __plugin_meta__ = PluginMetadata(
     name="舞萌maimai",
     description='指令：舞萌帮助',
     usage=logo,
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_maimai",
     supported_adapters={"~onebot.v11"},
```

### Comparing `nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/libraries/image.py` & `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/libraries/maimai_best_40.py` & `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimai_best_40.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/libraries/maimai_best_50.py` & `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimai_best_50.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/libraries/maimaidx_music.py` & `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/libraries/maimaidx_music.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.2/nonebot_plugin_maimai/public.py` & `nonebot_plugin_maimai-0.2.3/nonebot_plugin_maimai/public.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_maimai-0.2.2/pyproject.toml` & `nonebot_plugin_maimai-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_maimai"
-version = "0.2.2"
+version = "0.2.3"
 description= "Maimai DX plugin for NoneBot"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_maimai"
 repository = "https://github.com/Agnes4m/nonebot_plugin_maimai"
 keywords = ["maimai", "nonebot2", "plugin"]
@@ -23,14 +23,15 @@
 ]
  
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = "^3.8.3"
 nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = ">=2.1.3"
+nonebot_plugin_htmlrender = "^0.2.0.3"
 pillow = ">=9.3.0"
 httpx = ">=0.22.0"
 nonebot-plugin-txt2img = "^0.3.0"
 bs4 = "^0.0.1"
  
 [tool.poetry.dev-dependencies]
```

### Comparing `nonebot_plugin_maimai-0.2.2/PKG-INFO` & `nonebot_plugin_maimai-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-maimai
-Version: 0.2.2
+Version: 0.2.3
 Summary: Maimai DX plugin for NoneBot
 Home-page: https://github.com/Agnes4m/nonebot_plugin_maimai
 License: MIT
 Keywords: maimai,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: httpx (>=0.22.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.3)
 Requires-Dist: nonebot-plugin-txt2img (>=0.3.0,<0.4.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0)
 Requires-Dist: pillow (>=9.3.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_maimai
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
   <br>
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-maimai Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-maimai Version: 0.2.3 Summary:
 Maimai DX plugin for NoneBot Home-page: https://github.com/Agnes4m/
 nonebot_plugin_maimai License: MIT Keywords: maimai,nonebot2,plugin Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: httpx (>=0.22.0) Requires-
 Dist: nonebot-adapter-onebot (>=2.1.3) Requires-Dist: nonebot-plugin-txt2img
-(>=0.3.0,<0.4.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist: pillow
-(>=9.3.0) Project-URL: Repository, https://github.com/Agnes4m/
-nonebot_plugin_maimai Description-Content-Type: text/markdown
+(>=0.3.0,<0.4.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist:
+nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0) Requires-Dist: pillow (>=9.3.0)
+Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_maimai
+Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot_plugin_maimai _â¨maimaiDXï¼nonebot2æä»¶çæ¬â¨_ [GitHub_stars]
               [GitHub_issues] [QQ_Chat_Group] [python] [NoneBot]
 ## è¯´æï¼å·²æ´æ°èèå½æ2023ï¼éæ°ä¸è½½èµæºï¼ ä»[mai-bot]
 (https://github.com/Diving-Fish/mai-
 bot)éénonebot2æä»¶ï¼æµè¯ç¯å¢nonebot2.0.0 ä¿®æ¹é¨åï¼ - b40/
```

