# Comparing `tmp/nitrogfx-py-0.1.0.tar.gz` & `tmp/nitrogfx-py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrogfx-py-0.1.0.tar", last modified: Sat Jun 24 12:46:48 2023, max compression
+gzip compressed data, was "nitrogfx-py-0.1.1.tar", last modified: Sat Jun 24 13:38:31 2023, max compression
```

## Comparing `nitrogfx-py-0.1.0.tar` & `nitrogfx-py-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 fexx      (1000) fexx      (1000)        0 2023-06-24 12:46:48.038993 nitrogfx-py-0.1.0/
--rw-rw-r--   0 fexx      (1000) fexx      (1000)    35150 2023-06-06 20:46:54.000000 nitrogfx-py-0.1.0/LICENSE.txt
--rw-rw-r--   0 fexx      (1000) fexx      (1000)    41807 2023-06-24 12:46:48.038993 nitrogfx-py-0.1.0/PKG-INFO
--rw-rw-r--   0 fexx      (1000) fexx      (1000)      717 2023-06-24 12:42:14.000000 nitrogfx-py-0.1.0/README.md
-drwxrwxr-x   0 fexx      (1000) fexx      (1000)        0 2023-06-24 12:46:48.038993 nitrogfx-py-0.1.0/nitrogfx_py.egg-info/
--rw-rw-r--   0 fexx      (1000) fexx      (1000)    41807 2023-06-24 12:46:48.000000 nitrogfx-py-0.1.0/nitrogfx_py.egg-info/PKG-INFO
--rw-rw-r--   0 fexx      (1000) fexx      (1000)      210 2023-06-24 12:46:48.000000 nitrogfx-py-0.1.0/nitrogfx_py.egg-info/SOURCES.txt
--rw-rw-r--   0 fexx      (1000) fexx      (1000)        1 2023-06-24 12:46:48.000000 nitrogfx-py-0.1.0/nitrogfx_py.egg-info/dependency_links.txt
--rw-rw-r--   0 fexx      (1000) fexx      (1000)       14 2023-06-24 12:46:48.000000 nitrogfx-py-0.1.0/nitrogfx_py.egg-info/requires.txt
--rw-rw-r--   0 fexx      (1000) fexx      (1000)        9 2023-06-24 12:46:48.000000 nitrogfx-py-0.1.0/nitrogfx_py.egg-info/top_level.txt
--rw-rw-r--   0 fexx      (1000) fexx      (1000)      750 2023-06-24 11:43:21.000000 nitrogfx-py-0.1.0/pyproject.toml
--rw-rw-r--   0 fexx      (1000) fexx      (1000)       38 2023-06-24 12:46:48.038993 nitrogfx-py-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 13:38:31.968492 nitrogfx-py-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35150 2023-06-24 13:38:14.000000 nitrogfx-py-0.1.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    41806 2023-06-24 13:38:31.968492 nitrogfx-py-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-06-24 13:38:14.000000 nitrogfx-py-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 13:38:31.967492 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    41806 2023-06-24 13:38:31.000000 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-24 13:38:31.000000 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 13:38:31.000000 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-24 13:38:31.000000 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-24 13:38:31.000000 nitrogfx-py-0.1.1/nitrogfx_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-06-24 13:38:14.000000 nitrogfx-py-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 13:38:31.968492 nitrogfx-py-0.1.1/setup.cfg
```

### Comparing `nitrogfx-py-0.1.0/LICENSE.txt` & `nitrogfx-py-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nitrogfx-py-0.1.0/PKG-INFO` & `nitrogfx-py-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrogfx-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Nintendo DS Graphic format library
 Author-email: Fexean <3699814-Fexean@users.noreply.gitlab.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,23 +695,25 @@
 Currently it supports:
 
 - NCGR/NCBR tilesets
 - NSCR tilemaps
 - NCLR palettes
 - NCER sprite data
 
-The formats aren't perfectly implemented so the this most likely won't work with every game out there.
+The formats aren't perfectly implemented so this most likely won't work with every file from every game out there.
 
 ## Install from pip
 
     pip install nitrogfx-py
 
 ## Install from source (for development)
 
     git clone https://gitlab.com/Fexean/ntrgfx-py
     pip install --upgrade pip
     pip install -e ntrgfx-py
 
 ## Documentation
 
-The code is documented with docstrings. You can view them online at: https://fexean.gitlab.io/ntrgfx-py/nitrogfx.html
+The code is documented with docstrings.
+
+You can view them online at: https://fexean.gitlab.io/ntrgfx-py
```

### Comparing `nitrogfx-py-0.1.0/README.md` & `nitrogfx-py-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 Currently it supports:
 
 - NCGR/NCBR tilesets
 - NSCR tilemaps
 - NCLR palettes
 - NCER sprite data
 
-The formats aren't perfectly implemented so the this most likely won't work with every game out there.
+The formats aren't perfectly implemented so this most likely won't work with every file from every game out there.
 
 ## Install from pip
 
     pip install nitrogfx-py
 
 ## Install from source (for development)
 
     git clone https://gitlab.com/Fexean/ntrgfx-py
     pip install --upgrade pip
     pip install -e ntrgfx-py
 
 ## Documentation
 
-The code is documented with docstrings. You can view them online at: https://fexean.gitlab.io/ntrgfx-py/nitrogfx.html
+The code is documented with docstrings.
+
+You can view them online at: https://fexean.gitlab.io/ntrgfx-py
```

### Comparing `nitrogfx-py-0.1.0/nitrogfx_py.egg-info/PKG-INFO` & `nitrogfx-py-0.1.1/nitrogfx_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrogfx-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Nintendo DS Graphic format library
 Author-email: Fexean <3699814-Fexean@users.noreply.gitlab.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,23 +695,25 @@
 Currently it supports:
 
 - NCGR/NCBR tilesets
 - NSCR tilemaps
 - NCLR palettes
 - NCER sprite data
 
-The formats aren't perfectly implemented so the this most likely won't work with every game out there.
+The formats aren't perfectly implemented so this most likely won't work with every file from every game out there.
 
 ## Install from pip
 
     pip install nitrogfx-py
 
 ## Install from source (for development)
 
     git clone https://gitlab.com/Fexean/ntrgfx-py
     pip install --upgrade pip
     pip install -e ntrgfx-py
 
 ## Documentation
 
-The code is documented with docstrings. You can view them online at: https://fexean.gitlab.io/ntrgfx-py/nitrogfx.html
+The code is documented with docstrings.
+
+You can view them online at: https://fexean.gitlab.io/ntrgfx-py
```

### Comparing `nitrogfx-py-0.1.0/pyproject.toml` & `nitrogfx-py-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nitrogfx-py"
-version = "0.1.0"
+version = "0.1.1"
 keywords = ["NDS", "Nintendo DS", "NCGR", "NCLR", "NSCR"]
 authors = [
   { name="Fexean", email="3699814-Fexean@users.noreply.gitlab.com" },
 ]
 description = "Nintendo DS Graphic format library"
 readme = "README.md"
 requires-python = ">=3.7"
```

