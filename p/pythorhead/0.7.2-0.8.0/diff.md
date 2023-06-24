# Comparing `tmp/pythorhead-0.7.2.tar.gz` & `tmp/pythorhead-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.7.2.tar", last modified: Fri Jun 23 10:19:03 2023, max compression
+gzip compressed data, was "pythorhead-0.8.0.tar", last modified: Sat Jun 24 06:39:50 2023, max compression
```

## Comparing `pythorhead-0.7.2.tar` & `pythorhead-0.8.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.254359 pythorhead-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.250359 pythorhead-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.250359 pythorhead-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-23 10:18:47.000000 pythorhead-0.7.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-23 10:18:47.000000 pythorhead-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-23 10:18:53.000000 pythorhead-0.7.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-23 10:18:47.000000 pythorhead-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-23 10:19:03.254359 pythorhead-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-23 10:18:47.000000 pythorhead-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.250359 pythorhead-0.7.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-23 10:18:47.000000 pythorhead-0.7.2/examples/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-23 10:18:47.000000 pythorhead-0.7.2/examples/user.py
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-23 10:18:47.000000 pythorhead-0.7.2/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-23 10:18:53.000000 pythorhead-0.7.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.250359 pythorhead-0.7.2/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/post.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.254359 pythorhead-0.7.2/pythorhead/types/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/types/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/types/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/types/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.254359 pythorhead-0.7.2/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-23 10:19:03.000000 pythorhead-0.7.2/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-23 10:19:03.000000 pythorhead-0.7.2/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:19:03.000000 pythorhead-0.7.2/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 10:19:03.000000 pythorhead-0.7.2/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:18:47.000000 pythorhead-0.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:19:03.254359 pythorhead-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:39:50.971352 pythorhead-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:39:50.967352 pythorhead-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:39:50.967352 pythorhead-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-24 06:39:33.000000 pythorhead-0.8.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-24 06:39:33.000000 pythorhead-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-24 06:39:40.000000 pythorhead-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-24 06:39:33.000000 pythorhead-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-24 06:39:50.967352 pythorhead-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-24 06:39:33.000000 pythorhead-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:39:50.967352 pythorhead-0.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-24 06:39:33.000000 pythorhead-0.8.0/examples/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-24 06:39:33.000000 pythorhead-0.8.0/examples/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-24 06:39:33.000000 pythorhead-0.8.0/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-24 06:39:41.000000 pythorhead-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:39:50.967352 pythorhead-0.8.0/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:39:50.967352 pythorhead-0.8.0/pythorhead/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/types/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/types/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-24 06:39:33.000000 pythorhead-0.8.0/pythorhead/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 06:39:50.967352 pythorhead-0.8.0/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-24 06:39:50.000000 pythorhead-0.8.0/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-24 06:39:50.000000 pythorhead-0.8.0/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 06:39:50.000000 pythorhead-0.8.0/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 06:39:50.000000 pythorhead-0.8.0/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 06:39:33.000000 pythorhead-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 06:39:50.971352 pythorhead-0.8.0/setup.cfg
```

### Comparing `pythorhead-0.7.2/.github/workflows/pypi.yml` & `pythorhead-0.8.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.2/.gitignore` & `pythorhead-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.2/CHANGELOG.md` & `pythorhead-0.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [v0.8.0](https://github.com/db0/pythorhead/tree/v0.8.0) (2023-06-24)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.7.2...v0.8.0)
+
+**Merged pull requests:**
+
+- initial image upload implentation [\#21](https://github.com/db0/pythorhead/pull/21) ([NicKoehler](https://github.com/NicKoehler))
+
 ## [v0.7.2](https://github.com/db0/pythorhead/tree/v0.7.2) (2023-06-23)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.7.1...v0.7.2)
 
 **Merged pull requests:**
 
 - added comment methods [\#20](https://github.com/db0/pythorhead/pull/20) ([retiolus](https://github.com/retiolus))
```

### Comparing `pythorhead-0.7.2/LICENSE` & `pythorhead-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.2/PKG-INFO` & `pythorhead-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.7.2
+Version: 0.8.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.7.2/README.md` & `pythorhead-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.2/examples/pm.py` & `pythorhead-0.8.0/examples/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,59 @@
-
 ## python examples/user.py db0
 
-import os
 import argparse
 import json
-from pythorhead import Lemmy
+import os
 
+from pythorhead import Lemmy
 
 arg_parser = argparse.ArgumentParser()
-arg_parser.add_argument('username', action="store")
-arg_parser.add_argument('content', action="store")
-arg_parser.add_argument('-d', '--lemmy_domain', action='store', required=False, type=str, help="the domain in which to look for this user")
-arg_parser.add_argument('-u', '--lemmy_username', action='store', required=False, type=str, help="Which user to authenticate as")
-arg_parser.add_argument('-p', '--lemmy_password', action='store', required=False, type=str, help="Which password to authenticate with")
+arg_parser.add_argument("username", action="store")
+arg_parser.add_argument(
+    "-d",
+    "--lemmy_domain",
+    action="store",
+    required=False,
+    type=str,
+    help="the domain in which to look for this user",
+)
+arg_parser.add_argument(
+    "-u",
+    "--lemmy_username",
+    action="store",
+    required=False,
+    type=str,
+    help="Which user to authenticate as",
+)
+arg_parser.add_argument(
+    "-p",
+    "--lemmy_password",
+    action="store",
+    required=False,
+    type=str,
+    help="Which password to authenticate with",
+)
 args = arg_parser.parse_args()
 
 
-
 lemmy_domain = args.lemmy_domain
 if not lemmy_domain:
-    lemmy_domain = os.getenv('LEMMY_DOMAIN', "lemmy.dbzer0.com")
+    lemmy_domain = os.getenv("LEMMY_DOMAIN", "lemmy.dbzer0.com")
 if not lemmy_domain:
     raise Exception("You need to provide a lemmy domain via env var or arg")
 
 lemmy_username = args.lemmy_username
 if not lemmy_username:
     lemmy_username = os.getenv("LEMMY_USERNAME")
 
-lemmy_password = args.lemmy_username
+lemmy_password = args.lemmy_password
 if not lemmy_password:
     lemmy_password = os.getenv("LEMMY_PASSWORD")
 
 lemmy = Lemmy(f"https://{lemmy_domain}")
 if lemmy_username and lemmy_password:
-    lemmy.log_in(lemmy_username, lemmy_password)
+    login = lemmy.log_in(lemmy_username, lemmy_password)
 user = lemmy.user.get(username=args.username)
-if not user:
-    raise Exception("No valid username found")
-pm = lemmy.private_message(args.content,user["person_view"]["person"]["id"])
-if not pm:
-    print("Sending private message failed")
+if user:
+    print(json.dumps(user["person_view"], indent=4))
+else:
+    print("no matching username found")
```

### Comparing `pythorhead-0.7.2/examples/user.py` & `pythorhead-0.8.0/examples/pm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,61 @@
-
 ## python examples/user.py db0
 
-import os
 import argparse
 import json
-from pythorhead import Lemmy
+import os
 
+from pythorhead import Lemmy
 
 arg_parser = argparse.ArgumentParser()
-arg_parser.add_argument('username', action="store")
-arg_parser.add_argument('-d', '--lemmy_domain', action='store', required=False, type=str, help="the domain in which to look for this user")
-arg_parser.add_argument('-u', '--lemmy_username', action='store', required=False, type=str, help="Which user to authenticate as")
-arg_parser.add_argument('-p', '--lemmy_password', action='store', required=False, type=str, help="Which password to authenticate with")
+arg_parser.add_argument("username", action="store")
+arg_parser.add_argument("content", action="store")
+arg_parser.add_argument(
+    "-d",
+    "--lemmy_domain",
+    action="store",
+    required=False,
+    type=str,
+    help="the domain in which to look for this user",
+)
+arg_parser.add_argument(
+    "-u",
+    "--lemmy_username",
+    action="store",
+    required=False,
+    type=str,
+    help="Which user to authenticate as",
+)
+arg_parser.add_argument(
+    "-p",
+    "--lemmy_password",
+    action="store",
+    required=False,
+    type=str,
+    help="Which password to authenticate with",
+)
 args = arg_parser.parse_args()
 
 
-
 lemmy_domain = args.lemmy_domain
 if not lemmy_domain:
-    lemmy_domain = os.getenv('LEMMY_DOMAIN', "lemmy.dbzer0.com")
+    lemmy_domain = os.getenv("LEMMY_DOMAIN", "lemmy.dbzer0.com")
 if not lemmy_domain:
     raise Exception("You need to provide a lemmy domain via env var or arg")
 
 lemmy_username = args.lemmy_username
 if not lemmy_username:
     lemmy_username = os.getenv("LEMMY_USERNAME")
 
-lemmy_password = args.lemmy_password
+lemmy_password = args.lemmy_username
 if not lemmy_password:
     lemmy_password = os.getenv("LEMMY_PASSWORD")
 
 lemmy = Lemmy(f"https://{lemmy_domain}")
 if lemmy_username and lemmy_password:
-    login = lemmy.log_in(lemmy_username, lemmy_password)
+    lemmy.log_in(lemmy_username, lemmy_password)
 user = lemmy.user.get(username=args.username)
-if user:
-    print(json.dumps(user["person_view"], indent=4))
-else:
-    print("no matching username found")
+if not user:
+    raise Exception("No valid username found")
+pm = lemmy.private_message(args.content, user["person_view"]["person"]["id"])
+if not pm:
+    print("Sending private message failed")
```

### Comparing `pythorhead-0.7.2/logo.png` & `pythorhead-0.8.0/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.2/pyproject.toml` & `pythorhead-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.7.2"
+version = "v0.8.0"
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.7.2/pythorhead/post.py` & `pythorhead-0.8.0/pythorhead/comment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,332 +1,274 @@
-from typing import Any, List, Literal, Optional
-
-from pythorhead.requestor import Request
-from pythorhead.types import FeatureType, ListingType, PostSortType
-
-
-class Post:
-    def __init__(self,_requestor):
-        self._requestor = _requestor
-
-    def get(
-        self,
-        post_id: int,
-        comment_id: Optional[int] = None,
-    ) -> Optional[dict]:
-        """
-        Get a post.
-
-        Args:
-            post_id (int)
-            comment_id (int, optional) Defaults to None.
-
-        Returns:
-            dict: post view
-        """
-        get_post = {
-            "id": post_id,
-        }
-
-        if comment_id is not None:
-            get_post["comment_id"] = comment_id
-
-        return self._requestor.request(Request.GET, "/post", params=get_post)
-
-    def list(  # noqa: A003
-        self,
-        community_id: Optional[int] = None,
-        community_name: Optional[str] = None,
-        limit: Optional[int] = None,
-        page: Optional[int] = None,
-        saved_only: Optional[bool] = None,
-        sort: Optional[PostSortType] = None,
-        type_: Optional[ListingType] = None,
-    ) -> List[dict]:
-        """
-
-        Get posts, with various filters.
-
-        Args:
-            community_id (int, optional): Defaults to None.
-            community_name (str, optional): Defaults to None.
-            limit (int, optional): Defaults to None.
-            page (int, optional): Defaults to None.
-            saved_only (bool, optional): Defaults to None.
-            sort (SortType, optional): Defaults to None.
-            type_ (ListingType, optional): Defaults to None.
-
-        Returns:
-            list[dict]: list of posts
-        """
-        list_post: dict = {}
-
-        if community_id is not None:
-            list_post["community_id"] = community_id
-        if community_name is not None:
-            list_post["community_name"] = community_name
-        if limit is not None:
-            list_post["limit"] = limit
-        if page is not None:
-            list_post["page"] = page
-        if saved_only is not None:
-            list_post["saved_only"] = saved_only
-        if sort is not None:
-            list_post["sort"] = sort.value
-        if type_ is not None:
-            list_post["type_"] = type_.value
-        if data := self._requestor.request(Request.GET, "/post/list", params=list_post):
-            return data["posts"]
-        return []
-
-    def create(
-        self,
-        community_id: int,
-        name: str,
-        url: Optional[str] = None,
-        body: Optional[str] = None,
-        nsfw: Optional[bool] = None,
-        honeypot: Optional[str] = None,
-        language_id: Optional[int] = None,
-    ) -> Optional[dict]:
-        """
-        Create a post
-
-        Args:
-            community_id (int)
-            name (str)
-            url (str, optional): Defaults to None.
-            body (str, optional): Defaults to None.
-            nsfw (bool, optional): Defaults to None.
-            honeypot (str, optional): Defaults to None.
-            language_id (int, optional): Defaults to None.
-
-        Returns:
-            Optional[dict]: post data if successful
-        """
-        new_post = {
-            "community_id": community_id,
-            "name": name,
-        }
-
-        if url is not None:
-            new_post["url"] = url
-        if body is not None:
-            new_post["body"] = body
-        if nsfw is not None:
-            new_post["nsfw"] = nsfw
-        if honeypot is not None:
-            new_post["honeypot"] = honeypot
-        if language_id is not None:
-            new_post["language_id"] = language_id
-
-        return self._requestor.request(Request.POST, "/post", json=new_post)
-
-    def delete(self, post_id: int, deleted: bool) -> Optional[dict]:
-        """
-        Deletes / Restore a post
-
-        Args:
-            post_id (int)
-            deleted (bool)
-
-        Returns:
-            Optional[dict]: post data if successful
-        """
-        delete_post = {
-            "post_id": post_id,
-            "deleted": deleted,
-        }
-        return self._requestor.request(Request.POST, "/post/delete", json=delete_post)
-
-    def remove(self, post_id: int, removed: bool, reason: Optional[str] = None) -> Optional[dict]:
-        """
-
-        Moderator remove / restore a post.
-
-        Args:
-            post_id (int)
-            removed (bool)
-            reason (str, optional): Defaults to None.
-
-        Returns:
-            Optional[dict]: post data if successful
-        """
-        remove_post = {
-            "post_id": post_id,
-            "removed": removed,
-        }
-        if reason is not None:
-            remove_post["reason"] = reason
-
-        return self._requestor.request(Request.POST, "/post/remove", json=remove_post)
-
-    def edit(
-        self,
-        post_id: int,
-        name: Optional[str] = None,
-        url: Optional[str] = None,
-        body: Optional[str] = None,
-        nsfw: Optional[bool] = None,
-        language_id: Optional[int] = None,
-    ) -> Optional[dict]:
-        """
-
-        Edit a post
-
-        Args:
-            post_id (int)
-            name (str, optional): Defaults to None.
-            url (str, optional): Defaults to None.
-            body (str, optional): Defaults to None.
-            nsfw (bool, optional): Defaults to None.
-            language_id (int, optional): Defaults to None.
-
-        Returns:
-            Optional[dict]: post data if successful
-        """
-        edit_post: dict[str, Any] = {
-            "post_id": post_id,
-        }
-        if name is not None:
-            edit_post["name"] = name
-        if url is not None:
-            edit_post["url"] = url
-        if body is not None:
-            edit_post["body"] = body
-        if nsfw is not None:
-            edit_post["nsfw"] = nsfw
-        if language_id is not None:
-            edit_post["language_id"] = language_id
-
-        return self._requestor.request(Request.PUT, "/post", json=edit_post)
-
-    def like(self, post_id: int, score: Literal[-1, 0, 1]) -> Optional[dict]:
-        """
-        Like / Dislike a post
-
-        Args:
-            post_id (int)
-            score (int)
-
-        Returns:
-            Optional[dict]: post data if successful
-        """
-        like_post = {
-            "post_id": post_id,
-            "score": score,
-        }
-        return self._requestor.request(Request.POST, "/post/like", json=like_post)
-
-    def save(self, post_id: int, saved: bool) -> Optional[dict]:
-        """
-
-        Add / Remove a post to saved posts
-
-        Args:
-            post_id (int)
-            saved (bool)
-
-        Returns:
-            Optional[dict]: post data if successful
-        """
-        save_post = {
-            "post_id": post_id,
-            "save": saved,
-        }
-        return self._requestor.request(Request.PUT, "/post/save", json=save_post)
-
-    def report(self, post_id: int, reason: str) -> Optional[dict]:
-        """
-
-        Report a post
-
-        Args:
-            post_id (int)
-            reason (str)
-
-        Returns:
-            Optional[dict]: post report data if successful
-        """
-        report_post = {
-            "post_id": post_id,
-            "reason": reason,
-        }
-        return self._requestor.request(Request.POST, "/post/report", json=report_post)
-
-    def feature(self, post_id: int, feature: bool, feature_type: FeatureType) -> Optional[dict]:
-        """
-
-        Add / Remove Feature from a post
-
-        Args:
-            post_id (int)
-            feature (bool)
-            feature_type (FeatureType)
-
-        Returns:
-            Optional[dict]: post data if successful
-        """
-
-        feature_post = {
-            "post_id": post_id,
-            "featured": feature,
-            "feature_type": feature_type.value,
-        }
-        return self._requestor.request(Request.POST, "/post/feature", json=feature_post)
-
-    def lock(self, post_id: int, locked: bool) -> Optional[dict]:
-        """
-
-        A moderator can lock a post ( IE disable new comments )
-
-        Args:
-            post_id (int)
-            locked (bool)
-
-        Returns:
-            Optional[dict]: post data if successful
-        """
-
-        lock_post = {
-            "post_id": post_id,
-            "locked": locked,
-        }
-        return self._requestor.request(Request.POST, "/post/lock", json=lock_post)
-
-    def mark_as_read(self, post_id: int, read: bool) -> Optional[dict]:
-        """
-
-        Mark a post as read
-
-        Args:
-            post_id (int)
-            read (bool)
-
-        Returns:
-            Optional[dict]: post data if successful
-        """
-
-        mark_as_read_post = {
-            "post_id": post_id,
-            "read": read,
-        }
-        return self._requestor.request(Request.POST, "/post/mark_as_read", json=mark_as_read_post)
-
-    def site_metadata(self, url: str) -> Optional[dict]:
-        """
-
-        Fetch metadata for any given site.
-
-        Args:
-            url (str)
-
-        Returns:
-            Optional[dict]: post data if successful
-        """
-
-        site_metadata_post = {
-            "url": url,
-        }
-        return self._requestor.request(Request.GET, "/post/site_metadata", params=site_metadata_post)
-
-    __call__ = create
+from typing import Any, List, Literal, Optional
+
+from pythorhead.requestor import Request, Requestor
+from pythorhead.types import CommentSortType, ListingType
+
+
+class Comment:
+    def __init__(self, _requestor: Requestor):
+        self._requestor = _requestor
+
+    def list(  # noqa: A003
+        self,
+        community_id: Optional[int] = None,
+        community_name: Optional[str] = None,
+        limit: Optional[int] = None,
+        max_depth: Optional[int] = None,
+        page: Optional[int] = None,
+        parent_id: Optional[int] = None,
+        post_id: Optional[int] = None,
+        saved_only: Optional[bool] = None,
+        sort: Optional[CommentSortType] = None,
+        type_: Optional[ListingType] = None,
+    ) -> List[dict]:
+        """
+
+        Get comments, with various filters.
+
+        Args:
+            community_id (Optional[int], optional): Defaults to None.
+            community_name (Optional[str], optional): Defaults to None.
+            limit (Optional[int], optional): Defaults to None.
+            max_depth (Optional[int], optional): Defaults to None.
+            page (Optional[int], optional): Defaults to None.
+            parent_id (Optional[int], optional): Defaults to None.
+            post_id (Optional[int], optional): Defaults to None.
+            saved_only (Optional[bool], optional): Defaults to None.
+            sort (Optional[CommentSortType], optional): Defaults to None.
+            type_ (Optional[ListingType], optional): Defaults to None.
+
+        Returns:
+            List[dict]: list of comments
+        """
+        list_comment = {}
+        if community_id is not None:
+            list_comment["community_id"] = community_id
+        if community_name is not None:
+            list_comment["community_name"] = community_name
+        if limit is not None:
+            list_comment["limit"] = limit
+        if max_depth is not None:
+            list_comment["max_depth"] = max_depth
+        if page is not None:
+            list_comment["page"] = page
+        if parent_id is not None:
+            list_comment["parent_id"] = parent_id
+        if post_id is not None:
+            list_comment["post_id"] = post_id
+        if saved_only is not None:
+            list_comment["saved_only"] = saved_only
+        if sort is not None:
+            list_comment["sort"] = sort.value
+        if type_ is not None:
+            list_comment["type"] = type_.value
+
+        if data := self._requestor.api(Request.GET, "/comment/list", params=list_comment):
+            return data["comments"]
+        return []
+
+    def create(
+        self,
+        post_id: int,
+        content: str,
+        form_id: Optional[str] = None,
+        parent_id: Optional[int] = None,
+        language_id: Optional[int] = None,
+    ) -> Optional[dict]:
+        """
+        Create a comment.
+
+        Args:
+            post_id (int)
+            content (str)
+            form_id (Optional[int], optional): Defaults to None.
+            parent_id (Optional[int], optional): Defaults to None.
+            language_id (Optional[int], optional): Defaults to None.
+
+        Returns:
+            Optional[dict]: created comment data if successful
+        """
+
+        create_comment = {
+            "post_id": post_id,
+            "content": content,
+        }
+        if form_id is not None:
+            create_comment["form_id"] = form_id
+        if parent_id is not None:
+            create_comment["parent_id"] = parent_id
+        if language_id is not None:
+            create_comment["language_id"] = language_id
+
+        return self._requestor.api(
+            Request.POST,
+            "/comment",
+            json=create_comment,
+        )
+
+    def edit(
+        self,
+        comment_id: int,
+        content: Optional[str] = None,
+        distinguished: Optional[bool] = None,
+        form_id: Optional[str] = None,
+        language_id: Optional[int] = None,
+    ) -> Optional[dict]:
+        """
+        Edit a comment.
+
+        Args:
+            comment_id (int)
+            content (Optional[str], optional): Defaults to None.
+            distinguished (Optional[bool], optional): Defaults to None.
+            form_id (Optional[str], optional): Defaults to None.
+            language_id (Optional[int], optional): Defaults to None.
+
+        Returns:
+            Optional[dict]: edited comment data if successful
+        """
+        edit_comment: dict[Any, Any] = {
+            "comment_id": comment_id,
+        }
+        if content is not None:
+            edit_comment["content"] = content
+        if distinguished is not None:
+            edit_comment["distinguished"] = distinguished
+        if form_id is not None:
+            edit_comment["form_id"] = form_id
+        if language_id is not None:
+            edit_comment["language_id"] = language_id
+
+        return self._requestor.api(
+            Request.PUT,
+            "/comment",
+            json=edit_comment,
+        )
+
+    def like(self, comment_id: int, score: Literal[-1, 0, 1]) -> Optional[dict]:
+        """
+        Like / Dislike a comment.
+
+        Args:
+            comment_id (int)
+            score (int)
+
+        Returns:
+            Optional[dict]: like comment data if successful
+        """
+        return self._requestor.api(
+            Request.POST,
+            "/comment/like",
+            json={
+                "comment_id": comment_id,
+                "score": score,
+            },
+        )
+
+    def delete(self, comment_id: int, deleted: bool) -> Optional[dict]:
+        """
+        Delete / Restore a comment.
+
+        Args:
+            comment_id (int): comment_id
+            deleted (bool): deleted
+
+        Returns:
+            Optional[dict]: deleted comment data if successful
+        """
+        return self._requestor.api(
+            Request.POST,
+            "/comment/delete",
+            json={
+                "comment_id": comment_id,
+                "deleted": deleted,
+            },
+        )
+
+    def remove(self, comment_id: int, removed: bool, reason: Optional[str] = None) -> Optional[dict]:
+        """
+        Moderator remove / restore a comment.
+
+        Args:
+            comment_id (int)
+            removed (bool)
+            reason (str, optional): Defaults to None.
+
+        Returns:
+            Optional[dict]: removed comment data if successful
+        """
+
+        remove_comment = {
+            "comment_id": comment_id,
+            "removed": removed,
+        }
+
+        if reason is not None:
+            remove_comment["reason"] = reason
+
+        return self._requestor.api(
+            Request.POST,
+            "/comment/remove",
+            json=remove_comment,
+        )
+
+    def save(self, comment_id: int, save: bool) -> Optional[dict]:
+        """
+        Add / Remove a comment from saved.
+
+        Args:
+            comment_id (int)
+            save (bool)
+
+        Returns:
+            Optional[dict]: saved comment data if successful
+
+        """
+        return self._requestor.api(
+            Request.PUT,
+            "/comment/save",
+            json={
+                "comment_id": comment_id,
+                "save": save,
+            },
+        )
+
+    def report(self, comment_id: int, reason: str) -> Optional[dict]:
+        """
+        Report a comment.
+
+        Args:
+            comment_id (int): comment_id
+            reason (str): reason
+
+        Returns:
+            Optional[dict]: report comment data if successful
+        """
+        return self._requestor.api(
+            Request.POST,
+            "/comment/report",
+            json={
+                "comment_id": comment_id,
+                "reason": reason,
+            },
+        )
+
+    def mark_as_read(self, comment_reply_id: int, read: bool) -> Optional[dict]:
+        """
+
+        Mark a comment as read
+
+        Args:
+            comment_reply_id (int)
+            read (bool)
+
+        Returns:
+            Optional[dict]: comment data if successful
+        """
+
+        mark_as_read_comment = {
+            "comment_reply_id": comment_reply_id,
+            "read": read,
+        }
+        return self._requestor.api(Request.POST, "/comment/mark_as_read", json=mark_as_read_comment)
+
+    __call__ = create
```

### Comparing `pythorhead-0.7.2/pythorhead/requestor.py` & `pythorhead-0.8.0/pythorhead/requestor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,86 @@
-import logging
-from enum import Enum
-from typing import Optional
-
-import requests
-
-from pythorhead.auth import Authentication
-
-logger = logging.getLogger(__name__)
-
-
-class Request(Enum):
-    GET = "GET"
-    PUT = "PUT"
-    POST = "POST"
-
-
-REQUEST_MAP = {
-    Request.GET: requests.get,
-    Request.PUT: requests.put,
-    Request.POST: requests.post,
-}
-
-
-class Requestor:
-    nodeinfo: dict = None
-    domain: Optional[str] = None
-
-    def __init__(self):
-        self._auth = Authentication()
-        self.set_api_base_url = self._auth.set_api_base_url
-
-    def set_domain(self, domain: str):
-        self.domain = domain
-        self._auth.set_api_base_url(f"{self.domain}/api/v3")
-        try:
-            self.nodeinfo = requests.get(f"{self.domain}/nodeinfo/2.0.json", timeout=2).json()
-        except Exception as err:
-            logger.error(f"Problem encountered retrieving Lemmy nodeinfo: {err}")
-            return
-        software = self.nodeinfo.get("software",{}).get("name")
-        if software != "lemmy":
-            logger.error(f"Domain name does not appear to contain a lemmy software, but instead '{software}")
-            return
-        logger.info(f"Connected succesfully to Lemmy v{self.nodeinfo['software']['version']} instance {self.domain}")
-
-
-    def request(self, method: Request, endpoint: str, **kwargs) -> Optional[dict]:
-        logger.info(f"Requesting {method} {endpoint}")
-        if self._auth.token:
-            if (data := kwargs.get("json")) is not None:
-                data["auth"] = self._auth.token
-            if (data := kwargs.get("params")) is not None:
-                data["auth"] = self._auth.token
-
-        r = REQUEST_MAP[method](f"{self._auth.api_base_url}{endpoint}", **kwargs)
-
-        if not r.ok:
-            logger.error(f"Error encountered while {method}: {r.text}")
-            return
-
-        return r.json()
-
-    def log_in(self, username_or_email: str, password: str) -> bool:
-        payload = {
-            "username_or_email": username_or_email,
-            "password": password,
-        }
-        if data := self.request(Request.POST, "/user/login", json=payload):
-            self._auth.set_token(data["jwt"])
-        return self._auth.token is not None
-
-    def log_out(self) -> None:
-        self._auth.token = None
+import logging
+from enum import Enum
+from typing import Optional
+
+import requests
+
+from pythorhead.auth import Authentication
+
+logger = logging.getLogger(__name__)
+
+
+class Request(Enum):
+    GET = "GET"
+    PUT = "PUT"
+    POST = "POST"
+
+
+REQUEST_MAP = {
+    Request.GET: requests.get,
+    Request.PUT: requests.put,
+    Request.POST: requests.post,
+}
+
+
+class Requestor:
+    nodeinfo: Optional[dict] = None
+    domain: Optional[str] = None
+
+    def __init__(self):
+        self._auth = Authentication()
+        self.set_api_base_url = self._auth.set_api_base_url
+
+    def set_domain(self, domain: str):
+        self.domain = domain
+        self._auth.set_api_base_url(self.domain)
+        try:
+            self.nodeinfo = requests.get(f"{self.domain}/nodeinfo/2.0.json", timeout=2).json()
+        except Exception as err:
+            logger.error(f"Problem encountered retrieving Lemmy nodeinfo: {err}")
+            return
+        software = self.nodeinfo.get("software", {}).get("name")
+        if software != "lemmy":
+            logger.error(f"Domain name does not appear to contain a lemmy software, but instead '{software}")
+            return
+        logger.info(f"Connected succesfully to Lemmy v{self.nodeinfo['software']['version']} instance {self.domain}")
+
+    def api(self, method: Request, endpoint: str, **kwargs) -> Optional[dict]:
+        logger.info(f"Requesting API {method} {endpoint}")
+        if self._auth.token:
+            if (data := kwargs.get("json")) is not None:
+                data["auth"] = self._auth.token
+            if (data := kwargs.get("params")) is not None:
+                data["auth"] = self._auth.token
+        try:
+            r = REQUEST_MAP[method](f"{self._auth.api_url}{endpoint}", **kwargs)
+        except Exception as err:
+            logger.error(f"Error encountered while {method}: {err}")
+            return
+        if not r.ok:
+            logger.error(f"Error encountered while {method}: {r.text}")
+            return
+
+        return r.json()
+
+    def image(self, method: Request, **kwargs) -> Optional[dict]:
+        logger.info(f"Requesting image {method}")
+        cookies = {}
+        if self._auth.token:
+            cookies["jwt"] = self._auth.token
+        r = REQUEST_MAP[method](self._auth.image_url, cookies=cookies, **kwargs)
+        if not r.ok:
+            logger.error(f"Error encountered while {method}: {r.text}")
+            return
+        return r.json()
+
+    def log_in(self, username_or_email: str, password: str) -> bool:
+        payload = {
+            "username_or_email": username_or_email,
+            "password": password,
+        }
+        if data := self.api(Request.POST, "/user/login", json=payload):
+            self._auth.set_token(data["jwt"])
+        return self._auth.token is not None
+
+    def log_out(self) -> None:
+        self._auth.token = None
```

### Comparing `pythorhead-0.7.2/pythorhead/site.py` & `pythorhead-0.8.0/pythorhead/site.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,121 @@
-from typing import Any, List, Literal, Optional
-
-from pythorhead.requestor import Request
-from pythorhead.types import ListingType
-
-
-class Site:
-    def __init__(self,_requestor):
-        self._requestor = _requestor
-
-    def get(
-        self,
-    ) -> Optional[dict]:
-        """
-        Get site details.
-
-        Returns:
-            dict: site view
-        """
-        return self._requestor.request(Request.GET, "/site")
-
-    def edit(
-        self,
-        name: Optional[str] = None,
-        sidebar: Optional[str] = None,
-        description: Optional[str] = None,
-        icon: Optional[str] = None,
-        banner: Optional[str] = None,
-        enable_downvotes: Optional[bool] = None,
-        enable_nsfw: Optional[bool] = None,
-        community_creation_admin_only: Optional[bool] = None,
-        require_email_verification: Optional[bool] = None,
-        application_question: Optional[str] = None,
-        private_instance: Optional[bool] = None,
-        default_theme: Optional[str] = None,
-        default_post_listing_type: Optional[ListingType] = None,
-        legal_information: Optional[str] = None,
-        application_email_admins: Optional[bool] = None,
-        hide_modlog_mod_names: Optional[bool] = None,
-        discussion_languages = None,
-        slur_filter_regex: Optional[str] = None,
-        actor_name_max_length: Optional[int] = None,
-        rate_limit_message: Optional[int] = None,
-        rate_limit_message_per_second: Optional[int] = None,
-        rate_limit_post: Optional[int] = None,
-        rate_limit_post_per_second: Optional[int] = None,
-        rate_limit_register: Optional[int] = None,
-        rate_limit_register_per_second: Optional[int] = None,
-        rate_limit_image: Optional[int] = None,
-        rate_limit_image_per_second: Optional[int] = None,
-        rate_limit_comment: Optional[int] = None,
-        rate_limit_comment_per_second: Optional[int] = None,
-        rate_limit_search: Optional[int] = None,
-        rate_limit_search_per_second: Optional[int] = None,
-        federation_enabled: Optional[bool] = None,
-        federation_debug: Optional[bool] = None,
-        federation_worker_count: Optional[int] = None,
-        captcha_enabled: Optional[bool] = None,
-        captcha_difficulty: Optional[str] = None,
-        allowed_instances: Optional[List] = None,
-        blocked_instances: Optional[List] = None,
-        taglines: Optional[List] = None,
-        registration_mode = None,
-        reports_email_admins: Optional[bool] = None,
-    ) -> Optional[dict]:
-        """
-
-        Edit site details
-
-        Args:
-            name (str, optional): Defaults to None.
-            sidebar (str, optional): Defaults to None.
-            description (str, optional): Defaults to None.
-            icon (str, optional): Defaults to None.
-            banner (str, optional): Defaults to None.
-            enable_downvotes (bool, optional): Defaults to None.
-            enable_nsfw (bool, optional): Defaults to None.
-            community_creation_admin_only (bool, optional): Defaults to None.
-            require_email_verification (bool, optional): Defaults to None.
-            application_question (str, optional): Defaults to None.
-            private_instance (bool, optional): Defaults to None.
-            default_theme (str, optional): Defaults to None.
-            default_post_listing_type (ListingType, optional): Defaults to None.
-            legal_information (str, optional): Defaults to None.
-            application_email_admins (bool, optional): Defaults to None.
-            hide_modlog_mod_names (bool, optional): Defaults to None.
-            discussion_languages (LanguageType, optional): Defaults to None.
-            slur_filter_regex (str, optional): Defaults to None.
-            actor_name_max_length (int, optional): Defaults to None.
-            rate_limit_message (int, optional): Defaults to None.
-            rate_limit_message_per_second (int, optional): Defaults to None.
-            rate_limit_post (int, optional): Defaults to None.
-            rate_limit_post_per_second (int, optional): Defaults to None.
-            rate_limit_register (int, optional): Defaults to None.
-            rate_limit_register_per_second (int, optional): Defaults to None.
-            rate_limit_image (int, optional): Defaults to None.
-            rate_limit_image_per_second (int, optional): Defaults to None.
-            rate_limit_comment (int, optional): Defaults to None.
-            rate_limit_comment_per_second (int, optional): Defaults to None.
-            rate_limit_search (int, optional): Defaults to None.
-            rate_limit_search_per_second (int, optional): Defaults to None.
-            federation_enabled (bool, optional): Defaults to None.
-            federation_debug (bool, optional): Defaults to None.
-            federation_worker_count (int, optional): Defaults to None.
-            captcha_enabled (bool, optional): Defaults to None.
-            captcha_difficulty (str, optional): Defaults to None.
-            allowed_instances (List(str), optional): Defaults to None.
-            blocked_instances (List(str), optional): Defaults to None.
-            taglines (List(str), optional): Defaults to None.
-            registration_mode Defaults to None.
-            reports_email_admins (bool, optional): Defaults to None.
-        Returns:
-            Optional[dict]: post data if successful
-        """
-        edit_site: dict[str, Any] = {key: value for key, value in locals().items() if value is not None and key != 'self'}
-        if len(edit_site) == 0:
-            raise Exception("Must provide at least one site property to change")
-        
-        return self._requestor.request(Request.PUT, "/site", json=edit_site)
+from typing import Any, List, Optional
+
+from pythorhead.requestor import Request, Requestor
+from pythorhead.types import ListingType
+
+
+class Site:
+    def __init__(self, _requestor: Requestor):
+        self._requestor = _requestor
+
+    def get(
+        self,
+    ) -> Optional[dict]:
+        """
+        Get site details.
+
+        Returns:
+            dict: site view
+        """
+        return self._requestor.api(Request.GET, "/site")
+
+    def edit(
+        self,
+        name: Optional[str] = None,
+        sidebar: Optional[str] = None,
+        description: Optional[str] = None,
+        icon: Optional[str] = None,
+        banner: Optional[str] = None,
+        enable_downvotes: Optional[bool] = None,
+        enable_nsfw: Optional[bool] = None,
+        community_creation_admin_only: Optional[bool] = None,
+        require_email_verification: Optional[bool] = None,
+        application_question: Optional[str] = None,
+        private_instance: Optional[bool] = None,
+        default_theme: Optional[str] = None,
+        default_post_listing_type: Optional[ListingType] = None,
+        legal_information: Optional[str] = None,
+        application_email_admins: Optional[bool] = None,
+        hide_modlog_mod_names: Optional[bool] = None,
+        discussion_languages=None,
+        slur_filter_regex: Optional[str] = None,
+        actor_name_max_length: Optional[int] = None,
+        rate_limit_message: Optional[int] = None,
+        rate_limit_message_per_second: Optional[int] = None,
+        rate_limit_post: Optional[int] = None,
+        rate_limit_post_per_second: Optional[int] = None,
+        rate_limit_register: Optional[int] = None,
+        rate_limit_register_per_second: Optional[int] = None,
+        rate_limit_image: Optional[int] = None,
+        rate_limit_image_per_second: Optional[int] = None,
+        rate_limit_comment: Optional[int] = None,
+        rate_limit_comment_per_second: Optional[int] = None,
+        rate_limit_search: Optional[int] = None,
+        rate_limit_search_per_second: Optional[int] = None,
+        federation_enabled: Optional[bool] = None,
+        federation_debug: Optional[bool] = None,
+        federation_worker_count: Optional[int] = None,
+        captcha_enabled: Optional[bool] = None,
+        captcha_difficulty: Optional[str] = None,
+        allowed_instances: Optional[List] = None,
+        blocked_instances: Optional[List] = None,
+        taglines: Optional[List] = None,
+        registration_mode=None,
+        reports_email_admins: Optional[bool] = None,
+    ) -> Optional[dict]:
+        """
+
+        Edit site details
+
+        Args:
+            name (str, optional): Defaults to None.
+            sidebar (str, optional): Defaults to None.
+            description (str, optional): Defaults to None.
+            icon (str, optional): Defaults to None.
+            banner (str, optional): Defaults to None.
+            enable_downvotes (bool, optional): Defaults to None.
+            enable_nsfw (bool, optional): Defaults to None.
+            community_creation_admin_only (bool, optional): Defaults to None.
+            require_email_verification (bool, optional): Defaults to None.
+            application_question (str, optional): Defaults to None.
+            private_instance (bool, optional): Defaults to None.
+            default_theme (str, optional): Defaults to None.
+            default_post_listing_type (ListingType, optional): Defaults to None.
+            legal_information (str, optional): Defaults to None.
+            application_email_admins (bool, optional): Defaults to None.
+            hide_modlog_mod_names (bool, optional): Defaults to None.
+            discussion_languages (LanguageType, optional): Defaults to None.
+            slur_filter_regex (str, optional): Defaults to None.
+            actor_name_max_length (int, optional): Defaults to None.
+            rate_limit_message (int, optional): Defaults to None.
+            rate_limit_message_per_second (int, optional): Defaults to None.
+            rate_limit_post (int, optional): Defaults to None.
+            rate_limit_post_per_second (int, optional): Defaults to None.
+            rate_limit_register (int, optional): Defaults to None.
+            rate_limit_register_per_second (int, optional): Defaults to None.
+            rate_limit_image (int, optional): Defaults to None.
+            rate_limit_image_per_second (int, optional): Defaults to None.
+            rate_limit_comment (int, optional): Defaults to None.
+            rate_limit_comment_per_second (int, optional): Defaults to None.
+            rate_limit_search (int, optional): Defaults to None.
+            rate_limit_search_per_second (int, optional): Defaults to None.
+            federation_enabled (bool, optional): Defaults to None.
+            federation_debug (bool, optional): Defaults to None.
+            federation_worker_count (int, optional): Defaults to None.
+            captcha_enabled (bool, optional): Defaults to None.
+            captcha_difficulty (str, optional): Defaults to None.
+            allowed_instances (List(str), optional): Defaults to None.
+            blocked_instances (List(str), optional): Defaults to None.
+            taglines (List(str), optional): Defaults to None.
+            registration_mode Defaults to None.
+            reports_email_admins (bool, optional): Defaults to None.
+        Returns:
+            Optional[dict]: post data if successful
+        """
+        edit_site: dict[str, Any] = {
+            key: value for key, value in locals().items() if value is not None and key != "self"
+        }
+        if len(edit_site) == 0:
+            raise Exception("Must provide at least one site property to change")
+
+        return self._requestor.api(Request.PUT, "/site", json=edit_site)
```

### Comparing `pythorhead-0.7.2/pythorhead/user.py` & `pythorhead-0.8.0/pythorhead/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from typing import Any, List, Literal, Optional
-
-from pythorhead.requestor import Request, Requestor
-from pythorhead.types import PostSortType
-
-
-class User:
-    def __init__(self,_requestor):
-        self._requestor = _requestor
-
-    def get(
-        self,
-        person_id: Optional[str] = None,
-        username: Optional[str] = None,
-        sort: Optional[PostSortType] = None,
-        page: Optional[int] = None,
-        limit: Optional[int] = None,
-        community_id: Optional[int] = None,
-        saved_only: Optional[bool] = None,
-    ) -> Optional[dict]:
-        """
-        Get user details with various filters.
-
-        Args:
-            person_id (Optional[str], optional): Defaults to None.
-            username (Optional[str], optional): Defaults to None.
-            sort (Optional[CommentSortType], optional): Defaults to None.
-            page (Optional[int], optional): Defaults to None.
-            limit (Optional[int], optional): Defaults to None.
-            community_id (Optional[int], optional): Defaults to None.
-            saved_only (Optional[bool], optional): Defaults to None.
-        Returns:
-            dict: user view
-        """
-        params: dict[str, Any] = {key: value for key, value in locals().items() if value is not None and key != 'self'}
-        return self._requestor.request(Request.GET, "/user", params=params)
+from typing import Any, List, Literal, Optional
+
+from pythorhead.requestor import Request, Requestor
+from pythorhead.types import PostSortType
+
+
+class User:
+    def __init__(self, _requestor: Requestor):
+        self._requestor = _requestor
+
+    def get(
+        self,
+        person_id: Optional[str] = None,
+        username: Optional[str] = None,
+        sort: Optional[PostSortType] = None,
+        page: Optional[int] = None,
+        limit: Optional[int] = None,
+        community_id: Optional[int] = None,
+        saved_only: Optional[bool] = None,
+    ) -> Optional[dict]:
+        """
+        Get user details with various filters.
+
+        Args:
+            person_id (Optional[str], optional): Defaults to None.
+            username (Optional[str], optional): Defaults to None.
+            sort (Optional[CommentSortType], optional): Defaults to None.
+            page (Optional[int], optional): Defaults to None.
+            limit (Optional[int], optional): Defaults to None.
+            community_id (Optional[int], optional): Defaults to None.
+            saved_only (Optional[bool], optional): Defaults to None.
+        Returns:
+            dict: user view
+        """
+        params: dict[str, Any] = {key: value for key, value in locals().items() if value is not None and key != "self"}
+        return self._requestor.api(Request.GET, "/user", params=params)
```

### Comparing `pythorhead-0.7.2/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.8.0/pythorhead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.7.2
+Version: 0.8.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.7.2/pythorhead.egg-info/SOURCES.txt` & `pythorhead-0.8.0/pythorhead.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 requirements.txt
 .github/workflows/pypi.yml
 examples/pm.py
 examples/user.py
 pythorhead/__init__.py
 pythorhead/auth.py
 pythorhead/comment.py
+pythorhead/image.py
 pythorhead/lemmy.py
 pythorhead/post.py
 pythorhead/private_message.py
 pythorhead/requestor.py
 pythorhead/site.py
 pythorhead/user.py
 pythorhead.egg-info/PKG-INFO
```

