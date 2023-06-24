# Comparing `tmp/cny-1.0.3-py3-none-any.whl.zip` & `tmp/cny-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 146650 bytes, number of entries: 8
+Zip file size: 146632 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat   173056 b- defN 23-Jun-15 05:40 cny/DataX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat   156672 b- defN 23-Jun-15 05:40 cny/DataX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      419 b- defN 23-Jun-24 14:55 cny/__init__.py
--rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-24 15:01 cny-1.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      580 b- defN 23-Jun-24 15:01 cny-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-24 15:01 cny-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-24 15:01 cny-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      608 b- defN 23-Jun-24 15:01 cny-1.0.3.dist-info/RECORD
-8 files, 331909 bytes uncompressed, 145600 bytes compressed:  56.1%
+-rw-rw-rw-  2.0 fat      419 b- defN 23-Jun-24 15:03 cny/__init__.py
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-24 15:04 cny-1.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      549 b- defN 23-Jun-24 15:04 cny-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-24 15:04 cny-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-24 15:04 cny-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      608 b- defN 23-Jun-24 15:04 cny-1.0.5.dist-info/RECORD
+8 files, 331878 bytes uncompressed, 145582 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: cny/DataX.cp39-win_amd64.pyd
 Comment: 
 
 Filename: cny/__init__.py
 Comment: 
 
-Filename: cny-1.0.3.dist-info/LICENSE
+Filename: cny-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: cny-1.0.3.dist-info/METADATA
+Filename: cny-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: cny-1.0.3.dist-info/WHEEL
+Filename: cny-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: cny-1.0.3.dist-info/top_level.txt
+Filename: cny-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: cny-1.0.3.dist-info/RECORD
+Filename: cny-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cny/__init__.py

```diff
@@ -1,8 +1,8 @@
 # 定义当使用“from my_package import *”时导入的内容
 #__all__ = ["DateTimeX"]  # *导入类时限制在此范围
 
-from .DateTimeX import DateTimeX     # 日期获取
-#from .DataX import DataX             # 数据处理
+#from .DateTimeX import DateTimeX     # 日期获取
+from .DataX import DataX             # 数据处理
 #from .TextX import TextX             # 文本处理
 #from .SQLstrX import SQLstrX         # RPASQL处理
 #from .PathX import PathX             # 路径处理(修改文件名等)
```

## Comparing `cny-1.0.3.dist-info/METADATA` & `cny-1.0.5.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: cny
-Version: 1.0.3
+Version: 1.0.5
 Summary: cny公测工具包
 Home-page: https://cns.ink/example
 Author: rambo
 Author-email: 6566666@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: python-dateutil
 
 ## cny
 cny公测专用库
 
 
 ## 安装方法
 pip install cny
```

