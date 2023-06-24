# Comparing `tmp/smunger-0.1.0.tar.gz` & `tmp/smunger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smunger-0.1.0.tar", max compression
+gzip compressed data, was "smunger-0.1.1.tar", max compression
```

## Comparing `smunger-0.1.0.tar` & `smunger-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1070 2023-06-14 06:12:39.224249 smunger-0.1.0/LICENSE
--rw-r--r--   0        0        0     2863 2023-06-14 06:12:39.224249 smunger-0.1.0/README.md
--rw-r--r--   0        0        0     3017 2023-06-14 06:12:39.228249 smunger-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      992 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/__init__.py
--rw-r--r--   0        0        0     2558 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/annotate.py
--rw-r--r--   0        0        0     6804 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/cli.py
--rw-r--r--   0        0        0       83 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/console.py
--rw-r--r--   0        0        0     6818 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/constant.py
--rw-r--r--   0        0        0     5060 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/io.py
--rw-r--r--   0        0        0     3993 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/liftover.py
--rw-r--r--   0        0        0     5611 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/mapheader.py
--rw-r--r--   0        0        0     3742 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/plots.py
--rw-r--r--   0        0        0    12800 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/smunger.py
--rw-r--r--   0        0        0       37 2023-06-14 06:12:39.228249 smunger-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1456 2023-06-14 06:12:39.228249 smunger-0.1.0/tests/annota_rsid_test.py
--rw-r--r--   0        0        0      269 2023-06-14 06:12:39.228249 smunger-0.1.0/tests/exampledata/catalog.header.json
--rw-r--r--   0        0        0   115228 2023-06-14 06:12:39.228249 smunger-0.1.0/tests/exampledata/catalog.munged.hg38.txt.gz
--rw-r--r--   0        0        0   502256 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/catalog.munged.rsid.txt
--rw-r--r--   0        0        0   120144 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/catalog.munged.txt.gz
--rw-r--r--   0        0        0     1931 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/catalog.munged.txt.gz.tbi
--rw-r--r--   0        0        0   124530 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/catalog.txt.gz
--rw-r--r--   0        0        0       72 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/test.header.json
--rw-r--r--   0        0        0    41670 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/test.munged.txt.gz
--rw-r--r--   0        0        0      738 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/test.munged.txt.gz.tbi
--rw-r--r--   0        0        0   789756 2023-06-14 06:12:39.236249 smunger-0.1.0/tests/exampledata/test.txt.gz
--rw-r--r--   0        0        0     5207 1970-01-01 00:00:00.000000 smunger-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-24 07:16:42.316497 smunger-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2863 2023-06-24 07:16:42.316497 smunger-0.1.1/README.md
+-rw-r--r--   0        0        0     3017 2023-06-24 07:16:42.320497 smunger-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      992 2023-06-24 07:16:42.320497 smunger-0.1.1/smunger/__init__.py
+-rw-r--r--   0        0        0     2558 2023-06-24 07:16:42.320497 smunger-0.1.1/smunger/annotate.py
+-rw-r--r--   0        0        0     6804 2023-06-24 07:16:42.320497 smunger-0.1.1/smunger/cli.py
+-rw-r--r--   0        0        0       83 2023-06-24 07:16:42.320497 smunger-0.1.1/smunger/console.py
+-rw-r--r--   0        0        0     6818 2023-06-24 07:16:42.320497 smunger-0.1.1/smunger/constant.py
+-rw-r--r--   0        0        0     5060 2023-06-24 07:16:42.320497 smunger-0.1.1/smunger/io.py
+-rw-r--r--   0        0        0     4007 2023-06-24 07:16:42.320497 smunger-0.1.1/smunger/liftover.py
+-rw-r--r--   0        0        0     5611 2023-06-24 07:16:42.320497 smunger-0.1.1/smunger/mapheader.py
+-rw-r--r--   0        0        0     3742 2023-06-24 07:16:42.320497 smunger-0.1.1/smunger/plots.py
+-rw-r--r--   0        0        0    12800 2023-06-24 07:16:42.320497 smunger-0.1.1/smunger/smunger.py
+-rw-r--r--   0        0        0       37 2023-06-24 07:16:42.320497 smunger-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1456 2023-06-24 07:16:42.320497 smunger-0.1.1/tests/annota_rsid_test.py
+-rw-r--r--   0        0        0      269 2023-06-24 07:16:42.320497 smunger-0.1.1/tests/exampledata/catalog.header.json
+-rw-r--r--   0        0        0   115228 2023-06-24 07:16:42.320497 smunger-0.1.1/tests/exampledata/catalog.munged.hg38.txt.gz
+-rw-r--r--   0        0        0   502256 2023-06-24 07:16:42.324497 smunger-0.1.1/tests/exampledata/catalog.munged.rsid.txt
+-rw-r--r--   0        0        0   120144 2023-06-24 07:16:42.324497 smunger-0.1.1/tests/exampledata/catalog.munged.txt.gz
+-rw-r--r--   0        0        0     1931 2023-06-24 07:16:42.324497 smunger-0.1.1/tests/exampledata/catalog.munged.txt.gz.tbi
+-rw-r--r--   0        0        0   124530 2023-06-24 07:16:42.324497 smunger-0.1.1/tests/exampledata/catalog.txt.gz
+-rw-r--r--   0        0        0       72 2023-06-24 07:16:42.324497 smunger-0.1.1/tests/exampledata/test.header.json
+-rw-r--r--   0        0        0    41670 2023-06-24 07:16:42.324497 smunger-0.1.1/tests/exampledata/test.munged.txt.gz
+-rw-r--r--   0        0        0      738 2023-06-24 07:16:42.324497 smunger-0.1.1/tests/exampledata/test.munged.txt.gz.tbi
+-rw-r--r--   0        0        0   789756 2023-06-24 07:16:42.328497 smunger-0.1.1/tests/exampledata/test.txt.gz
+-rw-r--r--   0        0        0     5207 1970-01-01 00:00:00.000000 smunger-0.1.1/PKG-INFO
```

### Comparing `smunger-0.1.0/LICENSE` & `smunger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/README.md` & `smunger-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/pyproject.toml` & `smunger-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "smunger"
-version = "0.1.0"
+version = "0.1.1"
 homepage = "https://github.com/jianhua/smunger"
 description = "munger for GWAS summary statistics."
 authors = ["Jianhua Wang <jianhua.mert@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `smunger-0.1.0/smunger/__init__.py` & `smunger-0.1.1/smunger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 )
 from .liftover import liftover, liftover_file
 from .annotate import annotate_rsid, annotate_rsid_file
 from .plots import qqplot, get_qq_df, manhattan, get_manh_df, qqman
 
 __author__ = """Jianhua Wang"""
 __email__ = 'jianhua.mert@gmail.com'
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 # Set up logging
 logging.basicConfig(
     level=logging.WARNING,
     format="%(name)s - %(message)s",
     datefmt="[%X]",
     handlers=[RichHandler(rich_tracebacks=True, show_path=False)],
```

### Comparing `smunger-0.1.0/smunger/annotate.py` & `smunger-0.1.1/smunger/annotate.py`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/smunger/cli.py` & `smunger-0.1.1/smunger/cli.py`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/smunger/constant.py` & `smunger-0.1.1/smunger/constant.py`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/smunger/io.py` & `smunger-0.1.1/smunger/io.py`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/smunger/liftover.py` & `smunger-0.1.1/smunger/liftover.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,8 +111,8 @@
     for df in pd.read_csv(infile, sep='\t', chunksize=chunksize):
         logger.info(f'processing chunk {ith}...')
         df = liftover(df, inbuild, outbuild, chrom_col, pos_col)
         ith += 1
         if ith == 1:
             df.to_csv(outfile, sep='\t', index=False)
         else:
-            df.to_csv(outfile, sep='\t', index=False, mode='a')
+            df.to_csv(outfile, sep='\t', index=False, mode='a', header=False)
```

### Comparing `smunger-0.1.0/smunger/mapheader.py` & `smunger-0.1.1/smunger/mapheader.py`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/smunger/plots.py` & `smunger-0.1.1/smunger/plots.py`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/smunger/smunger.py` & `smunger-0.1.1/smunger/smunger.py`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/tests/annota_rsid_test.py` & `smunger-0.1.1/tests/annota_rsid_test.py`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/tests/exampledata/catalog.munged.hg38.txt.gz` & `smunger-0.1.1/tests/exampledata/catalog.munged.hg38.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/tests/exampledata/catalog.munged.rsid.txt` & `smunger-0.1.1/tests/exampledata/catalog.munged.rsid.txt`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/tests/exampledata/catalog.munged.txt.gz` & `smunger-0.1.1/tests/exampledata/catalog.munged.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/tests/exampledata/catalog.munged.txt.gz.tbi` & `smunger-0.1.1/tests/exampledata/catalog.munged.txt.gz.tbi`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/tests/exampledata/catalog.txt.gz` & `smunger-0.1.1/tests/exampledata/catalog.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/tests/exampledata/test.munged.txt.gz` & `smunger-0.1.1/tests/exampledata/test.munged.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/tests/exampledata/test.munged.txt.gz.tbi` & `smunger-0.1.1/tests/exampledata/test.munged.txt.gz.tbi`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/tests/exampledata/test.txt.gz` & `smunger-0.1.1/tests/exampledata/test.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.1.0/PKG-INFO` & `smunger-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smunger
-Version: 0.1.0
+Version: 0.1.1
 Summary: munger for GWAS summary statistics.
 Home-page: https://github.com/jianhua/smunger
 License: MIT
 Author: Jianhua Wang
 Author-email: jianhua.mert@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

