# Comparing `tmp/finderz-1.2.4.tar.gz` & `tmp/finderz-2.0.0.tar.gz`

## Comparing `finderz-1.2.4.tar` & `finderz-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,26 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-1.2.4/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-1.2.4/src/.DS_Store
--rw-r--r--   0        0        0     9713 2020-02-02 00:00:00.000000 finderz-1.2.4/src/FinderZ/FinderZLib.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 finderz-1.2.4/src/FinderZ/__init__.py
--rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/bash.sh
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/importTests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/insertion.txt
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/insertiontest.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/parentFunctions.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/updates/update.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 finderz-1.2.4/LICENSE
--rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 finderz-1.2.4/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 finderz-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 finderz-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.0/.DS_Store
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 finderz-2.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 finderz-2.0.0/docs/code structure.rst
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 finderz-2.0.0/docs/conf.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 finderz-2.0.0/docs/credits.rst
+-rw-r--r--   0        0        0    28295 2020-02-02 00:00:00.000000 finderz-2.0.0/docs/function use.rst
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 finderz-2.0.0/docs/index.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 finderz-2.0.0/docs/installation.rst
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 finderz-2.0.0/docs/updatev2.rst
+-rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.0/docs/img/logo-color.jpg
+-rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.0/logo/logo-color.jpg
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.0/old/src/.DS_Store
+-rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 finderz-2.0.0/old/src/FinderZ/FinderZLib.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 finderz-2.0.0/old/src/FinderZ/__init__.py
+-rw-r--r--   0        0        0    48923 2020-02-02 00:00:00.000000 finderz-2.0.0/src/FinderZV2.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 finderz-2.0.0/src/__init__.py
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 finderz-2.0.0/tests/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.0/tests/updates/.DS_Store
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 finderz-2.0.0/tests/updates/V2 Changelog.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 finderz-2.0.0/tests/updates/bash.sh
+-rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 finderz-2.0.0/tests/updates/parentFunctions.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 finderz-2.0.0/tests/updates/update.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 finderz-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 finderz-2.0.0/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 finderz-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 finderz-2.0.0/PKG-INFO
```

### Comparing `finderz-1.2.4/.DS_Store` & `finderz-2.0.0/.DS_Store`

 * *Files 0% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 00000270: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00000280: 735b 5368 6f77 5369 6465 6261 7209 0909  s[ShowSidebar...
 00000290: 095f 1018 7b7b 3438 302c 2031 3735 7d2c  ._..{{480, 175},
 000002a0: 207b 3932 302c 2034 3932 7d7d 0908 1523   {920, 492}}...#
 000002b0: 2f3b 525f 6b6c 6d6e 6f8a 0000 0000 0000  /;R_klmno.......
 000002c0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
 000002d0: 0000 0000 0000 0000 008b 0000 0003 0073  ...............s
-000002e0: 0072 0063 6473 636c 626f 6f6c 0100 0000  .r.cdsclbool....
+000002e0: 0072 0063 6473 636c 626f 6f6c 0000 0000  .r.cdsclbool....
 000002f0: 0300 7300 7200 6376 5372 6e6c 6f6e 6700  ..s.r.cvSrnlong.
 00000300: 0000 0100 0000 0500 7400 6500 7300 7400  ........t.e.s.t.
-00000310: 7364 7363 6c62 6f6f 6c00 0000 0000 0000  sdsclbool.......
+00000310: 7364 7363 6c62 6f6f 6c01 0000 0000 0000  sdsclbool.......
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `finderz-1.2.4/src/.DS_Store` & `finderz-2.0.0/old/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-1.2.4/src/FinderZ/FinderZLib.py` & `finderz-2.0.0/old/src/FinderZ/FinderZLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,17 +225,14 @@
 		newFilePath = os.path.dirname(filePath)
 		os.rename(filePath, newFilePath + "/" + newName)
 		
 	def renameDirectory(newName, directoryPath):
 		newDirectoryPath = os.path.dirname(os.path.dirname(directoryPath))
 		os.rename(directoryPath, newDirectoryPath + "/" + newName)
 
-
-
-
 	#Version 1.2.3:
 	def insertTextInFile(insertionText, lineNumber, filePath, appendNewLines = False):
 			
 		if lineNumber < 1:
 			raise Exception("ERR: Line number can not be less than 1.")
 		#Open the file and start scanning:
 		fileObject = open(filePath, 'r')
```

### Comparing `finderz-1.2.4/tests/updates/update.py` & `finderz-2.0.0/tests/updates/update.py`

 * *Files identical despite different names*

### Comparing `finderz-1.2.4/LICENSE` & `finderz-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finderz-1.2.4/README.md` & `finderz-2.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # FinderZ
-A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!
 
-![finderz-logo](https://user-images.githubusercontent.com/116693779/213965405-6b416655-09d6-4ef1-ae05-58c32035541d.png)
+Full File Management Library for Python. And growing (V2 is out!)
+
+![logo-color](https://github.com/PatzEdi/GeneralGithubRepoTesting/assets/116693779/d90bbd80-3c81-4153-8e1f-e8aa71bf7844)
 
 <p align="center">
 	<img src="https://img.shields.io/badge/License-GPL--3.0-brightgreen"
 		height="23">
 	<img src="https://img.shields.io/badge/Creator-PatzEdi-brightgreen"
 		height="23">
 	<img src="https://img.shields.io/badge/Version-Latest-brightgreen"
@@ -13,80 +14,66 @@
 	
 	
 </p>
 <p align = "center">
 	<img src="https://static.pepy.tech/badge/finderz"
 		height="23">
 </p>
-FinderZ uses the os, subprocess, and shutil libraries in order to function properly. 
+
+## **IMPORTANT: ** 
+**V2 is finally out! To check out the details, go to the readthedocs documentation under the update v2 section!**
+**LINK TO READ THE DOCS: [Documentation](https://finderz.readthedocs.io/en/latest/index.html)** 
+**IF YOU WANT TO USE THE SYNCHRONIZATION AND BACKUP CLASSeS, MAKE SURE TO THOROUGHLY READ THE [DOCUMENTATION](https://finderz.readthedocs.io/en/latest/index.html) IN ORDER TO PREVENT DATA LOSS**
 
 ## **Written in python, this library provides you with different file operation commands as well as info gathering commands on directories as well as files.** 
 ____________________________________________________________________________
-## **CHANGELOG: 1.2.4**
-- Release version 1.2.4
-- Added new functions: createFile and removeFile
-- With these new functions, you can easily create and remove singular files.
-- Fixed some README issues.
-
-If you want to create a single file, you can do so like this:
+## **CHANGELOG: V2.0.0**
 
-```
-from FinderZ import fileOperands
-
-fileOperands.createFile("FileName", "fileCreationPath")
-```
-Note that the "FileName" in this case may also include a file extension.
+To check out the details of V2, go to the [documentation](https://finderz.readthedocs.io/en/latest/index.html). This is a big update with many new things!
 
-- Documentation will be added soon that explains each function and functionality of each function in a detailed manner.
-
-Thank you all for 10K Downloads!
 
 ## **Usage**
 Installation:
 ```
 pip3 install FinderZ
 ```
 Importing:
 ```
 import FinderZ
 ```
-Example for finding files with a specific keyword:
-```
-FinderZ.fileOperands.findFiles("fileName", "Custom Directory")
-```
-Or, if you want to import a single class:
-```
-from FinderZ import fileOperands
 
-#Find the file, calling the command "fO":
-print(fileOperands.findFiles("fileName", "Custom Path"))
-```
 ## **Features**
-- Consists of three classes: GatherInfo, fileOperands, and callBash.
-- Find any file with a certain keyword. This means you no longer have to necessarily know the full name of the file in case you forgot it. 
-- Gather information such as files in a directory, name of those files, and even a createFiles tool as well as a curated removeFiles tool.
-- Is easy to add new things to the library.
+- Consists of three classes: GatherInfo, fileOperands, Synchronize, Backup, and callBash.
+- Advanced file operations, already built for you (including many options to choose from!) 
+- Supports regex operations for some functions, as well as specific filters and multiple other choices to choose from. Options such as exact search or something even just containing a keyword, or even having the option to choose to seaerch recursively, are all included.
+- Includes full-featured, reliable synchronization and backup classes.
+- Full set of info gathering tools under the GatherInfo class.
+- Full-featured documentation to guide you through each function in detail. 
 - In case of functionality restrictions, callBash is a function that calls a bash script in order to expand functionality at its peak.
 - Easy to use.
 - You no longer have to take your time in making those file management algorithms that take a while to complete.
 - Fast and efficient, includes a plethora of other features. 
 ____________________________________________________________________________
 ## **Why?**
-- I wanted to showcase how one can easily create a full library that manages files in order to save time in an efficient way. 
+- FinderZ is a way to easily expand on the file system of many operating system. It supports, MacOS, Windows, Linux, and Android.
 - Who wouldn't want a tool to manage their files easily in their python scripts? This will save time!
 ____________________________________________________________________________
 ## **How?**
-- Using iterating techniques for a few of the functions, I was able to complete actions recursively through different directories. 
-- The use of the os and subprocess modules (especially os) made everything easier, and what I did was basically structure a library to make life easier.
+- FinderZ is composed of many iterating techniques and parametric options. Based on these options, the core of each function deals with a user's choice of what to do or what not to do.
+- More info under the documentation!
 ____________________________________________________________________________
 ## **User notice**
-- Some of the functions are only there in case one has to get user input or wants to format things in a more visible way. These functions include askMainDir, and the expandListInfo functions.
-- This project is still a work in progress! It is very flexible in adding new functions. So far, there are still basic functions being added frequently, and some more advanced functions being added gradually. Thanks for being patient, and enjoy!
+- I am not responsible for any damage or data lost using the FinderZ library. 
+- If using the Synchronize class, make sure renaming files or directories is never the last thing you do before synchronization, unless it is the only thing you did do (no adding, removing, copying, etc. files before)
+- This project has just been released to version 2! It has grown so much, but it is still growing and improving.
 ____________________________________________________________________________
 ## **Services used (Credits):**
 - [OS module](https://docs.python.org/3/library/os.html)
 - [Shutil module](https://docs.python.org/3/library/shutil.html)
+- [Time module](https://docs.python.org/3/library/time.html)
+- [Hashlib module](https://docs.python.org/3/library/hashlib.html)
+- [re](https://docs.python.org/3/library/re.html)
 - [Subprocess module](https://docs.python.org/3/library/subprocess.html)
 
 ____________________________________________________________________________
 ## **Make sure to leave a star!**
 - If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
```

### Comparing `finderz-1.2.4/pyproject.toml` & `finderz-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FinderZ"
-version = "1.2.4"
+version = "2.0.0"
 authors = [
 	{ name="PatzEdi", email="patzedigithub@gmail.com" },
 ]
 description = "A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 keywords = ["files", "filemanagement", "library", "development"]
```

### Comparing `finderz-1.2.4/PKG-INFO` & `finderz-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinderZ
-Version: 1.2.4
+Version: 2.0.0
 Summary: A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!
 Project-URL: Homepage, https://github.com/PatzEdi
 Project-URL: Repository, https://github.com/PatzEdi/FinderZ
 Project-URL: Bug Tracker, https://github.com/PatzEdi/FinderZ/issues
 Author-email: PatzEdi <patzedigithub@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
@@ -12,17 +12,18 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # FinderZ
-A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!
 
-![finderz-logo](https://user-images.githubusercontent.com/116693779/213965405-6b416655-09d6-4ef1-ae05-58c32035541d.png)
+Full File Management Library for Python. And growing (V2 is out!)
+
+![logo-color](https://github.com/PatzEdi/GeneralGithubRepoTesting/assets/116693779/d90bbd80-3c81-4153-8e1f-e8aa71bf7844)
 
 <p align="center">
 	<img src="https://img.shields.io/badge/License-GPL--3.0-brightgreen"
 		height="23">
 	<img src="https://img.shields.io/badge/Creator-PatzEdi-brightgreen"
 		height="23">
 	<img src="https://img.shields.io/badge/Version-Latest-brightgreen"
@@ -30,80 +31,66 @@
 	
 	
 </p>
 <p align = "center">
 	<img src="https://static.pepy.tech/badge/finderz"
 		height="23">
 </p>
-FinderZ uses the os, subprocess, and shutil libraries in order to function properly. 
+
+## **IMPORTANT: ** 
+**V2 is finally out! To check out the details, go to the readthedocs documentation under the update v2 section!**
+**LINK TO READ THE DOCS: [Documentation](https://finderz.readthedocs.io/en/latest/index.html)** 
+**IF YOU WANT TO USE THE SYNCHRONIZATION AND BACKUP CLASSeS, MAKE SURE TO THOROUGHLY READ THE [DOCUMENTATION](https://finderz.readthedocs.io/en/latest/index.html) IN ORDER TO PREVENT DATA LOSS**
 
 ## **Written in python, this library provides you with different file operation commands as well as info gathering commands on directories as well as files.** 
 ____________________________________________________________________________
-## **CHANGELOG: 1.2.4**
-- Release version 1.2.4
-- Added new functions: createFile and removeFile
-- With these new functions, you can easily create and remove singular files.
-- Fixed some README issues.
-
-If you want to create a single file, you can do so like this:
+## **CHANGELOG: V2.0.0**
 
-```
-from FinderZ import fileOperands
-
-fileOperands.createFile("FileName", "fileCreationPath")
-```
-Note that the "FileName" in this case may also include a file extension.
+To check out the details of V2, go to the [documentation](https://finderz.readthedocs.io/en/latest/index.html). This is a big update with many new things!
 
-- Documentation will be added soon that explains each function and functionality of each function in a detailed manner.
-
-Thank you all for 10K Downloads!
 
 ## **Usage**
 Installation:
 ```
 pip3 install FinderZ
 ```
 Importing:
 ```
 import FinderZ
 ```
-Example for finding files with a specific keyword:
-```
-FinderZ.fileOperands.findFiles("fileName", "Custom Directory")
-```
-Or, if you want to import a single class:
-```
-from FinderZ import fileOperands
 
-#Find the file, calling the command "fO":
-print(fileOperands.findFiles("fileName", "Custom Path"))
-```
 ## **Features**
-- Consists of three classes: GatherInfo, fileOperands, and callBash.
-- Find any file with a certain keyword. This means you no longer have to necessarily know the full name of the file in case you forgot it. 
-- Gather information such as files in a directory, name of those files, and even a createFiles tool as well as a curated removeFiles tool.
-- Is easy to add new things to the library.
+- Consists of three classes: GatherInfo, fileOperands, Synchronize, Backup, and callBash.
+- Advanced file operations, already built for you (including many options to choose from!) 
+- Supports regex operations for some functions, as well as specific filters and multiple other choices to choose from. Options such as exact search or something even just containing a keyword, or even having the option to choose to seaerch recursively, are all included.
+- Includes full-featured, reliable synchronization and backup classes.
+- Full set of info gathering tools under the GatherInfo class.
+- Full-featured documentation to guide you through each function in detail. 
 - In case of functionality restrictions, callBash is a function that calls a bash script in order to expand functionality at its peak.
 - Easy to use.
 - You no longer have to take your time in making those file management algorithms that take a while to complete.
 - Fast and efficient, includes a plethora of other features. 
 ____________________________________________________________________________
 ## **Why?**
-- I wanted to showcase how one can easily create a full library that manages files in order to save time in an efficient way. 
+- FinderZ is a way to easily expand on the file system of many operating system. It supports, MacOS, Windows, Linux, and Android.
 - Who wouldn't want a tool to manage their files easily in their python scripts? This will save time!
 ____________________________________________________________________________
 ## **How?**
-- Using iterating techniques for a few of the functions, I was able to complete actions recursively through different directories. 
-- The use of the os and subprocess modules (especially os) made everything easier, and what I did was basically structure a library to make life easier.
+- FinderZ is composed of many iterating techniques and parametric options. Based on these options, the core of each function deals with a user's choice of what to do or what not to do.
+- More info under the documentation!
 ____________________________________________________________________________
 ## **User notice**
-- Some of the functions are only there in case one has to get user input or wants to format things in a more visible way. These functions include askMainDir, and the expandListInfo functions.
-- This project is still a work in progress! It is very flexible in adding new functions. So far, there are still basic functions being added frequently, and some more advanced functions being added gradually. Thanks for being patient, and enjoy!
+- I am not responsible for any damage or data lost using the FinderZ library. 
+- If using the Synchronize class, make sure renaming files or directories is never the last thing you do before synchronization, unless it is the only thing you did do (no adding, removing, copying, etc. files before)
+- This project has just been released to version 2! It has grown so much, but it is still growing and improving.
 ____________________________________________________________________________
 ## **Services used (Credits):**
 - [OS module](https://docs.python.org/3/library/os.html)
 - [Shutil module](https://docs.python.org/3/library/shutil.html)
+- [Time module](https://docs.python.org/3/library/time.html)
+- [Hashlib module](https://docs.python.org/3/library/hashlib.html)
+- [re](https://docs.python.org/3/library/re.html)
 - [Subprocess module](https://docs.python.org/3/library/subprocess.html)
 
 ____________________________________________________________________________
 ## **Make sure to leave a star!**
 - If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
```

