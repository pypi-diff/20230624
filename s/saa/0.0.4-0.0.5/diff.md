# Comparing `tmp/saa-0.0.4.tar.gz` & `tmp/saa-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saa-0.0.4.tar", max compression
+gzip compressed data, was "saa-0.0.5.tar", max compression
```

## Comparing `saa-0.0.4.tar` & `saa-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1079 2023-06-24 14:10:16.329917 saa-0.0.4/LICENSE
--rw-r--r--   0        0        0     7699 2023-06-24 14:10:16.329917 saa-0.0.4/README.md
--rw-r--r--   0        0        0      561 2023-06-24 14:10:16.329917 saa-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      125 2023-06-24 14:10:16.329917 saa-0.0.4/saa/__init__.py
--rw-r--r--   0        0        0     1519 2023-06-24 14:10:16.329917 saa-0.0.4/saa/clock.py
--rw-r--r--   0        0        0        0 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/__init__.py
--rw-r--r--   0        0        0      662 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/language.py
--rw-r--r--   0        0        0      837 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/numbers.py
--rw-r--r--   0        0        0      308 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/plugins.py
--rw-r--r--   0        0        0      644 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/template.py
--rw-r--r--   0        0        0      827 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/watch.py
--rw-r--r--   0        0        0     1599 2023-06-24 14:10:16.329917 saa-0.0.4/saa/luga/da/__init__.py
--rw-r--r--   0        0        0     1434 2023-06-24 14:10:16.329917 saa-0.0.4/saa/luga/en/__init__.py
--rw-r--r--   0        0        0     2186 2023-06-24 14:10:16.329917 saa-0.0.4/saa/luga/sw/__init__.py
--rw-r--r--   0        0        0     8191 1970-01-01 00:00:00.000000 saa-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-24 14:38:26.102207 saa-0.0.5/LICENSE
+-rw-r--r--   0        0        0     7699 2023-06-24 14:38:26.102207 saa-0.0.5/README.md
+-rw-r--r--   0        0        0      561 2023-06-24 14:38:26.102207 saa-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-06-24 14:38:26.102207 saa-0.0.5/saa/__init__.py
+-rw-r--r--   0        0        0     1519 2023-06-24 14:38:26.102207 saa-0.0.5/saa/clock.py
+-rw-r--r--   0        0        0        0 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/__init__.py
+-rw-r--r--   0        0        0      662 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/language.py
+-rw-r--r--   0        0        0      837 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/numbers.py
+-rw-r--r--   0        0        0      308 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/plugins.py
+-rw-r--r--   0        0        0      644 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/template.py
+-rw-r--r--   0        0        0      827 2023-06-24 14:38:26.102207 saa-0.0.5/saa/core/watch.py
+-rw-r--r--   0        0        0     1599 2023-06-24 14:38:26.102207 saa-0.0.5/saa/luga/da/__init__.py
+-rw-r--r--   0        0        0     1434 2023-06-24 14:38:26.102207 saa-0.0.5/saa/luga/en/__init__.py
+-rw-r--r--   0        0        0     2187 2023-06-24 14:38:26.102207 saa-0.0.5/saa/luga/sw/__init__.py
+-rw-r--r--   0        0        0     8191 1970-01-01 00:00:00.000000 saa-0.0.5/PKG-INFO
```

### Comparing `saa-0.0.4/LICENSE` & `saa-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `saa-0.0.4/README.md` & `saa-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `saa-0.0.4/pyproject.toml` & `saa-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saa"
-version = "0.0.4"
+version = "0.0.5"
 description = "Converting time into natural language phrases"
 authors = ["Prayson W. Daniel <praysonpi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.8.5"
```

### Comparing `saa-0.0.4/saa/clock.py` & `saa-0.0.5/saa/clock.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.4/saa/core/language.py` & `saa-0.0.5/saa/core/language.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.4/saa/core/numbers.py` & `saa-0.0.5/saa/core/numbers.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.4/saa/core/template.py` & `saa-0.0.5/saa/core/template.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.4/saa/core/watch.py` & `saa-0.0.5/saa/core/watch.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.4/saa/luga/da/__init__.py` & `saa-0.0.5/saa/luga/da/__init__.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.4/saa/luga/en/__init__.py` & `saa-0.0.5/saa/luga/en/__init__.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.4/saa/luga/sw/__init__.py` & `saa-0.0.5/saa/luga/sw/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 from saa.core.language import Luga
 
 
 @dataclass(init=False, eq=False, repr=False, frozen=False)
 class Swahili(Luga):
     time = {
-        "to": "saa {hour} na dakika {minute} time_indicator",
-        "past": "saa {hour} kasoro dakika {minute}time_indicator",
+        "to": "saa {hour} kasoro dakika {minute} time_indicator",
+        "past": "saa {hour} na dakika {minute} time_indicator",
         0: "saa {hour} time_indicator",
         15: "saa {hour} na robo time_indicator",
         45: "saa {hour} kasorobo time_indicator",
         30: "saa {hour} na nusu time_indicator",
     }
 
     number_connector = "na"
```

### Comparing `saa-0.0.4/PKG-INFO` & `saa-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saa
-Version: 0.0.4
+Version: 0.0.5
 Summary: Converting time into natural language phrases
 License: MIT
 Author: Prayson W. Daniel
 Author-email: praysonpi@gmail.com
 Requires-Python: >3.8.5
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

