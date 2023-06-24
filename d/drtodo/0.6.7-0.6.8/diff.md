# Comparing `tmp/drtodo-0.6.7.tar.gz` & `tmp/drtodo-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drtodo-0.6.7.tar", max compression
+gzip compressed data, was "drtodo-0.6.8.tar", max compression
```

## Comparing `drtodo-0.6.7.tar` & `drtodo-0.6.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-06-24 01:24:47.795187 drtodo-0.6.7/LICENSE
--rw-r--r--   0        0        0    14071 2023-06-24 01:25:08.695419 drtodo-0.6.7/drtodo/README.md
--rw-r--r--   0        0        0      224 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/__init__.py
--rw-r--r--   0        0        0       46 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/__main__.py
--rw-r--r--   0        0        0     4385 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/backup_command.py
--rw-r--r--   0        0        0    12999 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/main.py
--rw-r--r--   0        0        0      419 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/man/README.md
--rw-r--r--   0        0        0        0 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/man/__init__.py
--rw-r--r--   0        0        0     3023 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/man/config.md
--rw-r--r--   0        0        0     2577 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/man/intro.md
--rw-r--r--   0        0        0      874 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/man/mdfiles.md
--rw-r--r--   0        0        0     1423 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/man_command.py
--rw-r--r--   0        0        0     6776 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/mdparser.py
--rw-r--r--   0        0        0     1406 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/mistuneplugin.py
--rw-r--r--   0        0        0      719 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/rich_display.py
--rw-r--r--   0        0        0     7354 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/settings.py
--rw-r--r--   0        0        0     2771 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/taskitems.py
--rw-r--r--   0        0        0      256 2023-06-24 01:24:47.795187 drtodo-0.6.7/drtodo/util.py
--rw-r--r--   0        0        0      830 2023-06-24 01:25:06.027391 drtodo-0.6.7/pyproject.toml
--rw-r--r--   0        0        0    14965 1970-01-01 00:00:00.000000 drtodo-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-24 18:23:51.425433 drtodo-0.6.8/LICENSE
+-rw-r--r--   0        0        0    15648 2023-06-24 18:24:12.709692 drtodo-0.6.8/drtodo/README.md
+-rw-r--r--   0        0        0      224 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/__init__.py
+-rw-r--r--   0        0        0       46 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/__main__.py
+-rw-r--r--   0        0        0     4421 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/backup_command.py
+-rw-r--r--   0        0        0    15375 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/main.py
+-rw-r--r--   0        0        0      419 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/man/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/man/__init__.py
+-rw-r--r--   0        0        0     3023 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/man/config.md
+-rw-r--r--   0        0        0     2577 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/man/intro.md
+-rw-r--r--   0        0        0      874 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/man/mdfiles.md
+-rw-r--r--   0        0        0     1423 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/man_command.py
+-rw-r--r--   0        0        0     7308 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/mdparser.py
+-rw-r--r--   0        0        0     1406 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/mistuneplugin.py
+-rw-r--r--   0        0        0      719 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/rich_display.py
+-rw-r--r--   0        0        0     7354 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/settings.py
+-rw-r--r--   0        0        0     3297 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/taskitems.py
+-rw-r--r--   0        0        0      256 2023-06-24 18:23:51.425433 drtodo-0.6.8/drtodo/util.py
+-rw-r--r--   0        0        0      830 2023-06-24 18:24:09.681656 drtodo-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0    16542 1970-01-01 00:00:00.000000 drtodo-0.6.8/PKG-INFO
```

### Comparing `drtodo-0.6.7/LICENSE` & `drtodo-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.7/drtodo/README.md` & `drtodo-0.6.8/drtodo/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 
 ```console
 $ DrToDo [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
-* `-v, --verbose`: Verbose output
+* `-v, --verbose / -q, --quiet`: Verbose or quiet output  [default: quiet]
 * `--mdfile PATH`: Markdown file to use for todo list  [default: TODO.md]
 * `--section TEXT`: Section name in markdown file to use for todo list, with optional heading level, e.g. '## TODO'
 * `--reverse-order / --normal-order`: Whether todo items should be in reverse order (latest first)  [default: normal-order]
 * `-V, --version`: Show version and exit
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
@@ -273,14 +273,16 @@
 * `dbg`: List configuration, settings, version and...
 * `debug`: List configuration, settings, version and...
 * `done`: Mark one or more todo items as done
 * `init`: Initialize DrTodo folder and files
 * `list`: List todo items in the list
 * `ls`: List todo items in the list
 * `man`: Show detailed help and context for...
+* `remove`: Remove/delete todo items from the list
+* `rm`: Remove/delete todo items from the list
 * `show`: Show markdown file(s) with rich rendering.
 * `undone`: Mark one or more todo items as NOT done...
 
 ## `DrToDo add`
 
 Add a new todo item to the list
 
@@ -320,14 +322,15 @@
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `list`: Lists any existing backup files
 * `ls`: Lists any existing backup files
 * `restore`: Rolls back backup files by one (3 levels...
+* `rollback`: Rolls back backup files by one (3 levels...
 
 ### `DrToDo backup list`
 
 Lists any existing backup files
 
 **Usage**:
 
@@ -363,14 +366,28 @@
 $ DrToDo backup restore [OPTIONS]
 ```
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
+### `DrToDo backup rollback`
+
+Rolls back backup files by one (3 levels of backup are kept by default).
+
+**Usage**:
+
+```console
+$ DrToDo backup rollback [OPTIONS]
+```
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
 ## `DrToDo dbg`
 
 List configuration, settings, version and other debug info.
 
 **Usage**:
 
 ```console
@@ -565,14 +582,60 @@
 $ DrToDo man settings [OPTIONS]
 ```
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
+## `DrToDo remove`
+
+Remove/delete todo items from the list
+
+**Usage**:
+
+```console
+$ DrToDo remove [OPTIONS] [SPEC]
+```
+
+**Arguments**:
+
+* `[SPEC]`: ID, index, range or regular expression to match item text
+
+**Options**:
+
+* `-i, --id TEXT`: ID of the item to remove
+* `-n, --index INTEGER`: Index of the item to remove
+* `-r, --range TEXT`: Range of item indices to remove, e.g, 2:5, 2:, :5
+* `-m, --match TEXT`: Regular expression to match item text
+* `-G, --global`: Remove from global todo list, even if current folder is under a git repo
+* `--help`: Show this message and exit.
+
+## `DrToDo rm`
+
+Remove/delete todo items from the list
+
+**Usage**:
+
+```console
+$ DrToDo rm [OPTIONS] [SPEC]
+```
+
+**Arguments**:
+
+* `[SPEC]`: ID, index, range or regular expression to match item text
+
+**Options**:
+
+* `-i, --id TEXT`: ID of the item to remove
+* `-n, --index INTEGER`: Index of the item to remove
+* `-r, --range TEXT`: Range of item indices to remove, e.g, 2:5, 2:, :5
+* `-m, --match TEXT`: Regular expression to match item text
+* `-G, --global`: Remove from global todo list, even if current folder is under a git repo
+* `--help`: Show this message and exit.
+
 ## `DrToDo show`
 
 Show markdown file(s) with rich rendering. Defaults to the active, configured files.
 
 **Usage**:
 
 ```console
```

### Comparing `drtodo-0.6.7/drtodo/backup_command.py` & `drtodo-0.6.8/drtodo/backup_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
             for i, bakfile in scan_backups(location):
                 _print_file(-i, bakfile)
             _print_file('now', location)
             break   # only the first valid location is processed
 
 
 @app.command()
+@app.command_alias(name="rollback")
 def restore():
     """
     Rolls back backup files by one (3 levels of backup are kept by default).
     """
     locations = [globals.global_todofile] if force_global else [globals.global_todofile, globals.local_todofile]
     for location in locations:
         if location and location.exists():
```

### Comparing `drtodo-0.6.7/drtodo/main.py` & `drtodo-0.6.8/drtodo/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 app = Typer(
     no_args_is_help=True,
     rich_markup_mode="markdown",
     help=f"**{constants.appname}, MD**: *a straightforward todo list manager for markdown files in git repos.*",
     epilog=f"DrTodo can manage items in a global todo list ({globals.global_todofile_pretty})"
     f" and in a local todo list ({globals.local_todofile_pretty or 'if the current folder is under a git repo'})."
     f" Settings are read from config files and env variables (see *todo man config*).",
-    rich_help_panel="Integration")
+)
 
 
 def version_string() -> str:
     return f"{constants.appname} v{constants.version}"
 
 
 def ensure_appdir(may_create: bool = False) -> None:
@@ -73,45 +73,51 @@
         mdtext_part.style = "dim"
     if strike:
         mdtext_part.style = "strike"
     console().print(index_part + hash_part + checkmark_part, mdtext_part, end='')
 
 
 @app.command(name="list")
-@app.command(name="ls", hidden=True)
+@app.command_alias(name="ls")
 def list_command(
     spec: str = typer.Argument(None, help="ID, index, range or regular expression to match item text"),
     id: str = typer.Option(None, "--id", "-i", help="ID of the item to list"),
     index: int = typer.Option(None, "--index", "-n", help="Index of the item to list"),
     range: str = typer.Option(None, "--range", "-r", help="Range of item indices to list, e.g, 2:5, 2:, :5"),
     match: str = typer.Option(None, "--match", "-m", help="Regular expression to match item text"),
     # TODO: add more filter options, done/undone, priority, due, owner, etc.
 ):
     """
     List todo items in the list
     """
+
+    def listfromfile(todofile: Path):
+        if todofile and todofile.exists():
+            console().print(f"[header]{make_pretty_path(todofile)}[text]")
+            todo = TodoListParser()
+            todo.parse(todofile)
+            try:
+                items = taskitems.create_iterator(todo.items, omit_means_all=True,
+                                                  spec=spec, id=id, index=index, range=range, match=match)
+            except ValueError as e:
+                error_console().print(f"error: {e}")
+                raise typer.Exit(2)
+
+            for item in items:
+                print_todo_item(item)
+
     if globals.global_todofile and globals.global_todofile.exists():
-        console().print(f"[header]{globals.global_todofile_pretty}[text]")
-        todo = TodoListParser()
-        todo.parse(globals.global_todofile)
-        for item in taskitems.task_iterator(todo.items, omit_means_all=True,
-                                            spec=spec, id=id, index=index, range=range, match=match):
-            print_todo_item(item)
+        listfromfile(globals.global_todofile)
 
     if globals.local_todofile and globals.local_todofile.exists():
-        console().print(f"[header]{globals.local_todofile_pretty}[text]")
-        todo = TodoListParser()
-        todo.parse(globals.local_todofile)
-        for item in taskitems.task_iterator(todo.items, omit_means_all=True,
-                                            spec=spec, id=id, index=index, range=range, match=match):
-            print_todo_item(item)
+        listfromfile(globals.local_todofile)
 
 
 @app.command(name="debug")
-@app.command(name="dbg", hidden=True)
+@app.command_alias(name="dbg")
 def debug_command():
     """
     List configuration, settings, version and other debug info.
     """
     console().print(f"{version_string()}", highlight=False)
 
     d = constants.__dict__ | dict(settings) | globals.__dict__
@@ -126,15 +132,14 @@
         todo.add_item_after(add=todo_item, after=todo.items[-1])
         backup_command.save_with_backups(todofile_path, todo)
     else:
         error_console().print(f"Cannot add item to {todofile_path} because it does not exist")
         raise typer.Exit(2)
 
 
-# add [--priority <priority>] [--due <due>] [--owner <owner>] [--done] <item description>
 @app.command()
 def add(
     description: str,
     priority: int = typer.Option(None, "--priority", "-p"),
     due: str = typer.Option(None, "--due", "-d", help="Due date in any format"),
     owner: str = typer.Option(None, "--owner", "-o", help="Owner userid or name"),
     done: bool = typer.Option(False, "--done", "-D", help="Add item marked as done"),
@@ -146,51 +151,121 @@
     """
     duestr = f" due:{due}" if due else ""
     ownerstr = f" @{owner}" if owner else ""
     prioritystr = f" P{priority}" if priority else ""
     itemstr = f"{prioritystr}{ownerstr}{duestr} {description}".strip()
     todo_item = TaskListTraverser.create_item(itemstr, index=0, checked=done)
     if not global_todo and globals.local_todofile and globals.local_todofile.exists():
-        console().print(f"[header]{globals.local_todofile_pretty}[text]")
+        if (settings.verbose):
+            console().print(f"[header]{globals.local_todofile_pretty}[text]")
         _add_item(todo_item, globals.local_todofile)
     else:
         assert globals.global_todofile
-        console().print(f"[header]{globals.global_todofile_pretty}[text]")
+        if (settings.verbose):
+            console().print(f"[header]{globals.global_todofile_pretty}[text]")
         _add_item(todo_item, globals.global_todofile)
-    print_todo_item(todo_item)
+    if (settings.verbose):
+        print_todo_item(todo_item)
+
+
+@app.command(name="remove")
+@app.command_alias(name="rm")
+def remove_command(
+    spec: str = typer.Argument(None, help="ID, index, range or regular expression to match item text"),
+    id: str = typer.Option(None, "--id", "-i", help="ID of the item to remove"),
+    index: int = typer.Option(None, "--index", "-n", help="Index of the item to remove"),
+    range: str = typer.Option(None, "--range", "-r", help="Range of item indices to remove, e.g, 2:5, 2:, :5"),
+    match: str = typer.Option(None, "--match", "-m", help="Regular expression to match item text"),
+    # TODO: add more filter options, done/undone, priority, due, owner, etc.
+    global_todo: bool = typer.Option(False, "--global", "-G",
+                                     help="Remove from global todo list, even if current folder is under a git repo"),
+):
+    """
+    Remove/delete todo items from the list
+    """
+
+    def removefromfile(todo_file: Path) -> int:
+        count = 0
+        if todo_file and todo_file.exists():
+            if (settings.verbose):
+                console().print(f"[header]{make_pretty_path(todo_file)}[text]")
+            todo = TodoListParser()
+            todo.parse(todo_file)
+            try:
+                items = taskitems.create_iterator(todo.items, omit_means_all=False,
+                                                  spec=spec, id=id, index=index, range=range, match=match)
+            except ValueError as e:
+                error_console().print(f"error: {e}")
+                raise typer.Exit(2)
+
+            try:
+                # we gather then commit to remove from list we are iterating over
+                to_remove = []
+                for item in items:
+                    to_remove.append(item)
+
+                count = len(to_remove)
+                while to_remove:
+                    item = to_remove.pop(0)
+                    todo.remove_item(item)
+                    if (settings.verbose):
+                        print_todo_item(item)
+            except Exception as e:
+                error_console().print(f"no items removed: {e}")
+                raise typer.Exit(2)
+            finally:
+                backup_command.save_with_backups(todo_file, todo)
+        return count
+
+    if not global_todo and globals.local_todofile and globals.local_todofile.exists():
+        # remove from local todo list
+        removed = removefromfile(globals.local_todofile)
+    elif globals.global_todofile and globals.global_todofile.exists():
+        # remove from global todo list
+        removed = removefromfile(globals.global_todofile)
+    else:
+        removed = 0
+
+    if removed == 0:
+        error_console().print("nothing to remove")
+
 
 def _done_undone_marker(done: bool, spec, id, index, range, match, all):
     """
     Mark one or more todo items as done or undone.
     """
     # ensure exactly one of spec, id, index, match or all is not None
     if sum([spec is not None, id is not None, index is not None, range is not None, match is not None, all]) != 1:
         raise typer.BadParameter("Exactly one of --id, --index, --range, --match or --all must be provided")
 
-    if globals.global_todofile and globals.global_todofile.exists():
-        console().print(f"[header]{globals.global_todofile}[text] changes:")
-        todo = TodoListParser()
-        todo.parse(globals.global_todofile)
-        items = taskitems.task_iterator(todo.items, id=id, index=index, range=range, match=match) if not all else todo.items
-        for item in items:
-            item['checked'] = done
-            print_todo_item(item)
-        # write back to file
-        backup_command.save_with_backups(globals.global_todofile, todo)
+    def doneundonefromfile(todo_file: Optional[Path]) -> int:
+        count = 0
+        if todo_file and todo_file.exists():
+            if (settings.verbose):
+                console().print(f"[header]{make_pretty_path(todo_file)}[text] changes:")
+            todo = TodoListParser()
+            todo.parse(todo_file)
+            try:
+                items = taskitems.create_iterator(todo.items, omit_means_all=False,
+                                                  spec=spec, id=id, index=index, range=range, match=match) if not all else todo.items
+            except ValueError as e:
+                error_console().print(f"error: {e}")
+                raise typer.Exit(2)
+
+            for item in items:
+                item['checked'] = done
+                if (settings.verbose):
+                    print_todo_item(item)
+                count += 1
+            # write back to file
+            backup_command.save_with_backups(todo_file, todo)
+        return count
 
-    if globals.local_todofile and globals.local_todofile.exists():
-        console().print(f"[header]{globals.local_todofile}[text] changes:")
-        todo = TodoListParser()
-        todo.parse(globals.local_todofile)
-        items = taskitems.task_iterator(todo.items, id=id, index=index, range=range, match=match) if not all else todo.items
-        for item in items:
-            item['checked'] = done
-            print_todo_item(item)
-        # write back to file
-        backup_command.save_with_backups(globals.local_todofile, todo)
+    doneundonefromfile(globals.global_todofile)
+    doneundonefromfile(globals.local_todofile)
 
 
 # done [--id <id> | --index <index> | --all | --match <regular expression> | <specification>]
 # (exactly one option must be provided)
 @app.command()
 def done(
     spec: str = typer.Argument(None, help="ID, index, range or regular expression to match item text"),
@@ -228,15 +303,15 @@
          raw: bool = typer.Option(False, "--raw", help="Print the raw markdown man content")
         ):
     """
     Show markdown file(s) with rich rendering. Defaults to the active, configured files.
     """
     md_print = util.print_md_as_raw if raw else util.print_md_pretty
     if not files:
-        files = [globals.global_todofile, globals.local_todofile]
+        files = [x for x in [globals.global_todofile, globals.local_todofile] if x]
     for file in files:
         if file and file.exists():
             if len(files) > 1:
                 console().print(f"[header]{make_pretty_path(file)}[text]")
             with file.open() as f:
                 mdstring = f.read()
                 md_print(mdstring)
@@ -256,46 +331,43 @@
 
 def _version_callback(value: bool) -> None:
     if value:
         console().print(f"{version_string()}", highlight=False)
         raise typer.Exit()
 
 
-panel_GLOBAL = "Global Options"
 panel_FILESELECTION = "File Selection Options"
 
 
 # Typer callback handles global options like --mdfile and --verbose
 @app.callback()
 def main_callback(
     # settings_file: Optional[Path] = typer.Option(constants.appdir, "--settings", "-S", help="Settings file to use",
     #                                              rich_help_panel=panel_GLOBAL),
-    verbose: Optional[bool] = typer.Option(settings.verbose, "--verbose", "-v", help="Verbose output",
-                                           rich_help_panel=panel_GLOBAL),
-    mdfile: Optional[Path] = typer.Option(settings.mdfile, help="Markdown file to use for todo list",
-                                          rich_help_panel=panel_FILESELECTION),
-    section: Optional[str] = typer.Option(settings.section,
-                                          help="Section name in markdown file to use for todo list, with optional "\
-                                          "heading level, e.g. '## TODO'",
-                                          rich_help_panel=panel_FILESELECTION),
-    reverse_order: Optional[bool] = typer.Option(settings.reverse_order, "--reverse-order/--normal-order",
-                                                 help="Whether todo items should be in reverse order (latest first)",
-                                                 rich_help_panel=panel_FILESELECTION),
-    version: Optional[bool] = typer.Option(False, "--version", "-V", help="Show version and exit",
-                                           callback=_version_callback, is_eager=True, rich_help_panel=panel_GLOBAL),
+    verbose: bool = typer.Option(settings.verbose, "--verbose/--quiet", "-v/-q", help="Verbose or quiet output"),
+    mdfile: Path = typer.Option(settings.mdfile, help="Markdown file to use for todo list",
+                                rich_help_panel=panel_FILESELECTION),
+    section: str = typer.Option(settings.section,
+                                help="Section name in markdown file to use for todo list, with optional "\
+                                "heading level, e.g. '## TODO'",
+                                rich_help_panel=panel_FILESELECTION),
+    reverse_order: bool = typer.Option(settings.reverse_order, "--reverse-order/--normal-order",
+                                       help="Whether todo items should be in reverse order (latest first)",
+                                       rich_help_panel=panel_FILESELECTION),
+    version: bool = typer.Option(False, "--version", "-V", help="Show version and exit",
+                                 callback=_version_callback, is_eager=True),
 ):
-    settings.mdfile = mdfile
+    settings.mdfile = str(mdfile)
     settings.verbose = verbose
     settings.section = section
     settings.reverse_order = reverse_order
 
     # BUG: this is called even when the command is init, so it prints a warning about the appdir not existing
     ensure_appdir()
 
 
 def main(*args, **kwargs):
-    # typer_aliases(app=app)
     app(*args, **kwargs)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `drtodo-0.6.7/drtodo/man/config.md` & `drtodo-0.6.8/drtodo/man/config.md`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.7/drtodo/man/intro.md` & `drtodo-0.6.8/drtodo/man/intro.md`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.7/drtodo/man/mdfiles.md` & `drtodo-0.6.8/drtodo/man/mdfiles.md`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.7/drtodo/man_command.py` & `drtodo-0.6.8/drtodo/man_command.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.7/drtodo/mdparser.py` & `drtodo-0.6.8/drtodo/mdparser.py`

 * *Files 17% similar despite different names*

```diff
@@ -159,8 +159,20 @@
             # overwrite the children as a simple text token
             token['children'][0]['children'] = [{'type': 'text', 'raw': rawtext}]
 
     def write(self, pathname: Path):
         self._update_md_from_items()
         mdtext = self.markdownparser.render_state(self.state)
         with open(pathname, 'w') as f:
-            f.write(mdtext)
+            f.write(str(mdtext))
+
+    def remove_item(self, item: dict):
+        """Remove the given item from the items and state"""
+        # first find the index of the 'after' token in the parent list. if it fails we don't mess with the state
+        assert item['parent']
+        relative_index = item['parent'].index(item['token'])
+        assert relative_index >= 0
+        self.items.remove(item)
+        del item['parent'][relative_index]
+        # reindex all the items now
+        for i, item in enumerate(self.items):
+            item['index'] = i
```

### Comparing `drtodo-0.6.7/drtodo/mistuneplugin.py` & `drtodo-0.6.8/drtodo/mistuneplugin.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.7/drtodo/rich_display.py` & `drtodo-0.6.8/drtodo/rich_display.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.7/drtodo/settings.py` & `drtodo-0.6.8/drtodo/settings.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.7/drtodo/taskitems.py` & `drtodo-0.6.8/drtodo/taskitems.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,57 @@
 import re
-from typing import Optional, Union
+from typing import Generator, Optional, Union
 
 
 def parse_slice(s: str) -> slice:
     """
     parses a slice string like '1:3' and returns a tuple of (start, end) indexes.
     """
     split = s.split(':')
     if len(split) == 1:
         raise ValueError('slice must have at least one colon')
     return slice(*map(lambda x: int(x.strip()) if x.strip() else None, split))
 
 
 # iterator to traverse tasks that match a spec, id, index or re match (or all)
-def task_iterator(items: list, *,
-                  spec: Optional[Union[int, str]] = None,
-                  id: Optional[int] = None,
-                  index: Optional[int] = None,
-                  range: Optional[str] = None,
-                  match: Optional[str] = None,
-                  done: Optional[bool] = None,
-                  omit_means_all: bool = False
-):
+def create_iterator(items: list, *,
+                    spec: Optional[str] = None,
+                    id: Optional[str] = None,
+                    index: Optional[int] = None,
+                    range: Optional[Union[str, slice, range]] = None,
+                    match: Optional[str] = None,
+                    done: Optional[bool] = None,
+                    omit_means_all: bool = False
+) -> Generator:
     """
-    iterates through all tasks that match the given criteria:
+    returns an iterable that iterates through all tasks that match the given criteria:
     - spec: a string that can be an index, an ID or a regular expression
     - id: a task ID (partial hexadecimal hash)
     - index: a task index
     - range: a range of task indexes (e.g. 1:3, can use negative indexes from end as well)
     - match: a regular expression to match against the task text
     - done: whether to match only done tasks or only tasks not done
+    use as follows:
+
+    ```python
+    for item in create_iterator(items, spec='1:3'):
+        ...
+    ```
+
+    or
+
+    ```python
+    try:
+        iterator = create_iterator(items, spec='1:3')
+    except ValueError as e:
+        print(e)
+    else:
+        for item in iterator:
+            ...
+    ```
     """
     if spec is not None:
         # heuristics:
         # if spec has a single : in it, assume it's a range
         # if spec is a small integer, assume it's a positive index
         # if spec is a a pure hex string assume it's an ID
         # otherwise assume it's a regular expression
@@ -46,29 +64,33 @@
                     raise ValueError
             except ValueError:
                 if re.match(r'^[0-9a-f]+$', spec):
                     id = spec
                 else:
                     match = spec
 
-    if not omit_means_all and sum(spec is None, id is None, index is None, range is None, match is None, done is None) == 0:
+    if not omit_means_all and sum([spec is not None, id is not None, index is not None,
+                                   range is not None, match is not None, done is not None]) == 0:
         raise ValueError('no task selection criteria given')
 
     if isinstance(range, str):
         range = parse_slice(range)
 
     if isinstance(range, slice):
         import builtins
         range = builtins.range(*range.indices(len(items)))
 
-    for item in items:
-        if done is not None and item['checked'] != done:
-            continue
-        elif id is not None and not item['id'].startswith(id):
-            continue
-        elif index is not None and item['index'] != index:
-            continue
-        elif range is not None and item['index'] not in range:
-            continue
-        elif match is not None and not re.search(match, item['text']):
-            continue
-        yield item
+    def wrapped():
+        for item in items:
+            if done is not None and item['checked'] != done:
+                continue
+            elif id is not None and not item['id'].startswith(id):
+                continue
+            elif index is not None and item['index'] != index:
+                continue
+            elif range is not None and item['index'] not in range:
+                continue
+            elif match is not None and not re.search(match, item['text']):
+                continue
+            yield item
+
+    return wrapped()
```

### Comparing `drtodo-0.6.7/pyproject.toml` & `drtodo-0.6.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DrTodo"
-version = "0.6.7"
+version = "0.6.8"
 description = "DrTodo, MD: todo list manager using markdown files and git"
 authors = ["exilium <info@exilium.com>"]
 readme = "drtodo/README.md"
 license = "MIT"
 repository = "https://github.com/exilium-com/DrTodo"
 keywords = ["utilities", "todo", "markdown"]
```

### Comparing `drtodo-0.6.7/PKG-INFO` & `drtodo-0.6.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drtodo
-Version: 0.6.7
+Version: 0.6.8
 Summary: DrTodo, MD: todo list manager using markdown files and git
 Home-page: https://github.com/exilium-com/DrTodo
 License: MIT
 Keywords: utilities,todo,markdown
 Author: exilium
 Author-email: info@exilium.com
 Requires-Python: >=3.9,<4.0
@@ -276,15 +276,15 @@
 
 ```console
 $ DrToDo [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
-* `-v, --verbose`: Verbose output
+* `-v, --verbose / -q, --quiet`: Verbose or quiet output  [default: quiet]
 * `--mdfile PATH`: Markdown file to use for todo list  [default: TODO.md]
 * `--section TEXT`: Section name in markdown file to use for todo list, with optional heading level, e.g. '## TODO'
 * `--reverse-order / --normal-order`: Whether todo items should be in reverse order (latest first)  [default: normal-order]
 * `-V, --version`: Show version and exit
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
@@ -298,14 +298,16 @@
 * `dbg`: List configuration, settings, version and...
 * `debug`: List configuration, settings, version and...
 * `done`: Mark one or more todo items as done
 * `init`: Initialize DrTodo folder and files
 * `list`: List todo items in the list
 * `ls`: List todo items in the list
 * `man`: Show detailed help and context for...
+* `remove`: Remove/delete todo items from the list
+* `rm`: Remove/delete todo items from the list
 * `show`: Show markdown file(s) with rich rendering.
 * `undone`: Mark one or more todo items as NOT done...
 
 ## `DrToDo add`
 
 Add a new todo item to the list
 
@@ -345,14 +347,15 @@
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `list`: Lists any existing backup files
 * `ls`: Lists any existing backup files
 * `restore`: Rolls back backup files by one (3 levels...
+* `rollback`: Rolls back backup files by one (3 levels...
 
 ### `DrToDo backup list`
 
 Lists any existing backup files
 
 **Usage**:
 
@@ -388,14 +391,28 @@
 $ DrToDo backup restore [OPTIONS]
 ```
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
+### `DrToDo backup rollback`
+
+Rolls back backup files by one (3 levels of backup are kept by default).
+
+**Usage**:
+
+```console
+$ DrToDo backup rollback [OPTIONS]
+```
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
 ## `DrToDo dbg`
 
 List configuration, settings, version and other debug info.
 
 **Usage**:
 
 ```console
@@ -590,14 +607,60 @@
 $ DrToDo man settings [OPTIONS]
 ```
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
+## `DrToDo remove`
+
+Remove/delete todo items from the list
+
+**Usage**:
+
+```console
+$ DrToDo remove [OPTIONS] [SPEC]
+```
+
+**Arguments**:
+
+* `[SPEC]`: ID, index, range or regular expression to match item text
+
+**Options**:
+
+* `-i, --id TEXT`: ID of the item to remove
+* `-n, --index INTEGER`: Index of the item to remove
+* `-r, --range TEXT`: Range of item indices to remove, e.g, 2:5, 2:, :5
+* `-m, --match TEXT`: Regular expression to match item text
+* `-G, --global`: Remove from global todo list, even if current folder is under a git repo
+* `--help`: Show this message and exit.
+
+## `DrToDo rm`
+
+Remove/delete todo items from the list
+
+**Usage**:
+
+```console
+$ DrToDo rm [OPTIONS] [SPEC]
+```
+
+**Arguments**:
+
+* `[SPEC]`: ID, index, range or regular expression to match item text
+
+**Options**:
+
+* `-i, --id TEXT`: ID of the item to remove
+* `-n, --index INTEGER`: Index of the item to remove
+* `-r, --range TEXT`: Range of item indices to remove, e.g, 2:5, 2:, :5
+* `-m, --match TEXT`: Regular expression to match item text
+* `-G, --global`: Remove from global todo list, even if current folder is under a git repo
+* `--help`: Show this message and exit.
+
 ## `DrToDo show`
 
 Show markdown file(s) with rich rendering. Defaults to the active, configured files.
 
 **Usage**:
 
 ```console
```

