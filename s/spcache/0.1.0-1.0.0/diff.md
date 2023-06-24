# Comparing `tmp/spcache-0.1.0.tar.gz` & `tmp/spcache-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spcache-0.1.0.tar", max compression
+gzip compressed data, was "spcache-1.0.0.tar", max compression
```

## Comparing `spcache-0.1.0.tar` & `spcache-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-06-14 11:16:46.985486 spcache-0.1.0/LICENSE
--rw-r--r--   0        0        0       76 2023-06-14 11:16:46.985486 spcache-0.1.0/README.md
--rw-r--r--   0        0        0     3017 2023-06-14 11:16:46.985486 spcache-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       58 2023-06-14 11:16:46.985486 spcache-0.1.0/spcache/__init__.py
--rw-r--r--   0        0        0       64 2023-06-14 11:16:46.985486 spcache-0.1.0/spcache/__main__.py
--rw-r--r--   0        0        0     2903 2023-06-14 11:16:46.985486 spcache-0.1.0/spcache/cli.py
--rw-r--r--   0        0        0     2256 2023-06-14 11:16:46.985486 spcache-0.1.0/spcache/detect.py
--rw-r--r--   0        0        0     3133 2023-06-14 11:16:46.985486 spcache-0.1.0/spcache/env.py
--rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 spcache-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-24 09:50:01.464052 spcache-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3471 2023-06-24 09:50:01.464052 spcache-1.0.0/README.md
+-rw-r--r--   0        0        0     3017 2023-06-24 09:50:01.468052 spcache-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-06-24 09:50:01.468052 spcache-1.0.0/spcache/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-24 09:50:01.468052 spcache-1.0.0/spcache/__main__.py
+-rw-r--r--   0        0        0     4991 2023-06-24 09:50:01.468052 spcache-1.0.0/spcache/cli.py
+-rw-r--r--   0        0        0     2256 2023-06-24 09:50:01.468052 spcache-1.0.0/spcache/detect.py
+-rw-r--r--   0        0        0     3798 2023-06-24 09:50:01.468052 spcache-1.0.0/spcache/env.py
+-rw-r--r--   0        0        0     4850 1970-01-01 00:00:00.000000 spcache-1.0.0/PKG-INFO
```

### Comparing `spcache-0.1.0/LICENSE` & `spcache-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spcache-0.1.0/pyproject.toml` & `spcache-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spcache"
-version = "0.1.0"
+version = "1.0.0"
 description = "Ensure Spotify's cache size doesn't exceed a specified threshold."
 authors = ["Qwerty-133 <74311372+Qwerty-133@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/Qwerty-133/spcache"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `spcache-0.1.0/spcache/detect.py` & `spcache-1.0.0/spcache/detect.py`

 * *Files identical despite different names*

### Comparing `spcache-0.1.0/spcache/env.py` & `spcache-1.0.0/spcache/env.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.line_content = line_content
 
 
 @contextmanager
 def rewrite(
     path: dotenv.main.StrPath,
     encoding: t.Optional[str],
-) -> t.Iterator[t.Tuple[t.IO[str], t.IO[str]]]:
+) -> t.Iterator[t.Tuple[t.TextIO, t.TextIO]]:
     """Make changes to a file atomically."""
     if not os.path.isfile(path):
         with open(path, mode="w", encoding=encoding) as source:
             pass
 
     dest_file = tempfile.NamedTemporaryFile(mode="w", encoding=encoding, delete=False)
 
@@ -36,14 +36,15 @@
         os.unlink(dest_file.name)
         raise
 
     try:
         yield (source, dest_file)
     except BaseException:
         failed = True
+        raise
     else:
         failed = False
     finally:
         dest_file.close()
         source.close()
         if failed:
             os.unlink(dest_file.name)
@@ -80,15 +81,15 @@
     line_out = f"export {key_to_set}={value_out}\n" if export else f"{key_to_set}={value_out}\n"
     previous_value = None
 
     with rewrite(dotenv_path, encoding=encoding) as (source, dest):
         replaced = False
         missing_newline = False
         for mapping in dotenv.main.parse_stream(source):
-            if not ignore_errors:
+            if not ignore_errors and mapping.error:
                 raise InvalidLineError(mapping.original.line, mapping.original.string)
 
             if mapping.key == key_to_set:
                 dest.write(line_out)
                 replaced = True
                 previous_value = mapping.value
             else:
@@ -96,7 +97,29 @@
                 missing_newline = not mapping.original.string.endswith("\n")
         if not replaced:
             if missing_newline:
                 dest.write("\n")
             dest.write(line_out)
 
     return previous_value
+
+
+def get_key(
+    dotenv_path: dotenv.main.StrPath,
+    key: str,
+    ignore_errors: bool = False,
+) -> t.Optional[str]:
+    """
+    Obtain a key's value from the given .env file.
+
+    If the key doesn't exist, None is returned.
+    If ignore_errors is True, invalid lines in the file will be ignored.
+    """
+    with open(dotenv_path) as stream:
+        for mapping in dotenv.main.parse_stream(stream):
+            if not ignore_errors and mapping.error:
+                raise InvalidLineError(mapping.original.line, mapping.original.string)
+
+            if mapping.key == key:
+                return mapping.value
+
+    return None
```

