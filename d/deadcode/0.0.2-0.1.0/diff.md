# Comparing `tmp/deadcode-0.0.2.tar.gz` & `tmp/deadcode-0.1.0.tar.gz`

## Comparing `deadcode-0.0.2.tar` & `deadcode-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,25 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/__init__.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/cli.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/data_types.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/actions/__init__.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/actions/argument_parsing.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/module_a.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/module_b.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/test_deadcode.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/test_case1/hello_world.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/test_case1/subdir/one_more_file.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-0.0.2/deadcode/tests/test_case1/subdir/another_subdir/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-0.0.2/.gitignore
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 deadcode-0.0.2/README.md
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 deadcode-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 deadcode-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/cli.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/data_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/__init__.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/find_python_filenames.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/find_unused_names.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/get_unused_names_error_message.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/parse_abstract_syntax_trees.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/parse_arguments.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/parse_global_names.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/actions/read_files.py
+-rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/test_deadcode.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/files/classes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/files/functions.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/files/variables.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/files/subdir/one_more_file.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/tests/files/subdir/another_subdir/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/utils/__init__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/utils/flatten_lists.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 deadcode-0.1.0/deadcode/utils/path_matching.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 deadcode-0.1.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 deadcode-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 deadcode-0.1.0/README.md
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 deadcode-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 deadcode-0.1.0/PKG-INFO
```

### Comparing `deadcode-0.0.2/deadcode/utils.py` & `deadcode-0.1.0/deadcode/utils/flatten_lists.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import List, Optional
 
 
-def split_comma_separated_values(list_of_comma_separated_values: Optional[List[str]]) -> List[str]:
+def flatten_lists_of_comma_separated_values(
+    list_of_comma_separated_values: Optional[List[List[str]]],
+) -> List[str]:
     """Concatenates lists into one list."""
     if not list_of_comma_separated_values:
         return []
     list_of_comma_separated_values = flatten_list(list_of_comma_separated_values)
-    return flatten_list([v.split(",") for v in list_of_comma_separated_values])
+    return flatten_list([v.split(",") for v in list_of_comma_separated_values])  # type: ignore
 
 
-def flatten_list(list_of_lists: Optional[List[List[str]]]) -> List[str]:
+def flatten_list(list_of_lists: Optional[List[List]]) -> List:
     """Concatenates lists into one list."""
     if not list_of_lists:
         return []
     return [elem for elem_list in list_of_lists for elem in elem_list]
```

### Comparing `deadcode-0.0.2/.gitignore` & `deadcode-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `deadcode-0.0.2/pyproject.toml` & `deadcode-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deadcode"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
     {name = "Albertas Gimbutas", email = "albertasgim@gmail.com"},
 ]
 description = "Find and remove dead code."
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
@@ -36,25 +36,37 @@
 [tool.hatch.publish.index]  # Hatch docs: https://hatch.pypa.io/latest/config/build/
 disable = true
 
 [tool.hatch.build]
 include = ["**/*.py"]
 exclude = ["tests/**"]
 
+
+[tool.ruff]  # https://beta.ruff.rs/docs/settings/
+line-length = 120
+
+
 [tool.mypy]
 exclude = ["build", "dist", "venv"]
 python_version = "3.8"
 strict = true
 pretty = true
 color_output = true
 show_error_codes = true
 warn_return_any = true
 warn_unused_configs = true
 
+
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 known_third_party = ["deadcode"]
 
 
+[tool.black]
+max_line_length = 120
+line_length = 120
+target_version = ["py38"]
 
 
+[tool.pytest.ini_options]
+addopts = "--cov=. --cov-fail-under=90.0"
```

