# Comparing `tmp/cns-1.0.23-py3-none-any.whl.zip` & `tmp/cns-1.0.26-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 74988 bytes, number of entries: 8
+Zip file size: 74989 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat    84992 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    74240 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      415 b- defN 23-Jun-23 12:39 cns/__init__.py
--rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-24 09:06 cns-1.0.23.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4612 b- defN 23-Jun-24 09:06 cns-1.0.23.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-24 09:06 cns-1.0.23.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-24 09:06 cns-1.0.23.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      616 b- defN 23-Jun-24 09:06 cns-1.0.23.dist-info/RECORD
-8 files, 165449 bytes uncompressed, 73920 bytes compressed:  55.3%
+-rw-rw-rw-  2.0 fat      419 b- defN 23-Jun-24 09:18 cns/__init__.py
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-24 09:18 cns-1.0.26.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4612 b- defN 23-Jun-24 09:18 cns-1.0.26.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-24 09:18 cns-1.0.26.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-24 09:18 cns-1.0.26.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      616 b- defN 23-Jun-24 09:18 cns-1.0.26.dist-info/RECORD
+8 files, 165453 bytes uncompressed, 73921 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: cns/SQLstrX.cp39-win_amd64.pyd
 Comment: 
 
 Filename: cns/__init__.py
 Comment: 
 
-Filename: cns-1.0.23.dist-info/LICENSE
+Filename: cns-1.0.26.dist-info/LICENSE
 Comment: 
 
-Filename: cns-1.0.23.dist-info/METADATA
+Filename: cns-1.0.26.dist-info/METADATA
 Comment: 
 
-Filename: cns-1.0.23.dist-info/WHEEL
+Filename: cns-1.0.26.dist-info/WHEEL
 Comment: 
 
-Filename: cns-1.0.23.dist-info/top_level.txt
+Filename: cns-1.0.26.dist-info/top_level.txt
 Comment: 
 
-Filename: cns-1.0.23.dist-info/RECORD
+Filename: cns-1.0.26.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cns/__init__.py

```diff
@@ -1,8 +1,8 @@
 # 定义当使用“from my_package import *”时导入的内容
 #__all__ = ["DateTimeX"]  # *导入类时限制在此范围
 
-from .DateTimeX import DateTimeX     # 日期获取
-from .DataX import DataX             # 数据处理
-from .TextX import TextX             # 文本处理
+#from .DateTimeX import DateTimeX     # 日期获取
+#from .DataX import DataX             # 数据处理
+#from .TextX import TextX             # 文本处理
 from .SQLstrX import SQLstrX         # RPASQL处理
-from .PathX import PathX             # 路径处理(修改文件名等)
+#from .PathX import PathX             # 路径处理(修改文件名等)
```

## Comparing `cns-1.0.23.dist-info/METADATA` & `cns-1.0.26.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.0.23
+Version: 1.0.26
 Summary: cns工具包
 Home-page: https://cns.ink/example
 Author: rambo
 Author-email: 6566666@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

