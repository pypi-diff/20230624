# Comparing `tmp/finderz-2.0.1.tar.gz` & `tmp/finderz-2.0.2.tar.gz`

## Comparing `finderz-2.0.1.tar` & `finderz-2.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.1/.DS_Store
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 finderz-2.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 finderz-2.0.1/docs/code structure.rst
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 finderz-2.0.1/docs/conf.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 finderz-2.0.1/docs/credits.rst
--rw-r--r--   0        0        0    28295 2020-02-02 00:00:00.000000 finderz-2.0.1/docs/function use.rst
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 finderz-2.0.1/docs/index.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 finderz-2.0.1/docs/installation.rst
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 finderz-2.0.1/docs/updatev2.rst
--rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.1/docs/img/logo-color.jpg
--rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.1/logo/logo-color.jpg
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.1/old/src/.DS_Store
--rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 finderz-2.0.1/old/src/FinderZ/FinderZLib.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 finderz-2.0.1/old/src/FinderZ/__init__.py
--rw-r--r--   0        0        0    48923 2020-02-02 00:00:00.000000 finderz-2.0.1/src/FinderZV2.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 finderz-2.0.1/src/__init__.py
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 finderz-2.0.1/tests/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.1/tests/updates/.DS_Store
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 finderz-2.0.1/tests/updates/V2 Changelog.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 finderz-2.0.1/tests/updates/bash.sh
--rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 finderz-2.0.1/tests/updates/parentFunctions.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 finderz-2.0.1/tests/updates/update.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 finderz-2.0.1/LICENSE
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 finderz-2.0.1/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 finderz-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 finderz-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.2/.DS_Store
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 finderz-2.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 finderz-2.0.2/docs/code structure.rst
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 finderz-2.0.2/docs/conf.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 finderz-2.0.2/docs/credits.rst
+-rw-r--r--   0        0        0    28295 2020-02-02 00:00:00.000000 finderz-2.0.2/docs/function use.rst
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 finderz-2.0.2/docs/index.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 finderz-2.0.2/docs/installation.rst
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 finderz-2.0.2/docs/updatev2.rst
+-rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.2/docs/img/logo-color.jpg
+-rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.2/logo/logo-color.jpg
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.2/old/src/.DS_Store
+-rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 finderz-2.0.2/old/src/FinderZ/FinderZLib.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 finderz-2.0.2/old/src/FinderZ/__init__.py
+-rw-r--r--   0        0        0    48923 2020-02-02 00:00:00.000000 finderz-2.0.2/src/FinderZ/FinderZV2.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 finderz-2.0.2/src/FinderZ/__init__.py
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 finderz-2.0.2/tests/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.2/tests/updates/.DS_Store
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 finderz-2.0.2/tests/updates/V2 Changelog.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 finderz-2.0.2/tests/updates/bash.sh
+-rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 finderz-2.0.2/tests/updates/parentFunctions.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 finderz-2.0.2/tests/updates/update.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 finderz-2.0.2/LICENSE
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 finderz-2.0.2/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 finderz-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 finderz-2.0.2/PKG-INFO
```

### Comparing `finderz-2.0.1/.DS_Store` & `finderz-2.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/docs/code structure.rst` & `finderz-2.0.2/docs/code structure.rst`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/docs/conf.py` & `finderz-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/docs/function use.rst` & `finderz-2.0.2/docs/function use.rst`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/docs/index.rst` & `finderz-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/docs/updatev2.rst` & `finderz-2.0.2/docs/updatev2.rst`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/docs/img/logo-color.jpg` & `finderz-2.0.2/docs/img/logo-color.jpg`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/logo/logo-color.jpg` & `finderz-2.0.2/logo/logo-color.jpg`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/old/src/.DS_Store` & `finderz-2.0.2/old/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/old/src/FinderZ/FinderZLib.py` & `finderz-2.0.2/old/src/FinderZ/FinderZLib.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/src/FinderZV2.py` & `finderz-2.0.2/src/FinderZ/FinderZV2.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/tests/.DS_Store` & `finderz-2.0.2/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/tests/updates/.DS_Store` & `finderz-2.0.2/tests/updates/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/tests/updates/V2 Changelog.txt` & `finderz-2.0.2/tests/updates/V2 Changelog.txt`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/tests/updates/parentFunctions.py` & `finderz-2.0.2/tests/updates/parentFunctions.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/tests/updates/update.py` & `finderz-2.0.2/tests/updates/update.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/LICENSE` & `finderz-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/README.md` & `finderz-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `finderz-2.0.1/pyproject.toml` & `finderz-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FinderZ"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
 	{ name="PatzEdi", email="patzedigithub@gmail.com" },
 ]
 description = "A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 keywords = ["files", "filemanagement", "library", "development"]
```

### Comparing `finderz-2.0.1/PKG-INFO` & `finderz-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinderZ
-Version: 2.0.1
+Version: 2.0.2
 Summary: A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!
 Project-URL: Homepage, https://github.com/PatzEdi
 Project-URL: Repository, https://github.com/PatzEdi/FinderZ
 Project-URL: Bug Tracker, https://github.com/PatzEdi/FinderZ/issues
 Author-email: PatzEdi <patzedigithub@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
```

