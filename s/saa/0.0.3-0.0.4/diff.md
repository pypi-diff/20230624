# Comparing `tmp/saa-0.0.3.tar.gz` & `tmp/saa-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saa-0.0.3.tar", max compression
+gzip compressed data, was "saa-0.0.4.tar", max compression
```

## Comparing `saa-0.0.3.tar` & `saa-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1079 2023-06-16 19:40:27.482541 saa-0.0.3/LICENSE
--rw-r--r--   0        0        0     3248 2023-06-16 19:40:27.482541 saa-0.0.3/README.md
--rw-r--r--   0        0        0      441 2023-06-16 19:40:27.482541 saa-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      125 2023-06-16 19:40:27.482541 saa-0.0.3/saa/__init__.py
--rw-r--r--   0        0        0     1149 2023-06-16 19:40:27.482541 saa-0.0.3/saa/clock.py
--rw-r--r--   0        0        0        0 2023-06-16 19:40:27.482541 saa-0.0.3/saa/core/__init__.py
--rw-r--r--   0        0        0      575 2023-06-16 19:40:27.482541 saa-0.0.3/saa/core/language.py
--rw-r--r--   0        0        0      837 2023-06-16 19:40:27.482541 saa-0.0.3/saa/core/numbers.py
--rw-r--r--   0        0        0      308 2023-06-16 19:40:27.482541 saa-0.0.3/saa/core/plugins.py
--rw-r--r--   0        0        0      620 2023-06-16 19:40:27.482541 saa-0.0.3/saa/core/template.py
--rw-r--r--   0        0        0      827 2023-06-16 19:40:27.482541 saa-0.0.3/saa/core/watch.py
--rw-r--r--   0        0        0     1513 2023-06-16 19:40:27.482541 saa-0.0.3/saa/luga/da/__init__.py
--rw-r--r--   0        0        0     1370 2023-06-16 19:40:27.482541 saa-0.0.3/saa/luga/en/__init__.py
--rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 saa-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-24 14:10:16.329917 saa-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7699 2023-06-24 14:10:16.329917 saa-0.0.4/README.md
+-rw-r--r--   0        0        0      561 2023-06-24 14:10:16.329917 saa-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-06-24 14:10:16.329917 saa-0.0.4/saa/__init__.py
+-rw-r--r--   0        0        0     1519 2023-06-24 14:10:16.329917 saa-0.0.4/saa/clock.py
+-rw-r--r--   0        0        0        0 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/__init__.py
+-rw-r--r--   0        0        0      662 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/language.py
+-rw-r--r--   0        0        0      837 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/numbers.py
+-rw-r--r--   0        0        0      308 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/plugins.py
+-rw-r--r--   0        0        0      644 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/template.py
+-rw-r--r--   0        0        0      827 2023-06-24 14:10:16.329917 saa-0.0.4/saa/core/watch.py
+-rw-r--r--   0        0        0     1599 2023-06-24 14:10:16.329917 saa-0.0.4/saa/luga/da/__init__.py
+-rw-r--r--   0        0        0     1434 2023-06-24 14:10:16.329917 saa-0.0.4/saa/luga/en/__init__.py
+-rw-r--r--   0        0        0     2186 2023-06-24 14:10:16.329917 saa-0.0.4/saa/luga/sw/__init__.py
+-rw-r--r--   0        0        0     8191 1970-01-01 00:00:00.000000 saa-0.0.4/PKG-INFO
```

### Comparing `saa-0.0.3/LICENSE` & `saa-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `saa-0.0.3/saa/core/language.py` & `saa-0.0.4/saa/core/language.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from abc import abstractmethod, ABC, abstractproperty
 from dataclasses import dataclass
 
 
 @dataclass
 class Luga(ABC):
     @abstractproperty
-    def time(self):
+    def time(self) -> dict:
         pass
 
     @abstractproperty
-    def number_connector(self):
+    def number_connector(self) -> str:
         pass
 
     @abstractproperty
-    def connect_format(self):
+    def connect_format(self) -> str:
         pass
 
     @abstractproperty
-    def numbers(self):
+    def numbers(self) -> dict[int, str]:
         pass
 
     @abstractmethod
-    def time_logic(self):
+    def time_logic(hour: int, minute: int) -> tuple[int, int, str, str]:
         pass
 
     @abstractmethod
     def post_logic(text: str) -> str:
         pass
```

### Comparing `saa-0.0.3/saa/core/numbers.py` & `saa-0.0.4/saa/core/numbers.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.3/saa/core/watch.py` & `saa-0.0.4/saa/core/watch.py`

 * *Files identical despite different names*

### Comparing `saa-0.0.3/saa/luga/da/__init__.py` & `saa-0.0.4/saa/luga/da/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 from saa.core.language import Luga
 
 
-@dataclass
+@dataclass(init=False, eq=False, repr=False, frozen=False)
 class Danish(Luga):
     time = {
-        "to": "{minute} is_minutes i {hour}",
-        "past": "{minute} is_minutes over {hour}",
+        "to": "{minute} time_indicator i {hour}",
+        "past": "{minute} time_indicator over {hour}",
         0: "klokken {hour}",
         15: "kvart over {hour}",
         45: "kvart i {hour}",
         30: "halv{hour}",
     }
 
     number_connector = "og"
@@ -39,26 +39,26 @@
         20: "tyve",
         30: "tredive",
         40: "fyrre",
         50: "halvtreds",
     }
 
     @staticmethod
-    def time_logic(hour, minute) -> tuple[int, int, str, str]:
+    def time_logic(hour: int, minute: int) -> tuple[int, int, str, str]:
         is_to = "to" if minute >= 30 else "past"
-        is_minutes = "minutter" if minute > 1 else "minut"
+        time_indicator = "minutter" if minute > 1 else "minut"
 
         if is_to == "to":
             hour += 1
             minute = 60 - minute
 
-        return hour, minute, is_to, is_minutes
+        return hour, minute, is_to, time_indicator
 
     @staticmethod
-    def post_logic(text):
+    def post_logic(text: str) -> str:
         text = " ".join(
             word.replace("en", "et")
             if (word.startswith("halv") or word == "en")
             else word
             for word in text.split()
         )
         return text
```

### Comparing `saa-0.0.3/saa/luga/en/__init__.py` & `saa-0.0.4/saa/luga/en/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 from saa.core.language import Luga
 
 
-@dataclass
+@dataclass(init=False, eq=False, repr=False, frozen=False)
 class English(Luga):
     time = {
-        "to": "{minute} is_minutes to {hour}",
-        "past": "{minute} is_minutes past {hour}",
+        "to": "{minute} time_indicator to {hour}",
+        "past": "{minute} time_indicator past {hour}",
         0: "{hour} o'clock",
         15: "quarter past {hour}",
         45: "quarter to {hour}",
         30: "half past {hour}",
     }
     number_connector = "and"
     connect_format = "{0} {2}"
@@ -40,21 +40,21 @@
         40: "forty",
         50: "fifty",
     }
 
     @staticmethod
     def time_logic(hour, minute) -> tuple[int, int, str, str]:
         is_to = "to" if minute > 30 else "past"
-        is_minutes = "minutes" if minute > 1 else "minute"
+        time_indicator = "minutes" if minute > 1 else "minute"
 
         if is_to == "to":
             hour += 1
             minute = 60 - minute
 
-        return hour, minute, is_to, is_minutes
+        return hour, minute, is_to, time_indicator
 
     @staticmethod
     def post_logic(text: str) -> str:
         return text
 
 
 class Language(English):
```

