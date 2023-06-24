# Comparing `tmp/cryptoowl-0.0.1.tar.gz` & `tmp/cryptoowl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cryptoowl-0.0.1.tar", last modified: Sat Jun 24 20:09:41 2023, max compression
+gzip compressed data, was "cryptoowl-0.0.2.tar", last modified: Sat Jun 24 20:34:12 2023, max compression
```

## Comparing `cryptoowl-0.0.1.tar` & `cryptoowl-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 20:09:41.000000 cryptoowl-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-24 20:09:41.000000 cryptoowl-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-24 20:09:26.000000 cryptoowl-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 20:09:41.000000 cryptoowl-0.0.1/cryptoowl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-24 20:09:41.000000 cryptoowl-0.0.1/cryptoowl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-24 20:09:41.000000 cryptoowl-0.0.1/cryptoowl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 20:09:41.000000 cryptoowl-0.0.1/cryptoowl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 20:09:41.000000 cryptoowl-0.0.1/cryptoowl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 20:09:41.000000 cryptoowl-0.0.1/cryptoowl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 20:09:41.000000 cryptoowl-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 20:09:26.000000 cryptoowl-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 20:34:12.987843 cryptoowl-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-24 20:34:07.000000 cryptoowl-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-24 20:34:12.987843 cryptoowl-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-24 20:34:07.000000 cryptoowl-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 20:34:12.987843 cryptoowl-0.0.2/cryptoowl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-24 20:34:12.000000 cryptoowl-0.0.2/cryptoowl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-24 20:34:12.000000 cryptoowl-0.0.2/cryptoowl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 20:34:12.000000 cryptoowl-0.0.2/cryptoowl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 20:34:12.000000 cryptoowl-0.0.2/cryptoowl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 20:34:12.000000 cryptoowl-0.0.2/cryptoowl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 20:34:12.987843 cryptoowl-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 20:34:07.000000 cryptoowl-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

