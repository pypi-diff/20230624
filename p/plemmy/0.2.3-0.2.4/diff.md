# Comparing `tmp/plemmy-0.2.3.tar.gz` & `tmp/plemmy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.2.3.tar", last modified: Fri Jun 23 19:25:50 2023, max compression
+gzip compressed data, was "plemmy-0.2.4.tar", last modified: Sat Jun 24 16:58:04 2023, max compression
```

## Comparing `plemmy-0.2.3.tar` & `plemmy-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-23 19:25:50.818475 plemmy-0.2.3/
--rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.3/LICENSE
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-23 19:25:50.818292 plemmy-0.2.3/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.3/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-23 19:25:50.817187 plemmy-0.2.3/plemmy/
--rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.3/plemmy/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    70944 2023-06-23 19:23:23.000000 plemmy-0.2.3/plemmy/lemmyhttp.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     2803 2023-06-23 18:44:09.000000 plemmy-0.2.3/plemmy/utils.py
--rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-06-23 19:24:36.000000 plemmy-0.2.3/plemmy/version.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-23 19:25:50.818067 plemmy-0.2.3/plemmy.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/requires.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-06-23 19:25:50.818524 plemmy-0.2.3/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.3/setup.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-24 16:58:04.570548 plemmy-0.2.4/
+-rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.4/LICENSE
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-24 16:58:04.570384 plemmy-0.2.4/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.4/README.md
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-24 16:58:04.569120 plemmy-0.2.4/plemmy/
+-rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.4/plemmy/__init__.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    70949 2023-06-24 16:56:44.000000 plemmy-0.2.4/plemmy/lemmyhttp.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2803 2023-06-23 18:44:09.000000 plemmy-0.2.4/plemmy/utils.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-06-24 16:57:12.000000 plemmy-0.2.4/plemmy/version.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-24 16:58:04.570175 plemmy-0.2.4/plemmy.egg-info/
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/SOURCES.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/dependency_links.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/not-zip-safe
+-rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/requires.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-06-24 16:58:04.000000 plemmy-0.2.4/plemmy.egg-info/top_level.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-06-24 16:58:04.570595 plemmy-0.2.4/setup.cfg
+-rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.4/setup.py
```

### Comparing `plemmy-0.2.3/LICENSE` & `plemmy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.3/PKG-INFO` & `plemmy-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plemmy-0.2.3/README.md` & `plemmy-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.3/plemmy/lemmyhttp.py` & `plemmy-0.2.4/plemmy/lemmyhttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,15 +600,15 @@
 
         Returns:
             requests.Response: result of API call
         """
 
         form = create_form(locals())
         form["auth"] = self.key
-        return put_handler(f"{self._api_url}/post", self._headers, form)
+        return put_handler(f"{self._api_url}/community", self._headers, form)
 
     def edit_custom_emoji(self, alt_text: str, category: str, id: int,
                           image_url: str, keywords: List[str]
                           ) -> requests.Response:
         """ edit_custom_emoji: edits information for custom emoji
 
         Args:
```

### Comparing `plemmy-0.2.3/plemmy/utils.py` & `plemmy-0.2.4/plemmy/utils.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.3/plemmy.egg-info/PKG-INFO` & `plemmy-0.2.4/plemmy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plemmy-0.2.3/setup.py` & `plemmy-0.2.4/setup.py`

 * *Files identical despite different names*

