# Comparing `tmp/fictional_names-0.0.5.tar.gz` & `tmp/fictional_names-0.0.6.tar.gz`

## Comparing `fictional_names-0.0.5.tar` & `fictional_names-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fictional_names-0.0.5/LISENCE
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/.gitignore
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/dwarven.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/elven.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/giant.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/halfling.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_arab.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_erikson.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_greek.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_jordan.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_medieval.py
--rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_modern.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_norsemen.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_oriental.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_rowling.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_sapkowski.py
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_steampunk.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/human_tolkien.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/main.py
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/name_generator.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/orc.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/supportive_functions.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fictional_names-0.0.5/src/fictional_names/.vscode/settings.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fictional_names-0.0.5/README.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fictional_names-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fictional_names-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fictional_names-0.0.6/LISENCE
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/.gitignore
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/dwarven.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/elven.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/giant.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/halfling.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_arab.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_erikson.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_greek.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_jordan.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_medieval.py
+-rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_modern.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_norsemen.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_oriental.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_rowling.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_sapkowski.py
+-rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_steampunk.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/human_tolkien.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/name_generator.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/orc.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/supportive_functions.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fictional_names-0.0.6/src/fictional_names/.vscode/settings.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fictional_names-0.0.6/README.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fictional_names-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 fictional_names-0.0.6/PKG-INFO
```

### Comparing `fictional_names-0.0.5/LISENCE` & `fictional_names-0.0.6/LISENCE`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/.gitignore` & `fictional_names-0.0.6/src/fictional_names/.gitignore`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/dwarven.py` & `fictional_names-0.0.6/src/fictional_names/dwarven.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/elven.py` & `fictional_names-0.0.6/src/fictional_names/elven.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/giant.py` & `fictional_names-0.0.6/src/fictional_names/giant.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/halfling.py` & `fictional_names-0.0.6/src/fictional_names/halfling.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_arab.py` & `fictional_names-0.0.6/src/fictional_names/human_arab.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_erikson.py` & `fictional_names-0.0.6/src/fictional_names/human_erikson.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_greek.py` & `fictional_names-0.0.6/src/fictional_names/human_greek.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_jordan.py` & `fictional_names-0.0.6/src/fictional_names/human_jordan.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_medieval.py` & `fictional_names-0.0.6/src/fictional_names/human_medieval.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_modern.py` & `fictional_names-0.0.6/src/fictional_names/human_modern.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_norsemen.py` & `fictional_names-0.0.6/src/fictional_names/human_norsemen.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_oriental.py` & `fictional_names-0.0.6/src/fictional_names/human_oriental.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_rowling.py` & `fictional_names-0.0.6/src/fictional_names/human_rowling.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_sapkowski.py` & `fictional_names-0.0.6/src/fictional_names/human_sapkowski.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_steampunk.py` & `fictional_names-0.0.6/src/fictional_names/human_steampunk.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/human_tolkien.py` & `fictional_names-0.0.6/src/fictional_names/human_tolkien.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/name_generator.py` & `fictional_names-0.0.6/src/fictional_names/name_generator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from . import dwarven, elven, giant, halfling, orc, human_steampunk, human_modern, human_medieval, human_greek, human_norsemen, human_arab, human_oriental, human_tolkien, human_jordan, human_erikson, human_rowling, human_sapkowski
+from random import choice
 
-
-def generate_name(gender='male', style='modern'):
+def generate_name(gender=choice(['female', 'male']), style='modern'):
     if gender.lower() == 'male':
         match style:
             case 'elven':
                 name = elven.male
             case 'dwarven':
                 name = dwarven.male
             case 'giant':
@@ -70,18 +70,18 @@
                 name = human_jordan.female
             case 'erikson':
                 name = human_erikson.female
             case 'rowling':
                 name = human_rowling.female
             case 'sapkowski':
                 name = human_sapkowski.female
-            
+
     else:
         raise ValueError("Invalid gender specified. Please choose 'male' or 'female'.")
-    
+
     if style.lower() == 'elven':
         surname = elven.surname
     elif style.lower() == 'dwarven':
         surname = dwarven.surname
     elif style.lower() == 'giant':
         surname = giant.surname
     elif style.lower() == 'halfling':
@@ -108,14 +108,16 @@
         surname = human_jordan.surname
     elif style.lower() == 'erikson':
         surname = human_erikson.surname
     elif style.lower() == 'rowling':
         surname = human_rowling.surname
     elif style.lower() == 'sapkowski':
         surname = human_sapkowski.surname
-    
+    else:
+        raise ValueError("Invalid style specified. Please choose 'elven', 'dwarven', 'giant', 'halfling', 'orc', 'modern', 'greek', 'norsemen', 'arab', 'oriental', 'steampunk', 'medieval', 'tolkien', 'jordan', 'eriskon', 'rowling', or 'sapkowski'.")
+
     return f"{name} {surname}"
 
 
 if __name__ == '__main__':
     name = generate_name()
     print(name)
```

### Comparing `fictional_names-0.0.5/src/fictional_names/orc.py` & `fictional_names-0.0.6/src/fictional_names/orc.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/src/fictional_names/supportive_functions.py` & `fictional_names-0.0.6/src/fictional_names/supportive_functions.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.5/pyproject.toml` & `fictional_names-0.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fictional_names"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="a-tsagkalidis", email="arg.tsag@gmail.com" },
 ]
-description = "A small example package"
+description = "A package for generating fictional names"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `fictional_names-0.0.5/PKG-INFO` & `fictional_names-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fictional_names
-Version: 0.0.5
-Summary: A small example package
+Version: 0.0.6
+Summary: A package for generating fictional names
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: a-tsagkalidis <arg.tsag@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

