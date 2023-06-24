# Comparing `tmp/meo-0.0.8.tar.gz` & `tmp/meo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meo-0.0.8.tar", last modified: Wed Dec 21 05:23:52 2022, max compression
+gzip compressed data, was "meo-0.1.0.tar", last modified: Sat Jun 24 11:34:12 2023, max compression
```

## Comparing `meo-0.0.8.tar` & `meo-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-12-21 05:23:52.344956 meo-0.0.8/
--rw-rw-rw-   0        0        0     1087 2022-07-09 19:46:32.000000 meo-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      755 2022-12-21 05:23:52.343952 meo-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      338 2022-08-16 15:30:42.000000 meo-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-12-21 05:23:52.322960 meo-0.0.8/meo/
--rw-rw-rw-   0        0        0      126 2022-10-02 14:16:38.000000 meo-0.0.8/meo/__init__.py
--rw-rw-rw-   0        0        0      311 2022-10-02 14:16:14.000000 meo-0.0.8/meo/__version__.py
--rw-rw-rw-   0        0        0     1545 2022-12-21 05:23:29.000000 meo-0.0.8/meo/data.py
--rw-rw-rw-   0        0        0      591 2022-07-15 17:59:09.000000 meo-0.0.8/meo/flask.py
-drwxrwxrwx   0        0        0        0 2022-12-21 05:23:52.338960 meo-0.0.8/meo/math/
--rw-rw-rw-   0        0        0      112 2022-09-13 12:34:16.000000 meo-0.0.8/meo/math/__init__.py
--rw-rw-rw-   0        0        0      836 2022-07-15 17:46:05.000000 meo-0.0.8/meo/net.py
--rw-rw-rw-   0        0        0     2302 2022-09-12 03:16:17.000000 meo-0.0.8/meo/screen.py
-drwxrwxrwx   0        0        0        0 2022-12-21 05:23:52.340957 meo-0.0.8/meo/sound/
--rw-rw-rw-   0        0        0     1022 2022-08-12 18:57:30.000000 meo-0.0.8/meo/sound/__init__.py
--rw-rw-rw-   0        0        0      175 2022-09-13 11:42:12.000000 meo-0.0.8/meo/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-21 05:23:52.335963 meo-0.0.8/meo.egg-info/
--rw-rw-rw-   0        0        0      755 2022-12-21 05:23:52.000000 meo-0.0.8/meo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2022-12-21 05:23:52.000000 meo-0.0.8/meo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-21 05:23:52.000000 meo-0.0.8/meo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2022-12-21 05:23:52.000000 meo-0.0.8/meo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-21 05:23:52.344956 meo-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1304 2022-08-12 19:10:56.000000 meo-0.0.8/setup.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/
+-rw-r--r--   0 meo       (1000) meo       (1000)     1066 2023-06-24 09:52:08.000000 meo-0.1.0/LICENSE
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-24 11:34:12.412438 meo-0.1.0/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      317 2023-06-24 09:52:08.000000 meo-0.1.0/README.md
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/meo/
+-rw-r--r--   0 meo       (1000) meo       (1000)      127 2023-06-24 10:23:38.000000 meo-0.1.0/meo/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      300 2023-06-24 11:31:33.000000 meo-0.1.0/meo/__version__.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/meo/crack/
+-rw-r--r--   0 meo       (1000) meo       (1000)     4164 2023-06-24 11:27:45.000000 meo-0.1.0/meo/crack/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)        0 2023-06-24 11:23:59.000000 meo-0.1.0/meo/crack/zip.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     1492 2023-06-24 09:52:08.000000 meo-0.1.0/meo/data.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      576 2023-06-24 09:52:08.000000 meo-0.1.0/meo/flask.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      814 2023-06-24 09:52:08.000000 meo-0.1.0/meo/net.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     2228 2023-06-24 10:20:41.000000 meo-0.1.0/meo/screen.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/meo/sound/
+-rw-r--r--   0 meo       (1000) meo       (1000)      980 2023-06-24 09:52:08.000000 meo-0.1.0/meo/sound/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      167 2023-06-24 09:52:08.000000 meo-0.1.0/meo/utils.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/meo.egg-info/
+-rw-r--r--   0 meo       (1000) meo       (1000)      709 2023-06-24 11:34:12.000000 meo-0.1.0/meo.egg-info/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      324 2023-06-24 11:34:12.000000 meo-0.1.0/meo.egg-info/SOURCES.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-06-24 11:34:12.000000 meo-0.1.0/meo.egg-info/dependency_links.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        4 2023-06-24 11:34:12.000000 meo-0.1.0/meo.egg-info/top_level.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-06-24 11:34:12.412438 meo-0.1.0/setup.cfg
+-rwxr-xr-x   0 meo       (1000) meo       (1000)     1024 2023-06-24 11:23:01.000000 meo-0.1.0/setup.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-06-24 11:34:12.412438 meo-0.1.0/test/
+-rw-r--r--   0 meo       (1000) meo       (1000)       56 2023-06-24 10:34:35.000000 meo-0.1.0/test/test-read.py
+-rw-r--r--   0 meo       (1000) meo       (1000)      143 2023-06-24 10:57:51.000000 meo-0.1.0/test/test.py
```

### Comparing `meo-0.0.8/LICENSE` & `meo-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 喵不嗷
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 喵不嗷
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `meo-0.0.8/meo/data.py` & `meo-0.1.0/meo/data.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-""" IO of formatted file and object """
-import json
-import os
-
-
-def checkout_dir(dir_path):
-    """Create if the folder does not exist"""
-    if not os.path.exists(dir_path):
-        os.makedirs(dir_path)
-
-def _checkout_file_path(path):
-    fdir, _ = os.path.split(path)
-    checkout_dir(fdir)
-
-
-def to_json(obj, path: str, encoding='utf8', ensure_ascii=False, indent=None, auto_mkdirs=True):
-    """ Serialize obj as a JSON formatted stream to ```path```` """
-    if auto_mkdirs:
-        _checkout_file_path(path)
-    with open(path, 'w+', encoding=encoding) as _f:
-        json.dump(obj, _f, ensure_ascii=ensure_ascii, indent=indent)
-
-
-def to_file(path, data, mode='w+', encoding="utf8", auto_mkdirs=True):
-    """write file and auto create dir not existed """
-    if auto_mkdirs:
-        _checkout_file_path(path)
-    with open(path, mode, encoding=encoding) as _f:
-        return _f.write(data)
-
-
-def load_json(path: str):
-    """ load json file from ```path``` """
-    with open(path, 'rb') as _f:
-        return json.load(_f)
-
-
-def load_file(path, encoding=None):
-    '''read file auto-closed'''
-    with open(path, 'rb') as _f:
-        content = _f.read()
-
-    if encoding:
-        return content.decode(encoding=encoding)
-    return content
-
-def decode(_bytes: bytes):
-    """decide encoding and decode `_bytes`"""
-    assert isinstance(_bytes, bytes)
-    for encoding in ["utf8", 'gbk', 'utf16', 'utf32']:
-        try:
-            return _bytes.decode(encoding)
-        except: pass
+""" IO of formatted file and object """
+import json
+import os
+
+
+def checkout_dir(dir_path):
+    """Create if the folder does not exist"""
+    if not os.path.exists(dir_path):
+        os.makedirs(dir_path)
+
+def _checkout_file_path(path):
+    fdir, _ = os.path.split(path)
+    checkout_dir(fdir)
+
+
+def to_json(obj, path: str, encoding='utf8', ensure_ascii=False, indent=None, auto_mkdirs=True):
+    """ Serialize obj as a JSON formatted stream to ```path```` """
+    if auto_mkdirs:
+        _checkout_file_path(path)
+    with open(path, 'w+', encoding=encoding) as _f:
+        json.dump(obj, _f, ensure_ascii=ensure_ascii, indent=indent)
+
+
+def to_file(path, data, mode='w+', encoding="utf8", auto_mkdirs=True):
+    """write file and auto create dir not existed """
+    if auto_mkdirs:
+        _checkout_file_path(path)
+    with open(path, mode, encoding=encoding) as _f:
+        return _f.write(data)
+
+
+def load_json(path: str):
+    """ load json file from ```path``` """
+    with open(path, 'rb') as _f:
+        return json.load(_f)
+
+
+def load_file(path, encoding=None):
+    '''read file auto-closed'''
+    with open(path, 'rb') as _f:
+        content = _f.read()
+
+    if encoding:
+        return content.decode(encoding=encoding)
+    return content
+
+def decode(_bytes: bytes):
+    """decide encoding and decode `_bytes`"""
+    assert isinstance(_bytes, bytes)
+    for encoding in ["utf8", 'gbk', 'utf16', 'utf32']:
+        try:
+            return _bytes.decode(encoding)
+        except: pass
```

### Comparing `meo-0.0.8/meo/flask.py` & `meo-0.1.0/meo/flask.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-'''
-    function may be used in flask app.
-'''
-def allow_cors(flask_app):
-    """
-        allow cors after requet.
-    """
-    @flask_app.after_request
-    def cors(environ):
-        environ.headers['Access-Control-Allow-Origin'] = '*'
-        environ.headers['Access-Control-Allow-Method'] = '*'
-        environ.headers["Access-Control-Allow-Credentials"] = 'true'
-        environ.headers['Access-Control-Allow-Headers'] = 'Content-Type, Depth, User-Agent, " \
-            "X-File-Size, X-Requested-With, If-Modified-Since, X-File-Name, Cache-Control'
-        return environ
+'''
+    function may be used in flask app.
+'''
+def allow_cors(flask_app):
+    """
+        allow cors after requet.
+    """
+    @flask_app.after_request
+    def cors(environ):
+        environ.headers['Access-Control-Allow-Origin'] = '*'
+        environ.headers['Access-Control-Allow-Method'] = '*'
+        environ.headers["Access-Control-Allow-Credentials"] = 'true'
+        environ.headers['Access-Control-Allow-Headers'] = 'Content-Type, Depth, User-Agent, " \
+            "X-File-Size, X-Requested-With, If-Modified-Since, X-File-Name, Cache-Control'
+        return environ
```

### Comparing `meo-0.0.8/meo/net.py` & `meo-0.1.0/meo/net.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""
-for spider
-"""
-from enum import Enum
-
-class UserAgent(Enum):
-
-    """UA in different platform"""
-
-    FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:102.0) Gecko/20100101 Firefox/102.0"
-
-    SAFARI_IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 15_5 like Mac OS X) " \
-                    "AppleWebKit/605.1.15 (KHTML, like Gecko) " \
-                    "Version/15.4 Mobile/15E148 Safari/604.1"
-
-    SAFARI_IPAD = "Mozilla/5.0 (iPad; CPU OS 15_5 like Mac OS X) " \
-                    "AppleWebKit/605.1.15 (KHTML, like Gecko) " \
-                    "Version/15.4 Mobile/15E148 Safari/604.1"
-
-    SAFARI_IPOD = "Mozilla/5.0 (iPod touch; CPU iPhone 15_5 like Mac OS X) " \
-                    "AppleWebKit/605.1.15 (KHTML, like Gecko) " \
-                    "Version/15.4 Mobile/15E148 Safari/604.1"
+"""
+for spider
+"""
+from enum import Enum
+
+class UserAgent(Enum):
+
+    """UA in different platform"""
+
+    FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:102.0) Gecko/20100101 Firefox/102.0"
+
+    SAFARI_IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 15_5 like Mac OS X) " \
+                    "AppleWebKit/605.1.15 (KHTML, like Gecko) " \
+                    "Version/15.4 Mobile/15E148 Safari/604.1"
+
+    SAFARI_IPAD = "Mozilla/5.0 (iPad; CPU OS 15_5 like Mac OS X) " \
+                    "AppleWebKit/605.1.15 (KHTML, like Gecko) " \
+                    "Version/15.4 Mobile/15E148 Safari/604.1"
+
+    SAFARI_IPOD = "Mozilla/5.0 (iPod touch; CPU iPhone 15_5 like Mac OS X) " \
+                    "AppleWebKit/605.1.15 (KHTML, like Gecko) " \
+                    "Version/15.4 Mobile/15E148 Safari/604.1"
```

### Comparing `meo-0.0.8/meo/screen.py` & `meo-0.1.0/meo/screen.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-'''
-    Display input and output
-'''
-
-SYMBOL_PLAIN          = "\33[0m"
-SYMBOL_CURSOR_HIDDEN  = "\33[?25l"
-SYMBOL_CURSOR_DISPLAY = "\33[?25h"
-SYMBOL_BLANKING       = "\33[8m"
-
-FORMAT_FONT_BLACK    = "\33[30;1m{}\33[0m"
-FORMAT_FONT_RED      = "\33[31;1m{}\33[0m"
-FORMAT_FONT_GREEN    = "\33[32;1m{}\33[0m"
-FORMAT_FONT_YELLOW   = "\33[33;1m{}\33[0m"
-FORMAT_FONT_BLUE     = "\33[34;1m{}\33[0m"
-FORMAT_FONT_PRUPLE   = "\33[35;1m{}\33[0m"
-FORMAT_FONT_SKY_BLUE = "\33[36;1m{}\33[0m"
-FORMAT_FONT_WHITE    = "\33[37;1m{}\33[0m"
-
-FORMAT_BG_BLACK    = "\33[40;1m{}\33[0m"
-FORMAT_BG_RED      = "\33[41;1m{}\33[0m"
-FORMAT_BG_GREEN    = "\33[42;1m{}\33[0m"
-FORMAT_BG_YELLOW   = "\33[43;1m{}\33[0m"
-FORMAT_BG_BLUE     = "\33[44;1m{}\33[0m"
-FORMAT_BG_PRUPLE   = "\33[45;1m{}\33[0m"
-FORMAT_BG_SKY_BLUE = "\33[46;1m{}\33[0m"
-FORMAT_BG_WHITE    = "\33[47;1m{}\33[0m"
-
-FORMAT_UNDERLINE       = "\33[4m{}\33[0m"
-FORMAT_TWINKLE         = "\33[5m{}\33[0m"
-FORMAT_REVERSE_DISPLAY = "\33[7m{}\33[0m"
-FORMAT_BLANKING        = "\33[8m{}\33[0m"
-
-FORMAT_CURSOR_MOVE_UP    = "\33[{}A"
-FORMAT_CURSOR_MOVE_DOWN  = "\33[{}B"
-FORMAT_CURSOR_MOVE_RIGHT = "\33[{}C"
-FORMAT_CURSOR_MOVE_LEFT  = "\33[{}D"
-
-def red_font(text, end='\n'):
-    '''print ```text``` red font'''
-    print(FORMAT_FONT_RED.format(text), end=end)
-
-def green_font(text, end="\n"):
-    '''print ```text``` green font'''
-    print(FORMAT_FONT_GREEN.format(text), end=end)
-
-def blue_font(text, end="\n"):
-    '''print ```text``` blue font'''
-    print(FORMAT_FONT_BLUE.format(text), end=end)
-
-def sformat(text, *styles):
-    '''format string```text```'''
-    for _s in styles:
-        text = _s.format(text)
-    return text
-
-def clear_screen():
-    '''clear screen'''
-    print("\33[2J")
-
-def hidden_input(__prompt: object):
-    """ hidden keyboard input """
-    text = input("{}{}{}".format(__prompt, SYMBOL_CURSOR_HIDDEN, SYMBOL_BLANKING))
-    print("{}{}".format(SYMBOL_PLAIN, SYMBOL_CURSOR_DISPLAY), end='')
-    return text
-
-if __name__ == "__main__":
-
-    # _text = sformat("hello world", FORMAT_BG_BLUE, FORMAT_FONT_YELLOW, FORMAT_UNDERLINE)
-    # print(_text)
-    # print(FORMAT_CURSOR_MOVE_UP.format(20))
-    # clear_screen()
-    # __psw = hidden_input("psw: ")
-    # print(__psw)
-    ...
+'''
+    Display input and output
+'''
+
+SYMBOL_PLAIN          = "\33[0m"
+SYMBOL_CURSOR_HIDDEN  = "\33[?25l"
+SYMBOL_CURSOR_DISPLAY = "\33[?25h"
+SYMBOL_BLANKING       = "\33[8m"
+
+FORMAT_FONT_BLACK    = "\33[30;1m{}\33[0m"
+FORMAT_FONT_RED      = "\33[31;1m{}\33[0m"
+FORMAT_FONT_GREEN    = "\33[32;1m{}\33[0m"
+FORMAT_FONT_YELLOW   = "\33[33;1m{}\33[0m"
+FORMAT_FONT_BLUE     = "\33[34;1m{}\33[0m"
+FORMAT_FONT_PRUPLE   = "\33[35;1m{}\33[0m"
+FORMAT_FONT_SKY_BLUE = "\33[36;1m{}\33[0m"
+FORMAT_FONT_WHITE    = "\33[37;1m{}\33[0m"
+
+FORMAT_BG_BLACK    = "\33[40;1m{}\33[0m"
+FORMAT_BG_RED      = "\33[41;1m{}\33[0m"
+FORMAT_BG_GREEN    = "\33[42;1m{}\33[0m"
+FORMAT_BG_YELLOW   = "\33[43;1m{}\33[0m"
+FORMAT_BG_BLUE     = "\33[44;1m{}\33[0m"
+FORMAT_BG_PRUPLE   = "\33[45;1m{}\33[0m"
+FORMAT_BG_SKY_BLUE = "\33[46;1m{}\33[0m"
+FORMAT_BG_WHITE    = "\33[47;1m{}\33[0m"
+
+FORMAT_UNDERLINE       = "\33[4m{}\33[0m"
+FORMAT_TWINKLE         = "\33[5m{}\33[0m"
+FORMAT_REVERSE_DISPLAY = "\33[7m{}\33[0m"
+FORMAT_BLANKING        = "\33[8m{}\33[0m"
+
+FORMAT_CURSOR_MOVE_UP    = "\33[{}A"
+FORMAT_CURSOR_MOVE_DOWN  = "\33[{}B"
+FORMAT_CURSOR_MOVE_RIGHT = "\33[{}C"
+FORMAT_CURSOR_MOVE_LEFT  = "\33[{}D"
+
+def red_font(text, end='\n'):
+    '''print ```text``` red font'''
+    print(FORMAT_FONT_RED.format(text), end=end)
+
+def green_font(text, end="\n"):
+    '''print ```text``` green font'''
+    print(FORMAT_FONT_GREEN.format(text), end=end)
+
+def blue_font(text, end="\n"):
+    '''print ```text``` blue font'''
+    print(FORMAT_FONT_BLUE.format(text), end=end)
+
+def sformat(text, *styles):
+    '''format string```text```'''
+    for _s in styles:
+        text = _s.format(text)
+    return text
+
+def clear_screen():
+    '''clear screen'''
+    print("\33[2J")
+
+def hidden_input(__prompt: object):
+    """ hidden keyboard input """
+    text = input("{}{}{}".format(__prompt, SYMBOL_CURSOR_HIDDEN, SYMBOL_BLANKING))
+    print("{}{}".format(SYMBOL_PLAIN, SYMBOL_CURSOR_DISPLAY), end='')
+    return text
+
+if __name__ == "__main__":
+
+    # _text = sformat("hello world", FORMAT_BG_BLUE, FORMAT_FONT_YELLOW, FORMAT_UNDERLINE)
+    # print(_text)
+    # print(FORMAT_CURSOR_MOVE_UP.format(20))
+    # clear_screen()
+    # __psw = hidden_input("psw: ")
+    # print(__psw)
+    ...
```

### Comparing `meo-0.0.8/setup.py` & `meo-0.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,32 @@
-"""
-setup script
-"""
-import os
-import shutil
-from setuptools import setup, find_packages
-
-CUR_PATH = os.path.dirname(os.path.abspath(__file__))
-path = os.path.join(CUR_PATH, "build")
-if os.path.isdir(path):
-    print("INFO DEL DIR ", path)
-    shutil.rmtree(path)
-path = os.path.join(CUR_PATH, "dist")
-if os.path.isdir(path):
-    print("INFO DEL DIR ", path)
-    shutil.rmtree(path)
-
-info = {}
-with open(os.path.join(CUR_PATH, "meo/__version__.py"), 'r+', encoding='utf8') as f:
-    exec(f.read(), info)
-
-with open(os.path.join(CUR_PATH, "description.md"), 'r+', encoding='utf8') as f:
-    long_description = f.read()
-
-setup(
-    name         =  info['__title__'],
-    author       =  info["__author__"],
-    url          =  info["__url__"],
-    description  =  info["__description__"],
-    version      =  info["__version__"],
-    license      =  info["__license__"],
-    author_email =  info["__author_email__"],
-    packages     = find_packages(),
-    include_package_data = True,
-    long_description     = long_description,
-    long_description_content_type="text/markdown",
-    classifiers=(
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ),
-)
+#!/usr/bin/env python
+import os
+import shutil
+from setuptools import setup, find_packages
+
+CUR_PATH = os.path.dirname(os.path.abspath(__file__))
+
+info = {}
+with open(os.path.join(CUR_PATH, "meo/__version__.py"), 'r+', encoding='utf8') as f:
+    exec(f.read(), info)
+
+with open(os.path.join(CUR_PATH, "description.md"), 'r+', encoding='utf8') as f:
+    long_description = f.read()
+
+setup(
+    name         =  info['__title__'],
+    author       =  info["__author__"],
+    url          =  info["__url__"],
+    description  =  info["__description__"],
+    version      =  info["__version__"],
+    license      =  info["__license__"],
+    author_email =  info["__author_email__"],
+    packages     = find_packages(),
+    include_package_data = True,
+    long_description     = long_description,
+    long_description_content_type="text/markdown",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
+    ],
+)
```

