# Comparing `tmp/hubotlibs-0.1.4.tar.gz` & `tmp/hubotlibs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubotlibs-0.1.4.tar", last modified: Fri Jun 23 17:35:23 2023, max compression
+gzip compressed data, was "hubotlibs-0.1.5.tar", last modified: Sat Jun 24 07:31:22 2023, max compression
```

## Comparing `hubotlibs-0.1.4.tar` & `hubotlibs-0.1.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.926317 hubotlibs-0.1.4/
--rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2623 2023-06-23 17:35:23.926317 hubotlibs-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.869433 hubotlibs-0.1.4/hubotlibs/
--rw-rw-rw-   0        0        0     1110 2023-06-23 17:33:54.000000 hubotlibs-0.1.4/hubotlibs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.898391 hubotlibs-0.1.4/hubotlibs/dar/
--rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.1.4/hubotlibs/dar/__init__.py
--rw-rw-rw-   0        0        0     1759 2023-06-23 13:39:16.000000 hubotlibs-0.1.4/hubotlibs/dar/load.py
--rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/log.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.922328 hubotlibs-0.1.4/hubotlibs/dar/utils/
--rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/PyroHelpers.py
--rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/__init__.py
--rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/adminHelpers.py
--rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/ai.py
--rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/aiohttp_helper.py
--rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/basic.py
--rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.925319 hubotlibs-0.1.4/hubotlibs/dar/utils/db/
--rw-rw-rw-   0        0        0    14691 2023-06-23 14:43:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/db/__init__.py
--rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/db/permit.py
--rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/function.py
--rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/get_id.py
--rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/http.py
--rw-rw-rw-   0        0        0     2055 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/inline.py
--rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/interval.py
--rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/misc.py
--rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/parser.py
--rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/pilter.py
--rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/tools.py
--rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/unpack.py
--rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/utility.py
--rw-rw-rw-   0        0        0       47 2023-06-23 17:34:02.000000 hubotlibs-0.1.4/hubotlibs/version.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.895399 hubotlibs-0.1.4/hubotlibs.egg-info/
--rw-rw-rw-   0        0        0     2623 2023-06-23 17:35:23.000000 hubotlibs-0.1.4/hubotlibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-06-23 17:35:23.000000 hubotlibs-0.1.4/hubotlibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 17:35:23.000000 hubotlibs-0.1.4/hubotlibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-23 17:35:23.000000 hubotlibs-0.1.4/hubotlibs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-23 17:35:23.000000 hubotlibs-0.1.4/hubotlibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 17:35:23.928312 hubotlibs-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:31:22.209150 hubotlibs-0.1.5/
+-rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2623 2023-06-24 07:31:22.209150 hubotlibs-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 07:31:22.056151 hubotlibs-0.1.5/hubotlibs/
+-rw-rw-rw-   0        0        0     1110 2023-06-23 17:33:54.000000 hubotlibs-0.1.5/hubotlibs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:31:22.096894 hubotlibs-0.1.5/hubotlibs/dar/
+-rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.1.5/hubotlibs/dar/__init__.py
+-rw-rw-rw-   0        0        0     1759 2023-06-23 13:39:16.000000 hubotlibs-0.1.5/hubotlibs/dar/load.py
+-rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/log.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:31:22.193319 hubotlibs-0.1.5/hubotlibs/dar/utils/
+-rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/PyroHelpers.py
+-rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/__init__.py
+-rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/adminHelpers.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/ai.py
+-rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/aiohttp_helper.py
+-rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/basic.py
+-rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:31:22.207185 hubotlibs-0.1.5/hubotlibs/dar/utils/db/
+-rw-rw-rw-   0        0        0    14691 2023-06-23 14:43:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/db/__init__.py
+-rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/db/permit.py
+-rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/function.py
+-rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/get_id.py
+-rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/http.py
+-rw-rw-rw-   0        0        0     2703 2023-06-24 07:29:34.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/inline.py
+-rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/interval.py
+-rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/misc.py
+-rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/parser.py
+-rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/pilter.py
+-rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/tools.py
+-rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/unpack.py
+-rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.1.5/hubotlibs/dar/utils/utility.py
+-rw-rw-rw-   0        0        0       47 2023-06-24 07:29:40.000000 hubotlibs-0.1.5/hubotlibs/version.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:31:22.080710 hubotlibs-0.1.5/hubotlibs.egg-info/
+-rw-rw-rw-   0        0        0     2623 2023-06-24 07:31:21.000000 hubotlibs-0.1.5/hubotlibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-06-24 07:31:21.000000 hubotlibs-0.1.5/hubotlibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 07:31:21.000000 hubotlibs-0.1.5/hubotlibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-24 07:31:21.000000 hubotlibs-0.1.5/hubotlibs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-24 07:31:21.000000 hubotlibs-0.1.5/hubotlibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 07:31:22.211145 hubotlibs-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.1.5/setup.py
```

### Comparing `hubotlibs-0.1.4/LICENSE` & `hubotlibs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/PKG-INFO` & `hubotlibs-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.1.4/README.md` & `hubotlibs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/__init__.py` & `hubotlibs-0.1.5/hubotlibs/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/__init__.py` & `hubotlibs-0.1.5/hubotlibs/dar/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/load.py` & `hubotlibs-0.1.5/hubotlibs/dar/load.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/log.py` & `hubotlibs-0.1.5/hubotlibs/dar/log.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/PyroHelpers.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/adminHelpers.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/ai.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/ai.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/aiohttp_helper.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/basic.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/basic.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/constants.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/constants.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/db/__init__.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/db/permit.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/function.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/function.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/get_id.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/http.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/http.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/inline.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/inline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,49 @@
 from math import ceil
 
 from pyrogram.types import InlineKeyboardButton
 
+from haidar import *
+
 
 class EqInlineKeyboardButton(InlineKeyboardButton):
     def __eq__(self, other):
         return self.text == other.text
 
     def __lt__(self, other):
         return self.text < other.text
 
     def __gt__(self, other):
         return self.text > other.text
 
 
-def paginate_modules(page_n, module_dict, prefix, chat=None):
+def paginate_modules(user_id, page_n, module_dict, prefix, chat=None):
+    
+    data = {}
+            
+    if user_id in BASICID:
+        filter_set = {'limit', 'broadcast', 'help'}
+        for key, value in module_dict.items():
+            if key in filter_set:
+                data[key] = value
+            
+        return data
+    
+    elif user_id in MEDIUMID:
+        filter_set = {'limit', 'broadcast', 'pilter', 'help', 'afk', 'antipm'}
+        for key, value in module_dict.items():
+            if key in filter_set:
+                data[key] = value
+            
+        return data
+        
+    elif user_id in PREMIUMID or user_id in DEVS:
+        
+        return module_dict
+
     if not chat:
         modules = sorted(
             [
                 EqInlineKeyboardButton(
                     x.__MODULE__,
                     callback_data="{}_module({})".format(
                         prefix, x.__MODULE__.replace(" ", "_").lower()
```

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/interval.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/interval.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/misc.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/parser.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/parser.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/pilter.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/tools.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/unpack.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs/dar/utils/utility.py` & `hubotlibs-0.1.5/hubotlibs/dar/utils/utility.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/hubotlibs.egg-info/PKG-INFO` & `hubotlibs-0.1.5/hubotlibs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.1.4/hubotlibs.egg-info/SOURCES.txt` & `hubotlibs-0.1.5/hubotlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.4/setup.py` & `hubotlibs-0.1.5/setup.py`

 * *Files identical despite different names*

