# Comparing `tmp/nonebot_plugin_game_collection-2.2.7.tar.gz` & `tmp/nonebot_plugin_game_collection-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.2.7.tar", last modified: Fri Jun 23 21:49:34 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.2.8.tar", last modified: Sat Jun 24 17:04:14 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.2.7.tar` & `nonebot_plugin_game_collection-2.2.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.338017 nonebot_plugin_game_collection-2.2.7/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.7/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-06-23 21:49:34.336015 nonebot_plugin_game_collection-2.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.268810 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    19558 2023-06-23 21:38:06.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    60126 2023-06-22 17:20:27.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.287689 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9182 2023-06-20 12:33:55.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    13713 2023-06-23 11:42:31.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    19332 2023-06-23 14:22:48.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    18448 2023-06-23 21:09:29.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    29223 2023-06-23 14:03:04.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/config.py
--rw-rw-rw-   0        0        0     5586 2023-06-20 12:48:06.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/data.py
-drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.294698 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.323003 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12958 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5166 2023-06-23 21:28:38.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.327747 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2278 2023-06-20 13:08:13.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.333997 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0    13602 2023-06-23 21:48:13.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1141 2023-06-23 21:24:50.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.278019 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-06-23 21:49:34.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1947 2023-06-23 21:49:34.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 21:49:34.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-23 21:49:34.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-23 21:49:34.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 21:49:34.338017 nonebot_plugin_game_collection-2.2.7/setup.cfg
--rw-rw-rw-   0        0        0      710 2023-06-23 21:49:23.000000 nonebot_plugin_game_collection-2.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.189350 nonebot_plugin_game_collection-2.2.8/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.8/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-06-24 17:04:14.188849 nonebot_plugin_game_collection-2.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.125795 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    19529 2023-06-24 16:29:41.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    60126 2023-06-22 17:20:27.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.144312 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9182 2023-06-20 12:33:55.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    13713 2023-06-23 11:42:31.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    19332 2023-06-23 14:22:48.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    23191 2023-06-24 16:59:38.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    29223 2023-06-23 14:03:04.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/config.py
+-rw-rw-rw-   0        0        0     5586 2023-06-20 12:48:06.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/data.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.151318 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.176339 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12958 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5335 2023-06-24 06:35:42.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.178341 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2278 2023-06-20 13:08:13.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.186848 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0    16012 2023-06-24 16:57:10.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1141 2023-06-23 21:24:50.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:04:14.135303 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-24 17:04:13.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1947 2023-06-24 17:04:14.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 17:04:13.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-24 17:04:13.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-24 17:04:13.000000 nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 17:04:14.189851 nonebot_plugin_game_collection-2.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      710 2023-06-24 17:04:09.000000 nonebot_plugin_game_collection-2.2.8/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.2.7/LICENSE` & `nonebot_plugin_game_collection-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/README.md` & `nonebot_plugin_game_collection-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Account.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,15 @@
     info.append(my_info_account(msg,dist))
 
     # 加载股票信息
     msg = ""
     for stock in group_account.stocks:
         company_name = group_data[stock].company.company_name
         if i := group_account.stocks[stock]:
-            msg += f"[font_normal]{company_name}[nowrap]\n[right][color][green]{i}\n"
+            msg += f"{company_name}[nowrap]\n[right][color][green]{i}\n"
     if msg:
         info.append(linecard(msg, 880,endline = "股票信息"))
 
     return MessageSegment.image(info_Splicing(info,BG_path(event.user_id)))
 
 def my_props(event:MessageEvent) -> Message:
     """
@@ -333,15 +333,15 @@
         quant = "天" if prop_code[2] == "0" else "个"
         prop = props_library.get(prop_code,{"name": prop_code, "color": "black","rare": 1,"intro": "未知","des": "未知"})
 
         color = prop['color']
         name = prop['name']
         rare = prop['rare']
         msg = (
-            f"[font_big][color][{color}]【{name}】[nowrap]\n[right][font_big][color][{color}]{n}{quant}\n"
+            f"[font_big][color][{color}]【{name}】[nowrap][passport]\n[right]{n}{quant}\n"
             "----\n"
             + prop['intro'] + f"\n[right]{prop['des']}\n"
             )
 
         info.append(
             linecard(msg,
                      width = 880,
```

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Market.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/Prop.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     MessageEvent,
     GroupMessageEvent,
     MessageSegment
     )
 import random
 
 from .utils.utils import get_message_at
-from .utils.chart import linecard,gacha_info
+from .utils.chart import linecard_to_png
 from .data import props_library, props_index, element_library
 from .config import bot_name, sign_gold, revolt_gold, max_bet_gold, gacha_gold
 
 from .Manager import data,BG_path
 from . import Manager
 
 user_data = data.user
@@ -45,14 +45,43 @@
         props = random.choice(["61001","62101"])
     elif code == 52:
         props = random.choice(["63101","63102"])
     else:
         props = "11001"
     return props
 
+def random_airs() -> str:
+    """
+    随机获取道具。
+        rare:稀有度
+        return:道具代码
+        道具代码规则：
+        第1位：稀有度
+        第2位：道具性质：
+            1：空气
+            2：群内道具
+            3：全局道具
+        第3位：道具时效：
+            0：时效道具
+            1：永久道具
+        4,5位：本稀有度下的道具编号
+    """
+    code = random.randint(1,100)
+    if 0 < code <= 30:
+        props = "31001"
+    elif 30 < code <= 40:
+        props = "41001"
+    elif 40 < code <= 50:
+        props = random.choice(["51001","51002"])
+    elif code == 51:
+        props = "61001"
+    else:
+        props = "11001"
+    return props
+
 def gacha(event:MessageEvent, N:int):
     """
     抽卡
     """
     user,group_account = Manager.locate_user(event)
     if not group_account:
         return "私聊未关联账户，请发送【关联账户】关联群内账户。"
@@ -73,15 +102,15 @@
         star += rare
         if prop_code[1] == '1':
             airstar += rare
             air += 1
     else:
         data = sorted(res.items(),key = lambda x:int(x[0]),reverse=True)
 
-    info = []
+    msg = ""
     airdata = []
     for prop_code, n in data:
         if prop_code[1] == "2":
             props = group_account.props
             props.setdefault(prop_code,0)
             props[prop_code] += n
             quant =  "天" if prop_code[2] == "0" else "个"
@@ -93,84 +122,95 @@
         else:
             airdata.append((prop_code, n))
             continue
         prop_info = props_library.get(prop_code,{"name":prop_code, "color":"black","rare":1,"intro":"未知","des":"未知"})
         color = prop_info['color']
         name = prop_info['name']
         rare = prop_info['rare']
-        info.append(
-            linecard(f"[color][{color}]【{name}】[nowrap]\n[right][color][{color}]{n}{quant}\n",
-                     width = 440,
-                     height = 120,
-                     padding=(0,10),
-                     endline = rare*'☆',
-                     bg_color = "white"
-                     ))
-    user.props = {k:10 if k[2] == '0' and v > 30 else v for k, v in user.props.items()}
-    group_account.props = {k:v if v < 30 else 30 for k,v in group_account.props.items()}
-    if len(info)%2 == 1:
-        info.append(None)
+        msg += (
+            f"[color][{color}]{name}[nowrap][passport]\n"
+            f"[pixel][450]{rare*'☆'}[nowrap][passport]\n"
+            f"[right]{n}{quant}\n"
+            )
 
+    user.props = {k: v if k == "33101" else min(v, 30) for k, v in user.props.items()}
+    group_account.props = {k:min(30,v) for k,v in group_account.props.items()}
     for prop_code, n in airdata:
         prop_info = props_library.get(prop_code,{"name":prop_code, "color":"black","rare":1,"intro":"未知","des":"未知"})
         color = prop_info['color']
         name = prop_info['name']
         rare = prop_info['rare']
-        info.append(
-            linecard(f"[color][{color}]【{name}】[nowrap]\n[right][color][{color}]{n}次\n",
-                        width = 440,
-                        height = 120,
-                        padding=(0,10),
-                        endline = rare*'☆',
-                        bg_color = "white"
-                        ))
-    pt = star/N
-    if pt < 1.6:
-        level = "[color][#003300]理 想 气 体"
-    if pt < 1.88:
-        level = "[color][#003333]☆ 数据异常 ☆"
-    elif pt < 2.16:
-        level = "[color][#003366]☆☆ 一枚硬币 ☆☆"
-    elif pt < 2.44:
-        level = "[color][#003399]☆☆☆ 高斯分布 ☆☆☆"
-    elif pt < 2.72:
-        level = "[color][#0033CC]☆☆☆☆ 对称破缺 ☆☆☆☆"
-    elif pt < 3:
-        level = "[color][#0033FF]☆☆☆☆☆ 概率之子 ☆☆☆☆☆"
-    else:
-        level = "[color][#FF0000]☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆"
+        msg += (
+            f"[color][{color}]{name}[nowrap][passport]\n"
+            f"[pixel][450]{rare*'☆'}[nowrap][passport]\n"
+            f"[right]{n}个\n"
+            )
 
     if N >= 10:
+        pt = star/N
+        if pt < 1.6 or (air/N) > 0.8:
+            if air == N:
+                level = "[center][color][#003300]只 有 空 气"
+                user.gold += cost
+                group_account.gold += cost
+                msg = f"本次抽卡已免费（{cost}金币）\n" + msg
+            else:
+                level = "[center][color][#003300]理 想 气 体"
+            n = N//10
+            user.props.setdefault("03103",0)
+            user.props["03103"] += n
+            prop_info = props_library.get("03103",{"name":"03103", "color":"black","rare":1,"intro":"未知","des":"未知"})
+            color = prop_info['color']
+            name = prop_info['name']
+            msg += (
+                f"[color][{color}]{name}[nowrap][passport]\n"
+                f"[right]{n}个\n"
+                )
+        elif pt < 1.88:
+            level = "[left][color][#003333]☆[nowrap][passport]\n[center]数据异常[nowrap][passport]\n[right]☆"
+        elif pt < 2.16:
+            level = "[left][color][#003366]☆ ☆[nowrap][passport]\n[center]一枚硬币[nowrap][passport]\n[right]☆ ☆"
+        elif pt < 2.44:
+            level = "[left][color][#003399]☆ ☆ ☆[nowrap][passport]\n[center]高斯分布[nowrap][passport]\n[right]☆ ☆ ☆"
+        elif pt < 2.72:
+            level = "[left][color][#0033CC]☆ ☆ ☆ ☆[nowrap][passport]\n[center]对称破缺[nowrap][passport]\n[right]☆ ☆ ☆ ☆"
+        elif pt < 3:
+            level = "[left][color][#0033FF]☆ ☆ ☆ ☆ ☆[nowrap][passport]\n[center]概率之子[nowrap][passport]\n[right]☆ ☆ ☆ ☆ ☆"
+        else:
+            level = "[noautowrap][center][color][#FF0000]☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆"
         msg = (
-            f"{group_account.nickname}\n"
+            f"{level}\n"
             "----\n"
             f"抽卡次数：{N}[nowrap]\n"f"[pixel][450]空气占比：{round(air*100/N,2)}%\n"
             f"获得☆：{star}[nowrap]\n"f"[pixel][450]获得☆：{airstar}\n"
             f"平均每抽☆数：{round(pt,3)}[nowrap]\n"f"[pixel][450]空气质量：{round(airstar/air,3)}\n"
-            f"结果评定：[nowrap]\n{level}\n"
-            )
+            f"数据来源：{group_account.nickname}\n"
+            "----\n"
+            ) + msg
     else:
         msg = (
             f"{group_account.nickname}\n"
             "----\n"
             f"抽卡次数：{N}\n"
-            )
-        
+            "----\n"
+            ) + msg
         
-    return MessageSegment.image(gacha_info(linecard(msg,width = 880,endline = f"抽卡报告",bg_color = "white"),info))
+    return MessageSegment.image(linecard_to_png(msg))
 
 class Prop(str):
     def use(self, event:MessageEvent, count:int):
         """
         使用道具
         """
         if self == "03101":
             return self.use_03101(event,count)
         elif self == "03100":
             return self.use_03100(event)
+        elif self == "03103":
+            return self.use_03103(event,count)
         elif self == "33101":
             return self.use_33101(event,count)
         elif self == "42101":
             return self.use_42101(event)
         elif self == "52101":
             return self.use_52101(event)
         elif self == "52102":
@@ -220,14 +260,91 @@
 
         gold = count * max_bet_gold
         user.gold += gold
         group_account.gold += gold
         return f"你获得了{gold}金币。"
 
     @classmethod
+    def use_03103(cls, event:MessageEvent, count:int) -> str:
+        """
+        使用道具：空气礼包
+        """
+        user,group_account = Manager.locate_user(event)
+        if not group_account:
+            return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        props = user.props
+        if props.get("03103",0) < count:
+            return "数量不足"
+
+        props["03103"] -= count
+        if props["03103"] < 1:
+            del props["03103"]
+
+        N = count*10
+
+        res = {}
+        star = 0
+        airstar = 0
+        air = 0
+        for i in range(N):
+            prop_code = random_airs()
+            res.setdefault(prop_code,0)
+            res[prop_code] += 1
+            rare = int(prop_code[0])
+            star += rare
+            airstar += rare
+            air += 1
+        else:
+            data = sorted(res.items(),key = lambda x:int(x[0]),reverse=True)
+
+        msg = ""
+        props = group_account.props
+        for prop_code, n in data:
+            props.setdefault(prop_code,0)
+            props[prop_code] += n
+            prop_info = props_library.get(prop_code,{"name":prop_code, "color":"black","rare":1,"intro":"未知","des":"未知"})
+            color = prop_info['color']
+            name = prop_info['name']
+            rare = prop_info['rare']
+            msg += (
+                f"[color][{color}]{name}[nowrap][passport]\n"
+                f"[pixel][450]{rare*'☆'}[nowrap][passport]\n"
+                f"[right]{n}个\n"
+                )
+
+
+        pt = star/N
+        if pt < 1.6:
+            level = "[center][color][#003300]杂质级"
+        elif pt < 1.88:
+            level = "[left][color][#003333]☆[nowrap][passport]\n[center]工业级[nowrap][passport]\n[right]☆"
+        elif pt < 2.16:
+            level = "[left][color][#003366]☆ ☆[nowrap][passport]\n[center]试剂级[nowrap][passport]\n[right]☆ ☆"
+        elif pt < 2.44:
+            level = "[left][color][#003399]☆ ☆ ☆[nowrap][passport]\n[center]实验级[nowrap][passport]\n[right]☆ ☆ ☆"
+        elif pt < 2.72:
+            level = "[left][color][#0033CC]☆ ☆ ☆ ☆[nowrap][passport]\n[center]分析级[nowrap][passport]\n[right]☆ ☆ ☆ ☆"
+        elif pt < 3:
+            level = "[left][color][#0033FF]☆ ☆ ☆ ☆ ☆[nowrap][passport]\n[center]超纯级[nowrap][passport]\n[right]☆ ☆ ☆ ☆ ☆"
+        else:
+            level = "[noautowrap][center][color][#FF0000]☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆"
+
+        msg = (
+            f"{level}\n"
+            "----\n"
+            f"抽卡次数：{N}[nowrap]\n"f"[pixel][450]空气占比：{round(air*100/N,2)}%\n"
+            f"获得☆：{star}[nowrap]\n"f"[pixel][450]获得☆：{airstar}\n"
+            f"平均每抽☆数：{round(pt,3)}[nowrap]\n"f"[pixel][450]空气质量：{round(airstar/air,3)}\n"
+            f"数据来源：{group_account.nickname}\n"
+            "----\n"
+            ) + msg
+
+        return MessageSegment.image(linecard_to_png(msg))
+
+    @classmethod
     def use_33101(cls, event:MessageEvent, count:int) -> str:
         """
         使用道具：初级元素
         """
         user,group_account = Manager.locate_user(event)
         if not group_account:
             return "私聊未关联账户，请发送【关联账户】关联群内账户。"
```

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/data.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.954%*

 * *Differences: {"'03103'": "OrderedDict([('name', '空气礼包'), ('color', '#66CCFF'), ('rare', 0), ('intro', "*

 * *            "'可以获得10个随机空气!'), ('des', 'pV=nRT')])",*

 * * "'31001'": "{'intro': '与空气相比，这个比较优质。\\n......'}",*

 * * "'61001'": "{'intro': '纯净', 'des': '空气'}"}*

```diff
@@ -23,25 +23,32 @@
     "03102": {
         "color": "#0033FF ",
         "des": "\u611f\u8c22\u60a8\u7684\u8d21\u732e\u3002",
         "intro": "\u60a8\u7cbe\u51c6\u7684\u5b9a\u4f4d\u5230\u4e86\u7a0b\u5e8f\u7684\u6f0f\u6d1e\u5e76\u5c06\u5176\u53cd\u9988\u7ed9\u4e86\u5f00\u53d1\u8005\u3002",
         "name": "Debug\u5956\u7ae0",
         "rare": 0
     },
+    "03103": {
+        "color": "#66CCFF",
+        "des": "pV=nRT",
+        "intro": "\u53ef\u4ee5\u83b7\u5f9710\u4e2a\u968f\u673a\u7a7a\u6c14!",
+        "name": "\u7a7a\u6c14\u793c\u5305",
+        "rare": 0
+    },
     "11001": {
         "color": "#66CCFF",
         "des": "\u9664\u4e86\u7a7a\u6c14\u3002",
         "intro": "\u5982\u4f60\u6240\u89c1\uff0c\u8fd9\u91cc\u4ec0\u4e48\u4e5f\u6ca1\u6709\u3002",
         "name": "\u7a7a\u6c14",
         "rare": 1
     },
     "31001": {
         "color": "#66CCFF",
         "des": "\uff08\u4e00\u672c\u6b63\u7ecf\u7684\u80e1\u8bf4\u516b\u9053\uff09",
-        "intro": "\u4e0e\u7a7a\u6c14\u76f8\u6bd4\uff0c\u8fd9\u4e2a\u6bd4\u8f83\u4f18\u8d28\u3002\n\n......",
+        "intro": "\u4e0e\u7a7a\u6c14\u76f8\u6bd4\uff0c\u8fd9\u4e2a\u6bd4\u8f83\u4f18\u8d28\u3002\n......",
         "name": "\u4f18\u8d28\u7a7a\u6c14",
         "rare": 3
     },
     "32001": {
         "color": "#228B22",
         "des": "\u606d\u559c\u4f60\u83b7\u5f97\u4e86\u672c\u6b21\u6d3b\u52a8\u7684\u7eaa\u5ff5\u5956\u3002",
         "intro": "\u53ef\u4ee5\u5728\u8d44\u6599\u5361\u6216\u8005\u7ed3\u7b97\u754c\u9762\u4e0a\u663e\u793a\u56db\u53f6\u8349\u6807\u8bb0\uff0c\u4f46\u4f3c\u4e4e\u5e76\u6ca1\u6709\u4ec0\u4e48\u7528\u5904\u3002",
@@ -137,16 +144,16 @@
         "des": "\u611f\u8c22\u5404\u4f4d\u73a9\u5bb6\u7684\u652f\u6301\uff01",
         "intro": "\u6253\u5f00\u540e\u53ef\u4ee5\u83b7\u5f97\u3010\u91d1\u5e01\u7b7e\u5230-\u91cd\u7f6e\u7b7e\u5230\u3011\u8303\u56f4\u7684\u968f\u673a\u91d1\u5e01\u3002",
         "name": "\u968f\u673a\u7ea2\u5305",
         "rare": 5
     },
     "61001": {
         "color": "#66CCFF",
-        "des": "",
-        "intro": "",
+        "des": "\u7a7a\u6c14",
+        "intro": "\u7eaf\u51c0",
         "name": "\u7eaf\u51c0\u7a7a\u6c14",
         "rare": 6
     },
     "62101": {
         "color": "#0099FF",
         "des": "\u53ef\u4ee5\u7528\u6765\u3002\u3002\u3002",
         "intro": "\u65e0\u6bd4\u73cd\u8d35\u7684\u94bb\u77f3\uff0c\u53ea\u6709\u5343\u5206\u4e4b\u4e94\u7684\u6982\u7387\u83b7\u5f97\uff0c\u4ee5\u540e\u53ef\u80fd\u6709\u7528\u3002",
```

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/chart.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,14 +76,47 @@
         draw.text((x, y), line, font = font, fill = text_color)
         y += line_height
 
     output = BytesIO()
     image.save(output, format="png")
     return output
 
+import re
+
+class linecard_pattern:
+    align = re.compile(r"\[left\]|\[right\]|\[center\]|\[pixel\]\[.*?\]")
+    font = re.compile(r"\[font_big\]|\[font_normal\]|\[font_small\]|\[font\]\[.*?\]\[.*?\]")
+    color = re.compile(r"\[color\]\[.*?\]")
+    passport = re.compile(r"\[passport\]")
+    nowrap = re.compile(r"\[nowrap\]")
+    noautowrap = re.compile(r"\[noautowrap\]")
+
+def remove_tag(string, pattern):
+    match = pattern.search(string)
+    if match:
+        start = match.start()
+        end = match.end()
+        return string[:start] + string[end:],string[start:end]
+    else:
+        return None
+
+def line_warp(line:str,width:int,font):
+    text_x = 0
+    line_count = 1
+    new_str = ""
+    for char in line:
+        text_x += font.getlength(char)
+        if text_x > width:
+            new_str += "\n" + char
+            text_x = 0
+            line_count += 1 
+        else:
+            new_str += char
+    return new_str,line_count
+
 def linecard(
     text:str,
     width:int = None,
     height:int = None,
     font_size:int = None,
     padding:tuple = (20,20),
     spacing:float = 1.2,
@@ -99,132 +132,165 @@
         [right]靠右
         [center]居中
         [pixel][400]指定像素
 
         [font_big]大字体
         [font_normal]正常字体
         [font_small]小字体
+        [font][font_name][font_size]指定字体
 
         [color][#000000]指定本行颜色
 
-        不换行[nowrap]
+        [nowrap]不换行
+        [noautowrap]不自动换行
+        [passport]保持标记
     '''
     text = text.replace("\r\n","\n")
     lines = text.split('\n')
 
     if font_size:
         font_default = ImageFont.truetype(font = fontname, size = font_size, encoding = "utf-8")
     else:
         font_default = font_normal
 
-    Text = []
+    paddingX = padding[0]
+    paddingY = padding[1]
+
     X = []
     Y = [0,]
-    textheight = 0
-    tmpH = 0
+    Text = []
+
+    line_length = []
+
+    text_y = 0
+    maxFontLine = 0 # 如果本行是通过[nowrap]不换行标记拼接的多个行，那么记录最大的字体宽度以在换行时使用最大的字体
+
+    align = "left"
+    font = font_default
+    color = None
+    passport = 0
+    autowrap = True
+
     for line in lines:
-        if line.startswith("[left]"):
-            line = line[6:]
-            align = "left"
-        elif line.startswith("[right]"):
-            line = line[7:]
-            align = "right"
-        elif line.startswith("[center]"):
-            line = line[8:]
-            align = "center"
-        elif line.startswith("[pixel]["):
-            line = line[8:]
-            align = ""
-            i = 0
-            for c in line:
-                i += 1
-                if c == "]":
-                    break
-                align += c
-            line = line[i:]
-        else:
-            align = "left"
-
-        if line.startswith("[font_big]"):
-            line = line[10:]
-            font = font_big
-        elif line.startswith("[font_normal]"):
-            line = line[13:]
-            font = font_normal
-        elif line.startswith("[font_small]"):
-            line = line[12:]
-            font = font_small
-        else:
-            font = font_default
-
-        if line.startswith("[color]["):
-            line = line[8:]
-            color = ""
-            i = 0
-            for c in line:
-                i += 1
-                if c == "]":
-                    break
-                color += c
-            line = line[i:]
-        else:
-            color = None
-
-        if line.endswith("[nowrap]"):
-            line = line[:-8]
-            tmpH = max(tmpH,int(font.size * spacing))
+        passport -= 1
+
+        if res := remove_tag(line,linecard_pattern.align):
+            line, align = res
+            if align.startswith("[pixel]["):
+                align = align[8:-1]
+            else:
+                align = align[1:-1]
         else:
-            textheight += max(tmpH,int(font.size * spacing))
-            tmpH = 0
+            if passport == 1:
+                pass
+            else:
+                align = "left"
 
-        Y.append(textheight)
-        X.append(int(font.getlength(line) if align == "left" else 0))
+        if res := remove_tag(line,linecard_pattern.font):
+            line, font = res
+            if font.startswith("[font]["):
+                font = font[7:-1]
+                inner_font_name,inner_font_size = font.split("][",1)
+                inner_font_size = int(inner_font_size)
+                inner_font_size = inner_font_size if inner_font_size else font_size
+                font = ImageFont.truetype(font = inner_font_name, size = inner_font_size, encoding = "utf-8")
+            elif font == "[font_big]":
+                font = font_big
+            elif font == "[font_small]":
+                font = font_small
+            else:
+                font = font_normal
+        else:
+            if passport == 1:
+                pass
+            else:
+                font = font_default
+
+        if res := remove_tag(line,linecard_pattern.color):
+            line, color = res
+            color = color[8:-1]
+        else:
+            if passport == 1:
+                pass
+            else:
+                color = None
+
+        if res := remove_tag(line,linecard_pattern.noautowrap):
+            line = res[0]
+            autowrap = False
+        else:
+            if passport == 1:
+                pass
+            else:
+                autowrap = True
+
+        if res := remove_tag(line,linecard_pattern.nowrap):
+            line = res[0]
+            maxFontLine = max(maxFontLine,int(font.size * spacing))
+        else:
+            if autowrap and width and font.getlength(line) > width:
+                line,inner_line_count = line_warp(line,width - paddingX,font)
+                text_y += max(maxFontLine,inner_line_count * int(font.size * spacing))
+            else:
+                text_y += max(maxFontLine,int(font.size * spacing))
+            maxFontLine = 0
+
+        if res := remove_tag(line,linecard_pattern.passport):
+            line = res[0]
+            passport = 2
+
+        line_length.append(int(font.getlength(line) if align == "left" else 0))
+        Y.append(text_y)
         Text.append([line, font, color, align])
 
-    lineX = []
     for i in range(len(lines)):
         if Y[i] == Y[i-1]:
-            lineX.append(X[i-1])
-            X[i] += X[i-1]
+            X.append(line_length[i-1])
+            line_length[i] += line_length[i-1]
         else:
-            lineX.append(0)
+            X.append(0)
 
-    paddingX = padding[0]
-    paddingY = padding[1]
-    width = width if width else (max(X) + paddingX*2)
+    width = width if width else (max(line_length) + paddingX*2)
     height = height if height else (Y[-1] + paddingY*2)
+
     canvas = canvas if canvas else Image.new("RGBA", (width, height), bg_color)
     draw = ImageDraw.Draw(canvas)
+
     for i in range(len(lines)):
-        y = Y[i] + paddingY
         line, font, color, align = Text[i]
+        text_y = Y[i] + paddingY
         if line == "----":
-            tmp = y + font.size//2
+            tmp = text_y + font.size//2
             color = color if color else 'gray'
             draw.line(((0, tmp), (width, tmp)), fill = color, width = 4)
         else:
             color = color if color else 'black'
             if align == "right":
-                x = int(width - font.getlength(line) - paddingX)
+                text_x = int(width - font.getlength(line) - paddingX)
             elif align == "center":
-                x = (width - font.getlength(line) )//2
+                text_x = (width - font.getlength(line) )//2
             elif align.isdigit():
-                x = int(align)
+                text_x = int(align)
             else:
-                x = lineX[i] + paddingX
-            draw.text((x, y),line, fill = color, font = font)
+                text_x = X[i] + paddingX
+            draw.text((text_x, text_y),line, fill = color, font = font)
 
     if endline:
         draw.line(((0, height - 60), (width, height - 60)), fill = "gray", width = 4)
-        x = int(width - font_small.getlength(endline) - 20)
-        draw.text((x,height - 45),endline, fill = "gray", font = font_small)
+        text_x = int(width - font_small.getlength(endline) - 20)
+        draw.text((text_x,height - 45),endline, fill = "gray", font = font_small)
 
     return canvas
 
-def gacha_info(report:IMG, info:List[IMG]):
+def linecard_to_png(msg):
+    output = BytesIO()
+    linecard(msg,width = 880,bg_color = "white",endline = "抽卡结果").save(output, format = "png")
+    return output
+
+def gacha_info0(report:IMG, info:List[IMG]):
     """
     抽卡信息拼接
         report:抽卡报告
         info:信息图片列表
     """
     x = 880
     y = report.size[1] + 10
@@ -235,15 +301,15 @@
 
     canvas = Image.new("RGB", (880,(130*length)//2 + report.size[1]), '#99CCFF')
     canvas.paste(report)
     for i in range(0, length, 2):
         l,r = info[i:i+2]
         canvas.paste(l, (0, y))
         if r:
-            canvas.paste(r, (440, y))
+            canvas.paste(r, (442, y))
         y += 130
     output = BytesIO()
     canvas.save(output,'png')
     return output
     
 async def bar_chart(user_id:int, info:str, lenth:float):
     """
```

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.2.8/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.7/setup.py` & `nonebot_plugin_game_collection-2.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.2.7',
+version='2.2.8',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

