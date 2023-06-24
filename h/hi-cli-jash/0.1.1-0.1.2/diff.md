# Comparing `tmp/hi-cli-jash-0.1.1.tar.gz` & `tmp/hi-cli-jash-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hi-cli-jash-0.1.1.tar", last modified: Sat Jun 24 05:03:06 2023, max compression
+gzip compressed data, was "hi-cli-jash-0.1.2.tar", last modified: Sat Jun 24 05:15:06 2023, max compression
```

## Comparing `hi-cli-jash-0.1.1.tar` & `hi-cli-jash-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 05:03:06.417986 hi-cli-jash-0.1.1/
--rw-rw-rw-   0        0        0      172 2023-06-24 05:03:06.417986 hi-cli-jash-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-06-24 04:47:58.000000 hi-cli-jash-0.1.1/hi.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:03:06.415984 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/
--rw-rw-rw-   0        0        0      172 2023-06-24 05:03:06.000000 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-06-24 05:03:06.000000 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 05:03:06.000000 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-24 05:03:06.000000 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        3 2023-06-24 05:03:06.000000 hi-cli-jash-0.1.1/hi_cli_jash.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 05:03:06.419185 hi-cli-jash-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      349 2023-06-24 05:02:33.000000 hi-cli-jash-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:15:06.480093 hi-cli-jash-0.1.2/
+-rw-rw-rw-   0        0        0      172 2023-06-24 05:15:06.478803 hi-cli-jash-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-06-24 05:14:48.000000 hi-cli-jash-0.1.2/hi.py
+drwxrwxrwx   0        0        0        0 2023-06-24 05:15:06.477807 hi-cli-jash-0.1.2/hi_cli_jash.egg-info/
+-rw-rw-rw-   0        0        0      172 2023-06-24 05:15:06.000000 hi-cli-jash-0.1.2/hi_cli_jash.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-06-24 05:15:06.000000 hi-cli-jash-0.1.2/hi_cli_jash.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 05:15:06.000000 hi-cli-jash-0.1.2/hi_cli_jash.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-24 05:15:06.000000 hi-cli-jash-0.1.2/hi_cli_jash.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        3 2023-06-24 05:15:06.000000 hi-cli-jash-0.1.2/hi_cli_jash.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 05:15:06.480093 hi-cli-jash-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      349 2023-06-24 05:15:01.000000 hi-cli-jash-0.1.2/setup.py
```

