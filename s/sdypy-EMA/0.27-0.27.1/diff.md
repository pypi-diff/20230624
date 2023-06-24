# Comparing `tmp/sdypy-EMA-0.27.tar.gz` & `tmp/sdypy-EMA-0.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdypy-EMA-0.27.tar", last modified: Tue Apr 18 13:00:35 2023, max compression
+gzip compressed data, was "sdypy-EMA-0.27.1.tar", last modified: Sat Jun 24 09:21:49 2023, max compression
```

## Comparing `sdypy-EMA-0.27.tar` & `sdypy-EMA-0.27.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 13:00:35.861803 sdypy-EMA-0.27/
--rw-rw-rw-   0        0        0     1091 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/LICENSE
--rw-rw-rw-   0        0        0     2873 2023-04-18 13:00:35.861803 sdypy-EMA-0.27/PKG-INFO
--rw-rw-rw-   0        0        0     2489 2023-04-18 12:59:27.000000 sdypy-EMA-0.27/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 13:00:35.837794 sdypy-EMA-0.27/sdypy/
-drwxrwxrwx   0        0        0        0 2023-04-18 13:00:35.845804 sdypy-EMA-0.27/sdypy/EMA/
--rw-rw-rw-   0        0        0    40478 2023-04-18 09:40:09.000000 sdypy-EMA-0.27/sdypy/EMA/EMA.py
--rw-rw-rw-   0        0        0      174 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/sdypy/EMA/__init__.py
--rw-rw-rw-   0        0        0     4779 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/sdypy/EMA/normal_modes.py
--rw-rw-rw-   0        0        0    18198 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/sdypy/EMA/pole_picking.py
--rw-rw-rw-   0        0        0     3376 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/sdypy/EMA/stabilization.py
--rw-rw-rw-   0        0        0     4620 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/sdypy/EMA/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:00:35.861803 sdypy-EMA-0.27/sdypy_EMA.egg-info/
--rw-rw-rw-   0        0        0     2873 2023-04-18 13:00:35.000000 sdypy-EMA-0.27/sdypy_EMA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-04-18 13:00:35.000000 sdypy-EMA-0.27/sdypy_EMA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 13:00:35.000000 sdypy-EMA-0.27/sdypy_EMA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-04-18 13:00:35.000000 sdypy-EMA-0.27/sdypy_EMA.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-18 13:00:35.000000 sdypy-EMA-0.27/sdypy_EMA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 13:00:35.861803 sdypy-EMA-0.27/setup.cfg
--rw-rw-rw-   0        0        0     1474 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:21:49.748250 sdypy-EMA-0.27.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-18 09:31:04.000000 sdypy-EMA-0.27.1/LICENSE
+-rw-rw-rw-   0        0        0     2913 2023-06-24 09:21:49.748250 sdypy-EMA-0.27.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2489 2023-04-18 12:59:27.000000 sdypy-EMA-0.27.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-24 09:21:49.728487 sdypy-EMA-0.27.1/sdypy/
+drwxrwxrwx   0        0        0        0 2023-06-24 09:21:49.748250 sdypy-EMA-0.27.1/sdypy/EMA/
+-rw-rw-rw-   0        0        0    40490 2023-06-24 09:20:13.000000 sdypy-EMA-0.27.1/sdypy/EMA/EMA.py
+-rw-rw-rw-   0        0        0      176 2023-06-24 09:20:13.000000 sdypy-EMA-0.27.1/sdypy/EMA/__init__.py
+-rw-rw-rw-   0        0        0     4779 2023-04-18 09:31:04.000000 sdypy-EMA-0.27.1/sdypy/EMA/normal_modes.py
+-rw-rw-rw-   0        0        0    18198 2023-04-18 09:31:04.000000 sdypy-EMA-0.27.1/sdypy/EMA/pole_picking.py
+-rw-rw-rw-   0        0        0     3516 2023-06-24 09:20:13.000000 sdypy-EMA-0.27.1/sdypy/EMA/stabilization.py
+-rw-rw-rw-   0        0        0     4648 2023-06-24 09:20:13.000000 sdypy-EMA-0.27.1/sdypy/EMA/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-24 09:21:49.748250 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/
+-rw-rw-rw-   0        0        0     2913 2023-06-24 09:21:49.000000 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-06-24 09:21:49.000000 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 09:21:49.000000 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-06-24 09:21:49.000000 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-24 09:21:49.000000 sdypy-EMA-0.27.1/sdypy_EMA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 09:21:49.748250 sdypy-EMA-0.27.1/setup.cfg
+-rw-rw-rw-   0        0        0     1525 2023-06-24 09:20:13.000000 sdypy-EMA-0.27.1/setup.py
```

### Comparing `sdypy-EMA-0.27/LICENSE` & `sdypy-EMA-0.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.27/PKG-INFO` & `sdypy-EMA-0.27.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: sdypy-EMA
-Version: 0.27
+Version: 0.27.1
 Summary: Experimental and operational modal analysis.
 Home-page: https://github.com/ladisk/pyEMA
 Author: Klemen Zaletelj, Domen Gorjup, Janko Slavič, Tomaž Bregar, Miha Pogačar, et al.
 Maintainer: Janko Slavič
 Maintainer-email: janko.slavic@fs.uni-lj.si
 License: UNKNOWN
 Platform: UNKNOWN
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 sdypy-EMA
 =========
 
 Experimental and operational modal analysis
```

### Comparing `sdypy-EMA-0.27/README.rst` & `sdypy-EMA-0.27.1/README.rst`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.27/sdypy/EMA/EMA.py` & `sdypy-EMA-0.27.1/sdypy/EMA/EMA.py`

 * *Files 0% similar despite different names*

```diff
@@ -926,15 +926,15 @@
     # weights = np.tile(np.sqrt(np.arange(lower_ind, upper_ind)), 2) # with sqrt
     # W = np.diag(weights/np.max(weights))
     # weights = np.tile(np.sum(1/((freq[:, None] - f)**2 + 1e5), axis=1), 2)[mask]
     # W = np.diag(weights/np.max(weights))
     # A_ = np.linalg.lstsq(W@P[mask], W@Y[mask])[0].T
 
 
-    A_ = np.linalg.lstsq(P[mask], Y[mask])[0].T
+    A_ = np.linalg.lstsq(P[mask], Y[mask], rcond=None)[0].T
     # modal constants
     Ar, Ai = np.split(A_[:, :2*w.shape[0]], 2, axis=1)
     A = Ar + 1j*Ai
 
    
     # residuals
     if lower_r == True and upper_r == True:
```

### Comparing `sdypy-EMA-0.27/sdypy/EMA/normal_modes.py` & `sdypy-EMA-0.27.1/sdypy/EMA/normal_modes.py`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.27/sdypy/EMA/pole_picking.py` & `sdypy-EMA-0.27.1/sdypy/EMA/pole_picking.py`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.27/sdypy/EMA/stabilization.py` & `sdypy-EMA-0.27.1/sdypy/EMA/stabilization.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,18 +69,21 @@
             # previous (N-1-th) data (eigenfrequencies). If the value equals:
             # --> 1, the data is within relative tolerance err_fn
             # --> 0, the data is outside the relative tolerance err_fn
             fn_test = np.zeros((len(fn), len(fn_temp[:, n - 1])), dtype='int')
             xi_test = np.zeros((len(xi), len(xi_temp[:, n - 1])), dtype='int')
 
             for i in range(len(fn)):
+                fn_temp[:, n-2][fn_temp[:, n-2] == 0] = 1e-10
+                xi_temp[:, n-2][xi_temp[:, n-2] == 0] = 1e-10
+                
                 fn_test[i, np.abs((fn[i] - fn_temp[:, n-2]) /
-                                  fn_temp[:, n-2]) < err_fn] = 1
+                                fn_temp[:, n-2]) < err_fn] = 1
                 xi_test[i, np.abs((xi[i] - xi_temp[:, n-2]) /
-                                  xi_temp[:, n-2]) < err_xi] = 1
+                                xi_temp[:, n-2]) < err_xi] = 1
 
                 fn_temp[i, n - 1] = fn[i]
                 xi_temp[i, n - 1] = xi[i]
 
                 test_fn[i, n-1] = np.sum(fn_test[i, :2*n])
                 test_xi[i, n-1] = np.sum(xi_test[i, :2*n])
```

### Comparing `sdypy-EMA-0.27/sdypy/EMA/tools.py` & `sdypy-EMA-0.27.1/sdypy/EMA/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     and :math:`\\zeta_r` are the :math:`r` th natural frequency [rad/s] and damping, respectively.
 
     :param sr: complex natural frequencies
     :return: natural frequency [Hz] and damping
     """
     # Extract natural frequency
     fr = np.sign(np.imag(sr)) * np.abs(sr)
+
+    fr[fr == 0] = -1e-10
     
     # Extract damping
     xir = -sr.real/fr
     
     # Convert natural frequency to Hz
     fr /= (2 * np.pi)
```

### Comparing `sdypy-EMA-0.27/sdypy_EMA.egg-info/PKG-INFO` & `sdypy-EMA-0.27.1/sdypy_EMA.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: sdypy-EMA
-Version: 0.27
+Version: 0.27.1
 Summary: Experimental and operational modal analysis.
 Home-page: https://github.com/ladisk/pyEMA
 Author: Klemen Zaletelj, Domen Gorjup, Janko Slavič, Tomaž Bregar, Miha Pogačar, et al.
 Maintainer: Janko Slavič
 Maintainer-email: janko.slavic@fs.uni-lj.si
 License: UNKNOWN
 Platform: UNKNOWN
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 sdypy-EMA
 =========
 
 Experimental and operational modal analysis
```

### Comparing `sdypy-EMA-0.27/setup.py` & `sdypy-EMA-0.27.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,9 +41,10 @@
       author='Klemen Zaletelj, Domen Gorjup, Janko Slavič, Tomaž Bregar, Miha Pogačar, et al.',
       maintainer='Janko Slavič',
       maintainer_email='janko.slavic@fs.uni-lj.si',
       description='Experimental and operational modal analysis.',
       url='https://github.com/ladisk/pyEMA',
       packages=['sdypy.EMA'],
       long_description=readme,
+      long_description_content_type='text/x-rst',
       install_requires=requirements
       )
```

