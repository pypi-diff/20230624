# Comparing `tmp/getpaper-0.1.7.tar.gz` & `tmp/getpaper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.1.7.tar", last modified: Fri Jun 23 23:35:10 2023, max compression
+gzip compressed data, was "getpaper-0.1.8.tar", last modified: Sat Jun 24 00:24:34 2023, max compression
```

## Comparing `getpaper-0.1.7.tar` & `getpaper-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:35:10.557100 getpaper-0.1.7/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.7/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-23 23:35:10.557100 getpaper-0.1.7/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3876 2023-06-23 23:00:00.000000 getpaper-0.1.7/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:35:10.557100 getpaper-0.1.7/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.7/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     7695 2023-06-23 22:48:27.000000 getpaper-0.1.7/getpaper/download.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6249 2023-06-23 22:51:14.000000 getpaper-0.1.7/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    11559 2023-06-23 23:31:19.000000 getpaper-0.1.7/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.7/getpaper/splitter.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:35:10.557100 getpaper-0.1.7/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      201 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-23 23:35:10.557100 getpaper-0.1.7/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1586 2023-06-23 23:32:37.000000 getpaper-0.1.7/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-24 00:24:34.633205 getpaper-0.1.8/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.8/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-24 00:24:34.633205 getpaper-0.1.8/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3876 2023-06-23 23:00:00.000000 getpaper-0.1.8/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-24 00:24:34.633205 getpaper-0.1.8/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.8/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     7695 2023-06-23 22:48:27.000000 getpaper-0.1.8/getpaper/download.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6249 2023-06-23 22:51:14.000000 getpaper-0.1.8/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    11749 2023-06-24 00:24:03.000000 getpaper-0.1.8/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.8/getpaper/splitter.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-24 00:24:34.633205 getpaper-0.1.8/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      201 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-24 00:24:34.000000 getpaper-0.1.8/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-24 00:24:34.633205 getpaper-0.1.8/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1586 2023-06-24 00:24:17.000000 getpaper-0.1.8/setup.py
```

### Comparing `getpaper-0.1.7/LICENSE` & `getpaper-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.7/PKG-INFO` & `getpaper-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.7
+Version: 0.1.8
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.1.7/README.md` & `getpaper-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.7/getpaper/download.py` & `getpaper-0.1.8/getpaper/download.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.7/getpaper/index.py` & `getpaper-0.1.8/getpaper/index.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.7/getpaper/parse.py` & `getpaper-0.1.8/getpaper/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,37 +99,39 @@
         strategy (str): The strategy to parse the papers. Default is "auto".
         pdf_infer_table_structure (bool): If True, attempts to infer table structure in PDFs. Default is True.
         include_page_breaks (bool): If True, includes page breaks in the parsed output. Default is False.
         recreate_parent (bool): If True, recreates the parent directory structure in the destination folder. Default is False.
         cores (Optional[int]): The number of cores to use. If not provided, uses all available cores.
 
     Returns:
-        list[Path]: A list of paths to the parsed papers.
+        list[Path], list[Failure]: A list of paths to the parsed papers and a list of Failtures
     """
     papers: list[Path] = traverse(parse_folder, lambda p: "pdf" in p.suffix)
     print(f"indexing {len(papers)} papers")
-    acc = []
+    parsed = []
     errors = []
 
     cores = cpu_count() if cores is None else min(cpu_count(), cores)
     with Pool(cores) as p:
         parse_func = partial(try_parse_paper, folder=destination, mode=mode, strategy=strategy,
                              pdf_infer_table_structure=pdf_infer_table_structure,
                              include_page_breaks=include_page_breaks, recreate_parent = recreate_parent)
         results = p.map(parse_func, papers)
         for result in results:
             if isinstance(result, pynction.monads.try_monad.Success):
-                acc = acc + result._value
+                parsed = parsed + result._value
+            elif isinstance(result, pynction.monads.try_monad.Failure):
+                errors.append(result._e)
             else:
-                errors = errors + result
+                print(f"unpredicted type of the {result}")
 
     print("papers parsing finished!")
     if len(errors) >0:
         print(f"errors discovered: {errors}")
-    return acc
+    return results, errors
 
 
 def papers_to_documents(folder: Path, suffix: str = ""):
     txt = traverse(folder, lambda p: "txt" in p.suffix)
     texts = [t for t in txt if suffix in t.name] if suffix != "" else txt
     docs: List[Document] = []
     for t in texts:
```

### Comparing `getpaper-0.1.7/getpaper/splitter.py` & `getpaper-0.1.8/getpaper/splitter.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.7/getpaper.egg-info/PKG-INFO` & `getpaper-0.1.8/getpaper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.7
+Version: 0.1.8
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.1.7/setup.py` & `getpaper-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
```

