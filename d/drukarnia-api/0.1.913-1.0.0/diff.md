# Comparing `tmp/drukarnia-api-0.1.913.tar.gz` & `tmp/drukarnia-api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drukarnia-api-0.1.913.tar", last modified: Wed Jun 21 18:56:04 2023, max compression
+gzip compressed data, was "drukarnia-api-1.0.0.tar", last modified: Sat Jun 24 15:57:15 2023, max compression
```

## Comparing `drukarnia-api-0.1.913.tar` & `drukarnia-api-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/drukarnia_api/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/article.py
--rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/author.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/drukarnia_api/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/shortcuts/class_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/drukarnia_api/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:56:04.379361 drukarnia-api-0.1.913/drukarnia_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-21 18:56:04.000000 drukarnia-api-0.1.913/drukarnia_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-21 18:56:04.000000 drukarnia-api-0.1.913/drukarnia_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:56:04.000000 drukarnia-api-0.1.913/drukarnia_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 18:56:04.000000 drukarnia-api-0.1.913/drukarnia_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 18:56:04.000000 drukarnia-api-0.1.913/drukarnia_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:56:04.383361 drukarnia-api-0.1.913/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-21 18:55:54.000000 drukarnia-api-0.1.913/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/drukarnia_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/article.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/author.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/drukarnia_api/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/shortcuts/class_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/drukarnia_api/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/drukarnia_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-24 15:57:15.000000 drukarnia-api-1.0.0/drukarnia_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-24 15:57:15.000000 drukarnia-api-1.0.0/drukarnia_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:57:15.000000 drukarnia-api-1.0.0/drukarnia_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-24 15:57:15.000000 drukarnia-api-1.0.0/drukarnia_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 15:57:15.000000 drukarnia-api-1.0.0/drukarnia_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 15:57:15.312033 drukarnia-api-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-24 15:57:06.000000 drukarnia-api-1.0.0/setup.py
```

### Comparing `drukarnia-api-0.1.913/LICENSE` & `drukarnia-api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.913/PKG-INFO` & `drukarnia-api-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.913
+Version: 1.0.0
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `drukarnia-api-0.1.913/README.md` & `drukarnia-api-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.913/drukarnia_api/article.py` & `drukarnia-api-1.0.0/drukarnia_api/article.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from datetime import datetime
 from warnings import warn
 from aiohttp import ClientSession
 
 from drukarnia_api.drukarnia_base import DrukarniaElement
-from drukarnia_api.shortcuts import data2authors, data2articles, data2tags
+from drukarnia_api.shortcuts import data2authors, data2articles, data2tags, data2comments
 
 from typing import TYPE_CHECKING, Tuple, Dict, List
 
 if TYPE_CHECKING:  # always False, used for type hints
     from drukarnia_api.author import Author
     from drukarnia_api.tag import Tag
+    from drukarnia_api.comment import Comment
 
 
 class Article(DrukarniaElement):
     def __init__(self, slug: str = None, article_id: str = None, *args, **kwargs):
         """
         Initializes an Article object with the given slug and article ID.
         """
@@ -30,56 +31,14 @@
 
         posted_comment_id = await self.request('post', '/api/articles/{_id}/comments'.format(_id=self.article_id),
                                                data={'comment': comment_text}, output='read')
         return str(posted_comment_id)
 
     @DrukarniaElement._control_attr('article_id')
     @DrukarniaElement._is_authenticated
-    async def reply2comment(self, comment_text: str, comment_id: str, root_comment: str,
-                            root_comment_owner: str, reply2user: str) -> str:
-        """
-        Posts a reply to a comment and returns the ID of the new comment.
-        """
-
-        new_comment_id = await self.request('post',
-                                            f'/api/articles/{self.article_id}/comments/{comment_id}/replies',
-                                            data={
-                                                  "comment": comment_text, "replyToComment": comment_id,
-                                                  "rootComment": root_comment,
-                                                  "rootCommentOwner": root_comment_owner, "replyToUser": reply2user
-                                                },
-                                            output='read'
-                                            )
-
-        return new_comment_id.decode('utf-8')
-
-    @DrukarniaElement._control_attr('article_id')
-    @DrukarniaElement._is_authenticated
-    async def delete_comment(self, comment_id: str) -> None:
-        """
-        Deletes a comment from the article.
-        """
-
-        await self.request('delete', f'/api/articles/{self.article_id}/comments/{comment_id}')
-
-    @DrukarniaElement._control_attr('article_id')
-    @DrukarniaElement._is_authenticated
-    async def like_comment(self, comment_id: str, unlike: bool = False) -> None:
-        """
-        Likes or unlikes a comment based on the 'delete' parameter.
-        """
-
-        if unlike:
-            await self.request('delete', f'/api/articles/{self.article_id}/comments/{comment_id}/likes')
-
-        else:
-            await self.request('post', f'/api/articles/{self.article_id}/comments/{comment_id}/likes')
-
-    @DrukarniaElement._control_attr('article_id')
-    @DrukarniaElement._is_authenticated
     async def like_article(self, n_likes: int) -> None:
         """
         Likes the article with the specified number of likes.
         """
 
         if not (0 <= n_likes <= 10):
             raise ValueError('Number of likes must be greater or equal to zero and lower or equal to ten')
@@ -125,19 +84,19 @@
         owner = self._access_data('owner', None)
         if owner is None:
             return None
 
         return await data2authors([owner], self.session)
 
     @property
-    def comments(self) -> List:
+    async def comments(self) -> Tuple['Comment']:
         """
         Retrieves the comments of the article.
         """
-        return self._access_data('comments', [])
+        return await data2comments(self._access_data('comments', []), self.session)
 
     @property
     async def recommended_articles(self) -> Tuple['Article']:
         """
         Retrieves the recommended articles related to the article.
         """
         return await data2articles(self._access_data('recommendedArticles', []), self.session)
```

### Comparing `drukarnia-api-0.1.913/drukarnia_api/author.py` & `drukarnia-api-1.0.0/drukarnia_api/author.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,36 +144,14 @@
         if unsubscribe:
             await self.request('delete', f'/api/relationships/subscribe/{author_id}')
             return None
 
         await self.request('post', f'/api/relationships/subscribe/{author_id}')
 
     @DrukarniaElement._is_authenticated
-    async def subscribe_tag(self, tag_id: str, unsubscribe: bool = False) -> None:
-        """
-        Subscribe or unsubscribe to/from a tag.
-        """
-        if unsubscribe:
-            await self.request('delete', f'/api/preferences/tags/{tag_id}')
-            return None
-
-        await self.request('put', f'/api/preferences/tags/{tag_id}')
-
-    @DrukarniaElement._is_authenticated
-    async def block_tag(self, tag_id: str, unblock: bool = False) -> None:
-        """
-        Block or unblock an author.
-        """
-        if unblock:
-            await self.request('put', f'/api/preferences/tags/{tag_id}/block', data={"isBlocked": False})
-            return None
-
-        await self.request('put', f'/api/preferences/tags/{tag_id}/block', data={"isBlocked": True})
-
-    @DrukarniaElement._is_authenticated
     async def block_author(self, author_id: str, unblock: bool = False) -> None:
         """
         Block or unblock an author.
         """
         if unblock:
             await self.request('patch', f'/api/relationships/block/{author_id}')
             return None
```

### Comparing `drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/connection.py` & `drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Callable, Dict, Generator, Tuple, List, Iterable
 import inspect
 from drukarnia_api.drukarnia_base.exceptions import DrukarniaAPIError
 
 
 async def _from_response(response: ClientResponse, output: str or List[str] or None) -> Any:
 
-    if not (200 <= int(response.status) < 300):
+    if int(response.status) not in [200, 201]:
         data = await response.json()
         raise DrukarniaAPIError(data['message'], response.status,
                                 response.request_info.method, str(response.request_info.url))
 
     if isinstance(output, str):
         data = await _from_response(response, [output])
         return data[0]
```

### Comparing `drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/element.py` & `drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/element.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.913/drukarnia_api/drukarnia_base/exceptions.py` & `drukarnia-api-1.0.0/drukarnia_api/drukarnia_base/exceptions.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.913/drukarnia_api/search.py` & `drukarnia-api-1.0.0/drukarnia_api/search.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.913/drukarnia_api/tag.py` & `drukarnia-api-1.0.0/drukarnia_api/tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,14 +44,38 @@
         tags = await self.request('get', f'/api/articles/tags/{self.tag_id}/related?page=1', output='json')
         if create_tags:
             tags = await data2tags(tags, self.session)
 
         return tags
 
     @DrukarniaElement._control_attr('tag_id')
+    @DrukarniaElement._is_authenticated
+    async def subscribe_tag(self, unsubscribe: bool = False) -> None:
+        """
+        Subscribe or unsubscribe to/from a tag.
+        """
+        if unsubscribe:
+            await self.request('delete', f'/api/preferences/tags/{self.tag_id}')
+            return None
+
+        await self.request('put', f'/api/preferences/tags/{self.tag_id}')
+
+    @DrukarniaElement._control_attr('tag_id')
+    @DrukarniaElement._is_authenticated
+    async def block_tag(self, unblock: bool = False) -> None:
+        """
+        Block or unblock an author.
+        """
+        if unblock:
+            await self.request('put', f'/api/preferences/tags/{self.tag_id}/block', data={"isBlocked": False})
+            return None
+
+        await self.request('put', f'/api/preferences/tags/{self.tag_id}/block', data={"isBlocked": True})
+
+    @DrukarniaElement._control_attr('tag_id')
     async def related_authors(self, create_tags: bool = True,) -> Tuple['Author'] or Tuple[Dict]:
         """
         Get the followers of the author.
         """
 
         # Make a request to get the followers of the author
         authors = await self.request('get', f'/api/users/tags/{self.tag_id}/related', output='json')
```

### Comparing `drukarnia-api-0.1.913/drukarnia_api.egg-info/PKG-INFO` & `drukarnia-api-1.0.0/drukarnia_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.913
+Version: 1.0.0
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `drukarnia-api-0.1.913/drukarnia_api.egg-info/SOURCES.txt` & `drukarnia-api-1.0.0/drukarnia_api.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 drukarnia_api/__init__.py
 drukarnia_api/article.py
 drukarnia_api/author.py
+drukarnia_api/comment.py
 drukarnia_api/search.py
 drukarnia_api/tag.py
 drukarnia_api.egg-info/PKG-INFO
 drukarnia_api.egg-info/SOURCES.txt
 drukarnia_api.egg-info/dependency_links.txt
 drukarnia_api.egg-info/requires.txt
 drukarnia_api.egg-info/top_level.txt
```

### Comparing `drukarnia-api-0.1.913/setup.py` & `drukarnia-api-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get requirements
 with open(path.join(HERE, 'requirements.txt')) as f:
     requirements = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="drukarnia-api",
-    version="0.1.913",
+    version="1.0.0",
     description="wrapper for the Drukarnia API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/androu-sys/drukarnia-api",
     author="Andrii Herts",
     license="MIT",
     classifiers=[
```

