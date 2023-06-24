# Comparing `tmp/pytarrs-0.1.2.tar.gz` & `tmp/pytarrs-0.1.3.tar.gz`

## Comparing `pytarrs-0.1.2.tar` & `pytarrs-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0      176 1970-01-01 00:00:00.000000 pytarrs-0.1.2/Cargo.toml
--rw-r--r--   0        0        0       49 2023-06-23 05:17:36.000000 pytarrs-0.1.2/README.md
--rw-r--r--   0        0        0     2796 2023-06-23 06:31:40.000000 pytarrs-0.1.2/src/lib.rs
--rw-r--r--   0        0        0      315 2023-06-23 06:24:05.000000 pytarrs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8628 2023-06-23 06:33:07.000000 pytarrs-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 pytarrs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      176 1970-01-01 00:00:00.000000 pytarrs-0.1.3/Cargo.toml
+-rw-r--r--   0        0        0       49 2023-06-23 05:17:36.000000 pytarrs-0.1.3/README.md
+-rw-r--r--   0        0        0     2188 2023-06-24 09:45:14.000000 pytarrs-0.1.3/src/grouper.rs
+-rw-r--r--   0        0        0     1574 2023-06-24 07:31:01.000000 pytarrs-0.1.3/src/lib.rs
+-rw-r--r--   0        0        0     2336 2023-06-24 07:40:40.000000 pytarrs-0.1.3/src/sample.rs
+-rw-r--r--   0        0        0     1591 2023-06-24 04:24:41.000000 pytarrs-0.1.3/src/tar.rs
+-rw-r--r--   0        0        0      315 2023-06-23 06:24:05.000000 pytarrs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8628 2023-06-24 09:46:59.000000 pytarrs-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 pytarrs-0.1.3/PKG-INFO
```

### Comparing `pytarrs-0.1.2/Cargo.lock` & `pytarrs-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pytarrs"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "pyo3",
  "tar",
 ]
 
 [[package]]
 name = "quote"
```

