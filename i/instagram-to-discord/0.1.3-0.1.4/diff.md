# Comparing `tmp/instagram-to-discord-0.1.3.tar.gz` & `tmp/instagram-to-discord-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram-to-discord-0.1.3.tar", last modified: Sat Jun 24 03:50:42 2023, max compression
+gzip compressed data, was "instagram-to-discord-0.1.4.tar", last modified: Sat Jun 24 03:55:09 2023, max compression
```

## Comparing `instagram-to-discord-0.1.3.tar` & `instagram-to-discord-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:50:42.757589 instagram-to-discord-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-24 03:50:30.000000 instagram-to-discord-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-24 03:50:42.757589 instagram-to-discord-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-24 03:50:30.000000 instagram-to-discord-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 03:50:30.000000 instagram-to-discord-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-24 03:50:42.757589 instagram-to-discord-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:50:42.757589 instagram-to-discord-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:50:42.757589 instagram-to-discord-0.1.3/src/instagram_to_discord/
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-24 03:50:30.000000 instagram-to-discord-0.1.3/src/instagram_to_discord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:50:42.757589 instagram-to-discord-0.1.3/src/instagram_to_discord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-24 03:50:42.000000 instagram-to-discord-0.1.3/src/instagram_to_discord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-24 03:50:42.000000 instagram-to-discord-0.1.3/src/instagram_to_discord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 03:50:42.000000 instagram-to-discord-0.1.3/src/instagram_to_discord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 03:50:42.000000 instagram-to-discord-0.1.3/src/instagram_to_discord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:55:09.024798 instagram-to-discord-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-24 03:54:56.000000 instagram-to-discord-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-24 03:55:09.024798 instagram-to-discord-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-24 03:54:56.000000 instagram-to-discord-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 03:54:56.000000 instagram-to-discord-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-24 03:55:09.024798 instagram-to-discord-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:55:09.020798 instagram-to-discord-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:55:09.020798 instagram-to-discord-0.1.4/src/instagram_to_discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-24 03:54:56.000000 instagram-to-discord-0.1.4/src/instagram_to_discord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:55:09.024798 instagram-to-discord-0.1.4/src/instagram_to_discord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-24 03:55:09.000000 instagram-to-discord-0.1.4/src/instagram_to_discord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-24 03:55:09.000000 instagram-to-discord-0.1.4/src/instagram_to_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 03:55:09.000000 instagram-to-discord-0.1.4/src/instagram_to_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 03:55:09.000000 instagram-to-discord-0.1.4/src/instagram_to_discord.egg-info/top_level.txt
```

### Comparing `instagram-to-discord-0.1.3/LICENSE` & `instagram-to-discord-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `instagram-to-discord-0.1.3/PKG-INFO` & `instagram-to-discord-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-to-discord
-Version: 0.1.3
+Version: 0.1.4
 Summary: Integrate instagram to discord
 Home-page: https://github.com/jd-apprentice/instagram-to-discord
 Author: jd-apprentice
 Author-email: contacto@jonathan.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -44,14 +44,20 @@
 
 For that we have a script called `fetch_posts.sh` localed in `utils/` folder. You can use it like this:
 
 ```bash
 sh utils/fetch_posts.sh <username>
 ```
 
+Or if you use Windows:
+
+```ps1
+script.bat <username>
+```
+
 This will create a folder with the name of the user and inside it will be the photos and videos that the user has uploaded.
 
 ```py
 import os
 from instagram-to-discord import DiscordInstagramPoster
 
 current_folder = os.getcwd()
```

### Comparing `instagram-to-discord-0.1.3/README.md` & `instagram-to-discord-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 
 For that we have a script called `fetch_posts.sh` localed in `utils/` folder. You can use it like this:
 
 ```bash
 sh utils/fetch_posts.sh <username>
 ```
 
+Or if you use Windows:
+
+```ps1
+script.bat <username>
+```
+
 This will create a folder with the name of the user and inside it will be the photos and videos that the user has uploaded.
 
 ```py
 import os
 from instagram-to-discord import DiscordInstagramPoster
 
 current_folder = os.getcwd()
```

### Comparing `instagram-to-discord-0.1.3/setup.cfg` & `instagram-to-discord-0.1.4/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 description-file = README.md
 license_files = LICENSE
 name = instagram-to-discord
-version = 0.1.3
+version = 0.1.4
 author = jd-apprentice
 author_email = contacto@jonathan.com.ar
 description = Integrate instagram to discord
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jd-apprentice/instagram-to-discord
 classifiers =
```

### Comparing `instagram-to-discord-0.1.3/src/instagram_to_discord/__init__.py` & `instagram-to-discord-0.1.4/src/instagram_to_discord/__init__.py`

 * *Files identical despite different names*

### Comparing `instagram-to-discord-0.1.3/src/instagram_to_discord.egg-info/PKG-INFO` & `instagram-to-discord-0.1.4/src/instagram_to_discord.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-to-discord
-Version: 0.1.3
+Version: 0.1.4
 Summary: Integrate instagram to discord
 Home-page: https://github.com/jd-apprentice/instagram-to-discord
 Author: jd-apprentice
 Author-email: contacto@jonathan.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -44,14 +44,20 @@
 
 For that we have a script called `fetch_posts.sh` localed in `utils/` folder. You can use it like this:
 
 ```bash
 sh utils/fetch_posts.sh <username>
 ```
 
+Or if you use Windows:
+
+```ps1
+script.bat <username>
+```
+
 This will create a folder with the name of the user and inside it will be the photos and videos that the user has uploaded.
 
 ```py
 import os
 from instagram-to-discord import DiscordInstagramPoster
 
 current_folder = os.getcwd()
```

