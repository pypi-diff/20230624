# Comparing `tmp/git2doc-0.2.1.tar.gz` & `tmp/git2doc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2doc-0.2.1.tar", last modified: Mon Jun 19 12:53:56 2023, max compression
+gzip compressed data, was "git2doc-0.2.2.tar", last modified: Sat Jun 24 21:15:37 2023, max compression
```

## Comparing `git2doc-0.2.1.tar` & `git2doc-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 12:53:56.852321 git2doc-0.2.1/
--rw-rw-rw-   0        0        0     3025 2023-06-19 12:53:56.850814 git2doc-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2356 2023-06-19 12:51:41.000000 git2doc-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 12:53:56.838128 git2doc-0.2.1/git2doc/
--rw-rw-rw-   0        0        0        0 2023-06-19 12:51:41.000000 git2doc-0.2.1/git2doc/__init__.py
--rw-rw-rw-   0        0        0     9322 2023-06-19 12:52:26.000000 git2doc-0.2.1/git2doc/loader.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:53:56.848832 git2doc-0.2.1/git2doc.egg-info/
--rw-rw-rw-   0        0        0     3025 2023-06-19 12:53:56.000000 git2doc-0.2.1/git2doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-06-19 12:53:56.000000 git2doc-0.2.1/git2doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 12:53:56.000000 git2doc-0.2.1/git2doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-19 12:53:56.000000 git2doc-0.2.1/git2doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 12:53:56.000000 git2doc-0.2.1/git2doc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 12:53:56.853328 git2doc-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      983 2023-06-19 12:53:22.000000 git2doc-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:15:37.174569 git2doc-0.2.2/
+-rw-rw-rw-   0        0        0     2588 2023-06-24 21:15:37.172570 git2doc-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1919 2023-06-19 20:38:01.000000 git2doc-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 21:15:37.159569 git2doc-0.2.2/git2doc/
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:38:01.000000 git2doc-0.2.2/git2doc/__init__.py
+-rw-rw-rw-   0        0        0    12158 2023-06-24 21:15:09.000000 git2doc-0.2.2/git2doc/loader.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:15:37.169574 git2doc-0.2.2/git2doc.egg-info/
+-rw-rw-rw-   0        0        0     2588 2023-06-24 21:15:37.000000 git2doc-0.2.2/git2doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-24 21:15:37.000000 git2doc-0.2.2/git2doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 21:15:37.000000 git2doc-0.2.2/git2doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-24 21:15:37.000000 git2doc-0.2.2/git2doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-24 21:15:37.000000 git2doc-0.2.2/git2doc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 21:15:37.175569 git2doc-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2023-06-24 21:15:30.000000 git2doc-0.2.2/setup.py
```

### Comparing `git2doc-0.2.1/PKG-INFO` & `git2doc-0.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,81 @@
 Metadata-Version: 2.1
 Name: git2doc
-Version: 0.2.1
+Version: 0.2.2
 Summary: A tool for converting git repositories into documents
 Home-page: https://github.com/voynow/git2doc
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# Git2Doc
+# Git2Doc 📚
 
-Git2Doc is a Python package for handling Git data. It provides functionality to load and process Git repositories, and supports concurrent file loading for improved performance. The package can be found on [PyPI](https://pypi.org/project/git2doc/).
+[![PyPI version](https://badge.fury.io/py/git2doc.svg)](https://pypi.org/project/git2doc/)
+
+Git2Doc is a Python package that allows you to convert git repositories into documents. It is designed to help developers analyze and understand codebases by providing an easy way to extract and process text content from git repositories.
 
 ## Table of Contents
 
 - [Installation](#installation)
-- [Setup](#setup)
 - [Usage](#usage)
-  - [Loading Git Repositories](#loading-git-repositories)
-  - [Getting Top Repositories](#getting-top-repositories)
-  - [Pipeline Fetch and Load](#pipeline-fetch-and-load)
+  - [Example: Fetch and Load Repositories](#example-fetch-and-load-repositories)
+  - [Example: Get Top Repositories](#example-get-top-repositories)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Installation
 
-To install Git2Doc, run the following command:
+To install Git2Doc, simply run:
 
 ```bash
 pip install git2doc
 ```
 
-## Setup
-
-Before using Git2Doc, make sure to have the following dependencies installed:
-
-- langchain
-- tiktoken
-- gitpython
-- python-dotenv
-- pandas
-
-You can install them using the following command:
-
-```bash
-pip install -r requirements.txt
-```
-
 ## Usage
 
-### Loading Git Repositories
-
-The main functionality of Git2Doc is provided by the `loader.py` module. Here's an example of how to use the `pull_code_from_repo` function to load a Git repository:
+### Example: Fetch and Load Repositories
 
 ```python
-from git2doc.loader import pull_code_from_repo
+from git2doc.loader import pipeline_fetch_and_load
 
-repo_url = "https://github.com/username/repo.git"
-branch = "main"
+# Fetch and load the top 5 repositories created in the last 7 days
+github_data = pipeline_fetch_and_load(n_repos=5, last_n_days=7)
 
-repo_data = pull_code_from_repo(repo_url, branch)
+# Print the metadata and documents for each repository
+for repo_key, repo_data in github_data.items():
+    print(f"Repository: {repo_key}")
+    print("Metadata:")
+    for key, value in repo_data["metadata"].items():
+        print(f"  {key}: {value}")
+    print("Documents:")
+    for doc in repo_data["docs"]:
+        print(f"  {doc.metadata['file_path']}: {doc.page_content[:50]}...")
 ```
 
-### Getting Top Repositories
-
-You can use the `get_top_repos` function to fetch the top repositories based on certain criteria:
+### Example: Get Top Repositories
 
 ```python
 from git2doc.loader import get_top_repos
 
-n_repos = 10
-last_n_days = 30
-language = "Python"
-sort = "stars"
-order = "desc"
-
-top_repos = get_top_repos(n_repos, last_n_days, language, sort, order)
-```
-
-### Pipeline Fetch and Load
-
-The `pipeline_fetch_and_load` function can be used to fetch and load repositories in a single step:
-
-```python
-from git2doc.loader import pipeline_fetch_and_load
-
-n_repos = 10
-last_n_days = 30
-language = "Python"
-sort = "stars"
-order = "desc"
+# Get the top 5 Python repositories created in the last 7 days
+top_repos = get_top_repos(n_repos=5, last_n_days=7, language="Python")
 
-github_data = pipeline_fetch_and_load(n_repos, last_n_days, language, sort, order)
+# Print the repository URLs
+for repo in top_repos:
+    print(repo["html_url"])
 ```
 
 ## Contributing
 
-If you'd like to contribute to Git2Doc, feel free to fork the repository and submit a pull request. If you have any questions or issues, please open an issue on the GitHub repository.
+Contributions are welcome! Please feel free to submit a pull request or open an issue on GitHub.
 
 ## License
 
-Git2Doc is released under the MIT License.
+Git2Doc is released under the [MIT License](https://opensource.org/licenses/MIT).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `git2doc-0.2.1/README.md` & `git2doc-0.2.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,64 @@
-# Git2Doc
+# Git2Doc 📚
 
-Git2Doc is a Python package for handling Git data. It provides functionality to load and process Git repositories, and supports concurrent file loading for improved performance. The package can be found on [PyPI](https://pypi.org/project/git2doc/).
+[![PyPI version](https://badge.fury.io/py/git2doc.svg)](https://pypi.org/project/git2doc/)
+
+Git2Doc is a Python package that allows you to convert git repositories into documents. It is designed to help developers analyze and understand codebases by providing an easy way to extract and process text content from git repositories.
 
 ## Table of Contents
 
 - [Installation](#installation)
-- [Setup](#setup)
 - [Usage](#usage)
-  - [Loading Git Repositories](#loading-git-repositories)
-  - [Getting Top Repositories](#getting-top-repositories)
-  - [Pipeline Fetch and Load](#pipeline-fetch-and-load)
+  - [Example: Fetch and Load Repositories](#example-fetch-and-load-repositories)
+  - [Example: Get Top Repositories](#example-get-top-repositories)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Installation
 
-To install Git2Doc, run the following command:
+To install Git2Doc, simply run:
 
 ```bash
 pip install git2doc
 ```
 
-## Setup
-
-Before using Git2Doc, make sure to have the following dependencies installed:
-
-- langchain
-- tiktoken
-- gitpython
-- python-dotenv
-- pandas
-
-You can install them using the following command:
-
-```bash
-pip install -r requirements.txt
-```
-
 ## Usage
 
-### Loading Git Repositories
-
-The main functionality of Git2Doc is provided by the `loader.py` module. Here's an example of how to use the `pull_code_from_repo` function to load a Git repository:
+### Example: Fetch and Load Repositories
 
 ```python
-from git2doc.loader import pull_code_from_repo
+from git2doc.loader import pipeline_fetch_and_load
 
-repo_url = "https://github.com/username/repo.git"
-branch = "main"
+# Fetch and load the top 5 repositories created in the last 7 days
+github_data = pipeline_fetch_and_load(n_repos=5, last_n_days=7)
 
-repo_data = pull_code_from_repo(repo_url, branch)
+# Print the metadata and documents for each repository
+for repo_key, repo_data in github_data.items():
+    print(f"Repository: {repo_key}")
+    print("Metadata:")
+    for key, value in repo_data["metadata"].items():
+        print(f"  {key}: {value}")
+    print("Documents:")
+    for doc in repo_data["docs"]:
+        print(f"  {doc.metadata['file_path']}: {doc.page_content[:50]}...")
 ```
 
-### Getting Top Repositories
-
-You can use the `get_top_repos` function to fetch the top repositories based on certain criteria:
+### Example: Get Top Repositories
 
 ```python
 from git2doc.loader import get_top_repos
 
-n_repos = 10
-last_n_days = 30
-language = "Python"
-sort = "stars"
-order = "desc"
-
-top_repos = get_top_repos(n_repos, last_n_days, language, sort, order)
-```
-
-### Pipeline Fetch and Load
-
-The `pipeline_fetch_and_load` function can be used to fetch and load repositories in a single step:
-
-```python
-from git2doc.loader import pipeline_fetch_and_load
-
-n_repos = 10
-last_n_days = 30
-language = "Python"
-sort = "stars"
-order = "desc"
+# Get the top 5 Python repositories created in the last 7 days
+top_repos = get_top_repos(n_repos=5, last_n_days=7, language="Python")
 
-github_data = pipeline_fetch_and_load(n_repos, last_n_days, language, sort, order)
+# Print the repository URLs
+for repo in top_repos:
+    print(repo["html_url"])
 ```
 
 ## Contributing
 
-If you'd like to contribute to Git2Doc, feel free to fork the repository and submit a pull request. If you have any questions or issues, please open an issue on the GitHub repository.
+Contributions are welcome! Please feel free to submit a pull request or open an issue on GitHub.
 
 ## License
 
-Git2Doc is released under the MIT License.
+Git2Doc is released under the [MIT License](https://opensource.org/licenses/MIT).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `git2doc-0.2.1/git2doc/loader.py` & `git2doc-0.2.2/git2doc/loader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import concurrent.futures
 from datetime import datetime, timedelta
 import dotenv
-import gc
 from git import Blob, Repo
-from git.exc import InvalidGitRepositoryError
+from git.exc import InvalidGitRepositoryError, GitCommandError
 import os
+import math
 from pathlib import Path
+import polars as pl
 import requests
 import shutil
 import stat
-from typing import Callable, List, Optional, Dict
-
-from langchain.docstore.document import Document
+import time
+from typing import List, Optional, Dict
 
 
 UNWANTED_TYPES = [
     ".ipynb",
     ".yaml",
     ".yml",
     ".json",
@@ -29,19 +29,38 @@
     ".jsonl",
     ".struct",
     ".map",
     ".obj",
     ".cleaned",
     ".dict",
     ".GIF",
+    ".tiktoken",
+    ".lock",
+    ".pack",
+    ".sub",
+    ".zh_CN",
+    ".dae",
+    ".zh_CN_tgt",
+    ".dat",
+    ".tsv",
+    ".tokens",
+    ".off",
+    ".sense",
+    ".log",
+    ".bvh",
+    ".onnx",
+    ".gltf",
+    ".cif",
+    ".geojson",
+    "pkl",
 ]
 REPODATA_FOLDER = "./repodata/"
 
 
-def load_file(item, output_path) -> Optional[Document]:
+def load_file(item, output_path) -> Optional[dict]:
     """
     Loads a single file from the repository.
 
     :param item: The file to load.
     :return: The document or None if the file should be skipped.
     """
     if not isinstance(item, Blob):
@@ -59,46 +78,44 @@
             file_type = os.path.splitext(item.name)[1]
 
             try:
                 text_content = content.decode("utf-8")
             except UnicodeDecodeError:
                 return None
 
-            metadata = {
+            return {
+                "page_content": text_content,
                 "file_path": rel_file_path,
                 "file_name": item.name,
                 "file_type": file_type,
             }
-            doc = Document(page_content=text_content, metadata=metadata)
-            return doc
     except Exception as e:
-        print(f"Error reading file {file_path}: {e}")
         return None
 
 
-def load_concurrently(repo, output_path) -> List[Document]:
+def load_concurrently(repo, output_path) -> List[dict]:
     """
     Loads all files from the repository in parallel.
 
     :return: A list of documents
     """
 
-    docs: List[Document] = []
+    files: List[dict] = []
     with concurrent.futures.ThreadPoolExecutor() as executor:
         future_to_item = {
             executor.submit(load_file, item, output_path): item
             for item in repo.tree().traverse()
         }
         for future in concurrent.futures.as_completed(future_to_item):
-            doc = future.result()
-            if doc is not None:
-                docs.append(doc)
+            file = future.result()
+            if file is not None:
+                files.append(file)
         executor.shutdown(wait=True)
 
-    return docs
+    return files
 
 
 def git_pull(clone_url, branch, output_path):
     """
     Pull the repo if it exists, otherwise clone it
 
     :param output_path: local path to output
@@ -117,20 +134,22 @@
             allow_unsafe_options=True,
             multi_options=["--config", "lfs.fetchexclude=*"],
         )
         repo.git.checkout(branch)
     return repo
 
 
-def docs_to_str(repo_data):
+def files_to_str(repo_data):
     """Convert repo data to raw text"""
     raw_repo = ""
     for item in repo_data:
-        if item.page_content:
-            raw_repo += f"{item.metadata['file_path']}:\n\n{item.page_content}\n\n"
+        if "page_content" in item:
+            raw_repo += (
+                f"{item['metadata']['file_path']}:\n\n{item['page_content']}\n\n"
+            )
     return raw_repo
 
 
 def readonly_to_writable(fn, file, err):
     """Exception handler for OS error on rmtree"""
     if Path(file).suffix in [".idx", ".pack"] and "PermissionError" == err[0].__name__:
         os.chmod(file, stat.S_IWRITE)
@@ -146,20 +165,21 @@
     :param return_str: return raw text or not
     """
     folder_name = "/".join(repo.split("/")[3:5])
     output_path = f"{REPODATA_FOLDER}{folder_name}/"
 
     # git pull, load, and delete repo
     repo = git_pull(repo, branch, output_path)
-    repo_docs = load_concurrently(repo, output_path)
+    repo_files = load_concurrently(repo, output_path)
+    repo.close()
 
     if delete:
         shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
 
-    return repo_docs
+    return repo_files
 
 
 def flatten_dict(dd, separator="_", prefix=""):
     """
     Flattens a dictionary with nested structures
 
     :param dd: Input dictionary to be flattened
@@ -185,20 +205,77 @@
     if not access_token:
         raise ValueError(
             "ACCESS_TOKEN not found. Either create a .env file or set the environment variable."
         )
     return access_token
 
 
-def get_top_repos(
+def get_time_intervals(last_n_days, n_intervals):
+    """
+    Divide the last_n_days into n_intervals based on number of repositories.
+    """
+    days_per_interval = last_n_days // n_intervals
+    end_date = datetime.now()
+    start_date = end_date - timedelta(days=last_n_days)
+
+    intervals = []
+    for _ in range(n_intervals):
+        next_date = min(start_date + timedelta(days=days_per_interval), end_date)
+        intervals.append(
+            (start_date.strftime("%Y-%m-%d"), next_date.strftime("%Y-%m-%d"))
+        )
+        start_date = next_date
+
+    return intervals
+
+
+def run_repos_query(url, headers, query, repo_batch_size, max_retries=3, retry_delay=5):
+    """Given a query, return a repo metadata"""
+    repos = []
+    page = 1
+
+    while len(repos) < repo_batch_size:
+        params = {
+            "q": query,
+            "sort": "stars",
+            "order": "desc",
+            "per_page": 100,
+            "page": page,
+        }
+        with requests.Session() as session:
+            session.headers.update(headers)
+
+            retries = 0
+            while retries < max_retries:
+                try:
+                    response = session.get(url, params=params)
+                    response.raise_for_status()
+                    data = response.json()
+                    repos.extend(data.get("items", []))
+                    break
+                except Exception:
+                    pass
+
+                retries += 1
+                if retries < max_retries:
+                    time.sleep(retry_delay)
+                else:
+                    if page >= 10:
+                        print(
+                            f"Failed to get repos after 10 pages. Returning {len(repos)} repos."
+                        )
+                        return repos[:repo_batch_size]
+        page += 1
+    return repos[:repo_batch_size]
+
+
+def get_repos_orchestrator(
     n_repos: int,
     last_n_days: int,
     language: str = None,
-    sort: str = "stars",
-    order: str = "desc",
 ) -> Dict[str, Dict]:
     """
     Query for repos created in the last n days
 
     :param n_repos: Number of repos to return
     :param last_n_days: Number of days to look back
     :param language: Language to filter by
@@ -208,111 +285,126 @@
     """
     access_token = get_access_token()
     url = "https://api.github.com/search/repositories"
     headers = {
         "Accept": "application/vnd.github.v3+json",
         "Authorization": f"Bearer {access_token}",
     }
+    base_query = f"language:{language}" if language else "is:public"
 
-    query = f"language:{language}" if language else "is:public"
-    date_since = (datetime.now() - timedelta(days=last_n_days)).strftime("%Y-%m-%d")
-    query += f" created:>{date_since}"
+    n_intervals = math.ceil(n_repos / 900) if n_repos > 900 else 1
+    intervals = get_time_intervals(last_n_days, n_intervals)
+    repo_batch_size = n_repos // n_intervals
+    print(
+        f"Querying {n_repos} repos, this will be done in {n_intervals} batches"
+    )
 
     repos = []
-    page = 1
-    while len(repos) < n_repos:
-        params = {
-            "q": query,
-            "sort": sort,
-            "order": order,
-            "per_page": 100,
-            "page": page,
-        }
+    for start_date, end_date in intervals:
+        query = f"{base_query} created:{start_date}..{end_date}"
+        print(f"Query: {repo_batch_size} repos on {start_date} -> {end_date}")
 
-        with requests.Session() as session:
-            session.headers.update(headers)
-            try:
-                response = session.get(url, params=params)
-                response.raise_for_status()
-                data = response.json()
-                repos.extend(data.get("items", []))
-            except requests.exceptions.HTTPError as errh:
-                print(f"HTTP Error: {errh}")
-            except requests.exceptions.ConnectionError as errc:
-                print(f"Error Connecting: {errc}")
-            except requests.exceptions.Timeout as errt:
-                print(f"Timeout Error: {errt}")
-            except requests.exceptions.RequestException as err:
-                print(f"Unknown Error: {err}")
-                break
-
-        # Increment the page number for the next iteration
-        page += 1
+        batch = run_repos_query(url, headers, query, repo_batch_size)
+        repos.extend(batch)
 
-    # Return only the number of repositories requested
-    return repos[:n_repos]
+    print()
+    return repos
 
 
 def pull_code_helper(repo_key, branch, delete, max_retries=3):
     """rmtree and retry on intermittent errors"""
     retries = 0
     while retries < max_retries:
         try:
             data = pull_code_from_repo(repo_key, branch=branch, delete=delete)
             return data
         except InvalidGitRepositoryError:
-            print(f"Error with {repo_key}, retrying... ({retries + 1}/{max_retries})")
             shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
             retries += 1
+        except GitCommandError:
+            shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
+            retries += 1
+    print(f"Failed to pull data from {repo_key} after {max_retries} attempts.")
+    return None
 
-    print(
-        f"Failed to pull data from {repo_key} after {max_retries} attempts. Skipping..."
+
+def write_to_parquet(filedata, metadata, base_filename, write_batch_counter):
+    """Write data to parquet files and clear the data"""
+    print(f"Writing batch {write_batch_counter} containing {len(filedata)} files..")
+
+    folder = "output_data"
+    if not os.path.exists(folder):
+        os.makedirs(folder)
+
+    pl.DataFrame(filedata).write_parquet(
+        f"{folder}/filedata_{base_filename}_{write_batch_counter}.parquet"
     )
-    return None
+    pl.DataFrame(metadata).write_parquet(
+        f"{folder}/metadata_{base_filename}_{write_batch_counter}.parquet"
+    )
+
+
+def process_repo(i, repo, metadata, filedata, delete=True):
+    """Process a repository and add its data to the metadata and filedata lists."""
+
+    if repo["size"]:
+        repo_key = repo["html_url"]
+        print(f"({i}) Processing {repo_key}...")
+
+        response = pull_code_helper(
+            repo_key,
+            branch=repo["default_branch"],
+            delete=delete,
+        )
+        if response:
+            metadata_preprocess = flatten_dict(repo)
+            metadata.append(metadata_preprocess)
+
+            for file_obj in response:
+                file_obj["repo_name"] = repo_key
+                filedata.append(file_obj)
+
+    return metadata, filedata
 
 
 def pipeline_fetch_and_load(
     n_repos: int,
     last_n_days: int,
     language: str = None,
-    sort: str = "stars",
-    order: str = "desc",
-    delete: bool = False,
-) -> Dict[str, Dict]:
-    # remove any old repos
-    if os.path.exists(REPODATA_FOLDER):
-        shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
+    write_batch_size: int = 100,
+) -> None:
+    try:
+        # cleanup repo data folder
+        if os.path.exists(REPODATA_FOLDER):
+            shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
 
-    response = get_top_repos(
-        n_repos=n_repos,
-        last_n_days=last_n_days,
-        language=language,
-        sort=sort,
-        order=order,
-    )
+        repos = get_repos_orchestrator(
+            n_repos=n_repos,
+            last_n_days=last_n_days,
+            language=language,
+        )
 
-    github_data = {}
-    for i, repo_metadata in enumerate(response):
-        repo_key = repo_metadata["html_url"]
-
-        if repo_metadata["size"]:
-            print(f"({i}) Processing {repo_key}...")
-
-            github_data[repo_key] = {}
-            github_data[repo_key]["metadata"] = repo_metadata
-
-            response = pull_code_helper(
-                repo_key,
-                branch=repo_metadata["default_branch"],
-                delete=delete,
+        base_filename = datetime.now().strftime("%Y%m%d%H%M%S")
+        write_batch_counter = 1
+        metadata = []
+        filedata = []
+
+        for i, repo in enumerate(repos):
+            metadata, filedata = process_repo(
+                i, repo, metadata, filedata
             )
-            if response:
-                github_data[repo_key]["docs"] = response
-            else:
-                del github_data[repo_key]
-        else:
-            print(f"Skipping {repo_key} as it is empty")
-
-    # clean up repo data
-    shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
 
-    return github_data
+            # If the batch size is reached, write the data to parquet files and clear the lists
+            if not (i + 1) % write_batch_size:
+                write_to_parquet(filedata, metadata, base_filename, write_batch_counter)
+                metadata.clear()
+                filedata.clear()
+                write_batch_counter += 1
+
+        # Write the remaining data to parquet files
+        if metadata and filedata:
+            write_to_parquet(filedata, metadata, base_filename, write_batch_counter)
+
+    finally:
+        # Always clean up the repo data folder
+        if os.path.exists(REPODATA_FOLDER):
+            shutil.rmtree(REPODATA_FOLDER, onerror=readonly_to_writable)
```

### Comparing `git2doc-0.2.1/git2doc.egg-info/PKG-INFO` & `git2doc-0.2.2/git2doc.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,81 @@
 Metadata-Version: 2.1
 Name: git2doc
-Version: 0.2.1
+Version: 0.2.2
 Summary: A tool for converting git repositories into documents
 Home-page: https://github.com/voynow/git2doc
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# Git2Doc
+# Git2Doc 📚
 
-Git2Doc is a Python package for handling Git data. It provides functionality to load and process Git repositories, and supports concurrent file loading for improved performance. The package can be found on [PyPI](https://pypi.org/project/git2doc/).
+[![PyPI version](https://badge.fury.io/py/git2doc.svg)](https://pypi.org/project/git2doc/)
+
+Git2Doc is a Python package that allows you to convert git repositories into documents. It is designed to help developers analyze and understand codebases by providing an easy way to extract and process text content from git repositories.
 
 ## Table of Contents
 
 - [Installation](#installation)
-- [Setup](#setup)
 - [Usage](#usage)
-  - [Loading Git Repositories](#loading-git-repositories)
-  - [Getting Top Repositories](#getting-top-repositories)
-  - [Pipeline Fetch and Load](#pipeline-fetch-and-load)
+  - [Example: Fetch and Load Repositories](#example-fetch-and-load-repositories)
+  - [Example: Get Top Repositories](#example-get-top-repositories)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Installation
 
-To install Git2Doc, run the following command:
+To install Git2Doc, simply run:
 
 ```bash
 pip install git2doc
 ```
 
-## Setup
-
-Before using Git2Doc, make sure to have the following dependencies installed:
-
-- langchain
-- tiktoken
-- gitpython
-- python-dotenv
-- pandas
-
-You can install them using the following command:
-
-```bash
-pip install -r requirements.txt
-```
-
 ## Usage
 
-### Loading Git Repositories
-
-The main functionality of Git2Doc is provided by the `loader.py` module. Here's an example of how to use the `pull_code_from_repo` function to load a Git repository:
+### Example: Fetch and Load Repositories
 
 ```python
-from git2doc.loader import pull_code_from_repo
+from git2doc.loader import pipeline_fetch_and_load
 
-repo_url = "https://github.com/username/repo.git"
-branch = "main"
+# Fetch and load the top 5 repositories created in the last 7 days
+github_data = pipeline_fetch_and_load(n_repos=5, last_n_days=7)
 
-repo_data = pull_code_from_repo(repo_url, branch)
+# Print the metadata and documents for each repository
+for repo_key, repo_data in github_data.items():
+    print(f"Repository: {repo_key}")
+    print("Metadata:")
+    for key, value in repo_data["metadata"].items():
+        print(f"  {key}: {value}")
+    print("Documents:")
+    for doc in repo_data["docs"]:
+        print(f"  {doc.metadata['file_path']}: {doc.page_content[:50]}...")
 ```
 
-### Getting Top Repositories
-
-You can use the `get_top_repos` function to fetch the top repositories based on certain criteria:
+### Example: Get Top Repositories
 
 ```python
 from git2doc.loader import get_top_repos
 
-n_repos = 10
-last_n_days = 30
-language = "Python"
-sort = "stars"
-order = "desc"
-
-top_repos = get_top_repos(n_repos, last_n_days, language, sort, order)
-```
-
-### Pipeline Fetch and Load
-
-The `pipeline_fetch_and_load` function can be used to fetch and load repositories in a single step:
-
-```python
-from git2doc.loader import pipeline_fetch_and_load
-
-n_repos = 10
-last_n_days = 30
-language = "Python"
-sort = "stars"
-order = "desc"
+# Get the top 5 Python repositories created in the last 7 days
+top_repos = get_top_repos(n_repos=5, last_n_days=7, language="Python")
 
-github_data = pipeline_fetch_and_load(n_repos, last_n_days, language, sort, order)
+# Print the repository URLs
+for repo in top_repos:
+    print(repo["html_url"])
 ```
 
 ## Contributing
 
-If you'd like to contribute to Git2Doc, feel free to fork the repository and submit a pull request. If you have any questions or issues, please open an issue on the GitHub repository.
+Contributions are welcome! Please feel free to submit a pull request or open an issue on GitHub.
 
 ## License
 
-Git2Doc is released under the MIT License.
+Git2Doc is released under the [MIT License](https://opensource.org/licenses/MIT).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `git2doc-0.2.1/setup.py` & `git2doc-0.2.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2doc',
-    version='0.2.1',
+    version='0.2.2',
     description='A tool for converting git repositories into documents',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2doc',
     packages=find_packages(),
     install_requires=[
         'langchain',
@@ -23,7 +23,10 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
 	],
 	long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type='text/markdown'
 )
+
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
```

