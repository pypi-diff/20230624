# Comparing `tmp/wpdetect-1.3.6.tar.gz` & `tmp/wpdetect-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wpdetect-1.3.6.tar", last modified: Fri Jun 26 18:43:16 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `wpdetect-1.3.6.tar` & `wpdetect-1.3.7.tar`

### file list

```diff
@@ -1,8 +1,7 @@
-drwxrwxrwx   0        0        0        0 2020-06-26 18:43:16.774899 wpdetect-1.3.6/
--rw-rw-rw-   0        0        0     2489 2020-06-26 18:43:16.776893 wpdetect-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2020-06-26 12:24:36.649398 wpdetect-1.3.6/README.rst
--rw-rw-rw-   0        0        0       41 2020-06-25 19:24:01.058081 wpdetect-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1405 2020-06-26 18:40:16.337816 wpdetect-1.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2020-06-26 18:43:16.773900 wpdetect-1.3.6/wpdetect/
--rw-rw-rw-   0        0        0        0 2020-06-26 18:24:02.225513 wpdetect-1.3.6/wpdetect/__init__.py
--rw-rw-rw-   0        0        0     6821 2020-06-26 18:26:26.534961 wpdetect-1.3.6/wpdetect/__main__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wpdetect-1.3.7/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wpdetect-1.3.7/wpdetect/__init__.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 wpdetect-1.3.7/wpdetect/__main__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wpdetect-1.3.7/LICENSE.txt
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 wpdetect-1.3.7/README.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 wpdetect-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 wpdetect-1.3.7/PKG-INFO
```

