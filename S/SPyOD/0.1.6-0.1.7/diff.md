# Comparing `tmp/SPyOD-0.1.6.tar.gz` & `tmp/SPyOD-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPyOD-0.1.6.tar", last modified: Tue Jun  6 02:47:44 2023, max compression
+gzip compressed data, was "SPyOD-0.1.7.tar", last modified: Sat Jun 24 12:49:04 2023, max compression
```

## Comparing `SPyOD-0.1.6.tar` & `SPyOD-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:47:44.210894 SPyOD-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-06 02:47:27.000000 SPyOD-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-06 02:47:44.210894 SPyOD-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-06 02:47:27.000000 SPyOD-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-06 02:47:28.000000 SPyOD-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 02:47:44.210894 SPyOD-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:47:44.206894 SPyOD-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:47:44.206894 SPyOD-0.1.6/src/SPyOD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-06 02:47:44.000000 SPyOD-0.1.6/src/SPyOD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-06 02:47:44.000000 SPyOD-0.1.6/src/SPyOD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:47:44.000000 SPyOD-0.1.6/src/SPyOD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 02:47:44.000000 SPyOD-0.1.6/src/SPyOD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:47:44.210894 SPyOD-0.1.6/src/spyod/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 02:47:28.000000 SPyOD-0.1.6/src/spyod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-06 02:47:28.000000 SPyOD-0.1.6/src/spyod/findpairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-06-06 02:47:28.000000 SPyOD-0.1.6/src/spyod/spod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:49:04.198551 SPyOD-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-24 12:48:52.000000 SPyOD-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-24 12:49:04.198551 SPyOD-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-24 12:48:52.000000 SPyOD-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-24 12:48:52.000000 SPyOD-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 12:49:04.198551 SPyOD-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:49:04.198551 SPyOD-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:49:04.198551 SPyOD-0.1.7/src/SPyOD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-24 12:49:04.000000 SPyOD-0.1.7/src/SPyOD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-24 12:49:04.000000 SPyOD-0.1.7/src/SPyOD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 12:49:04.000000 SPyOD-0.1.7/src/SPyOD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 12:49:04.000000 SPyOD-0.1.7/src/SPyOD.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:49:04.198551 SPyOD-0.1.7/src/spyod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 12:48:52.000000 SPyOD-0.1.7/src/spyod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-24 12:48:52.000000 SPyOD-0.1.7/src/spyod/findpairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-06-24 12:48:52.000000 SPyOD-0.1.7/src/spyod/spod.py
```

### Comparing `SPyOD-0.1.6/LICENSE` & `SPyOD-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SPyOD-0.1.6/PKG-INFO` & `SPyOD-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPyOD
-Version: 0.1.6
+Version: 0.1.7
 Summary: Spectral Proper Orthogonal Decomposition
 Author-email: Grigorios Hatzissawidis <grigorios.hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber <moritz.sieber@tu-berlin.de>
 Project-URL: Homepage, https://github.com/grigorishat/SPyOD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SPyOD Version: 0.1.6 Summary: Spectral Proper
+Metadata-Version: 2.1 Name: SPyOD Version: 0.1.7 Summary: Spectral Proper
 Orthogonal Decomposition Author-email: Grigorios Hatzissawidis
 hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber
 sieber@tu-berlin.de> Project-URL: Homepage, https://github.com/grigorishat/
 SPyOD Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # Spectral Proper Orthogonal Decomposition ## Table of contents *
```

### Comparing `SPyOD-0.1.6/README.md` & `SPyOD-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `SPyOD-0.1.6/pyproject.toml` & `SPyOD-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SPyOD"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Grigorios Hatzissawidis", email="grigorios.hatzissawidis@fst.tu-darmstadt.de" },
   { name="Moritz Sieber", email="moritz.sieber@tu-berlin.de" },
 ]
 description = "Spectral Proper Orthogonal Decomposition"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `SPyOD-0.1.6/src/SPyOD.egg-info/PKG-INFO` & `SPyOD-0.1.7/src/SPyOD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPyOD
-Version: 0.1.6
+Version: 0.1.7
 Summary: Spectral Proper Orthogonal Decomposition
 Author-email: Grigorios Hatzissawidis <grigorios.hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber <moritz.sieber@tu-berlin.de>
 Project-URL: Homepage, https://github.com/grigorishat/SPyOD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SPyOD Version: 0.1.6 Summary: Spectral Proper
+Metadata-Version: 2.1 Name: SPyOD Version: 0.1.7 Summary: Spectral Proper
 Orthogonal Decomposition Author-email: Grigorios Hatzissawidis
 hatzissawidis@fst.tu-darmstadt.de>, Moritz Sieber
 sieber@tu-berlin.de> Project-URL: Homepage, https://github.com/grigorishat/
 SPyOD Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # Spectral Proper Orthogonal Decomposition ## Table of contents *
```

### Comparing `SPyOD-0.1.6/src/spyod/findpairs.py` & `SPyOD-0.1.7/src/spyod/findpairs.py`

 * *Files identical despite different names*

### Comparing `SPyOD-0.1.6/src/spyod/spod.py` & `SPyOD-0.1.7/src/spyod/spod.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,39 +101,29 @@
         for i in range(Ncomp):
             U = np.transpose(args[i]).reshape((Ngrid, Nsnap))
             R = R + U.transpose() * Wxyz @ U
         R = R / Nsnap / np.sum(Wxyz)
 
         # calculate filtered correlation matrix S
 
-        if boundary == "periodic":
-            # convolve periodically extended matrix with filtered diagonal matrix
-
-            ind = np.array(range(1-Nfilt, Nsnap + Nfilt + 1))
-            ind = np.mod(ind - 1, Nsnap)
-            #S = convolve2d(R[np.ix_(ind, ind)], np.diag(f), mode = "valid")
-            S = fftconvolve(R[np.ix_(ind, ind)], np.diag(f), mode = "valid")
-
-
         # dft case
-        elif boundary == "DFTcase":
+        if boundary == "DFTcase":
             rr = np.zeros(Nsnap)
             for i in range(Nsnap):
                 rr[i] = np.sum(np.diag(R, i)) * f[0]
 
             # periodic boundary condition -> circulant matrix
             rr[1:] = rr[1:] + rr[:0:-1]
             S = toeplitz(rr)
 
-        # convolve zero padded matrix with filter diagonal matrix
-        # ("center" differs from matlab if number of rows/ columns is odd)
+        # if boundary is zero padded or periodic use the function convdiag
+        elif boundary == "zeros" or boundary == "periodic":
+            S = convdiag(R, np.diag(f), boundary=boundary)
+
 
-        elif boundary == "zeros":
-            #S = convolve2d(R,np.diag(f), mode = "same")
-            S = fftconvolve(R, np.diag(f), mode="same") # much faster than convolve2d
 
         # calculate eigenvalues and eigenvectors of S and sort in descending order
         # distinguish between DFTcase and periodic/ zeros, since eigh is used for symmetric matrices
 
         if boundary == "DFTcase":
 
             w, v = np.linalg.eigh(S, UPLO='U')
@@ -411,8 +401,38 @@
     if filt_type == 'box':
         f = np.ones(N_filt, dtype=precision)
     elif filt_type == 'gauss':
         f = np.exp(-np.linspace(-2.285, 2.285, 2 * N_filt + 1)**2, dtype=precision)
     else:
         raise Exception('unknown filter type.')
     f = f / np.sum(f)
-    return f
+    return f
+
+def convdiag(matrix, diagonal_matrix, boundary):
+    """_summary_
+
+    Args:
+        matrix R (numpy array): input covariance matrix to be convolved
+        diagonal_matrix (_type_): kernel as a diagonal matrix
+        boundary (_type_): 'zeros' or 'periodic' boundaries of the matrix
+
+    Raises:
+        ValueError: if boundary is not valid 
+
+    Returns:
+        matrix S: filtered covariance matrix
+    """
+    m, n = matrix.shape # should be m=n which is nsnap
+    d = diagonal_matrix.shape[0]
+    D = np.diag(diagonal_matrix)
+    pad_width = d // 2 # or Nfilt
+    if boundary == 'zeros':
+        padded_matrix = np.pad(matrix, pad_width, mode='constant')
+    elif boundary == 'periodic':
+        ind = np.array(range(1 - pad_width, m + pad_width + 1))
+        ind = np.mod(ind - 1, m)
+        padded_matrix = matrix[np.ix_(ind, ind)]
+    else:
+        raise ValueError("Boundary must be 'zeros' or 'periodic'.")
+    s0, s1 = padded_matrix.strides
+    MM=np.lib.stride_tricks.as_strided(padded_matrix, shape=(m, n, d), strides=(s0, s1, s0+s1))
+    return MM@D
```

