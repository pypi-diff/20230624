# Comparing `tmp/fictional_names-0.0.3.tar.gz` & `tmp/fictional_names-0.0.4.tar.gz`

## Comparing `fictional_names-0.0.3.tar` & `fictional_names-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fictional_names-0.0.3/LISENCE
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/.gitignore
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/dwarven.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/elven.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/giant.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/halfling.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_arab.py
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_erikson.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_greek.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_jordan.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_medieval.py
--rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_modern.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_norsemen.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_oriental.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_rowling.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_sapkowski.py
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_steampunk.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/human_tolkien.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/main.py
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/name_generator.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/orc.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/supportive_functions.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fictional_names-0.0.3/src/fictional_names/.vscode/settings.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fictional_names-0.0.3/README.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fictional_names-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fictional_names-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fictional_names-0.0.4/LISENCE
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/.gitignore
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/dwarven.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/elven.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/giant.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/halfling.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_arab.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_erikson.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_greek.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_jordan.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_medieval.py
+-rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_modern.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_norsemen.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_oriental.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_rowling.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_sapkowski.py
+-rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_steampunk.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/human_tolkien.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/main.py
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/name_generator.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/orc.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/supportive_functions.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fictional_names-0.0.4/src/fictional_names/.vscode/settings.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fictional_names-0.0.4/README.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fictional_names-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fictional_names-0.0.4/PKG-INFO
```

### Comparing `fictional_names-0.0.3/LISENCE` & `fictional_names-0.0.4/LISENCE`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.3/src/fictional_names/.gitignore` & `fictional_names-0.0.4/src/fictional_names/.gitignore`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.3/src/fictional_names/dwarven.py` & `fictional_names-0.0.4/src/fictional_names/dwarven.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname
 
 
 female_prefix = [
     "bal", "da", "din", "dur", "fal", "gim", "gin", "gor", "hel", "in", "kil", "li", "mha", "na",
     "nin", "ran", "sha", "thor", "tha", "zin"
 ]
```

### Comparing `fictional_names-0.0.3/src/fictional_names/elven.py` & `fictional_names-0.0.4/src/fictional_names/elven.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname
 
 
 female_prefix = [
     "ael", "al", "an", "ar", "cal", "dael", "el", "er", "fae", "fal", "fi", "gal", "gil", "glor",
     "hal", "ia", "id", "il", "im", "in", "laer", "lan", "leg", "li", "lind", "lith", "lor", "mae",
     "mel", "na", "nar", "nen", "ner", "or", "pe", "ran", "rhov", "sae", "saer", "se", "sil", "ta",
     "thal", "thar", "thing", "ti", "tir", "val", "ví", "yar", "zeph", "zim"
```

### Comparing `fictional_names-0.0.3/src/fictional_names/giant.py` & `fictional_names-0.0.4/src/fictional_names/giant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname_less
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname_less
 
 
 female_prefix = [
     "ar", "bal", "bar", "bran", "dar", "dran", "feth", "gras", "har", "jaf", "kar", "krul",
     "mar", "nar", "par", "rak", "ras", "sar", "tar", "thas", "thul", "war", "yas", "zar"
 ]
```

### Comparing `fictional_names-0.0.3/src/fictional_names/halfling.py` & `fictional_names-0.0.4/src/fictional_names/halfling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname_less
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname_less
 
 
 female_prefix = [
     "ber", "bri", "cla", "cor", "dal", "dor", "el", "fro", "gol", "har", "hil", "lav", "lil", "lo",
     "mar", "mel", "nar", "nor", "ol", "per", "pip", "ro", "sam", "san", "syl", "tas", "wil",
 ]
```

### Comparing `fictional_names-0.0.3/src/fictional_names/human_arab.py` & `fictional_names-0.0.4/src/fictional_names/human_arab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname_less
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname_less
 
 
 female_prefix = [
     "aisha", "amal", "asra", "bahia", "dalila", "esma", "fadia", "ghada", "hala", "jalila",
     "kamila", "laila", "maha", "nadia", "omaira", "rabia", "sabah", "tamara", "yasmin", "zahra"
 ]
```

### Comparing `fictional_names-0.0.3/src/fictional_names/human_erikson.py` & `fictional_names-0.0.4/src/fictional_names/human_erikson.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname
 
 
 female_suffix = [
     "a", "bel", "cia", "da", "el", "fae", "gwyn", "hia", "i", "ja", "ka", "la", "ma", "na", "ora", "pa",
     "qua", "ra", "sa", "ta", "ula", "va", "wa", "xa", "ya", "za",
     "belle", "cey", "dine", "elle", "finn", "grace", "hira", "ira", "jade", "kara", "lynn", "mara", "nora",
     "opal", "phina", "quella", "rina", "sera", "tia", "una", "vella", "wren", "xina", "yara", "zara"
```

### Comparing `fictional_names-0.0.3/src/fictional_names/human_greek.py` & `fictional_names-0.0.4/src/fictional_names/human_greek.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from random import choice
-from supportive_functions import generate_female_name, generate_male_name
+from .supportive_functions import generate_female_name, generate_male_name
 
 
 female_prefix = [
     "agá", "aléx", "amphí", "aná", "arí", "athén", "démé", "élektr", "eurydí", "euthén", "galát",
     "harmón", "hébé", "hér", "kalí", "kleió", "kyprí", "lét", "méliss", "nér", "orestí", "pandór",
     "penél", "perí", "philómél", "pó", "thál", "théod", "xén"
 ]
```

### Comparing `fictional_names-0.0.3/src/fictional_names/human_jordan.py` & `fictional_names-0.0.4/src/fictional_names/human_jordan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname_less
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname_less
 
 
 female_prefix = [
     "aer", "ash", "bri", "cer", "daen", "ela", "for", "gwe", "hel", "iri", "jen", "kal", "lyn",
     "mel", "ny", "oth", "pae", "qua", "rin", "san", "the", "uil", "val", "wyr", "xan", "yen", "zoe"
 ]
```

### Comparing `fictional_names-0.0.3/src/fictional_names/human_medieval.py` & `fictional_names-0.0.4/src/fictional_names/human_medieval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from random import choice
-from supportive_functions import generate_surname_less
+from .supportive_functions import generate_surname_less
 
 
 female_names = [
     "Adelaide",
     "Adriana",
     "Amara",
     "Amaryllis",
```

### Comparing `fictional_names-0.0.3/src/fictional_names/human_modern.py` & `fictional_names-0.0.4/src/fictional_names/human_modern.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.3/src/fictional_names/human_norsemen.py` & `fictional_names-0.0.4/src/fictional_names/human_norsemen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname_less
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname_less
 
 
 female_prefix = [
     "aða", "æl", "arn", "björn", "dís", "eið", "ey", "fríð", "gud", "gull", "gyð", "hild", "hjör",
     "ing", "líf", "run", "sif", "skjald", "skuld", "sól", "thor", "val", "víg", "ygg"
 ]
```

### Comparing `fictional_names-0.0.3/src/fictional_names/human_oriental.py` & `fictional_names-0.0.4/src/fictional_names/human_oriental.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname_less
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname_less
 
 
 female_prefix = [
     "ai", "an", "bo", "chi", "da", "en", "fu", "go", "ha", "hi", "i", "ka", "ko", "mi", "na",
     "no", "ra", "ri", "sa", "shi", "ta", "to", "tsu", "u", "ya", "yo", "zu"
 ]
```

### Comparing `fictional_names-0.0.3/src/fictional_names/human_rowling.py` & `fictional_names-0.0.4/src/fictional_names/human_rowling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname_less
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname_less
 
 
 female_prefix = [
     "ada", "al", "am", "an", "bel", "beth", "ca", "ce", "cha", "da", "de", "dra", "ela", "el", "ema",
     "en", "fa", "fay", "ga", "ge", "gi", "ha", "he", "hi", "ila", "il", "ima", "in", "ja", "je", "ka",
     "ke", "ki", "la", "le", "li", "ma", "me", "mi", "na", "ne", "ni", "ola", "ol", "oma", "pa", "pe",
     "pi", "qua", "ra", "re", "ri", "sa", "se", "sha", "ta", "te", "tha", "u", "va", "ve", "vi", "wa",
```

### Comparing `fictional_names-0.0.3/src/fictional_names/human_sapkowski.py` & `fictional_names-0.0.4/src/fictional_names/human_sapkowski.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname_less
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname_less
 
 
 female_prefix = [
     "cer", "cy", "dan", "el", "es", "fi", "gwen", "is", "jil", "ka", "la", "me", "nes", "phi", "que",
     "ri", "sha", "tri", "va", "wen", "xi", "ya", "zel"
 ]
```

### Comparing `fictional_names-0.0.3/src/fictional_names/human_steampunk.py` & `fictional_names-0.0.4/src/fictional_names/human_steampunk.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.3/src/fictional_names/human_tolkien.py` & `fictional_names-0.0.4/src/fictional_names/human_tolkien.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from supportive_functions import generate_female_name, generate_male_name, generate_surname_less
+from .supportive_functions import generate_female_name, generate_male_name, generate_surname_less
 
 
 male_prefix = [
     "aer", "ald", "an", "ar", "bar", "bor", "cal", "dal", "dan", "dur", "ed", "eld", "er", "fal",
     "fin", "gal", "gan", "gar", "had", "hal", "ian", "in", "kar", "kor", "lanc", "mar", "mer",
     "nor", "or", "rad", "ran", "ron", "sar", "sol", "tan", "thor", "tor", "ul", "val", "van",
     "vor", "wal", "war", "yor", "zar"
```

### Comparing `fictional_names-0.0.3/src/fictional_names/name_generator.py` & `fictional_names-0.0.4/src/fictional_names/name_generator.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.3/src/fictional_names/orc.py` & `fictional_names-0.0.4/src/fictional_names/orc.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.3/src/fictional_names/supportive_functions.py` & `fictional_names-0.0.4/src/fictional_names/supportive_functions.py`

 * *Files identical despite different names*

### Comparing `fictional_names-0.0.3/pyproject.toml` & `fictional_names-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fictional_names"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="a-tsagkalidis", email="arg.tsag@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `fictional_names-0.0.3/PKG-INFO` & `fictional_names-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fictional_names
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: a-tsagkalidis <arg.tsag@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

