# Comparing `tmp/ffmpeg-gpt-0.1.0.tar.gz` & `tmp/ffmpeg-gpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg-gpt-0.1.0.tar", last modified: Sat Jun 24 10:41:36 2023, max compression
+gzip compressed data, was "ffmpeg-gpt-0.1.1.tar", last modified: Sat Jun 24 10:52:22 2023, max compression
```

## Comparing `ffmpeg-gpt-0.1.0.tar` & `ffmpeg-gpt-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-24 10:41:36.629057 ffmpeg-gpt-0.1.0/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1118 2023-06-24 10:41:36.629057 ffmpeg-gpt-0.1.0/PKG-INFO
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      568 2023-06-24 10:39:44.000000 ffmpeg-gpt-0.1.0/README.md
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-24 10:41:36.629057 ffmpeg-gpt-0.1.0/ffmpeg_gpt/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      517 2023-06-24 10:39:44.000000 ffmpeg-gpt-0.1.0/ffmpeg_gpt/__init__.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      641 2023-06-24 10:39:44.000000 ffmpeg-gpt-0.1.0/ffmpeg_gpt/ffmpeg_gpt.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      303 2023-06-24 10:39:44.000000 ffmpeg-gpt-0.1.0/ffmpeg_gpt/utils.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-24 10:41:36.629057 ffmpeg-gpt-0.1.0/ffmpeg_gpt.egg-info/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1118 2023-06-24 10:41:36.000000 ffmpeg-gpt-0.1.0/ffmpeg_gpt.egg-info/PKG-INFO
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      292 2023-06-24 10:41:36.000000 ffmpeg-gpt-0.1.0/ffmpeg_gpt.egg-info/SOURCES.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)        1 2023-06-24 10:41:36.000000 ffmpeg-gpt-0.1.0/ffmpeg_gpt.egg-info/dependency_links.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       48 2023-06-24 10:41:36.000000 ffmpeg-gpt-0.1.0/ffmpeg_gpt.egg-info/entry_points.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       15 2023-06-24 10:41:36.000000 ffmpeg-gpt-0.1.0/ffmpeg_gpt.egg-info/requires.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       11 2023-06-24 10:41:36.000000 ffmpeg-gpt-0.1.0/ffmpeg_gpt.egg-info/top_level.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       38 2023-06-24 10:41:36.629057 ffmpeg-gpt-0.1.0/setup.cfg
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      742 2023-06-24 10:39:44.000000 ffmpeg-gpt-0.1.0/setup.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-24 10:52:22.509405 ffmpeg-gpt-0.1.1/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1309 2023-06-24 10:52:22.509405 ffmpeg-gpt-0.1.1/PKG-INFO
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      727 2023-06-24 10:46:31.000000 ffmpeg-gpt-0.1.1/README.md
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-24 10:52:22.509405 ffmpeg-gpt-0.1.1/ffmpeg_gpt/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      517 2023-06-24 10:39:44.000000 ffmpeg-gpt-0.1.1/ffmpeg_gpt/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      641 2023-06-24 10:39:44.000000 ffmpeg-gpt-0.1.1/ffmpeg_gpt/ffmpeg_gpt.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      303 2023-06-24 10:39:44.000000 ffmpeg-gpt-0.1.1/ffmpeg_gpt/utils.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-06-24 10:52:22.509405 ffmpeg-gpt-0.1.1/ffmpeg_gpt.egg-info/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1309 2023-06-24 10:52:22.000000 ffmpeg-gpt-0.1.1/ffmpeg_gpt.egg-info/PKG-INFO
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      292 2023-06-24 10:52:22.000000 ffmpeg-gpt-0.1.1/ffmpeg_gpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)        1 2023-06-24 10:52:22.000000 ffmpeg-gpt-0.1.1/ffmpeg_gpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)       48 2023-06-24 10:52:22.000000 ffmpeg-gpt-0.1.1/ffmpeg_gpt.egg-info/entry_points.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)       15 2023-06-24 10:52:22.000000 ffmpeg-gpt-0.1.1/ffmpeg_gpt.egg-info/requires.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)       11 2023-06-24 10:52:22.000000 ffmpeg-gpt-0.1.1/ffmpeg_gpt.egg-info/top_level.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)       38 2023-06-24 10:52:22.509405 ffmpeg-gpt-0.1.1/setup.cfg
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      742 2023-06-24 10:52:18.000000 ffmpeg-gpt-0.1.1/setup.py
```

### Comparing `ffmpeg-gpt-0.1.0/PKG-INFO` & `ffmpeg-gpt-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-gpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use GPT to generate ffmpeg commands
 Home-page: https://github.com/apirrone/ffmpeg_gpt
 Author: Antoine Pirrone
 Author-email: antoine.pirrone@gmail.com
 License: UNKNOWN
 Description: # ffmpeg_gpt
         
@@ -19,14 +19,18 @@
         ### From source
         ```bash
         git clone https://github.com/apirrone/ffmpeg_gpt
         cd ffmpeg_gpt
         pip install .
         ```
         
+        ### Set yout openai api key as an environment variable (put it in your .bashrc or equivalent for convenience)
+        ```bash
+        export OPENAI_API_KEY=<your_api_key>
+        ```
         ## Usage examples
         ```bash
         $ ffmpeg-gpt "flip the video input.mp4 vertically, and export all its frames in a directory named out"
         
         Generated script: 
         ===========
         #!/bin/bash
```

### Comparing `ffmpeg-gpt-0.1.0/README.md` & `ffmpeg-gpt-0.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 ### From source
 ```bash
 git clone https://github.com/apirrone/ffmpeg_gpt
 cd ffmpeg_gpt
 pip install .
 ```
 
+### Set yout openai api key as an environment variable (put it in your .bashrc or equivalent for convenience)
+```bash
+export OPENAI_API_KEY=<your_api_key>
+```
 ## Usage examples
 ```bash
 $ ffmpeg-gpt "flip the video input.mp4 vertically, and export all its frames in a directory named out"
 
 Generated script: 
 ===========
 #!/bin/bash
```

### Comparing `ffmpeg-gpt-0.1.0/ffmpeg_gpt/__init__.py` & `ffmpeg-gpt-0.1.1/ffmpeg_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-gpt-0.1.0/ffmpeg_gpt/ffmpeg_gpt.py` & `ffmpeg-gpt-0.1.1/ffmpeg_gpt/ffmpeg_gpt.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-gpt-0.1.0/ffmpeg_gpt.egg-info/PKG-INFO` & `ffmpeg-gpt-0.1.1/ffmpeg_gpt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-gpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use GPT to generate ffmpeg commands
 Home-page: https://github.com/apirrone/ffmpeg_gpt
 Author: Antoine Pirrone
 Author-email: antoine.pirrone@gmail.com
 License: UNKNOWN
 Description: # ffmpeg_gpt
         
@@ -19,14 +19,18 @@
         ### From source
         ```bash
         git clone https://github.com/apirrone/ffmpeg_gpt
         cd ffmpeg_gpt
         pip install .
         ```
         
+        ### Set yout openai api key as an environment variable (put it in your .bashrc or equivalent for convenience)
+        ```bash
+        export OPENAI_API_KEY=<your_api_key>
+        ```
         ## Usage examples
         ```bash
         $ ffmpeg-gpt "flip the video input.mp4 vertically, and export all its frames in a directory named out"
         
         Generated script: 
         ===========
         #!/bin/bash
```

### Comparing `ffmpeg-gpt-0.1.0/setup.py` & `ffmpeg-gpt-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="ffmpeg-gpt",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "openai==0.27.8"
     ],
     entry_points={
         "console_scripts": [
             "ffmpeg-gpt = ffmpeg_gpt:main",
```

