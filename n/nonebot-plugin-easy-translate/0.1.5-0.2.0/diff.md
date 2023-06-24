# Comparing `tmp/nonebot_plugin_easy_translate-0.1.5.tar.gz` & `tmp/nonebot_plugin_easy_translate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_easy_translate-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_easy_translate-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_easy_translate-0.1.5.tar` & `nonebot_plugin_easy_translate-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,11 @@
--rw-r--r--   0        0        0     2361 2023-01-16 14:22:35.455596 nonebot_plugin_easy_translate-0.1.5/nonebot_plugin_easy_translate/__init__.py
--rw-r--r--   0        0        0     3116 2023-01-24 15:19:05.268736 nonebot_plugin_easy_translate-0.1.5/nonebot_plugin_easy_translate/config.py
--rw-r--r--   0        0        0      923 2023-03-01 02:18:22.898498 nonebot_plugin_easy_translate-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1992 2023-01-24 15:19:28.357807 nonebot_plugin_easy_translate-0.1.5/README.md
--rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 nonebot_plugin_easy_translate-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2194 2023-06-24 12:33:36.404972 nonebot_plugin_easy_translate-0.2.0/nonebot_plugin_easy_translate/__init__.py
+-rw-r--r--   0        0        0     3195 2023-06-24 12:33:16.346476 nonebot_plugin_easy_translate-0.2.0/nonebot_plugin_easy_translate/config.py
+-rw-r--r--   0        0        0    16361 2023-06-24 12:30:09.439709 nonebot_plugin_easy_translate-0.2.0/nonebot_plugin_easy_translate/gtranslate/client.py
+-rw-r--r--   0        0        0     9264 2023-06-24 12:11:01.581303 nonebot_plugin_easy_translate-0.2.0/nonebot_plugin_easy_translate/gtranslate/constants.py
+-rw-r--r--   0        0        0     7615 2023-06-24 12:11:43.143487 nonebot_plugin_easy_translate-0.2.0/nonebot_plugin_easy_translate/gtranslate/gtoken.py
+-rw-r--r--   0        0        0     2127 2023-06-24 12:03:29.009358 nonebot_plugin_easy_translate-0.2.0/nonebot_plugin_easy_translate/gtranslate/models.py
+-rw-r--r--   0        0        0      248 2023-06-24 10:11:44.621612 nonebot_plugin_easy_translate-0.2.0/nonebot_plugin_easy_translate/gtranslate/urls.py
+-rw-r--r--   0        0        0     1980 2023-06-24 10:11:44.446199 nonebot_plugin_easy_translate-0.2.0/nonebot_plugin_easy_translate/gtranslate/utils.py
+-rw-r--r--   0        0        0      913 2023-06-24 12:45:56.929961 nonebot_plugin_easy_translate-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2014 2023-06-24 12:45:17.208902 nonebot_plugin_easy_translate-0.2.0/README.md
+-rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 nonebot_plugin_easy_translate-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_easy_translate-0.1.5/nonebot_plugin_easy_translate/__init__.py` & `nonebot_plugin_easy_translate-0.2.0/nonebot_plugin_easy_translate/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     GroupMessageEvent,
     MessageEvent,
     PrivateMessageEvent,
 )
 from nonebot.params import RegexGroup
 from nonebot.plugin import PluginMetadata
 from .config import pc, var
+from gtranslate.client import Translator
 
 __plugin_meta__ = PluginMetadata(
     name="简单翻译插件",
     description="免key翻译，使用谷歌翻译",
     usage=f"""插件命令如下：
 翻译/x译x  # 试试就知道怎么用了
 """,
@@ -34,44 +35,42 @@
 @fanyi.handle()
 async def handle_fanyi(matchgroup=RegexGroup()):
     in_ = matchgroup[3]
     if not in_:
         await fanyi.finish("翻译/x译x [内容]\n直接翻译是自动识别，x是指定语言\nx支持：中（简中）、繁（繁中）、英、日、韩、法、俄、德")
 
     dd = {
-        "中": "zh-CN",
-        "繁": "zh-TW",
+        "中": "zh-cn",
+        "繁": "zh-tw",
         "英": "en",
         "日": "ja",
         "韩": "ko",
         "法": "fr",
         "俄": "ru",
         "德": "de",
     }
 
     if matchgroup[0] == "翻译":
-        from_ = "auto"
-        to_ = "auto"
+        src = "auto"
+        dest = "zh-cn"
     else:
         try:
-            from_ = dd[matchgroup[1]]
-            to_ = dd[matchgroup[2]]
+            src = dd[matchgroup[1]]
+            dest = dd[matchgroup[2]]
         except KeyError:
             await fanyi.finish("不支持该语种")
 
-    data = {"data": [in_, from_, to_]}
-    async with AsyncClient(verify=False, follow_redirects=True) as c:
-        resp = await c.post(
-            "https://hf.space/embed/mikeee/gradio-gtr/+/api/predict", json=data
-        )
-        if resp.status_code != 200:
-            await fanyi.finish(f"翻译接口调用失败\n错误代码{resp.status_code},{resp.text}")
-
-        result = resp.json()
-        result = result["data"][0]
+    try:
+        result = (
+            await Translator(proxies=pc.easy_translate_http_proxy).translate(
+                in_, dest=dest, src=src
+            )
+        ).text
+    except Exception as e:
+        result = repr(e)
 
     await fanyi.finish(result)
 
     # 有道 免key翻译
     # params = {"q": in_mess, "from": ff, "to": tt}
     # async with AsyncClient(
     #     verify=False,
```

### Comparing `nonebot_plugin_easy_translate-0.1.5/nonebot_plugin_easy_translate/config.py` & `nonebot_plugin_easy_translate-0.2.0/nonebot_plugin_easy_translate/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,41 +4,44 @@
 from nonebot.adapters import Bot
 from typing import Optional, List, Dict, Tuple
 
 
 class Config(BaseModel, extra=Extra.ignore):
     # 机器人的QQ号（如果写了就按优先级响应，否则就第一个连上的响应） ['1234','5678','6666']
     easy_translate_bot_qqnum_list: List[str] = []  # 可选
+    # 代理
+    easy_translate_http_proxy: Optional[str] = None  # 可选
 
 
 class Var:
     # 处理消息的bot
     handle_bot: Optional[Bot] = None
 
 
 driver = get_driver()
 
 pc = Config.parse_obj(driver.config)
 var = Var()
 
+
 # qq机器人连接时执行
 @driver.on_bot_connect
 async def on_bot_connect(bot: Bot):
     # 是否有写bot qq，如果写了只处理bot qq在列表里的
     if (
         pc.easy_translate_bot_qqnum_list
         and bot.self_id in pc.easy_translate_bot_qqnum_list
     ):
         # 如果已经有bot连了
         if var.handle_bot:
             # 当前bot qq 下标
             handle_bot_id_index = pc.easy_translate_bot_qqnum_list.index(
                 var.handle_bot.self_id
             )
-            # 连过俩的bot qq 下标
+            # 新连接的bot qq 下标
             new_bot_id_index = pc.easy_translate_bot_qqnum_list.index(bot.self_id)
             # 判断优先级，下标越低优先级越高
             if new_bot_id_index < handle_bot_id_index:
                 var.handle_bot = bot
 
         # 没bot连就直接给
         else:
```

### Comparing `nonebot_plugin_easy_translate-0.1.5/pyproject.toml` & `nonebot_plugin_easy_translate-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nonebot_plugin_easy_translate"
-version = "0.1.5"
-description = "Nonebot2 免api key简单翻译插件"
+version = "0.2.0"
+description = "Nonebot2 谷歌翻译插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_easy_translate"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_easy_translate"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_easy_translate"
 documentation = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_easy_translate#README.md"
```

### Comparing `nonebot_plugin_easy_translate-0.1.5/PKG-INFO` & `nonebot_plugin_easy_translate-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-easy-translate
-Version: 0.1.5
-Summary: Nonebot2 免api key简单翻译插件
+Version: 0.2.0
+Summary: Nonebot2 谷歌翻译插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_easy_translate
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -39,16 +39,15 @@
   <a href="https://v2.nonebot.dev/">
     <img src="https://img.shields.io/static/v1?label=nonebot&message=v2rc1%2B&color=green" alt="nonebot2">
   </a>
   <img src="https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue" alt="python">
 </p>
 
 ## 简介
-使用了sena-nana大佬给的接口，他的仓库
-<a href="https://github.com/sena-nana/nonebot-plugin-novelai/blob/main/nonebot_plugin_novelai/extension/translation.py">sena-nana/nonebot-plugin-novelai</a>，不需要使用梯子和api key就能使用的翻译插件
+之前的免梯谷歌翻译接口寄了，现在用的是[谷歌翻译库](https://py-googletrans.readthedocs.io/en/latest/#googletrans.Translator.translate)，我把代码改成异步然后当插件用了，得用梯子
 
 <img width="500" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_easy_translate/readme_img/fanyi.jpg"/>
 
 ## 安装
 
 使用nb-cli安装
 ```bash
@@ -69,14 +68,18 @@
 
 ## 插件命令  
 | 指令 | 说明 |
 |:-----:|:----:|
 | 翻译 | 你发一下就知道啦 |
 
 ## 更新日志
+### 2023/6/24 \[v0.2.0]
+
+* 改用谷歌翻译库，需要梯子了
+
 ### 2023/1/24 \[v0.1.4]
 
 * 修复多bot处理bug
 
 ### 2023/1/16 \[v0.1.3]
 
 * 最低python版本兼容至3.8
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-easy-translate Version: 0.1.5
-Summary: Nonebot2 åapi keyç®åç¿»è¯æä»¶ Home-page: https://github.com/
-nikissXI/nonebot_plugins/tree/main/nonebot_plugin_easy_translate License: MIT
-Author: nikissXI Author-email: 1299577815@qq.com Requires-Python: >=3.8
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.22.0) Requires-Dist: nonebot-adapter-onebot (>=2.0.0)
+Metadata-Version: 2.1 Name: nonebot-plugin-easy-translate Version: 0.2.0
+Summary: Nonebot2 è°·æ­ç¿»è¯æä»¶ Home-page: https://github.com/nikissXI/
+nonebot_plugins/tree/main/nonebot_plugin_easy_translate License: MIT Author:
+nikissXI Author-email: 1299577815@qq.com Requires-Python: >=3.8 Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Dist: httpx (>=0.22.0) Requires-Dist: nonebot-adapter-onebot (>=2.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc1) Project-URL: Documentation, https://
 github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_easy_translate#README.md Project-URL: Repository, https://
 github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_easy_translate
 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                  # nonebot_plugin_easy_translate _â¨ Nonebot2
                 ç®åæç¨è°·æ­ç¿»è¯æä»¶ï¼åkeyï¼ â¨_
                          [license] [nonebot2] [python]
-## ç®ä» ä½¿ç¨äºsena-nanaå¤§ä½¬ç»çæ¥å£ï¼ä»çä»åº sena-nana/
-nonebot-plugin-novelaiï¼ä¸éè¦ä½¿ç¨æ¢¯å­åapi
-keyå°±è½ä½¿ç¨çç¿»è¯æä»¶ [https://raw.githubusercontent.com/nikissXI/
-nonebot_plugins/main/nonebot_plugin_easy_translate/readme_img/fanyi.jpg] ##
-å®è£ ä½¿ç¨nb-cliå®è£ ```bash nb plugin install
-nonebot_plugin_easy_translate ``` æè
+## ç®ä» ä¹åçåæ¢¯è°·æ­ç¿»è¯æ¥å£å¯äºï¼ç°å¨ç¨çæ¯
+[è°·æ­ç¿»è¯åº](https://py-googletrans.readthedocs.io/en/latest/
+#googletrans.Translator.translate)ï¼ææä»£ç æ¹æå¼æ­¥ç¶åå½æä»¶ç¨äºï¼å¾ç¨æ¢¯å­
+[https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/
+nonebot_plugin_easy_translate/readme_img/fanyi.jpg] ## å®è£ ä½¿ç¨nb-
+cliå®è£ ```bash nb plugin install nonebot_plugin_easy_translate ``` æè
 ç´æ¥ææä»¶cloneä¸æ¥æ¾è¿å»pluginsæä»¶å¤¹ ## å¯ééç½®
 å¨botå¯¹åºç.envæä»¶ä¿®æ¹ ```bash #
 æºå¨äººçQQå·åè¡¨ï¼å¦ææå¤ä¸ªbotè¿æ¥ï¼ä¼æç§å¡«åçlistï¼å·¦è¾¹çæºå¨äººQQä¼åçº§æé«
 1234 > 5678 > 6666ï¼ä¼èªå¨åæ¢ #
 å¦æä¸å¡«è¯¥éç½®åç±ç¬¬ä¸ä¸ªè¿ä¸çbotååº
 easy_translate_bot_qqnum_list = [1234,5678,6666] ``` ## æä»¶å½ä»¤ | æä»¤ |
 è¯´æ | |:-----:|:----:| | ç¿»è¯ | ä½ åä¸ä¸å°±ç¥éå¦ | ## æ´æ°æ¥å¿
-### 2023/1/24 \[v0.1.4] * ä¿®å¤å¤botå¤çbug ### 2023/1/16 \[v0.1.3] *
+### 2023/6/24 \[v0.2.0] * æ¹ç¨è°·æ­ç¿»è¯åºï¼éè¦æ¢¯å­äº ### 2023/1/24
+\[v0.1.4] * ä¿®å¤å¤botå¤çbug ### 2023/1/16 \[v0.1.3] *
 æä½pythonçæ¬å¼å®¹è³3.8 ### 2023/1/15 \[v0.1.2] * åå¸æä»¶
```

