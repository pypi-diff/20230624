# Comparing `tmp/morss-20221213.2216.tar.gz` & `tmp/morss-20230623.2301.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morss-20221213.2216.tar", last modified: Tue Dec 13 22:16:33 2022, max compression
+gzip compressed data, was "morss-20230623.2301.tar", last modified: Fri Jun 23 23:01:14 2023, max compression
```

## Comparing `morss-20221213.2216.tar` & `morss-20230623.2301.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 22:16:32.190688 morss-20221213.2216/
--rw-r--r--   0 root         (0) root         (0)    34523 2022-12-13 22:13:18.000000 morss-20221213.2216/LICENSE
--rw-r--r--   0 root         (0) root         (0)    17662 2022-12-13 22:16:31.874024 morss-20221213.2216/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17225 2022-12-13 22:13:18.000000 morss-20221213.2216/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 22:16:30.810697 morss-20221213.2216/morss/
--rw-r--r--   0 root         (0) root         (0)      869 2022-12-13 22:13:18.000000 morss-20221213.2216/morss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1352 2022-12-13 22:13:18.000000 morss-20221213.2216/morss/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3822 2022-12-13 22:13:18.000000 morss-20221213.2216/morss/caching.py
--rw-r--r--   0 root         (0) root         (0)     4107 2022-12-13 22:13:18.000000 morss-20221213.2216/morss/cli.py
--rw-r--r--   0 root         (0) root         (0)    22734 2022-12-13 22:13:18.000000 morss-20221213.2216/morss/crawler.py
--rw-r--r--   0 root         (0) root         (0)     2938 2022-12-13 22:13:18.000000 morss-20221213.2216/morss/feedify.ini
--rw-r--r--   0 root         (0) root         (0)    23557 2022-12-13 22:13:18.000000 morss-20221213.2216/morss/feeds.py
--rw-r--r--   0 root         (0) root         (0)    12373 2022-12-13 22:13:18.000000 morss-20221213.2216/morss/morss.py
--rw-r--r--   0 root         (0) root         (0)    11496 2022-12-13 22:13:18.000000 morss-20221213.2216/morss/readabilite.py
--rw-r--r--   0 root         (0) root         (0)     1713 2022-12-13 22:13:18.000000 morss-20221213.2216/morss/util.py
--rw-r--r--   0 root         (0) root         (0)     8484 2022-12-13 22:13:18.000000 morss-20221213.2216/morss/wsgi.py
--rwxr-xr-x   0 root         (0) root         (0)      822 2022-12-13 22:13:18.000000 morss-20221213.2216/morss-helper
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 22:16:31.514026 morss-20221213.2216/morss.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17662 2022-12-13 22:16:18.000000 morss-20221213.2216/morss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      437 2022-12-13 22:16:19.000000 morss-20221213.2216/morss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 22:16:18.000000 morss-20221213.2216/morss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2022-12-13 22:16:18.000000 morss-20221213.2216/morss.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      111 2022-12-13 22:16:18.000000 morss-20221213.2216/morss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-12-13 22:16:18.000000 morss-20221213.2216/morss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-13 22:16:32.190688 morss-20221213.2216/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1240 2022-12-13 22:13:18.000000 morss-20221213.2216/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-13 22:16:31.810691 morss-20221213.2216/www/
--rw-r--r--   0 root         (0) root         (0)     1154 2022-12-13 22:13:18.000000 morss-20221213.2216/www/index.html
--rw-r--r--   0 root         (0) root         (0)      735 2022-12-13 22:13:18.000000 morss-20221213.2216/www/logo.svg
--rw-r--r--   0 root         (0) root         (0)     8258 2022-12-13 22:13:18.000000 morss-20221213.2216/www/sheet.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:14.315560 morss-20230623.2301/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-06-23 23:01:02.000000 morss-20230623.2301/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    17771 2023-06-23 23:01:14.315560 morss-20230623.2301/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17334 2023-06-23 23:01:02.000000 morss-20230623.2301/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:14.311560 morss-20230623.2301/morss/
+-rw-r--r--   0 root         (0) root         (0)      869 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/caching.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/cli.py
+-rw-r--r--   0 root         (0) root         (0)    22734 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/crawler.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/feedify.ini
+-rw-r--r--   0 root         (0) root         (0)    23557 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/feeds.py
+-rw-r--r--   0 root         (0) root         (0)    12442 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/morss.py
+-rw-r--r--   0 root         (0) root         (0)    11496 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/readabilite.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/util.py
+-rw-r--r--   0 root         (0) root         (0)     8484 2023-06-23 23:01:02.000000 morss-20230623.2301/morss/wsgi.py
+-rwxr-xr-x   0 root         (0) root         (0)      822 2023-06-23 23:01:02.000000 morss-20230623.2301/morss-helper
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:14.315560 morss-20230623.2301/morss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17771 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-23 23:01:14.000000 morss-20230623.2301/morss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 23:01:14.315560 morss-20230623.2301/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-06-23 23:01:02.000000 morss-20230623.2301/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:14.315560 morss-20230623.2301/tests/
+-rw-r--r--   0 root         (0) root         (0)     3516 2023-06-23 23:01:02.000000 morss-20230623.2301/tests/test_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-06-23 23:01:02.000000 morss-20230623.2301/tests/test_feeds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 23:01:14.315560 morss-20230623.2301/www/
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-06-23 23:01:02.000000 morss-20230623.2301/www/index.html
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-23 23:01:02.000000 morss-20230623.2301/www/logo.svg
+-rw-r--r--   0 root         (0) root         (0)     8258 2023-06-23 23:01:02.000000 morss-20230623.2301/www/sheet.xsl
```

### Comparing `morss-20221213.2216/LICENSE` & `morss-20230623.2301/LICENSE`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/PKG-INFO` & `morss-20230623.2301/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morss
-Version: 20221213.2216
+Version: 20230623.2301
 Summary: Get full-text RSS feeds
 Home-page: http://morss.it/
 Author: pictuga
 Author-email: contact@pictuga.com
 License: AGPL v3
 Project-URL: Source, https://git.pictuga.com/pictuga/morss
 Project-URL: Bug Tracker, https://github.com/pictuga/morss/issues
@@ -407,16 +407,16 @@
 
 ```
 usage: morss [-h] [--post STRING] [--xpath XPATH]
              [--format {rss,json,html,csv}] [--search STRING] [--clip]
              [--indent] [--cache] [--force] [--proxy]
              [--order {first,last,newest,oldest}] [--firstlink] [--resolve]
              [--items XPATH] [--item_link XPATH] [--item_title XPATH]
-             [--item_content XPATH] [--item_time XPATH] [--nolink] [--noref]
-             [--silent]
+             [--item_content XPATH] [--item_time XPATH]
+             [--mode {xml,html,json}] [--nolink] [--noref] [--silent]
              url
 
 Get full-text RSS feeds
 
 positional arguments:
   url                   feed url
 
@@ -452,14 +452,16 @@
                         xpath rule to match all the RSS entries
   --item_link XPATH     xpath rule relative to items to point to the entry's
                         link
   --item_title XPATH    entry's title
   --item_content XPATH  entry's content
   --item_time XPATH     entry's date & time (accepts a wide range of time
                         formats)
+  --mode {xml,html,json}
+                        parser to use for the custom feeds
 
 misc:
   --nolink              drop links, but keeps links' inner text
   --noref               drop items' link
   --silent              don't output the final RSS (useless on its own, but
                         can be nice when debugging)
```

### Comparing `morss-20221213.2216/README.md` & `morss-20230623.2301/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -391,16 +391,16 @@
 
 ```
 usage: morss [-h] [--post STRING] [--xpath XPATH]
              [--format {rss,json,html,csv}] [--search STRING] [--clip]
              [--indent] [--cache] [--force] [--proxy]
              [--order {first,last,newest,oldest}] [--firstlink] [--resolve]
              [--items XPATH] [--item_link XPATH] [--item_title XPATH]
-             [--item_content XPATH] [--item_time XPATH] [--nolink] [--noref]
-             [--silent]
+             [--item_content XPATH] [--item_time XPATH]
+             [--mode {xml,html,json}] [--nolink] [--noref] [--silent]
              url
 
 Get full-text RSS feeds
 
 positional arguments:
   url                   feed url
 
@@ -436,14 +436,16 @@
                         xpath rule to match all the RSS entries
   --item_link XPATH     xpath rule relative to items to point to the entry's
                         link
   --item_title XPATH    entry's title
   --item_content XPATH  entry's content
   --item_time XPATH     entry's date & time (accepts a wide range of time
                         formats)
+  --mode {xml,html,json}
+                        parser to use for the custom feeds
 
 misc:
   --nolink              drop links, but keeps links' inner text
   --noref               drop items' link
   --silent              don't output the final RSS (useless on its own, but
                         can be nice when debugging)
```

### Comparing `morss-20221213.2216/morss/__init__.py` & `morss-20230623.2301/morss/__init__.py`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/morss/__main__.py` & `morss-20230623.2301/morss/__main__.py`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/morss/caching.py` & `morss-20230623.2301/morss/caching.py`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/morss/cli.py` & `morss-20230623.2301/morss/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
     group = parser.add_argument_group('custom feeds')
     group.add_argument('--items', action='store', type=str, metavar='XPATH', help='(mandatory to activate the custom feeds function) xpath rule to match all the RSS entries')
     group.add_argument('--item_link', action='store', type=str, metavar='XPATH', help='xpath rule relative to items to point to the entry\'s link')
     group.add_argument('--item_title', action='store', type=str, metavar='XPATH', help='entry\'s title')
     group.add_argument('--item_content', action='store', type=str, metavar='XPATH', help='entry\'s content')
     group.add_argument('--item_time', action='store', type=str, metavar='XPATH', help='entry\'s date & time (accepts a wide range of time formats)')
+    group.add_argument('--mode', default=None, choices=('xml', 'html', 'json'), help='parser to use for the custom feeds')
 
     group = parser.add_argument_group('misc')
     group.add_argument('--nolink', action='store_true', help='drop links, but keeps links\' inner text')
     group.add_argument('--noref', action='store_true', help='drop items\' link')
     group.add_argument('--silent', action='store_true', help='don\'t output the final RSS (useless on its own, but can be nice when debugging)')
 
     options = Options(vars(parser.parse_args()))
```

### Comparing `morss-20221213.2216/morss/crawler.py` & `morss-20230623.2301/morss/crawler.py`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/morss/feedify.ini` & `morss-20230623.2301/morss/feedify.ini`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/morss/feeds.py` & `morss-20230623.2301/morss/feeds.py`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/morss/morss.py` & `morss-20230623.2301/morss/morss.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,17 @@
 
     if options.items:
         # using custom rules
         ruleset = {}
 
         ruleset['items'] = options.items
 
+        if options.mode:
+            ruleset['mode'] = options.mode
+
         ruleset['title'] = options.get('title', '//head/title')
         ruleset['desc'] = options.get('desc', '//head/meta[@name="description"]/@content')
 
         ruleset['item_title'] = options.get('item_title', '.')
         ruleset['item_link'] = options.get('item_link', '(.|.//a|ancestor::a)/@href')
 
         if options.item_content:
```

### Comparing `morss-20221213.2216/morss/readabilite.py` & `morss-20230623.2301/morss/readabilite.py`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/morss/util.py` & `morss-20230623.2301/morss/util.py`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/morss/wsgi.py` & `morss-20230623.2301/morss/wsgi.py`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/morss-helper` & `morss-20230623.2301/morss-helper`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/morss.egg-info/PKG-INFO` & `morss-20230623.2301/morss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morss
-Version: 20221213.2216
+Version: 20230623.2301
 Summary: Get full-text RSS feeds
 Home-page: http://morss.it/
 Author: pictuga
 Author-email: contact@pictuga.com
 License: AGPL v3
 Project-URL: Source, https://git.pictuga.com/pictuga/morss
 Project-URL: Bug Tracker, https://github.com/pictuga/morss/issues
@@ -407,16 +407,16 @@
 
 ```
 usage: morss [-h] [--post STRING] [--xpath XPATH]
              [--format {rss,json,html,csv}] [--search STRING] [--clip]
              [--indent] [--cache] [--force] [--proxy]
              [--order {first,last,newest,oldest}] [--firstlink] [--resolve]
              [--items XPATH] [--item_link XPATH] [--item_title XPATH]
-             [--item_content XPATH] [--item_time XPATH] [--nolink] [--noref]
-             [--silent]
+             [--item_content XPATH] [--item_time XPATH]
+             [--mode {xml,html,json}] [--nolink] [--noref] [--silent]
              url
 
 Get full-text RSS feeds
 
 positional arguments:
   url                   feed url
 
@@ -452,14 +452,16 @@
                         xpath rule to match all the RSS entries
   --item_link XPATH     xpath rule relative to items to point to the entry's
                         link
   --item_title XPATH    entry's title
   --item_content XPATH  entry's content
   --item_time XPATH     entry's date & time (accepts a wide range of time
                         formats)
+  --mode {xml,html,json}
+                        parser to use for the custom feeds
 
 misc:
   --nolink              drop links, but keeps links' inner text
   --noref               drop items' link
   --silent              don't output the final RSS (useless on its own, but
                         can be nice when debugging)
```

### Comparing `morss-20221213.2216/setup.py` & `morss-20230623.2301/setup.py`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/www/index.html` & `morss-20230623.2301/www/index.html`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/www/logo.svg` & `morss-20230623.2301/www/logo.svg`

 * *Files identical despite different names*

### Comparing `morss-20221213.2216/www/sheet.xsl` & `morss-20230623.2301/www/sheet.xsl`

 * *Files identical despite different names*

