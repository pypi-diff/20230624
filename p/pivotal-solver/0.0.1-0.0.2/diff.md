# Comparing `tmp/pivotal-solver-0.0.1.tar.gz` & `tmp/pivotal-solver-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pivotal-solver-0.0.1.tar", last modified: Sat Jun 24 15:41:00 2023, max compression
+gzip compressed data, was "pivotal-solver-0.0.2.tar", last modified: Sat Jun 24 15:47:51 2023, max compression
```

## Comparing `pivotal-solver-0.0.1.tar` & `pivotal-solver-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:41:00.962053 pivotal-solver-0.0.1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      126 2023-06-24 13:09:14.000000 pivotal-solver-0.0.1/.flake8
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       62 2023-06-24 13:26:47.000000 pivotal-solver-0.0.1/.gitignore
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      355 2023-06-24 13:09:14.000000 pivotal-solver-0.0.1/.pre-commit-config.yaml
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1064 2023-06-24 13:13:25.000000 pivotal-solver-0.0.1/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5553 2023-06-24 15:41:00.962053 pivotal-solver-0.0.1/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3382 2023-06-24 15:28:12.000000 pivotal-solver-0.0.1/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    16866 2023-06-24 14:54:44.000000 pivotal-solver-0.0.1/logo.svg
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:41:00.954053 pivotal-solver-0.0.1/pivotal/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      200 2023-06-24 15:26:18.000000 pivotal-solver-0.0.1/pivotal/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10871 2023-06-24 15:15:47.000000 pivotal-solver-0.0.1/pivotal/api.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      172 2023-06-24 13:33:47.000000 pivotal-solver-0.0.1/pivotal/errors.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6460 2023-06-24 13:36:24.000000 pivotal-solver-0.0.1/pivotal/simplex.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:41:00.954053 pivotal-solver-0.0.1/pivotal_solver.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5553 2023-06-24 15:41:00.000000 pivotal-solver-0.0.1/pivotal_solver.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      457 2023-06-24 15:41:00.000000 pivotal-solver-0.0.1/pivotal_solver.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-06-24 15:41:00.000000 pivotal-solver-0.0.1/pivotal_solver.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       44 2023-06-24 15:41:00.000000 pivotal-solver-0.0.1/pivotal_solver.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        8 2023-06-24 15:41:00.000000 pivotal-solver-0.0.1/pivotal_solver.egg-info/top_level.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1387 2023-06-24 15:39:54.000000 pivotal-solver-0.0.1/pyproject.toml
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:41:00.958053 pivotal-solver-0.0.1/resources/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   468869 2023-06-24 13:09:14.000000 pivotal-solver-0.0.1/resources/2_Simplex.pdf
--rw-rw-r--   0 tomas     (1000) tomas     (1000)  2807945 2023-06-16 22:01:01.000000 pivotal-solver-0.0.1/resources/cvut_fel_opt.pdf
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   677438 2023-06-24 13:09:14.000000 pivotal-solver-0.0.1/resources/mitocw.pdf
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-06-24 15:41:00.962053 pivotal-solver-0.0.1/setup.cfg
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:41:00.962053 pivotal-solver-0.0.1/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4460 2023-06-24 13:26:24.000000 pivotal-solver-0.0.1/tests/test_api.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4668 2023-06-24 13:09:14.000000 pivotal-solver-0.0.1/tests/test_simplex.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:47:51.148971 pivotal-solver-0.0.2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      126 2023-06-24 13:09:14.000000 pivotal-solver-0.0.2/.flake8
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       62 2023-06-24 13:26:47.000000 pivotal-solver-0.0.2/.gitignore
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      355 2023-06-24 13:09:14.000000 pivotal-solver-0.0.2/.pre-commit-config.yaml
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1064 2023-06-24 13:13:25.000000 pivotal-solver-0.0.2/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5560 2023-06-24 15:47:51.144971 pivotal-solver-0.0.2/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3389 2023-06-24 15:46:19.000000 pivotal-solver-0.0.2/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    16866 2023-06-24 14:54:44.000000 pivotal-solver-0.0.2/logo.svg
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:47:51.140971 pivotal-solver-0.0.2/pivotal/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      200 2023-06-24 15:47:25.000000 pivotal-solver-0.0.2/pivotal/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10871 2023-06-24 15:15:47.000000 pivotal-solver-0.0.2/pivotal/api.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      172 2023-06-24 13:33:47.000000 pivotal-solver-0.0.2/pivotal/errors.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6460 2023-06-24 13:36:24.000000 pivotal-solver-0.0.2/pivotal/simplex.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:47:51.140971 pivotal-solver-0.0.2/pivotal_solver.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5560 2023-06-24 15:47:51.000000 pivotal-solver-0.0.2/pivotal_solver.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      457 2023-06-24 15:47:51.000000 pivotal-solver-0.0.2/pivotal_solver.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-06-24 15:47:51.000000 pivotal-solver-0.0.2/pivotal_solver.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       44 2023-06-24 15:47:51.000000 pivotal-solver-0.0.2/pivotal_solver.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        8 2023-06-24 15:47:51.000000 pivotal-solver-0.0.2/pivotal_solver.egg-info/top_level.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1387 2023-06-24 15:39:54.000000 pivotal-solver-0.0.2/pyproject.toml
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:47:51.144971 pivotal-solver-0.0.2/resources/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   468869 2023-06-24 13:09:14.000000 pivotal-solver-0.0.2/resources/2_Simplex.pdf
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)  2807945 2023-06-16 22:01:01.000000 pivotal-solver-0.0.2/resources/cvut_fel_opt.pdf
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   677438 2023-06-24 13:09:14.000000 pivotal-solver-0.0.2/resources/mitocw.pdf
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-06-24 15:47:51.148971 pivotal-solver-0.0.2/setup.cfg
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-06-24 15:47:51.144971 pivotal-solver-0.0.2/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4460 2023-06-24 13:26:24.000000 pivotal-solver-0.0.2/tests/test_api.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4668 2023-06-24 13:09:14.000000 pivotal-solver-0.0.2/tests/test_simplex.py
```

### Comparing `pivotal-solver-0.0.1/LICENSE` & `pivotal-solver-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.1/PKG-INFO` & `pivotal-solver-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pivotal-solver
-Version: 0.0.1
+Version: 0.0.2
 Summary: High-level Linear Programming solver using the Simplex algorithm
 Author-email: Tomas Roun <tomas.roun8@gmail.com>
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -73,15 +73,15 @@
 ## Installation
 
 Python >=3.10 is required.
 
 Install via pip:
 
 ```bash
-pip install pivotal
+pip install pivotal-solver
 ```
 
 ## API
 
 ### Variables
 
 `Variable` instances implement `__add__`, `__sub__` and other magic methods, so you can use them directly in expressions such as `2*x + 10 - y`.
```

### Comparing `pivotal-solver-0.0.1/README.md` & `pivotal-solver-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ## Installation
 
 Python >=3.10 is required.
 
 Install via pip:
 
 ```bash
-pip install pivotal
+pip install pivotal-solver
 ```
 
 ## API
 
 ### Variables
 
 `Variable` instances implement `__add__`, `__sub__` and other magic methods, so you can use them directly in expressions such as `2*x + 10 - y`.
```

### Comparing `pivotal-solver-0.0.1/logo.svg` & `pivotal-solver-0.0.2/logo.svg`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.1/pivotal/api.py` & `pivotal-solver-0.0.2/pivotal/api.py`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.1/pivotal/simplex.py` & `pivotal-solver-0.0.2/pivotal/simplex.py`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.1/pivotal_solver.egg-info/PKG-INFO` & `pivotal-solver-0.0.2/pivotal_solver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pivotal-solver
-Version: 0.0.1
+Version: 0.0.2
 Summary: High-level Linear Programming solver using the Simplex algorithm
 Author-email: Tomas Roun <tomas.roun8@gmail.com>
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -73,15 +73,15 @@
 ## Installation
 
 Python >=3.10 is required.
 
 Install via pip:
 
 ```bash
-pip install pivotal
+pip install pivotal-solver
 ```
 
 ## API
 
 ### Variables
 
 `Variable` instances implement `__add__`, `__sub__` and other magic methods, so you can use them directly in expressions such as `2*x + 10 - y`.
```

### Comparing `pivotal-solver-0.0.1/pyproject.toml` & `pivotal-solver-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.1/resources/2_Simplex.pdf` & `pivotal-solver-0.0.2/resources/2_Simplex.pdf`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.1/resources/cvut_fel_opt.pdf` & `pivotal-solver-0.0.2/resources/cvut_fel_opt.pdf`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.1/resources/mitocw.pdf` & `pivotal-solver-0.0.2/resources/mitocw.pdf`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.1/tests/test_api.py` & `pivotal-solver-0.0.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pivotal-solver-0.0.1/tests/test_simplex.py` & `pivotal-solver-0.0.2/tests/test_simplex.py`

 * *Files identical despite different names*

