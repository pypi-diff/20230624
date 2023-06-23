# Comparing `tmp/getpaper-0.1.4.tar.gz` & `tmp/getpaper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.1.4.tar", last modified: Fri Jun 23 01:02:25 2023, max compression
+gzip compressed data, was "getpaper-0.1.6.tar", last modified: Fri Jun 23 23:01:14 2023, max compression
```

## Comparing `getpaper-0.1.4.tar` & `getpaper-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 01:02:25.874754 getpaper-0.1.4/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.4/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3965 2023-06-23 01:02:25.874754 getpaper-0.1.4/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3350 2023-06-23 01:02:04.000000 getpaper-0.1.4/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 01:02:25.874754 getpaper-0.1.4/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.4/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     6949 2023-06-23 01:00:00.000000 getpaper-0.1.4/getpaper/download.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4452 2023-06-21 21:08:34.000000 getpaper-0.1.4/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     6795 2023-06-23 00:55:10.000000 getpaper-0.1.4/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.4/getpaper/splitter.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 01:02:25.874754 getpaper-0.1.4/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3965 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-23 01:02:25.000000 getpaper-0.1.4/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-23 01:02:25.874754 getpaper-0.1.4/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1572 2023-06-23 01:02:04.000000 getpaper-0.1.4/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:01:14.544437 getpaper-0.1.6/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.6/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-23 23:01:14.544437 getpaper-0.1.6/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3876 2023-06-23 23:00:00.000000 getpaper-0.1.6/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:01:14.544437 getpaper-0.1.6/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.6/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     7695 2023-06-23 22:48:27.000000 getpaper-0.1.6/getpaper/download.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6249 2023-06-23 22:51:14.000000 getpaper-0.1.6/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    10895 2023-06-23 23:00:00.000000 getpaper-0.1.6/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.6/getpaper/splitter.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-23 23:01:14.544437 getpaper-0.1.6/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4491 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      201 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-23 23:01:14.000000 getpaper-0.1.6/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-23 23:01:14.544437 getpaper-0.1.6/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1586 2023-06-23 22:36:47.000000 getpaper-0.1.6/setup.py
```

### Comparing `getpaper-0.1.4/LICENSE` & `getpaper-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.4/PKG-INFO` & `getpaper-0.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-Metadata-Version: 2.1
-Name: getpaper
-Version: 0.1.4
-Summary: getpaper - papers download made easy!
-Author: antonkulaga (Anton Kulaga)
-Author-email: <antonkulaga@gmail.com>
-Keywords: python,utils,files,papers,download
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # getpaper
 Paper downloader
 
 # getting started
 
 Install the library with:
 ```bash
 pip install getpaper
 ```
 
+On linux systems you sometimes need to check that build essentials are installed:
+```bash
+sudo apt install build-essential.
+```
+It is also recommended to use micromamba, conda, anaconda or other environments to avoid bloating system python with too many dependencies.
+
 # Usage
 ## Downloading papers
 
 After the installation you can either import the library into your python code or you can use the console scripts.
 
 If you install from pip calling download will mean calling getpaper/download.py , for parse - getpaper/parse.py , for index - getpaper/index.py
 
@@ -65,35 +53,43 @@
 Same function can be called from the command line:
 ```bash
 download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder "data/output/test/papers" --threads 5
 ```
 
 ## Parsing the papers
 
-You can parse the downloaded papers with the unstructure library. For example if the papers are in the folder test, you can run:
+You can parse the downloaded papers with the unstructured library. For example if the papers are in the folder test, you can run:
 ```bash
 getpaper/parse.py parse_folder --folder data/output/test/papers --threads 5
 ```
 You can also parse papers on a per-file basis, for example:
 ```bash
 getpaper/parse.py parse_paper --paper data/output/test/papers/10.3390/ijms22031073.pdf
 ```
 
+## Count tokens
+
+To evaluate how much you want to split texts and how much embeddings will cost you it is useful to compute token number:
+
+```bash
+getpaper/parse.py count_tokens --path /home/antonkulaga/sources/non-animal-models/data/inputs/datasets
+```
+
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
-For example if you have your papers inside data/output/test/papers folder and you want to make a ChromaDB index at data/output/test/index you can do it by:
+For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
 python getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
 
 Detectron2 is required for using models from the layoutparser model zoo but is not automatically installed with this package. 
-For MacOS and Linux, build from source with:
+For macOS and Linux, build from source with:
 
-pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
+pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
```

### Comparing `getpaper-0.1.4/getpaper/download.py` & `getpaper-0.1.6/getpaper/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,37 +78,48 @@
     """
     try_resolve = try_doi_from_pubmed(pubmed)
     return try_resolve.flat_map(lambda doi: try_download(doi, destination, skip_if_exist, name))
 
 
 async def try_download_async(executor: Executor, doi: str, destination: Path, skip_if_exist: bool = True, name: Optional[str] = None) -> (str, Path):
     """
-    downloads the paper by doi
-    :param executor: ThreadPoolExecutor to run blocking IO in
-    :param doi:
-    :param destination: where to put the results
-    :param skip_if_exist:
-    :param name:
-    :return: Try monad with the result
+    Asynchronously download a paper using its DOI.
+
+    Args:
+        executor (Executor): The ThreadPoolExecutor to run blocking IO in.
+        doi (str): The DOI of the paper to download.
+        destination (Path): The directory where the downloaded paper should be stored.
+        skip_if_exist (bool): If True, skip the download if the paper already exists in the destination. Default is True.
+        name (Optional[str]): The name of the file to save the paper as. If not provided, use the DOI. Default is None.
+
+    Returns:
+        (str, Path): A tuple containing the DOI of the paper and the path to the downloaded paper.
     """
+
+    # Construct the URL for the paper using the DOI
     doi_url = f"https://doi.org/{doi}"
     paper = (destination / f"{doi}.pdf").absolute().resolve() if name is None else (destination / f"{name.replace(',pdf', '')}.pdf").absolute().resolve()
 
+    # If the paper already exists and we are skipping existing papers, return the DOI and path
     if skip_if_exist and paper.exists():
         print(f"Paper {paper} for {doi} already exists!")
         return doi, paper
 
+    # Get a reference to the current event loop
     loop = asyncio.get_event_loop()
 
     def blocking_io():
+        # Download the paper
+        # This is a blocking IO operation, so it's run in the executor
         scihub_download(doi_url, paper_type="doi", out=str(paper))
         return paper  # Explicitly return the path of the downloaded file
 
     _ = await loop.run_in_executor(executor, blocking_io)
 
+    # Return the DOI and path to the downloaded paper
     return doi, Path
 
 
 def download_papers(dois: List[str], destination: Path, threads: int) -> (OrderedDict[str, Path], List[str]):
     """
     :param dois: List of DOIs of the papers to download
     :param destination: Directory where to put the downloaded papers
@@ -118,16 +129,16 @@
     # Create a ThreadPoolExecutor with desired number of threads
     with ThreadPoolExecutor(max_workers=threads) as executor:
         # Create a coroutine for each download
         coroutines = [try_download_async(executor, doi, destination) for doi in dois]
 
         # Get the current event loop, run the downloads, and wait for all of them to finish
         loop = asyncio.get_event_loop()
-        downloaded: List[str, Path] = loop.run_until_complete(asyncio.gather(*coroutines))
-    partitions: List[List[str, Path]] = seq(downloaded).partition(lambda kv: isinstance(kv[1], Path)).to_list()
+        downloaded: List[(str, Path)] = loop.run_until_complete(asyncio.gather(*coroutines))
+    partitions: List[List[(str, Path)]] = seq(downloaded).partition(lambda kv: isinstance(kv[1], Path)).to_list()
     return OrderedDict(partitions[0]), [kv[0] for kv in partitions[1]]
 
 
 
 @click.group(invoke_without_command=False)
 @click.pass_context
 def app(ctx: Context):
```

### Comparing `getpaper-0.1.4/getpaper/splitter.py` & `getpaper-0.1.6/getpaper/splitter.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.4/getpaper.egg-info/PKG-INFO` & `getpaper-0.1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.4
+Version: 0.1.6
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -22,14 +22,20 @@
 # getting started
 
 Install the library with:
 ```bash
 pip install getpaper
 ```
 
+On linux systems you sometimes need to check that build essentials are installed:
+```bash
+sudo apt install build-essential.
+```
+It is also recommended to use micromamba, conda, anaconda or other environments to avoid bloating system python with too many dependencies.
+
 # Usage
 ## Downloading papers
 
 After the installation you can either import the library into your python code or you can use the console scripts.
 
 If you install from pip calling download will mean calling getpaper/download.py , for parse - getpaper/parse.py , for index - getpaper/index.py
 
@@ -65,35 +71,43 @@
 Same function can be called from the command line:
 ```bash
 download download_papers --dois "10.3390/ijms22031073" --dois "10.1038/s41597-020-00710-z" --dois "wrong" --folder "data/output/test/papers" --threads 5
 ```
 
 ## Parsing the papers
 
-You can parse the downloaded papers with the unstructure library. For example if the papers are in the folder test, you can run:
+You can parse the downloaded papers with the unstructured library. For example if the papers are in the folder test, you can run:
 ```bash
 getpaper/parse.py parse_folder --folder data/output/test/papers --threads 5
 ```
 You can also parse papers on a per-file basis, for example:
 ```bash
 getpaper/parse.py parse_paper --paper data/output/test/papers/10.3390/ijms22031073.pdf
 ```
 
+## Count tokens
+
+To evaluate how much you want to split texts and how much embeddings will cost you it is useful to compute token number:
+
+```bash
+getpaper/parse.py count_tokens --path /home/antonkulaga/sources/non-animal-models/data/inputs/datasets
+```
+
 ## Indexing papers
 
 We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
-For example if you have your papers inside data/output/test/papers folder and you want to make a ChromaDB index at data/output/test/index you can do it by:
+For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
 python getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
 
 Detectron2 is required for using models from the layoutparser model zoo but is not automatically installed with this package. 
-For MacOS and Linux, build from source with:
+For macOS and Linux, build from source with:
 
 pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
```

### Comparing `getpaper-0.1.4/setup.py` & `getpaper-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.4'
+VERSION = '0.1.6'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
@@ -19,15 +19,15 @@
     author_email="<antonkulaga@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=['pyfunctional', 'more-itertools', 'click', 'python-dotenv', 'tiktoken', 'pynction',
                       'unstructured', 'unstructured-inference', 'unstructured[local-inference]', 'unstructured.PaddleOCR',
-                      'scidownl', 'langchain', 'openai', 'chromadb'],
+                      'scidownl', 'langchain', 'openai', 'chromadb', 'Deprecated'],
     keywords=['python', 'utils', 'files', 'papers', 'download'],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         "Operating System :: Unix",
```

