# Comparing `tmp/pcloud-1.1.tar.gz` & `tmp/pcloud-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcloud-1.1.tar", last modified: Mon Nov 14 17:22:35 2022, max compression
+gzip compressed data, was "pcloud-1.2.tar", last modified: Sat Jun 24 05:54:06 2023, max compression
```

## Comparing `pcloud-1.1.tar` & `pcloud-1.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-11-14 17:22:35.601806 pcloud-1.1/
--rw-r--r--   0 tom        (501) staff       (20)     3044 2022-11-14 17:22:34.000000 pcloud-1.1/CHANGES.rst
--rw-r--r--   0 tom        (501) staff       (20)     3352 2022-11-14 17:22:34.000000 pcloud-1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 tom        (501) staff       (20)      143 2022-11-14 17:22:34.000000 pcloud-1.1/CONTRIBUTORS.rst
--rw-r--r--   0 tom        (501) staff       (20)     1066 2022-11-14 17:22:34.000000 pcloud-1.1/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)      141 2022-11-14 17:22:34.000000 pcloud-1.1/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)     8969 2022-11-14 17:22:35.601943 pcloud-1.1/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     4819 2022-11-14 17:22:34.000000 pcloud-1.1/README.rst
--rw-r--r--   0 tom        (501) staff       (20)      427 2022-11-14 17:22:34.000000 pcloud-1.1/SECURITY.md
--rw-r--r--   0 tom        (501) staff       (20)       79 2022-11-14 17:22:35.602344 pcloud-1.1/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     1817 2022-11-14 17:22:34.000000 pcloud-1.1/setup.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-11-14 17:22:35.591326 pcloud-1.1/src/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-11-14 17:22:35.596122 pcloud-1.1/src/pcloud/
--rw-r--r--   0 tom        (501) staff       (20)       77 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    16704 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/api.py
--rw-r--r--   0 tom        (501) staff       (20)     1563 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/oauth2.py
--rw-r--r--   0 tom        (501) staff       (20)     5906 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/pcloudfs.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-11-14 17:22:35.599909 pcloud-1.1/src/pcloud/tests/
--rw-r--r--   0 tom        (501) staff       (20)      500 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/conftest.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-11-14 17:22:35.601562 pcloud-1.1/src/pcloud/tests/data/
--rw-r--r--   0 tom        (501) staff       (20)      256 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/data/extractarchive.json
--rw-r--r--   0 tom        (501) staff       (20)       19 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/data/file_close.json
--rw-r--r--   0 tom        (501) staff       (20)       52 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/data/file_open.json
--rw-r--r--   0 tom        (501) staff       (20)      129 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/data/getdigest.json
--rw-r--r--   0 tom        (501) staff       (20)       14 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/data/upload.txt
--rw-r--r--   0 tom        (501) staff       (20)       41 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/data/userinfo.json
--rw-r--r--   0 tom        (501) staff       (20)     1433 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/server.py
--rw-r--r--   0 tom        (501) staff       (20)     2195 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/test_api.py
--rw-r--r--   0 tom        (501) staff       (20)     2375 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/test_integration.py
--rw-r--r--   0 tom        (501) staff       (20)     2237 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/test_oauth2.py
--rw-r--r--   0 tom        (501) staff       (20)     1731 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/tests/test_validate.py
--rw-r--r--   0 tom        (501) staff       (20)      974 2022-11-14 17:22:34.000000 pcloud-1.1/src/pcloud/validate.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-11-14 17:22:35.598118 pcloud-1.1/src/pcloud.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     8969 2022-11-14 17:22:35.000000 pcloud-1.1/src/pcloud.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      889 2022-11-14 17:22:35.000000 pcloud-1.1/src/pcloud.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2022-11-14 17:22:35.000000 pcloud-1.1/src/pcloud.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       98 2022-11-14 17:22:35.000000 pcloud-1.1/src/pcloud.egg-info/entry_points.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2022-11-14 17:22:35.000000 pcloud-1.1/src/pcloud.egg-info/not-zip-safe
--rw-r--r--   0 tom        (501) staff       (20)       49 2022-11-14 17:22:35.000000 pcloud-1.1/src/pcloud.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)        7 2022-11-14 17:22:35.000000 pcloud-1.1/src/pcloud.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)      111 2022-11-14 17:22:34.000000 pcloud-1.1/test_requirements.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-24 05:54:06.008827 pcloud-1.2/
+-rw-r--r--   0 tom        (501) staff       (20)     3559 2023-06-24 05:54:05.000000 pcloud-1.2/CHANGES.rst
+-rw-r--r--   0 tom        (501) staff       (20)     3137 2023-06-24 05:54:05.000000 pcloud-1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 tom        (501) staff       (20)     9783 2023-06-24 05:54:05.000000 pcloud-1.2/CONTRIBUTING.md
+-rw-r--r--   0 tom        (501) staff       (20)      143 2023-06-24 05:54:05.000000 pcloud-1.2/CONTRIBUTORS.rst
+-rw-r--r--   0 tom        (501) staff       (20)     1066 2023-06-24 05:54:05.000000 pcloud-1.2/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)      141 2023-06-24 05:54:05.000000 pcloud-1.2/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)     9508 2023-06-24 05:54:06.009024 pcloud-1.2/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     4843 2023-06-24 05:54:05.000000 pcloud-1.2/README.rst
+-rw-r--r--   0 tom        (501) staff       (20)      427 2023-06-24 05:54:05.000000 pcloud-1.2/SECURITY.md
+-rw-r--r--   0 tom        (501) staff       (20)       79 2023-06-24 05:54:06.009537 pcloud-1.2/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     1816 2023-06-24 05:54:05.000000 pcloud-1.2/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-24 05:54:05.994981 pcloud-1.2/src/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-24 05:54:06.001299 pcloud-1.2/src/pcloud/
+-rw-r--r--   0 tom        (501) staff       (20)       77 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    17407 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/api.py
+-rw-r--r--   0 tom        (501) staff       (20)     2051 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/oauth2.py
+-rw-r--r--   0 tom        (501) staff       (20)     5905 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/pcloudfs.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-24 05:54:06.006366 pcloud-1.2/src/pcloud/tests/
+-rw-r--r--   0 tom        (501) staff       (20)      500 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/conftest.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-24 05:54:06.008533 pcloud-1.2/src/pcloud/tests/data/
+-rw-r--r--   0 tom        (501) staff       (20)      256 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/data/extractarchive.json
+-rw-r--r--   0 tom        (501) staff       (20)       19 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/data/file_close.json
+-rw-r--r--   0 tom        (501) staff       (20)       52 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/data/file_open.json
+-rw-r--r--   0 tom        (501) staff       (20)      129 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/data/getdigest.json
+-rw-r--r--   0 tom        (501) staff       (20)       14 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/data/upload.txt
+-rw-r--r--   0 tom        (501) staff       (20)       41 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/data/userinfo.json
+-rw-r--r--   0 tom        (501) staff       (20)     1411 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/server.py
+-rw-r--r--   0 tom        (501) staff       (20)     3079 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/test_api.py
+-rw-r--r--   0 tom        (501) staff       (20)      304 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/test_helpers.py
+-rw-r--r--   0 tom        (501) staff       (20)     2605 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/test_integration.py
+-rw-r--r--   0 tom        (501) staff       (20)     2365 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/test_oauth2.py
+-rw-r--r--   0 tom        (501) staff       (20)     1745 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/tests/test_validate.py
+-rw-r--r--   0 tom        (501) staff       (20)      974 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud/validate.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-24 05:54:06.003894 pcloud-1.2/src/pcloud.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     9508 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      938 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       98 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud.egg-info/entry_points.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud.egg-info/not-zip-safe
+-rw-r--r--   0 tom        (501) staff       (20)       49 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)        7 2023-06-24 05:54:05.000000 pcloud-1.2/src/pcloud.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)      149 2023-06-24 05:54:05.000000 pcloud-1.2/test_requirements.txt
```

### Comparing `pcloud-1.1/CHANGES.rst` & `pcloud-1.2/CHANGES.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 =========
 
+1.2 (2023-06-24)
+----------------
+
+- Add `CONTRIBUTING` guideline and update `CODE_OF_CONDUCT` document [tomgross]
+- Add Sonarcloud checker and report test coverage [tomgross]
+- Add test for listtokens endpoint [tomgross]
+- Changed repo name to https://github.com/tomgross/pcloud/ to be consistent (https://github.com/tomgross/pcloud/issues/70) [tomgross]
+- Implement `sharefolder`-endpoint [tomgross]
+- Replace ``cgi.FieldStorage`` by ``multipart`` avoiding
+  the ``cgi`` module deprecated by Python 3.11. [tomgross]
+
 1.1 (2022-11-14)
 ----------------
 
 - Fix upload with int folderid #63 [tomgross]
 - Add pytest timeout and update testing dependencies [tomgross]
 - Implement `copyfile` and `downloadfileasync` methods [tomgross]
 - Implement `setlanguage`, `getfeedback`, `diff` & `getfilehistory` methods [tomgross]
@@ -24,17 +35,17 @@
 - Documented headless OAuth [tomgross]
 
 1.0b1 (2021-11-26)
 ------------------
 
 - Python 3.10 compatibility and dependency updates
 - Change port of test server 5000 -> 5023
-- Add *getpubzip* API method (https://github.com/tomgross/pycloud/issues/51)
+- Add *getpubzip* API method (https://github.com/tomgross/pcloud/issues/51)
 - Allow uploading BIG files by using MultipartEncoder of requests_toolbelt
-  (https://github.com/tomgross/pycloud/issues/25, https://github.com/tomgross/pycloud/issues/44)
+  (https://github.com/tomgross/pcloud/issues/25, https://github.com/tomgross/pcloud/issues/44)
 - Log login process
   [tomgross]
 
 1.0a10 (2021-07-11)
 -------------------
 
 - State and test Python 3.9 support [tomgross]
@@ -101,15 +112,15 @@
 - Fix error while using makedirs from PyFilesystem with recreate=True
   [blasterspike]
 
 1.0a5 (2018-10-22)
 ------------------
 
 - Fix error while using makedirs from PyFilesystem
-  https://github.com/tomgross/pycloud/issues/10
+  https://github.com/tomgross/pcloud/issues/10
   [blasterspike]
 
 - Test and claim Python 3.7 compatibility
   [tomgross]
 
 1.0a4 (2017-10-29)
 ------------------
```

### Comparing `pcloud-1.1/CODE_OF_CONDUCT.md` & `pcloud-1.2/CODE_OF_CONDUCT.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,70 @@
-# Contributor Covenant Code of Conduct
+# Code of Conduct - pCloud Python API
 
 ## Our Pledge
 
 In the interest of fostering an open and welcoming environment, we as
-contributors and maintainers pledge to making participation in our project and
+contributors and maintainers pledge to make participation in our project and
 our community a harassment-free experience for everyone, regardless of age, body
 size, disability, ethnicity, sex characteristics, gender identity and expression,
 level of experience, education, socio-economic status, nationality, personal
 appearance, race, religion, or sexual identity and orientation.
 
 ## Our Standards
 
-Examples of behavior that contributes to creating a positive environment
-include:
+Examples of behavior that contributes to a positive environment for our
+community include:
 
-* Using welcoming and inclusive language
-* Being respectful of differing viewpoints and experiences
-* Gracefully accepting constructive criticism
-* Focusing on what is best for the community
-* Showing empathy towards other community members
-
-Examples of unacceptable behavior by participants include:
-
-* The use of sexualized language or imagery and unwelcome sexual attention or
- advances
-* Trolling, insulting/derogatory comments, and personal or political attacks
+* Demonstrating empathy and kindness toward other people
+* Being respectful of differing opinions, viewpoints, and experiences
+* Giving and gracefully accepting constructive feedback
+* Accepting responsibility and apologizing to those affected by our mistakes,
+  and learning from the experience
+* Focusing on what is best not just for us as individuals, but for the
+  overall community
+
+Examples of unacceptable behavior include:
+
+* The use of sexualized language or imagery, and sexual attention or
+  advances
+* Trolling, insulting or derogatory comments, and personal or political attacks
 * Public or private harassment
-* Publishing others' private information, such as a physical or electronic
- address, without explicit permission
+* Publishing others' private information, such as a physical or email
+  address, without their explicit permission
 * Other conduct which could reasonably be considered inappropriate in a
- professional setting
+  professional setting
 
 ## Our Responsibilities
 
-Project maintainers are responsible for clarifying the standards of acceptable
-behavior and are expected to take appropriate and fair corrective action in
+Project maintainers are responsible for clarifying and enforcing our standards of
+acceptable behavior and will take appropriate and fair corrective action in
 response to any instances of unacceptable behavior.
 
-Project maintainers have the right and responsibility to remove, edit, or
-reject comments, commits, code, wiki edits, issues, and other contributions
-that are not aligned to this Code of Conduct, or to ban temporarily or
-permanently any contributor for other behaviors that they deem inappropriate,
-threatening, offensive, or harmful.
+Project maintainers have the right and responsibility to remove, edit, or reject
+comments, commits, code, wiki edits, issues, and other contributions that are
+not aligned to this Code of Conduct, or to ban
+temporarily or permanently any contributor for other behaviors that they deem
+inappropriate, threatening, offensive, or harmful.
 
 ## Scope
 
-This Code of Conduct applies both within project spaces and in public spaces
-when an individual is representing the project or its community. Examples of
-representing a project or community include using an official project e-mail
-address, posting via an official social media account, or acting as an appointed
-representative at an online or offline event. Representation of a project may be
-further defined and clarified by project maintainers.
+This Code of Conduct applies within all community spaces, and also applies when
+an individual is officially representing the community in public spaces.
+Examples of representing our community include using an official e-mail address,
+posting via an official social media account, or acting as an appointed
+representative at an online or offline event.
 
 ## Enforcement
 
 Instances of abusive, harassing, or otherwise unacceptable behavior may be
-reported by contacting the project team at itconsense@gmail.com. All
-complaints will be reviewed and investigated and will result in a response that
-is deemed necessary and appropriate to the circumstances. The project team is
-obligated to maintain confidentiality with regard to the reporter of an incident.
-Further details of specific enforcement policies may be posted separately.
-
-Project maintainers who do not follow or enforce the Code of Conduct in good
-faith may face temporary or permanent repercussions as determined by other
-members of the project's leadership.
+reported to the community leaders responsible for enforcement at <itconsense@gmail.com>.
+All complaints will be reviewed and investigated promptly and fairly.
 
-## Attribution
-
-This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4,
-available at https://www.contributor-covenant.org/version/1/4/code-of-conduct.html
+All community leaders are obligated to respect the privacy and security of the
+reporter of any incident.
 
-[homepage]: https://www.contributor-covenant.org
+## Attribution
 
-For answers to common questions about this code of conduct, see
-https://www.contributor-covenant.org/faq
+This Code of Conduct is adapted from the [Contributor Covenant](https://contributor-covenant.org/), version
+[1.4](https://www.contributor-covenant.org/version/1/4/code-of-conduct/code_of_conduct.md) and
+[2.0](https://www.contributor-covenant.org/version/2/0/code_of_conduct/code_of_conduct.md),
+and was generated by [contributing-gen](https://github.com/bttger/contributing-gen).
```

### Comparing `pcloud-1.1/LICENSE` & `pcloud-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pcloud-1.1/PKG-INFO` & `pcloud-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcloud
-Version: 1.1
+Version: 1.2
 Summary: A client library for pCloud
 Home-page: https://pypi.python.org/pypi/pcloud
 Author: Tom Gross
 Author-email: itconsense@gmail.com
 License: MIT
 Keywords: Python pCloud REST
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,16 +24,16 @@
 Provides-Extra: pyfs
 License-File: LICENSE
 
 ==============================================================================
 pcloud - A Python API client for pCloud
 ==============================================================================
 
-.. image:: https://travis-ci.org/tomgross/pycloud.svg?branch=master
-    :target: https://travis-ci.org/tomgross/pycloud
+.. image:: https://github.com/tomgross/pcloud/actions/workflows/pcloud-test.yml/badge.svg
+    :target: https://github.com/tomgross/pcloud/actions
 
 This Python **(Version >= 3.6 only!)** library provides a Python API to the pCloud storage.
 
 Features
 ========
 
 - Can be used as a library
@@ -161,16 +161,16 @@
 you need to add a file with the same name as the method + the `.json` suffix
 in the tests/data directory (like `getdigest.json`).
 The file contains the expected JSON result.
 
 Contribute
 ==========
 
-- Issue Tracker: https://github.com/tomgross/pycloud/issues
-- Source Code: https://github.com/tomgross/pycloud
+- Issue Tracker: https://github.com/tomgross/pcloud/issues
+- Source Code: https://github.com/tomgross/pcloud
 
 License
 =======
 
 The project is licensed under MIT (see LICENSE).
 
 
@@ -183,14 +183,25 @@
 - olokelo
 - qo4on
 
 
 Changelog
 =========
 
+1.2 (2023-06-24)
+----------------
+
+- Add `CONTRIBUTING` guideline and update `CODE_OF_CONDUCT` document [tomgross]
+- Add Sonarcloud checker and report test coverage [tomgross]
+- Add test for listtokens endpoint [tomgross]
+- Changed repo name to https://github.com/tomgross/pcloud/ to be consistent (https://github.com/tomgross/pcloud/issues/70) [tomgross]
+- Implement `sharefolder`-endpoint [tomgross]
+- Replace ``cgi.FieldStorage`` by ``multipart`` avoiding
+  the ``cgi`` module deprecated by Python 3.11. [tomgross]
+
 1.1 (2022-11-14)
 ----------------
 
 - Fix upload with int folderid #63 [tomgross]
 - Add pytest timeout and update testing dependencies [tomgross]
 - Implement `copyfile` and `downloadfileasync` methods [tomgross]
 - Implement `setlanguage`, `getfeedback`, `diff` & `getfilehistory` methods [tomgross]
@@ -210,17 +221,17 @@
 - Documented headless OAuth [tomgross]
 
 1.0b1 (2021-11-26)
 ------------------
 
 - Python 3.10 compatibility and dependency updates
 - Change port of test server 5000 -> 5023
-- Add *getpubzip* API method (https://github.com/tomgross/pycloud/issues/51)
+- Add *getpubzip* API method (https://github.com/tomgross/pcloud/issues/51)
 - Allow uploading BIG files by using MultipartEncoder of requests_toolbelt
-  (https://github.com/tomgross/pycloud/issues/25, https://github.com/tomgross/pycloud/issues/44)
+  (https://github.com/tomgross/pcloud/issues/25, https://github.com/tomgross/pcloud/issues/44)
 - Log login process
   [tomgross]
 
 1.0a10 (2021-07-11)
 -------------------
 
 - State and test Python 3.9 support [tomgross]
@@ -287,15 +298,15 @@
 - Fix error while using makedirs from PyFilesystem with recreate=True
   [blasterspike]
 
 1.0a5 (2018-10-22)
 ------------------
 
 - Fix error while using makedirs from PyFilesystem
-  https://github.com/tomgross/pycloud/issues/10
+  https://github.com/tomgross/pcloud/issues/10
   [blasterspike]
 
 - Test and claim Python 3.7 compatibility
   [tomgross]
 
 1.0a4 (2017-10-29)
 ------------------
```

### Comparing `pcloud-1.1/README.rst` & `pcloud-1.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ==============================================================================
 pcloud - A Python API client for pCloud
 ==============================================================================
 
-.. image:: https://travis-ci.org/tomgross/pycloud.svg?branch=master
-    :target: https://travis-ci.org/tomgross/pycloud
+.. image:: https://github.com/tomgross/pcloud/actions/workflows/pcloud-test.yml/badge.svg
+    :target: https://github.com/tomgross/pcloud/actions
 
 This Python **(Version >= 3.6 only!)** library provides a Python API to the pCloud storage.
 
 Features
 ========
 
 - Can be used as a library
@@ -135,14 +135,14 @@
 you need to add a file with the same name as the method + the `.json` suffix
 in the tests/data directory (like `getdigest.json`).
 The file contains the expected JSON result.
 
 Contribute
 ==========
 
-- Issue Tracker: https://github.com/tomgross/pycloud/issues
-- Source Code: https://github.com/tomgross/pycloud
+- Issue Tracker: https://github.com/tomgross/pcloud/issues
+- Source Code: https://github.com/tomgross/pcloud
 
 License
 =======
 
 The project is licensed under MIT (see LICENSE).
```

### Comparing `pcloud-1.1/setup.py` & `pcloud-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="pcloud",
-    version="1.1",
+    version="1.2",
     description="A client library for pCloud",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
@@ -44,15 +44,15 @@
     packages=find_packages("src", exclude=["ez_setup"]),
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         "requests",
         "requests-toolbelt",
-        "setuptools",
+        "setuptools"
     ],
     extras_require={"pyfs": ["fs"]},
     entry_points={
         "console_scripts": [
             "pcloud-cli = pcloud.api:main",
         ],
         "fs.opener": ["pcloud  = pcloud.pcloudfs:PCloudOpener"],
```

### Comparing `pcloud-1.1/src/pcloud/api.py` & `pcloud-1.2/src/pcloud/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 from pcloud.validate import MODE_AND
 from pcloud.validate import RequiredParameterCheck
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 from urllib.parse import urlparse
 from urllib.parse import urlunsplit
 
 import argparse
+import datetime
 import logging
 import os.path
 import requests
 import sys
 import zipfile
 
 
-log = logging.getLogger("pycloud")
+log = logging.getLogger("pcloud")
 log.setLevel(logging.INFO)
 
 handler = logging.StreamHandler(sys.stderr)
 handler.setLevel(logging.INFO)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 handler.setFormatter(formatter)
 log.addHandler(handler)
@@ -39,29 +40,41 @@
     """Authentication failed"""
 
 
 class OnlyPcloudError(NotImplementedError):
     """Feature restricted to pCloud"""
 
 
+# Helpers
+
+
+def to_api_datetime(dt):
+    """Converter to a datetime structure the pCloud API understands
+
+    See https://docs.pcloud.com/structures/datetime.html
+    """
+    if isinstance(dt, datetime.datetime):
+        return dt.isoformat()
+    return dt
+
+
 def main():
     parser = argparse.ArgumentParser(description="pCloud command line client")
     parser.add_argument(
         "username", help="The username for login into your pCloud account"
     )
     parser.add_argument(
         "password", help="The password for login into your pCloud account"
     )
     args = parser.parse_args()
     pyc = PyCloud(args.username, args.password)
     print(pyc)
 
 
 class PyCloud(object):
-
     endpoints = {
         "api": "https://api.pcloud.com/",
         "eapi": "https://eapi.pcloud.com/",
         "test": "http://localhost:5023/",
         "nearest": "",
     }
 
@@ -436,21 +449,30 @@
         return self._do_request("extractarchiveprogress", **kwargs)
 
     @RequiredParameterCheck(("progresshash",))
     def savezipprogress(self, **kwargs):
         return self._do_request("savezipprogress", **kwargs)
 
     # Sharing
+    @RequiredParameterCheck(("path", "folderid"))
+    @RequiredParameterCheck(("mail", "permissions"), mode=MODE_AND)
     def sharefolder(self, **kwargs):
-        raise NotImplementedError
+        return self._do_request("sharefolder", **kwargs)
 
     def listshares(self, **kwargs):
-        return self._do_request("listshares")
+        return self._do_request("listshares", **kwargs)
 
     # Public links
+    @RequiredParameterCheck(("path", "folderid"))
+    def getfolderpublink(self, **kwargs):
+        expire = kwargs.get("expire")
+        if expire is not None:
+            kwargs["expire"] = to_api_datetime(expire)
+        return self._do_request("getfolderpublink", **kwargs)
+
     @RequiredParameterCheck(("code",))
     def getpubzip(self, unzip=False, **kwargs):
         zipresponse = self._do_request(
             "getpubzip", authenticate=False, json=False, **kwargs
         )
         if not unzip:
             return zipresponse
```

### Comparing `pcloud-1.1/src/pcloud/oauth2.py` & `pcloud-1.2/src/pcloud/oauth2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+import _thread
+
 from http.server import BaseHTTPRequestHandler
 from http.server import HTTPServer
 from urllib.parse import parse_qs
 from urllib.parse import urlparse
 from webbrowser import open_new
 
 
@@ -36,18 +38,28 @@
     redirect_url = REDIRECT_URL
 
     def __init__(self, client_id):
         self._id = client_id
         self.auth_url = f"https://my.pcloud.com/oauth2/authorize?response_type=code&redirect_uri={self.redirect_url}&client_id={self._id}"
 
     def open_browser(self):
+        """Hook which is called before request is handled."""
         open_new(self.auth_url)
 
     def close_browser(self):
-        pass
+        """Hook which is called after request is handled."""
 
     def get_access_token(self):
+        http_server = HTTPServer(("localhost", PORT), HTTPServerHandler)
+
+        # Solution taken from https://stackoverflow.com/a/12651298
+        # There might be better ways than accessing the internal
+        # _thread library for starting the http-server non-blocking
+        # but I did not found any ;-)
+        def start_server():
+            http_server.handle_request()
+
+        _thread.start_new_thread(start_server, ())
         self.open_browser()
-        httpServer = HTTPServer(("localhost", PORT), HTTPServerHandler)
-        httpServer.handle_request()
         self.close_browser()
-        return httpServer.access_token, httpServer.pc_hostname
+        http_server.server_close()
+        return http_server.access_token, http_server.pc_hostname
```

### Comparing `pcloud-1.1/src/pcloud/pcloudfs.py` & `pcloud-1.2/src/pcloud/pcloudfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,14 @@
         self.pcloud.deletefolder(path=path)
 
     def removetree(self, dir_path):
         self.pcloud.deletefolderrecursive(path=dir_path)
 
 
 class PCloudOpener(Opener):
-
     protocols = ["pcloud"]
 
     @staticmethod
     def open_fs(fs_url, parse_result, writeable, create, cwd):
         _, _, directory = parse_result.resource.partition("/")
         fs = PCloudFS(username=parse_result.username, password=parse_result.password)
         if directory:
```

### Comparing `pcloud-1.1/src/pcloud/tests/server.py` & `pcloud-1.2/src/pcloud/tests/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 from http.server import BaseHTTPRequestHandler
-
+from multipart import MultipartParser
+from multipart import parse_options_header
 from os.path import dirname
 from os.path import join
 import socketserver
-import cgi
 
 
 class MockHandler(BaseHTTPRequestHandler):
     # Handler for GET requests
     def do_GET(self):
         self.send_response(200)
         self.send_header("Content-type", "applicaton/json")
@@ -17,32 +17,25 @@
         path = self.path[1:].split("?")
         with open(join(dirname(__file__), "data", path[0] + ".json")) as f:
             data = f.read()
         self.wfile.write(bytes(data, "utf-8"))
 
     # Handler for POST requests
     def do_POST(self):
-        form = cgi.FieldStorage(
-            fp=self.rfile,
-            headers=self.headers,
-            environ={
-                "REQUEST_METHOD": "POST",
-                "CONTENT_TYPE": self.headers["Content-Type"],
-            },
+        content_length = int(self.headers["Content-Length"])
+        _, options = parse_options_header(self.headers["Content-Type"])
+        form = MultipartParser(
+            self.rfile, options["boundary"], content_length=content_length
         )
-        if "upload.txt" in form:
-            file_ = form.getvalue("upload.txt")
-        else:
-            file_ = form.getvalue("file")
-        size = len(file_)
+        file_ = form.get("file")
         self.send_response(200)
         self.send_header("Content-type", "applicaton/json")
         self.end_headers()
-        print(f"File: {file_}, Size: {size}", end="")
+        print(f"File: {file_.value.encode('utf-8')}, Size: {file_.size}", end="")
         # Send the json message
         self.wfile.write(
-            bytes('{ "result": 0, "metadata": {"size": %s} }' % size, "utf-8")
+            bytes('{ "result": 0, "metadata": {"size": %s} }' % file_.size, "utf-8")
         )
 
 
 class MockServer(socketserver.TCPServer):
     allow_reuse_address = True
```

### Comparing `pcloud-1.1/src/pcloud/tests/test_api.py` & `pcloud-1.2/src/pcloud/tests/test_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,60 @@
 #
 from pcloud import api
 from pcloud.pcloudfs import PCloudFS
 
+import datetime
 import json
 import os.path
 import pytest
 
 
+class NoOpSession(object):
+    kwargs = {}
+
+    def get(self, url, **kwargs):
+        self.kwargs = kwargs
+        self.kwargs["url"] = url
+        return self
+
+    def json(self):
+        return self.kwargs
+
+
 class DummyPyCloud(api.PyCloud):
-    def __init__(self, username, password):
+    noop = False
+
+    def get_auth_token(self):
+        if self.noop:
+            self.auth_token = None
+            self.access_token = None
+        else:
+            return super(DummyPyCloud, self).get_auth_token()
+
+    def __init__(self, username, password, noop=False):
+        if noop:
+            self.noop = True
         super(DummyPyCloud, self).__init__(username, password, endpoint="test")
+        if noop:
+            self.session = NoOpSession()
 
 
 class DummyPCloudFS(PCloudFS):
-
     factory = DummyPyCloud
 
 
+def test_getfolderpublink():
+    api = DummyPyCloud("john", "doe", noop=True)
+    dt = datetime.datetime(2023, 10, 5, 12, 3, 12)
+    assert api.getfolderpublink(folderid=20, expire=dt) == {
+        "params": {"expire": "2023-10-05T12:03:12", "folderid": 20},
+        "url": "http://localhost:5023/getfolderpublink",
+    }
+
+
 @pytest.mark.usefixtures("start_mock_server")
 class TestPcloudApi(object):
     def test_getdigest(self):
         api = DummyPyCloud("foo", "bar")
         assert api.getdigest() == b"YGtAxbUpI85Zvs7lC7Z62rBwv907TBXhV2L867Hkh"
 
     def test_get_auth_token(self):
```

### Comparing `pcloud-1.1/src/pcloud/tests/test_integration.py` & `pcloud-1.2/src/pcloud/tests/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import pytest
+import time
 import zipfile
 
 from io import BytesIO
 from pathlib import Path
 from pcloud.api import PyCloud
 from pcloud.api import O_CREAT
 
@@ -60,13 +61,23 @@
     zipfmem = BytesIO(zipresponse)
     zf = zipfile.ZipFile(zipfmem)
     result_code = zf.testzip()
     assert result_code is None
 
 
 def test_copyfile(pycloud, testfolder):
-    testfilename = 'Getting started with pCloud.pdf'
-    tofilename = f'/{folder_for_tests}/{testfilename}'
-    resp = pycloud.copyfile(path=f'/{testfilename}', topath=tofilename)
-    assert resp['result'] == 0
+    testfilename = "Getting started with pCloud.pdf"
+    tofilename = f"/{folder_for_tests}/{testfilename}"
+    resp = pycloud.copyfile(path=f"/{testfilename}", topath=tofilename)
+    assert resp["result"] == 0
+    time.sleep(1)
     resp = pycloud.checksumfile(path=tofilename)
-    assert resp['sha256'] == 'df745d42f69266c49141ea7270c45240cf883b9cdb6a14fffcdff33c04c5304c'
+    assert (
+        resp.get("sha256")
+        == "df745d42f69266c49141ea7270c45240cf883b9cdb6a14fffcdff33c04c5304c"
+    ), f"Failure with checksum in {resp}"
+
+
+def test_listtokens(pycloud):
+    result = pycloud.listtokens()
+    assert result["result"] == 0
+    assert len(result["tokens"]) > 1
```

### Comparing `pcloud-1.1/src/pcloud/tests/test_validate.py` & `pcloud-1.2/src/pcloud/tests/test_validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 
     def test_validiate_all_path(self):
         with pytest.raises(ValueError):
             foo_all(path="/", bar="x")
 
     def test_validiate_all_folderid(self):
         with pytest.raises(ValueError):
-            foo_all(folderid="0") == (None, "0", None)
+            assert foo_all(folderid="0") == (None, "0", None)
 
     def test_validiate_all(self):
-        foo_all(folderid="0", path="/") == ("/", "0", None)
+        assert foo_all(folderid="0", path="/") == ("/", "0", None)
 
 
 class TestMultipleValidators(object):
     def test_single(self):
         with pytest.raises(ValueError):
             assert extractarchive(path="1", fileid=1)
```

### Comparing `pcloud-1.1/src/pcloud/validate.py` & `pcloud-1.2/src/pcloud/validate.py`

 * *Files identical despite different names*

### Comparing `pcloud-1.1/src/pcloud.egg-info/PKG-INFO` & `pcloud-1.2/src/pcloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcloud
-Version: 1.1
+Version: 1.2
 Summary: A client library for pCloud
 Home-page: https://pypi.python.org/pypi/pcloud
 Author: Tom Gross
 Author-email: itconsense@gmail.com
 License: MIT
 Keywords: Python pCloud REST
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,16 +24,16 @@
 Provides-Extra: pyfs
 License-File: LICENSE
 
 ==============================================================================
 pcloud - A Python API client for pCloud
 ==============================================================================
 
-.. image:: https://travis-ci.org/tomgross/pycloud.svg?branch=master
-    :target: https://travis-ci.org/tomgross/pycloud
+.. image:: https://github.com/tomgross/pcloud/actions/workflows/pcloud-test.yml/badge.svg
+    :target: https://github.com/tomgross/pcloud/actions
 
 This Python **(Version >= 3.6 only!)** library provides a Python API to the pCloud storage.
 
 Features
 ========
 
 - Can be used as a library
@@ -161,16 +161,16 @@
 you need to add a file with the same name as the method + the `.json` suffix
 in the tests/data directory (like `getdigest.json`).
 The file contains the expected JSON result.
 
 Contribute
 ==========
 
-- Issue Tracker: https://github.com/tomgross/pycloud/issues
-- Source Code: https://github.com/tomgross/pycloud
+- Issue Tracker: https://github.com/tomgross/pcloud/issues
+- Source Code: https://github.com/tomgross/pcloud
 
 License
 =======
 
 The project is licensed under MIT (see LICENSE).
 
 
@@ -183,14 +183,25 @@
 - olokelo
 - qo4on
 
 
 Changelog
 =========
 
+1.2 (2023-06-24)
+----------------
+
+- Add `CONTRIBUTING` guideline and update `CODE_OF_CONDUCT` document [tomgross]
+- Add Sonarcloud checker and report test coverage [tomgross]
+- Add test for listtokens endpoint [tomgross]
+- Changed repo name to https://github.com/tomgross/pcloud/ to be consistent (https://github.com/tomgross/pcloud/issues/70) [tomgross]
+- Implement `sharefolder`-endpoint [tomgross]
+- Replace ``cgi.FieldStorage`` by ``multipart`` avoiding
+  the ``cgi`` module deprecated by Python 3.11. [tomgross]
+
 1.1 (2022-11-14)
 ----------------
 
 - Fix upload with int folderid #63 [tomgross]
 - Add pytest timeout and update testing dependencies [tomgross]
 - Implement `copyfile` and `downloadfileasync` methods [tomgross]
 - Implement `setlanguage`, `getfeedback`, `diff` & `getfilehistory` methods [tomgross]
@@ -210,17 +221,17 @@
 - Documented headless OAuth [tomgross]
 
 1.0b1 (2021-11-26)
 ------------------
 
 - Python 3.10 compatibility and dependency updates
 - Change port of test server 5000 -> 5023
-- Add *getpubzip* API method (https://github.com/tomgross/pycloud/issues/51)
+- Add *getpubzip* API method (https://github.com/tomgross/pcloud/issues/51)
 - Allow uploading BIG files by using MultipartEncoder of requests_toolbelt
-  (https://github.com/tomgross/pycloud/issues/25, https://github.com/tomgross/pycloud/issues/44)
+  (https://github.com/tomgross/pcloud/issues/25, https://github.com/tomgross/pcloud/issues/44)
 - Log login process
   [tomgross]
 
 1.0a10 (2021-07-11)
 -------------------
 
 - State and test Python 3.9 support [tomgross]
@@ -287,15 +298,15 @@
 - Fix error while using makedirs from PyFilesystem with recreate=True
   [blasterspike]
 
 1.0a5 (2018-10-22)
 ------------------
 
 - Fix error while using makedirs from PyFilesystem
-  https://github.com/tomgross/pycloud/issues/10
+  https://github.com/tomgross/pcloud/issues/10
   [blasterspike]
 
 - Test and claim Python 3.7 compatibility
   [tomgross]
 
 1.0a4 (2017-10-29)
 ------------------
```

### Comparing `pcloud-1.1/src/pcloud.egg-info/SOURCES.txt` & `pcloud-1.2/src/pcloud.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 CHANGES.rst
 CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 CONTRIBUTORS.rst
 LICENSE
 MANIFEST.in
 README.rst
 SECURITY.md
 setup.cfg
 setup.py
@@ -19,14 +20,15 @@
 src/pcloud.egg-info/entry_points.txt
 src/pcloud.egg-info/not-zip-safe
 src/pcloud.egg-info/requires.txt
 src/pcloud.egg-info/top_level.txt
 src/pcloud/tests/conftest.py
 src/pcloud/tests/server.py
 src/pcloud/tests/test_api.py
+src/pcloud/tests/test_helpers.py
 src/pcloud/tests/test_integration.py
 src/pcloud/tests/test_oauth2.py
 src/pcloud/tests/test_validate.py
 src/pcloud/tests/data/extractarchive.json
 src/pcloud/tests/data/file_close.json
 src/pcloud/tests/data/file_open.json
 src/pcloud/tests/data/getdigest.json
```

