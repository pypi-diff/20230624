# Comparing `tmp/dj3base-0.1.0.tar.gz` & `tmp/dj3base-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj3base-0.1.0.tar", last modified: Sun Jun 11 14:53:41 2023, max compression
+gzip compressed data, was "dj3base-0.1.1.tar", last modified: Sat Jun 24 06:35:30 2023, max compression
```

## Comparing `dj3base-0.1.0.tar` & `dj3base-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxrwxr-x   0 qiang     (1000) qiang     (1000)        0 2023-06-11 14:53:41.669265 dj3base-0.1.0/
--rw-rw-r--   0 qiang     (1000) qiang     (1000)    11357 2023-03-27 09:15:19.000000 dj3base-0.1.0/LICENSE
--rw-rw-r--   0 qiang     (1000) qiang     (1000)       65 2023-06-11 14:45:58.000000 dj3base-0.1.0/MANIFEST.in
--rw-rw-r--   0 qiang     (1000) qiang     (1000)     1165 2023-06-11 14:53:41.669265 dj3base-0.1.0/PKG-INFO
--rw-rw-r--   0 qiang     (1000) qiang     (1000)      103 2023-06-11 14:47:02.000000 dj3base-0.1.0/README.md
-drwxrwxr-x   0 qiang     (1000) qiang     (1000)        0 2023-06-11 14:53:41.669265 dj3base-0.1.0/dj3base/
--rw-rw-r--   0 qiang     (1000) qiang     (1000)       46 2023-06-11 14:45:00.000000 dj3base-0.1.0/dj3base/__init__.py
--rw-rw-r--   0 qiang     (1000) qiang     (1000)      170 2023-06-11 14:52:32.000000 dj3base-0.1.0/dj3base/type_hints.py
-drwxrwxr-x   0 qiang     (1000) qiang     (1000)        0 2023-06-11 14:53:41.669265 dj3base-0.1.0/dj3base.egg-info/
--rw-rw-r--   0 qiang     (1000) qiang     (1000)     1165 2023-06-11 14:53:41.000000 dj3base-0.1.0/dj3base.egg-info/PKG-INFO
--rw-rw-r--   0 qiang     (1000) qiang     (1000)      244 2023-06-11 14:53:41.000000 dj3base-0.1.0/dj3base.egg-info/SOURCES.txt
--rw-rw-r--   0 qiang     (1000) qiang     (1000)        1 2023-06-11 14:53:41.000000 dj3base-0.1.0/dj3base.egg-info/dependency_links.txt
--rw-rw-r--   0 qiang     (1000) qiang     (1000)        1 2023-06-11 14:53:41.000000 dj3base-0.1.0/dj3base.egg-info/not-zip-safe
--rw-rw-r--   0 qiang     (1000) qiang     (1000)        8 2023-06-11 14:53:41.000000 dj3base-0.1.0/dj3base.egg-info/top_level.txt
--rw-rw-r--   0 qiang     (1000) qiang     (1000)     1075 2023-06-11 14:53:41.669265 dj3base-0.1.0/setup.cfg
--rw-rw-r--   0 qiang     (1000) qiang     (1000)       39 2023-03-27 09:15:19.000000 dj3base-0.1.0/setup.py
+drwxrwxr-x   0 qiang     (1000) qiang     (1000)        0 2023-06-24 06:35:30.615777 dj3base-0.1.1/
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)    11357 2023-03-27 09:15:19.000000 dj3base-0.1.1/LICENSE
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)       65 2023-06-11 14:45:58.000000 dj3base-0.1.1/MANIFEST.in
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)     1165 2023-06-24 06:35:30.615777 dj3base-0.1.1/PKG-INFO
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)      103 2023-06-11 14:47:02.000000 dj3base-0.1.1/README.md
+drwxrwxr-x   0 qiang     (1000) qiang     (1000)        0 2023-06-24 06:35:30.615777 dj3base-0.1.1/dj3base/
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)       46 2023-06-24 06:33:55.000000 dj3base-0.1.1/dj3base/__init__.py
+drwxrwxr-x   0 qiang     (1000) qiang     (1000)        0 2023-06-24 06:35:30.615777 dj3base-0.1.1/dj3base/commands/
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)       72 2023-06-24 06:23:39.000000 dj3base-0.1.1/dj3base/commands/__init__.py
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)      584 2023-06-24 06:23:16.000000 dj3base-0.1.1/dj3base/commands/singleton_command.py
+drwxrwxr-x   0 qiang     (1000) qiang     (1000)        0 2023-06-24 06:35:30.615777 dj3base-0.1.1/dj3base/tests/
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)       24 2023-06-24 06:24:17.000000 dj3base-0.1.1/dj3base/tests/__init__.py
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)      143 2023-06-24 06:33:55.000000 dj3base-0.1.1/dj3base/tests/utils.py
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)      170 2023-06-11 14:52:32.000000 dj3base-0.1.1/dj3base/type_hints.py
+drwxrwxr-x   0 qiang     (1000) qiang     (1000)        0 2023-06-24 06:35:30.615777 dj3base-0.1.1/dj3base.egg-info/
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)     1165 2023-06-24 06:35:30.000000 dj3base-0.1.1/dj3base.egg-info/PKG-INFO
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)      390 2023-06-24 06:35:30.000000 dj3base-0.1.1/dj3base.egg-info/SOURCES.txt
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)        1 2023-06-24 06:35:30.000000 dj3base-0.1.1/dj3base.egg-info/dependency_links.txt
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)        1 2023-06-24 06:35:30.000000 dj3base-0.1.1/dj3base.egg-info/not-zip-safe
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)        6 2023-06-24 06:35:30.000000 dj3base-0.1.1/dj3base.egg-info/requires.txt
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)        8 2023-06-24 06:35:30.000000 dj3base-0.1.1/dj3base.egg-info/top_level.txt
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)     1102 2023-06-24 06:35:30.615777 dj3base-0.1.1/setup.cfg
+-rw-rw-r--   0 qiang     (1000) qiang     (1000)       39 2023-03-27 09:15:19.000000 dj3base-0.1.1/setup.py
```

### Comparing `dj3base-0.1.0/LICENSE` & `dj3base-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj3base-0.1.0/PKG-INFO` & `dj3base-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj3base
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django utils.
 Home-page: https://gitee.com/three-kinds/dj3base
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://gitee.com/three-kinds/dj3base
 Project-URL: Source, https://gitee.com/three-kinds/dj3base
```

### Comparing `dj3base-0.1.0/dj3base.egg-info/PKG-INFO` & `dj3base-0.1.1/dj3base.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj3base
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django utils.
 Home-page: https://gitee.com/three-kinds/dj3base
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://gitee.com/three-kinds/dj3base
 Project-URL: Source, https://gitee.com/three-kinds/dj3base
```

### Comparing `dj3base-0.1.0/setup.cfg` & `dj3base-0.1.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -27,12 +27,14 @@
 	Source = https://gitee.com/three-kinds/dj3base
 
 [options]
 python_requires = >=3.8
 packages = dj3base
 include_package_data = true
 zip_safe = false
+install_requires = 
+	tendo
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

