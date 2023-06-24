# Comparing `tmp/hi-cli-jash-0.1.0.tar.gz` & `tmp/hi-cli-jash-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hi-cli-jash-0.1.0.tar", last modified: Sat Jun 24 04:52:20 2023, max compression
+gzip compressed data, was "hi-cli-jash-0.1.1.tar", last modified: Sat Jun 24 05:03:06 2023, max compression
```

## Comparing `hi-cli-jash-0.1.0.tar` & `hi-cli-jash-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 04:52:20.041847 hi-cli-jash-0.1.0/
--rw-rw-rw-   0        0        0      172 2023-06-24 04:52:20.040841 hi-cli-jash-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 04:52:20.038950 hi-cli-jash-0.1.0/hi_cli_jash.egg-info/
--rw-rw-rw-   0        0        0      172 2023-06-24 04:52:19.000000 hi-cli-jash-0.1.0/hi_cli_jash.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-06-24 04:52:19.000000 hi-cli-jash-0.1.0/hi_cli_jash.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 04:52:19.000000 hi-cli-jash-0.1.0/hi_cli_jash.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-24 04:52:19.000000 hi-cli-jash-0.1.0/hi_cli_jash.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 04:52:19.000000 hi-cli-jash-0.1.0/hi_cli_jash.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 04:52:20.041847 hi-cli-jash-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      353 2023-06-24 04:52:15.000000 hi-cli-jash-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:03:06.417986 hi-cli-jash-0.1.1/
+-rw-rw-rw-   0        0        0      172 2023-06-24 05:03:06.417986 hi-cli-jash-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-06-24 04:47:58.000000 hi-cli-jash-0.1.1/hi.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:03:06.415984 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/
+-rw-rw-rw-   0        0        0      172 2023-06-24 05:03:06.000000 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-06-24 05:03:06.000000 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 05:03:06.000000 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-24 05:03:06.000000 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        3 2023-06-24 05:03:06.000000 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 05:03:06.419185 hi-cli-jash-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      349 2023-06-24 05:02:33.000000 hi-cli-jash-0.1.1/setup.py
```

