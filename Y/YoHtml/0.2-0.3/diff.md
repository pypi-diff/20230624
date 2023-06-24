# Comparing `tmp/YoHtml-0.2.tar.gz` & `tmp/YoHtml-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YoHtml-0.2.tar", last modified: Sat Jun 24 06:11:19 2023, max compression
+gzip compressed data, was "YoHtml-0.3.tar", last modified: Sat Jun 24 06:18:59 2023, max compression
```

## Comparing `YoHtml-0.2.tar` & `YoHtml-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 06:11:19.614143 YoHtml-0.2/
--rw-rw-rw-   0        0        0     1064 2023-06-24 05:46:30.000000 YoHtml-0.2/LICENSE
--rw-rw-rw-   0        0        0     1466 2023-06-24 06:11:19.611832 YoHtml-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1030 2023-06-24 05:46:30.000000 YoHtml-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 06:11:19.607436 YoHtml-0.2/YoHtml.egg-info/
--rw-rw-rw-   0        0        0     1466 2023-06-24 06:11:19.000000 YoHtml-0.2/YoHtml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-06-24 06:11:19.000000 YoHtml-0.2/YoHtml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 06:11:19.000000 YoHtml-0.2/YoHtml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 06:11:19.000000 YoHtml-0.2/YoHtml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 06:11:19.615145 YoHtml-0.2/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-06-24 06:07:49.000000 YoHtml-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 06:11:19.610362 YoHtml-0.2/yohtml/
--rw-rw-rw-   0        0        0     1039 2023-06-24 05:46:30.000000 YoHtml-0.2/yohtml/HTPY.py
--rw-rw-rw-   0        0        0       18 2023-06-24 05:46:30.000000 YoHtml-0.2/yohtml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:18:59.670459 YoHtml-0.3/
+-rw-rw-rw-   0        0        0     1064 2023-06-24 05:46:30.000000 YoHtml-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1466 2023-06-24 06:18:59.670459 YoHtml-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1030 2023-06-24 05:46:30.000000 YoHtml-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 06:18:59.665456 YoHtml-0.3/YoHtml.egg-info/
+-rw-rw-rw-   0        0        0     1466 2023-06-24 06:18:59.000000 YoHtml-0.3/YoHtml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-06-24 06:18:59.000000 YoHtml-0.3/YoHtml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 06:18:59.000000 YoHtml-0.3/YoHtml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 06:18:59.000000 YoHtml-0.3/YoHtml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 06:18:59.671580 YoHtml-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-06-24 06:18:39.000000 YoHtml-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:18:59.669454 YoHtml-0.3/yohtml/
+-rw-rw-rw-   0        0        0     1039 2023-06-24 05:46:30.000000 YoHtml-0.3/yohtml/HTPY.py
+-rw-rw-rw-   0        0        0       18 2023-06-24 06:18:38.000000 YoHtml-0.3/yohtml/__init__.py
```

### Comparing `YoHtml-0.2/LICENSE` & `YoHtml-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `YoHtml-0.2/PKG-INFO` & `YoHtml-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YoHtml
-Version: 0.2
+Version: 0.3
 Summary: This allows you to create HTML websites in Python language
 Home-page: https://github.com/weee456/PyHtml-yobi
 Author: weee456
 Author-email: jhweee456@outlook.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `YoHtml-0.2/README.md` & `YoHtml-0.3/README.md`

 * *Files identical despite different names*

### Comparing `YoHtml-0.2/YoHtml.egg-info/PKG-INFO` & `YoHtml-0.3/YoHtml.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YoHtml
-Version: 0.2
+Version: 0.3
 Summary: This allows you to create HTML websites in Python language
 Home-page: https://github.com/weee456/PyHtml-yobi
 Author: weee456
 Author-email: jhweee456@outlook.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `YoHtml-0.2/setup.py` & `YoHtml-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="YoHtml",
-    version="0.2",
+    version="0.3",
     license='MIT',
     author="weee456",
     author_email="jhweee456@outlook.com",
     description="This allows you to create HTML websites in Python language",
     long_description=open('README.md', 'r', encoding='utf8').read(),
     url="https://github.com/weee456/PyHtml-yobi",
     packages=setuptools.find_packages(),
```

### Comparing `YoHtml-0.2/yohtml/HTPY.py` & `YoHtml-0.3/yohtml/HTPY.py`

 * *Files identical despite different names*

