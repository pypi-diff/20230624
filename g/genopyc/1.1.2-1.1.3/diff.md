# Comparing `tmp/genopyc-1.1.2-py3-none-any.whl.zip` & `tmp/genopyc-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 424166 bytes, number of entries: 8
+Zip file size: 424167 bytes, number of entries: 8
 -rwxrwxrwx  2.0 unx      978 b- defN 23-Jun-24 20:45 genopyc/__init__.py
 -rwxrwxrwx  2.0 unx    42339 b- defN 23-Jun-24 20:43 genopyc/genopyc.py
 -rwxrwxrwx  2.0 unx  1302100 b- defN 23-Jun-21 11:17 genopyc/data/hippie_interactome.sif
--rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-24 20:45 genopyc-1.1.2.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-24 20:45 genopyc-1.1.2.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-24 20:45 genopyc-1.1.2.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-24 20:45 genopyc-1.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-24 20:45 genopyc-1.1.2.dist-info/RECORD
-8 files, 1381271 bytes uncompressed, 423066 bytes compressed:  69.4%
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-24 20:49 genopyc-1.1.3.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-24 20:49 genopyc-1.1.3.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-24 20:49 genopyc-1.1.3.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-24 20:49 genopyc-1.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-24 20:49 genopyc-1.1.3.dist-info/RECORD
+8 files, 1381271 bytes uncompressed, 423067 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: genopyc/genopyc.py
 Comment: 
 
 Filename: genopyc/data/hippie_interactome.sif
 Comment: 
 
-Filename: genopyc-1.1.2.dist-info/LICENSE.txt
+Filename: genopyc-1.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-1.1.2.dist-info/METADATA
+Filename: genopyc-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-1.1.2.dist-info/WHEEL
+Filename: genopyc-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-1.1.2.dist-info/top_level.txt
+Filename: genopyc-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-1.1.2.dist-info/RECORD
+Filename: genopyc-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `genopyc-1.1.2.dist-info/LICENSE.txt` & `genopyc-1.1.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `genopyc-1.1.2.dist-info/METADATA` & `genopyc-1.1.3.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genopyc
-Version: 1.1.2
+Version: 1.1.3
 Author: Francesco Gualdi
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: numpy
```

## Comparing `genopyc-1.1.2.dist-info/RECORD` & `genopyc-1.1.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 genopyc/__init__.py,sha256=njXl6cbbGkaY8POLyttPL5C6oBSA9LENNwW1zhzKHvE,978
 genopyc/genopyc.py,sha256=3vw1e-rk4Gim95VvxhiVKcRHO-FerVgcW8odIuWXEiI,42339
 genopyc/data/hippie_interactome.sif,sha256=iqdnCWTnTXIs43-jMLNijQ2PJWd7CRSVMHnh8miE1vs,1302100
-genopyc-1.1.2.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-genopyc-1.1.2.dist-info/METADATA,sha256=6MvecJcaFta_3mjudXny-VQNaeoKTck33qzJ406BGAI,596
-genopyc-1.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-genopyc-1.1.2.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
-genopyc-1.1.2.dist-info/RECORD,,
+genopyc-1.1.3.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+genopyc-1.1.3.dist-info/METADATA,sha256=WWjMK7jzfA_FP0cLNnS3nIQP3e2yB_M_WtCODdH1LVQ,596
+genopyc-1.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+genopyc-1.1.3.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
+genopyc-1.1.3.dist-info/RECORD,,
```

