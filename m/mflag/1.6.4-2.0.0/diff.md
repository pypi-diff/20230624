# Comparing `tmp/mflag-1.6.4.tar.gz` & `tmp/mflag-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mflag-1.6.4.tar", last modified: Sat Feb 11 19:33:49 2023, max compression
+gzip compressed data, was "mflag-2.0.0.tar", last modified: Sat Jun 24 10:52:06 2023, max compression
```

## Comparing `mflag-1.6.4.tar` & `mflag-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-11 19:33:49.219762 mflag-1.6.4/
--rwxrwxrwx   0 root         (0) root         (0)     1071 2022-07-20 18:39:20.000000 mflag-1.6.4/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     2566 2023-02-11 19:33:49.219576 mflag-1.6.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2383 2023-02-11 19:33:49.000000 mflag-1.6.4/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-11 19:33:49.217163 mflag-1.6.4/mflag/
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-02-11 19:33:19.000000 mflag-1.6.4/mflag/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-11 19:33:49.219131 mflag-1.6.4/mflag/src/
--rwxrwxrwx   0 root         (0) root         (0)     4559 2023-02-11 19:18:19.000000 mflag-1.6.4/mflag/src/flag.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-11 19:33:49.218827 mflag-1.6.4/mflag.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     2566 2023-02-11 19:33:49.000000 mflag-1.6.4/mflag.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      206 2023-02-11 19:33:49.000000 mflag-1.6.4/mflag.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-02-11 19:33:49.000000 mflag-1.6.4/mflag.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-02-11 19:33:49.000000 mflag-1.6.4/mflag.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-02-11 19:33:49.000000 mflag-1.6.4/mflag.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-02-11 19:33:49.219840 mflag-1.6.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      459 2023-02-11 19:33:44.000000 mflag-1.6.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:52:06.525730 mflag-2.0.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1071 2023-06-24 10:44:31.000000 mflag-2.0.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-24 10:52:06.525580 mflag-2.0.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2026 2023-06-24 10:44:31.000000 mflag-2.0.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:52:06.522562 mflag-2.0.0/mflag/
+-rwxrwxrwx   0 root         (0) root         (0)      202 2023-06-24 10:49:16.000000 mflag-2.0.0/mflag/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:52:06.524042 mflag-2.0.0/mflag/src/
+-rwxrwxrwx   0 root         (0) root         (0)     4962 2023-06-24 10:44:31.000000 mflag-2.0.0/mflag/src/flag.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:52:06.521478 mflag-2.0.0/mflag/src/rcmng/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:52:06.524541 mflag-2.0.0/mflag/src/rcmng/client/
+-rwxrwxrwx   0 root         (0) root         (0)     1631 2023-06-24 10:41:50.000000 mflag-2.0.0/mflag/src/rcmng/client/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      433 2023-06-24 09:19:59.000000 mflag-2.0.0/mflag/src/rcmng/client/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:52:06.524965 mflag-2.0.0/mflag/src/rcmng/server/
+-rwxrwxrwx   0 root         (0) root         (0)     6832 2023-06-24 10:42:40.000000 mflag-2.0.0/mflag/src/rcmng/server/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      255 2023-06-24 08:55:53.000000 mflag-2.0.0/mflag/src/rcmng/server/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:52:06.525324 mflag-2.0.0/mflag/src/rcmng/submit/
+-rwxrwxrwx   0 root         (0) root         (0)      844 2023-06-24 10:18:10.000000 mflag-2.0.0/mflag/src/rcmng/submit/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      444 2023-06-24 10:33:05.000000 mflag-2.0.0/mflag/src/rcmng/submit/run.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-24 10:52:06.523779 mflag-2.0.0/mflag.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     2209 2023-06-24 10:52:06.000000 mflag-2.0.0/mflag.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      401 2023-06-24 10:52:06.000000 mflag-2.0.0/mflag.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-24 10:52:06.000000 mflag-2.0.0/mflag.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       47 2023-06-24 10:52:06.000000 mflag-2.0.0/mflag.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2023-06-24 10:52:06.000000 mflag-2.0.0/mflag.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-24 10:52:06.525780 mflag-2.0.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      513 2023-06-24 10:51:18.000000 mflag-2.0.0/setup.py
```

### Comparing `mflag-1.6.4/LICENSE` & `mflag-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mflag-1.6.4/PKG-INFO` & `mflag-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflag
-Version: 1.6.4
+Version: 2.0.0
 Summary: put/remove flags for files and folders
 Author: Moses Dastmard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mflag: powerful Python toolkit for mark/unmark files and directories 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/mflag/)
@@ -19,16 +19,16 @@
 https://github.com/MosesDastmard/mflag
 
 Binary installers for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/mflag/)
 
 
 ```python
-# !pip install mflag
-from mflag import Flag, JobManager
+# !pip install flagify
+from mflag import Flag
 import pandas as pd
 import os
 ```
 
 
 ```python
 # lets make a simple csv file
@@ -51,35 +51,14 @@
 ```
 
 
 ```python
 Process(process_name='convert_csv_to_parquet').run('data.csv', 'data.parquet')
 ```
 
-    the file data.csv is already processed
-
-
 
 ```python
 Process(process_name='convert_csv_to_parquet').run('data.csv', 'data.parquet')
 ```
 
     the file data.csv is already processed
 
-
-
-```python
-# with JobManager(job_dir_path='job_manager', job_id='job_1') as jm:
-#     print("hello world")
-```
-
-    hello world
-
-
-
-```python
-# with JobManager(job_dir_path='job_manager', job_id='job_1') as jm:
-#     print("hello world")
-```
-
-    job_id=job_1 is already done, no need to run it again
-
```

### Comparing `mflag-1.6.4/README.md` & `mflag-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 https://github.com/MosesDastmard/mflag
 
 Binary installers for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/mflag/)
 
 
 ```python
-# !pip install mflag
-from mflag import Flag, JobManager
+# !pip install flagify
+from mflag import Flag
 import pandas as pd
 import os
 ```
 
 
 ```python
 # lets make a simple csv file
@@ -43,35 +43,14 @@
 ```
 
 
 ```python
 Process(process_name='convert_csv_to_parquet').run('data.csv', 'data.parquet')
 ```
 
-    the file data.csv is already processed
-
-
 
 ```python
 Process(process_name='convert_csv_to_parquet').run('data.csv', 'data.parquet')
 ```
 
     the file data.csv is already processed
 
-
-
-```python
-# with JobManager(job_dir_path='job_manager', job_id='job_1') as jm:
-#     print("hello world")
-```
-
-    hello world
-
-
-
-```python
-# with JobManager(job_dir_path='job_manager', job_id='job_1') as jm:
-#     print("hello world")
-```
-
-    job_id=job_1 is already done, no need to run it again
-
```

### Comparing `mflag-1.6.4/mflag/src/flag.py` & `mflag-2.0.0/mflag/src/flag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 import os
 import sys
 from os.path import join
+import pandas as pd
 from mpath import get_path_info
 from datetime import datetime
-import json
 flag_extention = '.flg'
 
 class Flag:
     def __init__(self, process_name, hidden=True) -> None:
         self.process_name = process_name
         self.hidden = hidden
         self.get_path_info = get_path_info
@@ -69,55 +69,61 @@
         
         
 class SkipWithBlock(Exception):
     pass
 
 
 class JobManager:
-    def __init__(self, job_dir_path, job_id, job_name="", job_description="", process_name=""):
-        self.job_dir_path = Path(job_dir_path)
+    def __init__(self, job_file_path, job_id, job_name="", job_description="", process_name=""):
+        self.job_file_path = Path(job_file_path)
+        assert not os.path.isdir(self.job_file_path), f"job_file_path={self.job_file_path} is not a valid file path"
         self.job_id = job_id
         self.job_name = job_name
         self.job_description = job_description
         self.process_name = process_name
-        self.job_file_path = os.path.join(self.job_dir_path, self.job_id + ".json")
+        self.job_file_dir = self.job_file_path.parent.absolute()
         
     def __initial_check(self):
-        os.makedirs(self.job_dir_path, exist_ok=True)
+        os.makedirs(self.job_file_dir, exist_ok=True)
+        if not os.path.exists(self.job_file_path):
+            self.__create_empty_job_file()
+    
+    def __create_empty_job_file(self):
+        job_df = pd.DataFrame(columns=['job_id', 'job_name', 'job_description', 'process_name', 'issue_date', 'finish_date'])
+        job_df.set_index('job_id', inplace=True)
+        job_df.to_csv(self.job_file_path)
     
     def __is_job_done(self):
-        if not os.path.exists(self.job_file_path):
-            job_dict = {'job_id':self.job_id, 'job_name':self.job_name, 'job_description':self.job_description, 'process_name':self.process_name, 'issue_date':str(datetime.now())}
-            with open(self.job_file_path, 'w') as f:
-                json.dump(job_dict, f)
-            return False
+        job_df = pd.read_csv(self.job_file_path, index_col=0)
+        if self.job_id not in job_df.index:
+            for col, value in {'job_name':self.job_name, 'job_description':self.job_description, 'process_name':self.process_name, 'issue_date':datetime.now(), 'finish_date':None}.items():
+                job_df.loc[self.job_id, col] = value
+            job_df.to_csv(self.job_file_path)
+            return True
+        job_row = job_df.loc[self.job_id]
+        if pd.isna(job_row['finish_date']):
+            return True
         else:
-            with open(self.job_file_path, 'r') as f:
-                job_dict = json.load(f)
-                if 'finish_date' in job_dict.keys():
-                    print(f"job_id={self.job_id} is already done, no need to run it again")
-                    return True
+            print(f"job_id={self.job_id} is already done, no need to run it again")
             return False
 
     def __enter__(self):
         self.__initial_check()
-        if self.__is_job_done():
+        if not self.__is_job_done():
             sys.settrace(lambda *args, **keys: None)
             frame = sys._getframe(1)
             frame.f_trace = self.trace
 
     def trace(self, frame, event, arg):
         raise SkipWithBlock()
     
     def __finish_job(self):
-        with open(self.job_file_path, 'r') as f:
-            job_dict = json.load(f)
-            job_dict['finish_date'] = str(datetime.now())
-        with open(self.job_file_path, 'w') as f:
-            json.dump(job_dict, f)
+        job_df = pd.read_csv(self.job_file_path, index_col=0)
+        job_df.loc[self.job_id, 'finish_date'] = datetime.now()
+        job_df.to_csv(self.job_file_path)
         
     def __exit__(self, type, value, traceback):
         if type is None:
             self.__finish_job()
             return  # No exception
 
         if issubclass(type, SkipWithBlock):
```

### Comparing `mflag-1.6.4/mflag.egg-info/PKG-INFO` & `mflag-2.0.0/mflag.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflag
-Version: 1.6.4
+Version: 2.0.0
 Summary: put/remove flags for files and folders
 Author: Moses Dastmard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mflag: powerful Python toolkit for mark/unmark files and directories 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/mflag/)
@@ -19,16 +19,16 @@
 https://github.com/MosesDastmard/mflag
 
 Binary installers for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/mflag/)
 
 
 ```python
-# !pip install mflag
-from mflag import Flag, JobManager
+# !pip install flagify
+from mflag import Flag
 import pandas as pd
 import os
 ```
 
 
 ```python
 # lets make a simple csv file
@@ -51,35 +51,14 @@
 ```
 
 
 ```python
 Process(process_name='convert_csv_to_parquet').run('data.csv', 'data.parquet')
 ```
 
-    the file data.csv is already processed
-
-
 
 ```python
 Process(process_name='convert_csv_to_parquet').run('data.csv', 'data.parquet')
 ```
 
     the file data.csv is already processed
 
-
-
-```python
-# with JobManager(job_dir_path='job_manager', job_id='job_1') as jm:
-#     print("hello world")
-```
-
-    hello world
-
-
-
-```python
-# with JobManager(job_dir_path='job_manager', job_id='job_1') as jm:
-#     print("hello world")
-```
-
-    job_id=job_1 is already done, no need to run it again
-
```

