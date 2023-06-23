# Comparing `tmp/bitalign-0.2.tar.gz` & `tmp/bitalign-0.3.0-pp39-pypy39_pp73-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitalign-0.2.tar", last modified: Wed Jun 14 21:37:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

