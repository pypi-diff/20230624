# Comparing `tmp/lanablas-0.0.4.tar.gz` & `tmp/lanablas-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanablas-0.0.4.tar", last modified: Fri Jun 23 13:29:59 2023, max compression
+gzip compressed data, was "lanablas-0.0.5.tar", last modified: Sat Jun 24 14:16:03 2023, max compression
```

## Comparing `lanablas-0.0.4.tar` & `lanablas-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 13:29:59.231470 lanablas-0.0.4/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.4/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-06-23 13:29:59.231239 lanablas-0.0.4/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1047 2023-06-23 12:38:32.000000 lanablas-0.0.4/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 13:29:59.229360 lanablas-0.0.4/lanablas/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-23 13:22:23.000000 lanablas-0.0.4/lanablas/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8357 2023-06-23 13:26:46.000000 lanablas-0.0.4/lanablas/matrix.c
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 13:29:59.230884 lanablas-0.0.4/lanablas.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-06-23 13:29:58.000000 lanablas-0.0.4/lanablas.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-23 13:29:59.000000 lanablas-0.0.4/lanablas.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-23 13:29:58.000000 lanablas-0.0.4/lanablas.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-23 13:29:58.000000 lanablas-0.0.4/lanablas.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-23 13:29:59.231561 lanablas-0.0.4/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-23 13:22:17.000000 lanablas-0.0.4/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 14:16:03.949165 lanablas-0.0.5/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.5/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-06-24 14:16:03.948777 lanablas-0.0.5/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1047 2023-06-23 13:36:45.000000 lanablas-0.0.5/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 14:16:03.946147 lanablas-0.0.5/lanablas/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-24 09:52:46.000000 lanablas-0.0.5/lanablas/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10242 2023-06-24 14:15:59.000000 lanablas-0.0.5/lanablas/matrix.c
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 14:16:03.948170 lanablas-0.0.5/lanablas.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-06-24 14:16:03.000000 lanablas-0.0.5/lanablas.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-24 14:16:03.000000 lanablas-0.0.5/lanablas.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-24 14:16:03.000000 lanablas-0.0.5/lanablas.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-24 14:16:03.000000 lanablas-0.0.5/lanablas.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-24 14:16:03.949305 lanablas-0.0.5/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-24 09:51:56.000000 lanablas-0.0.5/setup.py
```

### Comparing `lanablas-0.0.4/LICENSE` & `lanablas-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lanablas-0.0.4/PKG-INFO` & `lanablas-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.3
+pip install lanablas==0.0.4
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
```

### Comparing `lanablas-0.0.4/README.md` & `lanablas-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.3
+pip install lanablas==0.0.4
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
```

### Comparing `lanablas-0.0.4/lanablas/__init__.py` & `lanablas-0.0.5/lanablas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union, List
 from matrix import Matrix
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 
 def inject(data: Union[float, int, List, List[List]]) -> List[List[float]]:
     """
     Injects the input data into a matrix.
 
     Args:
```

### Comparing `lanablas-0.0.4/lanablas/matrix.c` & `lanablas-0.0.5/lanablas/matrix.c`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 typedef struct {
     PyObject_HEAD
     int rows;
     int cols;
     double** data;
 } MatrixObject;
 
+static PyTypeObject MatrixType;
 
 static PyObject* Matrix_new(PyTypeObject* type, PyObject* args) {
 
     PyObject* pyList;
     if (!PyArg_ParseTuple(args, "O", &pyList)) {
         PyErr_SetString(PyExc_TypeError, "Invalid argument: expected a list");
         return NULL;
@@ -171,15 +172,14 @@
     }
 
     return (PyObject*)matrix;
 
 }
 
 
-
 static PyObject* Matrix_shape(MatrixObject* self) {
     PyObject* shape = PyTuple_New(2);
     PyObject* rows = PyLong_FromLong(self->rows);
     PyObject* cols = PyLong_FromLong(self->cols);
     PyTuple_SetItem(shape, 0, rows);
     PyTuple_SetItem(shape, 1, cols);
     return shape;
@@ -222,14 +222,93 @@
 
 static PyGetSetDef Matrix_getsetters[] = {
     {"shape", (getter)Matrix_shape, NULL, "Return the shape of the matrix as a tuple", NULL},
     {NULL}
 };
 
 
+PyObject * Matrix_add(PyObject *self, PyObject *other) {
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
+            result->data[i][j] = selfMatrix->data[i][j] + otherMatrix->data[i][j];
+        }
+    }
+
+    return (PyObject*)result;
+    // Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
+    // value->data = ((Value *)self)->data + ((Value *)other)->data;
+    // value->grad = 0.0;
+    // value->prev = PyTuple_Pack(2, self, other);
+    // value->op = PyUnicode_FromString("+");
+    // value->func_idx = 0;
+    // return (PyObject *)value;
+}
+
+
+PyNumberMethods Matrix_as_number = {
+    Matrix_add,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+};
+
+
+
 static PyObject* Matrix_repr(MatrixObject* self) {
     PyObject* result = PyUnicode_New(0, 0);
     for (int i = 0; i < self->rows; i++) {
         if (i == 0) {
             PyUnicode_AppendAndDel(&result, PyUnicode_FromString("Matrix(["));
         }
         PyUnicode_AppendAndDel(&result, PyUnicode_FromString("["));
@@ -258,14 +337,15 @@
     .tp_doc = "Matrix object",
     .tp_basicsize = sizeof(MatrixObject),
     .tp_itemsize = 0,
     .tp_flags = Py_TPFLAGS_DEFAULT,
     .tp_new = PyType_GenericNew,
     .tp_dealloc = (destructor)Matrix_dealloc,
     .tp_repr = (reprfunc)Matrix_repr,
+    .tp_as_number = &Matrix_as_number,
     .tp_methods = MatrixExtensionMethods,
     .tp_getset = Matrix_getsetters,
 };
 
 
 static struct PyModuleDef matrix_extension_module = {
     PyModuleDef_HEAD_INIT,
```

### Comparing `lanablas-0.0.4/lanablas.egg-info/PKG-INFO` & `lanablas-0.0.5/lanablas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.3
+pip install lanablas==0.0.4
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
```

### Comparing `lanablas-0.0.4/setup.py` & `lanablas-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     extra_compile_args=['-std=c11'],  # Set the C standard to C11
     include_dirs=['/usr/local/opt/openblas/include'],  # BLAS include directory
     library_dirs=['/usr/local/opt/openblas/lib'],  # BLAS library directory
 )
 
 setup(
 name='lanablas',
-    version='0.0.4',
+    version='0.0.5',
     description='Extension module for matrix multiplication',
     author='Marco Salvalaggio',
     author_email='mar.salvalaggio@gmail.com',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['lanablas'],
```

