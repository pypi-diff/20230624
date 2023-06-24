# Comparing `tmp/mizue-0.3.4.tar.gz` & `tmp/mizue-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizue-0.3.4.tar", last modified: Wed Jun 21 18:24:38 2023, max compression
+gzip compressed data, was "mizue-0.4.0.tar", last modified: Sat Jun 24 18:19:38 2023, max compression
```

## Comparing `mizue-0.3.4.tar` & `mizue-0.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.354353 mizue-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 18:24:19.000000 mizue-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-21 18:24:38.354353 mizue-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-21 18:24:19.000000 mizue-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.346353 mizue-0.3.4/mizue/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.346353 mizue-0.3.4/mizue/file/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/file/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.346353 mizue-0.3.4/mizue/network/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.350353 mizue-0.3.4/mizue/network/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.350353 mizue-0.3.4/mizue/network/downloader/data/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/data/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/download_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/download_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/downloader_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/network/downloader/progress_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.350353 mizue-0.3.4/mizue/printer/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.350353 mizue-0.3.4/mizue/printer/grid/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/border_character_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/border_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/cell_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/column_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/grid/row_border_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/printer/terminal_colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.354353 mizue-0.3.4/mizue/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/progress/colorful_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/progress/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/progress/progress_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/progress/spinner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.354353 mizue-0.3.4/mizue/util/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/util/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/util/signal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/util/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-21 18:24:19.000000 mizue-0.3.4/mizue/util/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:24:38.346353 mizue-0.3.4/mizue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-21 18:24:38.000000 mizue-0.3.4/mizue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-21 18:24:38.000000 mizue-0.3.4/mizue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:24:38.000000 mizue-0.3.4/mizue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 18:24:38.000000 mizue-0.3.4/mizue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 18:24:38.000000 mizue-0.3.4/mizue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:24:38.354353 mizue-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-21 18:24:36.000000 mizue-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:19:38.131269 mizue-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-24 18:19:20.000000 mizue-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-24 18:19:38.131269 mizue-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-24 18:19:20.000000 mizue-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:19:38.127269 mizue-0.4.0/mizue/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:19:38.127269 mizue-0.4.0/mizue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/file/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:19:38.127269 mizue-0.4.0/mizue/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:19:38.127269 mizue-0.4.0/mizue/network/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/network/downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:19:38.127269 mizue-0.4.0/mizue/network/downloader/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/network/downloader/data/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/network/downloader/download_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/network/downloader/download_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/network/downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/network/downloader/downloader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/network/downloader/progress_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:19:38.127269 mizue-0.4.0/mizue/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:19:38.131269 mizue-0.4.0/mizue/printer/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/grid/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/grid/border_character_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/grid/border_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/grid/cell_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/grid/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/grid/column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/grid/row_border_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/printer/terminal_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:19:38.131269 mizue-0.4.0/mizue/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/progress/colorful_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/progress/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/progress/progress_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/progress/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:19:38.131269 mizue-0.4.0/mizue/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/util/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/util/signal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/util/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-24 18:19:20.000000 mizue-0.4.0/mizue/util/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:19:38.127269 mizue-0.4.0/mizue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-24 18:19:38.000000 mizue-0.4.0/mizue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-24 18:19:38.000000 mizue-0.4.0/mizue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 18:19:38.000000 mizue-0.4.0/mizue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-24 18:19:38.000000 mizue-0.4.0/mizue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 18:19:38.000000 mizue-0.4.0/mizue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 18:19:38.131269 mizue-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-24 18:19:36.000000 mizue-0.4.0/setup.py
```

### Comparing `mizue-0.3.4/LICENSE` & `mizue-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/PKG-INFO` & `mizue-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.3.4
+Version: 0.4.0
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mizue-0.3.4/README.md` & `mizue-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/file/fileutils.py` & `mizue-0.4.0/mizue/file/fileutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import os
 
 
 class FileUtils:
     @staticmethod
+    def get_files_of_type(path, file_type, recursive=False, fullpath=True):
+        filelist = FileUtils.list_files(path, recursive=recursive, fullpath=fullpath)
+        return [f for f in filelist if f.endswith(file_type)]
+
+    @staticmethod
     def get_readable_file_size(size: int, suffix: str = "B"):
         for unit in ['', 'K', 'M', 'G', 'T', 'P', 'E', 'Z']:
             if abs(size) < 1024.0:
                 return "%3.2f%s%s%s" % (size, " ", unit, suffix)
             size /= 1024.0
         return "%.1f%s%s%s" % (size, " ", 'Y', suffix)
```

### Comparing `mizue-0.3.4/mizue/network/downloader/data/colors.json` & `mizue-0.4.0/mizue/network/downloader/data/colors.json`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/network/downloader/download_event.py` & `mizue-0.4.0/mizue/network/downloader/download_event.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/network/downloader/downloader.py` & `mizue-0.4.0/mizue/network/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/network/downloader/downloader_tool.py` & `mizue-0.4.0/mizue/network/downloader/downloader_tool.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/printer/grid/border_character_codes.py` & `mizue-0.4.0/mizue/printer/grid/border_character_codes.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/printer/grid/column.py` & `mizue-0.4.0/mizue/printer/grid/column.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/printer/grid/grid.py` & `mizue-0.4.0/mizue/printer/grid/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,37 @@
 from .column import Column
 from .column_settings import ColumnSettings
 from .row_border_position import RowBorderPosition
 
 
 class Grid:
     def __init__(self, columns: list[ColumnSettings], data: list[list[str]]):
+        self._columns = []
         self.border_color = None
         self.border_style = BorderStyle.BASIC
         self.cell_renderer: Callable[[CellRendererArgs], str] = lambda args: Grid._get_default_cell_renderer(args)
-        self.columns = []
         self.data = data
-        self._prepare_columns(columns)
+        if len(columns) > 0:
+            self._prepare_columns(columns)
+
+    @property
+    def columns(self) -> list[Column]:
+        return self._columns
+
+    @columns.setter
+    def columns(self, value: list[ColumnSettings]) -> None:
+        self._prepare_columns(value)
+
+    def fill_screen(self):
+        terminal_width = Utility.get_terminal_width()
+        total_width = sum([column.width for column in self.columns]) + (4 * len(self.columns))
+        if total_width < terminal_width:
+            remaining_width = terminal_width - sum([column.width for column in self.columns]) - (4 * len(self.columns))
+            for column in self.columns:
+                column.width += int(remaining_width / len(self.columns))
 
     def print(self) -> None:
         """Print the grid"""
         print(self._buffer())
 
     def _buffer(self) -> str:
         buffer = [self._create_row_border(RowBorderPosition.TOP), os.linesep]
@@ -255,24 +272,17 @@
     def _prepare_columns(self, column_data: list[ColumnSettings]):
         columns: list[Column] = []
         for i, column_setting in enumerate(column_data):
             column = Column(settings=column_setting)
             column.index = i
             column.width = column_setting["width"] if "width" in column_setting else self._find_max_cell_width(column)
             columns.append(column)
-        self.columns = columns
+        self._columns = columns
         self._resize_columns_to_fit()
 
-    def _resize_columns_to_fit2(self):
-        terminal_width = Utility.get_terminal_width()
-        total_column_width = sum(column.width for column in self.columns)
-        if total_column_width > terminal_width:
-            for cx in range(0, len(self.columns)):
-                self.columns[cx].width = int((terminal_width * self.columns[cx].width) / total_column_width) - 4
-
     def _resize_columns_to_fit(self):
         terminal_width = Utility.get_terminal_width()
         new_column_width = int(terminal_width / len(self.columns))
         long_columns = [column for column in self.columns if column.width >= new_column_width]
 
         remaining_width = 0
         for column in self.columns:
```

### Comparing `mizue-0.3.4/mizue/printer/printer.py` & `mizue-0.4.0/mizue/printer/printer.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/progress/colorful_progress.py` & `mizue-0.4.0/mizue/progress/colorful_progress.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/progress/progress.py` & `mizue-0.4.0/mizue/progress/progress.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/progress/progress_renderer_args.py` & `mizue-0.4.0/mizue/progress/progress_renderer_args.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/progress/spinner.py` & `mizue-0.4.0/mizue/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/util/event_listener.py` & `mizue-0.4.0/mizue/util/event_listener.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/util/signal_handler.py` & `mizue-0.4.0/mizue/util/signal_handler.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue/util/utility.py` & `mizue-0.4.0/mizue/util/utility.py`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/mizue.egg-info/PKG-INFO` & `mizue-0.4.0/mizue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.3.4
+Version: 0.4.0
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mizue-0.3.4/mizue.egg-info/SOURCES.txt` & `mizue-0.4.0/mizue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizue-0.3.4/setup.py` & `mizue-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="mizue",
-    version="0.3.4",
+    version="0.4.0",
     description="A Python package for various utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Hoshilily",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
```

