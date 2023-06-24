# Comparing `tmp/even-dist-0.3.0.tar.gz` & `tmp/even_dist-0.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "even-dist-0.3.0.tar", last modified: Sat Jun 24 02:25:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

