# Comparing `tmp/instagram-to-discord-0.1.1.tar.gz` & `tmp/instagram-to-discord-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram-to-discord-0.1.1.tar", last modified: Sat Jun 24 01:36:09 2023, max compression
+gzip compressed data, was "instagram-to-discord-0.1.2.tar", last modified: Sat Jun 24 03:46:16 2023, max compression
```

## Comparing `instagram-to-discord-0.1.1.tar` & `instagram-to-discord-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-24 01:35:57.000000 instagram-to-discord-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-24 01:35:57.000000 instagram-to-discord-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 01:35:57.000000 instagram-to-discord-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/src/instagram_to_discord/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-24 01:35:57.000000 instagram-to-discord-0.1.1/src/instagram_to_discord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:36:09.377630 instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-24 01:36:09.000000 instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-24 01:36:09.000000 instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 01:36:09.000000 instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 01:36:09.000000 instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:46:16.814049 instagram-to-discord-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-24 03:46:07.000000 instagram-to-discord-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-24 03:46:16.814049 instagram-to-discord-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-24 03:46:07.000000 instagram-to-discord-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 03:46:07.000000 instagram-to-discord-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-24 03:46:16.814049 instagram-to-discord-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:46:16.810049 instagram-to-discord-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:46:16.810049 instagram-to-discord-0.1.2/src/instagram_to_discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-24 03:46:07.000000 instagram-to-discord-0.1.2/src/instagram_to_discord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:46:16.810049 instagram-to-discord-0.1.2/src/instagram_to_discord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-24 03:46:16.000000 instagram-to-discord-0.1.2/src/instagram_to_discord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-24 03:46:16.000000 instagram-to-discord-0.1.2/src/instagram_to_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 03:46:16.000000 instagram-to-discord-0.1.2/src/instagram_to_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 03:46:16.000000 instagram-to-discord-0.1.2/src/instagram_to_discord.egg-info/top_level.txt
```

### Comparing `instagram-to-discord-0.1.1/LICENSE` & `instagram-to-discord-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `instagram-to-discord-0.1.1/PKG-INFO` & `instagram-to-discord-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-to-discord
-Version: 0.1.1
+Version: 0.1.2
 Summary: Integrate instagram to discord
 Home-page: https://github.com/jd-apprentice/instagram-to-discord
 Author: jd-apprentice
 Author-email: contacto@jonathan.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -65,9 +65,9 @@
 
 discord_instagram_poster = DiscordInstagramPoster({
     "webhook_url": webhook_url,
     "footer_text": footer_text,
     "footer_icon": footer_url,
     "title": title
 })
-discord_instagram_poster.get_latest_photo(folder_path)
+discord_instagram_poster.get_latest_json(folder_path)
 ```
```

### Comparing `instagram-to-discord-0.1.1/README.md` & `instagram-to-discord-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,9 +51,9 @@
 
 discord_instagram_poster = DiscordInstagramPoster({
     "webhook_url": webhook_url,
     "footer_text": footer_text,
     "footer_icon": footer_url,
     "title": title
 })
-discord_instagram_poster.get_latest_photo(folder_path)
+discord_instagram_poster.get_latest_json(folder_path)
 ```
```

### Comparing `instagram-to-discord-0.1.1/setup.cfg` & `instagram-to-discord-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 description-file = README.md
 license_files = LICENSE
 name = instagram-to-discord
-version = 0.1.1
+version = 0.1.2
 author = jd-apprentice
 author_email = contacto@jonathan.com.ar
 description = Integrate instagram to discord
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jd-apprentice/instagram-to-discord
 classifiers =
```

### Comparing `instagram-to-discord-0.1.1/src/instagram_to_discord/__init__.py` & `instagram-to-discord-0.1.2/src/instagram_to_discord/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,27 +66,26 @@
             return
 
         if response.status_code == 204:
             print("Message sent successfully.")
         else:
             print("Message could not be sent.")
 
-    def get_latest_photo(self, directory: str) -> None:
+    def get_latest_json(self, directory: str) -> None:
         """
-        directory -- The directory where the photos are stored.
+        directory -- The directory where the files are stored.
         
-        Get the latest photo from a directory and send it to Discord.
+        Get the latest JSON file with .json.xz extension from a directory.
         """
 
         files = os.listdir(directory)
-        photo_files = [file for file in files if file.endswith(".jpg")]
-        latest_photo = max(photo_files)
+        json_files = [file for file in files if file.endswith(".json.xz")]
+        latest_json = max(json_files)
 
-        json_file = latest_photo.replace(".jpg", ".json.xz")
-        json_path = os.path.join(directory, json_file)
+        json_path = os.path.join(directory, latest_json)
 
         with lzma.open(json_path, "rt") as file:
             json_content = file.read()
 
         json_data = json.loads(json_content)
 
         # Author information
```

### Comparing `instagram-to-discord-0.1.1/src/instagram_to_discord.egg-info/PKG-INFO` & `instagram-to-discord-0.1.2/src/instagram_to_discord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-to-discord
-Version: 0.1.1
+Version: 0.1.2
 Summary: Integrate instagram to discord
 Home-page: https://github.com/jd-apprentice/instagram-to-discord
 Author: jd-apprentice
 Author-email: contacto@jonathan.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -65,9 +65,9 @@
 
 discord_instagram_poster = DiscordInstagramPoster({
     "webhook_url": webhook_url,
     "footer_text": footer_text,
     "footer_icon": footer_url,
     "title": title
 })
-discord_instagram_poster.get_latest_photo(folder_path)
+discord_instagram_poster.get_latest_json(folder_path)
 ```
```

