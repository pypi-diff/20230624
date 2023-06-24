# Comparing `tmp/user-discord-1.0.0.tar.gz` & `tmp/user_discord-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user-discord-1.0.0.tar", last modified: Sat Jun 24 17:12:53 2023, max compression
+gzip compressed data, was "user_discord-1.0.1.tar", last modified: Sat Jun 24 17:22:50 2023, max compression
```

## Comparing `user-discord-1.0.0.tar` & `user_discord-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 17:12:53.244121 user-discord-1.0.0/
--rw-rw-rw-   0        0        0      443 2023-06-24 17:12:53.243120 user-discord-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3545 2023-06-24 16:52:42.000000 user-discord-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 17:12:53.245118 user-discord-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-24 17:12:45.000000 user-discord-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:12:53.220924 user-discord-1.0.0/user_discord/
--rw-rw-rw-   0        0        0     5612 2023-06-24 16:38:07.000000 user-discord-1.0.0/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-24 17:12:53.241122 user-discord-1.0.0/user_discord.egg-info/
--rw-rw-rw-   0        0        0      443 2023-06-24 17:12:52.000000 user-discord-1.0.0/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-06-24 17:12:53.000000 user-discord-1.0.0/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 17:12:52.000000 user-discord-1.0.0/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-24 17:12:52.000000 user-discord-1.0.0/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 17:12:52.000000 user-discord-1.0.0/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 17:22:50.014940 user_discord-1.0.1/
+-rw-rw-rw-   0        0        0      443 2023-06-24 17:22:50.013935 user_discord-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3545 2023-06-24 16:52:42.000000 user_discord-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 17:22:50.015938 user_discord-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-24 17:22:23.000000 user_discord-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:22:49.972462 user_discord-1.0.1/user_discord/
+-rw-rw-rw-   0        0        0     5612 2023-06-24 16:38:07.000000 user_discord-1.0.1/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:22:49.992448 user_discord-1.0.1/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-06-24 17:22:49.000000 user_discord-1.0.1/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-06-24 17:22:49.000000 user_discord-1.0.1/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 17:22:49.000000 user_discord-1.0.1/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-24 17:22:49.000000 user_discord-1.0.1/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 17:22:49.000000 user_discord-1.0.1/user_discord.egg-info/top_level.txt
```

### Comparing `user-discord-1.0.0/README.md` & `user_discord-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `user-discord-1.0.0/setup.py` & `user_discord-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 ` https://discord.gg/WR9MNs5Hqv`
 ### How to install?
 `pip install user-discord`
 ### No work
 Join-server, login, access discord database :D"""
 
 setup(
-    name="user-discord",
+    name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="1.0.0",
+    version="1.0.1",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

### Comparing `user-discord-1.0.0/user_discord/user_discord.py` & `user_discord-1.0.1/user_discord/user_discord.py`

 * *Files identical despite different names*

