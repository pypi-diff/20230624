# Comparing `tmp/tui_rsync-0.8.12.tar.gz` & `tmp/tui_rsync-0.8.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_rsync-0.8.12.tar", max compression
+gzip compressed data, was "tui_rsync-0.8.13.tar", max compression
```

## Comparing `tui_rsync-0.8.12.tar` & `tui_rsync-0.8.13.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      389 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/README.rst
--rw-r--r--   0        0        0      725 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/__init__.py
--rw-r--r--   0        0        0      163 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/__init__.py
--rw-r--r--   0        0        0     1889 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/cli.py
--rw-r--r--   0        0        0       47 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/groups/__init__.py
--rw-r--r--   0        0        0     1814 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/groups/group_prompt.py
--rw-r--r--   0        0        0     2432 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/groups/group_remove.py
--rw-r--r--   0        0        0     3600 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/groups/group_update.py
--rw-r--r--   0        0        0     2644 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/groups/groups.py
--rw-r--r--   0        0        0     3018 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/label_prompt.py
--rw-r--r--   0        0        0     2110 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/path_prompt.py
--rw-r--r--   0        0        0     2000 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/rsync.py
--rw-r--r--   0        0        0       47 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/source/__init__.py
--rw-r--r--   0        0        0     3228 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/source/source.py
--rw-r--r--   0        0        0     2414 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/source/source_remove.py
--rw-r--r--   0        0        0     4146 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/source/source_update.py
--rw-r--r--   0        0        0     4311 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/cli/sync.py
--rw-r--r--   0        0        0       38 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/config/__init__.py
--rw-r--r--   0        0        0     2211 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/config/app.py
--rw-r--r--   0        0        0      156 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/main.py
--rw-r--r--   0        0        0      230 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/models/__init__.py
--rw-r--r--   0        0        0     6775 2023-06-23 16:17:38.478660 tui_rsync-0.8.12/tui_rsync/models/models.py
--rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 tui_rsync-0.8.12/setup.py
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 tui_rsync-0.8.12/PKG-INFO
+-rw-r--r--   0        0        0      389 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/README.rst
+-rw-r--r--   0        0        0      725 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/__init__.py
+-rw-r--r--   0        0        0     1889 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/cli.py
+-rw-r--r--   0        0        0       47 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/groups/__init__.py
+-rw-r--r--   0        0        0     1814 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/groups/group_prompt.py
+-rw-r--r--   0        0        0     2432 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/groups/group_remove.py
+-rw-r--r--   0        0        0     3600 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/groups/group_update.py
+-rw-r--r--   0        0        0     2644 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/groups/groups.py
+-rw-r--r--   0        0        0     3018 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/label_prompt.py
+-rw-r--r--   0        0        0     2110 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/path_prompt.py
+-rw-r--r--   0        0        0     2000 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/rsync.py
+-rw-r--r--   0        0        0       47 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/source/__init__.py
+-rw-r--r--   0        0        0     3349 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/source/source.py
+-rw-r--r--   0        0        0     2414 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/source/source_remove.py
+-rw-r--r--   0        0        0     2363 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/source/source_show.py
+-rw-r--r--   0        0        0     4146 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/source/source_update.py
+-rw-r--r--   0        0        0     4311 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/cli/sync.py
+-rw-r--r--   0        0        0       38 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/config/__init__.py
+-rw-r--r--   0        0        0     2211 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/config/app.py
+-rw-r--r--   0        0        0      156 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/main.py
+-rw-r--r--   0        0        0      230 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/models/__init__.py
+-rw-r--r--   0        0        0     7126 2023-06-24 14:31:52.221086 tui_rsync-0.8.13/tui_rsync/models/models.py
+-rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 tui_rsync-0.8.13/setup.py
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 tui_rsync-0.8.13/PKG-INFO
```

### Comparing `tui_rsync-0.8.12/pyproject.toml` & `tui_rsync-0.8.13/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tui-rsync"
-version = "0.8.12"
+version = "0.8.13"
 description = "tui-rsync will help you to manage yours backups."
 authors = ["Kostiantyn Klochko <kostya_klochko@ukr.net>"]
 readme = "README.rst"
 license = "GPL-3.0-or-later"
 packages = [{include = "tui_rsync"}]
 repository = "https://gitlab.com/KKlochko/tui-rsync"
 keywords = ["tui", "cli", "rsync", "backup"]
```

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/cli.py` & `tui_rsync-0.8.13/tui_rsync/cli/cli.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/groups/group_prompt.py` & `tui_rsync-0.8.13/tui_rsync/cli/groups/group_prompt.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/groups/group_remove.py` & `tui_rsync-0.8.13/tui_rsync/cli/groups/group_remove.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/groups/group_update.py` & `tui_rsync-0.8.13/tui_rsync/cli/groups/group_update.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/groups/groups.py` & `tui_rsync-0.8.13/tui_rsync/cli/groups/groups.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/label_prompt.py` & `tui_rsync-0.8.13/tui_rsync/cli/label_prompt.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/path_prompt.py` & `tui_rsync-0.8.13/tui_rsync/cli/path_prompt.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/rsync.py` & `tui_rsync-0.8.13/tui_rsync/cli/rsync.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/source/source.py` & `tui_rsync-0.8.13/tui_rsync/cli/source/source.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,19 +20,21 @@
 from rich.console import Console
 from rich.prompt import Prompt
 from typing import List, Optional
 import typer
 
 from tui_rsync.models.models import Source, Destination, SyncCommand, Path
 from tui_rsync.cli.label_prompt import LabelPrompt
+from tui_rsync.cli.source.source_show import source_show
 from tui_rsync.cli.source.source_update import source_update
 from tui_rsync.cli.source.source_remove import source_remove
 
 console = Console()
 source = typer.Typer()
+source.add_typer(source_show, name="show", help="Show sources")
 source.add_typer(source_update, name="update", help="Update sources")
 source.add_typer(source_remove, name="remove", help="Remove sources")
 
 @source.command()
 def add(
     label: str = typer.Option(
         None, "--label", "-l",
```

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/source/source_remove.py` & `tui_rsync-0.8.13/tui_rsync/cli/source/source_remove.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/source/source_update.py` & `tui_rsync-0.8.13/tui_rsync/cli/source/source_update.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/cli/sync.py` & `tui_rsync-0.8.13/tui_rsync/cli/sync.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/config/app.py` & `tui_rsync-0.8.13/tui_rsync/config/app.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.12/tui_rsync/models/models.py` & `tui_rsync-0.8.13/tui_rsync/models/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,26 @@
         self.save()
 
     def __str__(self) -> str:
         return f"{self.label}"
 
     def __repr__(self) -> str:
         return f"{self.label}"
+
+    def show_format(self) -> str:
+        output = f"[b]label:[/] {self.label}\n" \
+                 f"[b]source:[/] {self.source.path}\n" \
+                 f"[b]args:[/] {self.args}\n" \
+                 f"[b]destionations:[/] \n"
+
+        for destination in self.destinations:
+            output+=f"\t{destination.path}\n"
+
+        return output
+
 class Destination(BaseModel):
     source = ForeignKeyField(Source, backref='destinations')
     path = ForeignKeyField(Path)
 
     def __str__(self) -> str:
         return f"{self.path}"
```

### Comparing `tui_rsync-0.8.12/setup.py` & `tui_rsync-0.8.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['tui-rsync = tui_rsync.main:main']}
 
 setup_kwargs = {
     'name': 'tui-rsync',
-    'version': '0.8.12',
+    'version': '0.8.13',
     'description': 'tui-rsync will help you to manage yours backups.',
     'long_description': 'tui-rsync\n=========\n\n|PyPI version|\n\ntui-rsync is the application that will help you to manage yours backups.\nIt uses rsync for syncing backups.\n\nDependencies\n============\n\n-  rsync\n-  fzf\n\nAuthor\n======\n\nKostiantyn Klochko (c) 2023\n\nLicense\n=======\n\nUnder GNU GPL v3 license\n\n.. |PyPI version| image:: https://badge.fury.io/py/tui-rsync.svg\n   :target: https://badge.fury.io/py/tui-rsync\n',
     'author': 'Kostiantyn Klochko',
     'author_email': 'kostya_klochko@ukr.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/KKlochko/tui-rsync',
```

### Comparing `tui_rsync-0.8.12/PKG-INFO` & `tui_rsync-0.8.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui-rsync
-Version: 0.8.12
+Version: 0.8.13
 Summary: tui-rsync will help you to manage yours backups.
 Home-page: https://gitlab.com/KKlochko/tui-rsync
 License: GPL-3.0-or-later
 Keywords: tui,cli,rsync,backup
 Author: Kostiantyn Klochko
 Author-email: kostya_klochko@ukr.net
 Requires-Python: >=3.10,<4.0
```

