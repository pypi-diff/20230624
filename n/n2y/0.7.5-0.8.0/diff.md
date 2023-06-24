# Comparing `tmp/n2y-0.7.5.tar.gz` & `tmp/n2y-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n2y-0.7.5.tar", last modified: Sat Jan 21 18:49:31 2023, max compression
+gzip compressed data, was "n2y-0.8.0.tar", last modified: Sat Jun 24 01:25:06 2023, max compression
```

## Comparing `n2y-0.7.5.tar` & `n2y-0.8.0.tar`

### file list

```diff
@@ -1,45 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 18:49:31.442188 n2y-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-01-21 18:49:31.442188 n2y-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23024 2023-01-21 18:49:22.000000 n2y-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 18:49:31.438188 n2y-0.7.5/n2y/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 18:49:31.442188 n2y-0.7.5/n2y/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/data/mermaid_err.png
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/mentions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/notion_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 18:49:31.442188 n2y-0.7.5/n2y/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/plugins/deepheaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/plugins/expandlinktopages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/plugins/footnotes.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/plugins/linkedheaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/plugins/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/plugins/rawcodeblocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/plugins/removecallouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/plugins/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/property_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/rich_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-01-21 18:49:22.000000 n2y-0.7.5/n2y/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 18:49:31.442188 n2y-0.7.5/n2y.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-01-21 18:49:31.000000 n2y-0.7.5/n2y.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-01-21 18:49:31.000000 n2y-0.7.5/n2y.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-21 18:49:31.000000 n2y-0.7.5/n2y.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-21 18:49:31.000000 n2y-0.7.5/n2y.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-21 18:49:31.000000 n2y-0.7.5/n2y.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-01-21 18:49:31.000000 n2y-0.7.5/n2y.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-21 18:49:31.442188 n2y-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-01-21 18:49:22.000000 n2y-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.981220 n2y-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-24 01:25:06.981220 n2y-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28070 2023-06-24 01:24:55.000000 n2y-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.973220 n2y-0.8.0/n2y/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.977220 n2y-0.8.0/n2y/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/data/mermaid_err.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/mentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25357 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/notion_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.977220 n2y-0.8.0/n2y/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/dbfootnotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/deepheaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/expandbluetoggles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/expandlinktopages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/jinjarenderpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/linkedheaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/rawcodeblocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/plugins/removecallouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/property_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/rich_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-06-24 01:24:55.000000 n2y-0.8.0/n2y/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.977220 n2y-0.8.0/n2y.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-24 01:25:06.000000 n2y-0.8.0/n2y.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-24 01:25:06.981220 n2y-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-24 01:24:55.000000 n2y-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 01:25:06.981220 n2y-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_append_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_audit_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_expandbluetoggles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_first_pass_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_jinjarenderpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_linkedheaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_plain_text_to_pandoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_plugin_dbfootnotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_property_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_rich_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-24 01:24:55.000000 n2y-0.8.0/tests/test_utils.py
```

### Comparing `n2y-0.7.5/PKG-INFO` & `n2y-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n2y
-Version: 0.7.5
+Version: 0.8.0
 Summary: Notion to YAML
 Home-page: https://github.com/innolitics/n2y
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: notion documentation yaml markdown
 Classifier: Development Status :: 4 - Beta
```

### Comparing `n2y-0.7.5/README.md` & `n2y-0.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,24 +4,22 @@
 
 This commandline tool exports data from selected Notion pages and databases into YAML and markdown files. Internally, it converts the Notion pages into a [Pandoc](https://pandoc.org) AST, which enables fine-grained customization of the conversion process.
 
 We use it at [Innolitics](https://innolitics.com) to generate pages for our website, thus allowing us to use Notion as a content management system. We also use it to generate PDFs and Word Documents from Notion pages.
 
 ## Installation
 
-To install the tool, just run:
+Install first `pandoc` and `mermaid` CLIs. Please note that `n2y` has only been tested with `pandoc 2.19.2` and `mermaid-cli 9.4.0`. This [pandoc](https://github.com/jgm/pandoc/releases/tag/2.19.2) link will take you to their `2.19.2` github releases page. This [mermaid](https://github.com/mermaid-js/mermaid-cli) link will take you to their github page where you will find installation instructions. If using `npm` to install `mermaid`, append `@9.4.0` to the `npm` command to install that specific version.
+
+Finally, install `n2y`:
 
 ```
 pip install n2y
 ```
 
-You'll also need to install [pandoc](https://github.com/jgm/pandoc/releases/). We've tested against version 2.16.2, but any newer versions should work too.
-
-Note: n2y has only been tested with `pandoc 2.18` and `mermaid-cli 8.11`.
-
 ## Authorization
 
 Before you'll be able to export any content from your Notion account you'll first need to give n2y permission to access the pages. You'll need to be an admin.
 
 To do this, go to the "Settings and Members" page in Notion. You should see an "Integrations" option in the side bar. Click the link that says "Develop your own integrations" and follow the instructions on the page. Copy the "Internal Integration Token" into the `NOTION_ACCESS_TOKEN` environment variable.
 
 Finally, in Notion you'll need to share the relevant pages with your internal integration---just like you'd share a page with another person.
@@ -43,17 +41,18 @@
 | --- | --- |
 | id | The notion database or page id, taken from the "share URL". |
 | node_type | Either "database_as_yaml", "database_as_files", or "page". |
 | output | The path the output file, or directory, where the data will be written. |
 | pandoc_format | The [pandoc format](https://pandoc.org/MANUAL.html#general-options) that we're generating. |
 | pandoc_options | A list of strings that are [writer options](https://pandoc.org/MANUAL.html#general-writer-options) for pandoc. |
 | content_property | When set, it indicates the property name that will contain the content of the notion pages in that databse. If set to `None`, then only the page's properties will be included in the export. (Only applies to the `database_as_files` node type.) |
+| yaml_front_matter | Only used when exporting to text files. Indicates if the page properties should be exported as yaml front matter. |
 | id_property | When set, this indicates the property name in which to place the page's underlying notion ID. |
 | url_property | When set, this indicates the property name in which to place the page's underlying notion url. |
-| filename_property | This key is required for the "database_as_files" node type; when set, it indicates which property to use when generating the file name. |
+| filename_template | This key is only used for the "database_as_files" node type; when set, it provides a [format string](https://docs.python.org/3/library/string.html#formatstrings) that is evaluated against the page's properties to generate the file name. Note that the filenames are sanitized. When not set, the title property is used and the extension is deduced from the `pandoc_format`. A special "TITLE" property may be used to access the title property in the template string. |
 | plugins | A list of python modules to use as plugins. |
 | notion_filter | A [notion filter object](https://developers.notion.com/reference/post-database-query-filter) to be applied to the database. |
 | notion_sorts | A [notion sorts object](https://developers.notion.com/reference/post-database-query-sort) to be applied to the database. |
 | property_map | A mapping between the name of properties in Notion, and the name of the properties in the exported files. |
 
 ## Example Configuration Files
 
@@ -75,18 +74,18 @@
 The same database could be exported into a set of markdown files as follows:
 
 ```
 exports:
 - id: 176fa24d4b7f4256877e60a1035b45a4
   node_type: database_as_files
   output: directory
-  filename_property: "Name"
+  filename_template: "{Name}.md"
 ```
 
-Each page in the database will generate a single markdown file, named according to the `filename_property`. This process will automatically skip pages whose "Name" property is empty.
+Each page in the database will generate a single markdown file, named according to the `filename_template`. This process will automatically skip pages whose "Name" property is empty.
 
 ### Convert a Page to a Markdown File
 
 An individual notion page (e.g., with a share URL like this https://www.notion.so/All-Blocks-Test-Page-5f18c7d7eda44986ae7d938a12817cc0) could be exported to markdown with this minimal configuration file:
 
 ```
 exports:
@@ -119,30 +118,30 @@
     - "n2y.plugins.expandlinktopages"
   content_property: null
   id_property: id
   url_property: url
 exports:
   - output: "documents/dhf"
     node_type: "database_as_files"
-    filename_property: "Name"
+    filename_template: "{Name}.md"
     id: e24f839e724848d69342d43c07cb5f3e
     plugins:
       - "n2y.plugins.mermaid"
       - "n2y.plugins.rawcodeblocks"
       - "n2y.plugins.removecallouts"
       - "n2y.plugins.deepheaders"
       - "n2y.plugins.expandlinktopages"
       - "plugins.page"
       - "plugins.idmentions"
     notion_filter:
       property: "Tags"
       multi_select: { "contains": "DHF" }
   - output: "documents/510k"
     id: e24f839e724848d69342d43c07cb5f3e
-    filename_property: "Name"
+    filename_template: "{Name}.md"
     node_type: "database_as_files"
     plugins:
       - "n2y.plugins.mermaid"
       - "n2y.plugins.rawcodeblocks"
       - "n2y.plugins.removecallouts"
       - "n2y.plugins.deepheaders"
       - "n2y.plugins.expandlinktopages"
@@ -237,31 +236,59 @@
 | ToggleBlock | Convert the toggles into a bulleted list. |
 | VideoBlock | Acts the same way as the Image block |
 
 Most of the Notion blocks can generate their pandoc AST from _only_ their own data. The one exception is the list item blocks; pandoc, unlike Notion, has an encompassing node in the AST for the entire list. The `ListItemBlock.list_to_pandoc` class method is responsible for generating this top-level node.
 
 ## Built-in Plugins
 
-N2y provides a few builtin plugins. These plugins are all turned off by default. Brief descriptions are provided below, but see [the code](https://github.com/innolitics/n2y/tree/rich-text-extensions/n2y/plugins) for details.
+N2y provides a few builtin plugins. These plugins are all turned off by default. Brief descriptions are provided below, but see [the code](https://github.com/innolitics/n2y/tree/main/n2y/plugins) for details.
+
+### Jinja Render Page
+
+CodeBlocks whose caption begins with "{jinja=pandocformat}" will be rendered using [Jinja](https://jinja.palletsprojects.com/en/3.1.x/templates/) into text and then read into the AST using the specified pandoc input format. Note that, other than the special "plain" format, the pandocformat must be available both for reading and writing.
+
+Any databases that are [mentioned](https://www.notion.so/help/comments-mentions-and-reminders) in the codeblock's caption will be made available in the jinja render context within the `databases` dictionary.
+
+Take the following code block for example:
+
+```
+<table>
+  <tr><th>Name</th><th>Email</th></tr>
+  {% for person in databases["People"] %}
+  <tr><td>{{person.Name}}</td><td>{{person.Email}}</td></tr>
+  {% endfor %}
+</table>
+```
+
+The caption would be, "{jinja=html} @People," where "Name" and "Email" are properties in the "People" database.
+
+Note that any rich text properties are rendered into the pandoc input format specified.
 
-### Render
+The codeblock's parent page's properties are made available in the `page` context variable.
 
-When CodeBlocks are captioned "{template}", the block is rendered as jinja using yaml data previously cached by n2y
+The jinja context has a few special filters available to it:
+
+| Name | Type | Description |
+| --- | --- | --- |
+| `join_to` | filter | Make it possible to join notion databases together. |
+| `first_pass_output` | object | Makes it possible to access the full text of the initial page's render. Useful if you want to render a glossary of terms that are used on the page. |
+
+See the [code](https://github.com/innolitics/n2y/blob/main/n2y/plugins/jinjarenderpage.py) for details.
 
 ### Deep Headers
 
 Notion only support three levels of headers, but sometimes this is not enough. This plugin enables support for h4 and h5 headers in the documents exported from Notion. Any Notion h3 whose text begins with the characters "= " is converted to an h4, and any h3 that begins with "== " is converted to an h5, and so on.
 
 ### Remove Callouts
 
 Completely remove all callout blocks. It's often helpful to include help text in callout blocks, but usually this help text should be stripped out of the final generated documents.
 
 ### Raw Fenced Code Blocks
 
-Any code block whose caption begins with "{=language}" will be made into a raw block for pandoc to parse. This is useful if you need to drop into Raw HTML or other formats. See [the pandoc documentation](https://pandoc.org/MANUAL.html#generic-raw-attribute) for more details on the raw code blocks.
+Any code block whose caption begins with "{=pandocformat}" will be made into a raw block for pandoc to parse. This is useful if you need to drop into Raw HTML or other output formats that pandoc supports. See [the pandoc documentation](https://pandoc.org/MANUAL.html#generic-raw-attribute) for more details on the raw code blocks.
 
 ### Mermaid Fenced Code Blocks
 
 Adds support for generating mermaid diagrams from codeblocks with the "mermaid" language, as supported in the Notion UI.
 
 This plugin assumes that the `mmdc` mermaid commandline tool is available, and will throw an exception if it is not.
 
@@ -271,20 +298,27 @@
 
 Replace headers with links back to the originating notion block.
 
 ### Footnotes
 
 Adds support for Pandoc-style footnotes. Any `text` rich texts that contain footnote references in the format `[^NUMBER]` (eg: `...some claim [^2].`) will be linked to the corresponding footnote paragraph block starting with `[NUMBER]:` (eg: `[2]: This is a footnote.`).
 
+### DB Footnotes
+Adds general footnote support (not specialized for markdown) with the expectation that all footnote content is placed in an inline database on the original page wherein footnote references are made. Specific footnote references are made with Notion's page mention feature, mentioning a specific footnote page in the database. For example, each page in the database can simply be titled with a footnote number and contain the footnote text as the page content. The inline database must have a title that ends with "Footnotes."
+
 ### Expand Link To Page Blocks
 
 When this plugin is enabled, any "link to page" block (which can be created using the `/link` command in the Notion UI), will be replaced with the content of the page that is linked to. This makes it possible to use the "link to page" block to include repeated content in multiple locations. It is like a "synced content block" in this way, but unlike "synced content blocks" which don't play well when duplicating child pages, the "link to page" blocks can be duplicated more easily.
 
 Note that any link to a page that the integration doesn't have access to will be skipped entirely (Notion returns an "Unsupported Block" in this case).
 
+### Hidden Jinja Toggles
+
+When this plugin is enabled, any "blue" colored toggle block will have it's children directly rendered. The text on the toggle itself will be ignored.
+
 ## Architecture
 
 An n2y run is divided into four stages:
 
 1. Loading the configuration (mostly in `config.py`)
 2. Retrieve data from Notion (by instantiating various Notion object instances, e.g., `Page`, `Block`, `RichText`, etc.)
 3. Convert to the pandoc AST (by calling `block.to_pandoc()`)
@@ -294,14 +328,18 @@
 
 Every block has a `page` property which refers to the page that contains it.
 
 Every rich text object and mention has a `block` property that is either refers
 back to the block that contains it, or is None if the rich text is within a
 property value or some other location.
 
+## Cache
+
+During development, it can be convenient to cache requests to Notion. This feature can be enabled by setting the `N2Y_CACHE` environment variable to the location of the sqlite file you'd like to use as your Notion request cache. To flush the cache, simply delete the file. Note that this feature is only available if you include dev options.
+
 ## Releases
 
 Any git commit tagged with a string starting with "v" will automatically be pushed to pypi.
 
 Be sure to update the [setup.py](https://github.com/innolitics/n2y/blob/main/setup.py#L14) version number first.
 
 You can create the tag using, e.g., `git tag v0.3.4` and you can push it using `git push && git push --tags`.
@@ -319,29 +357,62 @@
 You can then run the tests and the linter as follows:
 
 ```
 flake8 .
 pytest tests
 ```
 
+## Developer Tools
+
+### Pandoc
+
+`n2y` is built on top of [`pandoc`](https://pandoc.org/MANUAL.html), using it to build intermediate representations and for output generation. Being familiar with the pandoc AST is important as an `n2y` developer. Documentation is available for the [native Haskell AST](https://hackage.haskell.org/package/pandoc-types-1.23) and for the corresponding [Python wrapper library](https://boisgera.github.io/pandoc/document/) used directly by `n2y`.
+
+As part of a typical development cycle, you can use the `pandoc` CLI to inspect the relationship between, for example, GitHub-flavored Markdown and the native `pandoc` AST. The following CLI invocation of `pandoc` takes in the GitHub-flavored Markdown file "example.md", converts it to the `pandoc` AST in JSON format, and pipes this output to the command line `jq` JSON processor program for viewing in the terminal:
+
+```
+pandoc -f gfm -t json example.md | jq .
+```
+
+The following command performs a full round-trip from GitHub-flavored Markdown to the `pandoc` AST and back to GitHub-flavored Markdown:
+
+```
+pandoc -f gfm -t json example.md | pandoc -f json -t gfm
+```
+
 ## Roadmap
 
 Here are some features we're planning to add in the future:
 
 - Make the plugin system more fully featured and easier to use
 - Add support for recursively dumping sets of pages and preserving links between them
 - Add some sort of Notion API caching mechanism
 - Add more examples to the documentation
 
 ## Changelog
 
+### v0.9.0
+
+- Replace the `filename_property` configuration option with the more generic `filename_template`.
+- Make it so we can render pages into any pandoc format
+- Include properties as pandoc meta values
+- Add export config option to indicate if we should export YAML front matter
+
+### v0.8.0
+
+- Add requests cache to speed up dev loop
+- Update `jinjarenderpage` so that it no pulls databases mentioned in the
+  caption, instead of relying on the exports list. Also, make the
+  jinjacodeblocks support any pandoc format.
+- Make it so that we can render property values into any pandoc format
+
 ### v0.7.5
 
 - Flatten Column List Blocks
-- Add render plugin to render jinja in code blocks
+- Add `jinjarenderpage` plugin to render jinja in code blocks
 
 ### v0.7.4
 
 - Add features that allow the notion Client to retry api calls after being rate limited.
 
 ### v0.7.3
```

### Comparing `n2y-0.7.5/n2y/audit.py` & `n2y-0.8.0/n2y/audit.py`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y/blocks.py` & `n2y-0.8.0/n2y/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
 from itertools import groupby
 from urllib.parse import urljoin
 
 from pandoc.types import (
-    Period, Meta, Pandoc, Link, HorizontalRule, BlockQuote, Image, MetaString,
-    Table, TableHead, TableBody, TableFoot, RowHeadColumns, Row, Cell, RowSpan,
-    Str, Para, Plain, Header, CodeBlock, BulletList, OrderedList, Decimal, Space,
-    ColSpan, ColWidthDefault, AlignDefault, Caption, Math, DisplayMath, LineBreak
+    Period, Pandoc, Link, HorizontalRule, BlockQuote, Image, Table, TableHead,
+    TableBody, TableFoot, RowHeadColumns, Row, Cell, RowSpan, Str, Para, Plain,
+    Header, CodeBlock, BulletList, OrderedList, Decimal, Space, ColSpan,
+    ColWidthDefault, AlignDefault, Caption, Math, DisplayMath, LineBreak
 )
 
+from n2y.utils import yaml_map_to_meta, header_id_from_text
+
 
 logger = logging.getLogger(__name__)
 
 
 class Block:
     """
     A Notion page's content consists of a tree of nested Blocks.
@@ -66,15 +68,17 @@
         pandoc_ast = []
         for block_type, blocks in groupby(self.children, lambda c: type(c)):
             if issubclass(block_type, ListItemBlock):
                 pandoc_ast.append(block_type.list_to_pandoc(blocks))
             else:
                 for b in blocks:
                     result = b.to_pandoc()
-                    if isinstance(result, list):
+                    if block_type == ChildPageBlock:
+                        pandoc_ast.extend(result[1])
+                    elif isinstance(result, list):
                         # a few blocks return lists of nodes
                         pandoc_ast.extend(result)
                     elif result is not None:
                         # a plugin may decide to return None to indicate the
                         # block should be removed; ideally pandoc.types.Nil
                         # would handle this, but it doesn't appear to work
                         pandoc_ast.append(result)
@@ -105,15 +109,22 @@
         super().__init__(client, notion_data, page, get_children)
         self.title = self.notion_type_data["title"]
 
     def to_pandoc(self):
         assert self.children is not None
         if self.children:
             children = self.children_to_pandoc()
-            return Pandoc(Meta({'title': MetaString(self.title)}), children)
+            if self.page:
+                properties = self.page.properties_to_values()
+            else:
+                properties = {}
+            if 'title' not in properties:
+                properties['title'] = self.title
+            meta = yaml_map_to_meta(properties)
+            return Pandoc(meta, children)
         else:
             return None
 
 
 class EquationBlock(Block):
     def __init__(self, client, notion_data, page, get_children=True):
         super().__init__(client, notion_data, page, get_children)
@@ -152,28 +163,33 @@
             self.notion_type_data["rich_text"], self
         )
 
     def to_pandoc(self):
         content = [Plain(self.rich_text.to_pandoc())]
         if self.has_children:
             children = self.children_to_pandoc()
-            content.extend(children)
+            for child in children:
+                if isinstance(child, Table):
+                    # A bug in pandoc's markdown reader makes it unable to register mid-list tables.
+                    # This adds an extra space between the table and the previous list item, which
+                    # Allows the table to be read as such.
+                    content.append(Para([]))
+                content.append(child)
         return content
 
     @classmethod
     def list_to_pandoc(klass, items):
         return BulletList([b.to_pandoc() for b in items])
 
 
 class ToDoListItemBlock(BulletedListItemBlock):
     def __init__(self, client, notion_data, page, get_children=True):
         super().__init__(client, notion_data, page, get_children)
         self.checked = self.notion_type_data['checked']
 
-        # TODO: Move this into the "to_pandoc" stage
         box = '☒ ' if self.checked else '☐ '
         self.rich_text.prepend(box)
 
 
 class NumberedListItemBlock(ListItemBlock):
     def __init__(self, client, notion_data, page, get_children=True):
         super().__init__(client, notion_data, page, get_children)
@@ -181,15 +197,19 @@
             self.notion_type_data["rich_text"], self
         )
 
     def to_pandoc(self):
         content = [Plain(self.rich_text.to_pandoc())]
         if self.has_children:
             children = self.children_to_pandoc()
-            content.extend(children)
+            for child in children:
+                if isinstance(child, Table):
+                    # See comment in BulletedListItemBlock.to_pandoc()
+                    content.append(Para([]))
+                content.append(child)
         return content
 
     @classmethod
     def list_to_pandoc(klass, items):
         return OrderedList((1, Decimal(), Period()), [b.to_pandoc() for b in items])
 
 
@@ -203,15 +223,16 @@
         # The Notion UI allows one to bold the text in a header, but the bold
         # styling isn't displayed. Thus, to avoid unexpected appearances of
         # bold text in the generated documents, bolding is removed.
         for rich_text in self.rich_text:
             rich_text.bold = False
 
     def to_pandoc(self):
-        return Header(self.level, ('', [], []), self.rich_text.to_pandoc())
+        section_id = header_id_from_text(self.rich_text.to_plain_text())
+        return Header(self.level, (section_id, [], []), self.rich_text.to_pandoc())
 
 
 class HeadingOneBlock(HeadingBlock):
     level = 1
 
 
 class HeadingTwoBlock(HeadingBlock):
@@ -344,18 +365,18 @@
 
     def to_pandoc(self):
         url = None
         if self.file.type == "external":
             url = self.file.url
         elif self.file.type == "file":
             url = self.client.download_file(self.file.url, self.page, self.notion_id)
-        img_alt = [Str(url)]
+        caption = []
         if self.caption:
-            img_alt = self.caption.to_pandoc()
-        return Para([Image(('', [], []), img_alt, (url, ''))])
+            caption = self.caption.to_pandoc()
+        return Para([Image(('', [], []), caption, (url, ''))])
 
 
 class TableBlock(Block):
     def __init__(self, client, notion_data, page, get_children=True):
         super().__init__(client, notion_data, page, get_children)
         self.has_column_header = self.notion_type_data['has_column_header']
         self.has_row_header = self.notion_type_data['has_row_header']
@@ -612,15 +633,15 @@
             node = self.client.get_page(self.linked_node_id)
         elif self.link_type == "database_id":
             node = self.client.get_database(self.linked_node_id)
         else:
             raise NotImplementedError(f"Unknown link type: {self.link_type}")
 
         if node is None:
-            msg = "Permission denied when attempting to access linked node [%s]"
+            msg = "Permission denied when attempting to access linked node (%r)"
             logger.warning(msg, self.notion_url)
             return None
         else:
             title = node.title.to_pandoc()
             return Para(title)
```

### Comparing `n2y-0.7.5/n2y/comment.py` & `n2y-0.8.0/n2y/comment.py`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y/data/mermaid_err.png` & `n2y-0.8.0/n2y/data/mermaid_err.png`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y/database.py` & `n2y-0.8.0/n2y/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,30 +38,30 @@
 
     @property
     def children(self):
         if self._children is None:
             self._children = self.client.get_database_pages(self.notion_id)
         return self._children
 
-    def get_children(self):
-        self._children = self.client.get_database_pages(self.notion_id)
-
     def children_filtered(self, filter, sort=None):
-        loading_from_cache = filter is not None
-        if loading_from_cache:
+        if filter is not None:
             tupled_filter = self._tuplize(filter)
             tupled_sort = self._tuplize(sort)
             if tupled_filter not in self._filtered_children:
                 self._filtered_children[tupled_filter] = {}
             if tupled_sort not in self._filtered_children[tupled_filter]:
                 self._filtered_children[tupled_filter][tupled_sort] = \
                     self.client.get_database_pages(self.notion_id, filter, sort)
-            return self._filtered_children[tupled_filter][tupled_sort]
+            children = self._filtered_children[tupled_filter][tupled_sort]
         else:
-            return self.children
+            children = self.children
+        for i, child in enumerate(children):
+            if not self.client.page_class_is_in_use(child):
+                children[i] = self.client._wrap_notion_page(child.notion_data)
+        return children
 
     def _tuplize(self, item):
         if callable(getattr(item, "items", None)):
             return tuple([(key, self._tuplize(val)) for (key, val) in item.items()])
         elif hasattr(item, '__iter__') and type(item) is not str:
             return tuple([self._tuplize(i) for i in item])
         else:
```

### Comparing `n2y-0.7.5/n2y/errors.py` & `n2y-0.8.0/n2y/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class PluginError(N2YError):
     """
     Raised due to various errors loading a plugin.
     """
     pass
 
 
-class UseNextClass(Exception):
+class UseNextClass(N2YError):
     """
     Used by plugin classes to indicate that the next class should be used instead of them.
     """
     pass
 
 
 class RequestTimeoutError(N2YError):
@@ -54,14 +54,29 @@
             )
         super().__init__(message)
         self.status = response.status_code
         self.headers = response.headers
         self.body = response.text
 
 
+class APIResponseError(HTTPResponseError):
+    """An error raised by Notion API."""
+
+    def __init__(self, response, message, code) -> None:
+        super().__init__(response, f"{message} [{code}]")
+        self.code = code
+
+
+class ObjectNotFound(APIResponseError):
+    def __init__(self, response, message) -> None:
+        code = APIErrorCode.ObjectNotFound
+        super().__init__(response, f"{message} [{code}]", code)
+        self.code = code
+
+
 class APIErrorCode(str, Enum):
     Unauthorized = "unauthorized"
     """The bearer token is not valid."""
 
     RestrictedResource = "restricted_resource"
     """Given the bearer token used, the client doesn't have permission to
     perform this operation."""
@@ -94,28 +109,22 @@
     """An unexpected error occurred. Reach out to Notion support."""
 
     ServiceUnavailable = "service_unavailable"
     """Notion is unavailable. Try again later.
     This can occur when the time to respond to a request takes longer than 60 seconds,
     the maximum request timeout."""
 
+    GatewayTimeoutError = "gateway_timeout"
+    """Notion timed out while attempting to complete this request. Please try again later."""
 
-class APIResponseError(HTTPResponseError):
-    """An error raised by Notion API."""
-
-    def __init__(self, response, message, code) -> None:
-        super().__init__(response, f"{message} [{code}]")
-        self.code = code
+    MissingVersion = "missing_version"
+    """The request is missing the required Notion-Version header"""
 
-
-class ObjectNotFound(APIResponseError):
-    def __init__(self, response, message) -> None:
-        code = APIErrorCode.ObjectNotFound
-        super().__init__(response, f"{message} [{code}]", code)
-        self.code = code
+    DatabaseConnectionUnavailable = "database_connection_unavailable"
+    """Notion's database is unavailable or in an unqueryable state. Try again later."""
 
 
 def is_api_error_code(code: str) -> bool:
     """Check if given code belongs to the list of valid API error codes."""
     if isinstance(code, str):
         return code in (error_code.value for error_code in APIErrorCode)
     return False
```

### Comparing `n2y-0.7.5/n2y/export.py` & `n2y-0.8.0/n2y/export.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 """
 This module contains all the code responsible for exporting `page.Page` and
 `database.Database` objects into the various supported file formats.
 """
 import os
 import logging
 
+from pandoc.types import Table
 import yaml
 
-from n2y.utils import pandoc_write_or_log_errors, sanitize_filename
+from n2y.utils import (
+    pandoc_format_to_file_extension,
+    pandoc_write_or_log_errors,
+    sanitize_filename,
+)
 
 logger = logging.getLogger(__name__)
 
 
-def _page_properties(page, id_property=None, url_property=None, property_map=None):
+def _page_properties(
+    page,
+    pandoc_format=None,
+    id_property=None,
+    url_property=None,
+    property_map=None,
+):
+    if pandoc_format is None:
+        pandoc_format = "markdown"
     if property_map is None:
         property_map = {}
-    properties = page.properties_to_values()
+    properties = page.properties_to_values(pandoc_format)
     if id_property in properties:
         logger.warning(
             'The id property "%s" is shadowing an existing '
-            'property with the same name', id_property,
+            "property with the same name",
+            id_property,
         )
     if id_property:
         properties[id_property] = page.notion_id
 
     if url_property in properties:
         logger.warning(
             'The url property "%s" is shadowing an existing '
-            'property with the same name', url_property,
+            "property with the same name",
+            url_property,
         )
     if url_property:
         properties[url_property] = page.notion_url
     for original, new in property_map.items():
         if original in properties:
             properties[new] = properties.pop(original)
         else:
@@ -40,26 +55,65 @@
     return properties
 
 
 def export_page(
     page,
     pandoc_format,
     pandoc_options,
+    yaml_front_matter=True,
     id_property=None,
     url_property=None,
     property_map=None,
 ):
-    page_properties = _page_properties(page, id_property, url_property, property_map)
     pandoc_ast = page.to_pandoc()
+
+    if (number_empty_headers := _count_headerless_tables(pandoc_ast)) > 0:
+        if "markdown" in pandoc_format or "gfm" in pandoc_format:
+            logger.warning(
+                "%d table(s) will present empty headers to maintain Markdown spec (%r)",
+                number_empty_headers,
+                page.notion_url,
+            )
+
     page_content = pandoc_write_or_log_errors(pandoc_ast, pandoc_format, pandoc_options)
-    return '\n'.join([
-        '---',
-        yaml.dump(page_properties) + '---',
-        page_content,
-    ])
+    if isinstance(page_content, str) and yaml_front_matter:
+        page_properties = _page_properties(
+            page,
+            pandoc_format,
+            id_property,
+            url_property,
+            property_map,
+        )
+        return "\n".join(
+            [
+                "---",
+                yaml.dump(page_properties) + "---",
+                page_content,
+            ]
+        )
+    else:
+        # if the result is a binary file, return it as is (since we can't add YAML metadata to it)
+        return page_content
+
+
+def _count_headerless_tables(pandoc_ast):
+    """
+    Count the number of tables in the AST that will result in empty
+    header rows prepended by Pandoc.
+    """
+    number_empty_headers = 0
+    if pandoc_ast and any(isinstance(e, Table) for e in pandoc_ast[1]):
+        for element in pandoc_ast[1]:
+            if isinstance(element, Table):
+                _, head = element[3]
+                # We do count empty rows
+                number_header_rows = sum(1 for _, row in head)
+                if number_header_rows == 0:
+                    number_empty_headers += 1
+    return number_empty_headers
 
 
 def database_to_yaml(
     database,
     pandoc_format,
     pandoc_options,
     notion_filter=None,
@@ -68,76 +122,100 @@
     url_property=None,
     content_property=None,
     property_map=None,
 ):
     if content_property in database.schema:
         logger.warning(
             'The content property "%s" is shadowing an existing '
-            'property with the same name', content_property,
+            "property with the same name",
+            content_property,
         )
     results = []
     for page in database.children_filtered(notion_filter, notion_sorts):
-        result = _page_properties(page, id_property, url_property, property_map)
+        result = _page_properties(
+            page, pandoc_format, id_property, url_property, property_map
+        )
         if content_property:
             pandoc_ast = page.to_pandoc()
             if pandoc_ast:
                 result[content_property] = pandoc_write_or_log_errors(
-                    pandoc_ast, pandoc_format, pandoc_options,
+                    pandoc_ast,
+                    pandoc_format,
+                    pandoc_options,
                 )
             else:
                 result[content_property] = None
         results.append(result)
-    return yaml.dump(results, sort_keys=False)
+    return results
 
 
-def database_to_markdown_files(
+def database_to_files(
     database,
     directory,
     pandoc_format,
     pandoc_options,
-    filename_property=None,
+    yaml_front_matter=True,
+    filename_template=None,
     notion_filter=None,
     notion_sorts=None,
     id_property=None,
     url_property=None,
     property_map=None,
 ):
-    os.makedirs(directory, exist_ok=True)
     seen_file_names = set()
-    counts = {'unnamed': 0, 'duplicate': 0}
+    counts = {"unnamed": 0, "duplicate": 0}
     for page in database.children_filtered(notion_filter, notion_sorts):
-        page_filename = _page_filename(page, filename_property)
+        page_filename = _page_filename(page, pandoc_format, filename_template)
         if page_filename:
             if page_filename not in seen_file_names:
                 seen_file_names.add(page_filename)
-                with open(os.path.join(directory, f"{page_filename}.md"), 'w') as f:
-                    document = export_page(
-                        page,
-                        pandoc_format,
-                        pandoc_options,
-                        id_property,
-                        url_property,
-                        property_map,
-                    )
-                    f.write(document)
+                document = export_page(
+                    page,
+                    pandoc_format,
+                    pandoc_options,
+                    yaml_front_matter,
+                    id_property,
+                    url_property,
+                    property_map,
+                )
+                write_document(document, os.path.join(directory, page_filename))
             else:
-                logger.warning('Skipping page named "%s" since it has been used', page_filename)
-                counts['duplicate'] += 1
+                logger.warning(
+                    'Skipping page named "%s" since it has been used', page_filename
+                )
+                counts["duplicate"] += 1
         else:
-            counts['unnamed'] += 1
+            counts["unnamed"] += 1
     for key, count in counts.items():
         if count > 0:
             logger.info("%d %s page(s) skipped", count, key)
 
 
-def _page_filename(page, filename_property):
-    # TODO: switch to using the database's natural keys as the file names
-    if filename_property is None:
-        return sanitize_filename(page.title.to_plain_text())
-    elif filename_property in page.properties:
-        return sanitize_filename(page.properties[filename_property].to_value())
+def write_document(document, path):
+    if isinstance(document, bytes):
+        file_mode = "wb"
     else:
-        logger.warning(
-            'Invalid filename property, "%s". Valid options are %s',
-            filename_property, ", ".join(page.properties.keys()),
-        )
-        return sanitize_filename(page.title.to_plain_text())
+        file_mode = "w"
+    if os.path.dirname(path):
+        os.makedirs(os.path.dirname(path), exist_ok=True)
+    with open(path, file_mode) as f:
+        f.write(document)
+
+
+def _page_filename(page, pandoc_format, filename_template=None):
+    page_title = page.title.to_plain_text()
+    if filename_template is None:
+        extension = pandoc_format_to_file_extension(pandoc_format)
+        return sanitize_filename(f"{page_title}.{extension}")
+    else:
+        page_properties = page.properties_to_values()
+        if "TITLE" not in page_properties:
+            page_properties["TITLE"] = page_title
+        try:
+            return sanitize_filename(filename_template.format(**page_properties))
+        except KeyError:
+            logger.warning(
+                'Invalid filename property, "%s". Valid options are %s',
+                filename_template,
+                ", ".join(page.properties.keys()),
+            )
+            return _page_filename(page, pandoc_format)
```

### Comparing `n2y-0.7.5/n2y/file.py` & `n2y-0.8.0/n2y/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,7 +19,10 @@
         elif notion_data['type'] == "external":
             logger.debug('Instantiating external file "%s"', notion_data['external']['url'])
             self.type = "external"
             self.url = notion_data['external']['url']
         else:
             file_type = notion_data['type']
             raise ValueError(f'Unknown file type "{file_type}"')
+
+    def to_value(self):
+        return self.url
```

### Comparing `n2y-0.7.5/n2y/main.py` & `n2y-0.8.0/n2y/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,77 @@
 import os
 import sys
 import logging
 import argparse
 import pkg_resources
+import yaml
 
 from n2y import notion
-from n2y.config import load_config
-from n2y.utils import load_yaml, share_link_from_id, DEFAULT_MAX_RETRIES
-from n2y.export import export_page, database_to_yaml, database_to_markdown_files
+from n2y.config import load_config, merge_default_config
+from n2y.utils import share_link_from_id
+from n2y.export import export_page, database_to_yaml, database_to_files, write_document
 
 logger = None
 
 
 def cli_main():
     args = sys.argv[1:]
     access_token = os.environ.get('NOTION_ACCESS_TOKEN', None)
-    sys.exit(main(args, access_token))
+    n2y_cache = os.environ.get('N2Y_CACHE', None)
+    sys.exit(main(args, access_token, n2y_cache))
 
 
-def main(raw_args, access_token):
+def main(raw_args, access_token, n2y_cache=None):
     parser = argparse.ArgumentParser(
         description="Move data from Notion into YAML/markdown",
         formatter_class=argparse.RawTextHelpFormatter,
     )
     parser.add_argument("config", help="The path to the config file")
     parser.add_argument(
-        "--render-config",
-        help="yaml file that configures jinja for the \"render.py\" plugin if it's active"
-    )
-    parser.add_argument(
-        '--max_retries', '-m', default=DEFAULT_MAX_RETRIES,
-        help=(
-            'The maximum amount of times an API request will be retried after being rate '
-            'limited. This argument must be an integer greater than or equal to 5'
-        )
-    )
-    parser.add_argument(
         "--verbosity", '-v', default='INFO',
         help="Level to set the root logging module to",
     )
     parser.add_argument(
         "--version", action='version', version=pkg_resources.require("n2y")[0].version,
         help="The version of n2y installed",
     )
 
     args = parser.parse_args(raw_args)
 
     logging_level = logging.__dict__[args.verbosity]
-    logging.basicConfig(level=logging_level)
+    stdout_handler = logging.StreamHandler(stream=sys.stdout)
+    logging.basicConfig(level=logging_level, handlers=[stdout_handler])
     global logger
     logger = logging.getLogger(__name__)
 
+    if n2y_cache is not None:
+        try:
+            import requests_cache
+            requests_cache.install_cache(n2y_cache, backend='sqlite', expire_after=-1)
+            logger.info("Using cache at %s", n2y_cache)
+        except ImportError:
+            logger.warning(
+                "The requests_cache module is not installed. "
+                "Ignoring N2Y_CACHE %s", n2y_cache,
+            )
+
     if access_token is None:
         logger.critical('No NOTION_ACCESS_TOKEN environment variable is set')
         return 1
 
-    if args.render_config is None:
-        render_config = args.render_config
-    else:
-        with open(args.render_config) as data_file:
-            data_string = data_file.read()
-        render_config = load_yaml(data_string)
-
     config = load_config(args.config)
     if config is None:
         return 2
+    export_defaults = merge_default_config(config.get("export_defaults", {}))
 
     client = notion.Client(
         access_token,
         config["media_root"],
         config["media_url"],
-        max_retries=args.max_retries,
-        render_config=render_config
+        export_defaults=export_defaults,
     )
 
     error_occurred = False
     for export in config['exports']:
         logger.info("Exporting to %s", export['output'])
         client.load_plugins(export["plugins"])
         export_completed = _export_node_from_config(client, export)
@@ -91,24 +87,24 @@
         if page is None:
             msg = (
                 "Unable to find page with id '%s' (%s). "
                 "Perhaps the integration doesn't have permission to access this page?"
             )
             logger.error(msg, export['id'], share_link_from_id(export['id']))
             return False
-        result = export_page(
+        document = export_page(
             page,
             export["pandoc_format"],
             export["pandoc_options"],
+            export["yaml_front_matter"],
             export["id_property"],
             export["url_property"],
             export["property_map"],
         )
-        with open(export["output"], "w") as f:
-            f.write(result)
+        write_document(document, export["output"])
     else:
         database = client.get_database(export['id'])
         if database is None:
             msg = (
                 "Unable to find database with id '%s' (%s). "
                 "Perhaps the integration doesn't have permission to access this database?"
             )
@@ -122,24 +118,24 @@
                 id_property=export["id_property"],
                 url_property=export["url_property"],
                 content_property=export["content_property"],
                 notion_filter=export["notion_filter"],
                 notion_sorts=export["notion_sorts"],
                 property_map=export["property_map"],
             )
-            client.cache_yaml(export['output'], export['id'], result)
-            with open(export["output"], "w") as f:
-                f.write(result)
+            result = yaml.dump(result, sort_keys=False)
+            write_document(result, export["output"])
         elif node_type == "database_as_files":
-            database_to_markdown_files(
+            database_to_files(
                 database=database,
                 directory=export["output"],
                 pandoc_format=export["pandoc_format"],
                 pandoc_options=export["pandoc_options"],
-                filename_property=export["filename_property"],
+                yaml_front_matter=export["yaml_front_matter"],
+                filename_template=export["filename_template"],
                 notion_filter=export["notion_filter"],
                 notion_sorts=export["notion_sorts"],
                 id_property=export["id_property"],
                 url_property=export["url_property"],
                 property_map=export["property_map"],
             )
         else:
```

### Comparing `n2y-0.7.5/n2y/mentions.py` & `n2y-0.8.0/n2y/mentions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pandoc.types import Str
 from n2y.blocks import RowBlock
-
+from n2y.rich_text import RichText
 from n2y.utils import process_notion_date, processed_date_to_plain_text
 
 
 class Mention:
     def __init__(self, client, notion_data, plain_text, block=None):
         self.client = client
         self.block = block
@@ -14,15 +14,17 @@
 
 class UserMention(Mention):
     def __init__(self, client, notion_data, plain_text, block=None):
         super().__init__(client, notion_data, plain_text, block)
         self.user = client.wrap_notion_user(notion_data["user"])
 
     def to_pandoc(self):
-        return [Str(self.user.name)] if self.user.name else []
+        return RichText.plain_text_to_pandoc(
+            self.user.name
+        )if self.user.name else []
 
 
 class PageMention(Mention):
     def __init__(self, client, notion_data, plain_text, block=None):
         # workaround for a bug in the Notion API wheren the plain_text is
         # untitled inside simple tables
         if plain_text == "Untitled" and isinstance(block, RowBlock):
@@ -32,24 +34,24 @@
 
         super().__init__(client, notion_data, plain_text, block)
         self.notion_page_id = notion_data["page"]["id"]
 
     def to_pandoc(self):
         # TODO: if the page is being exported too, then make this a relative
         # URL to that page
-        return [Str(self.plain_text)]
+        return RichText.plain_text_to_pandoc(self.plain_text)
 
 
 class DatabaseMention(Mention):
     def __init__(self, client, notion_data, plain_text, block=None):
         super().__init__(client, notion_data, plain_text, block)
         self.notion_database_id = notion_data["database"]["id"]
 
     def to_pandoc(self):
-        return [Str(self.plain_text)]
+        return RichText.plain_text_to_pandoc(self.plain_text)
 
 
 class DateMention(Mention):
     def __init__(self, client, notion_data, plain_text, block=None):
         super().__init__(client, notion_data, plain_text, block)
         self.processed_date = process_notion_date(notion_data["date"])
```

### Comparing `n2y-0.7.5/n2y/notion.py` & `n2y-0.8.0/n2y/notion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import json
 import logging
 import requests
-import functools
 import importlib.util
-from time import sleep
 from os import path, makedirs
 from urllib.parse import urljoin, urlparse
 
 from n2y.user import User
 from n2y.file import File
 from n2y.page import Page
 from n2y.emoji import Emoji
@@ -15,21 +13,24 @@
 from n2y.database import Database
 from n2y.blocks import DEFAULT_BLOCKS
 from n2y.mentions import DEFAULT_MENTIONS
 from n2y.properties import DEFAULT_PROPERTIES
 from n2y.notion_mocks import mock_rich_text_array
 from n2y.property_values import DEFAULT_PROPERTY_VALUES
 from n2y.rich_text import DEFAULT_RICH_TEXTS, RichTextArray
-from n2y.utils import load_yaml, sanitize_filename, strip_hyphens, DEFAULT_MAX_RETRIES
+from n2y.utils import retry_api_call, sanitize_filename, strip_hyphens
+from n2y.config import merge_default_config
 from n2y.errors import (
     HTTPResponseError, APIResponseError, ObjectNotFound, PluginError,
     UseNextClass, is_api_error_code, APIErrorCode
 )
 
 
+# TODO: Rename this file `client.py`
+
 DEFAULT_NOTION_CLASSES = {
     "page": Page,
     "database": Database,
     "blocks": DEFAULT_BLOCKS,
     "properties": DEFAULT_PROPERTIES,
     "property_values": DEFAULT_PROPERTY_VALUES,
     "user": User,
@@ -40,48 +41,14 @@
     "mentions": DEFAULT_MENTIONS,
     "comment": Comment,
 }
 
 
 logger = logging.getLogger(__name__)
 
-# TODO: Rename this file `client.py`
-
-
-def retry_api_call(api_call):
-    @functools.wraps(api_call)
-    def wrapper(*args, **kwargs):
-        client = args[0]
-        if not isinstance(client, Client):
-            raise NotImplementedError(
-                'The first argument of functions wrapped by '
-                'retry_api_call must be a n2y.notion `Client` object'
-            )
-        try:
-            response = api_call(*args, **kwargs)
-            client.retry_count = 0
-            return response
-        except APIResponseError as err:
-            can_retry = 'retry-after' in err.headers
-            if can_retry and client.retry_api_calls:
-                client.retry_count += 1
-                retry_after = float(err.headers['retry-after'])
-                logger.info(
-                    'Client has been rate limited. This API call '
-                    f'will be retried in {retry_after} seconds'
-                )
-                sleep(retry_after)
-                return wrapper(*args, **kwargs)
-            else:
-                client.retry_api_calls or logger.warning(
-                    'The maximum amount of retries for this function has been reached'
-                )
-                raise err
-    return wrapper
-
 
 class Client:
     """
     An instance of the client class has a few purposes:
 
     1. To retrieve data from Notion
     2. To determine what classes to use to wrap this notion data
@@ -95,53 +62,34 @@
 
     def __init__(
         self,
         access_token,
         media_root='.',
         media_url='',
         plugins=None,
-        max_retries=DEFAULT_MAX_RETRIES,
-        render_config=None
+        export_defaults=None,
     ):
-        self.render_config = render_config
         self.access_token = access_token
         self.media_root = media_root
         self.media_url = media_url
-        self.max_retries = max_retries
-        self.retry_count = 0
+        self.export_defaults = export_defaults or merge_default_config({})
 
         self.base_url = "https://api.notion.com/v1/"
         self.headers = {
             "Authorization": f"Bearer {self.access_token}",
             "Content-Type": "application/json",
             "Notion-Version": "2022-06-28",
         }
 
         self.databases_cache = {}
         self.pages_cache = {}
-        self.yaml_cache = {}
 
         self.load_plugins(plugins)
         self.plugin_data = {}
 
-    @property
-    def retry_api_calls(self):
-        return self.max_retries > self.retry_count
-
-    @property
-    def max_retries(self):
-        return self._max_retries
-
-    @max_retries.setter
-    def max_retries(self, val):
-        if int(val) > DEFAULT_MAX_RETRIES:
-            raise NotImplementedError('max_retries must be an integer no larger than 5')
-        else:
-            self._max_retries = int(val)
-
     def get_default_classes(self):
         notion_classes = {}
         for notion_object, object_types in DEFAULT_NOTION_CLASSES.items():
             if type(object_types) == dict:
                 notion_classes[notion_object] = {k: [v] for k, v in object_types.items()}
             else:
                 notion_classes[notion_object] = [object_types]
@@ -168,40 +116,47 @@
 
     def _override_notion_classes(self, notion_object, object_types, default_object_types):
         # E.g., there are many types of notion blocks but only one type of notion page.
         notion_object_has_types = isinstance(default_object_types, dict)
 
         if notion_object_has_types and isinstance(object_types, dict):
             for object_type, plugin_class in object_types.items():
-                if object_type in default_object_types:
-                    class_being_replaced = default_object_types[object_type]
-                    # assumes all of the default classes have a single parent class
-                    base_class = class_being_replaced.__bases__[0]
-                    if issubclass(plugin_class, base_class):
-                        self.notion_classes[notion_object][object_type].append(plugin_class)
-                    else:
-                        raise PluginError(
-                            f'Cannot use "{plugin_class.__name__}", as it doesn\'t '
-                            f'override the base class "{base_class.__name__}"',
-                        )
-                else:
-                    raise PluginError(f'Invalid type "{object_type}" for "{notion_object}"')
+                self._organize_notion_classes(
+                    default_object_types, notion_object, object_type, plugin_class
+                )
         elif notion_object_has_types and not isinstance(object_types, dict):
             raise PluginError(f'Expecting dict for "{notion_object}", found "{type(object_types)}"')
         else:
             plugin_class = object_types
             base_class = default_object_types
             if issubclass(plugin_class, base_class):
                 self.notion_classes[notion_object].append(plugin_class)
             else:
                 raise PluginError(
                     f'Cannot use "{plugin_class.__name__}", as it doesn\'t '
                     f'override the base class "{base_class.__name__}"',
                 )
 
+    def _organize_notion_classes(
+        self, default_object_types, notion_object, object_type, plugin_class
+    ):
+        if object_type in default_object_types:
+            class_being_replaced = default_object_types[object_type]
+            # assumes all of the default classes have a single parent class
+            base_class = class_being_replaced.__bases__[0]
+            if issubclass(plugin_class, base_class):
+                self.notion_classes[notion_object][object_type].append(plugin_class)
+            else:
+                raise PluginError(
+                    f'Cannot use "{plugin_class.__name__}", as it doesn\'t '
+                    f'override the base class "{base_class.__name__}"',
+                )
+        else:
+            raise PluginError(f'Invalid type "{object_type}" for "{notion_object}"')
+
     def get_class_list(self, notion_object, object_type=None):
         if object_type is None:
             return self.notion_classes[notion_object]
         try:
             return self.notion_classes[notion_object][object_type]
         except KeyError:
             raise NotImplementedError(f'Unknown "{notion_object}" class of type "{object_type}"')
@@ -226,18 +181,30 @@
         `get_page` or through `get_database_pages`. Thus, it's possible that a
         database page be first retrieved individually and then retrieved via the
         full database. In this case, it's unfortunate (but unavoidable) that we
         retrieved the data from Notion twice, but even so we don't want to
         replace our existing page instance, along with it's content or other
         state that has been added to it.
         """
-        if notion_data["id"] in self.pages_cache:
+        page_in_cache = notion_data["id"] in self.pages_cache
+        if page_in_cache and self.page_class_is_in_use(
+            # Need to check that the page in the client cache was instantiated using
+            # the currently favored page class. Otherwise, plugins set for one export
+            # will be used in another or a plugin will be set but not used.
+            # As we currently use the `jinjarenderpage` plugin for all pages,
+            # this check is most likely uneccessary at this point.
+            self.pages_cache[notion_data["id"]]
+        ):
             return self.pages_cache[notion_data["id"]]
         else:
             page = self.instantiate_class("page", None, self, notion_data)
+            not page_in_cache or logger.warning((
+                "page in cache overwritten at "
+                f"key \"{notion_data['id']}\""
+            ))
             self.pages_cache[page.notion_id] = page
             return page
 
     def _wrap_notion_database(self, notion_data):
         return self.instantiate_class("database", None, self, notion_data)
 
     def wrap_notion_block(self, notion_data, page, get_children):
@@ -270,16 +237,22 @@
             "mentions", notion_data["type"],
             self, notion_data, plain_text, block,
         )
 
     def wrap_notion_property(self, notion_data):
         return self.instantiate_class("properties", notion_data["type"], self, notion_data)
 
-    def wrap_notion_property_value(self, notion_data):
-        return self.instantiate_class("property_values", notion_data["type"], self, notion_data)
+    def wrap_notion_property_value(self, notion_data, page):
+        return self.instantiate_class(
+            "property_values",
+            notion_data["type"],
+            self,
+            notion_data,
+            page
+        )
 
     def get_page_or_database(self, object_id):
         """
         First attempt to get the page corresponding with the object id; if
         the page doesn't exist, then attempt to retrieve the database. This
         trial-and-error is necessary because the API doesn't provide a means to
         determining what type of object corresponds with an ID and we don't want
@@ -296,25 +269,29 @@
         Retrieve the database (but not it's pages) if its not in the cache. Even
         if it is in the cache.
         """
         if database_id in self.databases_cache:
             database = self.databases_cache[database_id]
         else:
             try:
-                notion_database = self._get_url(f"{self.base_url}databases/{database_id}")
+                notion_database = self.get_notion_database(database_id)
                 database = self._wrap_notion_database(notion_database)
             except ObjectNotFound:
                 database = None
             self.databases_cache[database_id] = database
         return database
 
+    def get_notion_database(self, database_id):
+        return self._get_url(f"{self.base_url}databases/{database_id}")
+
     def get_database_pages(self, database_id, filter=None, sorts=None):
         notion_pages = self.get_database_notion_pages(database_id, filter, sorts)
         return [self._wrap_notion_page(np) for np in notion_pages]
 
+    @retry_api_call
     def get_database_notion_pages(self, database_id, filter, sorts):
         url = f"{self.base_url}databases/{database_id}/query"
         request_data = {}
         if filter:
             request_data["filter"] = filter
         if sorts:
             request_data["sorts"] = sorts
@@ -322,42 +299,49 @@
 
     def get_page(self, page_id):
         """
         Retrieve the page if its not in the cache.
         """
         if page_id in self.pages_cache:
             page = self.pages_cache[page_id]
+            if not self.page_class_is_in_use(page):
+                page = self.instantiate_class("page", None, self, page.notion_data)
         else:
             try:
-                notion_page = self._get_url(f"{self.base_url}pages/{page_id}")
+                notion_page = self.get_notion_page(page_id)
             except ObjectNotFound:
                 self.pages_cache[page_id] = None
                 return
             # _wrap_notion_page will add the page to the cache
             page = self._wrap_notion_page(notion_page)
         return page
 
+    def get_notion_page(self, page_id):
+        return self._get_url(f"{self.base_url}pages/{page_id}")
+
     def get_block(self, block_id, page, get_children=True):
         notion_block = self.get_notion_block(block_id)
         return self.wrap_notion_block(notion_block, page, get_children)
 
     @retry_api_call
     def get_notion_block(self, block_id):
         url = f"{self.base_url}blocks/{block_id}"
         response = requests.get(url, headers=self.headers)
         return self._parse_response(response)
 
     def get_child_blocks(self, block_id, page, get_children):
         child_notion_blocks = self.get_child_notion_blocks(block_id)
         return [self.wrap_notion_block(b, page, get_children) for b in child_notion_blocks]
 
+    @retry_api_call
     def get_child_notion_blocks(self, block_id):
         url = f"{self.base_url}blocks/{block_id}/children"
         return self._paginated_request(self._get_url, url, {})
 
+    @retry_api_call
     def get_comments(self, block_id):
         url = f"{self.base_url}comments"
         comments = self._paginated_request(self._get_url, url, {"block_id": block_id})
         return [self.wrap_notion_comment(nd) for nd in comments]
 
     def wrap_notion_comment(self, notion_data):
         return self.instantiate_class("comment", None, self, notion_data)
@@ -467,124 +451,158 @@
         ]
         for page in db_children:
             page['parent'] = {
                 'type': 'database_id',
                 'database_id': destination['id']
             }
             for key in page['properties'].keys():
-                prop = page['properties'][key]
-                del prop['id']
-                prop_type = prop['type']
-                del prop['type']
-                prop_type_info = prop[prop_type]
-                if isinstance(prop_type_info, dict):
-                    if 'id' in prop_type_info:
-                        del prop_type_info['id']
-                elif isinstance(prop_type_info, list) and prop_type != 'relation':
-                    for item in prop_type_info:
-                        if 'id' in item:
-                            del item['id']
+                page['properties'][key] = self._edit_notion_child_property(
+                    page['properties'][key]
+                )
             self.create_notion_page(page)
 
+    def _edit_notion_child_property(self, prop):
+        del prop['id']
+        prop_type = prop['type']
+        del prop['type']
+        prop_type_info = prop[prop_type]
+        if isinstance(prop_type_info, dict):
+            if 'id' in prop_type_info:
+                del prop_type_info['id']
+        elif isinstance(prop_type_info, list) and prop_type != 'relation':
+            for item in prop_type_info:
+                if 'id' in item:
+                    del item['id']
+        return prop
+
     @retry_api_call
     def append_child_notion_blocks(self, block_id, children):
         '''
         Appends each datapoint of a list of notion_data as children to the block specified by id.
         Please note that not all block types are allowed to have children, so this method only works
         for those that are.
         '''
-        def append_blocks(i1, i2, blocks, list):
-            max_new_blocks = 100
-            if i1 < i2:
-                child_list = blocks[i1:i2]
-                length = len(child_list)
-                for i in range(0, length, max_new_blocks):
-                    portion_index_stop = i + max_new_blocks
-                    if portion_index_stop < length:
-                        portion = child_list[i:portion_index_stop]
-                    else:
-                        portion = child_list[i:]
-                    response = requests.patch(
-                        f"{self.base_url}blocks/{block_id}/children",
-                        json={"children": portion}, headers=self.headers
-                    )
-                    appension_return = self._parse_response(response)
-                    list.extend(appension_return['results'])
-            return list
-
-        last_i = 0
+        previous_i = 0
         children_appended = []
         parent = self.get_page_or_database(block_id) or self.get_block(block_id, None)
         parent_type = parent.notion_data["object"]
-        type_is_database = lambda child: 'type' in child and child['type'] == 'child_database'
-        object_is_database = lambda child: child['object'] == 'database'
-        type_is_page = lambda child: 'type' in child and child['type'] == 'child_page'
-        object_is_page = lambda child: child['object'] == 'page'
-        bad_keys = [
-            'last_edited_by',
-            'created_time',
-            'last_edited_time',
-            'created_by'
-        ]
+
+        def type_is_database(child):
+            return 'type' in child and child['type'] == 'child_database'
+
+        def object_is_database(child):
+            return child['object'] == 'database'
+
+        def type_is_page(child):
+            return 'type' in child and child['type'] == 'child_page'
+
+        def object_is_page(child):
+            return child['object'] == 'page'
+
         for i, child in enumerate(children):
             if object_is_database(child) or type_is_database(child):
-                children_appended = append_blocks(last_i, i, children, children_appended)
-                if parent_type == 'block':
-                    logger.warning((
-                        'Skipping database with block type parent as '
-                        'appension is currently unsupported by Notion API'
-                    ))
-                    child_database = {}
-                else:
-                    database = self.get_database(child['id'])
-                    child = {
-                        key: value
-                        for (key, value) in
-                        database.notion_data.items()
-                        if key not in bad_keys
-                    }
-                    child['parent'] = {
-                        'type': f'{parent_type}_id',
-                        f'{parent_type}_id': parent.notion_id
-                    }
-                    child_database = self.create_notion_database(child)
-                    if database.children:
-                        notion_children = [child.notion_data for child in database.children]
-                        self.copy_notion_database_children(notion_children, child_database)
+                children_appended = self._append_blocks(
+                    block_id, children, children_appended, previous_i, i
+                )
+                child_database = self._copy_notion_database_child_database(
+                    parent, parent_type, child
+                )
                 children_appended.append(child_database)
-                last_i = i + 1
+                previous_i = i + 1
             elif object_is_page(child) or type_is_page(child):
-                children_appended = append_blocks(last_i, i, children, children_appended)
-                if parent_type == 'block':
-                    logger.warning((
-                        'Skipping page with block type parent as '
-                        'appension is currently unsupported by Notion API'
-                    ))
-                    child_page = {}
-                else:
-                    page = self.get_page(child['id'])
-                    child = {
-                        key: value
-                        for (key, value) in
-                        page.notion_data.items()
-                        if key not in bad_keys
-                    }
-                    child['parent'] = {
-                        'type': f'{parent_type}_id',
-                        f'{parent_type}_id': parent.notion_id
-                    }
-                    child_page = self.create_notion_page(child)
+                children_appended = self._append_blocks(
+                    block_id, children, children_appended, previous_i, i
+                )
+                child_page = self._copy_notion_database_child_page(parent, parent_type, child)
                 children_appended.append(child_page)
-                last_i = i + 1
+                previous_i = i + 1
             elif i == len(children) - 1:
-                children_appended = append_blocks(
-                    last_i, len(children), children, children_appended
+                children_appended = self._append_blocks(
+                    block_id, children, children_appended, previous_i, len(children)
                 )
         return children_appended
 
+    def _append_blocks(self, block_id, full_child_data_list, appension_history_list, i1=0, i2=0):
+        max_new_blocks = 100
+        if i1 < i2:
+            child_data_list = full_child_data_list[i1:i2]
+            length = len(child_data_list)
+            for i in range(0, length, max_new_blocks):
+                portion_index_stop = i + max_new_blocks
+                if portion_index_stop < length:
+                    portion = child_data_list[i:portion_index_stop]
+                else:
+                    portion = child_data_list[i:]
+                response = requests.patch(
+                    f"{self.base_url}blocks/{block_id}/children",
+                    json={"children": portion}, headers=self.headers
+                )
+                appension_return = self._parse_response(response)
+                appension_history_list.extend(appension_return['results'])
+        return appension_history_list
+
+    def _copy_notion_database_child_page(self, parent, parent_type, child_notion_data):
+        bad_keys = [
+            'last_edited_by',
+            'created_time',
+            'last_edited_time',
+            'created_by'
+        ]
+        if parent_type == 'block':
+            logger.warning((
+                'Skipping page with block type parent as '
+                'appension is currently unsupported by Notion API'
+            ))
+            child_page = {}
+        else:
+            page = self.get_page(child_notion_data['id'])
+            child_page_data = {
+                key: value
+                for (key, value) in
+                page.notion_data.items()
+                if key not in bad_keys
+            }
+            child_page_data['parent'] = {
+                'type': f'{parent_type}_id',
+                f'{parent_type}_id': parent.notion_id
+            }
+            child_page = self.create_notion_page(child_page_data)
+        return child_page
+
+    def _copy_notion_database_child_database(self, parent, parent_type, child_notion_data):
+        bad_keys = [
+            'last_edited_by',
+            'created_time',
+            'last_edited_time',
+            'created_by'
+        ]
+        if parent_type == 'block':
+            logger.warning((
+                'Skipping database with block type parent as '
+                'appension is currently unsupported by Notion API'
+            ))
+            child_database = {}
+        else:
+            database = self.get_database(child_notion_data['id'])
+            child_database_data = {
+                key: value
+                for (key, value) in
+                database.notion_data.items()
+                if key not in bad_keys
+            }
+            child_database_data['parent'] = {
+                'type': f'{parent_type}_id',
+                f'{parent_type}_id': parent.notion_id
+            }
+            child_database = self.create_notion_database(child_database_data)
+            if database.children:
+                notion_children = [child.notion_data for child in database.children]
+                self.copy_notion_database_children(notion_children, child_database)
+        return child_database
+
     @retry_api_call
     def create_notion_comment(self, page_id, text_blocks_descriptors):
         data = {
             "rich_text": mock_rich_text_array(text_blocks_descriptors),
             "parent": {
                 "type": "page_id",
                 "page_id": page_id,
@@ -611,23 +629,15 @@
         headers = {**self.headers}
         del headers['Content-Type']
         response = requests.delete(
             f"{self.base_url}blocks/{block_id}", headers=headers
         )
         return self._parse_response(response)
 
-    def cache_yaml(self, data_filename, database_id, data_string):
-        data_name, _ = path.splitext(path.basename(data_filename))
-        if data_name in self.yaml_cache:
-            raise ValueError('There is already data attached to the key "{}"'.format(data_name))
-        yaml_data = load_yaml(data_string)
-        self.yaml_cache[data_name] = {
-            'id': database_id,
-            'data': yaml_data
-        }
-        return data_name
-
-    def context_from_yaml_cache(self):
-        context = {}
-        for data_name in self.yaml_cache:
-            context[data_name] = self.yaml_cache[data_name]['data']
-        return context
+    def page_class_is_in_use(self, page):
+        '''
+        Checks if the given page has been instantiated
+        with the currently favored page class in use.
+        '''
+        if page is None or self.notion_classes['page'][-1] == type(page):
+            return True
+        return False
```

### Comparing `n2y-0.7.5/n2y/notion_mocks.py` & `n2y-0.8.0/n2y/notion_mocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,26 @@
 def mock_rich_text_array(text_blocks_descriptors):
     if isinstance(text_blocks_descriptors, str):
         return [mock_rich_text(text_blocks_descriptors, [])]
     else:
         return [mock_rich_text(*desc) for desc in text_blocks_descriptors]
 
 
-def mock_rich_text(text, annotations=None, href=None, mention=None, link=None):
+def mock_rich_text(text, annotations=None, href=None, mention=None, link=None, equation=None):
     if annotations is None:
         annotations = []
-    if mention is None:
-        rich_text_type = 'text'
-        content = {'content': text, 'link': link}
-    else:
+    if mention:
         rich_text_type = 'mention'
         content = mention
+    elif equation:
+        rich_text_type = 'equation'
+        content = equation
+    else:
+        rich_text_type = 'text'
+        content = {'content': text, 'link': link}
     return {
         'type': rich_text_type,
         'annotations': mock_annotations(annotations),
         'plain_text': text,
         'href': href,
         rich_text_type: content,
     }
@@ -71,19 +74,19 @@
         'type': 'page',
         'page': {
             'id': mock_id(),
         },
     }
 
 
-def mock_database_mention():
+def mock_database_mention(id=None):
     return {
         'type': 'database',
         'database': {
-            'id': mock_id(),
+            'id': id or mock_id(),
         },
     }
 
 
 def mock_block(block_type, content, has_children=False, **kwargs):
     created_by = mock_user()
     created_time = datetime.now().isoformat()
@@ -183,15 +186,17 @@
                 'title': mock_rich_text_array(title)
             }, **extra_properties,
         },
         'url': f'https://www.notion.so/{hyphenated_title}-{notion_id}',
     }
 
 
-def mock_database(title='Mock Database', extra_properties={}):
+def mock_database(title='Mock Database', extra_properties=None):
+    if extra_properties is None:
+        extra_properties = {}
     hyphenated_title = title.replace(" ", "-")
     created_time = datetime.now().isoformat()
     notion_id = mock_id()
     user = mock_user()
     return {
         'object': 'database',
         'id': notion_id,
@@ -202,39 +207,20 @@
         'created_by': user,
         'last_edited_by': user,
         'title': mock_rich_text_array(title),
         'description': [],
         'is_inline': False,
         'archived': False,
         'properties': {
-            'Tags': {
-                'id': mock_id(),
-                'name': 'Tags',
-                'type': 'multi_select',
-                'multi_select': {'options': []}
-            },
-            'Number': {
-                'id': mock_id(),
-                'name': 'Number',
-                'type': 'number',
-                'number': {'format': 'number'}
-            },
             'Name': {
-                'id': 'title',
+                'id': 'title',  # all title properties have id 'title'
                 'name': 'Name',
                 'type': 'title',
                 'title': {}
             }, **extra_properties,
         },
         'parent': {
             'type': 'page_id',
             'page_id': mock_id()
         },
         'url': f'https://www.notion.so/{hyphenated_title}-{notion_id}',
     }
-
-
-class MockResponse():
-    def __init__(self, time, code):
-        self.headers = {'retry-after': time}
-        self.text = ''
-        self.status_code = code
```

### Comparing `n2y-0.7.5/n2y/page.py` & `n2y-0.8.0/n2y/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.last_edited_time = fromisoformat(notion_data['last_edited_time'])
         self.last_edited_by = client.wrap_notion_user(notion_data['last_edited_by'])
         self.archived = notion_data['archived']
         self.emoji = self._init_icon(notion_data['icon'])
         self.cover = notion_data['cover'] and client.wrap_notion_file(notion_data['cover'])
         self.archived = notion_data['archived']
         self.properties = {
-            k: client.wrap_notion_property_value(npv)
+            k: client.wrap_notion_property_value(npv, self)
             for k, npv in notion_data['properties'].items()
         }
         self.notion_parent = notion_data['parent']
         self.notion_url = notion_data['url']
 
         self._block = None
         self._children = None
@@ -99,9 +99,9 @@
         else:
             assert parent_type == "database_id"
             return self.client.get_database(self.notion_parent["database_id"])
 
     def to_pandoc(self):
         return self.block.to_pandoc()
 
-    def properties_to_values(self):
-        return {k: v.to_value() for k, v in self.properties.items()}
+    def properties_to_values(self, pandoc_format=None):
+        return {k: v.to_value(pandoc_format) for k, v in self.properties.items()}
```

### Comparing `n2y-0.7.5/n2y/plugins/deepheaders.py` & `n2y-0.8.0/n2y/plugins/deepheaders.py`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y/plugins/expandlinktopages.py` & `n2y-0.8.0/n2y/plugins/expandlinktopages.py`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y/plugins/footnotes.py` & `n2y-0.8.0/n2y/plugins/footnotes.py`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y/plugins/linkedheaders.py` & `n2y-0.8.0/n2y/plugins/linkedheaders.py`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y/plugins/mermaid.py` & `n2y-0.8.0/n2y/plugins/mermaid.py`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y/plugins/rawcodeblocks.py` & `n2y-0.8.0/n2y/plugins/rawcodeblocks.py`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y/plugins/removecallouts.py` & `n2y-0.8.0/n2y/plugins/removecallouts.py`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y/properties.py` & `n2y-0.8.0/n2y/properties.py`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y/property_values.py` & `n2y-0.8.0/n2y/property_values.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,260 +4,269 @@
 from n2y.utils import fromisoformat, process_notion_date, processed_date_to_plain_text
 
 
 logger = logging.getLogger(__name__)
 
 
 class PropertyValue:
-    def __init__(self, client, notion_data):
+    def __init__(self, client, notion_data, page):
         self.client = client
         self.notion_property_id = notion_data.get(
             'id', None)  # will be none for rollup array values
         self.notion_type = notion_data['type']
+        self.page = page
 
-    def to_value(self):
+    def to_value(self, pandoc_format=None):
         raise NotImplementedError()
 
 
 class TitlePropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
+    def __init__(self, client, notion_data, page):
         # TODO: handle the case when there are more than 25 rich text items in the property
         # See https://developers.notion.com/reference/retrieve-a-page-property
-        super().__init__(client, notion_data)
+        super().__init__(client, notion_data, page)
         self.rich_text = client.wrap_notion_rich_text_array(notion_data['title'])
 
-    def to_value(self):
+    def to_value(self, _=None):
         # Notion allows styling of the title, however, in their UI they display
         # the title property without any styling. Thus, if you copy/paste styled
         # text into a title this styling can be hidden and can re-appear after
         # the document conversion. To avoid this surprise, we only generate
         # plain text here.
         return self.rich_text.to_plain_text()
 
 
 class TextPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
+    def __init__(self, client, notion_data, page):
         # TODO: handle the case when there are more than 25 rich text items in the property
         # See https://developers.notion.com/reference/retrieve-a-page-property
-        super().__init__(client, notion_data)
+        super().__init__(client, notion_data, page)
         self.rich_text = client.wrap_notion_rich_text_array(notion_data['rich_text'])
 
-    def to_value(self):
-        return self.rich_text.to_markdown()
+    def to_value(self, pandoc_format):
+        if pandoc_format is None:
+            return self.rich_text.to_plain_text()
+        else:
+            return self.rich_text.to_value(pandoc_format)
 
 
 class NumberPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.number = notion_data['number']
 
-    def to_value(self):
+    def to_value(self, _=None):
         return self.number
 
 
 class SelectPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         notion_select = notion_data['select']
         if notion_select is not None:
             self.notion_option_id = notion_select['id']
             self.name = notion_select['name']
             self.color = notion_select['color']
         else:
             self.notion_option_id = None
             self.name = None
             self.color = None
 
-    def to_value(self):
+    def to_value(self, _=None):
         # Note: the Notion UI shouldn't allow you to have two options with the
         # same name
         return self.name
 
 
 class MultiSelectPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.options = [MultiSelectOption(self.client, no) for no in notion_data['multi_select']]
 
-    def to_value(self):
+    def to_value(self, _=None):
         # Note: the Notion UI shouldn't allow you to have two options with the
         # same name
         return [o.name for o in self.options]
 
 
 class MultiSelectOption:
     def __init__(self, client, notion_option):
         self.client = client
         self.notion_id = notion_option['id']
         self.name = notion_option['name']
         self.color = notion_option['color']
 
 
 class DatePropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
+    def __init__(self, client, notion_data, page):
         # TODO: handle timezones
-        super().__init__(client, notion_data)
+        super().__init__(client, notion_data, page)
         self.value = process_notion_date(notion_data['date'])
 
-    def to_value(self):
+    def to_value(self, _=None):
         return self.value
 
     def to_plain_text(self):
         return processed_date_to_plain_text(self.value)
 
 
 class PeoplePropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.people = [client.wrap_notion_user(nu) for nu in notion_data['people']]
 
-    def to_value(self):
+    def to_value(self, _=None):
         return [u.to_value() for u in self.people]
 
 
 class FilesPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.files = [client.wrap_notion_file(nf) for nf in notion_data['files']]
 
-    def to_value(self):
+    def to_value(self, _):
         return [f.to_value() for f in self.files]
 
 
 class CheckboxPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.checkbox = notion_data['checkbox']
 
-    def to_value(self):
+    def to_value(self, _):
         return self.checkbox
 
 
 class UrlPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.url = notion_data['url']
 
-    def to_value(self):
+    def to_value(self, _=None):
         return self.url
 
 
 class EmailPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.email = notion_data['email']
 
-    def to_value(self):
+    def to_value(self, _=None):
         return self.email
 
 
 class PhoneNumberPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.phone_number = notion_data['phone_number']
 
-    def to_value(self):
+    def to_value(self, _=None):
         return self.phone_number
 
 
 class FormulaPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         # TODO: set other attributes
         notion_formula = notion_data["formula"]
         if notion_formula["type"] == "date":
             self.value = process_notion_date(notion_formula["date"])
         else:
             self.value = notion_formula[notion_formula["type"]]
 
-    def to_value(self):
+    def to_value(self, _=None):
         return self.value
 
 
 class RelationPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        # TODO: handle the case when there are more than 25 pages in the relation
-        # See https://developers.notion.com/reference/retrieve-a-page-property
-        super().__init__(client, notion_data)
-        self.ids = [related["id"] for related in notion_data["relation"]]
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
+        if "has_more" not in notion_data or not notion_data["has_more"]:
+            self.ids = [related["id"] for related in notion_data["relation"]]
+        else:
+            url = f"{client.base_url}pages/{page.notion_id}/properties/{self.notion_property_id}"
+            self.ids = [
+                r["relation"]["id"] for r in
+                client._paginated_request(client._get_url, url, {})
+            ]
 
-    def to_value(self):
+    def to_value(self, _=None):
         return self.ids
 
 
 class RollupPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
+    def __init__(self, client, notion_data, page):
         # TODO: handle the case when the rollup needs to be paginated
         # See https://developers.notion.com/reference/retrieve-a-page-property
-        super().__init__(client, notion_data)
+        super().__init__(client, notion_data, page)
         notion_rollup = notion_data["rollup"]
         self.rollup_type = notion_rollup["type"]
         self.function = notion_rollup["function"]
         if self.rollup_type == "date":
             self.value = process_notion_date(notion_rollup['date'])
         elif self.rollup_type == "string":
             self.value = notion_rollup['string']
         elif self.rollup_type == "number":
             self.value = notion_rollup['number']
         elif self.rollup_type == "array":
             self.value = [
-                self.client.wrap_notion_property_value(pv)
+                self.client.wrap_notion_property_value(pv, page)
                 for pv in notion_rollup['array']
             ]
         else:
             logger.warning("Unhandled rollup type %s", notion_rollup["type"])
             self.value = notion_rollup[notion_rollup["type"]]
         # TODO: handle arrays of dates
 
-    def to_value(self):
+    def to_value(self, pandoc_format):
         if self.rollup_type == "date":
             return self.value
         elif self.rollup_type == "string":
             return self.value
         elif self.rollup_type == "number":
             return self.value
         elif self.rollup_type == "array":
-            return [pv.to_value() for pv in self.value]
+            return [pv.to_value(pandoc_format) for pv in self.value]
         else:
             return self.value
 
 
 class CreatedTimePropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.created_time = fromisoformat(notion_data['created_time'])
 
-    def to_value(self):
+    def to_value(self, _=None):
         return datetime.isoformat(self.created_time)
 
 
 class CreatedByPropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.created_by = client.wrap_notion_user(notion_data['created_by'])
 
-    def to_value(self):
+    def to_value(self, _=None):
         return self.created_by.to_value()
 
 
 class LastEditedTimePropertyValue(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.last_edited_time = fromisoformat(notion_data['last_edited_time'])
 
-    def to_value(self):
+    def to_value(self, _=None):
         return datetime.isoformat(self.last_edited_time)
 
 
 class LastEditedBy(PropertyValue):
-    def __init__(self, client, notion_data):
-        super().__init__(client, notion_data)
+    def __init__(self, client, notion_data, page):
+        super().__init__(client, notion_data, page)
         self.last_edited_by = client.wrap_notion_user(notion_data['last_edited_by'])
 
-    def to_value(self):
+    def to_value(self, _=None):
         return self.last_edited_by.to_value()
 
 
 DEFAULT_PROPERTY_VALUES = {
     'title': TitlePropertyValue,
     'rich_text': TextPropertyValue,
     'number': NumberPropertyValue,
```

### Comparing `n2y-0.7.5/n2y/rich_text.py` & `n2y-0.8.0/n2y/rich_text.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections import deque
 
 from pandoc.types import (
     Str, Space, LineBreak, Strong, Emph, Strikeout, Code, Link,
     Underline, Math, InlineMath
 )
 
-from n2y.utils import pandoc_ast_to_markdown
+from n2y.utils import pandoc_write_or_log_errors
 from n2y.notion_mocks import mock_rich_text
 
 
 logger = logging.getLogger(__name__)
 
 
 class RichText:
@@ -39,16 +39,20 @@
         self.underline = annotations["underline"]
         self.code = annotations["code"]
         self.color = annotations["color"]
 
     def to_pandoc(self):
         raise NotImplementedError()
 
-    def to_markdown(self):
-        return pandoc_ast_to_markdown(self.to_pandoc()).strip('\n')
+    def to_value(self, pandoc_format):
+        return pandoc_write_or_log_errors(
+            self.to_pandoc(),
+            format=pandoc_format,
+            options=[],
+        )
 
     @classmethod
     def plain_text_to_pandoc(klass, plain_text):
         ast = []
         match = re.findall(r"( +)|(\xa0+)|(\S+)|(\n+)|(\t+)", plain_text)
         for m in match:
             space, non_breaking_space, word, newline, tab = m
@@ -104,19 +108,22 @@
         if self.strikethrough:
             result = [Strikeout(result)]
 
         return list(prependages) + result + list(appendages)
 
 
 class MentionRichText(RichText):
-    def __init__(self, client, notion_data, block=None):
+    def __init__(self, client, notion_data, block=None, mention=None):
         super().__init__(client, notion_data, block)
-        self.mention = client.wrap_notion_mention(
-            notion_data['mention'], notion_data["plain_text"], block,
-        )
+        if mention is None:
+            self.mention = client.wrap_notion_mention(
+                notion_data['mention'], notion_data["plain_text"], block,
+            )
+        else:
+            self.mention = mention
 
     def to_pandoc(self):
         if self.code:
             logger.warning('Code formatting is being dropped on mention "%s"', self.plain_text)
         mention_ast = self.mention.to_pandoc()
         return self.annotate_pandoc_ast(mention_ast)
 
@@ -194,16 +201,20 @@
 
     def __getitem__(self, index):
         return self.items[index]
 
     def to_pandoc(self):
         return sum([item.to_pandoc() for item in self.items], [])
 
-    def to_markdown(self):
-        return pandoc_ast_to_markdown(self.to_pandoc()).strip('\n')
+    def to_value(self, pandoc_format):
+        return pandoc_write_or_log_errors(
+            self.to_pandoc(),
+            format=pandoc_format,
+            options=[],
+        )
 
     def to_plain_text(self):
         return ''.join(item.plain_text for item in self.items)
 
     def matches(self, regexp):
         if len(self.items) > 0:
             first_item = self.items[0]
@@ -219,12 +230,9 @@
                 string_len = len(string)
                 if first_item.plain_text[:string_len] == string:
                     self.items[0].plain_text = first_item.plain_text[string_len:]
                     if self.items[0].plain_text == "":
                         self.items.pop(0)
 
     def prepend(self, string):
-        if len(self.items) > 0:
-            self.items[0].plain_text = string + self.items[0].plain_text
-        else:
-            rich_text = TextRichText.from_plain_text(self.client, string)
-            self.items.append(rich_text)
+        rich_text = TextRichText.from_plain_text(self.client, string)
+        self.items.insert(0, rich_text)
```

### Comparing `n2y-0.7.5/n2y/user.py` & `n2y-0.8.0/n2y/user.py`

 * *Files identical despite different names*

### Comparing `n2y-0.7.5/n2y.egg-info/PKG-INFO` & `n2y-0.8.0/n2y.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n2y
-Version: 0.7.5
+Version: 0.8.0
 Summary: Notion to YAML
 Home-page: https://github.com/innolitics/n2y
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: notion documentation yaml markdown
 Classifier: Development Status :: 4 - Beta
```

### Comparing `n2y-0.7.5/setup.py` & `n2y-0.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 description = 'Notion to YAML'
 
 setup(
     name='n2y',
-    version='0.7.5',
+    version='0.8.0',
     description=description,
     long_description=description,
     long_description_content_type='text/x-rst',
     url='https://github.com/innolitics/n2y',
     author='Innolitics, LLC',
     author_email='info@innolitics.com',
     license='MIT',
@@ -32,14 +32,15 @@
     packages=find_packages(exclude=['tests']),
     install_requires=['pyyaml', 'requests', 'pandoc', 'jinja2'],
     extras_require={
         'dev': [
             'pytest',
             'flake8',
             'check-manifest',
+            'requests-cache',
         ]
     },
     include_package_data=True,
     package_data={'n2y': ['data/mermaid_err.png']},
     entry_points={
         'console_scripts': [
             'n2y = n2y.main:cli_main',
```

