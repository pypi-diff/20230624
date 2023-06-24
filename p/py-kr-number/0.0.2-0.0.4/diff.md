# Comparing `tmp/py_kr_number-0.0.2-py3-none-any.whl.zip` & `tmp/py_kr_number-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3647 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     2639 b- defN 23-Jun-24 08:10 pkn.py
--rw-rw-rw-  2.0 fat     1088 b- defN 23-Jun-24 08:44 py_kr_number-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      796 b- defN 23-Jun-24 08:44 py_kr_number-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-24 08:44 py_kr_number-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-24 08:44 py_kr_number-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      472 b- defN 23-Jun-24 08:44 py_kr_number-0.0.2.dist-info/RECORD
-6 files, 5091 bytes uncompressed, 2789 bytes compressed:  45.2%
+Zip file size: 3641 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     2635 b- defN 23-Jun-24 09:11 pkn.py
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Jun-24 09:23 py_kr_number-0.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      796 b- defN 23-Jun-24 09:23 py_kr_number-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-24 09:23 py_kr_number-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-24 09:23 py_kr_number-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      472 b- defN 23-Jun-24 09:23 py_kr_number-0.0.4.dist-info/RECORD
+6 files, 5087 bytes uncompressed, 2783 bytes compressed:  45.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pkn.py
 Comment: 
 
-Filename: py_kr_number-0.0.2.dist-info/LICENSE
+Filename: py_kr_number-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: py_kr_number-0.0.2.dist-info/METADATA
+Filename: py_kr_number-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: py_kr_number-0.0.2.dist-info/WHEEL
+Filename: py_kr_number-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: py_kr_number-0.0.2.dist-info/top_level.txt
+Filename: py_kr_number-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: py_kr_number-0.0.2.dist-info/RECORD
+Filename: py_kr_number-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pkn.py

```diff
@@ -66,13 +66,13 @@
         elif count == 16:
             list_1.append("경")
         elif count == 20:
             list_1.append("해")
         list_1.append(r_str[i])
         count += 1
     list_1.reverse()
-    list_1.append("원")
+    list_1.append(end)
     return ''.join(list_1)
 def help_pkn():
     print("====<help>====")
     print("> convert(numberm, won)")
-    print("> help()")
+    print("> help()")
```

## Comparing `py_kr_number-0.0.2.dist-info/LICENSE` & `py_kr_number-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `py_kr_number-0.0.2.dist-info/METADATA` & `py_kr_number-0.0.4.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-kr-number
-Version: 0.0.2
+Version: 0.0.4
 Summary: Simple Korean unit conversion module
 Home-page: https://github.com/yeokyoomin/py_kr_number.git
 Author: yeokyoomin
 Author-email: msdhgoom@gmail.com
 License: yeokyoomin
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

