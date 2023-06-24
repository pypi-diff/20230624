# Comparing `tmp/pypinyin-g2pw-0.3.0.tar.gz` & `tmp/pypinyin-g2pw-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypinyin-g2pw-0.3.0.tar", last modified: Sat Sep  3 06:55:50 2022, max compression
+gzip compressed data, was "pypinyin-g2pw-0.4.0.tar", last modified: Sat Jun 24 08:08:08 2023, max compression
```

## Comparing `pypinyin-g2pw-0.3.0.tar` & `pypinyin-g2pw-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mg         (501) wheel        (0)        0 2022-09-03 06:55:50.183738 pypinyin-g2pw-0.3.0/
--rw-r--r--   0 mg         (501) wheel        (0)     3877 2022-09-03 06:55:50.183984 pypinyin-g2pw-0.3.0/PKG-INFO
--rw-r--r--   0 mg         (501) wheel        (0)     2760 2022-09-03 06:42:06.000000 pypinyin-g2pw-0.3.0/README.md
--rw-r--r--   0 mg         (501) wheel        (0)      105 2022-08-21 10:33:17.000000 pypinyin-g2pw-0.3.0/pyproject.toml
--rw-r--r--   0 mg         (501) wheel        (0)       67 2022-09-03 06:55:50.184808 pypinyin-g2pw-0.3.0/setup.cfg
--rw-r--r--   0 mg         (501) wheel        (0)      930 2022-09-03 06:42:15.000000 pypinyin-g2pw-0.3.0/setup.py
-drwxr-xr-x   0 mg         (501) wheel        (0)        0 2022-09-03 06:55:50.178640 pypinyin-g2pw-0.3.0/src/
-drwxr-xr-x   0 mg         (501) wheel        (0)        0 2022-09-03 06:55:50.180794 pypinyin-g2pw-0.3.0/src/pypinyin_g2pw/
--rw-r--r--   0 mg         (501) wheel        (0)       80 2022-08-13 13:11:43.000000 pypinyin-g2pw-0.3.0/src/pypinyin_g2pw/__init__.py
--rw-r--r--   0 mg         (501) wheel        (0)     3548 2022-08-28 02:48:13.000000 pypinyin-g2pw-0.3.0/src/pypinyin_g2pw/g2pw.py
-drwxr-xr-x   0 mg         (501) wheel        (0)        0 2022-09-03 06:55:50.183242 pypinyin-g2pw-0.3.0/src/pypinyin_g2pw.egg-info/
--rw-r--r--   0 mg         (501) wheel        (0)     3877 2022-09-03 06:55:50.000000 pypinyin-g2pw-0.3.0/src/pypinyin_g2pw.egg-info/PKG-INFO
--rw-r--r--   0 mg         (501) wheel        (0)      303 2022-09-03 06:55:50.000000 pypinyin-g2pw-0.3.0/src/pypinyin_g2pw.egg-info/SOURCES.txt
--rw-r--r--   0 mg         (501) wheel        (0)        1 2022-09-03 06:55:50.000000 pypinyin-g2pw-0.3.0/src/pypinyin_g2pw.egg-info/dependency_links.txt
--rw-r--r--   0 mg         (501) wheel        (0)       29 2022-09-03 06:55:50.000000 pypinyin-g2pw-0.3.0/src/pypinyin_g2pw.egg-info/requires.txt
--rw-r--r--   0 mg         (501) wheel        (0)       14 2022-09-03 06:55:50.000000 pypinyin-g2pw-0.3.0/src/pypinyin_g2pw.egg-info/top_level.txt
+drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-06-24 08:08:08.312273 pypinyin-g2pw-0.4.0/
+-rw-r--r--   0 mg         (501) wheel        (0)     3877 2023-06-24 08:08:08.312459 pypinyin-g2pw-0.4.0/PKG-INFO
+-rw-r--r--   0 mg         (501) wheel        (0)     2760 2023-06-24 07:39:10.000000 pypinyin-g2pw-0.4.0/README.md
+-rw-r--r--   0 mg         (501) wheel        (0)      105 2022-08-21 10:33:17.000000 pypinyin-g2pw-0.4.0/pyproject.toml
+-rw-r--r--   0 mg         (501) wheel        (0)       67 2023-06-24 08:08:08.313051 pypinyin-g2pw-0.4.0/setup.cfg
+-rw-r--r--   0 mg         (501) wheel        (0)      930 2023-06-24 08:03:14.000000 pypinyin-g2pw-0.4.0/setup.py
+drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-06-24 08:08:08.306816 pypinyin-g2pw-0.4.0/src/
+drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-06-24 08:08:08.309509 pypinyin-g2pw-0.4.0/src/pypinyin_g2pw/
+-rw-r--r--   0 mg         (501) wheel        (0)       80 2022-08-13 13:11:43.000000 pypinyin-g2pw-0.4.0/src/pypinyin_g2pw/__init__.py
+-rw-r--r--   0 mg         (501) wheel        (0)     3573 2023-06-24 07:41:30.000000 pypinyin-g2pw-0.4.0/src/pypinyin_g2pw/g2pw.py
+drwxr-xr-x   0 mg         (501) wheel        (0)        0 2023-06-24 08:08:08.311891 pypinyin-g2pw-0.4.0/src/pypinyin_g2pw.egg-info/
+-rw-r--r--   0 mg         (501) wheel        (0)     3877 2023-06-24 08:08:08.000000 pypinyin-g2pw-0.4.0/src/pypinyin_g2pw.egg-info/PKG-INFO
+-rw-r--r--   0 mg         (501) wheel        (0)      303 2023-06-24 08:08:08.000000 pypinyin-g2pw-0.4.0/src/pypinyin_g2pw.egg-info/SOURCES.txt
+-rw-r--r--   0 mg         (501) wheel        (0)        1 2023-06-24 08:08:08.000000 pypinyin-g2pw-0.4.0/src/pypinyin_g2pw.egg-info/dependency_links.txt
+-rw-r--r--   0 mg         (501) wheel        (0)       29 2023-06-24 08:08:08.000000 pypinyin-g2pw-0.4.0/src/pypinyin_g2pw.egg-info/requires.txt
+-rw-r--r--   0 mg         (501) wheel        (0)       14 2023-06-24 08:08:08.000000 pypinyin-g2pw-0.4.0/src/pypinyin_g2pw.egg-info/top_level.txt
```

### Comparing `pypinyin-g2pw-0.3.0/PKG-INFO` & `pypinyin-g2pw-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypinyin-g2pw
-Version: 0.3.0
+Version: 0.4.0
 Summary: 基于 g2pW 提升 pypinyin 的准确性。
 Home-page: https://github.com/mozillazg/pypinyin-g2pW
 Author: mozillazg
 Author-email: mozillazg101@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mozillazg/pypinyin-g2pW/issues
 Description: # pypinyin-g2pW
```

### Comparing `pypinyin-g2pw-0.3.0/README.md` & `pypinyin-g2pw-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pypinyin-g2pw-0.3.0/setup.py` & `pypinyin-g2pw-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="pypinyin-g2pw",
-    version="0.3.0",
+    version="0.4.0",
     author="mozillazg",
     author_email="mozillazg101@gmail.com",
     description="基于 g2pW 提升 pypinyin 的准确性。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mozillazg/pypinyin-g2pW",
     project_urls={
```

### Comparing `pypinyin-g2pw-0.3.0/src/pypinyin_g2pw/g2pw.py` & `pypinyin-g2pw-0.4.0/src/pypinyin_g2pw/g2pw.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 from g2pw.api import G2PWConverter
 
 
 class G2PWPinyin(Pinyin):
     def __init__(self, model_dir='G2PWModel/', model_source=None,
                  num_workers=None, batch_size=None,
                  turnoff_tqdm=True, enable_non_tradional_chinese=True,
-                 v_to_u=False, neutral_tone_with_five=False, **kwargs):
+                 v_to_u=False, neutral_tone_with_five=False, tone_sandhi=False, **kwargs):
         self._g2pw = G2PWConverter(
             model_dir=model_dir,
             style='pinyin',
             model_source=model_source,
             num_workers=num_workers,
             batch_size=batch_size,
             turnoff_tqdm=turnoff_tqdm,
             enable_non_tradional_chinese=enable_non_tradional_chinese,
         )
         self._converter = Converter(
             self._g2pw, v_to_u=v_to_u,
             neutral_tone_with_five=neutral_tone_with_five,
-            tone_sandhi=False,
+            tone_sandhi=tone_sandhi,
         )
 
     def get_seg(self, **kwargs):
         return simple_seg
 
 
 class Converter(UltimateConverter):
```

### Comparing `pypinyin-g2pw-0.3.0/src/pypinyin_g2pw.egg-info/PKG-INFO` & `pypinyin-g2pw-0.4.0/src/pypinyin_g2pw.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypinyin-g2pw
-Version: 0.3.0
+Version: 0.4.0
 Summary: 基于 g2pW 提升 pypinyin 的准确性。
 Home-page: https://github.com/mozillazg/pypinyin-g2pW
 Author: mozillazg
 Author-email: mozillazg101@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mozillazg/pypinyin-g2pW/issues
 Description: # pypinyin-g2pW
```

