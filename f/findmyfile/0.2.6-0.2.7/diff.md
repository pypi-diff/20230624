# Comparing `tmp/findmyfile-0.2.6.tar.gz` & `tmp/findmyfile-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyfile-0.2.6.tar", last modified: Sat Jun 24 11:14:11 2023, max compression
+gzip compressed data, was "findmyfile-0.2.7.tar", last modified: Sat Jun 24 11:26:19 2023, max compression
```

## Comparing `findmyfile-0.2.6.tar` & `findmyfile-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-24 11:14:11.906000 findmyfile-0.2.6/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1061 2023-06-24 01:20:32.000000 findmyfile-0.2.6/LICENCE.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      688 2023-06-24 11:14:11.886000 findmyfile-0.2.6/PKG-INFO
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     2500 2023-06-24 10:15:12.000000 findmyfile-0.2.6/README.md
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-24 11:14:11.506000 findmyfile-0.2.6/findmyfile/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       39 2023-06-24 10:58:56.000000 findmyfile-0.2.6/findmyfile/__init__.py
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       64 2023-06-24 10:59:26.000000 findmyfile-0.2.6/findmyfile/__main__.py
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     7966 2023-06-24 11:01:26.000000 findmyfile-0.2.6/findmyfile/main.py
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-24 11:14:11.831000 findmyfile-0.2.6/findmyfile.egg-info/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      688 2023-06-24 11:14:10.000000 findmyfile-0.2.6/findmyfile.egg-info/PKG-INFO
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      301 2023-06-24 11:14:11.000000 findmyfile-0.2.6/findmyfile.egg-info/SOURCES.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        1 2023-06-24 11:14:10.000000 findmyfile-0.2.6/findmyfile.egg-info/dependency_links.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       47 2023-06-24 11:14:10.000000 findmyfile-0.2.6/findmyfile.egg-info/entry_points.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       39 2023-06-24 11:14:10.000000 findmyfile-0.2.6/findmyfile.egg-info/requires.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       11 2023-06-24 11:14:10.000000 findmyfile-0.2.6/findmyfile.egg-info/top_level.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       38 2023-06-24 11:14:11.903000 findmyfile-0.2.6/setup.cfg
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1682 2023-06-24 11:13:49.000000 findmyfile-0.2.6/setup.py
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-24 11:26:19.562000 findmyfile-0.2.7/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1061 2023-06-24 01:20:32.000000 findmyfile-0.2.7/LICENCE.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      688 2023-06-24 11:26:19.546000 findmyfile-0.2.7/PKG-INFO
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     2500 2023-06-24 10:15:12.000000 findmyfile-0.2.7/README.md
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-24 11:26:19.183000 findmyfile-0.2.7/findmyfile/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       39 2023-06-24 10:58:56.000000 findmyfile-0.2.7/findmyfile/__init__.py
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       64 2023-06-24 10:59:26.000000 findmyfile-0.2.7/findmyfile/__main__.py
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     7966 2023-06-24 11:01:26.000000 findmyfile-0.2.7/findmyfile/main.py
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-24 11:26:19.496000 findmyfile-0.2.7/findmyfile.egg-info/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      688 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/PKG-INFO
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      301 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        1 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       45 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/entry_points.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       39 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/requires.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       11 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/top_level.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       38 2023-06-24 11:26:19.560000 findmyfile-0.2.7/setup.cfg
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1680 2023-06-24 11:26:11.000000 findmyfile-0.2.7/setup.py
```

### Comparing `findmyfile-0.2.6/LICENCE.txt` & `findmyfile-0.2.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `findmyfile-0.2.6/PKG-INFO` & `findmyfile-0.2.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyfile
-Version: 0.2.6
+Version: 0.2.7
 Summary: This package allows you to search a directory for documents that match keywords
 Home-page: https://github.com/Sanjin84/findmyfile
 Download-URL: https://github.com/Sanjin84/findmyfile/archive/refs/tags/v_01.tar.gz
 Author: Sanjin Dedic
 Author-email: sanjindedic8@gmail.com
 License: MIT
 Keywords: file search,find file,search directory
```

### Comparing `findmyfile-0.2.6/README.md` & `findmyfile-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `findmyfile-0.2.6/findmyfile/main.py` & `findmyfile-0.2.7/findmyfile/main.py`

 * *Files identical despite different names*

### Comparing `findmyfile-0.2.6/findmyfile.egg-info/PKG-INFO` & `findmyfile-0.2.7/findmyfile.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyfile
-Version: 0.2.6
+Version: 0.2.7
 Summary: This package allows you to search a directory for documents that match keywords
 Home-page: https://github.com/Sanjin84/findmyfile
 Download-URL: https://github.com/Sanjin84/findmyfile/archive/refs/tags/v_01.tar.gz
 Author: Sanjin Dedic
 Author-email: sanjindedic8@gmail.com
 License: MIT
 Keywords: file search,find file,search directory
```

### Comparing `findmyfile-0.2.6/setup.py` & `findmyfile-0.2.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='findmyfile',         # How you named your package folder (MyLib)
     packages=find_packages(),   # Chose the same as "name"
-    version='0.2.6',      # Start with a small number and increase it with every change you make
+    version='0.2.7',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='This package allows you to search a directory for documents that match keywords',
     author='Sanjin Dedic',                   # Type in your name
     author_email='sanjindedic8@gmail.com',      # Type in your E-Mail
     # Provide either the link to your github or to your website
     url='https://github.com/Sanjin84/findmyfile',
     # I explain this later on
     download_url='https://github.com/Sanjin84/findmyfile/archive/refs/tags/v_01.tar.gz',
     # Keywords that define your package best
     keywords=['file search', 'find file', 'search directory'],
     entry_points={
         'console_scripts': [
-            'fmf = find_my_file.main:main',
+            'fmf = findmyfile.main:main',
         ],
     },
     install_requires=[
         # Add your dependencies here
         'PyMuPDF',
         'python-docx',
         'python-pptx',
```

