# Comparing `tmp/constrainedlr-0.1.0.tar.gz` & `tmp/constrainedlr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constrainedlr-0.1.0.tar", last modified: Sun May 21 15:35:18 2023, max compression
+gzip compressed data, was "constrainedlr-0.1.1.tar", last modified: Sat Jun 24 13:30:34 2023, max compression
```

## Comparing `constrainedlr-0.1.0.tar` & `constrainedlr-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:35:18.743839 constrainedlr-0.1.0/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 constrainedlr-0.1.0/LICENCE
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2165 2023-05-21 15:35:18.738841 constrainedlr-0.1.0/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1209 2023-05-21 15:22:40.000000 constrainedlr-0.1.0/README.md
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1304 2023-05-21 15:34:06.000000 constrainedlr-0.1.0/pyproject.toml
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-21 15:35:18.745840 constrainedlr-0.1.0/setup.cfg
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:35:18.276847 constrainedlr-0.1.0/src/
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:35:18.467857 constrainedlr-0.1.0/src/constrainedlr/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       61 2023-05-21 15:30:34.000000 constrainedlr-0.1.0/src/constrainedlr/__init__.py
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     4246 2023-05-21 15:32:15.000000 constrainedlr-0.1.0/src/constrainedlr/model.py
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      774 2023-05-21 15:31:21.000000 constrainedlr-0.1.0/src/constrainedlr/validation.py
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:35:18.668841 constrainedlr-0.1.0/src/constrainedlr.egg-info/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2165 2023-05-21 15:35:18.000000 constrainedlr-0.1.0/src/constrainedlr.egg-info/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      343 2023-05-21 15:35:18.000000 constrainedlr-0.1.0/src/constrainedlr.egg-info/SOURCES.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-21 15:35:18.000000 constrainedlr-0.1.0/src/constrainedlr.egg-info/dependency_links.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       48 2023-05-21 15:35:18.000000 constrainedlr-0.1.0/src/constrainedlr.egg-info/requires.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       14 2023-05-21 15:35:18.000000 constrainedlr-0.1.0/src/constrainedlr.egg-info/top_level.txt
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-21 15:35:18.701839 constrainedlr-0.1.0/tests/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3589 2023-05-21 15:22:05.000000 constrainedlr-0.1.0/tests/test_fit.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:30:34.426851 constrainedlr-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2023-06-21 18:38:31.000000 constrainedlr-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0     2610 2023-06-24 13:30:34.424829 constrainedlr-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1598 2023-06-21 18:38:31.000000 constrainedlr-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1324 2023-06-24 13:28:35.000000 constrainedlr-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:30:34.426851 constrainedlr-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 13:30:34.284833 constrainedlr-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 13:30:34.332887 constrainedlr-0.1.1/src/constrainedlr/
+-rw-rw-rw-   0        0        0       61 2023-06-21 18:38:31.000000 constrainedlr-0.1.1/src/constrainedlr/__init__.py
+-rw-rw-rw-   0        0        0     7790 2023-06-24 13:24:48.000000 constrainedlr-0.1.1/src/constrainedlr/model.py
+-rw-rw-rw-   0        0        0     2409 2023-06-23 17:34:14.000000 constrainedlr-0.1.1/src/constrainedlr/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:30:34.410829 constrainedlr-0.1.1/src/constrainedlr.egg-info/
+-rw-rw-rw-   0        0        0     2610 2023-06-24 13:30:34.000000 constrainedlr-0.1.1/src/constrainedlr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-24 13:30:34.000000 constrainedlr-0.1.1/src/constrainedlr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:30:34.000000 constrainedlr-0.1.1/src/constrainedlr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-24 13:30:34.000000 constrainedlr-0.1.1/src/constrainedlr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-24 13:30:34.000000 constrainedlr-0.1.1/src/constrainedlr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 13:30:34.420833 constrainedlr-0.1.1/tests/
+-rw-rw-rw-   0        0        0     4887 2023-06-23 17:34:14.000000 constrainedlr-0.1.1/tests/test_fit.py
```

### Comparing `constrainedlr-0.1.0/LICENCE` & `constrainedlr-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `constrainedlr-0.1.0/pyproject.toml` & `constrainedlr-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'constrainedlr'
-version = '0.1.0'
+version = '0.1.1'
 description = 'Constrained Linear Regression with sklearn-compatible API'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
 dependencies = [
   "numpy>=1.18.0",
   "scikit-learn>=1.2.2",
   "cvxopt>=1.3.1",
+  "pandas>=1.2.0",
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
```

### Comparing `constrainedlr-0.1.0/tests/test_fit.py` & `constrainedlr-0.1.1/tests/test_fit.py`

 * *Files 21% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # Perform multiple tests since signs are produced randomly
     np.random.seed(0)
     for _ in range(10):
         signs = np.random.choice([-1, 1], size=X.shape[1])
         features_sign_constraints = dict(zip(list(range(X.shape[1])), signs))
         clr.fit(X, y, coefficients_sign_constraints=features_sign_constraints)
 
-        assert np.alltrue(np.sign(clr.coef_) == signs)
+        assert np.all(np.sign(clr.coef_) == signs)
 
 
 def test_intercept_sign():
     clr = ConstrainedLinearRegression(fit_intercept=True)
     clr.fit(X, y, intercept_sign_constraint=1)
     assert clr.intercept_ > 0
 
@@ -107,7 +107,37 @@
         clr.fit(X, y, sample_weight=sample_weight)
 
         lr = LinearRegression()
         lr.fit(X, y, sample_weight=sample_weight)
 
         assert np.allclose(lr.intercept_, clr.intercept_, atol=atol)
         assert np.allclose(lr.coef_, clr.coef_, atol=atol)
+
+
+def test_coefficients_range_constraints():
+    clr = ConstrainedLinearRegression(fit_intercept=True)
+
+    # Perform multiple tests since bounds are produced randomly
+    np.random.seed(0)
+    for _ in range(50):
+        n_contraints = np.random.randint(0, X.shape[1])
+
+        # Add range constraints in a random set of features
+        coefficients_range_constraints = {}
+        for _ in range(n_contraints):
+            feature = np.random.randint(0, X.shape[1])
+
+            # Add either lower, or upper, or both contraints
+            feature_contraints = {}
+            if np.random.random() > 0.5:
+                feature_contraints.update({"upper": np.random.normal(100, 20)})
+            if np.random.random() > 0.5:
+                feature_contraints.update({"lower": np.random.normal(-100, 20)})
+            coefficients_range_constraints.update({feature: feature_contraints})
+
+        clr.fit(X, y, coefficients_range_constraints=coefficients_range_constraints)
+
+        for feature, contraints in coefficients_range_constraints.items():
+            if "upper" in contraints:
+                assert clr.coef_[feature] <= contraints["upper"] + atol
+            if "lower" in contraints:
+                assert clr.coef_[feature] >= contraints["lower"] - atol
```

