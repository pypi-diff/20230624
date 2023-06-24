# Comparing `tmp/constrainedlr-0.1.1.tar.gz` & `tmp/constrainedlr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constrainedlr-0.1.1.tar", last modified: Sat Jun 24 13:30:34 2023, max compression
+gzip compressed data, was "constrainedlr-0.1.2.tar", last modified: Sat Jun 24 14:16:17 2023, max compression
```

## Comparing `constrainedlr-0.1.1.tar` & `constrainedlr-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 13:30:34.426851 constrainedlr-0.1.1/
--rw-rw-rw-   0        0        0     1089 2023-06-21 18:38:31.000000 constrainedlr-0.1.1/LICENCE
--rw-rw-rw-   0        0        0     2610 2023-06-24 13:30:34.424829 constrainedlr-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1598 2023-06-21 18:38:31.000000 constrainedlr-0.1.1/README.md
--rw-rw-rw-   0        0        0     1324 2023-06-24 13:28:35.000000 constrainedlr-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 13:30:34.426851 constrainedlr-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-24 13:30:34.284833 constrainedlr-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-24 13:30:34.332887 constrainedlr-0.1.1/src/constrainedlr/
--rw-rw-rw-   0        0        0       61 2023-06-21 18:38:31.000000 constrainedlr-0.1.1/src/constrainedlr/__init__.py
--rw-rw-rw-   0        0        0     7790 2023-06-24 13:24:48.000000 constrainedlr-0.1.1/src/constrainedlr/model.py
--rw-rw-rw-   0        0        0     2409 2023-06-23 17:34:14.000000 constrainedlr-0.1.1/src/constrainedlr/validation.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:30:34.410829 constrainedlr-0.1.1/src/constrainedlr.egg-info/
--rw-rw-rw-   0        0        0     2610 2023-06-24 13:30:34.000000 constrainedlr-0.1.1/src/constrainedlr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-06-24 13:30:34.000000 constrainedlr-0.1.1/src/constrainedlr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 13:30:34.000000 constrainedlr-0.1.1/src/constrainedlr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-24 13:30:34.000000 constrainedlr-0.1.1/src/constrainedlr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-24 13:30:34.000000 constrainedlr-0.1.1/src/constrainedlr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-24 13:30:34.420833 constrainedlr-0.1.1/tests/
--rw-rw-rw-   0        0        0     4887 2023-06-23 17:34:14.000000 constrainedlr-0.1.1/tests/test_fit.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:16:17.334225 constrainedlr-0.1.2/
+-rw-rw-rw-   0        0        0     1089 2023-06-21 18:38:31.000000 constrainedlr-0.1.2/LICENCE
+-rw-rw-rw-   0        0        0     2610 2023-06-24 14:16:17.333225 constrainedlr-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1598 2023-06-21 18:38:31.000000 constrainedlr-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1324 2023-06-24 14:14:38.000000 constrainedlr-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 14:16:17.335236 constrainedlr-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 14:16:17.212226 constrainedlr-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 14:16:17.247226 constrainedlr-0.1.2/src/constrainedlr/
+-rw-rw-rw-   0        0        0       61 2023-06-21 18:38:31.000000 constrainedlr-0.1.2/src/constrainedlr/__init__.py
+-rw-rw-rw-   0        0        0     7671 2023-06-24 13:55:44.000000 constrainedlr-0.1.2/src/constrainedlr/model.py
+-rw-rw-rw-   0        0        0     2727 2023-06-24 13:57:55.000000 constrainedlr-0.1.2/src/constrainedlr/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:16:17.321245 constrainedlr-0.1.2/src/constrainedlr.egg-info/
+-rw-rw-rw-   0        0        0     2610 2023-06-24 14:16:17.000000 constrainedlr-0.1.2/src/constrainedlr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-24 14:16:17.000000 constrainedlr-0.1.2/src/constrainedlr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 14:16:17.000000 constrainedlr-0.1.2/src/constrainedlr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-24 14:16:17.000000 constrainedlr-0.1.2/src/constrainedlr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-24 14:16:17.000000 constrainedlr-0.1.2/src/constrainedlr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 14:16:17.329247 constrainedlr-0.1.2/tests/
+-rw-rw-rw-   0        0        0     4887 2023-06-24 13:53:15.000000 constrainedlr-0.1.2/tests/test_fit.py
```

### Comparing `constrainedlr-0.1.1/LICENCE` & `constrainedlr-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `constrainedlr-0.1.1/PKG-INFO` & `constrainedlr-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.1 Summary: Constrained
+Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.2 Summary: Constrained
 Linear Regression with sklearn-compatible API Author-email: Theodore Tsitsimis
 tsitsimis@gmail.com> Project-URL: Homepage, https://github.com/tsitsimis/
 constrainedlr Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `constrainedlr-0.1.1/README.md` & `constrainedlr-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `constrainedlr-0.1.1/pyproject.toml` & `constrainedlr-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'constrainedlr'
-version = '0.1.1'
+version = '0.1.2'
 description = 'Constrained Linear Regression with sklearn-compatible API'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
```

### Comparing `constrainedlr-0.1.1/src/constrainedlr/model.py` & `constrainedlr-0.1.2/src/constrainedlr/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 alpha must be a non-negative float i.e. in [0, inf).
 
         Attributes:
             coef_:
                 Weight vector of shape (n_features,).
 
             intercept_:
-                Independent/constant term in regressin model. Set to None if fit_intercept = False.
+                Independent/constant term in regression model. Set to None if fit_intercept = False.
         """
         self.fit_intercept = fit_intercept
         self.coef_ = None
         self.intercept_ = None
         self.alpha = alpha
 
     def fit(
@@ -111,27 +111,25 @@
         # Quadratic program
         P = X.T.dot(W).dot(X) + self.alpha * np.eye(dim)
         P = matrix(P)
         q = (-y.T.dot(W).dot(X)).T
         q = matrix(q)
 
         G, h = None, None
-        if len(coefficients_sign_constraints) > 0:
-            features_sign_constraints_full = {feature: 0 for feature in range(n_features)}
-            features_sign_constraints_full.update(coefficients_sign_constraints)
-            diag_values = list(features_sign_constraints_full.values())
-            if self.fit_intercept:
-                diag_values.append(intercept_sign_constraint)
-            G = -1.0 * np.diag(
-                diag_values
-            )  # Negate since cvxopt by convention accepts inequalities of the form Gx <= h
-            G = matrix(G)
-            h = np.zeros(dim)
-            h = matrix(h)
-        elif len(coefficients_range_constraints) > 0:
+        features_sign_constraints_full = {feature: 0 for feature in range(n_features)}
+        features_sign_constraints_full.update(coefficients_sign_constraints)
+        diag_values = list(features_sign_constraints_full.values())
+        if self.fit_intercept:
+            diag_values.append(intercept_sign_constraint)
+        G = -1.0 * np.diag(diag_values)  # Negate since cvxopt by convention accepts inequalities of the form Gx <= h
+        G = matrix(G)
+        h = np.zeros(dim)
+        h = matrix(h)
+
+        if len(coefficients_range_constraints) > 0:
             coefficients_upper_bound_constraints = {
                 k: v for k, v in coefficients_range_constraints.items() if "upper" in v
             }
             G_upper = np.zeros((len(coefficients_upper_bound_constraints), dim))
             for i, feature in enumerate(coefficients_upper_bound_constraints.keys()):
                 G_upper[i, feature] = 1
             h_upper = np.array([v["upper"] for k, v in coefficients_upper_bound_constraints.items()])
```

### Comparing `constrainedlr-0.1.1/src/constrainedlr/validation.py` & `constrainedlr-0.1.2/src/constrainedlr/validation.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,20 @@
                 "Keys of coefficients_sign_constraints must be integers within the interval [0, X.shape[1])"
             )
         if (min(coef_indices) < 0) or (max(coef_indices) >= X.shape[1]):
             raise ValueError(
                 "Keys of coefficients_sign_constraints must be integers within the interval [0, X.shape[1])"
             )
 
+        if len(set(coefficients_sign_constraints.values()) - {-1, 0, 1}) > 0:
+            raise ValueError(
+                "Values of coefficients_sign_constraints must be 0, -1, or 1, for no sign constraint, "
+                "negative sign constraint, or positive sign constraint respectively"
+            )
+
 
 def validate_coefficients_range_constraints(coefficients_range_constraints: dict, X) -> None:
     if type(coefficients_range_constraints) != dict:
         raise ValueError("coefficients_range_constraints must be of type dict")
 
     if len(coefficients_range_constraints) > 0:
         coef_indices = list(coefficients_range_constraints.keys())
```

### Comparing `constrainedlr-0.1.1/src/constrainedlr.egg-info/PKG-INFO` & `constrainedlr-0.1.2/src/constrainedlr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.1 Summary: Constrained
+Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.2 Summary: Constrained
 Linear Regression with sklearn-compatible API Author-email: Theodore Tsitsimis
 tsitsimis@gmail.com> Project-URL: Homepage, https://github.com/tsitsimis/
 constrainedlr Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `constrainedlr-0.1.1/tests/test_fit.py` & `constrainedlr-0.1.2/tests/test_fit.py`

 * *Files identical despite different names*

