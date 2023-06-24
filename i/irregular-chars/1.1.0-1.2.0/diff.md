# Comparing `tmp/irregular-chars-1.1.0.tar.gz` & `tmp/irregular-chars-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irregular-chars-1.1.0.tar", last modified: Sat Jun 24 19:11:19 2023, max compression
+gzip compressed data, was "irregular-chars-1.2.0.tar", last modified: Sat Jun 24 20:20:58 2023, max compression
```

## Comparing `irregular-chars-1.1.0.tar` & `irregular-chars-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 19:11:19.829247 irregular-chars-1.1.0/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-24 15:34:45.000000 irregular-chars-1.1.0/LICENSE
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      500 2023-06-24 19:11:19.825247 irregular-chars-1.1.0/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      461 2023-06-24 18:19:52.000000 irregular-chars-1.1.0/README.md
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 19:11:19.825247 irregular-chars-1.1.0/irregular_chars/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      123 2023-06-24 19:07:24.000000 irregular-chars-1.1.0/irregular_chars/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1518 2023-06-24 19:03:48.000000 irregular-chars-1.1.0/irregular_chars/sound_symbol.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       95 2023-06-24 18:51:05.000000 irregular-chars-1.1.0/irregular_chars/unicodes.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      694 2023-06-24 18:29:06.000000 irregular-chars-1.1.0/irregular_chars/zero_width.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 19:11:19.825247 irregular-chars-1.1.0/irregular_chars.egg-info/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      500 2023-06-24 19:11:19.000000 irregular-chars-1.1.0/irregular_chars.egg-info/PKG-INFO
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      401 2023-06-24 19:11:19.000000 irregular-chars-1.1.0/irregular_chars.egg-info/SOURCES.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-24 19:11:19.000000 irregular-chars-1.1.0/irregular_chars.egg-info/dependency_links.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       22 2023-06-24 19:11:19.000000 irregular-chars-1.1.0/irregular_chars.egg-info/top_level.txt
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-24 19:11:19.829247 irregular-chars-1.1.0/setup.cfg
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      730 2023-06-24 19:10:57.000000 irregular-chars-1.1.0/setup.py
-drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 19:11:19.825247 irregular-chars-1.1.0/tests/
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 14:44:31.000000 irregular-chars-1.1.0/tests/__init__.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      966 2023-06-24 19:10:03.000000 irregular-chars-1.1.0/tests/test_sound_symbols.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      928 2023-06-24 19:04:32.000000 irregular-chars-1.1.0/tests/test_unicodes.py
--rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      901 2023-06-24 19:06:15.000000 irregular-chars-1.1.0/tests/test_zero_width_spaces.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 20:20:58.973553 irregular-chars-1.2.0/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1069 2023-06-24 15:34:45.000000 irregular-chars-1.2.0/LICENSE
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      500 2023-06-24 20:20:58.969553 irregular-chars-1.2.0/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1143 2023-06-24 20:19:57.000000 irregular-chars-1.2.0/README.md
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 20:20:58.969553 irregular-chars-1.2.0/irregular_chars/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      523 2023-06-24 20:03:06.000000 irregular-chars-1.2.0/irregular_chars/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      719 2023-06-24 20:15:01.000000 irregular-chars-1.2.0/irregular_chars/space.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     1503 2023-06-24 19:36:27.000000 irregular-chars-1.2.0/irregular_chars/splitted.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       95 2023-06-24 18:51:05.000000 irregular-chars-1.2.0/irregular_chars/unicodes.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      179 2023-06-24 20:06:39.000000 irregular-chars-1.2.0/irregular_chars/utils.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     3245 2023-06-24 19:58:04.000000 irregular-chars-1.2.0/irregular_chars/width.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 20:20:58.969553 irregular-chars-1.2.0/irregular_chars.egg-info/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      500 2023-06-24 20:20:58.000000 irregular-chars-1.2.0/irregular_chars.egg-info/PKG-INFO
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      462 2023-06-24 20:20:58.000000 irregular-chars-1.2.0/irregular_chars.egg-info/SOURCES.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        1 2023-06-24 20:20:58.000000 irregular-chars-1.2.0/irregular_chars.egg-info/dependency_links.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       22 2023-06-24 20:20:58.000000 irregular-chars-1.2.0/irregular_chars.egg-info/top_level.txt
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)       38 2023-06-24 20:20:58.973553 irregular-chars-1.2.0/setup.cfg
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      730 2023-06-24 20:20:48.000000 irregular-chars-1.2.0/setup.py
+drwxrwxr-x   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 20:20:58.969553 irregular-chars-1.2.0/tests/
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)        0 2023-06-24 14:44:31.000000 irregular-chars-1.2.0/tests/__init__.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      966 2023-06-24 20:03:43.000000 irregular-chars-1.2.0/tests/test_sound_symbols.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      928 2023-06-24 19:04:32.000000 irregular-chars-1.2.0/tests/test_unicodes.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)     6034 2023-06-24 20:11:24.000000 irregular-chars-1.2.0/tests/test_width.py
+-rw-rw-r--   0 masatoemata  (1000) masatoemata  (1000)      959 2023-06-24 20:03:34.000000 irregular-chars-1.2.0/tests/test_zero_width_spaces.py
```

### Comparing `irregular-chars-1.1.0/LICENSE` & `irregular-chars-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.1.0/irregular_chars/sound_symbol.py` & `irregular-chars-1.2.0/irregular_chars/splitted.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from .utils import replace_pair
+
 SOUND_SYMBOL_VARIATIONS = [
     ("ガ", "ガ"),
     ("ギ", "ギ"),
     ("グ", "グ"),
     ("ゲ", "ゲ"),
     ("ゴ", "ゴ"),
     ("が", "が"),
@@ -55,10 +57,8 @@
 def combine_sound_symbols(text: str) -> str:
     """
     >>> combine_sound_symbols("ガギグゲゴ")
     'ガギグゲゴ'
     >>> combine_sound_symbols("がぎぐげご")
     'がぎぐげご'
     """
-    for pair in SOUND_SYMBOL_VARIATIONS:
-        text = text.replace(pair[0], pair[1])
-    return text
+    return replace_pair(text, SOUND_SYMBOL_VARIATIONS)
```

### Comparing `irregular-chars-1.1.0/irregular_chars/zero_width.py` & `irregular-chars-1.2.0/irregular_chars/space.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,11 +12,12 @@
     "NARROW NO-BREAK SPACE": u"\u202F",
     "MEDIUM MATHEMATICAL SPACE": u"\u205F",
     "WORD JOINER": u"\u2060",
     "COMBINING GRAPHEME JOINER": u"\u034F",
 }
 
 
-def remove_zero_width(text: str) -> str:
-    for char in ZERO_WIDTH_SPACES.values():
+def remove_zero_width_spaces(text: str) -> str:
+    pairs = ZERO_WIDTH_SPACES.values()
+    for char in pairs:
         text = text.replace(char, "")
     return text
```

### Comparing `irregular-chars-1.1.0/setup.py` & `irregular-chars-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="irregular-chars",
-    version="1.1.0",
+    version="1.2.0",
     description="A library for cleaning text, such as removing zero-width characters or"
     "converting full-width characters to half-width",
     packages=find_packages(),
     install_requires=[],
     classifiers=[  # パッケージのメタデータ（詳細は https://pypi.org/classifiers/ を参照）
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
```

### Comparing `irregular-chars-1.1.0/tests/test_sound_symbols.py` & `irregular-chars-1.2.0/tests/test_sound_symbols.py`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.1.0/tests/test_unicodes.py` & `irregular-chars-1.2.0/tests/test_unicodes.py`

 * *Files identical despite different names*

### Comparing `irregular-chars-1.1.0/tests/test_zero_width_spaces.py` & `irregular-chars-1.2.0/tests/test_zero_width_spaces.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import pytest
 
-from irregular_chars import remove_zero_width
-from irregular_chars.zero_width import ZERO_WIDTH_SPACES
+from irregular_chars import remove_zero_width_spaces
+from irregular_chars.space import ZERO_WIDTH_SPACES
 
 
 @pytest.mark.parametrize("name, char", ZERO_WIDTH_SPACES.items())
-def test_remove_zero_width(name, char):
+def test_remove_zero_width_spaces(name, char):
     test_str = f"Hello{char}World"
     expected_str = "HelloWorld"
-    assert remove_zero_width(test_str) == expected_str
+    assert remove_zero_width_spaces(test_str) == expected_str
 
 
-def test_remove_zero_width_multiple_and_mixed():
+def test_remove_zero_width_spaces_multiple_and_mixed():
     test_str = f"Hello{ZERO_WIDTH_SPACES['ZERO WIDTH SPACE']}W{ZERO_WIDTH_SPACES['ZERO WIDTH JOINER']}orld"
     expected_str = "HelloWorld"
-    assert remove_zero_width(test_str) == expected_str
+    assert remove_zero_width_spaces(test_str) == expected_str
 
 
-def test_remove_zero_width_no_change():
+def test_remove_zero_width_spaces_no_change():
     test_str = "Hello World"
     expected_str = "Hello World"
-    assert remove_zero_width(test_str) == expected_str
+    assert remove_zero_width_spaces(test_str) == expected_str
 
 
-def test_remove_zero_width_use_quotations():
+def test_remove_zero_width_spaces_use_quotations():
     origin = '"​"""⁡""­"'
     expect = '"""""""'
-    assert expect == remove_zero_width(origin)
+    assert expect == remove_zero_width_spaces(origin)
```

