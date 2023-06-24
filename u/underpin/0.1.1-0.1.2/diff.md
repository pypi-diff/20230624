# Comparing `tmp/underpin-0.1.1.tar.gz` & `tmp/underpin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "underpin-0.1.1.tar", max compression
+gzip compressed data, was "underpin-0.1.2.tar", max compression
```

## Comparing `underpin-0.1.1.tar` & `underpin-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     5249 2023-06-23 18:55:48.347419 underpin-0.1.1/README.md
--rw-r--r--   0        0        0      634 2023-06-24 18:43:33.407167 underpin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      241 2023-06-24 18:37:51.805665 underpin-0.1.1/underpin/__init__.py
--rw-r--r--   0        0        0     4903 2023-06-24 18:40:18.954022 underpin-0.1.1/underpin/__main__.py
--rw-r--r--   0        0        0        0 2023-06-19 12:50:03.485800 underpin-0.1.1/underpin/ai/model.py
--rw-r--r--   0        0        0     1970 2023-06-24 18:42:04.030347 underpin-0.1.1/underpin/config.py
--rw-r--r--   0        0        0        0 2023-06-20 22:47:20.939127 underpin-0.1.1/underpin/pipeline/__init__.py
--rw-r--r--   0        0        0     1433 2023-06-23 01:47:02.446887 underpin-0.1.1/underpin/pipeline/default.py
--rw-r--r--   0        0        0      425 2023-06-21 02:44:49.044800 underpin-0.1.1/underpin/schema/ChangeSet.py
--rw-r--r--   0        0        0       32 2023-06-21 11:12:05.687373 underpin-0.1.1/underpin/schema/__init__.py
--rw-r--r--   0        0        0        2 2023-06-21 10:31:27.006880 underpin-0.1.1/underpin/schema/common.py
--rw-r--r--   0        0        0        0 2023-06-19 12:46:41.715073 underpin-0.1.1/underpin/setup.py
--rw-r--r--   0        0        0     5896 2023-06-24 17:30:50.918085 underpin-0.1.1/underpin/templates/UnderpinTemplate.py
--rw-r--r--   0        0        0      212 2023-06-23 01:25:27.413799 underpin-0.1.1/underpin/templates/__init__.py
--rw-r--r--   0        0        0      996 2023-06-23 23:35:03.076115 underpin-0.1.1/underpin/templates/template_containers.py
--rw-r--r--   0        0        0     1927 2023-06-23 23:31:19.123321 underpin-0.1.1/underpin/templates/template_yaml.py
--rw-r--r--   0        0        0       65 2023-06-23 18:39:36.198580 underpin-0.1.1/underpin/utils/__init__.py
--rw-r--r--   0        0        0     1552 2023-06-24 12:27:34.207003 underpin-0.1.1/underpin/utils/funcs.py
--rw-r--r--   0        0        0     5931 2023-06-23 23:47:28.252790 underpin-0.1.1/underpin/utils/git/GitContext.py
--rw-r--r--   0        0        0     6923 2023-06-22 02:29:29.670561 underpin-0.1.1/underpin/utils/git/__init__.py
--rw-r--r--   0        0        0      820 2023-06-23 11:16:03.325554 underpin-0.1.1/underpin/utils/io/__init__.py
--rw-r--r--   0        0        0     5849 1970-01-01 00:00:00.000000 underpin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5249 2023-06-23 18:55:48.347419 underpin-0.1.2/README.md
+-rw-r--r--   0        0        0      613 2023-06-24 18:54:34.469973 underpin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      241 2023-06-24 18:37:51.805665 underpin-0.1.2/underpin/__init__.py
+-rw-r--r--   0        0        0     4903 2023-06-24 18:40:18.954022 underpin-0.1.2/underpin/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:50:03.485800 underpin-0.1.2/underpin/ai/model.py
+-rw-r--r--   0        0        0     1970 2023-06-24 18:42:04.030347 underpin-0.1.2/underpin/config.py
+-rw-r--r--   0        0        0        0 2023-06-20 22:47:20.939127 underpin-0.1.2/underpin/pipeline/__init__.py
+-rw-r--r--   0        0        0     1433 2023-06-23 01:47:02.446887 underpin-0.1.2/underpin/pipeline/default.py
+-rw-r--r--   0        0        0      425 2023-06-21 02:44:49.044800 underpin-0.1.2/underpin/schema/ChangeSet.py
+-rw-r--r--   0        0        0       32 2023-06-21 11:12:05.687373 underpin-0.1.2/underpin/schema/__init__.py
+-rw-r--r--   0        0        0        2 2023-06-21 10:31:27.006880 underpin-0.1.2/underpin/schema/common.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:46:41.715073 underpin-0.1.2/underpin/setup.py
+-rw-r--r--   0        0        0     5896 2023-06-24 17:30:50.918085 underpin-0.1.2/underpin/templates/UnderpinTemplate.py
+-rw-r--r--   0        0        0      212 2023-06-23 01:25:27.413799 underpin-0.1.2/underpin/templates/__init__.py
+-rw-r--r--   0        0        0      996 2023-06-23 23:35:03.076115 underpin-0.1.2/underpin/templates/template_containers.py
+-rw-r--r--   0        0        0     1927 2023-06-23 23:31:19.123321 underpin-0.1.2/underpin/templates/template_yaml.py
+-rw-r--r--   0        0        0       65 2023-06-23 18:39:36.198580 underpin-0.1.2/underpin/utils/__init__.py
+-rw-r--r--   0        0        0     1552 2023-06-24 12:27:34.207003 underpin-0.1.2/underpin/utils/funcs.py
+-rw-r--r--   0        0        0     5931 2023-06-23 23:47:28.252790 underpin-0.1.2/underpin/utils/git/GitContext.py
+-rw-r--r--   0        0        0     6923 2023-06-22 02:29:29.670561 underpin-0.1.2/underpin/utils/git/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-23 11:16:03.325554 underpin-0.1.2/underpin/utils/io/__init__.py
+-rw-r--r--   0        0        0     5807 1970-01-01 00:00:00.000000 underpin-0.1.2/PKG-INFO
```

### Comparing `underpin-0.1.1/README.md` & `underpin-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `underpin-0.1.1/pyproject.toml` & `underpin-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "underpin"
-version = "0.1.1"
+version = "0.1.2"
 description = "tools for sending app modules to k8s infrastructure and managing app versions"
 authors = ["mr-saoirse <amartey@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
 loguru = "^0.7.0"
-pydantic = "^1.10.9"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^6.0.0"
 pytest-mock = "*"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "*"
```

### Comparing `underpin-0.1.1/underpin/__main__.py` & `underpin-0.1.2/underpin/__main__.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.1/underpin/config.py` & `underpin-0.1.2/underpin/config.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.1/underpin/pipeline/default.py` & `underpin-0.1.2/underpin/pipeline/default.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.1/underpin/templates/UnderpinTemplate.py` & `underpin-0.1.2/underpin/templates/UnderpinTemplate.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.1/underpin/templates/template_containers.py` & `underpin-0.1.2/underpin/templates/template_containers.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.1/underpin/templates/template_yaml.py` & `underpin-0.1.2/underpin/templates/template_yaml.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.1/underpin/utils/funcs.py` & `underpin-0.1.2/underpin/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.1/underpin/utils/git/GitContext.py` & `underpin-0.1.2/underpin/utils/git/GitContext.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.1/underpin/utils/git/__init__.py` & `underpin-0.1.2/underpin/utils/git/__init__.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.1/underpin/utils/io/__init__.py` & `underpin-0.1.2/underpin/utils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `underpin-0.1.1/PKG-INFO` & `underpin-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: underpin
-Version: 0.1.1
+Version: 0.1.2
 Summary: tools for sending app modules to k8s infrastructure and managing app versions
 License: MIT
 Author: mr-saoirse
 Author-email: amartey@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Underpinnings
 
 Underpinnings is an experimental utility to explore a two-repo pattern for migrating templated apps from an "applications" repo to a K8s "infrastructure" repo.
```

