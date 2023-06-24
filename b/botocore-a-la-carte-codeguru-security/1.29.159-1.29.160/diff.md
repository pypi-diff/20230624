# Comparing `tmp/botocore-a-la-carte-codeguru-security-1.29.159.tar.gz` & `tmp/botocore_a_la_carte_codeguru_security-1.29.160-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-codeguru-security-1.29.159.tar", last modified: Fri Jun 23 01:42:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

