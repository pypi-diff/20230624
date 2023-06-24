# Comparing `tmp/YoHtml-0.3.tar.gz` & `tmp/YoHtml-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YoHtml-0.3.tar", last modified: Sat Jun 24 06:18:59 2023, max compression
+gzip compressed data, was "YoHtml-0.5.tar", last modified: Sat Jun 24 13:58:37 2023, max compression
```

## Comparing `YoHtml-0.3.tar` & `YoHtml-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 06:18:59.670459 YoHtml-0.3/
--rw-rw-rw-   0        0        0     1064 2023-06-24 05:46:30.000000 YoHtml-0.3/LICENSE
--rw-rw-rw-   0        0        0     1466 2023-06-24 06:18:59.670459 YoHtml-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1030 2023-06-24 05:46:30.000000 YoHtml-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 06:18:59.665456 YoHtml-0.3/YoHtml.egg-info/
--rw-rw-rw-   0        0        0     1466 2023-06-24 06:18:59.000000 YoHtml-0.3/YoHtml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-06-24 06:18:59.000000 YoHtml-0.3/YoHtml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 06:18:59.000000 YoHtml-0.3/YoHtml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 06:18:59.000000 YoHtml-0.3/YoHtml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 06:18:59.671580 YoHtml-0.3/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-06-24 06:18:39.000000 YoHtml-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 06:18:59.669454 YoHtml-0.3/yohtml/
--rw-rw-rw-   0        0        0     1039 2023-06-24 05:46:30.000000 YoHtml-0.3/yohtml/HTPY.py
--rw-rw-rw-   0        0        0       18 2023-06-24 06:18:38.000000 YoHtml-0.3/yohtml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:58:37.497660 YoHtml-0.5/
+-rw-rw-rw-   0        0        0     1064 2023-06-24 05:46:30.000000 YoHtml-0.5/LICENSE
+-rw-rw-rw-   0        0        0     1444 2023-06-24 13:58:37.481757 YoHtml-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1008 2023-06-24 13:52:34.000000 YoHtml-0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 13:58:37.458397 YoHtml-0.5/YoHtml.egg-info/
+-rw-rw-rw-   0        0        0     1444 2023-06-24 13:58:37.000000 YoHtml-0.5/YoHtml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-06-24 13:58:37.000000 YoHtml-0.5/YoHtml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:58:37.000000 YoHtml-0.5/YoHtml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 13:58:37.000000 YoHtml-0.5/YoHtml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:58:37.497660 YoHtml-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-06-24 13:58:01.000000 YoHtml-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:58:37.466427 YoHtml-0.5/yohtml/
+-rw-rw-rw-   0        0        0     1829 2023-06-24 13:16:43.000000 YoHtml-0.5/yohtml/HTPY.py
+-rw-rw-rw-   0        0        0     1050 2023-06-24 13:17:15.000000 YoHtml-0.5/yohtml/__init__.py
```

### Comparing `YoHtml-0.3/LICENSE` & `YoHtml-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `YoHtml-0.3/PKG-INFO` & `YoHtml-0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YoHtml
-Version: 0.3
+Version: 0.5
 Summary: This allows you to create HTML websites in Python language
 Home-page: https://github.com/weee456/PyHtml-yobi
 Author: weee456
 Author-email: jhweee456@outlook.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,31 +13,31 @@
 License-File: LICENSE
 
 # PyHtml
 HTML 파싱  모듈 개발 (24/06/2023{FM 11:38} address : Korea) by : weee456
 
 # ko-kr(사용법) | en-us(Instructions)
 
-pip install PyHtml
+pip install YoHtml
 
 ===================================================================
 
-from pyhtml import pyhtml
+import yohtml
 
 ============================Lib import======================================
 
-DOCTYPE = pyhtml.HTPY.DOCTYPE(type='html')
+DOCTYPE = yohtml.DOCTYPE(type='html')
 
-html = pyhtml.HTPY.html(lang='ko')
+html = yohtml.html(lang='ko')
 
-body = pyhtml.HTPY.body()
+body = yohtml.HTPY.body()
 
-h1 = pyhtml.HTPY.Text(size='h1', text='hi')
+h1 = yohtml.HTPY.Text(size='h1', text='hi')
 
-close = pyhtml.HTPY.all_close()
+close = yohtml.HTPY.all_close()
 
 file = open('html_test.html','w',encoding='UTF-8')
 
 =============================Parsing========================================
 
 f = file.write(DOCTYPE)
```

### Comparing `YoHtml-0.3/README.md` & `YoHtml-0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # PyHtml
 HTML 파싱  모듈 개발 (24/06/2023{FM 11:38} address : Korea) by : weee456
 
 # ko-kr(사용법) | en-us(Instructions)
 
-pip install PyHtml
+pip install YoHtml
 
 ===================================================================
 
-from pyhtml import pyhtml
+import yohtml
 
 ============================Lib import======================================
 
-DOCTYPE = pyhtml.HTPY.DOCTYPE(type='html')
+DOCTYPE = yohtml.DOCTYPE(type='html')
 
-html = pyhtml.HTPY.html(lang='ko')
+html = yohtml.html(lang='ko')
 
-body = pyhtml.HTPY.body()
+body = yohtml.HTPY.body()
 
-h1 = pyhtml.HTPY.Text(size='h1', text='hi')
+h1 = yohtml.HTPY.Text(size='h1', text='hi')
 
-close = pyhtml.HTPY.all_close()
+close = yohtml.HTPY.all_close()
 
 file = open('html_test.html','w',encoding='UTF-8')
 
 =============================Parsing========================================
 
 f = file.write(DOCTYPE)
```

### Comparing `YoHtml-0.3/YoHtml.egg-info/PKG-INFO` & `YoHtml-0.5/YoHtml.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YoHtml
-Version: 0.3
+Version: 0.5
 Summary: This allows you to create HTML websites in Python language
 Home-page: https://github.com/weee456/PyHtml-yobi
 Author: weee456
 Author-email: jhweee456@outlook.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,31 +13,31 @@
 License-File: LICENSE
 
 # PyHtml
 HTML 파싱  모듈 개발 (24/06/2023{FM 11:38} address : Korea) by : weee456
 
 # ko-kr(사용법) | en-us(Instructions)
 
-pip install PyHtml
+pip install YoHtml
 
 ===================================================================
 
-from pyhtml import pyhtml
+import yohtml
 
 ============================Lib import======================================
 
-DOCTYPE = pyhtml.HTPY.DOCTYPE(type='html')
+DOCTYPE = yohtml.DOCTYPE(type='html')
 
-html = pyhtml.HTPY.html(lang='ko')
+html = yohtml.html(lang='ko')
 
-body = pyhtml.HTPY.body()
+body = yohtml.HTPY.body()
 
-h1 = pyhtml.HTPY.Text(size='h1', text='hi')
+h1 = yohtml.HTPY.Text(size='h1', text='hi')
 
-close = pyhtml.HTPY.all_close()
+close = yohtml.HTPY.all_close()
 
 file = open('html_test.html','w',encoding='UTF-8')
 
 =============================Parsing========================================
 
 f = file.write(DOCTYPE)
```

### Comparing `YoHtml-0.3/setup.py` & `YoHtml-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="YoHtml",
-    version="0.3",
+    version="0.5",
     license='MIT',
     author="weee456",
     author_email="jhweee456@outlook.com",
     description="This allows you to create HTML websites in Python language",
     long_description=open('README.md', 'r', encoding='utf8').read(),
     url="https://github.com/weee456/PyHtml-yobi",
     packages=setuptools.find_packages(),
```

