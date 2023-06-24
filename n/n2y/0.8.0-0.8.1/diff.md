# Comparing `tmp/n2y-0.8.0.tar.gz` & `tmp/n2y-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n2y-0.8.0.tar", last modified: Sat Jun 24 01:25:06 2023, max compression
+gzip compressed data, was "n2y-0.8.1.tar", last modified: Sat Jun 24 02:18:16 2023, max compression
```

## Comparing `n2y-0.8.0.tar` & `n2y-0.8.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.981220 n2y-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-24 01:25:06.981220 n2y-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28070 2023-06-24 01:24:55.000000 n2y-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.973220 n2y-0.8.0/n2y/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.977220 n2y-0.8.0/n2y/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/data/mermaid_err.png
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/mentions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25357 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/notion_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.977220 n2y-0.8.0/n2y/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/dbfootnotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/deepheaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/expandbluetoggles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/expandlinktopages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/footnotes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/jinjarenderpage.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/linkedheaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/rawcodeblocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/removecallouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/property_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/rich_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.977220 n2y-0.8.0/n2y.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-24 01:25:06.981220 n2y-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-24 01:24:55.000000 n2y-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.981220 n2y-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_append_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_audit_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_expandbluetoggles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_first_pass_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_jinjarenderpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_linkedheaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_plain_text_to_pandoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_plugin_dbfootnotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_property_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_rich_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:18:16.116239 n2y-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-24 02:18:16.116239 n2y-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28126 2023-06-24 02:18:05.000000 n2y-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:18:16.108239 n2y-0.8.1/n2y/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:18:16.112239 n2y-0.8.1/n2y/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/data/mermaid_err.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-24 02:18:05.000000 n2y-0.8.1/n2y/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/mentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25357 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/notion_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:18:16.112239 n2y-0.8.1/n2y/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/plugins/dbfootnotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/plugins/deepheaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/plugins/expandbluetoggles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/plugins/expandlinktopages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/plugins/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/plugins/jinjarenderpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/plugins/linkedheaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/plugins/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/plugins/rawcodeblocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/plugins/removecallouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/property_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/rich_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-06-24 02:18:06.000000 n2y-0.8.1/n2y/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:18:16.112239 n2y-0.8.1/n2y.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-24 02:18:16.000000 n2y-0.8.1/n2y.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-24 02:18:16.000000 n2y-0.8.1/n2y.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 02:18:16.000000 n2y-0.8.1/n2y.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-24 02:18:16.000000 n2y-0.8.1/n2y.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 02:18:16.000000 n2y-0.8.1/n2y.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-24 02:18:16.000000 n2y-0.8.1/n2y.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-24 02:18:16.116239 n2y-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-24 02:18:06.000000 n2y-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 02:18:16.116239 n2y-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_append_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_audit_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_expandbluetoggles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_first_pass_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_jinjarenderpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_linkedheaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_plain_text_to_pandoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_plugin_dbfootnotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_property_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_rich_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-24 02:18:06.000000 n2y-0.8.1/tests/test_utils.py
```

### Comparing `n2y-0.8.0/PKG-INFO` & `n2y-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n2y
-Version: 0.8.0
+Version: 0.8.1
 Summary: Notion to YAML
 Home-page: https://github.com/innolitics/n2y
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: notion documentation yaml markdown
 Classifier: Development Status :: 4 - Beta
```

### Comparing `n2y-0.8.0/README.md` & `n2y-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -386,23 +386,24 @@
 - Make the plugin system more fully featured and easier to use
 - Add support for recursively dumping sets of pages and preserving links between them
 - Add some sort of Notion API caching mechanism
 - Add more examples to the documentation
 
 ## Changelog
 
-### v0.9.0
+### v0.8.1
+
+- Add basic support for undocumented "audio" block type
+
+### v0.8.0
 
 - Replace the `filename_property` configuration option with the more generic `filename_template`.
 - Make it so we can render pages into any pandoc format
 - Include properties as pandoc meta values
 - Add export config option to indicate if we should export YAML front matter
-
-### v0.8.0
-
 - Add requests cache to speed up dev loop
 - Update `jinjarenderpage` so that it no pulls databases mentioned in the
   caption, instead of relying on the exports list. Also, make the
   jinjacodeblocks support any pandoc format.
 - Make it so that we can render property values into any pandoc format
 
 ### v0.7.5
```

### Comparing `n2y-0.8.0/n2y/audit.py` & `n2y-0.8.1/n2y/audit.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/blocks.py` & `n2y-0.8.1/n2y/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -542,31 +542,44 @@
         return None
 
 
 class EmbedBlock(WarningBlock):
     pass
 
 
-class VideoBlock(Block):
+class ContentBlock(Block):
+    """
+    Generic base class for blocks that contain file-based content that should be
+    downloaded and then linked to.
+    """
     def __init__(self, client, notion_data, page, get_children=True):
         super().__init__(client, notion_data, page, get_children)
-        self.file = client.wrap_notion_file(notion_data['video'])
+        self.file = client.wrap_notion_file(self.notion_type_data)
         self.caption = client.wrap_notion_rich_text_array(self.notion_type_data["caption"], self)
 
     def to_pandoc(self):
         url = None
         if self.file.type == "external":
             url = self.file.url
         elif self.file.type == "file":
             url = self.client.download_file(self.file.url, self.page, self.notion_id)
         content_ast = [Link(('', [], []), [Str(url)], (url, ''))]
         if self.caption:
             caption_ast = self.caption.to_pandoc()
             return render_with_caption(content_ast, caption_ast)
-        return Para(content_ast)
+        else:
+            return Para(content_ast)
+
+
+class AudioBlock(ContentBlock):
+    pass
+
+
+class VideoBlock(ContentBlock):
+    pass
 
 
 class PdfBlock(Block):
     def __init__(self, client, notion_data, page, get_children=True):
         super().__init__(client, notion_data, page, get_children)
         self.pdf = client.wrap_notion_file(notion_data['pdf'])
         self.caption = client.wrap_notion_rich_text_array(self.notion_type_data["caption"], self)
@@ -668,14 +681,15 @@
     "numbered_list_item": NumberedListItemBlock,
     "to_do": ToDoListItemBlock,
     "toggle": ToggleBlock,
     "child_page": ChildPageBlock,
     "child_database": ChildDatabaseBlock,
     "embed": EmbedBlock,
     "image": ImageBlock,
+    "audio": AudioBlock,
     "video": VideoBlock,
     "file": FileBlock,
     "pdf": PdfBlock,
     "bookmark": BookmarkBlock,
     "callout": CalloutBlock,
     "quote": QuoteBlock,
     "equation": EquationBlock,
```

### Comparing `n2y-0.8.0/n2y/comment.py` & `n2y-0.8.1/n2y/comment.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/config.py` & `n2y-0.8.1/n2y/config.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/data/mermaid_err.png` & `n2y-0.8.1/n2y/data/mermaid_err.png`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/database.py` & `n2y-0.8.1/n2y/database.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/errors.py` & `n2y-0.8.1/n2y/errors.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/export.py` & `n2y-0.8.1/n2y/export.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/file.py` & `n2y-0.8.1/n2y/file.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/main.py` & `n2y-0.8.1/n2y/main.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/mentions.py` & `n2y-0.8.1/n2y/mentions.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/notion.py` & `n2y-0.8.1/n2y/notion.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/notion_mocks.py` & `n2y-0.8.1/n2y/notion_mocks.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/page.py` & `n2y-0.8.1/n2y/page.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/plugins/dbfootnotes.py` & `n2y-0.8.1/n2y/plugins/dbfootnotes.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/plugins/deepheaders.py` & `n2y-0.8.1/n2y/plugins/deepheaders.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/plugins/expandbluetoggles.py` & `n2y-0.8.1/n2y/plugins/expandbluetoggles.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/plugins/expandlinktopages.py` & `n2y-0.8.1/n2y/plugins/expandlinktopages.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/plugins/footnotes.py` & `n2y-0.8.1/n2y/plugins/footnotes.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/plugins/jinjarenderpage.py` & `n2y-0.8.1/n2y/plugins/jinjarenderpage.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/plugins/linkedheaders.py` & `n2y-0.8.1/n2y/plugins/linkedheaders.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/plugins/mermaid.py` & `n2y-0.8.1/n2y/plugins/mermaid.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/plugins/rawcodeblocks.py` & `n2y-0.8.1/n2y/plugins/rawcodeblocks.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/plugins/removecallouts.py` & `n2y-0.8.1/n2y/plugins/removecallouts.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/properties.py` & `n2y-0.8.1/n2y/properties.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/property_values.py` & `n2y-0.8.1/n2y/property_values.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/rich_text.py` & `n2y-0.8.1/n2y/rich_text.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/user.py` & `n2y-0.8.1/n2y/user.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y/utils.py` & `n2y-0.8.1/n2y/utils.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/n2y.egg-info/PKG-INFO` & `n2y-0.8.1/n2y.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n2y
-Version: 0.8.0
+Version: 0.8.1
 Summary: Notion to YAML
 Home-page: https://github.com/innolitics/n2y
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: notion documentation yaml markdown
 Classifier: Development Status :: 4 - Beta
```

### Comparing `n2y-0.8.0/n2y.egg-info/SOURCES.txt` & `n2y-0.8.1/n2y.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/setup.py` & `n2y-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 description = 'Notion to YAML'
 
 setup(
     name='n2y',
-    version='0.8.0',
+    version='0.8.1',
     description=description,
     long_description=description,
     long_description_content_type='text/x-rst',
     url='https://github.com/innolitics/n2y',
     author='Innolitics, LLC',
     author_email='info@innolitics.com',
     license='MIT',
```

### Comparing `n2y-0.8.0/tests/test_append_end_to_end.py` & `n2y-0.8.1/tests/test_append_end_to_end.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_audit_end_to_end.py` & `n2y-0.8.1/tests/test_audit_end_to_end.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_blocks.py` & `n2y-0.8.1/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_config.py` & `n2y-0.8.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_end_to_end.py` & `n2y-0.8.1/tests/test_end_to_end.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,14 +244,16 @@
     assert "Mention: Simple Test Database" in lines
     assert "Simple Test Database" in lines  # from the LinkToPageBlock
 
     # a bookmark with a caption and without
     assert "<https://innolitics.com>" in lines
     assert "[Bookmark caption](https://innolitics.com)" in lines
 
+    # TODO: Add assertions about audio blocks and video blocks
+
     # the word "caption" is bolded
     assert "![Image **caption**](media/All_Blocks_Test_Page-5f1b0813453.jpeg)" in lines
 
     # from a file block in the Notion page
     assert os.path.exists(tmpdir / "media" / "All_Blocks_Test_Page-5f1b0813453.jpeg")
```

### Comparing `n2y-0.8.0/tests/test_expandbluetoggles.py` & `n2y-0.8.1/tests/test_expandbluetoggles.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_export.py` & `n2y-0.8.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_first_pass_output.py` & `n2y-0.8.1/tests/test_first_pass_output.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_jinjarenderpage.py` & `n2y-0.8.1/tests/test_jinjarenderpage.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_linkedheaders.py` & `n2y-0.8.1/tests/test_linkedheaders.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_plain_text_to_pandoc.py` & `n2y-0.8.1/tests/test_plain_text_to_pandoc.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_plugin_dbfootnotes.py` & `n2y-0.8.1/tests/test_plugin_dbfootnotes.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_plugins.py` & `n2y-0.8.1/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_property_values.py` & `n2y-0.8.1/tests/test_property_values.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_rich_text.py` & `n2y-0.8.1/tests/test_rich_text.py`

 * *Files identical despite different names*

### Comparing `n2y-0.8.0/tests/test_utils.py` & `n2y-0.8.1/tests/test_utils.py`

 * *Files identical despite different names*

