# Comparing `tmp/pythorhead-0.8.3.tar.gz` & `tmp/pythorhead-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.8.3.tar", last modified: Sat Jun 24 16:28:08 2023, max compression
+gzip compressed data, was "pythorhead-0.9.0.tar", last modified: Sat Jun 24 19:34:52 2023, max compression
```

## Comparing `pythorhead-0.8.3.tar` & `pythorhead-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:28:08.898544 pythorhead-0.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:28:08.894544 pythorhead-0.8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:28:08.894544 pythorhead-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-24 16:27:44.000000 pythorhead-0.8.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-24 16:27:44.000000 pythorhead-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-06-24 16:27:52.000000 pythorhead-0.8.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-24 16:27:44.000000 pythorhead-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-24 16:28:08.898544 pythorhead-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-24 16:27:44.000000 pythorhead-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:28:08.894544 pythorhead-0.8.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-24 16:27:44.000000 pythorhead-0.8.3/examples/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-24 16:27:44.000000 pythorhead-0.8.3/examples/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-24 16:27:44.000000 pythorhead-0.8.3/examples/user.py
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-24 16:27:44.000000 pythorhead-0.8.3/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-24 16:27:52.000000 pythorhead-0.8.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:28:08.898544 pythorhead-0.8.3/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/post.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:28:08.898544 pythorhead-0.8.3/pythorhead/types/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/types/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/types/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/types/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-24 16:27:44.000000 pythorhead-0.8.3/pythorhead/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 16:28:08.898544 pythorhead-0.8.3/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-24 16:28:08.000000 pythorhead-0.8.3/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-24 16:28:08.000000 pythorhead-0.8.3/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 16:28:08.000000 pythorhead-0.8.3/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 16:28:08.000000 pythorhead-0.8.3/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 16:27:44.000000 pythorhead-0.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 16:28:08.898544 pythorhead-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:34:52.355025 pythorhead-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:34:52.351025 pythorhead-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:34:52.351025 pythorhead-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-24 19:34:31.000000 pythorhead-0.9.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-24 19:34:31.000000 pythorhead-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-06-24 19:34:39.000000 pythorhead-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-24 19:34:31.000000 pythorhead-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-24 19:34:52.355025 pythorhead-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-24 19:34:31.000000 pythorhead-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:34:52.355025 pythorhead-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-24 19:34:31.000000 pythorhead-0.9.0/examples/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-24 19:34:31.000000 pythorhead-0.9.0/examples/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-24 19:34:31.000000 pythorhead-0.9.0/examples/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-24 19:34:31.000000 pythorhead-0.9.0/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-24 19:34:39.000000 pythorhead-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:34:52.355025 pythorhead-0.9.0/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/community.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:34:52.355025 pythorhead-0.9.0/pythorhead/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/types/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/types/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-24 19:34:31.000000 pythorhead-0.9.0/pythorhead/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:34:52.355025 pythorhead-0.9.0/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-24 19:34:52.000000 pythorhead-0.9.0/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-24 19:34:52.000000 pythorhead-0.9.0/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:34:52.000000 pythorhead-0.9.0/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 19:34:52.000000 pythorhead-0.9.0/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:34:31.000000 pythorhead-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:34:52.355025 pythorhead-0.9.0/setup.cfg
```

### Comparing `pythorhead-0.8.3/.github/workflows/pypi.yml` & `pythorhead-0.9.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/.gitignore` & `pythorhead-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/CHANGELOG.md` & `pythorhead-0.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [v0.9.0](https://github.com/db0/pythorhead/tree/v0.9.0) (2023-06-24)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.8.3...v0.9.0)
+
+**Merged pull requests:**
+
+- feat: community create [\#25](https://github.com/db0/pythorhead/pull/25) ([sab666](https://github.com/sab666))
+
 ## [v0.8.3](https://github.com/db0/pythorhead/tree/v0.8.3) (2023-06-24)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.8.2...v0.8.3)
 
 **Merged pull requests:**
 
 - Supporting more PostSortType [\#26](https://github.com/db0/pythorhead/pull/26) ([NicKoehler](https://github.com/NicKoehler))
```

### Comparing `pythorhead-0.8.3/LICENSE` & `pythorhead-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/PKG-INFO` & `pythorhead-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.8.3
+Version: 0.9.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.8.3/README.md` & `pythorhead-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/examples/pm.py` & `pythorhead-0.9.0/examples/pm.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/examples/site.py` & `pythorhead-0.9.0/examples/site.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/examples/user.py` & `pythorhead-0.9.0/examples/user.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/logo.png` & `pythorhead-0.9.0/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/pyproject.toml` & `pythorhead-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.8.3"
+version = "v0.9.0"
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.8.3/pythorhead/comment.py` & `pythorhead-0.9.0/pythorhead/comment.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/pythorhead/image.py` & `pythorhead-0.9.0/pythorhead/image.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/pythorhead/lemmy.py` & `pythorhead-0.9.0/pythorhead/lemmy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import Optional
 
 from pythorhead.comment import Comment
+from pythorhead.community import Community
 from pythorhead.image import Image
 from pythorhead.post import Post
 from pythorhead.private_message import PrivateMessage
 from pythorhead.requestor import Request, Requestor
 from pythorhead.site import Site
 from pythorhead.user import User
 
@@ -16,14 +17,15 @@
     _known_communities = {}
     _requestor: Requestor
 
     def __init__(self, api_base_url: str) -> None:
         self._requestor = Requestor()
         self._requestor.set_domain(api_base_url)
         self.post = Post(self._requestor)
+        self.community = Community(self._requestor)
         self.comment = Comment(self._requestor)
         self.site = Site(self._requestor)
         self.user = User(self._requestor)
         self.private_message = PrivateMessage(self._requestor)
         self.image = Image(self._requestor)
 
     @property
```

### Comparing `pythorhead-0.8.3/pythorhead/post.py` & `pythorhead-0.9.0/pythorhead/post.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/pythorhead/private_message.py` & `pythorhead-0.9.0/pythorhead/private_message.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/pythorhead/requestor.py` & `pythorhead-0.9.0/pythorhead/requestor.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/pythorhead/site.py` & `pythorhead-0.9.0/pythorhead/site.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/pythorhead/user.py` & `pythorhead-0.9.0/pythorhead/user.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.8.3/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.9.0/pythorhead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.8.3
+Version: 0.9.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.8.3/pythorhead.egg-info/SOURCES.txt` & `pythorhead-0.9.0/pythorhead.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 .github/workflows/pypi.yml
 examples/pm.py
 examples/site.py
 examples/user.py
 pythorhead/__init__.py
 pythorhead/auth.py
 pythorhead/comment.py
+pythorhead/community.py
 pythorhead/image.py
 pythorhead/lemmy.py
 pythorhead/post.py
 pythorhead/private_message.py
 pythorhead/requestor.py
 pythorhead/site.py
 pythorhead/user.py
```

