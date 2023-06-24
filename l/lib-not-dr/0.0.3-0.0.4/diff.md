# Comparing `tmp/lib-not-dr-0.0.3.tar.gz` & `tmp/lib-not-dr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-not-dr-0.0.3.tar", last modified: Sat Jun 24 13:08:57 2023, max compression
+gzip compressed data, was "lib-not-dr-0.0.4.tar", last modified: Sat Jun 24 18:21:21 2023, max compression
```

## Comparing `lib-not-dr-0.0.3.tar` & `lib-not-dr-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 13:08:57.803095 lib-not-dr-0.0.3/
--rw-rw-rw-   0        0        0    17098 2023-06-09 16:24:01.000000 lib-not-dr-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    21199 2023-06-24 13:08:57.802096 lib-not-dr-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      749 2023-06-24 13:07:13.000000 lib-not-dr-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 13:08:57.781096 lib-not-dr-0.0.3/lib_not_dr/
--rw-rw-rw-   0        0        0      205 2023-06-24 13:07:05.000000 lib-not-dr-0.0.3/lib_not_dr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:08:57.791096 lib-not-dr-0.0.3/lib_not_dr/nuitka/
--rw-rw-rw-   0        0        0     6464 2023-06-24 12:56:32.000000 lib-not-dr-0.0.3/lib_not_dr/nuitka/compile.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:08:57.799096 lib-not-dr-0.0.3/lib_not_dr/types/
--rw-rw-rw-   0        0        0      785 2023-06-17 04:51:13.000000 lib-not-dr-0.0.3/lib_not_dr/types/__init__.py
--rw-rw-rw-   0        0        0     8943 2023-06-24 13:04:34.000000 lib-not-dr-0.0.3/lib_not_dr/types/options.py
--rw-rw-rw-   0        0        0     8114 2023-06-17 04:49:52.000000 lib-not-dr-0.0.3/lib_not_dr/types/version.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:08:57.789096 lib-not-dr-0.0.3/lib_not_dr.egg-info/
--rw-rw-rw-   0        0        0    21199 2023-06-24 13:08:57.000000 lib-not-dr-0.0.3/lib_not_dr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-06-24 13:08:57.000000 lib-not-dr-0.0.3/lib_not_dr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 13:08:57.000000 lib-not-dr-0.0.3/lib_not_dr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 13:08:57.000000 lib-not-dr-0.0.3/lib_not_dr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      393 2023-06-24 13:07:10.000000 lib-not-dr-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 13:08:57.803095 lib-not-dr-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 18:21:21.417413 lib-not-dr-0.0.4/
+-rw-rw-rw-   0        0        0    17098 2023-06-09 16:24:01.000000 lib-not-dr-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    21441 2023-06-24 18:21:21.416403 lib-not-dr-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      749 2023-06-24 13:59:54.000000 lib-not-dr-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 18:21:21.395788 lib-not-dr-0.0.4/lib_not_dr/
+-rw-rw-rw-   0        0        0      205 2023-06-24 13:59:51.000000 lib-not-dr-0.0.4/lib_not_dr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:21:21.406786 lib-not-dr-0.0.4/lib_not_dr/nuitka/
+-rw-rw-rw-   0        0        0     6464 2023-06-24 12:56:32.000000 lib-not-dr-0.0.4/lib_not_dr/nuitka/compile.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:21:21.413791 lib-not-dr-0.0.4/lib_not_dr/types/
+-rw-rw-rw-   0        0        0      785 2023-06-17 04:51:13.000000 lib-not-dr-0.0.4/lib_not_dr/types/__init__.py
+-rw-rw-rw-   0        0        0     8943 2023-06-24 13:04:34.000000 lib-not-dr-0.0.4/lib_not_dr/types/options.py
+-rw-rw-rw-   0        0        0     8114 2023-06-17 04:49:52.000000 lib-not-dr-0.0.4/lib_not_dr/types/version.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:21:21.404786 lib-not-dr-0.0.4/lib_not_dr.egg-info/
+-rw-rw-rw-   0        0        0    21441 2023-06-24 18:21:21.000000 lib-not-dr-0.0.4/lib_not_dr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-06-24 18:21:21.000000 lib-not-dr-0.0.4/lib_not_dr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:21:21.000000 lib-not-dr-0.0.4/lib_not_dr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 18:21:21.000000 lib-not-dr-0.0.4/lib_not_dr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-06-24 13:58:50.000000 lib-not-dr-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 18:21:21.417413 lib-not-dr-0.0.4/setup.cfg
```

### Comparing `lib-not-dr-0.0.3/LICENSE` & `lib-not-dr-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.3/PKG-INFO` & `lib-not-dr-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-not-dr
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python lib created from Difficult Rocket development
 Author-email: shenjackyuanjie <3695888@qq.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -373,29 +373,32 @@
         
         Exhibit B - "Incompatible With Secondary Licenses" Notice
         ---------------------------------------------------------
         
           This Source Code Form is "Incompatible With Secondary Licenses", as
           defined by the Mozilla Public License, v. 2.0.
         
+Project-URL: Homepage, https://github.com/shenjackyuanjie/lib-not-dr
+Project-URL: Repository, https://github.com/shenjackyuanjie/lib-not-dr
+Project-URL: Changelog, https://github.com/shenjackyuanjie/lib-not-dr/blob/main/docs/change_log.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lib-not-dr
 
 A python lib came from [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) development
 
 一个在 [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) 开发中 分离出来的 python 库
 
 ## Information/信息
 
-- Version/版本: 0.0.3
+- Version/版本: 0.0.4
 
 ### Author/作者
 
 [shenjackyuanjie](https://github/shenjackyuanjie)
 
 ### License/许可证
```

### Comparing `lib-not-dr-0.0.3/README.md` & `lib-not-dr-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 A python lib came from [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) development
 
 一个在 [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) 开发中 分离出来的 python 库
 
 ## Information/信息
 
-- Version/版本: 0.0.3
+- Version/版本: 0.0.4
 
 ### Author/作者
 
 [shenjackyuanjie](https://github/shenjackyuanjie)
 
 ### License/许可证
```

### Comparing `lib-not-dr-0.0.3/lib_not_dr/nuitka/compile.py` & `lib-not-dr-0.0.4/lib_not_dr/nuitka/compile.py`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.3/lib_not_dr/types/__init__.py` & `lib-not-dr-0.0.4/lib_not_dr/types/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.3/lib_not_dr/types/options.py` & `lib-not-dr-0.0.4/lib_not_dr/types/options.py`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.3/lib_not_dr/types/version.py` & `lib-not-dr-0.0.4/lib_not_dr/types/version.py`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.3/lib_not_dr.egg-info/PKG-INFO` & `lib-not-dr-0.0.4/lib_not_dr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-not-dr
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python lib created from Difficult Rocket development
 Author-email: shenjackyuanjie <3695888@qq.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -373,29 +373,32 @@
         
         Exhibit B - "Incompatible With Secondary Licenses" Notice
         ---------------------------------------------------------
         
           This Source Code Form is "Incompatible With Secondary Licenses", as
           defined by the Mozilla Public License, v. 2.0.
         
+Project-URL: Homepage, https://github.com/shenjackyuanjie/lib-not-dr
+Project-URL: Repository, https://github.com/shenjackyuanjie/lib-not-dr
+Project-URL: Changelog, https://github.com/shenjackyuanjie/lib-not-dr/blob/main/docs/change_log.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lib-not-dr
 
 A python lib came from [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) development
 
 一个在 [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) 开发中 分离出来的 python 库
 
 ## Information/信息
 
-- Version/版本: 0.0.3
+- Version/版本: 0.0.4
 
 ### Author/作者
 
 [shenjackyuanjie](https://github/shenjackyuanjie)
 
 ### License/许可证
```

