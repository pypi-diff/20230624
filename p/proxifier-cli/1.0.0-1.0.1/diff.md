# Comparing `tmp/proxifier-cli-1.0.0.tar.gz` & `tmp/proxifier-cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxifier-cli-1.0.0.tar", last modified: Sat Jun 24 14:05:28 2023, max compression
+gzip compressed data, was "proxifier-cli-1.0.1.tar", last modified: Sat Jun 24 20:29:44 2023, max compression
```

## Comparing `proxifier-cli-1.0.0.tar` & `proxifier-cli-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 14:05:28.387954 proxifier-cli-1.0.0/
--rw-rw-rw-   0        0        0       35 2023-06-24 14:05:08.000000 proxifier-cli-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      507 2023-06-24 14:05:28.386961 proxifier-cli-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 14:05:28.374917 proxifier-cli-1.0.0/proxifier_cli/
--rw-rw-rw-   0        0        0        0 2023-06-24 13:28:18.000000 proxifier-cli-1.0.0/proxifier_cli/__init__.py
--rw-rw-rw-   0        0        0      465 2023-06-24 13:59:30.000000 proxifier-cli-1.0.0/proxifier_cli/process.py
--rw-rw-rw-   0        0        0     1385 2023-06-24 13:21:57.000000 proxifier-cli-1.0.0/proxifier_cli/profile.ppx
--rw-rw-rw-   0        0        0     1025 2023-06-24 14:00:19.000000 proxifier-cli-1.0.0/proxifier_cli/profiles.py
-drwxrwxrwx   0        0        0        0 2023-06-24 14:05:28.383941 proxifier-cli-1.0.0/proxifier_cli.egg-info/
--rw-rw-rw-   0        0        0      507 2023-06-24 14:05:28.000000 proxifier-cli-1.0.0/proxifier_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-06-24 14:05:28.000000 proxifier-cli-1.0.0/proxifier_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 14:05:28.000000 proxifier-cli-1.0.0/proxifier_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-24 14:05:28.000000 proxifier-cli-1.0.0/proxifier_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 14:05:28.388970 proxifier-cli-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      704 2023-06-24 14:01:41.000000 proxifier-cli-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:29:44.296098 proxifier-cli-1.0.1/
+-rw-rw-rw-   0        0        0      507 2023-06-24 20:29:44.294103 proxifier-cli-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 20:29:44.275044 proxifier-cli-1.0.1/proxifier_cli/
+-rw-rw-rw-   0        0        0       43 2023-06-24 20:28:41.000000 proxifier-cli-1.0.1/proxifier_cli/__init__.py
+-rw-rw-rw-   0        0        0      465 2023-06-24 13:59:30.000000 proxifier-cli-1.0.1/proxifier_cli/process.py
+-rw-rw-rw-   0        0        0     1385 2023-06-24 13:21:57.000000 proxifier-cli-1.0.1/proxifier_cli/profile.ppx
+-rw-rw-rw-   0        0        0     1075 2023-06-24 20:26:45.000000 proxifier-cli-1.0.1/proxifier_cli/profiles.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:29:44.292089 proxifier-cli-1.0.1/proxifier_cli.egg-info/
+-rw-rw-rw-   0        0        0      507 2023-06-24 20:29:44.000000 proxifier-cli-1.0.1/proxifier_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-24 20:29:44.000000 proxifier-cli-1.0.1/proxifier_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 20:29:44.000000 proxifier-cli-1.0.1/proxifier_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-24 20:29:44.000000 proxifier-cli-1.0.1/proxifier_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 20:29:44.299116 proxifier-cli-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-06-24 20:29:26.000000 proxifier-cli-1.0.1/setup.py
```

### Comparing `proxifier-cli-1.0.0/proxifier_cli/profile.ppx` & `proxifier-cli-1.0.1/proxifier_cli/profile.ppx`

 * *Files identical despite different names*

### Comparing `proxifier-cli-1.0.0/proxifier_cli/profiles.py` & `proxifier-cli-1.0.1/proxifier_cli/profiles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import time
 
 from proxifier_cli.process import close_proxifier
 from proxifier_cli.process import start_proxifier
 
+BASE_DIR = os.path.abspath(os.path.dirname(__file__))
+
 
 def create_profile(address, port, username, password, protocol="HTTPS"):
-    with open(os.path.join("proxifier_cli", "profile.ppx")) as fp:
+    with open(os.path.join(BASE_DIR, "profile.ppx")) as fp:
         profile = fp.read()
         return profile.format(
             protocol=protocol,
             password=password,
             username=username,
             port=port,
             address=address,
```

