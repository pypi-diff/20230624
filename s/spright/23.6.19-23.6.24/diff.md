# Comparing `tmp/spright-23.6.19.tar.gz` & `tmp/spright-23.6.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spright-23.6.19.tar", last modified: Mon Jun 19 19:47:04 2023, max compression
+gzip compressed data, was "spright-23.6.24.tar", last modified: Sat Jun 24 18:06:56 2023, max compression
```

## Comparing `spright-23.6.19.tar` & `spright-23.6.24.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-19 19:47:04.990763 spright-23.6.19/
--rw-r--r--   0 hannu     (1000) hannu     (1000)    35149 2022-10-08 15:41:02.000000 spright-23.6.19/LICENSE
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       19 2022-10-24 17:07:23.000000 spright-23.6.19/MANIFEST.in
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      648 2023-06-19 19:47:04.990763 spright-23.6.19/PKG-INFO
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      544 2023-06-16 10:55:09.000000 spright-23.6.19/README.md
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      950 2023-06-19 19:46:51.000000 spright-23.6.19/pyproject.toml
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       38 2023-06-19 19:47:04.990763 spright-23.6.19/setup.cfg
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-19 19:47:04.990763 spright-23.6.19/spright/
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      113 2023-06-16 11:10:55.000000 spright-23.6.19/spright/__init__.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      686 2023-06-16 11:10:55.000000 spright-23.6.19/spright/core.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)     4057 2023-06-16 11:10:55.000000 spright-23.6.19/spright/distribution.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)     1740 2023-06-16 11:10:55.000000 spright-23.6.19/spright/io.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)     3119 2023-06-16 11:10:55.000000 spright-23.6.19/spright/lpf.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)    10904 2023-06-16 11:10:55.000000 spright-23.6.19/spright/model.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)     3147 2023-06-16 11:10:55.000000 spright-23.6.19/spright/rdmodel.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)    11166 2023-06-16 11:10:55.000000 spright-23.6.19/spright/rmestimator.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)     3723 2023-06-16 11:10:55.000000 spright-23.6.19/spright/rmrelation.py
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       67 2023-06-16 11:10:55.000000 spright-23.6.19/spright/version.py
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-19 19:47:04.990763 spright-23.6.19/spright.egg-info/
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      648 2023-06-19 19:47:04.000000 spright-23.6.19/spright.egg-info/PKG-INFO
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      414 2023-06-19 19:47:04.000000 spright-23.6.19/spright.egg-info/SOURCES.txt
--rw-rw-r--   0 hannu     (1000) hannu     (1000)        1 2023-06-19 19:47:04.000000 spright-23.6.19/spright.egg-info/dependency_links.txt
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       76 2023-06-19 19:47:04.000000 spright-23.6.19/spright.egg-info/requires.txt
--rw-rw-r--   0 hannu     (1000) hannu     (1000)        8 2023-06-19 19:47:04.000000 spright-23.6.19/spright.egg-info/top_level.txt
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-19 19:47:04.990763 spright-23.6.19/tests/
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       58 2023-06-16 16:52:08.000000 spright-23.6.19/tests/test_installation.py
+drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-24 18:06:56.217131 spright-23.6.24/
+-rw-r--r--   0 hannu     (1000) hannu     (1000)    35149 2022-10-08 15:41:02.000000 spright-23.6.24/LICENSE
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)       19 2022-10-24 17:07:23.000000 spright-23.6.24/MANIFEST.in
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      655 2023-06-24 18:06:56.217131 spright-23.6.24/PKG-INFO
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      544 2023-06-16 10:55:09.000000 spright-23.6.24/README.md
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      957 2023-06-24 18:05:26.000000 spright-23.6.24/pyproject.toml
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)       38 2023-06-24 18:06:56.217131 spright-23.6.24/setup.cfg
+drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-24 18:06:56.209131 spright-23.6.24/spright/
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      113 2023-06-16 11:10:55.000000 spright-23.6.24/spright/__init__.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      686 2023-06-16 11:10:55.000000 spright-23.6.24/spright/core.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     4057 2023-06-16 11:10:55.000000 spright-23.6.24/spright/distribution.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     1740 2023-06-16 11:10:55.000000 spright-23.6.24/spright/io.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     3119 2023-06-16 11:10:55.000000 spright-23.6.24/spright/lpf.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)    10980 2023-06-24 18:03:22.000000 spright-23.6.24/spright/model.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     3147 2023-06-16 11:10:55.000000 spright-23.6.24/spright/rdmodel.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)    11166 2023-06-16 11:10:55.000000 spright-23.6.24/spright/rmestimator.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)     3722 2023-06-22 14:20:14.000000 spright-23.6.24/spright/rmrelation.py
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)       67 2023-06-16 11:10:55.000000 spright-23.6.24/spright/version.py
+drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-24 18:06:56.209131 spright-23.6.24/spright.egg-info/
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      655 2023-06-24 18:06:56.000000 spright-23.6.24/spright.egg-info/PKG-INFO
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)      414 2023-06-24 18:06:56.000000 spright-23.6.24/spright.egg-info/SOURCES.txt
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)        1 2023-06-24 18:06:56.000000 spright-23.6.24/spright.egg-info/dependency_links.txt
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)       76 2023-06-24 18:06:56.000000 spright-23.6.24/spright.egg-info/requires.txt
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)        8 2023-06-24 18:06:56.000000 spright-23.6.24/spright.egg-info/top_level.txt
+drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2023-06-24 18:06:56.209131 spright-23.6.24/tests/
+-rw-rw-r--   0 hannu     (1000) hannu     (1000)       58 2023-06-16 16:52:08.000000 spright-23.6.24/tests/test_installation.py
```

### Comparing `spright-23.6.19/LICENSE` & `spright-23.6.24/LICENSE`

 * *Files identical despite different names*

### Comparing `spright-23.6.19/PKG-INFO` & `spright-23.6.24/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: spright
-Version: 23.6.19
+Version: 23.6.24
 Summary: Bayesian radius-density-mass relation for small planets.
 Author-email: Hannu Parviainen <hpparvi@gmail.com>
-Project-URL: homepage, https://github.com/hpparvi/
+Project-URL: homepage, https://github.com/hpparvi/spright
 Keywords: astronomy,astrophysics,exoplanets
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `spright-23.6.19/README.md` & `spright-23.6.24/README.md`

 * *Files identical despite different names*

### Comparing `spright-23.6.19/pyproject.toml` & `spright-23.6.24/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spright"
-version = "23.06.19"
+version = "23.06.24"
 description = 'Bayesian radius-density-mass relation for small planets.'
 authors=[{name='Hannu Parviainen', email='hpparvi@gmail.com'}]
 classifiers=[
   "Topic :: Scientific/Engineering",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "Development Status :: 5 - Production/Stable",
@@ -12,15 +12,15 @@
   "Operating System :: OS Independent",
   "Programming Language :: Python",
 ]
 keywords = ['astronomy',  'astrophysics',  'exoplanets']
 dependencies = ["numpy", "numba", "scipy", "pandas", "astropy", "pytransit", "arviz", "corner", "tqdm", "celerite", "emcee"]
 
 [project.urls]
-homepage = 'https://github.com/hpparvi/'
+homepage = 'https://github.com/hpparvi/spright'
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `spright-23.6.19/spright/core.py` & `spright-23.6.24/spright/core.py`

 * *Files identical despite different names*

### Comparing `spright-23.6.19/spright/distribution.py` & `spright-23.6.24/spright/distribution.py`

 * *Files identical despite different names*

### Comparing `spright-23.6.19/spright/io.py` & `spright-23.6.24/spright/io.py`

 * *Files identical despite different names*

### Comparing `spright-23.6.19/spright/lpf.py` & `spright-23.6.24/spright/lpf.py`

 * *Files identical despite different names*

### Comparing `spright-23.6.19/spright/model.py` & `spright-23.6.24/spright/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,26 +177,29 @@
             lnt[:] = 0
             for j in range(ns):
                 lnt[j] = log(model(densities[j], radii[j], pvp[i], cs, r0, dr, drocky, dwater)).sum()
             maxl = max(lnt)
             lnl[i] = maxl + log(exp(lnt - maxl).mean())
     return lnl
 
-
+@njit
 def invert_cdf(values, cdf, res):
     x = linspace(0, 1.0, res)
     y = zeros(res)
     y[0] = values[0]
     y[-1] = values[-1]
     i, j = 0, 0
     for j in range(res-2):
         while cdf[i] < x[j+1]:
             i += 1
-        a = (x[j+1] - cdf[i-1]) / (cdf[i] - cdf[i-1])
-        y[j+1] = (1-a)*values[i-1] + a*values[i]
+        if i > 0:
+            a = (x[j+1] - cdf[i-1]) / (cdf[i] - cdf[i-1])
+            y[j+1] = (1-a)*values[i-1] + a*values[i]
+        else:
+            y[j+1] = values[0]
     return x, y
 
 
 def create_radius_density_map(pvs: ndarray, r0, dr, drocky, dwater,
                               rlims: tuple[float, float] = (0.5, 6.0), dlims: tuple[float, float] = (0, 12),
                               rres: int = 200, dres: int = 100, components = None) -> (ndarray, ndarray, ndarray):
     radii = linspace(*rlims, num=rres)
```

### Comparing `spright-23.6.19/spright/rdmodel.py` & `spright-23.6.24/spright/rdmodel.py`

 * *Files identical despite different names*

### Comparing `spright-23.6.19/spright/rmestimator.py` & `spright-23.6.24/spright/rmestimator.py`

 * *Files identical despite different names*

### Comparing `spright-23.6.19/spright/rmrelation.py` & `spright-23.6.24/spright/rmrelation.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ----------
         fname
             Radius-density table file.
         """
 
         self.rdm = RadiusDensityModel()
         if fname is None:
-            fname = Path(__file__).parent / 'data' / 'rdmap.fits'
+            fname = Path(__file__).parent / 'data' / 'stpm.fits'
         with pf.open(fname) as f:
             self.rd_posterior = f[0].data.copy()
             self.icdf = f[1].data.copy()
             h0 = f[0].header
             self.densities = h0['CRVAL1'] + arange(h0['NAXIS1']) * h0['CDELT1']
             h1 = f[1].header
             self.radii = h1['CRVAL2'] + arange(h1['NAXIS2']) * h1['CDELT2']
```

### Comparing `spright-23.6.19/spright.egg-info/PKG-INFO` & `spright-23.6.24/spright.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: spright
-Version: 23.6.19
+Version: 23.6.24
 Summary: Bayesian radius-density-mass relation for small planets.
 Author-email: Hannu Parviainen <hpparvi@gmail.com>
-Project-URL: homepage, https://github.com/hpparvi/
+Project-URL: homepage, https://github.com/hpparvi/spright
 Keywords: astronomy,astrophysics,exoplanets
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

