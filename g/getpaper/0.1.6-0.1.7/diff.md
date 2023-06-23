# Comparing `tmp/getpaper-0.1.6.tar.gz` & `tmp/getpaper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.1.6.tar", last modified: Fri Jun 23 23:01:14 2023, max compression
+gzip compressed data, was "getpaper-0.1.7.tar", last modified: Fri Jun 23 23:35:10 2023, max compression
```

## Comparing `getpaper-0.1.6.tar` & `getpaper-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:01:14.544437 getpaper-0.1.6/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.6/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-23 23:01:14.544437 getpaper-0.1.6/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3876 2023-06-23 23:00:00.000000 getpaper-0.1.6/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:01:14.544437 getpaper-0.1.6/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.6/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     7695 2023-06-23 22:48:27.000000 getpaper-0.1.6/getpaper/download.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6249 2023-06-23 22:51:14.000000 getpaper-0.1.6/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    10895 2023-06-23 23:00:00.000000 getpaper-0.1.6/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.6/getpaper/splitter.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:01:14.544437 getpaper-0.1.6/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      201 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-23 23:01:14.544437 getpaper-0.1.6/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1586 2023-06-23 22:36:47.000000 getpaper-0.1.6/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:35:10.557100 getpaper-0.1.7/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.7/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-23 23:35:10.557100 getpaper-0.1.7/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3876 2023-06-23 23:00:00.000000 getpaper-0.1.7/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:35:10.557100 getpaper-0.1.7/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.7/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     7695 2023-06-23 22:48:27.000000 getpaper-0.1.7/getpaper/download.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6249 2023-06-23 22:51:14.000000 getpaper-0.1.7/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    11559 2023-06-23 23:31:19.000000 getpaper-0.1.7/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.7/getpaper/splitter.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:35:10.557100 getpaper-0.1.7/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      201 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-23 23:35:10.000000 getpaper-0.1.7/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-23 23:35:10.557100 getpaper-0.1.7/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1586 2023-06-23 23:32:37.000000 getpaper-0.1.7/setup.py
```

### Comparing `getpaper-0.1.6/LICENSE` & `getpaper-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.6/PKG-INFO` & `getpaper-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.6
+Version: 0.1.7
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.1.6/README.md` & `getpaper-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.6/getpaper/download.py` & `getpaper-0.1.7/getpaper/download.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.6/getpaper/index.py` & `getpaper-0.1.7/getpaper/index.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.6/getpaper/parse.py` & `getpaper-0.1.7/getpaper/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
 from typing import Optional, List, Dict
 
 import click
+import pynction.monads.try_monad
 import tiktoken
 from click import Context
 from functional import seq
 from langchain.document_loaders import UnstructuredPDFLoader
 from langchain.schema import Document
 from pycomfort.files import traverse
 from multiprocessing import Pool, cpu_count
 from functools import partial
 from deprecated import deprecated
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
 
+from pynction import Try
+
+
 def num_tokens_openai(string: str, model: str, price_per_1k: float = 0.0001) -> (int, float):
     """Returns the number of tokens for a model"""
     encoding = tiktoken.encoding_for_model(model)
     n_tokens = len(encoding.encode(string))
     return n_tokens, n_tokens / 1000.0 * price_per_1k
 
 """
@@ -36,30 +40,29 @@
 }
 
 
 def parse_paper(paper: Path, folder: Optional[Path] = None,
                 mode: str = "single", strategy: str = "auto",
                 pdf_infer_table_structure: bool = True,
                 include_page_breaks: bool = False, recreate_parent: bool = False
-                ):
+                ) -> List[Path]:
     """
     Parses the paper using Unstructured paper parser
     :param paper:
     :param folder:
     :param mode: can be single or paged
     :param recreate_parent: can be useful if we grouped papers by subfolders (for example for dois)
     :return:
     """
     bin_file = open(str(paper), "rb")
     loader = UnstructuredPDFLoader(file_path=None, file = bin_file,  mode=mode,
                                    pdf_infer_table_structure=pdf_infer_table_structure,
                                    strategy = strategy, include_page_breaks = include_page_breaks)
     where = paper.parent if folder is None else folder / paper.parent.name if recreate_parent else folder
     where.mkdir(parents=True, exist_ok=True)
-    print(f"WHERE IS {where} and recreate_parent is {recreate_parent}")
     docs: list[Document] = loader.load()
     if len(docs) ==1:
         name = f"{paper.stem}.txt"
         f = where / name
         print(f"writing {f}")
         f.write_text(docs[0].page_content)
         return [f]
@@ -69,14 +72,20 @@
             name = f"{paper.stem}_{i}.txt"
             f = (where / name)
             print(f"writing {f}")
             f.write_text(doc.page_content)
             acc.append(f)
         return acc
 
+def try_parse_paper(paper: Path, folder: Optional[Path] = None,
+                    mode: str = "single", strategy: str = "auto",
+                    pdf_infer_table_structure: bool = True,
+                    include_page_breaks: bool = False, recreate_parent: bool = False) -> Try[List[Path]]:
+    return Try.of(lambda: parse_paper(paper, folder, mode, strategy, pdf_infer_table_structure, include_page_breaks, recreate_parent))
+
 
 def parse_papers(parse_folder: Path, destination: Optional[Path] = None,
                  mode: str = "single", strategy: str = "auto",
                  pdf_infer_table_structure: bool = True,
                  include_page_breaks: bool = False, recreate_parent: bool = False, cores: Optional[int] = None):
     """
     Function to parse multiple papers using multiple cores.
@@ -95,25 +104,31 @@
 
     Returns:
         list[Path]: A list of paths to the parsed papers.
     """
     papers: list[Path] = traverse(parse_folder, lambda p: "pdf" in p.suffix)
     print(f"indexing {len(papers)} papers")
     acc = []
+    errors = []
 
     cores = cpu_count() if cores is None else min(cpu_count(), cores)
     with Pool(cores) as p:
-        parse_func = partial(parse_paper, folder=destination, mode=mode, strategy=strategy,
+        parse_func = partial(try_parse_paper, folder=destination, mode=mode, strategy=strategy,
                              pdf_infer_table_structure=pdf_infer_table_structure,
                              include_page_breaks=include_page_breaks, recreate_parent = recreate_parent)
         results = p.map(parse_func, papers)
         for result in results:
-            acc = acc + result
+            if isinstance(result, pynction.monads.try_monad.Success):
+                acc = acc + result._value
+            else:
+                errors = errors + result
 
     print("papers parsing finished!")
+    if len(errors) >0:
+        print(f"errors discovered: {errors}")
     return acc
 
 
 def papers_to_documents(folder: Path, suffix: str = ""):
     txt = traverse(folder, lambda p: "txt" in p.suffix)
     texts = [t for t in txt if suffix in t.name] if suffix != "" else txt
     docs: List[Document] = []
@@ -211,15 +226,15 @@
 @click.option('--destination', type=click.STRING, default=None, help="destination folder")
 @click.option('--mode', type=click.Choice(["single", "elements", "paged"]), default="single", help="paper mode to be used")
 @click.option('--strategy', type=click.Choice(["auto", "hi_res", "fast"]), default="auto", help="parsing strategy to be used, auto by default")
 @click.option('--infer_tables', type=click.BOOL, default=True, help="if the table structure should be inferred")
 @click.option('--include_page_breaks', type=click.BOOL, default=False, help="if page breaks should be included")
 @click.option('--cores', '-t', type=int, default=None, help='Number of cores to use')
 @click.option('--recreate_parent', type=click.BOOL, default=False, help="if parent folder should be recreated in the new destination")
-def parse_paper_command(folder: str,destination: str, mode: str, strategy: str, infer_tables: bool, include_page_breaks: bool, cores: Optional[int], recreate_parent: bool):
+def parse_paper_command(folder: str, destination: str, mode: str, strategy: str, infer_tables: bool, include_page_breaks: bool, cores: Optional[int], recreate_parent: bool):
     parse_folder = Path(folder)
     destination_folder = Path(destination) if destination is not None else None
     print(f"parsing paper {folder} with mode={mode} {'' if destination_folder is None else 'destination folder ' + destination}")
     return parse_papers(parse_folder, destination_folder, mode, strategy, infer_tables, include_page_breaks, recreate_parent, cores = cores)
 
 
 if __name__ == '__main__':
```

### Comparing `getpaper-0.1.6/getpaper/splitter.py` & `getpaper-0.1.7/getpaper/splitter.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.6/getpaper.egg-info/PKG-INFO` & `getpaper-0.1.7/getpaper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.6
+Version: 0.1.7
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.1.6/setup.py` & `getpaper-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
```

