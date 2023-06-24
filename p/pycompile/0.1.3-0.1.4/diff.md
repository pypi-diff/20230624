# Comparing `tmp/pycompile-0.1.3.tar.gz` & `tmp/pycompile-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompile-0.1.3.tar", max compression
+gzip compressed data, was "pycompile-0.1.4.tar", max compression
```

## Comparing `pycompile-0.1.3.tar` & `pycompile-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1074 2023-06-23 19:00:09.392543 pycompile-0.1.3/LICENSE
--rw-r--r--   0        0        0     2195 2023-06-23 19:00:09.392543 pycompile-0.1.3/README.md
--rw-r--r--   0        0        0     1233 2023-06-23 19:00:09.392543 pycompile-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      307 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/__init__.py
--rw-r--r--   0        0        0     3696 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/benchmark.py
--rw-r--r--   0        0        0     3525 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/cli.py
--rw-r--r--   0        0        0     2641 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/compiler_handler.py
--rw-r--r--   0        0        0        0 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/__init__.py
--rw-r--r--   0        0        0      192 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/fib.py
--rw-r--r--   0        0        0      254 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/harmonic.py
--rw-r--r--   0        0        0      176 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/sum.py
--rw-r--r--   0        0        0      144 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/sum_of_sqaures.py
--rw-r--r--   0        0        0       99 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/test_fib.py
--rw-r--r--   0        0        0      131 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/test_harmonic_mean.py
--rw-r--r--   0        0        0       95 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/test_sum.py
--rw-r--r--   0        0        0      131 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/test_sum_of_sqaures.py
--rw-r--r--   0        0        0     4074 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/file_handler.py
--rw-r--r--   0        0        0     1194 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/helpers.py
--rw-r--r--   0        0        0     1341 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/logging_setup.py
--rw-r--r--   0        0        0     3209 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/wrappers.py
--rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 pycompile-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-24 11:24:13.499420 pycompile-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2368 2023-06-24 11:24:13.499420 pycompile-0.1.4/README.md
+-rw-r--r--   0        0        0     1233 2023-06-24 11:24:13.499420 pycompile-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      307 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/__init__.py
+-rw-r--r--   0        0        0     3684 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/benchmark.py
+-rw-r--r--   0        0        0     3039 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/cli.py
+-rw-r--r--   0        0        0     2641 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/compiler_handler.py
+-rw-r--r--   0        0        0        0 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/__init__.py
+-rw-r--r--   0        0        0      192 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/fib.py
+-rw-r--r--   0        0        0      254 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/harmonic.py
+-rw-r--r--   0        0        0      176 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/sum.py
+-rw-r--r--   0        0        0      144 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/sum_of_sqaures.py
+-rw-r--r--   0        0        0       99 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/test_fib.py
+-rw-r--r--   0        0        0      131 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/test_harmonic_mean.py
+-rw-r--r--   0        0        0       95 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/test_sum.py
+-rw-r--r--   0        0        0      131 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/examples/test_sum_of_sqaures.py
+-rw-r--r--   0        0        0     4062 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/file_handler.py
+-rw-r--r--   0        0        0     1194 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/helpers.py
+-rw-r--r--   0        0        0     1341 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/logging_setup.py
+-rw-r--r--   0        0        0     3209 2023-06-24 11:24:13.499420 pycompile-0.1.4/src/wrappers.py
+-rw-r--r--   0        0        0     3053 1970-01-01 00:00:00.000000 pycompile-0.1.4/PKG-INFO
```

### Comparing `pycompile-0.1.3/LICENSE` & `pycompile-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.3/README.md` & `pycompile-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 | `--input-path PATH`   | by default it will exclude any `test` and `__init__.py` files |
 | `--clean-source`      | Deletes the sources files.                                    |
 | `--keep-builds`       | Keeps the temp build files.                                   |
 | `--clean-executables` | Deletes the shared objects (`.so`) files.                     |
 | `--engine`            | Can be `cython` or `nuitka`.                                  |
 | `-exclude-glob-paths` | Glob file patterns for excluding specific files.              |
 | `--verbose`           | Increase log messages.                                        |
+| `--benchmark`         | Benchmark the examples.                                       |
 
 ### Compiling the examples
 For compiling the `examples` use the following command:
 ```bash
 pycompile -i examples
 ```
 which by default, deletes any temp build files and keeps the source files.
@@ -58,9 +59,14 @@
 
 
 ### Benchmark sample examples
 For running a benchmark on  the `examples` use the following command:
 ```bash
 pycompile -b 
 ```
+
 [![asciicast](https://asciinema.org/a/592966.svg)](https://asciinema.org/a/592966)
 
+
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/pycompile)
+
+
```

### Comparing `pycompile-0.1.3/pyproject.toml` & `pycompile-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycompile"
-version = "0.1.3"
+version = "0.1.4"
 description = "A CLI tool for compiling python"
 authors = ["iplitharas <johnplitharas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "src" }
 ]
```

### Comparing `pycompile-0.1.3/src/benchmark.py` & `pycompile-0.1.4/src/benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 Colors.RESET,
             )
             sys.exit(1)
 
         file_handler = FileHandler(
             input_path=self.examples_path,
         )
-        self.dir_files = file_handler.parse_files()
+        self.dir_files = file_handler.start()
 
     def move_examples(self, temp_dir: Path) -> None:
         """
         Copies all python files in the temp directory.
         """
         for file_path in self.examples_path.glob("*.py"):
             dest_path = temp_dir / file_path.name
@@ -89,15 +89,15 @@
         self.benchmark(directory=self.examples_path)
         for compiler in self.compilers:
             with tempfile.TemporaryDirectory() as temp_dir:
                 temp_dir = Path(temp_dir)
                 self.move_examples(temp_dir=temp_dir)
                 dir_files = FileHandler(
                     input_path=temp_dir,
-                ).parse_files()
+                ).start()
                 compiler_handler = CompilerHandler(
                     files=dir_files,
                     compiler=compiler,
                     clean_source=True,
                     keep_builds=False,
                 )
                 compiler_handler.start()
```

### Comparing `pycompile-0.1.3/src/cli.py` & `pycompile-0.1.4/src/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 @click.command()
 @click.option(
     "-i",
     "--input-path",
     required=False,
     type=click.Path(exists=True),
     help="Specify the file/folder input path, "
-    "by default it will exclude any `test` and `__ini__.py` files",
+    "by default it will exclude any `test` and `__init__.py` files",
 )
 @click.option(
     "-ex",
     "--exclude-glob-paths",
     required=False,
     multiple=True,
     type=str,
@@ -75,56 +75,31 @@
     "--benchmark",
     required=False,
     flag_value=True,
     default=False,
     help="Benchmark the examples.",
 )
 def main(  # pylint: disable=too-many-arguments
-    input_path,
-    exclude_glob_paths,
+    input_path: Path,
+    exclude_glob_paths: list[str],
     verbose,
-    engine,
-    clean_source,
-    keep_builds,
-    clean_executables,
-    benchmark,
+    engine: str,
+    clean_source: bool,
+    keep_builds: bool,
+    clean_executables: bool,
+    benchmark: bool,
 ):
     r"""
                                           _ _
     _ __  _   _  ___ ___  _ __ ___  _ __ (_) | ___
    | '_ \| | | |/ __/ _ \| '_ ` _ \| '_ \| | |/ _ \
    | |_) | |_| | (_| (_) | | | | | | |_) | | |  __/
    | .__/ \__, |\___\___/|_| |_| |_| .__/|_|_|\___|
    |_|    |___/                    |_|
    """
-    handle_user_input(
-        input_path,
-        exclude_glob_paths,
-        verbose,
-        engine,
-        clean_source,
-        keep_builds,
-        clean_executables,
-        benchmark,
-    )
-
-
-def handle_user_input(  # pylint: disable=too-many-arguments
-    input_path: Path,
-    exclude_glob_paths: list[str],
-    verbose: int,
-    engine: str,
-    clean_source: bool,
-    keep_builds: bool,
-    clean_executables: bool,
-    benchmark: bool,
-) -> None:
-    """
-    Helper function for handling the user input.
-    """
     setup_logging(verbose)
     if benchmark:
         bench = Benchmark()
         bench.start()
         sys.exit(0)
 
     if not input_path:
@@ -132,15 +107,15 @@
             "%s Input path is missing, exiting...%s", Colors.FAIL, Colors.RESET
         )
         sys.exit(1)
 
     dir_files = FileHandler(
         input_path=input_path,
         additional_exclude_patterns=exclude_glob_paths,
-    ).parse_files()
+    ).start()
 
     if dir_files:
         compiler = (
             CythonWrapper() if engine.lower() == "cython" else NuitkaWrapper()
         )
         compiler_handler = CompilerHandler(
             files=dir_files,
```

### Comparing `pycompile-0.1.3/src/compiler_handler.py` & `pycompile-0.1.4/src/compiler_handler.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.3/src/file_handler.py` & `pycompile-0.1.4/src/file_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 logger = logging.getLogger(__name__)
 
 
 class FileHandler:
     """
     FileHandler is responsible for finding all the `.py` files  given
     any `input_path`.
-    example usage: FileHandler("./my_module).parse_files()
+    example usage: FileHandler("./my_module).start()
     """
 
     def __init__(
         self,
         input_path: Path | str,
         additional_exclude_patterns: list[str] = None,
     ):
@@ -63,15 +63,15 @@
             "**/test**",
             "**/__init__.py",
         ]
 
         if additional_exclude_patterns:
             self._exclude_patterns.extend(additional_exclude_patterns)
 
-    def parse_files(self) -> dict[str : list[Path]]:
+    def start(self) -> dict[str : list[Path]]:
         """
         For the given `input path` collect all valid `.py` files.
         :return: a dictionary for valid files within each directory.
         """
 
         files = defaultdict(list[Path])
         excluded_files = list(self._filter_files())
```

### Comparing `pycompile-0.1.3/src/helpers.py` & `pycompile-0.1.4/src/helpers.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.3/src/logging_setup.py` & `pycompile-0.1.4/src/logging_setup.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.3/src/wrappers.py` & `pycompile-0.1.4/src/wrappers.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.3/PKG-INFO` & `pycompile-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycompile
-Version: 0.1.3
+Version: 0.1.4
 Summary: A CLI tool for compiling python
 License: MIT
 Author: iplitharas
 Author-email: johnplitharas@gmail.com
 Requires-Python: >3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -62,14 +62,15 @@
 | `--input-path PATH`   | by default it will exclude any `test` and `__init__.py` files |
 | `--clean-source`      | Deletes the sources files.                                    |
 | `--keep-builds`       | Keeps the temp build files.                                   |
 | `--clean-executables` | Deletes the shared objects (`.so`) files.                     |
 | `--engine`            | Can be `cython` or `nuitka`.                                  |
 | `-exclude-glob-paths` | Glob file patterns for excluding specific files.              |
 | `--verbose`           | Increase log messages.                                        |
+| `--benchmark`         | Benchmark the examples.                                       |
 
 ### Compiling the examples
 For compiling the `examples` use the following command:
 ```bash
 pycompile -i examples
 ```
 which by default, deletes any temp build files and keeps the source files.
@@ -78,10 +79,15 @@
 
 
 ### Benchmark sample examples
 For running a benchmark on  the `examples` use the following command:
 ```bash
 pycompile -b 
 ```
+
 [![asciicast](https://asciinema.org/a/592966.svg)](https://asciinema.org/a/592966)
 
 
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/pycompile)
+
+
+
```

