# Comparing `tmp/sam_ml-py-0.5.0.tar.gz` & `tmp/sam_ml-py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_ml-py-0.5.0.tar", last modified: Thu Jun 22 06:54:01 2023, max compression
+gzip compressed data, was "sam_ml-py-0.6.0.tar", last modified: Sat Jun 24 09:47:20 2023, max compression
```

## Comparing `sam_ml-py-0.5.0.tar` & `sam_ml-py-0.6.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.690299 sam_ml-py-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-22 06:54:01.690299 sam_ml-py-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.682299 sam_ml-py-0.5.0/sam_ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.682299 sam_ml-py-0.5.0/sam_ml/config/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/config/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.682299 sam_ml-py-0.5.0/sam_ml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.686299 sam_ml-py-0.5.0/sam_ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/AdaBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/BaggingClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/BernoulliNB.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/ClassifierTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/DecisionTreeClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/ExtraTreesClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/GaussianNB.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/GaussianProcessClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/GradientBoostingMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/KNeighborsClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/LinearDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/LinearSupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/MLPClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/QuadraticDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/SupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/XGBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20573 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/main_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/main_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/main_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.690299 sam_ml-py-0.5.0/sam_ml_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-22 06:54:01.000000 sam_ml-py-0.5.0/sam_ml_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-22 06:54:01.000000 sam_ml-py-0.5.0/sam_ml_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 06:54:01.000000 sam_ml-py-0.5.0/sam_ml_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-22 06:54:01.000000 sam_ml-py-0.5.0/sam_ml_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 06:54:01.000000 sam_ml-py-0.5.0/sam_ml_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 06:54:01.690299 sam_ml-py-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.831864 sam_ml-py-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-24 09:47:20.831864 sam_ml-py-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.823865 sam_ml-py-0.6.0/sam_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.827865 sam_ml-py-0.6.0/sam_ml/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/config/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.827865 sam_ml-py-0.6.0/sam_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/data/synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.831864 sam_ml-py-0.6.0/sam_ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/AdaBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/BaggingClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/BernoulliNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/ClassifierTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/DecisionTreeClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/ExtraTreesClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/GaussianNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/GaussianProcessClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/GradientBoostingMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/KNeighborsClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/LinearDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/LinearSupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/MLPClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/QuadraticDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/SupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/XGBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22099 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/main_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/main_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/main_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/sam_ml/models/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:47:20.831864 sam_ml-py-0.6.0/sam_ml_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-24 09:47:20.000000 sam_ml-py-0.6.0/sam_ml_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-24 09:47:20.000000 sam_ml-py-0.6.0/sam_ml_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 09:47:20.000000 sam_ml-py-0.6.0/sam_ml_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-24 09:47:20.000000 sam_ml-py-0.6.0/sam_ml_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 09:47:20.000000 sam_ml-py-0.6.0/sam_ml_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 09:47:20.831864 sam_ml-py-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-24 09:47:06.000000 sam_ml-py-0.6.0/setup.py
```

### Comparing `sam_ml-py-0.5.0/LICENSE` & `sam_ml-py-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/PKG-INFO` & `sam_ml-py-0.6.0/sam_ml_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sam_ml-py
-Version: 0.5.0
+Name: sam-ml-py
+Version: 0.6.0
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `sam_ml-py-0.5.0/README.md` & `sam_ml-py-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/sam_ml/config/logging.py` & `sam_ml-py-0.6.0/sam_ml/config/logging.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/sam_ml/data/embeddings.py` & `sam_ml-py-0.6.0/sam_ml/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/sam_ml/data/feature_selection.py` & `sam_ml-py-0.6.0/sam_ml/data/feature_selection.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/sam_ml/data/sampling.py` & `sam_ml-py-0.6.0/sam_ml/data/sampling.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/sam_ml/data/scaler.py` & `sam_ml-py-0.6.0/sam_ml/data/scaler.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/sam_ml/data/synthetic_data.py` & `sam_ml-py-0.6.0/sam_ml/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/sam_ml/models/AdaBoostClassifier.py` & `sam_ml-py-0.6.0/sam_ml/models/AdaBoostClassifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,20 +27,22 @@
         """
         model_type = "ABC"
         model = AdaBoostClassifier(
             random_state=random_state,
             **kwargs,
         )
         if type(model.estimator) == RandomForestClassifier:
-            core_estimator = [RandomForestClassifier(max_depth=i, n_estimators=j) for i in range(1,11) for j in (5, 10, 20, 50, 100)]
+            core_estimator = [RandomForestClassifier(max_depth=i, n_estimators=j) for j in  (100, 50, 20, 10, 5) for i in range(1,11)]
+        elif type(model.estimator) == DecisionTreeClassifier or model.estimator is None:
+            core_estimator = [DecisionTreeClassifier(max_depth=i) for i in range(1,11)]
         else:
-            core_estimator= [DecisionTreeClassifier(max_depth=i) for i in range(1,11)]
+            core_estimator = [SVC(probability=True, kernel='linear'), GradientBoostingClassifier(), LogisticRegression()]
         
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "estimator": Categorical("estimator", core_estimator+[SVC(probability=True, kernel='linear'), LogisticRegression(), GradientBoostingClassifier()]),
-            "n_estimators": Integer("n_estimators", (10, 3000), log=True),
-            "learning_rate": Float("learning_rate", (0.005, 2), distribution=Beta(10, 5)),
-            "algorithm": Categorical("algorithm", ["SAMME.R", "SAMME"]),
+            "estimator": Categorical("estimator", core_estimator, default=core_estimator[2]),
+            "n_estimators": Integer("n_estimators", (10, 3000), log=True, default=50),
+            "learning_rate": Float("learning_rate", (0.005, 2), distribution=Beta(10, 5), default=1),
+            "algorithm": Categorical("algorithm", ["SAMME.R", "SAMME"], default="SAMME.R"),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/BaggingClassifier.py` & `sam_ml-py-0.6.0/sam_ml/models/BaggingClassifier.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,22 +35,24 @@
         model_type = "BC"
         model = BaggingClassifier(
             random_state=random_state,
             n_jobs=n_jobs,
             **kwargs,
         )
         if type(model.estimator) == RandomForestClassifier:
-            core_estimator = [RandomForestClassifier(max_depth=i, n_estimators=j) for i in range(1,11) for j in (5, 10, 20, 50, 100)]
-        else:
+            core_estimator = [RandomForestClassifier(max_depth=i, n_estimators=j) for j in (100, 50, 20, 10, 5) for i in range(1,11)]
+        elif type(model.estimator) == DecisionTreeClassifier or model.estimator is None:
             core_estimator = [DecisionTreeClassifier(max_depth=i) for i in range(1,11)]
+        else:
+            core_estimator = [SVC(probability=True, kernel='linear'), GradientBoostingClassifier(), KNeighborsClassifier(), LogisticRegression()]
 
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "estimator": Categorical("estimator", core_estimator+[SVC(probability=True, kernel='linear'), LogisticRegression(), GradientBoostingClassifier(), KNeighborsClassifier()]),
-            "n_estimators": Integer("n_estimators", (3, 3000), distribution=Beta(1, 15)),
-            "max_samples": Float("max_samples", (0.1, 1)),
-            "max_features": Categorical("max_features", [0.5, 1.0, 2, 4]),
+            "estimator": Categorical("estimator", core_estimator, default=core_estimator[3]),
+            "n_estimators": Integer("n_estimators", (3, 3000), distribution=Beta(1, 15), default=10),
+            "max_samples": Float("max_samples", (0.1, 1), default=1),
+            "max_features": Categorical("max_features", [0.5, 0.9, 1.0, 2, 4], default=1.0),
             "bootstrap": Categorical("bootstrap", [True, False], default=True),
             "bootstrap_features": Categorical("bootstrap_features", [True, False], default=False),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/BernoulliNB.py` & `sam_ml-py-0.6.0/sam_ml/models/BernoulliNB.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,11 +18,11 @@
             fit_prior: whether to learn class prior probabilities or not. If false, a uniform prior will be used
         """
         model_type = "BNB"
         model = BernoulliNB(**kwargs,)
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "fit_prior": Categorical("fit_prior", [True, False]),
-            "binarize": Integer("binarize", (0, 10)),
+            "fit_prior": Categorical("fit_prior", [True, False], default=True),
+            "binarize": Integer("binarize", (0, 10), default=0),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/ClassifierTest.py` & `sam_ml-py-0.6.0/sam_ml/models/ClassifierTest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import os
 import sys
 import warnings
+from copy import copy
 from typing import Union
 
 import pandas as pd
 
 # to deactivate pygame promt 
 os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
 
 import pygame
 from pkg_resources import resource_filename
 from sklearn.ensemble import RandomForestClassifier
+from sklearn.linear_model import LogisticRegression
 from tqdm.auto import tqdm
 
 from sam_ml.config import setup_logger
 from sam_ml.data import Embeddings_builder, Sampler, Scaler, Selector
 
 from .AdaBoostClassifier import ABC
 from .BaggingClassifier import BC
@@ -30,32 +32,37 @@
 from .LogisticRegression import LR
 from .main_classifier import Classifier
 from .main_pipeline import Pipeline
 from .MLPClassifier import MLPC
 from .QuadraticDiscriminantAnalysis import QDA
 from .RandomForestClassifier import RFC
 from .SupportVectorClassifier import SVC
+from .XGBoostClassifier import XGBC
 
 logger = setup_logger(__name__)
 
 if not sys.warnoptions:
     warnings.simplefilter("ignore")
     os.environ["PYTHONWARNINGS"] = "ignore" # Also affects subprocesses
 
 
 class CTest:
     """ AutoML class """
 
-    def __init__(self, models: Union[str, list[Classifier]] = "all", vectorizer: Union[str, Embeddings_builder] = None, scaler: Union[str, Scaler] = None, selector: Union[str, Selector] = None, sampler: Union[str, Sampler] = None):
+    def __init__(self, models: Union[str, list[Classifier]] = "search", vectorizer: Union[str, Embeddings_builder] = None, scaler: Union[str, Scaler] = None, selector: Union[str, Selector] = None, sampler: Union[str, Sampler] = None):
         """
         @params:
             models:
-                list of Wrapperclass models from sam_ml library
-                'all': use all Wrapperclass models (18+ models) from sam_ml library
-                'basic': use basic Wrapperclass models (9 models) from sam_ml library (LogisticRegression, MLP Classifier, LinearSVC, DecisionTreeClassifier, RandomForestClassifier, SVC, Gradientboostingmachine, AdaboostClassifier, KNeighborsClassifier)
+
+                - list of Wrapperclass models from this library
+
+                - 'all': use all Wrapperclass models (18+ models)
+
+                - 'basic': use basic Wrapperclass models (8 models) (LogisticRegression, MLP Classifier, LinearSVC, DecisionTreeClassifier, RandomForestClassifier, SVC, Gradientboostingmachine, KNeighborsClassifier)
+
             vectorizer: type of "data.embeddings.Embeddings_builder" or Embeddings_builder class object for automatic string column vectorizing (None for no vectorizing)
             scaler: type of "data.scaler.Scaler" or Scaler class object for scaling the data (None for no scaling)
             selector: type of "data.feature_selection.Selector" or Selector class object for feature selection (None for no selecting)
             sampling: type of "data.sampling.Sampler" or Sampler class object for sampling the train data (None for no sampling)
         """
         self.__models_input = models
 
@@ -131,51 +138,58 @@
         @params:
             kind:
                 "all": use all models
                 "basic": use a simple combination (LogisticRegression, MLP Classifier, LinearSVC, DecisionTreeClassifier, RandomForestClassifier, SVC, Gradientboostingmachine, AdaboostClassifier, KNeighborsClassifier)
         """
         if kind == "all":
             models = [
-                LR(model_name="LogisticRegression (l2 penalty)"),
-                LR(model_name="LogisticRegression (elasticnet penalty)", penalty="elasticnet", solver="saga", l1_ratio=0.5),
+                LR(),
                 QDA(),
                 LDA(),
                 MLPC(),
                 LSVC(),
                 DTC(),
                 RFC(),
-                SVC(model_name="SupportVectorClassifier (rbf-kernel)"),
+                SVC(),
                 GBM(),
                 
                 ABC(model_name="AdaBoostClassifier (DTC based)"),
                 ABC(
                     estimator=RandomForestClassifier(max_depth=5, random_state=42),
                     model_name="AdaBoostClassifier (RFC based)",
                 ),
+                ABC(
+                    estimator=LogisticRegression(),
+                    model_name="AdaBoostClassifier (mixed based)",
+                ),
                 KNC(),
                 ETC(),
                 GNB(),
                 BNB(),
                 GPC(),
                 BC(model_name="BaggingClassifier (DTC based)"),
                 BC(
                     estimator=RandomForestClassifier(max_depth=5, random_state=42),
                     model_name="BaggingClassifier (RFC based)",
                 ),
+                BC(
+                    estimator=LogisticRegression(),
+                    model_name="BaggingClassifier (mixed based)",
+                ),
+                XGBC(),
             ]
         elif kind == "basic":
             models = [
                 LR(),
                 MLPC(),
                 LSVC(),
                 DTC(),
                 RFC(),
-                SVC(model_name="SupportVectorClassifier (rbf-kernel)"),
+                SVC(),
                 GBM(),
-                ABC(model_name="AdaBoostClassifier (DTC based)"),
                 KNC(),
             ]
         else:
             print(f"Cannot find model combination '{kind}' --> using all models")
             models = self.model_combs("all")
 
         return models
@@ -228,15 +242,15 @@
             logger.info("KeyboardInterrupt - output interim result")
             return self.scores
 
     def eval_models_cv(
         self,
         X: pd.DataFrame,
         y: pd.Series,
-        cv_num: int = 10,
+        cv_num: int = 5,
         avg: str = "macro",
         pos_label: Union[int, str] = -1,
         small_data_eval: bool = False,
         secondary_scoring: str = None,
         strength: int = 3,
     ) -> dict[str, dict]:
         """
@@ -296,14 +310,51 @@
                 print(scores)
         else:
             logger.warning("no scores are created -> use 'eval_models()'/'eval_models_cv()' to create scores")
             scores = None
 
         return scores
 
+    def find_best_model_randomCV(
+        self,
+        x_train: pd.DataFrame,
+        y_train: pd.Series,
+        x_test: pd.DataFrame,
+        y_test: pd.Series,
+        n_trails: int = 5,
+        scoring: str = "accuracy",
+        avg: str = "macro",
+        pos_label: Union[int, str] = -1,
+        secondary_scoring: str = None,
+        strength: int = 3,
+        small_data_eval: bool = False,
+        cv_num: int = 3,
+    ) -> dict:
+        for key in tqdm(self.models.keys(), desc="randomCVsearch"):
+            best_hyperparameters, best_score = self.models[key].randomCVsearch(x_train, y_train, n_trails, scoring, avg, pos_label, secondary_scoring, strength, small_data_eval, cv_num, True)
+            logger.info(f"{self.models[key].model_name} - score: {best_score} ({scoring}) - parameters: {best_hyperparameters}")
+            model_best = copy(self.models[key])
+            model_best.set_params(**best_hyperparameters)
+            train_score, train_time = model_best.train(x_train, y_train, console_out=False)
+            scores = model_best.evaluate(x_test, y_test, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength, console_out=False)
+            
+            scores["train_time"] = train_time
+            scores["train_score"] = train_score
+            scores["best_score (rCVs)"] = best_score
+            scores["best_hyperparameters (rCVs)"] = best_hyperparameters
+            self.scores[key] = scores
+        sorted_scores = self.output_scores_as_pd(sort_by=[scoring, "s_score", "train_time"], console_out=False)
+        best_model_type = sorted_scores.iloc[0].name
+        best_model_value = sorted_scores.iloc[0][scoring]
+        best_model_hyperparameters = sorted_scores.iloc[0]["best_hyperparameters (rCVs)"]
+        logger.info(f"best model type {best_model_type} - {scoring}: {best_model_value} - parameters: {best_model_hyperparameters}")
+        self.__finish_sound()
+        return self.scores
+
+
     # def find_best_model(
     #     self,
     #     x_train: pd.DataFrame,
     #     y_train: pd.Series,
     #     x_test: pd.DataFrame,
     #     y_test: pd.Series,
     #     cv_kind: str = "no",
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/DecisionTreeClassifier.py` & `sam_ml-py-0.6.0/sam_ml/models/DecisionTreeClassifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,13 +25,13 @@
         model = DecisionTreeClassifier(
             random_state=random_state,
             **kwargs,
         )
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "criterion": Categorical("criterion", ["gini", "entropy"]),
-            "max_depth": Integer("max_depth", (1, 10)),
-            "min_samples_split": Integer("min_samples_split", (2, 10)),
-            "min_samples_leaf": Integer("min_samples_leaf", (1, 5)),
+            "criterion": Categorical("criterion", ["gini", "entropy"], default="gini"),
+            "max_depth": Integer("max_depth", (1, 10), default=5),
+            "min_samples_split": Integer("min_samples_split", (2, 10), default=2),
+            "min_samples_leaf": Integer("min_samples_leaf", (1, 5), default=1),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/ExtraTreesClassifier.py` & `sam_ml-py-0.6.0/sam_ml/models/ExtraTreesClassifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             n_jobs=n_jobs,
             random_state=random_state,
             **kwargs,
         )
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "n_estimators": Integer("n_estimators", (10, 1000), log=True),
-            "max_depth": Integer("max_depth", (3, 15), distribution=Normal(5, 3)),
-            "min_samples_split": Integer("min_samples_split", (2, 10)),
-            "min_samples_leaf": Integer("min_samples_leaf", (1, 4)),
+            "n_estimators": Integer("n_estimators", (10, 1000), log=True, default=100),
+            "max_depth": Integer("max_depth", (3, 15), distribution=Normal(5, 3), default=5),
+            "min_samples_split": Integer("min_samples_split", (2, 10), default=2),
+            "min_samples_leaf": Integer("min_samples_leaf", (1, 4), default=1),
             "bootstrap": Categorical("bootstrap", [True, False], default=False),
-            "criterion": Categorical("criterion", ["gini", "entropy"]),
+            "criterion": Categorical("criterion", ["gini", "entropy"], default="gini"),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/GaussianNB.py` & `sam_ml-py-0.6.0/sam_ml/models/GaussianNB.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,10 +18,10 @@
             var_smoothing: Portion of the largest variance of all features that is added to variances for calculation stability
         """
         model_type = "GNB"
         model = GaussianNB(**kwargs,)
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "var_smoothing": Float("var_smoothing", (0.00000000001, 1), log=True)
+            "var_smoothing": Float("var_smoothing", (1e-11, 1), log=True, default=1e-9)
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/GaussianProcessClassifier.py` & `sam_ml-py-0.6.0/sam_ml/models/GaussianProcessClassifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,11 +22,11 @@
         model_type = "GPC"
         model = GaussianProcessClassifier(
             n_jobs=n_jobs, random_state=random_state, **kwargs,
         )
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "multi_class": Categorical("multi_class", ["one_vs_rest", "one_vs_one"]),
-            "max_iter_predict": Integer("max_iter_predict", (1, 1000), log=True),
+            "multi_class": Categorical("multi_class", ["one_vs_rest", "one_vs_one"], default="one_vs_rest"),
+            "max_iter_predict": Integer("max_iter_predict", (1, 1000), log=True, default=100),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/GradientBoostingMachine.py` & `sam_ml-py-0.6.0/sam_ml/models/GradientBoostingMachine.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,18 +29,18 @@
             random_state: random_state for model
         """
         model_type = "GBM"
         model = GradientBoostingClassifier(random_state=random_state, **kwargs,)
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "n_estimators": Integer("n_estimators", (20, 1500), log=True),
-            "max_depth": Integer("max_depth", (1, 15), distribution=Normal(4, 4)),
-            "min_samples_split": Integer("min_samples_split", (2, 100), log=True),
-            "min_samples_leaf": Integer("min_samples_leaf", (2, 100), log=True),
-            "max_features": Categorical("max_features", ["auto", "sqrt", "log2"]),
-            "subsample": Float("subsample", (0.7, 1)),
-            "criterion": Categorical("criterion", ["friedman_mse", "mse"]),
-            "loss": Categorical("loss", ["deviance", "exponential"]),
-            "learning_rate": Float("learning_rate", (0.005, 0.1), log=True),
+            "n_estimators": Integer("n_estimators", (20, 1500), log=True, default=100),
+            "max_depth": Integer("max_depth", (1, 15), distribution=Normal(5, 3), default=3),
+            "min_samples_split": Integer("min_samples_split", (2, 100), log=True, default=2),
+            "min_samples_leaf": Integer("min_samples_leaf", (1, 100), log=True, default=1),
+            "max_features": Categorical("max_features", ["auto", "sqrt", "log2"], default="auto"),
+            "subsample": Float("subsample", (0.7, 1), default=1),
+            "criterion": Categorical("criterion", ["friedman_mse", "squared_error"], default="friedman_mse"),
+            "loss": Categorical("loss", ["log_loss", "deviance", "exponential"], default="log_loss"),
+            "learning_rate": Float("learning_rate", (0.005, 0.3), log=True, default=0.1),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/KNeighborsClassifier.py` & `sam_ml-py-0.6.0/sam_ml/models/KNeighborsClassifier.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,13 +22,13 @@
             n_jobs: the number of parallel jobs to run for neighbors search [problem with n_jobs = -1 --> kernel dies]
         """
         model_type = "KNC"
         model = KNeighborsClassifier(**kwargs,)
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "n_neighbors": Integer("n_neighbors", (1, 30)),
-            "p": Integer("p", (1, 5)),
-            "leaf_size": Integer("leaf_size", (1, 50)),
-            "weights": Categorical("weights", ["uniform", "distance"]),
+            "n_neighbors": Integer("n_neighbors", (1, 30), default=5),
+            "p": Integer("p", (1, 5), default=2),
+            "leaf_size": Integer("leaf_size", (1, 50), default=30),
+            "weights": Categorical("weights", ["uniform", "distance"], default="uniform"),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/LinearDiscriminantAnalysis.py` & `sam_ml-py-0.6.0/sam_ml/models/LinearDiscriminantAnalysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,13 +18,13 @@
             shrinkage: shrinkage parameters (does not work with 'svd' solver)
         """
         model_type = "LDA"
         model = LinearDiscriminantAnalysis(**kwargs)
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "solver": Categorical("solver", ["lsqr", "eigen", "svd"], weights=[0.475, 0.475, 0.05]),
-            "shrinkage": Float("shrinkage", (0, 1)),
+            "solver": Categorical("solver", ["lsqr", "eigen", "svd"], weights=[0.475, 0.475, 0.05], default="svd"),
+            "shrinkage": Float("shrinkage", (0, 1), default=0),
             })
         shrinkage_cond = InCondition(grid["shrinkage"], grid["solver"], ["lsqr", "eigen"])
         grid.add_condition(shrinkage_cond)
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/LinearSupportVectorClassifier.py` & `sam_ml-py-0.6.0/sam_ml/models/LinearSupportVectorClassifier.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from ConfigSpace import Categorical, ConfigurationSpace, Float
+from ConfigSpace import (Categorical, ConfigurationSpace, Float,
+                         ForbiddenAndConjunction, ForbiddenEqualsClause)
 from sklearn.svm import LinearSVC
 
 from .main_classifier import Classifier
 
 
 class LSVC(Classifier):
     """ LinearSupportVectorClassifier Wrapper class """
@@ -26,12 +27,17 @@
         model = LinearSVC(
             random_state=random_state,
             **kwargs,
         )
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "penalty": Categorical("penalty", ["l1", "l2"]),
-            "dual": Categorical("dual", [True, False]),
-            "C": Float("C", (0.00001, 1000000), log=True),
+            "penalty": Categorical("penalty", ["l1", "l2"], default="l2"),
+            "dual": Categorical("dual", [True, False], default=True),
+            "C": Float("C", (0.1, 1000), log=True, default=1),
             })
+        penalty_dual = ForbiddenAndConjunction(
+            ForbiddenEqualsClause(grid["dual"], True),
+            ForbiddenEqualsClause(grid["penalty"], "l1"),
+        )
+        grid.add_forbidden_clause(penalty_dual)
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/LogisticRegression.py` & `sam_ml-py-0.6.0/sam_ml/models/LogisticRegression.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,17 @@
             random_state=random_state,
             **kwargs,
         )
         grid = ConfigurationSpace(
             seed=42,
             space={
             "solver": Categorical("solver", ["newton-cg", "lbfgs", "liblinear", "sag", "saga"], weights=[0.15, 0.15, 0.15, 0.15, 0.4], default="lbfgs"),
-            "penalty": Categorical("penalty", ["l2", "elasticnet"]),
-            "C": Float("C", (0.01, 100), log=True),
-            "l1_ratio": Float("l1_ratio", (0.01, 1)),
+            "penalty": Categorical("penalty", ["l2", "elasticnet"], default="l2"),
+            "C": Float("C", (0.01, 100), log=True, default=1),
+            "l1_ratio": Float("l1_ratio", (0.01, 1), default=0.1),
             })
         solver_and_penalty = ForbiddenAndConjunction(
             ForbiddenEqualsClause(grid["penalty"], "elasticnet"),
             ForbiddenInClause(grid["solver"], ["newton-cg", "lbfgs", "liblinear", "sag"]),
         )
         l1_ratio_cond = EqualsCondition(grid["l1_ratio"], grid["penalty"], "elasticnet")
         grid.add_forbidden_clause(solver_and_penalty)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/MLPClassifier.py` & `sam_ml-py-0.6.0/sam_ml/models/MLPClassifier.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,14 @@
         model = MLPClassifier(
             random_state=random_state,
             **kwargs,
         )
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "hidden_layer_sizes": Categorical("hidden_layer_sizes", ((10, 30, 10), (20,), (10,), (100,), (50,50,50), (50,100,50))),
-            "activation": Categorical("activation", ["tanh", "relu", "logistic"]),
-            "solver": Categorical("solver", ["sgd", "adam"]),
-            "alpha": Float("alpha", (0.0001, 0.05), log=True),
-            "learning_rate": Categorical("learning_rate", ["constant", "adaptive"]),
+            "hidden_layer_sizes": Categorical("hidden_layer_sizes", ((10, 30, 10), (20,), (10,), (100,), (50,50,50), (50,100,50)), default=(100, )),
+            "activation": Categorical("activation", ["tanh", "relu", "logistic"], default="relu"),
+            "solver": Categorical("solver", ["sgd", "adam"], default="adam"),
+            "alpha": Float("alpha", (0.0001, 0.05), log=True, default=0.0001),
+            "learning_rate": Categorical("learning_rate", ["constant", "adaptive"], default="constant"),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/QuadraticDiscriminantAnalysis.py` & `sam_ml-py-0.6.0/sam_ml/models/QuadraticDiscriminantAnalysis.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,10 +21,10 @@
             reg_param: regularizes the per-class covariance estimates by transforming
         """
         model_type = "QDA"
         model = QuadraticDiscriminantAnalysis(**kwargs)
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "reg_param": Float("reg_param", (0, 1)),
+            "reg_param": Float("reg_param", (0, 1), default=0),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/RandomForestClassifier.py` & `sam_ml-py-0.6.0/sam_ml/models/RandomForestClassifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             n_jobs=n_jobs,
             random_state=random_state,
             **kwargs,
         )
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "n_estimators": Integer("n_estimators", (10, 1000), log=True),
-            "max_depth": Integer("max_depth", (3, 15), distribution=Normal(5, 3)),
-            "min_samples_split": Integer("min_samples_split", (2, 10)),
-            "min_samples_leaf": Integer("min_samples_leaf", (1, 4)),
+            "n_estimators": Integer("n_estimators", (10, 1000), log=True, default=100),
+            "max_depth": Integer("max_depth", (3, 15), distribution=Normal(5, 3), default=5),
+            "min_samples_split": Integer("min_samples_split", (2, 10), default=2),
+            "min_samples_leaf": Integer("min_samples_leaf", (1, 4), default=1),
             "bootstrap": Categorical("bootstrap", [True, False], default=True),
-            "criterion": Categorical("criterion", ["gini", "entropy"]),
+            "criterion": Categorical("criterion", ["gini", "entropy"], default="gini"),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/SupportVectorClassifier.py` & `sam_ml-py-0.6.0/sam_ml/models/SupportVectorClassifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,18 +32,18 @@
             kernel=kernel,
             random_state=random_state,
             **kwargs,
         )
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "kernel": Categorical("kernel", ["rbf", "poly", "sigmoid"]),
-            "gamma": Float("gamma", (0.0001, 1), log=True),
-            "C": Float("C", (0.1, 1000), log=True),
-            "probability": Categorical("probability", [True, False]),
+            "kernel": Categorical("kernel", ["rbf", "poly", "sigmoid"], default="rbf"),
+            "gamma": Float("gamma", (0.0001, 1), log=True, default=0.001),
+            "C": Float("C", (0.1, 1000), log=True, default=1),
+            "probability": Categorical("probability", [True, False], default=False),
             })
         super().__init__(model, model_name, model_type, grid)
 
     def feature_importance(self):
         if self.model.kernel == "linear":
             super().feature_importance()
         else:
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/XGBoostClassifier.py` & `sam_ml-py-0.6.0/sam_ml/models/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-from ConfigSpace import ConfigurationSpace, Float, Integer, Normal
-from xgboost import XGBClassifier
-
+from .AdaBoostClassifier import ABC
+from .BaggingClassifier import BC
+from .BernoulliNB import BNB
+from .ClassifierTest import CTest
+from .DecisionTreeClassifier import DTC
+from .ExtraTreesClassifier import ETC
+from .GaussianNB import GNB
+from .GaussianProcessClassifier import GPC
+from .GradientBoostingMachine import GBM
+from .KNeighborsClassifier import KNC
+from .LinearDiscriminantAnalysis import LDA
+from .LinearSupportVectorClassifier import LSVC
+from .LogisticRegression import LR
 from .main_classifier import Classifier
+from .main_model import Model
+from .main_pipeline import Pipeline
+from .MLPClassifier import MLPC
+from .QuadraticDiscriminantAnalysis import QDA
+from .RandomForestClassifier import RFC
+from .SupportVectorClassifier import SVC
+from .XGBoostClassifier import XGBC
 
-
-class XGBC(Classifier):
-    """ SupportVectorClassifier Wrapper class """
-
-    def __init__(
-        self,
-        model_name: str = "XGBClassifier",
-        n_jobs: str = -1,
-        random_state: int = 42,
-        **kwargs,
-    ):
-        """
-        @param (important one):
-            random_state: random_state for model
-            n_jobs: how many cores shall be used (-1 means all)
-        """
-        model_type = "XGBC"
-        model = XGBClassifier(
-            n_jobs=n_jobs,
-            random_state=random_state,
-            **kwargs,
-        )
-        grid = ConfigurationSpace(
-            seed=42,
-            space={
-            "max_depth": Integer("max_depth", (3, 10)),
-            "gamma": Float('gamma', (1, 9)),
-            'reg_alpha' : Integer('reg_alpha', (40, 180)),
-            'reg_lambda' : Float('reg_lambda', (0, 1)),
-            'colsample_bytree' : Float('colsample_bytree', (0.5, 1)),
-            'min_child_weight' : Integer('min_child_weight', (0, 10)),
-            'n_estimators': Integer("n_estimators", bounds=(50, 750), distribution=Normal(150, 100)),
-            "learning_rate": Float("learning_rate", bounds=(0.001, 0.30), log=True),
-            })
-        super().__init__(model, model_name, model_type, grid)
-
-    def feature_importance(self):
-        super().feature_importance()
+__all__ = {
+    "model parent class": "Model",
+    "classifier parent class": "Classifier",
+    "pipeline class": "Pipeline",
+    "AutoML class": "CTest",
+    "RandomForestClassifier": "RFC",
+    "LogisticRegression": "LR",
+    "DecisionTreeClassifier": "DCT",
+    "SupportVectorClassifier": "SVC",
+    "MLP Classifier": "MLPC",
+    "GradientBoostingMachine": "GBM",
+    "AdaBoostClassifier": "ABC",
+    "KNeighborsClassifier": "KNC",
+    "ExtraTreesClassifier": "ETC",
+    "GaussianNaiveBayes": "GNB",
+    "BernoulliNaiveBayes": "BNB",
+    "GaussianProcessClassifier": "GPC",
+    "QuadraticDiscriminantAnalysis": "QDA",
+    "LinearDiscriminantAnalysis": "LDA",
+    "BaggingClassifier": "BC",
+    "LinearSupportVectorClassifier": "LSVC",
+    "XGBoostClassifier": "XGBC",
+}
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/main_classifier.py` & `sam_ml-py-0.6.0/sam_ml/models/main_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,39 @@
     def grid(self):
         """
         @return:
             hyperparameter tuning grid of the model
         """
         return self._grid
     
-    def get_random_params(self):
+    def get_random_config(self):
         """
         @return;
             set of random parameter from grid
         """
         return dict(self.grid.sample_configuration(1))
+    
+    def get_random_configs(self, n_trails: int) -> list:
+        """
+        @return;
+            n_trails elements in list with sets of random parameterd from grid
+
+        NOTE: filter out duplicates -> could be less than n_trails
+        """
+        if n_trails<1:
+            raise ValueError(f"n_trails has to be greater 0, but {n_trails}<1")
+        
+        configs = [self._grid.get_default_configuration()]
+        if n_trails == 2:
+            configs += [self._grid.sample_configuration(n_trails-1)]
+        else:
+            configs += self._grid.sample_configuration(n_trails-1)
+        # remove duplicates
+        configs = list(dict.fromkeys(configs))
+        return configs
 
     def replace_grid(self, new_grid: ConfigurationSpace):
         """
         function to replace self.grid 
 
         e.g.:
             ConfigurationSpace(
@@ -199,16 +218,16 @@
         score = pd_scores["average"]
         self.cv_scores = {
             "accuracy": score[list(score.keys())[6]],
             "precision": score[list(score.keys())[2]],
             "recall": score[list(score.keys())[4]],
             "s_score": score[list(score.keys())[8]],
             "l_score": score[list(score.keys())[10]],
-            "avg train score": score[list(score.keys())[7]],
-            "avg train time": str(timedelta(seconds = round(score[list(score.keys())[0]]))),
+            "train_score": score[list(score.keys())[7]],
+            "train_time": str(timedelta(seconds = round(score[list(score.keys())[0]]))),
         }
 
         logger.debug(f"cross validation {self.model_name} - finished")
 
         if console_out:
             print()
             print(pd_scores)
@@ -275,16 +294,16 @@
 
         self.cv_scores = {
             "accuracy": accuracy,
             "precision": precision,
             "recall": recall,
             "s_score": s_score,
             "l_score": l_score,
-            "avg train score": avg_train_score,
-            "avg train time": avg_train_time,
+            "train_score": avg_train_score,
+            "train_time": avg_train_time,
         }
 
         logger.debug(f"cross validation {self.model_name} - finished")
 
         if console_out:
             print()
             print("classification report:")
@@ -381,36 +400,53 @@
     #     print(f"Incumbent cost: {incumbent_cost}")
 
     def randomCVsearch(
         self,
         x_train: pd.DataFrame,
         y_train: pd.Series,
         n_trails: int = 10,
-        cv_num: int = 5,
         scoring: str = "accuracy",
         avg: str = "macro",
         pos_label: Union[int, str] = -1,
         secondary_scoring: str = None,
         strength: int = 3,
-    ):
+        small_data_eval: bool = False,
+        cv_num: int = 5,
+        leave_loadbar: bool = True,
+    ) -> tuple[dict, float]:
         results = []
-        configs = self._grid.sample_configuration(n_trails)
-        # remove duplicates
-        configs = list(dict.fromkeys(configs))
-
-        for config in tqdm(configs, desc="randomCVsearch"):
-            model = copy(self)
-            model.set_params(**config)
-            score = model.cross_validation(x_train, y_train, cv_num=cv_num, console_out=False, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength)
-            config_dict = dict(config)
-            config_dict[scoring] = score[scoring]
-            results.append(config_dict)
+        configs = self.get_random_configs(n_trails)
+        at_least_one_run: bool = False
+        try:
+            for config in tqdm(configs, desc=f"randomCVsearch ({self.model_name})", leave=leave_loadbar):
+                model = copy(self)
+                model.set_params(**config)
+                if small_data_eval:
+                    score = model.cross_validation_small_data(x_train, y_train, console_out=False, leave_loadbar=False, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength)
+                else:
+                    score = model.cross_validation(x_train, y_train, cv_num=cv_num, console_out=False, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength)
+                config_dict = dict(config)
+                config_dict[scoring] = score[scoring]
+                results.append(config_dict)
+                at_least_one_run = True
+        except KeyboardInterrupt:
+            logger.info("KeyboardInterrupt - output interim result")
+            if not at_least_one_run:
+                return {}, -1
+            
+
+        self.rCVsearch_results = pd.DataFrame(results, dtype=object).sort_values(by=scoring, ascending=False)
+
+        # for-loop to keep dtypes of columns
+        best_hyperparameters = {} 
+        for col in self.rCVsearch_results.columns:
+            value = self.rCVsearch_results[col].iloc[0]
+            if str(value) != "nan":
+                best_hyperparameters[col] = value
 
-        self.rCVsearch_results = pd.DataFrame(results).sort_values(by=scoring, ascending=False)
-        best_hyperparameters = dict(self.rCVsearch_results.iloc[0])
         best_score = best_hyperparameters[scoring]
         best_hyperparameters.pop(scoring)
         
         return best_hyperparameters, best_score
 
     # def gridsearch(
     #     self,
```

### Comparing `sam_ml-py-0.5.0/sam_ml/models/main_model.py` & `sam_ml-py-0.6.0/sam_ml/models/main_model.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/sam_ml/models/main_pipeline.py` & `sam_ml-py-0.6.0/sam_ml/models/main_pipeline.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/sam_ml/models/scorer.py` & `sam_ml-py-0.6.0/sam_ml/models/scorer.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/sam_ml_py.egg-info/PKG-INFO` & `sam_ml-py-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sam-ml-py
-Version: 0.5.0
+Name: sam_ml-py
+Version: 0.6.0
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `sam_ml-py-0.5.0/sam_ml_py.egg-info/SOURCES.txt` & `sam_ml-py-0.6.0/sam_ml_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.5.0/setup.py` & `sam_ml-py-0.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="sam_ml-py",
-    version="0.5.0",
+    version="0.6.0",
     description="a library for ML programing created by Samuel Brinkmann",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     packages=find_packages(),
     package_data={},
     scripts=[],
```

