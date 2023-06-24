# Comparing `tmp/nonebot_plugin_code-0.0.5.tar.gz` & `tmp/nonebot_plugin_code-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_code-0.0.5.tar", last modified: Thu Jan 19 17:32:31 2023, max compression
+gzip compressed data, was "nonebot_plugin_code-0.0.6.tar", last modified: Sat Jun 24 09:06:06 2023, max compression
```

## Comparing `nonebot_plugin_code-0.0.5.tar` & `nonebot_plugin_code-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:32:31.901990 nonebot_plugin_code-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-19 17:32:21.000000 nonebot_plugin_code-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-01-19 17:32:31.901990 nonebot_plugin_code-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-01-19 17:32:21.000000 nonebot_plugin_code-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:32:31.901990 nonebot_plugin_code-0.0.5/nonebot_plugin_code/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-01-19 17:32:21.000000 nonebot_plugin_code-0.0.5/nonebot_plugin_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-01-19 17:32:21.000000 nonebot_plugin_code-0.0.5/nonebot_plugin_code/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 17:32:31.901990 nonebot_plugin_code-0.0.5/nonebot_plugin_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-01-19 17:32:31.000000 nonebot_plugin_code-0.0.5/nonebot_plugin_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-19 17:32:31.000000 nonebot_plugin_code-0.0.5/nonebot_plugin_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 17:32:31.000000 nonebot_plugin_code-0.0.5/nonebot_plugin_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-19 17:32:31.000000 nonebot_plugin_code-0.0.5/nonebot_plugin_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-19 17:32:31.000000 nonebot_plugin_code-0.0.5/nonebot_plugin_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 17:32:31.901990 nonebot_plugin_code-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-01-19 17:32:21.000000 nonebot_plugin_code-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:06:06.860721 nonebot_plugin_code-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-24 09:05:55.000000 nonebot_plugin_code-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-24 09:06:06.860721 nonebot_plugin_code-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-24 09:05:55.000000 nonebot_plugin_code-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:06:06.860721 nonebot_plugin_code-0.0.6/nonebot_plugin_code/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-24 09:05:55.000000 nonebot_plugin_code-0.0.6/nonebot_plugin_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-24 09:05:55.000000 nonebot_plugin_code-0.0.6/nonebot_plugin_code/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:06:06.860721 nonebot_plugin_code-0.0.6/nonebot_plugin_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-24 09:06:06.000000 nonebot_plugin_code-0.0.6/nonebot_plugin_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-24 09:06:06.000000 nonebot_plugin_code-0.0.6/nonebot_plugin_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 09:06:06.000000 nonebot_plugin_code-0.0.6/nonebot_plugin_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-24 09:06:06.000000 nonebot_plugin_code-0.0.6/nonebot_plugin_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-24 09:06:06.000000 nonebot_plugin_code-0.0.6/nonebot_plugin_code.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 09:06:06.860721 nonebot_plugin_code-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-24 09:05:55.000000 nonebot_plugin_code-0.0.6/setup.py
```

### Comparing `nonebot_plugin_code-0.0.5/LICENSE` & `nonebot_plugin_code-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_code-0.0.5/PKG-INFO` & `nonebot_plugin_code-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_code
-Version: 0.0.5
+Version: 0.0.6
 Summary: nonebot2 plugin run code online
 Home-page: https://github.com/yzyyz1387/nonebot_plugin_code
 Author: yzyyz1387
 Author-email: youzyyz1384@qq.com
 Keywords: pip,nonebot2,nonebot,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_code Version: 0.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_code Version: 0.0.6 Summary:
 nonebot2 plugin run code online Home-page: https://github.com/yzyyz1387/
 nonebot_plugin_code Author: yzyyz1387 Author-email: youzyyz1384@qq.com
 Keywords: pip,nonebot2,nonebot,nonebot_plugin Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE
                                    [nonebot]
```

### Comparing `nonebot_plugin_code-0.0.5/README.md` & `nonebot_plugin_code-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_code-0.0.5/nonebot_plugin_code/__init__.py` & `nonebot_plugin_code-0.0.6/nonebot_plugin_code/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_code-0.0.5/nonebot_plugin_code.egg-info/PKG-INFO` & `nonebot_plugin_code-0.0.6/nonebot_plugin_code.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-code
-Version: 0.0.5
+Version: 0.0.6
 Summary: nonebot2 plugin run code online
 Home-page: https://github.com/yzyyz1387/nonebot_plugin_code
 Author: yzyyz1387
 Author-email: youzyyz1384@qq.com
 Keywords: pip,nonebot2,nonebot,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-code Version: 0.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-code Version: 0.0.6 Summary:
 nonebot2 plugin run code online Home-page: https://github.com/yzyyz1387/
 nonebot_plugin_code Author: yzyyz1387 Author-email: youzyyz1384@qq.com
 Keywords: pip,nonebot2,nonebot,nonebot_plugin Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE
                                    [nonebot]
```

### Comparing `nonebot_plugin_code-0.0.5/setup.py` & `nonebot_plugin_code-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_code",
-    version="0.0.5",
+    version="0.0.6",
     author="yzyyz1387",
     author_email="youzyyz1384@qq.com",
     keywords=("pip", "nonebot2", "nonebot", "nonebot_plugin"),
     description="""nonebot2 plugin run code online""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yzyyz1387/nonebot_plugin_code",
```

