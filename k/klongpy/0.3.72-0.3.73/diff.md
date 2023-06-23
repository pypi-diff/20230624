# Comparing `tmp/klongpy-0.3.72.tar.gz` & `tmp/klongpy-0.3.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klongpy-0.3.72.tar", last modified: Fri Jun 23 22:40:40 2023, max compression
+gzip compressed data, was "klongpy-0.3.73.tar", last modified: Fri Jun 23 23:30:35 2023, max compression
```

## Comparing `klongpy-0.3.72.tar` & `klongpy-0.3.73.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 22:40:40.669765 klongpy-0.3.72/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.72/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 22:40:40.669765 klongpy-0.3.72/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)    10605 2023-04-13 20:55:52.000000 klongpy-0.3.72/README.md
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 22:40:40.669765 klongpy-0.3.72/klongpy/
--rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.72/klongpy/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    12840 2023-06-23 22:40:09.000000 klongpy-0.3.72/klongpy/adverbs.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2904 2023-04-13 22:28:51.000000 klongpy-0.3.72/klongpy/backend.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    27806 2023-06-23 22:40:09.000000 klongpy-0.3.72/klongpy/core.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    30738 2023-06-23 22:40:09.000000 klongpy-0.3.72/klongpy/dyads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    20414 2023-06-23 22:40:09.000000 klongpy-0.3.72/klongpy/interpreter.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14191 2023-04-13 20:55:52.000000 klongpy-0.3.72/klongpy/monads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    11920 2023-03-12 00:53:23.000000 klongpy-0.3.72/klongpy/sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.72/klongpy/sys_var.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.72/klongpy/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 22:40:40.669765 klongpy-0.3.72/klongpy.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 22:40:40.000000 klongpy-0.3.72/klongpy.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-06-23 22:40:40.000000 klongpy-0.3.72/klongpy.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-06-23 22:40:40.000000 klongpy-0.3.72/klongpy.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-06-23 22:40:40.000000 klongpy-0.3.72/klongpy.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-06-23 22:40:40.000000 klongpy-0.3.72/klongpy.egg-info/top_level.txt
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 22:40:40.669765 klongpy-0.3.72/scripts/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6355 2023-03-07 16:11:08.000000 klongpy-0.3.72/scripts/kgpy
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-06-23 22:40:40.669765 klongpy-0.3.72/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-06-23 22:40:09.000000 klongpy-0.3.72/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 22:40:40.669765 klongpy-0.3.72/tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6326 2023-06-23 00:44:02.000000 klongpy-0.3.72/tests/test_accel.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.72/tests/test_examples.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    21480 2023-06-23 00:44:02.000000 klongpy-0.3.72/tests/test_extra_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2021 2023-06-23 22:40:09.000000 klongpy-0.3.72/tests/test_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2790 2023-03-12 16:05:26.000000 klongpy-0.3.72/tests/test_interop.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3762 2023-06-23 22:40:09.000000 klongpy-0.3.72/tests/test_join_over.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.72/tests/test_prog.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.72/tests/test_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.72/tests/test_suite_file.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    11903 2023-03-12 00:53:23.000000 klongpy-0.3.72/tests/test_sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     7954 2022-12-08 17:42:38.000000 klongpy-0.3.72/tests/test_util.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 23:30:35.058063 klongpy-0.3.73/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.73/LICENSE
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 23:30:35.058063 klongpy-0.3.73/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)    10605 2023-04-13 20:55:52.000000 klongpy-0.3.73/README.md
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 23:30:35.058063 klongpy-0.3.73/klongpy/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.73/klongpy/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12840 2023-06-23 22:40:09.000000 klongpy-0.3.73/klongpy/adverbs.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2904 2023-04-13 22:28:51.000000 klongpy-0.3.73/klongpy/backend.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    27722 2023-06-23 23:29:21.000000 klongpy-0.3.73/klongpy/core.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    30746 2023-06-23 23:29:21.000000 klongpy-0.3.73/klongpy/dyads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    20414 2023-06-23 22:40:09.000000 klongpy-0.3.73/klongpy/interpreter.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14191 2023-04-13 20:55:52.000000 klongpy-0.3.73/klongpy/monads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11920 2023-03-12 00:53:23.000000 klongpy-0.3.73/klongpy/sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.73/klongpy/sys_var.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.73/klongpy/utils.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 23:30:35.058063 klongpy-0.3.73/klongpy.egg-info/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 23:30:35.000000 klongpy-0.3.73/klongpy.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-06-23 23:30:35.000000 klongpy-0.3.73/klongpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-06-23 23:30:35.000000 klongpy-0.3.73/klongpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-06-23 23:30:35.000000 klongpy-0.3.73/klongpy.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-06-23 23:30:35.000000 klongpy-0.3.73/klongpy.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 23:30:35.058063 klongpy-0.3.73/scripts/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6355 2023-03-07 16:11:08.000000 klongpy-0.3.73/scripts/kgpy
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-06-23 23:30:35.058063 klongpy-0.3.73/setup.cfg
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-06-23 23:29:21.000000 klongpy-0.3.73/setup.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 23:30:35.058063 klongpy-0.3.73/tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6326 2023-06-23 00:44:02.000000 klongpy-0.3.73/tests/test_accel.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.73/tests/test_examples.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    21632 2023-06-23 23:29:21.000000 klongpy-0.3.73/tests/test_extra_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2021 2023-06-23 22:40:09.000000 klongpy-0.3.73/tests/test_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2790 2023-03-12 16:05:26.000000 klongpy-0.3.73/tests/test_interop.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3762 2023-06-23 22:40:09.000000 klongpy-0.3.73/tests/test_join_over.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.73/tests/test_prog.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.73/tests/test_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.73/tests/test_suite_file.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11903 2023-03-12 00:53:23.000000 klongpy-0.3.73/tests/test_sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7954 2022-12-08 17:42:38.000000 klongpy-0.3.73/tests/test_util.py
```

### Comparing `klongpy-0.3.72/LICENSE` & `klongpy-0.3.73/LICENSE`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/PKG-INFO` & `klongpy-0.3.73/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.72
+Version: 0.3.73
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `klongpy-0.3.72/README.md` & `klongpy-0.3.73/README.md`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/klongpy/adverbs.py` & `klongpy-0.3.73/klongpy/adverbs.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/klongpy/backend.py` & `klongpy-0.3.73/klongpy/backend.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/klongpy/core.py` & `klongpy-0.3.73/klongpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,23 +325,21 @@
         if a.dtype != 'O':
             if np.isarray(b):
                 if b.dtype != 'O':
                     # 1
                     return f(a,b)
                 else:
                     # 2
-                    assert len(a) == len(b)
                     return np.asarray([vec_fn2(x, y, f) for x,y in zip(a,b)], dtype=object)
             else:
                 # 3
                 return f(a,b)
         else:
             if np.isarray(b):
                 # 4
-                assert len(a) == len(b)
                 return np.asarray([vec_fn2(x, y, f) for x,y in zip(a,b)], dtype=object)
             else:
                 # 5
                 return np.asarray([vec_fn2(x,b,f) for x in a], dtype=object)
     else:
         if np.isarray(b):
             if b.dtype != 'O':
```

### Comparing `klongpy-0.3.72/klongpy/dyads.py` & `klongpy-0.3.73/klongpy/dyads.py`

 * *Files 1% similar despite different names*

```diff
@@ -697,15 +697,15 @@
                    2^-5  -->  0.03125
                   0.3^3  -->  0.027
                   2^0.5  -->  1.41421356237309504
 
     """
     def _e(a,b):
         r = np.power(float(a) if is_integer(a) else a, b)
-        return np.dtype('int').type(r) if np.trunc(r) == r else r
+        return np.dtype('int').type(r) if np.all(np.trunc(r) == r) else r
     return vec_fn2(a, b, _e)
 
 
 def eval_dyad_remainder(a, b):
     """
 
         a!b                                                  [Remainder]
```

### Comparing `klongpy-0.3.72/klongpy/interpreter.py` & `klongpy-0.3.73/klongpy/interpreter.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/klongpy/monads.py` & `klongpy-0.3.73/klongpy/monads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/klongpy/sys_fn.py` & `klongpy-0.3.73/klongpy/sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/klongpy/sys_var.py` & `klongpy-0.3.73/klongpy/sys_var.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/klongpy/utils.py` & `klongpy-0.3.73/klongpy/utils.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/klongpy.egg-info/PKG-INFO` & `klongpy-0.3.73/klongpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.72
+Version: 0.3.73
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `klongpy-0.3.72/klongpy.egg-info/SOURCES.txt` & `klongpy-0.3.73/klongpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/scripts/kgpy` & `klongpy-0.3.73/scripts/kgpy`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/setup.py` & `klongpy-0.3.73/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 
 setup(
     name='klongpy',
     packages=['klongpy'],
-    version='0.3.72',
+    version='0.3.73',
     description='Python implementation of Klong language.',
     author='Brian Guarraci',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `klongpy-0.3.72/tests/test_accel.py` & `klongpy-0.3.73/tests/test_accel.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/tests/test_examples.py` & `klongpy-0.3.73/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/tests/test_extra_suite.py` & `klongpy-0.3.73/tests/test_extra_suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 
 # add tests not included in the original kg suite
 class TestExtraCoreSuite(unittest.TestCase):
 
     def assert_eval_cmp(self, a, b, klong=None):
         self.assertTrue(eval_cmp(a, b, klong=klong))
 
+    def test_power(self):
+        klong = KlongInterpreter()
+        r = klong('[1 2 3]^2')
+        self.assertTrue(array_equal(r, np.array([1,4,9])))
+
     def test_dyad_join_mixed_types(self):
         klong = KlongInterpreter()
         r = klong(',/["a" [1]]')
         self.assertTrue(array_equal(r, np.array(['a', 1], dtype='object')))
 
     def test_dyad_join_nested_array(self):
         klong = KlongInterpreter()
```

### Comparing `klongpy-0.3.72/tests/test_fn.py` & `klongpy-0.3.73/tests/test_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/tests/test_interop.py` & `klongpy-0.3.73/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/tests/test_join_over.py` & `klongpy-0.3.73/tests/test_join_over.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/tests/test_prog.py` & `klongpy-0.3.73/tests/test_prog.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/tests/test_suite.py` & `klongpy-0.3.73/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/tests/test_suite_file.py` & `klongpy-0.3.73/tests/test_suite_file.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/tests/test_sys_fn.py` & `klongpy-0.3.73/tests/test_sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.72/tests/test_util.py` & `klongpy-0.3.73/tests/test_util.py`

 * *Files identical despite different names*

