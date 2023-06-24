# Comparing `tmp/jupyter_cleaner-0.2.0.tar.gz` & `tmp/jupyter_cleaner-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_cleaner-0.2.0.tar", max compression
+gzip compressed data, was "jupyter_cleaner-0.2.1.tar", max compression
```

## Comparing `jupyter_cleaner-0.2.0.tar` & `jupyter_cleaner-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-21 17:07:31.522031 jupyter_cleaner-0.2.0/jupyter_cleaner/__init__.py
--rw-r--r--   0        0        0    16233 2023-06-23 07:52:40.510421 jupyter_cleaner-0.2.0/jupyter_cleaner/jupyter_cleaner.py
--rw-r--r--   0        0        0     1092 2023-06-21 17:40:20.719190 jupyter_cleaner-0.2.0/LICENSE
--rw-r--r--   0        0        0     1795 2023-06-23 07:54:53.033923 jupyter_cleaner-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1991 2023-06-23 07:54:37.232156 jupyter_cleaner-0.2.0/README.md
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jupyter_cleaner-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 17:07:31.522031 jupyter_cleaner-0.2.1/jupyter_cleaner/__init__.py
+-rw-r--r--   0        0        0    16790 2023-06-24 19:41:04.694071 jupyter_cleaner-0.2.1/jupyter_cleaner/jupyter_cleaner.py
+-rw-r--r--   0        0        0     1092 2023-06-21 17:40:20.719190 jupyter_cleaner-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1795 2023-06-24 19:42:32.682098 jupyter_cleaner-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1991 2023-06-23 07:54:37.232156 jupyter_cleaner-0.2.1/README.md
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jupyter_cleaner-0.2.1/PKG-INFO
```

### Comparing `jupyter_cleaner-0.2.0/jupyter_cleaner/jupyter_cleaner.py` & `jupyter_cleaner-0.2.1/jupyter_cleaner/jupyter_cleaner.py`

 * *Files 6% similar despite different names*

```diff
@@ -274,84 +274,100 @@
         help="Format code of every cell (uses black)",
     )
     parser.add_argument(
         "--reorder_imports",
         action="store_false",
         help="Reorder imports of every cell (uses reorder-python-imports)",
     )
+    parser.add_argument(
+        "--ignore_pyproject",
+        action="store_false",
+        help="Argparse will over-ride pyproject",
+    )
     args = parser.parse_args()
     return (
         args.files_or_dirs,
         args.execution_count,
         args.remove_code_output,
         args.format,
         args.reorder_imports,
         args.indent_level,
         args.exclude_files_or_dirs,
+        args.ignore_pyproject,
     )
 
 
-def get_lab_files(files_or_dirss: List[Path]) -> List[Path]:
+def get_lab_files(files_or_dirs: List[Path]) -> List[Path]:
     files = []
-    for file_or_dir in files_or_dirss:
+    for file_or_dir in files_or_dirs:
         if file_or_dir.is_dir():
             files.extend([p for p in file_or_dir.rglob("*.ipynb")])
         elif file_or_dir.is_file() and file_or_dir.suffix == ".ipynb":
             files.append(file_or_dir)
         else:
             raise ValueError("File or directory does not exist or could not be found")
     return list(set(files))
 
 
 def process_inputs(
-    args_files_or_dirss: List[str],
+    args_files_or_dirs: List[str],
     args_execution_count: int,
     args_remove_code_output: bool,
     args_format: bool,
     args_reorder_imports: bool,
     args_indent_level: int,
     args_exclude_files_or_dirs: Union[List[str], None],
-    project_files_or_dirss: Union[List[str], str, None],
+    args_ignore_pyproject: bool,
+    project_files_or_dirs: Union[List[str], str, None],
     project_execution_count: Union[int, None],
     project_remove_code_output: Union[bool, None],
     project_format: Union[bool, None],
     project_reorder_imports: Union[bool, None],
     project_indent_level: Union[int, None],
     project_exclude_files_or_dirs: Union[List[str], str, None],
 ) -> Tuple[List[Path], int, bool, bool, bool, int, List[Path]]:
     """Creates inputs of the right format and prioritises pyproject inputs over argparse inputs, outside of files and directories where all inputs are combined.
 
-    :param List[str] args_files_or_dirss: files or directories from argparse
+    :param List[str] args_files_or_dirs: files or directories from argparse
     :param List[str] args_exclude_files_or_dirs: files or directories to exclude from argparse
     :param int args_execution_count: execution count from argparse
     :param bool args_remove_code_output: remove code output from argparse
     :param bool args_format: apply formatting from argparse
     :param bool args_reorder_imports: reorder imports from argparse
-    :param Union[List[str], str, None] project_files_or_dirss: files or directories from pyproject
+    :param Union[List[str], str, None] project_files_or_dirs: files or directories from pyproject
     :param Union[List[str], str, None] project_exclude_files_or_dirs: files or directories to exclude from pyproject
     :param Union[int, None] project_execution_count: execution count from pyproject
     :param Union[bool, None] project_remove_code_output: remove code output from pyproject
     :param Union[bool, None] project_format: apply formatting from pyproject
     :param Union[bool, None] project_reorder_imports: reorder imports from pyproject
     :return Tuple[ Union[List[str], str, None], Union[int, None], Union[bool, None], Union[bool, None], Union[bool, None], ]: inputs to run()
     """
-    if args_files_or_dirss is None:
-        args_files_or_dirss = [Path.cwd().resolve()]
-    if project_files_or_dirss is None:
-        project_files_or_dirss = []
-    elif isinstance(project_files_or_dirss, str):
-        project_files_or_dirss = [project_files_or_dirss]
-    files_or_dirss = [Path(f) for f in project_files_or_dirss + args_files_or_dirss]
+    if args_ignore_pyproject:
+        project_files_or_dirs = None
+        project_execution_count = None
+        project_remove_code_output = None
+        project_format = None
+        project_reorder_imports = None
+        project_indent_level = None
+        project_exclude_files_or_dirs = None
+
+    if args_files_or_dirs is None:
+        args_files_or_dirs = [Path.cwd().resolve()]
+    if project_files_or_dirs is None:
+        project_files_or_dirs = []
+    elif isinstance(project_files_or_dirs, str):
+        project_files_or_dirs = [project_files_or_dirs]
+    files_or_dirs = [Path(f) for f in project_files_or_dirs + args_files_or_dirs]
     if project_exclude_files_or_dirs is None:
         project_exclude_files_or_dirs = []
     elif isinstance(project_exclude_files_or_dirs, str):
         project_exclude_files_or_dirs = [project_exclude_files_or_dirs]
     if args_exclude_files_or_dirs is None:
         args_exclude_files_or_dirs = []
-    exclude_files_or_dirss = [
+    exclude_files_or_dirs = [
         Path(f) for f in project_exclude_files_or_dirs + args_exclude_files_or_dirs
     ]
     execution_count = (
         project_execution_count
         if project_execution_count is not None
         else args_execution_count
     )
@@ -367,72 +383,74 @@
         else args_reorder_imports
     )
     indent_level = (
         project_indent_level if project_indent_level is not None else args_indent_level
     )
 
     return (
-        files_or_dirss,
+        files_or_dirs,
         execution_count,
         remove_code_output,
         format,
         reorder_imports,
         indent_level,
-        exclude_files_or_dirss,
+        exclude_files_or_dirs,
     )
 
 
 def main():
     (
-        args_files_or_dirss,
+        args_files_or_dirs,
         args_execution_count,
         args_remove_code_output,
         args_format,
         args_reorder_imports,
         args_indent_level,
         args_exclude_files_or_dirs,
+        args_ignore_pyproject,
     ) = parse_args()
 
     (
-        project_files_or_dirss,
+        project_files_or_dirs,
         project_execution_count,
         project_remove_code_output,
         project_format,
         project_reorder_imports,
         project_indent_level,
         project_exclude_files_or_dirs,
     ) = parse_pyproject()
 
     (
-        files_or_dirss,
+        files_or_dirs,
         execution_count,
         remove_code_output,
         format,
         reorder_imports,
         indent_level,
-        exclude_files_or_dirss,
+        exclude_files_or_dirs,
     ) = process_inputs(
-        args_files_or_dirss,
+        args_files_or_dirs,
         args_execution_count,
         args_remove_code_output,
         args_format,
         args_reorder_imports,
         args_indent_level,
         args_exclude_files_or_dirs,
-        project_files_or_dirss,
+        args_ignore_pyproject,
+        project_files_or_dirs,
         project_execution_count,
         project_remove_code_output,
         project_format,
         project_reorder_imports,
         project_indent_level,
         project_exclude_files_or_dirs,
     )
 
-    files = get_lab_files(files_or_dirss)
-    exclude_files = get_lab_files(exclude_files_or_dirss)
+    files = get_lab_files(files_or_dirs)
+    exclude_files = get_lab_files(exclude_files_or_dirs)
 
     run(
         files,
         execution_count,
         remove_code_output,
         format,
         reorder_imports,
```

### Comparing `jupyter_cleaner-0.2.0/LICENSE` & `jupyter_cleaner-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_cleaner-0.2.0/pyproject.toml` & `jupyter_cleaner-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jupyter-cleaner"
-version = "0.2.0"
+version = "0.2.1"
 description = "Easy git tracking of Jupyter lab files"
 license = "MIT"
 authors = ["Daniel Stoops <danielstoops25@gmail.com>"]
 maintainers = ["Daniel Stoops <danielstoops25@gmail.com>"]
 readme = "README.md"
 packages = [{include = "jupyter_cleaner"}]
 homepage = "https://github.com/Stoops-ML/jupyter-cleaner"
```

### Comparing `jupyter_cleaner-0.2.0/README.md` & `jupyter_cleaner-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_cleaner-0.2.0/PKG-INFO` & `jupyter_cleaner-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-cleaner
-Version: 0.2.0
+Version: 0.2.1
 Summary: Easy git tracking of Jupyter lab files
 Home-page: https://github.com/Stoops-ML/jupyter-cleaner
 License: MIT
 Author: Daniel Stoops
 Author-email: danielstoops25@gmail.com
 Maintainer: Daniel Stoops
 Maintainer-email: danielstoops25@gmail.com
```

