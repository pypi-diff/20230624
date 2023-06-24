# Comparing `tmp/cns-1.0.26-py3-none-any.whl.zip` & `tmp/cns-1.0.27-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,19 @@
-Zip file size: 74989 bytes, number of entries: 8
+Zip file size: 460997 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat   173056 b- defN 23-Jun-15 05:40 cns/DataX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   156672 b- defN 23-Jun-15 05:40 cns/DataX.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    82944 b- defN 23-Jun-02 15:12 cns/DateTimeX.cp36-win32.pyd
+-rw-rw-rw-  2.0 fat    99840 b- defN 23-Jun-02 15:11 cns/DateTimeX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    88576 b- defN 23-Jun-02 15:13 cns/DateTimeX.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    71168 b- defN 23-Jun-23 11:03 cns/PathX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    59392 b- defN 23-Jun-23 11:02 cns/PathX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    84992 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    74240 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      419 b- defN 23-Jun-24 09:18 cns/__init__.py
--rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-24 09:18 cns-1.0.26.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4612 b- defN 23-Jun-24 09:18 cns-1.0.26.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-24 09:18 cns-1.0.26.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-24 09:18 cns-1.0.26.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      616 b- defN 23-Jun-24 09:18 cns-1.0.26.dist-info/RECORD
-8 files, 165453 bytes uncompressed, 73921 bytes compressed:  55.3%
+-rw-rw-rw-  2.0 fat    77312 b- defN 23-Jun-23 11:03 cns/TextX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    65536 b- defN 23-Jun-23 11:02 cns/TextX.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      415 b- defN 23-Jun-23 12:39 cns/__init__.py
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-24 14:46 cns-1.0.27.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1939 b- defN 23-Jun-24 14:46 cns-1.0.27.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-24 14:46 cns-1.0.27.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-24 14:46 cns-1.0.27.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1400 b- defN 23-Jun-24 14:46 cns-1.0.27.dist-info/RECORD
+17 files, 1038056 bytes uncompressed, 458725 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -1,25 +1,52 @@
+Filename: cns/DataX.cp36-win_amd64.pyd
+Comment: 
+
+Filename: cns/DataX.cp39-win_amd64.pyd
+Comment: 
+
+Filename: cns/DateTimeX.cp36-win32.pyd
+Comment: 
+
+Filename: cns/DateTimeX.cp36-win_amd64.pyd
+Comment: 
+
+Filename: cns/DateTimeX.cp39-win_amd64.pyd
+Comment: 
+
+Filename: cns/PathX.cp36-win_amd64.pyd
+Comment: 
+
+Filename: cns/PathX.cp39-win_amd64.pyd
+Comment: 
+
 Filename: cns/SQLstrX.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/SQLstrX.cp39-win_amd64.pyd
 Comment: 
 
+Filename: cns/TextX.cp36-win_amd64.pyd
+Comment: 
+
+Filename: cns/TextX.cp39-win_amd64.pyd
+Comment: 
+
 Filename: cns/__init__.py
 Comment: 
 
-Filename: cns-1.0.26.dist-info/LICENSE
+Filename: cns-1.0.27.dist-info/LICENSE
 Comment: 
 
-Filename: cns-1.0.26.dist-info/METADATA
+Filename: cns-1.0.27.dist-info/METADATA
 Comment: 
 
-Filename: cns-1.0.26.dist-info/WHEEL
+Filename: cns-1.0.27.dist-info/WHEEL
 Comment: 
 
-Filename: cns-1.0.26.dist-info/top_level.txt
+Filename: cns-1.0.27.dist-info/top_level.txt
 Comment: 
 
-Filename: cns-1.0.26.dist-info/RECORD
+Filename: cns-1.0.27.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cns/__init__.py

```diff
@@ -1,8 +1,8 @@
 # 定义当使用“from my_package import *”时导入的内容
 #__all__ = ["DateTimeX"]  # *导入类时限制在此范围
 
-#from .DateTimeX import DateTimeX     # 日期获取
-#from .DataX import DataX             # 数据处理
-#from .TextX import TextX             # 文本处理
+from .DateTimeX import DateTimeX     # 日期获取
+from .DataX import DataX             # 数据处理
+from .TextX import TextX             # 文本处理
 from .SQLstrX import SQLstrX         # RPASQL处理
-#from .PathX import PathX             # 路径处理(修改文件名等)
+from .PathX import PathX             # 路径处理(修改文件名等)
```

