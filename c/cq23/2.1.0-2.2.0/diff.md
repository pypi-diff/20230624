# Comparing `tmp/cq23-2.1.0.tar.gz` & `tmp/cq23-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-2.1.0.tar", last modified: Tue Jun 20 12:04:40 2023, max compression
+gzip compressed data, was "cq23-2.2.0.tar", last modified: Sat Jun 24 02:24:47 2023, max compression
```

## Comparing `cq23-2.1.0.tar` & `cq23-2.2.0.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.051012 cq23-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-20 12:04:40.051012 cq23-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-20 12:04:32.000000 cq23-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 12:04:32.000000 cq23-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-20 12:04:40.051012 cq23-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.039012 cq23-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.039012 cq23-2.1.0/src/cq23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.043012 cq23-2.1.0/src/cq23/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.043012 cq23-2.1.0/src/cq23/build_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/build_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/build_image/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/build_image/docker_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.043012 cq23-2.1.0/src/cq23/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/replay/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/web_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/web_server/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/web_server/files/loading_screen.html
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.051012 cq23-2.1.0/src/cq23/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/zip/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.043012 cq23-2.1.0/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.414855 cq23-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-24 02:24:47.414855 cq23-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-24 02:24:39.000000 cq23-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-24 02:24:39.000000 cq23-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-24 02:24:47.414855 cq23-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.406854 cq23-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/build_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/build_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/build_image/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/build_image/docker_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/client_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/client_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/client_logs/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/web_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23/web_server/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/web_server/files/loading_screen.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.414855 cq23-2.2.0/src/cq23/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-24 02:24:39.000000 cq23-2.2.0/src/cq23/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:24:47.410854 cq23-2.2.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 02:24:47.000000 cq23-2.2.0/src/cq23.egg-info/top_level.txt
```

### Comparing `cq23-2.1.0/PKG-INFO` & `cq23-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.1.0
+Version: 2.2.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.1.0/setup.cfg` & `cq23-2.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 2.1.0
+version = 2.2.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-2.1.0/src/cq23/admin/aws.py` & `cq23-2.2.0/src/cq23/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/admin/builder.py` & `cq23-2.2.0/src/cq23/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/admin/worker.py` & `cq23-2.2.0/src/cq23/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/build_image/command.py` & `cq23-2.2.0/src/cq23/build_image/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/build_image/docker_tools.py` & `cq23-2.2.0/src/cq23/build_image/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/check/command.py` & `cq23-2.2.0/src/cq23/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/cleanup/command.py` & `cq23-2.2.0/src/cq23/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/main/command.py` & `cq23-2.2.0/src/cq23/main/command.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 
 from cq23.admin.builder import command as builder
 from cq23.admin.worker import command as worker
 from cq23.build_image.command import build
 from cq23.check.command import check
+from cq23.client_logs.command import logs
 from cq23.cleanup.command import cleanup
 from cq23.new_client.command import new_client
 from cq23.replay.command import replay
 from cq23.run_game.command import run_game
 from cq23.zip.command import zip
 
 from .utils import restore_cwd
@@ -19,14 +20,15 @@
         + "> cq23 new python my_bot\n"
         + "> cq23 build <name>\n"
         + "> cq23 run\n"
         + "> cq23 run map=<map name>\n"
         + "> cq23 replay\n"
         + "> cq23 zip\n"
         + "> cq23 check\n"
+        + "> cq23 logs <client name>\n"
         + "> cq23 cleanup\n\n"
         + "If you need help with the competition, post a message in Discord or email us at info@codequest.club."
     )
     print(message)
 
 
 @restore_cwd
@@ -37,14 +39,15 @@
         "new": new_client,
         "build": build,
         "run": run_game,
         "replay": replay,
         "cleanup": cleanup,
         "zip": zip,
         "check": check,
+        "logs": logs,
         "worker": worker,
         "builder": builder,
     }
 
     if not command_args or command_args[0].lower() not in first_arg_mapping.keys():
         help_message()
     else:
```

### Comparing `cq23-2.1.0/src/cq23/main/utils.py` & `cq23-2.2.0/src/cq23/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/new_client/command.py` & `cq23-2.2.0/src/cq23/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/replay/command.py` & `cq23-2.2.0/src/cq23/replay/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/run_game/command.py` & `cq23-2.2.0/src/cq23/run_game/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/run_game/docker_tools.py` & `cq23-2.2.0/src/cq23/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/run_game/gcs.py` & `cq23-2.2.0/src/cq23/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/web_server/files/loading_screen.html` & `cq23-2.2.0/src/cq23/web_server/files/loading_screen.html`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/web_server/flask_api.py` & `cq23-2.2.0/src/cq23/web_server/flask_api.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23/zip/command.py` & `cq23-2.2.0/src/cq23/zip/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.1.0/src/cq23.egg-info/PKG-INFO` & `cq23-2.2.0/src/cq23.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.1.0
+Version: 2.2.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.1.0/src/cq23.egg-info/SOURCES.txt` & `cq23-2.2.0/src/cq23.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 src/cq23/build_image/__init__.py
 src/cq23/build_image/command.py
 src/cq23/build_image/docker_tools.py
 src/cq23/check/__init__.py
 src/cq23/check/command.py
 src/cq23/cleanup/__init__.py
 src/cq23/cleanup/command.py
+src/cq23/client_logs/__init__.py
+src/cq23/client_logs/command.py
 src/cq23/main/__init__.py
 src/cq23/main/command.py
 src/cq23/main/utils.py
 src/cq23/new_client/__init__.py
 src/cq23/new_client/command.py
 src/cq23/replay/__init__.py
 src/cq23/replay/command.py
```

