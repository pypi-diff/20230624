# Comparing `tmp/jmcomic-2.0.6.tar.gz` & `tmp/jmcomic-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.0.6.tar", last modified: Fri Jun 23 06:32:58 2023, max compression
+gzip compressed data, was "jmcomic-2.0.7.tar", last modified: Sat Jun 24 09:47:42 2023, max compression
```

## Comparing `jmcomic-2.0.6.tar` & `jmcomic-2.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:32:58.581547 jmcomic-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-23 06:32:49.000000 jmcomic-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-23 06:32:58.581547 jmcomic-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-23 06:32:49.000000 jmcomic-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 06:32:58.581547 jmcomic-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-23 06:32:49.000000 jmcomic-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:32:58.577546 jmcomic-2.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:32:58.581547 jmcomic-2.0.6/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:32:58.581547 jmcomic-2.0.6/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-23 06:32:58.000000 jmcomic-2.0.6/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-23 06:32:58.000000 jmcomic-2.0.6/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:32:58.000000 jmcomic-2.0.6/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 06:32:58.000000 jmcomic-2.0.6/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 06:32:58.000000 jmcomic-2.0.6/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:42.676393 jmcomic-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-24 09:47:28.000000 jmcomic-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-24 09:47:42.676393 jmcomic-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-24 09:47:28.000000 jmcomic-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 09:47:42.676393 jmcomic-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-24 09:47:28.000000 jmcomic-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:42.672393 jmcomic-2.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:42.672393 jmcomic-2.0.7/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-06-24 09:47:28.000000 jmcomic-2.0.7/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:42.676393 jmcomic-2.0.7/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-24 09:47:42.000000 jmcomic-2.0.7/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-24 09:47:42.000000 jmcomic-2.0.7/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 09:47:42.000000 jmcomic-2.0.7/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 09:47:42.000000 jmcomic-2.0.7/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-24 09:47:42.000000 jmcomic-2.0.7/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.0.6/LICENSE` & `jmcomic-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.6/PKG-INFO` & `jmcomic-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.0.6/README.md` & `jmcomic-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.6/setup.py` & `jmcomic-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.6/src/jmcomic/api.py` & `jmcomic-2.0.7/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.6/src/jmcomic/jm_client_impl.py` & `jmcomic-2.0.7/src/jmcomic/jm_client_impl.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,31 +71,40 @@
 
     # noinspection PyMethodMayBeStatic, PyUnusedLocal
     def before_retry(self, e, kwargs, retry_count, url):
         jm_debug('error', str(e))
 
     def enable_cache(self, debug=False):
         def wrap_func_cache(func_name, cache_dict_name):
+            import common
+            if common.VERSION > '0.4.8':
+                cache = common.cache
+                cache_dict = {}
+                cache_hit_msg = (f'【缓存命中】{cache_dict_name} ' + '→ [{}]') if debug is True else None
+                cache_miss_msg = (f'【缓存缺失】{cache_dict_name} ' + '← [{}]') if debug is True else None
+                cache = cache(
+                    cache_dict=cache_dict,
+                    cache_hit_msg=cache_hit_msg,
+                    cache_miss_msg=cache_miss_msg,
+                )
+                setattr(self, cache_dict_name, cache_dict)
+            else:
+                if sys.version_info < (3, 9):
+                    raise NotImplementedError('不支持启用JmcomicClient缓存。\n'
+                                              '请更新python版本到3.9以上，'
+                                              '或更新commonX: `pip install commonX --upgrade`')
+                import functools
+                cache = functools.cache
+
             if hasattr(self, cache_dict_name):
                 return
 
-            cache_dict = {}
-            setattr(self, cache_dict_name, cache_dict)
-
             # 重载本对象的方法
             func = getattr(self, func_name)
-
-            cache_hit_msg = f'【缓存命中】{cache_dict_name} ' + '→ [{}]' if debug is True else None
-            cache_miss_msg = f'【缓存缺失】{cache_dict_name} ' + '← [{}]' if debug is True else None
-
-            wrap_func = enable_cache(
-                cache_dict=cache_dict,
-                cache_hit_msg=cache_hit_msg,
-                cache_miss_msg=cache_miss_msg,
-            )(func)
+            wrap_func = cache(func)
 
             setattr(self, func_name, wrap_func)
 
         for func in {
             'get_photo_detail',
             'get_album_detail',
             'search_album',
@@ -145,26 +154,28 @@
 
         # 检查 page_arr 和 data_original_domain
         if photo_detail.page_arr is None or photo_detail.data_original_domain is None:
             new = self.get_photo_detail(photo_detail.photo_id, False)
             new.from_album = photo_detail.from_album
             photo_detail.__dict__.update(new.__dict__)
 
-    def search_album(self, search_query, main_tag=0):
+    def search_album(self, search_query, main_tag=0, page=1) -> JmSearchPage:
         params = {
             'main_tag': main_tag,
             'search_query': search_query,
+            'page': page,
         }
 
         resp = self.get_jm_html('/search/photos', params=params, allow_redirects=True)
 
         # 检查是否发生了重定向
         # 因为如果搜索的是禁漫车号，会直接跳转到本子详情页面
         if resp.redirect_count != 0 and '/album/' in resp.url:
-            return JmcomicText.analyse_jm_album_html(resp.text)
+            album = JmcomicText.analyse_jm_album_html(resp.text)
+            return JmSearchPage.wrap_single_album(album)
         else:
             return JmSearchSupport.analyse_jm_search_html(resp.text)
 
     # -- 帐号管理 --
 
     def login(self,
               username,
@@ -280,15 +291,15 @@
             + (f'URL=[{url}]' if url is not None else '')
         )
 
 
 class JmApiClient(AbstractJmClient):
     API_SEARCH = '/search'
 
-    def search_album(self, search_query: str, main_tag=0) -> JmApiResp:
+    def search_album(self, search_query, main_tag=0, page=1) -> JmApiResp:
         """
         model_data: {
           "search_query": "MANA",
           "total": "177",
           "content": [
             {
               "id": "441923",
@@ -308,14 +319,16 @@
           ]
         }
         """
         return self.get(
             self.API_SEARCH,
             params={
                 'search_query': search_query,
+                'main_tag': main_tag,
+                'page': page,
             }
         )
 
     def get(self, url, **kwargs) -> JmApiResp:
         # set headers
         headers, key_ts = self.headers_key_ts
         kwargs.setdefault('headers', headers)
```

### Comparing `jmcomic-2.0.6/src/jmcomic/jm_client_interface.py` & `jmcomic-2.0.7/src/jmcomic/jm_client_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
     def get_photo_detail(self, photo_id, fetch_album=True) -> JmPhotoDetail:
         raise NotImplementedError
 
     def ensure_photo_can_use(self, photo_detail: JmPhotoDetail):
         raise NotImplementedError
 
-    def search_album(self, search_query, main_tag=0) -> Union[JmSearchPage, JmAlbumDetail]:
+    def search_album(self, search_query: str, main_tag: int = 0, page: int = 1) -> JmSearchPage:
         raise NotImplementedError
 
     def of_api_url(self, api_path, domain):
         raise NotImplementedError
 
     def enable_cache(self, debug=False):
         raise NotImplementedError
```

### Comparing `jmcomic-2.0.6/src/jmcomic/jm_config.py` & `jmcomic-2.0.7/src/jmcomic/jm_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,24 +70,26 @@
     @classmethod
     def headers(cls, authority=None):
         return {
             'authority': authority or '18comic.vip',
             'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,'
                       'application/signed-exchange;v=b3;q=0.7',
             'accept-language': 'zh-CN,zh;q=0.9',
+            'cache-control': 'no-cache',
             'referer': 'https://18comic.vip',
-            'sec-ch-ua': '"Google Chrome";v="111", "Not(A:Brand";v="8", "Chromium";v="111"',
+            'pragma': 'no-cache',
+            'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'sec-fetch-dest': 'document',
             'sec-fetch-mode': 'navigate',
-            'sec-fetch-site': 'same-origin',
+            'sec-fetch-site': 'none',
             'sec-fetch-user': '?1',
             'upgrade-insecure-requests': '1',
-            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 '
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 '
                           'Safari/537.36',
         }
 
     # noinspection PyUnusedLocal
     @classmethod
     def jm_debug(cls, topic: str, msg: str):
         if cls.enable_jm_debug is True:
```

### Comparing `jmcomic-2.0.6/src/jmcomic/jm_entity.py` & `jmcomic-2.0.7/src/jmcomic/jm_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,16 +302,37 @@
 
     def __iter__(self) -> Generator[JmPhotoDetail, Any, None]:
         return super().__iter__()
 
 
 class JmSearchPage(IterableEntity):
 
-    def __init__(self, album_info_list):
+    def __init__(self, album_info_list: List[Tuple[str, str, StrNone, StrNone, List[str]]]):
         # (album_id, title, category_none, label_sub_none, tag_list)
-        self.album_info_list: List[Tuple[str, str, StrNone, StrNone, List[str]]] = album_info_list
+        self.album_info_list = album_info_list
 
     def __len__(self):
         return len(self.album_info_list)
 
     def __getitem__(self, item):
         return self.album_info_list[item][0:2]
+
+    @property
+    def single_album(self) -> JmAlbumDetail:
+        return getattr(self, 'album')
+
+    @classmethod
+    def wrap_single_album(cls, album: JmAlbumDetail) -> 'JmSearchPage':
+        # ('462257', '[無邪気漢化組] [きょくちょ] 楓と鈴 4.5', '短篇', '漢化', [])
+        # (album_id, title, category_none, label_sub_none, tag_list)
+
+        album_info = (
+            album.album_id,
+            album.title,
+            None,
+            None,
+            album.keywords,
+        )
+        obj = JmSearchPage([album_info])
+
+        setattr(obj, 'album', album)
+        return obj
```

### Comparing `jmcomic-2.0.6/src/jmcomic/jm_option.py` & `jmcomic-2.0.7/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.6/src/jmcomic/jm_toolkit.py` & `jmcomic-2.0.7/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.6/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.0.7/src/jmcomic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

