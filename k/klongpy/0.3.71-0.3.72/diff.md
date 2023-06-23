# Comparing `tmp/klongpy-0.3.71.tar.gz` & `tmp/klongpy-0.3.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klongpy-0.3.71.tar", last modified: Fri Jun 23 00:44:26 2023, max compression
+gzip compressed data, was "klongpy-0.3.72.tar", last modified: Fri Jun 23 22:40:40 2023, max compression
```

## Comparing `klongpy-0.3.71.tar` & `klongpy-0.3.72.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 00:44:26.793443 klongpy-0.3.71/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.71/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 00:44:26.793443 klongpy-0.3.71/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)    10605 2023-04-13 20:55:52.000000 klongpy-0.3.71/README.md
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 00:44:26.793443 klongpy-0.3.71/klongpy/
--rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.71/klongpy/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    13005 2023-06-23 00:44:02.000000 klongpy-0.3.71/klongpy/adverbs.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2904 2023-04-13 22:28:51.000000 klongpy-0.3.71/klongpy/backend.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    23120 2023-06-23 00:44:02.000000 klongpy-0.3.71/klongpy/core.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    30983 2023-06-23 00:44:02.000000 klongpy-0.3.71/klongpy/dyads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    20402 2023-04-03 23:16:48.000000 klongpy-0.3.71/klongpy/interpreter.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14191 2023-04-13 20:55:52.000000 klongpy-0.3.71/klongpy/monads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    11920 2023-03-12 00:53:23.000000 klongpy-0.3.71/klongpy/sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.71/klongpy/sys_var.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.71/klongpy/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 00:44:26.793443 klongpy-0.3.71/klongpy.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 00:44:26.000000 klongpy-0.3.71/klongpy.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-06-23 00:44:26.000000 klongpy-0.3.71/klongpy.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-06-23 00:44:26.000000 klongpy-0.3.71/klongpy.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-06-23 00:44:26.000000 klongpy-0.3.71/klongpy.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-06-23 00:44:26.000000 klongpy-0.3.71/klongpy.egg-info/top_level.txt
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 00:44:26.793443 klongpy-0.3.71/scripts/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6355 2023-03-07 16:11:08.000000 klongpy-0.3.71/scripts/kgpy
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-06-23 00:44:26.793443 klongpy-0.3.71/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-06-23 00:44:02.000000 klongpy-0.3.71/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 00:44:26.793443 klongpy-0.3.71/tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6326 2023-06-23 00:44:02.000000 klongpy-0.3.71/tests/test_accel.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.71/tests/test_examples.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    21480 2023-06-23 00:44:02.000000 klongpy-0.3.71/tests/test_extra_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1952 2023-03-12 01:19:51.000000 klongpy-0.3.71/tests/test_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2790 2023-03-12 16:05:26.000000 klongpy-0.3.71/tests/test_interop.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3808 2023-06-23 00:44:02.000000 klongpy-0.3.71/tests/test_join_over.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.71/tests/test_prog.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.71/tests/test_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.71/tests/test_suite_file.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    11903 2023-03-12 00:53:23.000000 klongpy-0.3.71/tests/test_sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     7954 2022-12-08 17:42:38.000000 klongpy-0.3.71/tests/test_util.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 22:40:40.669765 klongpy-0.3.72/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.72/LICENSE
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 22:40:40.669765 klongpy-0.3.72/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)    10605 2023-04-13 20:55:52.000000 klongpy-0.3.72/README.md
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 22:40:40.669765 klongpy-0.3.72/klongpy/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.72/klongpy/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12840 2023-06-23 22:40:09.000000 klongpy-0.3.72/klongpy/adverbs.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2904 2023-04-13 22:28:51.000000 klongpy-0.3.72/klongpy/backend.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    27806 2023-06-23 22:40:09.000000 klongpy-0.3.72/klongpy/core.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    30738 2023-06-23 22:40:09.000000 klongpy-0.3.72/klongpy/dyads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    20414 2023-06-23 22:40:09.000000 klongpy-0.3.72/klongpy/interpreter.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14191 2023-04-13 20:55:52.000000 klongpy-0.3.72/klongpy/monads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11920 2023-03-12 00:53:23.000000 klongpy-0.3.72/klongpy/sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.72/klongpy/sys_var.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.72/klongpy/utils.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 22:40:40.669765 klongpy-0.3.72/klongpy.egg-info/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 22:40:40.000000 klongpy-0.3.72/klongpy.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-06-23 22:40:40.000000 klongpy-0.3.72/klongpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-06-23 22:40:40.000000 klongpy-0.3.72/klongpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-06-23 22:40:40.000000 klongpy-0.3.72/klongpy.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-06-23 22:40:40.000000 klongpy-0.3.72/klongpy.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 22:40:40.669765 klongpy-0.3.72/scripts/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6355 2023-03-07 16:11:08.000000 klongpy-0.3.72/scripts/kgpy
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-06-23 22:40:40.669765 klongpy-0.3.72/setup.cfg
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-06-23 22:40:09.000000 klongpy-0.3.72/setup.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 22:40:40.669765 klongpy-0.3.72/tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6326 2023-06-23 00:44:02.000000 klongpy-0.3.72/tests/test_accel.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.72/tests/test_examples.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    21480 2023-06-23 00:44:02.000000 klongpy-0.3.72/tests/test_extra_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2021 2023-06-23 22:40:09.000000 klongpy-0.3.72/tests/test_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2790 2023-03-12 16:05:26.000000 klongpy-0.3.72/tests/test_interop.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3762 2023-06-23 22:40:09.000000 klongpy-0.3.72/tests/test_join_over.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.72/tests/test_prog.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.72/tests/test_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.72/tests/test_suite_file.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11903 2023-03-12 00:53:23.000000 klongpy-0.3.72/tests/test_sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7954 2022-12-08 17:42:38.000000 klongpy-0.3.72/tests/test_util.py
```

### Comparing `klongpy-0.3.71/LICENSE` & `klongpy-0.3.72/LICENSE`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/PKG-INFO` & `klongpy-0.3.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.71
+Version: 0.3.72
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `klongpy-0.3.71/README.md` & `klongpy-0.3.72/README.md`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/klongpy/adverbs.py` & `klongpy-0.3.72/klongpy/adverbs.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     elif s == ':*':
         return eval_dyad_adverb_iterate
     elif s == ':~':
         return (lambda f,a,b,k=klong: eval_adverb_while(k,f,a,b)) if arity == 2 else eval_adverb_converge
     raise RuntimeError(f"unknown adverb: {s}")
 
 
-def eval_adverb_converge(f, a):
+def eval_adverb_converge(f, a, op):
     """
         f:~a                                                  [Converge]
 
         Find the fixpoint of f(a), if any. The fixpoint of "f" is a value
         "a" for which f(a) = a. For example,
 
         {(x+2%x)%2}:~2
@@ -53,25 +53,25 @@
     """
     def _e(p,q):
         if not isinstance(p, type(q)):
             return False
         if is_number(p):
             return np.isclose(p,q)
         elif np.isarray(p):
-            return (p.shape == q.shape) and (np.isclose(p,q)).all()
+            return (p.shape == q.shape) and np.allclose(p,q)
         return p == q
     x = f(a)
     xx = f(x)
     while not _e(x,xx):
         x = xx
         xx = f(x)
     return x
 
 
-def eval_adverb_each(f, a):
+def eval_adverb_each(f, a, op):
     """
 
         f'a                                                       [Each]
 
         If "a" is a list, apply "f" to each member of "a":
 
         f'a  -->  f(a1),...,f(aN)
@@ -155,15 +155,15 @@
     see: eval_dyad_adverb_each_left
     """
     b = str_to_chr_arr(b) if isinstance(b,str) else b
     return np.asarray([f(x,a) for x in b])
 
 
 
-def eval_adverb_each_pair(f, a):
+def eval_adverb_each_pair(f, a, op):
     """
 
         f:'a                                                 [Each-Pair]
 
         If "a" is a list of more than one element, apply "f" to each
         consecutive pair of "a":
 
@@ -197,15 +197,15 @@
     """
     while not safe_eq(a, 0):
         b = f(b)
         a = a - 1
     return b
 
 
-def eval_adverb_over(f, a):
+def eval_adverb_over(f, a, op):
     """
         f/a                                                       [Over]
 
         If "a" is a list, fold "f" over "a":
 
         f/a  -->  f(...f(f(a1;a2);a3)...;aN))
         +/a  -->  ((...(a1+a2)+...)+aN)
@@ -216,33 +216,30 @@
 
         Example: +/[1 2 3 4]  -->  10
     """
     if is_atom(a):
         return a
     if len(a) == 1:
         return a[0]
-    # introspect into the wrapped operation and determine if we can optimize
-    spec = inspect.getargspec(f)
-    wrapped = spec.defaults[-1]
     # https://docs.cupy.dev/en/stable/reference/ufunc.html
     # TODO: can we use NumPy reduce when CuPy backend primary?
-    if isinstance(wrapped, KGOp):
-        if safe_eq(wrapped.a,'+'):
+    if isinstance(op, KGOp):
+        if safe_eq(op.a,'+'):
             return np.add.reduce(a)
-        elif safe_eq(wrapped.a, '-'):
+        elif safe_eq(op.a, '-'):
             return np.subtract.reduce(a)
-        elif safe_eq(wrapped.a, '*') and hasattr(np.multiply,'reduce'):
+        elif safe_eq(op.a, '*') and hasattr(np.multiply,'reduce'):
             return np.multiply.reduce(a)
-        elif safe_eq(wrapped.a, '%') and hasattr(np.divide,'reduce'):
+        elif safe_eq(op.a, '%') and hasattr(np.divide,'reduce'):
             return np.divide.reduce(a)
-        elif safe_eq(wrapped.a, '&') and len(a.shape) == 1:
+        elif safe_eq(op.a, '&') and len(a.shape) == 1:
             return np.min(a)
-        elif safe_eq(wrapped.a, '|') and len(a.shape) == 1:
+        elif safe_eq(op.a, '|') and len(a.shape) == 1:
             return np.max(a)
-        elif safe_eq(wrapped.a, ',') and np.isarray(a) and a.dtype != 'O':
+        elif safe_eq(op.a, ',') and np.isarray(a) and a.dtype != 'O':
             return a if a.ndim == 1 else np.concatenate(a, axis=0)
     return functools.reduce(f, a)
 
 
 def eval_adverb_over_neutral(f, a, b):
     """
 
@@ -308,15 +305,15 @@
     r = [a, *q]
     try:
         return np.asarray(r)
     except ValueError:
         return cast_malformed_array(r)
 
 
-def eval_adverb_scan_over(f, a):
+def eval_adverb_scan_over(f, a, op):
     """
         see eval_adverb_scan_over_neutral
     """
     if is_atom(a):
         return a
     # https://docs.cupy.dev/en/stable/reference/ufunc.html
     if safe_eq(f, eval_dyad_add) and hasattr(np.add, 'accumulate'):
@@ -330,15 +327,15 @@
     r = list(itertools.accumulate(a, f))
     try:
         return np.asarray(r)
     except ValueError:
         return cast_malformed_array(r)
 
 
-def eval_adverb_scan_converging(f, a):
+def eval_adverb_scan_converging(f, a, op):
     """
 
         f\~a                                           [Scan-Converging]
 
         Monadic \~ is like monadic :~, but returns a list of all
         intermediate results instead of just the end result. The
         last element of the list will be same as the result of a
```

### Comparing `klongpy-0.3.71/klongpy/backend.py` & `klongpy-0.3.72/klongpy/backend.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/klongpy/core.py` & `klongpy-0.3.72/klongpy/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             return ":dyad"
         return ":triad"
 
     def is_op(self):
         return isinstance(self.a,KGOp)
 
     def is_adverb_chain(self):
-        return (isinstance(self.a,list) and isinstance(self.a[0], KGAdverb))
+        return isinstance(self.a,list) and isinstance(self.a[0],KGAdverb)
 
 
 class KGFnWrapper:
     def __init__(self, klong, fn):
         self.klong = klong
         self.fn = fn
 
@@ -94,17 +94,16 @@
 
     lambda x,y: x + y
     lambda klong, x: klong(x)
 
     """
     def __init__(self, fn):
         self.fn = fn
-        self.args = inspect.getfullargspec(self.fn)[0]
+        self.args = inspect.signature(self.fn, follow_wrapped=True).parameters
         self.provide_klong = 'klong' in self.args
-        # self.keep_context = 'keep_context' in self.args
 
     def __call__(self, klong, ctx):
         params = [ctx[reserved_fn_symbol_map[x]] for x in reserved_fn_args if x in self.args]
         return self.fn(klong, *params) if self.provide_klong else self.fn(*params)
 
     def get_arity(self):
         return len(self.args) - 1 if self.provide_klong else len(self.args)
@@ -133,15 +132,14 @@
     def __enter__(self):
         return self
 
     def __exit__(self, ext_type, exc_value, traceback):
         self._fh.close()
 
 
-
 class RangeError(Exception):
     def __init__(self, i):
         self.i = i
         super().__init__()
 
 
 reserved_fn_args = ['x','y','z']
@@ -185,35 +183,34 @@
 def in_map(x, v):
     try:
         return x in v
     except Exception:
         return False
 
 
-def array_equal(a,b):
+def array_equal(a, b):
     """
     Recursively determine if two values or arrays are equal.
 
     NumPy ops (e.g. array_equal) are not sufficiently general purpose for this, so we need our own.
     """
     if is_list(a):
-        if is_list(b):
-            if len(a) != len(b):
-                return False
+        if is_list(b) and len(a) == len(b):
+            for x, y in zip(a, b):
+                if not array_equal(x, y):
+                    return False
+            return True
         else:
             return False
     else:
         if is_list(b):
             return False
         else:
             return np.isclose(a,b) if is_number(a) and is_number(b) else a == b
 
-    r = np.asarray([array_equal(x,y) for x,y in zip(a,b)])
-    return r.all()
-
 
 def has_none(a):
     if safe_eq(a, None) or not isinstance(a,list):
         return False
     for q in a:
         if q is None:
             return True
@@ -265,16 +262,15 @@
 def safe_eq(a,b):
     return isinstance(a,type(b)) and a == b
 
 
 def rec_flatten(a):
     if not is_list(a) or len(a) == 0:
         return a
-    r = np.asarray([(rec_flatten(x) if np.isarray(x) else x) for x in a]).flatten()
-    return np.hstack(r) if len(r) > 1 else r
+    return np.concatenate([rec_flatten(x) if is_list(x) else np.array([x]) for x in a]).ravel()
 
 
 def rec_fn(a,f):
     return np.asarray([rec_fn(x, f) for x in a], dtype=object) if is_list(a) else f(a)
 
 
 def vec_fn(a, f):
@@ -284,23 +280,51 @@
         return np.asarray([((vec_fn(x, f)) if is_list(x) else f(x)) for x in a] if is_list(a) else f(a), dtype=object)
     return f(a)
 
 
 def rec_fn2(a,b,f):
     return np.asarray([rec_fn2(x, y, f) for x,y in zip(a,b)], dtype=object) if is_list(a) and is_list(b) else f(a,b)
 
-# 1 vec[A],vec[B]
-# 2 vec[A],obj_vec[B]
-# 3 vec[A],scalar[B]
-# 4 obj_vec[A],vec[B] (may either be vec[B] or obj_vec[B])
-# 5 obj_vec[A],scalar[B]
-# 6 scalar[A],vec[B]
-# 7 scalar[A],obj_vec[B]
-# 8 scalar[A],scalar[B]
+
 def vec_fn2(a, b, f):
+    """
+    Apply function `f` recursively to the elements of `a` and `b`, which can be scalar values, vectors, or nested vectors.
+
+    This function distinguishes 8 cases based on the types and dimensions of `a` and `b`:
+
+    1. vec[A],vec[B]: `f` is applied directly to `a` and `b`.
+    2. vec[A],obj_vec[B]: `f` is applied recursively to pairs of elements in `a` and `b`.
+    3. vec[A],scalar[B]: `f` is applied directly to `a` and `b`.
+    4. obj_vec[A],vec[B]: `f` is applied recursively to pairs of elements in `a` and `b`.
+    5. obj_vec[A],scalar[B]: `f` is applied recursively to the elements in `a` and the scalar `b`.
+    6. scalar[A],vec[B]: `f` is applied directly to `a` and `b`.
+    7. scalar[A],obj_vec[B]: `f` is applied recursively to the scalar `a` and the elements in `b`.
+    8. scalar[A],scalar[B]: `f` is applied directly to `a` and `b`.
+
+    Parameters
+    ----------
+    a, b : numpy.array or any type
+        The inputs to `f`. They can be numpy arrays of any data type. If they are arrays, they should have the same shape. 
+        Non-array inputs can be of any type that `f` can accept.
+
+    f : callable
+        A function that takes two arguments and can handle the types and dimensions of `a` and `b`.
+
+    Returns
+    -------
+    numpy.array or any type
+        The result of applying `f` to `a` and `b`, which can be a scalar, a vector, or a nested vector depending on 
+        the inputs and `f`.
+
+    Notes
+    -----
+    This function assumes that `f` can handle the types and dimensions of `a` and `b`, and that `a` and `b` have the same 
+    shape if they are arrays. It does not check these conditions, so unexpected results or errors may occur if they are 
+    not satisfied.
+    """
     if np.isarray(a):
         if a.dtype != 'O':
             if np.isarray(b):
                 if b.dtype != 'O':
                     # 1
                     return f(a,b)
                 else:
@@ -327,14 +351,100 @@
                 # 7
                 return np.asarray([vec_fn2(a,x,f) for x in b], dtype=object)
         else:
             # 8
             return f(a,b)
 
 
+def all_fn2(a, b, f):
+    """
+    Apply function `f` recursively to the elements of `a` and `b`, returning `False` immediately if `f` returns `False`.
+
+    This function distinguishes 8 cases based on the types and dimensions of `a` and `b`:
+
+    1. vec[A],vec[B]: `f` is applied directly to `a` and `b`.
+    2. vec[A],obj_vec[B]: `f` is applied recursively to pairs of elements in `a` and `b`.
+    3. vec[A],scalar[B]: `f` is applied directly to `a` and `b`.
+    4. obj_vec[A],vec[B]: `f` is applied recursively to pairs of elements in `a` and `b`.
+    5. obj_vec[A],scalar[B]: `f` is applied recursively to the elements in `a` and the scalar `b`.
+    6. scalar[A],vec[B]: `f` is applied directly to `a` and `b`.
+    7. scalar[A],obj_vec[B]: `f` is applied recursively to the scalar `a` and the elements in `b`.
+    8. scalar[A],scalar[B]: `f` is applied directly to `a` and `b`.
+
+    If at any point `f` returns `False`, the function returns `False` immediately ("short-circuits"). If `f` returns `True` 
+    for all pairs of elements, the function returns `True`.
+
+    Parameters
+    ----------
+    a, b : numpy.array or any type
+        The inputs to `f`. They can be numpy arrays of any data type. If they are arrays, they should have the same shape. 
+        Non-array inputs can be of any type that `f` can accept.
+
+    f : callable
+        A function that takes two arguments and returns a boolean. It should return `True` when the condition it checks is 
+        satisfied, and `False` otherwise.
+
+    Returns
+    -------
+    bool
+        `True` if all applications of `f` return `True`, `False` otherwise.
+
+    Notes
+    -----
+    This function assumes that `f` is a function that returns a boolean, and that `a` and `b` have the same shape if they 
+    are arrays. It does not check these conditions, so unexpected results or errors may occur if they are not satisfied.
+    """
+    if np.isarray(a):
+        if a.dtype != 'O':
+            if np.isarray(b):
+                if b.dtype != 'O':
+                    # 1
+                    return f(a,b)
+                else:
+                    # 2
+                    for x, y in zip(a, b):
+                        res = all_fn2(x, y, f)
+                        if not res:
+                            return False
+                    return True
+            else:
+                # 3
+                return f(a,b)
+        else:
+            if np.isarray(b):
+                # 4
+                for x, y in zip(a, b):
+                    res = all_fn2(x, y, f)
+                    if not res:
+                        return False
+                return True
+            else:
+                # 5
+                for x in a:
+                    res = all_fn2(x, b, f)
+                    if not res:
+                        return False
+                return True
+    else:
+        if np.isarray(b):
+            if b.dtype != 'O':
+                # 6
+                return f(a,b)
+            else:
+                # 7
+                for x in b:
+                    res = all_fn2(a, x, f)
+                    if not res:
+                        return False
+                return True
+        else: 
+            # 8
+            return f(a,b)
+
+
 def is_symbolic(c):
     return isinstance(c, str) and (c.isalpha() or c.isdigit() or c == '.')
 
 
 def is_char(x):
     return isinstance(x, KGChar)
 
@@ -517,14 +627,16 @@
             if not cmatch(t,i,'"'):
                 break
         r.append(c)
         i += 1
     return i,"".join(r)
 
 
+copy_lambda = KGLambda(lambda x: copy.deepcopy(x))
+
 def read_cond(klong, t, i=0):
     """
 
         # A conditional expression has two forms: :[e1;e2;e3] means "if
         # e1 is true, evaluate to e2, else evaluate to e3".
         # :[e1;e2:|e3;e4;e5] is short for :[e1;e2:[e3;e4;e5]], i.e. the
         # ":|" acts as an "else-if" operator. There may be any number of
@@ -618,15 +730,15 @@
         if aa.isalpha() or aa == '.':
             return read_sym(t, i=i+1, module=module)
         elif aa.isnumeric() or aa == '"':
             return kg_read(t, i+1, ignore_newline=ignore_newline, module=module)
         elif aa == '{':
             i, d = read_list(t, '}', i=i+2, module=module)
             d = list_to_dict(d)
-            return i, KGCall(KGLambda(lambda x: copy.deepcopy(x)),args=d,arity=0)
+            return i, KGCall(copy_lambda,args=d,arity=0)
         elif aa == '[':
             return i+2,':['
         elif aa == '|':
             return i+2,':|'
         return i+2,KGOp(f":{aa}",arity=0)
     elif safe_eq(a, '['):
         return read_list(t, ']', i=i+1, module=module)
```

### Comparing `klongpy-0.3.71/klongpy/dyads.py` & `klongpy-0.3.72/klongpy/dyads.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,22 +580,15 @@
                            "foo"~"foo"  -->  1
                              :foo~:foo  -->  1
                                0cx~0cx  -->  1
                        [1 2 3]~[1 2 3]  -->  1
                    [1 [2] 3]~[1 [4] 3]  -->  0
 
     """
-    def _e(x,y):
-        return np.isclose(x,y) if (is_number(x) and is_number(y)) else np.all(np.asarray(x,dtype=object) == np.asarray(y,dtype=object))
-    if is_list(a):
-        if is_list(b):
-            return kg_truth(rec_flatten(vec_fn2(a, b, _e)).all() if len(a) == len(b) else 0)
-    elif not is_list(b):
-        return kg_truth(_e(a,b))
-    return False
+    return kg_truth(all_fn2(a, b, lambda x,y: np.isclose(x, y) if is_number(x) and is_number(y) else np.all(x == y)))
 
 
 def eval_dyad_maximum(a, b):
     """
 
         a|b                                                     [Max/Or]
```

### Comparing `klongpy-0.3.71/klongpy/interpreter.py` & `klongpy-0.3.72/klongpy/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     if arr[0].arity == 1:
         f = lambda x,k=klong,a=arr[0].a: k.eval(KGCall(a, [x], arity=1))
     else:
         f = lambda x,y,k=klong,a=arr[0].a: k.eval(KGCall(a, [x,y], arity=2))
     for i in range(1,len(arr)-1):
         o = get_adverb_fn(klong, arr[i].a, arity=arr[i].arity)
         if arr[i].arity == 1:
-            f = lambda x,f=f,o=o: o(f,x)
+            f = lambda x,f=f,o=o: o(f,x,op=arr[0].a)
         else:
             f = lambda x,y,f=f,o=o: o(f,x,y)
     if arr[-2].arity == 1:
         f = lambda a=arr[-1],f=f,k=klong: f(k.eval(a))
     else:
         f = lambda a=arr[-1],f=f,k=klong: f(k.eval(a[0]),k.eval(a[1]))
     return f
@@ -545,29 +545,29 @@
         if isinstance(x, KGSym):
             try:
                 return self._context[x]
             except KeyError:
                 if x not in reserved_fn_symbols:
                     self._context[x] = x
                 return x
-        elif isinstance(x, KGCond):
-            q = self.call(x[0])
-            p = not ((is_number(q) and q == 0) or is_empty(q))
-            return self.call(x[1]) if p else self.call(x[2])
         elif isinstance(x, KGCall) and not (x.is_op() or x.is_adverb_chain()):
             return self._eval_fn(KGFn(x.a,x.args,x.arity))
         elif isinstance(x, KGFn):
             if x.is_op():
                 f = self._get_op_fn(x.a.a, x.a.arity)
                 fa = (x.args if isinstance(x.args, list) else [x.args]) if x.args is not None else x.args
                 _y = self.eval(fa[1]) if x.a.arity == 2 else None
                 _x = fa[0] if x.a.a == '::' else self.eval(fa[0])
                 return f(_x) if x.a.arity == 1 else f(_x, _y)
             elif x.is_adverb_chain():
                 return chain_adverbs(self, x.a)()
+        elif isinstance(x, KGCond):
+            q = self.call(x[0])
+            p = not ((is_number(q) and q == 0) or is_empty(q))
+            return self.call(x[1]) if p else self.call(x[2])
         elif isinstance(x,list) and len(x) > 0:
             return [self.call(y) for y in x][-1]
         return x
 
     def __call__(self, x, *args, **kwds):
         """
         Convience method for executing Klong programs.
```

### Comparing `klongpy-0.3.71/klongpy/monads.py` & `klongpy-0.3.72/klongpy/monads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/klongpy/sys_fn.py` & `klongpy-0.3.72/klongpy/sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/klongpy/sys_var.py` & `klongpy-0.3.72/klongpy/sys_var.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/klongpy/utils.py` & `klongpy-0.3.72/klongpy/utils.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/klongpy.egg-info/PKG-INFO` & `klongpy-0.3.72/klongpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.71
+Version: 0.3.72
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `klongpy-0.3.71/klongpy.egg-info/SOURCES.txt` & `klongpy-0.3.72/klongpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/scripts/kgpy` & `klongpy-0.3.72/scripts/kgpy`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/setup.py` & `klongpy-0.3.72/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 
 setup(
     name='klongpy',
     packages=['klongpy'],
-    version='0.3.71',
+    version='0.3.72',
     description='Python implementation of Klong language.',
     author='Brian Guarraci',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `klongpy-0.3.71/tests/test_accel.py` & `klongpy-0.3.72/tests/test_accel.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/tests/test_examples.py` & `klongpy-0.3.72/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/tests/test_extra_suite.py` & `klongpy-0.3.72/tests/test_extra_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/tests/test_fn.py` & `klongpy-0.3.72/tests/test_fn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import unittest
 
 from utils import *
-
 from klongpy import KlongInterpreter
 
 
 class TestFunctionsSuite(unittest.TestCase):
 
     def assert_eval_cmp(self, a, b, klong=None):
         self.assertTrue(eval_cmp(a, b, klong=klong))
@@ -62,7 +61,11 @@
         Test the entire suite file.
         """
         klong = KlongInterpreter()
         with open("tests/klong_fn.kg", "r") as f:
             klong(f.read())
             r = klong('err')
             self.assertEqual(r, 0)
+
+if __name__ == "__main__":
+    run_suite_file("klong_join_over.kg")
+
```

### Comparing `klongpy-0.3.71/tests/test_interop.py` & `klongpy-0.3.72/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/tests/test_join_over.py` & `klongpy-0.3.72/tests/test_join_over.py`

 * *Files 9% similar despite different names*

```diff
@@ -94,12 +94,14 @@
             print(f"executed {i} lines")
 
 
     def test_gen_file(self):
         """
         Test the entire suite file.
         """
-        klong = KlongInterpreter()
-        with open("tests/klong_join_over.kg", "r") as f:
-            klong(f.read())
-            r = klong('err')
-            self.assertEqual(r, 0)
+        self.assertEqual(run_suite_file('klong_join_over.kg'), 0)
+
+
+if __name__ == "__main__":
+    run_suite_file("klong_join_over.kg")
+
+
```

### Comparing `klongpy-0.3.71/tests/test_prog.py` & `klongpy-0.3.72/tests/test_prog.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/tests/test_suite.py` & `klongpy-0.3.72/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/tests/test_suite_file.py` & `klongpy-0.3.72/tests/test_suite_file.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/tests/test_sys_fn.py` & `klongpy-0.3.72/tests/test_sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.71/tests/test_util.py` & `klongpy-0.3.72/tests/test_util.py`

 * *Files identical despite different names*

