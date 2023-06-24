# Comparing `tmp/yerbamate-0.9.239.tar.gz` & `tmp/yerbamate-0.9.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yerbamate-0.9.239.tar", last modified: Sat May 13 17:53:04 2023, max compression
+gzip compressed data, was "yerbamate-0.9.24.tar", last modified: Sat Jun 24 09:28:39 2023, max compression
```

## Comparing `yerbamate-0.9.239.tar` & `yerbamate-0.9.24.tar`

### file list

```diff
@@ -1,88 +1,112 @@
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.303707 yerbamate-0.9.239/
--rw-r--r--   0 al        (1000) al        (1001)     1079 2023-04-08 19:56:23.000000 yerbamate-0.9.239/LICENSE
--rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.239/MANIFEST.in
--rw-r--r--   0 al        (1000) al        (1001)    11582 2023-05-13 17:53:04.303707 yerbamate-0.9.239/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1001)    10948 2023-04-08 19:56:23.000000 yerbamate-0.9.239/README.md
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.297707 yerbamate-0.9.239/packages/
--rw-r--r--   0 al        (1000) al        (1001)      112 2023-04-22 15:20:01.000000 yerbamate-0.9.239/packages/requirements.txt
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.298707 yerbamate-0.9.239/packages/yerbamate/
--rw-r--r--   0 al        (1000) al        (1001)      130 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.299707 yerbamate-0.9.239/packages/yerbamate/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      291 2023-04-08 19:57:52.000000 yerbamate-0.9.239/packages/yerbamate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5598 2023-05-13 17:52:22.000000 yerbamate-0.9.239/packages/yerbamate/__pycache__/environment.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     8269 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/__pycache__/mate.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     9389 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.299707 yerbamate-0.9.239/packages/yerbamate/api/
--rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.299707 yerbamate-0.9.239/packages/yerbamate/api/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      153 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1427 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.299707 yerbamate-0.9.239/packages/yerbamate/api/data/
--rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.300707 yerbamate-0.9.239/packages/yerbamate/api/data/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      197 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5655 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)    11926 2023-05-03 21:24:59.000000 yerbamate-0.9.239/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     3316 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     9460 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/module_manager.py
--rw-r--r--   0 al        (1000) al        (1001)    15485 2023-05-03 21:24:50.000000 yerbamate-0.9.239/packages/yerbamate/api/data/module_repository.py
--rw-r--r--   0 al        (1000) al        (1001)     3447 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/package.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.300707 yerbamate-0.9.239/packages/yerbamate/api/data/sources/
--rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.300707 yerbamate-0.9.239/packages/yerbamate/api/data/sources/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      166 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1127 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.300707 yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/
--rw-r--r--   0 al        (1000) al        (1001)       35 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.301707 yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      217 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5521 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5734 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5573 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/io.py
--rw-r--r--   0 al        (1000) al        (1001)     5130 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/local.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.301707 yerbamate-0.9.239/packages/yerbamate/api/data/sources/remote/
--rw-r--r--   0 al        (1000) al        (1001)       37 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/remote/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.301707 yerbamate-0.9.239/packages/yerbamate/api/data/sources/remote/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      220 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/remote/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     2132 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1078 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/remote/remote.py
--rw-r--r--   0 al        (1000) al        (1001)      365 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/sources/source.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.301707 yerbamate-0.9.239/packages/yerbamate/api/data/utils/
--rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/utils/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.302707 yerbamate-0.9.239/packages/yerbamate/api/data/utils/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      164 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)      540 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1035 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     4487 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)      326 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/utils/exp_util.py
--rw-r--r--   0 al        (1000) al        (1001)     1197 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/utils/git_util.py
--rw-r--r--   0 al        (1000) al        (1001)     7395 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/data/utils/gitdir.py
--rw-r--r--   0 al        (1000) al        (1001)      869 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/api/mate_api.py
--rw-r--r--   0 al        (1000) al        (1001)      294 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/constants.py
--rw-r--r--   0 al        (1000) al        (1001)     7512 2023-05-13 17:50:47.000000 yerbamate-0.9.239/packages/yerbamate/environment.py
--rw-r--r--   0 al        (1000) al        (1001)     7829 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/mate.py
--rw-r--r--   0 al        (1000) al        (1001)    10611 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/mate_cli.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.302707 yerbamate-0.9.239/packages/yerbamate/utils/
--rw-r--r--   0 al        (1000) al        (1001)     1433 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/utils/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.302707 yerbamate-0.9.239/packages/yerbamate/utils/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)     2016 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)      814 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     3761 2023-04-09 10:03:11.000000 yerbamate-0.9.239/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     2145 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/utils/bunch.py
--rw-r--r--   0 al        (1000) al        (1001)     1386 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/utils/git_url_parser.py
--rw-r--r--   0 al        (1000) al        (1001)     4419 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/utils/utils.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.303707 yerbamate-0.9.239/packages/yerbamate/yerbamate.egg-info/
--rw-r--r--   0 al        (1000) al        (1001)      601 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/yerbamate.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1001)      342 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/yerbamate.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) al        (1001)        1 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/yerbamate.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) al        (1001)       10 2023-04-08 19:56:23.000000 yerbamate-0.9.239/packages/yerbamate/yerbamate.egg-info/top_level.txt
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.298707 yerbamate-0.9.239/packages/yerbamate.egg-info/
--rw-r--r--   0 al        (1000) al        (1001)    11582 2023-05-13 17:53:04.000000 yerbamate-0.9.239/packages/yerbamate.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1001)     3195 2023-05-13 17:53:04.000000 yerbamate-0.9.239/packages/yerbamate.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) al        (1001)        1 2023-05-13 17:53:04.000000 yerbamate-0.9.239/packages/yerbamate.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) al        (1001)       82 2023-05-13 17:53:04.000000 yerbamate-0.9.239/packages/yerbamate.egg-info/requires.txt
--rw-r--r--   0 al        (1000) al        (1001)       10 2023-05-13 17:53:04.000000 yerbamate-0.9.239/packages/yerbamate.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) al        (1001)      107 2023-05-13 17:53:04.303707 yerbamate-0.9.239/setup.cfg
--rw-r--r--   0 al        (1000) al        (1001)     1279 2023-05-13 17:50:59.000000 yerbamate-0.9.239/setup.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-13 17:53:04.297707 yerbamate-0.9.239/src/
--rwxr-xr-x   0 al        (1000) al        (1001)       62 2023-04-08 19:56:23.000000 yerbamate-0.9.239/src/mate
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.228664 yerbamate-0.9.24/
+-rw-r--r--   0 al        (1000) al        (1001)     1079 2023-04-08 19:56:23.000000 yerbamate-0.9.24/LICENSE
+-rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.24/MANIFEST.in
+-rw-r--r--   0 al        (1000) al        (1001)    11581 2023-06-24 09:28:39.228664 yerbamate-0.9.24/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)    10948 2023-04-08 19:56:23.000000 yerbamate-0.9.24/README.md
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.220664 yerbamate-0.9.24/packages/
+-rw-r--r--   0 al        (1000) al        (1001)      112 2023-04-22 15:20:01.000000 yerbamate-0.9.24/packages/requirements.txt
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.221665 yerbamate-0.9.24/packages/yerbamate/
+-rw-r--r--   0 al        (1000) al        (1001)      130 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.222664 yerbamate-0.9.24/packages/yerbamate/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      291 2023-04-08 19:57:52.000000 yerbamate-0.9.24/packages/yerbamate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      365 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5929 2023-06-24 08:46:46.000000 yerbamate-0.9.24/packages/yerbamate/__pycache__/environment.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)    11851 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/__pycache__/environment.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     8595 2023-06-22 06:53:24.000000 yerbamate-0.9.24/packages/yerbamate/__pycache__/mate.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)    11024 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/__pycache__/mate.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     9400 2023-06-18 07:38:25.000000 yerbamate-0.9.24/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)    17457 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/__pycache__/mate_cli.cpython-311.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.222664 yerbamate-0.9.24/packages/yerbamate/api/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.222664 yerbamate-0.9.24/packages/yerbamate/api/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      153 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      169 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1427 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     2065 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/__pycache__/mate_api.cpython-311.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.223664 yerbamate-0.9.24/packages/yerbamate/api/data/
+-rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.224664 yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      197 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      227 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5655 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)    11637 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/module_manager.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)    12224 2023-06-24 08:17:21.000000 yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)    26197 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/module_repository.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     3316 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     4821 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/package.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     9460 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/module_manager.py
+-rw-r--r--   0 al        (1000) al        (1001)    16076 2023-06-24 08:17:19.000000 yerbamate-0.9.24/packages/yerbamate/api/data/module_repository.py
+-rw-r--r--   0 al        (1000) al        (1001)     3447 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/package.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.224664 yerbamate-0.9.24/packages/yerbamate/api/data/sources/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.224664 yerbamate-0.9.24/packages/yerbamate/api/data/sources/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      166 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      182 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1127 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1391 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/__pycache__/source.cpython-311.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.224664 yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/
+-rw-r--r--   0 al        (1000) al        (1001)       35 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.225664 yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      217 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      247 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5521 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     9425 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5734 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     9568 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5573 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/io.py
+-rw-r--r--   0 al        (1000) al        (1001)     5130 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/local.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.225664 yerbamate-0.9.24/packages/yerbamate/api/data/sources/remote/
+-rw-r--r--   0 al        (1000) al        (1001)       37 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/remote/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.225664 yerbamate-0.9.24/packages/yerbamate/api/data/sources/remote/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      220 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/remote/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      250 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/remote/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     2132 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     3069 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1078 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/remote/remote.py
+-rw-r--r--   0 al        (1000) al        (1001)      365 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/sources/source.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.226664 yerbamate-0.9.24/packages/yerbamate/api/data/utils/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.226664 yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      164 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      180 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      540 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1008 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1035 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     2021 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     4487 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     8470 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      326 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/exp_util.py
+-rw-r--r--   0 al        (1000) al        (1001)     1197 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/git_util.py
+-rw-r--r--   0 al        (1000) al        (1001)     7395 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/data/utils/gitdir.py
+-rw-r--r--   0 al        (1000) al        (1001)      869 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/api/mate_api.py
+-rw-r--r--   0 al        (1000) al        (1001)      294 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/constants.py
+-rw-r--r--   0 al        (1000) al        (1001)     8513 2023-06-24 08:40:14.000000 yerbamate-0.9.24/packages/yerbamate/environment.py
+-rw-r--r--   0 al        (1000) al        (1001)     8287 2023-06-18 07:40:45.000000 yerbamate-0.9.24/packages/yerbamate/mate.py
+-rw-r--r--   0 al        (1000) al        (1001)    10655 2023-06-18 07:37:58.000000 yerbamate-0.9.24/packages/yerbamate/mate_cli.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.227664 yerbamate-0.9.24/packages/yerbamate/utils/
+-rw-r--r--   0 al        (1000) al        (1001)     1433 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/utils/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.227664 yerbamate-0.9.24/packages/yerbamate/utils/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)     2016 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     3616 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      814 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1244 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/utils/__pycache__/bunch.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     3761 2023-04-09 10:03:11.000000 yerbamate-0.9.24/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     6920 2023-05-15 08:31:30.000000 yerbamate-0.9.24/packages/yerbamate/utils/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     2145 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/utils/bunch.py
+-rw-r--r--   0 al        (1000) al        (1001)     1386 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/utils/git_url_parser.py
+-rw-r--r--   0 al        (1000) al        (1001)     4419 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/utils/utils.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.228664 yerbamate-0.9.24/packages/yerbamate/yerbamate.egg-info/
+-rw-r--r--   0 al        (1000) al        (1001)      601 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/yerbamate.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)      342 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/yerbamate.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) al        (1001)        1 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/yerbamate.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) al        (1001)       10 2023-04-08 19:56:23.000000 yerbamate-0.9.24/packages/yerbamate/yerbamate.egg-info/top_level.txt
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.221665 yerbamate-0.9.24/packages/yerbamate.egg-info/
+-rw-r--r--   0 al        (1000) al        (1001)    11581 2023-06-24 09:28:39.000000 yerbamate-0.9.24/packages/yerbamate.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)     4804 2023-06-24 09:28:39.000000 yerbamate-0.9.24/packages/yerbamate.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) al        (1001)        1 2023-06-24 09:28:39.000000 yerbamate-0.9.24/packages/yerbamate.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) al        (1001)       82 2023-06-24 09:28:39.000000 yerbamate-0.9.24/packages/yerbamate.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) al        (1001)       10 2023-06-24 09:28:39.000000 yerbamate-0.9.24/packages/yerbamate.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) al        (1001)      107 2023-06-24 09:28:39.228664 yerbamate-0.9.24/setup.cfg
+-rw-r--r--   0 al        (1000) al        (1001)     1278 2023-06-24 09:25:56.000000 yerbamate-0.9.24/setup.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-06-24 09:28:39.220664 yerbamate-0.9.24/src/
+-rwxr-xr-x   0 al        (1000) al        (1001)       62 2023-04-08 19:56:23.000000 yerbamate-0.9.24/src/mate
```

### Comparing `yerbamate-0.9.239/LICENSE` & `yerbamate-0.9.24/LICENSE`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/PKG-INFO` & `yerbamate-0.9.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yerbamate
-Version: 0.9.239
+Version: 0.9.24
 Summary:  A python module and experiment manager for deep learning
 Home-page: https://github.com/oalee/yerbamate
 Author: Giulio Zani, Ali Rahimi
 Author-email: yerba.mate.dl@proton.me
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `yerbamate-0.9.239/README.md` & `yerbamate-0.9.24/README.md`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/__pycache__/environment.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/__pycache__/environment.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 13 17:50:47 2023 UTC, .py size: 7512 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f7cd 5f64 581d 0000  o........._dX...
+00000000: 6f0d 0d0a 0000 0000 eeab 9664 4121 0000  o..........dA!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 5a05 4700 6403 6404  d.l.Z.d.Z.G.d.d.
 00000060: 8400 6404 6506 8303 5a07 6401 5300 2905  ..d.e...Z.d.S.).
 00000070: e900 0000 004e da03 656e 7663 0000 0000  .....N..envc....
@@ -13,338 +13,359 @@
 000000c0: 0664 0964 0a84 005a 0787 0066 0164 0b64  .d.d...Z...f.d.d
 000000d0: 0c84 085a 0864 1587 0066 0164 0e64 0c84  ...Z.d...f.d.d..
 000000e0: 095a 0864 1564 0f64 1084 015a 0964 1564  .Z.d.d.d...Z.d.d
 000000f0: 1164 1284 015a 0a64 1364 1484 005a 0b87  .d...Z.d.d...Z..
 00000100: 0004 005a 0c53 0029 16da 0b45 6e76 6972  ...Z.S.)...Envir
 00000110: 6f6e 6d65 6e74 6301 0000 0000 0000 0000  onmentc.........
 00000120: 0000 0004 0000 0007 0000 0043 0000 0073  ...........C...s
-00000130: 5401 0000 6401 7c00 5f00 6401 7c00 5f01  T...d.|._.d.|._.
+00000130: 9601 0000 6401 7c00 5f00 6401 7c00 5f01  ....d.|._.d.|._.
 00000140: 6401 7c00 5f02 6401 7c00 5f03 6900 7c00  d.|._.d.|._.i.|.
-00000150: 5f04 7a0b 7405 7c00 7406 6a07 6402 1900  _.z.t.|.t.j.d...
-00000160: 6403 8303 0100 5700 6e04 0100 0100 0100  d.....W.n.......
-00000170: 5900 7406 6a07 6402 6400 8502 1900 7c00  Y.t.j.d.d.....|.
-00000180: 5f08 7c00 a009 a100 7c00 5f0a 7406 6a07  _.|.....|._.t.j.
-00000190: 4400 5d29 7d01 6404 7c01 7601 7236 712f  D.])}.d.|.v.r6q/
-000001a0: 7c01 a00b 6404 a101 5c02 7d02 7d03 7c00  |...d...\.}.}.|.
-000001b0: a00c 7c03 a101 7d03 7c02 a00d 6405 a101  ..|...}.|...d...
-000001c0: 724d 7c02 6406 6400 8502 1900 7d02 7405  rM|.d.d.....}.t.
-000001d0: 7c00 7c02 7c03 8303 0100 7c03 7c00 6a04  |.|.|.....|.|.j.
-000001e0: 7c02 3c00 712f 7406 6a07 6407 1900 7c00  |.<.q/t.j.d...|.
-000001f0: 5f0e 6408 7c00 6a0e 7600 7284 740f 6a10  _.d.|.j.v.r.t.j.
-00000200: 6a11 7406 6a07 6406 6409 8502 1900 8e00  j.t.j.d.d.......
-00000210: 7c00 5f12 740f 6a10 a011 7c00 6a0a 640a  |._.t.j...|.j.d.
-00000220: 7406 6a07 6406 1900 7406 6a07 640b 1900  t.j.d...t.j.d...
-00000230: 640c 1700 a104 7c00 5f0e 6e17 7c00 6a0e  d.....|._.n.|.j.
-00000240: a00b 640d a101 640e 6400 8502 1900 7c00  ..d...d.d.....|.
-00000250: 5f12 740f 6a10 6a11 7c00 6a12 8e00 6400  _.t.j.j.|.j...d.
-00000260: 640f 8502 1900 7c00 5f12 7c00 a013 a100  d.....|._.|.....
-00000270: 0100 7c00 6a02 72a8 7c00 a014 a100 0100  ..|.j.r.|.......
-00000280: 6400 5300 6400 5300 2910 4e46 e901 0000  d.S.d.S.).NF....
-00000290: 0054 fa01 3d7a 022d 2de9 0200 0000 7201  .T..=z.--.....r.
-000002a0: 0000 007a 0862 696e 2f6d 6174 65e9 0400  ...z.bin/mate...
-000002b0: 0000 5a0b 6578 7065 7269 6d65 6e74 73e9  ..Z.experiments.
-000002c0: 0300 0000 7a03 2e70 79fa 012f e9fe ffff  ....z..py../....
-000002d0: ffe9 fdff ffff 2915 5a07 7265 7374 6172  ......).Z.restar
-000002e0: 74da 0474 6573 745a 0574 7261 696e da06  t..testZ.train..
-000002f0: 7361 6d70 6c65 da07 6870 6172 616d 73da  sample..hparams.
-00000300: 0773 6574 6174 7472 da03 7379 73da 0461  .setattr..sys..a
-00000310: 7267 76da 0461 7267 73da 175f 456e 7669  rgv..args.._Envi
-00000320: 726f 6e6d 656e 745f 5f66 696e 645f 726f  ronment__find_ro
-00000330: 6f74 da05 5f72 6f6f 74da 0573 706c 6974  ot.._root..split
-00000340: da13 636f 6e76 6572 745f 7374 725f 746f  ..convert_str_to
-00000350: 5f64 6174 61da 0a73 7461 7274 7377 6974  _data..startswit
-00000360: 68da 055f 7061 7468 da02 6f73 da04 7061  h.._path..os..pa
-00000370: 7468 da04 6a6f 696e da04 6e61 6d65 da15  th..join..name..
-00000380: 5f45 6e76 6972 6f6e 6d65 6e74 5f5f 7365  _Environment__se
-00000390: 745f 656e 76da 215f 456e 7669 726f 6e6d  t_env.!_Environm
-000003a0: 656e 745f 5f67 656e 6572 6174 655f 6578  ent__generate_ex
-000003b0: 7065 7269 6d65 6e74 2904 da04 7365 6c66  periment)...self
-000003c0: da03 6172 67da 036b 6579 da05 7661 6c75  ..arg..key..valu
-000003d0: 65a9 0072 2300 0000 fa3b 2f68 6f6d 652f  e..r#....;/home/
-000003e0: 616c 2f47 6974 4875 622f 7965 7262 616d  al/GitHub/yerbam
-000003f0: 6174 652f 7061 636b 6167 6573 2f79 6572  ate/packages/yer
-00000400: 6261 6d61 7465 2f65 6e76 6972 6f6e 6d65  bamate/environme
-00000410: 6e74 2e70 79da 085f 5f69 6e69 745f 5f0e  nt.py..__init__.
-00000420: 0000 0073 4000 0000 0603 0601 0601 0601  ...s@...........
-00000430: 0601 0203 1601 0601 0201 1002 0a02 0a03  ................
-00000440: 0801 0201 0e01 0a01 0a02 0c01 0c02 0c01  ................
-00000450: 0c02 0a01 1801 0601 1a01 08ff 1604 1801  ................
-00000460: 0802 0602 0c01 04ff 7a14 456e 7669 726f  ........z.Enviro
-00000470: 6e6d 656e 742e 5f5f 696e 6974 5f5f 6302  nment.__init__c.
-00000480: 0000 0000 0000 0000 0000 0002 0000 000b  ................
-00000490: 0000 0043 0000 0073 6000 0000 7a05 7400  ...C...s`...z.t.
-000004a0: 7c01 8301 5700 5300 0400 7401 792f 0100  |...W.S...t.y/..
-000004b0: 0100 0100 7a07 7402 7c01 8301 5700 0600  ....z.t.|...W...
-000004c0: 5900 5300 0400 7401 792e 0100 0100 0100  Y.S...t.y.......
-000004d0: 7c01 6401 7600 7222 5900 5900 6402 5300  |.d.v.r"Y.Y.d.S.
-000004e0: 7c01 6403 7600 722a 5900 5900 6404 5300  |.d.v.r*Y.Y.d.S.
-000004f0: 5900 5900 7c01 5300 7700 7700 2905 4e29  Y.Y.|.S.w.w.).N)
-00000500: 02da 0454 7275 65da 0474 7275 6554 2902  ...True..trueT).
-00000510: da05 4661 6c73 65da 0566 616c 7365 4629  ..False..falseF)
-00000520: 03da 0369 6e74 da0a 5661 6c75 6545 7272  ...int..ValueErr
-00000530: 6f72 da05 666c 6f61 7429 0272 1f00 0000  or..float).r....
-00000540: da05 696e 7075 7472 2300 0000 7223 0000  ..inputr#...r#..
-00000550: 0072 2400 0000 7216 0000 003d 0000 0073  .r$...r....=...s
-00000560: 1c00 0000 0201 0a01 0c01 0201 0e01 0c01  ................
-00000570: 0801 0801 0801 0801 04ff 0403 02fa 02fd  ................
-00000580: 7a1f 456e 7669 726f 6e6d 656e 742e 636f  z.Environment.co
-00000590: 6e76 6572 745f 7374 725f 746f 5f64 6174  nvert_str_to_dat
-000005a0: 6163 0100 0000 0000 0000 0000 0000 0300  ac..............
-000005b0: 0000 0700 0000 4300 0000 734e 0000 0074  ......C...sN...t
-000005c0: 00a0 01a1 007d 0174 006a 02a0 0374 006a  .....}.t.j...t.j
-000005d0: 02a0 047c 0164 01a1 02a1 0172 2574 05a0  ...|.d.....r%t..
-000005e0: 0674 0774 006a 02a0 047c 0164 01a1 0264  .t.t.j...|.d...d
-000005f0: 0283 02a1 017d 0274 006a 02a0 047c 017c  .....}.t.j...|.|
-00000600: 0264 0319 00a1 0253 0064 0053 0029 044e  .d.....S.d.S.).N
-00000610: fa09 6d61 7465 2e6a 736f 6eda 0172 da07  ..mate.json..r..
-00000620: 7072 6f6a 6563 7429 0872 1900 0000 da06  project).r......
-00000630: 6765 7463 7764 721a 0000 00da 0665 7869  getcwdr......exi
-00000640: 7374 7372 1b00 0000 da04 6a73 6f6e da04  stsr......json..
-00000650: 6c6f 6164 da04 6f70 656e 2903 721f 0000  load..open).r...
-00000660: 0072 1a00 0000 da04 636f 6e66 7223 0000  .r......confr#..
-00000670: 0072 2300 0000 7224 0000 005a 0b5f 5f66  .r#...r$...Z.__f
-00000680: 696e 645f 726f 6f74 4b00 0000 730a 0000  ind_rootK...s...
-00000690: 0008 0316 021a 0112 0204 027a 1745 6e76  ...........z.Env
-000006a0: 6972 6f6e 6d65 6e74 2e5f 5f66 696e 645f  ironment.__find_
-000006b0: 726f 6f74 6301 0000 0000 0000 0000 0000  rootc...........
-000006c0: 0007 0000 0008 0000 0043 0000 0073 d200  .........C...s..
-000006d0: 0000 6700 6401 a201 7d01 6400 7d02 7c01  ..g.d...}.d.}.|.
-000006e0: 4400 5d0e 7d03 7c03 7c00 6a00 7600 7216  D.].}.|.|.j.v.r.
-000006f0: 7c00 6a00 7c03 1900 7d02 0100 6e01 7108  |.j.|...}...n.q.
-00000700: 7c02 6400 7500 721d 6400 5300 7401 6a02  |.d.u.r.d.S.t.j.
-00000710: a003 7c02 a101 732a 7401 6a04 7c02 6402  ..|...s*t.j.|.d.
-00000720: 6403 8d02 0100 7401 6a02 a005 7c02 6404  d.....t.j...|.d.
-00000730: a102 7d04 7406 a007 7c00 6a08 7c04 a102  ..}.t...|.j.|...
-00000740: 0100 7c00 6a09 6900 6b03 7267 7401 6a02  ..|.j.i.k.rgt.j.
-00000750: a005 7c02 6405 a102 7d05 740a 7c05 6406  ..|.d...}.t.|.d.
-00000760: 8302 8f14 7d06 740b 6a0c 740d 7c00 6a09  ....}.t.j.t.|.j.
-00000770: 8301 7c06 6407 6408 8d03 0100 5700 6400  ..|.d.d.....W.d.
-00000780: 0400 0400 8303 0100 6400 5300 3100 7360  ........d.S.1.s`
-00000790: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
-000007a0: 6400 5300 2909 4e29 06da 0772 6573 756c  d.S.).N)...resul
-000007b0: 7473 5a0c 7265 7375 6c74 735f 7061 7468  tsZ.results_path
-000007c0: 5a0b 7265 7375 6c74 735f 6469 725a 0473  Z.results_dirZ.s
-000007d0: 6176 655a 0973 6176 655f 7061 7468 5a08  aveZ.save_pathZ.
-000007e0: 7361 7665 5f64 6972 5429 01da 0865 7869  save_dirT)...exi
-000007f0: 7374 5f6f 6b7a 0d65 7870 6572 696d 656e  st_okz.experimen
-00000800: 742e 7079 7a0f 6578 7065 7269 6d65 6e74  t.pyz.experiment
-00000810: 2e6a 736f 6eda 0177 7207 0000 00a9 01da  .json..wr.......
-00000820: 0669 6e64 656e 7429 0e72 0200 0000 7219  .indent).r....r.
-00000830: 0000 0072 1a00 0000 7232 0000 00da 086d  ...r....r2.....m
-00000840: 616b 6564 6972 7372 1b00 0000 da06 7368  akedirsr......sh
-00000850: 7574 696c da08 636f 7079 6669 6c65 7218  util..copyfiler.
-00000860: 0000 0072 0e00 0000 7235 0000 0072 3300  ...r....r5...r3.
-00000870: 0000 da04 6475 6d70 da04 6469 6374 2907  ....dump..dict).
-00000880: 721f 0000 0072 3700 0000 da06 7265 7375  r....r7.....resu
-00000890: 6c74 7221 0000 005a 0973 6176 655f 6669  ltr!...Z.save_fi
-000008a0: 6c65 5a0b 7061 7261 6d73 5f66 696c 65da  leZ.params_file.
-000008b0: 0166 7223 0000 0072 2300 0000 7224 0000  .fr#...r#...r$..
-000008c0: 005a 155f 5f67 656e 6572 6174 655f 6578  .Z.__generate_ex
-000008d0: 7065 7269 6d65 6e74 5700 0000 7326 0000  perimentW...s&..
-000008e0: 0008 0204 0208 010a 010a 0104 0102 fe08  ................
-000008f0: 0304 010c 010e 010e 020e 020a 040e 010c  ................
-00000900: 0318 0122 ff04 fc7a 2145 6e76 6972 6f6e  ..."...z!Environ
-00000910: 6d65 6e74 2e5f 5f67 656e 6572 6174 655f  ment.__generate_
-00000920: 6578 7065 7269 6d65 6e74 6301 0000 0000  experimentc.....
-00000930: 0000 0000 0000 000d 0000 0009 0000 0043  ...............C
-00000940: 0000 0073 6002 0000 7400 6a01 a002 6401  ...s`...t.j...d.
-00000950: a101 7d01 7403 a004 7405 7c01 6402 8302  ..}.t...t.|.d...
-00000960: a101 7d02 7400 6a01 a002 6403 a101 7d03  ..}.t.j...d...}.
-00000970: 7400 6a01 a006 7c03 a101 7350 7407 6404  t.j...|...sPt.d.
-00000980: 8301 0100 7408 7c02 7600 7229 7c02 7408  ....t.|.v.r)|.t.
-00000990: 1900 a009 a100 7d04 6e03 6405 6701 7d04  ......}.n.d.g.}.
-000009a0: 6406 6407 8400 7c04 4400 8301 7d05 7405  d.d...|.D...}.t.
-000009b0: 7c03 6408 8302 8f10 7d06 7403 6a0a 7c05  |.d.....}.t.j.|.
-000009c0: 7c06 6409 640a 8d03 0100 5700 6400 0400  |.d.d.....W.d...
-000009d0: 0400 8303 0100 6e08 3100 734b 7701 0100  ......n.1.sKw...
-000009e0: 0100 0100 5900 0100 7405 7c03 6402 8302  ....Y...t.|.d...
-000009f0: 8f1f 7d06 7a07 7403 a004 7c06 a101 7d07  ..}.z.t...|...}.
-00000a00: 5700 6e0f 0400 7403 6a0b 6a0c 796c 0100  W.n...t.j.j.yl..
-00000a10: 0100 0100 6405 640b 6901 7d07 5900 6e01  ....d.d.i.}.Y.n.
-00000a20: 7700 5700 6400 0400 0400 8303 0100 6e08  w.W.d.........n.
-00000a30: 3100 7377 7701 0100 0100 0100 5900 0100  1.sww.......Y...
-00000a40: 6700 7d08 7408 7c02 7600 72a7 7c07 a00d  g.}.t.|.v.r.|...
-00000a50: a100 4400 5d20 5c02 7d09 7d0a 7c07 7c09  ..D.] \.}.}.|.|.
-00000a60: 1900 640b 6b02 72a6 7c09 7400 6a0e 7600  ..d.k.r.|.t.j.v.
-00000a70: 729d 7400 6a0e 7c09 1900 7c07 7c09 3c00  r.t.j.|...|.|.<.
-00000a80: 7186 7c08 a00f 7c09 a101 0100 7c0a 7c07  q.|...|.....|.|.
-00000a90: 7c09 3c00 7186 7410 7c08 8301 640c 6b04  |.<.q.t.|...d.k.
-00000aa0: 72d6 7407 640d 8301 0100 7c08 4400 5d19  r.t.d.....|.D.].
-00000ab0: 7d09 7c09 7c02 7408 1900 7600 72c1 7c02  }.|.|.t...v.r.|.
-00000ac0: 7408 1900 7c09 1900 6e01 640e 7d0b 7407  t...|...n.d.}.t.
-00000ad0: 7c09 9b00 640f 7c0b 9b00 9d03 8301 0100  |...d.|.........
-00000ae0: 71b3 7407 6410 8301 0100 7411 a012 6411  q.t.d.....t...d.
-00000af0: a101 0100 6412 6701 7d0c 7c0c 4400 5d38  ....d.g.}.|.D.]8
-00000b00: 7d09 7c09 7c07 7600 72f5 7400 6a01 6a02  }.|.|.v.r.t.j.j.
-00000b10: 7c07 7c09 1900 6701 7c00 6a13 a014 6413  |.|...g.|.j...d.
-00000b20: a101 a201 5200 8e00 7c07 7c09 3c00 0100  ....R...|.|.<...
-00000b30: 6e1f 7400 6a0e a015 7c09 6400 a102 6400  n.t.j...|.d...d.
-00000b40: 7501 9001 7213 7400 6a0e a015 7c09 6400  u...r.t.j...|.d.
-00000b50: a102 640b 6b03 9001 7213 7400 6a0e a015  ..d.k...r.t.j...
-00000b60: 7c09 a101 7c07 7c09 3c00 0100 6e01 71db  |...|.|.<...n.q.
-00000b70: 7410 7c07 8301 640c 6b02 9001 7228 7407  t.|...d.k...r(t.
-00000b80: 6414 8301 0100 7407 6410 8301 0100 7411  d.....t.d.....t.
-00000b90: a012 6411 a101 0100 7416 7c00 6415 7c07  ..d.....t.|.d.|.
-00000ba0: 8303 0100 6400 5300 2916 4e72 2e00 0000  ....d.S.).Nr....
-00000bb0: 722f 0000 007a 0865 6e76 2e6a 736f 6e7a  r/...z.env.jsonz
-00000bc0: 4045 6e76 6972 6f6e 6d65 6e74 2066 696c  @Environment fil
-00000bd0: 6520 6e6f 7420 666f 756e 642c 2063 7265  e not found, cre
-00000be0: 6174 696e 6720 6f6e 6520 7769 7468 2064  ating one with d
-00000bf0: 6566 6175 6c74 733a 2065 6e76 2e6a 736f  efaults: env.jso
-00000c00: 6e72 3700 0000 6301 0000 0000 0000 0000  nr7...c.........
-00000c10: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00000c20: 1200 0000 6900 7c00 5d05 7d01 7c01 6400  ....i.|.].}.|.d.
-00000c30: 9302 7102 5300 2901 da00 7223 0000 0029  ..q.S.)...r#...)
-00000c40: 02da 022e 3072 2100 0000 7223 0000 0072  ....0r!...r#...r
-00000c50: 2300 0000 7224 0000 00da 0a3c 6469 6374  #...r$.....<dict
-00000c60: 636f 6d70 3e7f 0000 0073 0200 0000 1200  comp>....s......
-00000c70: 7a29 456e 7669 726f 6e6d 656e 742e 5f5f  z)Environment.__
-00000c80: 7365 745f 656e 762e 3c6c 6f63 616c 733e  set_env.<locals>
-00000c90: 2e3c 6469 6374 636f 6d70 3e72 3900 0000  .<dictcomp>r9...
-00000ca0: 7207 0000 0072 3a00 0000 7243 0000 0072  r....r:...rC...r
-00000cb0: 0100 0000 7a47 456e 7669 726f 6e6d 656e  ....zGEnvironmen
-00000cc0: 7420 7661 7269 6162 6c65 7320 6e6f 7420  t variables not 
-00000cd0: 666f 756e 642e 2053 6574 2074 6865 6d20  found. Set them 
-00000ce0: 696e 2065 6e76 2e6a 736f 6e20 6f72 2069  in env.json or i
-00000cf0: 6e20 796f 7572 2073 6865 6c6c 2e7a 1d52  n your shell.z.R
-00000d00: 6571 7569 7265 6420 656e 7669 726f 6e6d  equired environm
-00000d10: 656e 7420 7661 7269 6162 6c65 fa03 203a  ent variable.. :
-00000d20: 20fa 0a45 7869 7469 6e67 2e2e 2e72 0400   ..Exiting...r..
-00000d30: 0000 5a09 6175 746f 5f73 6176 6572 0900  ..Z.auto_saver..
-00000d40: 0000 7a59 7265 7375 6c74 732f 7361 7665  ..zYresults/save
-00000d50: 5f64 6972 2f73 6176 6520 656e 7669 726f  _dir/save enviro
-00000d60: 6e6d 656e 7420 7661 7269 6162 6c65 2069  nment variable i
-00000d70: 7320 656d 7074 792e 2053 6574 2069 7420  s empty. Set it 
-00000d80: 696e 2065 6e76 2e6a 736f 6e20 6f72 2069  in env.json or i
-00000d90: 6e20 796f 7572 2073 6865 6c6c 2e72 0200  n your shell.r..
-00000da0: 0000 2917 7219 0000 0072 1a00 0000 721b  ..).r....r....r.
-00000db0: 0000 0072 3300 0000 7234 0000 0072 3500  ...r3...r4...r5.
-00000dc0: 0000 7232 0000 00da 0570 7269 6e74 da07  ..r2.....print..
-00000dd0: 454e 565f 4b45 59da 046b 6579 7372 3f00  ENV_KEY..keysr?.
-00000de0: 0000 da07 6465 636f 6465 725a 0f4a 534f  ....decoderZ.JSO
-00000df0: 4e44 6563 6f64 6545 7272 6f72 da05 6974  NDecodeError..it
-00000e00: 656d 73da 0765 6e76 6972 6f6e da06 6170  ems..environ..ap
-00000e10: 7065 6e64 da03 6c65 6e72 1000 0000 da04  pend..lenr......
-00000e20: 6578 6974 721c 0000 0072 1500 0000 da03  exitr....r......
-00000e30: 6765 7472 0f00 0000 290d 721f 0000 005a  getr....).r....Z
-00000e40: 0e6d 6174 655f 636f 6e66 5f70 6174 6872  .mate_conf_pathr
-00000e50: 3600 0000 5a08 656e 765f 7061 7468 da0d  6...Z.env_path..
-00000e60: 7265 7175 6972 6564 5f6b 6579 735a 0b64  required_keysZ.d
-00000e70: 6566 7561 6c74 5f65 6e76 7242 0000 0072  efualt_envrB...r
-00000e80: 0200 0000 5a0d 656e 765f 6e6f 745f 666f  ....Z.env_not_fo
-00000e90: 756e 6472 2100 0000 7222 0000 005a 0464  undr!...r"...Z.d
-00000ea0: 6573 635a 0e73 6561 7263 685f 7265 7375  escZ.search_resu
-00000eb0: 6c74 7372 2300 0000 7223 0000 0072 2400  ltsr#...r#...r$.
-00000ec0: 0000 5a09 5f5f 7365 745f 656e 7672 0000  ..Z.__set_envr..
-00000ed0: 0073 6e00 0000 0c01 1001 0c02 0c01 0801  .sn.............
-00000ee0: 0802 0e01 0602 0e02 0c02 1201 1cff 0c03  ................
-00000ef0: 0201 0e01 1001 0402 08ff 02ff 0280 1cfd  ................
-00000f00: 0408 0802 1001 0c01 0a01 1001 0a03 0801  ................
-00000f10: 0280 0c02 0201 0201 04ff 0802 1c01 1401  ................
-00000f20: 0802 0a01 0603 0801 0801 2401 0402 2801  ..........$...(.
-00000f30: 1001 0402 0280 0e02 0201 0201 04ff 0802  ................
-00000f40: 0a01 1002 7a15 456e 7669 726f 6e6d 656e  ....z.Environmen
-00000f50: 742e 5f5f 7365 745f 656e 7663 0200 0000  t.__set_envc....
-00000f60: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000f70: 0300 0000 73be 0000 007c 017c 006a 0076  ....s....|.|.j.v
-00000f80: 0072 0a7c 006a 007c 0119 0053 0074 016a  .r.|.j.|...S.t.j
-00000f90: 02a0 037c 0164 00a1 027d 027c 0264 0075  ...|.d...}.|.d.u
-00000fa0: 0172 177c 0253 007c 017c 0076 0172 597c  .r.|.S.|.|.v.rY|
-00000fb0: 017c 006a 0476 0072 257c 006a 047c 0119  .|.j.v.r%|.j.|..
-00000fc0: 0053 007c 017c 006a 0076 0072 2f7c 006a  .S.|.|.j.v.r/|.j
-00000fd0: 007c 0119 0053 007c 017c 006a 0576 0072  .|...S.|.|.j.v.r
-00000fe0: 397c 006a 057c 0119 0053 007c 0264 0075  9|.j.|...S.|.d.u
-00000ff0: 0073 417c 0264 016b 0272 5774 0664 027c  .sA|.d.k.rWt.d.|
-00001000: 019b 0064 039d 0383 0101 0074 0664 0483  ...d.......t.d..
-00001010: 0101 0074 0664 0583 0101 0074 07a0 0864  ...t.d.....t...d
-00001020: 06a1 0101 006e 027c 0253 0074 0983 00a0  .....n.|.S.t....
-00001030: 0a7c 01a1 0153 0029 074e 7243 0000 007a  .|...S.).NrC...z
-00001040: 1545 6e76 6972 6f6e 6d65 6e74 2076 6172  .Environment var
-00001050: 6961 626c 6520 7a30 206e 6f74 2066 6f75  iable z0 not fou
-00001060: 6e64 2e20 5365 7420 6974 2069 6e20 656e  nd. Set it in en
-00001070: 762e 6a73 6f6e 206f 7220 696e 2079 6f75  v.json or in you
-00001080: 7220 7368 656c 6c2e 7a48 4f72 2073 6574  r shell.zHOr set
-00001090: 2061 7320 616e 2061 7267 756d 656e 7420   as an argument 
-000010a0: 746f 2074 6865 2073 6372 6970 743a 2070  to the script: p
-000010b0: 7974 686f 6e20 2d6d 206d 6f64 756c 652e  ython -m module.
-000010c0: 7472 6169 6e20 6172 673d 3120 6172 6732  train arg=1 arg2
-000010d0: 3d32 7247 0000 0072 0400 0000 290b 720e  =2rG...r....).r.
-000010e0: 0000 0072 1900 0000 724d 0000 0072 5100  ...r....rM...rQ.
-000010f0: 0000 7202 0000 00da 085f 5f64 6963 745f  ..r......__dict_
-00001100: 5f72 4800 0000 7210 0000 0072 5000 0000  _rH...r....rP...
-00001110: da05 7375 7065 72da 0b5f 5f67 6574 6974  ..super..__getit
-00001120: 656d 5f5f 2903 721f 0000 0072 2100 0000  em__).r....r!...
-00001130: da03 7265 73a9 01da 095f 5f63 6c61 7373  ..res....__class
-00001140: 5f5f 7223 0000 0072 2400 0000 7255 0000  __r#...r$...rU..
-00001150: 00b6 0000 0073 2e00 0000 0a04 0a01 0e02  .....s..........
-00001160: 0802 0401 0802 0a03 0a01 0a02 0a01 0a02  ................
-00001170: 0a01 1002 0201 0a01 04ff 0202 0201 04ff  ................
-00001180: 0802 0c01 0402 0c02 7a17 456e 7669 726f  ........z.Enviro
-00001190: 6e6d 656e 742e 5f5f 6765 7469 7465 6d5f  nment.__getitem_
-000011a0: 5f4e 6303 0000 0000 0000 0000 0000 0004  _Nc.............
-000011b0: 0000 0004 0000 0003 0000 0073 6e00 0000  ...........sn...
-000011c0: 7c01 7c00 6a00 7600 720a 7c00 6a00 7c01  |.|.j.v.r.|.j.|.
-000011d0: 1900 5300 7401 6a02 a003 7c01 6400 a102  ..S.t.j...|.d...
-000011e0: 7d03 7c03 6400 7501 7217 7c03 5300 7c01  }.|.d.u.r.|.S.|.
-000011f0: 7c00 7600 7221 7404 8300 a005 7c01 a101  |.v.r!t.....|...
-00001200: 5300 7c01 7c00 6a06 7600 722b 7c00 6a06  S.|.|.j.v.r+|.j.
-00001210: 7c01 1900 5300 7c01 7c00 6a07 7600 7235  |...S.|.|.j.v.r5
-00001220: 7c00 6a07 7c01 1900 5300 7c02 5300 a901  |.j.|...S.|.S...
-00001230: 4e29 0872 0e00 0000 7219 0000 0072 4d00  N).r....r....rM.
-00001240: 0000 7251 0000 0072 5400 0000 7255 0000  ..rQ...rT...rU..
-00001250: 0072 0200 0000 7253 0000 0029 0472 1f00  .r....rS...).r..
-00001260: 0000 7221 0000 00da 0764 6566 6175 6c74  ..r!.....default
-00001270: 7256 0000 0072 5700 0000 7223 0000 0072  rV...rW...r#...r
-00001280: 2400 0000 7255 0000 00da 0000 0073 1800  $...rU.......s..
-00001290: 0000 0a03 0a01 0e03 0802 0401 0802 0c01  ................
-000012a0: 0a04 0a01 0a05 0a01 0402 6303 0000 0000  ..........c.....
-000012b0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-000012c0: 0000 00f3 0c00 0000 7c00 a000 7c01 7c02  ........|...|.|.
-000012d0: a102 5300 7259 0000 00a9 0172 5500 0000  ..S.rY.....rU...
-000012e0: a903 721f 0000 0072 2100 0000 725a 0000  ..r....r!...rZ..
-000012f0: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
-00001300: da08 6765 745f 6974 656d f600 0000 f302  ..get_item......
-00001310: 0000 000c 017a 1445 6e76 6972 6f6e 6d65  .....z.Environme
-00001320: 6e74 2e67 6574 5f69 7465 6d63 0300 0000  nt.get_itemc....
-00001330: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00001340: 4300 0000 725b 0000 0072 5900 0000 725c  C...r[...rY...r\
-00001350: 0000 0072 5d00 0000 7223 0000 0072 2300  ...r]...r#...r#.
-00001360: 0000 7224 0000 00da 0a67 6574 5f68 7061  ..r$.....get_hpa
-00001370: 7261 6df9 0000 0072 5f00 0000 7a16 456e  ram....r_...z.En
-00001380: 7669 726f 6e6d 656e 742e 6765 745f 6870  vironment.get_hp
-00001390: 6172 616d 6301 0000 0000 0000 0000 0000  aramc...........
-000013a0: 0003 0000 0005 0000 0043 0000 0073 7000  .........C...sp.
-000013b0: 0000 7400 6401 7c00 6a01 9b00 9d02 8301  ..t.d.|.j.......
-000013c0: 0100 7400 6402 8301 0100 7c00 6a02 a003  ..t.d.....|.j...
-000013d0: a100 4400 5d0d 5c02 7d01 7d02 7400 7c01  ..D.].\.}.}.t.|.
-000013e0: 9b00 6403 7c02 9b00 9d03 8301 0100 7111  ..d.|.........q.
-000013f0: 7400 6404 8301 0100 7c00 6a04 a003 a100  t.d.....|.j.....
-00001400: 4400 5d0d 5c02 7d01 7d02 7400 7c01 9b00  D.].\.}.}.t.|...
-00001410: 6403 7c02 9b00 9d03 8301 0100 7128 6400  d.|.........q(d.
-00001420: 5300 2905 4e7a 0c45 7870 6572 696d 656e  S.).Nz.Experimen
-00001430: 743a 207a 1048 7970 6572 7061 7261 6d65  t: z.Hyperparame
-00001440: 7465 7273 3a72 4600 0000 7a16 456e 7669  ters:rF...z.Envi
-00001450: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00001460: 733a 2905 7248 0000 0072 1c00 0000 720e  s:).rH...r....r.
-00001470: 0000 0072 4c00 0000 7202 0000 0029 0372  ...rL...r....).r
-00001480: 1f00 0000 7221 0000 0072 2200 0000 7223  ....r!...r"...r#
-00001490: 0000 0072 2300 0000 7224 0000 00da 0a70  ...r#...r$.....p
-000014a0: 7269 6e74 5f69 6e66 6ffc 0000 0073 1000  rint_info....s..
-000014b0: 0000 1002 0802 1201 1401 0802 1201 1401  ................
-000014c0: 04ff 7a16 456e 7669 726f 6e6d 656e 742e  ..z.Environment.
-000014d0: 7072 696e 745f 696e 666f 7259 0000 0029  print_inforY...)
-000014e0: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000014f0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001500: 616d 655f 5f72 2500 0000 7216 0000 0072  ame__r%...r....r
-00001510: 1300 0000 721e 0000 0072 1d00 0000 7255  ....r....r....rU
-00001520: 0000 0072 5e00 0000 7260 0000 0072 6100  ...r^...r`...ra.
-00001530: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-00001540: 5f72 2300 0000 7223 0000 0072 5700 0000  _r#...r#...rW...
-00001550: 7224 0000 0072 0300 0000 0c00 0000 7316  r$...r........s.
-00001560: 0000 0008 0008 0208 2f08 0e08 0c08 1b0c  ......../.......
-00001570: 440e 240a 1c0a 0310 0372 0300 0000 2908  D.$......r....).
-00001580: 7233 0000 0072 1900 0000 723d 0000 0072  r3...r....r=...r
-00001590: 1000 0000 5a04 6970 6462 7249 0000 0072  ....Z.ipdbrI...r
-000015a0: 4000 0000 7203 0000 0072 2300 0000 7223  @...r....r#...r#
-000015b0: 0000 0072 2300 0000 7224 0000 00da 083c  ...r#...r$.....<
-000015c0: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
-000015d0: 0801 0801 0801 0801 0801 0403 1403       ..............
+00000150: 5f04 6400 7c00 5f05 7a14 7406 7c00 7407  _.d.|._.z.t.|.t.
+00000160: 6a08 6402 1900 6403 8303 0100 7406 7c00  j.d...d.....t.|.
+00000170: 6404 7407 6a08 6402 1900 8303 0100 5700  d.t.j.d.......W.
+00000180: 6e04 0100 0100 0100 5900 7407 6a08 6402  n.......Y.t.j.d.
+00000190: 6400 8502 1900 7c00 5f09 7c00 a00a a100  d.....|._.|.....
+000001a0: 7c00 5f0b 740c 6a0d a00e 7c00 6a0b a101  |._.t.j...|.j...
+000001b0: 7c00 5f0f 7c00 6a0f 7407 6a0d 7601 724d  |._.|.j.t.j.v.rM
+000001c0: 7407 6a0d a010 7c00 6a0f a101 0100 7407  t.j...|.j.....t.
+000001d0: 6a08 4400 5d29 7d01 6405 7c01 7601 7257  j.D.])}.d.|.v.rW
+000001e0: 7150 7c01 a011 6405 a101 5c02 7d02 7d03  qP|...d...\.}.}.
+000001f0: 7c00 a012 7c03 a101 7d03 7c02 a013 6406  |...|...}.|...d.
+00000200: a101 726e 7c02 6407 6400 8502 1900 7d02  ..rn|.d.d.....}.
+00000210: 7406 7c00 7c02 7c03 8303 0100 7c03 7c00  t.|.|.|.....|.|.
+00000220: 6a04 7c02 3c00 7150 7407 6a08 6408 1900  j.|.<.qPt.j.d...
+00000230: 7c00 5f14 6409 7c00 6a14 7600 72a5 740c  |._.d.|.j.v.r.t.
+00000240: 6a0d 6a15 7407 6a08 6407 640a 8502 1900  j.j.t.j.d.d.....
+00000250: 8e00 7c00 5f16 740c 6a0d a015 7c00 6a0b  ..|._.t.j...|.j.
+00000260: 640b 7407 6a08 6407 1900 7407 6a08 640c  d.t.j.d...t.j.d.
+00000270: 1900 640d 1700 a104 7c00 5f14 6e17 7c00  ..d.....|._.n.|.
+00000280: 6a14 a011 640e a101 640f 6400 8502 1900  j...d...d.d.....
+00000290: 7c00 5f16 740c 6a0d 6a15 7c00 6a16 8e00  |._.t.j.j.|.j...
+000002a0: 6400 6410 8502 1900 7c00 5f16 7c00 a017  d.d.....|._.|...
+000002b0: a100 0100 7c00 6a02 72c9 7c00 a018 a100  ....|.j.r.|.....
+000002c0: 0100 6400 5300 6400 5300 2911 4e46 e901  ..d.S.d.S.).NF..
+000002d0: 0000 0054 da06 6163 7469 6f6e da01 3d7a  ...T..action..=z
+000002e0: 022d 2de9 0200 0000 7201 0000 007a 0862  .--.....r....z.b
+000002f0: 696e 2f6d 6174 65e9 0400 0000 5a0b 6578  in/mate.....Z.ex
+00000300: 7065 7269 6d65 6e74 73e9 0300 0000 7a03  periments.....z.
+00000310: 2e70 79fa 012f e9fe ffff ffe9 fdff ffff  .py../..........
+00000320: 2919 5a07 7265 7374 6172 74da 0474 6573  ).Z.restart..tes
+00000330: 745a 0574 7261 696e da06 7361 6d70 6c65  tZ.train..sample
+00000340: da07 6870 6172 616d 7372 0500 0000 da07  ..hparamsr......
+00000350: 7365 7461 7474 72da 0373 7973 da04 6172  setattr..sys..ar
+00000360: 6776 da04 6172 6773 da17 5f45 6e76 6972  gv..args.._Envir
+00000370: 6f6e 6d65 6e74 5f5f 6669 6e64 5f72 6f6f  onment__find_roo
+00000380: 74da 055f 726f 6f74 da02 6f73 da04 7061  t.._root..os..pa
+00000390: 7468 da07 6469 726e 616d 65da 095f 726f  th..dirname.._ro
+000003a0: 6f74 5f64 6972 da06 6170 7065 6e64 da05  ot_dir..append..
+000003b0: 7370 6c69 74da 1363 6f6e 7665 7274 5f73  split..convert_s
+000003c0: 7472 5f74 6f5f 6461 7461 da0a 7374 6172  tr_to_data..star
+000003d0: 7473 7769 7468 da05 5f70 6174 68da 046a  tswith.._path..j
+000003e0: 6f69 6eda 046e 616d 65da 155f 456e 7669  oin..name.._Envi
+000003f0: 726f 6e6d 656e 745f 5f73 6574 5f65 6e76  ronment__set_env
+00000400: da21 5f45 6e76 6972 6f6e 6d65 6e74 5f5f  .!_Environment__
+00000410: 6765 6e65 7261 7465 5f65 7870 6572 696d  generate_experim
+00000420: 656e 7429 04da 0473 656c 66da 0361 7267  ent)...self..arg
+00000430: da03 6b65 79da 0576 616c 7565 a900 7227  ..key..value..r'
+00000440: 0000 00fa 3b2f 686f 6d65 2f61 6c2f 4769  ....;/home/al/Gi
+00000450: 7448 7562 2f79 6572 6261 6d61 7465 2f70  tHub/yerbamate/p
+00000460: 6163 6b61 6765 732f 7965 7262 616d 6174  ackages/yerbamat
+00000470: 652f 656e 7669 726f 6e6d 656e 742e 7079  e/environment.py
+00000480: da08 5f5f 696e 6974 5f5f 0c00 0000 734a  ..__init__....sJ
+00000490: 0000 0006 0206 0106 0106 0106 0106 0102  ................
+000004a0: 0312 0116 0106 0102 0110 020a 0210 010c  ................
+000004b0: 020e 010a 0308 0102 010e 010a 010a 020c  ................
+000004c0: 010c 020c 010c 020a 0118 0106 011a 0108  ................
+000004d0: ff16 0518 0108 0206 020c 0104 ff7a 1445  .............z.E
+000004e0: 6e76 6972 6f6e 6d65 6e74 2e5f 5f69 6e69  nvironment.__ini
+000004f0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+00000500: 0200 0000 0b00 0000 4300 0000 7360 0000  ........C...s`..
+00000510: 007a 0574 007c 0183 0157 0053 0004 0074  .z.t.|...W.S...t
+00000520: 0179 2f01 0001 0001 007a 0774 027c 0183  .y/......z.t.|..
+00000530: 0157 0006 0059 0053 0004 0074 0179 2e01  .W...Y.S...t.y..
+00000540: 0001 0001 007c 0164 0176 0072 2259 0059  .....|.d.v.r"Y.Y
+00000550: 0064 0253 007c 0164 0376 0072 2a59 0059  .d.S.|.d.v.r*Y.Y
+00000560: 0064 0453 0059 0059 007c 0153 0077 0077  .d.S.Y.Y.|.S.w.w
+00000570: 0029 054e 2902 da04 5472 7565 da04 7472  .).N)...True..tr
+00000580: 7565 5429 02da 0546 616c 7365 da05 6661  ueT)...False..fa
+00000590: 6c73 6546 2903 da03 696e 74da 0a56 616c  lseF)...int..Val
+000005a0: 7565 4572 726f 72da 0566 6c6f 6174 2902  ueError..float).
+000005b0: 7223 0000 00da 0569 6e70 7574 7227 0000  r#.....inputr'..
+000005c0: 0072 2700 0000 7228 0000 0072 1c00 0000  .r'...r(...r....
+000005d0: 4100 0000 731c 0000 0002 010a 010c 0102  A...s...........
+000005e0: 010e 010c 0108 0108 0108 0108 0104 ff04  ................
+000005f0: 0302 fa02 fd7a 1f45 6e76 6972 6f6e 6d65  .....z.Environme
+00000600: 6e74 2e63 6f6e 7665 7274 5f73 7472 5f74  nt.convert_str_t
+00000610: 6f5f 6461 7461 6301 0000 0000 0000 0000  o_datac.........
+00000620: 0000 0005 0000 0008 0000 0043 0000 0073  ...........C...s
+00000630: b600 0000 7400 a001 a100 7d01 7400 6a02  ....t.....}.t.j.
+00000640: a003 7400 6a02 a004 7c01 6401 a102 a101  ..t.j...|.d.....
+00000650: 7225 7405 a006 7407 7400 6a02 a004 7c01  r%t...t.t.j...|.
+00000660: 6401 a102 6402 8302 a101 7d02 7400 6a02  d...d.....}.t.j.
+00000670: a004 7c01 7c02 6403 1900 a102 5300 6404  ..|.|.d.....S.d.
+00000680: 7d03 7408 7c03 8301 4400 5d2b 7d04 7400  }.t.|...D.]+}.t.
+00000690: 6a02 a009 7c01 a101 7d01 7400 6a02 a003  j...|...}.t.j...
+000006a0: 7400 6a02 a004 7c01 6401 a102 a101 7256  t.j...|.d.....rV
+000006b0: 7405 a006 7407 7400 6a02 a004 7c01 6401  t...t.t.j...|.d.
+000006c0: a102 6402 8302 a101 7d02 7400 6a02 a004  ..d.....}.t.j...
+000006d0: 7c01 7c02 6403 1900 a102 0200 0100 5300  |.|.d.........S.
+000006e0: 712b 740a 6405 8301 8201 2906 4efa 096d  q+t.d.....).N..m
+000006f0: 6174 652e 6a73 6f6e da01 72da 0770 726f  ate.json..r..pro
+00000700: 6a65 6374 7208 0000 007a 1e43 6f75 6c64  jectr....z.Could
+00000710: 206e 6f74 2066 696e 6420 726f 6f74 206f   not find root o
+00000720: 6620 7072 6f6a 6563 7429 0b72 1600 0000  f project).r....
+00000730: da06 6765 7463 7764 7217 0000 00da 0665  ..getcwdr......e
+00000740: 7869 7374 7372 1f00 0000 da04 6a73 6f6e  xistsr......json
+00000750: da04 6c6f 6164 da04 6f70 656e da05 7261  ..load..open..ra
+00000760: 6e67 6572 1800 0000 da09 4578 6365 7074  nger......Except
+00000770: 696f 6e29 0572 2300 0000 7217 0000 00da  ion).r#...r.....
+00000780: 0463 6f6e 665a 0d6d 6178 5f72 6563 7572  .confZ.max_recur
+00000790: 7369 6f6e da01 6972 2700 0000 7227 0000  sion..ir'...r'..
+000007a0: 0072 2800 0000 5a0b 5f5f 6669 6e64 5f72  .r(...Z.__find_r
+000007b0: 6f6f 744f 0000 0073 1800 0000 0803 1602  ootO...s........
+000007c0: 1a01 1202 0403 0c01 0c02 1602 1a01 1602  ................
+000007d0: 02fd 0805 7a17 456e 7669 726f 6e6d 656e  ....z.Environmen
+000007e0: 742e 5f5f 6669 6e64 5f72 6f6f 7463 0100  t.__find_rootc..
+000007f0: 0000 0000 0000 0000 0000 0700 0000 0800  ................
+00000800: 0000 4300 0000 73d2 0000 0067 0064 01a2  ..C...s....g.d..
+00000810: 017d 0164 007d 027c 0144 005d 0e7d 037c  .}.d.}.|.D.].}.|
+00000820: 037c 006a 0076 0072 167c 006a 007c 0319  .|.j.v.r.|.j.|..
+00000830: 007d 0201 006e 0171 087c 0264 0075 0072  .}...n.q.|.d.u.r
+00000840: 1d64 0053 0074 016a 02a0 037c 02a1 0173  .d.S.t.j...|...s
+00000850: 2a74 016a 047c 0264 0264 038d 0201 0074  *t.j.|.d.d.....t
+00000860: 016a 02a0 057c 0264 04a1 027d 0474 06a0  .j...|.d...}.t..
+00000870: 077c 006a 087c 04a1 0201 007c 006a 0969  .|.j.|.....|.j.i
+00000880: 006b 0372 6774 016a 02a0 057c 0264 05a1  .k.rgt.j...|.d..
+00000890: 027d 0574 0a7c 0564 0683 028f 147d 0674  .}.t.|.d.....}.t
+000008a0: 0b6a 0c74 0d7c 006a 0983 017c 0664 0764  .j.t.|.j...|.d.d
+000008b0: 088d 0301 0057 0064 0004 0004 0083 0301  .....W.d........
+000008c0: 0064 0053 0031 0073 6077 0101 0001 0001  .d.S.1.s`w......
+000008d0: 0059 0001 0064 0053 0064 0053 0029 094e  .Y...d.S.d.S.).N
+000008e0: 2906 da07 7265 7375 6c74 735a 0c72 6573  )...resultsZ.res
+000008f0: 756c 7473 5f70 6174 685a 0b72 6573 756c  ults_pathZ.resul
+00000900: 7473 5f64 6972 da04 7361 7665 da09 7361  ts_dir..save..sa
+00000910: 7665 5f70 6174 685a 0873 6176 655f 6469  ve_pathZ.save_di
+00000920: 7254 2901 da08 6578 6973 745f 6f6b 7a0d  rT)...exist_okz.
+00000930: 6578 7065 7269 6d65 6e74 2e70 797a 0f65  experiment.pyz.e
+00000940: 7870 6572 696d 656e 742e 6a73 6f6e da01  xperiment.json..
+00000950: 7772 0800 0000 a901 da06 696e 6465 6e74  wr........indent
+00000960: 290e 7202 0000 0072 1600 0000 7217 0000  ).r....r....r...
+00000970: 0072 3600 0000 da08 6d61 6b65 6469 7273  .r6.....makedirs
+00000980: 721f 0000 00da 0673 6875 7469 6cda 0863  r......shutil..c
+00000990: 6f70 7966 696c 6572 1e00 0000 720f 0000  opyfiler....r...
+000009a0: 0072 3900 0000 7237 0000 00da 0464 756d  .r9...r7.....dum
+000009b0: 70da 0464 6963 7429 0772 2300 0000 723e  p..dict).r#...r>
+000009c0: 0000 00da 0672 6573 756c 7472 2500 0000  .....resultr%...
+000009d0: 5a09 7361 7665 5f66 696c 655a 0b70 6172  Z.save_fileZ.par
+000009e0: 616d 735f 6669 6c65 da01 6672 2700 0000  ams_file..fr'...
+000009f0: 7227 0000 0072 2800 0000 5a15 5f5f 6765  r'...r(...Z.__ge
+00000a00: 6e65 7261 7465 5f65 7870 6572 696d 656e  nerate_experimen
+00000a10: 7468 0000 0073 2600 0000 0802 0408 0801  th...s&.........
+00000a20: 0a01 0a01 0401 02fe 0803 0401 0c01 0e01  ................
+00000a30: 0e02 0e02 0a04 0e01 0c03 1801 22ff 04fc  ............"...
+00000a40: 7a21 456e 7669 726f 6e6d 656e 742e 5f5f  z!Environment.__
+00000a50: 6765 6e65 7261 7465 5f65 7870 6572 696d  generate_experim
+00000a60: 656e 7463 0100 0000 0000 0000 0000 0000  entc............
+00000a70: 0d00 0000 0900 0000 4300 0000 7368 0200  ........C...sh..
+00000a80: 0074 006a 01a0 027c 006a 0364 01a1 027d  .t.j...|.j.d...}
+00000a90: 0174 04a0 0574 067c 0164 0283 02a1 017d  .t...t.|.d.....}
+00000aa0: 0274 006a 01a0 027c 006a 0364 03a1 027d  .t.j...|.j.d...}
+00000ab0: 0374 006a 01a0 077c 03a1 0173 5474 0864  .t.j...|...sTt.d
+00000ac0: 0483 0101 0074 097c 0276 0072 2d7c 0274  .....t.|.v.r-|.t
+00000ad0: 0919 00a0 0aa1 007d 046e 0364 0567 017d  .......}.n.d.g.}
+00000ae0: 0464 0664 0784 007c 0444 0083 017d 0574  .d.d...|.D...}.t
+00000af0: 067c 0364 0883 028f 107d 0674 046a 0b7c  .|.d.....}.t.j.|
+00000b00: 057c 0664 0964 0a8d 0301 0057 0064 0004  .|.d.d.....W.d..
+00000b10: 0004 0083 0301 006e 0831 0073 4f77 0101  .......n.1.sOw..
+00000b20: 0001 0001 0059 0001 0074 067c 0364 0283  .....Y...t.|.d..
+00000b30: 028f 1f7d 067a 0774 04a0 057c 06a1 017d  ...}.z.t...|...}
+00000b40: 0757 006e 0f04 0074 046a 0c6a 0d79 7001  .W.n...t.j.j.yp.
+00000b50: 0001 0001 0064 0564 0b69 017d 0759 006e  .....d.d.i.}.Y.n
+00000b60: 0177 0057 0064 0004 0004 0083 0301 006e  .w.W.d.........n
+00000b70: 0831 0073 7b77 0101 0001 0001 0059 0001  .1.s{w.......Y..
+00000b80: 0067 007d 0874 097c 0276 0072 ab7c 07a0  .g.}.t.|.v.r.|..
+00000b90: 0ea1 0044 005d 205c 027d 097d 0a7c 077c  ...D.] \.}.}.|.|
+00000ba0: 0919 0064 0b6b 0272 aa7c 0974 006a 0f76  ...d.k.r.|.t.j.v
+00000bb0: 0072 a174 006a 0f7c 0919 007c 077c 093c  .r.t.j.|...|.|.<
+00000bc0: 0071 8a7c 08a0 107c 09a1 0101 007c 0a7c  .q.|...|.....|.|
+00000bd0: 077c 093c 0071 8a74 117c 0883 0164 0c6b  .|.<.q.t.|...d.k
+00000be0: 0472 da74 0864 0d83 0101 007c 0844 005d  .r.t.d.....|.D.]
+00000bf0: 197d 097c 097c 0274 0919 0076 0072 c57c  .}.|.|.t...v.r.|
+00000c00: 0274 0919 007c 0919 006e 0164 0e7d 0b74  .t...|...n.d.}.t
+00000c10: 087c 099b 0064 0f7c 0b9b 009d 0383 0101  .|...d.|........
+00000c20: 0071 b774 0864 1083 0101 0074 12a0 1364  .q.t.d.....t...d
+00000c30: 11a1 0101 0064 1267 017d 0c7c 0c44 005d  .....d.g.}.|.D.]
+00000c40: 387d 097c 097c 0776 0072 f974 006a 016a  8}.|.|.v.r.t.j.j
+00000c50: 027c 077c 0919 0067 017c 006a 14a0 1564  .|.|...g.|.j...d
+00000c60: 13a1 01a2 0152 008e 007c 077c 093c 0001  .....R...|.|.<..
+00000c70: 006e 1f74 006a 0fa0 167c 0964 00a1 0264  .n.t.j...|.d...d
+00000c80: 0075 0190 0172 1774 006a 0fa0 167c 0964  .u...r.t.j...|.d
+00000c90: 00a1 0264 0b6b 0390 0172 1774 006a 0fa0  ...d.k...r.t.j..
+00000ca0: 167c 09a1 017c 077c 093c 0001 006e 0171  .|...|.|.<...n.q
+00000cb0: df74 117c 0783 0164 0c6b 0290 0172 2c74  .t.|...d.k...r,t
+00000cc0: 0864 1483 0101 0074 0864 1083 0101 0074  .d.....t.d.....t
+00000cd0: 12a0 1364 11a1 0101 0074 177c 0064 157c  ...d.....t.|.d.|
+00000ce0: 0783 0301 0064 0053 0029 164e 7232 0000  .....d.S.).Nr2..
+00000cf0: 0072 3300 0000 7a08 656e 762e 6a73 6f6e  .r3...z.env.json
+00000d00: 7a40 456e 7669 726f 6e6d 656e 7420 6669  z@Environment fi
+00000d10: 6c65 206e 6f74 2066 6f75 6e64 2c20 6372  le not found, cr
+00000d20: 6561 7469 6e67 206f 6e65 2077 6974 6820  eating one with 
+00000d30: 6465 6661 756c 7473 3a20 656e 762e 6a73  defaults: env.js
+00000d40: 6f6e 723e 0000 0063 0100 0000 0000 0000  onr>...c........
+00000d50: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00000d60: 7312 0000 0069 007c 005d 057d 017c 0164  s....i.|.].}.|.d
+00000d70: 0093 0271 0253 0029 01da 0072 2700 0000  ...q.S.)...r'...
+00000d80: 2902 da02 2e30 7225 0000 0072 2700 0000  )....0r%...r'...
+00000d90: 7227 0000 0072 2800 0000 da0a 3c64 6963  r'...r(.....<dic
+00000da0: 7463 6f6d 703e 9600 0000 7302 0000 0012  tcomp>....s.....
+00000db0: 007a 2945 6e76 6972 6f6e 6d65 6e74 2e5f  .z)Environment._
+00000dc0: 5f73 6574 5f65 6e76 2e3c 6c6f 6361 6c73  _set_env.<locals
+00000dd0: 3e2e 3c64 6963 7463 6f6d 703e 7242 0000  >.<dictcomp>rB..
+00000de0: 0072 0800 0000 7243 0000 0072 4c00 0000  .r....rC...rL...
+00000df0: 7201 0000 007a 4745 6e76 6972 6f6e 6d65  r....zGEnvironme
+00000e00: 6e74 2076 6172 6961 626c 6573 206e 6f74  nt variables not
+00000e10: 2066 6f75 6e64 2e20 5365 7420 7468 656d   found. Set them
+00000e20: 2069 6e20 656e 762e 6a73 6f6e 206f 7220   in env.json or 
+00000e30: 696e 2079 6f75 7220 7368 656c 6c2e 7a1d  in your shell.z.
+00000e40: 5265 7175 6972 6564 2065 6e76 6972 6f6e  Required environ
+00000e50: 6d65 6e74 2076 6172 6961 626c 65fa 0320  ment variable.. 
+00000e60: 3a20 fa0a 4578 6974 696e 672e 2e2e 7204  : ..Exiting...r.
+00000e70: 0000 005a 0961 7574 6f5f 7361 7665 720a  ...Z.auto_saver.
+00000e80: 0000 007a 5972 6573 756c 7473 2f73 6176  ...zYresults/sav
+00000e90: 655f 6469 722f 7361 7665 2065 6e76 6972  e_dir/save envir
+00000ea0: 6f6e 6d65 6e74 2076 6172 6961 626c 6520  onment variable 
+00000eb0: 6973 2065 6d70 7479 2e20 5365 7420 6974  is empty. Set it
+00000ec0: 2069 6e20 656e 762e 6a73 6f6e 206f 7220   in env.json or 
+00000ed0: 696e 2079 6f75 7220 7368 656c 6c2e 7202  in your shell.r.
+00000ee0: 0000 0029 1872 1600 0000 7217 0000 0072  ...).r....r....r
+00000ef0: 1f00 0000 7219 0000 0072 3700 0000 7238  ....r....r7...r8
+00000f00: 0000 0072 3900 0000 7236 0000 00da 0570  ...r9...r6.....p
+00000f10: 7269 6e74 da07 454e 565f 4b45 59da 046b  rint..ENV_KEY..k
+00000f20: 6579 7372 4800 0000 da07 6465 636f 6465  eysrH.....decode
+00000f30: 72da 0f4a 534f 4e44 6563 6f64 6545 7272  r..JSONDecodeErr
+00000f40: 6f72 da05 6974 656d 73da 0765 6e76 6972  or..items..envir
+00000f50: 6f6e 721a 0000 00da 036c 656e 7211 0000  onr......lenr...
+00000f60: 00da 0465 7869 7472 2000 0000 721b 0000  ...exitr ...r...
+00000f70: 00da 0367 6574 7210 0000 0029 0d72 2300  ...getr....).r#.
+00000f80: 0000 5a0e 6d61 7465 5f63 6f6e 665f 7061  ..Z.mate_conf_pa
+00000f90: 7468 723c 0000 005a 0865 6e76 5f70 6174  thr<...Z.env_pat
+00000fa0: 68da 0d72 6571 7569 7265 645f 6b65 7973  h..required_keys
+00000fb0: 5a0b 6465 6675 616c 745f 656e 7672 4b00  Z.defualt_envrK.
+00000fc0: 0000 7202 0000 005a 0d65 6e76 5f6e 6f74  ..r....Z.env_not
+00000fd0: 5f66 6f75 6e64 7225 0000 0072 2600 0000  _foundr%...r&...
+00000fe0: da04 6465 7363 5a0e 7365 6172 6368 5f72  ..descZ.search_r
+00000ff0: 6573 756c 7473 7227 0000 0072 2700 0000  esultsr'...r'...
+00001000: 7228 0000 005a 095f 5f73 6574 5f65 6e76  r(...Z.__set_env
+00001010: 8900 0000 7376 0000 0010 0110 0110 020c  ....sv..........
+00001020: 0108 0108 020e 0106 020e 020c 0212 011c  ................
+00001030: ff0c 0302 010e 0110 0104 0208 ff02 ff02  ................
+00001040: 801c fd04 0808 0210 010c 010a 0110 010a  ................
+00001050: 0308 0102 800c 0202 0102 0104 ff08 030c  ................
+00001060: 030c ff02 0202 fd14 0508 020a 0106 0308  ................
+00001070: 0108 0124 0104 0214 0214 0110 0204 0202  ...$............
+00001080: 800e 0202 0102 0104 ff08 030a 0110 027a  ...............z
+00001090: 1545 6e76 6972 6f6e 6d65 6e74 2e5f 5f73  .Environment.__s
+000010a0: 6574 5f65 6e76 6302 0000 0000 0000 0000  et_envc.........
+000010b0: 0000 0003 0000 0004 0000 0003 0000 0073  ...............s
+000010c0: be00 0000 7c01 7c00 6a00 7600 720a 7c00  ....|.|.j.v.r.|.
+000010d0: 6a00 7c01 1900 5300 7401 6a02 a003 7c01  j.|...S.t.j...|.
+000010e0: 6400 a102 7d02 7c02 6400 7501 7217 7c02  d...}.|.d.u.r.|.
+000010f0: 5300 7c01 7c00 7601 7259 7c01 7c00 6a04  S.|.|.v.rY|.|.j.
+00001100: 7600 7225 7c00 6a04 7c01 1900 5300 7c01  v.r%|.j.|...S.|.
+00001110: 7c00 6a00 7600 722f 7c00 6a00 7c01 1900  |.j.v.r/|.j.|...
+00001120: 5300 7c01 7c00 6a05 7600 7239 7c00 6a05  S.|.|.j.v.r9|.j.
+00001130: 7c01 1900 5300 7c02 6400 7500 7341 7c02  |...S.|.d.u.sA|.
+00001140: 6401 6b02 7257 7406 6402 7c01 9b00 6403  d.k.rWt.d.|...d.
+00001150: 9d03 8301 0100 7406 6404 8301 0100 7406  ......t.d.....t.
+00001160: 6405 8301 0100 7407 a008 6406 a101 0100  d.....t...d.....
+00001170: 6e02 7c02 5300 7409 8300 a00a 7c01 a101  n.|.S.t.....|...
+00001180: 5300 2907 4e72 4c00 0000 7a15 456e 7669  S.).NrL...z.Envi
+00001190: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+000011a0: 207a 3020 6e6f 7420 666f 756e 642e 2053   z0 not found. S
+000011b0: 6574 2069 7420 696e 2065 6e76 2e6a 736f  et it in env.jso
+000011c0: 6e20 6f72 2069 6e20 796f 7572 2073 6865  n or in your she
+000011d0: 6c6c 2e7a 484f 7220 7365 7420 6173 2061  ll.zHOr set as a
+000011e0: 6e20 6172 6775 6d65 6e74 2074 6f20 7468  n argument to th
+000011f0: 6520 7363 7269 7074 3a20 7079 7468 6f6e  e script: python
+00001200: 202d 6d20 6d6f 6475 6c65 2e74 7261 696e   -m module.train
+00001210: 2061 7267 3d31 2061 7267 323d 3272 5000   arg=1 arg2=2rP.
+00001220: 0000 7204 0000 0029 0b72 0f00 0000 7216  ..r....).r....r.
+00001230: 0000 0072 5700 0000 725a 0000 0072 0200  ...rW...rZ...r..
+00001240: 0000 da08 5f5f 6469 6374 5f5f 7251 0000  ....__dict__rQ..
+00001250: 0072 1100 0000 7259 0000 00da 0573 7570  .r....rY.....sup
+00001260: 6572 da0b 5f5f 6765 7469 7465 6d5f 5f29  er..__getitem__)
+00001270: 0372 2300 0000 7225 0000 00da 0372 6573  .r#...r%.....res
+00001280: a901 da09 5f5f 636c 6173 735f 5f72 2700  ....__class__r'.
+00001290: 0000 7228 0000 0072 5f00 0000 d600 0000  ..r(...r_.......
+000012a0: 732e 0000 000a 030a 010e 0208 0204 0108  s...............
+000012b0: 020a 030a 010a 020a 010a 020a 0110 0202  ................
+000012c0: 010a 0104 ff02 0302 0104 ff08 030c 0104  ................
+000012d0: 020c 027a 1745 6e76 6972 6f6e 6d65 6e74  ...z.Environment
+000012e0: 2e5f 5f67 6574 6974 656d 5f5f 4e63 0300  .__getitem__Nc..
+000012f0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+00001300: 0000 0300 0000 736e 0000 007c 017c 006a  ......sn...|.|.j
+00001310: 0076 0072 0a7c 006a 007c 0119 0053 0074  .v.r.|.j.|...S.t
+00001320: 016a 02a0 037c 0164 00a1 027d 037c 0364  .j...|.d...}.|.d
+00001330: 0075 0172 177c 0353 007c 017c 0076 0072  .u.r.|.S.|.|.v.r
+00001340: 2174 0483 00a0 057c 01a1 0153 007c 017c  !t.....|...S.|.|
+00001350: 006a 0676 0072 2b7c 006a 067c 0119 0053  .j.v.r+|.j.|...S
+00001360: 007c 017c 006a 0776 0072 357c 006a 077c  .|.|.j.v.r5|.j.|
+00001370: 0119 0053 007c 0253 00a9 014e 2908 720f  ...S.|.S...N).r.
+00001380: 0000 0072 1600 0000 7257 0000 0072 5a00  ...r....rW...rZ.
+00001390: 0000 725e 0000 0072 5f00 0000 7202 0000  ..r^...r_...r...
+000013a0: 0072 5d00 0000 2904 7223 0000 0072 2500  .r]...).r#...r%.
+000013b0: 0000 da07 6465 6661 756c 7472 6000 0000  ....defaultr`...
+000013c0: 7261 0000 0072 2700 0000 7228 0000 0072  ra...r'...r(...r
+000013d0: 5f00 0000 fb00 0000 7318 0000 000a 020a  _.......s.......
+000013e0: 010e 0308 0204 0108 020c 010a 040a 010a  ................
+000013f0: 050a 0104 0263 0300 0000 0000 0000 0000  .....c..........
+00001400: 0000 0300 0000 0400 0000 4300 0000 f30c  ..........C.....
+00001410: 0000 007c 00a0 007c 017c 02a1 0253 0072  ...|...|.|...S.r
+00001420: 6300 0000 a901 725f 0000 00a9 0372 2300  c.....r_.....r#.
+00001430: 0000 7225 0000 0072 6400 0000 7227 0000  ..r%...rd...r'..
+00001440: 0072 2700 0000 7228 0000 00da 0867 6574  .r'...r(.....get
+00001450: 5f69 7465 6d16 0100 00f3 0200 0000 0c01  _item...........
+00001460: 7a14 456e 7669 726f 6e6d 656e 742e 6765  z.Environment.ge
+00001470: 745f 6974 656d 6303 0000 0000 0000 0000  t_itemc.........
+00001480: 0000 0003 0000 0004 0000 0043 0000 0072  ...........C...r
+00001490: 6500 0000 7263 0000 0072 6600 0000 7267  e...rc...rf...rg
+000014a0: 0000 0072 2700 0000 7227 0000 0072 2800  ...r'...r'...r(.
+000014b0: 0000 da0a 6765 745f 6870 6172 616d 1901  ....get_hparam..
+000014c0: 0000 7269 0000 007a 1645 6e76 6972 6f6e  ..ri...z.Environ
+000014d0: 6d65 6e74 2e67 6574 5f68 7061 7261 6d63  ment.get_hparamc
+000014e0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+000014f0: 0500 0000 4300 0000 7370 0000 0074 0064  ....C...sp...t.d
+00001500: 017c 006a 019b 009d 0283 0101 0074 0064  .|.j.........t.d
+00001510: 0283 0101 007c 006a 02a0 03a1 0044 005d  .....|.j.....D.]
+00001520: 0d5c 027d 017d 0274 007c 019b 0064 037c  .\.}.}.t.|...d.|
+00001530: 029b 009d 0383 0101 0071 1174 0064 0483  .........q.t.d..
+00001540: 0101 007c 006a 04a0 03a1 0044 005d 0d5c  ...|.j.....D.].\
+00001550: 027d 017d 0274 007c 019b 0064 037c 029b  .}.}.t.|...d.|..
+00001560: 009d 0383 0101 0071 2864 0053 0029 054e  .......q(d.S.).N
+00001570: 7a0c 4578 7065 7269 6d65 6e74 3a20 7a10  z.Experiment: z.
+00001580: 4879 7065 7270 6172 616d 6574 6572 733a  Hyperparameters:
+00001590: 724f 0000 007a 1645 6e76 6972 6f6e 6d65  rO...z.Environme
+000015a0: 6e74 2076 6172 6961 626c 6573 3a29 0572  nt variables:).r
+000015b0: 5100 0000 7220 0000 0072 0f00 0000 7256  Q...r ...r....rV
+000015c0: 0000 0072 0200 0000 2903 7223 0000 0072  ...r....).r#...r
+000015d0: 2500 0000 7226 0000 0072 2700 0000 7227  %...r&...r'...r'
+000015e0: 0000 0072 2800 0000 da0a 7072 696e 745f  ...r(.....print_
+000015f0: 696e 666f 1c01 0000 7310 0000 0010 0208  info....s.......
+00001600: 0212 0114 0108 0212 0114 0104 ff7a 1645  .............z.E
+00001610: 6e76 6972 6f6e 6d65 6e74 2e70 7269 6e74  nvironment.print
+00001620: 5f69 6e66 6f72 6300 0000 290d da08 5f5f  _inforc...)...__
+00001630: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00001640: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00001650: 7229 0000 0072 1c00 0000 7214 0000 0072  r)...r....r....r
+00001660: 2200 0000 7221 0000 0072 5f00 0000 7268  "...r!...r_...rh
+00001670: 0000 0072 6a00 0000 726b 0000 00da 0d5f  ...rj...rk....._
+00001680: 5f63 6c61 7373 6365 6c6c 5f5f 7227 0000  _classcell__r'..
+00001690: 0072 2700 0000 7261 0000 0072 2800 0000  .r'...ra...r(...
+000016a0: 7203 0000 000b 0000 0073 1600 0000 0800  r........s......
+000016b0: 0801 0835 080e 0819 0821 0c4d 0e25 0a1b  ...5.....!.M.%..
+000016c0: 0a03 1003 7203 0000 0029 0872 3700 0000  ....r....).r7...
+000016d0: 7216 0000 0072 4600 0000 7211 0000 00da  r....rF...r.....
+000016e0: 0469 7064 6272 5200 0000 7249 0000 0072  .ipdbrR...rI...r
+000016f0: 0300 0000 7227 0000 0072 2700 0000 7227  ....r'...r'...r'
+00001700: 0000 0072 2800 0000 da08 3c6d 6f64 756c  ...r(.....<modul
+00001710: 653e 0100 0000 730e 0000 0008 0008 0108  e>....s.........
+00001720: 0108 0108 0104 0314 03                   .........
```

### Comparing `yerbamate-0.9.239/packages/yerbamate/__pycache__/mate.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/__pycache__/mate.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr  8 19:56:23 2023 UTC, .py size: 7829 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,517 +1,538 @@
-00000000: 6f0d 0d0a 0000 0000 e7c6 3164 951e 0000  o.........1d....
+00000000: 6f0d 0d0a 0000 0000 fdb4 8e64 5f20 0000  o..........d_ ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 6400 6403 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6401 6c07 5a07 6400 6401 6c08 5a08 6404  d.l.Z.d.d.l.Z.d.
 00000070: 6405 6c09 6d09 5a09 0100 6400 6401 6c0a  d.l.m.Z...d.d.l.
 00000080: 5a0a 6400 6406 6c0b 6d0c 5a0c 0100 4700  Z.d.d.l.m.Z...G.
 00000090: 6407 6408 8400 6408 8302 5a0d 6401 5300  d.d...d...Z.d.S.
 000000a0: 2909 e900 0000 004e 2901 da02 696f 2901  )......N)...io).
 000000b0: da07 4d61 7465 4150 49e9 0100 0000 2901  ..MateAPI.....).
 000000c0: da05 7574 696c 7329 01da 084f 7074 696f  ..utils)...Optio
 000000d0: 6e61 6c63 0000 0000 0000 0000 0000 0000  nalc............
-000000e0: 0000 0000 0600 0000 4000 0000 73c0 0000  ........@...s...
-000000f0: 0065 005a 0164 005a 0264 015a 0364 2864  .e.Z.d.Z.d.Z.d(d
+000000e0: 0000 0000 0600 0000 4000 0000 73c8 0000  ........@...s...
+000000f0: 0065 005a 0164 005a 0264 015a 0364 2a64  .e.Z.d.Z.d.Z.d*d
 00000100: 0364 0484 015a 0465 0564 0565 0666 0264  .d...Z.e.d.e.f.d
 00000110: 0664 0784 0483 015a 0764 0864 0984 005a  .d.....Z.d.d...Z
-00000120: 0809 0a09 0b64 2964 0c65 0664 0d65 0966  .....d)d.e.d.e.f
+00000120: 0809 0a09 0b64 2b64 0c65 0664 0d65 0966  .....d+d.e.d.e.f
 00000130: 0464 0e64 0f84 055a 0a64 1065 0666 0264  .d.d...Z.d.e.f.d
 00000140: 1164 1284 045a 0b64 1364 1484 005a 0c64  .d...Z.d.d...Z.d
 00000150: 1565 0664 1665 0664 1765 0666 0664 1864  .e.d.e.d.e.f.d.d
 00000160: 1984 045a 0d64 1a65 0666 0264 1b64 1c84  ...Z.d.e.f.d.d..
-00000170: 045a 0e64 1d65 0664 1e65 0666 0464 1f64  .Z.d.e.d.e.f.d.d
-00000180: 2084 045a 0f64 1d65 0664 1e65 0666 0464   ..Z.d.e.d.e.f.d
-00000190: 2164 2284 045a 1064 2365 0666 0264 2464  !d"..Z.d#e.f.d$d
-000001a0: 2584 045a 1164 2664 2784 005a 1264 0a53  %..Z.d&d'..Z.d.S
-000001b0: 0029 2ada 044d 6174 657a 310a 2020 2020  .)*..Matez1.    
-000001c0: 4d61 7465 2c20 796f 7572 2066 7269 656e  Mate, your frien
-000001d0: 646c 7920 4d4c 2070 726f 6a65 6374 206d  dly ML project m
-000001e0: 616e 6167 6572 2e0a 2020 2020 4663 0200  anager..    Fc..
-000001f0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000200: 0000 4300 0000 733e 0000 0064 017c 005f  ..C...s>...d.|._
-00000210: 0064 017c 005f 0174 026a 03a0 0474 05a1  .d.|._.t.j...t..
-00000220: 017c 005f 0664 007c 005f 077c 00a0 08a1  .|._.d.|._.|....
-00000230: 0001 0074 097c 006a 0783 017c 005f 0a64  ...t.|.j...|._.d
-00000240: 007c 005f 0b64 0053 0029 024e da00 290c  .|._.d.S.).N..).
-00000250: da0b 726f 6f74 5f66 6f6c 6465 72da 0973  ..root_folder..s
-00000260: 6176 655f 7061 7468 da02 6f73 da04 7061  ave_path..os..pa
-00000270: 7468 da07 6469 726e 616d 65da 085f 5f66  th..dirname..__f
-00000280: 696c 655f 5f5a 0e63 7572 7265 6e74 5f66  ile__Z.current_f
-00000290: 6f6c 6465 72da 0663 6f6e 6669 67da 0f5f  older..config.._
-000002a0: 4d61 7465 5f5f 6669 6e64 726f 6f74 7203  Mate__findrootr.
-000002b0: 0000 00da 0361 7069 5a0a 7275 6e5f 7061  .....apiZ.run_pa
-000002c0: 7261 6d73 2902 da04 7365 6c66 da04 696e  rams)...self..in
-000002d0: 6974 a900 7214 0000 00fa 342f 686f 6d65  it..r.....4/home
-000002e0: 2f61 6c2f 4769 7448 7562 2f79 6572 6261  /al/GitHub/yerba
-000002f0: 6d61 7465 2f70 6163 6b61 6765 732f 7965  mate/packages/ye
-00000300: 7262 616d 6174 652f 6d61 7465 2e70 79da  rbamate/mate.py.
-00000310: 085f 5f69 6e69 745f 5f15 0000 0073 0e00  .__init__....s..
-00000320: 0000 0601 0601 0e01 0601 0801 0c01 0a01  ................
-00000330: 7a0d 4d61 7465 2e5f 5f69 6e69 745f 5fda  z.Mate.__init__.
-00000340: 0c70 726f 6a65 6374 5f6e 616d 6563 0100  .project_namec..
-00000350: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000360: 0000 4f00 0000 731c 0000 0074 006a 017c  ..O...s....t.j.|
-00000370: 0067 017c 01a2 0152 0069 007c 02a4 018e  .g.|...R.i.|....
-00000380: 0101 0064 0153 0029 0261 df01 0000 0a0a  ...d.S.).a......
-00000390: 2020 2020 2020 2020 606d 6174 6520 696e          `mate in
-000003a0: 6974 207b 7072 6f6a 6563 745f 6e61 6d65  it {project_name
-000003b0: 7d60 0a0a 2020 2020 2020 2020 496e 6974  }`..        Init
-000003c0: 6961 6c69 7a65 7320 6120 6e65 7720 7072  ializes a new pr
-000003d0: 6f6a 6563 742e 0a20 2020 2020 2020 2054  oject..        T
-000003e0: 6869 7320 7769 6c6c 2063 7265 6174 6520  his will create 
-000003f0: 7468 6520 666f 6c6c 6f77 696e 6720 7374  the following st
-00000400: 7275 6374 7572 653a 0a20 2020 2020 2020  ructure:.       
-00000410: 2060 6060 0a20 2020 2020 2020 202f 0a20   ```.        /. 
-00000420: 2020 2020 2020 207c 2d2d 206d 6f64 656c         |-- model
-00000430: 732f 0a20 2020 2020 2020 207c 2020 207c  s/.        |   |
-00000440: 2d2d 205f 5f69 6e69 745f 5f2e 7079 0a20  -- __init__.py. 
-00000450: 2020 2020 2020 207c 2d2d 2065 7870 6572         |-- exper
-00000460: 696d 656e 7473 2f0a 2020 2020 2020 2020  iments/.        
-00000470: 7c20 2020 7c2d 2d20 5f5f 696e 6974 5f5f  |   |-- __init__
-00000480: 2e70 790a 2020 2020 2020 2020 7c2d 2d20  .py.        |-- 
-00000490: 7472 6169 6e65 7273 2f0a 2020 2020 2020  trainers/.      
-000004a0: 2020 7c20 2020 7c2d 2d20 5f5f 696e 6974    |   |-- __init
-000004b0: 5f5f 2e70 790a 2020 2020 2020 2020 7c2d  __.py.        |-
-000004c0: 2d20 6461 7461 2f0a 2020 2020 2020 2020  - data/.        
-000004d0: 7c20 2020 7c2d 2d20 5f5f 696e 6974 5f5f  |   |-- __init__
-000004e0: 2e70 790a 2020 2020 2020 2020 6060 600a  .py.        ```.
-000004f0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00000500: 2020 2020 2020 2020 2020 2070 726f 6a65             proje
-00000510: 6374 5f6e 616d 653a 204e 616d 6520 6f66  ct_name: Name of
-00000520: 2074 6865 2070 726f 6a65 6374 2e0a 0a20   the project... 
-00000530: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
-00000540: 0a20 2020 2020 2020 2020 2020 2060 6d61  .            `ma
-00000550: 7465 2069 6e69 7420 6d79 5f70 726f 6a65  te init my_proje
-00000560: 6374 600a 0a20 2020 2020 2020 204e 2902  ct`..        N).
-00000570: 7203 0000 005a 0c69 6e69 745f 7072 6f6a  r....Z.init_proj
-00000580: 6563 7429 0372 1700 0000 da04 6172 6773  ect).r......args
-00000590: da06 6b77 6172 6773 7214 0000 0072 1400  ..kwargsr....r..
-000005a0: 0000 7215 0000 0072 1300 0000 1e00 0000  ..r....r........
-000005b0: 7302 0000 001c 1c7a 094d 6174 652e 696e  s......z.Mate.in
-000005c0: 6974 6301 0000 0000 0000 0000 0000 0001  itc.............
-000005d0: 0000 0003 0000 0043 0000 0073 1000 0000  .......C...s....
-000005e0: 7c00 6a00 a001 6401 a101 0100 6402 5300  |.j...d.....d.S.
-000005f0: 2903 612b 0200 000a 2020 2020 2020 2020  ).a+....        
-00000600: 4765 6e65 7261 7465 7320 7265 7175 6972  Generates requir
-00000610: 656d 656e 7473 2e74 7874 2c20 6465 7065  ements.txt, depe
-00000620: 6e64 656e 6369 6573 2e6a 736f 6e20 616e  ndencies.json an
-00000630: 6420 6578 706f 7274 732e 6d64 2066 6f72  d exports.md for
-00000640: 2073 6861 7269 6e67 2061 6e64 2072 6570   sharing and rep
-00000650: 726f 6475 6369 6269 6c69 7479 2e0a 0a20  roducibility... 
-00000660: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
-00000670: 2020 2020 2020 2020 2020 2020 606d 6174              `mat
-00000680: 6520 6578 706f 7274 600a 0a20 2020 2020  e export`..     
-00000690: 2020 204f 7574 7075 743a 0a20 2020 2020     Output:.     
-000006a0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-000006b0: 2020 2020 2020 2047 656e 6572 6174 6564         Generated
-000006c0: 2072 6571 7569 7265 6d65 6e74 732e 7478   requirements.tx
-000006d0: 7420 666f 7220 6761 6e2f 6d6f 6465 6c73  t for gan/models
-000006e0: 2f6c 6761 6e0a 2020 2020 2020 2020 2020  /lgan.          
-000006f0: 2020 4765 6e65 7261 7465 6420 6465 7065    Generated depe
-00000700: 6e64 656e 6369 6573 2e6a 736f 6e20 666f  ndencies.json fo
-00000710: 7220 6761 6e2f 6578 7065 7269 6d65 6e74  r gan/experiment
-00000720: 732f 6c77 6761 6e0a 2020 2020 2020 2020  s/lwgan.        
-00000730: 2020 2020 4765 6e65 7261 7465 6420 7265      Generated re
-00000740: 7175 6972 656d 656e 7473 2e74 7874 2066  quirements.txt f
-00000750: 6f72 2067 616e 2f65 7870 6572 696d 656e  or gan/experimen
-00000760: 7473 2f6c 7767 616e 0a20 2020 2020 2020  ts/lwgan.       
-00000770: 2020 2020 2047 656e 6572 6174 6564 2072       Generated r
-00000780: 6571 7569 7265 6d65 6e74 732e 7478 7420  equirements.txt 
-00000790: 666f 7220 6761 6e2f 7472 6169 6e65 7273  for gan/trainers
-000007a0: 2f6c 6761 6e0a 2020 2020 2020 2020 2020  /lgan.          
-000007b0: 2020 4765 6e65 7261 7465 6420 7265 7175    Generated requ
-000007c0: 6972 656d 656e 7473 2e74 7874 2066 6f72  irements.txt for
-000007d0: 2067 616e 2f64 6174 612f 6361 7273 0a20   gan/data/cars. 
-000007e0: 2020 2020 2020 2020 2020 2045 7870 6f72             Expor
-000007f0: 7465 6420 746f 2065 7870 6f72 742e 6d64  ted to export.md
-00000800: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-00000810: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000820: 2020 da06 6578 706f 7274 4ea9 0272 1100    ..exportN..r..
-00000830: 0000 da04 6175 746f a901 7212 0000 0072  ....auto..r....r
-00000840: 1400 0000 7214 0000 0072 1500 0000 721a  ....r....r....r.
-00000850: 0000 003c 0000 00f3 0200 0000 1012 7a0b  ...<..........z.
-00000860: 4d61 7465 2e65 7870 6f72 744e 54da 0b6d  Mate.exportNT..m
-00000870: 6f64 756c 655f 6e61 6d65 da0b 6f75 7470  odule_name..outp
-00000880: 7574 5f6a 736f 6e63 0300 0000 0000 0000  ut_jsonc........
-00000890: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
-000008a0: 7332 0000 007c 006a 00a0 017c 01a1 017d  s2...|.j...|...}
-000008b0: 037c 0272 1374 0274 036a 047c 0364 0164  .|.r.t.t.j.|.d.d
-000008c0: 028d 0283 0101 0064 0353 0074 027c 0383  .......d.S.t.|..
-000008d0: 0101 0064 0353 0029 047a ee0a 0a0a 2020  ...d.S.).z....  
-000008e0: 2020 2020 2020 4c69 7374 7320 616c 6c20        Lists all 
-000008f0: 6176 6169 6c61 626c 6520 6d6f 6475 6c65  available module
-00000900: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
-00000910: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
-00000920: 6475 6c65 5f6e 616d 653a 204e 616d 6520  dule_name: Name 
-00000930: 6f66 2074 6865 206d 6f64 756c 6520 746f  of the module to
-00000940: 206c 6973 742e 2049 6620 6e6f 7420 7370   list. If not sp
-00000950: 6563 6966 6965 642c 2061 6c6c 206d 6f64  ecified, all mod
-00000960: 756c 6573 2077 696c 6c20 6265 206c 6973  ules will be lis
-00000970: 7465 642e 0a0a 2020 2020 2020 2020 4578  ted...        Ex
-00000980: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-00000990: 2020 2020 606d 6174 6520 6c69 7374 206d      `mate list m
-000009a0: 6f64 656c 7360 0a0a 2020 2020 2020 2020  odels`..        
-000009b0: 2020 2020 606d 6174 6520 6c69 7374 600a      `mate list`.
-000009c0: 0a20 2020 2020 2020 20e9 0400 0000 a901  .        .......
-000009d0: da06 696e 6465 6e74 4e29 0572 1100 0000  ..indentN).r....
-000009e0: da04 6c69 7374 da05 7072 696e 74da 046a  ..list..print..j
-000009f0: 736f 6eda 0564 756d 7073 2904 7212 0000  son..dumps).r...
-00000a00: 0072 1f00 0000 7220 0000 00da 026c 6972  .r....r .....lir
-00000a10: 1400 0000 7214 0000 0072 1500 0000 7224  ....r....r....r$
-00000a20: 0000 0050 0000 0073 0800 0000 0c14 0401  ...P...s........
-00000a30: 1601 0c02 7a09 4d61 7465 2e6c 6973 74da  ....z.Mate.list.
-00000a40: 0763 6f6d 6d61 6e64 6302 0000 0000 0000  .commandc.......
-00000a50: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00000a60: 0073 1000 0000 7c00 6a00 a001 7c01 a101  .s....|.j...|...
-00000a70: 0100 6401 5300 2902 618e 0100 000a 0a20  ..d.S.).a...... 
-00000a80: 2020 2020 2020 2060 6d61 7465 2061 7574         `mate aut
-00000a90: 6f20 7b63 6f6d 6d61 6e64 7d60 0a0a 2020  o {command}`..  
-00000aa0: 2020 2020 2020 5661 7269 6f75 7320 636f        Various co
-00000ab0: 6d6d 616e 6473 2074 6f20 6865 6c70 2077  mmands to help w
-00000ac0: 6974 6820 7468 6520 6465 7665 6c6f 706d  ith the developm
-00000ad0: 656e 7420 7072 6f63 6573 732e 0a0a 0a20  ent process.... 
-00000ae0: 2020 2020 2020 2063 6f6d 6d61 6e64 733a         commands:
-00000af0: 0a20 2020 2020 2020 202d 2060 6578 706f  .        - `expo
-00000b00: 7274 603a 2043 7265 6174 6573 2061 2072  rt`: Creates a r
-00000b10: 6571 7569 7265 6d65 6e74 732e 7478 7420  equirements.txt 
-00000b20: 616e 6420 6465 7065 6e64 656e 6369 6573  and dependencies
-00000b30: 2e6a 736f 6e20 6669 6c65 7320 666f 7220  .json files for 
-00000b40: 7368 6172 696e 6720 616e 6420 7265 7072  sharing and repr
-00000b50: 6f64 7563 6962 696c 6974 792e 0a20 2020  oducibility..   
-00000b60: 2020 2020 202d 2060 696e 6974 603a 2041       - `init`: A
-00000b70: 7574 6f6d 6174 6963 616c 6c79 2063 7265  utomatically cre
-00000b80: 6174 6573 2060 5f5f 696e 6974 5f5f 2e70  ates `__init__.p
-00000b90: 7960 2066 696c 6573 2069 6e20 7468 6520  y` files in the 
-00000ba0: 7072 6f6a 6563 7420 7374 7275 6374 7572  project structur
-00000bb0: 652e 0a0a 2020 2020 2020 2020 4578 616d  e...        Exam
-00000bc0: 706c 653a 0a0a 0a20 2020 2020 2020 2020  ple:...         
-00000bd0: 2020 2060 6d61 7465 2061 7574 6f20 6578     `mate auto ex
-00000be0: 706f 7274 600a 2020 2020 2020 2020 2020  port`.          
-00000bf0: 2020 606d 6174 6520 6175 746f 2069 6e69    `mate auto ini
-00000c00: 7460 0a20 2020 2020 2020 204e 721b 0000  t`.        Nr...
-00000c10: 0029 0272 1200 0000 7229 0000 0072 1400  .).r....r)...r..
-00000c20: 0000 7214 0000 0072 1500 0000 721c 0000  ..r....r....r...
-00000c30: 006a 0000 0072 1e00 0000 7a09 4d61 7465  .j...r....z.Mate
-00000c40: 2e61 7574 6f63 0100 0000 0000 0000 0000  .autoc..........
-00000c50: 0000 0100 0000 0500 0000 4300 0000 731c  ..........C...s.
-00000c60: 0000 0074 0074 016a 027c 006a 03a0 04a1  ...t.t.j.|.j....
-00000c70: 0064 0164 028d 0283 0101 0064 0353 0029  .d.d.......d.S.)
-00000c80: 047a 4e0a 2020 2020 2020 2020 5072 696e  .zN.        Prin
-00000c90: 7473 2061 2073 756d 6d61 7279 206f 6620  ts a summary of 
-00000ca0: 7468 6520 7072 6f6a 6563 7420 6d6f 6475  the project modu
-00000cb0: 6c65 732e 2053 616d 6520 6173 2060 6d61  les. Same as `ma
-00000cc0: 7465 206c 6973 7460 0a20 2020 2020 2020  te list`.       
-00000cd0: 2072 2100 0000 7222 0000 004e 2905 7225   r!...r"...N).r%
-00000ce0: 0000 0072 2600 0000 7227 0000 0072 1100  ...r&...r'...r..
-00000cf0: 0000 da07 7375 6d6d 6172 7972 1d00 0000  ....summaryr....
-00000d00: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-00000d10: 2a00 0000 7e00 0000 7302 0000 001c 057a  *...~...s......z
-00000d20: 0c4d 6174 652e 7375 6d6d 6172 79da 066d  .Mate.summary..m
-00000d30: 6f64 756c 65da 046e 616d 65da 0464 6573  odule..name..des
-00000d40: 7463 0400 0000 0000 0000 0000 0000 0900  tc..............
-00000d50: 0000 0700 0000 4f00 0000 73ec 0000 0074  ......O...s....t
-00000d60: 006a 01a0 027c 006a 037c 017c 02a1 037d  .j...|.j.|.|...}
-00000d70: 0674 006a 01a0 047c 06a1 0173 1f74 0564  .t.j...|...s.t.d
-00000d80: 017c 019b 0064 027c 029b 0064 039d 0583  .|...d.|...d....
-00000d90: 0101 0074 06a0 0764 04a1 0101 0074 006a  ...t...d.....t.j
-00000da0: 01a0 027c 006a 037c 017c 03a1 037d 0774  ...|.j.|.|...}.t
-00000db0: 006a 01a0 047c 07a1 0172 6164 057c 0476  .j...|...rad.|.v
-00000dc0: 0072 3f74 08a0 097c 07a1 0101 0074 0564  .r?t...|.....t.d
-00000dd0: 067c 079b 009d 0283 0101 006e 2274 0564  .|.........n"t.d
-00000de0: 077c 039b 0064 089d 0383 0101 0074 0a64  .|...d.......t.d
-00000df0: 0983 017d 087c 0864 0a6b 0272 5c74 08a0  ...}.|.d.k.r\t..
-00000e00: 097c 07a1 0101 0074 0564 067c 079b 009d  .|.....t.d.|....
-00000e10: 0283 0101 006e 0574 06a0 0764 04a1 0101  .....n.t...d....
-00000e20: 0074 08a0 0b7c 067c 07a1 0201 0074 0564  .t...|.|.....t.d
-00000e30: 017c 019b 0064 027c 029b 0064 0b7c 079b  .|...d.|...d.|..
-00000e40: 009d 0683 0101 0064 0c53 0029 0d61 8a01  .......d.S.).a..
-00000e50: 0000 0a20 2020 2020 2020 2060 6d61 7465  ...        `mate
-00000e60: 2063 6c6f 6e65 207b 6d6f 6475 6c65 7d20   clone {module} 
-00000e70: 7b6e 616d 657d 207b 6465 7374 7d20 7b2d  {name} {dest} {-
-00000e80: 6f7d 600a 0a20 2020 2020 2020 2043 6c6f  o}`..        Clo
-00000e90: 6e65 7320 6120 736f 7572 6365 2063 6f64  nes a source cod
-00000ea0: 6520 6d6f 6475 6c65 2074 6f20 6120 6e65  e module to a ne
-00000eb0: 7720 6465 7374 696e 6174 696f 6e2e 0a0a  w destination...
-00000ec0: 2020 2020 2020 2020 4172 6773 3a0a 0a20          Args:.. 
-00000ed0: 2020 2020 2020 2020 2020 206d 6f64 756c             modul
-00000ee0: 653a 204d 6f64 756c 6520 746f 2063 6c6f  e: Module to clo
-00000ef0: 6e65 2e0a 0a20 2020 2020 2020 2020 2020  ne...           
-00000f00: 206e 616d 653a 204e 616d 6520 6f66 2074   name: Name of t
-00000f10: 6865 206d 6f64 756c 6520 746f 2063 6c6f  he module to clo
-00000f20: 6e65 2e0a 0a20 2020 2020 2020 2020 2020  ne...           
-00000f30: 2064 6573 743a 2044 6573 7469 6e61 7469   dest: Destinati
-00000f40: 6f6e 2074 6f20 636c 6f6e 6520 7468 6520  on to clone the 
-00000f50: 6d6f 6475 6c65 2074 6f2e 0a0a 2020 2020  module to...    
-00000f60: 2020 2020 2020 2020 2d6f 3a20 4f76 6572          -o: Over
-00000f70: 7772 6974 6520 6465 7374 696e 6174 696f  write destinatio
-00000f80: 6e20 6966 2069 7420 6578 6973 7473 2e0a  n if it exists..
-00000f90: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-00000fa0: 3a0a 0a20 2020 2020 2020 2020 2020 2060  :..            `
-00000fb0: 6d61 7465 2063 6c6f 6e65 206d 6f64 656c  mate clone model
-00000fc0: 7320 746f 7263 685f 7669 7420 6d79 5f76  s torch_vit my_v
-00000fd0: 6974 600a 2020 2020 2020 2020 7a07 4d6f  it`.        z.Mo
-00000fe0: 6475 6c65 20fa 012f 7a0f 2064 6f65 7320  dule ../z. does 
-00000ff0: 6e6f 7420 6578 6973 7472 0400 0000 7a02  not existr....z.
-00001000: 2d6f 7a08 5265 6d6f 7665 6420 7a0c 4465  -oz.Removed z.De
-00001010: 7374 696e 6174 696f 6e20 7a07 2065 7869  stination z. exi
-00001020: 7374 737a 124f 7665 7277 7269 7465 3f20  stsz.Overwrite? 
-00001030: 2879 2f6e 293a 20da 0179 7a0b 2063 6c6f  (y/n): ..yz. clo
-00001040: 6e65 6420 746f 204e 290c 720b 0000 0072  ned to N).r....r
-00001050: 0c00 0000 da04 6a6f 696e 7209 0000 00da  ......joinr.....
-00001060: 0665 7869 7374 7372 2500 0000 da03 7379  .existsr%.....sy
-00001070: 73da 0465 7869 74da 0673 6875 7469 6cda  s..exit..shutil.
-00001080: 0672 6d74 7265 65da 0569 6e70 7574 da08  .rmtree..input..
-00001090: 636f 7079 7472 6565 2909 7212 0000 0072  copytree).r....r
-000010a0: 2b00 0000 722c 0000 0072 2d00 0000 7218  +...r,...r-...r.
-000010b0: 0000 0072 1900 0000 da0b 6d6f 6475 6c65  ...r......module
-000010c0: 5f70 6174 685a 0964 6573 745f 7061 7468  _pathZ.dest_path
-000010d0: da09 6f76 6572 7772 6974 6572 1400 0000  ..overwriter....
-000010e0: 7214 0000 0072 1500 0000 da05 636c 6f6e  r....r......clon
-000010f0: 6585 0000 0073 2200 0000 1216 0c01 1601  e....s".........
-00001100: 0a01 1203 0c01 0802 0a01 1001 1002 0801  ................
-00001110: 0801 0a01 1001 0a02 0c03 1e02 7a0a 4d61  ............z.Ma
-00001120: 7465 2e63 6c6f 6e65 da0a 6d6f 6465 6c5f  te.clone..model_
-00001130: 6e61 6d65 6302 0000 0000 0000 0000 0000  namec...........
-00001140: 0002 0000 0001 0000 0043 0000 0073 0400  .........C...s..
-00001150: 0000 6400 5300 2901 4e72 1400 0000 2902  ..d.S.).Nr....).
-00001160: 7212 0000 0072 3b00 0000 7214 0000 0072  r....r;...r....r
-00001170: 1400 0000 7215 0000 00da 0873 6e61 7073  ....r......snaps
-00001180: 686f 74b5 0000 0073 0200 0000 0401 7a0d  hot....s......z.
-00001190: 4d61 7465 2e73 6e61 7073 686f 74da 0a65  Mate.snapshot..e
-000011a0: 7870 5f6d 6f64 756c 65da 0365 7870 6303  xp_module..expc.
-000011b0: 0000 0000 0000 0000 0000 0007 0000 000a  ................
-000011c0: 0000 004f 0000 0073 8800 0000 7c00 6a00  ...O...s....|.j.
-000011d0: 6a01 6401 7c01 7c02 6704 7d05 6402 a002  j.d.|.|.g.}.d...
-000011e0: 7c05 a101 7d05 7a07 7403 7c05 8301 0100  |...}.z.t.|.....
-000011f0: 5700 6407 5300 0400 7404 7943 0100 7d06  W.d.S...t.yC..}.
-00001200: 0100 7a23 7405 6403 7c01 9b00 6404 7c02  ..z#t.d.|...d.|.
-00001210: 9b00 9d04 8301 0100 7405 6405 8301 0100  ........t.d.....
-00001220: 7c00 a006 6401 a101 0100 7407 a008 a100  |...d.....t.....
-00001230: 0100 7409 a00a 6406 a101 0100 5700 5900  ..t...d.....W.Y.
-00001240: 6407 7d06 7e06 6407 5300 6407 7d06 7e06  d.}.~.d.S.d.}.~.
-00001250: 7701 7700 2908 61e0 0100 000a 2020 2020  w.w.).a.....    
-00001260: 2020 2020 4578 6563 7574 6573 2061 6e20      Executes an 
-00001270: 6578 7065 7269 6d65 6e74 2e0a 0a20 2020  experiment...   
-00001280: 2020 2020 2055 7361 6765 3a20 6060 6d61       Usage: ``ma
-00001290: 7465 2074 7261 696e 207b 6d6f 6475 6c65  te train {module
-000012a0: 7d20 7b65 7870 6572 696d 656e 747d 6060  } {experiment}``
-000012b0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-000012c0: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-000012d0: 5f6d 6f64 756c 653a 204e 616d 6520 6f66  _module: Name of
-000012e0: 2074 6865 206d 6f64 756c 6520 7768 6572   the module wher
-000012f0: 6520 7468 6520 6578 7065 7269 6d65 6e74  e the experiment
-00001300: 2069 7320 6c6f 6361 7465 642e 0a0a 2020   is located...  
-00001310: 2020 2020 2020 2020 2020 6578 703a 204e            exp: N
-00001320: 616d 6520 6f66 2074 6865 2065 7870 6572  ame of the exper
-00001330: 696d 656e 742e 0a0a 2020 2020 2020 2020  iment...        
-00001340: 4578 616d 706c 653a 0a20 2020 2020 2020  Example:.       
-00001350: 2020 2020 2060 0a20 2020 2020 2020 2020       `.         
-00001360: 2020 206d 6174 6520 7472 6169 6e20 6578     mate train ex
-00001370: 7065 7269 6d65 6e74 7320 6d79 5f65 7870  periments my_exp
-00001380: 6572 696d 656e 7460 0a0a 2020 2020 2020  eriment`..      
-00001390: 2020 5468 6973 2077 696c 6c20 7275 6e20    This will run 
-000013a0: 7468 6520 6578 7065 7269 6d65 6e74 2060  the experiment `
-000013b0: 6d79 5f65 7870 6572 696d 656e 7460 206c  my_experiment` l
-000013c0: 6f63 6174 6564 2069 6e20 7468 6520 6065  ocated in the `e
-000013d0: 7870 6572 696d 656e 7473 6020 6d6f 6475  xperiments` modu
-000013e0: 6c65 2e0a 0a20 2020 2020 2020 2045 7175  le...        Equ
-000013f0: 6976 616c 656e 7420 746f 2060 7079 7468  ivalent to `pyth
-00001400: 6f6e 202d 6d20 726f 6f74 5f6d 6f64 756c  on -m root_modul
-00001410: 652e 6578 7065 7269 6d65 6e74 732e 6d79  e.experiments.my
-00001420: 5f65 7870 6572 696d 656e 7420 7472 6169  _experiment trai
-00001430: 6e60 0a20 2020 2020 2020 20da 0b65 7870  n`.        ..exp
-00001440: 6572 696d 656e 7473 da01 2e7a 1145 7272  eriments...z.Err
-00001450: 6f72 2069 6e20 6c6f 6164 696e 6720 722e  or in loading r.
-00001460: 0000 007a 1641 7661 696c 6162 6c65 2065  ...z.Available e
-00001470: 7870 6572 696d 656e 7473 3a72 0400 0000  xperiments:r....
-00001480: 4e29 0b72 0f00 0000 da07 7072 6f6a 6563  N).r......projec
-00001490: 7472 3000 0000 da0a 5f5f 696d 706f 7274  tr0.....__import
-000014a0: 5f5f da09 4578 6365 7074 696f 6e72 2500  __..Exceptionr%.
-000014b0: 0000 7224 0000 00da 0974 7261 6365 6261  ..r$.....traceba
-000014c0: 636b da09 7072 696e 745f 6578 6372 3200  ck..print_excr2.
-000014d0: 0000 7233 0000 0029 0772 1200 0000 723d  ..r3...).r....r=
-000014e0: 0000 0072 3e00 0000 7218 0000 0072 1900  ...r>...r....r..
-000014f0: 0000 722b 0000 00da 0165 7214 0000 0072  ..r+.....er....r
-00001500: 1400 0000 7215 0000 00da 0574 7261 696e  ....r......train
-00001510: b800 0000 7318 0000 0010 160a 0102 020e  ....s...........
-00001520: 010e 0114 0108 010a 0108 0118 0308 8002  ................
-00001530: f97a 0a4d 6174 652e 7472 6169 6e63 0300  .z.Mate.trainc..
-00001540: 0000 0000 0000 0000 0000 0500 0000 0400  ................
-00001550: 0000 4f00 0000 731e 0000 007c 006a 007c  ..O...s....|.j.|
-00001560: 017c 0267 027c 03a2 0152 0069 007c 04a4  .|.g.|...R.i.|..
-00001570: 018e 0101 0064 0153 0029 0261 dd01 0000  .....d.S.).a....
-00001580: 0a20 2020 2020 2020 2045 7865 6375 7465  .        Execute
-00001590: 7320 616e 2065 7870 6572 696d 656e 742e  s an experiment.
-000015a0: 0a0a 2020 2020 2020 2020 5573 6167 653a  ..        Usage:
-000015b0: 2060 606d 6174 6520 7465 7374 207b 6d6f   ``mate test {mo
-000015c0: 6475 6c65 7d20 7b65 7870 6572 696d 656e  dule} {experimen
-000015d0: 747d 6060 0a0a 2020 2020 2020 2020 4172  t}``..        Ar
-000015e0: 6773 3a0a 0a20 2020 2020 2020 2020 2020  gs:..           
-000015f0: 2065 7870 5f6d 6f64 756c 653a 204e 616d   exp_module: Nam
-00001600: 6520 6f66 2074 6865 206d 6f64 756c 6520  e of the module 
-00001610: 7768 6572 6520 7468 6520 6578 7065 7269  where the experi
-00001620: 6d65 6e74 2069 7320 6c6f 6361 7465 642e  ment is located.
-00001630: 0a0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-00001640: 703a 204e 616d 6520 6f66 2074 6865 2065  p: Name of the e
-00001650: 7870 6572 696d 656e 742e 0a0a 2020 2020  xperiment...    
-00001660: 2020 2020 4578 616d 706c 653a 0a20 2020      Example:.   
-00001670: 2020 2020 2020 2020 2060 0a20 2020 2020           `.     
-00001680: 2020 2020 2020 206d 6174 6520 7465 7374         mate test
-00001690: 2065 7870 6572 696d 656e 7473 206d 795f   experiments my_
-000016a0: 6578 7065 7269 6d65 6e74 600a 0a20 2020  experiment`..   
-000016b0: 2020 2020 2054 6869 7320 7769 6c6c 2072       This will r
-000016c0: 756e 2074 6865 2065 7870 6572 696d 656e  un the experimen
-000016d0: 7420 606d 795f 6578 7065 7269 6d65 6e74  t `my_experiment
-000016e0: 6020 6c6f 6361 7465 6420 696e 2074 6865  ` located in the
-000016f0: 2060 6578 7065 7269 6d65 6e74 7360 206d   `experiments` m
-00001700: 6f64 756c 652e 0a0a 2020 2020 2020 2020  odule...        
-00001710: 4571 7569 7661 6c65 6e74 2074 6f20 6070  Equivalent to `p
-00001720: 7974 686f 6e20 2d6d 2072 6f6f 745f 6d6f  ython -m root_mo
-00001730: 6475 6c65 2e65 7870 6572 696d 656e 7473  dule.experiments
-00001740: 2e6d 795f 6578 7065 7269 6d65 6e74 2074  .my_experiment t
-00001750: 6573 7460 0a20 2020 2020 2020 204e 2901  est`.        N).
-00001760: 7247 0000 0029 0572 1200 0000 723d 0000  rG...).r....r=..
-00001770: 0072 3e00 0000 7218 0000 0072 1900 0000  .r>...r....r....
-00001780: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00001790: 0474 6573 74dc 0000 0073 0200 0000 1e14  .test....s......
-000017a0: 7a09 4d61 7465 2e74 6573 74da 0375 726c  z.Mate.test..url
-000017b0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-000017c0: 0004 0000 004f 0000 0073 1e00 0000 7c00  .....O...s....|.
-000017d0: 6a00 6a01 7c01 6701 7c02 a201 5200 6900  j.j.|.g.|...R.i.
-000017e0: 7c03 a401 8e01 0100 6401 5300 2902 6169  |.......d.S.).ai
-000017f0: 0500 000a 2020 2020 2020 2020 496e 7461  ....        Inta
-00001800: 6c6c 7320 6120 6d6f 6475 6c65 2066 726f  lls a module fro
-00001810: 6d20 6120 6769 7420 7265 706f 7369 746f  m a git reposito
-00001820: 7279 2e0a 0a20 2020 2020 2020 2055 7361  ry...        Usa
-00001830: 6765 3a20 6060 6d61 7465 2069 6e73 7461  ge: ``mate insta
-00001840: 6c6c 207b 7572 6c7d 202d 7b79 7c6e 7c6f  ll {url} -{y|n|o
-00001850: 7d20 7b70 6d7d 6060 0a0a 2020 2020 2020  } {pm}``..      
-00001860: 2020 496e 7374 616c 6c20 6d6f 6475 6c65    Install module
-00001870: 2073 7570 706f 7274 2074 6865 2066 6f6c   support the fol
-00001880: 6c6f 7769 6e67 2066 6f72 6d61 7473 3a0a  lowing formats:.
-00001890: 2020 2020 2020 2020 2d20 6060 6d61 7465          - ``mate
-000018a0: 2069 6e73 7461 6c6c 207b 636f 6d70 6c65   install {comple
-000018b0: 7465 5f75 726c 7d60 600a 2020 2020 2020  te_url}``.      
-000018c0: 2020 2d20 6060 6d61 7465 2069 6e73 7461    - ``mate insta
-000018d0: 6c6c 207b 7573 6572 7d2f 7b72 6570 6f7d  ll {user}/{repo}
-000018e0: 2f7b 726f 6f74 5f6d 6f64 756c 657d 2f7b  /{root_module}/{
-000018f0: 6d6f 6475 6c65 7d60 600a 2020 2020 2020  module}``.      
-00001900: 2020 2d20 6060 6d61 7465 2069 6e73 7461    - ``mate insta
-00001910: 6c6c 207b 7573 6572 7d2f 7b72 6570 6f7c  ll {user}/{repo|
-00001920: 726f 6f74 5f6d 6f64 756c 657d 2f7b 6d6f  root_module}/{mo
-00001930: 6475 6c65 7d60 600a 0a20 2020 2020 2020  dule}``..       
-00001940: 2041 7267 733a 0a20 2020 2020 2020 202d   Args:.        -
-00001950: 2020 2020 7572 6c3a 2055 726c 206f 6620      url: Url of 
-00001960: 7468 6520 6769 7420 7265 706f 7369 746f  the git reposito
-00001970: 7279 2e0a 2020 2020 2020 2020 2d20 2020  ry..        -   
-00001980: 202d 793a 2053 6b69 7073 2063 6f6e 6669   -y: Skips confi
-00001990: 726d 6174 696f 6e20 616e 6420 696e 7374  rmation and inst
-000019a0: 616c 6c73 2070 7974 686f 6e20 6465 7065  alls python depe
-000019b0: 6e64 656e 6369 6573 0a20 2020 2020 2020  ndencies.       
-000019c0: 202d 2020 2020 2d6e 3a20 536b 6970 7320   -    -n: Skips 
-000019d0: 696e 7374 616c 6c69 6e67 2070 7974 686f  installing pytho
-000019e0: 6e20 6465 7065 6e64 656e 6369 6573 0a20  n dependencies. 
-000019f0: 2020 2020 2020 202d 2020 2020 2d6f 3a20         -    -o: 
-00001a00: 4f76 6572 7772 6974 6573 2065 7869 7374  Overwrites exist
-00001a10: 696e 6720 636f 6465 206d 6f64 756c 6573  ing code modules
-00001a20: 0a20 2020 2020 2020 202d 2020 2020 706d  .        -    pm
-00001a30: 3a20 5061 636b 6167 6520 6d61 6e61 6765  : Package manage
-00001a40: 7220 746f 2075 7365 2e20 4465 6661 756c  r to use. Defaul
-00001a50: 7473 2074 6f20 6173 6b69 6e67 2074 6865  ts to asking the
-00001a60: 2075 7365 722e 0a0a 2020 2020 2020 2020   user...        
-00001a70: 4578 616d 706c 6520 496e 7374 616c 6c69  Example Installi
-00001a80: 6e67 2061 206d 6f64 756c 6520 6672 6f6d  ng a module from
-00001a90: 2073 7472 7563 7475 7265 6420 6769 7420   structured git 
-00001aa0: 7265 706f 7369 746f 7279 2028 7265 636f  repository (reco
-00001ab0: 6d6d 656e 6465 6429 3a0a 0a0a 2020 2020  mmended):...    
-00001ac0: 2020 2020 2020 2020 6d61 7465 2069 6e73          mate ins
-00001ad0: 7461 6c6c 206f 616c 6565 2f64 6565 702d  tall oalee/deep-
-00001ae0: 7669 7369 6f6e 2f64 6565 706e 6574 2f6d  vision/deepnet/m
-00001af0: 6f64 656c 732f 746f 7263 685f 7669 7420  odels/torch_vit 
-00001b00: 2d79 6f20 7069 700a 0a20 2020 2020 2020  -yo pip..       
-00001b10: 2020 2020 2054 6869 7320 7769 6c6c 2069       This will i
-00001b20: 6e73 7461 6c6c 2074 6865 206d 6f64 756c  nstall the modul
-00001b30: 6520 6074 6f72 6368 5f76 6974 6020 6672  e `torch_vit` fr
-00001b40: 6f6d 2074 6865 2072 6570 6f73 6974 6f72  om the repositor
-00001b50: 7920 606f 616c 6565 2f64 6565 702d 7669  y `oalee/deep-vi
-00001b60: 7369 6f6e 6020 696e 2074 6f20 796f 7572  sion` in to your
-00001b70: 2060 6d6f 6465 6c73 6020 666f 6c64 6572   `models` folder
-00001b80: 2e0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00001b90: 6520 6079 6f60 2066 6c61 6773 2077 696c  e `yo` flags wil
-00001ba0: 6c20 736b 6970 2063 6f6e 6669 726d 6174  l skip confirmat
-00001bb0: 696f 6e20 616e 6420 696e 7374 616c 6c20  ion and install 
-00001bc0: 7079 7468 6f6e 2064 6570 656e 6465 6e63  python dependenc
-00001bd0: 6965 7320 7573 696e 6720 7069 702e 0a0a  ies using pip...
-00001be0: 2020 2020 2020 2020 4578 616d 706c 6520          Example 
-00001bf0: 496e 7374 616c 6c69 6e67 2061 206d 6f64  Installing a mod
-00001c00: 756c 6520 6672 6f6d 2075 6e73 7472 7563  ule from unstruc
-00001c10: 7475 7265 6420 6769 7420 7265 706f 7369  tured git reposi
-00001c20: 746f 7279 3a0a 0a0a 2020 2020 2020 2020  tory:...        
-00001c30: 2020 2020 6d61 7465 2069 6e73 7461 6c6c      mate install
-00001c40: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00001c50: 636f 6d2f 7277 6967 6874 6d61 6e2f 7079  com/rwightman/py
-00001c60: 746f 7263 682d 696d 6167 652d 6d6f 6465  torch-image-mode
-00001c70: 6c73 2f74 7265 652f 6d61 696e 2f74 696d  ls/tree/main/tim
-00001c80: 6d0a 0a0a 2020 2020 2020 2020 2020 2020  m...            
-00001c90: 5468 6973 2077 696c 6c20 696e 7374 616c  This will instal
-00001ca0: 6c20 7468 6520 6d6f 6475 6c65 2060 7469  l the module `ti
-00001cb0: 6d6d 6020 6672 6f6d 2074 6865 2072 6570  mm` from the rep
-00001cc0: 6f73 6974 6f72 7920 6173 2061 2073 6973  ository as a sis
-00001cd0: 7465 7220 6d6f 6475 6c65 2074 6f20 796f  ter module to yo
-00001ce0: 7572 2072 6f6f 7420 6d6f 6475 6c65 2e0a  ur root module..
-00001cf0: 2020 2020 2020 2020 2020 2020 5461 6b65              Take
-00001d00: 2069 6e74 6f20 6163 636f 756e 7420 7468   into account th
-00001d10: 6174 2074 6869 7320 7769 6c6c 2069 6e73  at this will ins
-00001d20: 7461 6c6c 206f 6e6c 7920 7468 6520 636f  tall only the co
-00001d30: 6465 2061 6e64 206e 6f74 2074 6865 2070  de and not the p
-00001d40: 7974 686f 6e20 6465 7065 6e64 656e 6369  ython dependenci
-00001d50: 6573 2e0a 2020 2020 2020 2020 4e29 0272  es..        N).r
-00001d60: 1100 0000 5a0b 696e 7374 616c 6c5f 7572  ....Z.install_ur
-00001d70: 6c29 0472 1200 0000 7249 0000 0072 1800  l).r....rI...r..
-00001d80: 0000 7219 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00001d90: 0072 1500 0000 da07 696e 7374 616c 6cf2  .r......install.
-00001da0: 0000 0073 0200 0000 1e23 7a0c 4d61 7465  ...s.....#z.Mate
-00001db0: 2e69 6e73 7461 6c6c 6301 0000 0000 0000  .installc.......
-00001dc0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00001dd0: 0073 1400 0000 7400 a001 a100 5c02 7c00  .s....t.....\.|.
-00001de0: 5f02 7c00 5f03 6401 5300 2902 7a71 0a20  _.|._.d.S.).zq. 
-00001df0: 2020 2020 2020 204d 6574 686f 6420 696e         Method in
-00001e00: 2063 6861 7267 6520 6f66 2066 696e 6469   charge of findi
-00001e10: 6e67 2074 6865 2072 6f6f 7420 666f 6c64  ng the root fold
-00001e20: 6572 206f 6620 7468 6520 7072 6f6a 6563  er of the projec
-00001e30: 7420 616e 6420 7265 6164 696e 6720 7468  t and reading th
-00001e40: 6520 636f 6e74 656e 7420 6f66 206d 6174  e content of mat
-00001e50: 652e 6a73 6f6e 0a20 2020 2020 2020 204e  e.json.        N
-00001e60: 2904 7202 0000 005a 0966 696e 645f 726f  ).r....Z.find_ro
-00001e70: 6f74 7209 0000 0072 0f00 0000 721d 0000  otr....r....r...
-00001e80: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
-00001e90: 5a0a 5f5f 6669 6e64 726f 6f74 1701 0000  Z.__findroot....
-00001ea0: 7302 0000 0014 047a 0f4d 6174 652e 5f5f  s......z.Mate.__
-00001eb0: 6669 6e64 726f 6f74 2901 4629 024e 5429  findroot).F).NT)
-00001ec0: 13da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00001ed0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001ee0: 616d 655f 5fda 075f 5f64 6f63 5f5f 7216  ame__..__doc__r.
-00001ef0: 0000 00da 0c73 7461 7469 636d 6574 686f  .....staticmetho
-00001f00: 64da 0373 7472 7213 0000 0072 1a00 0000  d..strr....r....
-00001f10: da04 626f 6f6c 7224 0000 0072 1c00 0000  ..boolr$...r....
-00001f20: 722a 0000 0072 3a00 0000 723c 0000 0072  r*...r:...r<...r
-00001f30: 4700 0000 7248 0000 0072 4a00 0000 7210  G...rH...rJ...r.
-00001f40: 0000 0072 1400 0000 7214 0000 0072 1400  ...r....r....r..
-00001f50: 0000 7215 0000 0072 0700 0000 1000 0000  ..r....r........
-00001f60: 732a 0000 0008 0004 010a 0402 0910 0108  s*..............
-00001f70: 1d02 1602 0104 fd02 0202 fe02 030a fd0e  ................
-00001f80: 1a08 1416 070e 3012 0312 240e 160c 2572  ......0...$...%r
-00001f90: 0700 0000 290e 720b 0000 0072 4400 0000  ....).r....rD...
-00001fa0: 5a20 7965 7262 616d 6174 652e 6170 692e  Z yerbamate.api.
-00001fb0: 6461 7461 2e73 6f75 7263 6573 2e6c 6f63  data.sources.loc
-00001fc0: 616c 7202 0000 0072 2600 0000 5a16 7965  alr....r&...Z.ye
-00001fd0: 7262 616d 6174 652e 6170 692e 6d61 7465  rbamate.api.mate
-00001fe0: 5f61 7069 7203 0000 0072 3200 0000 da04  _apir....r2.....
-00001ff0: 6970 6462 7205 0000 0072 3400 0000 da06  ipdbr....r4.....
-00002000: 7479 7069 6e67 7206 0000 0072 0700 0000  typingr....r....
-00002010: 7214 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
-00002020: 1500 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00002030: 0000 7316 0000 0008 0008 010c 0108 010c  ..s.............
-00002040: 0108 0208 020c 0108 010c 0112 04         .............
+00000170: 045a 0e64 1d64 1e84 005a 0f64 1f65 0664  .Z.d.d...Z.d.e.d
+00000180: 2065 0666 0464 2164 2284 045a 1064 1f65   e.f.d!d"..Z.d.e
+00000190: 0664 2065 0666 0464 2364 2484 045a 1164  .d e.f.d#d$..Z.d
+000001a0: 2565 0666 0264 2664 2784 045a 1264 2864  %e.f.d&d'..Z.d(d
+000001b0: 2984 005a 1364 0a53 0029 2cda 044d 6174  )..Z.d.S.),..Mat
+000001c0: 657a 310a 2020 2020 4d61 7465 2c20 796f  ez1.    Mate, yo
+000001d0: 7572 2066 7269 656e 646c 7920 4d4c 2070  ur friendly ML p
+000001e0: 726f 6a65 6374 206d 616e 6167 6572 2e0a  roject manager..
+000001f0: 2020 2020 4663 0200 0000 0000 0000 0000      Fc..........
+00000200: 0000 0200 0000 0300 0000 4300 0000 733e  ..........C...s>
+00000210: 0000 0064 017c 005f 0064 017c 005f 0174  ...d.|._.d.|._.t
+00000220: 026a 03a0 0474 05a1 017c 005f 0664 007c  .j...t...|._.d.|
+00000230: 005f 077c 00a0 08a1 0001 0074 097c 006a  ._.|.......t.|.j
+00000240: 0783 017c 005f 0a64 007c 005f 0b64 0053  ...|._.d.|._.d.S
+00000250: 0029 024e da00 290c da0b 726f 6f74 5f66  .).N..)...root_f
+00000260: 6f6c 6465 72da 0973 6176 655f 7061 7468  older..save_path
+00000270: da02 6f73 da04 7061 7468 da07 6469 726e  ..os..path..dirn
+00000280: 616d 65da 085f 5f66 696c 655f 5f5a 0e63  ame..__file__Z.c
+00000290: 7572 7265 6e74 5f66 6f6c 6465 72da 0663  urrent_folder..c
+000002a0: 6f6e 6669 67da 0f5f 4d61 7465 5f5f 6669  onfig.._Mate__fi
+000002b0: 6e64 726f 6f74 7203 0000 00da 0361 7069  ndrootr......api
+000002c0: 5a0a 7275 6e5f 7061 7261 6d73 2902 da04  Z.run_params)...
+000002d0: 7365 6c66 da04 696e 6974 a900 7214 0000  self..init..r...
+000002e0: 00fa 342f 686f 6d65 2f61 6c2f 4769 7448  ..4/home/al/GitH
+000002f0: 7562 2f79 6572 6261 6d61 7465 2f70 6163  ub/yerbamate/pac
+00000300: 6b61 6765 732f 7965 7262 616d 6174 652f  kages/yerbamate/
+00000310: 6d61 7465 2e70 79da 085f 5f69 6e69 745f  mate.py..__init_
+00000320: 5f15 0000 0073 0e00 0000 0601 0601 0e01  _....s..........
+00000330: 0601 0801 0c01 0a01 7a0d 4d61 7465 2e5f  ........z.Mate._
+00000340: 5f69 6e69 745f 5fda 0c70 726f 6a65 6374  _init__..project
+00000350: 5f6e 616d 6563 0100 0000 0000 0000 0000  _namec..........
+00000360: 0000 0300 0000 0400 0000 4f00 0000 731c  ..........O...s.
+00000370: 0000 0074 006a 017c 0067 017c 01a2 0152  ...t.j.|.g.|...R
+00000380: 0069 007c 02a4 018e 0101 0064 0153 0029  .i.|.......d.S.)
+00000390: 0261 df01 0000 0a0a 2020 2020 2020 2020  .a......        
+000003a0: 606d 6174 6520 696e 6974 207b 7072 6f6a  `mate init {proj
+000003b0: 6563 745f 6e61 6d65 7d60 0a0a 2020 2020  ect_name}`..    
+000003c0: 2020 2020 496e 6974 6961 6c69 7a65 7320      Initializes 
+000003d0: 6120 6e65 7720 7072 6f6a 6563 742e 0a20  a new project.. 
+000003e0: 2020 2020 2020 2054 6869 7320 7769 6c6c         This will
+000003f0: 2063 7265 6174 6520 7468 6520 666f 6c6c   create the foll
+00000400: 6f77 696e 6720 7374 7275 6374 7572 653a  owing structure:
+00000410: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+00000420: 2020 2020 202f 0a20 2020 2020 2020 207c       /.        |
+00000430: 2d2d 206d 6f64 656c 732f 0a20 2020 2020  -- models/.     
+00000440: 2020 207c 2020 207c 2d2d 205f 5f69 6e69     |   |-- __ini
+00000450: 745f 5f2e 7079 0a20 2020 2020 2020 207c  t__.py.        |
+00000460: 2d2d 2065 7870 6572 696d 656e 7473 2f0a  -- experiments/.
+00000470: 2020 2020 2020 2020 7c20 2020 7c2d 2d20          |   |-- 
+00000480: 5f5f 696e 6974 5f5f 2e70 790a 2020 2020  __init__.py.    
+00000490: 2020 2020 7c2d 2d20 7472 6169 6e65 7273      |-- trainers
+000004a0: 2f0a 2020 2020 2020 2020 7c20 2020 7c2d  /.        |   |-
+000004b0: 2d20 5f5f 696e 6974 5f5f 2e70 790a 2020  - __init__.py.  
+000004c0: 2020 2020 2020 7c2d 2d20 6461 7461 2f0a        |-- data/.
+000004d0: 2020 2020 2020 2020 7c20 2020 7c2d 2d20          |   |-- 
+000004e0: 5f5f 696e 6974 5f5f 2e70 790a 2020 2020  __init__.py.    
+000004f0: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
+00000500: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00000510: 2020 2070 726f 6a65 6374 5f6e 616d 653a     project_name:
+00000520: 204e 616d 6520 6f66 2074 6865 2070 726f   Name of the pro
+00000530: 6a65 6374 2e0a 0a20 2020 2020 2020 2045  ject...        E
+00000540: 7861 6d70 6c65 3a0a 0a20 2020 2020 2020  xample:..       
+00000550: 2020 2020 2060 6d61 7465 2069 6e69 7420       `mate init 
+00000560: 6d79 5f70 726f 6a65 6374 600a 0a20 2020  my_project`..   
+00000570: 2020 2020 204e 2902 7203 0000 005a 0c69       N).r....Z.i
+00000580: 6e69 745f 7072 6f6a 6563 7429 0372 1700  nit_project).r..
+00000590: 0000 da04 6172 6773 da06 6b77 6172 6773  ....args..kwargs
+000005a0: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+000005b0: 1300 0000 1e00 0000 7302 0000 001c 1c7a  ........s......z
+000005c0: 094d 6174 652e 696e 6974 6301 0000 0000  .Mate.initc.....
+000005d0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+000005e0: 0000 0073 1000 0000 7c00 6a00 a001 6401  ...s....|.j...d.
+000005f0: a101 0100 6402 5300 2903 612b 0200 000a  ....d.S.).a+....
+00000600: 2020 2020 2020 2020 4765 6e65 7261 7465          Generate
+00000610: 7320 7265 7175 6972 656d 656e 7473 2e74  s requirements.t
+00000620: 7874 2c20 6465 7065 6e64 656e 6369 6573  xt, dependencies
+00000630: 2e6a 736f 6e20 616e 6420 6578 706f 7274  .json and export
+00000640: 732e 6d64 2066 6f72 2073 6861 7269 6e67  s.md for sharing
+00000650: 2061 6e64 2072 6570 726f 6475 6369 6269   and reproducibi
+00000660: 6c69 7479 2e0a 0a20 2020 2020 2020 2045  lity...        E
+00000670: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
+00000680: 2020 2020 606d 6174 6520 6578 706f 7274      `mate export
+00000690: 600a 0a20 2020 2020 2020 204f 7574 7075  `..        Outpu
+000006a0: 743a 0a20 2020 2020 2020 2020 2020 2060  t:.            `
+000006b0: 6060 0a20 2020 2020 2020 2020 2020 2047  ``.            G
+000006c0: 656e 6572 6174 6564 2072 6571 7569 7265  enerated require
+000006d0: 6d65 6e74 732e 7478 7420 666f 7220 6761  ments.txt for ga
+000006e0: 6e2f 6d6f 6465 6c73 2f6c 6761 6e0a 2020  n/models/lgan.  
+000006f0: 2020 2020 2020 2020 2020 4765 6e65 7261            Genera
+00000700: 7465 6420 6465 7065 6e64 656e 6369 6573  ted dependencies
+00000710: 2e6a 736f 6e20 666f 7220 6761 6e2f 6578  .json for gan/ex
+00000720: 7065 7269 6d65 6e74 732f 6c77 6761 6e0a  periments/lwgan.
+00000730: 2020 2020 2020 2020 2020 2020 4765 6e65              Gene
+00000740: 7261 7465 6420 7265 7175 6972 656d 656e  rated requiremen
+00000750: 7473 2e74 7874 2066 6f72 2067 616e 2f65  ts.txt for gan/e
+00000760: 7870 6572 696d 656e 7473 2f6c 7767 616e  xperiments/lwgan
+00000770: 0a20 2020 2020 2020 2020 2020 2047 656e  .            Gen
+00000780: 6572 6174 6564 2072 6571 7569 7265 6d65  erated requireme
+00000790: 6e74 732e 7478 7420 666f 7220 6761 6e2f  nts.txt for gan/
+000007a0: 7472 6169 6e65 7273 2f6c 6761 6e0a 2020  trainers/lgan.  
+000007b0: 2020 2020 2020 2020 2020 4765 6e65 7261            Genera
+000007c0: 7465 6420 7265 7175 6972 656d 656e 7473  ted requirements
+000007d0: 2e74 7874 2066 6f72 2067 616e 2f64 6174  .txt for gan/dat
+000007e0: 612f 6361 7273 0a20 2020 2020 2020 2020  a/cars.         
+000007f0: 2020 2045 7870 6f72 7465 6420 746f 2065     Exported to e
+00000800: 7870 6f72 742e 6d64 0a20 2020 2020 2020  xport.md.       
+00000810: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+00000820: 200a 2020 2020 2020 2020 da06 6578 706f   .        ..expo
+00000830: 7274 4ea9 0272 1100 0000 da04 6175 746f  rtN..r......auto
+00000840: a901 7212 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00000850: 0072 1500 0000 721a 0000 003c 0000 00f3  .r....r....<....
+00000860: 0200 0000 1012 7a0b 4d61 7465 2e65 7870  ......z.Mate.exp
+00000870: 6f72 744e 54da 0b6d 6f64 756c 655f 6e61  ortNT..module_na
+00000880: 6d65 da0b 6f75 7470 7574 5f6a 736f 6e63  me..output_jsonc
+00000890: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+000008a0: 0500 0000 4300 0000 7332 0000 007c 006a  ....C...s2...|.j
+000008b0: 00a0 017c 01a1 017d 037c 0272 1374 0274  ...|...}.|.r.t.t
+000008c0: 036a 047c 0364 0164 028d 0283 0101 0064  .j.|.d.d.......d
+000008d0: 0353 0074 027c 0383 0101 0064 0353 0029  .S.t.|.....d.S.)
+000008e0: 047a ee0a 0a0a 2020 2020 2020 2020 4c69  .z....        Li
+000008f0: 7374 7320 616c 6c20 6176 6169 6c61 626c  sts all availabl
+00000900: 6520 6d6f 6475 6c65 732e 0a0a 2020 2020  e modules...    
+00000910: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00000920: 2020 2020 2020 6d6f 6475 6c65 5f6e 616d        module_nam
+00000930: 653a 204e 616d 6520 6f66 2074 6865 206d  e: Name of the m
+00000940: 6f64 756c 6520 746f 206c 6973 742e 2049  odule to list. I
+00000950: 6620 6e6f 7420 7370 6563 6966 6965 642c  f not specified,
+00000960: 2061 6c6c 206d 6f64 756c 6573 2077 696c   all modules wil
+00000970: 6c20 6265 206c 6973 7465 642e 0a0a 2020  l be listed...  
+00000980: 2020 2020 2020 4578 616d 706c 6573 3a0a        Examples:.
+00000990: 2020 2020 2020 2020 2020 2020 606d 6174              `mat
+000009a0: 6520 6c69 7374 206d 6f64 656c 7360 0a0a  e list models`..
+000009b0: 2020 2020 2020 2020 2020 2020 606d 6174              `mat
+000009c0: 6520 6c69 7374 600a 0a20 2020 2020 2020  e list`..       
+000009d0: 20e9 0400 0000 a901 da06 696e 6465 6e74   .........indent
+000009e0: 4e29 0572 1100 0000 da04 6c69 7374 da05  N).r......list..
+000009f0: 7072 696e 74da 046a 736f 6eda 0564 756d  print..json..dum
+00000a00: 7073 2904 7212 0000 0072 1f00 0000 7220  ps).r....r....r 
+00000a10: 0000 00da 026c 6972 1400 0000 7214 0000  .....lir....r...
+00000a20: 0072 1500 0000 7224 0000 0050 0000 0073  .r....r$...P...s
+00000a30: 0800 0000 0c14 0401 1601 0c02 7a09 4d61  ............z.Ma
+00000a40: 7465 2e6c 6973 74da 0763 6f6d 6d61 6e64  te.list..command
+00000a50: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000a60: 0003 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+00000a70: 6a00 a001 7c01 a101 0100 6401 5300 2902  j...|.....d.S.).
+00000a80: 618e 0100 000a 0a20 2020 2020 2020 2060  a......        `
+00000a90: 6d61 7465 2061 7574 6f20 7b63 6f6d 6d61  mate auto {comma
+00000aa0: 6e64 7d60 0a0a 2020 2020 2020 2020 5661  nd}`..        Va
+00000ab0: 7269 6f75 7320 636f 6d6d 616e 6473 2074  rious commands t
+00000ac0: 6f20 6865 6c70 2077 6974 6820 7468 6520  o help with the 
+00000ad0: 6465 7665 6c6f 706d 656e 7420 7072 6f63  development proc
+00000ae0: 6573 732e 0a0a 0a20 2020 2020 2020 2063  ess....        c
+00000af0: 6f6d 6d61 6e64 733a 0a20 2020 2020 2020  ommands:.       
+00000b00: 202d 2060 6578 706f 7274 603a 2043 7265   - `export`: Cre
+00000b10: 6174 6573 2061 2072 6571 7569 7265 6d65  ates a requireme
+00000b20: 6e74 732e 7478 7420 616e 6420 6465 7065  nts.txt and depe
+00000b30: 6e64 656e 6369 6573 2e6a 736f 6e20 6669  ndencies.json fi
+00000b40: 6c65 7320 666f 7220 7368 6172 696e 6720  les for sharing 
+00000b50: 616e 6420 7265 7072 6f64 7563 6962 696c  and reproducibil
+00000b60: 6974 792e 0a20 2020 2020 2020 202d 2060  ity..        - `
+00000b70: 696e 6974 603a 2041 7574 6f6d 6174 6963  init`: Automatic
+00000b80: 616c 6c79 2063 7265 6174 6573 2060 5f5f  ally creates `__
+00000b90: 696e 6974 5f5f 2e70 7960 2066 696c 6573  init__.py` files
+00000ba0: 2069 6e20 7468 6520 7072 6f6a 6563 7420   in the project 
+00000bb0: 7374 7275 6374 7572 652e 0a0a 2020 2020  structure...    
+00000bc0: 2020 2020 4578 616d 706c 653a 0a0a 0a20      Example:... 
+00000bd0: 2020 2020 2020 2020 2020 2060 6d61 7465             `mate
+00000be0: 2061 7574 6f20 6578 706f 7274 600a 2020   auto export`.  
+00000bf0: 2020 2020 2020 2020 2020 606d 6174 6520            `mate 
+00000c00: 6175 746f 2069 6e69 7460 0a20 2020 2020  auto init`.     
+00000c10: 2020 204e 721b 0000 0029 0272 1200 0000     Nr....).r....
+00000c20: 7229 0000 0072 1400 0000 7214 0000 0072  r)...r....r....r
+00000c30: 1500 0000 721c 0000 006a 0000 0072 1e00  ....r....j...r..
+00000c40: 0000 7a09 4d61 7465 2e61 7574 6f63 0100  ..z.Mate.autoc..
+00000c50: 0000 0000 0000 0000 0000 0100 0000 0500  ................
+00000c60: 0000 4300 0000 731c 0000 0074 0074 016a  ..C...s....t.t.j
+00000c70: 027c 006a 03a0 04a1 0064 0164 028d 0283  .|.j.....d.d....
+00000c80: 0101 0064 0353 0029 047a 4e0a 2020 2020  ...d.S.).zN.    
+00000c90: 2020 2020 5072 696e 7473 2061 2073 756d      Prints a sum
+00000ca0: 6d61 7279 206f 6620 7468 6520 7072 6f6a  mary of the proj
+00000cb0: 6563 7420 6d6f 6475 6c65 732e 2053 616d  ect modules. Sam
+00000cc0: 6520 6173 2060 6d61 7465 206c 6973 7460  e as `mate list`
+00000cd0: 0a20 2020 2020 2020 2072 2100 0000 7222  .        r!...r"
+00000ce0: 0000 004e 2905 7225 0000 0072 2600 0000  ...N).r%...r&...
+00000cf0: 7227 0000 0072 1100 0000 da07 7375 6d6d  r'...r......summ
+00000d00: 6172 7972 1d00 0000 7214 0000 0072 1400  aryr....r....r..
+00000d10: 0000 7215 0000 0072 2a00 0000 7e00 0000  ..r....r*...~...
+00000d20: 7302 0000 001c 057a 0c4d 6174 652e 7375  s......z.Mate.su
+00000d30: 6d6d 6172 79da 066d 6f64 756c 65da 046e  mmary..module..n
+00000d40: 616d 65da 0464 6573 7463 0400 0000 0000  ame..destc......
+00000d50: 0000 0000 0000 0900 0000 0700 0000 4f00  ..............O.
+00000d60: 0000 73ec 0000 0074 006a 01a0 027c 006a  ..s....t.j...|.j
+00000d70: 037c 017c 02a1 037d 0674 006a 01a0 047c  .|.|...}.t.j...|
+00000d80: 06a1 0173 1f74 0564 017c 019b 0064 027c  ...s.t.d.|...d.|
+00000d90: 029b 0064 039d 0583 0101 0074 06a0 0764  ...d.......t...d
+00000da0: 04a1 0101 0074 006a 01a0 027c 006a 037c  .....t.j...|.j.|
+00000db0: 017c 03a1 037d 0774 006a 01a0 047c 07a1  .|...}.t.j...|..
+00000dc0: 0172 6164 057c 0476 0072 3f74 08a0 097c  .rad.|.v.r?t...|
+00000dd0: 07a1 0101 0074 0564 067c 079b 009d 0283  .....t.d.|......
+00000de0: 0101 006e 2274 0564 077c 039b 0064 089d  ...n"t.d.|...d..
+00000df0: 0383 0101 0074 0a64 0983 017d 087c 0864  .....t.d...}.|.d
+00000e00: 0a6b 0272 5c74 08a0 097c 07a1 0101 0074  .k.r\t...|.....t
+00000e10: 0564 067c 079b 009d 0283 0101 006e 0574  .d.|.........n.t
+00000e20: 06a0 0764 04a1 0101 0074 08a0 0b7c 067c  ...d.....t...|.|
+00000e30: 07a1 0201 0074 0564 017c 019b 0064 027c  .....t.d.|...d.|
+00000e40: 029b 0064 0b7c 079b 009d 0683 0101 0064  ...d.|.........d
+00000e50: 0c53 0029 0d61 8a01 0000 0a20 2020 2020  .S.).a.....     
+00000e60: 2020 2060 6d61 7465 2063 6c6f 6e65 207b     `mate clone {
+00000e70: 6d6f 6475 6c65 7d20 7b6e 616d 657d 207b  module} {name} {
+00000e80: 6465 7374 7d20 7b2d 6f7d 600a 0a20 2020  dest} {-o}`..   
+00000e90: 2020 2020 2043 6c6f 6e65 7320 6120 736f       Clones a so
+00000ea0: 7572 6365 2063 6f64 6520 6d6f 6475 6c65  urce code module
+00000eb0: 2074 6f20 6120 6e65 7720 6465 7374 696e   to a new destin
+00000ec0: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
+00000ed0: 4172 6773 3a0a 0a20 2020 2020 2020 2020  Args:..         
+00000ee0: 2020 206d 6f64 756c 653a 204d 6f64 756c     module: Modul
+00000ef0: 6520 746f 2063 6c6f 6e65 2e0a 0a20 2020  e to clone...   
+00000f00: 2020 2020 2020 2020 206e 616d 653a 204e           name: N
+00000f10: 616d 6520 6f66 2074 6865 206d 6f64 756c  ame of the modul
+00000f20: 6520 746f 2063 6c6f 6e65 2e0a 0a20 2020  e to clone...   
+00000f30: 2020 2020 2020 2020 2064 6573 743a 2044           dest: D
+00000f40: 6573 7469 6e61 7469 6f6e 2074 6f20 636c  estination to cl
+00000f50: 6f6e 6520 7468 6520 6d6f 6475 6c65 2074  one the module t
+00000f60: 6f2e 0a0a 2020 2020 2020 2020 2020 2020  o...            
+00000f70: 2d6f 3a20 4f76 6572 7772 6974 6520 6465  -o: Overwrite de
+00000f80: 7374 696e 6174 696f 6e20 6966 2069 7420  stination if it 
+00000f90: 6578 6973 7473 2e0a 0a20 2020 2020 2020  exists...       
+00000fa0: 2045 7861 6d70 6c65 3a0a 0a20 2020 2020   Example:..     
+00000fb0: 2020 2020 2020 2060 6d61 7465 2063 6c6f         `mate clo
+00000fc0: 6e65 206d 6f64 656c 7320 746f 7263 685f  ne models torch_
+00000fd0: 7669 7420 6d79 5f76 6974 600a 2020 2020  vit my_vit`.    
+00000fe0: 2020 2020 7a07 4d6f 6475 6c65 20fa 012f      z.Module ../
+00000ff0: 7a0f 2064 6f65 7320 6e6f 7420 6578 6973  z. does not exis
+00001000: 7472 0400 0000 7a02 2d6f 7a08 5265 6d6f  tr....z.-oz.Remo
+00001010: 7665 6420 7a0c 4465 7374 696e 6174 696f  ved z.Destinatio
+00001020: 6e20 7a07 2065 7869 7374 737a 124f 7665  n z. existsz.Ove
+00001030: 7277 7269 7465 3f20 2879 2f6e 293a 20da  rwrite? (y/n): .
+00001040: 0179 7a0b 2063 6c6f 6e65 6420 746f 204e  .yz. cloned to N
+00001050: 290c 720b 0000 0072 0c00 0000 da04 6a6f  ).r....r......jo
+00001060: 696e 7209 0000 00da 0665 7869 7374 7372  inr......existsr
+00001070: 2500 0000 da03 7379 73da 0465 7869 74da  %.....sys..exit.
+00001080: 0673 6875 7469 6cda 0672 6d74 7265 65da  .shutil..rmtree.
+00001090: 0569 6e70 7574 da08 636f 7079 7472 6565  .input..copytree
+000010a0: 2909 7212 0000 0072 2b00 0000 722c 0000  ).r....r+...r,..
+000010b0: 0072 2d00 0000 7218 0000 0072 1900 0000  .r-...r....r....
+000010c0: da0b 6d6f 6475 6c65 5f70 6174 685a 0964  ..module_pathZ.d
+000010d0: 6573 745f 7061 7468 da09 6f76 6572 7772  est_path..overwr
+000010e0: 6974 6572 1400 0000 7214 0000 0072 1500  iter....r....r..
+000010f0: 0000 da05 636c 6f6e 6585 0000 0073 2200  ....clone....s".
+00001100: 0000 1216 0c01 1601 0a01 1203 0c01 0802  ................
+00001110: 0a01 1001 1002 0801 0801 0a01 1001 0a02  ................
+00001120: 0c03 1e02 7a0a 4d61 7465 2e63 6c6f 6e65  ....z.Mate.clone
+00001130: da0a 6d6f 6465 6c5f 6e61 6d65 6302 0000  ..model_namec...
+00001140: 0000 0000 0000 0000 0002 0000 0001 0000  ................
+00001150: 0043 0000 0073 0400 0000 6400 5300 2901  .C...s....d.S.).
+00001160: 4e72 1400 0000 2902 7212 0000 0072 3b00  Nr....).r....r;.
+00001170: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00001180: 00da 0873 6e61 7073 686f 74b5 0000 0073  ...snapshot....s
+00001190: 0200 0000 0401 7a0d 4d61 7465 2e73 6e61  ......z.Mate.sna
+000011a0: 7073 686f 7463 0300 0000 0000 0000 0000  pshotc..........
+000011b0: 0000 0500 0000 0a00 0000 4300 0000 7388  ..........C...s.
+000011c0: 0000 007c 006a 006a 0164 017c 017c 0267  ...|.j.j.d.|.|.g
+000011d0: 047d 0364 02a0 027c 03a1 017d 037a 0774  .}.d...|...}.z.t
+000011e0: 037c 0383 0101 0057 0064 0053 0004 0074  .|.....W.d.S...t
+000011f0: 0479 4301 007d 0401 007a 2374 0564 037c  .yC..}...z#t.d.|
+00001200: 019b 0064 047c 029b 009d 0483 0101 0074  ...d.|.........t
+00001210: 0564 0583 0101 007c 00a0 067c 01a1 0101  .d.....|...|....
+00001220: 0074 07a0 08a1 0001 0074 09a0 0a64 06a1  .t.......t...d..
+00001230: 0101 0057 0059 0064 007d 047e 0464 0053  ...W.Y.d.}.~.d.S
+00001240: 0064 007d 047e 0477 0177 0029 074e da04  .d.}.~.w.w.).N..
+00001250: 6461 7461 da01 2efa 1145 7272 6f72 2069  data.....Error i
+00001260: 6e20 6c6f 6164 696e 6720 722e 0000 00fa  n loading r.....
+00001270: 1641 7661 696c 6162 6c65 2065 7870 6572  .Available exper
+00001280: 696d 656e 7473 3a72 0400 0000 a90b 720f  iments:r......r.
+00001290: 0000 00da 0770 726f 6a65 6374 7230 0000  .....projectr0..
+000012a0: 00da 0a5f 5f69 6d70 6f72 745f 5fda 0945  ...__import__..E
+000012b0: 7863 6570 7469 6f6e 7225 0000 0072 2400  xceptionr%...r$.
+000012c0: 0000 da09 7472 6163 6562 6163 6bda 0970  ....traceback..p
+000012d0: 7269 6e74 5f65 7863 7232 0000 0072 3300  rint_excr2...r3.
+000012e0: 0000 2905 7212 0000 00da 0b62 6173 655f  ..).r......base_
+000012f0: 6d6f 6475 6c65 5a0a 7375 625f 6d6f 6475  moduleZ.sub_modu
+00001300: 6c65 722b 0000 00da 0165 7214 0000 0072  ler+.....er....r
+00001310: 1400 0000 7215 0000 0072 3d00 0000 b800  ....r....r=.....
+00001320: 0000 7318 0000 0010 020a 0102 020e 010e  ..s.............
+00001330: 0114 0108 010a 0108 0118 0308 8002 f97a  ...............z
+00001340: 094d 6174 652e 6461 7461 da0a 6578 705f  .Mate.data..exp_
+00001350: 6d6f 6475 6c65 da03 6578 7063 0300 0000  module..expc....
+00001360: 0000 0000 0000 0000 0700 0000 0a00 0000  ................
+00001370: 4f00 0000 7388 0000 007c 006a 006a 0164  O...s....|.j.j.d
+00001380: 017c 017c 0267 047d 0564 02a0 027c 05a1  .|.|.g.}.d...|..
+00001390: 017d 057a 0774 037c 0583 0101 0057 0064  .}.z.t.|.....W.d
+000013a0: 0753 0004 0074 0479 4301 007d 0601 007a  .S...t.yC..}...z
+000013b0: 2374 0564 037c 019b 0064 047c 029b 009d  #t.d.|...d.|....
+000013c0: 0483 0101 0074 0564 0583 0101 007c 00a0  .....t.d.....|..
+000013d0: 0664 01a1 0101 0074 07a0 08a1 0001 0074  .d.....t.......t
+000013e0: 09a0 0a64 06a1 0101 0057 0059 0064 077d  ...d.....W.Y.d.}
+000013f0: 067e 0664 0753 0064 077d 067e 0677 0177  .~.d.S.d.}.~.w.w
+00001400: 0029 0861 e001 0000 0a20 2020 2020 2020  .).a.....       
+00001410: 2045 7865 6375 7465 7320 616e 2065 7870   Executes an exp
+00001420: 6572 696d 656e 742e 0a0a 2020 2020 2020  eriment...      
+00001430: 2020 5573 6167 653a 2060 606d 6174 6520    Usage: ``mate 
+00001440: 7472 6169 6e20 7b6d 6f64 756c 657d 207b  train {module} {
+00001450: 6578 7065 7269 6d65 6e74 7d60 600a 0a20  experiment}``.. 
+00001460: 2020 2020 2020 2041 7267 733a 0a0a 2020         Args:..  
+00001470: 2020 2020 2020 2020 2020 6578 705f 6d6f            exp_mo
+00001480: 6475 6c65 3a20 4e61 6d65 206f 6620 7468  dule: Name of th
+00001490: 6520 6d6f 6475 6c65 2077 6865 7265 2074  e module where t
+000014a0: 6865 2065 7870 6572 696d 656e 7420 6973  he experiment is
+000014b0: 206c 6f63 6174 6564 2e0a 0a20 2020 2020   located...     
+000014c0: 2020 2020 2020 2065 7870 3a20 4e61 6d65         exp: Name
+000014d0: 206f 6620 7468 6520 6578 7065 7269 6d65   of the experime
+000014e0: 6e74 2e0a 0a20 2020 2020 2020 2045 7861  nt...        Exa
+000014f0: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
+00001500: 2020 600a 2020 2020 2020 2020 2020 2020    `.            
+00001510: 6d61 7465 2074 7261 696e 2065 7870 6572  mate train exper
+00001520: 696d 656e 7473 206d 795f 6578 7065 7269  iments my_experi
+00001530: 6d65 6e74 600a 0a20 2020 2020 2020 2054  ment`..        T
+00001540: 6869 7320 7769 6c6c 2072 756e 2074 6865  his will run the
+00001550: 2065 7870 6572 696d 656e 7420 606d 795f   experiment `my_
+00001560: 6578 7065 7269 6d65 6e74 6020 6c6f 6361  experiment` loca
+00001570: 7465 6420 696e 2074 6865 2060 6578 7065  ted in the `expe
+00001580: 7269 6d65 6e74 7360 206d 6f64 756c 652e  riments` module.
+00001590: 0a0a 2020 2020 2020 2020 4571 7569 7661  ..        Equiva
+000015a0: 6c65 6e74 2074 6f20 6070 7974 686f 6e20  lent to `python 
+000015b0: 2d6d 2072 6f6f 745f 6d6f 6475 6c65 2e65  -m root_module.e
+000015c0: 7870 6572 696d 656e 7473 2e6d 795f 6578  xperiments.my_ex
+000015d0: 7065 7269 6d65 6e74 2074 7261 696e 600a  periment train`.
+000015e0: 2020 2020 2020 2020 da0b 6578 7065 7269          ..experi
+000015f0: 6d65 6e74 7372 3e00 0000 723f 0000 0072  mentsr>...r?...r
+00001600: 2e00 0000 7240 0000 0072 0400 0000 4e72  ....r@...r....Nr
+00001610: 4100 0000 2907 7212 0000 0072 4900 0000  A...).r....rI...
+00001620: 724a 0000 0072 1800 0000 7219 0000 0072  rJ...r....r....r
+00001630: 2b00 0000 7248 0000 0072 1400 0000 7214  +...rH...r....r.
+00001640: 0000 0072 1500 0000 da05 7472 6169 6eca  ...r......train.
+00001650: 0000 0073 1800 0000 1016 0a01 0202 0e01  ...s............
+00001660: 0e01 1401 0801 0a01 0801 1803 0880 02f9  ................
+00001670: 7a0a 4d61 7465 2e74 7261 696e 6303 0000  z.Mate.trainc...
+00001680: 0000 0000 0000 0000 0005 0000 0004 0000  ................
+00001690: 004f 0000 0073 1e00 0000 7c00 6a00 7c01  .O...s....|.j.|.
+000016a0: 7c02 6702 7c03 a201 5200 6900 7c04 a401  |.g.|...R.i.|...
+000016b0: 8e01 0100 6401 5300 2902 61dd 0100 000a  ....d.S.).a.....
+000016c0: 2020 2020 2020 2020 4578 6563 7574 6573          Executes
+000016d0: 2061 6e20 6578 7065 7269 6d65 6e74 2e0a   an experiment..
+000016e0: 0a20 2020 2020 2020 2055 7361 6765 3a20  .        Usage: 
+000016f0: 6060 6d61 7465 2074 6573 7420 7b6d 6f64  ``mate test {mod
+00001700: 756c 657d 207b 6578 7065 7269 6d65 6e74  ule} {experiment
+00001710: 7d60 600a 0a20 2020 2020 2020 2041 7267  }``..        Arg
+00001720: 733a 0a0a 2020 2020 2020 2020 2020 2020  s:..            
+00001730: 6578 705f 6d6f 6475 6c65 3a20 4e61 6d65  exp_module: Name
+00001740: 206f 6620 7468 6520 6d6f 6475 6c65 2077   of the module w
+00001750: 6865 7265 2074 6865 2065 7870 6572 696d  here the experim
+00001760: 656e 7420 6973 206c 6f63 6174 6564 2e0a  ent is located..
+00001770: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
+00001780: 3a20 4e61 6d65 206f 6620 7468 6520 6578  : Name of the ex
+00001790: 7065 7269 6d65 6e74 2e0a 0a20 2020 2020  periment...     
+000017a0: 2020 2045 7861 6d70 6c65 3a0a 2020 2020     Example:.    
+000017b0: 2020 2020 2020 2020 600a 2020 2020 2020          `.      
+000017c0: 2020 2020 2020 6d61 7465 2074 6573 7420        mate test 
+000017d0: 6578 7065 7269 6d65 6e74 7320 6d79 5f65  experiments my_e
+000017e0: 7870 6572 696d 656e 7460 0a0a 2020 2020  xperiment`..    
+000017f0: 2020 2020 5468 6973 2077 696c 6c20 7275      This will ru
+00001800: 6e20 7468 6520 6578 7065 7269 6d65 6e74  n the experiment
+00001810: 2060 6d79 5f65 7870 6572 696d 656e 7460   `my_experiment`
+00001820: 206c 6f63 6174 6564 2069 6e20 7468 6520   located in the 
+00001830: 6065 7870 6572 696d 656e 7473 6020 6d6f  `experiments` mo
+00001840: 6475 6c65 2e0a 0a20 2020 2020 2020 2045  dule...        E
+00001850: 7175 6976 616c 656e 7420 746f 2060 7079  quivalent to `py
+00001860: 7468 6f6e 202d 6d20 726f 6f74 5f6d 6f64  thon -m root_mod
+00001870: 756c 652e 6578 7065 7269 6d65 6e74 732e  ule.experiments.
+00001880: 6d79 5f65 7870 6572 696d 656e 7420 7465  my_experiment te
+00001890: 7374 600a 2020 2020 2020 2020 4e29 0172  st`.        N).r
+000018a0: 4c00 0000 2905 7212 0000 0072 4900 0000  L...).r....rI...
+000018b0: 724a 0000 0072 1800 0000 7219 0000 0072  rJ...r....r....r
+000018c0: 1400 0000 7214 0000 0072 1500 0000 da04  ....r....r......
+000018d0: 7465 7374 ee00 0000 7302 0000 001e 147a  test....s......z
+000018e0: 094d 6174 652e 7465 7374 da03 7572 6c63  .Mate.test..urlc
+000018f0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00001900: 0400 0000 4f00 0000 731e 0000 007c 006a  ....O...s....|.j
+00001910: 006a 017c 0167 017c 02a2 0152 0069 007c  .j.|.g.|...R.i.|
+00001920: 03a4 018e 0101 0064 0153 0029 0261 6905  .......d.S.).ai.
+00001930: 0000 0a20 2020 2020 2020 2049 6e74 616c  ...        Intal
+00001940: 6c73 2061 206d 6f64 756c 6520 6672 6f6d  ls a module from
+00001950: 2061 2067 6974 2072 6570 6f73 6974 6f72   a git repositor
+00001960: 792e 0a0a 2020 2020 2020 2020 5573 6167  y...        Usag
+00001970: 653a 2060 606d 6174 6520 696e 7374 616c  e: ``mate instal
+00001980: 6c20 7b75 726c 7d20 2d7b 797c 6e7c 6f7d  l {url} -{y|n|o}
+00001990: 207b 706d 7d60 600a 0a20 2020 2020 2020   {pm}``..       
+000019a0: 2049 6e73 7461 6c6c 206d 6f64 756c 6520   Install module 
+000019b0: 7375 7070 6f72 7420 7468 6520 666f 6c6c  support the foll
+000019c0: 6f77 696e 6720 666f 726d 6174 733a 0a20  owing formats:. 
+000019d0: 2020 2020 2020 202d 2060 606d 6174 6520         - ``mate 
+000019e0: 696e 7374 616c 6c20 7b63 6f6d 706c 6574  install {complet
+000019f0: 655f 7572 6c7d 6060 0a20 2020 2020 2020  e_url}``.       
+00001a00: 202d 2060 606d 6174 6520 696e 7374 616c   - ``mate instal
+00001a10: 6c20 7b75 7365 727d 2f7b 7265 706f 7d2f  l {user}/{repo}/
+00001a20: 7b72 6f6f 745f 6d6f 6475 6c65 7d2f 7b6d  {root_module}/{m
+00001a30: 6f64 756c 657d 6060 0a20 2020 2020 2020  odule}``.       
+00001a40: 202d 2060 606d 6174 6520 696e 7374 616c   - ``mate instal
+00001a50: 6c20 7b75 7365 727d 2f7b 7265 706f 7c72  l {user}/{repo|r
+00001a60: 6f6f 745f 6d6f 6475 6c65 7d2f 7b6d 6f64  oot_module}/{mod
+00001a70: 756c 657d 6060 0a0a 2020 2020 2020 2020  ule}``..        
+00001a80: 4172 6773 3a0a 2020 2020 2020 2020 2d20  Args:.        - 
+00001a90: 2020 2075 726c 3a20 5572 6c20 6f66 2074     url: Url of t
+00001aa0: 6865 2067 6974 2072 6570 6f73 6974 6f72  he git repositor
+00001ab0: 792e 0a20 2020 2020 2020 202d 2020 2020  y..        -    
+00001ac0: 2d79 3a20 536b 6970 7320 636f 6e66 6972  -y: Skips confir
+00001ad0: 6d61 7469 6f6e 2061 6e64 2069 6e73 7461  mation and insta
+00001ae0: 6c6c 7320 7079 7468 6f6e 2064 6570 656e  lls python depen
+00001af0: 6465 6e63 6965 730a 2020 2020 2020 2020  dencies.        
+00001b00: 2d20 2020 202d 6e3a 2053 6b69 7073 2069  -    -n: Skips i
+00001b10: 6e73 7461 6c6c 696e 6720 7079 7468 6f6e  nstalling python
+00001b20: 2064 6570 656e 6465 6e63 6965 730a 2020   dependencies.  
+00001b30: 2020 2020 2020 2d20 2020 202d 6f3a 204f        -    -o: O
+00001b40: 7665 7277 7269 7465 7320 6578 6973 7469  verwrites existi
+00001b50: 6e67 2063 6f64 6520 6d6f 6475 6c65 730a  ng code modules.
+00001b60: 2020 2020 2020 2020 2d20 2020 2070 6d3a          -    pm:
+00001b70: 2050 6163 6b61 6765 206d 616e 6167 6572   Package manager
+00001b80: 2074 6f20 7573 652e 2044 6566 6175 6c74   to use. Default
+00001b90: 7320 746f 2061 736b 696e 6720 7468 6520  s to asking the 
+00001ba0: 7573 6572 2e0a 0a20 2020 2020 2020 2045  user...        E
+00001bb0: 7861 6d70 6c65 2049 6e73 7461 6c6c 696e  xample Installin
+00001bc0: 6720 6120 6d6f 6475 6c65 2066 726f 6d20  g a module from 
+00001bd0: 7374 7275 6374 7572 6564 2067 6974 2072  structured git r
+00001be0: 6570 6f73 6974 6f72 7920 2872 6563 6f6d  epository (recom
+00001bf0: 6d65 6e64 6564 293a 0a0a 0a20 2020 2020  mended):...     
+00001c00: 2020 2020 2020 206d 6174 6520 696e 7374         mate inst
+00001c10: 616c 6c20 6f61 6c65 652f 6465 6570 2d76  all oalee/deep-v
+00001c20: 6973 696f 6e2f 6465 6570 6e65 742f 6d6f  ision/deepnet/mo
+00001c30: 6465 6c73 2f74 6f72 6368 5f76 6974 202d  dels/torch_vit -
+00001c40: 796f 2070 6970 0a0a 2020 2020 2020 2020  yo pip..        
+00001c50: 2020 2020 5468 6973 2077 696c 6c20 696e      This will in
+00001c60: 7374 616c 6c20 7468 6520 6d6f 6475 6c65  stall the module
+00001c70: 2060 746f 7263 685f 7669 7460 2066 726f   `torch_vit` fro
+00001c80: 6d20 7468 6520 7265 706f 7369 746f 7279  m the repository
+00001c90: 2060 6f61 6c65 652f 6465 6570 2d76 6973   `oalee/deep-vis
+00001ca0: 696f 6e60 2069 6e20 746f 2079 6f75 7220  ion` in to your 
+00001cb0: 606d 6f64 656c 7360 2066 6f6c 6465 722e  `models` folder.
+00001cc0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00001cd0: 2060 796f 6020 666c 6167 7320 7769 6c6c   `yo` flags will
+00001ce0: 2073 6b69 7020 636f 6e66 6972 6d61 7469   skip confirmati
+00001cf0: 6f6e 2061 6e64 2069 6e73 7461 6c6c 2070  on and install p
+00001d00: 7974 686f 6e20 6465 7065 6e64 656e 6369  ython dependenci
+00001d10: 6573 2075 7369 6e67 2070 6970 2e0a 0a20  es using pip... 
+00001d20: 2020 2020 2020 2045 7861 6d70 6c65 2049         Example I
+00001d30: 6e73 7461 6c6c 696e 6720 6120 6d6f 6475  nstalling a modu
+00001d40: 6c65 2066 726f 6d20 756e 7374 7275 6374  le from unstruct
+00001d50: 7572 6564 2067 6974 2072 6570 6f73 6974  ured git reposit
+00001d60: 6f72 793a 0a0a 0a20 2020 2020 2020 2020  ory:...         
+00001d70: 2020 206d 6174 6520 696e 7374 616c 6c20     mate install 
+00001d80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001d90: 6f6d 2f72 7769 6768 746d 616e 2f70 7974  om/rwightman/pyt
+00001da0: 6f72 6368 2d69 6d61 6765 2d6d 6f64 656c  orch-image-model
+00001db0: 732f 7472 6565 2f6d 6169 6e2f 7469 6d6d  s/tree/main/timm
+00001dc0: 0a0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
+00001dd0: 6869 7320 7769 6c6c 2069 6e73 7461 6c6c  his will install
+00001de0: 2074 6865 206d 6f64 756c 6520 6074 696d   the module `tim
+00001df0: 6d60 2066 726f 6d20 7468 6520 7265 706f  m` from the repo
+00001e00: 7369 746f 7279 2061 7320 6120 7369 7374  sitory as a sist
+00001e10: 6572 206d 6f64 756c 6520 746f 2079 6f75  er module to you
+00001e20: 7220 726f 6f74 206d 6f64 756c 652e 0a20  r root module.. 
+00001e30: 2020 2020 2020 2020 2020 2054 616b 6520             Take 
+00001e40: 696e 746f 2061 6363 6f75 6e74 2074 6861  into account tha
+00001e50: 7420 7468 6973 2077 696c 6c20 696e 7374  t this will inst
+00001e60: 616c 6c20 6f6e 6c79 2074 6865 2063 6f64  all only the cod
+00001e70: 6520 616e 6420 6e6f 7420 7468 6520 7079  e and not the py
+00001e80: 7468 6f6e 2064 6570 656e 6465 6e63 6965  thon dependencie
+00001e90: 732e 0a20 2020 2020 2020 204e 2902 7211  s..        N).r.
+00001ea0: 0000 005a 0b69 6e73 7461 6c6c 5f75 726c  ...Z.install_url
+00001eb0: 2904 7212 0000 0072 4e00 0000 7218 0000  ).r....rN...r...
+00001ec0: 0072 1900 0000 7214 0000 0072 1400 0000  .r....r....r....
+00001ed0: 7215 0000 00da 0769 6e73 7461 6c6c 0401  r......install..
+00001ee0: 0000 7302 0000 001e 237a 0c4d 6174 652e  ..s.....#z.Mate.
+00001ef0: 696e 7374 616c 6c63 0100 0000 0000 0000  installc........
+00001f00: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00001f10: 7314 0000 0074 00a0 01a1 005c 027c 005f  s....t.....\.|._
+00001f20: 027c 005f 0364 0153 0029 027a 710a 2020  .|._.d.S.).zq.  
+00001f30: 2020 2020 2020 4d65 7468 6f64 2069 6e20        Method in 
+00001f40: 6368 6172 6765 206f 6620 6669 6e64 696e  charge of findin
+00001f50: 6720 7468 6520 726f 6f74 2066 6f6c 6465  g the root folde
+00001f60: 7220 6f66 2074 6865 2070 726f 6a65 6374  r of the project
+00001f70: 2061 6e64 2072 6561 6469 6e67 2074 6865   and reading the
+00001f80: 2063 6f6e 7465 6e74 206f 6620 6d61 7465   content of mate
+00001f90: 2e6a 736f 6e0a 2020 2020 2020 2020 4e29  .json.        N)
+00001fa0: 0472 0200 0000 5a09 6669 6e64 5f72 6f6f  .r....Z.find_roo
+00001fb0: 7472 0900 0000 720f 0000 0072 1d00 0000  tr....r....r....
+00001fc0: 7214 0000 0072 1400 0000 7215 0000 005a  r....r....r....Z
+00001fd0: 0a5f 5f66 696e 6472 6f6f 7429 0100 0073  .__findroot)...s
+00001fe0: 0200 0000 1404 7a0f 4d61 7465 2e5f 5f66  ......z.Mate.__f
+00001ff0: 696e 6472 6f6f 7429 0146 2902 4e54 2914  indroot).F).NT).
+00002000: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00002010: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00002020: 6d65 5f5f da07 5f5f 646f 635f 5f72 1600  me__..__doc__r..
+00002030: 0000 da0c 7374 6174 6963 6d65 7468 6f64  ....staticmethod
+00002040: da03 7374 7272 1300 0000 721a 0000 00da  ..strr....r.....
+00002050: 0462 6f6f 6c72 2400 0000 721c 0000 0072  .boolr$...r....r
+00002060: 2a00 0000 723a 0000 0072 3c00 0000 723d  *...r:...r<...r=
+00002070: 0000 0072 4c00 0000 724d 0000 0072 4f00  ...rL...rM...rO.
+00002080: 0000 7210 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00002090: 0072 1400 0000 7215 0000 0072 0700 0000  .r....r....r....
+000020a0: 1000 0000 732c 0000 0008 0004 010a 0402  ....s,..........
+000020b0: 0910 0108 1d02 1602 0104 fd02 0202 fe02  ................
+000020c0: 030a fd0e 1a08 1416 070e 3008 0312 1212  ..........0.....
+000020d0: 240e 160c 2572 0700 0000 290e 720b 0000  $...%r....).r...
+000020e0: 0072 4500 0000 5a20 7965 7262 616d 6174  .rE...Z yerbamat
+000020f0: 652e 6170 692e 6461 7461 2e73 6f75 7263  e.api.data.sourc
+00002100: 6573 2e6c 6f63 616c 7202 0000 0072 2600  es.localr....r&.
+00002110: 0000 5a16 7965 7262 616d 6174 652e 6170  ..Z.yerbamate.ap
+00002120: 692e 6d61 7465 5f61 7069 7203 0000 0072  i.mate_apir....r
+00002130: 3200 0000 da04 6970 6462 7205 0000 0072  2.....ipdbr....r
+00002140: 3400 0000 da06 7479 7069 6e67 7206 0000  4.....typingr...
+00002150: 0072 0700 0000 7214 0000 0072 1400 0000  .r....r....r....
+00002160: 7214 0000 0072 1500 0000 da08 3c6d 6f64  r....r......<mod
+00002170: 756c 653e 0100 0000 7316 0000 0008 0008  ule>....s.......
+00002180: 010c 0108 010c 0108 0208 020c 0108 010c  ................
+00002190: 0112 04                                  ...
```

### Comparing `yerbamate-0.9.239/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr  8 19:56:23 2023 UTC, .py size: 10611 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e7c6 3164 7329 0000  o.........1ds)..
+00000000: 6f0d 0d0a 0000 0000 56b4 8e64 9f29 0000  o.......V..d.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6404  ..d.d.l.m.Z...d.
 00000050: 6405 6c06 5a06 6404 6406 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6404 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0b 6404 6405 6c0c 5a0c 6404 6405 6c0d  Z.d.d.l.Z.d.d.l.
@@ -420,168 +420,169 @@
 00001a30: 0000 0072 6200 0000 7259 0000 0072 2a00  ...rb...rY...r*.
 00001a40: 0000 7270 0000 0072 7300 0000 da04 6469  ..rp...rs.....di
 00001a50: 6374 7275 0000 0072 0b00 0000 720b 0000  ctru...r....r...
 00001a60: 0072 0b00 0000 720f 0000 0072 5000 0000  .r....r....rP...
 00001a70: 7200 0000 730e 0000 0008 0008 0108 1a08  r...s...........
 00001a80: 1614 2314 171a 0e72 5000 0000 7267 0000  ..#....rP...rg..
 00001a90: 0072 6800 0000 6302 0000 0000 0000 0000  .rh...c.........
-00001aa0: 0000 000d 0000 0008 0000 0043 0000 0073  ...........C...s
-00001ab0: 1801 0000 6900 7d02 6700 7d03 6401 7d04  ....i.}.g.}.d.}.
+00001aa0: 0000 000c 0000 0008 0000 0043 0000 0073  ...........C...s
+00001ab0: 0c01 0000 6900 7d02 6700 7d03 6401 7d04  ....i.}.g.}.d.}.
 00001ac0: 6402 7400 6602 6403 6404 8404 7d05 6402  d.t.f.d.d...}.d.
 00001ad0: 7400 6602 6405 6406 8404 7d06 7401 7c01  t.f.d.d...}.t.|.
 00001ae0: 8301 7401 7c00 8301 6b00 7229 7c01 7c05  ..t.|...k.r)|.|.
 00001af0: 6601 7401 7c00 8301 7401 7c01 8301 1800  f.t.|...t.|.....
-00001b00: 1400 1700 7d01 6407 6408 6c02 6d03 7d07  ....}.d.d.l.m.}.
-00001b10: 0100 7404 7405 7c00 7c01 8302 8301 4400  ..t.t.|.|.....D.
-00001b20: 5d51 5c02 7d08 5c02 7d09 7d0a 7c0a 7406  ]Q\.}.\.}.}.|.t.
-00001b30: 6b02 7243 7c06 7d0a 6e10 7c0a 7407 6a08  k.rC|.}.n.|.t.j.
-00001b40: 6b02 724b 7c05 7d0a 6e08 7409 7c0a 6409  k.rK|.}.n.t.|.d.
-00001b50: 8302 7253 7c0a 6a0a 7d0a 640a 7c09 7600  ..rS|.j.}.d.|.v.
-00001b60: 7267 7c09 a00b 640a a101 5c02 7d0b 7d0c  rg|...d...\.}.}.
-00001b70: 7c0a 7c0c 8301 7c02 7c0b 3c00 640b 7d04  |.|...|.|.<.d.}.
-00001b80: 7136 740c 7c0a 740d 8302 7270 7c0a 6407  q6t.|.t...rp|.d.
-00001b90: 1900 7d0a 7c03 a00e 7c0a 7c09 8301 a101  ..}.|...|.|.....
-00001ba0: 0100 7c04 7287 740f 640c 7c09 9b00 640d  ..|.r.t.d.|...d.
-00001bb0: 7c00 7c08 640e 1800 1900 9b00 9d04 8301  |.|.d...........
-00001bc0: 8201 7136 7c03 7c02 6602 5300 290f 4e46  ..q6|.|.f.S.).NF
-00001bd0: 7263 0000 0063 0100 0000 0000 0000 0000  rc...c..........
-00001be0: 0000 0300 0000 0900 0000 5300 0000 7368  ..........S...sh
-00001bf0: 0000 0074 0074 0174 0267 037d 017c 00a0  ...t.t.t.g.}.|..
-00001c00: 03a1 0064 0176 0072 0d64 0053 007c 00a0  ...d.v.r.d.S.|..
-00001c10: 03a1 0064 026b 0272 1564 0353 007c 00a0  ...d.k.r.d.S.|..
-00001c20: 03a1 0064 046b 0272 1d64 0553 007c 0144  ...d.k.r.d.S.|.D
-00001c30: 005d 127d 027a 077c 027c 0083 0157 0002  .].}.z.|.|...W..
-00001c40: 0001 0053 0004 0074 0479 3101 0001 0001  ...S...t.y1.....
-00001c50: 0059 0071 1f77 0064 0053 0029 064e 2902  .Y.q.w.d.S.).N).
-00001c60: da04 6e6f 6e65 da04 6e75 6c6c da04 7472  ..none..null..tr
-00001c70: 7565 54da 0566 616c 7365 4629 05da 0369  ueT..falseF)...i
-00001c80: 6e74 da05 666c 6f61 7472 2a00 0000 da05  nt..floatr*.....
-00001c90: 6c6f 7765 72da 0a56 616c 7565 4572 726f  lower..ValueErro
-00001ca0: 7229 0372 6300 0000 da05 7479 7065 73da  r).rc.....types.
-00001cb0: 0174 720b 0000 0072 0b00 0000 720f 0000  .tr....r....r...
-00001cc0: 00da 0f67 6f6f 645f 6775 6573 735f 7479  ...good_guess_ty
-00001cd0: 7065 fa00 0000 731c 0000 000a 010c 0104  pe....s.........
-00001ce0: 010c 0104 010c 0104 0108 0102 010e 010c  ................
-00001cf0: 0104 0102 ff04 fd7a 2563 6f6c 6c65 6374  .......z%collect
-00001d00: 5f61 7267 732e 3c6c 6f63 616c 733e 2e67  _args.<locals>.g
-00001d10: 6f6f 645f 6775 6573 735f 7479 7065 6301  ood_guess_typec.
-00001d20: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00001d30: 0000 0053 0000 0073 2800 0000 7c00 a000  ...S...s(...|...
-00001d40: a100 6401 6b02 7208 6402 5300 7c00 a000  ..d.k.r.d.S.|...
-00001d50: a100 6403 6b02 7210 6404 5300 7401 6405  ..d.k.r.d.S.t.d.
-00001d60: 8301 8201 2906 4e72 7b00 0000 5472 7c00  ....).Nr{...Tr|.
-00001d70: 0000 467a 0d4e 6f74 2061 2062 6f6f 6c65  ..Fz.Not a boole
-00001d80: 616e 2902 727f 0000 0072 8000 0000 2901  an).r....r....).
-00001d90: 7263 0000 0072 0b00 0000 720b 0000 0072  rc...r....r....r
-00001da0: 0f00 0000 da0c 626f 6f6c 6561 6e5f 7479  ......boolean_ty
-00001db0: 7065 0801 0000 730a 0000 000c 0104 010c  pe....s.........
-00001dc0: 0104 0108 027a 2263 6f6c 6c65 6374 5f61  .....z"collect_a
-00001dd0: 7267 732e 3c6c 6f63 616c 733e 2e62 6f6f  rgs.<locals>.boo
-00001de0: 6c65 616e 5f74 7970 6572 0500 0000 2901  lean_typer....).
-00001df0: da05 556e 696f 6eda 085f 5f61 7267 735f  ..Union..__args_
-00001e00: 5f72 2500 0000 547a 1470 6f73 6974 696f  _r%...Tz.positio
-00001e10: 6e61 6c20 6172 6775 6d65 6e74 207a 1820  nal argument z. 
-00001e20: 6166 7465 7220 6b65 7977 6f72 6420 6172  after keyword ar
-00001e30: 6775 6d65 6e74 2072 0100 0000 2910 722a  gument r....).r*
-00001e40: 0000 0072 3000 0000 da06 7479 7069 6e67  ...r0.....typing
-00001e50: 7285 0000 00da 0965 6e75 6d65 7261 7465  r......enumerate
-00001e60: 7260 0000 00da 0462 6f6f 6c72 1200 0000  r`.....boolr....
-00001e70: 7229 0000 00da 0768 6173 6174 7472 7286  r).....hasattrr.
-00001e80: 0000 0072 3100 0000 da0a 6973 696e 7374  ...r1.....isinst
-00001e90: 616e 6365 7211 0000 00da 0661 7070 656e  ancer......appen
-00001ea0: 6472 8000 0000 290d 7267 0000 0072 6800  dr....).rg...rh.
-00001eb0: 0000 da06 6b77 6172 6773 5a0f 706f 7369  ....kwargsZ.posi
-00001ec0: 7469 6f6e 616c 5f61 7267 735a 1770 6f73  tional_argsZ.pos
-00001ed0: 6974 696f 6e61 6c5f 6172 6773 5f73 7461  itional_args_sta
-00001ee0: 7274 6564 7283 0000 0072 8400 0000 7285  rtedr....r....r.
-00001ef0: 0000 00da 0169 7263 0000 0072 3b00 0000  .....irc...r;...
-00001f00: 7274 0000 00da 0576 616c 7565 720b 0000  rt.....valuer...
-00001f10: 0072 0b00 0000 720f 0000 00da 0c63 6f6c  .r....r......col
-00001f20: 6c65 6374 5f61 7267 73ef 0000 0073 3800  lect_args....s8.
-00001f30: 0000 0407 0401 0401 0e02 0e0e 1008 1a01  ................
-00001f40: 0c01 1a02 0801 0601 0a01 0601 0a01 0601  ................
-00001f50: 0801 0e01 0c01 0601 0a02 0801 0e01 0401  ................
-00001f60: 0201 1601 04ff 02ff 0805 7290 0000 0063  ..........r....c
-00001f70: 0000 0000 0000 0000 0000 0000 0d00 0000  ................
-00001f80: 0a00 0000 4300 0000 739c 0100 0074 0074  ....C...s....t.t
-00001f90: 0183 017d 0074 026a 0364 0164 0085 0219  ...}.t.j.d.d....
-00001fa0: 007d 017c 0164 0164 0085 0219 007d 0264  .}.|.d.d.....}.d
-00001fb0: 027d 0374 0464 0364 0484 007c 0044 0083  .}.t.d.d...|.D..
-00001fc0: 0183 017c 0317 007d 0474 0583 007d 0574  ...|...}.t...}.t
-00001fd0: 067c 0183 0164 056b 0273 2d7c 0164 0519  .|...d.k.s-|.d..
-00001fe0: 007c 0376 0072 4274 067c 0183 0164 016b  .|.v.rBt.|...d.k
-00001ff0: 0472 3c7c 05a0 077c 0164 0119 00a1 0101  .r<|...|.d......
-00002000: 0064 0053 007c 05a0 07a1 0001 0064 0053  .d.S.|.......d.S
-00002010: 007c 0164 0519 007d 0674 067c 0183 0164  .|.d...}.t.|...d
-00002020: 016b 0472 5c7c 0164 0119 0064 0676 0072  .k.r\|.d...d.v.r
-00002030: 5c74 087c 0683 017d 0774 097c 0783 0101  \t.|...}.t.|....
-00002040: 0064 0053 007c 067c 0076 0172 8b7a 0f74  .d.S.|.|.v.r.z.t
-00002050: 0183 007d 087c 086a 0a7c 0164 0164 0085  ...}.|.j.|.d.d..
-00002060: 0219 008e 0001 0057 0064 0053 0004 0074  .......W.d.S...t
-00002070: 0b79 8a01 007d 0901 007a 0f74 0c7c 0983  .y...}...z.t.|..
-00002080: 0101 007c 05a0 07a1 0001 0057 0059 0064  ...|.......W.Y.d
-00002090: 007d 097e 0964 0053 0064 007d 097e 0977  .}.~.d.S.d.}.~.w
-000020a0: 0177 0074 0464 0764 0484 007c 007c 0619  .w.t.d.d...|.|..
-000020b0: 0044 0083 0183 017d 0a74 0d7c 027c 0a83  .D.....}.t.|.|..
-000020c0: 025c 027d 0b7d 0c7c 0664 086b 0272 ab74  .\.}.}.|.d.k.r.t
-000020d0: 016a 0e7c 0b69 007c 0ca4 018e 0101 0064  .j.|.i.|.......d
-000020e0: 0053 0074 0183 007d 0874 0f7c 087c 0683  .S.t...}.t.|.|..
-000020f0: 0272 bf74 107c 087c 0683 027c 0b69 007c  .r.t.|.|...|.i.|
-00002100: 0ca4 018e 0101 0064 0053 0074 067c 0b83  .......d.S.t.|..
-00002110: 0164 096b 0272 cc7c 086a 0a7c 0b8e 0001  .d.k.r.|.j.|....
-00002120: 0064 0053 0064 0053 0029 0a4e 7201 0000  .d.S.d.S.).Nr...
-00002130: 0029 03da 0468 656c 70fa 062d 2d68 656c  .)...help..--hel
-00002140: 70fa 022d 6863 0100 0000 0000 0000 0000  p..-hc..........
-00002150: 0000 0200 0000 0500 0000 7300 0000 731c  ..........s...s.
-00002160: 0000 0081 007c 005d 097d 017c 01a0 0064  .....|.].}.|...d
-00002170: 0064 01a1 0256 0001 0071 0264 0253 0029  .d...V...q.d.S.)
-00002180: 0372 1a00 0000 fa01 2d4e 2901 da07 7265  .r......-N)...re
-00002190: 706c 6163 6529 0272 0c00 0000 7266 0000  place).r....rf..
-000021a0: 0072 0b00 0000 720b 0000 0072 0f00 0000  .r....r....r....
-000021b0: 7210 0000 0030 0100 0073 0400 0000 0280  r....0...s......
-000021c0: 1a00 7a17 6d61 696e 2e3c 6c6f 6361 6c73  ..z.main.<locals
-000021d0: 3e2e 3c67 656e 6578 7072 3e72 0500 0000  >.<genexpr>r....
-000021e0: 2902 7292 0000 0072 9300 0000 6301 0000  ).r....r....c...
-000021f0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00002200: 0073 0000 0073 3200 0000 8100 7c00 5d14  .s...s2.....|.].
-00002210: 7d01 7c01 6a00 7401 6a02 6a03 6b03 7216  }.|.j.t.j.j.k.r.
-00002220: 7c01 6a00 7401 6a02 6a04 6b03 7202 7c01  |.j.t.j.j.k.r.|.
-00002230: 6a05 5600 0100 7102 6400 5300 726e 0000  j.V...q.d.S.rn..
-00002240: 0029 06da 046b 696e 6472 1200 0000 da09  .)...kindr......
-00002250: 5061 7261 6d65 7465 72da 0b56 4152 5f4b  Parameter..VAR_K
-00002260: 4559 574f 5244 da0e 5641 525f 504f 5349  EYWORD..VAR_POSI
-00002270: 5449 4f4e 414c 723b 0000 0072 2b00 0000  TIONALr;...r+...
-00002280: 720b 0000 0072 0b00 0000 720f 0000 0072  r....r....r....r
-00002290: 1000 0000 4901 0000 7310 0000 0002 8004  ....I...s.......
-000022a0: 0002 020e 010e 0104 fd06 0304 fc72 5100  .............rQ.
-000022b0: 0000 722f 0000 0029 1172 2100 0000 7204  ..r/...).r!...r.
-000022c0: 0000 0072 4a00 0000 da04 6172 6776 7211  ...rJ.....argvr.
-000022d0: 0000 0072 5000 0000 7230 0000 0072 7000  ...rP...r0...rp.
-000022e0: 0000 7245 0000 0072 0200 0000 7253 0000  ..rE...r....rS..
-000022f0: 00da 0945 7863 6570 7469 6f6e da05 7072  ...Exception..pr
-00002300: 696e 7472 9000 0000 7251 0000 0072 8a00  intr....rQ...r..
-00002310: 0000 7214 0000 0029 0dda 076d 6574 686f  ..r....)...metho
-00002320: 6473 7267 0000 005a 0f72 6177 5f6d 6574  dsrg...Z.raw_met
-00002330: 686f 645f 6172 6773 5a09 6865 6c70 5f61  hod_argsZ.help_a
-00002340: 7267 73da 0761 6374 696f 6e73 7291 0000  rgs..actionsr...
-00002350: 00da 0661 6374 696f 6eda 026d 6472 7200  ...action..mdrr.
-00002360: 0000 da01 6572 6800 0000 5a08 706f 735f  ....erh...Z.pos_
-00002370: 6172 6773 728d 0000 0072 0b00 0000 720b  argsr....r....r.
-00002380: 0000 0072 0f00 0000 da04 6d61 696e 2b01  ...r......main+.
-00002390: 0000 7346 0000 0008 010e 010c 0104 0116  ..sF............
-000023a0: 0106 0118 020c 0112 010c 0208 0418 0108  ................
-000023b0: 010c 0108 0202 0106 0118 010e 0108 0116  ................
-000023c0: 0108 8002 fe08 0506 0208 fe0e 0708 0114  ................
-000023d0: 0106 020a 0118 010c 020e 0104 ff72 a200  .............r..
-000023e0: 0000 726e 0000 0029 1972 4100 0000 da05  ..rn...).rA.....
-000023f0: 7574 696c 7372 0200 0000 7203 0000 0072  utilsr....r....r
-00002400: 7200 0000 7204 0000 0072 1200 0000 7287  r...r....r....r.
-00002410: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
-00002420: 0000 da04 6970 6462 da02 6f73 724a 0000  ....ipdb..osrJ..
-00002430: 0072 2a00 0000 7218 0000 0072 2100 0000  .r*...r....r!...
-00002440: 7245 0000 0072 4f00 0000 7250 0000 0072  rE...rO...rP...r
-00002450: 6500 0000 7211 0000 0072 7800 0000 7290  e...r....rx...r.
-00002460: 0000 0072 a200 0000 720b 0000 0072 0b00  ...r....r....r..
-00002470: 0000 720b 0000 0072 0f00 0000 da08 3c6d  ..r....r......<m
-00002480: 6f64 756c 653e 0100 0000 731e 0000 0004  odule>....s.....
-00002490: 0010 0e0c 0108 0114 0108 0108 0108 010e  ................
-000024a0: 0308 0a14 080e 390e 0f26 7d0c 3c         ......9..&}.<
+00001b00: 1400 1700 7d01 7402 7403 7c00 7c01 8302  ....}.t.t.|.|...
+00001b10: 8301 4400 5d51 5c02 7d07 5c02 7d08 7d09  ..D.]Q\.}.\.}.}.
+00001b20: 7c09 7404 6b02 723d 7c06 7d09 6e10 7c09  |.t.k.r=|.}.n.|.
+00001b30: 7405 6a06 6b02 7245 7c05 7d09 6e08 7407  t.j.k.rE|.}.n.t.
+00001b40: 7c09 6407 8302 724d 7c09 6a08 7d09 6408  |.d...rM|.j.}.d.
+00001b50: 7c08 7600 7261 7c08 a009 6408 a101 5c02  |.v.ra|...d...\.
+00001b60: 7d0a 7d0b 7c09 7c0b 8301 7c02 7c0a 3c00  }.}.|.|...|.|.<.
+00001b70: 6409 7d04 7130 740a 7c09 740b 8302 726a  d.}.q0t.|.t...rj
+00001b80: 7c09 640a 1900 7d09 7c03 a00c 7c09 7c08  |.d...}.|...|.|.
+00001b90: 8301 a101 0100 7c04 7281 740d 640b 7c08  ......|.r.t.d.|.
+00001ba0: 9b00 640c 7c00 7c07 640d 1800 1900 9b00  ..d.|.|.d.......
+00001bb0: 9d04 8301 8201 7130 7c03 7c02 6602 5300  ......q0|.|.f.S.
+00001bc0: 290e 4e46 7263 0000 0063 0100 0000 0000  ).NFrc...c......
+00001bd0: 0000 0000 0000 0300 0000 0900 0000 5300  ..............S.
+00001be0: 0000 7368 0000 0074 0074 0174 0267 037d  ..sh...t.t.t.g.}
+00001bf0: 017c 00a0 03a1 0064 0176 0072 0d64 0053  .|.....d.v.r.d.S
+00001c00: 007c 00a0 03a1 0064 026b 0272 1564 0353  .|.....d.k.r.d.S
+00001c10: 007c 00a0 03a1 0064 046b 0272 1d64 0553  .|.....d.k.r.d.S
+00001c20: 007c 0144 005d 127d 027a 077c 027c 0083  .|.D.].}.z.|.|..
+00001c30: 0157 0002 0001 0053 0004 0074 0479 3101  .W.....S...t.y1.
+00001c40: 0001 0001 0059 0071 1f77 0064 0053 0029  .....Y.q.w.d.S.)
+00001c50: 064e 2902 da04 6e6f 6e65 da04 6e75 6c6c  .N)...none..null
+00001c60: da04 7472 7565 54da 0566 616c 7365 4629  ..trueT..falseF)
+00001c70: 05da 0369 6e74 da05 666c 6f61 7472 2a00  ...int..floatr*.
+00001c80: 0000 da05 6c6f 7765 72da 0a56 616c 7565  ....lower..Value
+00001c90: 4572 726f 7229 0372 6300 0000 da05 7479  Error).rc.....ty
+00001ca0: 7065 73da 0174 720b 0000 0072 0b00 0000  pes..tr....r....
+00001cb0: 720f 0000 00da 0f67 6f6f 645f 6775 6573  r......good_gues
+00001cc0: 735f 7479 7065 fa00 0000 731c 0000 000a  s_type....s.....
+00001cd0: 010c 0104 010c 0104 010c 0104 0108 0102  ................
+00001ce0: 010e 010c 0104 0102 ff04 fd7a 2563 6f6c  ...........z%col
+00001cf0: 6c65 6374 5f61 7267 732e 3c6c 6f63 616c  lect_args.<local
+00001d00: 733e 2e67 6f6f 645f 6775 6573 735f 7479  s>.good_guess_ty
+00001d10: 7065 6301 0000 0000 0000 0000 0000 0001  pec.............
+00001d20: 0000 0002 0000 0053 0000 0073 2800 0000  .......S...s(...
+00001d30: 7c00 a000 a100 6401 6b02 7208 6402 5300  |.....d.k.r.d.S.
+00001d40: 7c00 a000 a100 6403 6b02 7210 6404 5300  |.....d.k.r.d.S.
+00001d50: 7401 6405 8301 8201 2906 4e72 7b00 0000  t.d.....).Nr{...
+00001d60: 5472 7c00 0000 467a 0d4e 6f74 2061 2062  Tr|...Fz.Not a b
+00001d70: 6f6f 6c65 616e 2902 727f 0000 0072 8000  oolean).r....r..
+00001d80: 0000 2901 7263 0000 0072 0b00 0000 720b  ..).rc...r....r.
+00001d90: 0000 0072 0f00 0000 da0c 626f 6f6c 6561  ...r......boolea
+00001da0: 6e5f 7479 7065 0801 0000 730a 0000 000c  n_type....s.....
+00001db0: 0104 010c 0104 0108 027a 2263 6f6c 6c65  .........z"colle
+00001dc0: 6374 5f61 7267 732e 3c6c 6f63 616c 733e  ct_args.<locals>
+00001dd0: 2e62 6f6f 6c65 616e 5f74 7970 65da 085f  .boolean_type.._
+00001de0: 5f61 7267 735f 5f72 2500 0000 5472 0500  _args__r%...Tr..
+00001df0: 0000 7a14 706f 7369 7469 6f6e 616c 2061  ..z.positional a
+00001e00: 7267 756d 656e 7420 7a18 2061 6674 6572  rgument z. after
+00001e10: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+00001e20: 7420 7201 0000 0029 0e72 2a00 0000 7230  t r....).r*...r0
+00001e30: 0000 00da 0965 6e75 6d65 7261 7465 7260  .....enumerater`
+00001e40: 0000 00da 0462 6f6f 6c72 1200 0000 7229  .....boolr....r)
+00001e50: 0000 00da 0768 6173 6174 7472 7285 0000  .....hasattrr...
+00001e60: 0072 3100 0000 da0a 6973 696e 7374 616e  .r1.....isinstan
+00001e70: 6365 7211 0000 00da 0661 7070 656e 6472  cer......appendr
+00001e80: 8000 0000 290c 7267 0000 0072 6800 0000  ....).rg...rh...
+00001e90: da06 6b77 6172 6773 5a0f 706f 7369 7469  ..kwargsZ.positi
+00001ea0: 6f6e 616c 5f61 7267 735a 1770 6f73 6974  onal_argsZ.posit
+00001eb0: 696f 6e61 6c5f 6172 6773 5f73 7461 7274  ional_args_start
+00001ec0: 6564 7283 0000 0072 8400 0000 da01 6972  edr....r......ir
+00001ed0: 6300 0000 723b 0000 0072 7400 0000 da05  c...r;...rt.....
+00001ee0: 7661 6c75 6572 0b00 0000 720b 0000 0072  valuer....r....r
+00001ef0: 0f00 0000 da0c 636f 6c6c 6563 745f 6172  ......collect_ar
+00001f00: 6773 ef00 0000 7336 0000 0004 0704 0104  gs....s6........
+00001f10: 010e 020e 0e10 081a 011a 0208 0106 010a  ................
+00001f20: 0106 010a 0106 0108 010e 010c 0106 010a  ................
+00001f30: 0208 010e 0104 0102 0116 0104 ff02 ff08  ................
+00001f40: 0572 8e00 0000 6300 0000 0000 0000 0000  .r....c.........
+00001f50: 0000 000d 0000 000a 0000 0043 0000 0073  ...........C...s
+00001f60: bc01 0000 7400 7401 8301 7d00 7402 6a03  ....t.t...}.t.j.
+00001f70: 6401 6400 8502 1900 7d01 7c01 6401 6400  d.d.....}.|.d.d.
+00001f80: 8502 1900 7d02 6402 7d03 7404 6403 6404  ....}.d.}.t.d.d.
+00001f90: 8400 7c00 4400 8301 8301 7c03 1700 7d04  ..|.D.....|...}.
+00001fa0: 7405 8300 7d05 7406 7c01 8301 6405 6b02  t...}.t.|...d.k.
+00001fb0: 732d 7c01 6405 1900 7c03 7600 7242 7406  s-|.d...|.v.rBt.
+00001fc0: 7c01 8301 6401 6b04 723c 7c05 a007 7c01  |...d.k.r<|...|.
+00001fd0: 6401 1900 a101 0100 6400 5300 7c05 a007  d.......d.S.|...
+00001fe0: a100 0100 6400 5300 7c01 6405 1900 7d06  ....d.S.|.d...}.
+00001ff0: 7406 7c01 8301 6401 6b04 725c 7c01 6401  t.|...d.k.r\|.d.
+00002000: 1900 6406 7600 725c 7408 7c06 8301 7d07  ..d.v.r\t.|...}.
+00002010: 7409 7c07 8301 0100 6400 5300 7c06 7c00  t.|.....d.S.|.|.
+00002020: 7601 728b 7a0f 7401 8300 7d08 7c08 6a0a  v.r.z.t...}.|.j.
+00002030: 7c01 6401 6400 8502 1900 8e00 0100 5700  |.d.d.........W.
+00002040: 6400 5300 0400 740b 798a 0100 7d09 0100  d.S...t.y...}...
+00002050: 7a0f 740c 7c09 8301 0100 7c05 a007 a100  z.t.|.....|.....
+00002060: 0100 5700 5900 6400 7d09 7e09 6400 5300  ..W.Y.d.}.~.d.S.
+00002070: 6400 7d09 7e09 7701 7700 7404 6407 6404  d.}.~.w.w.t.d.d.
+00002080: 8400 7c00 7c06 1900 4400 8301 8301 7d0a  ..|.|...D.....}.
+00002090: 740d 7c02 7c0a 8302 5c02 7d0b 7d0c 7c06  t.|.|...\.}.}.|.
+000020a0: 6408 6b02 72ab 7401 6a0e 7c0b 6900 7c0c  d.k.r.t.j.|.i.|.
+000020b0: a401 8e01 0100 6400 5300 7401 8300 7d08  ......d.S.t...}.
+000020c0: 740f 7c08 7c06 8302 72bf 7410 7c08 7c06  t.|.|...r.t.|.|.
+000020d0: 8302 7c0b 6900 7c0c a401 8e01 0100 6400  ..|.i.|.......d.
+000020e0: 5300 7406 7c0b 8301 6409 6b02 72cc 7c08  S.t.|...d.k.r.|.
+000020f0: 6a0a 7c0b 8e00 0100 6400 5300 7c08 a011  j.|.....d.S.|...
+00002100: 7402 6a03 6401 1900 7402 6a03 6409 1900  t.j.d...t.j.d...
+00002110: 7402 6a03 640a 1900 a103 0100 6400 5300  t.j.d.......d.S.
+00002120: 290b 4e72 0100 0000 2903 da04 6865 6c70  ).Nr....)...help
+00002130: fa06 2d2d 6865 6c70 fa02 2d68 6301 0000  ..--help..-hc...
+00002140: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00002150: 0073 0000 0073 1c00 0000 8100 7c00 5d09  .s...s......|.].
+00002160: 7d01 7c01 a000 6400 6401 a102 5600 0100  }.|...d.d...V...
+00002170: 7102 6402 5300 2903 721a 0000 00fa 012d  q.d.S.).r......-
+00002180: 4e29 01da 0772 6570 6c61 6365 2902 720c  N)...replace).r.
+00002190: 0000 0072 6600 0000 720b 0000 0072 0b00  ...rf...r....r..
+000021a0: 0000 720f 0000 0072 1000 0000 2f01 0000  ..r....r..../...
+000021b0: 7304 0000 0002 801a 007a 176d 6169 6e2e  s........z.main.
+000021c0: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+000021d0: 723e 7205 0000 0029 0272 9000 0000 7291  r>r....).r....r.
+000021e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000021f0: 0200 0000 0300 0000 7300 0000 7332 0000  ........s...s2..
+00002200: 0081 007c 005d 147d 017c 016a 0074 016a  ...|.].}.|.j.t.j
+00002210: 026a 036b 0372 167c 016a 0074 016a 026a  .j.k.r.|.j.t.j.j
+00002220: 046b 0372 027c 016a 0556 0001 0071 0264  .k.r.|.j.V...q.d
+00002230: 0053 0072 6e00 0000 2906 da04 6b69 6e64  .S.rn...)...kind
+00002240: 7212 0000 00da 0950 6172 616d 6574 6572  r......Parameter
+00002250: da0b 5641 525f 4b45 5957 4f52 44da 0e56  ..VAR_KEYWORD..V
+00002260: 4152 5f50 4f53 4954 494f 4e41 4c72 3b00  AR_POSITIONALr;.
+00002270: 0000 722b 0000 0072 0b00 0000 720b 0000  ..r+...r....r...
+00002280: 0072 0f00 0000 7210 0000 0048 0100 0073  .r....r....H...s
+00002290: 1000 0000 0280 0400 0202 0e01 0e01 04fd  ................
+000022a0: 0603 04fc 7251 0000 0072 2f00 0000 e903  ....rQ...r/.....
+000022b0: 0000 0029 1272 2100 0000 7204 0000 0072  ...).r!...r....r
+000022c0: 4a00 0000 da04 6172 6776 7211 0000 0072  J.....argvr....r
+000022d0: 5000 0000 7230 0000 0072 7000 0000 7245  P...r0...rp...rE
+000022e0: 0000 0072 0200 0000 7253 0000 00da 0945  ...r....rS.....E
+000022f0: 7863 6570 7469 6f6e da05 7072 696e 7472  xception..printr
+00002300: 8e00 0000 7251 0000 0072 8800 0000 7214  ....rQ...r....r.
+00002310: 0000 00da 0a72 756e 5f6d 6f64 756c 6529  .....run_module)
+00002320: 0dda 076d 6574 686f 6473 7267 0000 005a  ...methodsrg...Z
+00002330: 0f72 6177 5f6d 6574 686f 645f 6172 6773  .raw_method_args
+00002340: 5a09 6865 6c70 5f61 7267 73da 0761 6374  Z.help_args..act
+00002350: 696f 6e73 728f 0000 00da 0661 6374 696f  ionsr......actio
+00002360: 6eda 026d 6472 7200 0000 da01 6572 6800  n..mdrr.....erh.
+00002370: 0000 5a08 706f 735f 6172 6773 728b 0000  ..Z.pos_argsr...
+00002380: 0072 0b00 0000 720b 0000 0072 0f00 0000  .r....r....r....
+00002390: da04 6d61 696e 2a01 0000 7346 0000 0008  ..main*...sF....
+000023a0: 010e 010c 0104 0116 0106 0118 020c 0112  ................
+000023b0: 010c 0208 0418 0108 010c 0108 0202 0106  ................
+000023c0: 0118 010e 0108 0116 0108 8002 fe08 0506  ................
+000023d0: 0208 fe0e 0708 0114 0106 020a 0118 010c  ................
+000023e0: 010e 0124 0272 a200 0000 726e 0000 0029  ...$.r....rn...)
+000023f0: 1972 4100 0000 da05 7574 696c 7372 0200  .rA.....utilsr..
+00002400: 0000 7203 0000 0072 7200 0000 7204 0000  ..r....rr...r...
+00002410: 0072 1200 0000 da06 7479 7069 6e67 7206  .r......typingr.
+00002420: 0000 0072 0700 0000 7208 0000 00da 0469  ...r....r......i
+00002430: 7064 62da 026f 7372 4a00 0000 722a 0000  pdb..osrJ...r*..
+00002440: 0072 1800 0000 7221 0000 0072 4500 0000  .r....r!...rE...
+00002450: 724f 0000 0072 5000 0000 7265 0000 0072  rO...rP...re...r
+00002460: 1100 0000 7278 0000 0072 8e00 0000 72a2  ....rx...r....r.
+00002470: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
+00002480: 0000 720f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00002490: 3e01 0000 0073 1e00 0000 0400 100e 0c01  >....s..........
+000024a0: 0801 1401 0801 0801 0801 0e03 080a 1408  ................
+000024b0: 0e39 0e0f 267d 0c3b                      .9..&}.;
```

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May  3 21:24:50 2023 UTC, .py size: 15485 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 22d1 5264 7d3c 0000  o.......".Rd}<..
+00000000: 6f0d 0d0a 0000 0000 8fa6 9664 cc3e 0000  o..........d.>..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 6403 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6402 6404 6c07 6d08 5a08 0100 6402  ..d.d.l.m.Z...d.
 00000070: 6405 6c09 6d0a 5a0a 0100 6402 6406 6c0b  d.l.m.Z...d.d.l.
@@ -102,46 +102,46 @@
 00000650: 0666 6f72 6d61 74da 0945 7863 6570 7469  .format..Excepti
 00000660: 6f6e 2908 7215 0000 005a 096d 6174 655f  on).r....Z.mate_
 00000670: 6a73 6f6e 5a03 6469 63da 0166 5a0a 696e  jsonZ.dic..fZ.in
 00000680: 6974 5f5f 6669 6c65 5a07 666f 6c64 6572  it__fileZ.folder
 00000690: 73da 0666 6f6c 6465 72da 0165 7212 0000  s..folder..er...
 000006a0: 0072 1200 0000 7213 0000 00da 0c69 6e69  .r....r......ini
 000006b0: 745f 7072 6f6a 6563 741c 0000 0073 4800  t_project....sH.
-000006c0: 0000 0c03 0a01 0c01 0802 0a01 0c02 0c01  ................
+000006c0: 0000 0c02 0a01 0c01 0802 0a01 0c02 0c01  ................
 000006d0: 0402 04ff 0c05 1201 1cff 0280 0803 0a01  ................
 000006e0: 0c02 0a01 0e01 0e01 0201 0801 0801 1801  ................
 000006f0: 1001 0c01 0e01 0280 0201 0401 0401 02ff  ................
 00000700: 0aff 0e06 1601 0880 02ff 7a1d 4d6f 6475  ..........z.Modu
 00000710: 6c65 5265 706f 7369 746f 7279 2e69 6e69  leRepository.ini
 00000720: 745f 7072 6f6a 6563 74da 0375 726c 6302  t_project..urlc.
 00000730: 0000 0000 0000 0000 0000 0004 0000 0004  ................
 00000740: 0000 004f 0000 0073 1e00 0000 7c00 6a00  ...O...s....|.j.
 00000750: 6a01 7c01 6701 7c02 a201 5200 6900 7c03  j.|.g.|...R.i.|.
 00000760: a401 8e01 0100 6400 5300 720d 0000 0029  ......d.S.r....)
 00000770: 0272 0f00 0000 da0f 696e 7374 616c 6c5f  .r......install_
 00000780: 7061 636b 6167 6529 0472 1100 0000 7236  package).r....r6
 00000790: 0000 00da 0461 7267 73da 066b 7761 7267  .....args..kwarg
 000007a0: 7372 1200 0000 7212 0000 0072 1300 0000  sr....r....r....
-000007b0: da0b 696e 7374 616c 6c5f 7572 6c47 0000  ..install_urlG..
-000007c0: 0073 0200 0000 1e02 7a1c 4d6f 6475 6c65  .s......z.Module
+000007b0: da0b 696e 7374 616c 6c5f 7572 6c46 0000  ..install_urlF..
+000007c0: 0073 0200 0000 1e01 7a1c 4d6f 6475 6c65  .s......z.Module
 000007d0: 5265 706f 7369 746f 7279 2e69 6e73 7461  Repository.insta
 000007e0: 6c6c 5f75 726c da07 636f 6d6d 616e 6463  ll_url..commandc
 000007f0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
 00000800: 0300 0000 4700 0000 7332 0000 007c 0164  ....G...s2...|.d
 00000810: 016b 0272 0a7c 00a0 00a1 0001 0064 0053  .k.r.|.......d.S
 00000820: 007c 0164 0276 0072 177c 00a0 017c 006a  .|.d.v.r.|...|.j
 00000830: 026a 03a1 0101 0064 0053 0064 0053 0029  .j.....d.S.d.S.)
 00000840: 034e da06 6578 706f 7274 2903 da04 696e  .N..export)...in
 00000850: 6974 da03 6669 78da 0169 2904 da19 5f4d  it..fix..i)..._M
 00000860: 6f64 756c 6552 6570 6f73 6974 6f72 795f  oduleRepository_
 00000870: 5f65 7870 6f72 74da 125f 5f67 656e 6572  _export..__gener
 00000880: 6174 655f 5f69 6e69 745f 5f72 0e00 0000  ate__init__r....
 00000890: 7216 0000 0029 0372 1100 0000 723b 0000  r....).r....r;..
 000008a0: 0072 3800 0000 7212 0000 0072 1200 0000  .r8...r....r....
-000008b0: 7213 0000 00da 0461 7574 6f4b 0000 0073  r......autoK...s
+000008b0: 7213 0000 00da 0461 7574 6f49 0000 0073  r......autoI...s
 000008c0: 0a00 0000 0801 0c01 0801 1201 04ff 7a15  ..............z.
 000008d0: 4d6f 6475 6c65 5265 706f 7369 746f 7279  ModuleRepository
 000008e0: 2e61 7574 6f4e da04 726f 6f74 6302 0000  .autoN..rootc...
 000008f0: 0000 0000 0000 0000 0006 0000 0009 0000  ................
 00000900: 0043 0000 0073 0201 0000 7400 6a01 a002  .C...s....t.j...
 00000910: 7c01 6401 a102 7d02 7400 6a01 a003 7c02  |.d...}.t.j...|.
 00000920: a101 732e 7404 7c02 6402 8302 8f0d 7d03  ..s.t.|.d.....}.
@@ -164,15 +164,15 @@
 00000a30: 5f5f da01 2e29 0a72 2200 0000 7223 0000  __...).r"...r#..
 00000a40: 0072 2a00 0000 7224 0000 0072 2b00 0000  .r*...r$...r+...
 00000a50: da05 7772 6974 6572 2700 0000 da07 6c69  ..writer'.....li
 00000a60: 7374 6469 72da 0569 7364 6972 7241 0000  stdir..isdirrA..
 00000a70: 0029 0672 1100 0000 7243 0000 005a 0869  .).r....rC...Z.i
 00000a80: 6e69 745f 5f70 7972 3200 0000 7233 0000  nit__pyr2...r3..
 00000a90: 0072 2300 0000 7212 0000 0072 1200 0000  .r#...r....r....
-00000aa0: 7213 0000 0072 4100 0000 5100 0000 7324  r....rA...Q...s$
+00000aa0: 7213 0000 0072 4100 0000 4f00 0000 7324  r....rA...O...s$
 00000ab0: 0000 000e 010c 010c 010c 011c ff0e 020e  ................
 00000ac0: 020e 011c 0102 010e 010c 010c 010c 011c  ................
 00000ad0: ff0e 020c 0104 f77a 234d 6f64 756c 6552  .......z#ModuleR
 00000ae0: 6570 6f73 6974 6f72 792e 5f5f 6765 6e65  epository.__gene
 00000af0: 7261 7465 5f5f 696e 6974 5f5f da04 7265  rate__init__..re
 00000b00: 7173 6302 0000 0000 0000 0000 0000 0005  qsc.............
 00000b10: 0000 0005 0000 0043 0000 0073 4a00 0000  .......C...sJ...
@@ -190,15 +190,15 @@
 00000bd0: 6178 5f72 656c 6561 7365 732e 6874 6d6c  ax_releases.html
 00000be0: 2902 da05 746f 7263 68da 036a 6178 724b  )...torch..jaxrK
 00000bf0: 0000 0072 4c00 0000 2902 da03 7365 74da  ...rL...)...set.
 00000c00: 0361 6464 2905 7211 0000 0072 4a00 0000  .add).r....rJ...
 00000c10: da04 7572 6c73 da07 696e 6465 7865 73da  ..urls..indexes.
 00000c20: 0372 6571 7212 0000 0072 1200 0000 7213  .reqr....r....r.
 00000c30: 0000 005a 125f 5f70 6172 7365 5f69 6e64  ...Z.__parse_ind
-00000c40: 6578 5f75 726c 7363 0000 0073 1600 0000  ex_urlsc...s....
+00000c40: 6578 5f75 726c 7361 0000 0073 1600 0000  ex_urlsa...s....
 00000c50: 0202 0201 06fe 0604 0801 0801 0e01 0801  ................
 00000c60: 0e01 0280 0402 7a23 4d6f 6475 6c65 5265  ......z#ModuleRe
 00000c70: 706f 7369 746f 7279 2e5f 5f70 6172 7365  pository.__parse
 00000c80: 5f69 6e64 6578 5f75 726c 7372 2300 0000  _index_urlsr#...
 00000c90: 6302 0000 0000 0000 0000 0000 0008 0000  c...............
 00000ca0: 0008 0000 0003 0000 0073 4601 0000 7400  .........sF...t.
 00000cb0: 7401 6a02 a003 7c01 a101 6401 8302 8f0c  t.j...|...d.....
@@ -221,526 +221,544 @@
 00000dc0: 7c02 a009 7c07 a101 0100 7187 5700 6400  |...|.....q.W.d.
 00000dd0: 0400 0400 8303 0100 6400 5300 3100 739a  ........d.S.1.s.
 00000de0: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
 00000df0: 6400 5300 290a 4eda 0172 6301 0000 0000  d.S.).N..rc.....
 00000e00: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
 00000e10: 0000 0073 2800 0000 6700 7c00 5d10 7d01  ...s(...g.|.].}.
 00000e20: 6400 7c01 7601 7212 6401 7c01 7601 7212  d.|.v.r.d.|.v.r.
-00000e30: 6402 7c01 7601 7202 7c01 9102 7102 5300  d.|.v.r.|...q.S.
-00000e40: 2903 7a0a 2e65 6767 3e3d 696e 666f 7a0a  ).z..egg>=infoz.
-00000e50: 2e65 6767 3d3d 696e 666f 7a0a 2e65 6767  .egg==infoz..egg
-00000e60: 7e3d 696e 666f 7212 0000 00a9 02da 022e  ~=infor.........
-00000e70: 30da 046c 696e 6572 1200 0000 7212 0000  0..liner....r...
-00000e80: 0072 1300 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-00000e90: 703e 7500 0000 730e 0000 0006 0002 0208  p>u...s.........
-00000ea0: 0108 0108 0102 fc06 047a 444d 6f64 756c  .........zDModul
-00000eb0: 6552 6570 6f73 6974 6f72 792e 5f5f 6164  eRepository.__ad
-00000ec0: 645f 696e 6465 785f 7572 6c5f 746f 5f72  d_index_url_to_r
-00000ed0: 6571 7569 7265 6d65 6e74 732e 3c6c 6f63  equirements.<loc
-00000ee0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e7a  als>.<listcomp>z
-00000ef0: 075c 2b63 755c 642b 6301 0000 0000 0000  .\+cu\d+c.......
-00000f00: 0000 0000 0002 0000 0006 0000 0013 0000  ................
-00000f10: 0073 1800 0000 6700 7c00 5d08 7d01 8800  .s....g.|.].}...
-00000f20: a000 6400 7c01 a102 9102 7102 5300 2901  ..d.|.....q.S.).
-00000f30: 7244 0000 0029 01da 0373 7562 7253 0000  rD...)...subrS..
-00000f40: 00a9 01da 0572 6567 6578 7212 0000 0072  .....regexr....r
-00000f50: 1300 0000 7256 0000 0080 0000 00f3 0200  ....rV..........
-00000f60: 0000 1800 7201 0000 0072 1700 0000 7a12  ....r....r....z.
-00000f70: 2d2d 6578 7472 612d 696e 6465 782d 7572  --extra-index-ur
-00000f80: 6c20 da01 0a29 0a72 2b00 0000 7222 0000  l ...).r+...r"..
-00000f90: 0072 2300 0000 722a 0000 00da 0972 6561  .r#...r*.....rea
-00000fa0: 646c 696e 6573 da03 6c65 6eda 0272 65da  dlines..len..re.
-00000fb0: 0763 6f6d 7069 6c65 da23 5f4d 6f64 756c  .compile.#_Modul
-00000fc0: 6552 6570 6f73 6974 6f72 795f 5f70 6172  eRepository__par
-00000fd0: 7365 5f69 6e64 6578 5f75 726c 7372 4700  se_index_urlsrG.
-00000fe0: 0000 2908 7211 0000 0072 2300 0000 7232  ..).r....r#...r2
-00000ff0: 0000 00da 056c 696e 6573 5a09 6c69 6e65  .....linesZ.line
-00001000: 636f 756e 7472 4f00 0000 7236 0000 0072  countrO...r6...r
-00001010: 5500 0000 7212 0000 0072 5800 0000 7213  U...r....rX...r.
-00001020: 0000 005a 1f5f 5f61 6464 5f69 6e64 6578  ...Z.__add_index
-00001030: 5f75 726c 5f74 6f5f 7265 7175 6972 656d  _url_to_requirem
-00001040: 656e 7473 7100 0000 7332 0000 0014 010a  entsq...s2......
-00001050: 011c ff08 0206 0102 0206 fe0a 0a12 010a  ................
-00001060: 020c 0114 0108 0114 0108 010c 0102 ff22  ..............."
-00001070: fd0c 0514 0108 010c 0102 ff22 ff04 ff7a  ..........."...z
-00001080: 304d 6f64 756c 6552 6570 6f73 6974 6f72  0ModuleRepositor
-00001090: 792e 5f5f 6164 645f 696e 6465 785f 7572  y.__add_index_ur
-000010a0: 6c5f 746f 5f72 6571 7569 7265 6d65 6e74  l_to_requirement
-000010b0: 7363 0200 0000 0000 0000 0000 0000 0500  sc..............
-000010c0: 0000 0600 0000 4300 0000 738a 0000 0074  ......C...s....t
-000010d0: 00a0 017c 01a1 0144 005d 3d7d 027c 02a0  ...|...D.]=}.|..
-000010e0: 0264 01a1 0173 117c 02a0 0264 02a1 0172  .d...s.|...d...r
-000010f0: 1271 0574 006a 03a0 047c 017c 02a1 027d  .q.t.j...|.|...}
-00001100: 0374 006a 03a0 057c 03a1 0172 4274 006a  .t.j...|...rBt.j
-00001110: 03a0 047c 017c 0264 03a1 037d 0474 006a  ...|.|.d...}.t.j
-00001120: 03a0 067c 04a1 0173 2e71 057c 0264 0476  ...|...s.q.|.d.v
-00001130: 0072 387c 006a 076a 087c 0176 0073 3d7c  .r8|.j.j.|.v.s=|
-00001140: 00a0 097c 03a1 0101 007c 00a0 0a7c 03a1  ...|.....|...|..
-00001150: 0101 0071 0564 0053 0029 054e 7246 0000  ...q.d.S.).NrF..
-00001160: 00da 025f 5f72 1b00 0000 2904 7220 0000  ...__r....).r ..
-00001170: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00001180: 290b 7222 0000 0072 4800 0000 da0a 7374  ).r"...rH.....st
-00001190: 6172 7473 7769 7468 7223 0000 0072 2a00  artswithr#...r*.
-000011a0: 0000 7249 0000 0072 2400 0000 720e 0000  ..rI...r$...r...
-000011b0: 0072 1600 0000 da2c 5f4d 6f64 756c 6552  .r.....,_ModuleR
-000011c0: 6570 6f73 6974 6f72 795f 5f67 656e 6572  epository__gener
-000011d0: 6174 655f 7069 705f 7265 7175 6972 656d  ate_pip_requirem
-000011e0: 656e 7473 da29 5f4d 6f64 756c 6552 6570  ents.)_ModuleRep
-000011f0: 6f73 6974 6f72 795f 5f67 656e 6572 6174  ository__generat
-00001200: 655f 6465 7073 5f69 6e5f 6465 7074 68a9  e_deps_in_depth.
-00001210: 0572 1100 0000 5a09 726f 6f74 5f70 6174  .r....Z.root_pat
-00001220: 68da 0364 6972 7223 0000 005a 0a69 6e69  h..dirr#...Z.ini
-00001230: 745f 5f70 6174 6872 1200 0000 7212 0000  t__pathr....r...
-00001240: 0072 1300 0000 5a18 5f5f 6765 6e65 7261  .r....Z.__genera
-00001250: 7465 5f64 6570 735f 696e 5f64 6570 7468  te_deps_in_depth
-00001260: 8e00 0000 731c 0000 000e 0414 0102 010e  ....s...........
-00001270: 010c 0110 020c 0102 0108 030c 010a 020a  ................
-00001280: 0202 8004 f07a 294d 6f64 756c 6552 6570  .....z)ModuleRep
-00001290: 6f73 6974 6f72 792e 5f5f 6765 6e65 7261  ository.__genera
-000012a0: 7465 5f64 6570 735f 696e 5f64 6570 7468  te_deps_in_depth
-000012b0: 6301 0000 0000 0000 0000 0000 0012 0000  c...............
-000012c0: 000b 0000 000f 0000 0073 4604 0000 7c00  .........sF...|.
-000012d0: a000 a100 0100 7c00 a001 a100 7d03 6700  ......|.....}.g.
-000012e0: 7d04 7c03 a002 a100 4400 5d2b 5c02 8900  }.|.....D.]+\...
-000012f0: 7d05 7403 7c05 8301 7401 7500 7225 7c04  }.t.|...t.u.r%|.
-00001300: a004 8700 6601 6401 6402 8408 7c05 4400  ....f.d.d...|.D.
-00001310: 8301 a101 0100 710e 7403 7c05 8301 7405  ......q.t.|...t.
-00001320: 7500 7239 7c04 a004 8700 6601 6403 6402  u.r9|.....f.d.d.
-00001330: 8408 7c05 a006 a100 4400 8301 a101 0100  ..|.....D.......
-00001340: 710e 6404 6402 8400 7c04 4400 8301 7d04  q.d.d...|.D...}.
-00001350: 7407 8300 7d06 7408 8300 7d07 7c07 a009  t...}.t...}.|...
-00001360: 6405 a101 6406 1900 7d08 7c07 a009 6405  d...d...}.|...d.
-00001370: a101 6407 1900 7d09 7c04 4400 5d47 7d0a  ..d...}.|.D.]G}.
-00001380: 7c07 9b00 7c00 6a0a 6a0b 9b00 6405 7c0a  |...|.j.j...d.|.
-00001390: 6408 1900 9b00 6405 7c0a 6409 1900 9b00  d.....d.|.d.....
-000013a0: 9d06 7c0a 640a 3c00 7c08 9b00 6405 7c09  ..|.d.<.|...d.|.
-000013b0: 9b00 6405 7c00 6a0a 6a0b 9b00 6405 7c0a  ..d.|.j.j...d.|.
-000013c0: 6408 1900 9b00 6405 7c0a 6409 1900 9b00  d.....d.|.d.....
-000013d0: 9d09 7c0a 640b 3c00 7c09 7c00 6a0a 6a0b  ..|.d.<.|.|.j.j.
-000013e0: 6b02 729e 7c08 9b00 6405 7c09 9b00 6405  k.r.|...d.|...d.
-000013f0: 7c0a 6408 1900 9b00 6405 7c0a 6409 1900  |.d.....d.|.d...
-00001400: 9b00 9d07 7c0a 640b 3c00 7157 7c04 4400  ....|.d.<.qW|.D.
-00001410: 5d91 7d0a 740c 6a0d a00e 7c00 6a0a 6a0b  ].}.t.j...|.j.j.
-00001420: 7c0a 6408 1900 7c0a 6409 1900 640c a104  |.d...|.d...d...
-00001430: 7d0b 740c 6a0d a00e 7c00 6a0a 6a0b 7c0a  }.t.j...|.j.j.|.
-00001440: 6408 1900 7c0a 6409 1900 640d a104 7d0c  d...|.d...d...}.
-00001450: 740c 6a0d a00f 7c0b a101 72e2 7410 7c0b  t.j...|...r.t.|.
-00001460: 640e 8302 8f0e 7d0d 7c0d a011 a100 7c0a  d.....}.|.....|.
-00001470: 640f 3c00 5700 6400 0400 0400 8303 0100  d.<.W.d.........
-00001480: 6e08 3100 73dd 7701 0100 0100 0100 5900  n.1.s.w.......Y.
-00001490: 0100 740c 6a0d a00f 7c0c a101 9001 721b  ..t.j...|.....r.
-000014a0: 7410 7c0c 640e 8302 8f24 7d0d 640f 7c0a  t.|.d....$}.d.|.
-000014b0: 7600 9001 7202 7c0a 640f 0500 1900 7412  v...r.|.d.....t.
-000014c0: a013 7c0d a101 640f 1900 3700 0300 3c00  ..|...d...7...<.
-000014d0: 6e09 7412 a013 7c0d a101 640f 1900 7c0a  n.t...|...d...|.
-000014e0: 640f 3c00 5700 6400 0400 0400 8303 0100  d.<.W.d.........
-000014f0: 6e09 3100 9001 7316 7701 0100 0100 0100  n.1...s.w.......
-00001500: 5900 0100 640f 7c0a 7600 9001 722b 6410  Y...d.|.v...r+d.
-00001510: 6402 8400 7c0a 640f 1900 4400 8301 7c0a  d...|.d...D...|.
-00001520: 640f 3c00 7c06 a014 7c0a 640f 1900 a101  d.<.|...|.d.....
-00001530: 0100 71a1 6411 6402 8400 7c06 4400 8301  ..q.d.d...|.D...
-00001540: 7d06 7415 7c06 6412 6413 8400 6414 6415  }.t.|.d.d...d.d.
-00001550: 8d03 7d06 6416 6402 8400 7c06 4400 8301  ..}.d.d...|.D...
-00001560: 7d06 7410 640c 6417 8302 8f15 7d0d 7c06  }.t.d.d.....}.|.
-00001570: 4400 5d0a 7d0e 7c0d a016 7c0e 6418 1700  D.].}.|...|.d...
-00001580: a101 0100 9001 7152 5700 6400 0400 0400  ......qRW.d.....
-00001590: 8303 0100 6e09 3100 9001 7368 7701 0100  ....n.1...shw...
-000015a0: 0100 0100 5900 0100 7c04 7d0f 6700 7d0f  ....Y...|.}.g.}.
-000015b0: 7410 6419 6417 8302 8f10 7d0d 7412 6a17  t.d.d.....}.t.j.
-000015c0: 7c04 7c0d 6407 641a 8d03 0100 5700 6400  |.|.d.d.....W.d.
-000015d0: 0400 0400 8303 0100 6e09 3100 9001 738a  ........n.1...s.
-000015e0: 7701 0100 0100 0100 5900 0100 7c04 4400  w.......Y...|.D.
-000015f0: 5d42 7d0a 640f 7c0a 7600 9001 72c0 6700  ]B}.d.|.v...r.g.
-00001600: 7d10 7c0a 640f 1900 4400 5d0f 7d0e 641b  }.|.d...D.].}.d.
-00001610: 7c0e 7600 9001 72a7 9001 719e 7c10 a004  |.v...r...q.|...
-00001620: 7c0e a101 0100 9001 719e 7c0f a004 7c0a  |.......q.|...|.
-00001630: 6409 1900 7c0a 6408 1900 7c0a 640b 1900  d...|.d...|.d...
-00001640: 7c10 641c 9c04 a101 0100 9001 7191 7c0f  |.d.........q.|.
-00001650: a004 7c0a 6409 1900 7c0a 6408 1900 7c0a  ..|.d...|.d...|.
-00001660: 640b 1900 7c0a 640f 1900 641c 9c04 a101  d...|.d...d.....
-00001670: 0100 9001 7191 7418 6a18 7c0f 641d 641e  ....q.t.j.|.d.d.
-00001680: 641f 6420 8d04 7d11 7418 6a18 7c04 641d  d.d ..}.t.j.|.d.
-00001690: 6421 6422 6414 6423 8d05 7d04 7410 6424  d!d"d.d#..}.t.d$
-000016a0: 6417 8302 8f0d 7d0d 7c0d a016 7c04 a101  d.....}.|...|...
-000016b0: 0100 5700 6400 0400 0400 8303 0100 6e09  ..W.d.........n.
-000016c0: 3100 9001 73fd 7701 0100 0100 0100 5900  1...s.w.......Y.
-000016d0: 0100 7410 6425 6417 8302 8f0d 7d0d 7c0d  ..t.d%d.....}.|.
-000016e0: a016 7c11 a101 0100 5700 6400 0400 0400  ..|.....W.d.....
-000016f0: 8303 0100 6e09 3100 9002 7318 7701 0100  ....n.1...s.w...
-00001700: 0100 0100 5900 0100 7419 6426 8301 0100  ....Y...t.d&....
-00001710: 6400 5300 2927 4e63 0100 0000 0000 0000  d.S.)'Nc........
-00001720: 0000 0000 0200 0000 0500 0000 1300 0000  ................
-00001730: f316 0000 0067 007c 005d 077d 0188 007c  .....g.|.].}...|
-00001740: 0164 009c 0291 0271 0253 00a9 0129 02da  .d.....q.S...)..
-00001750: 0474 7970 65da 046e 616d 6572 1200 0000  .type..namer....
-00001760: a902 7254 0000 0072 6b00 0000 a901 da03  ..rT...rk.......
-00001770: 6b65 7972 1200 0000 7213 0000 0072 5600  keyr....r....rV.
-00001780: 0000 ae00 0000 7302 0000 0016 007a 2d4d  ......s......z-M
-00001790: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
-000017a0: 5f5f 6578 706f 7274 2e3c 6c6f 6361 6c73  __export.<locals
-000017b0: 3e2e 3c6c 6973 7463 6f6d 703e 6301 0000  >.<listcomp>c...
-000017c0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-000017d0: 0013 0000 0072 6800 0000 7269 0000 0072  .....rh...ri...r
-000017e0: 1200 0000 726c 0000 0072 6d00 0000 7212  ....rl...rm...r.
-000017f0: 0000 0072 1300 0000 7256 0000 00b0 0000  ...r....rV......
-00001800: 0073 0600 0000 0600 0201 0eff 6301 0000  .s..........c...
-00001810: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00001820: 0053 0000 00f3 1a00 0000 6700 7c00 5d09  .S........g.|.].
-00001830: 7d01 7c01 4400 5d04 7d02 7c02 9103 7106  }.|.D.].}.|...q.
-00001840: 7102 5300 7212 0000 0072 1200 0000 a903  q.S.r....r......
-00001850: 7254 0000 005a 0773 7562 6c69 7374 da04  rT...Z.sublist..
-00001860: 6974 656d 7212 0000 0072 1200 0000 7213  itemr....r....r.
-00001870: 0000 0072 5600 0000 b500 0000 f302 0000  ...rV...........
-00001880: 001a 00fa 012f e903 0000 0072 1800 0000  ...../.....r....
-00001890: 726a 0000 0072 6b00 0000 7236 0000 00da  rj...rk...r6....
-000018a0: 0973 686f 7274 5f75 726c fa10 7265 7175  .short_url..requ
-000018b0: 6972 656d 656e 7473 2e74 7874 fa11 6465  irements.txt..de
-000018c0: 7065 6e64 656e 6369 6573 2e6a 736f 6e72  pendencies.jsonr
-000018d0: 5200 0000 da0c 6465 7065 6e64 656e 6369  R.....dependenci
-000018e0: 6573 6301 0000 0000 0000 0000 0000 0002  esc.............
-000018f0: 0000 0006 0000 0053 0000 00f3 1800 0000  .......S........
-00001900: 6700 7c00 5d08 7d01 7c01 a000 6400 6401  g.|.].}.|...d.d.
-00001910: a102 9102 7102 5300 2902 725b 0000 0072  ....q.S.).r[...r
-00001920: 4400 0000 a901 da07 7265 706c 6163 65a9  D.......replace.
-00001930: 0272 5400 0000 da03 6465 7072 1200 0000  .rT.....depr....
-00001940: 7212 0000 0072 1300 0000 7256 0000 00e4  r....r....rV....
-00001950: 0000 0073 0600 0000 0600 0c01 06ff 6301  ...s..........c.
-00001960: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001970: 0000 0053 0000 00f3 1800 0000 6700 7c00  ...S........g.|.
-00001980: 5d08 7d01 6400 7c01 7601 7202 7c01 9102  ].}.d.|.v.r.|...
-00001990: 7102 5300 2901 7a0e 6874 7470 733a 2f2f  q.S.).z.https://
-000019a0: 6769 7468 7562 7212 0000 0072 7c00 0000  githubr....r|...
-000019b0: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000019c0: 5600 0000 eb00 0000 725a 0000 0063 0100  V.......rZ...c..
-000019d0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000019e0: 0000 5300 0000 7308 0000 0064 017c 0076  ..S...s....d.|.v
-000019f0: 0053 0029 024e 7a11 2d2d 6578 7472 612d  .S.).Nz.--extra-
-00001a00: 696e 6465 782d 7572 6c72 1200 0000 2901  index-urlr....).
-00001a10: da01 7872 1200 0000 7212 0000 0072 1300  ..xr....r....r..
-00001a20: 0000 da08 3c6c 616d 6264 613e ee00 0000  ....<lambda>....
-00001a30: 7302 0000 0008 007a 2b4d 6f64 756c 6552  s......z+ModuleR
-00001a40: 6570 6f73 6974 6f72 792e 5f5f 6578 706f  epository.__expo
-00001a50: 7274 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  rt.<locals>.<lam
-00001a60: 6264 613e 5429 0272 6e00 0000 da07 7265  bda>T).rn.....re
-00001a70: 7665 7273 6563 0100 0000 0000 0000 0000  versec..........
-00001a80: 0000 0200 0000 0400 0000 5300 0000 7328  ..........S...s(
-00001a90: 0000 0067 007c 005d 107d 017c 0164 006b  ...g.|.].}.|.d.k
-00001aa0: 0373 107c 0164 016b 0373 107c 0164 026b  .s.|.d.k.s.|.d.k
-00001ab0: 0372 027c 0191 0271 0253 0029 0372 5b00  .r.|...q.S.).r[.
-00001ac0: 0000 fa01 2072 4400 0000 7212 0000 0072  .... rD...r....r
-00001ad0: 7c00 0000 7212 0000 0072 1200 0000 7213  |...r....r....r.
-00001ae0: 0000 0072 5600 0000 f000 0000 7302 0000  ...rV.......s...
-00001af0: 0028 0072 1700 0000 725b 0000 007a 0c65  .(.r....r[...z.e
-00001b00: 7870 6f72 7473 2e6a 736f 6e72 1900 0000  xports.jsonr....
-00001b10: 7a07 2d2d 6578 7472 6129 0472 6b00 0000  z.--extra).rk...
-00001b20: 726a 0000 0072 7500 0000 7278 0000 00da  rj...ru...rx....
-00001b30: 046b 6579 73da 056c 6174 6578 da05 6e65  .keys..latex..ne
-00001b40: 7665 7229 03da 0768 6561 6465 7273 da08  ver)...headers..
-00001b50: 7461 626c 6566 6d74 da09 7368 6f77 696e  tablefmt..showin
-00001b60: 6465 785a 0667 6974 6875 62da 0661 6c77  dexZ.github..alw
-00001b70: 6179 7329 0472 8600 0000 7287 0000 0072  ays).r....r....r
-00001b80: 8800 0000 5a10 6469 7361 626c 655f 6e75  ....Z.disable_nu
-00001b90: 6d70 6172 7365 7a09 6578 706f 7274 2e6d  mparsez.export.m
-00001ba0: 647a 0b65 7870 6f72 7473 2e74 6578 7a15  dz.exports.texz.
-00001bb0: 4578 706f 7274 6564 2074 6f20 6578 706f  Exported to expo
-00001bc0: 7274 2e6d 6429 1ada 285f 4d6f 6475 6c65  rt.md)..(_Module
-00001bd0: 5265 706f 7369 746f 7279 5f5f 6765 6e65  Repository__gene
-00001be0: 7261 7465 5f73 7562 5f70 6970 5f72 6571  rate_sub_pip_req
-00001bf0: 73da 046c 6973 74da 0569 7465 6d73 726a  s..list..itemsrj
-00001c00: 0000 00da 0661 7070 656e 64da 0464 6963  .....append..dic
-00001c10: 7472 8300 0000 724d 0000 0072 0500 0000  tr....rM...r....
-00001c20: da05 7370 6c69 7472 0e00 0000 7216 0000  ..splitr....r...
-00001c30: 0072 2200 0000 7223 0000 0072 2a00 0000  .r"...r#...r*...
-00001c40: 7224 0000 0072 2b00 0000 725c 0000 0072  r$...r+...r\...r
-00001c50: 2c00 0000 da04 6c6f 6164 da06 7570 6461  ,.....load..upda
-00001c60: 7465 da06 736f 7274 6564 7247 0000 0072  te..sortedrG...r
-00001c70: 2d00 0000 da08 7461 6275 6c61 7465 7227  -.....tabulater'
-00001c80: 0000 0029 1272 1100 0000 7238 0000 0072  ...).r....r8...r
-00001c90: 3900 0000 da07 6d6f 6475 6c65 73da 0574  9.....modules..t
-00001ca0: 6162 6c65 da05 7661 6c75 65da 0464 6570  able..value..dep
-00001cb0: 735a 0862 6173 655f 7572 6c5a 0975 7365  sZ.base_urlZ.use
-00001cc0: 725f 6e61 6d65 5a09 7265 706f 5f6e 616d  r_nameZ.repo_nam
-00001cd0: 6572 7100 0000 7223 0000 005a 0864 6570  erq...r#...Z.dep
-00001ce0: 5f70 6174 6872 3200 0000 727d 0000 005a  _pathr2...r}...Z
-00001cf0: 066c 7461 626c 655a 076e 6577 5f64 6570  .ltableZ.new_dep
-00001d00: 5a0b 6c61 7465 785f 7461 626c 6572 1200  Z.latex_tabler..
-00001d10: 0000 726d 0000 0072 1300 0000 5a08 5f5f  ..rm...r....Z.__
-00001d20: 6578 706f 7274 a400 0000 73dc 0000 0008  export....s.....
-00001d30: 0208 0204 0210 020c 011a 010c 010e 0106  ................
-00001d40: 0108 ff02 800e 0506 0306 020e 010e 0108  ................
-00001d50: 0122 0402 fe02 0102 ff2a 0502 fe02 0102  .".......*......
-00001d60: ff0c 0520 0502 fe02 0102 ff02 8008 0506  ... ............
-00001d70: 0114 0104 ff06 0314 0104 ff0c 040c 010e  ................
-00001d80: 011c ff0e 020c 010a 011c 0112 0202 801e  ................
-00001d90: fc0a 0806 0106 010a ff10 040e 0302 020a  ................
-00001da0: 0106 ff0e 030c 0308 0112 0102 ff1e ff04  ................
-00001db0: 0904 0a0c 0412 011e ff08 030a 0204 020c  ................
-00001dc0: 010a 0104 010e 0104 0106 0206 0106 0102  ................
-00001dd0: 0104 fc08 ff04 0906 0206 0106 0106 0104  ................
-00001de0: fc08 ff04 0b02 0102 0102 0102 0106 fc04  ................
-00001df0: 0802 0102 0102 0102 0102 0106 fb0c 0a0c  ................
-00001e00: 011e ff0c 030c 011e ff0c 037a 194d 6f64  ...........z.Mod
-00001e10: 756c 6552 6570 6f73 6974 6f72 792e 5f5f  uleRepository.__
-00001e20: 6578 706f 7274 6301 0000 0000 0000 0000  exportc.........
-00001e30: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
-00001e40: 8a00 0000 7c00 6a00 6a01 7d01 7c00 a002  ....|.j.j.}.|...
-00001e50: 7c01 a101 0100 7403 a004 6401 a101 4400  |.....t...d...D.
-00001e60: 5d34 7d02 7c02 a005 6401 a101 7320 7c02  ]4}.|...d...s |.
-00001e70: a005 6402 a101 7320 7c02 7c00 6a00 6a01  ..d...s |.|.j.j.
-00001e80: 6b02 7221 710e 7403 6a06 a007 6401 7c02  k.r!q.t.j...d.|.
-00001e90: a102 7d03 7403 6a06 a008 7c03 a101 7242  ..}.t.j...|...rB
-00001ea0: 7403 6a06 a007 6401 7c02 6403 a103 7d04  t.j...d.|.d...}.
-00001eb0: 7403 6a06 a009 7c04 a101 733d 710e 7c00  t.j...|...s=q.|.
-00001ec0: a00a 7c03 a101 0100 710e 6400 5300 2904  ..|.....q.d.S.).
-00001ed0: 4e72 4600 0000 7262 0000 0072 1b00 0000  NrF...rb...r....
-00001ee0: 290b 720e 0000 0072 1600 0000 7265 0000  ).r....r....re..
-00001ef0: 0072 2200 0000 7248 0000 0072 6300 0000  .r"...rH...rc...
-00001f00: 7223 0000 0072 2a00 0000 7249 0000 0072  r#...r*...rI...r
-00001f10: 2400 0000 7264 0000 0072 6600 0000 7212  $...rd...rf...r.
-00001f20: 0000 0072 1200 0000 7213 0000 005a 175f  ...r....r....Z._
-00001f30: 5f67 656e 6572 6174 655f 7375 625f 7069  _generate_sub_pi
-00001f40: 705f 7265 7173 4401 0000 7322 0000 0008  p_reqsD...s"....
-00001f50: 020a 010e 0208 0202 ff08 0202 fe0c 0302  ................
-00001f60: 020e 010c 0110 020c 0102 010a 0102 8004  ................
-00001f70: f37a 284d 6f64 756c 6552 6570 6f73 6974  .z(ModuleReposit
-00001f80: 6f72 792e 5f5f 6765 6e65 7261 7465 5f73  ory.__generate_s
-00001f90: 7562 5f70 6970 5f72 6571 7363 0200 0000  ub_pip_reqsc....
-00001fa0: 0000 0000 0000 0000 0e00 0000 0a00 0000  ................
-00001fb0: 0300 0000 736e 0200 0064 0164 0284 0074  ....sn...d.d...t
-00001fc0: 00a0 0188 01a1 0144 0083 017d 0264 0364  .......D...}.d.d
-00001fd0: 0284 007c 0244 0083 0164 0464 0284 0074  ...|.D...d.d...t
-00001fe0: 00a0 0188 01a1 0144 0083 0117 0089 0087  .......D........
-00001ff0: 0166 0164 0564 0284 087c 0244 0083 017d  .f.d.d...|.D...}
-00002000: 0374 0264 0664 0284 007c 0344 0083 0183  .t.d.d...|.D....
-00002010: 017d 0387 0066 0164 0764 0284 087c 0344  .}...f.d.d...|.D
-00002020: 0083 017d 0374 0383 007d 047c 0464 0075  ...}.t...}.|.d.u
-00002030: 0072 4374 0464 0883 0101 0064 0053 0074  .rCt.d.....d.S.t
-00002040: 0283 007d 057c 0344 005d 5d7d 067c 06a0  ...}.|.D.]]}.|..
-00002050: 0564 09a1 0172 5071 487c 006a 066a 0767  .d...rPqH|.j.j.g
-00002060: 017c 06a0 0864 0aa1 01a2 017d 077c 0764  .|...d.....}.|.d
-00002070: 0b19 0064 0917 007c 0764 0b3c 0067 007c  ...d...|.d.<.g.|
-00002080: 06a0 0864 0aa1 01a2 017d 0874 006a 09a0  ...d.....}.t.j..
-00002090: 0a74 006a 096a 0b7c 078e 00a1 0172 7d64  .t.j.j.|.....r}d
-000020a0: 0ca0 0b7c 0764 0064 0b85 0219 00a1 017d  ...|.d.d.......}
-000020b0: 096e 1d74 006a 09a0 0a74 006a 096a 0b7c  .n.t.j...t.j.j.|
-000020c0: 088e 00a1 0172 8e7c 0864 0d19 0064 0c17  .....r.|.d...d..
-000020d0: 007d 096e 0c7c 006a 066a 0764 0c17 007c  .}.n.|.j.j.d...|
-000020e0: 06a0 0c64 0a64 0ca1 0217 007d 097c 0472  ...d.d.....}.|.r
-000020f0: a07c 047c 0917 007d 097c 05a0 0d7c 09a1  .|.|...}.|...|..
-00002100: 0101 0071 4874 0e7c 0583 0164 0d6b 0272  ...qHt.|...d.k.r
-00002110: ae64 0053 007a 3774 006a 09a0 0b88 0164  .d.S.z7t.j.....d
-00002120: 0ea1 027d 0a74 006a 09a0 0a7c 0aa1 0172  ...}.t.j...|...r
-00002130: e274 0f7c 0a64 0f83 028f 187d 0b74 10a0  .t.|.d.....}.t..
-00002140: 117c 0ba1 017d 0a64 107c 0a76 0072 d07c  .|...}.d.|.v.r.|
-00002150: 0a64 1019 007d 0c6e 0269 007d 0c57 0064  .d...}.n.i.}.W.d
-00002160: 0004 0004 0083 0301 006e 0831 0073 dc77  .........n.1.s.w
-00002170: 0101 0001 0001 0059 0001 006e 0269 007d  .......Y...n.i.}
-00002180: 0c57 006e 1d04 0074 1290 0179 0201 007d  .W.n...t...y...}
-00002190: 0d01 007a 1074 0464 1188 019b 0064 129d  ...z.t.d.....d..
-000021a0: 0383 0101 0069 007d 0c57 0059 0064 007d  .....i.}.W.Y.d.}
-000021b0: 0d7e 0d6e 0564 007d 0d7e 0d77 0177 0074  .~.n.d.}.~.w.w.t
-000021c0: 0f74 006a 09a0 0b88 0164 0ea1 0264 1383  .t.j.....d...d..
-000021d0: 028f 1f7d 0b74 137c 0583 017c 0c64 149c  ...}.t.|...|.d..
-000021e0: 027d 0574 106a 147c 057c 0b64 1564 168d  .}.t.j.|.|.d.d..
-000021f0: 0301 0074 0464 1788 019b 009d 0283 0101  ...t.d..........
-00002200: 0057 0064 0004 0004 0083 0301 0064 0053  .W.d.........d.S
-00002210: 0031 0090 0173 3077 0101 0001 0001 0059  .1...s0w.......Y
-00002220: 0001 0064 0053 0029 184e 6301 0000 0000  ...d.S.).Nc.....
-00002230: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
-00002240: 0000 0073 2200 0000 6700 7c00 5d0d 7d01  ...s"...g.|.].}.
-00002250: 7c01 a000 6400 a101 720f 6401 7c01 7601  |...d...r.d.|.v.
-00002260: 7202 7c01 9102 7102 5300 2902 fa03 2e70  r.|...q.S.)....p
-00002270: 7972 6200 0000 2901 da08 656e 6473 7769  yrb...)...endswi
-00002280: 7468 a902 7254 0000 0072 3200 0000 7212  th..rT...r2...r.
-00002290: 0000 0072 1200 0000 7213 0000 0072 5600  ...r....r....rV.
-000022a0: 0000 5b01 0000 730c 0000 0008 0008 0102  ..[...s.........
-000022b0: ff08 0102 ff06 017a 414d 6f64 756c 6552  .......zAModuleR
-000022c0: 6570 6f73 6974 6f72 792e 5f5f 6765 6e65  epository.__gene
-000022d0: 7261 7465 5f6d 6174 655f 6465 7065 6e64  rate_mate_depend
-000022e0: 656e 6369 6573 2e3c 6c6f 6361 6c73 3e2e  encies.<locals>.
-000022f0: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
-00002300: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
-00002310: 0000 0072 7900 0000 2902 7298 0000 0072  ...ry...).r....r
-00002320: 4400 0000 727a 0000 00a9 0272 5400 0000  D...rz.....rT...
-00002330: da04 6669 6c65 7212 0000 0072 1200 0000  ..filer....r....
-00002340: 7213 0000 0072 5600 0000 5d01 0000 725a  r....rV...]...rZ
-00002350: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00002360: 0200 0000 0400 0000 5300 0000 727e 0000  ........S...r~..
-00002370: 0029 0172 6200 0000 7212 0000 0072 9a00  .).rb...r....r..
-00002380: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00002390: 0072 5600 0000 5d01 0000 7304 0000 0006  .rV...]...s.....
-000023a0: 0012 0163 0100 0000 0000 0000 0000 0000  ...c............
-000023b0: 0200 0000 0700 0000 1300 0000 731e 0000  ............s...
-000023c0: 0067 007c 005d 0b7d 0174 0074 016a 02a0  .g.|.].}.t.t.j..
-000023d0: 0388 007c 01a1 0283 0191 0271 0253 0072  ...|.......q.S.r
-000023e0: 1200 0000 2904 7204 0000 0072 2200 0000  ....).r....r"...
-000023f0: 7223 0000 0072 2a00 0000 729a 0000 0029  r#...r*...r....)
-00002400: 0172 2300 0000 7212 0000 0072 1300 0000  .r#...r....r....
-00002410: 7256 0000 0061 0100 0073 0a00 0000 0600  rV...a...s......
-00002420: 0201 02ff 0c01 08ff 6301 0000 0000 0000  ........c.......
-00002430: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
-00002440: 0072 6f00 0000 7212 0000 0072 1200 0000  .ro...r....r....
-00002450: 7270 0000 0072 1200 0000 7212 0000 0072  rp...r....r....r
-00002460: 1300 0000 7256 0000 0065 0100 0072 7200  ....rV...e...rr.
-00002470: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00002480: 0000 0006 0000 0013 0000 0073 2600 0000  ...........s&...
-00002490: 6700 7c00 5d0f 8900 7400 8700 6601 6400  g.|.]...t...f.d.
-000024a0: 6401 8408 8801 4400 8301 8301 7302 8800  d.....D.....s...
-000024b0: 9102 7102 5300 2902 6301 0000 0000 0000  ..q.S.).c.......
-000024c0: 0000 0000 0002 0000 0004 0000 0013 0000  ................
-000024d0: 0073 1400 0000 6700 7c00 5d06 7d01 7c01  .s....g.|.].}.|.
-000024e0: 8800 7600 9102 7102 5300 7212 0000 0072  ..v...q.S.r....r
-000024f0: 1200 0000 729b 0000 00a9 01da 066d 6f64  ....r........mod
-00002500: 756c 6572 1200 0000 7213 0000 0072 5600  uler....r....rV.
-00002510: 0000 6b01 0000 7302 0000 0014 007a 4c4d  ..k...s......zLM
-00002520: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
-00002530: 5f5f 6765 6e65 7261 7465 5f6d 6174 655f  __generate_mate_
-00002540: 6465 7065 6e64 656e 6369 6573 2e3c 6c6f  dependencies.<lo
-00002550: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00002560: 2e3c 6c69 7374 636f 6d70 3e29 01da 0361  .<listcomp>)...a
-00002570: 6e79 2901 7254 0000 0029 01da 0e6f 7269  ny).rT...)...ori
-00002580: 6769 6e61 6c5f 6669 6c65 7372 9d00 0000  ginal_filesr....
-00002590: 7213 0000 0072 5600 0000 6801 0000 730c  r....rV...h...s.
-000025a0: 0000 0006 0002 0214 0102 fd02 0106 ff7a  ...............z
-000025b0: 2c4e 6f20 6769 7420 7572 6c20 666f 756e  ,No git url foun
-000025c0: 642c 2073 6b69 7070 696e 6720 6465 7065  d, skipping depe
-000025d0: 6e64 656e 6369 6573 2e6a 736f 6e72 9800  ndencies.jsonr..
-000025e0: 0000 7246 0000 00e9 ffff ffff 7273 0000  ..rF........rs..
-000025f0: 0072 0100 0000 7277 0000 0072 5200 0000  .r....rw...rR...
-00002600: da03 656e 767a 0e45 7272 6f72 2072 6561  ..envz.Error rea
-00002610: 6469 6e67 207a 202f 6465 7065 6e64 656e  ding z /dependen
-00002620: 6369 6573 2e6a 736f 6e2c 2073 6b69 7070  cies.json, skipp
-00002630: 696e 6720 656e 7672 1700 0000 2902 7278  ing envr....).rx
-00002640: 0000 0072 a200 0000 7218 0000 0072 1900  ...r....r....r..
-00002650: 0000 7a20 4765 6e65 7261 7465 6420 6465  ..z Generated de
-00002660: 7065 6e64 656e 6369 6573 2e6a 736f 6e20  pendencies.json 
-00002670: 666f 7220 2915 7222 0000 0072 4800 0000  for ).r"...rH...
-00002680: 724d 0000 0072 0500 0000 7227 0000 0072  rM...r....r'...r
-00002690: 9900 0000 720e 0000 0072 1600 0000 728f  ....r....r....r.
-000026a0: 0000 0072 2300 0000 7224 0000 0072 2a00  ...r#...r$...r*.
-000026b0: 0000 727b 0000 0072 4e00 0000 725d 0000  ..r{...rN...r]..
-000026c0: 0072 2b00 0000 722c 0000 0072 9000 0000  .r+...r,...r....
-000026d0: 7231 0000 0072 8b00 0000 722d 0000 0029  r1...r....r-...)
-000026e0: 0e72 1100 0000 7223 0000 00da 0566 696c  .r....r#.....fil
-000026f0: 6573 5a10 7265 6c61 7469 7665 5f69 6d70  esZ.relative_imp
-00002700: 6f72 7473 5a07 7572 6c5f 6769 7472 9700  ortsZ.url_gitr..
-00002710: 0000 729e 0000 005a 0574 7061 7468 5a12  ..r....Z.tpathZ.
-00002720: 7369 7374 6572 5f6d 6f64 756c 655f 7061  sister_module_pa
-00002730: 7468 7236 0000 005a 0964 6570 735f 6a73  thr6...Z.deps_js
-00002740: 6f6e 7232 0000 0072 a200 0000 7234 0000  onr2...r....r4..
-00002750: 0072 1200 0000 2902 72a0 0000 0072 2300  .r....).r....r#.
-00002760: 0000 7213 0000 005a 1c5f 5f67 656e 6572  ..r....Z.__gener
-00002770: 6174 655f 6d61 7465 5f64 6570 656e 6465  ate_mate_depende
-00002780: 6e63 6965 7358 0100 0073 7600 0000 0a03  nciesX...sv.....
-00002790: 0201 08ff 1202 0801 08ff 0a04 0201 06ff  ................
-000027a0: 0203 0c01 04ff 0a04 0202 06fe 0606 0802  ................
-000027b0: 0801 0401 0602 0801 0a02 0201 1403 1001  ................
-000027c0: 0e02 1402 1402 1401 0e01 1802 0402 0801  ................
-000027d0: 0c01 0c02 0401 0202 0e02 0c01 0c01 0a02  ................
-000027e0: 0801 0a01 0402 0280 1cfa 0280 0409 0480  ................
-000027f0: 1001 1001 1001 0880 02fe 1604 0e01 1001  ................
-00002800: 1001 24fd 7a2d 4d6f 6475 6c65 5265 706f  ..$.z-ModuleRepo
-00002810: 7369 746f 7279 2e5f 5f67 656e 6572 6174  sitory.__generat
-00002820: 655f 6d61 7465 5f64 6570 656e 6465 6e63  e_mate_dependenc
-00002830: 6965 7363 0200 0000 0000 0000 0000 0000  iesc............
-00002840: 0900 0000 0600 0000 4300 0000 73b8 0000  ........C...s...
-00002850: 0074 00a0 017c 01a1 017d 0274 00a0 027c  .t...|...}.t...|
-00002860: 02a1 017d 037c 00a0 037c 01a1 0101 0067  ...}.|...|.....g
-00002870: 007d 047c 017c 006a 046a 056b 0272 2474  .}.|.|.j.j.k.r$t
-00002880: 00a0 0664 017c 0364 02a1 0301 007c 00a0  ...d.|.d.....|..
-00002890: 0764 01a1 0101 006e 1d74 00a0 0674 086a  .d.....n.t...t.j
-000028a0: 09a0 0a7c 0164 01a1 027c 0364 02a1 0301  ...|.d...|.d....
-000028b0: 007c 00a0 0774 086a 09a0 0a7c 0164 01a1  .|...t.j...|.d..
-000028c0: 02a1 0101 0074 0b64 037c 019b 009d 0283  .....t.d.|......
-000028d0: 0101 007c 0344 005d 147d 057c 0564 0419  ...|.D.].}.|.d..
-000028e0: 007d 067c 0564 0519 007d 077c 067c 0764  .}.|.d...}.|.|.d
-000028f0: 069c 027d 087c 04a0 0c7c 08a1 0101 0071  ...}.|...|.....q
-00002900: 4364 077c 0469 0153 0029 084e 7276 0000  Cd.|.i.S.).Nrv..
-00002910: 007a 027e 3d7a 1f47 656e 6572 6174 6564  .z.~=z.Generated
-00002920: 2072 6571 7569 7265 6d65 6e74 732e 7478   requirements.tx
-00002930: 7420 666f 7220 726b 0000 00da 0776 6572  t for rk.....ver
-00002940: 7369 6f6e 2902 726b 0000 0072 a400 0000  sion).rk...r....
-00002950: da03 7069 7029 0d72 0800 0000 5a0f 6765  ..pip).r....Z.ge
-00002960: 745f 616c 6c5f 696d 706f 7274 735a 1067  t_all_importsZ.g
-00002970: 6574 5f69 6d70 6f72 745f 6c6f 6361 6cda  et_import_local.
-00002980: 2d5f 4d6f 6475 6c65 5265 706f 7369 746f  -_ModuleReposito
-00002990: 7279 5f5f 6765 6e65 7261 7465 5f6d 6174  ry__generate_mat
-000029a0: 655f 6465 7065 6e64 656e 6369 6573 720e  e_dependenciesr.
-000029b0: 0000 0072 1600 0000 5a1a 6765 6e65 7261  ...r....Z.genera
-000029c0: 7465 5f72 6571 7569 7265 6d65 6e74 735f  te_requirements_
-000029d0: 6669 6c65 da30 5f4d 6f64 756c 6552 6570  file.0_ModuleRep
-000029e0: 6f73 6974 6f72 795f 5f61 6464 5f69 6e64  ository__add_ind
-000029f0: 6578 5f75 726c 5f74 6f5f 7265 7175 6972  ex_url_to_requir
-00002a00: 656d 656e 7473 7222 0000 0072 2300 0000  ementsr"...r#...
-00002a10: 722a 0000 0072 2700 0000 728d 0000 0029  r*...r'...r....)
-00002a20: 0972 1100 0000 7223 0000 00da 0769 6d70  .r....r#.....imp
-00002a30: 6f72 7473 5a11 696d 706f 7274 5f69 6e66  ortsZ.import_inf
-00002a40: 6f5f 6c6f 6361 6c5a 0b69 6d70 6f72 745f  o_localZ.import_
-00002a50: 696e 666f 5a02 696d 726b 0000 0072 a400  infoZ.imrk...r..
-00002a60: 0000 da03 7265 7372 1200 0000 7212 0000  ....resr....r...
-00002a70: 0072 1300 0000 5a1b 5f5f 6765 6e65 7261  .r....Z.__genera
-00002a80: 7465 5f70 6970 5f72 6571 7569 7265 6d65  te_pip_requireme
-00002a90: 6e74 73a6 0100 0073 3000 0000 0a03 0a03  nts....s0.......
-00002aa0: 0a02 0402 0c02 0401 0601 04ff 0c03 0403  ................
-00002ab0: 1001 04ff 0403 0c01 04ff 0e02 0802 0802  ................
-00002ac0: 0801 0203 0201 06fe 0c05 0802 7a2c 4d6f  ............z,Mo
-00002ad0: 6475 6c65 5265 706f 7369 746f 7279 2e5f  duleRepository._
-00002ae0: 5f67 656e 6572 6174 655f 7069 705f 7265  _generate_pip_re
-00002af0: 7175 6972 656d 656e 7473 729e 0000 0063  quirementsr....c
-00002b00: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00002b10: 0300 0000 4300 0000 731e 0000 007c 0164  ....C...s....|.d
-00002b20: 006b 0272 097c 006a 00a0 01a1 0053 007c  .k.r.|.j.....S.|
-00002b30: 006a 00a0 027c 01a1 0153 0072 0d00 0000  .j...|...S.r....
-00002b40: 2903 7210 0000 00da 0773 756d 6d61 7279  ).r......summary
-00002b50: 728b 0000 0029 0272 1100 0000 729e 0000  r....).r....r...
-00002b60: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00002b70: 728b 0000 00ce 0100 0073 0600 0000 0801  r........s......
-00002b80: 0a01 0c01 7a15 4d6f 6475 6c65 5265 706f  ....z.ModuleRepo
-00002b90: 7369 746f 7279 2e6c 6973 7463 0100 0000  sitory.listc....
-00002ba0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00002bb0: 4300 0000 730a 0000 007c 006a 00a0 01a1  C...s....|.j....
-00002bc0: 0053 0072 0d00 0000 2902 7210 0000 0072  .S.r....).r....r
-00002bd0: aa00 0000 2901 7211 0000 0072 1200 0000  ....).r....r....
-00002be0: 7212 0000 0072 1300 0000 da10 6765 745f  r....r......get_
-00002bf0: 6d61 7465 5f73 756d 6d61 7279 d301 0000  mate_summary....
-00002c00: 7302 0000 000a 017a 214d 6f64 756c 6552  s......z!ModuleR
-00002c10: 6570 6f73 6974 6f72 792e 6765 745f 6d61  epository.get_ma
-00002c20: 7465 5f73 756d 6d61 7279 da07 7061 636b  te_summary..pack
-00002c30: 6167 6563 0200 0000 0000 0000 0000 0000  agec............
-00002c40: 0200 0000 0300 0000 4300 0000 7310 0000  ........C...s...
-00002c50: 007c 006a 00a0 017c 01a1 0101 0064 0053  .|.j...|.....d.S
-00002c60: 0072 0d00 0000 2902 7210 0000 0072 3700  .r....).r....r7.
-00002c70: 0000 2902 7211 0000 0072 ac00 0000 7212  ..).r....r....r.
-00002c80: 0000 0072 1200 0000 7213 0000 0072 3700  ...r....r....r7.
-00002c90: 0000 d601 0000 7302 0000 0010 017a 204d  ......s......z M
-00002ca0: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
-00002cb0: 696e 7374 616c 6c5f 7061 636b 6167 6529  install_package)
-00002cc0: 0146 720d 0000 0029 16da 085f 5f6e 616d  .Fr....)...__nam
-00002cd0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00002ce0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0462  .__qualname__..b
-00002cf0: 6f6f 6c72 1400 0000 da0c 7374 6174 6963  oolr......static
-00002d00: 6d65 7468 6f64 da03 7374 7272 3500 0000  method..strr5...
-00002d10: 723a 0000 0072 4200 0000 7241 0000 0072  r:...rB...rA...r
-00002d20: 8b00 0000 7260 0000 0072 a700 0000 7265  ....r`...r....re
-00002d30: 0000 0072 4000 0000 728a 0000 0072 a600  ...r@...r....r..
-00002d40: 0000 7264 0000 0072 ab00 0000 7209 0000  ..rd...r....r...
-00002d50: 0072 3700 0000 7212 0000 0072 1200 0000  .r7...r....r....
-00002d60: 7212 0000 0072 1300 0000 720b 0000 0014  r....r....r.....
-00002d70: 0000 0073 2400 0000 0800 1001 0207 1001  ...s$...........
-00002d80: 0e2a 0e04 1006 1212 0e0e 081d 0816 007f  .*..............
-00002d90: 0821 0814 084e 1028 0805 1203 720b 0000  .!...N.(....r...
-00002da0: 0029 1672 2c00 0000 7222 0000 0072 5e00  .).r,...r"...r^.
-00002db0: 0000 7228 0000 0072 9300 0000 5a0e 6d6f  ..r(...r....Z.mo
-00002dc0: 6475 6c65 5f6d 616e 6167 6572 7203 0000  dule_managerr...
-00002dd0: 005a 0e75 7469 6c73 2e65 7870 5f75 7469  .Z.utils.exp_uti
-00002de0: 6c72 0400 0000 5a0e 7574 696c 732e 6769  lr....Z.utils.gi
-00002df0: 745f 7574 696c 7205 0000 005a 0e73 6f75  t_utilr....Z.sou
-00002e00: 7263 6573 2e72 656d 6f74 6572 0600 0000  rces.remoter....
-00002e10: 5a13 736f 7572 6365 732e 6c6f 6361 6c2e  Z.sources.local.
-00002e20: 6c6f 6361 6c72 0700 0000 7208 0000 0072  localr....r....r
-00002e30: ac00 0000 7209 0000 00da 0674 7970 696e  ....r......typin
-00002e40: 6772 0a00 0000 da04 6970 6462 720b 0000  gr......ipdbr...
-00002e50: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-00002e60: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00002e70: 0000 0073 1e00 0000 0800 0801 0801 0801  ...s............
-00002e80: 0802 0c02 0c01 0c01 0c01 0c01 0c01 0c02  ................
-00002e90: 0c01 0801 1203                           ......
+00000e30: 6400 7c01 7601 7202 7c01 9102 7102 5300  d.|.v.r.|...q.S.
+00000e40: 2902 7a0a 2e65 6767 3e3d 696e 666f 7a0a  ).z..egg>=infoz.
+00000e50: 2e65 6767 3d3d 696e 666f 7212 0000 00a9  .egg==infor.....
+00000e60: 02da 022e 30da 046c 696e 6572 1200 0000  ....0..liner....
+00000e70: 7212 0000 0072 1300 0000 da0a 3c6c 6973  r....r......<lis
+00000e80: 7463 6f6d 703e 7300 0000 730e 0000 0006  tcomp>s...s.....
+00000e90: 0002 0208 0108 0108 0102 fc06 047a 444d  .............zDM
+00000ea0: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
+00000eb0: 5f5f 6164 645f 696e 6465 785f 7572 6c5f  __add_index_url_
+00000ec0: 746f 5f72 6571 7569 7265 6d65 6e74 732e  to_requirements.
+00000ed0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00000ee0: 6d70 3e7a 075c 2b63 755c 642b 6301 0000  mp>z.\+cu\d+c...
+00000ef0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00000f00: 0013 0000 0073 1800 0000 6700 7c00 5d08  .....s....g.|.].
+00000f10: 7d01 8800 a000 6400 7c01 a102 9102 7102  }.....d.|.....q.
+00000f20: 5300 2901 7244 0000 0029 01da 0373 7562  S.).rD...)...sub
+00000f30: 7253 0000 00a9 01da 0572 6567 6578 7212  rS.......regexr.
+00000f40: 0000 0072 1300 0000 7256 0000 007e 0000  ...r....rV...~..
+00000f50: 00f3 0200 0000 1800 7201 0000 0072 1700  ........r....r..
+00000f60: 0000 7a12 2d2d 6578 7472 612d 696e 6465  ..z.--extra-inde
+00000f70: 782d 7572 6c20 da01 0a29 0a72 2b00 0000  x-url ...).r+...
+00000f80: 7222 0000 0072 2300 0000 722a 0000 00da  r"...r#...r*....
+00000f90: 0972 6561 646c 696e 6573 da03 6c65 6eda  .readlines..len.
+00000fa0: 0272 65da 0763 6f6d 7069 6c65 da23 5f4d  .re..compile.#_M
+00000fb0: 6f64 756c 6552 6570 6f73 6974 6f72 795f  oduleRepository_
+00000fc0: 5f70 6172 7365 5f69 6e64 6578 5f75 726c  _parse_index_url
+00000fd0: 7372 4700 0000 2908 7211 0000 0072 2300  srG...).r....r#.
+00000fe0: 0000 7232 0000 00da 056c 696e 6573 5a09  ..r2.....linesZ.
+00000ff0: 6c69 6e65 636f 756e 7472 4f00 0000 7236  linecountrO...r6
+00001000: 0000 0072 5500 0000 7212 0000 0072 5800  ...rU...r....rX.
+00001010: 0000 7213 0000 005a 1f5f 5f61 6464 5f69  ..r....Z.__add_i
+00001020: 6e64 6578 5f75 726c 5f74 6f5f 7265 7175  ndex_url_to_requ
+00001030: 6972 656d 656e 7473 6f00 0000 7332 0000  irementso...s2..
+00001040: 0014 010a 011c ff08 0206 0102 0206 fe0a  ................
+00001050: 0a12 010a 020c 0114 0108 0114 0108 010c  ................
+00001060: 0102 ff22 fd0c 0514 0108 010c 0102 ff22  ..."..........."
+00001070: ff04 ff7a 304d 6f64 756c 6552 6570 6f73  ...z0ModuleRepos
+00001080: 6974 6f72 792e 5f5f 6164 645f 696e 6465  itory.__add_inde
+00001090: 785f 7572 6c5f 746f 5f72 6571 7569 7265  x_url_to_require
+000010a0: 6d65 6e74 7363 0200 0000 0000 0000 0000  mentsc..........
+000010b0: 0000 0500 0000 0600 0000 4300 0000 738a  ..........C...s.
+000010c0: 0000 0074 00a0 017c 01a1 0144 005d 3d7d  ...t...|...D.]=}
+000010d0: 027c 02a0 0264 01a1 0173 117c 02a0 0264  .|...d...s.|...d
+000010e0: 02a1 0172 1271 0574 006a 03a0 047c 017c  ...r.q.t.j...|.|
+000010f0: 02a1 027d 0374 006a 03a0 057c 03a1 0172  ...}.t.j...|...r
+00001100: 4274 006a 03a0 047c 017c 0264 03a1 037d  Bt.j...|.|.d...}
+00001110: 0474 006a 03a0 067c 04a1 0173 2e71 057c  .t.j...|...s.q.|
+00001120: 0264 0476 0072 387c 006a 076a 087c 0176  .d.v.r8|.j.j.|.v
+00001130: 0073 3d7c 00a0 097c 03a1 0101 007c 00a0  .s=|...|.....|..
+00001140: 0a7c 03a1 0101 0071 0564 0053 0029 054e  .|.....q.d.S.).N
+00001150: 7246 0000 00da 025f 5f72 1b00 0000 2904  rF.....__r....).
+00001160: 7220 0000 0072 1d00 0000 721e 0000 0072  r ...r....r....r
+00001170: 1f00 0000 290b 7222 0000 0072 4800 0000  ....).r"...rH...
+00001180: da0a 7374 6172 7473 7769 7468 7223 0000  ..startswithr#..
+00001190: 0072 2a00 0000 7249 0000 0072 2400 0000  .r*...rI...r$...
+000011a0: 720e 0000 0072 1600 0000 da2c 5f4d 6f64  r....r.....,_Mod
+000011b0: 756c 6552 6570 6f73 6974 6f72 795f 5f67  uleRepository__g
+000011c0: 656e 6572 6174 655f 7069 705f 7265 7175  enerate_pip_requ
+000011d0: 6972 656d 656e 7473 da29 5f4d 6f64 756c  irements.)_Modul
+000011e0: 6552 6570 6f73 6974 6f72 795f 5f67 656e  eRepository__gen
+000011f0: 6572 6174 655f 6465 7073 5f69 6e5f 6465  erate_deps_in_de
+00001200: 7074 68a9 0572 1100 0000 5a09 726f 6f74  pth..r....Z.root
+00001210: 5f70 6174 68da 0364 6972 7223 0000 005a  _path..dirr#...Z
+00001220: 0a69 6e69 745f 5f70 6174 6872 1200 0000  .init__pathr....
+00001230: 7212 0000 0072 1300 0000 5a18 5f5f 6765  r....r....Z.__ge
+00001240: 6e65 7261 7465 5f64 6570 735f 696e 5f64  nerate_deps_in_d
+00001250: 6570 7468 8c00 0000 731c 0000 000e 0314  epth....s.......
+00001260: 0102 010e 010c 0110 020c 0102 0108 030c  ................
+00001270: 010a 020a 0202 8004 f07a 294d 6f64 756c  .........z)Modul
+00001280: 6552 6570 6f73 6974 6f72 792e 5f5f 6765  eRepository.__ge
+00001290: 6e65 7261 7465 5f64 6570 735f 696e 5f64  nerate_deps_in_d
+000012a0: 6570 7468 6301 0000 0000 0000 0000 0000  epthc...........
+000012b0: 0013 0000 000b 0000 000f 0000 0073 c204  .............s..
+000012c0: 0000 7c00 a000 a100 0100 7c00 a001 a100  ..|.......|.....
+000012d0: 7d03 6700 7d04 7c03 a002 a100 4400 5d3a  }.g.}.|.....D.]:
+000012e0: 5c02 8900 7d05 7403 7c05 8301 7401 7500  \...}.t.|...t.u.
+000012f0: 7234 7c04 a004 8700 6601 6401 6402 8408  r4|.....f.d.d...
+00001300: 7c05 4400 8301 a101 0100 7405 7c05 8301  |.D.......t.|...
+00001310: 6403 6b02 7233 7c04 a004 8800 8800 6404  d.k.r3|.......d.
+00001320: 9c02 6701 a101 0100 710e 7403 7c05 8301  ..g.....q.t.|...
+00001330: 7406 7500 7248 7c04 a004 8700 6601 6405  t.u.rH|.....f.d.
+00001340: 6402 8408 7c05 a007 a100 4400 8301 a101  d...|.....D.....
+00001350: 0100 710e 6406 6402 8400 7c04 4400 8301  ..q.d.d...|.D...
+00001360: 7d04 7408 8300 7d06 7409 8300 7d07 7c07  }.t...}.t...}.|.
+00001370: a00a 6407 a101 6408 1900 7d08 7c07 a00a  ..d...d...}.|...
+00001380: 6407 a101 6409 1900 7d09 7c04 4400 5d47  d...d...}.|.D.]G
+00001390: 7d0a 7c07 9b00 7c00 6a0b 6a0c 9b00 6407  }.|...|.j.j...d.
+000013a0: 7c0a 640a 1900 9b00 6407 7c0a 640b 1900  |.d.....d.|.d...
+000013b0: 9b00 9d06 7c0a 640c 3c00 7c08 9b00 6407  ....|.d.<.|...d.
+000013c0: 7c09 9b00 6407 7c00 6a0b 6a0c 9b00 6407  |...d.|.j.j...d.
+000013d0: 7c0a 640a 1900 9b00 6407 7c0a 640b 1900  |.d.....d.|.d...
+000013e0: 9b00 9d09 7c0a 640d 3c00 7c09 7c00 6a0b  ....|.d.<.|.|.j.
+000013f0: 6a0c 6b02 72ad 7c08 9b00 6407 7c09 9b00  j.k.r.|...d.|...
+00001400: 6407 7c0a 640a 1900 9b00 6407 7c0a 640b  d.|.d.....d.|.d.
+00001410: 1900 9b00 9d07 7c0a 640d 3c00 7166 7c04  ......|.d.<.qf|.
+00001420: 4400 5dc0 7d0a 740d 6a0e a00f 7c00 6a0b  D.].}.t.j...|.j.
+00001430: 6a0c 7c0a 640a 1900 7c0a 640b 1900 640e  j.|.d...|.d...d.
+00001440: a104 7d0b 740d 6a0e a00f 7c00 6a0b 6a0c  ..}.t.j...|.j.j.
+00001450: 7c0a 640a 1900 7c0a 640b 1900 640f a104  |.d...|.d...d...
+00001460: 7d0c 740d 6a0e a00f 7c00 6a0b 6a0c 7c0a  }.t.j...|.j.j.|.
+00001470: 640a 1900 640e a103 7d0d 740d 6a0e a010  d...d...}.t.j...
+00001480: 7c0b a101 72fd 7411 7c0b 6410 8302 8f0e  |...r.t.|.d.....
+00001490: 7d0e 7c0e a012 a100 7c0a 6411 3c00 5700  }.|.....|.d.<.W.
+000014a0: 6400 0400 0400 8303 0100 6e08 3100 73f8  d.........n.1.s.
+000014b0: 7701 0100 0100 0100 5900 0100 740d 6a0e  w.......Y...t.j.
+000014c0: a010 7c0c a101 9001 7236 7411 7c0c 6410  ..|.....r6t.|.d.
+000014d0: 8302 8f24 7d0e 6411 7c0a 7600 9001 721d  ...$}.d.|.v...r.
+000014e0: 7c0a 6411 0500 1900 7413 a014 7c0e a101  |.d.....t...|...
+000014f0: 6411 1900 3700 0300 3c00 6e09 7413 a014  d...7...<.n.t...
+00001500: 7c0e a101 6411 1900 7c0a 6411 3c00 5700  |...d...|.d.<.W.
+00001510: 6400 0400 0400 8303 0100 6e09 3100 9001  d.........n.1...
+00001520: 7331 7701 0100 0100 0100 5900 0100 740d  s1w.......Y...t.
+00001530: 6a0e a010 7c0d a101 9001 7259 7411 7c0d  j...|.....rYt.|.
+00001540: 6410 8302 8f0e 7d0e 7c0e a012 a100 7c0a  d.....}.|.....|.
+00001550: 6411 3c00 5700 6400 0400 0400 8303 0100  d.<.W.d.........
+00001560: 6e09 3100 9001 7354 7701 0100 0100 0100  n.1...sTw.......
+00001570: 5900 0100 6411 7c0a 7600 9001 7270 6412  Y...d.|.v...rpd.
+00001580: 6402 8400 7c0a 6411 1900 4400 8301 7c0a  d...|.d...D...|.
+00001590: 6411 3c00 7c06 a015 7c0a 6411 1900 a101  d.<.|...|.d.....
+000015a0: 0100 71b0 6413 6402 8400 7c06 4400 8301  ..q.d.d...|.D...
+000015b0: 7d06 7416 7c06 6414 6415 8400 6416 6417  }.t.|.d.d...d.d.
+000015c0: 8d03 7d06 6418 6402 8400 7c06 4400 8301  ..}.d.d...|.D...
+000015d0: 7d06 7411 640e 6419 8302 8f15 7d0e 7c06  }.t.d.d.....}.|.
+000015e0: 4400 5d0a 7d0f 7c0e a017 7c0f 641a 1700  D.].}.|...|.d...
+000015f0: a101 0100 9001 7190 5700 6400 0400 0400  ......q.W.d.....
+00001600: 8303 0100 6e09 3100 9001 73a6 7701 0100  ....n.1...s.w...
+00001610: 0100 0100 5900 0100 7c04 7d10 6700 7d10  ....Y...|.}.g.}.
+00001620: 7411 641b 6419 8302 8f10 7d0e 7413 6a18  t.d.d.....}.t.j.
+00001630: 7c04 7c0e 6409 641c 8d03 0100 5700 6400  |.|.d.d.....W.d.
+00001640: 0400 0400 8303 0100 6e09 3100 9001 73c8  ........n.1...s.
+00001650: 7701 0100 0100 0100 5900 0100 7c04 4400  w.......Y...|.D.
+00001660: 5d42 7d0a 6411 7c0a 7600 9001 72fe 6700  ]B}.d.|.v...r.g.
+00001670: 7d11 7c0a 6411 1900 4400 5d0f 7d0f 641d  }.|.d...D.].}.d.
+00001680: 7c0f 7600 9001 72e5 9001 71dc 7c11 a004  |.v...r...q.|...
+00001690: 7c0f a101 0100 9001 71dc 7c10 a004 7c0a  |.......q.|...|.
+000016a0: 640b 1900 7c0a 640a 1900 7c0a 640d 1900  d...|.d...|.d...
+000016b0: 7c11 641e 9c04 a101 0100 9001 71cf 7c10  |.d.........q.|.
+000016c0: a004 7c0a 640b 1900 7c0a 640a 1900 7c0a  ..|.d...|.d...|.
+000016d0: 640d 1900 7c0a 6411 1900 641e 9c04 a101  d...|.d...d.....
+000016e0: 0100 9001 71cf 7419 6a19 7c10 641f 6420  ....q.t.j.|.d.d 
+000016f0: 6421 6422 8d04 7d12 7419 6a19 7c04 641f  d!d"..}.t.j.|.d.
+00001700: 6423 6424 6416 6425 8d05 7d04 7411 6426  d#d$d.d%..}.t.d&
+00001710: 6419 8302 8f0d 7d0e 7c0e a017 7c04 a101  d.....}.|...|...
+00001720: 0100 5700 6400 0400 0400 8303 0100 6e09  ..W.d.........n.
+00001730: 3100 9002 733b 7701 0100 0100 0100 5900  1...s;w.......Y.
+00001740: 0100 7411 6427 6419 8302 8f0d 7d0e 7c0e  ..t.d'd.....}.|.
+00001750: a017 7c12 a101 0100 5700 6400 0400 0400  ..|.....W.d.....
+00001760: 8303 0100 6e09 3100 9002 7356 7701 0100  ....n.1...sVw...
+00001770: 0100 0100 5900 0100 741a 6428 8301 0100  ....Y...t.d(....
+00001780: 6400 5300 2929 4e63 0100 0000 0000 0000  d.S.))Nc........
+00001790: 0000 0000 0200 0000 0500 0000 1300 0000  ................
+000017a0: f316 0000 0067 007c 005d 077d 0188 007c  .....g.|.].}...|
+000017b0: 0164 009c 0291 0271 0253 00a9 01a9 02da  .d.....q.S......
+000017c0: 0474 7970 65da 046e 616d 6572 1200 0000  .type..namer....
+000017d0: a902 7254 0000 0072 6c00 0000 a901 da03  ..rT...rl.......
+000017e0: 6b65 7972 1200 0000 7213 0000 0072 5600  keyr....r....rV.
+000017f0: 0000 aa00 0000 f302 0000 0016 007a 2d4d  .............z-M
+00001800: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
+00001810: 5f5f 6578 706f 7274 2e3c 6c6f 6361 6c73  __export.<locals
+00001820: 3e2e 3c6c 6973 7463 6f6d 703e 7201 0000  >.<listcomp>r...
+00001830: 0072 6a00 0000 6301 0000 0000 0000 0000  .rj...c.........
+00001840: 0000 0002 0000 0005 0000 0013 0000 0072  ...............r
+00001850: 6800 0000 7269 0000 0072 1200 0000 726d  h...ri...r....rm
+00001860: 0000 0072 6e00 0000 7212 0000 0072 1300  ...rn...r....r..
+00001870: 0000 7256 0000 00af 0000 0072 7000 0000  ..rV.......rp...
+00001880: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00001890: 0004 0000 0053 0000 00f3 1a00 0000 6700  .....S........g.
+000018a0: 7c00 5d09 7d01 7c01 4400 5d04 7d02 7c02  |.].}.|.D.].}.|.
+000018b0: 9103 7106 7102 5300 7212 0000 0072 1200  ..q.q.S.r....r..
+000018c0: 0000 a903 7254 0000 005a 0773 7562 6c69  ....rT...Z.subli
+000018d0: 7374 da04 6974 656d 7212 0000 0072 1200  st..itemr....r..
+000018e0: 0000 7213 0000 0072 5600 0000 b300 0000  ..r....rV.......
+000018f0: f302 0000 001a 00fa 012f e903 0000 0072  ........./.....r
+00001900: 1800 0000 726b 0000 0072 6c00 0000 7236  ....rk...rl...r6
+00001910: 0000 00da 0973 686f 7274 5f75 726c fa10  .....short_url..
+00001920: 7265 7175 6972 656d 656e 7473 2e74 7874  requirements.txt
+00001930: fa11 6465 7065 6e64 656e 6369 6573 2e6a  ..dependencies.j
+00001940: 736f 6e72 5200 0000 da0c 6465 7065 6e64  sonrR.....depend
+00001950: 656e 6369 6573 6301 0000 0000 0000 0000  enciesc.........
+00001960: 0000 0002 0000 0006 0000 0053 0000 00f3  ...........S....
+00001970: 1800 0000 6700 7c00 5d08 7d01 7c01 a000  ....g.|.].}.|...
+00001980: 6400 6401 a102 9102 7102 5300 2902 725b  d.d.....q.S.).r[
+00001990: 0000 0072 4400 0000 a901 da07 7265 706c  ...rD.......repl
+000019a0: 6163 65a9 0272 5400 0000 da03 6465 7072  ace..rT.....depr
+000019b0: 1200 0000 7212 0000 0072 1300 0000 7256  ....r....r....rV
+000019c0: 0000 00e8 0000 0073 0600 0000 0600 0c01  .......s........
+000019d0: 06ff 6301 0000 0000 0000 0000 0000 0002  ..c.............
+000019e0: 0000 0004 0000 0053 0000 0073 2000 0000  .......S...s ...
+000019f0: 6700 7c00 5d0c 7d01 6400 7c01 7600 720c  g.|.].}.d.|.v.r.
+00001a00: 6401 7c01 7601 7302 7c01 9102 7102 5300  d.|.v.s.|...q.S.
+00001a10: 2902 7a0e 6874 7470 733a 2f2f 6769 7468  ).z.https://gith
+00001a20: 7562 7a04 2b67 6974 7212 0000 0072 7e00  ubz.+gitr....r~.
+00001a30: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00001a40: 0072 5600 0000 ef00 0000 7304 0000 0006  .rV.......s.....
+00001a50: 001a 0163 0100 0000 0000 0000 0000 0000  ...c............
+00001a60: 0100 0000 0200 0000 5300 0000 7308 0000  ........S...s...
+00001a70: 0064 017c 0076 0053 0029 024e 7a11 2d2d  .d.|.v.S.).Nz.--
+00001a80: 6578 7472 612d 696e 6465 782d 7572 6c72  extra-index-urlr
+00001a90: 1200 0000 2901 da01 7872 1200 0000 7212  ....)...xr....r.
+00001aa0: 0000 0072 1300 0000 da08 3c6c 616d 6264  ...r......<lambd
+00001ab0: 613e f300 0000 7302 0000 0008 007a 2b4d  a>....s......z+M
+00001ac0: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
+00001ad0: 5f5f 6578 706f 7274 2e3c 6c6f 6361 6c73  __export.<locals
+00001ae0: 3e2e 3c6c 616d 6264 613e 5429 0272 6f00  >.<lambda>T).ro.
+00001af0: 0000 da07 7265 7665 7273 6563 0100 0000  ....reversec....
+00001b00: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00001b10: 5300 0000 7328 0000 0067 007c 005d 107d  S...s(...g.|.].}
+00001b20: 017c 0164 006b 0373 107c 0164 016b 0373  .|.d.k.s.|.d.k.s
+00001b30: 107c 0164 026b 0372 027c 0191 0271 0253  .|.d.k.r.|...q.S
+00001b40: 0029 0372 5b00 0000 fa01 2072 4400 0000  .).r[..... rD...
+00001b50: 7212 0000 0072 7e00 0000 7212 0000 0072  r....r~...r....r
+00001b60: 1200 0000 7213 0000 0072 5600 0000 f500  ....r....rV.....
+00001b70: 0000 7302 0000 0028 0072 1700 0000 725b  ..s....(.r....r[
+00001b80: 0000 007a 0c65 7870 6f72 7473 2e6a 736f  ...z.exports.jso
+00001b90: 6e72 1900 0000 7a07 2d2d 6578 7472 6129  nr....z.--extra)
+00001ba0: 0472 6c00 0000 726b 0000 0072 7700 0000  .rl...rk...rw...
+00001bb0: 727a 0000 00da 046b 6579 73da 056c 6174  rz.....keys..lat
+00001bc0: 6578 da05 6e65 7665 7229 03da 0768 6561  ex..never)...hea
+00001bd0: 6465 7273 da08 7461 626c 6566 6d74 da09  ders..tablefmt..
+00001be0: 7368 6f77 696e 6465 785a 0667 6974 6875  showindexZ.githu
+00001bf0: 62da 0661 6c77 6179 7329 0472 8700 0000  b..always).r....
+00001c00: 7288 0000 0072 8900 0000 5a10 6469 7361  r....r....Z.disa
+00001c10: 626c 655f 6e75 6d70 6172 7365 7a09 6578  ble_numparsez.ex
+00001c20: 706f 7274 2e6d 647a 0b65 7870 6f72 7473  port.mdz.exports
+00001c30: 2e74 6578 7a15 4578 706f 7274 6564 2074  .texz.Exported t
+00001c40: 6f20 6578 706f 7274 2e6d 6429 1bda 285f  o export.md)..(_
+00001c50: 4d6f 6475 6c65 5265 706f 7369 746f 7279  ModuleRepository
+00001c60: 5f5f 6765 6e65 7261 7465 5f73 7562 5f70  __generate_sub_p
+00001c70: 6970 5f72 6571 73da 046c 6973 74da 0569  ip_reqs..list..i
+00001c80: 7465 6d73 726b 0000 00da 0661 7070 656e  temsrk.....appen
+00001c90: 6472 5d00 0000 da04 6469 6374 7284 0000  dr].....dictr...
+00001ca0: 0072 4d00 0000 7205 0000 00da 0573 706c  .rM...r......spl
+00001cb0: 6974 720e 0000 0072 1600 0000 7222 0000  itr....r....r"..
+00001cc0: 0072 2300 0000 722a 0000 0072 2400 0000  .r#...r*...r$...
+00001cd0: 722b 0000 0072 5c00 0000 722c 0000 00da  r+...r\...r,....
+00001ce0: 046c 6f61 64da 0675 7064 6174 65da 0673  .load..update..s
+00001cf0: 6f72 7465 6472 4700 0000 722d 0000 00da  ortedrG...r-....
+00001d00: 0874 6162 756c 6174 6572 2700 0000 2913  .tabulater'...).
+00001d10: 7211 0000 0072 3800 0000 7239 0000 00da  r....r8...r9....
+00001d20: 076d 6f64 756c 6573 da05 7461 626c 65da  .modules..table.
+00001d30: 0576 616c 7565 da04 6465 7073 5a08 6261  .value..depsZ.ba
+00001d40: 7365 5f75 726c 5a09 7573 6572 5f6e 616d  se_urlZ.user_nam
+00001d50: 655a 0972 6570 6f5f 6e61 6d65 7273 0000  eZ.repo_namers..
+00001d60: 0072 2300 0000 5a08 6465 705f 7061 7468  .r#...Z.dep_path
+00001d70: 5a0d 726f 6f74 5f64 6570 5f70 6174 6872  Z.root_dep_pathr
+00001d80: 3200 0000 727f 0000 005a 066c 7461 626c  2...r....Z.ltabl
+00001d90: 655a 076e 6577 5f64 6570 5a0b 6c61 7465  eZ.new_depZ.late
+00001da0: 785f 7461 626c 6572 1200 0000 726e 0000  x_tabler....rn..
+00001db0: 0072 1300 0000 5a08 5f5f 6578 706f 7274  .r....Z.__export
+00001dc0: a100 0000 73ee 0000 0008 0108 0204 0210  ....s...........
+00001dd0: 020c 0118 010c 0212 0102 800c 011c 0102  ................
+00001de0: 800e 0406 0306 020e 010e 0108 0122 0302  ............."..
+00001df0: fe02 0102 ff2a 0502 fe02 0102 ff0c 0520  .....*......... 
+00001e00: 0502 fe02 0102 ff02 8008 0506 0114 0104  ................
+00001e10: ff06 0314 0104 ff06 040e 0104 ff0c 040c  ................
+00001e20: 010e 011c ff0e 020c 010a 011c 0112 0202  ................
+00001e30: 801e fc0e 070c 010e 011e ff0a 0306 0106  ................
+00001e40: 010a ff0e 0402 8006 0302 0106 ff12 040e  ................
+00001e50: 020c 0308 0112 0102 ff1e ff04 0904 0a0c  ................
+00001e60: 0412 011e ff08 030a 0204 020c 010a 0104  ................
+00001e70: 010e 0104 0106 0206 0106 0102 0104 fc08  ................
+00001e80: ff04 0906 0206 0106 0106 0104 fc08 ff04  ................
+00001e90: 0b02 0102 0102 0102 0106 fc04 0802 0102  ................
+00001ea0: 0102 0102 0102 0106 fb0c 0a0c 011e ff0c  ................
+00001eb0: 030c 011e ff0c 037a 194d 6f64 756c 6552  .......z.ModuleR
+00001ec0: 6570 6f73 6974 6f72 792e 5f5f 6578 706f  epository.__expo
+00001ed0: 7274 6301 0000 0000 0000 0000 0000 0005  rtc.............
+00001ee0: 0000 0006 0000 0043 0000 0073 8a00 0000  .......C...s....
+00001ef0: 7c00 6a00 6a01 7d01 7c00 a002 7c01 a101  |.j.j.}.|...|...
+00001f00: 0100 7403 a004 6401 a101 4400 5d34 7d02  ..t...d...D.]4}.
+00001f10: 7c02 a005 6401 a101 7320 7c02 a005 6402  |...d...s |...d.
+00001f20: a101 7320 7c02 7c00 6a00 6a01 6b02 7221  ..s |.|.j.j.k.r!
+00001f30: 710e 7403 6a06 a007 6401 7c02 a102 7d03  q.t.j...d.|...}.
+00001f40: 7403 6a06 a008 7c03 a101 7242 7403 6a06  t.j...|...rBt.j.
+00001f50: a007 6401 7c02 6403 a103 7d04 7403 6a06  ..d.|.d...}.t.j.
+00001f60: a009 7c04 a101 733d 710e 7c00 a00a 7c03  ..|...s=q.|...|.
+00001f70: a101 0100 710e 6400 5300 2904 4e72 4600  ....q.d.S.).NrF.
+00001f80: 0000 7262 0000 0072 1b00 0000 290b 720e  ..rb...r....).r.
+00001f90: 0000 0072 1600 0000 7265 0000 0072 2200  ...r....re...r".
+00001fa0: 0000 7248 0000 0072 6300 0000 7223 0000  ..rH...rc...r#..
+00001fb0: 0072 2a00 0000 7249 0000 0072 2400 0000  .r*...rI...r$...
+00001fc0: 7264 0000 0072 6600 0000 7212 0000 0072  rd...rf...r....r
+00001fd0: 1200 0000 7213 0000 005a 175f 5f67 656e  ....r....Z.__gen
+00001fe0: 6572 6174 655f 7375 625f 7069 705f 7265  erate_sub_pip_re
+00001ff0: 7173 4901 0000 7322 0000 0008 010a 010e  qsI...s"........
+00002000: 0208 0202 ff08 0202 fe0c 0302 020e 010c  ................
+00002010: 0110 020c 0102 010a 0102 8004 f37a 284d  .............z(M
+00002020: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
+00002030: 5f5f 6765 6e65 7261 7465 5f73 7562 5f70  __generate_sub_p
+00002040: 6970 5f72 6571 7363 0200 0000 0000 0000  ip_reqsc........
+00002050: 0000 0000 0e00 0000 0a00 0000 0300 0000  ................
+00002060: 736e 0200 0064 0164 0284 0074 00a0 0188  sn...d.d...t....
+00002070: 01a1 0144 0083 017d 0264 0364 0284 007c  ...D...}.d.d...|
+00002080: 0244 0083 0164 0464 0284 0074 00a0 0188  .D...d.d...t....
+00002090: 01a1 0144 0083 0117 0089 0087 0166 0164  ...D.........f.d
+000020a0: 0564 0284 087c 0244 0083 017d 0374 0264  .d...|.D...}.t.d
+000020b0: 0664 0284 007c 0344 0083 0183 017d 0387  .d...|.D.....}..
+000020c0: 0066 0164 0764 0284 087c 0344 0083 017d  .f.d.d...|.D...}
+000020d0: 0374 0383 007d 047c 0464 0075 0072 4374  .t...}.|.d.u.rCt
+000020e0: 0464 0883 0101 0064 0053 0074 0283 007d  .d.....d.S.t...}
+000020f0: 057c 0344 005d 5d7d 067c 06a0 0564 09a1  .|.D.]]}.|...d..
+00002100: 0172 5071 487c 006a 066a 0767 017c 06a0  .rPqH|.j.j.g.|..
+00002110: 0864 0aa1 01a2 017d 077c 0764 0b19 0064  .d.....}.|.d...d
+00002120: 0917 007c 0764 0b3c 0067 007c 06a0 0864  ...|.d.<.g.|...d
+00002130: 0aa1 01a2 017d 0874 006a 09a0 0a74 006a  .....}.t.j...t.j
+00002140: 096a 0b7c 078e 00a1 0172 7d64 0ca0 0b7c  .j.|.....r}d...|
+00002150: 0764 0064 0b85 0219 00a1 017d 096e 1d74  .d.d.......}.n.t
+00002160: 006a 09a0 0a74 006a 096a 0b7c 088e 00a1  .j...t.j.j.|....
+00002170: 0172 8e7c 0864 0d19 0064 0c17 007d 096e  .r.|.d...d...}.n
+00002180: 0c7c 006a 066a 0764 0c17 007c 06a0 0c64  .|.j.j.d...|...d
+00002190: 0a64 0ca1 0217 007d 097c 0472 a07c 047c  .d.....}.|.r.|.|
+000021a0: 0917 007d 097c 05a0 0d7c 09a1 0101 0071  ...}.|...|.....q
+000021b0: 4874 0e7c 0583 0164 0d6b 0272 ae64 0053  Ht.|...d.k.r.d.S
+000021c0: 007a 3774 006a 09a0 0b88 0164 0ea1 027d  .z7t.j.....d...}
+000021d0: 0a74 006a 09a0 0a7c 0aa1 0172 e274 0f7c  .t.j...|...r.t.|
+000021e0: 0a64 0f83 028f 187d 0b74 10a0 117c 0ba1  .d.....}.t...|..
+000021f0: 017d 0a64 107c 0a76 0072 d07c 0a64 1019  .}.d.|.v.r.|.d..
+00002200: 007d 0c6e 0269 007d 0c57 0064 0004 0004  .}.n.i.}.W.d....
+00002210: 0083 0301 006e 0831 0073 dc77 0101 0001  .....n.1.s.w....
+00002220: 0001 0059 0001 006e 0269 007d 0c57 006e  ...Y...n.i.}.W.n
+00002230: 1d04 0074 1290 0179 0201 007d 0d01 007a  ...t...y...}...z
+00002240: 1074 0464 1188 019b 0064 129d 0383 0101  .t.d.....d......
+00002250: 0069 007d 0c57 0059 0064 007d 0d7e 0d6e  .i.}.W.Y.d.}.~.n
+00002260: 0564 007d 0d7e 0d77 0177 0074 0f74 006a  .d.}.~.w.w.t.t.j
+00002270: 09a0 0b88 0164 0ea1 0264 1383 028f 1f7d  .....d...d.....}
+00002280: 0b74 137c 0583 017c 0c64 149c 027d 0574  .t.|...|.d...}.t
+00002290: 106a 147c 057c 0b64 1564 168d 0301 0074  .j.|.|.d.d.....t
+000022a0: 0464 1788 019b 009d 0283 0101 0057 0064  .d...........W.d
+000022b0: 0004 0004 0083 0301 0064 0053 0031 0090  .........d.S.1..
+000022c0: 0173 3077 0101 0001 0001 0059 0001 0064  .s0w.......Y...d
+000022d0: 0053 0029 184e 6301 0000 0000 0000 0000  .S.).Nc.........
+000022e0: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
+000022f0: 2200 0000 6700 7c00 5d0d 7d01 7c01 a000  "...g.|.].}.|...
+00002300: 6400 a101 7202 6401 7c01 7601 7202 7c01  d...r.d.|.v.r.|.
+00002310: 9102 7102 5300 2902 fa03 2e70 7972 6200  ..q.S.)....pyrb.
+00002320: 0000 2901 da08 656e 6473 7769 7468 a902  ..)...endswith..
+00002330: 7254 0000 0072 3200 0000 7212 0000 0072  rT...r2...r....r
+00002340: 1200 0000 7213 0000 0072 5600 0000 5f01  ....r....rV..._.
+00002350: 0000 7302 0000 0022 007a 414d 6f64 756c  ..s....".zAModul
+00002360: 6552 6570 6f73 6974 6f72 792e 5f5f 6765  eRepository.__ge
+00002370: 6e65 7261 7465 5f6d 6174 655f 6465 7065  nerate_mate_depe
+00002380: 6e64 656e 6369 6573 2e3c 6c6f 6361 6c73  ndencies.<locals
+00002390: 3e2e 3c6c 6973 7463 6f6d 703e 6301 0000  >.<listcomp>c...
+000023a0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+000023b0: 0053 0000 0072 7b00 0000 2902 7299 0000  .S...r{...).r...
+000023c0: 0072 4400 0000 727c 0000 00a9 0272 5400  .rD...r|.....rT.
+000023d0: 0000 da04 6669 6c65 7212 0000 0072 1200  ....filer....r..
+000023e0: 0000 7213 0000 0072 5600 0000 6001 0000  ..r....rV...`...
+000023f0: 725a 0000 0063 0100 0000 0000 0000 0000  rZ...c..........
+00002400: 0000 0200 0000 0400 0000 5300 0000 7318  ..........S...s.
+00002410: 0000 0067 007c 005d 087d 0164 007c 0176  ...g.|.].}.d.|.v
+00002420: 0172 027c 0191 0271 0253 0029 0172 6200  .r.|...q.S.).rb.
+00002430: 0000 7212 0000 0072 9b00 0000 7212 0000  ..r....r....r...
+00002440: 0072 1200 0000 7213 0000 0072 5600 0000  .r....r....rV...
+00002450: 6001 0000 7304 0000 0006 0012 0163 0100  `...s........c..
+00002460: 0000 0000 0000 0000 0000 0200 0000 0700  ................
+00002470: 0000 1300 0000 731e 0000 0067 007c 005d  ......s....g.|.]
+00002480: 0b7d 0174 0074 016a 02a0 0388 007c 01a1  .}.t.t.j.....|..
+00002490: 0283 0191 0271 0253 0072 1200 0000 2904  .....q.S.r....).
+000024a0: 7204 0000 0072 2200 0000 7223 0000 0072  r....r"...r#...r
+000024b0: 2a00 0000 729b 0000 0029 0172 2300 0000  *...r....).r#...
+000024c0: 7212 0000 0072 1300 0000 7256 0000 0064  r....r....rV...d
+000024d0: 0100 0073 0200 0000 1e00 6301 0000 0000  ...s......c.....
+000024e0: 0000 0000 0000 0003 0000 0004 0000 0053  ...............S
+000024f0: 0000 0072 7100 0000 7212 0000 0072 1200  ...rq...r....r..
+00002500: 0000 7272 0000 0072 1200 0000 7212 0000  ..rr...r....r...
+00002510: 0072 1300 0000 7256 0000 0067 0100 0072  .r....rV...g...r
+00002520: 7400 0000 6301 0000 0000 0000 0000 0000  t...c...........
+00002530: 0001 0000 0006 0000 0013 0000 0073 2600  .............s&.
+00002540: 0000 6700 7c00 5d0f 8900 7400 8700 6601  ..g.|.]...t...f.
+00002550: 6400 6401 8408 8801 4400 8301 8301 7302  d.d.....D.....s.
+00002560: 8800 9102 7102 5300 2902 6301 0000 0000  ....q.S.).c.....
+00002570: 0000 0000 0000 0002 0000 0004 0000 0013  ................
+00002580: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
+00002590: 7c01 8800 7600 9102 7102 5300 7212 0000  |...v...q.S.r...
+000025a0: 0072 1200 0000 729c 0000 00a9 01da 066d  .r....r........m
+000025b0: 6f64 756c 6572 1200 0000 7213 0000 0072  oduler....r....r
+000025c0: 5600 0000 6d01 0000 7302 0000 0014 007a  V...m...s......z
+000025d0: 4c4d 6f64 756c 6552 6570 6f73 6974 6f72  LModuleRepositor
+000025e0: 792e 5f5f 6765 6e65 7261 7465 5f6d 6174  y.__generate_mat
+000025f0: 655f 6465 7065 6e64 656e 6369 6573 2e3c  e_dependencies.<
+00002600: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00002610: 703e 2e3c 6c69 7374 636f 6d70 3e29 01da  p>.<listcomp>)..
+00002620: 0361 6e79 2901 7254 0000 0029 01da 0e6f  .any).rT...)...o
+00002630: 7269 6769 6e61 6c5f 6669 6c65 7372 9e00  riginal_filesr..
+00002640: 0000 7213 0000 0072 5600 0000 6a01 0000  ..r....rV...j...
+00002650: 730c 0000 0006 0002 0214 0102 fd02 0106  s...............
+00002660: ff7a 2c4e 6f20 6769 7420 7572 6c20 666f  .z,No git url fo
+00002670: 756e 642c 2073 6b69 7070 696e 6720 6465  und, skipping de
+00002680: 7065 6e64 656e 6369 6573 2e6a 736f 6e72  pendencies.jsonr
+00002690: 9900 0000 7246 0000 00e9 ffff ffff 7275  ....rF........ru
+000026a0: 0000 0072 0100 0000 7279 0000 0072 5200  ...r....ry...rR.
+000026b0: 0000 da03 656e 767a 0e45 7272 6f72 2072  ....envz.Error r
+000026c0: 6561 6469 6e67 207a 202f 6465 7065 6e64  eading z /depend
+000026d0: 656e 6369 6573 2e6a 736f 6e2c 2073 6b69  encies.json, ski
+000026e0: 7070 696e 6720 656e 7672 1700 0000 2902  pping envr....).
+000026f0: 727a 0000 0072 a300 0000 7218 0000 0072  rz...r....r....r
+00002700: 1900 0000 7a20 4765 6e65 7261 7465 6420  ....z Generated 
+00002710: 6465 7065 6e64 656e 6369 6573 2e6a 736f  dependencies.jso
+00002720: 6e20 666f 7220 2915 7222 0000 0072 4800  n for ).r"...rH.
+00002730: 0000 724d 0000 0072 0500 0000 7227 0000  ..rM...r....r'..
+00002740: 0072 9a00 0000 720e 0000 0072 1600 0000  .r....r....r....
+00002750: 7290 0000 0072 2300 0000 7224 0000 0072  r....r#...r$...r
+00002760: 2a00 0000 727d 0000 0072 4e00 0000 725d  *...r}...rN...r]
+00002770: 0000 0072 2b00 0000 722c 0000 0072 9100  ...r+...r,...r..
+00002780: 0000 7231 0000 0072 8c00 0000 722d 0000  ..r1...r....r-..
+00002790: 0029 0e72 1100 0000 7223 0000 00da 0566  .).r....r#.....f
+000027a0: 696c 6573 5a10 7265 6c61 7469 7665 5f69  ilesZ.relative_i
+000027b0: 6d70 6f72 7473 5a07 7572 6c5f 6769 7472  mportsZ.url_gitr
+000027c0: 9800 0000 729f 0000 005a 0574 7061 7468  ....r....Z.tpath
+000027d0: 5a12 7369 7374 6572 5f6d 6f64 756c 655f  Z.sister_module_
+000027e0: 7061 7468 7236 0000 005a 0964 6570 735f  pathr6...Z.deps_
+000027f0: 6a73 6f6e 7232 0000 0072 a300 0000 7234  jsonr2...r....r4
+00002800: 0000 0072 1200 0000 2902 72a1 0000 0072  ...r....).r....r
+00002810: 2300 0000 7213 0000 005a 1c5f 5f67 656e  #...r....Z.__gen
+00002820: 6572 6174 655f 6d61 7465 5f64 6570 656e  erate_mate_depen
+00002830: 6465 6e63 6965 735c 0100 0073 6e00 0000  dencies\...sn...
+00002840: 1403 1201 0801 08ff 1204 0202 0c01 04ff  ................
+00002850: 0a04 0202 06fe 0606 0802 0801 0401 0602  ................
+00002860: 0801 0a01 0201 1403 1001 0e02 1402 1402  ................
+00002870: 1401 0e01 1802 0402 0801 0c01 0c02 0401  ................
+00002880: 0202 0e01 0c01 0c01 0a02 0801 0a01 0402  ................
+00002890: 0280 1cfa 0280 0409 0480 1001 1001 1001  ................
+000028a0: 0880 02fe 1604 0e01 1001 1001 24fd 7a2d  ............$.z-
+000028b0: 4d6f 6475 6c65 5265 706f 7369 746f 7279  ModuleRepository
+000028c0: 2e5f 5f67 656e 6572 6174 655f 6d61 7465  .__generate_mate
+000028d0: 5f64 6570 656e 6465 6e63 6965 7363 0200  _dependenciesc..
+000028e0: 0000 0000 0000 0000 0000 0a00 0000 0a00  ................
+000028f0: 0000 4300 0000 73fc 0000 007a 0c74 00a0  ..C...s....z.t..
+00002900: 017c 01a1 017d 0274 00a0 027c 02a1 017d  .|...}.t...|...}
+00002910: 0357 006e 1f04 0074 0379 2b01 007d 0401  .W.n...t.y+..}..
+00002920: 007a 1374 0464 017c 019b 009d 0283 0101  .z.t.d.|........
+00002930: 0074 047c 0483 0101 0069 0057 0006 0059  .t.|.....i.W...Y
+00002940: 0064 007d 047e 0453 0064 007d 047e 0477  .d.}.~.S.d.}.~.w
+00002950: 0177 007c 00a0 057c 01a1 0101 0067 007d  .w.|...|.....g.}
+00002960: 057c 017c 006a 066a 076b 0272 4674 00a0  .|.|.j.j.k.rFt..
+00002970: 0864 027c 0364 03a1 0301 007c 00a0 0964  .d.|.d.....|...d
+00002980: 02a1 0101 006e 1d74 00a0 0874 0a6a 0ba0  .....n.t...t.j..
+00002990: 0c7c 0164 02a1 027c 0364 03a1 0301 007c  .|.d...|.d.....|
+000029a0: 00a0 0974 0a6a 0ba0 0c7c 0164 02a1 02a1  ...t.j...|.d....
+000029b0: 0101 0074 0464 047c 019b 009d 0283 0101  ...t.d.|........
+000029c0: 007c 0344 005d 147d 067c 0664 0519 007d  .|.D.].}.|.d...}
+000029d0: 077c 0664 0619 007d 087c 077c 0864 079c  .|.d...}.|.|.d..
+000029e0: 027d 097c 05a0 0d7c 09a1 0101 0071 6564  .}.|...|.....qed
+000029f0: 087c 0569 0153 0029 094e 7a26 4572 726f  .|.i.S.).Nz&Erro
+00002a00: 7220 6765 6e65 7261 7469 6e67 2072 6571  r generating req
+00002a10: 7569 7265 6d65 6e74 732e 7478 7420 666f  uirements.txt fo
+00002a20: 7220 7278 0000 007a 023e 3d7a 1f47 656e  r rx...z.>=z.Gen
+00002a30: 6572 6174 6564 2072 6571 7569 7265 6d65  erated requireme
+00002a40: 6e74 732e 7478 7420 666f 7220 726c 0000  nts.txt for rl..
+00002a50: 00da 0776 6572 7369 6f6e 2902 726c 0000  ...version).rl..
+00002a60: 0072 a500 0000 da03 7069 7029 0e72 0800  .r......pip).r..
+00002a70: 0000 5a0f 6765 745f 616c 6c5f 696d 706f  ..Z.get_all_impo
+00002a80: 7274 735a 1067 6574 5f69 6d70 6f72 745f  rtsZ.get_import_
+00002a90: 6c6f 6361 6c72 3100 0000 7227 0000 00da  localr1...r'....
+00002aa0: 2d5f 4d6f 6475 6c65 5265 706f 7369 746f  -_ModuleReposito
+00002ab0: 7279 5f5f 6765 6e65 7261 7465 5f6d 6174  ry__generate_mat
+00002ac0: 655f 6465 7065 6e64 656e 6369 6573 720e  e_dependenciesr.
+00002ad0: 0000 0072 1600 0000 5a1a 6765 6e65 7261  ...r....Z.genera
+00002ae0: 7465 5f72 6571 7569 7265 6d65 6e74 735f  te_requirements_
+00002af0: 6669 6c65 da30 5f4d 6f64 756c 6552 6570  file.0_ModuleRep
+00002b00: 6f73 6974 6f72 795f 5f61 6464 5f69 6e64  ository__add_ind
+00002b10: 6578 5f75 726c 5f74 6f5f 7265 7175 6972  ex_url_to_requir
+00002b20: 656d 656e 7473 7222 0000 0072 2300 0000  ementsr"...r#...
+00002b30: 722a 0000 0072 8e00 0000 290a 7211 0000  r*...r....).r...
+00002b40: 0072 2300 0000 da07 696d 706f 7274 735a  .r#.....importsZ
+00002b50: 1169 6d70 6f72 745f 696e 666f 5f6c 6f63  .import_info_loc
+00002b60: 616c 7234 0000 005a 0b69 6d70 6f72 745f  alr4...Z.import_
+00002b70: 696e 666f 5a02 696d 726c 0000 0072 a500  infoZ.imrl...r..
+00002b80: 0000 da03 7265 7372 1200 0000 7212 0000  ....resr....r...
+00002b90: 0072 1300 0000 5a1b 5f5f 6765 6e65 7261  .r....Z.__genera
+00002ba0: 7465 5f70 6970 5f72 6571 7569 7265 6d65  te_pip_requireme
+00002bb0: 6e74 73a6 0100 0073 3a00 0000 0202 0a01  nts....s:.......
+00002bc0: 0e04 0e01 0e01 0801 1002 0880 02fc 0a06  ................
+00002bd0: 0402 0c02 0401 0601 04ff 0c03 0403 1001  ................
+00002be0: 04ff 1403 0e01 0802 0801 0801 0203 0201  ................
+00002bf0: 06fe 0c05 0802 7a2c 4d6f 6475 6c65 5265  ......z,ModuleRe
+00002c00: 706f 7369 746f 7279 2e5f 5f67 656e 6572  pository.__gener
+00002c10: 6174 655f 7069 705f 7265 7175 6972 656d  ate_pip_requirem
+00002c20: 656e 7473 729f 0000 0063 0200 0000 0000  entsr....c......
+00002c30: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00002c40: 0000 731e 0000 007c 0164 006b 0272 097c  ..s....|.d.k.r.|
+00002c50: 006a 00a0 01a1 0053 007c 006a 00a0 027c  .j.....S.|.j...|
+00002c60: 01a1 0153 0072 0d00 0000 2903 7210 0000  ...S.r....).r...
+00002c70: 00da 0773 756d 6d61 7279 728c 0000 0029  ...summaryr....)
+00002c80: 0272 1100 0000 729f 0000 0072 1200 0000  .r....r....r....
+00002c90: 7212 0000 0072 1300 0000 728c 0000 00d2  r....r....r.....
+00002ca0: 0100 0073 0600 0000 0801 0a01 0c01 7a15  ...s..........z.
+00002cb0: 4d6f 6475 6c65 5265 706f 7369 746f 7279  ModuleRepository
+00002cc0: 2e6c 6973 7463 0100 0000 0000 0000 0000  .listc..........
+00002cd0: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
+00002ce0: 0000 007c 006a 00a0 01a1 0053 0072 0d00  ...|.j.....S.r..
+00002cf0: 0000 2902 7210 0000 0072 ab00 0000 2901  ..).r....r....).
+00002d00: 7211 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00002d10: 1300 0000 da10 6765 745f 6d61 7465 5f73  ......get_mate_s
+00002d20: 756d 6d61 7279 d701 0000 7302 0000 000a  ummary....s.....
+00002d30: 017a 214d 6f64 756c 6552 6570 6f73 6974  .z!ModuleReposit
+00002d40: 6f72 792e 6765 745f 6d61 7465 5f73 756d  ory.get_mate_sum
+00002d50: 6d61 7279 da07 7061 636b 6167 6563 0200  mary..packagec..
+00002d60: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00002d70: 0000 4300 0000 7310 0000 007c 006a 00a0  ..C...s....|.j..
+00002d80: 017c 01a1 0101 0064 0053 0072 0d00 0000  .|.....d.S.r....
+00002d90: 2902 7210 0000 0072 3700 0000 2902 7211  ).r....r7...).r.
+00002da0: 0000 0072 ad00 0000 7212 0000 0072 1200  ...r....r....r..
+00002db0: 0000 7213 0000 0072 3700 0000 da01 0000  ..r....r7.......
+00002dc0: 7302 0000 0010 017a 204d 6f64 756c 6552  s......z ModuleR
+00002dd0: 6570 6f73 6974 6f72 792e 696e 7374 616c  epository.instal
+00002de0: 6c5f 7061 636b 6167 6529 0146 720d 0000  l_package).Fr...
+00002df0: 0029 16da 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
+00002e00: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00002e10: 6c6e 616d 655f 5fda 0462 6f6f 6c72 1400  lname__..boolr..
+00002e20: 0000 da0c 7374 6174 6963 6d65 7468 6f64  ....staticmethod
+00002e30: da03 7374 7272 3500 0000 723a 0000 0072  ..strr5...r:...r
+00002e40: 4200 0000 7241 0000 0072 8c00 0000 7260  B...rA...r....r`
+00002e50: 0000 0072 a800 0000 7265 0000 0072 4000  ...r....re...r@.
+00002e60: 0000 728b 0000 0072 a700 0000 7264 0000  ..r....r....rd..
+00002e70: 0072 ac00 0000 7209 0000 0072 3700 0000  .r....r....r7...
+00002e80: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00002e90: 1300 0000 720b 0000 0014 0000 0073 2400  ....r........s$.
+00002ea0: 0000 0800 1001 0207 1001 0e29 0e03 1006  ...........)....
+00002eb0: 1212 0e0e 081d 0815 007f 0829 0813 084a  ...........)...J
+00002ec0: 102c 0805 1203 720b 0000 0029 1672 2c00  .,....r....).r,.
+00002ed0: 0000 7222 0000 0072 5e00 0000 7228 0000  ..r"...r^...r(..
+00002ee0: 0072 9400 0000 5a0e 6d6f 6475 6c65 5f6d  .r....Z.module_m
+00002ef0: 616e 6167 6572 7203 0000 005a 0e75 7469  anagerr....Z.uti
+00002f00: 6c73 2e65 7870 5f75 7469 6c72 0400 0000  ls.exp_utilr....
+00002f10: 5a0e 7574 696c 732e 6769 745f 7574 696c  Z.utils.git_util
+00002f20: 7205 0000 005a 0e73 6f75 7263 6573 2e72  r....Z.sources.r
+00002f30: 656d 6f74 6572 0600 0000 5a13 736f 7572  emoter....Z.sour
+00002f40: 6365 732e 6c6f 6361 6c2e 6c6f 6361 6c72  ces.local.localr
+00002f50: 0700 0000 7208 0000 0072 ad00 0000 7209  ....r....r....r.
+00002f60: 0000 00da 0674 7970 696e 6772 0a00 0000  .....typingr....
+00002f70: da04 6970 6462 720b 0000 0072 1200 0000  ..ipdbr....r....
+00002f80: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00002f90: 083c 6d6f 6475 6c65 3e01 0000 0073 1e00  .<module>....s..
+00002fa0: 0000 0800 0801 0801 0801 0802 0c02 0c01  ................
+00002fb0: 0c01 0c01 0c01 0c01 0c02 0c01 0801 1203  ................
```

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/module_manager.py` & `yerbamate-0.9.24/packages/yerbamate/api/data/module_manager.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/module_repository.py` & `yerbamate-0.9.24/packages/yerbamate/api/data/module_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         self.package_manager = ModuleManager(config)
         self.remote = RemoteDataSource()
         self.local = LocalDataSource(config)
         # self.__generate_pip_requirements(self.config.project)
 
     @staticmethod
     def init_project(project_name: str):
-
         if not os.path.exists(project_name):
             os.mkdir(project_name)
             os.chdir(project_name)
         else:
             print("Project already exists")
             sys.exit(1)
 
@@ -65,15 +64,14 @@
                 )
             )
 
         except Exception as e:
             print(e)
 
     def install_url(self, url: str, *args, **kwargs):
-
         self.package_manager.install_package(url, *args, **kwargs)
 
     def auto(self, command: str, *args):
         if command == "export":
             self.__export()
         elif command in ["init", "fix", "i"]:
             self.__generate__init__(self.config.project)
@@ -115,15 +113,15 @@
             lines = f.readlines()
         linecount = len(lines)
         lines = [
             line
             for line in lines
             if not ".egg>=info" in line
             and not ".egg==info" in line
-            and not ".egg~=info" in line
+            and not ".egg>=info" in line
         ]
 
         # remove +cu{numbers} version form lines
         # regex for numbers with at least 1 digit
         regex = re.compile(r"\+cu\d+")
         lines = [regex.sub("", line) for line in lines]
 
@@ -136,15 +134,14 @@
                     f.write(line)
         elif linecount != len(lines):
             with open(os.path.join(path), "w") as f:
                 for line in lines:
                     f.write(line)
 
     def __generate_deps_in_depth(self, root_path):
-
         # init__path = os.path.join(path, "__init__.py")
 
         for dir in os.listdir(root_path):
             if dir.startswith(".") or dir.startswith("__"):
                 continue
             path = os.path.join(root_path, dir)
             if os.path.isdir(path):
@@ -158,40 +155,40 @@
                     and self.config.project in root_path
                 ):
                     self.__generate_pip_requirements(path)
 
                 self.__generate_deps_in_depth(path)
 
     def __export(self, *args, **kwargs):
-
         self.__generate_sub_pip_reqs()
 
         modules = self.list()
 
         table = []
 
         for key, value in modules.items():
             if type(value) is list:
                 table.append([{"type": key, "name": name} for name in value])
+                # if empty list, type and name are the same
+                if len(value) == 0:
+                    table.append([{"type": key, "name": key}])
             elif type(value) is dict:
-                table.append([{"type": key, "name": name}
-                             for name in value.keys()])
+                table.append([{"type": key, "name": name} for name in value.keys()])
 
         # ipdb.set_trace()
 
         table = [item for sublist in table for item in sublist]
 
         # add url to each item in table
         deps = set()
 
         base_url = parse_url_from_git()
         user_name = base_url.split("/")[3]
         repo_name = base_url.split("/")[4]
         for item in table:
-
             item[
                 "url"
             ] = f"{base_url}{self.config.project}/{item['type']}/{item['name']}"
             item[
                 "short_url"
             ] = f"{user_name}/{repo_name}/{self.config.project}/{item['type']}/{item['name']}"
 
@@ -208,38 +205,46 @@
             path = os.path.join(
                 self.config.project, item["type"], item["name"], "requirements.txt"
             )
             dep_path = os.path.join(
                 self.config.project, item["type"], item["name"], "dependencies.json"
             )
 
+            root_dep_path = os.path.join(
+                self.config.project, item["type"], "requirements.txt"
+            )
+
             if os.path.exists(path):
                 with open(path, "r") as f:
                     item["dependencies"] = f.readlines()
             if os.path.exists(dep_path):
                 with open(dep_path, "r") as f:
                     if "dependencies" in item:
                         item["dependencies"] += json.load(f)["dependencies"]
                     else:
                         item["dependencies"] = json.load(f)["dependencies"]
 
                     # item["module_dependencies"] = json.load(f)
+            if os.path.exists(root_dep_path):
+                with open(root_dep_path, "r") as f:
+                    item["dependencies"] = f.readlines()
 
             if "dependencies" in item:
                 item["dependencies"] = [
                     dep.replace("\n", "") for dep in item["dependencies"]
                 ]
 
-            deps.update(item["dependencies"])
+                deps.update(item["dependencies"])
 
-        # remove github urls from dependencies
-        deps = [dep for dep in deps if not "https://github" in dep]
+        # remove github urls from dependencies if it
+        deps = [
+            dep for dep in deps if not ("https://github" in dep and not "+git" in dep)
+        ]
         # set index urls should be on top, sort so that --extra-index-url is on top
-        deps = sorted(
-            deps, key=lambda x: "--extra-index-url" in x, reverse=True)
+        deps = sorted(deps, key=lambda x: "--extra-index-url" in x, reverse=True)
         # remove empty lines
         deps = [dep for dep in deps if dep != "\n" or dep != " " or dep != ""]
 
         # save deps in requirements.txt
         with open("requirements.txt", "w") as f:
             for dep in deps:
                 f.write(dep + "\n")
@@ -318,15 +323,14 @@
 
         with open("exports.tex", "w") as f:
             f.write(latex_table)
 
         print("Exported to export.md")
 
     def __generate_sub_pip_reqs(self):
-
         root_path = self.config.project
         self.__generate_deps_in_depth(root_path)
 
         for dir in os.listdir("."):
             if (
                 dir.startswith(".")
                 or dir.startswith("__")
@@ -340,22 +344,20 @@
                 if not os.path.exists(init__path):
                     continue
                 self.__generate_pip_requirements(path)
 
     def __generate_mate_dependencies(self, path):
         # ipdb.set_trace()
 
-        files = [f for f in os.listdir(
-            path) if f.endswith(".py") and "__" not in f]
+        files = [f for f in os.listdir(path) if f.endswith(".py") and "__" not in f]
         original_files = [file.replace(".py", "") for file in files] + [
             f for f in os.listdir(path) if "__" not in f
         ]
 
-        relative_imports = [get_relative_imports(
-            os.path.join(path, f)) for f in files]
+        relative_imports = [get_relative_imports(os.path.join(path, f)) for f in files]
         # flatten array to unique set
         relative_imports = set(
             [item for sublist in relative_imports for item in sublist]
         )
 
         relative_imports = [
             module
@@ -367,15 +369,14 @@
 
         if url_git is None:
             print("No git url found, skipping dependencies.json")
             return
 
         deps = set()
         for module in relative_imports:
-
             if module.endswith(".py"):
                 continue
             # if its a python file, return parent module
 
             tpath = [self.config.project, *module.split(".")]
             tpath[-1] = tpath[-1] + ".py"
 
@@ -393,15 +394,14 @@
                 url = url_git + url
             deps.add(url)
 
         if len(deps) == 0:
             return
 
         try:
-
             deps_json = os.path.join(path, "dependencies.json")
             if os.path.exists(deps_json):
                 with open(deps_json, "r") as f:
                     # ipdb.set_trace()
                     deps_json = json.load(f)
                     if "env" in deps_json:
                         env = deps_json["env"]
@@ -416,41 +416,45 @@
 
         with open(os.path.join(path, "dependencies.json"), "w") as f:
             deps = {"dependencies": list(deps), "env": env}
             json.dump(deps, f, indent=4)
             print(f"Generated dependencies.json for {path}")
 
     def __generate_pip_requirements(self, path):
-
         # ipdb.set_trace()
-        imports = pipreqs.get_all_imports(path)
-        # import_info_remote = pipreqs.get_imports_info(imports)
+        try:
+            imports = pipreqs.get_all_imports(path)
 
-        import_info_local = pipreqs.get_import_local(imports)
+            # import_info_remote = pipreqs.get_imports_info(imports)
+
+            import_info_local = pipreqs.get_import_local(imports)
+        except Exception as e:
+            print(f"Error generating requirements.txt for {path}")
+            print(e)
+            # raise e
+            return {}
 
         self.__generate_mate_dependencies(path)
 
         import_info = []
 
         if path == self.config.project:
             pipreqs.generate_requirements_file(
-                "requirements.txt", import_info_local, "~="
+                "requirements.txt", import_info_local, ">="
             )
             self.__add_index_url_to_requirements("requirements.txt")
 
         else:
             pipreqs.generate_requirements_file(
-                os.path.join(path, "requirements.txt"), import_info_local, "~="
+                os.path.join(path, "requirements.txt"), import_info_local, ">="
             )
-            self.__add_index_url_to_requirements(
-                os.path.join(path, "requirements.txt"))
+            self.__add_index_url_to_requirements(os.path.join(path, "requirements.txt"))
             print(f"Generated requirements.txt for {path}")
 
         for im in import_info_local:
-
             name = im["name"]
             version = im["version"]
 
             res = {
                 "name": name,
                 "version": version,
             }
```

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/package.py` & `yerbamate-0.9.24/packages/yerbamate/api/data/package.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/io.py` & `yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/io.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/sources/local/local.py` & `yerbamate-0.9.24/packages/yerbamate/api/data/sources/local/local.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/sources/remote/remote.py` & `yerbamate-0.9.24/packages/yerbamate/api/data/sources/remote/remote.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/utils/git_util.py` & `yerbamate-0.9.24/packages/yerbamate/api/data/utils/git_util.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/data/utils/gitdir.py` & `yerbamate-0.9.24/packages/yerbamate/api/data/utils/gitdir.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/api/mate_api.py` & `yerbamate-0.9.24/packages/yerbamate/api/mate_api.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/environment.py` & `yerbamate-0.9.24/packages/yerbamate/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-
 import json
 import os
 import shutil
 import sys
 import ipdb
 
 
 ENV_KEY = "env"
 
 
 class Environment(dict):
-
     def __init__(self):
-
         # default restart, test to False
         self.restart = False
         self.test = False
         self.train = False
         self.sample = False
         self.hparams = {}
+        self.action = None
 
         # set command to True
         try:
             setattr(self, sys.argv[1], True)
+            setattr(self, "action", sys.argv[1])
         except:
             pass
 
         self.args = sys.argv[1:]
 
         self._root = self.__find_root()
+        self._root_dir = os.path.dirname(self._root)
+
+        if self._root_dir not in sys.path:
+            sys.path.append(self._root_dir)
 
         # parse python -m module train arg=1 arg2=2
         for arg in sys.argv:
             if "=" not in arg:
                 continue
             key, value = arg.split("=")
             value = self.convert_str_to_data(value)
@@ -43,19 +46,20 @@
             setattr(self, key, value)
             self.hparams[key] = value
 
         self._path = sys.argv[0]
         if "bin/mate" in self._path:
             self.name = os.path.join(*sys.argv[2:4])
             self._path = os.path.join(
-                self._root, "experiments", sys.argv[2],  sys.argv[3] + ".py")
+                self._root, "experiments", sys.argv[2], sys.argv[3] + ".py"
+            )
             # detect path to experiment
         else:
             self.name = self._path.split("/")[-2:]
-            self.name = os.path.join(*self.name)[: -3]
+            self.name = os.path.join(*self.name)[:-3]
 
         self.__set_env()
 
         if self.train:
             self.__generate_experiment()
 
     def convert_str_to_data(self, input):
@@ -78,20 +82,39 @@
         path = os.getcwd()
 
         if os.path.exists(os.path.join(path, "mate.json")):
             conf = json.load(open(os.path.join(path, "mate.json"), "r"))
 
             return os.path.join(path, conf["project"])
 
+        # if not found, try to go up up two levels
+        max_recursion = 4
+        for i in range(max_recursion):
+            # os.getcwd is a dir, go up one level
+            path = os.path.dirname(path)
+            # print(path)
+            if os.path.exists(os.path.join(path, "mate.json")):
+                conf = json.load(open(os.path.join(path, "mate.json"), "r"))
+
+                return os.path.join(path, conf["project"])
+
+        raise Exception("Could not find root of project")
+
         return None
 
     def __generate_experiment(self):
         # copies the experiment to the results folder
-        results = ["results", "results_path",
-                   "results_dir", "save", "save_path", "save_dir"]
+        results = [
+            "results",
+            "results_path",
+            "results_dir",
+            "save",
+            "save_path",
+            "save_dir",
+        ]
         result = None
         for key in results:
             if key in self.env:
                 result = self.env[key]
                 break
         if result is None:
             return
@@ -108,18 +131,18 @@
             params_file = os.path.join(result, "experiment.json")
             # dump self to params
             # overwrite if exists
             with open(params_file, "w") as f:
                 json.dump(dict(self.hparams), f, indent=4)
 
     def __set_env(self):
-        mate_conf_path = os.path.join("mate.json")
+        mate_conf_path = os.path.join(self._root_dir, "mate.json")
         conf = json.load(open(mate_conf_path, "r"))
 
-        env_path = os.path.join("env.json")
+        env_path = os.path.join(self._root_dir, "env.json")
         if not os.path.exists(env_path):
             print("Environment file not found, creating one with defaults: env.json")
 
             if ENV_KEY in conf:
                 required_keys = conf[ENV_KEY].keys()
             else:
                 required_keys = ["results"]
@@ -147,44 +170,52 @@
                         # print(f"Environment variable {key} set to {os.environ[key]} from shell.")
                     else:
                         env_not_found.append(key)
                         env[key] = value
 
         if len(env_not_found) > 0:
             print(
-                f"Environment variables not found. Set them in env.json or in your shell.")
+                f"Environment variables not found. Set them in env.json or in your shell."
+            )
             for key in env_not_found:
-                desc = conf[ENV_KEY][key] if key in conf[ENV_KEY] else "Required environment variable"
+                desc = (
+                    conf[ENV_KEY][key]
+                    if key in conf[ENV_KEY]
+                    else "Required environment variable"
+                )
                 print(f"{key} : {desc}")
 
             print("Exiting...")
             sys.exit(1)
 
         # automatically append experiment name to results path
         search_results = ["auto_save"]
         for key in search_results:
             if key in env:
                 env[key] = os.path.join(env[key], *self.name.split("/"))
                 # env["results"] = env[key]
                 break
-            if os.environ.get(key, None) is not None and os.environ.get(key, None) != "":
+            if (
+                os.environ.get(key, None) is not None
+                and os.environ.get(key, None) != ""
+            ):
                 env[key] = os.environ.get(key)
                 # env["results"] = env[key]
                 break
 
         if len(env) == 0:
             print(
-                f"results/save_dir/save environment variable is empty. Set it in env.json or in your shell.")
+                f"results/save_dir/save environment variable is empty. Set it in env.json or in your shell."
+            )
             print("Exiting...")
             sys.exit(1)
 
         setattr(self, "env", env)
 
     def __getitem__(self, key):
-
         # default to environment variables
 
         if key in self.hparams:
             return self.hparams[key]
 
         res = os.environ.get(key, None)
 
@@ -201,26 +232,27 @@
                 return self.hparams[key]
 
             if key in self.__dict__:
                 return self.__dict__[key]
 
             if res is None or res == "":
                 print(
-                    f"Environment variable {key} not found. Set it in env.json or in your shell.")
+                    f"Environment variable {key} not found. Set it in env.json or in your shell."
+                )
                 print(
-                    "Or set as an argument to the script: python -m module.train arg=1 arg2=2")
+                    "Or set as an argument to the script: python -m module.train arg=1 arg2=2"
+                )
                 print("Exiting...")
                 sys.exit(1)
             else:
                 return res
 
         return super().__getitem__(key)
 
     def __getitem__(self, key, default=None):
-
         # default to hparams
         if key in self.hparams:
             return self.hparams[key]
 
         # default to environment variables
         res = os.environ.get(key, None)
```

### Comparing `yerbamate-0.9.239/packages/yerbamate/mate.py` & `yerbamate-0.9.24/packages/yerbamate/mate.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,14 +177,32 @@
         shutil.copytree(module_path, dest_path)
 
         print(f"Module {module}/{name} cloned to {dest_path}")
 
     def snapshot(self, model_name: str):
         pass
 
+    def data(self, base_module, sub_module):
+
+        module = [self.config.project, 'data', base_module, sub_module]
+        module = ".".join(module)
+
+        try:
+            __import__(module)
+        except Exception as e:
+            print(f"Error in loading {base_module}/{sub_module}")
+            print("Available experiments:")
+            self.list(base_module)
+            traceback.print_exc()
+
+            # print(e)
+            sys.exit(1)
+
+
+
     def train(self, exp_module: str, exp: str, *args, **kwargs):
         """
         Executes an experiment.
 
         Usage: ``mate train {module} {experiment}``
 
         Args:
```

### Comparing `yerbamate-0.9.239/packages/yerbamate/mate_cli.py` & `yerbamate-0.9.24/packages/yerbamate/mate_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,14 @@
         elif arg.lower() == "false":
             return False
         else:
             raise ValueError("Not a boolean")
 
     if len(annotations) < len(args):
         annotations = annotations + (good_guess_type,) * (len(args) - len(annotations))
-    from typing import Union
 
     for i, (arg, annotation) in enumerate(zip(args, annotations)):
         if annotation == bool:
             annotation = boolean_type
         elif annotation == inspect._empty:
             annotation = good_guess_type
         elif hasattr(annotation, "__args__"):
@@ -336,10 +335,11 @@
             pos_args, kwargs = collect_args(raw_method_args, annotations)
             if action == "init":
                 Mate.init(*pos_args, **kwargs)
             else:
                 mate = Mate()
                 if hasattr(mate, action):
                     getattr(mate, action)(*pos_args, **kwargs)
-                else:
-                    if len(pos_args) == 2:
+                elif len(pos_args) == 2:
                         mate.train(*pos_args)
+                else:
+                    mate.run_module(sys.argv[1], sys.argv[2], sys.argv[3])
```

### Comparing `yerbamate-0.9.239/packages/yerbamate/utils/__init__.py` & `yerbamate-0.9.24/packages/yerbamate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc` & `yerbamate-0.9.24/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/utils/bunch.py` & `yerbamate-0.9.24/packages/yerbamate/utils/bunch.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/utils/git_url_parser.py` & `yerbamate-0.9.24/packages/yerbamate/utils/git_url_parser.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/utils/utils.py` & `yerbamate-0.9.24/packages/yerbamate/utils/utils.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate/yerbamate.egg-info/PKG-INFO` & `yerbamate-0.9.24/packages/yerbamate/yerbamate.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.239/packages/yerbamate.egg-info/PKG-INFO` & `yerbamate-0.9.24/packages/yerbamate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yerbamate
-Version: 0.9.239
+Version: 0.9.24
 Summary:  A python module and experiment manager for deep learning
 Home-page: https://github.com/oalee/yerbamate
 Author: Giulio Zani, Ali Rahimi
 Author-email: yerba.mate.dl@proton.me
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `yerbamate-0.9.239/setup.py` & `yerbamate-0.9.24/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setup(
     name="yerbamate",
     description=" A python module and experiment manager for deep learning",
     author="Giulio Zani, Ali Rahimi",
     author_email="yerba.mate.dl@proton.me",
     url="https://github.com/oalee/yerbamate",
     python_requires=">=3.6",
-    version="0.9.239",
+    version="0.9.24",
     packages=find_packages("packages", exclude=["tests"]),
     include_package_data=True,
     package_dir={"": "packages/"},
     license="Apache License 2.0",
     license_files=("LICENSE",),
     long_description=long_description,
     long_description_content_type='text/markdown',
```

