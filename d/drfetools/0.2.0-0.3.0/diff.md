# Comparing `tmp/dRFEtools-0.2.0.tar.gz` & `tmp/drfetools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dRFEtools-0.2.0.tar", max compression
+gzip compressed data, was "drfetools-0.3.0.tar", max compression
```

## Comparing `dRFEtools-0.2.0.tar` & `drfetools-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,10 @@
--rw-r--r--   0        0        0    35149 2021-09-02 20:40:08.361607 dRFEtools-0.2.0/LICENSE
--rw-r--r--   0        0        0    21032 2021-10-28 17:27:02.400181 dRFEtools-0.2.0/README.md
--rw-r--r--   0        0        0       25 2021-09-09 01:19:06.737008 dRFEtools-0.2.0/dRFEtools/__init__.py
--rwxr-xr-x   0        0        0     9965 2021-12-30 14:12:43.421643 dRFEtools-0.2.0/dRFEtools/dRFEtools.py
--rw-r--r--   0        0        0     7758 2021-11-19 18:28:17.426641 dRFEtools-0.2.0/dRFEtools/dev_scoring.py
--rw-r--r--   0        0        0     5469 2022-02-17 23:26:14.004583 dRFEtools-0.2.0/dRFEtools/linear_models_rfe.py
--rw-r--r--   0        0        0     7627 2022-06-28 15:33:23.803477 dRFEtools-0.2.0/dRFEtools/lowess_redundant.py
--rw-r--r--   0        0        0     7251 2021-11-19 18:26:44.180058 dRFEtools-0.2.0/dRFEtools/random_forest.py
--rw-r--r--   0        0        0     1605 2021-09-30 19:29:32.228063 dRFEtools-0.2.0/dRFEtools/rank_function.py
--rw-r--r--   0        0        0     2874 2022-02-17 23:26:30.671346 dRFEtools-0.2.0/dRFEtools/svm_models.py
--rw-r--r--   0        0        0      940 2022-07-22 13:24:07.251148 dRFEtools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    22815 2022-07-22 13:25:11.844944 dRFEtools-0.2.0/setup.py
--rw-r--r--   0        0        0    22154 2022-07-22 13:25:11.847184 dRFEtools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-09-02 20:40:08.000000 drfetools-0.3.0/LICENSE
+-rw-r--r--   0        0        0    18838 2023-06-21 20:58:15.000000 drfetools-0.3.0/README.md
+-rw-r--r--   0        0        0       25 2021-09-09 01:19:06.000000 drfetools-0.3.0/dRFEtools/__init__.py
+-rwxr-xr-x   0        0        0     9851 2023-06-21 20:56:15.000000 drfetools-0.3.0/dRFEtools/dRFEtools.py
+-rw-r--r--   0        0        0     8251 2023-06-21 20:40:36.000000 drfetools-0.3.0/dRFEtools/dev_scoring.py
+-rw-r--r--   0        0        0     7643 2023-06-21 20:55:18.000000 drfetools-0.3.0/dRFEtools/lowess_redundant.py
+-rw-r--r--   0        0        0     7306 2023-06-21 20:40:54.000000 drfetools-0.3.0/dRFEtools/random_forest.py
+-rw-r--r--   0        0        0     1605 2021-09-30 19:29:32.000000 drfetools-0.3.0/dRFEtools/rank_function.py
+-rw-r--r--   0        0        0      950 2023-06-23 10:37:24.000000 drfetools-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    20021 1970-01-01 00:00:00.000000 drfetools-0.3.0/PKG-INFO
```

### Comparing `dRFEtools-0.2.0/LICENSE` & `drfetools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dRFEtools-0.2.0/README.md` & `drfetools-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,54 +25,62 @@
 
 Regression:
 
 1.  R2 (this can be negative if model is arbitrarily worse)
 2.  Explained variance
 3.  Mean squared error
 
-The package has been split in to three additional scripts for:
+The package has been split in to four additional scripts for:
 
-1.  Random forest feature elimination (AP)
-2.  Linear model regression feature elimination (KJB)
+1.  Out-of-bag dynamic RFE metrics (AP)
+2.  Validation set dynamic RFE metrics (KJB)
 3.  Rank features function (TK)
-4.  Lowess redundant selection (KJB)
+4.  Lowess core + peripheral selection (KJB)
 
 # Table of Contents
 
 1.  [Citation](#org7b64d47)
 2.  [Installation](#org04443e4)
-3.  [Reference Manual](#org5afd041)
+3.  [Tutorials](#org07777f88)
+4.  [Reference Manual](#org5afd041)
     1.  [dRFEtools main functions](#org6171433)
-    2.  [Redundant features functions](#org3cfdf65)
+    2.  [Peripheral features functions](#org3cfdf65)
     3.  [Plotting functions](#org8ecca01)
     4.  [Metric functions](#org377b1aa)
-    5.  [Linear model classes for dRFE](#org288aaeb)
-    6.  [SVM model classes for dRFE](#org1313shi)
-    7.  [Random forest helper functions](#orga29d49b)
-    8.  [Linear model helper functions](#orgbda21bf)
+    5.  [Random forest helper functions](#orga29d49b)
+    6.  [Linear model helper functions](#orgbda21bf)
 
 <a id="org7b64d47"></a>
 
 ## Citation
 
-If using please cite: [![DOI](https://zenodo.org/badge/402494754.svg)](https://zenodo.org/badge/latestdoi/402494754).
+If using please cite the following:
+Pre-print DOI: https://doi.org/10.1101/2022.07.27.501227
+[![DOI](https://zenodo.org/badge/402494754.svg)](https://zenodo.org/badge/latestdoi/402494754).
 
 
 <a id="org04443e4"></a>
 
 ## Installation
 
 `pip install --user dRFEtools`
 
+<a id="org07777f88"></a>
+## Tutorials
+
+Follow [this](https://github.com/LieberInstitute/dRFEtools_manuscript/blob/main/optimization/_m/optimization.ipynb) jupyter notebook for an example on optimization.
+
+The GitHub below has example code for sklearn simulation, biological simulation, and using BrainSEQ Phase 1.
+
+[https://github.com/LieberInstitute/dRFEtools_manuscript](https://github.com/LieberInstitute/dRFEtools_manuscript/tree/main)
 
 <a id="org5afd041"></a>
 
 ## Reference Manual
 
-
 <a id="org6171433"></a>
 
 ### dRFEtools main functions
 
 1.  dRFE - Random Forest
 
     `rf_rfe`
@@ -150,17 +158,32 @@
     -   keep_rate: percentage of features to keep
 
     **Yields:**
 
     -   int: number of features to keep
 
 
+5.  Calculate feature importance
+
+    `cal_feature_imp`
+
+    Generates feature importance from absolute value of feature weights.
+	
+	**Args:**
+	
+	-  estimator: the estimator to generate feature importance for
+	
+	**Yields:**
+	
+	-  estimator: returns the estimator with feature importance
+
+
 <a id="org3cfdf65"></a>
 
-### Redundant features functions
+### Peripheral features functions
 
 1.  Run lowess
 
     `run_lowess`
 
     This function runs the lowess function and caches it to memory.
 
@@ -253,60 +276,60 @@
     -   frac: the fraction of the data used when estimating each y-value. default 3/10
     -   multi: is this for multiple classes. default False
 
     **Yields:**
 
     -   int: number of max features (smallest subset)
 
-7.  Extract redundant lowess
+7.  Extract peripheral lowess
 
-    `extract_redundant_lowess`
+    `extract_peripheral_lowess`
 
-    This function extracts the redundant features based on rate of change of log10
+    This function extracts the peripheral features based on rate of change of log10
     transformed lowess fit curve.
 
     **Args:**
 
     -   d: dRFE dictionary
     -   frac: the fraction of the data used when estimating each y-value. default 3/10
     -   step_size: rate of change step size to analyze for extraction. default 0.05
     -   multi: is this for multiple classes. default False
 
     **Yields:**
 
-    -   int: number of redundant features
+    -   int: number of peripheral features
 
 8.  Optimize lowess plot
 
     `plot_with_lowess_vline`
 
-    Redundant set selection optimization plot. This will be ROC AUC for multiple
+    Peripheral set selection optimization plot. This will be ROC AUC for multiple
     classification (3+), NMI for binary classification, or R2 for regression. The
     plot returned has fraction and step size as well as lowess smoothed curve and
-    indication of predicted redundant set.
+    indication of predicted peripheral set.
 
     **Args:**
 
     -   d: feature elimination class dictionary
     -   fold: current fold
     -   out_dir: output directory. default '.'
     -   frac: the fraction of the data used when estimating each y-value. default 3/10
     -   step_size: rate of change step size to analyze for extraction. default 0.05
     -   classify: is this a classification algorithm. default True
     -   multi: does this have multiple (3+) classes. default True
 
     **Yields:**
 
-    -   graph: plot of dRFE with estimated redundant set indicated as well as fraction and set size used. It automatically saves files as pdf, png, and svg
+    -   graph: plot of dRFE with estimated peripheral set indicated as well as fraction and set size used. It automatically saves files as pdf, png, and svg
 
 9.  Plot lowess vline
 
     `plot_with_lowess_vline`
 
-    Plot feature elimination results with the redundant set indicated. This will be
+    Plot feature elimination results with the peripheral set indicated. This will be
     ROC AUC for multiple classification (3+), NMI for binary classification, or R2
     for regression.
 
     **Args:**
 
     -   d: feature elimination class dictionary
     -   fold: current fold
@@ -314,15 +337,15 @@
     -   frac: the fraction of the data used when estimating each y-value. default 3/10
     -   step_size: rate of change step size to analyze for extraction. default 0.05
     -   classify: is this a classification algorithm. default True
     -   multi: does this have multiple (3+) classes. default True
 
     **Yields:**
 
-    -   graph: plot of dRFE with estimated redundant set indicated, automatically saves files as pdf, png, and svg
+    -   graph: plot of dRFE with estimated peripheral set indicated, automatically saves files as pdf, png, and svg
 
 
 <a id="org8ecca01"></a>
 
 ### Plotting functions
 
 1.  Save plots
@@ -656,132 +679,14 @@
     -   X: a data frame of normalized values from developmental dataset
     -   Y: a vector of sample labels from training data set
 
     **Yields:**
 
     -   float: AUC ROC score
 
-<a id="org288aaeb"></a>
-
-### Linear model classes for dRFE
-
-1.  Lasso Class
-
-    `Lasso` and `LassoCV`
-
-    Add feature importance to Lasso class similar to
-    random forest output. LassoCV uses cross-validation for alpha tuning.
-
-2.  Ridge Class
-
-    `Ridge` and `RidgeCV`
-
-    Add feature importance to Ridge class similar to
-    random forest output. LassoCV uses cross-validation for alpha tuning.
-
-3.  ElasticNet Class
-
-    `ElasticNet` and `ElasticNetCV`
-
-    Add feature importance to ElasticNet class similar to
-    random forest output. ElasticNetCV uses cross-validation to chose alpha.
-
-4.  LinearRegression Class
-
-    `LinearRegression`
-
-    Add feature importance to LinearRegression class similar to
-    random forest output.
-
-5. LogisticRegression
-
-    `LogisticRegression`
-
-    Adds feature importance to LogisticRegression class similar to
-    random forest output. This was originally modified from Apua
-    Paquola script.
-
-<a id="org1313shi"></a>
-
-### SVM model classes for dRFE
-
-1.  LinearSVC Class
-
-    `LinearSVC`
-
-    Add feature importance to linear SVC class similar to
-    random forest output.
-
-2.  LinearSVR Class
-
-    `LinearSVR`
-
-    Add feature importance to linear SVR class similar to
-    random forest output.
-
-3.  SGDClassifier Class
-
-    `SGDClassifier`
-
-    Add feature importance to stochastic gradient descent classification
-    class similar to random forest output.
-
-4.  SGDRegressor Class
-
-    `SGDRegressor`
-
-    Add feature importance to stochastic gradient descent regression
-    class similar to random forest output.
-
-<a id="orga29d49b"></a>
-
-### Random forest helper functions
-
-1.  dRFE Subfunction
-
-    `rf_fe`
-
-    Iterate over features to by eliminated by step.
-
-    **Args:**
-
-    -   estimator: Random forest classifier object
-    -   X: a data frame of training data
-    -   Y: a vector of sample labels from training data set
-    -   n_features_iter: iterator for number of features to keep loop
-    -   features: a vector of feature names
-    -   fold: current fold
-    -   out_dir: output directory. default '.'
-    -   RANK: Boolean (True or False)
-
-    **Yields:**
-
-    -   list: a list with number of features, normalized mutual information score, accuracy score, and array of the indices for features to keep
-
-2.  dRFE Step function
-
-    `rf_fe_step`
-
-    Apply random forest to training data, rank features, conduct feature elimination.
-
-    **Args:**
-
-    -   estimator: Random forest classifier object
-    -   X: a data frame of training data
-    -   Y: a vector of sample labels from training data set
-    -   n_features_to_keep: number of features to keep
-    -   features: a vector of feature names
-    -   fold: current fold
-    -   out_dir: output directory. default '.'
-    -   RANK: Boolean (True or False)
-
-    **Yields:**
-
-    -   dict: a dictionary with number of features, normalized mutual information score, accuracy score, and selected features
-
 
 <a id="orgbda21bf"></a>
 
 ### Linear model helper functions
 
 1.  dRFE Subfunction
```

### Comparing `dRFEtools-0.2.0/dRFEtools/dRFEtools.py` & `drfetools-0.3.0/dRFEtools/dRFEtools.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,37 +12,35 @@
 3. Area under the curve (AUC) ROC curve
 
 Regression:
 1. R2 (this can be negative if model is arbitrarily worse)
 2. Explained variance
 3. Mean squared error
 
-The package has been split in to three additional scripts for:
-1. Random forest feature elimination (AP)
-2. Linear model regression feature elimination (KJB)
+The package has been split in to four additional scripts for:
+1. Out-of-bag dynamic RFE metrics (AP)
+2. Validation set dynamic RFE metrics (KJB)
 3. Rank features function (TK)
-4. Lowess redundant selection (KJB)
+4. Lowess core + peripheral selection (KJB)
 
 Original author Apuã Paquola (AP).
 Edits and package management by Kynon Jade Benjamin (KJB)
 Feature ranking modified from Tarun Katipalli (TK) ranking function.
 """
 __author__ = 'Apuã Paquola'
 
 import numpy as np
 import pandas as pd
 from plotnine import *
-from .svm_models import *
 from .dev_scoring import *
 from .random_forest import *
 from .lowess_redundant import *
-from .linear_models_rfe import *
 from warnings import filterwarnings
 from matplotlib.cbook import mplDeprecation
-from sklearn.metrics import balanced_accuracy_score
+
 filterwarnings("ignore", category=mplDeprecation)
 filterwarnings('ignore', category=UserWarning, module='plotnine.*')
 filterwarnings('ignore', category=DeprecationWarning, module='plotnine.*')
 
 
 def n_features_iter(nf, keep_rate):
     """
@@ -266,15 +264,15 @@
             label = 'NMI'
     else:
         label = 'R2'
     _, max_feat_log10 = extract_max_lowess(d, frac, multi, acc)
     x,y,z,_,_ = cal_lowess(d, frac, multi, acc)
     df_elim = pd.DataFrame({'X': x, 'Y': y})
     _,lo = extract_max_lowess(d, frac, multi, acc)
-    _,l1 = extract_redundant_lowess(d, frac, step_size, multi, acc)
+    _,l1 = extract_peripheral_lowess(d, frac, step_size, multi, acc)
     gg = ggplot(df_elim, aes(x='X', y='Y')) + geom_point(color='blue') + \
         geom_vline(xintercept=lo, color='blue', linetype='dashed') + \
         geom_vline(xintercept=l1, color='orange', linetype='dashed') +\
         scale_x_log10() + labs(x='log10(N Features)', y=label) +\
         theme_light()
     print(gg)
     save_plot(gg, "%s/%s_log10_dRFE_fold_%d" %
```

### Comparing `dRFEtools-0.2.0/dRFEtools/dev_scoring.py` & `drfetools-0.3.0/dRFEtools/dev_scoring.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 """
-This script contains the linear model modification of the original
-random forest feature elimination package. Instead of Out-of-Bag, it creates
-a developmental test set from the training data.
+This script contains the feature elimination step using a
+validation set (developmental) to train the dynamic feature
+elimination.
 
 Developed by Kynon Jade Benjamin.
 """
 
 __author__ = 'Kynon J Benjamin'
 
 import numpy as np
-import pandas as pd
 from itertools import chain
 from sklearn.metrics import r2_score
 from sklearn.base import is_classifier
 from .rank_function import features_rank_fnc
 from sklearn.metrics import mean_squared_error
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import explained_variance_score
 from sklearn.inspection import permutation_importance
 from sklearn.metrics import normalized_mutual_info_score
 from sklearn.metrics import roc_auc_score, accuracy_score
 
 
+def cal_feature_imp(estimator):
+    """
+    Adds feature importance to a scikit-learn estimator. This is similar
+    to random forest output feature importances output.
+
+    This function also checks dimensions to handle multi-class inputs.
+    """
+    if estimator.coef_.ndim == 1:
+        estimator.feature_importances_ = np.abs(estimator.coef_).flatten()
+    else:
+        estimator.feature_importances_ = np.amax(np.abs(estimator.coef_),
+                                                 axis=0).flatten()
+    return estimator
+
+
 def dev_predictions(estimator, X):
     """
     Extracts predictions using a development fold for linear model
     regression.
 
     Args:
     estimator: linear model regression object
@@ -170,14 +184,15 @@
     X1, X2, Y1, Y2 = train_test_split(X, Y, **kwargs)
     # print(X.shape[1], n_features_to_keep)
     assert n_features_to_keep <= X1.shape[1]
     estimator.fit(X1, Y1)
     test_indices = np.array(range(X1.shape[1]))
     #res = permutation_importance(estimator, X2, Y2, n_jobs=-1, random_state=13)
     #rank = test_indices[res.importances_mean.argsort()]
+    estimator = cal_feature_imp(estimator)
     rank = test_indices[np.argsort(estimator.feature_importances_)]
     rank = rank[::-1] # reverse sort
     selected = rank[0:n_features_to_keep]
     features_rank_fnc(features, rank, n_features_to_keep, fold, out_dir, RANK)
     if is_classifier(estimator):
         return {"n_features": X1.shape[1],
                 "nmi_score": dev_score_nmi(estimator, X2, Y2),
```

### Comparing `dRFEtools-0.2.0/dRFEtools/lowess_redundant.py` & `drfetools-0.3.0/dRFEtools/lowess_redundant.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-This script contains functions to calculate redundant features based
-on a lowess fitted curve. Uses a log10 transformation of feature inputs.
-Also contains the optimization plot function for manual parameter
-optimization for lowess.
+This script contains functions to calculate core + peripheral features
+based on a lowess fitted curve. Uses a log10 transformation of feature
+inputs. Also contains the optimization plot function for manual
+parameter optimization for lowess.
 
 Developed by Kynon Jade Benjamin.
 """
 
 __author__ = 'Kynon J Benjamin'
 
 import numpy as np
@@ -102,43 +102,43 @@
     transformed lowess fit curve.
 
     Args:
     d: Dictionary from dRFE
     frac: Fraction for lowess smoothing. Default 3/10.
 
     Yields:
-    int: number of redundant features
+    int: number of peripheral features
     """
     _,_,z,xnew,ynew = cal_lowess(d, frac, multi, acc)
     df_elim = get_elim_df_ordered(d, multi)
     df_lowess = pd.DataFrame({'X': xnew, 'Y': ynew,
                               'xprime': pd.DataFrame(z)[0],
                               'yprime': pd.DataFrame(z)[1]})
     val = df_lowess[(df_lowess['yprime'] == max(df_lowess.yprime))].X.values
     closest_val = min(df_elim['log10_x'].values, key=lambda x: abs(x - val))
     return df_elim[(df_elim['log10_x'] == closest_val)].x.values[0], closest_val
 
 
-def extract_redundant_lowess(d, frac=3/10, step_size=0.02, multi=False,
+def extract_peripheral_lowess(d, frac=3/10, step_size=0.02, multi=False,
                              acc=False):
     """
-    Extract redundant features based on rate of change of log10
+    Extract peripheral features based on rate of change of log10
     transformed lowess fit curve.
 
     Args:
     d: Dictionary from dRFE
     frac: Fraction for lowess smoothing. Default 3/10.
     step_size: Rate of change step size to analyze for extraction
     (default: 0.02)
     multi: Is the target multi-class (boolean). Default False.
     classify: Is the target classification (boolean). Default True.
     acc: Use accuracy metric to optimize data (boolean). Default False.
 
     Yields:
-    int: number of redundant features
+    int: number of peripheral features
     """
     _,_,z,xnew,ynew = cal_lowess(d, frac, multi, acc)
     df_elim = get_elim_df_ordered(d, multi)
     df_lowess = pd.DataFrame({'X': xnew, 'Y': ynew,
                               'xprime': pd.DataFrame(z)[0],
                               'yprime': pd.DataFrame(z)[1]})
     dxdy = cal_lowess_rate_log10(d, frac, multi, acc)
@@ -148,16 +148,16 @@
         lo = (dxdy.iloc[yy, 2] - dxdy.iloc[yy-1, 2]) > step_size
         l1 = dxdy.iloc[yy, 2] < 0
         local_peak.append(lo & l1)
     local_peak.append(False)
     peaks = dxdy[local_peak]
     val = df_lowess[(df_lowess['xprime'] == max(peaks.Features))].X.values
     redunt_feat_log10 = min(df_elim['log10_x'].values, key=lambda x: abs(x - val))
-    redundant_feat = df_elim[(df_elim['log10_x'] == redunt_feat_log10)].x.values[0]
-    return redundant_feat, redunt_feat_log10
+    peripheral_feat = df_elim[(df_elim['log10_x'] == redunt_feat_log10)].x.values[0]
+    return peripheral_feat, redunt_feat_log10
 
 
 def optimize_lowess_plot(d, fold, output_dir, frac=3/10, step_size=0.02,
                          classify=True, save_plot=False, multi=False, acc=False,
                          print_out=True):
     """
     Plot the LOWESS smoothing plot for RFE with lines annotating set selection.
@@ -189,25 +189,25 @@
     title = 'Fraction: %.2f, Step Size: %.2f' % (frac, step_size)
     # transform to linear scale
     x,y,z,_,_ = cal_lowess(d, frac, multi, acc)
     df_elim = pd.DataFrame({'X': np.exp(x) - 0.5, 'Y': y})
     lowess_df = pd.DataFrame(z, columns=["X0", "Y0"])
     lowess_df.loc[:,"X0"] = np.exp(lowess_df["X0"]) - 0.5
     lo,_ = extract_max_lowess(d, frac, multi, acc)
-    l1,_ = extract_redundant_lowess(d, frac, step_size, multi, acc)
+    l1,_ = extract_peripheral_lowess(d, frac, step_size, multi, acc)
     # Plot
     plt.clf()
     f1 = plt.figure()
     plt.plot(df_elim["X"], df_elim["Y"], 'o', label="dRFE")
     plt.plot(lowess_df["X0"], lowess_df["Y0"], '-', label="Lowess")
     plt.vlines(lo, ymin=np.min(y), ymax=np.max(y), colors='b',
                linestyles='--', label='Max Features')
     plt.vlines(l1, ymin=np.min(y), ymax=np.max(y),
                colors='orange', linestyles='--',
-               label='Redundant Features')
+               label='Peripheral Features')
     plt.xscale('log'); plt.xlabel('log(N Features)')
     plt.ylabel(label); plt.legend(loc='best'); plt.title(title)
     if save_plot:
         plt.savefig("%s/optimize_lowess_%s_frac%.2f_step_%.2f_%s.png" %
                     (output_dir, fold, frac, step_size, label.replace(" ", "_")))
         plt.savefig("%s/optimize_lowess_%s_frac%.2f_step_%.2f_%s.pdf" %
                     (output_dir, fold, frac, step_size, label.replace(" ", "_")))
```

### Comparing `dRFEtools-0.2.0/dRFEtools/random_forest.py` & `drfetools-0.3.0/dRFEtools/random_forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 1. Normalized mutual information
 2. Accuracy
 3. Area under the curve (AUC) ROC curve
 
 Original author Apua Paquola.
 Edits: Kynon Jade Benjamin
 Feature ranking modified from Tarun Katipalli ranking function.
+
+Additional modification by KJB to replace class definitions of functions.
 """
 
 __author__ = 'Kynon Jade Benjamin'
 
 import numpy as np
-import pandas as pd
 from itertools import chain
 from sklearn.metrics import r2_score
 from sklearn.metrics import roc_auc_score
 from sklearn.metrics import accuracy_score
 from .rank_function import features_rank_fnc
 from sklearn.metrics import mean_squared_error
 from sklearn.ensemble import RandomForestRegressor
```

### Comparing `dRFEtools-0.2.0/dRFEtools/rank_function.py` & `drfetools-0.3.0/dRFEtools/rank_function.py`

 * *Files identical despite different names*

### Comparing `dRFEtools-0.2.0/pyproject.toml` & `drfetools-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "dRFEtools"
 packages = [
     {include = "dRFEtools"}
 ]
-version = "0.2.0"
+version = "0.3.0"
 description = "A package for preforming dynamic recursive feature elimination with sklearn."
 authors = ["Kynon JM Benjamin <kj.benjamin90@gmail.com>", "Apuã Paquola <apua.paquola@libd.org>"]
 maintainers = ["Kynon JM Benjamin <kj.benjamin90@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
-homepage = "https://github.com/paquolalab/dRFEtools.git"
-repository = "https://github.com/paquolalab/dRFEtools.git"
+homepage = "https://github.com/LieberInstitute/dRFEtools.git"
+repository = "https://github.com/LieberInstitute/dRFEtools.git"
 keywords = ['recursive feature elimination', 'sklearn', 'feature ranking']
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 numpy = "^1.20.1"
 pandas = "^1.2.4"
 matplotlib = "^3.3.4"
```

### Comparing `dRFEtools-0.2.0/setup.py` & `drfetools-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,766 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: drfetools
+Version: 0.3.0
+Summary: A package for preforming dynamic recursive feature elimination with sklearn.
+Home-page: https://github.com/LieberInstitute/dRFEtools.git
+License: GPL-3.0-only
+Keywords: recursive feature elimination,sklearn,feature ranking
+Author: Kynon JM Benjamin
+Author-email: kj.benjamin90@gmail.com
+Maintainer: Kynon JM Benjamin
+Maintainer-email: kj.benjamin90@gmail.com
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (>=3.3.4,<4.0.0)
+Requires-Dist: numpy (>=1.20.1,<2.0.0)
+Requires-Dist: pandas (>=1.2.4,<2.0.0)
+Requires-Dist: plotnine (>=0.8.0,<0.9.0)
+Requires-Dist: scikit-learn (>=1.0,<2.0)
+Requires-Dist: scipy (>=1.6.0,<2.0.0)
+Requires-Dist: statsmodels (>=0.13.0,<0.14.0)
+Project-URL: Repository, https://github.com/LieberInstitute/dRFEtools.git
+Description-Content-Type: text/markdown
 
-packages = \
-['dRFEtools']
+# dRFEtools - dynamic Recursive Feature Elimination
 
-package_data = \
-{'': ['*']}
+`dRFEtools` is a package for dynamic recursive feature elimination with
+sklearn. Currently supporting random forest classification and regression,
+and linear models (linear, lasso, ridge, and elastic net).
 
-install_requires = \
-['matplotlib>=3.3.4,<4.0.0',
- 'numpy>=1.20.1,<2.0.0',
- 'pandas>=1.2.4,<2.0.0',
- 'plotnine>=0.8.0,<0.9.0',
- 'scikit-learn>=1.0,<2.0',
- 'scipy>=1.6.0,<2.0.0',
- 'statsmodels>=0.13.0,<0.14.0']
-
-setup_kwargs = {
-    'name': 'drfetools',
-    'version': '0.2.0',
-    'description': 'A package for preforming dynamic recursive feature elimination with sklearn.',
-    'long_description': '# dRFEtools - dynamic Recursive Feature Elimination\n\n`dRFEtools` is a package for dynamic recursive feature elimination with\nsklearn. Currently supporting random forest classification and regression,\nand linear models (linear, lasso, ridge, and elastic net).\n\nAuthors: Apuã Paquola, Kynon Jade Benjamin, and Tarun Katipalli\n\nPackage developed in Python 3.7+.\n\nIn addition to scikit-learn, `dRFEtools` is also built with NumPy, SciPy,\nPandas, matplotlib, plotnine, and statsmodels.\n\nThis package has several function to run dynamic recursive feature elimination\n(dRFE) for random forest and linear model classifier and regression models. For\nrandom forest, it assumes Out-of-Bag (OOB) is set to True. For linear models,\nit generates a developmental set. For both classification and regression, three\nmeasurements are calculated for feature selection:\n\nClassification:\n\n1.  Normalized mutual information\n2.  Accuracy\n3.  Area under the curve (AUC) ROC curve\n\nRegression:\n\n1.  R2 (this can be negative if model is arbitrarily worse)\n2.  Explained variance\n3.  Mean squared error\n\nThe package has been split in to three additional scripts for:\n\n1.  Random forest feature elimination (AP)\n2.  Linear model regression feature elimination (KJB)\n3.  Rank features function (TK)\n4.  Lowess redundant selection (KJB)\n\n# Table of Contents\n\n1.  [Citation](#org7b64d47)\n2.  [Installation](#org04443e4)\n3.  [Reference Manual](#org5afd041)\n    1.  [dRFEtools main functions](#org6171433)\n    2.  [Redundant features functions](#org3cfdf65)\n    3.  [Plotting functions](#org8ecca01)\n    4.  [Metric functions](#org377b1aa)\n    5.  [Linear model classes for dRFE](#org288aaeb)\n    6.  [SVM model classes for dRFE](#org1313shi)\n    7.  [Random forest helper functions](#orga29d49b)\n    8.  [Linear model helper functions](#orgbda21bf)\n\n<a id="org7b64d47"></a>\n\n## Citation\n\nIf using please cite: [![DOI](https://zenodo.org/badge/402494754.svg)](https://zenodo.org/badge/latestdoi/402494754).\n\n\n<a id="org04443e4"></a>\n\n## Installation\n\n`pip install --user dRFEtools`\n\n\n<a id="org5afd041"></a>\n\n## Reference Manual\n\n\n<a id="org6171433"></a>\n\n### dRFEtools main functions\n\n1.  dRFE - Random Forest\n\n    `rf_rfe`\n\n    Runs random forest feature elimination step over iterator process.\n\n    **Args:**\n\n    -   estimator: Random forest classifier object\n    -   X: a data frame of training data\n    -   Y: a vector of sample labels from training data set\n    -   features: a vector of feature names\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n    -   elimination_rate: percent rate to reduce feature list. default .2\n    -   RANK: Output feature ranking. default=True (Boolean)\n\n    **Yields:**\n\n    -   dict: a dictionary with number of features, normalized mutual information score, accuracy score, and array of the indexes for features to keep\n\n2.  dRFE - Linear Models\n\n    `dev_rfe`\n\n    Runs recursive feature elimination for linear model step over iterator\n    process assuming developmental set is needed.\n\n    **Args:**\n\n    -   estimator: regressor or classifier linear model object\n    -   X: a data frame of training data\n    -   Y: a vector of sample labels from training data set\n    -   features: a vector of feature names\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n    -   elimination_rate: percent rate to reduce feature list. default .2\n    -   dev_size: developmental set size. default \'0.20\'\n    -   RANK: run feature ranking, default \'True\'\n    -   SEED: random state. default \'True\'\n\n    **Yields:**\n\n    -   dict: a dictionary with number of features, r2 score, mean square error,\n        expalined variance, and array of the indices for features to keep\n\n3.  Feature Rank Function\n\n    `feature_rank_fnc`\n\n    This function ranks features within the feature elimination loop.\n\n    **Args:**\n\n    -   features: A vector of feature names\n    -   rank: A vector with feature ranks based on absolute value of feature importance\n    -   n_features_to_keep: Number of features to keep. (Int)\n    -   fold: Fold to analyzed. (Int)\n    -   out_dir: Output directory for text file. Default \'.\'\n    -   RANK: Boolean (True or False)\n\n    **Yields:**\n\n    -   Text file: Ranked features by fold tab-delimited text file, only if RANK=True\n\n4.  N Feature Iterator\n\n    `n_features_iter`\n\n    Determines the features to keep.\n\n    **Args:**\n\n    -   nf: current number of features\n    -   keep_rate: percentage of features to keep\n\n    **Yields:**\n\n    -   int: number of features to keep\n\n\n<a id="org3cfdf65"></a>\n\n### Redundant features functions\n\n1.  Run lowess\n\n    `run_lowess`\n\n    This function runs the lowess function and caches it to memory.\n\n    **Args:**\n\n    -   x: the x-values of the observed points\n    -   y: the y-values of the observed points\n    -   frac: the fraction of the data used when estimating each y-value. default 3/10\n\n    **Yields:**\n\n    -   z: 2D array of results\n\n2.  Convert array to tuple\n\n    `array_to_tuple`\n\n    This function attempts to convert a numpy array to a tuple.\n\n    **Args:**\n\n    -   np_array: numpy array\n\n    **Yields:**\n\n    -   tuple\n\n3.  Extract dRFE as a dataframe\n\n    `get_elim_df_ordered`\n\n    This function converts the dRFE dictionary to a pandas dataframe.\n\n    **Args:**\n\n    -   d: dRFE dictionary\n    -   multi: is this for multiple classes. (True or False)\n\n    **Yields:**\n\n    -   df_elim: dRFE as a dataframe with log10 transformed features\n\n4.  Calculate lowess curve\n\n    `cal_lowess`\n\n    This function calculates the lowess curve.\n\n    **Args:**\n\n    -   d: dRFE dictionary\n    -   frac: the fraction of the data used when estimating each y-value\n    -   multi: is this for multiple classes. (True or False)\n\n    **Yields:**\n\n    -   x: dRFE log10 transformed features\n    -   y: dRFE metrics\n    -   z: 2D numpy array with lowess curve\n    -   xnew: increased intervals\n    -   ynew: interpolated metrics for xnew\n\n5.  Calculate lowess curve for log10\n\n    `cal_lowess`\n\n    This function calculates the rate of change on the lowess fitted curve with\n    log10 transformated input.\n\n    **Args:**\n\n    -   d: dRFE dictionary\n    -   frac: the fraction of the data used when estimating each y-value\n    -   multi: is this for multiple classes. default False\n\n    **Yields:**\n\n    -   data frame: dataframe with n_features, lowess value, and rate of change (DxDy)\n\n6.  Extract max lowess\n\n    `extract_max_lowess`\n\n    This function extracts the max features based on rate of change of log10\n    transformed lowess fit curve.\n\n    **Args:**\n\n    -   d: dRFE dictionary\n    -   frac: the fraction of the data used when estimating each y-value. default 3/10\n    -   multi: is this for multiple classes. default False\n\n    **Yields:**\n\n    -   int: number of max features (smallest subset)\n\n7.  Extract redundant lowess\n\n    `extract_redundant_lowess`\n\n    This function extracts the redundant features based on rate of change of log10\n    transformed lowess fit curve.\n\n    **Args:**\n\n    -   d: dRFE dictionary\n    -   frac: the fraction of the data used when estimating each y-value. default 3/10\n    -   step_size: rate of change step size to analyze for extraction. default 0.05\n    -   multi: is this for multiple classes. default False\n\n    **Yields:**\n\n    -   int: number of redundant features\n\n8.  Optimize lowess plot\n\n    `plot_with_lowess_vline`\n\n    Redundant set selection optimization plot. This will be ROC AUC for multiple\n    classification (3+), NMI for binary classification, or R2 for regression. The\n    plot returned has fraction and step size as well as lowess smoothed curve and\n    indication of predicted redundant set.\n\n    **Args:**\n\n    -   d: feature elimination class dictionary\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n    -   frac: the fraction of the data used when estimating each y-value. default 3/10\n    -   step_size: rate of change step size to analyze for extraction. default 0.05\n    -   classify: is this a classification algorithm. default True\n    -   multi: does this have multiple (3+) classes. default True\n\n    **Yields:**\n\n    -   graph: plot of dRFE with estimated redundant set indicated as well as fraction and set size used. It automatically saves files as pdf, png, and svg\n\n9.  Plot lowess vline\n\n    `plot_with_lowess_vline`\n\n    Plot feature elimination results with the redundant set indicated. This will be\n    ROC AUC for multiple classification (3+), NMI for binary classification, or R2\n    for regression.\n\n    **Args:**\n\n    -   d: feature elimination class dictionary\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n    -   frac: the fraction of the data used when estimating each y-value. default 3/10\n    -   step_size: rate of change step size to analyze for extraction. default 0.05\n    -   classify: is this a classification algorithm. default True\n    -   multi: does this have multiple (3+) classes. default True\n\n    **Yields:**\n\n    -   graph: plot of dRFE with estimated redundant set indicated, automatically saves files as pdf, png, and svg\n\n\n<a id="org8ecca01"></a>\n\n### Plotting functions\n\n1.  Save plots\n\n    `save_plots`\n\n    This function save plot as svg, png, and pdf with specific label and dimension.\n\n    **Args:**\n\n    -   p: plotnine object\n    -   fn: file name without extensions\n    -   w: width, default 7\n    -   h: height, default 7\n\n    **Yields:** SVG, PNG, and PDF of plotnine object\n\n2.  Plot dRFE Accuracy\n\n    `plot_acc`\n\n    Plot feature elimination results for accuracy.\n\n    **Args:**\n\n    -   d: feature elimination class dictionary\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n\n    **Yields:**\n\n    -   graph: plot of feature by accuracy, automatically saves files as pdf, png, and svg\n\n3.  Plot dRFE NMI\n\n    `plot_nmi`\n\n    Plot feature elimination results for normalized mutual information.\n\n    **Args:**\n\n    -   d: feature elimination class dictionary\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n\n    **Yields:**\n\n    -   graph: plot of feature by NMI, automatically saves files as pdf, png, and svg\n\n4.  Plot dRFE ROC AUC\n\n    `plot_roc`\n\n    Plot feature elimination results for AUC ROC curve.\n\n    **Args:**\n\n    -   d: feature elimination class dictionary\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n\n    **Yields:**\n\n    -   graph: plot of feature by AUC, automatically saves files as pdf, png, and svg\n\n5.  Plot dRFE R2\n\n    `plot_r2`\n\n    Plot feature elimination results for R2 score. Note that this can be negative\n    if model is arbitarily worse.\n\n    **Args:**\n\n    -   d: feature elimination class dictionary\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n\n    **Yields:**\n\n    -   graph: plot of feature by R2, automatically saves files as pdf, png, and svg\n\n6.  Plot dRFE MSE\n\n    `plot_mse`\n\n    Plot feature elimination results for mean squared error score.\n\n    **Args:**\n\n    -   d: feature elimination class dictionary\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n\n    **Yields:**\n\n    -   graph: plot of feature by mean squared error, automatically saves files as pdf, png, and svg\n\n7.  Plot dRFE Explained Variance\n\n    `plot_evar`\n\n    Plot feature elimination results for explained variance score.\n\n    **Args:**\n\n    -   d: feature elimination class dictionary\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n\n    **Yields:**\n\n    -   graph: plot of feature by explained variance, automatically saves files as pdf, png, and svg\n\n\n<a id="org377b1aa"></a>\n\n### Metric functions\n\n1.  OOB Prediction\n\n    `oob_predictions`\n\n    Extracts out-of-bag (OOB) predictions from random forest classifier classes.\n\n    **Args:**\n\n    -   estimator: Random forest classifier object\n\n    **Yields:**\n\n    -   vector: OOB predicted labels\n\n2.  OOB Accuracy Score\n\n    `oob_score_accuracy`\n\n    Calculates the accuracy score from the OOB predictions.\n\n    **Args:**\n\n    -   estimator: Random forest classifier object\n    -   Y: a vector of sample labels from training data set\n\n    **Yields:**\n\n    -   float: accuracy score\n\n3.  OOB Normalized Mutual Information Score\n\n    `oob_score_nmi`\n\n    Calculates the normalized mutual information score from the OOB predictions.\n\n    **Args:**\n\n    -   estimator: Random forest classifier object\n    -   Y: a vector of sample labels from training data set\n\n    **Yields:**\n\n    -   float: normalized mutual information score\n\n4.  OOB Area Under ROC Curve Score\n\n    `oob_score_roc`\n\n    Calculates the area under the ROC curve score for the OOB predictions.\n\n    **Args:**\n\n    -   estimator: Random forest classifier object\n    -   Y: a vector of sample labels from training data set\n\n    **Yields:**\n\n    -   float: AUC ROC score\n\n5.  OOB R2 Score\n\n    `oob_score_r2`\n\n    Calculates the r2 score from the OOB predictions.\n\n    **Args:**\n\n    -   estimator: Random forest regressor object\n    -   Y: a vector of sample labels from training data set\n\n    **Yields:**\n\n    -   float: r2 score\n\n6.  OOB Mean Squared Error Score\n\n    `oob_score_mse`\n\n    Calculates the mean squared error score from the OOB predictions.\n\n    **Args:**\n\n    -   estimator: Random forest regressor object\n    -   Y: a vector of sample labels from training data set\n\n    **Yields:**\n\n    -   float: mean squared error score\n\n7.  OOB Explained Variance Score\n\n    `oob_score_evar`\n\n    Calculates the explained variance score for the OOB predictions.\n\n    **Args:**\n\n    -   estimator: Random forest regressor object\n    -   Y: a vector of sample labels from training data set\n\n    **Yields:**\n\n    -   float: explained variance score\n\n8.  Developmental Test Set Predictions\n\n    `dev_predictions`\n\n    Extracts predictions using a development fold for linear\n    regressor.\n\n    **Args:**\n\n    -   estimator: Linear model regression classifier object\n    -   X: a data frame of normalized values from developmental dataset\n\n    **Yields:**\n\n    -   vector: Development set predicted labels\n\n9.  Developmental Test Set R2 Score\n\n    `dev_score_r2`\n\n    Calculates the r2 score from the developmental dataset\n    predictions.\n\n    **Args:**\n\n    -   estimator: Linear model regressor object\n    -   X: a data frame of normalized values from developmental dataset\n    -   Y: a vector of sample labels from developmental dataset\n\n    **Yields:**\n\n    -   float: r2 score\n\n10. Developmental Test Set Mean Squared Error Score\n\n    `dev_score_mse`\n\n    Calculates the mean squared error score from the developmental dataset\n    predictions.\n\n    **Args:**\n\n    -   estimator: Linear model regressor object\n    -   X: a data frame of normalized values from developmental dataset\n    -   Y: a vector of sample labels from developmental dataset\n\n    **Yields:**\n\n    -   float: mean squared error score\n\n11. Developmental Test Set Explained Variance Score\n\n    `dev_score_evar`\n\n    Calculates the explained variance score for the develomental dataset predictions.\n\n    **Args:**\n\n    -   estimator: Linear model regressor object\n    -   X: a data frame of normalized values from developmental dataset\n    -   Y: a vector of sample labels from developmental data set\n\n    **Yields:**\n\n    -   float: explained variance score\n\n12.  DEV Accuracy Score\n\n    `dev_score_accuracy`\n\n    Calculates the accuracy score from the DEV predictions.\n\n    **Args:**\n\n    -   estimator: Linear model classifier object\n    -   X: a data frame of normalized values from developmental dataset\n    -   Y: a vector of sample labels from training data set\n\n    **Yields:**\n\n    -   float: accuracy score\n\n13.  DEV Normalized Mutual Information Score\n\n    `dev_score_nmi`\n\n    Calculates the normalized mutual information score from the DEV predictions.\n\n    **Args:**\n\n    -   estimator: Linear model classifier object\n    -   X: a data frame of normalized values from developmental dataset\n    -   Y: a vector of sample labels from training data set\n\n    **Yields:**\n\n    -   float: normalized mutual information score\n\n14.  DEV Area Under ROC Curve Score\n\n    `dev_score_roc`\n\n    Calculates the area under the ROC curve score for the DEV predictions.\n\n    **Args:**\n\n    -   estimator: Linear model classifier object\n    -   X: a data frame of normalized values from developmental dataset\n    -   Y: a vector of sample labels from training data set\n\n    **Yields:**\n\n    -   float: AUC ROC score\n\n<a id="org288aaeb"></a>\n\n### Linear model classes for dRFE\n\n1.  Lasso Class\n\n    `Lasso` and `LassoCV`\n\n    Add feature importance to Lasso class similar to\n    random forest output. LassoCV uses cross-validation for alpha tuning.\n\n2.  Ridge Class\n\n    `Ridge` and `RidgeCV`\n\n    Add feature importance to Ridge class similar to\n    random forest output. LassoCV uses cross-validation for alpha tuning.\n\n3.  ElasticNet Class\n\n    `ElasticNet` and `ElasticNetCV`\n\n    Add feature importance to ElasticNet class similar to\n    random forest output. ElasticNetCV uses cross-validation to chose alpha.\n\n4.  LinearRegression Class\n\n    `LinearRegression`\n\n    Add feature importance to LinearRegression class similar to\n    random forest output.\n\n5. LogisticRegression\n\n    `LogisticRegression`\n\n    Adds feature importance to LogisticRegression class similar to\n    random forest output. This was originally modified from Apua\n    Paquola script.\n\n<a id="org1313shi"></a>\n\n### SVM model classes for dRFE\n\n1.  LinearSVC Class\n\n    `LinearSVC`\n\n    Add feature importance to linear SVC class similar to\n    random forest output.\n\n2.  LinearSVR Class\n\n    `LinearSVR`\n\n    Add feature importance to linear SVR class similar to\n    random forest output.\n\n3.  SGDClassifier Class\n\n    `SGDClassifier`\n\n    Add feature importance to stochastic gradient descent classification\n    class similar to random forest output.\n\n4.  SGDRegressor Class\n\n    `SGDRegressor`\n\n    Add feature importance to stochastic gradient descent regression\n    class similar to random forest output.\n\n<a id="orga29d49b"></a>\n\n### Random forest helper functions\n\n1.  dRFE Subfunction\n\n    `rf_fe`\n\n    Iterate over features to by eliminated by step.\n\n    **Args:**\n\n    -   estimator: Random forest classifier object\n    -   X: a data frame of training data\n    -   Y: a vector of sample labels from training data set\n    -   n_features_iter: iterator for number of features to keep loop\n    -   features: a vector of feature names\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n    -   RANK: Boolean (True or False)\n\n    **Yields:**\n\n    -   list: a list with number of features, normalized mutual information score, accuracy score, and array of the indices for features to keep\n\n2.  dRFE Step function\n\n    `rf_fe_step`\n\n    Apply random forest to training data, rank features, conduct feature elimination.\n\n    **Args:**\n\n    -   estimator: Random forest classifier object\n    -   X: a data frame of training data\n    -   Y: a vector of sample labels from training data set\n    -   n_features_to_keep: number of features to keep\n    -   features: a vector of feature names\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n    -   RANK: Boolean (True or False)\n\n    **Yields:**\n\n    -   dict: a dictionary with number of features, normalized mutual information score, accuracy score, and selected features\n\n\n<a id="orgbda21bf"></a>\n\n### Linear model helper functions\n\n1.  dRFE Subfunction\n\n    `regr_fe`\n\n    Iterate over features to by eliminated by step.\n\n    **Args:**\n\n    -   estimator: regressor or classifier linear model object\n    -   X: a data frame of training data\n    -   Y: a vector of sample labels from training data set\n    -   n_features_iter: iterator for number of features to keep loop\n    -   features: a vector of feature names\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n    -   dev_size: developmental test set propotion of training\n    -   SEED: random state\n    -   RANK: Boolean (True or False)\n\n    **Yields:**\n\n    -   list: a list with number of features, r2 score, mean square error, expalined variance, and array of the indices for features to keep\n\n2.  dRFE Step function\n\n    `regr_fe_step`\n\n    Split training data into developmental dataset and apply estimator\n    to developmental dataset, rank features, and conduct feature\n    elimination, single steps.\n\n    **Args:**\n\n    -   estimator: regressor or classifier linear model object\n    -   X: a data frame of training data\n    -   Y: a vector of sample labels from training data set\n    -   n_features_to_keep: number of features to keep\n    -   features: a vector of feature names\n    -   fold: current fold\n    -   out_dir: output directory. default \'.\'\n    -   dev_size: developmental test set propotion of training\n    -   SEED: random state\n    -   RANK: Boolean (True or False)\n\n    **Yields:**\n\n    -   dict: a dictionary with number of features, r2 score, mean square error, expalined variance, and selected features\n',
-    'author': 'Kynon JM Benjamin',
-    'author_email': 'kj.benjamin90@gmail.com',
-    'maintainer': 'Kynon JM Benjamin',
-    'maintainer_email': 'kj.benjamin90@gmail.com',
-    'url': 'https://github.com/paquolalab/dRFEtools.git',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<4.0.0',
-}
+Authors: Apuã Paquola, Kynon Jade Benjamin, and Tarun Katipalli
 
+Package developed in Python 3.7+.
+
+In addition to scikit-learn, `dRFEtools` is also built with NumPy, SciPy,
+Pandas, matplotlib, plotnine, and statsmodels.
+
+This package has several function to run dynamic recursive feature elimination
+(dRFE) for random forest and linear model classifier and regression models. For
+random forest, it assumes Out-of-Bag (OOB) is set to True. For linear models,
+it generates a developmental set. For both classification and regression, three
+measurements are calculated for feature selection:
+
+Classification:
+
+1.  Normalized mutual information
+2.  Accuracy
+3.  Area under the curve (AUC) ROC curve
+
+Regression:
+
+1.  R2 (this can be negative if model is arbitrarily worse)
+2.  Explained variance
+3.  Mean squared error
+
+The package has been split in to four additional scripts for:
+
+1.  Out-of-bag dynamic RFE metrics (AP)
+2.  Validation set dynamic RFE metrics (KJB)
+3.  Rank features function (TK)
+4.  Lowess core + peripheral selection (KJB)
+
+# Table of Contents
+
+1.  [Citation](#org7b64d47)
+2.  [Installation](#org04443e4)
+3.  [Tutorials](#org07777f88)
+4.  [Reference Manual](#org5afd041)
+    1.  [dRFEtools main functions](#org6171433)
+    2.  [Peripheral features functions](#org3cfdf65)
+    3.  [Plotting functions](#org8ecca01)
+    4.  [Metric functions](#org377b1aa)
+    5.  [Random forest helper functions](#orga29d49b)
+    6.  [Linear model helper functions](#orgbda21bf)
+
+<a id="org7b64d47"></a>
+
+## Citation
+
+If using please cite the following:
+Pre-print DOI: https://doi.org/10.1101/2022.07.27.501227
+[![DOI](https://zenodo.org/badge/402494754.svg)](https://zenodo.org/badge/latestdoi/402494754).
+
+
+<a id="org04443e4"></a>
+
+## Installation
+
+`pip install --user dRFEtools`
+
+<a id="org07777f88"></a>
+## Tutorials
+
+Follow [this](https://github.com/LieberInstitute/dRFEtools_manuscript/blob/main/optimization/_m/optimization.ipynb) jupyter notebook for an example on optimization.
+
+The GitHub below has example code for sklearn simulation, biological simulation, and using BrainSEQ Phase 1.
+
+[https://github.com/LieberInstitute/dRFEtools_manuscript](https://github.com/LieberInstitute/dRFEtools_manuscript/tree/main)
+
+<a id="org5afd041"></a>
+
+## Reference Manual
+
+<a id="org6171433"></a>
+
+### dRFEtools main functions
+
+1.  dRFE - Random Forest
+
+    `rf_rfe`
+
+    Runs random forest feature elimination step over iterator process.
+
+    **Args:**
+
+    -   estimator: Random forest classifier object
+    -   X: a data frame of training data
+    -   Y: a vector of sample labels from training data set
+    -   features: a vector of feature names
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+    -   elimination_rate: percent rate to reduce feature list. default .2
+    -   RANK: Output feature ranking. default=True (Boolean)
+
+    **Yields:**
+
+    -   dict: a dictionary with number of features, normalized mutual information score, accuracy score, and array of the indexes for features to keep
+
+2.  dRFE - Linear Models
+
+    `dev_rfe`
+
+    Runs recursive feature elimination for linear model step over iterator
+    process assuming developmental set is needed.
+
+    **Args:**
+
+    -   estimator: regressor or classifier linear model object
+    -   X: a data frame of training data
+    -   Y: a vector of sample labels from training data set
+    -   features: a vector of feature names
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+    -   elimination_rate: percent rate to reduce feature list. default .2
+    -   dev_size: developmental set size. default '0.20'
+    -   RANK: run feature ranking, default 'True'
+    -   SEED: random state. default 'True'
+
+    **Yields:**
+
+    -   dict: a dictionary with number of features, r2 score, mean square error,
+        expalined variance, and array of the indices for features to keep
+
+3.  Feature Rank Function
+
+    `feature_rank_fnc`
+
+    This function ranks features within the feature elimination loop.
+
+    **Args:**
+
+    -   features: A vector of feature names
+    -   rank: A vector with feature ranks based on absolute value of feature importance
+    -   n_features_to_keep: Number of features to keep. (Int)
+    -   fold: Fold to analyzed. (Int)
+    -   out_dir: Output directory for text file. Default '.'
+    -   RANK: Boolean (True or False)
+
+    **Yields:**
+
+    -   Text file: Ranked features by fold tab-delimited text file, only if RANK=True
+
+4.  N Feature Iterator
+
+    `n_features_iter`
+
+    Determines the features to keep.
+
+    **Args:**
+
+    -   nf: current number of features
+    -   keep_rate: percentage of features to keep
+
+    **Yields:**
+
+    -   int: number of features to keep
+
+
+5.  Calculate feature importance
+
+    `cal_feature_imp`
+
+    Generates feature importance from absolute value of feature weights.
+	
+	**Args:**
+	
+	-  estimator: the estimator to generate feature importance for
+	
+	**Yields:**
+	
+	-  estimator: returns the estimator with feature importance
+
+
+<a id="org3cfdf65"></a>
+
+### Peripheral features functions
+
+1.  Run lowess
+
+    `run_lowess`
+
+    This function runs the lowess function and caches it to memory.
+
+    **Args:**
+
+    -   x: the x-values of the observed points
+    -   y: the y-values of the observed points
+    -   frac: the fraction of the data used when estimating each y-value. default 3/10
+
+    **Yields:**
+
+    -   z: 2D array of results
+
+2.  Convert array to tuple
+
+    `array_to_tuple`
+
+    This function attempts to convert a numpy array to a tuple.
+
+    **Args:**
+
+    -   np_array: numpy array
+
+    **Yields:**
+
+    -   tuple
+
+3.  Extract dRFE as a dataframe
+
+    `get_elim_df_ordered`
+
+    This function converts the dRFE dictionary to a pandas dataframe.
+
+    **Args:**
+
+    -   d: dRFE dictionary
+    -   multi: is this for multiple classes. (True or False)
+
+    **Yields:**
+
+    -   df_elim: dRFE as a dataframe with log10 transformed features
+
+4.  Calculate lowess curve
+
+    `cal_lowess`
+
+    This function calculates the lowess curve.
+
+    **Args:**
+
+    -   d: dRFE dictionary
+    -   frac: the fraction of the data used when estimating each y-value
+    -   multi: is this for multiple classes. (True or False)
+
+    **Yields:**
+
+    -   x: dRFE log10 transformed features
+    -   y: dRFE metrics
+    -   z: 2D numpy array with lowess curve
+    -   xnew: increased intervals
+    -   ynew: interpolated metrics for xnew
+
+5.  Calculate lowess curve for log10
+
+    `cal_lowess`
+
+    This function calculates the rate of change on the lowess fitted curve with
+    log10 transformated input.
+
+    **Args:**
+
+    -   d: dRFE dictionary
+    -   frac: the fraction of the data used when estimating each y-value
+    -   multi: is this for multiple classes. default False
+
+    **Yields:**
+
+    -   data frame: dataframe with n_features, lowess value, and rate of change (DxDy)
+
+6.  Extract max lowess
+
+    `extract_max_lowess`
+
+    This function extracts the max features based on rate of change of log10
+    transformed lowess fit curve.
+
+    **Args:**
+
+    -   d: dRFE dictionary
+    -   frac: the fraction of the data used when estimating each y-value. default 3/10
+    -   multi: is this for multiple classes. default False
+
+    **Yields:**
+
+    -   int: number of max features (smallest subset)
+
+7.  Extract peripheral lowess
+
+    `extract_peripheral_lowess`
+
+    This function extracts the peripheral features based on rate of change of log10
+    transformed lowess fit curve.
+
+    **Args:**
+
+    -   d: dRFE dictionary
+    -   frac: the fraction of the data used when estimating each y-value. default 3/10
+    -   step_size: rate of change step size to analyze for extraction. default 0.05
+    -   multi: is this for multiple classes. default False
+
+    **Yields:**
+
+    -   int: number of peripheral features
+
+8.  Optimize lowess plot
+
+    `plot_with_lowess_vline`
+
+    Peripheral set selection optimization plot. This will be ROC AUC for multiple
+    classification (3+), NMI for binary classification, or R2 for regression. The
+    plot returned has fraction and step size as well as lowess smoothed curve and
+    indication of predicted peripheral set.
+
+    **Args:**
+
+    -   d: feature elimination class dictionary
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+    -   frac: the fraction of the data used when estimating each y-value. default 3/10
+    -   step_size: rate of change step size to analyze for extraction. default 0.05
+    -   classify: is this a classification algorithm. default True
+    -   multi: does this have multiple (3+) classes. default True
+
+    **Yields:**
+
+    -   graph: plot of dRFE with estimated peripheral set indicated as well as fraction and set size used. It automatically saves files as pdf, png, and svg
+
+9.  Plot lowess vline
+
+    `plot_with_lowess_vline`
+
+    Plot feature elimination results with the peripheral set indicated. This will be
+    ROC AUC for multiple classification (3+), NMI for binary classification, or R2
+    for regression.
+
+    **Args:**
+
+    -   d: feature elimination class dictionary
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+    -   frac: the fraction of the data used when estimating each y-value. default 3/10
+    -   step_size: rate of change step size to analyze for extraction. default 0.05
+    -   classify: is this a classification algorithm. default True
+    -   multi: does this have multiple (3+) classes. default True
+
+    **Yields:**
+
+    -   graph: plot of dRFE with estimated peripheral set indicated, automatically saves files as pdf, png, and svg
+
+
+<a id="org8ecca01"></a>
+
+### Plotting functions
+
+1.  Save plots
+
+    `save_plots`
+
+    This function save plot as svg, png, and pdf with specific label and dimension.
+
+    **Args:**
+
+    -   p: plotnine object
+    -   fn: file name without extensions
+    -   w: width, default 7
+    -   h: height, default 7
+
+    **Yields:** SVG, PNG, and PDF of plotnine object
+
+2.  Plot dRFE Accuracy
+
+    `plot_acc`
+
+    Plot feature elimination results for accuracy.
+
+    **Args:**
+
+    -   d: feature elimination class dictionary
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+
+    **Yields:**
+
+    -   graph: plot of feature by accuracy, automatically saves files as pdf, png, and svg
+
+3.  Plot dRFE NMI
+
+    `plot_nmi`
+
+    Plot feature elimination results for normalized mutual information.
+
+    **Args:**
+
+    -   d: feature elimination class dictionary
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+
+    **Yields:**
+
+    -   graph: plot of feature by NMI, automatically saves files as pdf, png, and svg
+
+4.  Plot dRFE ROC AUC
+
+    `plot_roc`
+
+    Plot feature elimination results for AUC ROC curve.
+
+    **Args:**
+
+    -   d: feature elimination class dictionary
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+
+    **Yields:**
+
+    -   graph: plot of feature by AUC, automatically saves files as pdf, png, and svg
+
+5.  Plot dRFE R2
+
+    `plot_r2`
+
+    Plot feature elimination results for R2 score. Note that this can be negative
+    if model is arbitarily worse.
+
+    **Args:**
+
+    -   d: feature elimination class dictionary
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+
+    **Yields:**
+
+    -   graph: plot of feature by R2, automatically saves files as pdf, png, and svg
+
+6.  Plot dRFE MSE
+
+    `plot_mse`
+
+    Plot feature elimination results for mean squared error score.
+
+    **Args:**
+
+    -   d: feature elimination class dictionary
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+
+    **Yields:**
+
+    -   graph: plot of feature by mean squared error, automatically saves files as pdf, png, and svg
+
+7.  Plot dRFE Explained Variance
+
+    `plot_evar`
+
+    Plot feature elimination results for explained variance score.
+
+    **Args:**
+
+    -   d: feature elimination class dictionary
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+
+    **Yields:**
+
+    -   graph: plot of feature by explained variance, automatically saves files as pdf, png, and svg
+
+
+<a id="org377b1aa"></a>
+
+### Metric functions
+
+1.  OOB Prediction
+
+    `oob_predictions`
+
+    Extracts out-of-bag (OOB) predictions from random forest classifier classes.
+
+    **Args:**
+
+    -   estimator: Random forest classifier object
+
+    **Yields:**
+
+    -   vector: OOB predicted labels
+
+2.  OOB Accuracy Score
+
+    `oob_score_accuracy`
+
+    Calculates the accuracy score from the OOB predictions.
+
+    **Args:**
+
+    -   estimator: Random forest classifier object
+    -   Y: a vector of sample labels from training data set
+
+    **Yields:**
+
+    -   float: accuracy score
+
+3.  OOB Normalized Mutual Information Score
+
+    `oob_score_nmi`
+
+    Calculates the normalized mutual information score from the OOB predictions.
+
+    **Args:**
+
+    -   estimator: Random forest classifier object
+    -   Y: a vector of sample labels from training data set
+
+    **Yields:**
+
+    -   float: normalized mutual information score
+
+4.  OOB Area Under ROC Curve Score
+
+    `oob_score_roc`
+
+    Calculates the area under the ROC curve score for the OOB predictions.
+
+    **Args:**
+
+    -   estimator: Random forest classifier object
+    -   Y: a vector of sample labels from training data set
+
+    **Yields:**
+
+    -   float: AUC ROC score
+
+5.  OOB R2 Score
+
+    `oob_score_r2`
+
+    Calculates the r2 score from the OOB predictions.
+
+    **Args:**
+
+    -   estimator: Random forest regressor object
+    -   Y: a vector of sample labels from training data set
+
+    **Yields:**
+
+    -   float: r2 score
+
+6.  OOB Mean Squared Error Score
+
+    `oob_score_mse`
+
+    Calculates the mean squared error score from the OOB predictions.
+
+    **Args:**
+
+    -   estimator: Random forest regressor object
+    -   Y: a vector of sample labels from training data set
+
+    **Yields:**
+
+    -   float: mean squared error score
+
+7.  OOB Explained Variance Score
+
+    `oob_score_evar`
+
+    Calculates the explained variance score for the OOB predictions.
+
+    **Args:**
+
+    -   estimator: Random forest regressor object
+    -   Y: a vector of sample labels from training data set
+
+    **Yields:**
+
+    -   float: explained variance score
+
+8.  Developmental Test Set Predictions
+
+    `dev_predictions`
+
+    Extracts predictions using a development fold for linear
+    regressor.
+
+    **Args:**
+
+    -   estimator: Linear model regression classifier object
+    -   X: a data frame of normalized values from developmental dataset
+
+    **Yields:**
+
+    -   vector: Development set predicted labels
+
+9.  Developmental Test Set R2 Score
+
+    `dev_score_r2`
+
+    Calculates the r2 score from the developmental dataset
+    predictions.
+
+    **Args:**
+
+    -   estimator: Linear model regressor object
+    -   X: a data frame of normalized values from developmental dataset
+    -   Y: a vector of sample labels from developmental dataset
+
+    **Yields:**
+
+    -   float: r2 score
+
+10. Developmental Test Set Mean Squared Error Score
+
+    `dev_score_mse`
+
+    Calculates the mean squared error score from the developmental dataset
+    predictions.
+
+    **Args:**
+
+    -   estimator: Linear model regressor object
+    -   X: a data frame of normalized values from developmental dataset
+    -   Y: a vector of sample labels from developmental dataset
+
+    **Yields:**
+
+    -   float: mean squared error score
+
+11. Developmental Test Set Explained Variance Score
+
+    `dev_score_evar`
+
+    Calculates the explained variance score for the develomental dataset predictions.
+
+    **Args:**
+
+    -   estimator: Linear model regressor object
+    -   X: a data frame of normalized values from developmental dataset
+    -   Y: a vector of sample labels from developmental data set
+
+    **Yields:**
+
+    -   float: explained variance score
+
+12.  DEV Accuracy Score
+
+    `dev_score_accuracy`
+
+    Calculates the accuracy score from the DEV predictions.
+
+    **Args:**
+
+    -   estimator: Linear model classifier object
+    -   X: a data frame of normalized values from developmental dataset
+    -   Y: a vector of sample labels from training data set
+
+    **Yields:**
+
+    -   float: accuracy score
+
+13.  DEV Normalized Mutual Information Score
+
+    `dev_score_nmi`
+
+    Calculates the normalized mutual information score from the DEV predictions.
+
+    **Args:**
+
+    -   estimator: Linear model classifier object
+    -   X: a data frame of normalized values from developmental dataset
+    -   Y: a vector of sample labels from training data set
+
+    **Yields:**
+
+    -   float: normalized mutual information score
+
+14.  DEV Area Under ROC Curve Score
+
+    `dev_score_roc`
+
+    Calculates the area under the ROC curve score for the DEV predictions.
+
+    **Args:**
+
+    -   estimator: Linear model classifier object
+    -   X: a data frame of normalized values from developmental dataset
+    -   Y: a vector of sample labels from training data set
+
+    **Yields:**
+
+    -   float: AUC ROC score
+
+
+<a id="orgbda21bf"></a>
+
+### Linear model helper functions
+
+1.  dRFE Subfunction
+
+    `regr_fe`
+
+    Iterate over features to by eliminated by step.
+
+    **Args:**
+
+    -   estimator: regressor or classifier linear model object
+    -   X: a data frame of training data
+    -   Y: a vector of sample labels from training data set
+    -   n_features_iter: iterator for number of features to keep loop
+    -   features: a vector of feature names
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+    -   dev_size: developmental test set propotion of training
+    -   SEED: random state
+    -   RANK: Boolean (True or False)
+
+    **Yields:**
+
+    -   list: a list with number of features, r2 score, mean square error, expalined variance, and array of the indices for features to keep
+
+2.  dRFE Step function
+
+    `regr_fe_step`
+
+    Split training data into developmental dataset and apply estimator
+    to developmental dataset, rank features, and conduct feature
+    elimination, single steps.
+
+    **Args:**
+
+    -   estimator: regressor or classifier linear model object
+    -   X: a data frame of training data
+    -   Y: a vector of sample labels from training data set
+    -   n_features_to_keep: number of features to keep
+    -   features: a vector of feature names
+    -   fold: current fold
+    -   out_dir: output directory. default '.'
+    -   dev_size: developmental test set propotion of training
+    -   SEED: random state
+    -   RANK: Boolean (True or False)
+
+    **Yields:**
+
+    -   dict: a dictionary with number of features, r2 score, mean square error, expalined variance, and selected features
 
-setup(**setup_kwargs)
```

