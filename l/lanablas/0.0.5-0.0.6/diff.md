# Comparing `tmp/lanablas-0.0.5.tar.gz` & `tmp/lanablas-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanablas-0.0.5.tar", last modified: Sat Jun 24 14:16:03 2023, max compression
+gzip compressed data, was "lanablas-0.0.6.tar", last modified: Sat Jun 24 15:01:34 2023, max compression
```

## Comparing `lanablas-0.0.5.tar` & `lanablas-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 14:16:03.949165 lanablas-0.0.5/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.5/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-06-24 14:16:03.948777 lanablas-0.0.5/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1047 2023-06-23 13:36:45.000000 lanablas-0.0.5/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 14:16:03.946147 lanablas-0.0.5/lanablas/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-24 09:52:46.000000 lanablas-0.0.5/lanablas/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10242 2023-06-24 14:15:59.000000 lanablas-0.0.5/lanablas/matrix.c
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 14:16:03.948170 lanablas-0.0.5/lanablas.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-06-24 14:16:03.000000 lanablas-0.0.5/lanablas.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-24 14:16:03.000000 lanablas-0.0.5/lanablas.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-24 14:16:03.000000 lanablas-0.0.5/lanablas.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-24 14:16:03.000000 lanablas-0.0.5/lanablas.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-24 14:16:03.949305 lanablas-0.0.5/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-24 09:51:56.000000 lanablas-0.0.5/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 15:01:34.597684 lanablas-0.0.6/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.6/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1959 2023-06-24 15:01:34.597449 lanablas-0.0.6/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1547 2023-06-24 14:55:58.000000 lanablas-0.0.6/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 15:01:34.594761 lanablas-0.0.6/lanablas/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-24 14:56:09.000000 lanablas-0.0.6/lanablas/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11138 2023-06-24 14:57:13.000000 lanablas-0.0.6/lanablas/matrix.c
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 15:01:34.597010 lanablas-0.0.6/lanablas.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1959 2023-06-24 15:01:33.000000 lanablas-0.0.6/lanablas.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-24 15:01:34.000000 lanablas-0.0.6/lanablas.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-24 15:01:33.000000 lanablas-0.0.6/lanablas.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-24 15:01:34.000000 lanablas-0.0.6/lanablas.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-24 15:01:34.597766 lanablas-0.0.6/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-24 14:56:02.000000 lanablas-0.0.6/setup.py
```

### Comparing `lanablas-0.0.5/LICENSE` & `lanablas-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lanablas-0.0.5/PKG-INFO` & `lanablas-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## LanaBLAS 🐑
 
-[![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) 
+[![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) [![macOS](https://img.shields.io/badge/macos-compatible-brightgreen.svg)](https://github.com/your-repo) [![Windows](https://img.shields.io/badge/windows-not%20compatible-red.svg)](https://github.com/your-repo) [![Linux](https://img.shields.io/badge/linux-not%20compatible-red.svg)](https://github.com/your-repo) [![Tests Passing](https://img.shields.io/badge/tests-passing-brightgreen.svg)](https://github.com/your-repo)
+
 
 **L***inear* **A**lgebra for **n***octurnal* *and* **a**dventurous *data scientists exploring **BLAS***
 
 
 **LanaBLAS** is a repository primarily used for testing the development of CPython extension modules with external dependencies, such as ([OpenBLAS](https://github.com/xianyi/OpenBLAS)). It's a work-in-progress memetic project aimed at having fun and learning new things.
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.4
+pip install lanablas==0.0.6
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
 
-zeros = Matrix.zeros(3,3)
-print(zeros)
-print(type(zeros), zeros.shape)
+a = Matrix.ones(3,3)
+print(a)
+print(type(a), a.shape)
+
+b = Matrix.eye(3)
+print(b)
+print(type(b), b.shape)
+
+c = a + b
+print(c)
+print(type(c), b.shape)
 ```
 
 For more comprehensive examples, please visit the [examples](https://github.com/marcosalvalaggio/lana-blas/tree/main/examples) folder
```

### Comparing `lanablas-0.0.5/README.md` & `lanablas-0.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 ## LanaBLAS 🐑
 
-[![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) 
+[![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) [![macOS](https://img.shields.io/badge/macos-compatible-brightgreen.svg)](https://github.com/your-repo) [![Windows](https://img.shields.io/badge/windows-not%20compatible-red.svg)](https://github.com/your-repo) [![Linux](https://img.shields.io/badge/linux-not%20compatible-red.svg)](https://github.com/your-repo) [![Tests Passing](https://img.shields.io/badge/tests-passing-brightgreen.svg)](https://github.com/your-repo)
+
 
 **L***inear* **A**lgebra for **n***octurnal* *and* **a**dventurous *data scientists exploring **BLAS***
 
 
 **LanaBLAS** is a repository primarily used for testing the development of CPython extension modules with external dependencies, such as ([OpenBLAS](https://github.com/xianyi/OpenBLAS)). It's a work-in-progress memetic project aimed at having fun and learning new things.
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.4
+pip install lanablas==0.0.6
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
 
-zeros = Matrix.zeros(3,3)
-print(zeros)
-print(type(zeros), zeros.shape)
+a = Matrix.ones(3,3)
+print(a)
+print(type(a), a.shape)
+
+b = Matrix.eye(3)
+print(b)
+print(type(b), b.shape)
+
+c = a + b
+print(c)
+print(type(c), b.shape)
 ```
 
 For more comprehensive examples, please visit the [examples](https://github.com/marcosalvalaggio/lana-blas/tree/main/examples) folder
```

### Comparing `lanablas-0.0.5/lanablas/__init__.py` & `lanablas-0.0.6/lanablas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union, List
 from matrix import Matrix
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 def inject(data: Union[float, int, List, List[List]]) -> List[List[float]]:
     """
     Injects the input data into a matrix.
 
     Args:
```

### Comparing `lanablas-0.0.5/lanablas/matrix.c` & `lanablas-0.0.6/lanablas/matrix.c`

 * *Files 3% similar despite different names*

```diff
@@ -251,27 +251,54 @@
         result->data[i] = malloc(result->cols * sizeof(double));
         for (int j = 0; j < result->cols; j++) {
             result->data[i][j] = selfMatrix->data[i][j] + otherMatrix->data[i][j];
         }
     }
 
     return (PyObject*)result;
-    // Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
-    // value->data = ((Value *)self)->data + ((Value *)other)->data;
-    // value->grad = 0.0;
-    // value->prev = PyTuple_Pack(2, self, other);
-    // value->op = PyUnicode_FromString("+");
-    // value->func_idx = 0;
-    // return (PyObject *)value;
+
+}
+
+
+PyObject * Matrix_subtract(PyObject *self, PyObject *other) {
+    // Cast the input objects to MatrixObject
+    MatrixObject* selfMatrix = (MatrixObject*)self;
+    MatrixObject* otherMatrix = (MatrixObject*)other;
+
+    // Check if the dimensions of the matrices are compatible for addition
+    if (selfMatrix->rows != otherMatrix->rows || selfMatrix->cols != otherMatrix->cols) {
+        PyErr_SetString(PyExc_ValueError, "Matrix dimensions are not compatible for addition");
+        return NULL;
+    }
+
+    // Create a new MatrixObject for the result
+    MatrixObject* result = (MatrixObject*)MatrixType.tp_alloc(&MatrixType, 0);
+    if (result == NULL) {
+        PyErr_SetString(PyExc_MemoryError, "Failed to allocate memory for result matrix");
+        return NULL;
+    }
+
+    result->rows = selfMatrix->rows;
+    result->cols = selfMatrix->cols;
+    result->data = malloc(result->rows * sizeof(double*));
+    for (int i = 0; i < result->rows; i++) {
+        result->data[i] = malloc(result->cols * sizeof(double));
+        for (int j = 0; j < result->cols; j++) {
+            result->data[i][j] = selfMatrix->data[i][j] - otherMatrix->data[i][j];
+        }
+    }
+
+    return (PyObject*)result;
+
 }
 
 
 PyNumberMethods Matrix_as_number = {
     Matrix_add,
-    0,
+    Matrix_subtract,
     0,
     0,
     0,
     0,
     0,
     0,
     0,
@@ -300,15 +327,14 @@
     0,
     0,
     0,
     0,
 };
 
 
-
 static PyObject* Matrix_repr(MatrixObject* self) {
     PyObject* result = PyUnicode_New(0, 0);
     for (int i = 0; i < self->rows; i++) {
         if (i == 0) {
             PyUnicode_AppendAndDel(&result, PyUnicode_FromString("Matrix(["));
         }
         PyUnicode_AppendAndDel(&result, PyUnicode_FromString("["));
```

### Comparing `lanablas-0.0.5/lanablas.egg-info/PKG-INFO` & `lanablas-0.0.6/lanablas.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## LanaBLAS 🐑
 
-[![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) 
+[![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) [![macOS](https://img.shields.io/badge/macos-compatible-brightgreen.svg)](https://github.com/your-repo) [![Windows](https://img.shields.io/badge/windows-not%20compatible-red.svg)](https://github.com/your-repo) [![Linux](https://img.shields.io/badge/linux-not%20compatible-red.svg)](https://github.com/your-repo) [![Tests Passing](https://img.shields.io/badge/tests-passing-brightgreen.svg)](https://github.com/your-repo)
+
 
 **L***inear* **A**lgebra for **n***octurnal* *and* **a**dventurous *data scientists exploring **BLAS***
 
 
 **LanaBLAS** is a repository primarily used for testing the development of CPython extension modules with external dependencies, such as ([OpenBLAS](https://github.com/xianyi/OpenBLAS)). It's a work-in-progress memetic project aimed at having fun and learning new things.
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.4
+pip install lanablas==0.0.6
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
 
-zeros = Matrix.zeros(3,3)
-print(zeros)
-print(type(zeros), zeros.shape)
+a = Matrix.ones(3,3)
+print(a)
+print(type(a), a.shape)
+
+b = Matrix.eye(3)
+print(b)
+print(type(b), b.shape)
+
+c = a + b
+print(c)
+print(type(c), b.shape)
 ```
 
 For more comprehensive examples, please visit the [examples](https://github.com/marcosalvalaggio/lana-blas/tree/main/examples) folder
```

### Comparing `lanablas-0.0.5/setup.py` & `lanablas-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     extra_compile_args=['-std=c11'],  # Set the C standard to C11
     include_dirs=['/usr/local/opt/openblas/include'],  # BLAS include directory
     library_dirs=['/usr/local/opt/openblas/lib'],  # BLAS library directory
 )
 
 setup(
 name='lanablas',
-    version='0.0.5',
+    version='0.0.6',
     description='Extension module for matrix multiplication',
     author='Marco Salvalaggio',
     author_email='mar.salvalaggio@gmail.com',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['lanablas'],
```

