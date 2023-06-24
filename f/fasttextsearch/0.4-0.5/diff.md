# Comparing `tmp/fasttextsearch-0.4.tar.gz` & `tmp/fasttextsearch-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/ceph-kw/kangwei/code/text_search/dist/.tmp-qz66j422/fasttextsearch-0.4.tar", last modified: Tue May 16 11:03:30 2023, max compression
+gzip compressed data, was "/ceph-kw/kangwei/code/text_search/dist/.tmp-ommy2sa7/fasttextsearch-0.5.tar", last modified: Sat Jun 24 07:37:05 2023, max compression
```

## Comparing `fasttextsearch-0.4.tar` & `fasttextsearch-0.5.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.145554 fasttextsearch-0.4/
--rw-r--r--   0 kangwei   (1092) root         (0)     2277 2023-05-16 08:11:03.000000 fasttextsearch-0.4/CMakeLists.txt
--rw-r--r--   0 kangwei   (1092) root         (0)      143 2023-05-16 08:44:49.000000 fasttextsearch-0.4/MANIFEST.in
--rw-r--r--   0 kangwei   (1092) root         (0)     1185 2023-05-16 11:03:30.145554 fasttextsearch-0.4/PKG-INFO
--rw-r--r--   0 kangwei   (1092) root         (0)      593 2023-04-24 12:23:40.000000 fasttextsearch-0.4/README.md
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.103554 fasttextsearch-0.4/cmake/
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.105553 fasttextsearch-0.4/cmake/Modules/
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.105553 fasttextsearch-0.4/cmake/Modules/FetchContent/
--rw-r--r--   0 kangwei   (1092) root         (0)      831 2023-02-18 07:20:27.000000 fasttextsearch-0.4/cmake/Modules/FetchContent/CMakeLists.cmake.in
--rw-r--r--   0 kangwei   (1092) root         (0)    38023 2023-02-18 07:20:27.000000 fasttextsearch-0.4/cmake/Modules/FetchContent.cmake
--rw-r--r--   0 kangwei   (1092) root         (0)      135 2023-02-18 07:20:27.000000 fasttextsearch-0.4/cmake/Modules/README.md
--rw-r--r--   0 kangwei   (1092) root         (0)        0 2023-02-18 07:20:27.000000 fasttextsearch-0.4/cmake/__init__.py
--rw-r--r--   0 kangwei   (1092) root         (0)     3421 2023-03-31 03:33:51.000000 fasttextsearch-0.4/cmake/googletest.cmake
--rw-r--r--   0 kangwei   (1092) root         (0)     1800 2023-03-31 03:33:51.000000 fasttextsearch-0.4/cmake/pybind11.cmake
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.110554 fasttextsearch-0.4/fasttextsearch.egg-info/
--rw-r--r--   0 kangwei   (1092) root         (0)     1185 2023-05-16 11:03:30.000000 fasttextsearch-0.4/fasttextsearch.egg-info/PKG-INFO
--rw-r--r--   0 kangwei   (1092) root         (0)     2357 2023-05-16 11:03:30.000000 fasttextsearch-0.4/fasttextsearch.egg-info/SOURCES.txt
--rw-r--r--   0 kangwei   (1092) root         (0)        1 2023-05-16 11:03:30.000000 fasttextsearch-0.4/fasttextsearch.egg-info/dependency_links.txt
--rw-r--r--   0 kangwei   (1092) root         (0)        6 2023-05-16 11:03:30.000000 fasttextsearch-0.4/fasttextsearch.egg-info/requires.txt
--rw-r--r--   0 kangwei   (1092) root         (0)       24 2023-05-16 11:03:30.000000 fasttextsearch-0.4/fasttextsearch.egg-info/top_level.txt
--rw-r--r--   0 kangwei   (1092) root         (0)      769 2023-05-16 11:03:20.000000 fasttextsearch-0.4/pyproject.toml
--rw-r--r--   0 kangwei   (1092) root         (0)        6 2023-05-16 07:33:05.000000 fasttextsearch-0.4/requirements.txt
--rw-r--r--   0 kangwei   (1092) root         (0)       38 2023-05-16 11:03:30.146554 fasttextsearch-0.4/setup.cfg
--rw-r--r--   0 kangwei   (1092) root         (0)     2986 2023-05-16 10:41:11.000000 fasttextsearch-0.4/setup.py
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.111554 fasttextsearch-0.4/textsearch/
--rw-r--r--   0 kangwei   (1092) root         (0)       48 2023-02-18 12:05:47.000000 fasttextsearch-0.4/textsearch/CMakeLists.txt
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.120554 fasttextsearch-0.4/textsearch/csrc/
--rw-r--r--   0 kangwei   (1092) root         (0)      695 2023-05-16 07:24:32.000000 fasttextsearch-0.4/textsearch/csrc/CMakeLists.txt
--rw-r--r--   0 kangwei   (1092) root         (0)    13272 2023-05-04 04:46:37.000000 fasttextsearch-0.4/textsearch/csrc/levenshtein.h
--rw-r--r--   0 kangwei   (1092) root         (0)     4137 2023-05-04 04:46:37.000000 fasttextsearch-0.4/textsearch/csrc/levenshtein_test.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     4664 2023-05-04 04:46:37.000000 fasttextsearch-0.4/textsearch/csrc/match.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     4611 2023-05-04 04:46:37.000000 fasttextsearch-0.4/textsearch/csrc/match.h
--rw-r--r--   0 kangwei   (1092) root         (0)     3248 2023-05-04 04:46:37.000000 fasttextsearch-0.4/textsearch/csrc/match_test.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     5273 2023-04-12 07:57:56.000000 fasttextsearch-0.4/textsearch/csrc/suffix_array.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     3207 2023-03-31 03:33:51.000000 fasttextsearch-0.4/textsearch/csrc/suffix_array.h
--rw-r--r--   0 kangwei   (1092) root         (0)     3883 2023-04-24 11:25:03.000000 fasttextsearch-0.4/textsearch/csrc/suffix_array_test.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     2880 2023-04-24 11:25:03.000000 fasttextsearch-0.4/textsearch/csrc/utils.cc
--rw-r--r--   0 kangwei   (1092) root         (0)     3508 2023-04-24 11:25:03.000000 fasttextsearch-0.4/textsearch/csrc/utils.h
--rw-r--r--   0 kangwei   (1092) root         (0)     4862 2023-04-24 11:25:03.000000 fasttextsearch-0.4/textsearch/csrc/utils_test.cc
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.120554 fasttextsearch-0.4/textsearch/python/
--rw-r--r--   0 kangwei   (1092) root         (0)       78 2023-05-16 07:26:44.000000 fasttextsearch-0.4/textsearch/python/CMakeLists.txt
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.128553 fasttextsearch-0.4/textsearch/python/csrc/
--rw-r--r--   0 kangwei   (1092) root         (0)      169 2023-05-16 07:25:08.000000 fasttextsearch-0.4/textsearch/python/csrc/CMakeLists.txt
--rw-r--r--   0 kangwei   (1092) root         (0)     4925 2023-05-04 04:46:37.000000 fasttextsearch-0.4/textsearch/python/csrc/levenshtein.cc
--rw-r--r--   0 kangwei   (1092) root         (0)      985 2023-03-06 09:09:29.000000 fasttextsearch-0.4/textsearch/python/csrc/levenshtein.h
--rw-r--r--   0 kangwei   (1092) root         (0)     1850 2023-05-04 04:46:37.000000 fasttextsearch-0.4/textsearch/python/csrc/match.cc
--rw-r--r--   0 kangwei   (1092) root         (0)      961 2023-05-04 04:46:37.000000 fasttextsearch-0.4/textsearch/python/csrc/match.h
--rw-r--r--   0 kangwei   (1092) root         (0)     1637 2023-04-13 03:32:42.000000 fasttextsearch-0.4/textsearch/python/csrc/suffix_array.cc
--rw-r--r--   0 kangwei   (1092) root         (0)      988 2023-03-06 09:09:29.000000 fasttextsearch-0.4/textsearch/python/csrc/suffix_array.h
--rw-r--r--   0 kangwei   (1092) root         (0)      564 2023-05-16 11:01:58.000000 fasttextsearch-0.4/textsearch/python/csrc/text_search.cc
--rw-r--r--   0 kangwei   (1092) root         (0)      357 2023-03-31 03:33:51.000000 fasttextsearch-0.4/textsearch/python/csrc/text_search.h
--rw-r--r--   0 kangwei   (1092) root         (0)     4599 2023-04-24 11:25:03.000000 fasttextsearch-0.4/textsearch/python/csrc/utils.cc
--rw-r--r--   0 kangwei   (1092) root         (0)      318 2023-04-21 06:51:44.000000 fasttextsearch-0.4/textsearch/python/csrc/utils.h
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.134554 fasttextsearch-0.4/textsearch/python/tests/
--rw-r--r--   0 kangwei   (1092) root         (0)      848 2023-05-16 10:58:23.000000 fasttextsearch-0.4/textsearch/python/tests/CMakeLists.txt
--rwxr-xr-x   0 kangwei   (1092) root         (0)     4748 2023-04-24 11:25:03.000000 fasttextsearch-0.4/textsearch/python/tests/test_find_close_matches.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)     1943 2023-04-13 03:32:42.000000 fasttextsearch-0.4/textsearch/python/tests/test_levenshtein_distance.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)     1414 2023-05-04 04:46:37.000000 fasttextsearch-0.4/textsearch/python/tests/test_match.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)      950 2023-03-31 03:33:51.000000 fasttextsearch-0.4/textsearch/python/tests/test_row_ids_to_row_splits.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)    10687 2023-04-13 03:32:42.000000 fasttextsearch-0.4/textsearch/python/tests/test_sourced_text.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)     1359 2023-04-24 11:25:03.000000 fasttextsearch-0.4/textsearch/python/tests/test_suffix_array.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)     2007 2023-03-31 03:33:51.000000 fasttextsearch-0.4/textsearch/python/tests/test_text_source.py
--rwxr-xr-x   0 kangwei   (1092) root         (0)     2314 2023-03-31 03:33:51.000000 fasttextsearch-0.4/textsearch/python/tests/test_transcript.py
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.139554 fasttextsearch-0.4/textsearch/python/textsearch/
--rw-r--r--   0 kangwei   (1092) root         (0)     1871 2023-05-16 11:03:29.000000 fasttextsearch-0.4/textsearch/python/textsearch/__init__.py
-drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-05-16 11:03:30.144554 fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/
--rw-r--r--   0 kangwei   (1092) root         (0)     1292 2023-05-16 10:58:31.000000 fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)     8961 2023-05-05 09:46:59.000000 fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/datatypes.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)     2543 2023-05-05 09:46:59.000000 fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/levenshtein.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)    22969 2023-05-16 11:02:18.000000 fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/match.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)     5132 2023-05-16 11:02:18.000000 fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/suffix_array.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)     2910 2023-04-13 07:06:10.000000 fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/text_search.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)     3325 2023-05-16 11:02:18.000000 fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 kangwei   (1092) root         (0)    12992 2023-04-24 11:25:03.000000 fasttextsearch-0.4/textsearch/python/textsearch/datatypes.py
--rw-r--r--   0 kangwei   (1092) root         (0)     3594 2023-04-24 11:25:03.000000 fasttextsearch-0.4/textsearch/python/textsearch/levenshtein.py
--rw-r--r--   0 kangwei   (1092) root         (0)    39883 2023-05-16 07:26:01.000000 fasttextsearch-0.4/textsearch/python/textsearch/match.py
--rw-r--r--   0 kangwei   (1092) root         (0)     6695 2023-05-16 07:26:33.000000 fasttextsearch-0.4/textsearch/python/textsearch/suffix_array.py
--rw-r--r--   0 kangwei   (1092) root         (0)     3165 2023-05-16 07:26:31.000000 fasttextsearch-0.4/textsearch/python/textsearch/utils.py
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.170072 fasttextsearch-0.5/
+-rw-r--r--   0 kangwei   (1092) root         (0)     2277 2023-06-24 07:05:13.000000 fasttextsearch-0.5/CMakeLists.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)      143 2023-06-24 07:05:13.000000 fasttextsearch-0.5/MANIFEST.in
+-rw-r--r--   0 kangwei   (1092) root         (0)     1169 2023-06-24 07:37:05.169072 fasttextsearch-0.5/PKG-INFO
+-rw-r--r--   0 kangwei   (1092) root         (0)      577 2023-06-24 07:05:13.000000 fasttextsearch-0.5/README.md
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.131072 fasttextsearch-0.5/cmake/
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.133072 fasttextsearch-0.5/cmake/Modules/
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.134072 fasttextsearch-0.5/cmake/Modules/FetchContent/
+-rw-r--r--   0 kangwei   (1092) root         (0)      831 2023-02-18 07:20:27.000000 fasttextsearch-0.5/cmake/Modules/FetchContent/CMakeLists.cmake.in
+-rw-r--r--   0 kangwei   (1092) root         (0)    38023 2023-02-18 07:20:27.000000 fasttextsearch-0.5/cmake/Modules/FetchContent.cmake
+-rw-r--r--   0 kangwei   (1092) root         (0)      135 2023-02-18 07:20:27.000000 fasttextsearch-0.5/cmake/Modules/README.md
+-rw-r--r--   0 kangwei   (1092) root         (0)        0 2023-02-18 07:20:27.000000 fasttextsearch-0.5/cmake/__init__.py
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.134072 fasttextsearch-0.5/cmake/__pycache__/
+-rw-r--r--   0 kangwei   (1092) root         (0)      142 2023-05-16 11:29:34.000000 fasttextsearch-0.5/cmake/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)     3421 2023-03-31 03:33:51.000000 fasttextsearch-0.5/cmake/googletest.cmake
+-rw-r--r--   0 kangwei   (1092) root         (0)     1800 2023-03-31 03:33:51.000000 fasttextsearch-0.5/cmake/pybind11.cmake
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.139072 fasttextsearch-0.5/fasttextsearch.egg-info/
+-rw-r--r--   0 kangwei   (1092) root         (0)     1169 2023-06-24 07:37:05.000000 fasttextsearch-0.5/fasttextsearch.egg-info/PKG-INFO
+-rw-r--r--   0 kangwei   (1092) root         (0)     2399 2023-06-24 07:37:05.000000 fasttextsearch-0.5/fasttextsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)        1 2023-06-24 07:37:05.000000 fasttextsearch-0.5/fasttextsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)        6 2023-06-24 07:37:05.000000 fasttextsearch-0.5/fasttextsearch.egg-info/requires.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)       24 2023-06-24 07:37:05.000000 fasttextsearch-0.5/fasttextsearch.egg-info/top_level.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)      769 2023-06-24 07:05:13.000000 fasttextsearch-0.5/pyproject.toml
+-rw-r--r--   0 kangwei   (1092) root         (0)        6 2023-05-16 07:33:05.000000 fasttextsearch-0.5/requirements.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)       38 2023-06-24 07:37:05.170072 fasttextsearch-0.5/setup.cfg
+-rw-r--r--   0 kangwei   (1092) root         (0)     2986 2023-06-24 07:05:13.000000 fasttextsearch-0.5/setup.py
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.139072 fasttextsearch-0.5/textsearch/
+-rw-r--r--   0 kangwei   (1092) root         (0)       48 2023-02-18 12:05:47.000000 fasttextsearch-0.5/textsearch/CMakeLists.txt
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.147072 fasttextsearch-0.5/textsearch/csrc/
+-rw-r--r--   0 kangwei   (1092) root         (0)      695 2023-06-24 07:05:13.000000 fasttextsearch-0.5/textsearch/csrc/CMakeLists.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)    13272 2023-05-23 10:09:31.000000 fasttextsearch-0.5/textsearch/csrc/levenshtein.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     4137 2023-05-04 04:46:37.000000 fasttextsearch-0.5/textsearch/csrc/levenshtein_test.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     4694 2023-06-24 07:06:12.000000 fasttextsearch-0.5/textsearch/csrc/match.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     4611 2023-05-04 04:46:37.000000 fasttextsearch-0.5/textsearch/csrc/match.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     3248 2023-05-04 04:46:37.000000 fasttextsearch-0.5/textsearch/csrc/match_test.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     5273 2023-04-12 07:57:56.000000 fasttextsearch-0.5/textsearch/csrc/suffix_array.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     3207 2023-03-31 03:33:51.000000 fasttextsearch-0.5/textsearch/csrc/suffix_array.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     3883 2023-04-24 11:25:03.000000 fasttextsearch-0.5/textsearch/csrc/suffix_array_test.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     2880 2023-04-24 11:25:03.000000 fasttextsearch-0.5/textsearch/csrc/utils.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)     3508 2023-04-24 11:25:03.000000 fasttextsearch-0.5/textsearch/csrc/utils.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     4862 2023-04-24 11:25:03.000000 fasttextsearch-0.5/textsearch/csrc/utils_test.cc
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.147072 fasttextsearch-0.5/textsearch/python/
+-rw-r--r--   0 kangwei   (1092) root         (0)       78 2023-06-24 07:05:13.000000 fasttextsearch-0.5/textsearch/python/CMakeLists.txt
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.154072 fasttextsearch-0.5/textsearch/python/csrc/
+-rw-r--r--   0 kangwei   (1092) root         (0)      169 2023-06-24 07:05:13.000000 fasttextsearch-0.5/textsearch/python/csrc/CMakeLists.txt
+-rw-r--r--   0 kangwei   (1092) root         (0)     5003 2023-06-24 07:06:12.000000 fasttextsearch-0.5/textsearch/python/csrc/levenshtein.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)      985 2023-03-06 09:09:29.000000 fasttextsearch-0.5/textsearch/python/csrc/levenshtein.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     1850 2023-05-04 04:46:37.000000 fasttextsearch-0.5/textsearch/python/csrc/match.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)      961 2023-05-04 04:46:37.000000 fasttextsearch-0.5/textsearch/python/csrc/match.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     1637 2023-04-13 03:32:42.000000 fasttextsearch-0.5/textsearch/python/csrc/suffix_array.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)      988 2023-03-06 09:09:29.000000 fasttextsearch-0.5/textsearch/python/csrc/suffix_array.h
+-rw-r--r--   0 kangwei   (1092) root         (0)      564 2023-06-24 07:05:13.000000 fasttextsearch-0.5/textsearch/python/csrc/text_search.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)      357 2023-03-31 03:33:51.000000 fasttextsearch-0.5/textsearch/python/csrc/text_search.h
+-rw-r--r--   0 kangwei   (1092) root         (0)     4599 2023-04-24 11:25:03.000000 fasttextsearch-0.5/textsearch/python/csrc/utils.cc
+-rw-r--r--   0 kangwei   (1092) root         (0)      318 2023-04-21 06:51:44.000000 fasttextsearch-0.5/textsearch/python/csrc/utils.h
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.160072 fasttextsearch-0.5/textsearch/python/tests/
+-rw-r--r--   0 kangwei   (1092) root         (0)      848 2023-06-24 07:05:13.000000 fasttextsearch-0.5/textsearch/python/tests/CMakeLists.txt
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     4748 2023-04-24 11:25:03.000000 fasttextsearch-0.5/textsearch/python/tests/test_find_close_matches.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     1943 2023-04-13 03:32:42.000000 fasttextsearch-0.5/textsearch/python/tests/test_levenshtein_distance.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     1414 2023-05-04 04:46:37.000000 fasttextsearch-0.5/textsearch/python/tests/test_match.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)      950 2023-03-31 03:33:51.000000 fasttextsearch-0.5/textsearch/python/tests/test_row_ids_to_row_splits.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)    10687 2023-04-13 03:32:42.000000 fasttextsearch-0.5/textsearch/python/tests/test_sourced_text.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     1359 2023-04-24 11:25:03.000000 fasttextsearch-0.5/textsearch/python/tests/test_suffix_array.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     2007 2023-03-31 03:33:51.000000 fasttextsearch-0.5/textsearch/python/tests/test_text_source.py
+-rwxr-xr-x   0 kangwei   (1092) root         (0)     2314 2023-03-31 03:33:51.000000 fasttextsearch-0.5/textsearch/python/tests/test_transcript.py
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.164072 fasttextsearch-0.5/textsearch/python/textsearch/
+-rw-r--r--   0 kangwei   (1092) root         (0)      751 2023-06-24 07:37:05.000000 fasttextsearch-0.5/textsearch/python/textsearch/__init__.py
+drwxr-xr-x   0 kangwei   (1092) root         (0)        0 2023-06-24 07:37:05.169072 fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/
+-rw-r--r--   0 kangwei   (1092) root         (0)      948 2023-05-18 08:42:24.000000 fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)     8961 2023-05-05 09:46:59.000000 fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/datatypes.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)     2543 2023-05-05 09:46:59.000000 fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/levenshtein.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)    23181 2023-05-24 04:44:55.000000 fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/match.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)     5139 2023-05-18 08:42:24.000000 fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/suffix_array.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)     2910 2023-04-13 07:06:10.000000 fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/text_search.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)     3328 2023-05-18 08:42:24.000000 fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 kangwei   (1092) root         (0)    12992 2023-04-24 11:25:03.000000 fasttextsearch-0.5/textsearch/python/textsearch/datatypes.py
+-rw-r--r--   0 kangwei   (1092) root         (0)     3594 2023-04-24 11:25:03.000000 fasttextsearch-0.5/textsearch/python/textsearch/levenshtein.py
+-rw-r--r--   0 kangwei   (1092) root         (0)    40868 2023-06-24 07:06:12.000000 fasttextsearch-0.5/textsearch/python/textsearch/match.py
+-rw-r--r--   0 kangwei   (1092) root         (0)     6695 2023-06-24 07:05:13.000000 fasttextsearch-0.5/textsearch/python/textsearch/suffix_array.py
+-rw-r--r--   0 kangwei   (1092) root         (0)     3165 2023-06-24 07:05:13.000000 fasttextsearch-0.5/textsearch/python/textsearch/utils.py
```

### Comparing `fasttextsearch-0.4/CMakeLists.txt` & `fasttextsearch-0.5/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cmake_minimum_required(VERSION 3.8 FATAL_ERROR)
 project(textsearch)
 
-set(TS_VERSION "0.1")
+set(TS_VERSION "0.5")
 
 set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
 set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")
 
 set(CMAKE_SKIP_BUILD_RPATH FALSE)
 set(BUILD_RPATH_USE_ORIGIN TRUE)
```

### Comparing `fasttextsearch-0.4/README.md` & `fasttextsearch-0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Installation
 
-This section describes how to compile and use this project.
+## With pip
 
-(For developers only)
+```
+pip install fasttextsearch
+```
+
+## For developers
 
 ```bash
 pip install numpy
 
 git clone https://github.com/danpovey/text_search
 cd text_search
```

### Comparing `fasttextsearch-0.4/cmake/Modules/FetchContent/CMakeLists.cmake.in` & `fasttextsearch-0.5/cmake/Modules/FetchContent/CMakeLists.cmake.in`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/cmake/Modules/FetchContent.cmake` & `fasttextsearch-0.5/cmake/Modules/FetchContent.cmake`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/cmake/googletest.cmake` & `fasttextsearch-0.5/cmake/googletest.cmake`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/cmake/pybind11.cmake` & `fasttextsearch-0.5/cmake/pybind11.cmake`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/fasttextsearch.egg-info/SOURCES.txt` & `fasttextsearch-0.5/fasttextsearch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.py
 cmake/__init__.py
 cmake/googletest.cmake
 cmake/pybind11.cmake
 cmake/Modules/FetchContent.cmake
 cmake/Modules/README.md
 cmake/Modules/FetchContent/CMakeLists.cmake.in
+cmake/__pycache__/__init__.cpython-38.pyc
 fasttextsearch.egg-info/PKG-INFO
 fasttextsearch.egg-info/SOURCES.txt
 fasttextsearch.egg-info/dependency_links.txt
 fasttextsearch.egg-info/requires.txt
 fasttextsearch.egg-info/top_level.txt
 textsearch/CMakeLists.txt
 textsearch/csrc/CMakeLists.txt
```

### Comparing `fasttextsearch-0.4/pyproject.toml` & `fasttextsearch-0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "cmake>=3.8",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "fasttextsearch"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="Next-gen Kaldi development team", email="wkang.pku@gmail.com" },
 ]
 description="Some fast-ish algorithms for batch text search in moderate-sized collections, intended for data cleanup."
 dependencies = [
   "numpy",
 ]
```

### Comparing `fasttextsearch-0.4/setup.py` & `fasttextsearch-0.5/setup.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/csrc/CMakeLists.txt` & `fasttextsearch-0.5/textsearch/csrc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/csrc/levenshtein.h` & `fasttextsearch-0.5/textsearch/csrc/levenshtein.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/csrc/levenshtein_test.cc` & `fasttextsearch-0.5/textsearch/csrc/levenshtein_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/csrc/match.cc` & `fasttextsearch-0.5/textsearch/csrc/match.cc`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 namespace fasttextsearch {
 
 void GetLongestIncreasingPairs(
     const int32_t *seq1, const int32_t *seq2, int32_t size,
     std::vector<std::pair<int32_t, int32_t>> *best_trace) {
 
+  if (size == 0)
+    return;
+
   assert(size > 0);
   // sort this by i, then j.  prev_n values can be undefined for now.
   std::vector<internal::GoodMatch> sorted_pairs(size);
   for (int32_t i = 0; i < size; ++i) {
     sorted_pairs[i] = internal::GoodMatch(seq1[i], seq2[i]);
   }
   std::sort(sorted_pairs.begin(), sorted_pairs.end());
```

### Comparing `fasttextsearch-0.4/textsearch/csrc/match.h` & `fasttextsearch-0.5/textsearch/csrc/match.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/csrc/match_test.cc` & `fasttextsearch-0.5/textsearch/csrc/match_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/csrc/suffix_array.cc` & `fasttextsearch-0.5/textsearch/csrc/suffix_array.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/csrc/suffix_array.h` & `fasttextsearch-0.5/textsearch/csrc/suffix_array.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/csrc/suffix_array_test.cc` & `fasttextsearch-0.5/textsearch/csrc/suffix_array_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/csrc/utils.cc` & `fasttextsearch-0.5/textsearch/csrc/utils.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/csrc/utils.h` & `fasttextsearch-0.5/textsearch/csrc/utils.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/csrc/utils_test.cc` & `fasttextsearch-0.5/textsearch/csrc/utils_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/csrc/levenshtein.cc` & `fasttextsearch-0.5/textsearch/python/csrc/levenshtein.cc`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     The cost of deletion error, default 1.
   replace_cost:
     The cost of replacement error, default 1.
 
 Returns:
   Return a tuple which has two elements, the first element is the levenshtein
   distance, the second element is a list of tuple, each tuple in the list has
-  `start` and `end` (index into the target sequence) and `alignment`
+  `start` and `end` (index into the target sequence, for "global" mode, `start`
+  is always 0, `end` is always `len(target) - 1`) and `alignment`.
   See the examples below for more details.
 
 >>> from textsearch import levenshtein_distance
 >>> import numpy as np
 >>> query = np.array([1, 2, 3, 4], dtype=np.int32)
 >>> target = np.array([1, 5, 3, 4, 6, 7, 1, 2, 4], dtype=np.int32)
 >>> distance, alignments = levenshtein_distance(query, target)
```

### Comparing `fasttextsearch-0.4/textsearch/python/csrc/levenshtein.h` & `fasttextsearch-0.5/textsearch/python/csrc/levenshtein.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/csrc/match.cc` & `fasttextsearch-0.5/textsearch/python/csrc/match.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/csrc/match.h` & `fasttextsearch-0.5/textsearch/python/csrc/match.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/csrc/suffix_array.cc` & `fasttextsearch-0.5/textsearch/python/csrc/suffix_array.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/csrc/suffix_array.h` & `fasttextsearch-0.5/textsearch/python/csrc/suffix_array.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/csrc/text_search.cc` & `fasttextsearch-0.5/textsearch/python/csrc/text_search.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/csrc/utils.cc` & `fasttextsearch-0.5/textsearch/python/csrc/utils.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/tests/CMakeLists.txt` & `fasttextsearch-0.5/textsearch/python/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/tests/test_find_close_matches.py` & `fasttextsearch-0.5/textsearch/python/tests/test_find_close_matches.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/tests/test_levenshtein_distance.py` & `fasttextsearch-0.5/textsearch/python/tests/test_levenshtein_distance.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/tests/test_match.py` & `fasttextsearch-0.5/textsearch/python/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/tests/test_row_ids_to_row_splits.py` & `fasttextsearch-0.5/textsearch/python/tests/test_row_ids_to_row_splits.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/tests/test_sourced_text.py` & `fasttextsearch-0.5/textsearch/python/tests/test_sourced_text.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/tests/test_suffix_array.py` & `fasttextsearch-0.5/textsearch/python/tests/test_suffix_array.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/tests/test_text_source.py` & `fasttextsearch-0.5/textsearch/python/tests/test_text_source.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/tests/test_transcript.py` & `fasttextsearch-0.5/textsearch/python/tests/test_transcript.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/datatypes.cpython-38.pyc` & `fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/datatypes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/levenshtein.cpython-38.pyc` & `fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/levenshtein.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/match.cpython-38.pyc` & `fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/match.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue May 16 07:26:01 2023 UTC, .py size: 39883 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,1436 +1,1449 @@
-00000000: 550d 0d0a 0000 0000 0930 6364 cb9b 0000  U........0cd....
+00000000: 550d 0d0a 0000 0000 2896 6d64 5b9f 0000  U.......(.md[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000d 0000 0040 0000 0073 fa01 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6400  d.l.m.Z.m.Z...d.
-00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
-00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
-00000080: 6d0f 5a0f 6d10 5a10 0100 6400 6401 6c11  m.Z.m.Z...d.d.l.
-00000090: 5a12 6400 6407 6c13 6d14 5a15 6d16 5a16  Z.d.d.l.m.Z.m.Z.
-000000a0: 0100 6408 6409 6c17 6d18 5a18 0100 6408  ..d.d.l.m.Z...d.
-000000b0: 640a 6c19 6d1a 5a1a 6d1b 5a1b 6d1c 5a1c  d.l.m.Z.m.Z.m.Z.
-000000c0: 0100 6408 640b 6c1d 6d1e 5a1e 6d1f 5a1f  ..d.d.l.m.Z.m.Z.
-000000d0: 6d20 5a20 0100 6512 6a21 6512 6a21 650d  m Z ..e.j!e.j!e.
-000000e0: 650f 6522 6522 6602 1900 1900 640c 9c03  e.e"e"f.....d...
-000000f0: 640d 640e 8404 5a14 6424 651a 650d 650f  d.d...Z.d$e.e.e.
-00000100: 6522 6522 6602 1900 1900 6522 6523 650d  e"e"f.....e"e#e.
-00000110: 650f 6522 6522 6522 6522 6604 1900 1900  e.e"e"e"e"f.....
-00000120: 6411 9c05 6412 6413 8405 5a24 651a 650d  d...d.d...Z$e.e.
-00000130: 650c 6525 650b 6602 1900 1900 6522 650d  e.e%e.f.....e"e.
-00000140: 650f 650f 6522 6522 6602 1900 650d 650c  e.e.e"e"f...e.e.
-00000150: 6525 650b 6602 1900 1900 6602 1900 1900  e%e.f.....f.....
-00000160: 6414 9c04 6415 6416 8404 5a26 6425 651a  d...d.d...Z&d%e.
-00000170: 6512 6a21 6522 6523 650e 6509 1900 650d  e.j!e"e#e.e...e.
-00000180: 650f 650f 6522 6522 6602 1900 650d 650c  e.e.e"e"f...e.e.
-00000190: 6525 650b 6602 1900 1900 6602 1900 1900  e%e.f.....f.....
-000001a0: 6417 9c06 6418 6419 8405 5a27 651b 650d  d...d.d...Z'e.e.
-000001b0: 650f 6522 6522 6523 6603 1900 1900 641a  e.e"e"e#f.....d.
-000001c0: 9c02 641b 641c 8404 5a28 6510 651c 651b  ..d.d...Z(e.e.e.
-000001d0: 6602 1900 651b 650d 650c 6525 6510 6525  f...e.e.e.e%e.e%
-000001e0: 6522 6523 6603 1900 6602 1900 1900 641d  e"e#f...f.....d.
-000001f0: 9c03 641e 641f 8404 5a29 6426 6512 6a21  ..d.d...Z)d&e.j!
-00000200: 651a 6523 6522 650d 650d 650f 6522 6522  e.e#e"e.e.e.e"e"
-00000210: 6602 1900 1900 1900 6421 9c05 6422 6423  f.......d!..d"d#
-00000220: 8405 5a2a 6401 5300 2927 e900 0000 004e  ..Z*d.S.)'.....N
-00000230: 2901 da0b 6269 7365 6374 5f6c 6566 7429  )...bisect_left)
-00000240: 01da 0964 6174 6163 6c61 7373 2902 da08  ...dataclass)...
-00000250: 6865 6170 7075 7368 da07 6865 6170 706f  heappush..heappo
-00000260: 7029 01da 0a54 6872 6561 6450 6f6f 6c29  p)...ThreadPool)
-00000270: 06da 0341 6e79 da04 4469 6374 da04 4c69  ...Any..Dict..Li
-00000280: 7374 da08 4f70 7469 6f6e 616c da05 5475  st..Optional..Tu
-00000290: 706c 65da 0555 6e69 6f6e 2902 da1c 6765  ple..Union)...ge
-000002a0: 745f 6c6f 6e67 6573 745f 696e 6372 6561  t_longest_increa
-000002b0: 7369 6e67 5f70 6169 7273 da14 6c65 7665  sing_pairs..leve
-000002c0: 6e73 6874 6569 6e5f 6469 7374 616e 6365  nshtein_distance
-000002d0: e901 0000 0029 01da 1363 7265 6174 655f  .....)...create_
-000002e0: 7375 6666 6978 5f61 7272 6179 2903 da0b  suffix_array)...
-000002f0: 536f 7572 6365 6454 6578 74da 0a54 6578  SourcedText..Tex
-00000300: 7453 6f75 7263 65da 0a54 7261 6e73 6372  tSource..Transcr
-00000310: 6970 7429 03da 0a69 735f 6f76 6572 6c61  ipt)...is_overla
-00000320: 70da 0e69 735f 7075 6e63 7475 6174 696f  p..is_punctuatio
-00000330: 6eda 1572 6f77 5f69 6473 5f74 6f5f 726f  n..row_ids_to_ro
-00000340: 775f 7370 6c69 7473 2903 da04 7365 7131  w_splits)...seq1
-00000350: da04 7365 7132 da06 7265 7475 726e 6302  ..seq2..returnc.
-00000360: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-00000370: 0000 0043 0000 0073 6e00 0000 7c00 6a00  ...C...sn...|.j.
-00000380: 6401 6b02 7314 7401 7c00 6a00 8301 8201  d.k.s.t.|.j.....
-00000390: 7c01 6a00 6401 6b02 7328 7401 7c01 6a00  |.j.d.k.s(t.|.j.
-000003a0: 8301 8201 7c00 6a02 7c01 6a02 6b02 7344  ....|.j.|.j.k.sD
-000003b0: 7401 7c00 6a02 7c01 6a02 6602 8301 8201  t.|.j.|.j.f.....
-000003c0: 7403 6a04 7c00 7403 6a05 6402 8d02 7d02  t.j.|.t.j.d...}.
-000003d0: 7403 6a04 7c01 7403 6a05 6402 8d02 7d03  t.j.|.t.j.d...}.
-000003e0: 7406 7c02 7c03 8302 5300 2903 6117 0300  t.|.|...S.).a...
-000003f0: 000a 2020 2020 4765 7420 7468 6520 6c6f  ..    Get the lo
-00000400: 6e67 6573 7420 696e 6372 6561 7369 6e67  ngest increasing
-00000410: 2070 6169 7273 2066 6f72 2067 6976 656e   pairs for given
-00000420: 2073 6571 7565 6e63 6573 2e0a 2020 2020   sequences..    
-00000430: 5365 6520 6874 7470 733a 2f2f 6769 7468  See https://gith
-00000440: 7562 2e63 6f6d 2f64 616e 706f 7665 792f  ub.com/danpovey/
-00000450: 7465 7874 5f73 6561 7263 682f 6973 7375  text_search/issu
-00000460: 6573 2f32 3120 666f 7220 6d6f 7265 2064  es/21 for more d
-00000470: 6574 6169 6c73 2e0a 0a20 2020 2053 7570  etails...    Sup
-00000480: 706f 7365 2073 6571 3120 6973 205b 6931  pose seq1 is [i1
-00000490: 2c20 6932 2c20 6933 2e2e 2e20 694e 5d20  , i2, i3... iN] 
-000004a0: 616e 6420 7365 7132 2069 7320 5b6a 312c  and seq2 is [j1,
-000004b0: 206a 322c 206a 332e 2e2e 206a 4e5d 2c20   j2, j3... jN], 
-000004c0: 7468 6973 0a20 2020 2066 756e 6374 696f  this.    functio
-000004d0: 6e20 7265 7475 726e 7320 7468 6520 206c  n returns the  l
-000004e0: 6f6e 6765 7374 2069 6e63 7265 6173 696e  ongest increasin
-000004f0: 6720 7061 6972 733a 2028 6931 2c20 6a31  g pairs: (i1, j1
-00000500: 292c 2028 6932 2c20 6a32 292c 202e 2e2e  ), (i2, j2), ...
-00000510: 2028 694e 2c20 6a4e 290a 2020 2020 7375   (iN, jN).    su
-00000520: 6368 2074 6861 7420 6931 203c 3d20 6932  ch that i1 <= i2
-00000530: 203c 3d20 2e2e 2e20 3c3d 2069 4e2c 2061   <= ... <= iN, a
-00000540: 6e64 206a 3120 3c3d 206a 3220 3c3d 202e  nd j1 <= j2 <= .
-00000550: 2e2e 203c 3d20 6a4e 2e0a 0a20 2020 2041  .. <= jN...    A
-00000560: 7267 733a 0a20 2020 2020 2073 6571 313a  rgs:.      seq1:
-00000570: 0a20 2020 2020 2020 2054 6865 2066 6972  .        The fir
-00000580: 7374 2073 6571 7565 6e63 652e 0a20 2020  st sequence..   
-00000590: 2020 2073 6571 323a 0a20 2020 2020 2020     seq2:.       
-000005a0: 2054 6865 2073 6563 6f6e 6420 7365 7175   The second sequ
-000005b0: 656e 6365 2e0a 0a20 2020 203e 3e3e 2069  ence...    >>> i
-000005c0: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
-000005d0: 700a 2020 2020 3e3e 3e20 6672 6f6d 2074  p.    >>> from t
-000005e0: 6578 7473 6561 7263 6820 696d 706f 7274  extsearch import
-000005f0: 2067 6574 5f6c 6f6e 6765 7374 5f69 6e63   get_longest_inc
-00000600: 7265 6173 696e 675f 7061 6972 730a 2020  reasing_pairs.  
-00000610: 2020 3e3e 3e20 7365 7131 203d 206e 702e    >>> seq1 = np.
-00000620: 6172 7261 7928 5b30 2c20 312c 2031 2c20  array([0, 1, 1, 
-00000630: 322c 2032 2c20 332c 2034 2c20 352c 2036  2, 2, 3, 4, 5, 6
-00000640: 5d2c 2064 7479 7065 3d6e 702e 696e 7433  ], dtype=np.int3
-00000650: 3229 0a20 2020 203e 3e3e 2073 6571 3220  2).    >>> seq2 
-00000660: 3d20 6e70 2e61 7272 6179 285b 392c 2037  = np.array([9, 7
-00000670: 2c20 382c 2039 2c20 362c 2037 2c20 3130  , 8, 9, 6, 7, 10
-00000680: 2c20 3132 2c20 385d 2c20 6474 7970 653d  , 12, 8], dtype=
-00000690: 6e70 2e69 6e74 3634 290a 2020 2020 3e3e  np.int64).    >>
-000006a0: 3e20 6765 745f 6c6f 6e67 6573 745f 696e  > get_longest_in
-000006b0: 6372 6561 7369 6e67 5f70 6169 7273 2873  creasing_pairs(s
-000006c0: 6571 313d 7365 7131 2c20 7365 7132 3d73  eq1=seq1, seq2=s
-000006d0: 6571 3229 0a20 2020 205b 2831 2c20 3729  eq2).    [(1, 7)
-000006e0: 2c20 2831 2c20 3829 2c20 2832 2c20 3929  , (1, 8), (2, 9)
-000006f0: 2c20 2834 2c20 3130 292c 2028 352c 2031  , (4, 10), (5, 1
-00000700: 3229 5d0a 2020 2020 720f 0000 0029 01da  2)].    r....)..
-00000710: 0564 7479 7065 2907 da04 6e64 696d da0e  .dtype)...ndim..
-00000720: 4173 7365 7274 696f 6e45 7272 6f72 da04  AssertionError..
-00000730: 7369 7a65 da02 6e70 da11 6173 636f 6e74  size..np..ascont
-00000740: 6967 756f 7573 6172 7261 79da 0569 6e74  iguousarray..int
-00000750: 3332 da1d 5f67 6574 5f6c 6f6e 6765 7374  32.._get_longest
-00000760: 5f69 6e63 7265 6173 696e 675f 7061 6972  _increasing_pair
-00000770: 7329 0472 1700 0000 7218 0000 005a 0a73  s).r....r....Z.s
-00000780: 6571 315f 696e 7433 325a 0a73 6571 325f  eq1_int32Z.seq2_
-00000790: 696e 7433 32a9 0072 2200 0000 fa48 2f63  int32..r"....H/c
-000007a0: 6570 682d 6877 2f6b 616e 6777 6569 2f63  eph-hw/kangwei/c
-000007b0: 6f64 6532 2f74 6578 745f 7365 6172 6368  ode2/text_search
-000007c0: 2f74 6578 7473 6561 7263 682f 7079 7468  /textsearch/pyth
-000007d0: 6f6e 2f74 6578 7473 6561 7263 682f 6d61  on/textsearch/ma
-000007e0: 7463 682e 7079 720d 0000 0023 0000 0073  tch.pyr....#...s
-000007f0: 0c00 0000 0018 1401 1401 1c03 1001 1002  ................
-00000800: 720d 0000 00e9 8813 0000 e79a 9999 9999  r...............
-00000810: 99b9 3f29 05da 0c73 6f75 7263 6564 5f74  ..?)...sourced_t
-00000820: 6578 74da 0e6d 6174 6368 6564 5f70 6f69  ext..matched_poi
-00000830: 6e74 73da 0e73 6567 6d65 6e74 5f6c 656e  nts..segment_len
-00000840: 6774 68da 1b72 6566 6572 656e 6365 5f6c  gth..reference_l
-00000850: 656e 6774 685f 6469 6666 6572 656e 6365  ength_difference
-00000860: 7219 0000 0063 0400 0000 0000 0000 0000  r....c..........
-00000870: 0000 1c00 0000 0800 0000 4300 0000 7328  ..........C...s(
-00000880: 0300 0064 017d 0467 007d 0574 0064 0274  ...d.}.g.}.t.d.t
-00000890: 017c 0183 0183 0244 005d b67d 067c 017c  .|.....D.].}.|.|
-000008a0: 0619 0064 0119 007c 017c 0664 0218 0019  ...d...|.|.d....
-000008b0: 0064 0119 0018 007c 017c 0619 0064 0219  .d.....|.|...d..
-000008c0: 007c 017c 0664 0218 0019 0064 0219 0018  .|.|.d.....d....
-000008d0: 0066 027d 077c 0764 0119 007c 0764 0219  .f.}.|.d...|.d..
-000008e0: 006b 0072 167c 017c 0619 0064 0219 007c  .k.r.|.|...d...|
-000008f0: 017c 0419 0064 0219 0018 0064 0217 007c  .|...d.....d...|
-00000900: 017c 0619 0064 0119 007c 017c 0419 0064  .|...d...|.|...d
-00000910: 0119 0018 0064 0217 001b 007d 087c 0364  .....d.....}.|.d
-00000920: 031b 007d 097c 0864 027c 0918 006b 0073  ...}.|.d.|...k.s
-00000930: ba7c 0864 027c 0917 006b 0472 167c 05a0  .|.d.|...k.r.|..
-00000940: 027c 047c 0666 02a1 0101 007c 067d 0471  .|.|.f.....|.}.q
-00000950: 167c 05a0 027c 0474 017c 0183 0166 02a1  .|...|.t.|...f..
-00000960: 0101 0064 047d 0a64 0174 017c 0183 0166  ...d.}.d.t.|...f
-00000970: 027d 0b7c 0544 005d 387d 0c7c 017c 0c64  .}.|.D.]8}.|.|.d
-00000980: 0219 0064 0218 0019 0064 0119 007c 017c  ...d.....d...|.|
-00000990: 0c64 0119 0019 0064 0119 0018 007d 0d7c  .d.....d.....}.|
-000009a0: 0d7c 0a6b 0472 f47c 0d7d 0a7c 0c7d 0b71  .|.k.r.|.}.|.}.q
-000009b0: f467 007d 0e64 0564 0684 007d 0f7c 006a  .g.}.d.d...}.|.j
-000009c0: 037c 017c 0b64 0119 0019 0064 0219 0019  .|.|.d.....d....
-000009d0: 007d 107c 006a 047c 1019 007d 117c 006a  .}.|.j.|...}.|.j
-000009e0: 047c 1064 0217 0019 007d 127c 006a 037c  .|.d.....}.|.j.|
-000009f0: 017c 0b64 0119 0019 0064 0119 0019 007d  .|.d.....d.....}
-00000a00: 137c 006a 047c 1319 007d 147c 006a 047c  .|.j.|...}.|.j.|
-00000a10: 1364 0217 0019 007d 157c 017c 0b64 0119  .d.....}.|.|.d..
-00000a20: 0019 0064 0219 007c 017c 0b64 0119 0019  ...d...|.|.d....
-00000a30: 0064 0119 007c 1418 0018 007d 167c 147c  .d...|.....}.|.|
-00000a40: 167c 116b 0590 0172 ca7c 166e 027c 1166  .|.k...r.|.n.|.f
-00000a50: 027d 0474 007c 0b64 0119 007c 0b64 0219  .}.t.|.d...|.d..
-00000a60: 0083 0244 005d b67d 177c 017c 1719 0064  ...D.].}.|.|...d
-00000a70: 0119 007c 0464 0119 0018 007c 026b 0490  ...|.d.....|.k..
-00000a80: 0172 e27c 177c 0b64 0119 006b 0290 0272  .r.|.|.d...k...r
-00000a90: 1490 0171 e26e 827c 0464 0119 007d 187c  ...q.n.|.d...}.|
-00000aa0: 017c 1764 0218 0019 0064 0119 007d 197c  .|.d.....d...}.|
-00000ab0: 0464 0219 007d 1a7c 017c 1764 0218 0019  .d...}.|.|.d....
-00000ac0: 0064 0219 007d 1b7c 1b7c 1a18 007c 197c  .d...}.|.|...|.|
-00000ad0: 1818 001b 007d 087c 0364 031b 007d 097c  .....}.|.d...}.|
-00000ae0: 0864 027c 0918 006b 0090 0173 e27c 0864  .d.|...k...s.|.d
-00000af0: 027c 0917 006b 0490 0272 7c90 0171 e27c  .|...k...r|..q.|
-00000b00: 197c 1b66 027d 047c 0f7c 187c 197c 1a7c  .|.f.}.|.|.|.|.|
-00000b10: 1b7c 027c 0e83 0601 0090 0171 e27c 045c  .|.|.......q.|.\
-00000b20: 027d 187d 1a7c 157d 197c 1a7c 197c 1818  .}.}.|.}.|.|.|..
-00000b30: 0017 007d 1b7c 1b7c 126b 0190 0272 c07c  ...}.|.|.k...r.|
-00000b40: 1b6e 027c 127d 1b7c 197c 1818 007c 0264  .n.|.}.|.|...|.d
-00000b50: 071a 006b 0090 0372 127c 0e90 0272 fe7c  ...k...r.|...r.|
-00000b60: 0e64 0419 0064 0119 007c 197c 0e64 0419  .d...d...|.|.d..
-00000b70: 0064 0319 007c 1b66 047c 0e64 043c 006e  .d...|.f.|.d.<.n
-00000b80: 127c 0ea0 027c 187c 197c 1a7c 1b66 04a1  .|...|.|.|.|.f..
-00000b90: 0101 006e 127c 0f7c 187c 197c 1a7c 1b7c  ...n.|.|.|.|.|.|
-00000ba0: 027c 0e83 0601 007c 0e53 0029 0861 8b03  .|.....|.S.).a..
-00000bb0: 0000 0a20 2020 2042 7265 616b 206c 6f6e  ...    Break lon
-00000bc0: 6720 7175 6572 7920 696e 746f 2073 6d61  g query into sma
-00000bd0: 6c6c 2073 6567 6d65 6e74 7320 6174 2074  ll segments at t
-00000be0: 6865 206d 6174 6368 6564 2070 6f69 6e74  he matched point
-00000bf0: 7320 7769 7468 2074 6865 2060 7365 676d  s with the `segm
-00000c00: 656e 745f 6c65 6e67 7468 600a 2020 2020  ent_length`.    
-00000c10: 636f 6e73 7472 6169 6e74 2e0a 0a20 2020  constraint...   
-00000c20: 2041 7267 733a 0a20 2020 2020 2073 6f75   Args:.      sou
-00000c30: 7263 6564 5f74 6578 743a 0a20 2020 2020  rced_text:.     
-00000c40: 2020 2054 6865 2053 6f75 7263 6564 5465     The SourcedTe
-00000c50: 7874 2063 6f6e 7461 696e 696e 6720 7468  xt containing th
-00000c60: 6520 7175 6572 6965 7320 616e 6420 7265  e queries and re
-00000c70: 6665 7265 6e63 6573 2e0a 2020 2020 2020  ferences..      
-00000c80: 6d61 7463 6865 645f 706f 696e 7473 3a0a  matched_points:.
-00000c90: 2020 2020 2020 2020 4120 6c69 7374 206f          A list o
-00000ca0: 6620 6d61 7463 6865 6420 706f 696e 7473  f matched points
-00000cb0: 2c20 6561 6368 2069 7465 6d20 6973 2061  , each item is a
-00000cc0: 2070 6169 7220 6f66 2028 7175 6572 7920   pair of (query 
-00000cd0: 696e 6465 782c 2074 6172 6765 7420 696e  index, target in
-00000ce0: 6465 7829 0a20 2020 2020 2020 2069 6e20  dex).        in 
-00000cf0: 736f 7572 6365 645f 7465 7874 2e0a 2020  sourced_text..  
-00000d00: 2020 2020 7365 676d 656e 745f 6c65 6e67      segment_leng
-00000d10: 7468 3a0a 2020 2020 2020 2020 5468 6520  th:.        The 
-00000d20: 6578 7065 6374 6564 206c 656e 6774 6820  expected length 
-00000d30: 6f66 2074 6865 2073 6567 6d65 6e74 6564  of the segmented
-00000d40: 2070 6965 6365 2e20 4e6f 7465 3a20 7468   piece. Note: th
-00000d50: 6973 2069 7320 6e6f 7420 7265 616c 6c79  is is not really
-00000d60: 2074 6865 0a20 2020 2020 2020 206c 656e   the.        len
-00000d70: 6774 6820 6f66 2074 6865 2073 6567 6d65  gth of the segme
-00000d80: 6e74 732c 2074 6865 2073 6567 6d65 6e74  nts, the segment
-00000d90: 206c 656e 6774 6820 6d69 6768 7420 6265   length might be
-00000da0: 2061 206c 6974 746c 6520 6c6f 6e67 6572   a little longer
-00000db0: 0a20 2020 2020 2020 2074 6861 6e20 6073  .        than `s
-00000dc0: 6567 6d65 6e74 5f6c 656e 6774 6860 2c20  egment_length`, 
-00000dd0: 6c69 6b65 2060 7365 676d 656e 745f 6c65  like `segment_le
-00000de0: 6e67 7468 6020 2a20 312e 3235 0a20 2020  ngth` * 1.25.   
-00000df0: 2020 2072 6566 6572 656e 6365 5f6c 656e     reference_len
-00000e00: 6774 685f 6469 6666 6572 656e 6365 3a0a  gth_difference:.
-00000e10: 2020 2020 2020 2020 4265 6361 7573 6520          Because 
-00000e20: 6f66 2074 6865 2069 6e73 6572 7469 6f6e  of the insertion
-00000e30: 206f 7220 6465 6c65 7469 6f6e 2065 7272   or deletion err
-00000e40: 6f72 732c 2074 6865 2072 6566 6572 656e  ors, the referen
-00000e50: 6365 2073 6571 7565 6e63 6520 6d69 6768  ce sequence migh
-00000e60: 7420 6265 0a20 2020 2020 2020 2073 686f  t be.        sho
-00000e70: 7274 6572 206f 7220 6c6f 6e67 6572 2074  rter or longer t
-00000e80: 6861 6e20 7468 6520 7175 6572 792c 2073  han the query, s
-00000e90: 6f20 7468 6520 7265 6665 7265 6e63 6520  o the reference 
-00000ea0: 7365 676d 656e 7420 6c65 6e67 7468 2063  segment length c
-00000eb0: 616e 2062 6520 6672 6f6d 0a20 2020 2020  an be from.     
-00000ec0: 2020 2060 6c65 6e28 7175 6572 7929 202a     `len(query) *
-00000ed0: 2028 3120 2d20 7265 6665 7265 6e63 655f   (1 - reference_
-00000ee0: 6c65 6e67 7468 5f64 6966 6665 7265 6e63  length_differenc
-00000ef0: 6520 2f20 3229 6020 746f 0a20 2020 2020  e / 2)` to.     
-00000f00: 2020 2060 6c65 6e28 7175 6572 7929 202a     `len(query) *
-00000f10: 2028 3120 2b20 7265 6665 7265 6e63 655f   (1 + reference_
-00000f20: 6c65 6e67 7468 5f64 6966 6665 7265 6e63  length_differenc
-00000f30: 6520 2f20 3229 602e 0a20 2020 2072 0100  e / 2)`..    r..
-00000f40: 0000 720f 0000 00e9 0200 0000 e9ff ffff  ..r.............
-00000f50: ff63 0600 0000 0000 0000 0000 0000 0800  .c..............
-00000f60: 0000 0800 0000 5300 0000 7398 0000 007c  ......S...s....|
-00000f70: 017c 0018 007c 041a 007d 067c 0664 016b  .|...|...}.|.d.k
-00000f80: 0472 4c74 007c 0683 0144 005d 2e7d 077c  .rLt.|...D.].}.|
-00000f90: 05a0 017c 007c 007c 0417 007c 027c 027c  ...|.|.|...|.|.|
-00000fa0: 0417 0066 04a1 0101 007c 007c 0437 007d  ...f.....|.|.7.}
-00000fb0: 007c 027c 0437 007d 0271 1c7c 0572 827c  .|.|.7.}.q.|.r.|
-00000fc0: 017c 0018 007c 0464 021a 006b 0072 827c  .|...|.d...k.r.|
-00000fd0: 0564 0319 0064 0119 007c 017c 0564 0319  .d...d...|.|.d..
-00000fe0: 0064 0419 007c 0366 047c 0564 033c 006e  .d...|.f.|.d.<.n
-00000ff0: 127c 05a0 017c 007c 017c 027c 0366 04a1  .|...|.|.|.|.f..
-00001000: 0101 0064 0053 0029 054e 7201 0000 00e9  ...d.S.).Nr.....
-00001010: 0400 0000 722b 0000 0072 2a00 0000 2902  ....r+...r*...).
-00001020: da05 7261 6e67 65da 0661 7070 656e 6429  ..range..append)
-00001030: 08da 0b71 7565 7279 5f73 7461 7274 da09  ...query_start..
-00001040: 7175 6572 795f 656e 64da 0c74 6172 6765  query_end..targe
-00001050: 745f 7374 6172 74da 0a74 6172 6765 745f  t_start..target_
-00001060: 656e 6472 2800 0000 da08 7365 676d 656e  endr(.....segmen
-00001070: 7473 5a09 6e75 6d5f 6368 756e 6bda 0169  tsZ.num_chunk..i
-00001080: 7222 0000 0072 2200 0000 7223 0000 00da  r"...r"...r#....
-00001090: 0c61 6464 5f73 6567 6d65 6e74 7388 0000  .add_segments...
-000010a0: 0073 2600 0000 0003 0c01 0801 0c01 0402  .s&.............
-000010b0: 0201 0601 0201 06fc 02ff 0408 0801 0a03  ................
-000010c0: 1402 0a01 0201 0a01 02fc 0a07 7a22 5f62  ............z"_b
-000010d0: 7265 616b 5f71 7565 7279 2e3c 6c6f 6361  reak_query.<loca
-000010e0: 6c73 3e2e 6164 645f 7365 676d 656e 7473  ls>.add_segments
-000010f0: 722c 0000 0029 0572 2d00 0000 da03 6c65  r,...).r-.....le
-00001100: 6e72 2e00 0000 da03 646f 63da 0a64 6f63  nr......doc..doc
-00001110: 5f73 706c 6974 7329 1c72 2600 0000 7227  _splits).r&...r'
-00001120: 0000 0072 2800 0000 7229 0000 005a 1070  ...r(...r)...Z.p
-00001130: 7265 765f 6272 6561 6b5f 706f 696e 745a  rev_break_pointZ
-00001140: 1063 616e 6469 6461 7465 5f72 616e 6765  .candidate_range
-00001150: 7372 3400 0000 5a03 6761 70da 0572 6174  sr4...Z.gap..rat
-00001160: 696f da04 6861 6c66 da0a 6d61 785f 6c65  io..half..max_le
-00001170: 6e67 7468 5a08 6d61 785f 6974 656d da01  ngthZ.max_item..
-00001180: 635a 0e63 7572 7265 6e74 5f6c 656e 6774  cZ.current_lengt
-00001190: 6872 3300 0000 7235 0000 005a 0d74 6172  hr3...r5...Z.tar
-000011a0: 6765 745f 646f 635f 6964 5a0b 7461 7267  get_doc_idZ.targ
-000011b0: 6574 5f62 6173 655a 106e 6578 745f 7461  et_baseZ.next_ta
-000011c0: 7267 6574 5f62 6173 65da 0c71 7565 7279  rget_base..query
-000011d0: 5f64 6f63 5f69 64da 0a71 7565 7279 5f62  _doc_id..query_b
-000011e0: 6173 655a 0f6e 6578 745f 7175 6572 795f  aseZ.next_query_
-000011f0: 6261 7365 5a0b 7072 6576 5f74 6172 6765  baseZ.prev_targe
-00001200: 74da 0369 6e64 722f 0000 0072 3000 0000  t..indr/...r0...
-00001210: 7231 0000 0072 3200 0000 7222 0000 0072  r1...r2...r"...r
-00001220: 2200 0000 7223 0000 00da 0c5f 6272 6561  "...r#....._brea
-00001230: 6b5f 7175 6572 7946 0000 0073 a800 0000  k_queryF...s....
-00001240: 001d 0401 0401 1204 1a01 1afe 0404 1002  ................
-00001250: 1a01 1aff 0405 0801 1801 0e01 0602 1204  ................
-00001260: 0401 0c01 0801 2401 0801 0401 0604 0402  ......$.........
-00001270: 081c 1601 0a01 0e02 1601 0a01 0e04 0e01  ................
-00001280: 12ff 0404 0201 10fe 0408 1601 1a01 0e01  ................
-00001290: 0602 0801 1001 0801 1002 1001 0801 1c01  ................
-000012a0: 0402 0801 0201 0201 0201 0201 0201 0201  ................
-000012b0: 02fa 0809 0801 0402 0c01 1202 1201 0602  ................
-000012c0: 0a01 0201 0a01 02fc 0a07 0402 0201 0201  ................
-000012d0: 0201 02fc 02ff 0609 0201 0201 0201 0201  ................
-000012e0: 0201 0201 02fa 0408 7240 0000 0029 0472  ........r@...).r
-000012f0: 2600 0000 da0e 7375 625f 616c 6967 6e6d  &.....sub_alignm
-00001300: 656e 7473 da0b 6e75 6d5f 7175 6572 6965  ents..num_querie
-00001310: 7372 1900 0000 6303 0000 0000 0000 0000  sr....c.........
-00001320: 0000 001b 0000 000a 0000 0043 0000 0073  ...........C...s
-00001330: 5c02 0000 6401 6701 7c02 1400 7d03 6402  \...d.g.|...}.d.
-00001340: 7d04 7c01 4400 9002 5d42 7d05 7c05 6403  }.|.D...]B}.|.d.
-00001350: 1900 6402 1900 6404 6b02 7234 7400 a001  ..d...d.k.r4t...
-00001360: 6405 a101 0100 7112 7c05 6403 1900 6406  d.....q.|.d...d.
-00001370: 1900 6402 1900 5c03 7d06 7d07 7d08 7c05  ..d...\.}.}.}.|.
-00001380: 6407 1900 5c04 7d09 7d0a 7d0b 7d0c 7c00  d...\.}.}.}.}.|.
-00001390: 6a02 7c09 1900 7d0d 7c03 7c0d 1900 6401  j.|...}.|.|...d.
-000013a0: 6b08 7284 7c09 7c0b 7c06 1700 6602 6700  k.r.|.|.|...f.g.
-000013b0: 6602 7c03 7c0d 3c00 7c00 6a02 7c09 1900  f.|.|.<.|.j.|...
-000013c0: 7d0e 7c00 6a03 7c0e 1900 7d0f 7c00 6a04  }.|.j.|...}.|.j.
-000013d0: 7c0e 1900 7d10 7c03 7c0d 1900 6406 1900  |...}.|.|...d...
-000013e0: 7d11 7405 7c10 7406 8302 72be 7c10 6a07  }.t.|.t...r.|.j.
-000013f0: 6e02 6401 7d12 7c10 6a08 6a09 740a 6a0b  n.d.}.|.j.j.t.j.
-00001400: 6b02 72d4 6406 6e02 6408 7d13 7c09 7c0f  k.r.d.n.d.}.|.|.
-00001410: 1800 7d14 7c09 7d15 7c0b 7c06 1700 7d16  ..}.|.}.|.|...}.
-00001420: 7c12 6401 6b08 72f8 6402 6e0e 740c 7c12  |.d.k.r.d.n.t.|.
-00001430: 7c14 7c13 1400 1900 8301 7d17 7c08 4400  |.|.......}.|.D.
-00001440: 9001 5d46 7d18 7c18 6409 6b03 9001 723a  ..]F}.|.d.k...r:
-00001450: 7c12 6401 6b08 9001 722a 6402 6e0e 740c  |.d.k...r*d.n.t.
-00001460: 7c12 7c14 7c13 1400 1900 8301 7d17 7c18  |.|.|.......}.|.
-00001470: 640a 6b02 9001 7280 7c11 a00d 640b 740e  d.k...r.|...d.t.
-00001480: 7c00 6a08 7c15 1900 8301 740f 7c00 6a10  |.j.|.....t.|.j.
-00001490: 7c16 1900 8301 7c14 7c17 640c 9c05 a101  |.....|.|.d.....
-000014a0: 0100 7c14 6406 3700 7d14 7c15 6406 3700  ..|.d.7.}.|.d.7.
-000014b0: 7d15 6ed2 7c18 6409 6b02 9001 72be 7c11  }.n.|.d.k...r.|.
-000014c0: a00d 740e 7c00 6a08 7c16 1900 8301 640b  ..t.|.j.|.....d.
-000014d0: 740f 7c00 6a10 7c16 1900 8301 7c14 7c17  t.|.j.|.....|.|.
-000014e0: 640c 9c05 a101 0100 7c16 6406 3700 7d16  d.......|.d.7.}.
-000014f0: 6e94 7c18 640d 6b02 9001 73d6 7c18 640e  n.|.d.k...s.|.d.
-00001500: 6b02 9001 73d6 7411 8201 740e 7c00 6a08  k...s.t...t.|.j.
-00001510: 7c16 1900 8301 7d19 740e 7c00 6a08 7c15  |.....}.t.|.j.|.
-00001520: 1900 8301 7d1a 7c18 640d 6b02 9002 720c  ....}.|.d.k...r.
-00001530: 7c19 7c1a 6b02 9002 731a 7411 8201 6e0e  |.|.k...s.t...n.
-00001540: 7c19 7c1a 6b03 9002 731a 7411 8201 7c11  |.|.k...s.t...|.
-00001550: a00d 7c19 7c1a 740f 7c00 6a10 7c16 1900  ..|.|.t.|.j.|...
-00001560: 8301 7c14 7c17 640c 9c05 a101 0100 7c14  ..|.|.d.......|.
-00001570: 6406 3700 7d14 7c15 6406 3700 7d15 7c16  d.7.}.|.d.7.}.|.
-00001580: 6406 3700 7d16 9001 710c 7112 7c03 5300  d.7.}...q.q.|.S.
-00001590: 290f 612f 0400 000a 2020 2020 436f 6d62  ).a/....    Comb
-000015a0: 696e 6520 7468 6520 7365 676d 656e 7473  ine the segments
-000015b0: 2062 726f 6b65 6e20 6279 2060 5f62 7265   broken by `_bre
-000015c0: 616b 5f71 7565 7279 6020 746f 6765 7468  ak_query` togeth
-000015d0: 6572 2074 6f20 6765 7420 6120 6c6f 6e67  er to get a long
-000015e0: 2071 7565 7279 2e0a 0a20 2020 204e 6f74   query...    Not
-000015f0: 653a 2054 6865 2073 6567 6d65 6e74 7320  e: The segments 
-00001600: 6865 7265 2063 6f6e 7461 696e 2074 6865  here contain the
-00001610: 206c 6576 656e 7368 7465 696e 2061 6c69   levenshtein ali
-00001620: 676e 6d65 6e74 2e0a 0a20 2020 2041 7267  gnment...    Arg
-00001630: 733a 0a20 2020 2020 2073 6f75 7263 6564  s:.      sourced
-00001640: 5f74 6578 743a 0a20 2020 2020 2020 2054  _text:.        T
-00001650: 6865 2053 6f75 7263 6564 5465 7874 2063  he SourcedText c
-00001660: 6f6e 7461 696e 696e 6720 7468 6520 7175  ontaining the qu
-00001670: 6572 6965 7320 616e 6420 7265 6665 7265  eries and refere
-00001680: 6e63 6573 2e0a 2020 2020 2020 7375 625f  nces..      sub_
-00001690: 616c 6967 6e6d 656e 7473 3a0a 2020 2020  alignments:.    
-000016a0: 2020 2020 4120 6c69 7374 206f 6620 7365      A list of se
-000016b0: 676d 656e 7473 2c20 6561 6368 2069 7465  gments, each ite
-000016c0: 6d20 2872 6574 7572 6e65 6420 6279 206c  m (returned by l
-000016d0: 6576 656e 7368 7465 696e 5f77 6f72 6b65  evenshtein_worke
-000016e0: 7229 2063 6f6e 7461 696e 730a 2020 2020  r) contains.    
-000016f0: 2020 2020 7468 6520 7365 676d 656e 7420      the segment 
-00001700: 6974 2062 656c 6f6e 6773 2074 6f20 616e  it belongs to an
-00001710: 6420 7468 6520 6c65 7665 6e73 6874 6569  d the levenshtei
-00001720: 6e20 616c 6967 6e6d 656e 742e 0a20 2020  n alignment..   
-00001730: 2020 206e 756d 5f71 7565 7269 6573 3a0a     num_queries:.
-00001740: 2020 2020 2020 2020 5468 6520 6e75 6d62          The numb
-00001750: 6572 206f 6620 7175 6572 6965 732c 2074  er of queries, t
-00001760: 6869 7320 6172 6775 6d65 6e74 2069 7320  his argument is 
-00001770: 666f 7220 6566 6669 6369 656e 6379 2c20  for efficiency, 
-00001780: 6966 2077 6520 6b6e 6f77 206e 756d 6265  if we know numbe
-00001790: 720a 2020 2020 2020 2020 6f66 2071 7565  r.        of que
-000017a0: 7269 6573 2077 6520 6361 6e20 7072 6561  ries we can prea
-000017b0: 6c6c 6f63 6174 6520 7468 6520 6c69 7374  llocate the list
-000017c0: 2e0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-000017d0: 2020 2020 2052 6574 7572 6e20 6120 6c69       Return a li
-000017e0: 7374 206f 6620 7475 706c 6520 636f 6e74  st of tuple cont
-000017f0: 6169 6e69 6e67 2028 2871 7565 7279 5f73  aining ((query_s
-00001800: 7461 7274 2c20 7461 7267 6574 5f73 7461  tart, target_sta
-00001810: 7274 292c 205b 616c 6967 6e6d 656e 7420  rt), [alignment 
-00001820: 6974 656d 5d29 2e0a 2020 2020 2020 5468  item])..      Th
-00001830: 6520 6071 7565 7279 5f73 7461 7274 6020  e `query_start` 
-00001840: 616e 6420 6074 6172 6765 745f 7374 6172  and `target_star
-00001850: 7460 2061 7265 2069 6e64 6578 6573 2069  t` are indexes i
-00001860: 6e20 736f 7572 6365 645f 7465 7874 2c20  n sourced_text, 
-00001870: 7468 6520 6061 6c69 676e 6d65 6e74 2069  the `alignment i
-00001880: 7465 6d60 0a20 2020 2020 2069 7320 6120  tem`.      is a 
-00001890: 6c69 7374 2063 6f6e 7461 696e 696e 6720  list containing 
-000018a0: 7b22 7265 6622 3a20 7265 662c 2022 6879  {"ref": ref, "hy
-000018b0: 7022 3a20 6879 702c 2022 7265 665f 706f  p": hyp, "ref_po
-000018c0: 7322 3a20 7265 665f 706f 732c 2022 6879  s": ref_pos, "hy
-000018d0: 705f 706f 7322 3a20 6879 705f 706f 732c  p_pos": hyp_pos,
-000018e0: 0a20 2020 2020 2022 6879 705f 7469 6d65  .      "hyp_time
-000018f0: 223a 2068 7970 5f74 696d 657d 2c20 7265  ": hyp_time}, re
-00001900: 6620 6973 2074 6865 2074 6f6b 656e 2066  f is the token f
-00001910: 726f 6d20 7265 6665 7265 6e63 652c 2068  rom reference, h
-00001920: 7970 2069 7320 7468 6520 746f 6b65 6e20  yp is the token 
-00001930: 6672 6f6d 2071 7565 7279 2c0a 2020 2020  from query,.    
-00001940: 2020 7265 665f 706f 7320 6973 206c 6f63    ref_pos is loc
-00001950: 616c 2069 6e64 6578 2069 6e20 7265 6665  al index in refe
-00001960: 7265 6e63 6520 646f 6375 6d65 6e74 2c20  rence document, 
-00001970: 6879 705f 706f 7320 6973 206c 6f63 616c  hyp_pos is local
-00001980: 2069 6e64 6578 2069 6e20 7175 6572 7920   index in query 
-00001990: 646f 6375 6d65 6e74 2c0a 2020 2020 2020  document,.      
-000019a0: 6879 705f 7469 6d65 2069 7320 7468 6520  hyp_time is the 
-000019b0: 7469 6d65 7374 616d 7020 6f66 2068 7970  timestamp of hyp
-000019c0: 2e0a 2020 2020 4e72 0100 0000 da09 616c  ..    Nr......al
-000019d0: 6967 6e6d 656e 7472 2b00 0000 7a1b 536b  ignmentr+...z.Sk
-000019e0: 6970 7069 6e67 2065 6d70 7479 2073 7562  ipping empty sub
-000019f0: 2073 6567 6d65 6e74 2e72 0f00 0000 da07   segment.r......
-00001a00: 7365 676d 656e 7472 2c00 0000 da01 44da  segmentr,.....D.
-00001a10: 0149 da00 2905 da03 7265 66da 0368 7970  .I..)...ref..hyp
-00001a20: da07 7265 665f 706f 73da 0768 7970 5f70  ..ref_pos..hyp_p
-00001a30: 6f73 da08 6879 705f 7469 6d65 da01 43da  os..hyp_time..C.
-00001a40: 0153 2912 da07 6c6f 6767 696e 67da 0777  .S)...logging..w
-00001a50: 6172 6e69 6e67 7237 0000 0072 3800 0000  arningr7...r8...
-00001a60: da07 736f 7572 6365 73da 0a69 7369 6e73  ..sources..isins
-00001a70: 7461 6e63 6572 1300 0000 da05 7469 6d65  tancer......time
-00001a80: 73da 0b62 696e 6172 795f 7465 7874 721a  s..binary_textr.
-00001a90: 0000 0072 1e00 0000 da05 7569 6e74 38da  ...r......uint8.
-00001aa0: 0566 6c6f 6174 722e 0000 00da 0363 6872  .floatr......chr
-00001ab0: da03 696e 74da 0370 6f73 721c 0000 0029  ..int..posr....)
-00001ac0: 1b72 2600 0000 7241 0000 0072 4200 0000  .r&...rA...rB...
-00001ad0: da0a 616c 6967 6e6d 656e 7473 5a0f 7072  ..alignmentsZ.pr
-00001ae0: 6576 5f74 6172 6765 745f 656e 64da 0373  ev_target_end..s
-00001af0: 7562 5a12 7461 7267 6574 5f61 6c69 676e  ubZ.target_align
-00001b00: 5f73 7461 7274 5a10 7461 7267 6574 5f61  _startZ.target_a
-00001b10: 6c69 676e 5f65 6e64 5a09 616c 6967 6e5f  lign_endZ.align_
-00001b20: 7374 7272 2f00 0000 7230 0000 0072 3100  strr/...r0...r1.
-00001b30: 0000 7232 0000 005a 0871 7565 7279 5f69  ..r2...Z.query_i
-00001b40: 6472 3d00 0000 723e 0000 00da 0c71 7565  dr=...r>.....que
-00001b50: 7279 5f73 6f75 7263 65da 0661 6c69 676e  ry_source..align
-00001b60: 7372 5300 0000 5a0b 7469 6d65 5f73 7472  srS...Z.time_str
-00001b70: 6964 655a 1171 7565 7279 5f6c 6f63 616c  ideZ.query_local
-00001b80: 5f69 6e64 6578 5a0b 7175 6572 795f 696e  _indexZ.query_in
-00001b90: 6465 785a 0c74 6172 6765 745f 696e 6465  dexZ.target_inde
-00001ba0: 7872 4c00 0000 5a03 616c 6972 4800 0000  xrL...Z.alirH...
-00001bb0: 7249 0000 0072 2200 0000 7222 0000 0072  rI...r"...r"...r
-00001bc0: 2300 0000 da17 5f63 6f6d 6269 6e65 5f73  #....._combine_s
-00001bd0: 7562 5f61 6c69 676e 6d65 6e74 73f5 0000  ub_alignments...
-00001be0: 0073 8800 0000 001a 0a01 0401 0a01 1001  .s..............
-00001bf0: 0a01 0204 1601 1001 0a02 0c02 0a01 02fe  ................
-00001c00: 0805 0a01 0a01 0a03 0c03 1402 1602 0801  ................
-00001c10: 0401 0802 1c01 0a01 0a03 06ff 0802 0efd  ................
-00001c20: 0205 0a01 0402 0201 0c01 0c01 0201 02fb  ................
-00001c30: 04ff 0409 0801 0a01 0a01 0402 0c01 0201  ................
-00001c40: 0c01 0201 02fb 04ff 0409 0a02 1801 0e01  ................
-00001c50: 0e03 0a01 1002 0e01 0402 0201 0201 0c01  ................
-00001c60: 0201 02fb 04ff 0409 0801 0801 0e01 725e  ..............r^
-00001c70: 0000 0029 0672 2600 0000 da0d 636c 6f73  ...).r&.....clos
-00001c80: 655f 6d61 7463 6865 7372 2800 0000 7229  e_matchesr(...r)
-00001c90: 0000 00da 0b74 6872 6561 645f 706f 6f6c  .....thread_pool
-00001ca0: 7219 0000 0063 0500 0000 0000 0000 0000  r....c..........
-00001cb0: 0000 1e00 0000 0700 0000 4300 0000 7356  ..........C...sV
-00001cc0: 0200 007c 016a 005c 027d 057d 067c 006a  ...|.j.\.}.}.|.j
-00001cd0: 017c 0519 007d 077c 006a 027d 0874 03a0  .|...}.|.j.}.t..
-00001ce0: 0464 01a1 0101 0067 007d 0974 057c 0783  .d.....g.}.t.|..
-00001cf0: 0144 0090 015d c87d 0a7c 087c 0a19 007d  .D...].}.|.|...}
-00001d00: 0b7c 087c 0a64 0217 0019 007d 0c7c 087c  .|.|.d.....}.|.|
-00001d10: 0a64 0217 0019 007c 087c 0a19 0018 007d  .d.....|.|.....}
-00001d20: 0d74 06a0 077c 0b7c 0ca1 02a0 0864 0364  .t...|.|.....d.d
-00001d30: 02a1 027d 0e74 06a0 097c 0e7c 06a1 02a0  ...}.t...|.|....
-00001d40: 0aa1 007d 0e7c 017c 0b7c 0c85 0264 0464  ...}.|.|.|...d.d
-00001d50: 0485 0266 0219 00a0 0aa1 007d 0f74 0b7c  ...f.......}.t.|
-00001d60: 0e7c 0f83 027d 1074 0c7c 1083 0164 0218  .|...}.t.|...d..
-00001d70: 007d 117c 107c 1119 0064 0219 007c 006a  .}.|.|...d...|.j
-00001d80: 0d6a 0e64 0218 006b 0272 d27c 1164 0238  .j.d...k.r.|.d.8
-00001d90: 007d 1171 b07c 1064 057c 1185 0219 007d  .}.q.|.d.|.....}
-00001da0: 107c 006a 0174 06a0 0f64 0664 0784 007c  .|.j.t...d.d...|
-00001db0: 1044 0083 01a1 0119 007d 127c 127c 1264  .D.......}.|.|.d
-00001dc0: 0519 0018 007d 1274 107c 1283 017d 1364  .....}.t.|...}.d
-00001dd0: 037d 1464 0574 0c7c 1083 0166 027d 1574  .}.d.t.|...f.}.t
-00001de0: 057c 136a 0e64 0218 0083 0144 005d 6e7d  .|.j.d.....D.]n}
-00001df0: 167c 137c 1664 0217 0019 007c 137c 1619  .|.|.d.....|.|..
-00001e00: 0018 0064 086b 0090 0172 4c90 0171 2a7c  ...d.k...rL..q*|
-00001e10: 107c 137c 1664 0217 0019 0064 0218 0019  .|.|.d.....d....
-00001e20: 0064 0519 007c 107c 137c 1619 0019 0064  .d...|.|.|.....d
-00001e30: 0519 0018 007d 177c 177c 146b 0490 0172  .....}.|.|.k...r
-00001e40: 2a7c 177d 147c 137c 1619 007c 137c 1664  *|.}.|.|...|.|.d
-00001e50: 0217 0019 0066 027d 1590 0171 2a7c 1464  .....f.}...q*|.d
-00001e60: 097c 0d14 006b 0090 0172 bc74 03a0 1164  .|...k...r.t...d
-00001e70: 0a7c 0a9b 0064 0b9d 03a1 0101 0071 307c  .|...d.......q0|
-00001e80: 107c 1564 0519 007c 1564 0219 0085 0219  .|.d...|.d......
-00001e90: 007d 1074 127c 007c 107c 027c 0364 0c8d  .}.t.|.|.|.|.d..
-00001ea0: 047d 187c 1844 005d 147d 197c 09a0 137c  .}.|.D.].}.|...|
-00001eb0: 007c 1966 02a1 0101 0090 0171 e471 3074  .|.f.......q.q0t
-00001ec0: 03a0 0464 0da1 0101 0064 0e64 0f84 007d  ...d.....d.d...}
-00001ed0: 1a7c 0464 046b 0890 0272 1e74 1483 006e  .|.d.k...r.t...n
-00001ee0: 027c 047d 1b74 03a0 0464 10a1 0101 007c  .|.}.t...d.....|
-00001ef0: 1ba0 157c 1a7c 09a1 027d 1c7c 1ca0 16a1  ...|.|...}.|....
-00001f00: 007d 1d74 03a0 0464 11a1 0101 0074 177c  .}.t...d.....t.|
-00001f10: 007c 1d7c 0783 0353 0029 1261 0d07 0000  .|.|...S.).a....
-00001f20: 0a20 2020 2047 6574 206c 6576 656e 7368  .    Get levensh
-00001f30: 7465 696e 2061 6c69 676e 6d65 6e74 2066  tein alignment f
-00001f40: 6f72 2065 6163 6820 7175 6572 7920 646f  or each query do
-00001f50: 6375 6d65 6e74 2069 6e20 736f 7572 6365  cument in source
-00001f60: 645f 7465 7874 2e0a 0a20 2020 2046 6f72  d_text...    For
-00001f70: 2065 6163 6820 7175 6572 7920 646f 6375   each query docu
-00001f80: 6d65 6e74 2077 6520 7769 6c6c 206c 6f63  ment we will loc
-00001f90: 6174 6520 6974 7320 636f 7272 6573 706f  ate its correspo
-00001fa0: 6e64 696e 6720 7365 676d 656e 7420 696e  nding segment in
-00001fb0: 2074 6865 2072 6566 6572 656e 6365 0a20   the reference. 
-00001fc0: 2020 2064 6f63 756d 656e 7420 616e 6420     document and 
-00001fd0: 7265 7475 726e 2074 6865 206c 6576 656e  return the leven
-00001fe0: 7368 7465 696e 2061 6c69 676e 6d65 6e74  shtein alignment
-00001ff0: 2062 6574 7765 656e 2074 6865 2071 7565   between the que
-00002000: 7279 2061 6e64 2069 7473 2063 6f72 7265  ry and its corre
-00002010: 7370 6f6e 6469 6e67 0a20 2020 2072 6566  sponding.    ref
-00002020: 6572 656e 6365 2073 6567 6d65 6e74 2e0a  erence segment..
-00002030: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00002040: 2073 6f75 7263 6564 5f74 6578 743a 0a20   sourced_text:. 
-00002050: 2020 2020 2020 2054 6865 2053 6f75 7263         The Sourc
-00002060: 6564 5465 7874 2063 6f6e 7461 696e 696e  edText containin
-00002070: 6720 7468 6520 7175 6572 6965 7320 616e  g the queries an
-00002080: 6420 7265 6665 7265 6e63 6573 2c20 7468  d references, th
-00002090: 6520 6669 7273 7420 4e20 2877 6520 6361  e first N (we ca
-000020a0: 6e0a 2020 2020 2020 2020 6765 7420 6974  n.        get it
-000020b0: 2066 726f 6d20 636c 6f73 655f 6d61 7463   from close_matc
-000020c0: 6865 7329 2064 6f63 756d 656e 7473 2061  hes) documents a
-000020d0: 7265 2071 7565 7269 6573 2061 6e64 2074  re queries and t
-000020e0: 6865 206f 7468 6572 7320 6172 6520 7265  he others are re
-000020f0: 6665 7265 6e63 6573 2e0a 2020 2020 2020  ferences..      
-00002100: 636c 6f73 655f 6d61 7463 6865 733a 0a20  close_matches:. 
-00002110: 2020 2020 2020 2047 656e 6572 6174 6564         Generated
-00002120: 2066 726f 6d20 736f 7572 6365 645f 7465   from sourced_te
-00002130: 7874 2077 6974 6820 7468 6520 6675 6e63  xt with the func
-00002140: 7469 6f6e 2060 6669 6e64 5f63 616e 6469  tion `find_candi
-00002150: 6461 7465 5f6d 6174 6368 6573 602e 0a20  date_matches`.. 
-00002160: 2020 2020 2020 2049 7420 636f 6e74 6169         It contai
-00002170: 6e73 2074 6865 2063 6c6f 7365 206d 6174  ns the close mat
-00002180: 6368 6564 2072 6566 6572 656e 6365 2074  ched reference t
-00002190: 6f6b 656e 2066 6f72 2065 6163 6820 7175  oken for each qu
-000021a0: 6572 7920 746f 6b65 6e2e 0a20 2020 2020  ery token..     
-000021b0: 2073 6567 6d65 6e74 5f6c 656e 6774 683a   segment_length:
-000021c0: 0a20 2020 2020 2020 2054 6865 2071 7565  .        The que
-000021d0: 7279 206c 656e 6774 6820 6d69 6768 7420  ry length might 
-000021e0: 6265 206c 6f6e 672c 2069 6e20 6f72 6465  be long, in orde
-000021f0: 7220 746f 2061 6363 656c 6572 6174 6520  r to accelerate 
-00002200: 7468 6520 6c65 7665 6e73 6874 6569 6e0a  the levenshtein.
-00002210: 2020 2020 2020 2020 616c 676f 7269 7468          algorith
-00002220: 6d20 7765 2077 696c 6c20 7370 6c69 7420  m we will split 
-00002230: 7468 6520 6c6f 6e67 2071 7565 7279 2069  the long query i
-00002240: 6e74 6f20 736d 616c 6c65 7220 7365 676d  nto smaller segm
-00002250: 656e 7473 2c20 6073 6567 6d65 6e74 5f6c  ents, `segment_l
-00002260: 656e 6774 6860 0a20 2020 2020 2020 2069  ength`.        i
-00002270: 7320 7468 6520 6578 7065 6374 6564 206c  s the expected l
-00002280: 656e 6774 6820 6f66 2074 6865 2073 6d61  ength of the sma
-00002290: 6c6c 6572 2073 6567 6d65 6e74 732e 0a20  ller segments.. 
-000022a0: 2020 2020 2072 6566 6572 656e 6365 5f6c       reference_l
-000022b0: 656e 6774 685f 6469 6666 6572 656e 6365  ength_difference
-000022c0: 3a0a 2020 2020 2020 2020 4265 6361 7573  :.        Becaus
-000022d0: 6520 6f66 2074 6865 2069 6e73 6572 7469  e of the inserti
-000022e0: 6f6e 206f 7220 6465 6c65 7469 6f6e 2065  on or deletion e
-000022f0: 7272 6f72 732c 2074 6865 2072 6566 6572  rrors, the refer
-00002300: 656e 6365 2073 6571 7565 6e63 6520 6d69  ence sequence mi
-00002310: 6768 7420 6265 0a20 2020 2020 2020 2073  ght be.        s
-00002320: 686f 7274 6572 206f 7220 6c6f 6e67 6572  horter or longer
-00002330: 2074 6861 6e20 7468 6520 7175 6572 792c   than the query,
-00002340: 2073 6f20 7468 6520 7265 6665 7265 6e63   so the referenc
-00002350: 6520 7365 676d 656e 7420 6c65 6e67 7468  e segment length
-00002360: 2063 616e 2062 6520 6672 6f6d 0a20 2020   can be from.   
-00002370: 2020 2020 2060 6c65 6e28 7175 6572 7929       `len(query)
-00002380: 202a 2028 3120 2d20 7265 6665 7265 6e63   * (1 - referenc
-00002390: 655f 6c65 6e67 7468 5f64 6966 6665 7265  e_length_differe
-000023a0: 6e63 6520 2f20 3229 6020 746f 0a20 2020  nce / 2)` to.   
-000023b0: 2020 2020 2060 6c65 6e28 7175 6572 7929       `len(query)
-000023c0: 202a 2028 3120 2b20 7265 6665 7265 6e63   * (1 + referenc
-000023d0: 655f 6c65 6e67 7468 5f64 6966 6665 7265  e_length_differe
-000023e0: 6e63 6520 2f20 3229 602e 0a20 2020 2020  nce / 2)`..     
-000023f0: 2074 6872 6561 645f 706f 6f6c 3a0a 2020   thread_pool:.  
-00002400: 2020 2020 2020 5468 6520 5468 7265 6164        The Thread
-00002410: 506f 6f6c 2074 6f20 7275 6e20 6c65 7665  Pool to run leve
-00002420: 6e73 6874 6569 6e2e 0a20 2020 2052 6574  nshtein..    Ret
-00002430: 7572 6e73 3a0a 2020 2020 2020 5265 7475  urns:.      Retu
-00002440: 726e 2061 206c 6973 7420 6f66 2074 7570  rn a list of tup
-00002450: 6c65 2063 6f6e 7461 696e 696e 6720 2828  le containing ((
-00002460: 7175 6572 795f 7374 6172 742c 2074 6172  query_start, tar
-00002470: 6765 745f 7374 6172 7429 2c20 5b61 6c69  get_start), [ali
-00002480: 676e 6d65 6e74 2069 7465 6d5d 292e 0a20  gnment item]).. 
-00002490: 2020 2020 2054 6865 2060 7175 6572 795f       The `query_
-000024a0: 7374 6172 7460 2061 6e64 2060 7461 7267  start` and `targ
-000024b0: 6574 5f73 7461 7274 6020 6172 6520 696e  et_start` are in
-000024c0: 6465 7865 7320 696e 2073 6f75 7263 6564  dexes in sourced
-000024d0: 5f74 6578 742c 2074 6865 2060 616c 6967  _text, the `alig
-000024e0: 6e6d 656e 7420 6974 656d 600a 2020 2020  nment item`.    
-000024f0: 2020 6973 2061 206c 6973 7420 636f 6e74    is a list cont
-00002500: 6169 6e69 6e67 207b 2272 6566 223a 2072  aining {"ref": r
-00002510: 6566 2c20 2268 7970 223a 2068 7970 2c20  ef, "hyp": hyp, 
-00002520: 2272 6566 5f70 6f73 223a 2072 6566 5f70  "ref_pos": ref_p
-00002530: 6f73 2c20 2268 7970 5f70 6f73 223a 2068  os, "hyp_pos": h
-00002540: 7970 5f70 6f73 2c0a 2020 2020 2020 2268  yp_pos,.      "h
-00002550: 7970 5f74 696d 6522 3a20 6879 705f 7469  yp_time": hyp_ti
-00002560: 6d65 7d2c 2072 6566 2069 7320 7468 6520  me}, ref is the 
-00002570: 746f 6b65 6e20 6672 6f6d 2072 6566 6572  token from refer
-00002580: 656e 6365 2c20 6879 7020 6973 2074 6865  ence, hyp is the
-00002590: 2074 6f6b 656e 2066 726f 6d20 7175 6572   token from quer
-000025a0: 792c 0a20 2020 2020 2072 6566 5f70 6f73  y,.      ref_pos
-000025b0: 2069 7320 6c6f 6361 6c20 696e 6465 7820   is local index 
-000025c0: 696e 2072 6566 6572 656e 6365 2064 6f63  in reference doc
-000025d0: 756d 656e 742c 2068 7970 5f70 6f73 2069  ument, hyp_pos i
-000025e0: 7320 6c6f 6361 6c20 696e 6465 7820 696e  s local index in
-000025f0: 2071 7565 7279 2064 6f63 756d 656e 742c   query document,
-00002600: 0a20 2020 2020 2068 7970 5f74 696d 6520  .      hyp_time 
-00002610: 6973 2074 6865 2074 696d 6573 7461 6d70  is the timestamp
-00002620: 206f 6620 6879 702e 0a20 2020 207a 1847   of hyp..    z.G
-00002630: 6574 7469 6e67 206d 6174 6368 696e 6720  etting matching 
-00002640: 706f 696e 7473 2e72 0f00 0000 722b 0000  points.r....r+..
-00002650: 004e 7201 0000 0063 0100 0000 0000 0000  .Nr....c........
-00002660: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00002670: 7314 0000 0067 007c 005d 0c7d 017c 0164  s....g.|.].}.|.d
-00002680: 0019 0091 0271 0453 0029 0172 0f00 0000  .....q.S.).r....
-00002690: 7222 0000 0029 02da 022e 30da 0178 7222  r"...)....0..xr"
-000026a0: 0000 0072 2200 0000 7223 0000 00da 0a3c  ...r"...r#.....<
-000026b0: 6c69 7374 636f 6d70 3eb1 0100 0073 0400  listcomp>....s..
-000026c0: 0000 0600 0200 7a22 6765 745f 616c 6967  ......z"get_alig
-000026d0: 6e6d 656e 7473 2e3c 6c6f 6361 6c73 3e2e  nments.<locals>.
-000026e0: 3c6c 6973 7463 6f6d 703e 722a 0000 0067  <listcomp>r*...g
-000026f0: 1f85 eb51 b81e d53f 7a0f 536b 6970 7069  ...Q...?z.Skippi
-00002700: 6e67 2071 7565 7279 207a 342c 206c 6573  ng query z4, les
-00002710: 7320 7468 616e 2031 202f 2033 206f 6620  s than 1 / 3 of 
-00002720: 7175 6572 7920 6d61 7463 6865 6420 6279  query matched by
-00002730: 2063 6c6f 7365 5f6d 6174 6368 6573 2e29   close_matches.)
-00002740: 0472 2600 0000 7227 0000 0072 2800 0000  .r&...r'...r(...
-00002750: 7229 0000 007a 1d47 6574 7469 6e67 206d  r)...z.Getting m
-00002760: 6174 6368 696e 6720 706f 696e 7473 2064  atching points d
-00002770: 6f6e 652e 6302 0000 0000 0000 0000 0000  one.c...........
-00002780: 0005 0000 0005 0000 0053 0000 0073 4400  .........S...sD.
-00002790: 0000 7c00 6a00 7c01 6401 1900 7c01 6402  ..|.j.|.d...|.d.
-000027a0: 1900 8502 1900 7d02 7c00 6a00 7c01 6403  ......}.|.j.|.d.
-000027b0: 1900 7c01 6404 1900 8502 1900 7d03 7401  ..|.d.......}.t.
-000027c0: 7c02 7c03 6405 6406 8d03 7d04 7c01 7c04  |.|.d.d...}.|.|.
-000027d0: 6407 9c02 5300 2908 4e72 0100 0000 720f  d...S.).Nr....r.
-000027e0: 0000 0072 2a00 0000 e903 0000 00da 0667  ...r*..........g
-000027f0: 6c6f 6261 6c29 03da 0571 7565 7279 da06  lobal)...query..
-00002800: 7461 7267 6574 da04 6d6f 6465 2902 7244  target..mode).rD
-00002810: 0000 0072 4300 0000 2902 7254 0000 0072  ...rC...).rT...r
-00002820: 0e00 0000 2905 7226 0000 0072 4400 0000  ....).r&...rD...
-00002830: 7266 0000 0072 6700 0000 7243 0000 0072  rf...rg...rC...r
-00002840: 2200 0000 7222 0000 0072 2300 0000 da12  "...r"...r#.....
-00002850: 6c65 7665 6e73 6874 6569 6e5f 776f 726b  levenshtein_work
-00002860: 6572 da01 0000 730c 0000 0000 0116 0116  er....s.........
-00002870: 030e 0202 0102 fe7a 2a67 6574 5f61 6c69  .......z*get_ali
-00002880: 676e 6d65 6e74 732e 3c6c 6f63 616c 733e  gnments.<locals>
-00002890: 2e6c 6576 656e 7368 7465 696e 5f77 6f72  .levenshtein_wor
-000028a0: 6b65 727a 1a4d 6174 6368 696e 6720 7769  kerz.Matching wi
-000028b0: 7468 206c 6576 656e 7368 7465 696e 2e7a  th levenshtein.z
-000028c0: 1f4d 6174 6368 696e 6720 7769 7468 206c  .Matching with l
-000028d0: 6576 656e 7368 7465 696e 2064 6f6e 652e  evenshtein done.
-000028e0: 2918 da05 7368 6170 6572 3700 0000 7238  )...shaper7...r8
-000028f0: 0000 0072 4f00 0000 da04 696e 666f 722d  ...rO.....infor-
-00002900: 0000 0072 1e00 0000 da06 6172 616e 6765  ...r......arange
-00002910: da07 7265 7368 6170 65da 0474 696c 65da  ..reshape..tile.
-00002920: 0766 6c61 7474 656e 720d 0000 0072 3600  .flattenr....r6.
-00002930: 0000 7254 0000 0072 1d00 0000 da05 6172  ..rT...r......ar
-00002940: 7261 7972 1600 0000 7250 0000 0072 4000  rayr....rP...r@.
-00002950: 0000 722e 0000 0072 0600 0000 5a0d 7374  ..r....r....Z.st
-00002960: 6172 6d61 705f 6173 796e 63da 0367 6574  armap_async..get
-00002970: 725e 0000 0029 1e72 2600 0000 725f 0000  r^...).r&...r_..
-00002980: 0072 2800 0000 7229 0000 0072 6000 0000  .r(...r)...r`...
-00002990: da11 746f 745f 7175 6572 795f 7379 6d62  ..tot_query_symb
-000029a0: 6f6c 73da 116e 756d 5f63 6c6f 7365 5f6d  ols..num_close_m
-000029b0: 6174 6368 6573 7242 0000 00da 0a72 6f77  atchesrB.....row
-000029c0: 5f73 706c 6974 73da 0961 7267 756d 656e  _splits..argumen
-000029d0: 7473 da01 7172 2f00 0000 7230 0000 00da  ts..qr/...r0....
-000029e0: 0971 7565 7279 5f6c 656e 7217 0000 0072  .query_lenr....r
-000029f0: 1800 0000 7227 0000 005a 0874 7269 6d5f  ....r'...Z.trim_
-00002a00: 706f 735a 0764 6f63 5f69 6473 7238 0000  posZ.doc_idsr8..
-00002a10: 005a 0f6d 6178 5f6e 756d 5f6d 6174 6368  .Z.max_num_match
-00002a20: 6573 5a0a 6d61 785f 7261 6e67 6573 7234  esZ.max_rangesr4
-00002a30: 0000 005a 0b6e 756d 5f6d 6174 6368 6573  ...Z.num_matches
-00002a40: 7233 0000 00da 0373 6567 7269 0000 00da  r3.....segri....
-00002a50: 0470 6f6f 6c5a 0d61 7379 6e63 5f72 6573  .poolZ.async_res
-00002a60: 756c 7473 da07 7265 7375 6c74 7372 2200  ults..resultsr".
-00002a70: 0000 7222 0000 0072 2300 0000 da0e 6765  ..r"...r#.....ge
-00002a80: 745f 616c 6967 6e6d 656e 7473 6a01 0000  t_alignmentsj...
-00002a90: 736c 0000 0000 280a 010a 0206 020a 0104  sl....(.........
-00002aa0: 010e 0108 010c 0114 0414 0110 0218 020a  ................
-00002ab0: 040c 0118 010a 010c 051a 030c 0108 0104  ................
-00002ac0: 010c 0112 011a 0104 0216 010e ff02 ff02  ................
-00002ad0: 040a 0104 0118 020e 0104 010a ff04 0302  ................
-00002ae0: 0214 0402 0102 0102 0102 0102 fc06 0808  ................
-00002af0: 0114 020a 0208 0b14 010a 010c 0108 010a  ................
-00002b00: 0272 7b00 0000 2902 da0d 7461 7267 6574  .r{...)...target
-00002b10: 5f73 6f75 7263 6572 1900 0000 6302 0000  _sourcer....c...
-00002b20: 0000 0000 0000 0000 0030 0000 0007 0000  .........0......
-00002b30: 0043 0000 0073 c607 0000 7c01 5c02 5c02  .C...s....|.\.\.
-00002b40: 7d02 7d03 7d04 6700 7d05 6700 7d06 6401  }.}.}.g.}.g.}.d.
-00002b50: 7d07 7400 6402 6403 8400 7c04 6404 7c07  }.t.d.d...|.d.|.
-00002b60: 8502 1900 4400 8301 8301 7d08 6405 7d09  ....D.....}.d.}.
-00002b70: 7c09 7d0a 7c09 7d0b 6404 6701 7401 7c04  |.}.|.}.d.g.t.|.
-00002b80: 8301 1400 7d0c 6404 6701 7401 7c04 8301  ....}.d.g.t.|...
-00002b90: 1400 7d0d 7402 7c04 8301 4400 9002 5d5c  ..}.t.|...D...]\
-00002ba0: 5c02 7d0e 7d0f 7c0f 6406 1900 7c0f 6407  \.}.}.|.d...|.d.
-00002bb0: 1900 6b02 7d10 7c0e 6404 6b02 728c 7403  ..k.}.|.d.k.r.t.
-00002bc0: 7c10 8301 6e12 7c0c 7c0e 6408 1800 1900  |...n.|.|.d.....
-00002bd0: 7403 7c10 8301 1700 7c0c 7c0e 3c00 7c0e  t.|.....|.|.<.|.
-00002be0: 6404 6b02 72b6 7403 7c10 0c00 8301 6e14  d.k.r.t.|.....n.
-00002bf0: 7c0d 7c0e 6408 1800 1900 7403 7c10 0c00  |.|.d.....t.|...
-00002c00: 8301 1700 7c0d 7c0e 3c00 7c0e 7c07 1800  ....|.|.<.|.|...
-00002c10: 6404 6b05 9001 7208 7c04 7c0e 7c07 1800  d.k...r.|.|.|...
-00002c20: 1900 6406 1900 7c04 7c0e 7c07 1800 1900  ..d...|.|.|.....
-00002c30: 6407 1900 6b03 9001 7208 7c08 6408 3800  d...k...r.|.d.8.
-00002c40: 7d08 7c0e 7c07 1700 7401 7c04 8301 6b00  }.|.|...t.|...k.
-00002c50: 9001 7244 7c04 7c0e 7c07 1700 1900 6406  ..rD|.|.|.....d.
-00002c60: 1900 7c04 7c0e 7c07 1700 1900 6407 1900  ..|.|.|.....d...
-00002c70: 6b03 9001 7244 7c08 6408 3700 7d08 7c0e  k...rD|.d.7.}.|.
-00002c80: 6404 6b02 9001 7252 7c0a 6e16 7c0f 6409  d.k...rR|.n.|.d.
-00002c90: 1900 7c04 7c0e 6408 1800 1900 6409 1900  ..|.|.d.....d...
-00002ca0: 1800 7d11 7c11 7c0a 6b04 9001 7278 7c0a  ..}.|.|.k...rx|.
-00002cb0: 6e02 7c11 7d11 7c0e 7401 7c04 8301 6408  n.|.}.|.t.|...d.
-00002cc0: 1800 6b02 9001 7292 7c0a 6e16 7c04 7c0e  ..k...r.|.n.|.|.
-00002cd0: 6408 1700 1900 6409 1900 7c0f 6409 1900  d.....d...|.d...
-00002ce0: 1800 7d12 7c12 7c0a 6b04 9001 72b8 7c0a  ..}.|.|.k...r.|.
-00002cf0: 6e02 7c12 7d12 6404 7d13 7c0f 640a 1900  n.|.}.d.}.|.d...
-00002d00: 6408 1800 7d14 7c14 6404 6b05 9002 7222  d...}.|.d.k...r"
-00002d10: 7404 7c00 6a05 7c14 1900 8301 7d15 7406  t.|.j.|.....}.t.
-00002d20: 7c15 640b 640c 8d02 9001 72fc 7c0b 7d13  |.d.d.....r.|.}.
-00002d30: 9002 7122 6e22 7c15 640d 6b02 9002 7310  ..q"n"|.d.k...s.
-00002d40: 7406 7c15 8301 9002 7222 7c14 6408 3800  t.|.....r"|.d.8.
-00002d50: 7d14 6e04 9002 7122 9001 71cc 6404 7d16  }.n...q"..q.d.}.
-00002d60: 7c0f 640a 1900 6408 1700 7d14 7c14 7c00  |.d...d...}.|.|.
-00002d70: 6a05 6a07 6b00 9002 728c 7404 7c00 6a05  j.j.k...r.t.|.j.
-00002d80: 7c14 1900 8301 7d15 7406 7c15 640b 640c  |.....}.t.|.d.d.
-00002d90: 8d02 9002 7266 7c0b 7d16 9002 718c 6e22  ....rf|.}...q.n"
-00002da0: 7c15 640d 6b02 9002 737a 7406 7c15 8301  |.d.k...szt.|...
-00002db0: 9002 728c 7c14 6408 3700 7d14 6e04 9002  ..r.|.d.7.}.n...
-00002dc0: 718c 9002 7132 7c05 a008 7c0e 7c11 7c13  q...q2|...|.|.|.
-00002dd0: 1700 7c08 7c07 1b00 1800 6602 a101 0100  ..|.|.....f.....
-00002de0: 7c06 a008 7c0e 7c12 7c16 1700 7c08 7c07  |...|.|.|...|.|.
-00002df0: 1b00 1800 6602 a101 0100 7162 7409 7c05  ....f.....qbt.|.
-00002e00: 640e 640f 8400 640b 6410 8d03 7d17 7409  d.d...d.d...}.t.
-00002e10: 7c06 6411 640f 8400 640b 6410 8d03 7d18  |.d.d...d.d...}.
-00002e20: 6412 7d19 7c17 6404 7403 7401 7c05 8301  d.}.|.d.t.t.|...
-00002e30: 7c19 1400 8301 8502 1900 7d1a 7c18 6404  |.........}.|.d.
-00002e40: 7403 7401 7c06 8301 7c19 1400 8301 8502  t.t.|...|.......
-00002e50: 1900 7d1b 6700 7d1c 6700 7d1d 6413 7d1e  ..}.g.}.g.}.d.}.
-00002e60: 6414 7d1f 6415 7d20 7c09 7d21 6416 7d22  d.}.d.} |.}!d.}"
-00002e70: 6417 7d23 6418 7d24 7c1a 4400 9002 5d38  d.}#d.}$|.D...]8
-00002e80: 7d25 6700 7d26 7c25 6404 1900 6408 1700  }%g.}&|%d...d...
-00002e90: 7d27 7c27 7401 7c06 8301 6b00 9005 7232  }'|'t.|...k...r2
-00002ea0: 7c06 7c27 1900 6404 1900 7c25 6404 1900  |.|'..d...|%d...
-00002eb0: 1800 7c20 6b00 9005 7232 7c05 7c25 6404  ..| k...r2|.|%d.
-00002ec0: 1900 1900 6408 1900 7c06 7c27 1900 6408  ....d...|.|'..d.
-00002ed0: 1900 1700 7d28 7c09 7c0c 7c06 7c27 1900  ....}(|.|.|.|'..
-00002ee0: 6404 1900 1900 7c0c 7c25 6404 1900 1900  d.....|.|%d.....
-00002ef0: 1800 1400 7c06 7c27 1900 6404 1900 7c25  ....|.|'..d...|%
-00002f00: 6404 1900 1800 1b00 7d29 7c0d 7c06 7c27  d.......})|.|.|'
-00002f10: 1900 6404 1900 1900 7c0d 7c25 6404 1900  ..d.....|.|%d...
-00002f20: 1900 1800 7d2a 7c2a 7c06 7c27 1900 6404  ....}*|*|.|'..d.
-00002f30: 1900 7c25 6404 1900 1800 7c1f 1400 6b05  ..|%d.....|...k.
-00002f40: 9004 7216 7c27 6408 3700 7d27 9003 7158  ..r.|'d.7.}'..qX
-00002f50: 7c09 7c2a 1400 7c06 7c27 1900 6404 1900  |.|*..|.|'..d...
-00002f60: 7c25 6404 1900 1800 1b00 7d2b 7c04 7c06  |%d.......}+|.|.
-00002f70: 7c27 1900 6404 1900 1900 6409 1900 7c04  |'..d.....d...|.
-00002f80: 7c25 6404 1900 1900 6409 1900 1800 7d2c  |%d.....d.....},
-00002f90: 7c2c 7c22 6b05 9004 736a 7c2c 7c23 6b01  |,|"k...sj|,|#k.
-00002fa0: 9004 7272 740a 6419 8301 6e02 7c21 7d2d  ..rrt.d...n.|!}-
-00002fb0: 7c2c 7c24 6404 1900 6b00 9004 72aa 7c2c  |,|$d...k...r.|,
-00002fc0: 7c23 6b04 9004 72aa 7c2d 7c2c 7c23 1800  |#k...r.|-|,|#..
-00002fd0: 7c24 6404 1900 7c23 1800 1b00 7c21 1400  |$d...|#....|!..
-00002fe0: 1800 6e02 7c2d 7d2d 7c2c 7c24 6408 1900  ..n.|-}-|,|$d...
-00002ff0: 6b04 9004 72e2 7c2c 7c22 6b00 9004 72e2  k...r.|,|"k...r.
-00003000: 7c2d 7c22 7c2c 1800 7c22 7c24 6408 1900  |-|"|,..|"|$d...
-00003010: 1800 1b00 7c21 1400 1800 6e02 7c2d 7d2d  ....|!....n.|-}-
-00003020: 740b 7c26 7c28 7c29 1700 7c2b 1800 7c2d  t.|&|(|)..|+..|-
-00003030: 1700 7c25 6404 1900 7c06 7c27 1900 6404  ..|%d...|.|'..d.
-00003040: 1900 6602 6602 8302 0100 7401 7c26 8301  ..f.f.....t.|&..
-00003050: 7c1e 6b04 9005 7226 740c 7c26 8301 0100  |.k...r&t.|&....
-00003060: 7c27 6408 3700 7d27 9003 7158 7c26 9003  |'d.7.}'..qX|&..
-00003070: 7242 740c 7c26 8301 7d2e 7c2e 6404 1900  rBt.|&..}.|.d...
-00003080: 740a 6419 8301 6b03 9005 7232 7c1c a008  t.d...k...r2|...
-00003090: 7c2e 6408 1900 6404 1900 7c2e 6408 1900  |.d...d...|.d...
-000030a0: 6408 1900 7c2e 6404 1900 6603 a101 0100  d...|.d...f.....
-000030b0: 9005 7132 9003 7142 7c1b 4400 9002 5d34  ..q2..qB|.D...]4
-000030c0: 7d25 6700 7d26 7c25 6404 1900 6408 1800  }%g.}&|%d...d...
-000030d0: 7d27 7c27 6404 6b05 9007 726e 7c25 6404  }'|'d.k...rn|%d.
-000030e0: 1900 7c05 7c27 1900 6404 1900 1800 7c20  ..|.|'..d.....| 
-000030f0: 6b00 9007 726e 7c05 7c27 1900 6408 1900  k...rn|.|'..d...
-00003100: 7c06 7c25 6404 1900 1900 6408 1900 1700  |.|%d.....d.....
-00003110: 7d28 7c09 7c0c 7c25 6404 1900 1900 7c0c  }(|.|.|%d.....|.
-00003120: 7c05 7c27 1900 6404 1900 1900 1800 1400  |.|'..d.........
-00003130: 7c25 6404 1900 7c05 7c27 1900 6404 1900  |%d...|.|'..d...
-00003140: 1800 1b00 7d29 7c0d 7c25 6404 1900 1900  ....})|.|%d.....
-00003150: 7c0d 7c05 7c27 1900 6404 1900 1900 1800  |.|.|'..d.......
-00003160: 7d2a 7c2a 7c25 6404 1900 7c05 7c27 1900  }*|*|%d...|.|'..
-00003170: 6404 1900 1800 7c1f 1400 6b05 9006 7252  d.....|...k...rR
-00003180: 7c27 6408 3800 7d27 9005 7198 7c09 7c2a  |'d.8.}'..q.|.|*
-00003190: 1400 7c25 6404 1900 7c05 7c27 1900 6404  ..|%d...|.|'..d.
-000031a0: 1900 1800 1b00 7d2b 7c04 7c25 6404 1900  ......}+|.|%d...
-000031b0: 1900 6409 1900 7c04 7c05 7c27 1900 6404  ..d...|.|.|'..d.
-000031c0: 1900 1900 6409 1900 1800 7d2c 7c2c 7c22  ....d.....},|,|"
-000031d0: 6b05 9006 73a6 7c2c 7c23 6b01 9006 72ae  k...s.|,|#k...r.
-000031e0: 740a 6419 8301 6e02 7c21 7d2d 7c2c 7c24  t.d...n.|!}-|,|$
-000031f0: 6404 1900 6b00 9006 72e6 7c2c 7c23 6b04  d...k...r.|,|#k.
-00003200: 9006 72e6 7c2d 7c2c 7c23 1800 7c24 6404  ..r.|-|,|#..|$d.
-00003210: 1900 7c23 1800 1b00 7c21 1400 1800 6e02  ..|#....|!....n.
-00003220: 7c2d 7d2d 7c2c 7c24 6408 1900 6b04 9007  |-}-|,|$d...k...
-00003230: 721e 7c2c 7c22 6b00 9007 721e 7c2d 7c22  r.|,|"k...r.|-|"
-00003240: 7c2c 1800 7c22 7c24 6408 1900 1800 1b00  |,..|"|$d.......
-00003250: 7c21 1400 1800 6e02 7c2d 7d2d 740b 7c26  |!....n.|-}-t.|&
-00003260: 7c28 7c29 1700 7c2b 1800 7c2d 1700 7c05  |(|)..|+..|-..|.
-00003270: 7c27 1900 6404 1900 7c25 6404 1900 6602  |'..d...|%d...f.
-00003280: 6602 8302 0100 7401 7c26 8301 7c1e 6b04  f.....t.|&..|.k.
-00003290: 9007 7262 740c 7c26 8301 0100 7c27 6408  ..rbt.|&....|'d.
-000032a0: 3800 7d27 9005 7198 7c26 9005 7282 740c  8.}'..q.|&..r.t.
-000032b0: 7c26 8301 7d2e 7c2e 6404 1900 740a 6419  |&..}.|.d...t.d.
-000032c0: 8301 6b03 9007 726e 7c1d a008 7c2e 6408  ..k...rn|...|.d.
-000032d0: 1900 6404 1900 7c2e 6408 1900 6408 1900  ..d...|.d...d...
-000032e0: 7c2e 6404 1900 6603 a101 0100 9007 716e  |.d...f.......qn
-000032f0: 9005 7182 7c1c 7c1d 1700 7d2f 7c2f 5300  ..q.|.|...}/|/S.
-00003300: 291a 61f6 0b00 000a 2020 2020 5370 6c69  ).a.....    Spli
-00003310: 7420 7468 6520 6c6f 6e67 2061 6c69 676e  t the long align
-00003320: 6564 2071 7565 7279 2069 6e74 6f20 736d  ed query into sm
-00003330: 616c 6c65 7220 7365 676d 656e 7473 2e0a  aller segments..
-00003340: 0a20 2020 2077 6520 6372 6561 7465 2073  .    we create s
-00003350: 636f 7265 7320 666f 7220 6561 6368 2070  cores for each p
-00003360: 6f73 6974 696f 6e20 696e 2074 6865 2061  osition in the a
-00003370: 6c69 676e 6d65 6e74 2c20 636f 7272 6573  lignment, corres
-00003380: 706f 6e64 696e 6720 746f 2068 6f77 2067  ponding to how g
-00003390: 6f6f 640a 2020 2020 6120 706f 7369 7469  ood.    a positi
-000033a0: 6f6e 2069 7420 6973 2074 6f20 6265 6769  on it is to begi
-000033b0: 6e20 6f72 2065 6e64 2061 2073 706c 6974  n or end a split
-000033c0: 2e0a 0a20 2020 2020 2d20 6265 6769 6e20  ...     - begin 
-000033d0: 6120 7370 6c69 7420 2869 2e65 2e20 7468  a split (i.e. th
-000033e0: 6973 2069 7320 6669 7273 7420 706f 7369  is is first posi
-000033f0: 7469 6f6e 2069 6e20 6120 7365 676d 656e  tion in a segmen
-00003400: 7429 0a20 2020 2020 2020 202d 2070 6c75  t).        - plu
-00003410: 7320 7363 6f72 6520 6571 7561 6c20 746f  s score equal to
-00003420: 206e 756d 2073 696c 656e 6365 2073 6563   num silence sec
-00003430: 6f6e 6473 2074 6869 730a 2020 2020 2020  onds this.      
-00003440: 2020 2020 666f 6c6c 6f77 732c 2075 7020      follows, up 
-00003450: 746f 2073 6f6d 6520 6c69 6d69 7420 3320  to some limit 3 
-00003460: 7365 636f 6e64 732c 2069 2e65 2e20 7468  seconds, i.e. th
-00003470: 6973 2065 6c65 6d65 6e74 0a20 2020 2020  is element.     
-00003480: 2020 2020 206f 6620 7468 6520 5472 616e       of the Tran
-00003490: 7363 7269 7074 2773 2074 696d 6520 6d69  script's time mi
-000034a0: 6e75 7320 7468 6520 7072 6576 696f 7573  nus the previous
-000034b0: 2065 6c65 6d65 6e74 2773 2074 696d 653b   element's time;
-000034c0: 206f 7220 736f 6d65 2064 6566 6175 6c74   or some default
-000034d0: 2028 332e 3020 7365 6329 0a20 2020 2020   (3.0 sec).     
-000034e0: 2020 2020 2069 6620 7468 6973 2069 7320       if this is 
-000034f0: 7468 6520 6669 7273 7420 656c 656d 656e  the first elemen
-00003500: 7420 6f66 2074 6865 2054 7261 6e73 6372  t of the Transcr
-00003510: 6970 742e 0a20 2020 2020 2020 202d 2067  ipt..        - g
-00003520: 6f6f 6420 6966 2074 6865 7265 2061 7265  ood if there are
-00003530: 2066 6577 2065 7272 6f72 7320 6172 6f75   few errors arou
-00003540: 6e64 2074 6869 7320 706f 696e 7420 696e  nd this point in
-00003550: 2074 6865 2061 6c69 676e 6d65 6e74 2c20   the alignment, 
-00003560: 692e 652e 0a20 2020 2020 2020 2020 2073  i.e..          s
-00003570: 636f 7265 2063 6f72 7265 7370 6f6e 6469  core correspondi
-00003580: 6e67 2074 6f20 6e75 6d62 6572 206f 6620  ng to number of 
-00003590: 696e 732c 6465 6c2c 6d69 736d 6174 6368  ins,del,mismatch
-000035a0: 2077 6974 6869 6e20 6120 6365 7274 6169   within a certai
-000035b0: 6e0a 2020 2020 2020 2020 2020 7265 6769  n.          regi
-000035c0: 6f6e 206f 6620 7468 6973 2070 6f73 6974  on of this posit
-000035d0: 696f 6e2e 0a20 2020 2020 2020 202d 2067  ion..        - g
-000035e0: 6f6f 6420 6966 2074 6865 2070 7265 7669  ood if the previ
-000035f0: 6f75 7320 6e6f 6e2d 7768 6974 6573 7061  ous non-whitespa
-00003600: 6365 2063 6861 7261 6374 6572 2077 6173  ce character was
-00003610: 2061 2070 756e 6374 7561 7469 6f6e 0a20   a punctuation. 
-00003620: 2020 2020 2020 2020 2063 6861 7261 6374           charact
-00003630: 6572 2e20 2028 4c69 7374 7320 6f66 2077  er.  (Lists of w
-00003640: 6869 7465 7370 6163 6520 616e 6420 7075  hitespace and pu
-00003650: 6e63 7475 6174 696f 6e20 6368 6172 6163  nctuation charac
-00003660: 7465 7273 2077 696c 6c0a 2020 2020 2020  ters will.      
-00003670: 2020 2020 6265 2070 6173 7365 6420 696e      be passed in
-00003680: 290a 0a20 2020 2020 2d20 656e 6420 6120  )..     - end a 
-00003690: 7370 6c69 7420 2869 2e65 2e20 7468 6973  split (i.e. this
-000036a0: 2069 7320 7468 6520 6c61 7374 2070 6f73   is the last pos
-000036b0: 6974 696f 6e20 696e 2061 2073 6567 6d65  ition in a segme
-000036c0: 6e74 292e 0a20 2020 2020 2020 202d 2070  nt)..        - p
-000036d0: 6c75 7320 7363 6f72 6520 6571 7561 6c20  lus score equal 
-000036e0: 746f 206e 756d 6265 7220 6f66 2073 696c  to number of sil
-000036f0: 656e 6365 2073 6563 6f6e 6473 2066 6f6c  ence seconds fol
-00003700: 6c6f 7773 2074 6869 7320 706f 7369 7469  lows this positi
-00003710: 6f6e 2c20 7570 2074 6f20 736f 6d65 0a20  on, up to some. 
-00003720: 2020 2020 2020 2020 206c 696d 6974 2033           limit 3
-00003730: 2073 6563 6f6e 6473 2c20 692e 6520 6e65   seconds, i.e ne
-00003740: 7874 2065 6c65 6d65 6e74 206f 6620 7468  xt element of th
-00003750: 6520 5472 616e 7363 7269 7074 2773 2074  e Transcript's t
-00003760: 696d 6520 6d69 6e75 7320 7468 6973 2065  ime minus this e
-00003770: 6c65 6d65 6e74 2773 0a20 2020 2020 2020  lement's.       
-00003780: 2020 2074 696d 653b 206f 7220 736f 6d65     time; or some
-00003790: 2064 6566 6175 6c74 2028 332e 3020 7365   default (3.0 se
-000037a0: 6329 2069 6620 7468 6973 2069 7320 7468  c) if this is th
-000037b0: 6520 6c61 7374 2065 6c65 6d65 6e74 206f  e last element o
-000037c0: 6620 7468 6520 5472 616e 7363 7269 7074  f the Transcript
-000037d0: 2e0a 2020 2020 2020 2020 2d20 676f 6f64  ..        - good
-000037e0: 2069 6620 7468 6572 6520 6172 6520 6665   if there are fe
-000037f0: 7720 6572 726f 7273 2061 726f 756e 6420  w errors around 
-00003800: 7468 6973 2070 6f69 6e74 2069 6e20 7468  this point in th
-00003810: 6520 616c 6967 6e6d 656e 742c 2069 2e65  e alignment, i.e
-00003820: 2e0a 2020 2020 2020 2020 2020 7363 6f72  ..          scor
-00003830: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
-00003840: 746f 206e 756d 6265 7220 6f66 2069 6e73  to number of ins
-00003850: 2c64 656c 2c6d 6973 6d61 7463 6820 7769  ,del,mismatch wi
-00003860: 7468 696e 2061 2063 6572 7461 696e 0a20  thin a certain. 
-00003870: 2020 2020 2020 2020 2072 6567 696f 6e20           region 
-00003880: 6f66 2074 6869 7320 706f 7369 7469 6f6e  of this position
-00003890: 2e0a 2020 2020 2020 2020 2d20 676f 6f64  ..        - good
-000038a0: 2069 6620 7468 6520 666f 6c6c 6f77 696e   if the followin
-000038b0: 6720 6e6f 6e2d 7768 6974 6573 7061 6365  g non-whitespace
-000038c0: 2063 6861 7261 6374 6572 2069 7320 6120   character is a 
-000038d0: 7075 6e63 7475 6174 696f 6e20 6368 6172  punctuation char
-000038e0: 6163 7465 722e 0a0a 0a20 2020 2057 6520  acter....    We 
-000038f0: 7468 656e 2063 7265 6174 6520 6120 7275  then create a ru
-00003900: 6c65 2074 6f20 6173 7369 676e 2073 636f  le to assign sco
-00003910: 7265 7320 746f 2070 6f74 656e 7469 616c  res to potential
-00003920: 2073 6567 6d65 6e74 732e 2054 6869 7320   segments. This 
-00003930: 636f 6e73 6973 7420 6f66 0a20 2020 2074  consist of.    t
-00003940: 6865 2062 6567 696e 2d73 636f 7265 732c  he begin-scores,
-00003950: 2070 6c75 7320 7468 6520 656e 642d 7363   plus the end-sc
-00003960: 6f72 6573 2c20 706c 7573 3a0a 2020 2020  ores, plus:.    
-00003970: 2020 2d20 536f 6d65 206b 696e 6420 6f66    - Some kind of
-00003980: 2070 656e 616c 7479 2072 656c 6174 6564   penalty related
-00003990: 2074 6f20 7468 6520 6475 7261 7469 6f6e   to the duration
-000039a0: 206f 6620 7468 6520 7365 676d 656e 742c   of the segment,
-000039b0: 2065 2e67 2e0a 2020 2020 2020 2020 696e   e.g..        in
-000039c0: 6669 6e69 7479 2069 6620 6974 2773 206f  finity if it's o
-000039d0: 7665 7220 736f 6d65 206d 6178 2d64 7572  ver some max-dur
-000039e0: 6174 696f 6e20 6c69 6b65 2033 3020 7365  ation like 30 se
-000039f0: 636f 6e64 7320 6f72 206c 6573 7320 7468  conds or less th
-00003a00: 616e 2061 0a20 2020 2020 2020 206d 696e  an a.        min
-00003a10: 2d64 7572 6174 696f 6e20 6c69 6b65 2032  -duration like 2
-00003a20: 2073 6563 6f6e 6473 3b20 656c 7365 2c20   seconds; else, 
-00003a30: 6f6e 6520 7468 6174 2065 6e63 6f75 7261  one that encoura
-00003a40: 6765 7320 6120 6475 7261 7469 6f6e 2062  ges a duration b
-00003a50: 6574 7765 656e 0a20 2020 2020 2020 2035  etween.        5
-00003a60: 2074 6f20 3230 2073 6563 6f6e 6473 2e0a   to 20 seconds..
-00003a70: 2020 2020 2020 2d20 4120 626f 6e75 7320        - A bonus 
-00003a80: 666f 7220 7468 6520 6e75 6d62 6572 206f  for the number o
-00003a90: 6620 6d61 7463 6865 7320 696e 2074 6865  f matches in the
-00003aa0: 2061 6c69 676e 6d65 6e74 2e0a 2020 2020   alignment..    
-00003ab0: 2020 2d20 4120 7065 6e61 6c74 7920 666f    - A penalty fo
-00003ac0: 7220 7468 6520 6e75 6d62 6572 206f 6620  r the number of 
-00003ad0: 6572 726f 7273 2069 6e20 7468 6520 616c  errors in the al
-00003ae0: 6967 6e6d 656e 7420 2863 6f75 6c64 206d  ignment (could m
-00003af0: 756c 7469 706c 7920 7468 6973 2062 790a  ultiply this by.
-00003b00: 2020 2020 2020 2020 736f 6d65 2073 6361          some sca
-00003b10: 6c65 2064 6570 656e 6469 6e67 2068 6f77  le depending how
-00003b20: 206d 7563 6820 7765 2064 6f6e 2774 2077   much we don't w
-00003b30: 616e 7420 746f 2068 6176 6520 6572 726f  ant to have erro
-00003b40: 7273 2c20 6275 7420 736f 6d65 2065 7272  rs, but some err
-00003b50: 6f72 730a 2020 2020 2020 2020 6172 6520  ors.        are 
-00003b60: 6578 7065 6374 6564 2064 7565 2074 6f20  expected due to 
-00003b70: 626f 7468 2041 5352 2065 7272 6f72 7320  both ASR errors 
-00003b80: 616e 6420 6e6f 726d 616c 697a 6174 696f  and normalizatio
-00003b90: 6e20 6469 6666 6572 656e 6365 732e 290a  n differences.).
-00003ba0: 0a20 2020 204e 6578 742c 2077 6520 6361  .    Next, we ca
-00003bb0: 6e20 646f 2061 2073 6561 7263 6820 666f  n do a search fo
-00003bc0: 7220 6120 676f 6f64 2073 6567 6d65 6e74  r a good segment
-00003bd0: 6174 696f 6e2e 2020 596f 7520 636f 756c  ation.  You coul
-00003be0: 6420 6465 6669 6e65 2074 6865 2070 726f  d define the pro
-00003bf0: 626c 656d 0a20 2020 2061 7320 6765 7474  blem.    as gett
-00003c00: 696e 6720 7468 6520 6869 6768 6573 742d  ing the highest-
-00003c10: 7363 6f72 696e 6720 7365 7420 6f66 2073  scoring set of s
-00003c20: 6567 6d65 6e74 7320 7468 6174 2064 6f20  egments that do 
-00003c30: 6e6f 7420 6f76 6572 6c61 702e 2020 4f6e  not overlap.  On
-00003c40: 650a 2020 2020 706f 7373 6962 6c65 2077  e.    possible w
-00003c50: 6179 2074 6f20 646f 2069 7420 6973 2061  ay to do it is a
-00003c60: 7320 666f 6c6c 6f77 733a 0a20 2020 2020  s follows:.     
-00003c70: 2020 466f 7220 6561 6368 2062 6567 696e    For each begin
-00003c80: 5f70 6f73 6974 696f 6e20 696e 2074 6865  _position in the
-00003c90: 2074 6f70 2031 3025 206f 6620 7363 6f72   top 10% of scor
-00003ca0: 6573 2c20 6669 6e64 2074 6865 2034 2062  es, find the 4 b
-00003cb0: 6573 742d 7363 6f72 696e 6720 656e 645f  est-scoring end_
-00003cc0: 706f 7369 7469 6f6e 730a 2020 2020 2020  positions.      
-00003cd0: 2046 6f72 2065 6163 6820 656e 645f 706f   For each end_po
-00003ce0: 7369 7469 6f6e 2069 6e20 7468 6520 746f  sition in the to
-00003cf0: 7020 3130 2520 6f66 2073 636f 7265 732c  p 10% of scores,
-00003d00: 2066 696e 6420 7468 6520 3420 6265 7374   find the 4 best
-00003d10: 2d73 636f 7269 6e67 2062 6567 696e 5f70  -scoring begin_p
-00003d20: 6f73 6974 696f 6e73 0a20 2020 2041 7070  ositions.    App
-00003d30: 656e 6420 7468 6520 7072 6563 6564 696e  end the precedin
-00003d40: 6720 3220 7365 7473 206f 6620 7365 676d  g 2 sets of segm
-00003d50: 656e 7473 2074 6f20 6765 7420 6120 6c69  ents to get a li
-00003d60: 7374 206f 6620 6361 6e64 6964 6174 6520  st of candidate 
-00003d70: 7365 676d 656e 7473 2e0a 0a20 2020 2041  segments...    A
-00003d80: 7267 733a 0a20 2020 2020 2074 6172 6765  rgs:.      targe
-00003d90: 745f 736f 7572 6365 3a0a 2020 2020 2020  t_source:.      
-00003da0: 2020 4120 5465 7874 536f 7572 6365 2063    A TextSource c
-00003db0: 6f6e 7461 696e 696e 6720 7468 6520 6d61  ontaining the ma
-00003dc0: 7463 6865 6420 7265 6665 7265 6e63 652e  tched reference.
-00003dd0: 0a20 2020 2020 2061 6c69 676e 6d65 6e74  .      alignment
-00003de0: 3a0a 2020 2020 2020 2020 416c 6967 6e6d  :.        Alignm
-00003df0: 656e 7420 696e 666f 726d 6174 696f 6e2c  ent information,
-00003e00: 206f 6e65 2069 7465 6d20 6f66 2074 6865   one item of the
-00003e10: 2072 6574 7572 6e65 6420 616c 6967 6e6d   returned alignm
-00003e20: 656e 7473 2066 726f 6d20 6067 6574 5f61  ents from `get_a
-00003e30: 6c69 676e 6d65 6e74 7360 2e0a 0a20 2020  lignments`...   
-00003e40: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00003e50: 5265 7475 726e 7320 6120 6c69 7374 206f  Returns a list o
-00003e60: 6620 7475 706c 652c 2065 6163 6820 7475  f tuple, each tu
-00003e70: 706c 6520 636f 6e74 6169 6e73 2074 6865  ple contains the
-00003e80: 2073 7461 7274 2070 6f73 6974 696f 6e2c   start position,
-00003e90: 2065 6e64 2070 6f73 6974 696f 6e20 616e   end position an
-00003ea0: 6420 7363 6f72 6520 6f66 0a20 2020 2020  d score of.     
-00003eb0: 2063 7572 7265 6e74 2073 6567 6d65 6e74   current segment
-00003ec0: 2c20 7374 6172 7420 706f 7369 7469 6f6e  , start position
-00003ed0: 2061 6e64 2065 6e64 2070 6f73 6974 696f   and end positio
-00003ee0: 6e20 6172 6520 696e 6465 7865 7320 696e  n are indexes in
-00003ef0: 2061 6c69 676e 732e 0a20 2020 20e9 1400   aligns..    ...
-00003f00: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00003f10: 0000 0005 0000 0053 0000 0073 2400 0000  .......S...s$...
-00003f20: 6700 7c00 5d1c 7d01 7c01 6400 1900 7c01  g.|.].}.|.d...|.
-00003f30: 6401 1900 6b03 721c 6402 6e02 6403 9102  d...k.r.d.n.d...
-00003f40: 7104 5300 2904 7248 0000 0072 4900 0000  q.S.).rH...rI...
-00003f50: 720f 0000 0072 0100 0000 7222 0000 0029  r....r....r"...)
-00003f60: 0272 6100 0000 da05 616c 6967 6e72 2200  .ra.....alignr".
-00003f70: 0000 7222 0000 0072 2300 0000 7263 0000  ..r"...r#...rc..
-00003f80: 0033 0200 0073 0400 0000 0602 02ff 7a2b  .3...s........z+
-00003f90: 5f67 6574 5f73 6567 6d65 6e74 5f63 616e  _get_segment_can
-00003fa0: 6469 6461 7465 732e 3c6c 6f63 616c 733e  didates.<locals>
-00003fb0: 2e3c 6c69 7374 636f 6d70 3e72 0100 0000  .<listcomp>r....
-00003fc0: 7264 0000 0072 4800 0000 7249 0000 0072  rd...rH...rI...r
-00003fd0: 0f00 0000 724c 0000 0072 4a00 0000 5429  ....rL...rJ...T)
-00003fe0: 01da 0865 6f73 5f6f 6e6c 79fa 0120 6301  ...eos_only.. c.
-00003ff0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00004000: 0000 0053 0000 0073 0800 0000 7c00 6401  ...S...s....|.d.
-00004010: 1900 5300 a902 4e72 0f00 0000 7222 0000  ..S...Nr....r"..
-00004020: 00a9 0172 6200 0000 7222 0000 0072 2200  ...rb...r"...r".
-00004030: 0000 7223 0000 00da 083c 6c61 6d62 6461  ..r#.....<lambda
-00004040: 3e8e 0200 00f3 0000 0000 7a29 5f67 6574  >.........z)_get
-00004050: 5f73 6567 6d65 6e74 5f63 616e 6469 6461  _segment_candida
-00004060: 7465 732e 3c6c 6f63 616c 733e 2e3c 6c61  tes.<locals>.<la
-00004070: 6d62 6461 3ea9 02da 036b 6579 da07 7265  mbda>....key..re
-00004080: 7665 7273 6563 0100 0000 0000 0000 0000  versec..........
-00004090: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
-000040a0: 0000 007c 0064 0119 0053 0072 8100 0000  ...|.d...S.r....
-000040b0: 7222 0000 0072 8200 0000 7222 0000 0072  r"...r....r"...r
-000040c0: 2200 0000 7223 0000 0072 8300 0000 8f02  "...r#...r......
-000040d0: 0000 7284 0000 0072 2500 0000 722c 0000  ..r....r%...r,..
-000040e0: 0067 9a99 9999 9999 c93f e9e8 0300 00e9  .g.......?......
-000040f0: 1e00 0000 722a 0000 0029 02e9 0500 0000  ....r*...)......
-00004100: 727d 0000 007a 042d 696e 6629 0dda 0373  r}...z.-inf)...s
-00004110: 756d 7236 0000 00da 0965 6e75 6d65 7261  umr6.....enumera
-00004120: 7465 7258 0000 0072 5700 0000 7254 0000  terX...rW...rT..
-00004130: 0072 1500 0000 721d 0000 0072 2e00 0000  .r....r....r....
-00004140: da06 736f 7274 6564 7256 0000 0072 0400  ..sortedrV...r..
-00004150: 0000 7205 0000 0029 3072 7c00 0000 7243  ..r....)0r|...rC
-00004160: 0000 0072 2f00 0000 7231 0000 0072 5d00  ...r/...r1...r].
-00004170: 0000 5a0c 6265 6769 6e5f 7363 6f72 6573  ..Z.begin_scores
-00004180: 5a0a 656e 645f 7363 6f72 6573 5a10 6861  Z.end_scoresZ.ha
-00004190: 6c66 5f72 6567 696f 6e5f 7369 7a65 5a10  lf_region_sizeZ.
-000041a0: 6572 726f 7273 5f69 6e5f 7265 6769 6f6e  errors_in_region
-000041b0: 5a0a 6261 7365 5f73 636f 7265 5a0b 6d61  Z.base_scoreZ.ma
-000041c0: 785f 7369 6c65 6e63 655a 1170 756e 6374  x_silenceZ.punct
-000041d0: 7561 7469 6f6e 5f73 636f 7265 5a0c 6375  uation_scoreZ.cu
-000041e0: 6d73 756d 5f6d 6174 6368 5a0c 6375 6d73  msum_matchZ.cums
-000041f0: 756d 5f65 7272 6f72 7234 0000 0072 7e00  um_errorr4...r~.
-00004200: 0000 5a07 6d61 7463 6865 645a 0c70 7265  ..Z.matchedZ.pre
-00004210: 765f 7369 6c65 6e63 655a 0c70 6f73 745f  v_silenceZ.post_
-00004220: 7369 6c65 6e63 655a 1070 7265 765f 7075  silenceZ.prev_pu
-00004230: 6e63 7475 6174 696f 6eda 016a da0d 6375  nctuation..j..cu
-00004240: 7272 656e 745f 746f 6b65 6e5a 1070 6f73  rrent_tokenZ.pos
-00004250: 745f 7075 6e63 7475 6174 696f 6e5a 1373  t_punctuationZ.s
-00004260: 6f72 7465 645f 6265 6769 6e5f 7363 6f72  orted_begin_scor
-00004270: 6573 5a11 736f 7274 6564 5f65 6e64 5f73  esZ.sorted_end_s
-00004280: 636f 7265 735a 0974 6f70 5f72 6174 696f  coresZ.top_ratio
-00004290: 5a09 746f 705f 6265 6769 6e5a 0774 6f70  Z.top_beginZ.top
-000042a0: 5f65 6e64 5a0a 6265 6769 6e5f 6c69 7374  _endZ.begin_list
-000042b0: 5a08 656e 645f 6c69 7374 5a14 6e75 6d5f  Z.end_listZ.num_
-000042c0: 6f66 5f62 6573 745f 706f 7369 7469 6f6e  of_best_position
-000042d0: 5a10 6d61 785f 6572 726f 7273 5f72 6174  Z.max_errors_rat
-000042e0: 696f 5a0f 6d61 785f 7465 7874 5f6c 656e  ioZ.max_text_len
-000042f0: 6774 685a 1369 6e69 745f 6475 7261 7469  gthZ.init_durati
-00004300: 6f6e 5f73 636f 7265 5a0c 6d61 785f 6475  on_scoreZ.max_du
-00004310: 7261 7469 6f6e 5a0c 6d69 6e5f 6475 7261  rationZ.min_dura
-00004320: 7469 6f6e 5a11 6578 7065 6374 6564 5f64  tionZ.expected_d
-00004330: 7572 6174 696f 6eda 0469 7465 6d5a 0669  uration..itemZ.i
-00004340: 7465 6d5f 7172 3f00 0000 5a0b 706f 696e  tem_qr?...Z.poin
-00004350: 745f 7363 6f72 655a 0d6d 6174 6368 6564  t_scoreZ.matched
-00004360: 5f73 636f 7265 5a0c 746f 7461 6c5f 6572  _scoreZ.total_er
-00004370: 726f 7273 5a0b 6572 726f 725f 7363 6f72  rorsZ.error_scor
-00004380: 65da 0864 7572 6174 696f 6e5a 0e64 7572  e..durationZ.dur
-00004390: 6174 696f 6e5f 7363 6f72 6572 6200 0000  ation_scorerb...
-000043a0: da0a 6361 6e64 6964 6174 6573 7222 0000  ..candidatesr"..
-000043b0: 0072 2200 0000 7223 0000 00da 175f 6765  .r"...r#....._ge
-000043c0: 745f 7365 676d 656e 745f 6361 6e64 6964  t_segment_candid
-000043d0: 6174 6573 ee01 0000 73ac 0100 0000 3b0c  ates....s.....;.
-000043e0: 0304 0104 0304 0202 0106 020a fe04 ff04  ................
-000043f0: 0a04 0104 0202 ff02 050e 010e 0212 0110  ................
-00004400: 0222 ff06 0426 ff06 050e 020e 010e ff02  ."...&..........
-00004410: ff04 0408 0112 020e 010e ff02 ff04 0408  ................
-00004420: 0424 ff02 0312 030e ff08 0216 fd02 0512  .$..............
-00004430: 0304 010c 010a 010e 010e 0104 0106 0114  ................
-00004440: 010a 0208 0204 010c 010e 010e 010e 0104  ................
-00004450: 0106 0114 010a 0208 0104 0202 010e fe02  ................
-00004460: ff04 0604 0202 010e fe02 ff06 0712 0112  ................
-00004470: 0204 0118 0118 0304 0104 0204 0104 0104  ................
-00004480: 0202 ff02 0304 0104 0104 020a 0304 010c  ................
-00004490: 0128 011c 0302 011a ff02 0212 fe02 ff02  .(..............
-000044a0: 071c 021e 0108 0104 011c 0422 ff02 0606  ..........."....
-000044b0: ff04 0106 ff0c 0202 fd02 0b0a fc04 0406  ................
-000044c0: fc06 0106 010a ff02 0202 fe02 ff04 0502  ................
-000044d0: fa02 0e0a fc04 0406 fc06 0106 010a ff02  ................
-000044e0: 0202 fe02 ff04 0502 fa02 0902 0102 020e  ................
-000044f0: 0206 010a fe02 fe02 fe04 0a0e 0108 010c  ................
-00004500: 0106 0108 0112 012c 020a 0304 010c 0124  .......,.......$
-00004510: 011c 0302 011a ff02 0212 fe02 ff02 071c  ................
-00004520: 021e 0108 0104 011c 0422 ff02 0606 ff04  ........."......
-00004530: 0106 ff0c 0202 fd02 0b0a fc04 0406 fc06  ................
-00004540: 0106 010a ff02 0202 fe02 ff04 0502 fa02  ................
-00004550: 0e0a fc04 0406 fc06 0106 010a ff02 0202  ................
-00004560: fe02 ff04 0502 fa02 0902 0102 020e 020a  ................
-00004570: 0106 fe02 fe02 fe04 0a0e 0108 010c 0106  ................
-00004580: 0108 0112 012c 0208 0172 9300 0000 2903  .....,...r....).
-00004590: 725c 0000 0072 7c00 0000 7219 0000 0063  r\...r|...r....c
-000045a0: 0300 0000 0000 0000 0000 0000 1b00 0000  ................
-000045b0: 0c00 0000 4300 0000 7328 0200 007c 025c  ....C...s(...|.\
-000045c0: 025c 027d 037d 047d 0574 007c 017c 0264  .\.}.}.}.t.|.|.d
-000045d0: 018d 027d 0674 017c 0664 0264 0384 0064  ...}.t.|.d.d...d
-000045e0: 0464 058d 037d 0667 007d 0767 007d 087c  .d...}.g.}.g.}.|
-000045f0: 0644 005d 247d 0974 027c 077c 0964 0619  .D.]$}.t.|.|.d..
-00004600: 007c 0964 0719 0066 0283 0273 367c 08a0  .|.d...f...s6|..
-00004610: 037c 09a1 0101 0071 3667 007d 0a64 087d  .|.....q6g.}.d.}
-00004620: 0b64 097d 0c7c 0844 0090 015d b47d 0d7c  .d.}.|.D...].}.|
-00004630: 057c 0d64 0619 0019 0064 0a19 007d 0e7c  .|.d.....d...}.|
-00004640: 057c 0d64 0719 0019 0064 0a19 0064 0717  .|.d.....d...d..
-00004650: 007d 0f7c 0d64 0619 0064 066b 0272 aa7c  .}.|.d...d.k.r.|
-00004660: 0d64 0619 006e 0a7c 0d64 0619 0064 0718  .d...n.|.d...d..
-00004670: 007d 107c 057c 1019 0064 0b19 007c 057c  .}.|.|...d...|.|
-00004680: 0d64 0619 0019 0064 0b19 0017 0064 0c1b  .d.....d.....d..
-00004690: 007d 117c 0d64 0719 0074 047c 0583 0164  .}.|.d...t.|...d
-000046a0: 0718 006b 0272 f27c 0d64 0719 006e 0a7c  ...k.r.|.d...n.|
-000046b0: 0d64 0719 0064 0717 007d 127c 057c 1219  .d...d...}.|.|..
-000046c0: 0064 0b19 007c 057c 0d64 0719 0019 0064  .d...|.|.d.....d
-000046d0: 0b19 0017 0064 0c1b 007c 1118 007d 137c  .....d...|...}.|
-000046e0: 057c 0d64 0619 0019 0064 0d19 007d 147c  .|.d.....d...}.|
-000046f0: 057c 0d64 0719 0019 0064 0d19 0064 0717  .|.d.....d...d..
-00004700: 007d 1564 0ea0 0564 0f64 1084 007c 006a  .}.d...d.d...|.j
-00004710: 067c 147c 1585 0219 0044 0083 01a1 017d  .|.|.....D.....}
-00004720: 1674 047c 1683 017c 0b6b 0090 0172 7471  .t.|...|.k...rtq
-00004730: 6c64 0ea0 0564 1164 1084 007c 016a 067c  ld...d.d...|.j.|
-00004740: 0e7c 0f64 0717 0085 0219 0044 0083 01a1  .|.d.......D....
-00004750: 017d 177c 0e7c 0c18 0064 066b 0590 0172  .}.|.|...d.k...r
-00004760: ac7c 0e7c 0c18 006e 0264 067d 1864 0ea0  .|.|...n.d.}.d..
-00004770: 0564 1264 1084 007c 016a 067c 187c 0e85  .d.d...|.j.|.|..
-00004780: 0219 0044 0083 01a1 017d 197c 147c 0c18  ...D.....}.|.|..
-00004790: 0064 066b 0490 0172 e47c 147c 0c18 006e  .d.k...r.|.|...n
-000047a0: 0264 067d 1864 0ea0 0564 1364 1084 007c  .d.}.d...d.d...|
-000047b0: 006a 067c 187c 1485 0219 0044 0083 01a1  .j.|.|.....D....
-000047c0: 017d 1a7c 0aa0 037c 0e7c 0f7c 117c 137c  .}.|...|.|.|.|.|
-000047d0: 167c 177c 197c 1a64 149c 08a1 0101 0071  .|.|.|.d.......q
-000047e0: 6c7c 0a53 0029 1561 b302 0000 0a20 2020  l|.S.).a.....   
-000047f0: 2053 706c 6974 2061 206c 6f6e 6720 616c   Split a long al
-00004800: 6967 6e65 6420 7175 6572 7920 696e 746f  igned query into
-00004810: 2073 6d61 6c6c 6572 2073 6567 6d65 6e74   smaller segment
-00004820: 732e 0a0a 2020 2020 5765 2077 696c 6c20  s...    We will 
-00004830: 6372 6561 7465 2073 636f 7265 7320 666f  create scores fo
-00004840: 7220 6561 6368 2070 6f73 6974 696f 6e20  r each position 
-00004850: 696e 2074 6865 2061 6c69 676e 6d65 6e74  in the alignment
-00004860: 2c20 636f 7272 6573 706f 6e64 696e 6720  , corresponding 
-00004870: 746f 2068 6f77 2067 6f6f 640a 2020 2020  to how good.    
-00004880: 6120 706f 7369 7469 6f6e 2069 7420 6973  a position it is
-00004890: 2074 6f20 6265 6769 6e20 6f72 2065 6e64   to begin or end
-000048a0: 2061 2073 706c 6974 2e20 5765 2063 616e   a split. We can
-000048b0: 2074 6865 6e20 6372 6561 7465 2061 2072   then create a r
-000048c0: 756c 6520 746f 2061 7373 6967 6e20 7363  ule to assign sc
-000048d0: 6f72 6573 0a20 2020 2074 6f20 706f 7465  ores.    to pote
-000048e0: 6e74 6961 6c20 7365 676d 656e 7473 2e20  ntial segments. 
-000048f0: 5468 6520 7363 6f72 6573 2077 6f75 6c64  The scores would
-00004900: 2063 6f6e 7369 7374 206f 6620 7468 6520   consist of the 
-00004910: 6265 6769 6e2d 7363 6f72 6573 2c20 706c  begin-scores, pl
-00004920: 7573 2074 6865 2065 6e64 2d73 636f 7265  us the end-score
-00004930: 732c 0a20 2020 2070 6c75 7320 736f 6d65  s,.    plus some
-00004940: 206b 696e 6420 6f66 2073 636f 7265 7320   kind of scores 
-00004950: 6f66 2067 6976 656e 2073 6567 6d65 6e74  of given segment
-00004960: 2028 6475 7261 7469 6f6e 2c20 6d61 7463   (duration, matc
-00004970: 6869 6e67 2065 7272 6f72 7320 2e65 7463  hing errors .etc
-00004980: 292e 0a0a 2020 2020 4172 6773 3a0a 2020  )...    Args:.  
-00004990: 2020 2020 7175 6572 795f 736f 7572 6365      query_source
-000049a0: 3a0a 2020 2020 2020 2020 416e 2069 6e73  :.        An ins
-000049b0: 7461 6e63 6520 6f66 2054 7261 6e73 6372  tance of Transcr
-000049c0: 6970 7420 6f72 2054 6578 7453 6f75 7263  ipt or TextSourc
-000049d0: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
-000049e0: 2071 7565 7279 2e0a 2020 2020 2020 7461   query..      ta
-000049f0: 7267 6574 5f73 6f75 7263 653a 0a20 2020  rget_source:.   
-00004a00: 2020 2020 2041 6e20 696e 7374 616e 6365       An instance
-00004a10: 206f 6620 5465 7874 536f 7572 6365 2063   of TextSource c
-00004a20: 6f6e 7461 696e 696e 6720 7468 6520 6d61  ontaining the ma
-00004a30: 7463 6865 6420 7265 6665 7265 6e63 652e  tched reference.
-00004a40: 0a20 2020 2020 2061 6c69 676e 6d65 6e74  .      alignment
-00004a50: 3a0a 2020 2020 2020 2020 5468 6520 616c  :.        The al
-00004a60: 6967 6e6d 656e 742c 2061 6e20 6974 656d  ignment, an item
-00004a70: 2069 6e20 7468 6520 6c69 7374 2072 6574   in the list ret
-00004a80: 7572 6e65 6420 6279 2060 6765 745f 616c  urned by `get_al
-00004a90: 6967 6e6d 656e 7473 602e 0a20 2020 2029  ignments`..    )
-00004aa0: 0272 7c00 0000 7243 0000 0063 0100 0000  .r|...rC...c....
-00004ab0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00004ac0: 5300 0000 7308 0000 007c 0064 0119 0053  S...s....|.d...S
-00004ad0: 0029 024e 722a 0000 0072 2200 0000 7282  .).Nr*...r"...r.
-00004ae0: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
-00004af0: 0000 7283 0000 004b 0300 0072 8400 0000  ..r....K...r....
-00004b00: 7a25 7370 6c69 745f 696e 746f 5f73 6567  z%split_into_seg
-00004b10: 6d65 6e74 732e 3c6c 6f63 616c 733e 2e3c  ments.<locals>.<
-00004b20: 6c61 6d62 6461 3e54 7285 0000 0072 0100  lambda>Tr....r..
-00004b30: 0000 720f 0000 0072 8900 0000 7288 0000  ..r....r....r...
-00004b40: 0072 4a00 0000 724c 0000 0072 2a00 0000  .rJ...rL...r*...
-00004b50: 724b 0000 0072 4700 0000 6301 0000 0000  rK...rG...c.....
-00004b60: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00004b70: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
-00004b80: 7400 7c01 8301 9102 7104 5300 7222 0000  t.|.....q.S.r"..
-00004b90: 00a9 0172 5700 0000 a902 7261 0000 0072  ...rW.....ra...r
-00004ba0: 3400 0000 7222 0000 0072 2200 0000 7223  4...r"...r"...r#
-00004bb0: 0000 0072 6300 0000 6803 0000 7304 0000  ...rc...h...s...
-00004bc0: 0006 0002 007a 2773 706c 6974 5f69 6e74  .....z'split_int
-00004bd0: 6f5f 7365 676d 656e 7473 2e3c 6c6f 6361  o_segments.<loca
-00004be0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
-00004bf0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00004c00: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
-00004c10: 5d0c 7d01 7400 7c01 8301 9102 7104 5300  ].}.t.|.....q.S.
-00004c20: 7222 0000 0072 9400 0000 7295 0000 0072  r"...r....r....r
-00004c30: 2200 0000 7222 0000 0072 2300 0000 7263  "...r"...r#...rc
-00004c40: 0000 0072 0300 0073 0400 0000 0600 0200  ...r...s........
-00004c50: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00004c60: 0004 0000 0053 0000 0073 1400 0000 6700  .....S...s....g.
-00004c70: 7c00 5d0c 7d01 7400 7c01 8301 9102 7104  |.].}.t.|.....q.
-00004c80: 5300 7222 0000 0072 9400 0000 7295 0000  S.r"...r....r...
-00004c90: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
-00004ca0: 7263 0000 007c 0300 0073 0400 0000 0600  rc...|...s......
-00004cb0: 0200 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00004cc0: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
-00004cd0: 6700 7c00 5d0c 7d01 7400 7c01 8301 9102  g.|.].}.t.|.....
-00004ce0: 7104 5300 7222 0000 0072 9400 0000 7295  q.S.r"...r....r.
-00004cf0: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
-00004d00: 0000 7263 0000 0085 0300 0073 0400 0000  ..rc.......s....
-00004d10: 0600 0200 2908 5a0a 6265 6769 6e5f 6279  ....).Z.begin_by
-00004d20: 7465 5a08 656e 645f 6279 7465 5a0a 7374  teZ.end_byteZ.st
-00004d30: 6172 745f 7469 6d65 7291 0000 0072 4900  art_timer....rI.
-00004d40: 0000 7248 0000 00da 0770 7265 5f72 6566  ..rH.....pre_ref
-00004d50: da07 7072 655f 6879 7029 0772 9300 0000  ..pre_hyp).r....
-00004d60: 728d 0000 0072 1400 0000 722e 0000 0072  r....r....r....r
-00004d70: 3600 0000 da04 6a6f 696e 7254 0000 0029  6.....joinrT...)
-00004d80: 1b72 5c00 0000 727c 0000 0072 4300 0000  .r\...r|...rC...
-00004d90: 722f 0000 0072 3100 0000 725d 0000 0072  r/...r1...r]...r
-00004da0: 9200 0000 5a0f 7365 6c65 6374 6564 5f72  ....Z.selected_r
-00004db0: 616e 6765 7372 3300 0000 da01 7272 7a00  angesr3.....rrz.
-00004dc0: 0000 5a0f 6d69 6e5f 7465 7874 5f6c 656e  ..Z.min_text_len
-00004dd0: 6774 685a 1870 7265 6365 6469 6e67 5f63  gthZ.preceding_c
-00004de0: 6f6e 7465 7874 5f6c 656e 6774 6872 7800  ontext_lengthrx.
-00004df0: 0000 5a09 6265 6769 6e5f 706f 735a 0765  ..Z.begin_posZ.e
-00004e00: 6e64 5f70 6f73 5a0f 7072 6563 6564 696e  nd_posZ.precedin
-00004e10: 675f 696e 6465 78da 0573 7461 7274 5a0f  g_index..startZ.
-00004e20: 666f 6c6c 6f77 696e 675f 696e 6465 7872  following_indexr
-00004e30: 9100 0000 5a0d 6879 705f 6265 6769 6e5f  ....Z.hyp_begin_
-00004e40: 706f 735a 0b68 7970 5f65 6e64 5f70 6f73  posZ.hyp_end_pos
-00004e50: 7249 0000 0072 4800 0000 5a09 7072 655f  rI...rH...Z.pre_
-00004e60: 696e 6465 7872 9600 0000 7297 0000 0072  indexr....r....r
-00004e70: 2200 0000 7222 0000 0072 2300 0000 da13  "...r"...r#.....
-00004e80: 7370 6c69 745f 696e 746f 5f73 6567 6d65  split_into_segme
-00004e90: 6e74 7331 0300 0073 7a00 0000 0013 0c03  nts1...sz.......
-00004ea0: 0201 0200 02ff 0604 1205 0401 0401 0801  ................
-00004eb0: 1601 0c02 0401 0401 0402 0a01 1001 1402  ................
-00004ec0: 2001 2001 2802 1a01 02fe 0202 02fe 0404   . .(...........
-00004ed0: 1001 1401 0401 16ff 0405 0e01 0204 0401  ................
-00004ee0: 1aff 0406 0aff 0c02 02fd 0206 0401 16ff  ................
-00004ef0: 0406 0aff 0c02 02fd 0205 0401 16ff 0404  ................
-00004f00: 0402 0201 0201 0201 0201 0201 0201 0201  ................
-00004f10: 02f8 04ff 060c 729b 0000 00e7 0000 0000  ......r.........
-00004f20: 0000 f83f 2905 725f 0000 00da 0474 6578  ...?).r_.....tex
-00004f30: 74da 0c6c 656e 6774 685f 7261 7469 6fda  t..length_ratio.
-00004f40: 0e6e 756d 5f63 616e 6469 6461 7465 7372  .num_candidatesr
-00004f50: 1900 0000 6304 0000 0000 0000 0000 0000  ....c...........
-00004f60: 0019 0000 0007 0000 0043 0000 0073 0202  .........C...s..
-00004f70: 0000 7c00 6a00 6401 6b02 7314 7401 7c00  ..|.j.d.k.s.t.|.
-00004f80: 6a00 8301 8201 7c00 6a02 5c02 7d04 7d05  j.....|.j.\.}.}.
-00004f90: 7c01 6a03 6a04 7c04 6b04 733a 7401 7c01  |.j.j.|.k.s:t.|.
-00004fa0: 6a03 6a04 7c04 6602 8301 8201 7c01 6a05  j.j.|.f.....|.j.
-00004fb0: 7c04 1900 7d06 7c01 6a06 7d07 6700 7d08  |...}.|.j.}.g.}.
-00004fc0: 7407 7c06 8301 4400 9001 5da4 7d09 7c07  t.|...D...].}.|.
-00004fd0: 7c09 1900 7d0a 7c07 7c09 6402 1700 1900  |...}.|.|.d.....
-00004fe0: 7d0b 7c07 7c09 6402 1700 1900 7c07 7c09  }.|.|.d.....|.|.
-00004ff0: 1900 1800 7d0c 7c0c 7c02 1400 7d0d 7408  ....}.|.|...}.t.
-00005000: a009 7c00 7c0a 7c0b 8502 6403 6403 8502  ..|.|.|...d.d...
-00005010: 6602 1900 a00a a100 a101 7d0e 6404 6701  f.........}.d.g.
-00005020: 7c03 1400 7d0f 6402 7d10 7407 7c0e 6a04  |...}.d.}.t.|.j.
-00005030: 8301 4400 9001 5d22 7d11 7c01 6a05 7c0e  ..D...]"}.|.j.|.
-00005040: 7c11 1900 1900 7d12 7c01 6a0b 7c0e 7c11  |.....}.|.j.|.|.
-00005050: 1900 1900 7d13 7c10 7c0e 6a04 6b00 9001  ....}.|.|.j.k...
-00005060: 7226 7c01 6a05 7c0e 7c10 1900 1900 7c12  r&|.j.|.|.....|.
-00005070: 6b02 9001 7226 7c01 6a0b 7c0e 7c10 1900  k...r&|.j.|.|...
-00005080: 1900 7c13 7c0d 1700 6b00 9001 7226 7c10  ..|.|...k...r&|.
-00005090: 6402 3700 7d10 71e4 7c0e 7c11 1900 7c0e  d.7.}.q.|.|...|.
-000050a0: 7c10 6402 1800 1900 6402 1700 7c10 7c11  |.d.....d...|.|.
-000050b0: 1800 6603 7d14 7c14 6401 1900 7d15 6403  ..f.}.|.d...}.d.
-000050c0: 7d16 6405 7d17 740c 7c0f 8301 4400 5d5a  }.d.}.t.|...D.]Z
-000050d0: 5c02 7d11 7d18 7c18 6401 1900 7c15 6b00  \.}.}.|.d...|.k.
-000050e0: 9001 727e 7c18 6401 1900 7d15 7c11 7d16  ..r~|.d...}.|.}.
-000050f0: 7c14 6406 1900 7c18 6402 1900 6b00 9001  |.d...|.d...k...
-00005100: 725c 7c14 6401 1900 7c18 6401 1900 6b04  r\|.d...|.d...k.
-00005110: 9001 725c 7c14 7c0f 7c11 3c00 6407 7d17  ..r\|.|.|.<.d.}.
-00005120: 0100 9001 71b8 9001 715c 7c17 73c2 740d  ....q...q\|.s.t.
-00005130: 7c0f 8301 7c03 6b00 9001 72d6 7c0f a00e  |...|.k...r.|...
-00005140: 7c14 a101 0100 71c2 7c16 6403 6b09 72c2  |.....q.|.d.k.r.
-00005150: 7c14 7c0f 7c16 3c00 71c2 7c08 a00e 6408  |.|.|.<.q.|...d.
-00005160: 6409 8400 7c0f 4400 8301 a101 0100 7156  d...|.D.......qV
-00005170: 7c08 5300 290a 619f 0300 000a 2020 2020  |.S.).a.....    
-00005180: 4669 6e64 2063 616e 6469 6461 7465 2072  Find candidate r
-00005190: 6567 696f 6e73 2069 6e20 7265 6665 7265  egions in refere
-000051a0: 6e63 6520 646f 6375 6d65 6e74 2074 6861  nce document tha
-000051b0: 7420 636f 756c 6420 6265 2067 6f6f 6420  t could be good 
-000051c0: 6d61 7463 6865 7320 666f 720a 2020 2020  matches for.    
-000051d0: 6561 6368 2071 7565 7279 2064 6f63 756d  each query docum
-000051e0: 656e 742e 0a0a 2020 2020 4172 6773 3a0a  ent...    Args:.
-000051f0: 2020 2020 2020 2063 6c6f 7365 5f6d 6174         close_mat
-00005200: 6368 6573 3a20 616e 206e 702e 6e64 6172  ches: an np.ndar
-00005210: 7261 7920 6f66 2073 6861 7065 2028 746f  ray of shape (to
-00005220: 745f 7175 6572 795f 7379 6d62 6f6c 732c  t_query_symbols,
-00005230: 206e 756d 5f63 6c6f 7365 5f6d 6174 6368   num_close_match
-00005240: 6573 290a 2020 2020 2020 2020 2020 6173  es).          as
-00005250: 2072 6574 7572 6e65 6420 6279 2066 696e   returned by fin
-00005260: 645f 636c 6f73 655f 6d61 7463 6865 7328  d_close_matches(
-00005270: 292c 2069 6e64 6963 6174 696e 6720 7477  ), indicating tw
-00005280: 6f20 636c 6f73 6520 6d61 7463 6865 7320  o close matches 
-00005290: 7769 7468 696e 0a20 2020 2020 2020 2020  within.         
-000052a0: 2074 6865 2072 6566 6572 656e 6365 2074   the reference t
-000052b0: 6578 7420 666f 7220 6561 6368 2073 796d  ext for each sym
-000052c0: 626f 6c20 696e 2074 6865 2071 7565 7279  bol in the query
-000052d0: 2064 6f63 756d 656e 7473 2e0a 2020 2020   documents..    
-000052e0: 2020 2074 6578 743a 2020 5468 6520 536f     text:  The So
-000052f0: 7572 6365 6454 6578 7420 636f 7272 6573  urcedText corres
-00005300: 706f 6e64 696e 6720 746f 2074 6865 2071  ponding to the q
-00005310: 7565 7279 2061 6e64 2072 6566 6572 656e  uery and referen
-00005320: 6365 2064 6f63 756d 656e 7473 0a20 2020  ce documents.   
-00005330: 2020 2020 2020 2063 6f6d 6269 6e65 643b         combined;
-00005340: 206e 6565 6465 6420 666f 7220 6974 7320   needed for its 
-00005350: 6064 6f63 6020 6d65 6d62 6572 2077 6869  `doc` member whi
-00005360: 6368 2063 616e 2062 6520 6173 7375 6d65  ch can be assume
-00005370: 6420 746f 2062 6520 616e 206e 702e 6e64  d to be an np.nd
-00005380: 6172 7261 792e 0a20 2020 2020 2020 6c65  array..       le
-00005390: 6e67 7468 5f72 6174 696f 3a20 696e 6469  ngth_ratio: indi
-000053a0: 6361 7465 7320 7468 6520 6d61 7869 6d75  cates the maximu
-000053b0: 6d20 6361 6e64 6964 6174 652d 7265 6769  m candidate-regi
-000053c0: 6f6e 206c 656e 6774 682c 2077 6869 6368  on length, which
-000053d0: 2077 696c 6c20 6265 2072 6564 7563 6564   will be reduced
-000053e0: 0a20 2020 2020 2020 2020 2069 6620 7468  .          if th
-000053f0: 6520 6d61 7463 6869 6e67 2072 6566 6572  e matching refer
-00005400: 656e 6365 2064 6f63 756d 656e 7420 7761  ence document wa
-00005410: 7320 7368 6f72 7465 7220 7468 616e 2074  s shorter than t
-00005420: 6869 732e 0a20 2020 2020 2020 6e75 6d5f  his..       num_
-00005430: 6361 6e64 6964 6174 6573 3a20 2074 6865  candidates:  the
-00005440: 206e 756d 6265 7220 6f66 2063 616e 6469   number of candi
-00005450: 6461 7465 2072 6567 696f 6e73 2074 6f20  date regions to 
-00005460: 6669 6e64 2066 6f72 2065 6163 6820 7175  find for each qu
-00005470: 6572 790a 2020 2020 2020 2020 2020 646f  ery.          do
-00005480: 6375 6d65 6e74 2e0a 2020 2020 5265 7475  cument..    Retu
-00005490: 726e 733a 0a20 2020 2020 2020 4120 6c69  rns:.       A li
-000054a0: 7374 2c20 6f6e 6520 7065 7220 7175 6572  st, one per quer
-000054b0: 7920 646f 6375 6d65 6e74 2c20 6f66 2063  y document, of c
-000054c0: 6c6f 7365 206d 6174 6368 6573 2c20 7768  lose matches, wh
-000054d0: 6572 6520 6561 6368 2063 6c6f 7365 206d  ere each close m
-000054e0: 6174 6368 0a20 2020 2020 2020 6973 2061  atch.       is a
-000054f0: 2028 6265 6769 6e2c 2065 6e64 2920 706f   (begin, end) po
-00005500: 7369 7469 6f6e 2077 6974 6869 6e20 6074  sition within `t
-00005510: 6578 7460 2e0a 2020 2020 722a 0000 0072  ext`..    r*...r
-00005520: 0f00 0000 4e29 0372 0100 0000 7201 0000  ....N).r....r...
-00005530: 0072 0100 0000 4672 0100 0000 5463 0100  .r....Fr....Tc..
-00005540: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00005550: 0000 5300 0000 731c 0000 0067 007c 005d  ..S...s....g.|.]
-00005560: 147d 017c 0164 0019 007c 0164 0119 0066  .}.|.d...|.d...f
-00005570: 0291 0271 0453 0029 0272 0100 0000 720f  ...q.S.).r....r.
-00005580: 0000 0072 2200 0000 2902 7261 0000 0072  ...r"...).ra...r
-00005590: 3c00 0000 7222 0000 0072 2200 0000 7223  <...r"...r"...r#
-000055a0: 0000 0072 6300 0000 eb03 0000 7304 0000  ...rc.......s...
-000055b0: 0006 0002 007a 2a66 696e 645f 6361 6e64  .....z*find_cand
-000055c0: 6964 6174 655f 6d61 7463 6865 732e 3c6c  idate_matches.<l
-000055d0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000055e0: 3e29 0f72 1b00 0000 721c 0000 0072 6a00  >).r....r....rj.
-000055f0: 0000 7254 0000 0072 1d00 0000 7237 0000  ..rT...r....r7..
-00005600: 0072 3800 0000 722d 0000 0072 1e00 0000  .r8...r-...r....
-00005610: da04 736f 7274 726f 0000 0072 5900 0000  ..sortro...rY...
-00005620: 728c 0000 0072 3600 0000 722e 0000 0029  r....r6...r....)
-00005630: 1972 5f00 0000 729d 0000 0072 9e00 0000  .r_...r....r....
-00005640: 729f 0000 0072 7200 0000 7273 0000 005a  r....rr...rs...Z
-00005650: 0e6e 756d 5f71 7565 7279 5f64 6f63 7372  .num_query_docsr
-00005660: 7400 0000 5a11 6361 6e64 6964 6174 655f  t...Z.candidate_
-00005670: 6d61 7463 6865 7372 7600 0000 5a11 6d61  matchesrv...Z.ma
-00005680: 7463 6865 735f 7374 6172 745f 706f 735a  tches_start_posZ
-00005690: 0f6d 6174 6368 6573 5f65 6e64 5f70 6f73  .matches_end_pos
-000056a0: 5a11 6375 7272 656e 745f 7175 6572 795f  Z.current_query_
-000056b0: 6c65 6e5a 1672 6566 6572 656e 6365 5f63  lenZ.reference_c
-000056c0: 6875 6e6b 5f6c 656e 6774 685a 1563 7572  hunk_lengthZ.cur
-000056d0: 7265 6e74 5f63 6c6f 7365 5f6d 6174 6368  rent_close_match
-000056e0: 6573 5a12 6375 7272 656e 745f 6361 6e64  esZ.current_cand
-000056f0: 6964 6174 6573 728e 0000 0072 3400 0000  idatesr....r4...
-00005700: 5a06 646f 635f 6964 5a06 706f 735f 6964  Z.doc_idZ.pos_id
-00005710: da09 6361 6e64 6964 6174 655a 096d 696e  ..candidateZ.min
-00005720: 5f73 636f 7265 5a09 6d69 6e5f 696e 6465  _scoreZ.min_inde
-00005730: 785a 076f 7665 726c 6170 723c 0000 0072  xZ.overlapr<...r
-00005740: 2200 0000 7222 0000 0072 2300 0000 da16  "...r"...r#.....
-00005750: 6669 6e64 5f63 616e 6469 6461 7465 5f6d  find_candidate_m
-00005760: 6174 6368 6573 9703 0000 736a 0000 0000  atches....sj....
-00005770: 1814 010a 010e 0106 0102 fe06 050a 0206  ................
-00005780: 0204 020e 0108 010c 0114 0108 0204 0116  ................
-00005790: ff04 050a 0104 0110 010e 010e 0208 ff04  ................
-000057a0: 0210 fe04 030c 0106 ff02 fd04 060a 0306  ................
-000057b0: 010e 0106 fd04 0608 0104 0104 0110 010e  ................
-000057c0: 0108 0104 0124 0108 0104 010a 0104 010e  .....$..........
-000057d0: 010c 0208 010a 0116 0172 a200 0000 2902  .........r....).
-000057e0: 7224 0000 0072 2500 0000 2903 7224 0000  r$...r%...).r$..
-000057f0: 0072 2500 0000 4e29 0272 9c00 0000 720f  .r%...N).r....r.
-00005800: 0000 0029 2b72 4f00 0000 da06 6269 7365  ...)+rO.....bise
-00005810: 6374 7202 0000 00da 0b64 6174 6163 6c61  ctr......datacla
-00005820: 7373 6573 7203 0000 00da 0568 6561 7071  ssesr......heapq
-00005830: 7204 0000 0072 0500 0000 5a14 6d75 6c74  r....r....Z.mult
-00005840: 6970 726f 6365 7373 696e 672e 706f 6f6c  iprocessing.pool
-00005850: 7206 0000 00da 0674 7970 696e 6772 0700  r......typingr..
-00005860: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00005870: 0072 0b00 0000 720c 0000 00da 056e 756d  .r....r......num
-00005880: 7079 721e 0000 00da 0b5f 7465 7874 7365  pyr......_textse
-00005890: 6172 6368 720d 0000 0072 2100 0000 720e  archr....r!...r.
-000058a0: 0000 00da 0c73 7566 6669 785f 6172 7261  .....suffix_arra
-000058b0: 7972 1000 0000 da09 6461 7461 7479 7065  yr......datatype
-000058c0: 7372 1100 0000 7212 0000 0072 1300 0000  sr....r....r....
-000058d0: da05 7574 696c 7372 1400 0000 7215 0000  ..utilsr....r...
-000058e0: 0072 1600 0000 da07 6e64 6172 7261 7972  .r......ndarrayr
-000058f0: 5800 0000 7256 0000 0072 4000 0000 da03  X...rV...r@.....
-00005900: 7374 7272 5e00 0000 727b 0000 0072 9300  strr^...r{...r..
-00005910: 0000 729b 0000 0072 a200 0000 7222 0000  ..r....r....r"..
-00005920: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
-00005930: da08 3c6d 6f64 756c 653e 1100 0000 7376  ..<module>....sv
-00005940: 0000 0008 010c 010c 0110 010c 0120 0208  ............. ..
-00005950: 0210 040c 0114 0114 0404 0004 010e fe0c  ................
-00005960: 2600 0100 fc02 0102 010e 0102 0102 0112  &...............
-00005970: fb0c 7f00 3102 000e 0002 0122 fe0c 7800  ....1......"..x.
-00005980: 0100 0100 fb02 0102 0104 0102 0102 0106  ................
-00005990: 0122 fa0c 7f00 0602 0110 fe0c 7f00 7f00  ."..............
-000059a0: 460a 0002 0118 fe0c 6900 0100 fc02 0104  F.......i.......
-000059b0: 0102 0102 0102 0112 fb                   .........
+00000020: 000d 0000 0040 0000 0073 0202 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6406 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
+00000080: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
+00000090: 0100 6400 6401 6c12 5a13 6400 6407 6c14  ..d.d.l.Z.d.d.l.
+000000a0: 6d15 5a16 6d17 5a17 0100 6408 6409 6c18  m.Z.m.Z...d.d.l.
+000000b0: 6d19 5a19 0100 6408 640a 6c1a 6d1b 5a1b  m.Z...d.d.l.m.Z.
+000000c0: 6d1c 5a1c 6d1d 5a1d 0100 6408 640b 6c1e  m.Z.m.Z...d.d.l.
+000000d0: 6d1f 5a1f 6d20 5a20 6d21 5a21 0100 6513  m.Z.m Z m!Z!..e.
+000000e0: 6a22 6513 6a22 650e 6510 6523 6523 6602  j"e.j"e.e.e#e#f.
+000000f0: 1900 1900 640c 9c03 640d 640e 8404 5a15  ....d...d.d...Z.
+00000100: 6424 651b 650e 6510 6523 6523 6602 1900  d$e.e.e.e#e#f...
+00000110: 1900 6523 6524 650e 6510 6523 6523 6523  ..e#e$e.e.e#e#e#
+00000120: 6523 6604 1900 1900 6411 9c05 6412 6413  e#f.....d...d.d.
+00000130: 8405 5a25 651b 650e 650d 6526 650c 6602  ..Z%e.e.e.e&e.f.
+00000140: 1900 1900 6523 650e 6510 6510 6523 6523  ....e#e.e.e.e#e#
+00000150: 6602 1900 650e 650d 6526 650c 6602 1900  f...e.e.e&e.f...
+00000160: 1900 6602 1900 1900 6414 9c04 6415 6416  ..f.....d...d.d.
+00000170: 8404 5a27 6425 651b 6513 6a22 6523 6524  ..Z'd%e.e.j"e#e$
+00000180: 650f 650a 1900 650e 6510 6510 6523 6523  e.e...e.e.e.e#e#
+00000190: 6602 1900 650e 650d 6526 650c 6602 1900  f...e.e.e&e.f...
+000001a0: 1900 6602 1900 1900 6417 9c06 6418 6419  ..f.....d...d.d.
+000001b0: 8405 5a28 651c 650e 6510 6523 6523 6524  ..Z(e.e.e.e#e#e$
+000001c0: 6603 1900 1900 641a 9c02 641b 641c 8404  f.....d...d.d...
+000001d0: 5a29 6511 651d 651c 6602 1900 651c 650e  Z)e.e.e.f...e.e.
+000001e0: 650d 6526 6511 6526 6523 6524 6603 1900  e.e&e.e&e#e$f...
+000001f0: 6602 1900 1900 641d 9c03 641e 641f 8404  f.....d...d.d...
+00000200: 5a2a 6426 6513 6a22 651b 6524 6523 650e  Z*d&e.j"e.e$e#e.
+00000210: 650e 6510 6523 6523 6602 1900 1900 1900  e.e.e#e#f.......
+00000220: 6421 9c05 6422 6423 8405 5a2b 6401 5300  d!..d"d#..Z+d.S.
+00000230: 2927 e900 0000 004e 2901 da0b 6269 7365  )'.....N)...bise
+00000240: 6374 5f6c 6566 7429 01da 0964 6174 6163  ct_left)...datac
+00000250: 6c61 7373 2902 da08 6865 6170 7075 7368  lass)...heappush
+00000260: da07 6865 6170 706f 7029 01da 0a54 6872  ..heappop)...Thr
+00000270: 6561 6450 6f6f 6c29 06da 0341 6e79 da04  eadPool)...Any..
+00000280: 4469 6374 da04 4c69 7374 da08 4f70 7469  Dict..List..Opti
+00000290: 6f6e 616c da05 5475 706c 65da 0555 6e69  onal..Tuple..Uni
+000002a0: 6f6e 2902 da1c 6765 745f 6c6f 6e67 6573  on)...get_longes
+000002b0: 745f 696e 6372 6561 7369 6e67 5f70 6169  t_increasing_pai
+000002c0: 7273 da14 6c65 7665 6e73 6874 6569 6e5f  rs..levenshtein_
+000002d0: 6469 7374 616e 6365 e901 0000 0029 01da  distance.....)..
+000002e0: 1363 7265 6174 655f 7375 6666 6978 5f61  .create_suffix_a
+000002f0: 7272 6179 2903 da0b 536f 7572 6365 6454  rray)...SourcedT
+00000300: 6578 74da 0a54 6578 7453 6f75 7263 65da  ext..TextSource.
+00000310: 0a54 7261 6e73 6372 6970 7429 03da 0a69  .Transcript)...i
+00000320: 735f 6f76 6572 6c61 70da 0e69 735f 7075  s_overlap..is_pu
+00000330: 6e63 7475 6174 696f 6eda 1572 6f77 5f69  nctuation..row_i
+00000340: 6473 5f74 6f5f 726f 775f 7370 6c69 7473  ds_to_row_splits
+00000350: 2903 da04 7365 7131 da04 7365 7132 da06  )...seq1..seq2..
+00000360: 7265 7475 726e 6302 0000 0000 0000 0000  returnc.........
+00000370: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
+00000380: 6e00 0000 7c00 6a00 6401 6b02 7314 7401  n...|.j.d.k.s.t.
+00000390: 7c00 6a00 8301 8201 7c01 6a00 6401 6b02  |.j.....|.j.d.k.
+000003a0: 7328 7401 7c01 6a00 8301 8201 7c00 6a02  s(t.|.j.....|.j.
+000003b0: 7c01 6a02 6b02 7344 7401 7c00 6a02 7c01  |.j.k.sDt.|.j.|.
+000003c0: 6a02 6602 8301 8201 7403 6a04 7c00 7403  j.f.....t.j.|.t.
+000003d0: 6a05 6402 8d02 7d02 7403 6a04 7c01 7403  j.d...}.t.j.|.t.
+000003e0: 6a05 6402 8d02 7d03 7406 7c02 7c03 8302  j.d...}.t.|.|...
+000003f0: 5300 2903 6117 0300 000a 2020 2020 4765  S.).a.....    Ge
+00000400: 7420 7468 6520 6c6f 6e67 6573 7420 696e  t the longest in
+00000410: 6372 6561 7369 6e67 2070 6169 7273 2066  creasing pairs f
+00000420: 6f72 2067 6976 656e 2073 6571 7565 6e63  or given sequenc
+00000430: 6573 2e0a 2020 2020 5365 6520 6874 7470  es..    See http
+00000440: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000450: 616e 706f 7665 792f 7465 7874 5f73 6561  anpovey/text_sea
+00000460: 7263 682f 6973 7375 6573 2f32 3120 666f  rch/issues/21 fo
+00000470: 7220 6d6f 7265 2064 6574 6169 6c73 2e0a  r more details..
+00000480: 0a20 2020 2053 7570 706f 7365 2073 6571  .    Suppose seq
+00000490: 3120 6973 205b 6931 2c20 6932 2c20 6933  1 is [i1, i2, i3
+000004a0: 2e2e 2e20 694e 5d20 616e 6420 7365 7132  ... iN] and seq2
+000004b0: 2069 7320 5b6a 312c 206a 322c 206a 332e   is [j1, j2, j3.
+000004c0: 2e2e 206a 4e5d 2c20 7468 6973 0a20 2020  .. jN], this.   
+000004d0: 2066 756e 6374 696f 6e20 7265 7475 726e   function return
+000004e0: 7320 7468 6520 206c 6f6e 6765 7374 2069  s the  longest i
+000004f0: 6e63 7265 6173 696e 6720 7061 6972 733a  ncreasing pairs:
+00000500: 2028 6931 2c20 6a31 292c 2028 6932 2c20   (i1, j1), (i2, 
+00000510: 6a32 292c 202e 2e2e 2028 694e 2c20 6a4e  j2), ... (iN, jN
+00000520: 290a 2020 2020 7375 6368 2074 6861 7420  ).    such that 
+00000530: 6931 203c 3d20 6932 203c 3d20 2e2e 2e20  i1 <= i2 <= ... 
+00000540: 3c3d 2069 4e2c 2061 6e64 206a 3120 3c3d  <= iN, and j1 <=
+00000550: 206a 3220 3c3d 202e 2e2e 203c 3d20 6a4e   j2 <= ... <= jN
+00000560: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00000570: 2020 2073 6571 313a 0a20 2020 2020 2020     seq1:.       
+00000580: 2054 6865 2066 6972 7374 2073 6571 7565   The first seque
+00000590: 6e63 652e 0a20 2020 2020 2073 6571 323a  nce..      seq2:
+000005a0: 0a20 2020 2020 2020 2054 6865 2073 6563  .        The sec
+000005b0: 6f6e 6420 7365 7175 656e 6365 2e0a 0a20  ond sequence... 
+000005c0: 2020 203e 3e3e 2069 6d70 6f72 7420 6e75     >>> import nu
+000005d0: 6d70 7920 6173 206e 700a 2020 2020 3e3e  mpy as np.    >>
+000005e0: 3e20 6672 6f6d 2074 6578 7473 6561 7263  > from textsearc
+000005f0: 6820 696d 706f 7274 2067 6574 5f6c 6f6e  h import get_lon
+00000600: 6765 7374 5f69 6e63 7265 6173 696e 675f  gest_increasing_
+00000610: 7061 6972 730a 2020 2020 3e3e 3e20 7365  pairs.    >>> se
+00000620: 7131 203d 206e 702e 6172 7261 7928 5b30  q1 = np.array([0
+00000630: 2c20 312c 2031 2c20 322c 2032 2c20 332c  , 1, 1, 2, 2, 3,
+00000640: 2034 2c20 352c 2036 5d2c 2064 7479 7065   4, 5, 6], dtype
+00000650: 3d6e 702e 696e 7433 3229 0a20 2020 203e  =np.int32).    >
+00000660: 3e3e 2073 6571 3220 3d20 6e70 2e61 7272  >> seq2 = np.arr
+00000670: 6179 285b 392c 2037 2c20 382c 2039 2c20  ay([9, 7, 8, 9, 
+00000680: 362c 2037 2c20 3130 2c20 3132 2c20 385d  6, 7, 10, 12, 8]
+00000690: 2c20 6474 7970 653d 6e70 2e69 6e74 3634  , dtype=np.int64
+000006a0: 290a 2020 2020 3e3e 3e20 6765 745f 6c6f  ).    >>> get_lo
+000006b0: 6e67 6573 745f 696e 6372 6561 7369 6e67  ngest_increasing
+000006c0: 5f70 6169 7273 2873 6571 313d 7365 7131  _pairs(seq1=seq1
+000006d0: 2c20 7365 7132 3d73 6571 3229 0a20 2020  , seq2=seq2).   
+000006e0: 205b 2831 2c20 3729 2c20 2831 2c20 3829   [(1, 7), (1, 8)
+000006f0: 2c20 2832 2c20 3929 2c20 2834 2c20 3130  , (2, 9), (4, 10
+00000700: 292c 2028 352c 2031 3229 5d0a 2020 2020  ), (5, 12)].    
+00000710: 720f 0000 0029 01da 0564 7479 7065 2907  r....)...dtype).
+00000720: da04 6e64 696d da0e 4173 7365 7274 696f  ..ndim..Assertio
+00000730: 6e45 7272 6f72 da04 7369 7a65 da02 6e70  nError..size..np
+00000740: da11 6173 636f 6e74 6967 756f 7573 6172  ..ascontiguousar
+00000750: 7261 79da 0569 6e74 3332 da1d 5f67 6574  ray..int32.._get
+00000760: 5f6c 6f6e 6765 7374 5f69 6e63 7265 6173  _longest_increas
+00000770: 696e 675f 7061 6972 7329 0472 1700 0000  ing_pairs).r....
+00000780: 7218 0000 005a 0a73 6571 315f 696e 7433  r....Z.seq1_int3
+00000790: 325a 0a73 6571 325f 696e 7433 32a9 0072  2Z.seq2_int32..r
+000007a0: 2200 0000 fa47 2f63 6570 682d 6b77 2f6b  "....G/ceph-kw/k
+000007b0: 616e 6777 6569 2f63 6f64 652f 7465 7874  angwei/code/text
+000007c0: 5f73 6561 7263 682f 7465 7874 7365 6172  _search/textsear
+000007d0: 6368 2f70 7974 686f 6e2f 7465 7874 7365  ch/python/textse
+000007e0: 6172 6368 2f6d 6174 6368 2e70 7972 0d00  arch/match.pyr..
+000007f0: 0000 2400 0000 730c 0000 0000 1814 0114  ..$...s.........
+00000800: 011c 0310 0110 0272 0d00 0000 e988 1300  .......r........
+00000810: 00e7 9a99 9999 9999 b93f 2905 da0c 736f  .........?)...so
+00000820: 7572 6365 645f 7465 7874 da0e 6d61 7463  urced_text..matc
+00000830: 6865 645f 706f 696e 7473 da0e 7365 676d  hed_points..segm
+00000840: 656e 745f 6c65 6e67 7468 da1b 7265 6665  ent_length..refe
+00000850: 7265 6e63 655f 6c65 6e67 7468 5f64 6966  rence_length_dif
+00000860: 6665 7265 6e63 6572 1900 0000 6304 0000  ferencer....c...
+00000870: 0000 0000 0000 0000 001c 0000 0008 0000  ................
+00000880: 0043 0000 0073 2803 0000 6401 7d04 6700  .C...s(...d.}.g.
+00000890: 7d05 7400 6402 7401 7c01 8301 8302 4400  }.t.d.t.|.....D.
+000008a0: 5db6 7d06 7c01 7c06 1900 6401 1900 7c01  ].}.|.|...d...|.
+000008b0: 7c06 6402 1800 1900 6401 1900 1800 7c01  |.d.....d.....|.
+000008c0: 7c06 1900 6402 1900 7c01 7c06 6402 1800  |...d...|.|.d...
+000008d0: 1900 6402 1900 1800 6602 7d07 7c07 6401  ..d.....f.}.|.d.
+000008e0: 1900 7c07 6402 1900 6b00 7216 7c01 7c06  ..|.d...k.r.|.|.
+000008f0: 1900 6402 1900 7c01 7c04 1900 6402 1900  ..d...|.|...d...
+00000900: 1800 6402 1700 7c01 7c06 1900 6401 1900  ..d...|.|...d...
+00000910: 7c01 7c04 1900 6401 1900 1800 6402 1700  |.|...d.....d...
+00000920: 1b00 7d08 7c03 6403 1b00 7d09 7c08 6402  ..}.|.d...}.|.d.
+00000930: 7c09 1800 6b00 73ba 7c08 6402 7c09 1700  |...k.s.|.d.|...
+00000940: 6b04 7216 7c05 a002 7c04 7c06 6602 a101  k.r.|...|.|.f...
+00000950: 0100 7c06 7d04 7116 7c05 a002 7c04 7401  ..|.}.q.|...|.t.
+00000960: 7c01 8301 6602 a101 0100 6404 7d0a 6401  |...f.....d.}.d.
+00000970: 7401 7c01 8301 6602 7d0b 7c05 4400 5d38  t.|...f.}.|.D.]8
+00000980: 7d0c 7c01 7c0c 6402 1900 6402 1800 1900  }.|.|.d...d.....
+00000990: 6401 1900 7c01 7c0c 6401 1900 1900 6401  d...|.|.d.....d.
+000009a0: 1900 1800 7d0d 7c0d 7c0a 6b04 72f4 7c0d  ....}.|.|.k.r.|.
+000009b0: 7d0a 7c0c 7d0b 71f4 6700 7d0e 6405 6406  }.|.}.q.g.}.d.d.
+000009c0: 8400 7d0f 7c00 6a03 7c01 7c0b 6401 1900  ..}.|.j.|.|.d...
+000009d0: 1900 6402 1900 1900 7d10 7c00 6a04 7c10  ..d.....}.|.j.|.
+000009e0: 1900 7d11 7c00 6a04 7c10 6402 1700 1900  ..}.|.j.|.d.....
+000009f0: 7d12 7c00 6a03 7c01 7c0b 6401 1900 1900  }.|.j.|.|.d.....
+00000a00: 6401 1900 1900 7d13 7c00 6a04 7c13 1900  d.....}.|.j.|...
+00000a10: 7d14 7c00 6a04 7c13 6402 1700 1900 7d15  }.|.j.|.d.....}.
+00000a20: 7c01 7c0b 6401 1900 1900 6402 1900 7c01  |.|.d.....d...|.
+00000a30: 7c0b 6401 1900 1900 6401 1900 7c14 1800  |.d.....d...|...
+00000a40: 1800 7d16 7c14 7c16 7c11 6b05 9001 72ca  ..}.|.|.|.k...r.
+00000a50: 7c16 6e02 7c11 6602 7d04 7400 7c0b 6401  |.n.|.f.}.t.|.d.
+00000a60: 1900 7c0b 6402 1900 8302 4400 5db6 7d17  ..|.d.....D.].}.
+00000a70: 7c01 7c17 1900 6401 1900 7c04 6401 1900  |.|...d...|.d...
+00000a80: 1800 7c02 6b04 9001 72e2 7c17 7c0b 6401  ..|.k...r.|.|.d.
+00000a90: 1900 6b02 9002 7214 9001 71e2 6e82 7c04  ..k...r...q.n.|.
+00000aa0: 6401 1900 7d18 7c01 7c17 6402 1800 1900  d...}.|.|.d.....
+00000ab0: 6401 1900 7d19 7c04 6402 1900 7d1a 7c01  d...}.|.d...}.|.
+00000ac0: 7c17 6402 1800 1900 6402 1900 7d1b 7c1b  |.d.....d...}.|.
+00000ad0: 7c1a 1800 7c19 7c18 1800 1b00 7d08 7c03  |...|.|.....}.|.
+00000ae0: 6403 1b00 7d09 7c08 6402 7c09 1800 6b00  d...}.|.d.|...k.
+00000af0: 9001 73e2 7c08 6402 7c09 1700 6b04 9002  ..s.|.d.|...k...
+00000b00: 727c 9001 71e2 7c19 7c1b 6602 7d04 7c0f  r|..q.|.|.f.}.|.
+00000b10: 7c18 7c19 7c1a 7c1b 7c02 7c0e 8306 0100  |.|.|.|.|.|.....
+00000b20: 9001 71e2 7c04 5c02 7d18 7d1a 7c15 7d19  ..q.|.\.}.}.|.}.
+00000b30: 7c1a 7c19 7c18 1800 1700 7d1b 7c1b 7c12  |.|.|.....}.|.|.
+00000b40: 6b01 9002 72c0 7c1b 6e02 7c12 7d1b 7c19  k...r.|.n.|.}.|.
+00000b50: 7c18 1800 7c02 6407 1a00 6b00 9003 7212  |...|.d...k...r.
+00000b60: 7c0e 9002 72fe 7c0e 6404 1900 6401 1900  |...r.|.d...d...
+00000b70: 7c19 7c0e 6404 1900 6403 1900 7c1b 6604  |.|.d...d...|.f.
+00000b80: 7c0e 6404 3c00 6e12 7c0e a002 7c18 7c19  |.d.<.n.|...|.|.
+00000b90: 7c1a 7c1b 6604 a101 0100 6e12 7c0f 7c18  |.|.f.....n.|.|.
+00000ba0: 7c19 7c1a 7c1b 7c02 7c0e 8306 0100 7c0e  |.|.|.|.|.....|.
+00000bb0: 5300 2908 618b 0300 000a 2020 2020 4272  S.).a.....    Br
+00000bc0: 6561 6b20 6c6f 6e67 2071 7565 7279 2069  eak long query i
+00000bd0: 6e74 6f20 736d 616c 6c20 7365 676d 656e  nto small segmen
+00000be0: 7473 2061 7420 7468 6520 6d61 7463 6865  ts at the matche
+00000bf0: 6420 706f 696e 7473 2077 6974 6820 7468  d points with th
+00000c00: 6520 6073 6567 6d65 6e74 5f6c 656e 6774  e `segment_lengt
+00000c10: 6860 0a20 2020 2063 6f6e 7374 7261 696e  h`.    constrain
+00000c20: 742e 0a0a 2020 2020 4172 6773 3a0a 2020  t...    Args:.  
+00000c30: 2020 2020 736f 7572 6365 645f 7465 7874      sourced_text
+00000c40: 3a0a 2020 2020 2020 2020 5468 6520 536f  :.        The So
+00000c50: 7572 6365 6454 6578 7420 636f 6e74 6169  urcedText contai
+00000c60: 6e69 6e67 2074 6865 2071 7565 7269 6573  ning the queries
+00000c70: 2061 6e64 2072 6566 6572 656e 6365 732e   and references.
+00000c80: 0a20 2020 2020 206d 6174 6368 6564 5f70  .      matched_p
+00000c90: 6f69 6e74 733a 0a20 2020 2020 2020 2041  oints:.        A
+00000ca0: 206c 6973 7420 6f66 206d 6174 6368 6564   list of matched
+00000cb0: 2070 6f69 6e74 732c 2065 6163 6820 6974   points, each it
+00000cc0: 656d 2069 7320 6120 7061 6972 206f 6620  em is a pair of 
+00000cd0: 2871 7565 7279 2069 6e64 6578 2c20 7461  (query index, ta
+00000ce0: 7267 6574 2069 6e64 6578 290a 2020 2020  rget index).    
+00000cf0: 2020 2020 696e 2073 6f75 7263 6564 5f74      in sourced_t
+00000d00: 6578 742e 0a20 2020 2020 2073 6567 6d65  ext..      segme
+00000d10: 6e74 5f6c 656e 6774 683a 0a20 2020 2020  nt_length:.     
+00000d20: 2020 2054 6865 2065 7870 6563 7465 6420     The expected 
+00000d30: 6c65 6e67 7468 206f 6620 7468 6520 7365  length of the se
+00000d40: 676d 656e 7465 6420 7069 6563 652e 204e  gmented piece. N
+00000d50: 6f74 653a 2074 6869 7320 6973 206e 6f74  ote: this is not
+00000d60: 2072 6561 6c6c 7920 7468 650a 2020 2020   really the.    
+00000d70: 2020 2020 6c65 6e67 7468 206f 6620 7468      length of th
+00000d80: 6520 7365 676d 656e 7473 2c20 7468 6520  e segments, the 
+00000d90: 7365 676d 656e 7420 6c65 6e67 7468 206d  segment length m
+00000da0: 6967 6874 2062 6520 6120 6c69 7474 6c65  ight be a little
+00000db0: 206c 6f6e 6765 720a 2020 2020 2020 2020   longer.        
+00000dc0: 7468 616e 2060 7365 676d 656e 745f 6c65  than `segment_le
+00000dd0: 6e67 7468 602c 206c 696b 6520 6073 6567  ngth`, like `seg
+00000de0: 6d65 6e74 5f6c 656e 6774 6860 202a 2031  ment_length` * 1
+00000df0: 2e32 350a 2020 2020 2020 7265 6665 7265  .25.      refere
+00000e00: 6e63 655f 6c65 6e67 7468 5f64 6966 6665  nce_length_diffe
+00000e10: 7265 6e63 653a 0a20 2020 2020 2020 2042  rence:.        B
+00000e20: 6563 6175 7365 206f 6620 7468 6520 696e  ecause of the in
+00000e30: 7365 7274 696f 6e20 6f72 2064 656c 6574  sertion or delet
+00000e40: 696f 6e20 6572 726f 7273 2c20 7468 6520  ion errors, the 
+00000e50: 7265 6665 7265 6e63 6520 7365 7175 656e  reference sequen
+00000e60: 6365 206d 6967 6874 2062 650a 2020 2020  ce might be.    
+00000e70: 2020 2020 7368 6f72 7465 7220 6f72 206c      shorter or l
+00000e80: 6f6e 6765 7220 7468 616e 2074 6865 2071  onger than the q
+00000e90: 7565 7279 2c20 736f 2074 6865 2072 6566  uery, so the ref
+00000ea0: 6572 656e 6365 2073 6567 6d65 6e74 206c  erence segment l
+00000eb0: 656e 6774 6820 6361 6e20 6265 2066 726f  ength can be fro
+00000ec0: 6d0a 2020 2020 2020 2020 606c 656e 2871  m.        `len(q
+00000ed0: 7565 7279 2920 2a20 2831 202d 2072 6566  uery) * (1 - ref
+00000ee0: 6572 656e 6365 5f6c 656e 6774 685f 6469  erence_length_di
+00000ef0: 6666 6572 656e 6365 202f 2032 2960 2074  fference / 2)` t
+00000f00: 6f0a 2020 2020 2020 2020 606c 656e 2871  o.        `len(q
+00000f10: 7565 7279 2920 2a20 2831 202b 2072 6566  uery) * (1 + ref
+00000f20: 6572 656e 6365 5f6c 656e 6774 685f 6469  erence_length_di
+00000f30: 6666 6572 656e 6365 202f 2032 2960 2e0a  fference / 2)`..
+00000f40: 2020 2020 7201 0000 0072 0f00 0000 e902      r....r......
+00000f50: 0000 00e9 ffff ffff 6306 0000 0000 0000  ........c.......
+00000f60: 0000 0000 0009 0000 0007 0000 0053 0000  .............S..
+00000f70: 0073 ac00 0000 7c01 7c00 1800 7c04 1a00  .s....|.|...|...
+00000f80: 7d06 7c06 6401 6b04 7260 7400 7c06 8301  }.|.d.k.r`t.|...
+00000f90: 4400 5d42 7d07 7c02 7c04 1700 7c03 6b00  D.]B}.|.|...|.k.
+00000fa0: 7234 7c02 7c04 1700 6e02 7c03 7d08 7c05  r4|.|...n.|.}.|.
+00000fb0: a001 7c00 7c00 7c04 1700 7c02 7c08 6604  ..|.|.|...|.|.f.
+00000fc0: a101 0100 7c00 7c04 3700 7d00 7c02 7c04  ....|.|.7.}.|.|.
+00000fd0: 3700 7d02 711c 7c05 7296 7c01 7c00 1800  7.}.q.|.r.|.|...
+00000fe0: 7c04 6402 1a00 6b00 7296 7c05 6403 1900  |.d...k.r.|.d...
+00000ff0: 6401 1900 7c01 7c05 6403 1900 6404 1900  d...|.|.d...d...
+00001000: 7c03 6604 7c05 6403 3c00 6e12 7c05 a001  |.f.|.d.<.n.|...
+00001010: 7c00 7c01 7c02 7c03 6604 a101 0100 6400  |.|.|.|.f.....d.
+00001020: 5300 2905 4e72 0100 0000 e904 0000 0072  S.).Nr.........r
+00001030: 2b00 0000 722a 0000 0029 02da 0572 616e  +...r*...)...ran
+00001040: 6765 da06 6170 7065 6e64 2909 da0b 7175  ge..append)...qu
+00001050: 6572 795f 7374 6172 74da 0971 7565 7279  ery_start..query
+00001060: 5f65 6e64 da0c 7461 7267 6574 5f73 7461  _end..target_sta
+00001070: 7274 da0a 7461 7267 6574 5f65 6e64 7228  rt..target_endr(
+00001080: 0000 00da 0873 6567 6d65 6e74 735a 096e  .....segmentsZ.n
+00001090: 756d 5f63 6875 6e6b da01 695a 0f72 6561  um_chunk..iZ.rea
+000010a0: 6c5f 7461 7267 6574 5f65 6e64 7222 0000  l_target_endr"..
+000010b0: 0072 2200 0000 7223 0000 00da 0c61 6464  .r"...r#.....add
+000010c0: 5f73 6567 6d65 6e74 7389 0000 0073 2800  _segments....s(.
+000010d0: 0000 0003 0c01 0801 0c01 1801 0402 0201  ................
+000010e0: 0601 0201 02fc 02ff 0408 0801 0a03 1402  ................
+000010f0: 0a01 0201 0a01 02fc 0a07 7a22 5f62 7265  ..........z"_bre
+00001100: 616b 5f71 7565 7279 2e3c 6c6f 6361 6c73  ak_query.<locals
+00001110: 3e2e 6164 645f 7365 676d 656e 7473 722c  >.add_segmentsr,
+00001120: 0000 0029 0572 2d00 0000 da03 6c65 6e72  ...).r-.....lenr
+00001130: 2e00 0000 da03 646f 63da 0a64 6f63 5f73  ......doc..doc_s
+00001140: 706c 6974 7329 1c72 2600 0000 7227 0000  plits).r&...r'..
+00001150: 0072 2800 0000 7229 0000 005a 1070 7265  .r(...r)...Z.pre
+00001160: 765f 6272 6561 6b5f 706f 696e 745a 1063  v_break_pointZ.c
+00001170: 616e 6469 6461 7465 5f72 616e 6765 7372  andidate_rangesr
+00001180: 3400 0000 da03 6761 70da 0572 6174 696f  4.....gap..ratio
+00001190: da04 6861 6c66 da0a 6d61 785f 6c65 6e67  ..half..max_leng
+000011a0: 7468 5a08 6d61 785f 6974 656d da01 635a  thZ.max_item..cZ
+000011b0: 0e63 7572 7265 6e74 5f6c 656e 6774 6872  .current_lengthr
+000011c0: 3300 0000 7235 0000 005a 0d74 6172 6765  3...r5...Z.targe
+000011d0: 745f 646f 635f 6964 5a0b 7461 7267 6574  t_doc_idZ.target
+000011e0: 5f62 6173 655a 106e 6578 745f 7461 7267  _baseZ.next_targ
+000011f0: 6574 5f62 6173 65da 0c71 7565 7279 5f64  et_base..query_d
+00001200: 6f63 5f69 64da 0a71 7565 7279 5f62 6173  oc_id..query_bas
+00001210: 655a 0f6e 6578 745f 7175 6572 795f 6261  eZ.next_query_ba
+00001220: 7365 5a0b 7072 6576 5f74 6172 6765 74da  seZ.prev_target.
+00001230: 0369 6e64 722f 0000 0072 3000 0000 7231  .indr/...r0...r1
+00001240: 0000 0072 3200 0000 7222 0000 0072 2200  ...r2...r"...r".
+00001250: 0000 7223 0000 00da 0c5f 6272 6561 6b5f  ..r#....._break_
+00001260: 7175 6572 7947 0000 0073 9c00 0000 001d  queryG...s......
+00001270: 0401 0401 1204 1a01 1afe 0404 1002 1a01  ................
+00001280: 1aff 0405 0801 1801 0e01 0602 1204 0401  ................
+00001290: 0c01 0801 2401 0801 0401 0604 0402 081d  ....$...........
+000012a0: 1601 0a01 0e02 1601 0a01 0e04 0e01 12ff  ................
+000012b0: 0404 0201 10fe 0408 1601 1a01 0e01 0602  ................
+000012c0: 0801 1001 0801 1002 1001 0801 1c01 0402  ................
+000012d0: 0801 0201 0201 0201 0201 0201 0201 02fa  ................
+000012e0: 0809 0801 0402 0c01 1202 1201 0602 0a01  ................
+000012f0: 0201 0a01 02fc 0a07 1402 0201 0200 0200  ................
+00001300: 0200 0200 0200 02ff 0403 7241 0000 0029  ..........rA...)
+00001310: 0472 2600 0000 da0e 7375 625f 616c 6967  .r&.....sub_alig
+00001320: 6e6d 656e 7473 da0b 6e75 6d5f 7175 6572  nments..num_quer
+00001330: 6965 7372 1900 0000 6303 0000 0000 0000  iesr....c.......
+00001340: 0000 0000 001d 0000 000a 0000 0043 0000  .............C..
+00001350: 0073 c402 0000 6401 6701 7c02 1400 7d03  .s....d.g.|...}.
+00001360: 6402 7d04 7c01 4400 9002 5daa 7d05 7c05  d.}.|.D...].}.|.
+00001370: 6403 1900 6402 1900 6404 6b02 7234 7400  d...d...d.k.r4t.
+00001380: a001 6405 a101 0100 7112 7c05 6403 1900  ..d.....q.|.d...
+00001390: 6406 1900 6402 1900 5c03 7d06 7d07 7d08  d...d...\.}.}.}.
+000013a0: 7c05 6407 1900 5c04 7d09 7d0a 7d0b 7d0c  |.d...\.}.}.}.}.
+000013b0: 7c06 6402 6b02 736a 7402 7c06 8301 8201  |.d.k.sjt.|.....
+000013c0: 7c0c 7c0b 7c07 1700 6406 1700 6b02 738e  |.|.|...d...k.s.
+000013d0: 7402 7c0c 7c0b 7c07 1700 6406 1700 6602  t.|.|.|...d...f.
+000013e0: 8301 8201 7c00 6a03 7c09 1900 7d0d 7c03  ....|.j.|...}.|.
+000013f0: 7c0d 1900 6401 6b08 72b8 7c09 7c0b 7c06  |...d.k.r.|.|.|.
+00001400: 1700 6602 6700 6602 7c03 7c0d 3c00 7c00  ..f.g.f.|.|.<.|.
+00001410: 6a03 7c09 1900 7d0e 7c00 6a04 7c0e 1900  j.|...}.|.j.|...
+00001420: 7d0f 7c00 6a05 7c0e 1900 7d10 7c03 7c0d  }.|.j.|...}.|.|.
+00001430: 1900 6406 1900 7d11 7406 7c10 7407 8302  ..d...}.t.|.t...
+00001440: 72f2 7c10 6a08 6e02 6401 7d12 7c10 6a09  r.|.j.n.d.}.|.j.
+00001450: 6a0a 740b 6a0c 6b02 9001 720a 6406 6e02  j.t.j.k...r.d.n.
+00001460: 6408 7d13 7c0a 7c09 1800 7d14 7c09 7c0f  d.}.|.|...}.|.|.
+00001470: 1800 7d15 7c09 7d16 7c0b 7c06 1700 7d17  ..}.|.}.|.|...}.
+00001480: 7c12 6401 6b08 9001 7238 6402 6e0e 740d  |.d.k...r8d.n.t.
+00001490: 7c12 7c15 7c13 1400 1900 8301 7d18 7c08  |.|.|.......}.|.
+000014a0: 4400 9001 5d6e 7d19 7c15 7c14 6b00 9001  D...]n}.|.|.k...
+000014b0: 7260 7c15 6e06 7c14 6406 1800 7d15 7c12  r`|.n.|.d...}.|.
+000014c0: 6401 6b08 9001 7276 6402 6e0e 740d 7c12  d.k...rvd.n.t.|.
+000014d0: 7c15 7c13 1400 1900 8301 7d18 7c17 7c0c  |.|.......}.|.|.
+000014e0: 6b00 9001 7294 7c17 6e06 7c0c 6406 1800  k...r.|.n.|.d...
+000014f0: 7d17 740e 7c00 6a0f 7c17 1900 8301 7d1a  }.t.|.j.|.....}.
+00001500: 7c16 7c0a 6b00 9001 72b8 7c16 6e06 7c0a  |.|.k...r.|.n.|.
+00001510: 6406 1800 7d16 7c19 6409 6b02 9001 72fc  d...}.|.d.k...r.
+00001520: 7c11 a010 640a 7411 7c00 6a09 7c16 1900  |...d.t.|.j.|...
+00001530: 8301 7c1a 7c15 7c18 640b 9c05 a101 0100  ..|.|.|.d.......
+00001540: 7c15 6406 3700 7d15 7c16 6406 3700 7d16  |.d.7.}.|.d.7.}.
+00001550: 6ebe 7c19 640c 6b02 9002 7230 7c11 a010  n.|.d.k...r0|...
+00001560: 7411 7c00 6a09 7c17 1900 8301 640a 7c1a  t.|.j.|.....d.|.
+00001570: 7c15 7c18 640b 9c05 a101 0100 7c17 6406  |.|.d.......|.d.
+00001580: 3700 7d17 6e8a 7c19 640d 6b02 9002 7348  7.}.n.|.d.k...sH
+00001590: 7c19 640e 6b02 9002 7348 7402 8201 7411  |.d.k...sHt...t.
+000015a0: 7c00 6a09 7c17 1900 8301 7d1b 7411 7c00  |.j.|.....}.t.|.
+000015b0: 6a09 7c16 1900 8301 7d1c 7c19 640d 6b02  j.|.....}.|.d.k.
+000015c0: 9002 727e 7c1b 7c1c 6b02 9002 738c 7402  ..r~|.|.k...s.t.
+000015d0: 8201 6e0e 7c1b 7c1c 6b03 9002 738c 7402  ..n.|.|.k...s.t.
+000015e0: 8201 7c11 a010 7c1b 7c1c 7c1a 7c15 7c18  ..|...|.|.|.|.|.
+000015f0: 640b 9c05 a101 0100 7c15 6406 3700 7d15  d.......|.d.7.}.
+00001600: 7c16 6406 3700 7d16 7c17 6406 3700 7d17  |.d.7.}.|.d.7.}.
+00001610: 9001 714c 7112 7c03 5300 290f 612f 0400  ..qLq.|.S.).a/..
+00001620: 000a 2020 2020 436f 6d62 696e 6520 7468  ..    Combine th
+00001630: 6520 7365 676d 656e 7473 2062 726f 6b65  e segments broke
+00001640: 6e20 6279 2060 5f62 7265 616b 5f71 7565  n by `_break_que
+00001650: 7279 6020 746f 6765 7468 6572 2074 6f20  ry` together to 
+00001660: 6765 7420 6120 6c6f 6e67 2071 7565 7279  get a long query
+00001670: 2e0a 0a20 2020 204e 6f74 653a 2054 6865  ...    Note: The
+00001680: 2073 6567 6d65 6e74 7320 6865 7265 2063   segments here c
+00001690: 6f6e 7461 696e 2074 6865 206c 6576 656e  ontain the leven
+000016a0: 7368 7465 696e 2061 6c69 676e 6d65 6e74  shtein alignment
+000016b0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+000016c0: 2020 2073 6f75 7263 6564 5f74 6578 743a     sourced_text:
+000016d0: 0a20 2020 2020 2020 2054 6865 2053 6f75  .        The Sou
+000016e0: 7263 6564 5465 7874 2063 6f6e 7461 696e  rcedText contain
+000016f0: 696e 6720 7468 6520 7175 6572 6965 7320  ing the queries 
+00001700: 616e 6420 7265 6665 7265 6e63 6573 2e0a  and references..
+00001710: 2020 2020 2020 7375 625f 616c 6967 6e6d        sub_alignm
+00001720: 656e 7473 3a0a 2020 2020 2020 2020 4120  ents:.        A 
+00001730: 6c69 7374 206f 6620 7365 676d 656e 7473  list of segments
+00001740: 2c20 6561 6368 2069 7465 6d20 2872 6574  , each item (ret
+00001750: 7572 6e65 6420 6279 206c 6576 656e 7368  urned by levensh
+00001760: 7465 696e 5f77 6f72 6b65 7229 2063 6f6e  tein_worker) con
+00001770: 7461 696e 730a 2020 2020 2020 2020 7468  tains.        th
+00001780: 6520 7365 676d 656e 7420 6974 2062 656c  e segment it bel
+00001790: 6f6e 6773 2074 6f20 616e 6420 7468 6520  ongs to and the 
+000017a0: 6c65 7665 6e73 6874 6569 6e20 616c 6967  levenshtein alig
+000017b0: 6e6d 656e 742e 0a20 2020 2020 206e 756d  nment..      num
+000017c0: 5f71 7565 7269 6573 3a0a 2020 2020 2020  _queries:.      
+000017d0: 2020 5468 6520 6e75 6d62 6572 206f 6620    The number of 
+000017e0: 7175 6572 6965 732c 2074 6869 7320 6172  queries, this ar
+000017f0: 6775 6d65 6e74 2069 7320 666f 7220 6566  gument is for ef
+00001800: 6669 6369 656e 6379 2c20 6966 2077 6520  ficiency, if we 
+00001810: 6b6e 6f77 206e 756d 6265 720a 2020 2020  know number.    
+00001820: 2020 2020 6f66 2071 7565 7269 6573 2077      of queries w
+00001830: 6520 6361 6e20 7072 6561 6c6c 6f63 6174  e can preallocat
+00001840: 6520 7468 6520 6c69 7374 2e0a 2020 2020  e the list..    
+00001850: 5265 7475 726e 733a 0a20 2020 2020 2052  Returns:.      R
+00001860: 6574 7572 6e20 6120 6c69 7374 206f 6620  eturn a list of 
+00001870: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
+00001880: 2028 2871 7565 7279 5f73 7461 7274 2c20   ((query_start, 
+00001890: 7461 7267 6574 5f73 7461 7274 292c 205b  target_start), [
+000018a0: 616c 6967 6e6d 656e 7420 6974 656d 5d29  alignment item])
+000018b0: 2e0a 2020 2020 2020 5468 6520 6071 7565  ..      The `que
+000018c0: 7279 5f73 7461 7274 6020 616e 6420 6074  ry_start` and `t
+000018d0: 6172 6765 745f 7374 6172 7460 2061 7265  arget_start` are
+000018e0: 2069 6e64 6578 6573 2069 6e20 736f 7572   indexes in sour
+000018f0: 6365 645f 7465 7874 2c20 7468 6520 6061  ced_text, the `a
+00001900: 6c69 676e 6d65 6e74 2069 7465 6d60 0a20  lignment item`. 
+00001910: 2020 2020 2069 7320 6120 6c69 7374 2063       is a list c
+00001920: 6f6e 7461 696e 696e 6720 7b22 7265 6622  ontaining {"ref"
+00001930: 3a20 7265 662c 2022 6879 7022 3a20 6879  : ref, "hyp": hy
+00001940: 702c 2022 7265 665f 706f 7322 3a20 7265  p, "ref_pos": re
+00001950: 665f 706f 732c 2022 6879 705f 706f 7322  f_pos, "hyp_pos"
+00001960: 3a20 6879 705f 706f 732c 0a20 2020 2020  : hyp_pos,.     
+00001970: 2022 6879 705f 7469 6d65 223a 2068 7970   "hyp_time": hyp
+00001980: 5f74 696d 657d 2c20 7265 6620 6973 2074  _time}, ref is t
+00001990: 6865 2074 6f6b 656e 2066 726f 6d20 7265  he token from re
+000019a0: 6665 7265 6e63 652c 2068 7970 2069 7320  ference, hyp is 
+000019b0: 7468 6520 746f 6b65 6e20 6672 6f6d 2071  the token from q
+000019c0: 7565 7279 2c0a 2020 2020 2020 7265 665f  uery,.      ref_
+000019d0: 706f 7320 6973 206c 6f63 616c 2069 6e64  pos is local ind
+000019e0: 6578 2069 6e20 7265 6665 7265 6e63 6520  ex in reference 
+000019f0: 646f 6375 6d65 6e74 2c20 6879 705f 706f  document, hyp_po
+00001a00: 7320 6973 206c 6f63 616c 2069 6e64 6578  s is local index
+00001a10: 2069 6e20 7175 6572 7920 646f 6375 6d65   in query docume
+00001a20: 6e74 2c0a 2020 2020 2020 6879 705f 7469  nt,.      hyp_ti
+00001a30: 6d65 2069 7320 7468 6520 7469 6d65 7374  me is the timest
+00001a40: 616d 7020 6f66 2068 7970 2e0a 2020 2020  amp of hyp..    
+00001a50: 4e72 0100 0000 da09 616c 6967 6e6d 656e  Nr......alignmen
+00001a60: 7472 2b00 0000 7a1b 536b 6970 7069 6e67  tr+...z.Skipping
+00001a70: 2065 6d70 7479 2073 7562 2073 6567 6d65   empty sub segme
+00001a80: 6e74 2e72 0f00 0000 da07 7365 676d 656e  nt.r......segmen
+00001a90: 7472 2c00 0000 da01 49da 0029 05da 0372  tr,.....I..)...r
+00001aa0: 6566 da03 6879 70da 0772 6566 5f70 6f73  ef..hyp..ref_pos
+00001ab0: da07 6879 705f 706f 73da 0868 7970 5f74  ..hyp_pos..hyp_t
+00001ac0: 696d 65da 0144 da01 43da 0153 2912 da07  ime..D..C..S)...
+00001ad0: 6c6f 6767 696e 67da 0777 6172 6e69 6e67  logging..warning
+00001ae0: 721c 0000 0072 3700 0000 7238 0000 00da  r....r7...r8....
+00001af0: 0773 6f75 7263 6573 da0a 6973 696e 7374  .sources..isinst
+00001b00: 616e 6365 7213 0000 00da 0574 696d 6573  ancer......times
+00001b10: da0b 6269 6e61 7279 5f74 6578 7472 1a00  ..binary_textr..
+00001b20: 0000 721e 0000 00da 0575 696e 7438 da05  ..r......uint8..
+00001b30: 666c 6f61 74da 0369 6e74 da03 706f 7372  float..int..posr
+00001b40: 2e00 0000 da03 6368 7229 1d72 2600 0000  ......chr).r&...
+00001b50: 7242 0000 0072 4300 0000 da0a 616c 6967  rB...rC.....alig
+00001b60: 6e6d 656e 7473 5a0f 7072 6576 5f74 6172  nmentsZ.prev_tar
+00001b70: 6765 745f 656e 64da 0373 7562 5a12 7461  get_end..subZ.ta
+00001b80: 7267 6574 5f61 6c69 676e 5f73 7461 7274  rget_align_start
+00001b90: 5a10 7461 7267 6574 5f61 6c69 676e 5f65  Z.target_align_e
+00001ba0: 6e64 5a09 616c 6967 6e5f 7374 7272 2f00  ndZ.align_strr/.
+00001bb0: 0000 7230 0000 0072 3100 0000 7232 0000  ..r0...r1...r2..
+00001bc0: 005a 0871 7565 7279 5f69 6472 3e00 0000  .Z.query_idr>...
+00001bd0: 723f 0000 00da 0c71 7565 7279 5f73 6f75  r?.....query_sou
+00001be0: 7263 65da 0661 6c69 676e 7372 5400 0000  rce..alignsrT...
+00001bf0: 5a0b 7469 6d65 5f73 7472 6964 655a 0c71  Z.time_strideZ.q
+00001c00: 7565 7279 5f6c 656e 6774 685a 1171 7565  uery_lengthZ.que
+00001c10: 7279 5f6c 6f63 616c 5f69 6e64 6578 5a0b  ry_local_indexZ.
+00001c20: 7175 6572 795f 696e 6465 78da 0c74 6172  query_index..tar
+00001c30: 6765 745f 696e 6465 7872 4c00 0000 da03  get_indexrL.....
+00001c40: 616c 6972 4a00 0000 7248 0000 0072 4900  alirJ...rH...rI.
+00001c50: 0000 7222 0000 0072 2200 0000 7223 0000  ..r"...r"...r#..
+00001c60: 00da 175f 636f 6d62 696e 655f 7375 625f  ..._combine_sub_
+00001c70: 616c 6967 6e6d 656e 7473 eb00 0000 739c  alignments....s.
+00001c80: 0000 0000 1a0a 0104 010a 0110 010a 0102  ................
+00001c90: 0416 0110 0210 0312 0102 010a fe06 050a  ................
+00001ca0: 020c 020a 0102 fe08 050a 010a 010a 030c  ................
+00001cb0: 0314 0218 0208 0108 0104 0108 021e 010a  ................
+00001cc0: 0306 ff08 0206 fd02 061c ff02 0316 020e  ................
+00001cd0: 0116 010a 0104 0202 010c 0102 0102 0102  ................
+00001ce0: fb04 ff04 0908 010a 010a 0104 020c 0102  ................
+00001cf0: 0102 0102 0102 fb04 ff04 090a 0218 010e  ................
+00001d00: 010e 030a 0110 020e 0104 0202 0102 0102  ................
+00001d10: 0102 0102 fb04 ff04 0908 0108 010e 0172  ...............r
+00001d20: 6100 0000 2906 7226 0000 00da 0d63 6c6f  a...).r&.....clo
+00001d30: 7365 5f6d 6174 6368 6573 7228 0000 0072  se_matchesr(...r
+00001d40: 2900 0000 da0b 7468 7265 6164 5f70 6f6f  ).....thread_poo
+00001d50: 6c72 1900 0000 6305 0000 0000 0000 0000  lr....c.........
+00001d60: 0000 001e 0000 0007 0000 0043 0000 0073  ...........C...s
+00001d70: 6402 0000 7c01 6a00 5c02 7d05 7d06 7c00  d...|.j.\.}.}.|.
+00001d80: 6a01 7c05 1900 7d07 7c00 6a02 7d08 7403  j.|...}.|.j.}.t.
+00001d90: a004 6401 a101 0100 6700 7d09 7405 7c07  ..d.....g.}.t.|.
+00001da0: 8301 4400 9001 5dd6 7d0a 7c08 7c0a 1900  ..D...].}.|.|...
+00001db0: 7d0b 7c08 7c0a 6402 1700 1900 7d0c 7c08  }.|.|.d.....}.|.
+00001dc0: 7c0a 6402 1700 1900 7c08 7c0a 1900 1800  |.d.....|.|.....
+00001dd0: 7d0d 7406 a007 7c0b 7c0c a102 a008 6403  }.t...|.|.....d.
+00001de0: 6402 a102 7d0e 7406 a009 7c0e 7c06 a102  d...}.t...|.|...
+00001df0: a00a a100 7d0e 7c01 7c0b 7c0c 8502 6404  ....}.|.|.|...d.
+00001e00: 6404 8502 6602 1900 a00a a100 7d0f 740b  d...f.......}.t.
+00001e10: 7c0e 7c0f 8302 7d10 740c 7c10 8301 6405  |.|...}.t.|...d.
+00001e20: 6b02 72b2 7130 740c 7c10 8301 6402 1800  k.r.q0t.|...d...
+00001e30: 7d11 7c10 7c11 1900 6402 1900 7c00 6a0d  }.|.|...d...|.j.
+00001e40: 6a0e 6402 1800 6b02 72e0 7c11 6402 3800  j.d...k.r.|.d.8.
+00001e50: 7d11 71be 7c10 6405 7c11 8502 1900 7d10  }.q.|.d.|.....}.
+00001e60: 7c00 6a01 7406 a00f 6406 6407 8400 7c10  |.j.t...d.d...|.
+00001e70: 4400 8301 a101 1900 7d12 7c12 7c12 6405  D.......}.|.|.d.
+00001e80: 1900 1800 7d12 7410 7c12 8301 7d13 6403  ....}.t.|...}.d.
+00001e90: 7d14 6405 740c 7c10 8301 6602 7d15 7405  }.d.t.|...f.}.t.
+00001ea0: 7c13 6a0e 6402 1800 8301 4400 5d6e 7d16  |.j.d.....D.]n}.
+00001eb0: 7c13 7c16 6402 1700 1900 7c13 7c16 1900  |.|.d.....|.|...
+00001ec0: 1800 6408 6b00 9001 725a 9001 7138 7c10  ..d.k...rZ..q8|.
+00001ed0: 7c13 7c16 6402 1700 1900 6402 1800 1900  |.|.d.....d.....
+00001ee0: 6405 1900 7c10 7c13 7c16 1900 1900 6405  d...|.|.|.....d.
+00001ef0: 1900 1800 7d17 7c17 7c14 6b04 9001 7238  ....}.|.|.k...r8
+00001f00: 7c17 7d14 7c13 7c16 1900 7c13 7c16 6402  |.}.|.|...|.|.d.
+00001f10: 1700 1900 6602 7d15 9001 7138 7c14 6409  ....f.}...q8|.d.
+00001f20: 7c0d 1400 6b00 9001 72ca 7403 a011 640a  |...k...r.t...d.
+00001f30: 7c0a 9b00 640b 9d03 a101 0100 7130 7c10  |...d.......q0|.
+00001f40: 7c15 6405 1900 7c15 6402 1900 8502 1900  |.d...|.d.......
+00001f50: 7d10 7412 7c00 7c10 7c02 7c03 640c 8d04  }.t.|.|.|.|.d...
+00001f60: 7d18 7c18 4400 5d14 7d19 7c09 a013 7c00  }.|.D.].}.|...|.
+00001f70: 7c19 6602 a101 0100 9001 71f2 7130 7403  |.f.......q.q0t.
+00001f80: a004 640d a101 0100 640e 640f 8400 7d1a  ..d.....d.d...}.
+00001f90: 7c04 6404 6b08 9002 722c 7414 8300 6e02  |.d.k...r,t...n.
+00001fa0: 7c04 7d1b 7403 a004 6410 a101 0100 7c1b  |.}.t...d.....|.
+00001fb0: a015 7c1a 7c09 a102 7d1c 7c1c a016 a100  ..|.|...}.|.....
+00001fc0: 7d1d 7403 a004 6411 a101 0100 7417 7c00  }.t...d.....t.|.
+00001fd0: 7c1d 7c07 8303 5300 2912 610d 0700 000a  |.|...S.).a.....
+00001fe0: 2020 2020 4765 7420 6c65 7665 6e73 6874      Get levensht
+00001ff0: 6569 6e20 616c 6967 6e6d 656e 7420 666f  ein alignment fo
+00002000: 7220 6561 6368 2071 7565 7279 2064 6f63  r each query doc
+00002010: 756d 656e 7420 696e 2073 6f75 7263 6564  ument in sourced
+00002020: 5f74 6578 742e 0a0a 2020 2020 466f 7220  _text...    For 
+00002030: 6561 6368 2071 7565 7279 2064 6f63 756d  each query docum
+00002040: 656e 7420 7765 2077 696c 6c20 6c6f 6361  ent we will loca
+00002050: 7465 2069 7473 2063 6f72 7265 7370 6f6e  te its correspon
+00002060: 6469 6e67 2073 6567 6d65 6e74 2069 6e20  ding segment in 
+00002070: 7468 6520 7265 6665 7265 6e63 650a 2020  the reference.  
+00002080: 2020 646f 6375 6d65 6e74 2061 6e64 2072    document and r
+00002090: 6574 7572 6e20 7468 6520 6c65 7665 6e73  eturn the levens
+000020a0: 6874 6569 6e20 616c 6967 6e6d 656e 7420  htein alignment 
+000020b0: 6265 7477 6565 6e20 7468 6520 7175 6572  between the quer
+000020c0: 7920 616e 6420 6974 7320 636f 7272 6573  y and its corres
+000020d0: 706f 6e64 696e 670a 2020 2020 7265 6665  ponding.    refe
+000020e0: 7265 6e63 6520 7365 676d 656e 742e 0a0a  rence segment...
+000020f0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00002100: 736f 7572 6365 645f 7465 7874 3a0a 2020  sourced_text:.  
+00002110: 2020 2020 2020 5468 6520 536f 7572 6365        The Source
+00002120: 6454 6578 7420 636f 6e74 6169 6e69 6e67  dText containing
+00002130: 2074 6865 2071 7565 7269 6573 2061 6e64   the queries and
+00002140: 2072 6566 6572 656e 6365 732c 2074 6865   references, the
+00002150: 2066 6972 7374 204e 2028 7765 2063 616e   first N (we can
+00002160: 0a20 2020 2020 2020 2067 6574 2069 7420  .        get it 
+00002170: 6672 6f6d 2063 6c6f 7365 5f6d 6174 6368  from close_match
+00002180: 6573 2920 646f 6375 6d65 6e74 7320 6172  es) documents ar
+00002190: 6520 7175 6572 6965 7320 616e 6420 7468  e queries and th
+000021a0: 6520 6f74 6865 7273 2061 7265 2072 6566  e others are ref
+000021b0: 6572 656e 6365 732e 0a20 2020 2020 2063  erences..      c
+000021c0: 6c6f 7365 5f6d 6174 6368 6573 3a0a 2020  lose_matches:.  
+000021d0: 2020 2020 2020 4765 6e65 7261 7465 6420        Generated 
+000021e0: 6672 6f6d 2073 6f75 7263 6564 5f74 6578  from sourced_tex
+000021f0: 7420 7769 7468 2074 6865 2066 756e 6374  t with the funct
+00002200: 696f 6e20 6066 696e 645f 6361 6e64 6964  ion `find_candid
+00002210: 6174 655f 6d61 7463 6865 7360 2e0a 2020  ate_matches`..  
+00002220: 2020 2020 2020 4974 2063 6f6e 7461 696e        It contain
+00002230: 7320 7468 6520 636c 6f73 6520 6d61 7463  s the close matc
+00002240: 6865 6420 7265 6665 7265 6e63 6520 746f  hed reference to
+00002250: 6b65 6e20 666f 7220 6561 6368 2071 7565  ken for each que
+00002260: 7279 2074 6f6b 656e 2e0a 2020 2020 2020  ry token..      
+00002270: 7365 676d 656e 745f 6c65 6e67 7468 3a0a  segment_length:.
+00002280: 2020 2020 2020 2020 5468 6520 7175 6572          The quer
+00002290: 7920 6c65 6e67 7468 206d 6967 6874 2062  y length might b
+000022a0: 6520 6c6f 6e67 2c20 696e 206f 7264 6572  e long, in order
+000022b0: 2074 6f20 6163 6365 6c65 7261 7465 2074   to accelerate t
+000022c0: 6865 206c 6576 656e 7368 7465 696e 0a20  he levenshtein. 
+000022d0: 2020 2020 2020 2061 6c67 6f72 6974 686d         algorithm
+000022e0: 2077 6520 7769 6c6c 2073 706c 6974 2074   we will split t
+000022f0: 6865 206c 6f6e 6720 7175 6572 7920 696e  he long query in
+00002300: 746f 2073 6d61 6c6c 6572 2073 6567 6d65  to smaller segme
+00002310: 6e74 732c 2060 7365 676d 656e 745f 6c65  nts, `segment_le
+00002320: 6e67 7468 600a 2020 2020 2020 2020 6973  ngth`.        is
+00002330: 2074 6865 2065 7870 6563 7465 6420 6c65   the expected le
+00002340: 6e67 7468 206f 6620 7468 6520 736d 616c  ngth of the smal
+00002350: 6c65 7220 7365 676d 656e 7473 2e0a 2020  ler segments..  
+00002360: 2020 2020 7265 6665 7265 6e63 655f 6c65      reference_le
+00002370: 6e67 7468 5f64 6966 6665 7265 6e63 653a  ngth_difference:
+00002380: 0a20 2020 2020 2020 2042 6563 6175 7365  .        Because
+00002390: 206f 6620 7468 6520 696e 7365 7274 696f   of the insertio
+000023a0: 6e20 6f72 2064 656c 6574 696f 6e20 6572  n or deletion er
+000023b0: 726f 7273 2c20 7468 6520 7265 6665 7265  rors, the refere
+000023c0: 6e63 6520 7365 7175 656e 6365 206d 6967  nce sequence mig
+000023d0: 6874 2062 650a 2020 2020 2020 2020 7368  ht be.        sh
+000023e0: 6f72 7465 7220 6f72 206c 6f6e 6765 7220  orter or longer 
+000023f0: 7468 616e 2074 6865 2071 7565 7279 2c20  than the query, 
+00002400: 736f 2074 6865 2072 6566 6572 656e 6365  so the reference
+00002410: 2073 6567 6d65 6e74 206c 656e 6774 6820   segment length 
+00002420: 6361 6e20 6265 2066 726f 6d0a 2020 2020  can be from.    
+00002430: 2020 2020 606c 656e 2871 7565 7279 2920      `len(query) 
+00002440: 2a20 2831 202d 2072 6566 6572 656e 6365  * (1 - reference
+00002450: 5f6c 656e 6774 685f 6469 6666 6572 656e  _length_differen
+00002460: 6365 202f 2032 2960 2074 6f0a 2020 2020  ce / 2)` to.    
+00002470: 2020 2020 606c 656e 2871 7565 7279 2920      `len(query) 
+00002480: 2a20 2831 202b 2072 6566 6572 656e 6365  * (1 + reference
+00002490: 5f6c 656e 6774 685f 6469 6666 6572 656e  _length_differen
+000024a0: 6365 202f 2032 2960 2e0a 2020 2020 2020  ce / 2)`..      
+000024b0: 7468 7265 6164 5f70 6f6f 6c3a 0a20 2020  thread_pool:.   
+000024c0: 2020 2020 2054 6865 2054 6872 6561 6450       The ThreadP
+000024d0: 6f6f 6c20 746f 2072 756e 206c 6576 656e  ool to run leven
+000024e0: 7368 7465 696e 2e0a 2020 2020 5265 7475  shtein..    Retu
+000024f0: 726e 733a 0a20 2020 2020 2052 6574 7572  rns:.      Retur
+00002500: 6e20 6120 6c69 7374 206f 6620 7475 706c  n a list of tupl
+00002510: 6520 636f 6e74 6169 6e69 6e67 2028 2871  e containing ((q
+00002520: 7565 7279 5f73 7461 7274 2c20 7461 7267  uery_start, targ
+00002530: 6574 5f73 7461 7274 292c 205b 616c 6967  et_start), [alig
+00002540: 6e6d 656e 7420 6974 656d 5d29 2e0a 2020  nment item])..  
+00002550: 2020 2020 5468 6520 6071 7565 7279 5f73      The `query_s
+00002560: 7461 7274 6020 616e 6420 6074 6172 6765  tart` and `targe
+00002570: 745f 7374 6172 7460 2061 7265 2069 6e64  t_start` are ind
+00002580: 6578 6573 2069 6e20 736f 7572 6365 645f  exes in sourced_
+00002590: 7465 7874 2c20 7468 6520 6061 6c69 676e  text, the `align
+000025a0: 6d65 6e74 2069 7465 6d60 0a20 2020 2020  ment item`.     
+000025b0: 2069 7320 6120 6c69 7374 2063 6f6e 7461   is a list conta
+000025c0: 696e 696e 6720 7b22 7265 6622 3a20 7265  ining {"ref": re
+000025d0: 662c 2022 6879 7022 3a20 6879 702c 2022  f, "hyp": hyp, "
+000025e0: 7265 665f 706f 7322 3a20 7265 665f 706f  ref_pos": ref_po
+000025f0: 732c 2022 6879 705f 706f 7322 3a20 6879  s, "hyp_pos": hy
+00002600: 705f 706f 732c 0a20 2020 2020 2022 6879  p_pos,.      "hy
+00002610: 705f 7469 6d65 223a 2068 7970 5f74 696d  p_time": hyp_tim
+00002620: 657d 2c20 7265 6620 6973 2074 6865 2074  e}, ref is the t
+00002630: 6f6b 656e 2066 726f 6d20 7265 6665 7265  oken from refere
+00002640: 6e63 652c 2068 7970 2069 7320 7468 6520  nce, hyp is the 
+00002650: 746f 6b65 6e20 6672 6f6d 2071 7565 7279  token from query
+00002660: 2c0a 2020 2020 2020 7265 665f 706f 7320  ,.      ref_pos 
+00002670: 6973 206c 6f63 616c 2069 6e64 6578 2069  is local index i
+00002680: 6e20 7265 6665 7265 6e63 6520 646f 6375  n reference docu
+00002690: 6d65 6e74 2c20 6879 705f 706f 7320 6973  ment, hyp_pos is
+000026a0: 206c 6f63 616c 2069 6e64 6578 2069 6e20   local index in 
+000026b0: 7175 6572 7920 646f 6375 6d65 6e74 2c0a  query document,.
+000026c0: 2020 2020 2020 6879 705f 7469 6d65 2069        hyp_time i
+000026d0: 7320 7468 6520 7469 6d65 7374 616d 7020  s the timestamp 
+000026e0: 6f66 2068 7970 2e0a 2020 2020 7a18 4765  of hyp..    z.Ge
+000026f0: 7474 696e 6720 6d61 7463 6869 6e67 2070  tting matching p
+00002700: 6f69 6e74 732e 720f 0000 0072 2b00 0000  oints.r....r+...
+00002710: 4e72 0100 0000 6301 0000 0000 0000 0000  Nr....c.........
+00002720: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00002730: 1400 0000 6700 7c00 5d0c 7d01 7c01 6400  ....g.|.].}.|.d.
+00002740: 1900 9102 7104 5300 2901 720f 0000 0072  ....q.S.).r....r
+00002750: 2200 0000 2902 da02 2e30 da01 7872 2200  "...)....0..xr".
+00002760: 0000 7222 0000 0072 2300 0000 da0a 3c6c  ..r"...r#.....<l
+00002770: 6973 7463 6f6d 703e bb01 0000 7304 0000  istcomp>....s...
+00002780: 0006 0002 007a 2267 6574 5f61 6c69 676e  .....z"get_align
+00002790: 6d65 6e74 732e 3c6c 6f63 616c 733e 2e3c  ments.<locals>.<
+000027a0: 6c69 7374 636f 6d70 3e72 2a00 0000 671f  listcomp>r*...g.
+000027b0: 85eb 51b8 1ed5 3f7a 0f53 6b69 7070 696e  ..Q...?z.Skippin
+000027c0: 6720 7175 6572 7920 7a34 2c20 6c65 7373  g query z4, less
+000027d0: 2074 6861 6e20 3120 2f20 3320 6f66 2071   than 1 / 3 of q
+000027e0: 7565 7279 206d 6174 6368 6564 2062 7920  uery matched by 
+000027f0: 636c 6f73 655f 6d61 7463 6865 732e 2904  close_matches.).
+00002800: 7226 0000 0072 2700 0000 7228 0000 0072  r&...r'...r(...r
+00002810: 2900 0000 7a1d 4765 7474 696e 6720 6d61  )...z.Getting ma
+00002820: 7463 6869 6e67 2070 6f69 6e74 7320 646f  tching points do
+00002830: 6e65 2e63 0200 0000 0000 0000 0000 0000  ne.c............
+00002840: 0500 0000 0500 0000 5300 0000 7346 0000  ........S...sF..
+00002850: 007c 006a 007c 0164 0119 007c 0164 0219  .|.j.|.d...|.d..
+00002860: 0085 0219 007d 027c 006a 007c 0164 0319  .....}.|.j.|.d..
+00002870: 007c 0164 0419 0085 0219 007d 0374 017c  .|.d.......}.t.|
+00002880: 027c 0364 0564 068d 037d 047c 017c 047c  .|.d.d...}.|.|.|
+00002890: 0364 079c 0353 0029 084e 7201 0000 0072  .d...S.).Nr....r
+000028a0: 0f00 0000 722a 0000 00e9 0300 0000 da06  ....r*..........
+000028b0: 676c 6f62 616c 2903 da05 7175 6572 79da  global)...query.
+000028c0: 0674 6172 6765 74da 046d 6f64 6529 0372  .target..mode).r
+000028d0: 4500 0000 7244 0000 0072 6a00 0000 2902  E...rD...rj...).
+000028e0: 7255 0000 0072 0e00 0000 2905 7226 0000  rU...r....).r&..
+000028f0: 0072 4500 0000 7269 0000 0072 6a00 0000  .rE...ri...rj...
+00002900: 7244 0000 0072 2200 0000 7222 0000 0072  rD...r"...r"...r
+00002910: 2300 0000 da12 6c65 7665 6e73 6874 6569  #.....levenshtei
+00002920: 6e5f 776f 726b 6572 e401 0000 730e 0000  n_worker....s...
+00002930: 0000 0116 0116 030e 0202 0102 0102 fd7a  ...............z
+00002940: 2a67 6574 5f61 6c69 676e 6d65 6e74 732e  *get_alignments.
+00002950: 3c6c 6f63 616c 733e 2e6c 6576 656e 7368  <locals>.levensh
+00002960: 7465 696e 5f77 6f72 6b65 727a 1a4d 6174  tein_workerz.Mat
+00002970: 6368 696e 6720 7769 7468 206c 6576 656e  ching with leven
+00002980: 7368 7465 696e 2e7a 1f4d 6174 6368 696e  shtein.z.Matchin
+00002990: 6720 7769 7468 206c 6576 656e 7368 7465  g with levenshte
+000029a0: 696e 2064 6f6e 652e 2918 da05 7368 6170  in done.)...shap
+000029b0: 6572 3700 0000 7238 0000 0072 5000 0000  er7...r8...rP...
+000029c0: da04 696e 666f 722d 0000 0072 1e00 0000  ..infor-...r....
+000029d0: da06 6172 616e 6765 da07 7265 7368 6170  ..arange..reshap
+000029e0: 65da 0474 696c 65da 0766 6c61 7474 656e  e..tile..flatten
+000029f0: 720d 0000 0072 3600 0000 7255 0000 0072  r....r6...rU...r
+00002a00: 1d00 0000 da05 6172 7261 7972 1600 0000  ......arrayr....
+00002a10: 7251 0000 0072 4100 0000 722e 0000 0072  rQ...rA...r....r
+00002a20: 0600 0000 da0d 7374 6172 6d61 705f 6173  ......starmap_as
+00002a30: 796e 63da 0367 6574 7261 0000 0029 1e72  ync..getra...).r
+00002a40: 2600 0000 7262 0000 0072 2800 0000 7229  &...rb...r(...r)
+00002a50: 0000 0072 6300 0000 da11 746f 745f 7175  ...rc.....tot_qu
+00002a60: 6572 795f 7379 6d62 6f6c 73da 116e 756d  ery_symbols..num
+00002a70: 5f63 6c6f 7365 5f6d 6174 6368 6573 7243  _close_matchesrC
+00002a80: 0000 00da 0a72 6f77 5f73 706c 6974 73da  .....row_splits.
+00002a90: 0961 7267 756d 656e 7473 da01 7172 2f00  .arguments..qr/.
+00002aa0: 0000 7230 0000 00da 0971 7565 7279 5f6c  ..r0.....query_l
+00002ab0: 656e 7217 0000 0072 1800 0000 7227 0000  enr....r....r'..
+00002ac0: 005a 0874 7269 6d5f 706f 735a 0764 6f63  .Z.trim_posZ.doc
+00002ad0: 5f69 6473 7238 0000 005a 0f6d 6178 5f6e  _idsr8...Z.max_n
+00002ae0: 756d 5f6d 6174 6368 6573 5a0a 6d61 785f  um_matchesZ.max_
+00002af0: 7261 6e67 6573 7234 0000 005a 0b6e 756d  rangesr4...Z.num
+00002b00: 5f6d 6174 6368 6573 7233 0000 00da 0373  _matchesr3.....s
+00002b10: 6567 726c 0000 00da 0470 6f6f 6cda 0d61  egrl.....pool..a
+00002b20: 7379 6e63 5f72 6573 756c 7473 da07 7265  sync_results..re
+00002b30: 7375 6c74 7372 2200 0000 7222 0000 0072  sultsr"...r"...r
+00002b40: 2300 0000 da0e 6765 745f 616c 6967 6e6d  #.....get_alignm
+00002b50: 656e 7473 7001 0000 7370 0000 0000 280a  entsp...sp....(.
+00002b60: 010a 0206 020a 0104 010e 0108 010c 0114  ................
+00002b70: 0414 0110 0218 030a 020c 0102 040c 0118  ................
+00002b80: 010a 010c 051a 030c 0108 0104 010c 0112  ................
+00002b90: 011a 0104 0216 010e ff02 ff02 040a 0104  ................
+00002ba0: 0118 020e 0104 010a ff04 0302 0214 0402  ................
+00002bb0: 0102 0102 0102 0102 fc06 0808 0114 020a  ................
+00002bc0: 0208 0c14 010a 010c 0108 010a 0272 8000  .............r..
+00002bd0: 0000 2902 da0d 7461 7267 6574 5f73 6f75  ..)...target_sou
+00002be0: 7263 6572 1900 0000 6302 0000 0000 0000  rcer....c.......
+00002bf0: 0000 0000 0030 0000 0007 0000 0043 0000  .....0.......C..
+00002c00: 0073 c607 0000 7c01 5c02 5c02 7d02 7d03  .s....|.\.\.}.}.
+00002c10: 7d04 6700 7d05 6700 7d06 6401 7d07 7400  }.g.}.g.}.d.}.t.
+00002c20: 6402 6403 8400 7c04 6404 7c07 8502 1900  d.d...|.d.|.....
+00002c30: 4400 8301 8301 7d08 6405 7d09 7c09 7d0a  D.....}.d.}.|.}.
+00002c40: 7c09 7d0b 6404 6701 7401 7c04 8301 1400  |.}.d.g.t.|.....
+00002c50: 7d0c 6404 6701 7401 7c04 8301 1400 7d0d  }.d.g.t.|.....}.
+00002c60: 7402 7c04 8301 4400 9002 5d5c 5c02 7d0e  t.|...D...]\\.}.
+00002c70: 7d0f 7c0f 6406 1900 7c0f 6407 1900 6b02  }.|.d...|.d...k.
+00002c80: 7d10 7c0e 6404 6b02 728c 7403 7c10 8301  }.|.d.k.r.t.|...
+00002c90: 6e12 7c0c 7c0e 6408 1800 1900 7403 7c10  n.|.|.d.....t.|.
+00002ca0: 8301 1700 7c0c 7c0e 3c00 7c0e 6404 6b02  ....|.|.<.|.d.k.
+00002cb0: 72b6 7403 7c10 0c00 8301 6e14 7c0d 7c0e  r.t.|.....n.|.|.
+00002cc0: 6408 1800 1900 7403 7c10 0c00 8301 1700  d.....t.|.......
+00002cd0: 7c0d 7c0e 3c00 7c0e 7c07 1800 6404 6b05  |.|.<.|.|...d.k.
+00002ce0: 9001 7208 7c04 7c0e 7c07 1800 1900 6406  ..r.|.|.|.....d.
+00002cf0: 1900 7c04 7c0e 7c07 1800 1900 6407 1900  ..|.|.|.....d...
+00002d00: 6b03 9001 7208 7c08 6408 3800 7d08 7c0e  k...r.|.d.8.}.|.
+00002d10: 7c07 1700 7401 7c04 8301 6b00 9001 7244  |...t.|...k...rD
+00002d20: 7c04 7c0e 7c07 1700 1900 6406 1900 7c04  |.|.|.....d...|.
+00002d30: 7c0e 7c07 1700 1900 6407 1900 6b03 9001  |.|.....d...k...
+00002d40: 7244 7c08 6408 3700 7d08 7c0e 6404 6b02  rD|.d.7.}.|.d.k.
+00002d50: 9001 7252 7c0a 6e16 7c0f 6409 1900 7c04  ..rR|.n.|.d...|.
+00002d60: 7c0e 6408 1800 1900 6409 1900 1800 7d11  |.d.....d.....}.
+00002d70: 7c11 7c0a 6b04 9001 7278 7c0a 6e02 7c11  |.|.k...rx|.n.|.
+00002d80: 7d11 7c0e 7401 7c04 8301 6408 1800 6b02  }.|.t.|...d...k.
+00002d90: 9001 7292 7c0a 6e16 7c04 7c0e 6408 1700  ..r.|.n.|.|.d...
+00002da0: 1900 6409 1900 7c0f 6409 1900 1800 7d12  ..d...|.d.....}.
+00002db0: 7c12 7c0a 6b04 9001 72b8 7c0a 6e02 7c12  |.|.k...r.|.n.|.
+00002dc0: 7d12 6404 7d13 7c0f 640a 1900 6408 1800  }.d.}.|.d...d...
+00002dd0: 7d14 7c14 6404 6b05 9002 7222 7404 7c00  }.|.d.k...r"t.|.
+00002de0: 6a05 7c14 1900 8301 7d15 7406 7c15 640b  j.|.....}.t.|.d.
+00002df0: 640c 8d02 9001 72fc 7c0b 7d13 9002 7122  d.....r.|.}...q"
+00002e00: 6e22 7c15 640d 6b02 9002 7310 7406 7c15  n"|.d.k...s.t.|.
+00002e10: 8301 9002 7222 7c14 6408 3800 7d14 6e04  ....r"|.d.8.}.n.
+00002e20: 9002 7122 9001 71cc 6404 7d16 7c0f 640a  ..q"..q.d.}.|.d.
+00002e30: 1900 6408 1700 7d14 7c14 7c00 6a05 6a07  ..d...}.|.|.j.j.
+00002e40: 6b00 9002 728c 7404 7c00 6a05 7c14 1900  k...r.t.|.j.|...
+00002e50: 8301 7d15 7406 7c15 640b 640c 8d02 9002  ..}.t.|.d.d.....
+00002e60: 7266 7c0b 7d16 9002 718c 6e22 7c15 640d  rf|.}...q.n"|.d.
+00002e70: 6b02 9002 737a 7406 7c15 8301 9002 728c  k...szt.|.....r.
+00002e80: 7c14 6408 3700 7d14 6e04 9002 718c 9002  |.d.7.}.n...q...
+00002e90: 7132 7c05 a008 7c0e 7c11 7c13 1700 7c08  q2|...|.|.|...|.
+00002ea0: 7c07 1b00 1800 6602 a101 0100 7c06 a008  |.....f.....|...
+00002eb0: 7c0e 7c12 7c16 1700 7c08 7c07 1b00 1800  |.|.|...|.|.....
+00002ec0: 6602 a101 0100 7162 7409 7c05 640e 640f  f.....qbt.|.d.d.
+00002ed0: 8400 640b 6410 8d03 7d17 7409 7c06 6411  ..d.d...}.t.|.d.
+00002ee0: 640f 8400 640b 6410 8d03 7d18 6412 7d19  d...d.d...}.d.}.
+00002ef0: 7c17 6404 7403 7401 7c05 8301 7c19 1400  |.d.t.t.|...|...
+00002f00: 8301 8502 1900 7d1a 7c18 6404 7403 7401  ......}.|.d.t.t.
+00002f10: 7c06 8301 7c19 1400 8301 8502 1900 7d1b  |...|.........}.
+00002f20: 6700 7d1c 6700 7d1d 6413 7d1e 6414 7d1f  g.}.g.}.d.}.d.}.
+00002f30: 6415 7d20 7c09 7d21 6416 7d22 6417 7d23  d.} |.}!d.}"d.}#
+00002f40: 6418 7d24 7c1a 4400 9002 5d38 7d25 6700  d.}$|.D...]8}%g.
+00002f50: 7d26 7c25 6404 1900 6408 1700 7d27 7c27  }&|%d...d...}'|'
+00002f60: 7401 7c06 8301 6b00 9005 7232 7c06 7c27  t.|...k...r2|.|'
+00002f70: 1900 6404 1900 7c25 6404 1900 1800 7c20  ..d...|%d.....| 
+00002f80: 6b00 9005 7232 7c05 7c25 6404 1900 1900  k...r2|.|%d.....
+00002f90: 6408 1900 7c06 7c27 1900 6408 1900 1700  d...|.|'..d.....
+00002fa0: 7d28 7c09 7c0c 7c06 7c27 1900 6404 1900  }(|.|.|.|'..d...
+00002fb0: 1900 7c0c 7c25 6404 1900 1900 1800 1400  ..|.|%d.........
+00002fc0: 7c06 7c27 1900 6404 1900 7c25 6404 1900  |.|'..d...|%d...
+00002fd0: 1800 1b00 7d29 7c0d 7c06 7c27 1900 6404  ....})|.|.|'..d.
+00002fe0: 1900 1900 7c0d 7c25 6404 1900 1900 1800  ....|.|%d.......
+00002ff0: 7d2a 7c2a 7c06 7c27 1900 6404 1900 7c25  }*|*|.|'..d...|%
+00003000: 6404 1900 1800 7c1f 1400 6b05 9004 7216  d.....|...k...r.
+00003010: 7c27 6408 3700 7d27 9003 7158 7c09 7c2a  |'d.7.}'..qX|.|*
+00003020: 1400 7c06 7c27 1900 6404 1900 7c25 6404  ..|.|'..d...|%d.
+00003030: 1900 1800 1b00 7d2b 7c04 7c06 7c27 1900  ......}+|.|.|'..
+00003040: 6404 1900 1900 6409 1900 7c04 7c25 6404  d.....d...|.|%d.
+00003050: 1900 1900 6409 1900 1800 7d2c 7c2c 7c22  ....d.....},|,|"
+00003060: 6b05 9004 736a 7c2c 7c23 6b01 9004 7272  k...sj|,|#k...rr
+00003070: 740a 6419 8301 6e02 7c21 7d2d 7c2c 7c24  t.d...n.|!}-|,|$
+00003080: 6404 1900 6b00 9004 72aa 7c2c 7c23 6b04  d...k...r.|,|#k.
+00003090: 9004 72aa 7c2d 7c2c 7c23 1800 7c24 6404  ..r.|-|,|#..|$d.
+000030a0: 1900 7c23 1800 1b00 7c21 1400 1800 6e02  ..|#....|!....n.
+000030b0: 7c2d 7d2d 7c2c 7c24 6408 1900 6b04 9004  |-}-|,|$d...k...
+000030c0: 72e2 7c2c 7c22 6b00 9004 72e2 7c2d 7c22  r.|,|"k...r.|-|"
+000030d0: 7c2c 1800 7c22 7c24 6408 1900 1800 1b00  |,..|"|$d.......
+000030e0: 7c21 1400 1800 6e02 7c2d 7d2d 740b 7c26  |!....n.|-}-t.|&
+000030f0: 7c28 7c29 1700 7c2b 1800 7c2d 1700 7c25  |(|)..|+..|-..|%
+00003100: 6404 1900 7c06 7c27 1900 6404 1900 6602  d...|.|'..d...f.
+00003110: 6602 8302 0100 7401 7c26 8301 7c1e 6b04  f.....t.|&..|.k.
+00003120: 9005 7226 740c 7c26 8301 0100 7c27 6408  ..r&t.|&....|'d.
+00003130: 3700 7d27 9003 7158 7c26 9003 7242 740c  7.}'..qX|&..rBt.
+00003140: 7c26 8301 7d2e 7c2e 6404 1900 740a 6419  |&..}.|.d...t.d.
+00003150: 8301 6b03 9005 7232 7c1c a008 7c2e 6408  ..k...r2|...|.d.
+00003160: 1900 6404 1900 7c2e 6408 1900 6408 1900  ..d...|.d...d...
+00003170: 7c2e 6404 1900 6603 a101 0100 9005 7132  |.d...f.......q2
+00003180: 9003 7142 7c1b 4400 9002 5d34 7d25 6700  ..qB|.D...]4}%g.
+00003190: 7d26 7c25 6404 1900 6408 1800 7d27 7c27  }&|%d...d...}'|'
+000031a0: 6404 6b05 9007 726e 7c25 6404 1900 7c05  d.k...rn|%d...|.
+000031b0: 7c27 1900 6404 1900 1800 7c20 6b00 9007  |'..d.....| k...
+000031c0: 726e 7c05 7c27 1900 6408 1900 7c06 7c25  rn|.|'..d...|.|%
+000031d0: 6404 1900 1900 6408 1900 1700 7d28 7c09  d.....d.....}(|.
+000031e0: 7c0c 7c25 6404 1900 1900 7c0c 7c05 7c27  |.|%d.....|.|.|'
+000031f0: 1900 6404 1900 1900 1800 1400 7c25 6404  ..d.........|%d.
+00003200: 1900 7c05 7c27 1900 6404 1900 1800 1b00  ..|.|'..d.......
+00003210: 7d29 7c0d 7c25 6404 1900 1900 7c0d 7c05  })|.|%d.....|.|.
+00003220: 7c27 1900 6404 1900 1900 1800 7d2a 7c2a  |'..d.......}*|*
+00003230: 7c25 6404 1900 7c05 7c27 1900 6404 1900  |%d...|.|'..d...
+00003240: 1800 7c1f 1400 6b05 9006 7252 7c27 6408  ..|...k...rR|'d.
+00003250: 3800 7d27 9005 7198 7c09 7c2a 1400 7c25  8.}'..q.|.|*..|%
+00003260: 6404 1900 7c05 7c27 1900 6404 1900 1800  d...|.|'..d.....
+00003270: 1b00 7d2b 7c04 7c25 6404 1900 1900 6409  ..}+|.|%d.....d.
+00003280: 1900 7c04 7c05 7c27 1900 6404 1900 1900  ..|.|.|'..d.....
+00003290: 6409 1900 1800 7d2c 7c2c 7c22 6b05 9006  d.....},|,|"k...
+000032a0: 73a6 7c2c 7c23 6b01 9006 72ae 740a 6419  s.|,|#k...r.t.d.
+000032b0: 8301 6e02 7c21 7d2d 7c2c 7c24 6404 1900  ..n.|!}-|,|$d...
+000032c0: 6b00 9006 72e6 7c2c 7c23 6b04 9006 72e6  k...r.|,|#k...r.
+000032d0: 7c2d 7c2c 7c23 1800 7c24 6404 1900 7c23  |-|,|#..|$d...|#
+000032e0: 1800 1b00 7c21 1400 1800 6e02 7c2d 7d2d  ....|!....n.|-}-
+000032f0: 7c2c 7c24 6408 1900 6b04 9007 721e 7c2c  |,|$d...k...r.|,
+00003300: 7c22 6b00 9007 721e 7c2d 7c22 7c2c 1800  |"k...r.|-|"|,..
+00003310: 7c22 7c24 6408 1900 1800 1b00 7c21 1400  |"|$d.......|!..
+00003320: 1800 6e02 7c2d 7d2d 740b 7c26 7c28 7c29  ..n.|-}-t.|&|(|)
+00003330: 1700 7c2b 1800 7c2d 1700 7c05 7c27 1900  ..|+..|-..|.|'..
+00003340: 6404 1900 7c25 6404 1900 6602 6602 8302  d...|%d...f.f...
+00003350: 0100 7401 7c26 8301 7c1e 6b04 9007 7262  ..t.|&..|.k...rb
+00003360: 740c 7c26 8301 0100 7c27 6408 3800 7d27  t.|&....|'d.8.}'
+00003370: 9005 7198 7c26 9005 7282 740c 7c26 8301  ..q.|&..r.t.|&..
+00003380: 7d2e 7c2e 6404 1900 740a 6419 8301 6b03  }.|.d...t.d...k.
+00003390: 9007 726e 7c1d a008 7c2e 6408 1900 6404  ..rn|...|.d...d.
+000033a0: 1900 7c2e 6408 1900 6408 1900 7c2e 6404  ..|.d...d...|.d.
+000033b0: 1900 6603 a101 0100 9007 716e 9005 7182  ..f.......qn..q.
+000033c0: 7c1c 7c1d 1700 7d2f 7c2f 5300 291a 61f6  |.|...}/|/S.).a.
+000033d0: 0b00 000a 2020 2020 5370 6c69 7420 7468  ....    Split th
+000033e0: 6520 6c6f 6e67 2061 6c69 676e 6564 2071  e long aligned q
+000033f0: 7565 7279 2069 6e74 6f20 736d 616c 6c65  uery into smalle
+00003400: 7220 7365 676d 656e 7473 2e0a 0a20 2020  r segments...   
+00003410: 2077 6520 6372 6561 7465 2073 636f 7265   we create score
+00003420: 7320 666f 7220 6561 6368 2070 6f73 6974  s for each posit
+00003430: 696f 6e20 696e 2074 6865 2061 6c69 676e  ion in the align
+00003440: 6d65 6e74 2c20 636f 7272 6573 706f 6e64  ment, correspond
+00003450: 696e 6720 746f 2068 6f77 2067 6f6f 640a  ing to how good.
+00003460: 2020 2020 6120 706f 7369 7469 6f6e 2069      a position i
+00003470: 7420 6973 2074 6f20 6265 6769 6e20 6f72  t is to begin or
+00003480: 2065 6e64 2061 2073 706c 6974 2e0a 0a20   end a split... 
+00003490: 2020 2020 2d20 6265 6769 6e20 6120 7370      - begin a sp
+000034a0: 6c69 7420 2869 2e65 2e20 7468 6973 2069  lit (i.e. this i
+000034b0: 7320 6669 7273 7420 706f 7369 7469 6f6e  s first position
+000034c0: 2069 6e20 6120 7365 676d 656e 7429 0a20   in a segment). 
+000034d0: 2020 2020 2020 202d 2070 6c75 7320 7363         - plus sc
+000034e0: 6f72 6520 6571 7561 6c20 746f 206e 756d  ore equal to num
+000034f0: 2073 696c 656e 6365 2073 6563 6f6e 6473   silence seconds
+00003500: 2074 6869 730a 2020 2020 2020 2020 2020   this.          
+00003510: 666f 6c6c 6f77 732c 2075 7020 746f 2073  follows, up to s
+00003520: 6f6d 6520 6c69 6d69 7420 3320 7365 636f  ome limit 3 seco
+00003530: 6e64 732c 2069 2e65 2e20 7468 6973 2065  nds, i.e. this e
+00003540: 6c65 6d65 6e74 0a20 2020 2020 2020 2020  lement.         
+00003550: 206f 6620 7468 6520 5472 616e 7363 7269   of the Transcri
+00003560: 7074 2773 2074 696d 6520 6d69 6e75 7320  pt's time minus 
+00003570: 7468 6520 7072 6576 696f 7573 2065 6c65  the previous ele
+00003580: 6d65 6e74 2773 2074 696d 653b 206f 7220  ment's time; or 
+00003590: 736f 6d65 2064 6566 6175 6c74 2028 332e  some default (3.
+000035a0: 3020 7365 6329 0a20 2020 2020 2020 2020  0 sec).         
+000035b0: 2069 6620 7468 6973 2069 7320 7468 6520   if this is the 
+000035c0: 6669 7273 7420 656c 656d 656e 7420 6f66  first element of
+000035d0: 2074 6865 2054 7261 6e73 6372 6970 742e   the Transcript.
+000035e0: 0a20 2020 2020 2020 202d 2067 6f6f 6420  .        - good 
+000035f0: 6966 2074 6865 7265 2061 7265 2066 6577  if there are few
+00003600: 2065 7272 6f72 7320 6172 6f75 6e64 2074   errors around t
+00003610: 6869 7320 706f 696e 7420 696e 2074 6865  his point in the
+00003620: 2061 6c69 676e 6d65 6e74 2c20 692e 652e   alignment, i.e.
+00003630: 0a20 2020 2020 2020 2020 2073 636f 7265  .          score
+00003640: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+00003650: 6f20 6e75 6d62 6572 206f 6620 696e 732c  o number of ins,
+00003660: 6465 6c2c 6d69 736d 6174 6368 2077 6974  del,mismatch wit
+00003670: 6869 6e20 6120 6365 7274 6169 6e0a 2020  hin a certain.  
+00003680: 2020 2020 2020 2020 7265 6769 6f6e 206f          region o
+00003690: 6620 7468 6973 2070 6f73 6974 696f 6e2e  f this position.
+000036a0: 0a20 2020 2020 2020 202d 2067 6f6f 6420  .        - good 
+000036b0: 6966 2074 6865 2070 7265 7669 6f75 7320  if the previous 
+000036c0: 6e6f 6e2d 7768 6974 6573 7061 6365 2063  non-whitespace c
+000036d0: 6861 7261 6374 6572 2077 6173 2061 2070  haracter was a p
+000036e0: 756e 6374 7561 7469 6f6e 0a20 2020 2020  unctuation.     
+000036f0: 2020 2020 2063 6861 7261 6374 6572 2e20       character. 
+00003700: 2028 4c69 7374 7320 6f66 2077 6869 7465   (Lists of white
+00003710: 7370 6163 6520 616e 6420 7075 6e63 7475  space and punctu
+00003720: 6174 696f 6e20 6368 6172 6163 7465 7273  ation characters
+00003730: 2077 696c 6c0a 2020 2020 2020 2020 2020   will.          
+00003740: 6265 2070 6173 7365 6420 696e 290a 0a20  be passed in).. 
+00003750: 2020 2020 2d20 656e 6420 6120 7370 6c69      - end a spli
+00003760: 7420 2869 2e65 2e20 7468 6973 2069 7320  t (i.e. this is 
+00003770: 7468 6520 6c61 7374 2070 6f73 6974 696f  the last positio
+00003780: 6e20 696e 2061 2073 6567 6d65 6e74 292e  n in a segment).
+00003790: 0a20 2020 2020 2020 202d 2070 6c75 7320  .        - plus 
+000037a0: 7363 6f72 6520 6571 7561 6c20 746f 206e  score equal to n
+000037b0: 756d 6265 7220 6f66 2073 696c 656e 6365  umber of silence
+000037c0: 2073 6563 6f6e 6473 2066 6f6c 6c6f 7773   seconds follows
+000037d0: 2074 6869 7320 706f 7369 7469 6f6e 2c20   this position, 
+000037e0: 7570 2074 6f20 736f 6d65 0a20 2020 2020  up to some.     
+000037f0: 2020 2020 206c 696d 6974 2033 2073 6563       limit 3 sec
+00003800: 6f6e 6473 2c20 692e 6520 6e65 7874 2065  onds, i.e next e
+00003810: 6c65 6d65 6e74 206f 6620 7468 6520 5472  lement of the Tr
+00003820: 616e 7363 7269 7074 2773 2074 696d 6520  anscript's time 
+00003830: 6d69 6e75 7320 7468 6973 2065 6c65 6d65  minus this eleme
+00003840: 6e74 2773 0a20 2020 2020 2020 2020 2074  nt's.          t
+00003850: 696d 653b 206f 7220 736f 6d65 2064 6566  ime; or some def
+00003860: 6175 6c74 2028 332e 3020 7365 6329 2069  ault (3.0 sec) i
+00003870: 6620 7468 6973 2069 7320 7468 6520 6c61  f this is the la
+00003880: 7374 2065 6c65 6d65 6e74 206f 6620 7468  st element of th
+00003890: 6520 5472 616e 7363 7269 7074 2e0a 2020  e Transcript..  
+000038a0: 2020 2020 2020 2d20 676f 6f64 2069 6620        - good if 
+000038b0: 7468 6572 6520 6172 6520 6665 7720 6572  there are few er
+000038c0: 726f 7273 2061 726f 756e 6420 7468 6973  rors around this
+000038d0: 2070 6f69 6e74 2069 6e20 7468 6520 616c   point in the al
+000038e0: 6967 6e6d 656e 742c 2069 2e65 2e0a 2020  ignment, i.e..  
+000038f0: 2020 2020 2020 2020 7363 6f72 6520 636f          score co
+00003900: 7272 6573 706f 6e64 696e 6720 746f 206e  rresponding to n
+00003910: 756d 6265 7220 6f66 2069 6e73 2c64 656c  umber of ins,del
+00003920: 2c6d 6973 6d61 7463 6820 7769 7468 696e  ,mismatch within
+00003930: 2061 2063 6572 7461 696e 0a20 2020 2020   a certain.     
+00003940: 2020 2020 2072 6567 696f 6e20 6f66 2074       region of t
+00003950: 6869 7320 706f 7369 7469 6f6e 2e0a 2020  his position..  
+00003960: 2020 2020 2020 2d20 676f 6f64 2069 6620        - good if 
+00003970: 7468 6520 666f 6c6c 6f77 696e 6720 6e6f  the following no
+00003980: 6e2d 7768 6974 6573 7061 6365 2063 6861  n-whitespace cha
+00003990: 7261 6374 6572 2069 7320 6120 7075 6e63  racter is a punc
+000039a0: 7475 6174 696f 6e20 6368 6172 6163 7465  tuation characte
+000039b0: 722e 0a0a 0a20 2020 2057 6520 7468 656e  r....    We then
+000039c0: 2063 7265 6174 6520 6120 7275 6c65 2074   create a rule t
+000039d0: 6f20 6173 7369 676e 2073 636f 7265 7320  o assign scores 
+000039e0: 746f 2070 6f74 656e 7469 616c 2073 6567  to potential seg
+000039f0: 6d65 6e74 732e 2054 6869 7320 636f 6e73  ments. This cons
+00003a00: 6973 7420 6f66 0a20 2020 2074 6865 2062  ist of.    the b
+00003a10: 6567 696e 2d73 636f 7265 732c 2070 6c75  egin-scores, plu
+00003a20: 7320 7468 6520 656e 642d 7363 6f72 6573  s the end-scores
+00003a30: 2c20 706c 7573 3a0a 2020 2020 2020 2d20  , plus:.      - 
+00003a40: 536f 6d65 206b 696e 6420 6f66 2070 656e  Some kind of pen
+00003a50: 616c 7479 2072 656c 6174 6564 2074 6f20  alty related to 
+00003a60: 7468 6520 6475 7261 7469 6f6e 206f 6620  the duration of 
+00003a70: 7468 6520 7365 676d 656e 742c 2065 2e67  the segment, e.g
+00003a80: 2e0a 2020 2020 2020 2020 696e 6669 6e69  ..        infini
+00003a90: 7479 2069 6620 6974 2773 206f 7665 7220  ty if it's over 
+00003aa0: 736f 6d65 206d 6178 2d64 7572 6174 696f  some max-duratio
+00003ab0: 6e20 6c69 6b65 2033 3020 7365 636f 6e64  n like 30 second
+00003ac0: 7320 6f72 206c 6573 7320 7468 616e 2061  s or less than a
+00003ad0: 0a20 2020 2020 2020 206d 696e 2d64 7572  .        min-dur
+00003ae0: 6174 696f 6e20 6c69 6b65 2032 2073 6563  ation like 2 sec
+00003af0: 6f6e 6473 3b20 656c 7365 2c20 6f6e 6520  onds; else, one 
+00003b00: 7468 6174 2065 6e63 6f75 7261 6765 7320  that encourages 
+00003b10: 6120 6475 7261 7469 6f6e 2062 6574 7765  a duration betwe
+00003b20: 656e 0a20 2020 2020 2020 2035 2074 6f20  en.        5 to 
+00003b30: 3230 2073 6563 6f6e 6473 2e0a 2020 2020  20 seconds..    
+00003b40: 2020 2d20 4120 626f 6e75 7320 666f 7220    - A bonus for 
+00003b50: 7468 6520 6e75 6d62 6572 206f 6620 6d61  the number of ma
+00003b60: 7463 6865 7320 696e 2074 6865 2061 6c69  tches in the ali
+00003b70: 676e 6d65 6e74 2e0a 2020 2020 2020 2d20  gnment..      - 
+00003b80: 4120 7065 6e61 6c74 7920 666f 7220 7468  A penalty for th
+00003b90: 6520 6e75 6d62 6572 206f 6620 6572 726f  e number of erro
+00003ba0: 7273 2069 6e20 7468 6520 616c 6967 6e6d  rs in the alignm
+00003bb0: 656e 7420 2863 6f75 6c64 206d 756c 7469  ent (could multi
+00003bc0: 706c 7920 7468 6973 2062 790a 2020 2020  ply this by.    
+00003bd0: 2020 2020 736f 6d65 2073 6361 6c65 2064      some scale d
+00003be0: 6570 656e 6469 6e67 2068 6f77 206d 7563  epending how muc
+00003bf0: 6820 7765 2064 6f6e 2774 2077 616e 7420  h we don't want 
+00003c00: 746f 2068 6176 6520 6572 726f 7273 2c20  to have errors, 
+00003c10: 6275 7420 736f 6d65 2065 7272 6f72 730a  but some errors.
+00003c20: 2020 2020 2020 2020 6172 6520 6578 7065          are expe
+00003c30: 6374 6564 2064 7565 2074 6f20 626f 7468  cted due to both
+00003c40: 2041 5352 2065 7272 6f72 7320 616e 6420   ASR errors and 
+00003c50: 6e6f 726d 616c 697a 6174 696f 6e20 6469  normalization di
+00003c60: 6666 6572 656e 6365 732e 290a 0a20 2020  fferences.)..   
+00003c70: 204e 6578 742c 2077 6520 6361 6e20 646f   Next, we can do
+00003c80: 2061 2073 6561 7263 6820 666f 7220 6120   a search for a 
+00003c90: 676f 6f64 2073 6567 6d65 6e74 6174 696f  good segmentatio
+00003ca0: 6e2e 2020 596f 7520 636f 756c 6420 6465  n.  You could de
+00003cb0: 6669 6e65 2074 6865 2070 726f 626c 656d  fine the problem
+00003cc0: 0a20 2020 2061 7320 6765 7474 696e 6720  .    as getting 
+00003cd0: 7468 6520 6869 6768 6573 742d 7363 6f72  the highest-scor
+00003ce0: 696e 6720 7365 7420 6f66 2073 6567 6d65  ing set of segme
+00003cf0: 6e74 7320 7468 6174 2064 6f20 6e6f 7420  nts that do not 
+00003d00: 6f76 6572 6c61 702e 2020 4f6e 650a 2020  overlap.  One.  
+00003d10: 2020 706f 7373 6962 6c65 2077 6179 2074    possible way t
+00003d20: 6f20 646f 2069 7420 6973 2061 7320 666f  o do it is as fo
+00003d30: 6c6c 6f77 733a 0a20 2020 2020 2020 466f  llows:.       Fo
+00003d40: 7220 6561 6368 2062 6567 696e 5f70 6f73  r each begin_pos
+00003d50: 6974 696f 6e20 696e 2074 6865 2074 6f70  ition in the top
+00003d60: 2031 3025 206f 6620 7363 6f72 6573 2c20   10% of scores, 
+00003d70: 6669 6e64 2074 6865 2034 2062 6573 742d  find the 4 best-
+00003d80: 7363 6f72 696e 6720 656e 645f 706f 7369  scoring end_posi
+00003d90: 7469 6f6e 730a 2020 2020 2020 2046 6f72  tions.       For
+00003da0: 2065 6163 6820 656e 645f 706f 7369 7469   each end_positi
+00003db0: 6f6e 2069 6e20 7468 6520 746f 7020 3130  on in the top 10
+00003dc0: 2520 6f66 2073 636f 7265 732c 2066 696e  % of scores, fin
+00003dd0: 6420 7468 6520 3420 6265 7374 2d73 636f  d the 4 best-sco
+00003de0: 7269 6e67 2062 6567 696e 5f70 6f73 6974  ring begin_posit
+00003df0: 696f 6e73 0a20 2020 2041 7070 656e 6420  ions.    Append 
+00003e00: 7468 6520 7072 6563 6564 696e 6720 3220  the preceding 2 
+00003e10: 7365 7473 206f 6620 7365 676d 656e 7473  sets of segments
+00003e20: 2074 6f20 6765 7420 6120 6c69 7374 206f   to get a list o
+00003e30: 6620 6361 6e64 6964 6174 6520 7365 676d  f candidate segm
+00003e40: 656e 7473 2e0a 0a20 2020 2041 7267 733a  ents...    Args:
+00003e50: 0a20 2020 2020 2074 6172 6765 745f 736f  .      target_so
+00003e60: 7572 6365 3a0a 2020 2020 2020 2020 4120  urce:.        A 
+00003e70: 5465 7874 536f 7572 6365 2063 6f6e 7461  TextSource conta
+00003e80: 696e 696e 6720 7468 6520 6d61 7463 6865  ining the matche
+00003e90: 6420 7265 6665 7265 6e63 652e 0a20 2020  d reference..   
+00003ea0: 2020 2061 6c69 676e 6d65 6e74 3a0a 2020     alignment:.  
+00003eb0: 2020 2020 2020 416c 6967 6e6d 656e 7420        Alignment 
+00003ec0: 696e 666f 726d 6174 696f 6e2c 206f 6e65  information, one
+00003ed0: 2069 7465 6d20 6f66 2074 6865 2072 6574   item of the ret
+00003ee0: 7572 6e65 6420 616c 6967 6e6d 656e 7473  urned alignments
+00003ef0: 2066 726f 6d20 6067 6574 5f61 6c69 676e   from `get_align
+00003f00: 6d65 6e74 7360 2e0a 0a20 2020 2052 6574  ments`...    Ret
+00003f10: 7572 6e73 3a0a 2020 2020 2020 5265 7475  urns:.      Retu
+00003f20: 726e 7320 6120 6c69 7374 206f 6620 7475  rns a list of tu
+00003f30: 706c 652c 2065 6163 6820 7475 706c 6520  ple, each tuple 
+00003f40: 636f 6e74 6169 6e73 2074 6865 2073 7461  contains the sta
+00003f50: 7274 2070 6f73 6974 696f 6e2c 2065 6e64  rt position, end
+00003f60: 2070 6f73 6974 696f 6e20 616e 6420 7363   position and sc
+00003f70: 6f72 6520 6f66 0a20 2020 2020 2063 7572  ore of.      cur
+00003f80: 7265 6e74 2073 6567 6d65 6e74 2c20 7374  rent segment, st
+00003f90: 6172 7420 706f 7369 7469 6f6e 2061 6e64  art position and
+00003fa0: 2065 6e64 2070 6f73 6974 696f 6e20 6172   end position ar
+00003fb0: 6520 696e 6465 7865 7320 696e 2061 6c69  e indexes in ali
+00003fc0: 676e 732e 0a20 2020 20e9 1400 0000 6301  gns..    .....c.
+00003fd0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00003fe0: 0000 0053 0000 0073 2400 0000 6700 7c00  ...S...s$...g.|.
+00003ff0: 5d1c 7d01 7c01 6400 1900 7c01 6401 1900  ].}.|.d...|.d...
+00004000: 6b03 721c 6402 6e02 6403 9102 7104 5300  k.r.d.n.d...q.S.
+00004010: 2904 7248 0000 0072 4900 0000 720f 0000  ).rH...rI...r...
+00004020: 0072 0100 0000 7222 0000 0029 0272 6400  .r....r"...).rd.
+00004030: 0000 da05 616c 6967 6e72 2200 0000 7222  ....alignr"...r"
+00004040: 0000 0072 2300 0000 7266 0000 003e 0200  ...r#...rf...>..
+00004050: 0073 0400 0000 0602 02ff 7a2b 5f67 6574  .s........z+_get
+00004060: 5f73 6567 6d65 6e74 5f63 616e 6469 6461  _segment_candida
+00004070: 7465 732e 3c6c 6f63 616c 733e 2e3c 6c69  tes.<locals>.<li
+00004080: 7374 636f 6d70 3e72 0100 0000 7267 0000  stcomp>r....rg..
+00004090: 0072 4800 0000 7249 0000 0072 0f00 0000  .rH...rI...r....
+000040a0: 724c 0000 0072 4a00 0000 5429 01da 0865  rL...rJ...T)...e
+000040b0: 6f73 5f6f 6e6c 79fa 0120 6301 0000 0000  os_only.. c.....
+000040c0: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
+000040d0: 0000 0073 0800 0000 7c00 6401 1900 5300  ...s....|.d...S.
+000040e0: a902 4e72 0f00 0000 7222 0000 00a9 0172  ..Nr....r".....r
+000040f0: 6500 0000 7222 0000 0072 2200 0000 7223  e...r"...r"...r#
+00004100: 0000 00da 083c 6c61 6d62 6461 3e93 0200  .....<lambda>...
+00004110: 00f3 0000 0000 7a29 5f67 6574 5f73 6567  ......z)_get_seg
+00004120: 6d65 6e74 5f63 616e 6469 6461 7465 732e  ment_candidates.
+00004130: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
+00004140: 3ea9 02da 036b 6579 da07 7265 7665 7273  >....key..revers
+00004150: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
+00004160: 0000 0200 0000 5300 0000 7308 0000 007c  ......S...s....|
+00004170: 0064 0119 0053 0072 8600 0000 7222 0000  .d...S.r....r"..
+00004180: 0072 8700 0000 7222 0000 0072 2200 0000  .r....r"...r"...
+00004190: 7223 0000 0072 8800 0000 9402 0000 7289  r#...r........r.
+000041a0: 0000 0072 2500 0000 722c 0000 0067 9a99  ...r%...r,...g..
+000041b0: 9999 9999 c93f e9e8 0300 00e9 1e00 0000  .....?..........
+000041c0: 722a 0000 0029 02e9 0500 0000 7282 0000  r*...)......r...
+000041d0: 007a 042d 696e 6629 0dda 0373 756d 7236  .z.-inf)...sumr6
+000041e0: 0000 00da 0965 6e75 6d65 7261 7465 7258  .....enumeraterX
+000041f0: 0000 0072 5a00 0000 7255 0000 0072 1500  ...rZ...rU...r..
+00004200: 0000 721d 0000 0072 2e00 0000 da06 736f  ..r....r......so
+00004210: 7274 6564 7257 0000 0072 0400 0000 7205  rtedrW...r....r.
+00004220: 0000 0029 3072 8100 0000 7244 0000 0072  ...)0r....rD...r
+00004230: 2f00 0000 7231 0000 0072 5e00 0000 5a0c  /...r1...r^...Z.
+00004240: 6265 6769 6e5f 7363 6f72 6573 5a0a 656e  begin_scoresZ.en
+00004250: 645f 7363 6f72 6573 5a10 6861 6c66 5f72  d_scoresZ.half_r
+00004260: 6567 696f 6e5f 7369 7a65 5a10 6572 726f  egion_sizeZ.erro
+00004270: 7273 5f69 6e5f 7265 6769 6f6e 5a0a 6261  rs_in_regionZ.ba
+00004280: 7365 5f73 636f 7265 5a0b 6d61 785f 7369  se_scoreZ.max_si
+00004290: 6c65 6e63 655a 1170 756e 6374 7561 7469  lenceZ.punctuati
+000042a0: 6f6e 5f73 636f 7265 5a0c 6375 6d73 756d  on_scoreZ.cumsum
+000042b0: 5f6d 6174 6368 5a0c 6375 6d73 756d 5f65  _matchZ.cumsum_e
+000042c0: 7272 6f72 7234 0000 0072 8300 0000 da07  rrorr4...r......
+000042d0: 6d61 7463 6865 645a 0c70 7265 765f 7369  matchedZ.prev_si
+000042e0: 6c65 6e63 655a 0c70 6f73 745f 7369 6c65  lenceZ.post_sile
+000042f0: 6e63 655a 1070 7265 765f 7075 6e63 7475  nceZ.prev_punctu
+00004300: 6174 696f 6eda 016a da0d 6375 7272 656e  ation..j..curren
+00004310: 745f 746f 6b65 6e5a 1070 6f73 745f 7075  t_tokenZ.post_pu
+00004320: 6e63 7475 6174 696f 6e5a 1373 6f72 7465  nctuationZ.sorte
+00004330: 645f 6265 6769 6e5f 7363 6f72 6573 5a11  d_begin_scoresZ.
+00004340: 736f 7274 6564 5f65 6e64 5f73 636f 7265  sorted_end_score
+00004350: 735a 0974 6f70 5f72 6174 696f 5a09 746f  sZ.top_ratioZ.to
+00004360: 705f 6265 6769 6e5a 0774 6f70 5f65 6e64  p_beginZ.top_end
+00004370: 5a0a 6265 6769 6e5f 6c69 7374 5a08 656e  Z.begin_listZ.en
+00004380: 645f 6c69 7374 5a14 6e75 6d5f 6f66 5f62  d_listZ.num_of_b
+00004390: 6573 745f 706f 7369 7469 6f6e 5a10 6d61  est_positionZ.ma
+000043a0: 785f 6572 726f 7273 5f72 6174 696f 5a0f  x_errors_ratioZ.
+000043b0: 6d61 785f 7465 7874 5f6c 656e 6774 685a  max_text_lengthZ
+000043c0: 1369 6e69 745f 6475 7261 7469 6f6e 5f73  .init_duration_s
+000043d0: 636f 7265 da0c 6d61 785f 6475 7261 7469  core..max_durati
+000043e0: 6f6e da0c 6d69 6e5f 6475 7261 7469 6f6e  on..min_duration
+000043f0: da11 6578 7065 6374 6564 5f64 7572 6174  ..expected_durat
+00004400: 696f 6eda 0469 7465 6d5a 0669 7465 6d5f  ion..itemZ.item_
+00004410: 7172 4000 0000 5a0b 706f 696e 745f 7363  qr@...Z.point_sc
+00004420: 6f72 655a 0d6d 6174 6368 6564 5f73 636f  oreZ.matched_sco
+00004430: 7265 5a0c 746f 7461 6c5f 6572 726f 7273  reZ.total_errors
+00004440: 5a0b 6572 726f 725f 7363 6f72 65da 0864  Z.error_score..d
+00004450: 7572 6174 696f 6e5a 0e64 7572 6174 696f  urationZ.duratio
+00004460: 6e5f 7363 6f72 6572 6500 0000 da0a 6361  n_scorere.....ca
+00004470: 6e64 6964 6174 6573 7222 0000 0072 2200  ndidatesr"...r".
+00004480: 0000 7223 0000 00da 175f 6765 745f 7365  ..r#....._get_se
+00004490: 676d 656e 745f 6361 6e64 6964 6174 6573  gment_candidates
+000044a0: f901 0000 739c 0100 0000 3b0c 0304 0104  ....s.....;.....
+000044b0: 0304 0202 0106 020a fe04 ff04 0a04 0104  ................
+000044c0: 0202 ff02 050e 010e 0212 0110 0222 ff06  ............."..
+000044d0: 0426 ff06 050e 020e 010e ff02 ff04 0408  .&..............
+000044e0: 0112 020e 010e ff02 ff04 0408 0424 ff02  .............$..
+000044f0: 0312 030e ff08 0216 fd02 0512 0304 010c  ................
+00004500: 010a 010e 010e 0104 0106 0114 010a 0208  ................
+00004510: 0204 010c 010e 010e 010e 0104 0106 0114  ................
+00004520: 010a 0208 0104 0112 ff04 0304 0112 ff06  ................
+00004530: 0412 0112 0204 0118 0118 0304 0104 0204  ................
+00004540: 0104 0104 0202 ff02 0304 0104 0104 020a  ................
+00004550: 0304 010c 0128 011c 0302 011a ff02 0212  .....(..........
+00004560: fe02 ff02 071c 021e 0108 0104 011c 0422  ..............."
+00004570: ff02 0606 ff04 0106 ff0c 0202 fd02 0b0a  ................
+00004580: fc04 0406 fc06 0106 010a ff02 0202 fe02  ................
+00004590: ff04 0502 fa02 0e0a fc04 0406 fc06 0106  ................
+000045a0: 010a ff02 0202 fe02 ff04 0502 fa02 0902  ................
+000045b0: 0102 020e 0112 fe02 fe04 070e 0108 010c  ................
+000045c0: 0106 0108 0112 012c 020a 0304 010c 0124  .......,.......$
+000045d0: 011c 0302 011a ff02 0212 fe02 ff02 071c  ................
+000045e0: 021e 0108 0104 011c 0422 ff02 0606 ff04  ........."......
+000045f0: 0106 ff0c 0202 fd02 0b0a fc04 0406 fc06  ................
+00004600: 0106 010a ff02 0202 fe02 ff04 0502 fa02  ................
+00004610: 0e0a fc04 0406 fc06 0106 010a ff02 0202  ................
+00004620: fe02 ff04 0502 fa02 0902 0102 020e 0112  ................
+00004630: fe02 fe04 070e 0108 010c 0106 0108 0112  ................
+00004640: 012c 0208 0172 9c00 0000 2903 725d 0000  .,...r....).r]..
+00004650: 0072 8100 0000 7219 0000 0063 0300 0000  .r....r....c....
+00004660: 0000 0000 0000 0000 1b00 0000 0c00 0000  ................
+00004670: 4300 0000 7326 0200 007c 025c 025c 027d  C...s&...|.\.\.}
+00004680: 037d 047d 0574 007c 017c 0264 018d 027d  .}.}.t.|.|.d...}
+00004690: 0674 017c 0664 0264 0384 0064 0464 058d  .t.|.d.d...d.d..
+000046a0: 037d 0667 007d 0767 007d 087c 0644 005d  .}.g.}.g.}.|.D.]
+000046b0: 247d 0974 027c 077c 0964 0619 007c 0964  $}.t.|.|.d...|.d
+000046c0: 0719 0066 0283 0273 367c 08a0 037c 09a1  ...f...s6|...|..
+000046d0: 0101 0071 3667 007d 0a64 087d 0b64 097d  ...q6g.}.d.}.d.}
+000046e0: 0c7c 0844 0090 015d b27d 0d7c 057c 0d64  .|.D...].}.|.|.d
+000046f0: 0619 0019 0064 0a19 007d 0e7c 057c 0d64  .....d...}.|.|.d
+00004700: 0719 0019 0064 0a19 0064 0717 007d 0f7c  .....d...d...}.|
+00004710: 0d64 0619 0064 066b 0272 aa7c 0d64 0619  .d...d.k.r.|.d..
+00004720: 006e 0a7c 0d64 0619 0064 0718 007d 107c  .n.|.d...d...}.|
+00004730: 057c 0d64 0619 0019 0064 0b19 007d 117c  .|.d.....d...}.|
+00004740: 0d64 0719 0074 047c 0583 0164 0718 006b  .d...t.|...d...k
+00004750: 0272 e27c 0d64 0719 006e 0a7c 0d64 0719  .r.|.d...n.|.d..
+00004760: 0064 0717 007d 127c 057c 1219 0064 0b19  .d...}.|.|...d..
+00004770: 007c 057c 0d64 0719 0019 0064 0b19 0017  .|.|.d.....d....
+00004780: 0064 0c1b 007c 1118 007d 137c 057c 0d64  .d...|...}.|.|.d
+00004790: 0619 0019 0064 0d19 007d 147c 057c 0d64  .....d...}.|.|.d
+000047a0: 0719 0019 0064 0d19 0064 0717 007d 1564  .....d...d...}.d
+000047b0: 0ea0 0564 0f64 1084 007c 006a 067c 147c  ...d.d...|.j.|.|
+000047c0: 1585 0219 0044 0083 01a1 017d 1674 047c  .....D.....}.t.|
+000047d0: 1683 017c 0b6b 0090 0172 6471 6c64 0ea0  ...|.k...rdqld..
+000047e0: 0564 1164 1084 007c 016a 067c 0e7c 0f64  .d.d...|.j.|.|.d
+000047f0: 0717 0085 0219 0044 0083 01a1 017d 177c  .......D.....}.|
+00004800: 0e7c 0c18 0064 066b 0590 0172 9c7c 0e7c  .|...d.k...r.|.|
+00004810: 0c18 006e 0264 067d 1864 0ea0 0564 1264  ...n.d.}.d...d.d
+00004820: 1084 007c 016a 067c 187c 0e85 0219 0044  ...|.j.|.|.....D
+00004830: 0083 01a1 017d 197c 147c 0c18 0064 066b  .....}.|.|...d.k
+00004840: 0490 0172 d47c 147c 0c18 006e 0264 067d  ...r.|.|...n.d.}
+00004850: 1864 0ea0 0564 1364 1084 007c 006a 067c  .d...d.d...|.j.|
+00004860: 187c 1485 0219 0044 0083 01a1 017d 1a7c  .|.....D.....}.|
+00004870: 0aa0 037c 0e7c 0f7c 1174 07a0 0864 097c  ...|.|.|.t...d.|
+00004880: 1314 00a1 0164 091b 007c 167c 177c 197c  .....d...|.|.|.|
+00004890: 1a64 149c 08a1 0101 0071 6c7c 0a53 0029  .d.......ql|.S.)
+000048a0: 1561 b302 0000 0a20 2020 2053 706c 6974  .a.....    Split
+000048b0: 2061 206c 6f6e 6720 616c 6967 6e65 6420   a long aligned 
+000048c0: 7175 6572 7920 696e 746f 2073 6d61 6c6c  query into small
+000048d0: 6572 2073 6567 6d65 6e74 732e 0a0a 2020  er segments...  
+000048e0: 2020 5765 2077 696c 6c20 6372 6561 7465    We will create
+000048f0: 2073 636f 7265 7320 666f 7220 6561 6368   scores for each
+00004900: 2070 6f73 6974 696f 6e20 696e 2074 6865   position in the
+00004910: 2061 6c69 676e 6d65 6e74 2c20 636f 7272   alignment, corr
+00004920: 6573 706f 6e64 696e 6720 746f 2068 6f77  esponding to how
+00004930: 2067 6f6f 640a 2020 2020 6120 706f 7369   good.    a posi
+00004940: 7469 6f6e 2069 7420 6973 2074 6f20 6265  tion it is to be
+00004950: 6769 6e20 6f72 2065 6e64 2061 2073 706c  gin or end a spl
+00004960: 6974 2e20 5765 2063 616e 2074 6865 6e20  it. We can then 
+00004970: 6372 6561 7465 2061 2072 756c 6520 746f  create a rule to
+00004980: 2061 7373 6967 6e20 7363 6f72 6573 0a20   assign scores. 
+00004990: 2020 2074 6f20 706f 7465 6e74 6961 6c20     to potential 
+000049a0: 7365 676d 656e 7473 2e20 5468 6520 7363  segments. The sc
+000049b0: 6f72 6573 2077 6f75 6c64 2063 6f6e 7369  ores would consi
+000049c0: 7374 206f 6620 7468 6520 6265 6769 6e2d  st of the begin-
+000049d0: 7363 6f72 6573 2c20 706c 7573 2074 6865  scores, plus the
+000049e0: 2065 6e64 2d73 636f 7265 732c 0a20 2020   end-scores,.   
+000049f0: 2070 6c75 7320 736f 6d65 206b 696e 6420   plus some kind 
+00004a00: 6f66 2073 636f 7265 7320 6f66 2067 6976  of scores of giv
+00004a10: 656e 2073 6567 6d65 6e74 2028 6475 7261  en segment (dura
+00004a20: 7469 6f6e 2c20 6d61 7463 6869 6e67 2065  tion, matching e
+00004a30: 7272 6f72 7320 2e65 7463 292e 0a0a 2020  rrors .etc)...  
+00004a40: 2020 4172 6773 3a0a 2020 2020 2020 7175    Args:.      qu
+00004a50: 6572 795f 736f 7572 6365 3a0a 2020 2020  ery_source:.    
+00004a60: 2020 2020 416e 2069 6e73 7461 6e63 6520      An instance 
+00004a70: 6f66 2054 7261 6e73 6372 6970 7420 6f72  of Transcript or
+00004a80: 2054 6578 7453 6f75 7263 6520 636f 6e74   TextSource cont
+00004a90: 6169 6e69 6e67 2074 6865 2071 7565 7279  aining the query
+00004aa0: 2e0a 2020 2020 2020 7461 7267 6574 5f73  ..      target_s
+00004ab0: 6f75 7263 653a 0a20 2020 2020 2020 2041  ource:.        A
+00004ac0: 6e20 696e 7374 616e 6365 206f 6620 5465  n instance of Te
+00004ad0: 7874 536f 7572 6365 2063 6f6e 7461 696e  xtSource contain
+00004ae0: 696e 6720 7468 6520 6d61 7463 6865 6420  ing the matched 
+00004af0: 7265 6665 7265 6e63 652e 0a20 2020 2020  reference..     
+00004b00: 2061 6c69 676e 6d65 6e74 3a0a 2020 2020   alignment:.    
+00004b10: 2020 2020 5468 6520 616c 6967 6e6d 656e      The alignmen
+00004b20: 742c 2061 6e20 6974 656d 2069 6e20 7468  t, an item in th
+00004b30: 6520 6c69 7374 2072 6574 7572 6e65 6420  e list returned 
+00004b40: 6279 2060 6765 745f 616c 6967 6e6d 656e  by `get_alignmen
+00004b50: 7473 602e 0a20 2020 2029 0272 8100 0000  ts`..    ).r....
+00004b60: 7244 0000 0063 0100 0000 0000 0000 0000  rD...c..........
+00004b70: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
+00004b80: 0000 007c 0064 0119 0053 0029 024e 722a  ...|.d...S.).Nr*
+00004b90: 0000 0072 2200 0000 7287 0000 0072 2200  ...r"...r....r".
+00004ba0: 0000 7222 0000 0072 2300 0000 7288 0000  ..r"...r#...r...
+00004bb0: 004a 0300 0072 8900 0000 7a25 7370 6c69  .J...r....z%spli
+00004bc0: 745f 696e 746f 5f73 6567 6d65 6e74 732e  t_into_segments.
+00004bd0: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
+00004be0: 3e54 728a 0000 0072 0100 0000 720f 0000  >Tr....r....r...
+00004bf0: 0072 8e00 0000 728d 0000 0072 4a00 0000  .r....r....rJ...
+00004c00: 724c 0000 0072 2a00 0000 724b 0000 0072  rL...r*...rK...r
+00004c10: 4700 0000 6301 0000 0000 0000 0000 0000  G...c...........
+00004c20: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
+00004c30: 0000 6700 7c00 5d0c 7d01 7400 7c01 8301  ..g.|.].}.t.|...
+00004c40: 9102 7104 5300 7222 0000 00a9 0172 5a00  ..q.S.r".....rZ.
+00004c50: 0000 a902 7264 0000 0072 3400 0000 7222  ....rd...r4...r"
+00004c60: 0000 0072 2200 0000 7223 0000 0072 6600  ...r"...r#...rf.
+00004c70: 0000 6d03 0000 7304 0000 0006 0002 007a  ..m...s........z
+00004c80: 2773 706c 6974 5f69 6e74 6f5f 7365 676d  'split_into_segm
+00004c90: 656e 7473 2e3c 6c6f 6361 6c73 3e2e 3c6c  ents.<locals>.<l
+00004ca0: 6973 7463 6f6d 703e 6301 0000 0000 0000  istcomp>c.......
+00004cb0: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00004cc0: 0073 1400 0000 6700 7c00 5d0c 7d01 7400  .s....g.|.].}.t.
+00004cd0: 7c01 8301 9102 7104 5300 7222 0000 0072  |.....q.S.r"...r
+00004ce0: 9d00 0000 729e 0000 0072 2200 0000 7222  ....r....r"...r"
+00004cf0: 0000 0072 2300 0000 7266 0000 0077 0300  ...r#...rf...w..
+00004d00: 0073 0400 0000 0600 0200 6301 0000 0000  .s........c.....
+00004d10: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00004d20: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
+00004d30: 7400 7c01 8301 9102 7104 5300 7222 0000  t.|.....q.S.r"..
+00004d40: 0072 9d00 0000 729e 0000 0072 2200 0000  .r....r....r"...
+00004d50: 7222 0000 0072 2300 0000 7266 0000 0081  r"...r#...rf....
+00004d60: 0300 0073 0400 0000 0600 0200 6301 0000  ...s........c...
+00004d70: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00004d80: 0053 0000 0073 1400 0000 6700 7c00 5d0c  .S...s....g.|.].
+00004d90: 7d01 7400 7c01 8301 9102 7104 5300 7222  }.t.|.....q.S.r"
+00004da0: 0000 0072 9d00 0000 729e 0000 0072 2200  ...r....r....r".
+00004db0: 0000 7222 0000 0072 2300 0000 7266 0000  ..r"...r#...rf..
+00004dc0: 008a 0300 0073 0400 0000 0600 0200 2908  .....s........).
+00004dd0: da0a 6265 6769 6e5f 6279 7465 da08 656e  ..begin_byte..en
+00004de0: 645f 6279 7465 da0a 7374 6172 745f 7469  d_byte..start_ti
+00004df0: 6d65 729a 0000 0072 4900 0000 7248 0000  mer....rI...rH..
+00004e00: 00da 0770 7265 5f72 6566 da07 7072 655f  ...pre_ref..pre_
+00004e10: 6879 7029 0972 9c00 0000 7292 0000 0072  hyp).r....r....r
+00004e20: 1400 0000 722e 0000 0072 3600 0000 da04  ....r....r6.....
+00004e30: 6a6f 696e 7255 0000 00da 046d 6174 68da  joinrU.....math.
+00004e40: 0566 6c6f 6f72 291b 725d 0000 0072 8100  .floor).r]...r..
+00004e50: 0000 7244 0000 0072 2f00 0000 7231 0000  ..rD...r/...r1..
+00004e60: 0072 5e00 0000 729b 0000 005a 0f73 656c  .r^...r....Z.sel
+00004e70: 6563 7465 645f 7261 6e67 6573 7233 0000  ected_rangesr3..
+00004e80: 00da 0172 727f 0000 005a 0f6d 696e 5f74  ...rr....Z.min_t
+00004e90: 6578 745f 6c65 6e67 7468 5a18 7072 6563  ext_lengthZ.prec
+00004ea0: 6564 696e 675f 636f 6e74 6578 745f 6c65  eding_context_le
+00004eb0: 6e67 7468 727c 0000 005a 0962 6567 696e  ngthr|...Z.begin
+00004ec0: 5f70 6f73 da07 656e 645f 706f 735a 0f70  _pos..end_posZ.p
+00004ed0: 7265 6365 6469 6e67 5f69 6e64 6578 da05  receding_index..
+00004ee0: 7374 6172 745a 0f66 6f6c 6c6f 7769 6e67  startZ.following
+00004ef0: 5f69 6e64 6578 729a 0000 005a 0d68 7970  _indexr....Z.hyp
+00004f00: 5f62 6567 696e 5f70 6f73 5a0b 6879 705f  _begin_posZ.hyp_
+00004f10: 656e 645f 706f 7372 4900 0000 7248 0000  end_posrI...rH..
+00004f20: 005a 0970 7265 5f69 6e64 6578 72a2 0000  .Z.pre_indexr...
+00004f30: 0072 a300 0000 7222 0000 0072 2200 0000  .r....r"...r"...
+00004f40: 7223 0000 00da 1373 706c 6974 5f69 6e74  r#.....split_int
+00004f50: 6f5f 7365 676d 656e 7473 3003 0000 737a  o_segments0...sz
+00004f60: 0000 0000 130c 0302 0102 0002 ff06 0412  ................
+00004f70: 0504 0104 0108 0116 010c 0204 0104 0104  ................
+00004f80: 020a 0110 0114 0220 0410 0228 021a 0102  ....... ...(....
+00004f90: fe02 0202 fe04 0610 0114 0104 0116 ff04  ................
+00004fa0: 050e 0102 0404 011a ff04 060a ff0c 0202  ................
+00004fb0: fd02 0604 0116 ff04 060a ff0c 0202 fd02  ................
+00004fc0: 0504 0116 ff04 0404 0202 0102 0102 0110  ................
+00004fd0: 0102 0102 0102 0102 f804 ff06 0c72 aa00  .............r..
+00004fe0: 0000 e700 0000 0000 00f8 3f29 0572 6200  ..........?).rb.
+00004ff0: 0000 da04 7465 7874 da0c 6c65 6e67 7468  ....text..length
+00005000: 5f72 6174 696f da0e 6e75 6d5f 6361 6e64  _ratio..num_cand
+00005010: 6964 6174 6573 7219 0000 0063 0400 0000  idatesr....c....
+00005020: 0000 0000 0000 0000 1900 0000 0700 0000  ................
+00005030: 4300 0000 7302 0200 007c 006a 0064 016b  C...s....|.j.d.k
+00005040: 0273 1474 017c 006a 0083 0182 017c 006a  .s.t.|.j.....|.j
+00005050: 025c 027d 047d 057c 016a 036a 047c 046b  .\.}.}.|.j.j.|.k
+00005060: 0473 3a74 017c 016a 036a 047c 0466 0283  .s:t.|.j.j.|.f..
+00005070: 0182 017c 016a 057c 0419 007d 067c 016a  ...|.j.|...}.|.j
+00005080: 067d 0767 007d 0874 077c 0683 0144 0090  .}.g.}.t.|...D..
+00005090: 015d a47d 097c 077c 0919 007d 0a7c 077c  .].}.|.|...}.|.|
+000050a0: 0964 0217 0019 007d 0b7c 077c 0964 0217  .d.....}.|.|.d..
+000050b0: 0019 007c 077c 0919 0018 007d 0c7c 0c7c  ...|.|.....}.|.|
+000050c0: 0214 007d 0d74 08a0 097c 007c 0a7c 0b85  ...}.t...|.|.|..
+000050d0: 0264 0364 0385 0266 0219 00a0 0aa1 00a1  .d.d...f........
+000050e0: 017d 0e64 0467 017c 0314 007d 0f64 027d  .}.d.g.|...}.d.}
+000050f0: 1074 077c 0e6a 0483 0144 0090 015d 227d  .t.|.j...D...]"}
+00005100: 117c 016a 057c 0e7c 1119 0019 007d 127c  .|.j.|.|.....}.|
+00005110: 016a 0b7c 0e7c 1119 0019 007d 137c 107c  .j.|.|.....}.|.|
+00005120: 0e6a 046b 0090 0172 267c 016a 057c 0e7c  .j.k...r&|.j.|.|
+00005130: 1019 0019 007c 126b 0290 0172 267c 016a  .....|.k...r&|.j
+00005140: 0b7c 0e7c 1019 0019 007c 137c 0d17 006b  .|.|.....|.|...k
+00005150: 0090 0172 267c 1064 0237 007d 1071 e47c  ...r&|.d.7.}.q.|
+00005160: 0e7c 1119 007c 0e7c 1064 0218 0019 0064  .|...|.|.d.....d
+00005170: 0217 007c 107c 1118 0066 037d 147c 1464  ...|.|...f.}.|.d
+00005180: 0119 007d 1564 037d 1664 057d 1774 0c7c  ...}.d.}.d.}.t.|
+00005190: 0f83 0144 005d 5a5c 027d 117d 187c 1864  ...D.]Z\.}.}.|.d
+000051a0: 0119 007c 156b 0090 0172 7e7c 1864 0119  ...|.k...r~|.d..
+000051b0: 007d 157c 117d 167c 1464 0619 007c 1864  .}.|.}.|.d...|.d
+000051c0: 0219 006b 0090 0172 5c7c 1464 0119 007c  ...k...r\|.d...|
+000051d0: 1864 0119 006b 0490 0172 5c7c 147c 0f7c  .d...k...r\|.|.|
+000051e0: 113c 0064 077d 1701 0090 0171 b890 0171  .<.d.}.....q...q
+000051f0: 5c7c 1773 c274 0d7c 0f83 017c 036b 0090  \|.s.t.|...|.k..
+00005200: 0172 d67c 0fa0 0e7c 14a1 0101 0071 c27c  .r.|...|.....q.|
+00005210: 1664 036b 0972 c27c 147c 0f7c 163c 0071  .d.k.r.|.|.|.<.q
+00005220: c27c 08a0 0e64 0864 0984 007c 0f44 0083  .|...d.d...|.D..
+00005230: 01a1 0101 0071 567c 0853 0029 0a61 9f03  .....qV|.S.).a..
+00005240: 0000 0a20 2020 2046 696e 6420 6361 6e64  ...    Find cand
+00005250: 6964 6174 6520 7265 6769 6f6e 7320 696e  idate regions in
+00005260: 2072 6566 6572 656e 6365 2064 6f63 756d   reference docum
+00005270: 656e 7420 7468 6174 2063 6f75 6c64 2062  ent that could b
+00005280: 6520 676f 6f64 206d 6174 6368 6573 2066  e good matches f
+00005290: 6f72 0a20 2020 2065 6163 6820 7175 6572  or.    each quer
+000052a0: 7920 646f 6375 6d65 6e74 2e0a 0a20 2020  y document...   
+000052b0: 2041 7267 733a 0a20 2020 2020 2020 636c   Args:.       cl
+000052c0: 6f73 655f 6d61 7463 6865 733a 2061 6e20  ose_matches: an 
+000052d0: 6e70 2e6e 6461 7272 6179 206f 6620 7368  np.ndarray of sh
+000052e0: 6170 6520 2874 6f74 5f71 7565 7279 5f73  ape (tot_query_s
+000052f0: 796d 626f 6c73 2c20 6e75 6d5f 636c 6f73  ymbols, num_clos
+00005300: 655f 6d61 7463 6865 7329 0a20 2020 2020  e_matches).     
+00005310: 2020 2020 2061 7320 7265 7475 726e 6564       as returned
+00005320: 2062 7920 6669 6e64 5f63 6c6f 7365 5f6d   by find_close_m
+00005330: 6174 6368 6573 2829 2c20 696e 6469 6361  atches(), indica
+00005340: 7469 6e67 2074 776f 2063 6c6f 7365 206d  ting two close m
+00005350: 6174 6368 6573 2077 6974 6869 6e0a 2020  atches within.  
+00005360: 2020 2020 2020 2020 7468 6520 7265 6665          the refe
+00005370: 7265 6e63 6520 7465 7874 2066 6f72 2065  rence text for e
+00005380: 6163 6820 7379 6d62 6f6c 2069 6e20 7468  ach symbol in th
+00005390: 6520 7175 6572 7920 646f 6375 6d65 6e74  e query document
+000053a0: 732e 0a20 2020 2020 2020 7465 7874 3a20  s..       text: 
+000053b0: 2054 6865 2053 6f75 7263 6564 5465 7874   The SourcedText
+000053c0: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+000053d0: 6f20 7468 6520 7175 6572 7920 616e 6420  o the query and 
+000053e0: 7265 6665 7265 6e63 6520 646f 6375 6d65  reference docume
+000053f0: 6e74 730a 2020 2020 2020 2020 2020 636f  nts.          co
+00005400: 6d62 696e 6564 3b20 6e65 6564 6564 2066  mbined; needed f
+00005410: 6f72 2069 7473 2060 646f 6360 206d 656d  or its `doc` mem
+00005420: 6265 7220 7768 6963 6820 6361 6e20 6265  ber which can be
+00005430: 2061 7373 756d 6564 2074 6f20 6265 2061   assumed to be a
+00005440: 6e20 6e70 2e6e 6461 7272 6179 2e0a 2020  n np.ndarray..  
+00005450: 2020 2020 206c 656e 6774 685f 7261 7469       length_rati
+00005460: 6f3a 2069 6e64 6963 6174 6573 2074 6865  o: indicates the
+00005470: 206d 6178 696d 756d 2063 616e 6469 6461   maximum candida
+00005480: 7465 2d72 6567 696f 6e20 6c65 6e67 7468  te-region length
+00005490: 2c20 7768 6963 6820 7769 6c6c 2062 6520  , which will be 
+000054a0: 7265 6475 6365 640a 2020 2020 2020 2020  reduced.        
+000054b0: 2020 6966 2074 6865 206d 6174 6368 696e    if the matchin
+000054c0: 6720 7265 6665 7265 6e63 6520 646f 6375  g reference docu
+000054d0: 6d65 6e74 2077 6173 2073 686f 7274 6572  ment was shorter
+000054e0: 2074 6861 6e20 7468 6973 2e0a 2020 2020   than this..    
+000054f0: 2020 206e 756d 5f63 616e 6469 6461 7465     num_candidate
+00005500: 733a 2020 7468 6520 6e75 6d62 6572 206f  s:  the number o
+00005510: 6620 6361 6e64 6964 6174 6520 7265 6769  f candidate regi
+00005520: 6f6e 7320 746f 2066 696e 6420 666f 7220  ons to find for 
+00005530: 6561 6368 2071 7565 7279 0a20 2020 2020  each query.     
+00005540: 2020 2020 2064 6f63 756d 656e 742e 0a20       document.. 
+00005550: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00005560: 2020 2041 206c 6973 742c 206f 6e65 2070     A list, one p
+00005570: 6572 2071 7565 7279 2064 6f63 756d 656e  er query documen
+00005580: 742c 206f 6620 636c 6f73 6520 6d61 7463  t, of close matc
+00005590: 6865 732c 2077 6865 7265 2065 6163 6820  hes, where each 
+000055a0: 636c 6f73 6520 6d61 7463 680a 2020 2020  close match.    
+000055b0: 2020 2069 7320 6120 2862 6567 696e 2c20     is a (begin, 
+000055c0: 656e 6429 2070 6f73 6974 696f 6e20 7769  end) position wi
+000055d0: 7468 696e 2060 7465 7874 602e 0a20 2020  thin `text`..   
+000055e0: 2072 2a00 0000 720f 0000 004e 2903 7201   r*...r....N).r.
+000055f0: 0000 0072 0100 0000 7201 0000 0046 7201  ...r....r....Fr.
+00005600: 0000 0054 6301 0000 0000 0000 0000 0000  ...Tc...........
+00005610: 0002 0000 0005 0000 0053 0000 0073 1c00  .........S...s..
+00005620: 0000 6700 7c00 5d14 7d01 7c01 6400 1900  ..g.|.].}.|.d...
+00005630: 7c01 6401 1900 6602 9102 7104 5300 2902  |.d...f...q.S.).
+00005640: 7201 0000 0072 0f00 0000 7222 0000 0029  r....r....r"...)
+00005650: 0272 6400 0000 723d 0000 0072 2200 0000  .rd...r=...r"...
+00005660: 7222 0000 0072 2300 0000 7266 0000 00f0  r"...r#...rf....
+00005670: 0300 0073 0400 0000 0600 0200 7a2a 6669  ...s........z*fi
+00005680: 6e64 5f63 616e 6469 6461 7465 5f6d 6174  nd_candidate_mat
+00005690: 6368 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c  ches.<locals>.<l
+000056a0: 6973 7463 6f6d 703e 290f 721b 0000 0072  istcomp>).r....r
+000056b0: 1c00 0000 726d 0000 0072 5500 0000 721d  ....rm...rU...r.
+000056c0: 0000 0072 3700 0000 7238 0000 0072 2d00  ...r7...r8...r-.
+000056d0: 0000 721e 0000 00da 0473 6f72 7472 7200  ..r......sortrr.
+000056e0: 0000 7259 0000 0072 9100 0000 7236 0000  ..rY...r....r6..
+000056f0: 0072 2e00 0000 2919 7262 0000 0072 ac00  .r....).rb...r..
+00005700: 0000 72ad 0000 0072 ae00 0000 7276 0000  ..r....r....rv..
+00005710: 0072 7700 0000 5a0e 6e75 6d5f 7175 6572  .rw...Z.num_quer
+00005720: 795f 646f 6373 7278 0000 005a 1163 616e  y_docsrx...Z.can
+00005730: 6469 6461 7465 5f6d 6174 6368 6573 727a  didate_matchesrz
+00005740: 0000 005a 116d 6174 6368 6573 5f73 7461  ...Z.matches_sta
+00005750: 7274 5f70 6f73 5a0f 6d61 7463 6865 735f  rt_posZ.matches_
+00005760: 656e 645f 706f 735a 1163 7572 7265 6e74  end_posZ.current
+00005770: 5f71 7565 7279 5f6c 656e 5a16 7265 6665  _query_lenZ.refe
+00005780: 7265 6e63 655f 6368 756e 6b5f 6c65 6e67  rence_chunk_leng
+00005790: 7468 5a15 6375 7272 656e 745f 636c 6f73  thZ.current_clos
+000057a0: 655f 6d61 7463 6865 735a 1263 7572 7265  e_matchesZ.curre
+000057b0: 6e74 5f63 616e 6469 6461 7465 7372 9400  nt_candidatesr..
+000057c0: 0000 7234 0000 005a 0664 6f63 5f69 645a  ..r4...Z.doc_idZ
+000057d0: 0670 6f73 5f69 64da 0963 616e 6469 6461  .pos_id..candida
+000057e0: 7465 5a09 6d69 6e5f 7363 6f72 655a 096d  teZ.min_scoreZ.m
+000057f0: 696e 5f69 6e64 6578 da07 6f76 6572 6c61  in_index..overla
+00005800: 7072 3d00 0000 7222 0000 0072 2200 0000  pr=...r"...r"...
+00005810: 7223 0000 00da 1666 696e 645f 6361 6e64  r#.....find_cand
+00005820: 6964 6174 655f 6d61 7463 6865 739c 0300  idate_matches...
+00005830: 0073 6a00 0000 0018 1401 0a01 0e01 0601  .sj.............
+00005840: 02fe 0605 0a02 0602 0402 0e01 0801 0c01  ................
+00005850: 1401 0802 0401 16ff 0405 0a01 0401 1001  ................
+00005860: 0e01 0e02 08ff 0402 10fe 0403 0c01 06ff  ................
+00005870: 02fd 0406 0a03 0601 0e01 06fd 0406 0801  ................
+00005880: 0401 0401 1001 0e01 0801 0401 2401 0801  ............$...
+00005890: 0401 0a01 0401 0e01 0c02 0801 0a01 1601  ................
+000058a0: 72b2 0000 0029 0272 2400 0000 7225 0000  r....).r$...r%..
+000058b0: 0029 0372 2400 0000 7225 0000 004e 2902  .).r$...r%...N).
+000058c0: 72ab 0000 0072 0f00 0000 292c 7250 0000  r....r....),rP..
+000058d0: 0072 a500 0000 da06 6269 7365 6374 7202  .r......bisectr.
+000058e0: 0000 00da 0b64 6174 6163 6c61 7373 6573  .....dataclasses
+000058f0: 7203 0000 00da 0568 6561 7071 7204 0000  r......heapqr...
+00005900: 0072 0500 0000 da14 6d75 6c74 6970 726f  .r......multipro
+00005910: 6365 7373 696e 672e 706f 6f6c 7206 0000  cessing.poolr...
+00005920: 00da 0674 7970 696e 6772 0700 0000 7208  ...typingr....r.
+00005930: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
+00005940: 0000 720c 0000 00da 056e 756d 7079 721e  ..r......numpyr.
+00005950: 0000 00da 0f5f 6661 7374 7465 7874 7365  ....._fasttextse
+00005960: 6172 6368 720d 0000 0072 2100 0000 720e  archr....r!...r.
+00005970: 0000 00da 0c73 7566 6669 785f 6172 7261  .....suffix_arra
+00005980: 7972 1000 0000 da09 6461 7461 7479 7065  yr......datatype
+00005990: 7372 1100 0000 7212 0000 0072 1300 0000  sr....r....r....
+000059a0: da05 7574 696c 7372 1400 0000 7215 0000  ..utilsr....r...
+000059b0: 0072 1600 0000 da07 6e64 6172 7261 7972  .r......ndarrayr
+000059c0: 5800 0000 7257 0000 0072 4100 0000 da03  X...rW...rA.....
+000059d0: 7374 7272 6100 0000 7280 0000 0072 9c00  strra...r....r..
+000059e0: 0000 72aa 0000 0072 b200 0000 7222 0000  ..r....r....r"..
+000059f0: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
+00005a00: da08 3c6d 6f64 756c 653e 1100 0000 737a  ..<module>....sz
+00005a10: 0000 0008 0108 010c 010c 0110 010c 0120  ............... 
+00005a20: 0208 0210 040c 0114 0114 0404 0004 010e  ................
+00005a30: fe0c 2600 0100 fc02 0102 010e 0102 0102  ..&.............
+00005a40: 0112 fb0c 7f00 2602 000e 0002 0122 fe0c  ......&......"..
+00005a50: 7f00 0900 0100 0100 fb02 0102 0104 0102  ................
+00005a60: 0102 0106 0122 fa0c 7f00 0b02 0110 fe0c  ....."..........
+00005a70: 7f00 7f00 3a0a 0002 0118 fe0c 6f00 0100  ....:.......o...
+00005a80: fc02 0104 0102 0102 0102 0112 fb         .............
```

### Comparing `fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/suffix_array.cpython-38.pyc` & `fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/suffix_array.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue May 16 07:26:33 2023 UTC, .py size: 6695 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2930 6364 271a 0000  U.......)0cd'...
+00000000: 550d 0d0a 0000 0000 78e1 6564 331a 0000  U.......x.ed3...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6502  d.l.Z.d.d.l.Z.e.
 00000040: 6a03 6502 6a03 6402 9c02 6403 6404 8404  j.e.j.d...d.d...
 00000050: 5a04 6502 6a03 6502 6a03 6402 9c02 6405  Z.e.j.e.j.d...d.
 00000060: 6406 8404 5a05 640b 6502 6a03 6506 6506  d...Z.d.e.j.e.e.
 00000070: 6502 6a03 6408 9c04 6409 640a 8405 5a07  e.j.d...d.d...Z.
@@ -44,278 +44,279 @@
 000002b0: 6564 2031 2d44 2061 7272 6179 2e0a 2020  ed 1-D array..  
 000002c0: 2020 5429 01da 0e72 6574 7572 6e5f 696e    T)...return_in
 000002d0: 7665 7273 65a9 01da 0564 7479 7065 2907  verse....dtype).
 000002e0: da02 6e70 da06 756e 6971 7565 da07 6172  ..np..unique..ar
 000002f0: 6773 6f72 74da 0565 6d70 7479 da04 7369  gsort..empty..si
 00000300: 7a65 da05 696e 7433 32da 0661 7261 6e67  ze..int32..arang
 00000310: 6529 0572 0200 0000 5a07 756e 6971 7565  e).r....Z.unique
-00000320: 645a 0769 6e76 6572 7365 5a17 696e 6465  dZ.inverseZ.inde
+00000320: 64da 0769 6e76 6572 7365 5a17 696e 6465  d..inverseZ.inde
 00000330: 7865 735f 736f 7274 6564 3275 6e73 6f72  xes_sorted2unsor
 00000340: 7465 645a 1769 6e64 6578 6573 5f75 6e73  tedZ.indexes_uns
-00000350: 6f72 7465 6432 736f 7274 6564 a900 720e  orted2sorted..r.
-00000360: 0000 00fa 4f2f 6365 7068 2d68 772f 6b61  ....O/ceph-hw/ka
-00000370: 6e67 7765 692f 636f 6465 322f 7465 7874  ngwei/code2/text
-00000380: 5f73 6561 7263 682f 7465 7874 7365 6172  _search/textsear
-00000390: 6368 2f70 7974 686f 6e2f 7465 7874 7365  ch/python/textse
-000003a0: 6172 6368 2f73 7566 6669 785f 6172 7261  arch/suffix_arra
-000003b0: 792e 7079 da0c 5f72 656e 756d 6265 7269  y.py.._renumberi
-000003c0: 6e67 1500 0000 730a 0000 0000 0f12 030a  ng....s.........
-000003d0: 0112 0110 0272 1000 0000 6301 0000 0000  .....r....c.....
-000003e0: 0000 0000 0000 0006 0000 0005 0000 0043  ...............C
-000003f0: 0000 0073 8a00 0000 7c00 6a00 6401 6b02  ...s....|.j.d.k.
-00000400: 7314 7401 7c00 6a00 8301 8201 7402 7c00  s.t.|.j.....t.|.
-00000410: 8301 7d00 7c00 a003 a100 7d01 7c01 7404  ..}.|.....}.|.t.
-00000420: a005 7c00 6a06 a101 6a03 6401 1800 6b00  ..|.j...j.d...k.
-00000430: 7342 7401 7c01 8301 8201 7c01 6401 1700  sBt.|.....|.d...
-00000440: 7d02 7404 6a07 7c02 6402 6402 6402 6704  }.t.j.|.d.d.d.g.
-00000450: 7c00 6a06 6403 8d02 7d03 7404 a008 7c00  |.j.d...}.t...|.
-00000460: 7c03 6702 a101 7d04 7404 6a09 7c04 7404  |.g...}.t.j.|.t.
-00000470: 6a0a 6403 8d02 7d05 740b a00c 7c05 a101  j.d...}.t...|...
-00000480: 5300 2904 612d 0300 0043 7265 6174 6520  S.).a-...Create 
-00000490: 6120 7375 6666 6978 2061 7272 6179 2066  a suffix array f
-000004a0: 726f 6d20 6120 312d 4420 696e 7075 7420  rom a 1-D input 
-000004b0: 6172 7261 792e 0a0a 2020 2020 6869 6e74  array...    hint
-000004c0: 3a0a 2020 2020 2020 506c 6561 7365 2072  :.      Please r
-000004d0: 6566 6572 2074 6f20 6874 7470 733a 2f2f  efer to https://
-000004e0: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
-000004f0: 2f77 696b 692f 5375 6666 6978 5f61 7272  /wiki/Suffix_arr
-00000500: 6179 0a20 2020 2020 2066 6f72 2077 6861  ay.      for wha
-00000510: 7420 7375 6666 6978 2061 7272 6179 2069  t suffix array i
-00000520: 732e 2044 6966 6665 7265 6e74 2066 726f  s. Different fro
-00000530: 6d20 7468 6520 6162 6f76 6520 5769 6b69  m the above Wiki
-00000540: 7065 6469 610a 2020 2020 2020 6172 7469  pedia.      arti
-00000550: 636c 6520 7468 6520 7370 6563 6961 6c20  cle the special 
-00000560: 7365 6e74 696e 656c 206c 6574 7465 7220  sentinel letter 
-00000570: 6060 2460 6020 696e 2060 7465 7874 7365  ``$`` in `textse
-00000580: 6172 6368 605f 0a20 2020 2020 2069 7320  arch`_.      is 
-00000590: 6b6e 6f77 6e20 6173 2045 4f53 2061 6e64  known as EOS and
-000005a0: 2069 7420 6973 206c 6172 6765 7220 7468   it is larger th
-000005b0: 616e 2061 6e79 206f 7468 6572 2063 6861  an any other cha
-000005c0: 7261 6374 6572 732e 0a0a 2020 2020 4172  racters...    Ar
-000005d0: 6773 3a0a 2020 2020 2020 6172 7261 793a  gs:.      array:
-000005e0: 0a20 2020 2020 2020 2041 2031 2d44 2069  .        A 1-D i
-000005f0: 6e74 6567 6572 2028 6f72 2075 6e73 6967  nteger (or unsig
-00000600: 6e65 6420 696e 7465 6765 7229 2061 7272  ned integer) arr
-00000610: 6179 206f 6620 7368 6170 6520 6060 2873  ay of shape ``(s
-00000620: 6571 5f6c 656e 202d 2031 2c29 6060 2e0a  eq_len - 1,)``..
-00000630: 0a20 2020 2020 2020 204e 6f74 653a 0a20  .        Note:. 
-00000640: 2020 2020 2020 2020 2049 6e73 6964 6520           Inside 
-00000650: 7468 6973 2066 756e 6374 696f 6e2c 2077  this function, w
-00000660: 6520 7769 6c6c 2061 7070 656e 6420 6578  e will append ex
-00000670: 706c 6963 6974 6c79 2061 6e20 454f 530a  plicitly an EOS.
-00000680: 2020 2020 2020 2020 2020 7379 6d62 6f6c            symbol
-00000690: 2074 6861 7420 6973 206c 6172 6765 7220   that is larger 
-000006a0: 7468 616e 2060 6061 7272 6179 2e6d 6178  than ``array.max
-000006b0: 2829 6060 2e0a 2020 2020 5265 7475 726e  ()``..    Return
-000006c0: 733a 0a20 2020 2020 2052 6574 7572 6e73  s:.      Returns
-000006d0: 2061 2073 7566 6669 7820 6172 7261 7920   a suffix array 
-000006e0: 6f66 2074 7970 6520 6060 6e70 2e69 6e74  of type ``np.int
-000006f0: 3332 6060 2c20 6f66 2073 6861 7065 2060  32``, of shape `
-00000700: 6028 7365 715f 6c65 6e2c 2960 602e 0a20  `(seq_len,)``.. 
-00000710: 2020 2020 2054 6869 7320 7769 6c6c 2063       This will c
-00000720: 6f6e 7369 7374 206f 6620 736f 6d65 2070  onsist of some p
-00000730: 6572 6d75 7461 7469 6f6e 206f 6620 7468  ermutation of th
-00000740: 6520 656c 656d 656e 7473 0a20 2020 2020  e elements.     
-00000750: 2060 6030 202e 2e20 7365 715f 6c65 6e20   ``0 .. seq_len 
-00000760: 2d20 3160 602e 0a0a 2020 2020 2a2a 5573  - 1``...    **Us
-00000770: 6167 6520 6578 616d 706c 6573 2a2a 3a0a  age examples**:.
-00000780: 0a20 2020 2020 2020 202e 2e20 6c69 7465  .        .. lite
-00000790: 7261 6c69 6e63 6c75 6465 3a3a 2063 6f64  ralinclude:: cod
-000007a0: 652f 7375 6666 6978 2d61 7272 6179 2e70  e/suffix-array.p
-000007b0: 790a 2020 2020 e901 0000 0072 0100 0000  y.    .....r....
-000007c0: 7205 0000 0029 0dda 046e 6469 6dda 0e41  r....)...ndim..A
-000007d0: 7373 6572 7469 6f6e 4572 726f 7272 1000  ssertionErrorr..
-000007e0: 0000 da03 6d61 7872 0700 0000 da05 6969  ....maxr......ii
-000007f0: 6e66 6f72 0600 0000 7202 0000 00da 0b63  nfor....r......c
-00000800: 6f6e 6361 7465 6e61 7465 da11 6173 636f  oncatenate..asco
-00000810: 6e74 6967 756f 7573 6172 7261 7972 0c00  ntiguousarrayr..
-00000820: 0000 da0b 5f74 6578 7473 6561 7263 68da  ...._textsearch.
-00000830: 1363 7265 6174 655f 7375 6666 6978 5f61  .create_suffix_a
-00000840: 7272 6179 2906 7202 0000 005a 0a6d 6178  rray).r....Z.max
-00000850: 5f73 796d 626f 6c5a 0365 6f73 da07 7061  _symbolZ.eos..pa
-00000860: 6464 696e 675a 0c70 6164 6465 645f 6172  ddingZ.padded_ar
-00000870: 7261 795a 0b61 7272 6179 5f69 6e74 3332  rayZ.array_int32
-00000880: 720e 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
-00000890: 1900 0000 2e00 0000 7312 0000 0000 1914  ........s.......
-000008a0: 0708 0208 011e 0108 0118 020e 0310 0172  ...............r
-000008b0: 1900 0000 7211 0000 0029 04da 0c73 7566  ....r....)...suf
-000008c0: 6669 785f 6172 7261 79da 0971 7565 7279  fix_array..query
-000008d0: 5f6c 656e da11 6e75 6d5f 636c 6f73 655f  _len..num_close_
-000008e0: 6d61 7463 6865 7372 0300 0000 6303 0000  matchesr....c...
-000008f0: 0000 0000 0000 0000 000b 0000 0007 0000  ................
-00000900: 0043 0000 0073 4a01 0000 7c01 6401 6b05  .C...sJ...|.d.k.
-00000910: 7310 7400 7c01 8301 8201 7c00 6a01 6402  s.t.|.....|.j.d.
-00000920: 6b02 7324 7400 7c00 6a01 8301 8201 7c00  k.s$t.|.j.....|.
-00000930: 6a02 7403 6a04 6b02 733a 7400 7c00 6a02  j.t.j.k.s:t.|.j.
-00000940: 8301 8201 7c00 6a05 7d03 7c01 7c03 6b00  ....|.j.}.|.|.k.
-00000950: 7354 7400 7c01 7c03 6602 8301 8201 7c02  sTt.|.|.f.....|.
-00000960: 6402 6b05 7364 7400 7c02 8301 8201 7403  d.k.sdt.|.....t.
-00000970: 6a06 7c01 7c02 6403 1400 6602 7c03 6403  j.|.|.d...f.|.d.
-00000980: 1800 7c00 6a02 6404 8d03 7d04 7c03 6403  ..|.j.d...}.|.d.
-00000990: 1800 6701 7c02 1400 7d05 6900 7d06 6401  ..g.|...}.i.}.d.
-000009a0: 7d07 7407 7c03 6402 1800 8301 4400 5da0  }.t.|.d.....D.].
-000009b0: 7d08 7c00 7c08 1900 7d09 7c09 7c01 6b05  }.|.|...}.|.|.k.
-000009c0: 9001 721c 7c09 7c05 7c07 7c02 1600 3c00  ..r.|.|.|.|...<.
-000009d0: 7c07 6402 3700 7d07 7408 7c06 8301 4400  |.d.7.}.t.|...D.
-000009e0: 5d42 7d0a 7c09 7c04 7c0a 7c06 7c0a 1900  ]B}.|.|.|.|.|...
-000009f0: 6602 3c00 7c06 7c0a 1900 7c02 6403 1400  f.<.|.|...|.d...
-00000a00: 6402 1800 6b02 9001 7208 7c06 7c0a 3d00  d...k...r.|.|.=.
-00000a10: 71d6 7c06 7c0a 0500 1900 6402 3700 0300  q.|.|.....d.7...
-00000a20: 3c00 71d6 71a4 7407 7c02 8301 4400 5d16  <.q.q.t.|...D.].
-00000a30: 7d08 7c05 7c08 1900 7c04 7c09 7c08 6602  }.|.|...|.|.|.f.
-00000a40: 3c00 9001 7124 7c02 7c06 7c09 3c00 71a4  <...q$|.|.|.<.q.
-00000a50: 7c04 5300 2905 612a 0800 0041 7373 756d  |.S.).a*...Assum
-00000a60: 696e 6720 7468 6520 7375 6666 6978 2061  ing the suffix a
-00000a70: 7272 6179 2077 6173 2063 7265 6174 6564  rray was created
-00000a80: 2066 726f 6d20 6120 7465 7874 2077 6865   from a text whe
-00000a90: 7265 2074 6865 2066 6972 7374 0a20 2020  re the first.   
-00000aa0: 2060 6071 7565 7279 5f6c 656e 6060 2070   ``query_len`` p
-00000ab0: 6f73 6974 696f 6e73 2072 6570 7265 7365  ositions represe
-00000ac0: 6e74 2074 6865 2071 7565 7279 2074 6578  nt the query tex
-00000ad0: 7420 616e 6420 7468 6520 7265 6d61 696e  t and the remain
-00000ae0: 696e 6720 706f 7369 7469 6f6e 730a 2020  ing positions.  
-00000af0: 2020 7265 7072 6573 656e 7420 7468 6520    represent the 
-00000b00: 7265 6665 7265 6e63 6520 7465 7874 2c20  reference text, 
-00000b10: 7265 7475 726e 2061 206c 6973 7420 696e  return a list in
-00000b20: 6469 6361 7469 6e67 2c20 666f 7220 6561  dicating, for ea
-00000b30: 6368 2073 7566 6669 780a 2020 2020 706f  ch suffix.    po
-00000b40: 7369 7469 6f6e 2069 6e20 7468 6520 7175  sition in the qu
-00000b50: 6572 7920 7465 7874 2c20 7468 6520 7477  ery text, the tw
-00000b60: 6f20 7375 6666 6978 2070 6f73 6974 696f  o suffix positio
-00000b70: 6e73 2069 6e20 7468 6520 7265 6665 7265  ns in the refere
-00000b80: 6e63 6520 7465 7874 0a20 2020 2074 6861  nce text.    tha
-00000b90: 7420 696d 6d65 6469 6174 656c 7920 7072  t immediately pr
-00000ba0: 6563 6564 6520 616e 6420 666f 6c6c 6f77  ecede and follow
-00000bb0: 2069 7420 6c65 7869 636f 6772 6170 6869   it lexicographi
-00000bc0: 6361 6c6c 792e 2020 2849 2074 6869 6e6b  cally.  (I think
-00000bd0: 2073 7566 6669 780a 2020 2020 706f 7369   suffix.    posi
-00000be0: 7469 6f6e 2072 6566 6572 7320 746f 2074  tion refers to t
-00000bf0: 6865 206c 6173 7420 6368 6172 6163 7465  he last characte
-00000c00: 7220 6f66 2061 2073 7566 6669 7829 2e0a  r of a suffix)..
-00000c10: 0a20 2020 2054 6869 7320 6973 2065 6173  .    This is eas
-00000c20: 7920 746f 2064 6f20 6672 6f6d 2074 6865  y to do from the
-00000c30: 2073 7566 6669 7820 6172 7261 7920 7769   suffix array wi
-00000c40: 7468 6f75 7420 636f 6d70 7574 696e 672c  thout computing,
-00000c50: 2066 6f72 2065 7861 6d70 6c65 2c0a 2020   for example,.  
-00000c60: 2020 7468 6520 4c43 5020 6172 7261 793b    the LCP array;
-00000c70: 2061 6e64 2069 7420 7072 6f64 7563 6573   and it produces
-00000c80: 2065 7861 6374 6c79 2032 206d 6174 6368   exactly 2 match
-00000c90: 6573 2070 6572 2070 6f73 6974 696f 6e20  es per position 
-00000ca0: 696e 2074 6865 2071 7565 7279 0a20 2020  in the query.   
-00000cb0: 2074 6578 742c 2077 6869 6368 2069 7320   text, which is 
-00000cc0: 616c 736f 2063 6f6e 7665 6e69 656e 742e  also convenient.
-00000cd0: 0a0a 2020 2020 284e 6f74 653a 2074 6865  ..    (Note: the
-00000ce0: 2071 7565 7279 2061 6e64 2072 6566 6572   query and refer
-00000cf0: 656e 6365 2074 6578 7473 2063 6f75 6c64  ence texts could
-00000d00: 2065 6163 6820 7265 7072 6573 656e 7420   each represent 
-00000d10: 6d75 6c74 6970 6c65 2073 6570 6172 6174  multiple separat
-00000d20: 650a 2020 2020 7365 7175 656e 6365 732c  e.    sequences,
-00000d30: 2062 7574 2074 6861 7420 6973 2068 616e   but that is han
-00000d40: 646c 6564 2062 7920 6f74 6865 7220 636f  dled by other co
-00000d50: 6465 3b20 636c 6173 7320 536f 7572 6365  de; class Source
-00000d60: 6454 6578 7420 6b65 6570 7320 7472 6163  dText keeps trac
-00000d70: 6b0a 2020 2020 6f66 2074 6861 7420 696e  k.    of that in
-00000d80: 666f 726d 6174 696f 6e2e 290a 0a20 2020  formation.)..   
-00000d90: 2041 7267 733a 0a20 2020 2020 7375 6666   Args:.     suff
-00000da0: 6978 5f61 7272 6179 3a0a 2020 2020 2020  ix_array:.      
-00000db0: 2041 2073 7566 6669 7820 6172 7261 7920   A suffix array 
-00000dc0: 6173 2063 7265 6174 6564 2062 7920 3a66  as created by :f
-00000dd0: 756e 633a 6063 7265 6174 655f 7375 6666  unc:`create_suff
-00000de0: 6978 5f61 7272 6179 602c 206f 6620 6474  ix_array`, of dt
-00000df0: 7970 650a 2020 2020 2020 2060 606e 702e  ype.       ``np.
-00000e00: 696e 7433 3260 6020 616e 6420 7368 6170  int32`` and shap
-00000e10: 6520 6060 2873 6571 5f6c 656e 2c29 6060  e ``(seq_len,)``
-00000e20: 2e0a 0a20 2020 2020 7175 6572 795f 6c65  ...     query_le
-00000e30: 6e3a 0a20 2020 2020 2020 4120 6e75 6d62  n:.       A numb
-00000e40: 6572 2060 6030 203c 3d20 7175 6572 795f  er ``0 <= query_
-00000e50: 6c65 6e20 3c20 7365 715f 6c65 6e60 602c  len < seq_len``,
-00000e60: 2069 6e64 6963 6174 696e 6720 7468 6520   indicating the 
-00000e70: 6c65 6e67 7468 2069 6e20 7379 6d62 6f6c  length in symbol
-00000e80: 730a 2020 2020 2020 2028 6c69 6b65 6c79  s.       (likely
-00000e90: 2062 7974 6573 2920 6f66 2074 6865 2071   bytes) of the q
-00000ea0: 7565 7279 2070 6172 7420 6f66 2074 6865  uery part of the
-00000eb0: 2074 6578 7420 7468 6174 2077 6173 2075   text that was u
-00000ec0: 7365 6420 746f 2063 7265 6174 650a 2020  sed to create.  
-00000ed0: 2020 2020 2060 6073 7566 6669 785f 6172       ``suffix_ar
-00000ee0: 7261 7960 602e 0a0a 2020 2020 5265 7475  ray``...    Retu
-00000ef0: 726e 733a 0a20 2020 2020 2052 6574 7572  rns:.      Retur
-00000f00: 6e20 616e 206e 702e 6e64 6172 7261 7920  n an np.ndarray 
-00000f10: 6f66 2073 6861 7065 2060 6028 7175 6572  of shape ``(quer
-00000f20: 795f 6c65 6e20 2a20 322c 2960 602c 206f  y_len * 2,)``, o
-00000f30: 6620 7468 6520 7361 6d65 2064 7479 7065  f the same dtype
-00000f40: 2061 730a 2020 2020 2020 6060 7375 6666   as.      ``suff
-00000f50: 6978 5f61 7272 6179 6060 2c20 696e 2077  ix_array``, in w
-00000f60: 6869 6368 2070 6f73 6974 696f 6e73 2060  hich positions `
-00000f70: 6032 2a69 6060 2061 6e64 2060 6032 2a69  `2*i`` and ``2*i
-00000f80: 202b 2031 6060 2072 6570 7265 7365 6e74   + 1`` represent
-00000f90: 0a20 2020 2020 2074 6865 2074 776f 2070  .      the two p
-00000fa0: 6f73 6974 696f 6e73 2069 6e20 7468 6520  ositions in the 
-00000fb0: 6f72 6967 696e 616c 2074 6578 7420 7468  original text th
-00000fc0: 6174 2061 7265 2077 6974 6869 6e20 7468  at are within th
-00000fd0: 6520 7265 6665 7265 6e63 650a 2020 2020  e reference.    
-00000fe0: 2020 706f 7274 696f 6e2c 2061 6e64 2077    portion, and w
-00000ff0: 6869 6368 2069 6d6d 6564 6961 7465 6c79  hich immediately
-00001000: 2070 7265 6365 6465 2061 6e64 2066 6f6c   precede and fol
-00001010: 6c6f 772c 2069 6e20 7468 6520 7375 6666  low, in the suff
-00001020: 6978 2061 7272 6179 2c0a 2020 2020 2020  ix array,.      
-00001030: 7175 6572 7920 706f 7369 7469 6f6e 2060  query position `
-00001040: 6069 6060 2e20 2054 6869 7320 6d65 616e  `i``.  This mean
-00001050: 7320 7468 6174 2074 6865 2073 7566 6669  s that the suffi
-00001060: 7865 7320 656e 6469 6e67 2061 7420 7468  xes ending at th
-00001070: 6f73 650a 2020 2020 2020 706f 7369 7469  ose.      positi
-00001080: 6f6e 7320 6172 6520 7265 7665 7273 652d  ons are reverse-
-00001090: 6c65 7869 636f 6772 6170 6869 6361 6c6c  lexicographicall
-000010a0: 7920 636c 6f73 6520 746f 2074 6865 2073  y close to the s
-000010b0: 7566 6669 7820 656e 6469 6e67 2061 740a  uffix ending at.
-000010c0: 2020 2020 2020 706f 7369 7469 6f6e 2060        position `
-000010d0: 6069 6060 2e20 2041 7320 6120 7370 6563  `i``.  As a spec
-000010e0: 6961 6c20 6361 7365 2c20 6966 206f 6e65  ial case, if one
-000010f0: 206f 6620 7468 6573 6520 7265 7475 726e   of these return
-00001100: 6564 206e 756d 6265 7273 2077 6f75 6c64  ed numbers would
-00001110: 0a20 2020 2020 2065 7175 616c 2074 6865  .      equal the
-00001120: 2045 4f53 2070 6f73 6974 696f 6e20 2870   EOS position (p
-00001130: 6f73 6974 696f 6e20 7365 715f 6c65 6e20  osition seq_len 
-00001140: 2d20 3129 2c20 6f72 2069 6620 6120 7175  - 1), or if a qu
-00001150: 6572 7920 706f 7369 7469 6f6e 2069 730a  ery position is.
-00001160: 2020 2020 2020 6265 666f 7265 2061 6e79        before any
-00001170: 2072 6566 6572 656e 6365 2070 6f73 6974   reference posit
-00001180: 696f 6e20 696e 2074 6865 2073 7566 6669  ion in the suffi
-00001190: 7820 6172 6179 2c20 7765 206f 7574 7075  x aray, we outpu
-000011a0: 740a 2020 2020 2020 6060 7365 715f 6c65  t.      ``seq_le
-000011b0: 6e20 2d20 3260 6020 696e 7374 6561 6420  n - 2`` instead 
-000011c0: 746f 2061 766f 6964 2068 6176 696e 6720  to avoid having 
-000011d0: 746f 2068 616e 646c 6520 7370 6563 6961  to handle specia
-000011e0: 6c20 6361 7365 7320 6c61 7465 7220 6f6e  l cases later on
-000011f0: 0a20 2020 2020 2028 616e 7977 6179 2c20  .      (anyway, 
-00001200: 7468 6573 6520 776f 756c 6420 6e6f 7420  these would not 
-00001210: 7265 7072 6573 656e 7420 6120 636c 6f73  represent a clos
-00001220: 6520 6d61 7463 6829 2e0a 0a20 2020 202e  e match)...    .
-00001230: 2e20 6869 6e74 3a3a 0a0a 2020 2020 2020  . hint::..      
-00001240: 2020 506c 6561 7365 2072 6566 6572 2074    Please refer t
-00001250: 6f20 3a72 6566 3a60 6669 6e64 5f63 6c6f  o :ref:`find_clo
-00001260: 7365 5f6d 6174 6368 6573 5f74 7574 6f72  se_matches_tutor
-00001270: 6961 6c60 2066 6f72 2075 7361 6765 732e  ial` for usages.
-00001280: 0a20 2020 2072 0100 0000 7211 0000 00e9  .    r....r.....
-00001290: 0200 0000 2902 da0a 6669 6c6c 5f76 616c  ....)...fill_val
-000012a0: 7565 7206 0000 0029 0972 1300 0000 7212  uer....).r....r.
-000012b0: 0000 0072 0600 0000 7207 0000 0072 0c00  ...r....r....r..
-000012c0: 0000 720b 0000 00da 0466 756c 6cda 0572  ..r......full..r
-000012d0: 616e 6765 da04 6c69 7374 290b 721b 0000  ange..list).r...
-000012e0: 0072 1c00 0000 721d 0000 005a 0773 6571  .r....r....Z.seq
-000012f0: 5f6c 656e da06 6f75 7470 7574 5a09 7072  _len..outputZ.pr
-00001300: 6576 5f72 6566 735a 0c75 6e66 696e 6973  ev_refsZ.unfinis
-00001310: 6865 645f 715a 0a72 6566 735f 696e 6465  hed_qZ.refs_inde
-00001320: 78da 0169 5a08 7465 7874 5f70 6f73 da01  x..iZ.text_pos..
-00001330: 6b72 0e00 0000 720e 0000 0072 0f00 0000  kr....r....r....
-00001340: da12 6669 6e64 5f63 6c6f 7365 5f6d 6174  ..find_close_mat
-00001350: 6368 6573 5c00 0000 7338 0000 0000 2d10  ches\...s8....-.
-00001360: 0114 0116 0106 0114 0210 0204 010a 0106  ................
-00001370: 0104 fd06 060e 0404 0204 0110 0108 010a  ................
-00001380: 010c 0108 010c 0110 0116 0108 0214 020c  ................
-00001390: 0114 020a 0272 2600 0000 2901 7211 0000  .....r&...).r...
-000013a0: 0029 0872 1800 0000 da05 6e75 6d70 7972  .).r......numpyr
-000013b0: 0700 0000 da07 6e64 6172 7261 7972 1000  ......ndarrayr..
-000013c0: 0000 7219 0000 00da 0369 6e74 7226 0000  ..r......intr&..
-000013d0: 0072 0e00 0000 720e 0000 0072 0e00 0000  .r....r....r....
-000013e0: 720f 0000 00da 083c 6d6f 6475 6c65 3e11  r......<module>.
-000013f0: 0000 0073 1400 0000 0801 0803 1419 142f  ...s.........../
-00001400: 00ff 0201 0400 0200 0201 04fe            ............
+00000350: 6f72 7465 6432 736f 7274 6564 a900 720f  orted2sorted..r.
+00000360: 0000 00fa 4e2f 6365 7068 2d6b 772f 6b61  ....N/ceph-kw/ka
+00000370: 6e67 7765 692f 636f 6465 2f74 6578 745f  ngwei/code/text_
+00000380: 7365 6172 6368 2f74 6578 7473 6561 7263  search/textsearc
+00000390: 682f 7079 7468 6f6e 2f74 6578 7473 6561  h/python/textsea
+000003a0: 7263 682f 7375 6666 6978 5f61 7272 6179  rch/suffix_array
+000003b0: 2e70 79da 0c5f 7265 6e75 6d62 6572 696e  .py.._renumberin
+000003c0: 6715 0000 0073 0a00 0000 000f 1203 0a01  g....s..........
+000003d0: 1201 1002 7211 0000 0063 0100 0000 0000  ....r....c......
+000003e0: 0000 0000 0000 0600 0000 0500 0000 4300  ..............C.
+000003f0: 0000 738a 0000 007c 006a 0064 016b 0273  ..s....|.j.d.k.s
+00000400: 1474 017c 006a 0083 0182 0174 027c 0083  .t.|.j.....t.|..
+00000410: 017d 007c 00a0 03a1 007d 017c 0174 04a0  .}.|.....}.|.t..
+00000420: 057c 006a 06a1 016a 0364 0118 006b 0073  .|.j...j.d...k.s
+00000430: 4274 017c 0183 0182 017c 0164 0117 007d  Bt.|.....|.d...}
+00000440: 0274 046a 077c 0264 0264 0264 0267 047c  .t.j.|.d.d.d.g.|
+00000450: 006a 0664 038d 027d 0374 04a0 087c 007c  .j.d...}.t...|.|
+00000460: 0367 02a1 017d 0474 046a 097c 0474 046a  .g...}.t.j.|.t.j
+00000470: 0a64 038d 027d 0574 0ba0 0c7c 05a1 0153  .d...}.t...|...S
+00000480: 0029 0461 3103 0000 4372 6561 7465 2061  .).a1...Create a
+00000490: 2073 7566 6669 7820 6172 7261 7920 6672   suffix array fr
+000004a0: 6f6d 2061 2031 2d44 2069 6e70 7574 2061  om a 1-D input a
+000004b0: 7272 6179 2e0a 0a20 2020 2068 696e 743a  rray...    hint:
+000004c0: 0a20 2020 2020 2050 6c65 6173 6520 7265  .      Please re
+000004d0: 6665 7220 746f 2068 7474 7073 3a2f 2f65  fer to https://e
+000004e0: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+000004f0: 7769 6b69 2f53 7566 6669 785f 6172 7261  wiki/Suffix_arra
+00000500: 790a 2020 2020 2020 666f 7220 7768 6174  y.      for what
+00000510: 2073 7566 6669 7820 6172 7261 7920 6973   suffix array is
+00000520: 2e20 4469 6666 6572 656e 7420 6672 6f6d  . Different from
+00000530: 2074 6865 2061 626f 7665 2057 696b 6970   the above Wikip
+00000540: 6564 6961 0a20 2020 2020 2061 7274 6963  edia.      artic
+00000550: 6c65 2074 6865 2073 7065 6369 616c 2073  le the special s
+00000560: 656e 7469 6e65 6c20 6c65 7474 6572 2060  entinel letter `
+00000570: 6024 6060 2069 6e20 6066 6173 7474 6578  `$`` in `fasttex
+00000580: 7473 6561 7263 6860 5f0a 2020 2020 2020  tsearch`_.      
+00000590: 6973 206b 6e6f 776e 2061 7320 454f 5320  is known as EOS 
+000005a0: 616e 6420 6974 2069 7320 6c61 7267 6572  and it is larger
+000005b0: 2074 6861 6e20 616e 7920 6f74 6865 7220   than any other 
+000005c0: 6368 6172 6163 7465 7273 2e0a 0a20 2020  characters...   
+000005d0: 2041 7267 733a 0a20 2020 2020 2061 7272   Args:.      arr
+000005e0: 6179 3a0a 2020 2020 2020 2020 4120 312d  ay:.        A 1-
+000005f0: 4420 696e 7465 6765 7220 286f 7220 756e  D integer (or un
+00000600: 7369 676e 6564 2069 6e74 6567 6572 2920  signed integer) 
+00000610: 6172 7261 7920 6f66 2073 6861 7065 2060  array of shape `
+00000620: 6028 7365 715f 6c65 6e20 2d20 312c 2960  `(seq_len - 1,)`
+00000630: 602e 0a0a 2020 2020 2020 2020 4e6f 7465  `...        Note
+00000640: 3a0a 2020 2020 2020 2020 2020 496e 7369  :.          Insi
+00000650: 6465 2074 6869 7320 6675 6e63 7469 6f6e  de this function
+00000660: 2c20 7765 2077 696c 6c20 6170 7065 6e64  , we will append
+00000670: 2065 7870 6c69 6369 746c 7920 616e 2045   explicitly an E
+00000680: 4f53 0a20 2020 2020 2020 2020 2073 796d  OS.          sym
+00000690: 626f 6c20 7468 6174 2069 7320 6c61 7267  bol that is larg
+000006a0: 6572 2074 6861 6e20 6060 6172 7261 792e  er than ``array.
+000006b0: 6d61 7828 2960 602e 0a20 2020 2052 6574  max()``..    Ret
+000006c0: 7572 6e73 3a0a 2020 2020 2020 5265 7475  urns:.      Retu
+000006d0: 726e 7320 6120 7375 6666 6978 2061 7272  rns a suffix arr
+000006e0: 6179 206f 6620 7479 7065 2060 606e 702e  ay of type ``np.
+000006f0: 696e 7433 3260 602c 206f 6620 7368 6170  int32``, of shap
+00000700: 6520 6060 2873 6571 5f6c 656e 2c29 6060  e ``(seq_len,)``
+00000710: 2e0a 2020 2020 2020 5468 6973 2077 696c  ..      This wil
+00000720: 6c20 636f 6e73 6973 7420 6f66 2073 6f6d  l consist of som
+00000730: 6520 7065 726d 7574 6174 696f 6e20 6f66  e permutation of
+00000740: 2074 6865 2065 6c65 6d65 6e74 730a 2020   the elements.  
+00000750: 2020 2020 6060 3020 2e2e 2073 6571 5f6c      ``0 .. seq_l
+00000760: 656e 202d 2031 6060 2e0a 0a20 2020 202a  en - 1``...    *
+00000770: 2a55 7361 6765 2065 7861 6d70 6c65 732a  *Usage examples*
+00000780: 2a3a 0a0a 2020 2020 2020 2020 2e2e 206c  *:..        .. l
+00000790: 6974 6572 616c 696e 636c 7564 653a 3a20  iteralinclude:: 
+000007a0: 636f 6465 2f73 7566 6669 782d 6172 7261  code/suffix-arra
+000007b0: 792e 7079 0a20 2020 20e9 0100 0000 7201  y.py.    .....r.
+000007c0: 0000 0072 0500 0000 290d da04 6e64 696d  ...r....)...ndim
+000007d0: da0e 4173 7365 7274 696f 6e45 7272 6f72  ..AssertionError
+000007e0: 7211 0000 00da 036d 6178 7207 0000 00da  r......maxr.....
+000007f0: 0569 696e 666f 7206 0000 0072 0200 0000  .iinfor....r....
+00000800: da0b 636f 6e63 6174 656e 6174 65da 1161  ..concatenate..a
+00000810: 7363 6f6e 7469 6775 6f75 7361 7272 6179  scontiguousarray
+00000820: 720c 0000 00da 0f5f 6661 7374 7465 7874  r......_fasttext
+00000830: 7365 6172 6368 da13 6372 6561 7465 5f73  search..create_s
+00000840: 7566 6669 785f 6172 7261 7929 0672 0200  uffix_array).r..
+00000850: 0000 5a0a 6d61 785f 7379 6d62 6f6c da03  ..Z.max_symbol..
+00000860: 656f 73da 0770 6164 6469 6e67 5a0c 7061  eos..paddingZ.pa
+00000870: 6464 6564 5f61 7272 6179 5a0b 6172 7261  dded_arrayZ.arra
+00000880: 795f 696e 7433 3272 0f00 0000 720f 0000  y_int32r....r...
+00000890: 0072 1000 0000 721a 0000 002e 0000 0073  .r....r........s
+000008a0: 1200 0000 0019 1407 0802 0801 1e01 0801  ................
+000008b0: 1802 0e03 1001 721a 0000 0072 1200 0000  ......r....r....
+000008c0: 2904 da0c 7375 6666 6978 5f61 7272 6179  )...suffix_array
+000008d0: da09 7175 6572 795f 6c65 6eda 116e 756d  ..query_len..num
+000008e0: 5f63 6c6f 7365 5f6d 6174 6368 6573 7203  _close_matchesr.
+000008f0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00000900: 0b00 0000 0700 0000 4300 0000 734a 0100  ........C...sJ..
+00000910: 007c 0164 016b 0573 1074 007c 0183 0182  .|.d.k.s.t.|....
+00000920: 017c 006a 0164 026b 0273 2474 007c 006a  .|.j.d.k.s$t.|.j
+00000930: 0183 0182 017c 006a 0274 036a 046b 0273  .....|.j.t.j.k.s
+00000940: 3a74 007c 006a 0283 0182 017c 006a 057d  :t.|.j.....|.j.}
+00000950: 037c 017c 036b 0073 5474 007c 017c 0366  .|.|.k.sTt.|.|.f
+00000960: 0283 0182 017c 0264 026b 0573 6474 007c  .....|.d.k.sdt.|
+00000970: 0283 0182 0174 036a 067c 017c 0264 0314  .....t.j.|.|.d..
+00000980: 0066 027c 0364 0318 007c 006a 0264 048d  .f.|.d...|.j.d..
+00000990: 037d 047c 0364 0318 0067 017c 0214 007d  .}.|.d...g.|...}
+000009a0: 0569 007d 0664 017d 0774 077c 0364 0218  .i.}.d.}.t.|.d..
+000009b0: 0083 0144 005d a07d 087c 007c 0819 007d  ...D.].}.|.|...}
+000009c0: 097c 097c 016b 0590 0172 1c7c 097c 057c  .|.|.k...r.|.|.|
+000009d0: 077c 0216 003c 007c 0764 0237 007d 0774  .|...<.|.d.7.}.t
+000009e0: 087c 0683 0144 005d 427d 0a7c 097c 047c  .|...D.]B}.|.|.|
+000009f0: 0a7c 067c 0a19 0066 023c 007c 067c 0a19  .|.|...f.<.|.|..
+00000a00: 007c 0264 0314 0064 0218 006b 0290 0172  .|.d...d...k...r
+00000a10: 087c 067c 0a3d 0071 d67c 067c 0a05 0019  .|.|.=.q.|.|....
+00000a20: 0064 0237 0003 003c 0071 d671 a474 077c  .d.7...<.q.q.t.|
+00000a30: 0283 0144 005d 167d 087c 057c 0819 007c  ...D.].}.|.|...|
+00000a40: 047c 097c 0866 023c 0090 0171 247c 027c  .|.|.f.<...q$|.|
+00000a50: 067c 093c 0071 a47c 0453 0029 0561 2a08  .|.<.q.|.S.).a*.
+00000a60: 0000 4173 7375 6d69 6e67 2074 6865 2073  ..Assuming the s
+00000a70: 7566 6669 7820 6172 7261 7920 7761 7320  uffix array was 
+00000a80: 6372 6561 7465 6420 6672 6f6d 2061 2074  created from a t
+00000a90: 6578 7420 7768 6572 6520 7468 6520 6669  ext where the fi
+00000aa0: 7273 740a 2020 2020 6060 7175 6572 795f  rst.    ``query_
+00000ab0: 6c65 6e60 6020 706f 7369 7469 6f6e 7320  len`` positions 
+00000ac0: 7265 7072 6573 656e 7420 7468 6520 7175  represent the qu
+00000ad0: 6572 7920 7465 7874 2061 6e64 2074 6865  ery text and the
+00000ae0: 2072 656d 6169 6e69 6e67 2070 6f73 6974   remaining posit
+00000af0: 696f 6e73 0a20 2020 2072 6570 7265 7365  ions.    represe
+00000b00: 6e74 2074 6865 2072 6566 6572 656e 6365  nt the reference
+00000b10: 2074 6578 742c 2072 6574 7572 6e20 6120   text, return a 
+00000b20: 6c69 7374 2069 6e64 6963 6174 696e 672c  list indicating,
+00000b30: 2066 6f72 2065 6163 6820 7375 6666 6978   for each suffix
+00000b40: 0a20 2020 2070 6f73 6974 696f 6e20 696e  .    position in
+00000b50: 2074 6865 2071 7565 7279 2074 6578 742c   the query text,
+00000b60: 2074 6865 2074 776f 2073 7566 6669 7820   the two suffix 
+00000b70: 706f 7369 7469 6f6e 7320 696e 2074 6865  positions in the
+00000b80: 2072 6566 6572 656e 6365 2074 6578 740a   reference text.
+00000b90: 2020 2020 7468 6174 2069 6d6d 6564 6961      that immedia
+00000ba0: 7465 6c79 2070 7265 6365 6465 2061 6e64  tely precede and
+00000bb0: 2066 6f6c 6c6f 7720 6974 206c 6578 6963   follow it lexic
+00000bc0: 6f67 7261 7068 6963 616c 6c79 2e20 2028  ographically.  (
+00000bd0: 4920 7468 696e 6b20 7375 6666 6978 0a20  I think suffix. 
+00000be0: 2020 2070 6f73 6974 696f 6e20 7265 6665     position refe
+00000bf0: 7273 2074 6f20 7468 6520 6c61 7374 2063  rs to the last c
+00000c00: 6861 7261 6374 6572 206f 6620 6120 7375  haracter of a su
+00000c10: 6666 6978 292e 0a0a 2020 2020 5468 6973  ffix)...    This
+00000c20: 2069 7320 6561 7379 2074 6f20 646f 2066   is easy to do f
+00000c30: 726f 6d20 7468 6520 7375 6666 6978 2061  rom the suffix a
+00000c40: 7272 6179 2077 6974 686f 7574 2063 6f6d  rray without com
+00000c50: 7075 7469 6e67 2c20 666f 7220 6578 616d  puting, for exam
+00000c60: 706c 652c 0a20 2020 2074 6865 204c 4350  ple,.    the LCP
+00000c70: 2061 7272 6179 3b20 616e 6420 6974 2070   array; and it p
+00000c80: 726f 6475 6365 7320 6578 6163 746c 7920  roduces exactly 
+00000c90: 3220 6d61 7463 6865 7320 7065 7220 706f  2 matches per po
+00000ca0: 7369 7469 6f6e 2069 6e20 7468 6520 7175  sition in the qu
+00000cb0: 6572 790a 2020 2020 7465 7874 2c20 7768  ery.    text, wh
+00000cc0: 6963 6820 6973 2061 6c73 6f20 636f 6e76  ich is also conv
+00000cd0: 656e 6965 6e74 2e0a 0a20 2020 2028 4e6f  enient...    (No
+00000ce0: 7465 3a20 7468 6520 7175 6572 7920 616e  te: the query an
+00000cf0: 6420 7265 6665 7265 6e63 6520 7465 7874  d reference text
+00000d00: 7320 636f 756c 6420 6561 6368 2072 6570  s could each rep
+00000d10: 7265 7365 6e74 206d 756c 7469 706c 6520  resent multiple 
+00000d20: 7365 7061 7261 7465 0a20 2020 2073 6571  separate.    seq
+00000d30: 7565 6e63 6573 2c20 6275 7420 7468 6174  uences, but that
+00000d40: 2069 7320 6861 6e64 6c65 6420 6279 206f   is handled by o
+00000d50: 7468 6572 2063 6f64 653b 2063 6c61 7373  ther code; class
+00000d60: 2053 6f75 7263 6564 5465 7874 206b 6565   SourcedText kee
+00000d70: 7073 2074 7261 636b 0a20 2020 206f 6620  ps track.    of 
+00000d80: 7468 6174 2069 6e66 6f72 6d61 7469 6f6e  that information
+00000d90: 2e29 0a0a 2020 2020 4172 6773 3a0a 2020  .)..    Args:.  
+00000da0: 2020 2073 7566 6669 785f 6172 7261 793a     suffix_array:
+00000db0: 0a20 2020 2020 2020 4120 7375 6666 6978  .       A suffix
+00000dc0: 2061 7272 6179 2061 7320 6372 6561 7465   array as create
+00000dd0: 6420 6279 203a 6675 6e63 3a60 6372 6561  d by :func:`crea
+00000de0: 7465 5f73 7566 6669 785f 6172 7261 7960  te_suffix_array`
+00000df0: 2c20 6f66 2064 7479 7065 0a20 2020 2020  , of dtype.     
+00000e00: 2020 6060 6e70 2e69 6e74 3332 6060 2061    ``np.int32`` a
+00000e10: 6e64 2073 6861 7065 2060 6028 7365 715f  nd shape ``(seq_
+00000e20: 6c65 6e2c 2960 602e 0a0a 2020 2020 2071  len,)``...     q
+00000e30: 7565 7279 5f6c 656e 3a0a 2020 2020 2020  uery_len:.      
+00000e40: 2041 206e 756d 6265 7220 6060 3020 3c3d   A number ``0 <=
+00000e50: 2071 7565 7279 5f6c 656e 203c 2073 6571   query_len < seq
+00000e60: 5f6c 656e 6060 2c20 696e 6469 6361 7469  _len``, indicati
+00000e70: 6e67 2074 6865 206c 656e 6774 6820 696e  ng the length in
+00000e80: 2073 796d 626f 6c73 0a20 2020 2020 2020   symbols.       
+00000e90: 286c 696b 656c 7920 6279 7465 7329 206f  (likely bytes) o
+00000ea0: 6620 7468 6520 7175 6572 7920 7061 7274  f the query part
+00000eb0: 206f 6620 7468 6520 7465 7874 2074 6861   of the text tha
+00000ec0: 7420 7761 7320 7573 6564 2074 6f20 6372  t was used to cr
+00000ed0: 6561 7465 0a20 2020 2020 2020 6060 7375  eate.       ``su
+00000ee0: 6666 6978 5f61 7272 6179 6060 2e0a 0a20  ffix_array``... 
+00000ef0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00000f00: 2020 5265 7475 726e 2061 6e20 6e70 2e6e    Return an np.n
+00000f10: 6461 7272 6179 206f 6620 7368 6170 6520  darray of shape 
+00000f20: 6060 2871 7565 7279 5f6c 656e 202a 2032  ``(query_len * 2
+00000f30: 2c29 6060 2c20 6f66 2074 6865 2073 616d  ,)``, of the sam
+00000f40: 6520 6474 7970 6520 6173 0a20 2020 2020  e dtype as.     
+00000f50: 2060 6073 7566 6669 785f 6172 7261 7960   ``suffix_array`
+00000f60: 602c 2069 6e20 7768 6963 6820 706f 7369  `, in which posi
+00000f70: 7469 6f6e 7320 6060 322a 6960 6020 616e  tions ``2*i`` an
+00000f80: 6420 6060 322a 6920 2b20 3160 6020 7265  d ``2*i + 1`` re
+00000f90: 7072 6573 656e 740a 2020 2020 2020 7468  present.      th
+00000fa0: 6520 7477 6f20 706f 7369 7469 6f6e 7320  e two positions 
+00000fb0: 696e 2074 6865 206f 7269 6769 6e61 6c20  in the original 
+00000fc0: 7465 7874 2074 6861 7420 6172 6520 7769  text that are wi
+00000fd0: 7468 696e 2074 6865 2072 6566 6572 656e  thin the referen
+00000fe0: 6365 0a20 2020 2020 2070 6f72 7469 6f6e  ce.      portion
+00000ff0: 2c20 616e 6420 7768 6963 6820 696d 6d65  , and which imme
+00001000: 6469 6174 656c 7920 7072 6563 6564 6520  diately precede 
+00001010: 616e 6420 666f 6c6c 6f77 2c20 696e 2074  and follow, in t
+00001020: 6865 2073 7566 6669 7820 6172 7261 792c  he suffix array,
+00001030: 0a20 2020 2020 2071 7565 7279 2070 6f73  .      query pos
+00001040: 6974 696f 6e20 6060 6960 602e 2020 5468  ition ``i``.  Th
+00001050: 6973 206d 6561 6e73 2074 6861 7420 7468  is means that th
+00001060: 6520 7375 6666 6978 6573 2065 6e64 696e  e suffixes endin
+00001070: 6720 6174 2074 686f 7365 0a20 2020 2020  g at those.     
+00001080: 2070 6f73 6974 696f 6e73 2061 7265 2072   positions are r
+00001090: 6576 6572 7365 2d6c 6578 6963 6f67 7261  everse-lexicogra
+000010a0: 7068 6963 616c 6c79 2063 6c6f 7365 2074  phically close t
+000010b0: 6f20 7468 6520 7375 6666 6978 2065 6e64  o the suffix end
+000010c0: 696e 6720 6174 0a20 2020 2020 2070 6f73  ing at.      pos
+000010d0: 6974 696f 6e20 6060 6960 602e 2020 4173  ition ``i``.  As
+000010e0: 2061 2073 7065 6369 616c 2063 6173 652c   a special case,
+000010f0: 2069 6620 6f6e 6520 6f66 2074 6865 7365   if one of these
+00001100: 2072 6574 7572 6e65 6420 6e75 6d62 6572   returned number
+00001110: 7320 776f 756c 640a 2020 2020 2020 6571  s would.      eq
+00001120: 7561 6c20 7468 6520 454f 5320 706f 7369  ual the EOS posi
+00001130: 7469 6f6e 2028 706f 7369 7469 6f6e 2073  tion (position s
+00001140: 6571 5f6c 656e 202d 2031 292c 206f 7220  eq_len - 1), or 
+00001150: 6966 2061 2071 7565 7279 2070 6f73 6974  if a query posit
+00001160: 696f 6e20 6973 0a20 2020 2020 2062 6566  ion is.      bef
+00001170: 6f72 6520 616e 7920 7265 6665 7265 6e63  ore any referenc
+00001180: 6520 706f 7369 7469 6f6e 2069 6e20 7468  e position in th
+00001190: 6520 7375 6666 6978 2061 7261 792c 2077  e suffix aray, w
+000011a0: 6520 6f75 7470 7574 0a20 2020 2020 2060  e output.      `
+000011b0: 6073 6571 5f6c 656e 202d 2032 6060 2069  `seq_len - 2`` i
+000011c0: 6e73 7465 6164 2074 6f20 6176 6f69 6420  nstead to avoid 
+000011d0: 6861 7669 6e67 2074 6f20 6861 6e64 6c65  having to handle
+000011e0: 2073 7065 6369 616c 2063 6173 6573 206c   special cases l
+000011f0: 6174 6572 206f 6e0a 2020 2020 2020 2861  ater on.      (a
+00001200: 6e79 7761 792c 2074 6865 7365 2077 6f75  nyway, these wou
+00001210: 6c64 206e 6f74 2072 6570 7265 7365 6e74  ld not represent
+00001220: 2061 2063 6c6f 7365 206d 6174 6368 292e   a close match).
+00001230: 0a0a 2020 2020 2e2e 2068 696e 743a 3a0a  ..    .. hint::.
+00001240: 0a20 2020 2020 2020 2050 6c65 6173 6520  .        Please 
+00001250: 7265 6665 7220 746f 203a 7265 663a 6066  refer to :ref:`f
+00001260: 696e 645f 636c 6f73 655f 6d61 7463 6865  ind_close_matche
+00001270: 735f 7475 746f 7269 616c 6020 666f 7220  s_tutorial` for 
+00001280: 7573 6167 6573 2e0a 2020 2020 7201 0000  usages..    r...
+00001290: 0072 1200 0000 e902 0000 0029 02da 0a66  .r.........)...f
+000012a0: 696c 6c5f 7661 6c75 6572 0600 0000 2909  ill_valuer....).
+000012b0: 7214 0000 0072 1300 0000 7206 0000 0072  r....r....r....r
+000012c0: 0700 0000 720c 0000 0072 0b00 0000 da04  ....r....r......
+000012d0: 6675 6c6c da05 7261 6e67 65da 046c 6973  full..range..lis
+000012e0: 7429 0b72 1d00 0000 721e 0000 0072 1f00  t).r....r....r..
+000012f0: 0000 da07 7365 715f 6c65 6eda 066f 7574  ....seq_len..out
+00001300: 7075 745a 0970 7265 765f 7265 6673 5a0c  putZ.prev_refsZ.
+00001310: 756e 6669 6e69 7368 6564 5f71 5a0a 7265  unfinished_qZ.re
+00001320: 6673 5f69 6e64 6578 da01 695a 0874 6578  fs_index..iZ.tex
+00001330: 745f 706f 73da 016b 720f 0000 0072 0f00  t_pos..kr....r..
+00001340: 0000 7210 0000 00da 1266 696e 645f 636c  ..r......find_cl
+00001350: 6f73 655f 6d61 7463 6865 735c 0000 0073  ose_matches\...s
+00001360: 3800 0000 002d 1001 1401 1601 0601 1402  8....-..........
+00001370: 1002 0401 0a01 0601 04fd 0606 0e04 0402  ................
+00001380: 0401 1001 0801 0a01 0c01 0801 0c01 1001  ................
+00001390: 1601 0802 1402 0c01 1402 0a02 7229 0000  ............r)..
+000013a0: 0029 0172 1200 0000 2908 7219 0000 00da  .).r....).r.....
+000013b0: 056e 756d 7079 7207 0000 00da 076e 6461  .numpyr......nda
+000013c0: 7272 6179 7211 0000 0072 1a00 0000 da03  rrayr....r......
+000013d0: 696e 7472 2900 0000 720f 0000 0072 0f00  intr)...r....r..
+000013e0: 0000 720f 0000 0072 1000 0000 da08 3c6d  ..r....r......<m
+000013f0: 6f64 756c 653e 1100 0000 7314 0000 0008  odule>....s.....
+00001400: 0108 0314 1914 2f00 ff02 0104 0002 0002  ....../.........
+00001410: 0104 fe                                  ...
```

### Comparing `fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/text_search.cpython-38.pyc` & `fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/text_search.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/textsearch/__pycache__/utils.cpython-38.pyc` & `fasttextsearch-0.5/textsearch/python/textsearch/__pycache__/utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue May 16 07:26:31 2023 UTC, .py size: 3165 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2730 6364 5d0c 0000  U.......'0cd]...
+00000000: 550d 0d0a 0000 0000 78e1 6564 610c 0000  U.......x.eda...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a06 6400 6404 6c07 6d08 5a09 0100 4700  Z.d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 650a 8303 5a0b 6506  d.d...d.e...Z.e.
 00000070: 6a0c 6506 6a0c 6407 9c02 6408 6409 8404  j.e.j.d...d.d...
@@ -23,186 +23,186 @@
 00000160: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
 00000170: 2400 0000 7c01 7c00 6b06 7210 7c00 7c01  $...|.|.k.r.|.|.
 00000180: 1900 5300 7400 6401 7c01 9b00 6402 9d03  ..S.t.d.|...d...
 00000190: 8301 8201 6400 5300 a903 4e7a 134e 6f20  ....d.S...Nz.No 
 000001a0: 7375 6368 2061 7474 7269 6275 7465 2027  such attribute '
 000001b0: fa01 27a9 01da 0e41 7474 7269 6275 7465  ..'....Attribute
 000001c0: 4572 726f 72a9 02da 0473 656c 66da 036b  Error....self..k
-000001d0: 6579 a900 720e 0000 00fa 482f 6365 7068  ey..r.....H/ceph
-000001e0: 2d68 772f 6b61 6e67 7765 692f 636f 6465  -hw/kangwei/code
-000001f0: 322f 7465 7874 5f73 6561 7263 682f 7465  2/text_search/te
-00000200: 7874 7365 6172 6368 2f70 7974 686f 6e2f  xtsearch/python/
-00000210: 7465 7874 7365 6172 6368 2f75 7469 6c73  textsearch/utils
-00000220: 2e70 79da 0b5f 5f67 6574 6174 7472 5f5f  .py..__getattr__
-00000230: 0800 0000 7306 0000 0000 0108 0108 017a  ....s..........z
-00000240: 1941 7474 7269 6275 7465 4469 6374 2e5f  .AttributeDict._
-00000250: 5f67 6574 6174 7472 5f5f 6303 0000 0000  _getattr__c.....
-00000260: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
-00000270: 0000 0073 0c00 0000 7c02 7c00 7c01 3c00  ...s....|.|.|.<.
-00000280: 6400 5300 2901 4e72 0e00 0000 2903 720c  d.S.).Nr....).r.
-00000290: 0000 0072 0d00 0000 da05 7661 6c75 6572  ...r......valuer
-000002a0: 0e00 0000 720e 0000 0072 0f00 0000 da0b  ....r....r......
-000002b0: 5f5f 7365 7461 7474 725f 5f0d 0000 0073  __setattr__....s
-000002c0: 0200 0000 0001 7a19 4174 7472 6962 7574  ......z.Attribut
-000002d0: 6544 6963 742e 5f5f 7365 7461 7474 725f  eDict.__setattr_
-000002e0: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
-000002f0: 0000 0400 0000 4300 0000 7326 0000 007c  ......C...s&...|
-00000300: 017c 006b 0672 127c 007c 013d 0064 0053  .|.k.r.|.|.=.d.S
-00000310: 0074 0064 017c 019b 0064 029d 0383 0182  .t.d.|...d......
-00000320: 0164 0053 0072 0700 0000 7209 0000 0072  .d.S.r....r....r
-00000330: 0b00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00000340: 0000 00da 0b5f 5f64 656c 6174 7472 5f5f  .....__delattr__
-00000350: 1000 0000 7308 0000 0000 0108 0106 0104  ....s...........
-00000360: 017a 1941 7474 7269 6275 7465 4469 6374  .z.AttributeDict
-00000370: 2e5f 5f64 656c 6174 7472 5f5f 4e29 06da  .__delattr__N)..
-00000380: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000390: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000003a0: 655f 5f72 1000 0000 7212 0000 0072 1300  e__r....r....r..
-000003b0: 0000 720e 0000 0072 0e00 0000 720e 0000  ..r....r....r...
-000003c0: 0072 0f00 0000 7206 0000 0007 0000 0073  .r....r........s
-000003d0: 0600 0000 0801 0805 0803 7206 0000 0029  ..........r....)
-000003e0: 02da 0772 6f77 5f69 6473 da06 7265 7475  ...row_ids..retu
-000003f0: 726e 6301 0000 0000 0000 0000 0000 0003  rnc.............
-00000400: 0000 0004 0000 0043 0000 0073 6200 0000  .......C...sb...
-00000410: 7c00 6a00 6401 6b02 7314 7401 7c00 6a00  |.j.d.k.s.t.|.j.
-00000420: 8301 8201 7c00 6a02 7403 6a04 6b02 732a  ....|.j.t.j.k.s*
-00000430: 7401 7c00 6a02 8301 8201 7403 a005 7c00  t.|.j.....t...|.
-00000440: a101 7d00 7c00 6402 1900 6401 1700 7d01  ..}.|.d...d...}.
-00000450: 7403 6a06 7c01 6401 1700 7403 6a04 6403  t.j.|.d...t.j.d.
-00000460: 8d02 7d02 7407 7c00 7c02 8302 0100 7c02  ..}.t.|.|.....|.
-00000470: 5300 2904 7ac8 436f 6e76 6572 7420 726f  S.).z.Convert ro
-00000480: 7720 6964 7320 746f 2072 6f77 2073 706c  w ids to row spl
-00000490: 6974 732e 0a0a 2020 2020 4172 6773 3a0a  its...    Args:.
-000004a0: 2020 2020 2020 726f 775f 6964 733a 0a20        row_ids:. 
-000004b0: 2020 2020 2020 2041 2031 2d44 2061 7272         A 1-D arr
-000004c0: 6179 206f 6620 6474 7970 6520 6e70 2e75  ay of dtype np.u
-000004d0: 696e 7433 3220 636f 6e74 6169 6e69 6e67  int32 containing
-000004e0: 2072 6f77 2069 6473 2e0a 2020 2020 5265   row ids..    Re
-000004f0: 7475 726e 733a 0a20 2020 2020 2052 6574  turns:.      Ret
-00000500: 7572 6e20 6120 312d 4420 6172 7261 7920  urn a 1-D array 
-00000510: 6f66 2064 7479 7065 206e 702e 7569 6e74  of dtype np.uint
-00000520: 3332 2063 6f6e 7461 696e 696e 6720 726f  32 containing ro
-00000530: 7720 7370 6c69 7473 2e0a 2020 2020 e901  w splits..    ..
-00000540: 0000 00e9 ffff ffff 2901 da05 6474 7970  ........)...dtyp
-00000550: 6529 08da 046e 6469 6dda 0e41 7373 6572  e)...ndim..Asser
-00000560: 7469 6f6e 4572 726f 7272 1b00 0000 da02  tionErrorr......
-00000570: 6e70 da06 7569 6e74 3332 da11 6173 636f  np..uint32..asco
-00000580: 6e74 6967 756f 7573 6172 7261 79da 0565  ntiguousarray..e
-00000590: 6d70 7479 da16 5f72 6f77 5f69 6473 5f74  mpty.._row_ids_t
-000005a0: 6f5f 726f 775f 7370 6c69 7473 2903 7217  o_row_splits).r.
-000005b0: 0000 005a 086e 756d 5f72 6f77 735a 0a72  ...Z.num_rowsZ.r
-000005c0: 6f77 5f73 706c 6974 7372 0e00 0000 720e  ow_splitsr....r.
-000005d0: 0000 0072 0f00 0000 7205 0000 0017 0000  ...r....r.......
-000005e0: 0073 0e00 0000 0009 1401 1602 0a01 0c01  .s..............
-000005f0: 1402 0a01 7205 0000 00e7 0000 0000 0000  ....r...........
-00000600: e03f 2904 da06 7261 6e67 6573 da05 7175  .?)...ranges..qu
-00000610: 6572 79da 0d6f 7665 726c 6170 5f72 6174  ery..overlap_rat
-00000620: 696f 7218 0000 0063 0300 0000 0000 0000  ior....c........
-00000630: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
-00000640: 7362 0100 0064 017d 0374 007c 007c 0183  sb...d.}.t.|.|..
-00000650: 027d 047c 0464 026b 0272 5e7c 0072 5c7c  .}.|.d.k.r^|.r\|
-00000660: 0164 0319 007c 0064 0219 0064 0219 0018  .d...|.d...d....
-00000670: 0074 017c 0064 0219 0064 0319 007c 0064  .t.|.d...d...|.d
-00000680: 0219 0064 0219 0018 007c 0164 0319 007c  ...d.....|.d...|
-00000690: 0164 0219 0018 0083 027c 0214 006b 047d  .d.......|...k.}
-000006a0: 036e ee7c 0474 027c 0083 016b 0272 ba7c  .n.|.t.|...k.r.|
-000006b0: 007c 0464 0318 0019 0064 0319 007c 0164  .|.d.....d...|.d
-000006c0: 0219 0018 0074 017c 007c 0464 0318 0019  .....t.|.|.d....
-000006d0: 0064 0319 007c 007c 0464 0318 0019 0064  .d...|.|.d.....d
-000006e0: 0219 0018 007c 0164 0319 007c 0164 0219  .....|.d...|.d..
-000006f0: 0018 0083 027c 0214 006b 047d 036e 927c  .....|...k.}.n.|
-00000700: 007c 0464 0318 0019 0064 0319 007c 0164  .|.d.....d...|.d
-00000710: 0219 0018 0074 017c 007c 0464 0318 0019  .....t.|.|.d....
-00000720: 0064 0319 007c 007c 0464 0318 0019 0064  .d...|.|.d.....d
-00000730: 0219 0018 007c 0164 0319 007c 0164 0219  .....|.d...|.d..
-00000740: 0018 0083 027c 0214 006b 0490 0170 4a7c  .....|...k...pJ|
-00000750: 0164 0319 007c 007c 0419 0064 0219 0018  .d...|.|...d....
-00000760: 0074 017c 007c 0419 0064 0319 007c 007c  .t.|.|...d...|.|
-00000770: 0419 0064 0219 0018 007c 0164 0319 007c  ...d.....|.d...|
-00000780: 0164 0219 0018 0083 027c 0214 006b 047d  .d.......|...k.}
-00000790: 037c 0390 0173 5e7c 00a0 037c 047c 01a1  .|...s^|...|.|..
-000007a0: 0201 007c 0353 0029 0461 6602 0000 0a20  ...|.S.).af.... 
-000007b0: 2020 2052 6574 7572 6e20 6966 2074 6865     Return if the
-000007c0: 2067 6976 656e 2072 616e 6765 206f 7665   given range ove
-000007d0: 726c 6170 7320 7769 7468 2074 6865 2065  rlaps with the e
-000007e0: 7869 7374 696e 6720 7261 6e67 6573 2e0a  xisting ranges..
-000007f0: 0a20 2020 2043 6175 7469 6f6e 3a0a 2020  .    Caution:.  
-00000800: 2020 2020 6072 616e 6765 7360 2077 696c      `ranges` wil
-00000810: 6c20 6265 206d 6f64 6966 6965 6420 696e  l be modified in
-00000820: 2074 6869 7320 6675 6e63 7469 6f6e 2028   this function (
-00000830: 7768 656e 2072 6574 7572 6e69 6e67 2046  when returning F
-00000840: 616c 7365 290a 0a20 2020 204e 6f74 653a  alse)..    Note:
-00000850: 206f 7665 726c 6170 7069 6e67 2068 6572   overlapping her
-00000860: 6520 6d65 616e 7320 7468 6520 6c65 6e67  e means the leng
-00000870: 7468 206f 6620 6f76 6572 6c61 7070 696e  th of overlappin
-00000880: 6720 6172 6561 2069 7320 6772 6561 7465  g area is greate
-00000890: 7220 7468 616e 0a20 2020 2073 6f6d 6520  r than.    some 
-000008a0: 7468 7265 7368 6f6c 6420 2863 7572 7265  threshold (curre
-000008b0: 6e74 6c79 2c20 7468 6520 7468 7265 7368  ntly, the thresh
-000008c0: 6f6c 6420 6973 2060 6f76 6572 6c61 705f  old is `overlap_
-000008d0: 7261 7469 6f60 206d 756c 7469 706c 7920  ratio` multiply 
-000008e0: 7468 6520 6c65 6e67 7468 0a20 2020 206f  the length.    o
-000008f0: 6620 7468 6520 7368 6f72 7465 7220 6f76  f the shorter ov
-00000900: 6572 6c61 7070 696e 6720 7261 6e67 6573  erlapping ranges
-00000910: 292e 0a0a 2020 2020 4172 6773 3a0a 2020  )...    Args:.  
-00000920: 2020 2020 7261 6e67 6573 3a0a 2020 2020      ranges:.    
-00000930: 2020 2020 5468 6520 6578 6973 7469 6e67      The existing
-00000940: 2072 616e 6765 732c 2069 7420 6973 2073   ranges, it is s
-00000950: 6f72 7465 6420 696e 2061 7363 656e 6469  orted in ascendi
-00000960: 6e67 206f 7264 6572 206f 6e20 696e 7075  ng order on inpu
-00000970: 742c 2061 6e64 2077 6520 7769 6c6c 0a20  t, and we will. 
-00000980: 2020 2020 2020 206b 6565 7020 6974 2073         keep it s
-00000990: 6f72 7465 6420 696e 2074 6869 7320 6675  orted in this fu
-000009a0: 6e63 7469 6f6e 2e0a 2020 2020 2020 7175  nction..      qu
-000009b0: 6572 793a 0a20 2020 2020 2020 2054 6865  ery:.        The
-000009c0: 2067 6976 656e 2072 616e 6765 2e0a 0a20   given range... 
-000009d0: 2020 2052 6574 7572 6e3a 0a20 2020 2020     Return:.     
-000009e0: 2052 6574 7572 6e20 5472 7565 2069 6620   Return True if 
-000009f0: 6861 7669 6e67 206f 7665 726c 6170 206f  having overlap o
-00000a00: 7468 6572 7769 7365 2046 616c 7365 2e0a  therwise False..
-00000a10: 2020 2020 4672 0100 0000 7219 0000 0029      Fr....r....)
-00000a20: 0472 0200 0000 da03 6d69 6eda 036c 656e  .r......min..len
-00000a30: da06 696e 7365 7274 2905 7224 0000 0072  ..insert).r$...r
-00000a40: 2500 0000 7226 0000 00da 0a69 735f 6f76  %...r&.....is_ov
-00000a50: 6572 6c61 70da 0569 6e64 6578 720e 0000  erlap..indexr...
-00000a60: 0072 0e00 0000 720f 0000 0072 2a00 0000  .r....r....r*...
-00000a70: 2b00 0000 733c 0000 0000 1704 010a 0108  +...s<..........
-00000a80: 0104 0212 012c ff02 ff04 040c 0216 0130  .....,.........0
-00000a90: 0102 ff02 ff02 ff04 0716 0130 0102 ff02  ...........0....
-00000aa0: ff02 ff04 0512 0128 0102 ff02 ff02 fb02  .......(........
-00000ab0: 0a06 010c 0172 2a00 0000 4629 03da 0163  .....r*...F)...c
-00000ac0: da08 656f 735f 6f6e 6c79 7218 0000 0063  ..eos_onlyr....c
-00000ad0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000ae0: 0200 0000 4300 0000 7314 0000 007c 0172  ....C...s....|.r
-00000af0: 0c7c 0064 016b 0653 007c 0064 026b 0653  .|.d.k.S.|.d.k.S
-00000b00: 0029 037a db0a 2020 2020 5265 7475 726e  .).z..    Return
-00000b10: 2054 7275 6520 6966 2074 6865 2067 6976   True if the giv
-00000b20: 656e 2063 6861 7261 6374 6572 2069 7320  en character is 
-00000b30: 6120 7075 6e63 7475 6174 696f 6e2e 0a0a  a punctuation...
-00000b40: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00000b50: 633a 0a20 2020 2020 2020 2054 6865 2067  c:.        The g
-00000b60: 6976 656e 2063 6861 7261 6374 6572 2e0a  iven character..
-00000b70: 2020 2020 2020 656f 735f 6f6e 6c79 3a0a        eos_only:.
-00000b80: 2020 2020 2020 2020 4966 2054 7275 6520          If True 
-00000b90: 7468 6520 7075 6e63 7475 6174 696f 6e73  the punctuations
-00000ba0: 2061 7265 206f 6e6c 7920 7468 6f73 6520   are only those 
-00000bb0: 696e 6469 6361 7469 6e67 2065 6e64 206f  indicating end o
-00000bc0: 6620 6120 7365 6e74 656e 6365 2028 2e3f  f a sentence (.?
-00000bd0: 2120 666f 7220 6e6f 7729 2e0a 2020 2020  ! for now)..    
-00000be0: 7a03 2e3f 217a 0e2c 2e3b 3f21 2829 3a2d  z..?!z.,.;?!():-
-00000bf0: 3c3e 2d2f 2272 0e00 0000 2902 722c 0000  <>-/"r....).r,..
-00000c00: 0072 2d00 0000 720e 0000 0072 0e00 0000  .r-...r....r....
-00000c10: 720f 0000 00da 0e69 735f 7075 6e63 7475  r......is_punctu
-00000c20: 6174 696f 6e60 0000 0073 0600 0000 000a  ation`...s......
-00000c30: 0401 0801 722e 0000 0029 0172 2300 0000  ....r....).r#...
-00000c40: 2901 4629 13da 0662 6973 6563 7472 0200  ).F)...bisectr..
-00000c50: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
-00000c60: 0400 0000 da05 6e75 6d70 7972 1e00 0000  ......numpyr....
-00000c70: da0b 5f74 6578 7473 6561 7263 6872 0500  .._textsearchr..
-00000c80: 0000 7222 0000 00da 0464 6963 7472 0600  ..r".....dictr..
-00000c90: 0000 da07 6e64 6172 7261 79da 0369 6e74  ....ndarray..int
-00000ca0: da05 666c 6f61 74da 0462 6f6f 6c72 2a00  ..float..boolr*.
-00000cb0: 0000 da03 7374 7272 2e00 0000 720e 0000  ....strr....r...
-00000cc0: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00000cd0: da08 3c6d 6f64 756c 653e 0100 0000 731a  ..<module>....s.
-00000ce0: 0000 000c 0110 0108 010c 0310 1014 1500  ................
-00000cf0: ff02 010e 000a 0002 0102 fe0c 35         ............5
+000001d0: 6579 a900 720e 0000 00fa 472f 6365 7068  ey..r.....G/ceph
+000001e0: 2d6b 772f 6b61 6e67 7765 692f 636f 6465  -kw/kangwei/code
+000001f0: 2f74 6578 745f 7365 6172 6368 2f74 6578  /text_search/tex
+00000200: 7473 6561 7263 682f 7079 7468 6f6e 2f74  tsearch/python/t
+00000210: 6578 7473 6561 7263 682f 7574 696c 732e  extsearch/utils.
+00000220: 7079 da0b 5f5f 6765 7461 7474 725f 5f08  py..__getattr__.
+00000230: 0000 0073 0600 0000 0001 0801 0801 7a19  ...s..........z.
+00000240: 4174 7472 6962 7574 6544 6963 742e 5f5f  AttributeDict.__
+00000250: 6765 7461 7474 725f 5f63 0300 0000 0000  getattr__c......
+00000260: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
+00000270: 0000 730c 0000 007c 027c 007c 013c 0064  ..s....|.|.|.<.d
+00000280: 0053 0029 014e 720e 0000 0029 0372 0c00  .S.).Nr....).r..
+00000290: 0000 720d 0000 00da 0576 616c 7565 720e  ..r......valuer.
+000002a0: 0000 0072 0e00 0000 720f 0000 00da 0b5f  ...r....r......_
+000002b0: 5f73 6574 6174 7472 5f5f 0d00 0000 7302  _setattr__....s.
+000002c0: 0000 0000 017a 1941 7474 7269 6275 7465  .....z.Attribute
+000002d0: 4469 6374 2e5f 5f73 6574 6174 7472 5f5f  Dict.__setattr__
+000002e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000002f0: 0004 0000 0043 0000 0073 2600 0000 7c01  .....C...s&...|.
+00000300: 7c00 6b06 7212 7c00 7c01 3d00 6400 5300  |.k.r.|.|.=.d.S.
+00000310: 7400 6401 7c01 9b00 6402 9d03 8301 8201  t.d.|...d.......
+00000320: 6400 5300 7207 0000 0072 0900 0000 720b  d.S.r....r....r.
+00000330: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
+00000340: 0000 da0b 5f5f 6465 6c61 7474 725f 5f10  ....__delattr__.
+00000350: 0000 0073 0800 0000 0001 0801 0601 0401  ...s............
+00000360: 7a19 4174 7472 6962 7574 6544 6963 742e  z.AttributeDict.
+00000370: 5f5f 6465 6c61 7474 725f 5f4e 2906 da08  __delattr__N)...
+00000380: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000390: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000003a0: 5f5f 7210 0000 0072 1200 0000 7213 0000  __r....r....r...
+000003b0: 0072 0e00 0000 720e 0000 0072 0e00 0000  .r....r....r....
+000003c0: 720f 0000 0072 0600 0000 0700 0000 7306  r....r........s.
+000003d0: 0000 0008 0108 0508 0372 0600 0000 2902  .........r....).
+000003e0: da07 726f 775f 6964 73da 0672 6574 7572  ..row_ids..retur
+000003f0: 6e63 0100 0000 0000 0000 0000 0000 0300  nc..............
+00000400: 0000 0400 0000 4300 0000 7362 0000 007c  ......C...sb...|
+00000410: 006a 0064 016b 0273 1474 017c 006a 0083  .j.d.k.s.t.|.j..
+00000420: 0182 017c 006a 0274 036a 046b 0273 2a74  ...|.j.t.j.k.s*t
+00000430: 017c 006a 0283 0182 0174 03a0 057c 00a1  .|.j.....t...|..
+00000440: 017d 007c 0064 0219 0064 0117 007d 0174  .}.|.d...d...}.t
+00000450: 036a 067c 0164 0117 0074 036a 0464 038d  .j.|.d...t.j.d..
+00000460: 027d 0274 077c 007c 0283 0201 007c 0253  .}.t.|.|.....|.S
+00000470: 0029 047a c843 6f6e 7665 7274 2072 6f77  .).z.Convert row
+00000480: 2069 6473 2074 6f20 726f 7720 7370 6c69   ids to row spli
+00000490: 7473 2e0a 0a20 2020 2041 7267 733a 0a20  ts...    Args:. 
+000004a0: 2020 2020 2072 6f77 5f69 6473 3a0a 2020       row_ids:.  
+000004b0: 2020 2020 2020 4120 312d 4420 6172 7261        A 1-D arra
+000004c0: 7920 6f66 2064 7479 7065 206e 702e 7569  y of dtype np.ui
+000004d0: 6e74 3332 2063 6f6e 7461 696e 696e 6720  nt32 containing 
+000004e0: 726f 7720 6964 732e 0a20 2020 2052 6574  row ids..    Ret
+000004f0: 7572 6e73 3a0a 2020 2020 2020 5265 7475  urns:.      Retu
+00000500: 726e 2061 2031 2d44 2061 7272 6179 206f  rn a 1-D array o
+00000510: 6620 6474 7970 6520 6e70 2e75 696e 7433  f dtype np.uint3
+00000520: 3220 636f 6e74 6169 6e69 6e67 2072 6f77  2 containing row
+00000530: 2073 706c 6974 732e 0a20 2020 20e9 0100   splits..    ...
+00000540: 0000 e9ff ffff ff29 01da 0564 7479 7065  .......)...dtype
+00000550: 2908 da04 6e64 696d da0e 4173 7365 7274  )...ndim..Assert
+00000560: 696f 6e45 7272 6f72 721b 0000 00da 026e  ionErrorr......n
+00000570: 70da 0675 696e 7433 32da 1161 7363 6f6e  p..uint32..ascon
+00000580: 7469 6775 6f75 7361 7272 6179 da05 656d  tiguousarray..em
+00000590: 7074 79da 165f 726f 775f 6964 735f 746f  pty.._row_ids_to
+000005a0: 5f72 6f77 5f73 706c 6974 7329 0372 1700  _row_splits).r..
+000005b0: 0000 da08 6e75 6d5f 726f 7773 5a0a 726f  ....num_rowsZ.ro
+000005c0: 775f 7370 6c69 7473 720e 0000 0072 0e00  w_splitsr....r..
+000005d0: 0000 720f 0000 0072 0500 0000 1700 0000  ..r....r........
+000005e0: 730e 0000 0000 0914 0116 020a 010c 0114  s...............
+000005f0: 020a 0172 0500 0000 e700 0000 0000 00e0  ...r............
+00000600: 3f29 04da 0672 616e 6765 73da 0571 7565  ?)...ranges..que
+00000610: 7279 da0d 6f76 6572 6c61 705f 7261 7469  ry..overlap_rati
+00000620: 6f72 1800 0000 6303 0000 0000 0000 0000  or....c.........
+00000630: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
+00000640: 6201 0000 6401 7d03 7400 7c00 7c01 8302  b...d.}.t.|.|...
+00000650: 7d04 7c04 6402 6b02 725e 7c00 725c 7c01  }.|.d.k.r^|.r\|.
+00000660: 6403 1900 7c00 6402 1900 6402 1900 1800  d...|.d...d.....
+00000670: 7401 7c00 6402 1900 6403 1900 7c00 6402  t.|.d...d...|.d.
+00000680: 1900 6402 1900 1800 7c01 6403 1900 7c01  ..d.....|.d...|.
+00000690: 6402 1900 1800 8302 7c02 1400 6b04 7d03  d.......|...k.}.
+000006a0: 6eee 7c04 7402 7c00 8301 6b02 72ba 7c00  n.|.t.|...k.r.|.
+000006b0: 7c04 6403 1800 1900 6403 1900 7c01 6402  |.d.....d...|.d.
+000006c0: 1900 1800 7401 7c00 7c04 6403 1800 1900  ....t.|.|.d.....
+000006d0: 6403 1900 7c00 7c04 6403 1800 1900 6402  d...|.|.d.....d.
+000006e0: 1900 1800 7c01 6403 1900 7c01 6402 1900  ....|.d...|.d...
+000006f0: 1800 8302 7c02 1400 6b04 7d03 6e92 7c00  ....|...k.}.n.|.
+00000700: 7c04 6403 1800 1900 6403 1900 7c01 6402  |.d.....d...|.d.
+00000710: 1900 1800 7401 7c00 7c04 6403 1800 1900  ....t.|.|.d.....
+00000720: 6403 1900 7c00 7c04 6403 1800 1900 6402  d...|.|.d.....d.
+00000730: 1900 1800 7c01 6403 1900 7c01 6402 1900  ....|.d...|.d...
+00000740: 1800 8302 7c02 1400 6b04 9001 704a 7c01  ....|...k...pJ|.
+00000750: 6403 1900 7c00 7c04 1900 6402 1900 1800  d...|.|...d.....
+00000760: 7401 7c00 7c04 1900 6403 1900 7c00 7c04  t.|.|...d...|.|.
+00000770: 1900 6402 1900 1800 7c01 6403 1900 7c01  ..d.....|.d...|.
+00000780: 6402 1900 1800 8302 7c02 1400 6b04 7d03  d.......|...k.}.
+00000790: 7c03 9001 735e 7c00 a003 7c04 7c01 a102  |...s^|...|.|...
+000007a0: 0100 7c03 5300 2904 6166 0200 000a 2020  ..|.S.).af....  
+000007b0: 2020 5265 7475 726e 2069 6620 7468 6520    Return if the 
+000007c0: 6769 7665 6e20 7261 6e67 6520 6f76 6572  given range over
+000007d0: 6c61 7073 2077 6974 6820 7468 6520 6578  laps with the ex
+000007e0: 6973 7469 6e67 2072 616e 6765 732e 0a0a  isting ranges...
+000007f0: 2020 2020 4361 7574 696f 6e3a 0a20 2020      Caution:.   
+00000800: 2020 2060 7261 6e67 6573 6020 7769 6c6c     `ranges` will
+00000810: 2062 6520 6d6f 6469 6669 6564 2069 6e20   be modified in 
+00000820: 7468 6973 2066 756e 6374 696f 6e20 2877  this function (w
+00000830: 6865 6e20 7265 7475 726e 696e 6720 4661  hen returning Fa
+00000840: 6c73 6529 0a0a 2020 2020 4e6f 7465 3a20  lse)..    Note: 
+00000850: 6f76 6572 6c61 7070 696e 6720 6865 7265  overlapping here
+00000860: 206d 6561 6e73 2074 6865 206c 656e 6774   means the lengt
+00000870: 6820 6f66 206f 7665 726c 6170 7069 6e67  h of overlapping
+00000880: 2061 7265 6120 6973 2067 7265 6174 6572   area is greater
+00000890: 2074 6861 6e0a 2020 2020 736f 6d65 2074   than.    some t
+000008a0: 6872 6573 686f 6c64 2028 6375 7272 656e  hreshold (curren
+000008b0: 746c 792c 2074 6865 2074 6872 6573 686f  tly, the thresho
+000008c0: 6c64 2069 7320 606f 7665 726c 6170 5f72  ld is `overlap_r
+000008d0: 6174 696f 6020 6d75 6c74 6970 6c79 2074  atio` multiply t
+000008e0: 6865 206c 656e 6774 680a 2020 2020 6f66  he length.    of
+000008f0: 2074 6865 2073 686f 7274 6572 206f 7665   the shorter ove
+00000900: 726c 6170 7069 6e67 2072 616e 6765 7329  rlapping ranges)
+00000910: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00000920: 2020 2072 616e 6765 733a 0a20 2020 2020     ranges:.     
+00000930: 2020 2054 6865 2065 7869 7374 696e 6720     The existing 
+00000940: 7261 6e67 6573 2c20 6974 2069 7320 736f  ranges, it is so
+00000950: 7274 6564 2069 6e20 6173 6365 6e64 696e  rted in ascendin
+00000960: 6720 6f72 6465 7220 6f6e 2069 6e70 7574  g order on input
+00000970: 2c20 616e 6420 7765 2077 696c 6c0a 2020  , and we will.  
+00000980: 2020 2020 2020 6b65 6570 2069 7420 736f        keep it so
+00000990: 7274 6564 2069 6e20 7468 6973 2066 756e  rted in this fun
+000009a0: 6374 696f 6e2e 0a20 2020 2020 2071 7565  ction..      que
+000009b0: 7279 3a0a 2020 2020 2020 2020 5468 6520  ry:.        The 
+000009c0: 6769 7665 6e20 7261 6e67 652e 0a0a 2020  given range...  
+000009d0: 2020 5265 7475 726e 3a0a 2020 2020 2020    Return:.      
+000009e0: 5265 7475 726e 2054 7275 6520 6966 2068  Return True if h
+000009f0: 6176 696e 6720 6f76 6572 6c61 7020 6f74  aving overlap ot
+00000a00: 6865 7277 6973 6520 4661 6c73 652e 0a20  herwise False.. 
+00000a10: 2020 2046 7201 0000 0072 1900 0000 2904     Fr....r....).
+00000a20: 7202 0000 00da 036d 696e da03 6c65 6eda  r......min..len.
+00000a30: 0669 6e73 6572 7429 0572 2500 0000 7226  .insert).r%...r&
+00000a40: 0000 0072 2700 0000 da0a 6973 5f6f 7665  ...r'.....is_ove
+00000a50: 726c 6170 da05 696e 6465 7872 0e00 0000  rlap..indexr....
+00000a60: 720e 0000 0072 0f00 0000 722b 0000 002b  r....r....r+...+
+00000a70: 0000 0073 3c00 0000 0017 0401 0a01 0801  ...s<...........
+00000a80: 0402 1201 2cff 02ff 0404 0c02 1601 3001  ....,.........0.
+00000a90: 02ff 02ff 02ff 0407 1601 3001 02ff 02ff  ..........0.....
+00000aa0: 02ff 0405 1201 2801 02ff 02ff 02fb 020a  ......(.........
+00000ab0: 0601 0c01 722b 0000 0046 2903 da01 63da  ....r+...F)...c.
+00000ac0: 0865 6f73 5f6f 6e6c 7972 1800 0000 6302  .eos_onlyr....c.
+00000ad0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00000ae0: 0000 0043 0000 0073 1400 0000 7c01 720c  ...C...s....|.r.
+00000af0: 7c00 6401 6b06 5300 7c00 6402 6b06 5300  |.d.k.S.|.d.k.S.
+00000b00: 2903 7adb 0a20 2020 2052 6574 7572 6e20  ).z..    Return 
+00000b10: 5472 7565 2069 6620 7468 6520 6769 7665  True if the give
+00000b20: 6e20 6368 6172 6163 7465 7220 6973 2061  n character is a
+00000b30: 2070 756e 6374 7561 7469 6f6e 2e0a 0a20   punctuation... 
+00000b40: 2020 2041 7267 733a 0a20 2020 2020 2063     Args:.      c
+00000b50: 3a0a 2020 2020 2020 2020 5468 6520 6769  :.        The gi
+00000b60: 7665 6e20 6368 6172 6163 7465 722e 0a20  ven character.. 
+00000b70: 2020 2020 2065 6f73 5f6f 6e6c 793a 0a20       eos_only:. 
+00000b80: 2020 2020 2020 2049 6620 5472 7565 2074         If True t
+00000b90: 6865 2070 756e 6374 7561 7469 6f6e 7320  he punctuations 
+00000ba0: 6172 6520 6f6e 6c79 2074 686f 7365 2069  are only those i
+00000bb0: 6e64 6963 6174 696e 6720 656e 6420 6f66  ndicating end of
+00000bc0: 2061 2073 656e 7465 6e63 6520 282e 3f21   a sentence (.?!
+00000bd0: 2066 6f72 206e 6f77 292e 0a20 2020 207a   for now)..    z
+00000be0: 032e 3f21 7a0e 2c2e 3b3f 2128 293a 2d3c  ..?!z.,.;?!():-<
+00000bf0: 3e2d 2f22 720e 0000 0029 0272 2d00 0000  >-/"r....).r-...
+00000c00: 722e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000c10: 0f00 0000 da0e 6973 5f70 756e 6374 7561  ......is_punctua
+00000c20: 7469 6f6e 6000 0000 7306 0000 0000 0a04  tion`...s.......
+00000c30: 0108 0172 2f00 0000 2901 7224 0000 0029  ...r/...).r$...)
+00000c40: 0146 2913 da06 6269 7365 6374 7202 0000  .F)...bisectr...
+00000c50: 00da 0674 7970 696e 6772 0300 0000 7204  ...typingr....r.
+00000c60: 0000 00da 056e 756d 7079 721e 0000 00da  .....numpyr.....
+00000c70: 0f5f 6661 7374 7465 7874 7365 6172 6368  ._fasttextsearch
+00000c80: 7205 0000 0072 2200 0000 da04 6469 6374  r....r".....dict
+00000c90: 7206 0000 00da 076e 6461 7272 6179 da03  r......ndarray..
+00000ca0: 696e 74da 0566 6c6f 6174 da04 626f 6f6c  int..float..bool
+00000cb0: 722b 0000 00da 0373 7472 722f 0000 0072  r+.....strr/...r
+00000cc0: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
+00000cd0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000ce0: 0073 1a00 0000 0c01 1001 0801 0c03 1010  .s..............
+00000cf0: 1415 00ff 0201 0e00 0a00 0201 02fe 0c35  ...............5
```

### Comparing `fasttextsearch-0.4/textsearch/python/textsearch/datatypes.py` & `fasttextsearch-0.5/textsearch/python/textsearch/datatypes.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/textsearch/levenshtein.py` & `fasttextsearch-0.5/textsearch/python/textsearch/levenshtein.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/textsearch/match.py` & `fasttextsearch-0.5/textsearch/python/textsearch/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+import math
 from bisect import bisect_left
 from dataclasses import dataclass
 from heapq import heappush, heappop
 from multiprocessing.pool import ThreadPool
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
@@ -135,20 +136,25 @@
 
     def add_segments(
         query_start, query_end, target_start, target_end, segment_length, segments
     ):
         num_chunk = (query_end - query_start) // segment_length
         if num_chunk > 0:
             for i in range(num_chunk):
+                real_target_end = (
+                    target_start + segment_length
+                    if target_start + segment_length < target_end
+                    else target_end
+                )
                 segments.append(
                     (
                         query_start,
                         query_start + segment_length,
                         target_start,
-                        target_start + segment_length,
+                        real_target_end,
                     )
                 )
                 query_start += segment_length
                 target_start += segment_length
         # if the remaining part is smaller than segment_length // 4, we will append
         # it to the last segment rather than creating a new segment.
         if segments and query_end - query_start < segment_length // 4:
@@ -275,14 +281,21 @@
             logging.warning(f"Skipping empty sub segment.")
             continue
         # for the global mode of levenshtein, there is only one alignment
         # See docs in `levenshtein_distance` for the meaning of target_align_start,
         # target_align_end and align_str
         target_align_start, target_align_end, align_str = sub["alignment"][1][0]
         query_start, query_end, target_start, target_end = sub["segment"]
+        # we are doing levenshtein_distance in "global" mode
+        assert target_align_start == 0, target_align_start
+        assert target_end == (target_start + target_align_end + 1), (
+            target_end,
+            target_start + target_align_end + 1,
+        )
+
         query_id = sourced_text.doc[query_start]
 
         if alignments[query_id] is None:
             alignments[query_id] = (
                 (query_start, target_start + target_align_start),
                 [],
             )
@@ -295,44 +308,50 @@
         aligns = alignments[query_id][1]
         # Note: query_source could be TextSource or Transcript, only Transcript
         # has times.
         times = query_source.times if isinstance(query_source, Transcript) else None
         # The times is in byte level.
         time_stride = 1 if query_source.binary_text.dtype == np.uint8 else 4
 
+        query_length = query_end - query_start
         query_local_index = query_start - query_base
         query_index = query_start
         target_index = target_start + target_align_start
 
         hyp_time = 0 if times is None else float(times[query_local_index * time_stride])
         for ali in align_str:
-            if ali != "D":
-                hyp_time = (
-                    0
-                    if times is None
-                    else float(times[query_local_index * time_stride])
-                )
+            query_local_index = (
+                query_local_index
+                if query_local_index < query_length
+                else query_length - 1
+            )
+            hyp_time = (
+                0 if times is None else float(times[query_local_index * time_stride])
+            )
+            target_index = target_index if target_index < target_end else target_end - 1
+            ref_pos = int(sourced_text.pos[target_index])
+            query_index = query_index if query_index < query_end else query_end - 1
             if ali == "I":
                 aligns.append(
                     {
                         "ref": "",
                         "hyp": chr(sourced_text.binary_text[query_index]),
-                        "ref_pos": int(sourced_text.pos[target_index]),
+                        "ref_pos": ref_pos,
                         "hyp_pos": query_local_index,
                         "hyp_time": hyp_time,
                     }
                 )
                 query_local_index += 1
                 query_index += 1
             elif ali == "D":
                 aligns.append(
                     {
                         "ref": chr(sourced_text.binary_text[target_index]),
                         "hyp": "",
-                        "ref_pos": int(sourced_text.pos[target_index]),
+                        "ref_pos": ref_pos,
                         "hyp_pos": query_local_index,
                         "hyp_time": hyp_time,
                     }
                 )
                 target_index += 1
             else:
                 assert ali == "C" or ali == "S"
@@ -344,15 +363,15 @@
                     assert ref == hyp
                 else:
                     assert ref != hyp
                 aligns.append(
                     {
                         "ref": ref,
                         "hyp": hyp,
-                        "ref_pos": int(sourced_text.pos[target_index]),
+                        "ref_pos": ref_pos,
                         "hyp_pos": query_local_index,
                         "hyp_time": hyp_time,
                     }
                 )
                 query_local_index += 1
                 query_index += 1
                 target_index += 1
@@ -416,14 +435,17 @@
         seq1 = np.arange(query_start, query_end).reshape(-1, 1)
         seq1 = np.tile(seq1, num_close_matches).flatten()
 
         seq2 = close_matches[query_start:query_end, :].flatten()
         # matched_points is a list of (query index, target index), global index in sourced_text
         matched_points = get_longest_increasing_pairs(seq1, seq2)
 
+        if len(matched_points) == 0:
+            continue
+
         # In the algorithm of `find_close_matches`, `sourced_text.binary_text.size - 1`
         # means no close_matches
         trim_pos = len(matched_points) - 1
         while matched_points[trim_pos][1] == sourced_text.binary_text.size - 1:
             trim_pos -= 1
         matched_points = matched_points[0:trim_pos]
 
@@ -476,14 +498,15 @@
         target = sourced_text.binary_text[segment[2] : segment[3]]
         # Using global matching mode here, thanks to `get_longest_increasing_pairs`
         # we have very good matching points.
         alignment = levenshtein_distance(query=query, target=target, mode="global")
         return {
             "segment": segment,
             "alignment": alignment,
+            "target": target,
         }
 
     pool = ThreadPool() if thread_pool is None else thread_pool
     logging.info("Matching with levenshtein.")
     async_results = pool.starmap_async(levenshtein_worker, arguments)
     results = async_results.get()
     logging.info("Matching with levenshtein done.")
@@ -856,20 +879,26 @@
     preceding_context_length = 1000
 
     for seg in segments:
         begin_pos = aligns[seg[0]]["ref_pos"]
         end_pos = aligns[seg[1]]["ref_pos"] + 1
 
         preceding_index = seg[0] if seg[0] == 0 else seg[0] - 1
-        start = (aligns[preceding_index]["hyp_time"] + aligns[seg[0]]["hyp_time"]) / 2
+
+        # start = (aligns[preceding_index]["hyp_time"] + aligns[seg[0]]["hyp_time"]) / 2
+
+        start = aligns[seg[0]]["hyp_time"]
+
         following_index = seg[1] if seg[1] == len(aligns) - 1 else seg[1] + 1
         duration = (
             aligns[following_index]["hyp_time"] + aligns[seg[1]]["hyp_time"]
         ) / 2 - start
 
+        # duration = aligns[seg[1]]["hyp_time"] - start
+
         hyp_begin_pos = aligns[seg[0]]["hyp_pos"]
         hyp_end_pos = aligns[seg[1]]["hyp_pos"] + 1
         hyp = "".join(
             [chr(i) for i in query_source.binary_text[hyp_begin_pos:hyp_end_pos]]
         )
 
         # skipping segment that has too short text
@@ -902,15 +931,15 @@
         )
 
         results.append(
             {
                 "begin_byte": begin_pos,
                 "end_byte": end_pos,
                 "start_time": start,
-                "duration": duration,
+                "duration": math.floor(1000 * duration) / 1000,
                 "hyp": hyp,
                 "ref": ref,
                 "pre_ref": pre_ref,
                 "pre_hyp": pre_hyp,
             }
         )
     return results
```

### Comparing `fasttextsearch-0.4/textsearch/python/textsearch/suffix_array.py` & `fasttextsearch-0.5/textsearch/python/textsearch/suffix_array.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.4/textsearch/python/textsearch/utils.py` & `fasttextsearch-0.5/textsearch/python/textsearch/utils.py`

 * *Files identical despite different names*

