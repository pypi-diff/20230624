# Comparing `tmp/instagram-to-discord-0.1.tar.gz` & `tmp/instagram-to-discord-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram-to-discord-0.1.tar", last modified: Sat Jun 24 00:47:39 2023, max compression
+gzip compressed data, was "instagram-to-discord-0.1.1.tar", last modified: Sat Jun 24 01:36:09 2023, max compression
```

## Comparing `instagram-to-discord-0.1.tar` & `instagram-to-discord-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-24 00:47:39.664791 instagram-to-discord-0.1/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    35148 2023-06-23 23:00:57.000000 instagram-to-discord-0.1/LICENSE
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2070 2023-06-24 00:47:39.664791 instagram-to-discord-0.1/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1506 2023-06-24 00:34:34.000000 instagram-to-discord-0.1/README.md
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      103 2023-06-24 00:42:50.000000 instagram-to-discord-0.1/pyproject.toml
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      661 2023-06-24 00:47:39.664791 instagram-to-discord-0.1/setup.cfg
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      539 2023-06-24 00:04:07.000000 instagram-to-discord-0.1/setup.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-24 00:47:39.664791 instagram-to-discord-0.1/src/
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-24 00:47:39.664791 instagram-to-discord-0.1/src/instagram_to_discord/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3258 2023-06-24 00:46:24.000000 instagram-to-discord-0.1/src/instagram_to_discord/__init__.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-24 00:47:39.664791 instagram-to-discord-0.1/src/instagram_to_discord.egg-info/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2070 2023-06-24 00:47:39.000000 instagram-to-discord-0.1/src/instagram_to_discord.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      327 2023-06-24 00:47:39.000000 instagram-to-discord-0.1/src/instagram_to_discord.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2023-06-24 00:47:39.000000 instagram-to-discord-0.1/src/instagram_to_discord.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       42 2023-06-24 00:47:39.000000 instagram-to-discord-0.1/src/instagram_to_discord.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       21 2023-06-24 00:47:39.000000 instagram-to-discord-0.1/src/instagram_to_discord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-24 01:35:57.000000 instagram-to-discord-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-24 01:35:57.000000 instagram-to-discord-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 01:35:57.000000 instagram-to-discord-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/src/instagram_to_discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-24 01:35:57.000000 instagram-to-discord-0.1.1/src/instagram_to_discord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-24 01:36:09.000000 instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-24 01:36:09.000000 instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 01:36:09.000000 instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 01:36:09.000000 instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/top_level.txt
```

### Comparing `instagram-to-discord-0.1/LICENSE` & `instagram-to-discord-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `instagram-to-discord-0.1/PKG-INFO` & `instagram-to-discord-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: instagram-to-discord
-Version: 0.1
+Version: 0.1.1
 Summary: Integrate instagram to discord
 Home-page: https://github.com/jd-apprentice/instagram-to-discord
-Author: Jonathan Dyallo
+Author: jd-apprentice
 Author-email: contacto@jonathan.com.ar
-License: GNU GPLv3
-Keywords: integration,instagram,discord,python,webhooks
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,14 +16,18 @@
 
 ![IMAGE](https://i.ytimg.com/vi/bawUOnhbdLw/maxresdefault.jpg)
 
 ## Description 📝
 
 This is a simple abstraction layer for the Instagram API, which allows you to get the latest posts from a user and send them to a Discord channel.
 
+## How it works? ⁉
+
+![image](https://github.com/jd-apprentice/instagram-to-discord/assets/68082746/368fe303-f714-4572-86c5-064f08daeb19)
+
 ## Installation 📦
 
 ```bash
 pip install instagram-to-discord
 ```
 
 Or you can install it from the source code:
```

### Comparing `instagram-to-discord-0.1/README.md` & `instagram-to-discord-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 ![IMAGE](https://i.ytimg.com/vi/bawUOnhbdLw/maxresdefault.jpg)
 
 ## Description 📝
 
 This is a simple abstraction layer for the Instagram API, which allows you to get the latest posts from a user and send them to a Discord channel.
 
+## How it works? ⁉
+
+![image](https://github.com/jd-apprentice/instagram-to-discord/assets/68082746/368fe303-f714-4572-86c5-064f08daeb19)
+
 ## Installation 📦
 
 ```bash
 pip install instagram-to-discord
 ```
 
 Or you can install it from the source code:
@@ -48,8 +52,8 @@
 discord_instagram_poster = DiscordInstagramPoster({
     "webhook_url": webhook_url,
     "footer_text": footer_text,
     "footer_icon": footer_url,
     "title": title
 })
 discord_instagram_poster.get_latest_photo(folder_path)
-```
+```
```

### Comparing `instagram-to-discord-0.1/setup.cfg` & `instagram-to-discord-0.1.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 description-file = README.md
 license_files = LICENSE
 name = instagram-to-discord
-version = 0.1.0
+version = 0.1.1
 author = jd-apprentice
 author_email = contacto@jonathan.com.ar
 description = Integrate instagram to discord
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jd-apprentice/instagram-to-discord
 classifiers =
```

### Comparing `instagram-to-discord-0.1/src/instagram_to_discord/__init__.py` & `instagram-to-discord-0.1.1/src/instagram_to_discord/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,19 @@
                         "url": photo_url
                     }
                 }
             ],
             "attachments": []
         }
 
-        response = requests.post(self._webhook_url, json=data)
+        try:
+            response = requests.post(self._webhook_url, json=data)
+        except requests.exceptions.MissingSchema:
+            print("Invalid webhook URL.")
+            return
 
         if response.status_code == 204:
             print("Message sent successfully.")
         else:
             print("Message could not be sent.")
 
     def get_latest_photo(self, directory: str) -> None:
```

### Comparing `instagram-to-discord-0.1/src/instagram_to_discord.egg-info/PKG-INFO` & `instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: instagram-to-discord
-Version: 0.1
+Version: 0.1.1
 Summary: Integrate instagram to discord
 Home-page: https://github.com/jd-apprentice/instagram-to-discord
-Author: Jonathan Dyallo
+Author: jd-apprentice
 Author-email: contacto@jonathan.com.ar
-License: GNU GPLv3
-Keywords: integration,instagram,discord,python,webhooks
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,14 +16,18 @@
 
 ![IMAGE](https://i.ytimg.com/vi/bawUOnhbdLw/maxresdefault.jpg)
 
 ## Description 📝
 
 This is a simple abstraction layer for the Instagram API, which allows you to get the latest posts from a user and send them to a Discord channel.
 
+## How it works? ⁉
+
+![image](https://github.com/jd-apprentice/instagram-to-discord/assets/68082746/368fe303-f714-4572-86c5-064f08daeb19)
+
 ## Installation 📦
 
 ```bash
 pip install instagram-to-discord
 ```
 
 Or you can install it from the source code:
```

