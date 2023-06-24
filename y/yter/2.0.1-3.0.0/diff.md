# Comparing `tmp/yter-2.0.1.tar.gz` & `tmp/yter-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yter-2.0.1.tar", last modified: Thu Mar  9 15:10:32 2023, max compression
+gzip compressed data, was "yter-3.0.0.tar", last modified: Sat Jun 24 02:17:15 2023, max compression
```

## Comparing `yter-2.0.1.tar` & `yter-3.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 15:10:32.670249 yter-2.0.1/
--rw-rw-rw-   0        0        0     1081 2023-03-09 15:02:41.000000 yter-2.0.1/LICENSE
--rw-rw-rw-   0        0        0       18 2023-03-09 15:02:41.000000 yter-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2521 2023-03-09 15:10:32.669247 yter-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-03-09 15:05:17.000000 yter-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-09 15:10:32.670249 yter-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      926 2023-03-09 15:02:41.000000 yter-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:10:32.644857 yter-2.0.1/test/
--rw-rw-rw-   0        0        0     3838 2023-03-09 15:02:41.000000 yter-2.0.1/test/test_fun.py
--rw-rw-rw-   0        0        0     1294 2023-03-09 15:02:41.000000 yter-2.0.1/test/test_key.py
--rw-rw-rw-   0        0        0      158 2023-03-09 15:02:41.000000 yter-2.0.1/test/test_star.py
--rw-rw-rw-   0        0        0     1432 2023-03-09 15:02:41.000000 yter-2.0.1/test/test_ytr.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:10:32.649202 yter-2.0.1/yter/
--rw-rw-rw-   0        0        0      406 2023-03-09 15:02:41.000000 yter-2.0.1/yter/__init__.py
--rw-rw-rw-   0        0        0     7667 2023-03-09 15:02:41.000000 yter-2.0.1/yter/_fun.py
--rw-rw-rw-   0        0        0     3538 2023-03-09 15:03:45.000000 yter-2.0.1/yter/_key.py
--rw-rw-rw-   0        0        0     3974 2023-03-09 15:02:41.000000 yter-2.0.1/yter/_ytr.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:10:32.668713 yter-2.0.1/yter.egg-info/
--rw-rw-rw-   0        0        0     2521 2023-03-09 15:10:32.000000 yter-2.0.1/yter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-03-09 15:10:32.000000 yter-2.0.1/yter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 15:10:32.000000 yter-2.0.1/yter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-03-09 15:10:32.000000 yter-2.0.1/yter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 15:10:32.000000 yter-2.0.1/yter.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-24 02:17:15.428684 yter-3.0.0/
+-rw-rw-rw-   0        0        0     1081 2023-03-09 15:02:41.000000 yter-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-03-09 15:02:41.000000 yter-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2519 2023-06-24 02:17:15.427698 yter-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1874 2023-06-24 02:08:31.000000 yter-3.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 02:17:15.428684 yter-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      926 2023-03-09 15:02:41.000000 yter-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:17:15.405369 yter-3.0.0/test/
+-rw-rw-rw-   0        0        0     3893 2023-05-29 14:39:48.000000 yter-3.0.0/test/test_fun.py
+-rw-rw-rw-   0        0        0     1287 2023-06-14 05:23:52.000000 yter-3.0.0/test/test_key.py
+-rw-rw-rw-   0        0        0      158 2023-03-09 15:02:41.000000 yter-3.0.0/test/test_star.py
+-rw-rw-rw-   0        0        0     2142 2023-06-22 03:20:01.000000 yter-3.0.0/test/test_ytr.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:17:15.410013 yter-3.0.0/yter/
+-rw-rw-rw-   0        0        0      419 2023-06-14 05:20:37.000000 yter-3.0.0/yter/__init__.py
+-rw-rw-rw-   0        0        0    11952 2023-06-22 02:44:16.000000 yter-3.0.0/yter/_fun.py
+-rw-rw-rw-   0        0        0     4692 2023-06-22 02:46:02.000000 yter-3.0.0/yter/_key.py
+-rw-rw-rw-   0        0        0     7960 2023-06-22 03:17:54.000000 yter-3.0.0/yter/_ytr.py
+drwxrwxrwx   0        0        0        0 2023-06-24 02:17:15.424689 yter-3.0.0/yter.egg-info/
+-rw-rw-rw-   0        0        0     2519 2023-06-24 02:17:15.000000 yter-3.0.0/yter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-24 02:17:15.000000 yter-3.0.0/yter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 02:17:15.000000 yter-3.0.0/yter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-24 02:17:15.000000 yter-3.0.0/yter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 15:10:32.000000 yter-3.0.0/yter.egg-info/zip-safe
```

### Comparing `yter-2.0.1/LICENSE` & `yter-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yter-2.0.1/PKG-INFO` & `yter-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yter
-Version: 2.0.1
+Version: 3.0.0
 Summary: Clever, quick iterators that make your smile whiter
 Home-page: https://gitlab.com/shredwheat/yter
 Author: Peter Shinners
 Author-email: pete@shinners.org
 License: MIT
 Keywords: iterator itertools
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,21 +13,20 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 # yter
 
-Version 2.0.1
-2023, March 9
+Version 3.0.0
+2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
-This will work with versions of Python 2.6+ and 3.2+. The tests also pass with
-recent Pypy and Jython releases.
+This will work with versions of Python 2.6+ and 3.2+.
 
 
 ## Functions
 
 There are many functions that process data from iterators in efficient ways.
 
 * `yany` -- Extended version of the builtin any, test if any values are true
@@ -35,34 +34,35 @@
 * `ylen` -- Complete an iterator and get number of values
 * `first` -- Get the first value from an iteraterable
 * `last` -- Get the final value from an iteraterable
 * `head` -- Get the first values from an iteraterable
 * `tail` -- Get the last values from an iteraterable
 * `minmax` -- Find the minimum and maximum values from an iterable
 * `isiter` -- Test if an object is iterable, but not a string type
-* `sequence` -- Efficient copy of non sequence data
+* `uniter` -- Efficient copy of non sequence data
 * `repeat` -- Efficient lazy copy of non sequence data
 
 
 ## Iterators
 
 There are several iterators that wrap an existing iterator and process it's output.
 
 * `call` -- Iterator that works with mixed callable types
 * `percent` -- Iterator that skips a percentage of values
 * `flat` -- Iterator of values from a iterable of iterators
 * `chunk` -- Iterator of lists with a fixed size from iterable
 * `key` -- Iterator of pairs of key result and original values
+* `choose` -- Split into iterators for true and false values
 * `unique` -- Iterate only the unique values
 * `duplicates` -- Iterate only the duplicated values
 
 
 ## Keys
 
 Utility functions that are useful to use as a key argument
 
-* `formatter` -- Create a function that formats given values into strings
+* `format` -- Create a function that formats given values into strings
 * `numeric` -- Split a string into string and integer sections
 * `getter` -- Shorthand for attrgetter, itemgetter, and methodcaller operators
 
 
 [More documentation](https://gitlab.com/shredwheat/yter/blob/master/docs/docs/index.md) found in the repository.
```

### Comparing `yter-2.0.1/README.md` & `yter-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # yter
 
-Version 2.0.1
-2023, March 9
+Version 3.0.0
+2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
-This will work with versions of Python 2.6+ and 3.2+. The tests also pass with
-recent Pypy and Jython releases.
+This will work with versions of Python 2.6+ and 3.2+.
 
 
 ## Functions
 
 There are many functions that process data from iterators in efficient ways.
 
 * `yany` -- Extended version of the builtin any, test if any values are true
@@ -18,34 +17,35 @@
 * `ylen` -- Complete an iterator and get number of values
 * `first` -- Get the first value from an iteraterable
 * `last` -- Get the final value from an iteraterable
 * `head` -- Get the first values from an iteraterable
 * `tail` -- Get the last values from an iteraterable
 * `minmax` -- Find the minimum and maximum values from an iterable
 * `isiter` -- Test if an object is iterable, but not a string type
-* `sequence` -- Efficient copy of non sequence data
+* `uniter` -- Efficient copy of non sequence data
 * `repeat` -- Efficient lazy copy of non sequence data
 
 
 ## Iterators
 
 There are several iterators that wrap an existing iterator and process it's output.
 
 * `call` -- Iterator that works with mixed callable types
 * `percent` -- Iterator that skips a percentage of values
 * `flat` -- Iterator of values from a iterable of iterators
 * `chunk` -- Iterator of lists with a fixed size from iterable
 * `key` -- Iterator of pairs of key result and original values
+* `choose` -- Split into iterators for true and false values
 * `unique` -- Iterate only the unique values
 * `duplicates` -- Iterate only the duplicated values
 
 
 ## Keys
 
 Utility functions that are useful to use as a key argument
 
-* `formatter` -- Create a function that formats given values into strings
+* `format` -- Create a function that formats given values into strings
 * `numeric` -- Split a string into string and integer sections
 * `getter` -- Shorthand for attrgetter, itemgetter, and methodcaller operators
 
 
 [More documentation](https://gitlab.com/shredwheat/yter/blob/master/docs/docs/index.md) found in the repository.
```

### Comparing `yter-2.0.1/setup.py` & `yter-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `yter-2.0.1/test/test_fun.py` & `yter-3.0.0/test/test_fun.py`

 * *Files 14% similar despite different names*

```diff
@@ -104,43 +104,44 @@
     assert yter.isiter([1])
     assert yter.isiter(range(1))
 
     assert not yter.isiter(None)
     assert not yter.isiter(9)
     assert not yter.isiter("")
     assert not yter.isiter("a")
+    assert not yter.isiter(Exception("Failure"))
 
     assert yter.isiter(itertools.chain((1,)))
 
 
-def test_sequence():
+def test_uniter():
     l = [1, 2]
-    assert yter.sequence(l) is l
+    assert yter.uniter(l) is l
 
     il = iter(l)
-    assert yter.sequence(il) is not il
+    assert yter.uniter(il) is not il
 
     d = {1: 1, 2: 2}
-    assert yter.sequence(d) is d
+    assert yter.uniter(d) is d
 
     c = itertools.chain((1,))
-    assert yter.sequence(c) is not c
+    assert yter.uniter(c) is not c
 
     _xrange = __builtins__.get("xrange", __builtins__["range"])
     x = _xrange(3)
-    assert yter.sequence(x) is x
+    assert yter.uniter(x) is x
 
     f = open(__file__, "rb")
-    assert yter.sequence(f) is not f
+    assert yter.uniter(f) is not f
 
 
-def test_repeat():
+def test_repeatable():
     a = [1, 2, 3]
-    assert yter.repeat(a) is a
+    assert yter.repeatable(a) is a
     b = dict.fromkeys(a)
-    assert yter.repeat(b) is b
+    assert yter.repeatable(b) is b
     c = itertools.chain(a)
-    d = yter.repeat(c)
+    d = yter.repeatable(c)
     assert c is not d
     first = next(iter(d))
     assert list(d) == list(d)
-    assert yter.repeat(d) is d
+    assert yter.repeatable(d) is d
```

### Comparing `yter-2.0.1/test/test_key.py` & `yter-3.0.0/test/test_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pytest
 import yter
 
 
-def test_formatter():
-    assert yter.formatter("val")(None) == "val"
-    assert yter.formatter("{0:3d}")(22) == " 22"
-    assert yter.formatter("{it}", it=True)(False) == "True"
+def test_format():
+    assert yter.format("val")(None) == "val"
+    assert yter.format("{0:3d}")(22) == " 22"
+    assert yter.format("{it}", it=True)(False) == "True"
     with pytest.raises(IndexError):
-        yter.formatter("{1}")("one")
+        yter.format("{1}")("one")
 
 
 def test_numeric():
     assert yter.numeric("one2three") == ("one", 2, "three")
     assert yter.numeric("one-2three") == ("one", -2, "three")
-    assert yter.numeric("1two3") == (1, "two", 3)
-    assert yter.numeric("88") == (88,)
+    assert yter.numeric("1two3") == ("", 1, "two", 3)
+    assert yter.numeric("88") == ("", 88,)
     assert yter.numeric("eight-eight") == ("eight-eight",)
     assert yter.numeric("eight-") == ("eight-",)
     assert yter.numeric("-") == ("-",)
     assert yter.numeric("") == ()
 
 
 def test_getter():
```

### Comparing `yter-2.0.1/yter.egg-info/PKG-INFO` & `yter-3.0.0/yter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yter
-Version: 2.0.1
+Version: 3.0.0
 Summary: Clever, quick iterators that make your smile whiter
 Home-page: https://gitlab.com/shredwheat/yter
 Author: Peter Shinners
 Author-email: pete@shinners.org
 License: MIT
 Keywords: iterator itertools
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,21 +13,20 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 # yter
 
-Version 2.0.1
-2023, March 9
+Version 3.0.0
+2023, June 23
 
 Clever, quick iterator functions that make your smile whiter.
 
-This will work with versions of Python 2.6+ and 3.2+. The tests also pass with
-recent Pypy and Jython releases.
+This will work with versions of Python 2.6+ and 3.2+.
 
 
 ## Functions
 
 There are many functions that process data from iterators in efficient ways.
 
 * `yany` -- Extended version of the builtin any, test if any values are true
@@ -35,34 +34,35 @@
 * `ylen` -- Complete an iterator and get number of values
 * `first` -- Get the first value from an iteraterable
 * `last` -- Get the final value from an iteraterable
 * `head` -- Get the first values from an iteraterable
 * `tail` -- Get the last values from an iteraterable
 * `minmax` -- Find the minimum and maximum values from an iterable
 * `isiter` -- Test if an object is iterable, but not a string type
-* `sequence` -- Efficient copy of non sequence data
+* `uniter` -- Efficient copy of non sequence data
 * `repeat` -- Efficient lazy copy of non sequence data
 
 
 ## Iterators
 
 There are several iterators that wrap an existing iterator and process it's output.
 
 * `call` -- Iterator that works with mixed callable types
 * `percent` -- Iterator that skips a percentage of values
 * `flat` -- Iterator of values from a iterable of iterators
 * `chunk` -- Iterator of lists with a fixed size from iterable
 * `key` -- Iterator of pairs of key result and original values
+* `choose` -- Split into iterators for true and false values
 * `unique` -- Iterate only the unique values
 * `duplicates` -- Iterate only the duplicated values
 
 
 ## Keys
 
 Utility functions that are useful to use as a key argument
 
-* `formatter` -- Create a function that formats given values into strings
+* `format` -- Create a function that formats given values into strings
 * `numeric` -- Split a string into string and integer sections
 * `getter` -- Shorthand for attrgetter, itemgetter, and methodcaller operators
 
 
 [More documentation](https://gitlab.com/shredwheat/yter/blob/master/docs/docs/index.md) found in the repository.
```

