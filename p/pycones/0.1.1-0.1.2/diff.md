# Comparing `tmp/pycones-0.1.1.tar.gz` & `tmp/pycones-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycones-0.1.1.tar", max compression
+gzip compressed data, was "pycones-0.1.2.tar", max compression
```

## Comparing `pycones-0.1.1.tar` & `pycones-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      172 2023-06-23 10:06:11.466750 pycones-0.1.1/README.md
--rw-r--r--   0        0        0      434 2023-06-23 10:04:20.896751 pycones-0.1.1/pycones/__init__.py
--rw-r--r--   0        0        0      680 2023-06-23 10:04:37.246752 pycones-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 pycones-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      373 2023-06-24 09:08:37.437746 pycones-0.1.2/README.md
+-rw-r--r--   0        0        0      435 2023-06-24 09:07:55.327757 pycones-0.1.2/pycones/__init__.py
+-rw-r--r--   0        0        0      676 2023-06-24 09:07:55.327757 pycones-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 pycones-0.1.2/PKG-INFO
```

### Comparing `pycones-0.1.1/pyproject.toml` & `pycones-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "pycones"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["william <william_swl@163.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
-matplotlib = "^3.7.1"
-numpy = "^1.25.0"
-pandas = "^2.0.2"
+python = ">=3.6"
+matplotlib = ">=3.0"
+numpy = ">=1.0"
+pandas = ">=2.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
 tox = "^4.6.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "0.1.1"
+current_version = "0.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'version = "{version}"',
 ]
```

