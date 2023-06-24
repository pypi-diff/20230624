# Comparing `tmp/bhv-0.5.8.tar.gz` & `tmp/bhv-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.5.8.tar", last modified: Sun Jun 11 01:25:23 2023, max compression
+gzip compressed data, was "bhv-0.6.0a0.tar", last modified: Sat Jun 24 10:03:46 2023, max compression
```

## Comparing `bhv-0.5.8.tar` & `bhv-0.6.0a0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:25:23.386929 bhv-0.5.8/
--rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.5.8/LICENSE
--rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-11 01:25:23.386929 bhv-0.5.8/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.5.8/README.md
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:25:23.385929 bhv-0.5.8/bhv/
--rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.5.8/bhv/__init__.py
--rw-r--r--   0 adam      (1000) adam      (1000)    14829 2023-06-06 19:12:06.000000 bhv-0.5.8/bhv/abstract.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:25:23.386929 bhv-0.5.8/bhv/cnative/
--rw-r--r--   0 adam      (1000) adam      (1000)     9757 2023-06-11 01:14:47.000000 bhv-0.5.8/bhv/cnative/bindings.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)     7142 2023-06-11 01:24:16.000000 bhv-0.5.8/bhv/cnative/packed.h
--rw-r--r--   0 adam      (1000) adam      (1000)      392 2023-06-07 20:21:30.000000 bhv-0.5.8/bhv/cnative/shared.h
--rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/embedding.py
--rw-r--r--   0 adam      (1000) adam      (1000)     4220 2023-06-06 19:12:06.000000 bhv-0.5.8/bhv/lookup.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1476 2023-06-11 00:46:52.000000 bhv-0.5.8/bhv/native.py
--rw-r--r--   0 adam      (1000) adam      (1000)    11951 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/np.py
--rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/poibin.py
--rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/pytorch.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/shared.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/slice.py
--rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/symbolic.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/unification.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3456 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/vanilla.py
--rw-r--r--   0 adam      (1000) adam      (1000)      782 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/visualization.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:25:23.386929 bhv-0.5.8/bhv.egg-info/
--rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-11 01:25:23.000000 bhv-0.5.8/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)      441 2023-06-11 01:25:23.000000 bhv-0.5.8/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-11 01:25:23.000000 bhv-0.5.8/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       45 2023-06-11 01:25:23.000000 bhv-0.5.8/bhv.egg-info/requires.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-11 01:25:23.000000 bhv-0.5.8/bhv.egg-info/top_level.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-11 01:25:23.386929 bhv-0.5.8/setup.cfg
--rw-r--r--   0 adam      (1000) adam      (1000)     1633 2023-06-11 01:25:11.000000 bhv-0.5.8/setup.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:03:46.825026 bhv-0.6.0a0/
+-rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.6.0a0/LICENSE
+-rw-r--r--   0 adam      (1000) adam      (1000)     1092 2023-06-24 10:03:46.825026 bhv-0.6.0a0/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.6.0a0/README.md
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:03:46.823026 bhv-0.6.0a0/bhv/
+-rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.6.0a0/bhv/__init__.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    16739 2023-06-24 07:40:55.000000 bhv-0.6.0a0/bhv/abstract.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:03:46.824026 bhv-0.6.0a0/bhv/cnative/
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:03:46.824026 bhv-0.6.0a0/bhv/cnative/TurboSHAKEref/
+-rw-r--r--   0 adam      (1000) adam      (1000)    11896 2023-06-11 12:27:27.000000 bhv-0.6.0a0/bhv/cnative/TurboSHAKEref/KeccakP-1600-reference.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     2537 2023-06-11 12:27:27.000000 bhv-0.6.0a0/bhv/cnative/TurboSHAKEref/KeccakSponge.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     2381 2023-06-11 12:27:27.000000 bhv-0.6.0a0/bhv/cnative/TurboSHAKEref/TurboSHAKE.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)    11558 2023-06-24 09:31:02.000000 bhv-0.6.0a0/bhv/cnative/bindings.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-06-24 07:34:04.000000 bhv-0.6.0a0/bhv/embedding.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     4208 2023-06-24 07:40:55.000000 bhv-0.6.0a0/bhv/lookup.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1897 2023-06-24 07:40:55.000000 bhv-0.6.0a0/bhv/native.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    12443 2023-06-24 07:40:55.000000 bhv-0.6.0a0/bhv/np.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.6.0a0/bhv/poibin.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.6.0a0/bhv/pytorch.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-06-16 16:14:43.000000 bhv-0.6.0a0/bhv/shared.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.6.0a0/bhv/slice.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.6.0a0/bhv/symbolic.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.6.0a0/bhv/unification.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3575 2023-06-18 07:52:14.000000 bhv-0.6.0a0/bhv/vanilla.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1372 2023-06-24 07:40:55.000000 bhv-0.6.0a0/bhv/visualization.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-24 10:03:46.824026 bhv-0.6.0a0/bhv.egg-info/
+-rw-r--r--   0 adam      (1000) adam      (1000)     1092 2023-06-24 10:03:46.000000 bhv-0.6.0a0/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)      536 2023-06-24 10:03:46.000000 bhv-0.6.0a0/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-24 10:03:46.000000 bhv-0.6.0a0/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       44 2023-06-24 10:03:46.000000 bhv-0.6.0a0/bhv.egg-info/requires.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-24 10:03:46.000000 bhv-0.6.0a0/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-24 10:03:46.825026 bhv-0.6.0a0/setup.cfg
+-rw-r--r--   0 adam      (1000) adam      (1000)     1922 2023-06-24 10:03:16.000000 bhv-0.6.0a0/setup.py
```

### Comparing `bhv-0.5.8/LICENSE` & `bhv-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.5.8/PKG-INFO` & `bhv-0.6.0a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.5.8
+Version: 0.6.0a0
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
@@ -18,13 +18,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Provides-Extra: torch
-Provides-Extra: numpy
+Provides-Extra: pytorch
+Provides-Extra: np
 License-File: LICENSE
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
```

### Comparing `bhv-0.5.8/README.md` & `bhv-0.6.0a0/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.5.8/bhv/abstract.py` & `bhv-0.6.0a0/bhv/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from statistics import NormalDist
 from itertools import accumulate
 from functools import cache
 from operator import or_, and_
-from math import comb
+from math import comb, log2
 
 from .shared import *
 
 
 class AbstractBHV:
     # recall
     # information_entropy(p) = -p*log2(p) - (1 - p)*log2(1 - p)
@@ -167,15 +167,18 @@
     def active_fraction(self) -> float:
         return self.active()/DIMENSION
 
     def hamming(self, other: Self) -> int:
         return (self ^ other).active()
 
     def bit_error_rate(self, other: Self) -> float:
-        return (self ^ other).active_fraction()
+        return self.hamming(other)/DIMENSION
+
+    def overlap(self, other: Self) -> float:
+        return (self & other).active_fraction()
 
     def jaccard(self, other: Self, distance=False) -> float:
         union_active = (self | other).active()
         if union_active == 0:
             raise RuntimeError("Jaccard index where both vectors are zero")
         res = (self & other).active() / union_active
         return 1. - res if distance else res
@@ -224,18 +227,81 @@
     def related(self, other: Self, stdvs=6) -> bool:
         return abs(self.std_apart(other)) <= stdvs
 
     def unrelated(self, other: Self, stdvs=6) -> bool:
         return abs(self.std_apart(other, invert=True)) <= stdvs
 
     def bias_rel(self, other: Self, rel: Self) -> float:
-        rel_l = (rel & self).active()
-        rel_r = (rel & other).active()
+        rel_l = rel.overlap(self)
+        rel_r = rel.overlap(other)
         return rel_l/(rel_l + rel_r)
 
+    def mutual_information(self, other: Self, distance=False) -> float:
+        nself = ~self
+        nother = ~other
+
+        # Probabilities
+        P00 = nself.overlap(nother)
+        P01 = nself.overlap(other)
+        P10 = self.overlap(nother)
+        P11 = self.overlap(other)
+
+        # Marginal probabilities
+        PX0 = (P00 + P01)
+        PX1 = (P10 + P11)
+        PY0 = (P00 + P10)
+        PY1 = (P01 + P11)
+
+        # Mutual Information
+        MI = 0
+        if P00 and PX0 and PY0:
+            MI += P00 * log2(P00 / (PX0 * PY0))
+        if P01 and PX0 and PY1:
+            MI += P01 * log2(P01 / (PX0 * PY1))
+        if P10 and PX1 and PY0:
+            MI += P10 * log2(P10 / (PX1 * PY0))
+        if P11 and PX1 and PY1:
+            MI += P11 * log2(P11 / (PX1 * PY1))
+
+        return 1 - MI if distance else MI
+
+    def tversky(self, other: Self, l: float, r: float) -> float:
+        o = self.overlap(other)
+        lr = self.overlap(~other)
+        rl = other.overlap(~self)
+        return o/(l*lr + r*rl + o)
+
+    def to_bytes(self):
+        raise NotImplementedError()
+
+    @classmethod
+    def from_bytes(cls, bs):
+        raise NotImplementedError()
+
+    def bits(self):
+        for b in self.to_bytes():
+            yield (b >> 7) & 0x1
+            yield (b >> 6) & 0x1
+            yield (b >> 5) & 0x1
+            yield (b >> 4) & 0x1
+            yield (b >> 3) & 0x1
+            yield (b >> 2) & 0x1
+            yield (b >> 1) & 0x1
+            yield b & 0x1
+
+    @classmethod
+    def from_bitstream(cls, bits_s):
+        it = iter(bits_s)
+        bs = bytes(
+            (next(it) << 7) | (next(it) << 6) | (next(it) << 5) | (next(it) << 4) | (next(it) << 3) | (next(it) << 2) | (next(it) << 1) | next(it)
+            for _ in range(DIMENSION//8)
+        )
+        return cls.from_bytes(bs)
+
+
     # Alternative implementations
 
     @classmethod
     def _majority3_select(cls, a: Self, b: Self, c: Self) -> Self:
         # C:  1 0 0 1 0 1 1
 
         # |:  1 1 1 1 0 1 0
```

### Comparing `bhv-0.5.8/bhv/cnative/bindings.cpp` & `bhv-0.6.0a0/bhv/cnative/bindings.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #include <cstdlib>
-
+#define PY_SSIZE_T_CLEAN size_t
 #include <Python.h>
 #include "structmember.h"
 
 #include "packed.h"
 
 typedef struct {
     PyObject_HEAD
@@ -30,15 +30,17 @@
 static PyObject *BHV_random(PyTypeObject *type, PyObject *args);
 
 static PyObject *BHV_majority(PyTypeObject *type, PyObject *args);
 
 static PyObject *BHV_representative(PyTypeObject *type, PyObject *args);
 
 static PyObject *BHV_select(BHV *cond, PyObject *args);
-static PyObject *BHV_permute(BHV *v1, PyObject *args);
+static PyObject *BHV_permute(BHV *x, PyObject *args);
+static PyObject *BHV_rehash(BHV *x, PyObject *args);
+static PyObject *BHV_swap_halves(BHV *x, PyObject *args);
 
 static PyObject *BHV_eq(BHV *v1, PyObject *args);
 static PyObject *BHV_richcompare(PyObject *self, PyObject *other, int op) {
     switch (op) {
         case Py_EQ: if (bhv::eq(((BHV*)self)->data, ((BHV*)other)->data)) Py_RETURN_TRUE; else Py_RETURN_FALSE;
         case Py_NE: if (bhv::eq(((BHV*)self)->data, ((BHV*)other)->data)) Py_RETURN_FALSE; else Py_RETURN_TRUE;
         default:
@@ -50,14 +52,17 @@
 static PyObject *BHV_xor(PyObject *v1, PyObject *v2);
 static PyObject *BHV_and(PyObject *v1, PyObject *v2);
 static PyObject *BHV_or(PyObject *v1, PyObject *v2);
 static PyObject *BHV_invert(PyObject *v);
 
 static PyObject *BHV_hamming(BHV *v1, PyObject *args);
 
+static PyObject *BHV_to_bytes(BHV *x, PyObject *Py_UNUSED(ignored));
+static PyObject *BHV_from_bytes(PyTypeObject *type, PyObject *args);
+
 static PyObject *BHV_active(BHV *v, PyObject *Py_UNUSED(ignored)) {
     return Py_BuildValue("i", bhv::active(v->data));
 }
 
 static PyMemberDef BHV_members[] = {
         {nullptr}
 };
@@ -71,20 +76,28 @@
                 "The majority of a list of BHVs"},
         {"representative", (PyCFunction) BHV_representative, METH_CLASS | METH_VARARGS,
                 "Random representative of a list of BHVs"},
         {"select",         (PyCFunction) BHV_select,         METH_VARARGS,
                 "MUX or IF-THEN-ELSE"},
         {"permute",         (PyCFunction) BHV_permute,         METH_VARARGS,
                 "Word-level permutation"},
+        {"rehash",         (PyCFunction) BHV_rehash,         METH_NOARGS,
+                "Hash the vector into another vector"},
+        {"swap_halves",         (PyCFunction) BHV_swap_halves,         METH_NOARGS,
+                "Swap the halves of the vector"},
         {"eq",         (PyCFunction) BHV_eq,         METH_VARARGS,
                 "Check equality"},
         {"hamming",         (PyCFunction) BHV_hamming,         METH_VARARGS,
                 "Hamming distance between two BHVs"},
         {"active",         (PyCFunction) BHV_active,     METH_NOARGS,
                 "Count the number of active bits"},
+        {"to_bytes",         (PyCFunction) BHV_to_bytes,         METH_NOARGS,
+                "Bytes normalized form"},
+        {"from_bytes",         (PyCFunction) BHV_from_bytes,         METH_CLASS | METH_VARARGS,
+                "Construct from bytes normalized form"},
         {nullptr}
 };
 
 static PyNumberMethods BHV_nb_methods = {
     .nb_invert = (unaryfunc)BHV_invert,
     .nb_and = (binaryfunc)BHV_and,
     .nb_xor = (binaryfunc)BHV_xor,
@@ -242,22 +255,56 @@
         return nullptr;
 
     PyObject * ret = BHV_new(&BHVType, nullptr, nullptr);
     bhv::select_into(cond->data, when1->data, when0->data, ((BHV *) ret)->data);
     return ret;
 }
 
-static PyObject *BHV_permute(BHV *cond, PyObject *args) {
+static PyObject *BHV_permute(BHV *x, PyObject *args) {
     int32_t perm;
 
     if (!PyArg_ParseTuple(args, "i", &perm))
         return nullptr;
 
     PyObject * ret = BHV_new(&BHVType, nullptr, nullptr);
-    bhv::permute_into(cond->data, perm, ((BHV *) ret)->data);
+    bhv::permute_into(x->data, perm, ((BHV *) ret)->data);
+    return ret;
+}
+
+static PyObject *BHV_rehash(BHV *x, PyObject *args) {
+    PyObject * ret = BHV_new(&BHVType, nullptr, nullptr);
+    ((BHV *) ret)->data = bhv::zero();
+    bhv::rehash_into(x->data, ((BHV *) ret)->data);
+    return ret;
+}
+
+static PyObject *BHV_swap_halves(BHV *x, PyObject *args) {
+    PyObject * ret = BHV_new(&BHVType, nullptr, nullptr);
+    bhv::swap_halves_into(x->data, ((BHV *) ret)->data);
+    return ret;
+}
+
+static PyObject *BHV_to_bytes(BHV *x, PyObject *Py_UNUSED(ignored)) {
+    return PyBytes_FromStringAndSize((char*)x->data, BYTES);
+}
+
+static PyObject *BHV_from_bytes(PyTypeObject *type, PyObject *args) {
+    PyObject * ret = BHV_new(&BHVType, nullptr, nullptr);
+    char* buf;
+    size_t size;
+
+    if (!PyArg_ParseTuple(args, "s#", &buf, &size))
+        return nullptr;
+
+    if (size != BYTES) {
+        PyErr_SetString(PyExc_TypeError, "Bytes object didn't have the right size");
+        return nullptr;
+    }
+
+    memcpy(((BHV*)ret)->data, buf, BYTES);
     return ret;
 }
 
 static PyObject *dimension(PyObject * self, PyObject * args, PyObject * kwds) {
     return PyLong_FromLong(BITS);
 }
```

### Comparing `bhv-0.5.8/bhv/embedding.py` & `bhv-0.6.0a0/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.8/bhv/lookup.py` & `bhv-0.6.0a0/bhv/lookup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 K = TypeVar("K")
 
 
 class Store(Generic[K]):
     @classmethod
-    def auto_associative(cls, vs: Iterable[AbstractBHV]) -> 'StoreList[AbstractBHV]':
+    def auto_associative(cls, vs: Iterable[AbstractBHV]) -> 'Store[int]':
         return cls(dict(enumerate(vs)))
 
     def __init__(self, hvs: Mapping[K, AbstractBHV]):
         self.hvs = hvs
 
     def related(self, v: AbstractBHV, threshold=6) -> Iterator[K]:
         raise NotImplementedError()
```

### Comparing `bhv-0.5.8/bhv/native.py` & `bhv-0.6.0a0/bhv/native.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,13 +40,27 @@
 
     def hamming(self, other):
         return self.ins.hamming(other.ins)
 
     def permute(self, permutation_id: int):
         return NativePackedBHV(self.ins.permute(permutation_id))
 
+    def rehash(self):
+        return NativePackedBHV(self.ins.rehash())
+
+    def swap_halves(self):
+        return NativePackedBHV(self.ins.swap_halves())
+
     def __eq__(self, other):
         return self.ins == other.ins
 
+    @classmethod
+    def from_bytes(cls, bs):
+        return NativePackedBHV(CNativePackedBHV.from_bytes(bs))
+
+    def to_bytes(self):
+        return self.ins.to_bytes()
+
 NativePackedBHV.ZERO = NativePackedBHV(CNativePackedBHV.ZERO)
 NativePackedBHV.ONE = NativePackedBHV(CNativePackedBHV.ONE)
 NativePackedBHV.HALF = NativePackedBHV(CNativePackedBHV.HALF)
+NativePackedBHV._FEISTAL_SUBKEYS = NativePackedBHV.nrand2(NativePackedBHV._FEISTAL_ROUNDS, 4)
```

### Comparing `bhv-0.5.8/bhv/np.py` & `bhv-0.6.0a0/bhv/np.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,14 +89,24 @@
 
     def pack8(self) -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(np.packbits(self.data))
 
     def pack64(self) -> 'NumPyPacked64BHV':
         return NumPyPacked64BHV(np.packbits(self.data).view(dtype=np.uint64))
 
+    def to_bytes(self):
+        return self.pack8().to_bytes()
+
+    @classmethod
+    def from_bytes(cls, bs):
+        return NumPyPacked8BHV.from_bytes(bs).unpack()
+
+    def bits(self):
+        return iter(self.data.astype(np.uint8))
+
 NumPyBoolBHV.ZERO = NumPyBoolBHV(np.zeros(DIMENSION, dtype=np.bool_))
 NumPyBoolBHV.ONE = NumPyBoolBHV(np.ones(DIMENSION, dtype=np.bool_))
 NumPyBoolBHV._FEISTAL_SUBKEYS = NumPyBoolBHV.nrand2(NumPyBoolBHV._FEISTAL_ROUNDS, 4)
 _halfb = np.zeros(DIMENSION, dtype=np.bool_)
 _halfb[:DIMENSION//2] = np.bool_(True)
 NumPyBoolBHV.HALF = NumPyBoolBHV(_halfb)
 
@@ -147,18 +157,17 @@
     def permute_bytes(self, permutation: 'NumPyBytePermutation') -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(self.data[permutation.data])
 
     def permute(self, permutation_id: 'int | tuple[int, ...]') -> 'NumPyPacked8BHV':
         return self.permute_bytes(NumPyBytePermutation.get(permutation_id))
 
     def rehash(self) -> 'NumPyPacked8BHV':
-        byte_data = self.data.tobytes()
+        byte_data = self.to_bytes()
         rehashed_byte_data = hashlib.shake_256(byte_data).digest(DIMENSION//8)
-        rehashed_data = np.frombuffer(rehashed_byte_data, dtype=np.uint8)
-        return NumPyPacked8BHV(rehashed_data)
+        return NumPyPacked8BHV.from_bytes(rehashed_byte_data)
 
     def __eq__(self, other: 'NumPyPacked8BHV') -> bool:
         return np.array_equal(self.data, other.data)
 
     def __xor__(self, other: 'NumPyPacked8BHV') -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(np.bitwise_xor(self.data, other.data))
 
@@ -182,14 +191,22 @@
 
     def unpack(self) -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.unpackbits(self.data))
 
     def repack64(self) -> 'NumPyPacked64BHV':
         return NumPyPacked64BHV(self.data.view(dtype=np.uint64))
 
+    def to_bytes(self):
+        return self.data.tobytes()
+
+    @classmethod
+    def from_bytes(cls, bs):
+        return cls(np.frombuffer(bs, dtype=np.uint8))
+
+
 NumPyPacked8BHV.ZERO = NumPyPacked8BHV(np.zeros(DIMENSION//8, dtype=np.uint8))
 NumPyPacked8BHV.ONE = NumPyPacked8BHV(np.full(DIMENSION//8, fill_value=255, dtype=np.uint8))
 NumPyPacked8BHV._FEISTAL_SUBKEYS = NumPyPacked8BHV.nrand2(NumPyPacked8BHV._FEISTAL_ROUNDS, 4)
 _half8 = np.zeros(DIMENSION//8, dtype=np.uint8)
 _half8[:DIMENSION//16] = np.uint8(255)
 NumPyPacked8BHV.HALF = NumPyPacked8BHV(_half8)
 
@@ -250,21 +267,21 @@
         return self.repack8().rehash().repack64()
 
     def roll_words(self, n: int) -> 'NumPyPacked64BHV':
         assert abs(n) < DIMENSION//64, "only supports DIMENSION/64 rolls"
         return NumPyPacked64BHV(np.roll(self.data, n))
 
     def roll_word_bits(self, n: int) -> 'NumPyPacked64BHV':
-        assert abs(permutation_id) < 64, "only supports 64 rolls"
+        assert abs(n) < 64, "only supports 64 rolls"
         if n == 0:
             return NumPyPacked64BHV(self.data)
         elif n > 0:
-            return np.bitwise_or(np.right_shift(self.data, d), np.left_shift(self.data, (64 - d)))
+            return np.bitwise_or(np.right_shift(self.data, n), np.left_shift(self.data, (64 - n)))
         else:
-            return np.bitwise_or(np.left_shift(self.data, d), np.right_shift(self.data, (64 - d)))
+            return np.bitwise_or(np.left_shift(self.data, n), np.right_shift(self.data, (64 - n)))
 
     # roll_words and roll_word_bits could be combined for more options allowing positive and negative combinations
     # ((1 2 3 4) (a b c d) (α β γ δ))
     # rolled by 1, -2 for example results in
     # ((γ δ α β) (3 4 1 2) (c d a b))
 
     def permute_words(self, permutation: 'NumPyWordPermutation') -> 'NumPyPacked64BHV':
@@ -297,13 +314,20 @@
 
     def unpack(self) -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.unpackbits(self.data.view(np.uint8)))
 
     def repack8(self) -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(self.data.view(dtype=np.uint8))
 
+    def to_bytes(self):
+        return self.repack8().to_bytes()
+
+    @classmethod
+    def from_bytes(cls, bs):
+        return NumPyPacked8BHV.from_bytes(bs).repack64()
+
 NumPyPacked64BHV.ZERO = NumPyPacked64BHV(np.zeros(DIMENSION//64, dtype=np.uint64))
 NumPyPacked64BHV.ONE = NumPyPacked64BHV(np.full(DIMENSION//64, fill_value=-1, dtype=np.uint64))
 NumPyPacked64BHV._FEISTAL_SUBKEYS = NumPyPacked64BHV.nrand2(NumPyPacked64BHV._FEISTAL_ROUNDS, 4)
 _half64 = np.zeros(DIMENSION//64, dtype=np.uint64)
 _half64[:DIMENSION//128] = np.uint64(-1)
 NumPyPacked64BHV.HALF = NumPyPacked64BHV(_half64)
```

### Comparing `bhv-0.5.8/bhv/poibin.py` & `bhv-0.6.0a0/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.8/bhv/pytorch.py` & `bhv-0.6.0a0/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.8/bhv/shared.py` & `bhv-0.6.0a0/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.8/bhv/slice.py` & `bhv-0.6.0a0/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.8/bhv/symbolic.py` & `bhv-0.6.0a0/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.8/bhv/unification.py` & `bhv-0.6.0a0/bhv/unification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.8/bhv/vanilla.py` & `bhv-0.6.0a0/bhv/vanilla.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,12 +82,18 @@
     def to_int(self) -> int:
         return int.from_bytes(self.data, byteorder, signed=False)
 
     @classmethod
     def from_int(cls, i: int):
         return VanillaBHV(i.to_bytes(DIMENSION//8, byteorder, signed=False))
 
+    def to_bytes(self):
+        return self.data
+
+    @classmethod
+    def from_bytes(cls, bs):
+        return cls(bs)
 
 VanillaBHV.ZERO = VanillaBHV(bytes([0 for _ in range(DIMENSION//8)]))
 VanillaBHV.ONE = VanillaBHV(bytes([0xff for _ in range(DIMENSION//8)]))
 VanillaBHV._FEISTAL_SUBKEYS = VanillaBHV.nrand2(VanillaBHV._FEISTAL_ROUNDS, 4)
 VanillaBHV.HALF = VanillaBHV(bytes([0 for _ in range(DIMENSION//16)] + [0xff for _ in range(DIMENSION//16)]))
```

### Comparing `bhv-0.5.8/bhv/visualization.py` & `bhv-0.6.0a0/bhv/visualization.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .abstract import AbstractBHV
+from .abstract import AbstractBHV, DIMENSION
 
 
 class DistanceGraph:
     @classmethod
     def from_scope(cls, local_dict):
         return cls(*zip(*[(v, k) for k, v in local_dict.items() if isinstance(v, AbstractBHV)]))
 
@@ -15,7 +15,24 @@
 
     def graphviz(self):
         for i, (r, l) in enumerate(zip(self.adj, self.labels)):
             print(f"{i} [label=\"{l}\"];")
             for j, d in enumerate(r):
                 if d != 0 and i < j:
                     print(f"{i} -- {j} [label=\"{d}\"];")
+
+
+class Image:
+    def __init__(self, hvs: 'list[AbstractBHV]'):
+        self.hvs = hvs
+
+    def pbm(self, file: 'IO[Any]', binary=False):
+        if binary:
+            file.write(b"P4\n" + bytes(str(DIMENSION), "ascii") + b" " + bytes(str(len(self.hvs)), "ascii") + b"\n")
+            for hv in self.hvs:
+                file.write(hv.to_bytes())
+        else:
+            file.write(f"P1\n{DIMENSION} {len(self.hvs)}\n")
+            for hv in self.hvs:
+                for bit in hv.bits():
+                    file.write('1' if bit else '0')
+                file.write('\n')
```

### Comparing `bhv-0.5.8/bhv.egg-info/PKG-INFO` & `bhv-0.6.0a0/bhv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.5.8
+Version: 0.6.0a0
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
@@ -18,13 +18,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Provides-Extra: torch
-Provides-Extra: numpy
+Provides-Extra: pytorch
+Provides-Extra: np
 License-File: LICENSE
 
 Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).
```

### Comparing `bhv-0.5.8/setup.py` & `bhv-0.6.0a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from setuptools import setup, find_packages, Extension
 
-VERSION = '0.5.8'
+VERSION = '0.6.0a'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 native = Extension("bhv.cnative",
-                   sources=['bhv/cnative/bindings.cpp'],
-                   include_dirs=['bhv/cnative'],
+                   sources=['bhv/cnative/bindings.cpp',
+                            'bhv/cnative/TurboSHAKEref/TurboSHAKE.cpp',
+                            'bhv/cnative/TurboSHAKEref/KeccakSponge.cpp',
+                            'bhv/cnative/TurboSHAKEref/KeccakP-1600-reference.cpp',
+                            ],
+                   include_dirs=['bhv/cnative', 'bhv/cnative/TurboSHAKEref'],
                    extra_compile_args=['-std=c++2a', '-O3', '-march=native'],
                    language='c++')
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
     author_email="contact@adamv.be",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     url="https://github.com/Adam-Vandervorst/PyBHV",
     packages=find_packages(),
     install_requires=[],
     extras_require={
-        "torch": ["torch>=2.0.0"],
-        "numpy": ["numpy>=1.24.2"],
+        "pytorch": ["torch>=2.0.0"],
+        "np": ["numpy>=1.24.2"],
     },
     keywords='ai binary hypervector hdc bsc',
     python_requires='>=3.8',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
 
         'Intended Audience :: Developers',
```

