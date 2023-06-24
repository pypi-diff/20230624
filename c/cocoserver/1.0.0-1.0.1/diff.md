# Comparing `tmp/cocoserver-1.0.0.tar.gz` & `tmp/cocoserver-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocoserver-1.0.0.tar", last modified: Sat Jun 24 14:12:13 2023, max compression
+gzip compressed data, was "cocoserver-1.0.1.tar", last modified: Sat Jun 24 14:31:50 2023, max compression
```

## Comparing `cocoserver-1.0.0.tar` & `cocoserver-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:12:13.597147 cocoserver-1.0.0/
--rw-r--r--   0 culler     (501) staff       (20)    18092 2023-06-24 13:34:32.000000 cocoserver-1.0.0/LICENSE
--rw-r--r--   0 culler     (501) staff       (20)     2046 2023-06-24 14:12:13.596548 cocoserver-1.0.0/PKG-INFO
--rw-r--r--   0 culler     (501) staff       (20)     1879 2023-06-24 14:10:04.000000 cocoserver-1.0.0/README.rst
--rw-r--r--   0 culler     (501) staff       (20)     1132 2023-06-24 13:39:31.000000 cocoserver-1.0.0/pyproject.toml
--rw-r--r--   0 culler     (501) staff       (20)       38 2023-06-24 14:12:13.597294 cocoserver-1.0.0/setup.cfg
--rw-r--r--   0 culler     (501) staff       (20)      434 2023-06-24 13:39:31.000000 cocoserver-1.0.0/setup.py
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:12:13.591942 cocoserver-1.0.0/src/
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:12:13.594158 cocoserver-1.0.0/src/cocoserver/
--rw-r--r--   0 culler     (501) staff       (20)     5963 2023-06-24 14:11:40.000000 cocoserver-1.0.0/src/cocoserver/__init__.py
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:12:13.596054 cocoserver-1.0.0/src/cocoserver.egg-info/
--rw-r--r--   0 culler     (501) staff       (20)     2046 2023-06-24 14:12:13.000000 cocoserver-1.0.0/src/cocoserver.egg-info/PKG-INFO
--rw-r--r--   0 culler     (501) staff       (20)      221 2023-06-24 14:12:13.000000 cocoserver-1.0.0/src/cocoserver.egg-info/SOURCES.txt
--rw-r--r--   0 culler     (501) staff       (20)        1 2023-06-24 14:12:13.000000 cocoserver-1.0.0/src/cocoserver.egg-info/dependency_links.txt
--rw-r--r--   0 culler     (501) staff       (20)       11 2023-06-24 14:12:13.000000 cocoserver-1.0.0/src/cocoserver.egg-info/top_level.txt
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:31:50.699493 cocoserver-1.0.1/
+-rw-r--r--   0 culler     (501) staff       (20)    18092 2023-06-24 13:34:32.000000 cocoserver-1.0.1/LICENSE
+-rw-r--r--   0 culler     (501) staff       (20)     2138 2023-06-24 14:31:50.699116 cocoserver-1.0.1/PKG-INFO
+-rw-r--r--   0 culler     (501) staff       (20)     1971 2023-06-24 14:27:51.000000 cocoserver-1.0.1/README.rst
+-rw-r--r--   0 culler     (501) staff       (20)     1132 2023-06-24 13:39:31.000000 cocoserver-1.0.1/pyproject.toml
+-rw-r--r--   0 culler     (501) staff       (20)       38 2023-06-24 14:31:50.699596 cocoserver-1.0.1/setup.cfg
+-rw-r--r--   0 culler     (501) staff       (20)      434 2023-06-24 13:39:31.000000 cocoserver-1.0.1/setup.py
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:31:50.693984 cocoserver-1.0.1/src/
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:31:50.696362 cocoserver-1.0.1/src/cocoserver/
+-rw-r--r--   0 culler     (501) staff       (20)     5963 2023-06-24 14:31:27.000000 cocoserver-1.0.1/src/cocoserver/__init__.py
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-24 14:31:50.698516 cocoserver-1.0.1/src/cocoserver.egg-info/
+-rw-r--r--   0 culler     (501) staff       (20)     2138 2023-06-24 14:31:50.000000 cocoserver-1.0.1/src/cocoserver.egg-info/PKG-INFO
+-rw-r--r--   0 culler     (501) staff       (20)      221 2023-06-24 14:31:50.000000 cocoserver-1.0.1/src/cocoserver.egg-info/SOURCES.txt
+-rw-r--r--   0 culler     (501) staff       (20)        1 2023-06-24 14:31:50.000000 cocoserver-1.0.1/src/cocoserver.egg-info/dependency_links.txt
+-rw-r--r--   0 culler     (501) staff       (20)       11 2023-06-24 14:31:50.000000 cocoserver-1.0.1/src/cocoserver.egg-info/top_level.txt
```

### Comparing `cocoserver-1.0.0/LICENSE` & `cocoserver-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cocoserver-1.0.0/PKG-INFO` & `cocoserver-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocoserver
-Version: 1.0.0
+Version: 1.0.1
 Summary: A local HTTP server for compressed content.
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 A Simple HTTP Server for Static Content
 =======================================
 
@@ -24,20 +24,21 @@
 typical case of serving compressed content over the internet since the
 compression is done in advance. It also takes significantly less space
 on the user's disk. (Brotli compression would be even more efficient
 in both ways, but web browsers still tend to only support Brotli
 compression over https, due to the prevalence of broken proxy servers
 on the internet.)
 
-The package includes a script (compress_site.py) for compressing all of
-the .html, .css, .js and .woff files below a given site root directory.
-The tool is aware of Sphinx's tendency to produce many identical copies
-of the same (large) _static directory.  So it also collects the contents
-of all of the _static subdirectories into one _static directory in the
-root, replacing the others by symlinks.
+Source code is available on `Github <https://github.com/3-manifolds/cocoserver/>`_.
+The git repository includes a script (compress_site.py) for compressing all of
+the .html, .css, .js and .woff files below a given site root directory.  The
+tool is aware of Sphinx's tendency to produce many identical copies of the same
+(large) _static directory.  So it also collects the contents of all of the
+_static subdirectories into one _static directory in the root, replacing the
+others by symlinks.
 
 The server can be installed by running: ``python3 -m pip install cocoserver``.
 
 To use the server::
   
   >>> from cocoserver import StaticServer
   >>> s = StaticServer('my/site/root')
```

### Comparing `cocoserver-1.0.0/README.rst` & `cocoserver-1.0.1/src/cocoserver.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: cocoserver
+Version: 1.0.1
+Summary: A local HTTP server for compressed content.
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 A Simple HTTP Server for Static Content
 =======================================
 
 This Python module provides a modified version of the ThreadedHTTPServer
 class from the http.server module in the standard library.  This server
 is designed to serve a static web site, such as documentation for a
 python project generated by Sphinx and installed with the software.  It
@@ -17,20 +24,21 @@
 typical case of serving compressed content over the internet since the
 compression is done in advance. It also takes significantly less space
 on the user's disk. (Brotli compression would be even more efficient
 in both ways, but web browsers still tend to only support Brotli
 compression over https, due to the prevalence of broken proxy servers
 on the internet.)
 
-The package includes a script (compress_site.py) for compressing all of
-the .html, .css, .js and .woff files below a given site root directory.
-The tool is aware of Sphinx's tendency to produce many identical copies
-of the same (large) _static directory.  So it also collects the contents
-of all of the _static subdirectories into one _static directory in the
-root, replacing the others by symlinks.
+Source code is available on `Github <https://github.com/3-manifolds/cocoserver/>`_.
+The git repository includes a script (compress_site.py) for compressing all of
+the .html, .css, .js and .woff files below a given site root directory.  The
+tool is aware of Sphinx's tendency to produce many identical copies of the same
+(large) _static directory.  So it also collects the contents of all of the
+_static subdirectories into one _static directory in the root, replacing the
+others by symlinks.
 
 The server can be installed by running: ``python3 -m pip install cocoserver``.
 
 To use the server::
   
   >>> from cocoserver import StaticServer
   >>> s = StaticServer('my/site/root')
```

### Comparing `cocoserver-1.0.0/pyproject.toml` & `cocoserver-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cocoserver-1.0.0/src/cocoserver/__init__.py` & `cocoserver-1.0.1/src/cocoserver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import email
 import shutil
 import datetime
 import webbrowser
 import urllib.parse
 import importlib.metadata
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 class GzipHTTPRequestHandler(SimpleHTTPRequestHandler):
 
     def log_message(self, format, *args):
         # We have no place for the log messages to go.
         pass
```

