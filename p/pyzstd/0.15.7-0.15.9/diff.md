# Comparing `tmp/pyzstd-0.15.7.tar.gz` & `tmp/pyzstd-0.15.9-cp37-cp37m-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzstd-0.15.7.tar", last modified: Fri Apr 21 12:31:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

