# Comparing `tmp/BlockFrame-1.0.5.tar.gz` & `tmp/BlockFrame-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlockFrame-1.0.5.tar", last modified: Mon May  8 15:12:17 2023, max compression
+gzip compressed data, was "BlockFrame-1.1.0.tar", last modified: Sat Jun 24 08:31:10 2023, max compression
```

## Comparing `BlockFrame-1.0.5.tar` & `BlockFrame-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 15:12:17.135266 BlockFrame-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-08 15:12:17.100678 BlockFrame-1.0.5/BlockFrame/
--rw-rw-rw-   0        0        0       75 2023-05-07 16:54:53.000000 BlockFrame-1.0.5/BlockFrame/__init__.py
--rw-rw-rw-   0        0        0      832 2023-05-07 18:26:27.000000 BlockFrame-1.0.5/BlockFrame/block_frame.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:12:17.125228 BlockFrame-1.0.5/BlockFrame/chunking_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-1.0.5/BlockFrame/chunking_service/__init__.py
--rw-rw-rw-   0        0        0     8877 2023-05-08 15:10:57.000000 BlockFrame-1.0.5/BlockFrame/chunking_service/chunking.py
--rw-rw-rw-   0        0        0     1106 2023-05-08 15:11:18.000000 BlockFrame-1.0.5/BlockFrame/chunking_service/config.py
--rw-rw-rw-   0        0        0     1657 2023-05-07 15:14:26.000000 BlockFrame-1.0.5/BlockFrame/chunking_service/fetcher.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:12:17.133259 BlockFrame-1.0.5/BlockFrame/database_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-1.0.5/BlockFrame/database_service/__init__.py
--rw-rw-rw-   0        0        0     1193 2023-05-08 15:11:50.000000 BlockFrame-1.0.5/BlockFrame/database_service/database.py
--rw-rw-rw-   0        0        0     1599 2023-05-08 13:09:22.000000 BlockFrame-1.0.5/BlockFrame/database_service/defaultmodel.py
--rw-rw-rw-   0        0        0      377 2023-04-30 09:16:12.000000 BlockFrame-1.0.5/BlockFrame/database_service/getters.py
--rw-rw-rw-   0        0        0     1518 2023-05-07 17:44:18.000000 BlockFrame-1.0.5/BlockFrame/database_service/initalisation.py
--rw-rw-rw-   0        0        0      241 2023-03-26 14:17:13.000000 BlockFrame-1.0.5/BlockFrame/database_service/setters.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:12:17.122328 BlockFrame-1.0.5/BlockFrame.egg-info/
--rw-rw-rw-   0        0        0     5313 2023-05-08 15:12:16.000000 BlockFrame-1.0.5/BlockFrame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-05-08 15:12:17.000000 BlockFrame-1.0.5/BlockFrame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 15:12:16.000000 BlockFrame-1.0.5/BlockFrame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-08 15:12:16.000000 BlockFrame-1.0.5/BlockFrame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 15:12:16.000000 BlockFrame-1.0.5/BlockFrame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5313 2023-05-08 15:12:17.134259 BlockFrame-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-08 15:12:17.135266 BlockFrame-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1412 2023-05-08 15:12:08.000000 BlockFrame-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:31:10.666745 BlockFrame-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-24 08:31:10.638548 BlockFrame-1.1.0/BlockFrame/
+-rw-rw-rw-   0        0        0      373 2023-06-24 08:26:21.000000 BlockFrame-1.1.0/BlockFrame/__init__.py
+-rw-rw-rw-   0        0        0     1510 2023-06-24 08:30:24.000000 BlockFrame-1.1.0/BlockFrame/block_frame.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:31:10.657609 BlockFrame-1.1.0/BlockFrame/chunking_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-1.1.0/BlockFrame/chunking_service/__init__.py
+-rw-rw-rw-   0        0        0    11022 2023-06-24 08:30:24.000000 BlockFrame-1.1.0/BlockFrame/chunking_service/chunking.py
+-rw-rw-rw-   0        0        0     2961 2023-06-24 08:30:24.000000 BlockFrame-1.1.0/BlockFrame/chunking_service/config.py
+-rw-rw-rw-   0        0        0     2905 2023-06-24 08:30:24.000000 BlockFrame-1.1.0/BlockFrame/chunking_service/fetcher.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:31:10.664715 BlockFrame-1.1.0/BlockFrame/database_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-1.1.0/BlockFrame/database_service/__init__.py
+-rw-rw-rw-   0        0        0     1400 2023-06-24 08:30:24.000000 BlockFrame-1.1.0/BlockFrame/database_service/database.py
+-rw-rw-rw-   0        0        0     1599 2023-05-08 13:09:22.000000 BlockFrame-1.1.0/BlockFrame/database_service/defaultmodel.py
+-rw-rw-rw-   0        0        0      377 2023-04-30 09:16:12.000000 BlockFrame-1.1.0/BlockFrame/database_service/getters.py
+-rw-rw-rw-   0        0        0     3638 2023-06-24 08:30:24.000000 BlockFrame-1.1.0/BlockFrame/database_service/initalisation.py
+-rw-rw-rw-   0        0        0      241 2023-06-24 08:30:20.000000 BlockFrame-1.1.0/BlockFrame/database_service/setters.py
+drwxrwxrwx   0        0        0        0 2023-06-24 08:31:10.653640 BlockFrame-1.1.0/BlockFrame.egg-info/
+-rw-rw-rw-   0        0        0     5210 2023-06-24 08:31:10.000000 BlockFrame-1.1.0/BlockFrame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-06-24 08:31:10.000000 BlockFrame-1.1.0/BlockFrame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 08:31:10.000000 BlockFrame-1.1.0/BlockFrame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-24 08:31:10.000000 BlockFrame-1.1.0/BlockFrame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 08:31:10.000000 BlockFrame-1.1.0/BlockFrame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5210 2023-06-24 08:31:10.666745 BlockFrame-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-24 08:31:10.667705 BlockFrame-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1441 2023-06-24 08:29:30.000000 BlockFrame-1.1.0/setup.py
```

### Comparing `BlockFrame-1.0.5/BlockFrame/chunking_service/chunking.py` & `BlockFrame-1.1.0/BlockFrame/chunking_service/chunking.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import hashlib
 import math
 import os
 import pathlib
+import tempfile
 import uuid
 from datetime import datetime, timedelta
-import tempfile
+
 from ..database_service.defaultmodel import ChunkHashes, DefaultChunkModel
 
 
 class ChunksExistsError(Exception):
     pass
 
 
+# The ChunkHandler class initializes various attributes related to chunking files.
 class ChunkHandler:
     def __init__(self, *args, **kwargs) -> None:
         self.config = kwargs.get("config")
         self.path = self.config["file-storage-path"]
         self.option = kwargs.get("option")
         self.chunking_method: str = ""
         self.db = kwargs.get("db")
@@ -28,14 +30,28 @@
         self,
         file_bytes=None,
         file_name=None,
         size=None,
         files: list = None,
         custom_chunker: callable = None,
     ):
+        """
+        This function sets various attributes related to a file, including its name, size, and hash values.
+
+        :param file_bytes: A bytes object representing the contents of a file
+        :param file_name: The name of the file to be targeted for chunking and hashing
+        :param size: The size parameter is used to specify the size of the file in bytes. It is an optional
+        parameter and can be used to provide the size of the file if it is not provided in the file_bytes
+        parameter
+        :param files: A list of file paths to be included in the target
+        :type files: list
+        :param custom_chunker: A callable function that can be used to customize the chunking process of the
+        file
+        :type custom_chunker: callable
+        """
         self.custom_chunker = custom_chunker
         self.primary_uuid = uuid.uuid4()
         self.original_file_hash = ""
         self.chunk_file_hashes = []
         self.file_name = file_name
         self.file_bytes = file_bytes
         self.chunk_file_uid = []
@@ -51,25 +67,32 @@
 
         elif self.file_name is None:
             raise ValueError("Either file_bytes or file_name must be provided")
         elif not pathlib.Path(self.file_name).exists:
             raise FileNotFoundError(f"{self.file_name} does not exist")
 
     def generic_chunks(self):
+        """
+        This function generates chunks of a file's bytes based on a specified size.
+        """
         if self.file_bytes:
             _size = len(self.file_bytes) // self.size
             for i in range(self.size):
                 yield self.file_bytes[i * _size : (i + 1) * _size]
         else:
             _size = os.stat(self.file_name).st_size // self.size
             with open(self.file_name, "rb") as f:
                 while content := f.read(_size):
                     yield content
 
     def time_based_chunks(self):
+        """
+        This function reads a file in chunks and estimates the time required to transfer the remaining data
+        based on the transfer rate of the previous chunks.
+        """
         self.chunk_counter = 0
         with open(self.file_name, "rb") as f:
             while True:
                 start_time = (
                     datetime.now()
                 )  # time the transfer of the previous chunk started
                 content = f.read(self.chunk_size_estimate)
@@ -100,23 +123,26 @@
                                 remaining_bytes / (self.chunk_time_estimate + 1),
                             ),
                             1,
                         )
                     )
 
     def secure_chunks(self):
+        """
+        This function generates secure chunks of a file by adjusting the chunk size based on collision
+        probability.
+        """
         with open(self.file_name, "rb") as f:
             file_size = os.stat(self.file_name).st_size
             while True:
                 chunk_size = self.chunk_size_estimate
                 num_chunks = math.ceil(file_size / chunk_size)
                 if num_chunks >= 4:
                     break
                 chunk_size = math.ceil(file_size / 4)
-                num_chunks = 4
                 self.chunk_size_estimate = chunk_size
 
             while content := f.read(chunk_size):
                 yield content
                 self.chunk_counter += 1
                 if self.chunk_counter % self.window_size == 0:
                     # use a sliding window to estimate the collision probability
@@ -136,14 +162,18 @@
                                 ),
                             ),
                             1,
                         )
                     )
 
     def produce_chunks(self):
+        """
+        This function produces chunks of a file based on different options and saves them to a directory
+        while also calculating their hashes.
+        """
         if self.option == "custom":
             split_files = self.custom_chunker(self.file_name, self.size)
 
         else:
             match self.option:
                 case "generic":
                     split_files = self.generic_chunks()
@@ -182,32 +212,43 @@
                 _hash.update(f.read())
                 count += 1
                 f.write(bytes(chunk))
             self.chunk_file_uid.append(_file_chunk_uid)
             self.chunk_file_hashes.append(_hash.hexdigest())
 
     def hasher(self):
+        """
+        This function calculates the SHA256 hash of a file in chunks of 1024 bytes.
+        """
         _hash = hashlib.sha256()
         with open(self.file_name, "rb") as file:
             chunk = 0
             while chunk != b"":
                 chunk = file.read(1024)
                 _hash.update(chunk)
         self.original_file_hash = _hash.hexdigest()
 
     def find_chunks_from_name(self):
+        """
+        This function returns the number of files in a directory that start with a specific string.
+        :return: The function `find_chunks_from_name` returns the number of files in the directory specified
+        by `self.path` that start with the string `"{self.primary_uuid}_chunk_"`.
+        """
         return len(
             [
                 x
                 for x in os.listdir(self.path)
                 if x.startswith(f"{self.primary_uuid}_chunk_")
             ]
         )
 
     def save_to_db(self):
+        """
+        This function saves information about a file and its chunks to a database.
+        """
         with self.db as session:
             model = DefaultChunkModel(
                 file_uuid=str(self.primary_uuid),
                 file_name=self.file_name,
                 size=self.find_chunks_from_name(),
                 original_file_hash=self.original_file_hash,
                 split_length=len(self.chunk_file_uid),
@@ -222,10 +263,13 @@
                         chunk_size=len(str(_uid)),
                     )
                 )
             session.add(model)
             session.commit()
 
     def generic_chunking(self):
+        """
+        This function performs generic chunking, hashing, and saving to a database.
+        """
         self.produce_chunks()
         self.hasher()
         self.save_to_db()
```

### Comparing `BlockFrame-1.0.5/BlockFrame/database_service/defaultmodel.py` & `BlockFrame-1.1.0/BlockFrame/database_service/defaultmodel.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.5/BlockFrame.egg-info/PKG-INFO` & `BlockFrame-1.1.0/BlockFrame.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: BlockFrame
-Version: 1.0.5
+Version: 1.1.0
 Summary: File Chunking Library to work as a data-store solution alongside webapps and software.
 Home-page: https://github.com/Wizock/BlockFrame/
 Author: Rohaan Ahmed
 Author-email: silent.death3500@gmail.com
 Project-URL: Bug Tracker, https://github.com/Wizock/BlockFrame/issues
 Project-URL: Documentation, https://blockframe.readthedocs.io/
 Project-URL: Source Code, https://github.com/Wizock/BlockFrame/
-Keywords: file chunking,data-store,webapps,software
+Keywords: file chunking,chunker,sqlalchemy,config,data-store,webapps,software
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -47,35 +47,31 @@
 ## Usage
 
 Here's an example of how to use BlockFrame to chunk and store a file:
 
 ```py
 import pathlib
 
-from BlockFrame import BlockFrame
-from BlockFrame.database_service.defaultmodel import DefaultChunkModel
+from BlockFrame import block_frame
 
+# initialize BlockFrame
 config_path = pathlib.Path("./config.json").absolute()
-block_frame = BlockFrame(config_path, option="generic")
+block_frame = block_frame.BlockFrame(config_path, option="generic")
 
-chunker = block_frame.chunker
-fetcher = block_frame.fetcher
-chunker_db = block_frame.database
 
-chunker_db.create_table(DefaultChunkModel)
+# chunking
+block_frame.chunker.target(file_name="image.jpg", size=5)
 
-chunker.target("image.jpg", size=5)
+block_frame.chunker.generic_chunking()
 
-chunker.generic_chunking()
 
-fetcher.target("image.jpg")
+# fetcher
+block_frame.fetcher.target("image.jpg")
 
-print(fetcher.collect_chunks())
-
-fetcher.fetch()
+block_frame.fetcher.fetch()
 ```
 
 # Collaboration Tips
 
 - If you encounter any issues or have suggestions for improvement, please open an issue on GitHub.
 - Pull requests are welcome! Please ensure that your code adheres to the project's coding standards and that tests are passing before submitting a pull request.
 - If you want to contribute but don't know where to start, please check the project's issues page or open-source guide for guidance.
```

### Comparing `BlockFrame-1.0.5/BlockFrame.egg-info/SOURCES.txt` & `BlockFrame-1.1.0/BlockFrame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BlockFrame-1.0.5/PKG-INFO` & `BlockFrame-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: BlockFrame
-Version: 1.0.5
+Version: 1.1.0
 Summary: File Chunking Library to work as a data-store solution alongside webapps and software.
 Home-page: https://github.com/Wizock/BlockFrame/
 Author: Rohaan Ahmed
 Author-email: silent.death3500@gmail.com
 Project-URL: Bug Tracker, https://github.com/Wizock/BlockFrame/issues
 Project-URL: Documentation, https://blockframe.readthedocs.io/
 Project-URL: Source Code, https://github.com/Wizock/BlockFrame/
-Keywords: file chunking,data-store,webapps,software
+Keywords: file chunking,chunker,sqlalchemy,config,data-store,webapps,software
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -47,35 +47,31 @@
 ## Usage
 
 Here's an example of how to use BlockFrame to chunk and store a file:
 
 ```py
 import pathlib
 
-from BlockFrame import BlockFrame
-from BlockFrame.database_service.defaultmodel import DefaultChunkModel
+from BlockFrame import block_frame
 
+# initialize BlockFrame
 config_path = pathlib.Path("./config.json").absolute()
-block_frame = BlockFrame(config_path, option="generic")
+block_frame = block_frame.BlockFrame(config_path, option="generic")
 
-chunker = block_frame.chunker
-fetcher = block_frame.fetcher
-chunker_db = block_frame.database
 
-chunker_db.create_table(DefaultChunkModel)
+# chunking
+block_frame.chunker.target(file_name="image.jpg", size=5)
 
-chunker.target("image.jpg", size=5)
+block_frame.chunker.generic_chunking()
 
-chunker.generic_chunking()
 
-fetcher.target("image.jpg")
+# fetcher
+block_frame.fetcher.target("image.jpg")
 
-print(fetcher.collect_chunks())
-
-fetcher.fetch()
+block_frame.fetcher.fetch()
 ```
 
 # Collaboration Tips
 
 - If you encounter any issues or have suggestions for improvement, please open an issue on GitHub.
 - Pull requests are welcome! Please ensure that your code adheres to the project's coding standards and that tests are passing before submitting a pull request.
 - If you want to contribute but don't know where to start, please check the project's issues page or open-source guide for guidance.
```

### Comparing `BlockFrame-1.0.5/setup.py` & `BlockFrame-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="BlockFrame",
-    version="1.0.5",
+    version="1.1.0",
     author="Rohaan Ahmed",
     author_email="silent.death3500@gmail.com",
     description="File Chunking Library to work as a data-store solution alongside webapps and software.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
@@ -27,9 +27,9 @@
     python_requires=">=3.6",
     url="https://github.com/Wizock/BlockFrame/",
     project_urls={
         "Bug Tracker": "https://github.com/Wizock/BlockFrame/issues",
         "Documentation": "https://blockframe.readthedocs.io/",
         "Source Code": "https://github.com/Wizock/BlockFrame/",
     },
-    keywords="file chunking, data-store, webapps, software",
+    keywords="file chunking, chunker, sqlalchemy, config, data-store, webapps, software",
 )
```

