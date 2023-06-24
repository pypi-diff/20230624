# Comparing `tmp/sqlean.py-0.21.5-cp39-cp39-win_amd64.whl.zip` & `tmp/sqlean.py-0.21.5.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 759175 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      966 b- defN 23-Jun-15 15:07 sqlean/__init__.py
--rw-rw-rw-  2.0 fat  1484288 b- defN 23-Jun-15 15:16 sqlean/_sqlite3.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2700 b- defN 23-Jun-15 15:07 sqlean/dbapi2.py
--rw-rw-rw-  2.0 fat     2466 b- defN 23-Jun-15 15:16 sqlean.py-0.21.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-15 15:16 sqlean.py-0.21.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-15 15:16 sqlean.py-0.21.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      551 b- defN 23-Jun-15 15:16 sqlean.py-0.21.5.dist-info/RECORD
-7 files, 1491078 bytes uncompressed, 758205 bytes compressed:  49.2%
+Zip file size: 2836393 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 19:37 sqlean.py-0.21.5.1.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 19:37 sqlean.py.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 19:37 sqlean/
+-rw-rw-r--  2.0 unx      657 b- defN 23-Jun-24 19:37 sqlean.py-0.21.5.1.dist-info/RECORD
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-24 19:37 sqlean.py-0.21.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     4456 b- defN 23-Jun-24 19:37 sqlean.py-0.21.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-24 19:37 sqlean.py-0.21.5.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      996 b- defN 23-Jun-24 19:37 sqlean/__init__.py
+-rwxr-xr-x  2.0 unx  7782152 b- defN 23-Jun-24 19:37 sqlean/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     1123 b- defN 23-Jun-24 19:37 sqlean/extensions.py
+-rw-r--r--  2.0 unx     2700 b- defN 23-Jun-24 19:37 sqlean/dbapi2.py
+11 files, 7792241 bytes uncompressed, 2834935 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,22 +1,34 @@
-Filename: sqlean/__init__.py
+Filename: sqlean.py-0.21.5.1.dist-info/
 Comment: 
 
-Filename: sqlean/_sqlite3.cp39-win_amd64.pyd
+Filename: sqlean.py.libs/
 Comment: 
 
-Filename: sqlean/dbapi2.py
+Filename: sqlean/
+Comment: 
+
+Filename: sqlean.py-0.21.5.1.dist-info/RECORD
+Comment: 
+
+Filename: sqlean.py-0.21.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: sqlean.py-0.21.5.dist-info/METADATA
+Filename: sqlean.py-0.21.5.1.dist-info/METADATA
 Comment: 
 
-Filename: sqlean.py-0.21.5.dist-info/WHEEL
+Filename: sqlean.py-0.21.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlean.py-0.21.5.dist-info/top_level.txt
+Filename: sqlean/__init__.py
+Comment: 
+
+Filename: sqlean/_sqlite3.cpython-37m-x86_64-linux-gnu.so
 Comment: 
 
-Filename: sqlean.py-0.21.5.dist-info/RECORD
+Filename: sqlean/extensions.py
+Comment: 
+
+Filename: sqlean/dbapi2.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## sqlean/__init__.py

```diff
@@ -14,8 +14,9 @@
 #    claim that you wrote the original software. If you use this software
 #    in a product, an acknowledgment in the product documentation would be
 #    appreciated but is not required.
 # 2. Altered source versions must be plainly marked as such, and must not be
 #    misrepresented as being the original software.
 # 3. This notice may not be removed or altered from any source distribution.
 
+from sqlean import extensions
 from sqlean.dbapi2 import *
```

