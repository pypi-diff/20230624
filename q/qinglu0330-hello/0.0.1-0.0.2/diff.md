# Comparing `tmp/qinglu0330_hello-0.0.1.tar.gz` & `tmp/qinglu0330_hello-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qinglu0330_hello-0.0.1.tar", last modified: Sat Jun 24 01:51:04 2023, max compression
+gzip compressed data, was "qinglu0330_hello-0.0.2.tar", last modified: Sat Jun 24 02:04:36 2023, max compression
```

## Comparing `qinglu0330_hello-0.0.1.tar` & `qinglu0330_hello-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 qinglu     (501) staff       (20)        0 2023-06-24 01:51:04.445086 qinglu0330_hello-0.0.1/
--rw-r--r--   0 qinglu     (501) staff       (20)       60 2023-06-24 01:51:04.444974 qinglu0330_hello-0.0.1/PKG-INFO
--rw-r--r--   0 qinglu     (501) staff       (20)       15 2023-06-24 01:28:10.000000 qinglu0330_hello-0.0.1/hello.py
-drwxr-xr-x   0 qinglu     (501) staff       (20)        0 2023-06-24 01:51:04.444831 qinglu0330_hello-0.0.1/qinglu0330_hello.egg-info/
--rw-r--r--   0 qinglu     (501) staff       (20)       60 2023-06-24 01:51:04.000000 qinglu0330_hello-0.0.1/qinglu0330_hello.egg-info/PKG-INFO
--rw-r--r--   0 qinglu     (501) staff       (20)      177 2023-06-24 01:51:04.000000 qinglu0330_hello-0.0.1/qinglu0330_hello.egg-info/SOURCES.txt
--rw-r--r--   0 qinglu     (501) staff       (20)        1 2023-06-24 01:51:04.000000 qinglu0330_hello-0.0.1/qinglu0330_hello.egg-info/dependency_links.txt
--rw-r--r--   0 qinglu     (501) staff       (20)        6 2023-06-24 01:51:04.000000 qinglu0330_hello-0.0.1/qinglu0330_hello.egg-info/top_level.txt
--rw-r--r--   0 qinglu     (501) staff       (20)       38 2023-06-24 01:51:04.445120 qinglu0330_hello-0.0.1/setup.cfg
--rw-r--r--   0 qinglu     (501) staff       (20)      112 2023-06-24 01:50:51.000000 qinglu0330_hello-0.0.1/setup.py
+drwxr-xr-x   0 qinglu     (501) staff       (20)        0 2023-06-24 02:04:36.759989 qinglu0330_hello-0.0.2/
+-rw-r--r--   0 qinglu     (501) staff       (20)       60 2023-06-24 02:04:36.759882 qinglu0330_hello-0.0.2/PKG-INFO
+drwxr-xr-x   0 qinglu     (501) staff       (20)        0 2023-06-24 02:04:36.759288 qinglu0330_hello-0.0.2/qinglu0330_hello/
+-rw-r--r--   0 qinglu     (501) staff       (20)       15 2023-06-24 01:28:10.000000 qinglu0330_hello-0.0.2/qinglu0330_hello/hello.py
+drwxr-xr-x   0 qinglu     (501) staff       (20)        0 2023-06-24 02:04:36.759741 qinglu0330_hello-0.0.2/qinglu0330_hello.egg-info/
+-rw-r--r--   0 qinglu     (501) staff       (20)       60 2023-06-24 02:04:36.000000 qinglu0330_hello-0.0.2/qinglu0330_hello.egg-info/PKG-INFO
+-rw-r--r--   0 qinglu     (501) staff       (20)      194 2023-06-24 02:04:36.000000 qinglu0330_hello-0.0.2/qinglu0330_hello.egg-info/SOURCES.txt
+-rw-r--r--   0 qinglu     (501) staff       (20)        1 2023-06-24 02:04:36.000000 qinglu0330_hello-0.0.2/qinglu0330_hello.egg-info/dependency_links.txt
+-rw-r--r--   0 qinglu     (501) staff       (20)       17 2023-06-24 02:04:36.000000 qinglu0330_hello-0.0.2/qinglu0330_hello.egg-info/top_level.txt
+-rw-r--r--   0 qinglu     (501) staff       (20)       38 2023-06-24 02:04:36.760022 qinglu0330_hello-0.0.2/setup.cfg
+-rw-r--r--   0 qinglu     (501) staff       (20)      112 2023-06-24 02:04:30.000000 qinglu0330_hello-0.0.2/setup.py
```

