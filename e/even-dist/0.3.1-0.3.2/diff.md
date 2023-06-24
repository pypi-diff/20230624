# Comparing `tmp/even_dist-0.3.1-py3-none-any.whl.zip` & `tmp/even_dist-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 3107 bytes, number of entries: 9
+Zip file size: 3265 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Jun-24 00:32 even_dist/__init__.py
 -rw-rw-rw-  2.0 fat      713 b- defN 23-Jun-24 00:11 even_dist/even_dist.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-24 01:57 hello/__init__.py
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-24 02:37 hello/fadf.txt
 -rw-rw-rw-  2.0 fat       21 b- defN 23-Jun-24 02:01 hello/hello.txt
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-24 02:31 even_dist-0.3.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      449 b- defN 23-Jun-24 02:31 even_dist-0.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-24 02:31 even_dist-0.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-24 02:31 even_dist-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      690 b- defN 23-Jun-24 02:31 even_dist-0.3.1.dist-info/RECORD
-9 files, 3125 bytes uncompressed, 1913 bytes compressed:  38.8%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-24 02:38 even_dist-0.3.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      449 b- defN 23-Jun-24 02:38 even_dist-0.3.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-24 02:38 even_dist-0.3.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-24 02:38 even_dist-0.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      758 b- defN 23-Jun-24 02:38 even_dist-0.3.2.dist-info/RECORD
+10 files, 3201 bytes uncompressed, 1967 bytes compressed:  38.6%
```

## zipnote {}

```diff
@@ -3,26 +3,29 @@
 
 Filename: even_dist/even_dist.py
 Comment: 
 
 Filename: hello/__init__.py
 Comment: 
 
+Filename: hello/fadf.txt
+Comment: 
+
 Filename: hello/hello.txt
 Comment: 
 
-Filename: even_dist-0.3.1.dist-info/LICENSE
+Filename: even_dist-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: even_dist-0.3.1.dist-info/METADATA
+Filename: even_dist-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: even_dist-0.3.1.dist-info/WHEEL
+Filename: even_dist-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: even_dist-0.3.1.dist-info/top_level.txt
+Filename: even_dist-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: even_dist-0.3.1.dist-info/RECORD
+Filename: even_dist-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `even_dist-0.3.1.dist-info/LICENSE` & `even_dist-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `even_dist-0.3.1.dist-info/RECORD` & `even_dist-0.3.2.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 even_dist/__init__.py,sha256=_hp6Ra0MzYT_hyhfXeY9ChFjewnc4OswrNhZfmdA9BU,53
 even_dist/even_dist.py,sha256=__DjHpA9ElBbbUBwowt_tdCy_7N1ktZIe6T9X0gC4KU,713
 hello/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+hello/fadf.txt,sha256=nzsedlYAJyBPGFEjuJrI4fEriwPCXF41SzLHhtjfvHY,8
 hello/hello.txt,sha256=bjUtEt1LG-1BNHlMgLpbII5yxzILakA-4hROMkusGQk,21
-even_dist-0.3.1.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-even_dist-0.3.1.dist-info/METADATA,sha256=KDeh7Ydw7ReDPKAmpcy1IcGHS6g1b9FcamEZe4GWs_c,449
-even_dist-0.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-even_dist-0.3.1.dist-info/top_level.txt,sha256=hDrgdyDLgZmR7lkbPjoTK-2RwXVzkM5vGJsvI2BQP6w,16
-even_dist-0.3.1.dist-info/RECORD,,
+even_dist-0.3.2.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+even_dist-0.3.2.dist-info/METADATA,sha256=_AfvAqV8E7AlXXCw-lLkwE-orKb4XrbvP5tiPESM5E8,449
+even_dist-0.3.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+even_dist-0.3.2.dist-info/top_level.txt,sha256=hDrgdyDLgZmR7lkbPjoTK-2RwXVzkM5vGJsvI2BQP6w,16
+even_dist-0.3.2.dist-info/RECORD,,
```

