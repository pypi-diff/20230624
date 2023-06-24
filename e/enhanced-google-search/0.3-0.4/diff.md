# Comparing `tmp/enhanced_google_search-0.3.tar.gz` & `tmp/enhanced_google_search-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhanced_google_search-0.3.tar", last modified: Sun May 21 13:50:20 2023, max compression
+gzip compressed data, was "enhanced_google_search-0.4.tar", last modified: Sat Jun 24 19:29:17 2023, max compression
```

## Comparing `enhanced_google_search-0.3.tar` & `enhanced_google_search-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 13:50:20.579959 enhanced_google_search-0.3/
--rw-rw-rw-   0        0        0     1170 2023-05-21 13:50:20.578961 enhanced_google_search-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      843 2023-05-21 13:48:48.000000 enhanced_google_search-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 13:50:20.579959 enhanced_google_search-0.3/setup.cfg
--rw-rw-rw-   0        0        0      528 2023-05-21 13:49:17.000000 enhanced_google_search-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 13:50:20.541860 enhanced_google_search-0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 13:50:20.574973 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/
--rw-rw-rw-   0        0        0     1170 2023-05-21 13:50:19.000000 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-21 13:50:20.000000 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 13:50:19.000000 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-21 13:50:19.000000 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-21 13:50:19.000000 enhanced_google_search-0.3/src/enhanced_google_search.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1159 2023-05-19 13:17:04.000000 enhanced_google_search-0.3/src/enhanced_google_search.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:29:17.723999 enhanced_google_search-0.4/
+-rw-rw-rw-   0        0        0     1173 2023-06-24 19:29:17.723999 enhanced_google_search-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      846 2023-06-24 19:26:36.000000 enhanced_google_search-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 19:29:17.723999 enhanced_google_search-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      528 2023-06-24 19:26:40.000000 enhanced_google_search-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 19:29:17.698002 enhanced_google_search-0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 19:29:17.722003 enhanced_google_search-0.4/src/enhanced_google_search.egg-info/
+-rw-rw-rw-   0        0        0     1173 2023-06-24 19:29:17.000000 enhanced_google_search-0.4/src/enhanced_google_search.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-06-24 19:29:17.000000 enhanced_google_search-0.4/src/enhanced_google_search.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 19:29:17.000000 enhanced_google_search-0.4/src/enhanced_google_search.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-24 19:29:17.000000 enhanced_google_search-0.4/src/enhanced_google_search.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-24 19:29:17.000000 enhanced_google_search-0.4/src/enhanced_google_search.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1182 2023-06-24 19:26:55.000000 enhanced_google_search-0.4/src/enhanced_google_search.py
```

### Comparing `enhanced_google_search-0.3/PKG-INFO` & `enhanced_google_search-0.4/src/enhanced_google_search.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: enhanced_google_search
-Version: 0.3
+Name: enhanced-google-search
+Version: 0.4
 Summary: An enhanced google search library
 Home-page: https://github.com/K-K-L-L/google_search_py
 Author: KKLL
 Keywords: googlesearch.py,enhanced_google_search,python google search,google search pypi,google api
 Description-Content-Type: text/markdown
 
 # enhanced_google_search
@@ -43,8 +43,8 @@
 ```py
 from enhanced_google_search import search
 
 results = search("Python", num = 2) # Number of results
 print(results)
 ```
 
-**Discord: KKLL#9777**
+**Discord: imacoolhuman**
```

### Comparing `enhanced_google_search-0.3/README.md` & `enhanced_google_search-0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 ```py
 from enhanced_google_search import search
 
 results = search("Python", num = 2) # Number of results
 print(results)
 ```
 
-**Discord: KKLL#9777**
+**Discord: imacoolhuman**
```

### Comparing `enhanced_google_search-0.3/setup.py` & `enhanced_google_search-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="enhanced_google_search",
-    version="0.3",
+    version="0.4",
     description="An enhanced google search library",
     author="KKLL",
     url="https://github.com/K-K-L-L/google_search_py",
     long_description=str(open("README.md", "r", encoding="utf-8").read()),
     long_description_content_type="text/markdown",
     keywords="googlesearch.py, enhanced_google_search, python google search, google search pypi, google api",
     package_dir={"": "src"},
```

### Comparing `enhanced_google_search-0.3/src/enhanced_google_search.egg-info/PKG-INFO` & `enhanced_google_search-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: enhanced-google-search
-Version: 0.3
+Name: enhanced_google_search
+Version: 0.4
 Summary: An enhanced google search library
 Home-page: https://github.com/K-K-L-L/google_search_py
 Author: KKLL
 Keywords: googlesearch.py,enhanced_google_search,python google search,google search pypi,google api
 Description-Content-Type: text/markdown
 
 # enhanced_google_search
@@ -43,8 +43,8 @@
 ```py
 from enhanced_google_search import search
 
 results = search("Python", num = 2) # Number of results
 print(results)
 ```
 
-**Discord: KKLL#9777**
+**Discord: imacoolhuman**
```

### Comparing `enhanced_google_search-0.3/src/enhanced_google_search.py` & `enhanced_google_search-0.4/src/enhanced_google_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Union, List, Dict
 import httpx
 import re
 
 
-def search(query: str, lang: str = "en", num: int = 10, headers: Union[Dict[str, str], None] ={"User-Agent":
+def search(query: str, lang: str = "en", num: int = 10, headers: Union[Dict[str, str], None] = {"User-Agent":
                 "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0"}) -> List[Union[dict, str]]:
 
     results: List[Union[dict, str]] = []
 
     base_url: str = f"https://www.google.com/search?q={query}&num=30&hl={lang}"
 
     page: str = httpx.get(base_url, headers=headers).text
 
     web: str = '<div class="yuRUbf"><a href="(.*?)" data-jsarwt=".*?" ' \
-                   'data-usg=".*?" data-ved=".*?"><br><h3 class="LC20lb MBeuO DKV0Md">(.*?)</h3>.*?' \
-                   '<div class="VwiC3b yXK7lf MUxGbd yDYNvb lyLwlc lEBKkf" style="-webkit-line-clamp:2">' \
-                   '<span>(.*?)</span></div>'
+               'data-usg=".*?" data-ved=".*?"><br><h3 class="LC20lb MBeuO DKV0Md">(.*?)</h3>.*?' \
+               '<div class="VwiC3b yXK7lf MUxGbd yDYNvb lyLwlc lEBKkf" style="-webkit-line-clamp:2">' \
+               '<span>(.*?)</span></div>'
 
     for i in re.findall(pattern=web, string=page):
+        url = i[0].split('" ')[0]
         results.append({
-            "url": i[0],
+            "url": url,
             "title": i[1].replace('<span dir=\"ltr\">', "").replace("</span>", ""),
             "description": re.sub('<[^<>]+>', '', i[2])
         })
 
-
-    return results[:num if len(results) > num else len(results)]
+    return results[:num if len(results) > num else len(results)]
```

#### html2text {}

```diff
@@ -4,11 +4,11 @@
 20100101 Firefox/108.0"}) -> List[Union[dict, str]]: results: List[Union[dict,
 str]] = [] base_url: str = f"https://www.google.com/search?q={query}&num=30&hl=
 {lang}" page: str = httpx.get(base_url, headers=headers).text web: str = '
  \ 'data-usg=".*?" data-ved=".*?">
 **** (.*?) ****
 .*?' \ '
 ' \ '(.*?)
-' for i in re.findall(pattern=web, string=page): results.append({ "url": i[0],
-"title": i[1].replace('', "").replace("", ""), "description": re.sub('<
-[^<>]+>', '', i[2]) }) return results[:num if len(results) > num else len
-(results)]
+' for i in re.findall(pattern=web, string=page): url = i[0].split('" ')[0]
+results.append({ "url": url, "title": i[1].replace('', "").replace("", ""),
+"description": re.sub('<[^<>]+>', '', i[2]) }) return results[:num if len
+(results) > num else len(results)]
```

