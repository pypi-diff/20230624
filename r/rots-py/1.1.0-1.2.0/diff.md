# Comparing `tmp/rots-py-1.1.0.tar.gz` & `tmp/rots-py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rots-py-1.1.0.tar", last modified: Thu Jun 15 14:23:00 2023, max compression
+gzip compressed data, was "rots-py-1.2.0.tar", last modified: Sat Jun 24 16:17:46 2023, max compression
```

## Comparing `rots-py-1.1.0.tar` & `rots-py-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 14:23:00.094057 rots-py-1.1.0/
--rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     4815 2023-06-15 14:23:00.092056 rots-py-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3018 2023-06-15 14:04:54.000000 rots-py-1.1.0/README.md
--rw-rw-rw-   0        0        0      724 2023-06-15 14:07:22.000000 rots-py-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 14:23:00.094057 rots-py-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 14:22:59.888403 rots-py-1.1.0/src/
--rw-rw-rw-   0        0        0        0 2023-04-18 12:38:29.000000 rots-py-1.1.0/src/__init__.py
--rw-rw-rw-   0        0        0      164 2023-04-18 12:48:35.000000 rots-py-1.1.0/src/__main__.py
--rw-rw-rw-   0        0        0     3101 2023-04-26 17:07:58.000000 rots-py-1.1.0/src/calculateOverlaps1.py
--rw-rw-rw-   0        0        0     2816 2023-04-26 17:08:25.000000 rots-py-1.1.0/src/calculateOverlaps2.py
--rw-rw-rw-   0        0        0     8531 2023-06-14 11:03:17.000000 rots-py-1.1.0/src/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:22:59.895388 rots-py-1.1.0/src/optim_cy/
--rw-rw-rw-   0        0        0      173 2023-06-13 17:42:24.000000 rots-py-1.1.0/src/optim_cy/setup.py
--rw-rw-rw-   0        0        0    11162 2023-06-15 13:24:45.000000 rots-py-1.1.0/src/rots.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:23:00.057860 rots-py-1.1.0/src/rots_py.egg-info/
--rw-rw-rw-   0        0        0     4815 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       78 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 16:17:46.007294 rots-py-1.2.0/
+-rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6228 2023-06-24 16:17:46.005295 rots-py-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4431 2023-06-24 16:12:35.000000 rots-py-1.2.0/README.md
+-rw-rw-rw-   0        0        0      726 2023-06-24 16:12:58.000000 rots-py-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 16:17:46.007294 rots-py-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 16:17:45.392735 rots-py-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 16:17:45.586198 rots-py-1.2.0/src/optim_cy/
+-rw-rw-rw-   0        0        0      542 2023-06-17 21:26:16.000000 rots-py-1.2.0/src/optim_cy/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:17:45.735870 rots-py-1.2.0/src/rots_py.egg-info/
+-rw-rw-rw-   0        0        0     6228 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-24 16:17:45.000000 rots-py-1.2.0/src/rots_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 16:17:46.000295 rots-py-1.2.0/src/rotspy/
+-rw-rw-rw-   0        0        0      108 2023-06-23 15:38:53.000000 rots-py-1.2.0/src/rotspy/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-06-23 15:31:50.000000 rots-py-1.2.0/src/rotspy/__main__.py
+-rw-rw-rw-   0        0        0     3101 2023-04-26 17:07:58.000000 rots-py-1.2.0/src/rotspy/calculateOverlaps1.py
+-rw-rw-rw-   0        0        0     2816 2023-04-26 17:08:25.000000 rots-py-1.2.0/src/rotspy/calculateOverlaps2.py
+-rw-rw-rw-   0        0        0    10374 2023-06-24 16:05:38.000000 rots-py-1.2.0/src/rotspy/helpers.py
+-rw-rw-rw-   0        0        0     2382 2023-06-23 15:38:30.000000 rots-py-1.2.0/src/rotspy/plot_rots.py
+-rw-rw-rw-   0        0        0    11320 2023-06-23 15:40:17.000000 rots-py-1.2.0/src/rotspy/rots.py
```

### Comparing `rots-py-1.1.0/LICENSE` & `rots-py-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rots-py-1.1.0/PKG-INFO` & `rots-py-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rots-py
-Version: 1.1.0
+Version: 1.2.0
 Summary: ROTS gene ranking implementation in Python
 Author-email: "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq" <fmamadbe@abo.fi>
 License: MIT License
         
         Copyright (c) 2023 EDISS-intake2-team4
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,32 +45,38 @@
 # Installation 
 ```
 pip install rots-py
 ```
 
 # Usage
 ```python  
-import rots
+from rotspy import rots, plot_rots, get_summary
 
 # Load data
 data = ...
 group = ...
 
 # Run ROTS
-result = rots.rots(data, group, B=500, log=True, verbose=True, progress=True)
+result = rots(data, group, B=500, log=True, verbose=True, progress=True)
 
 # Get the ranking
 ranking_statistic = result["d"]
 fdr = result["fdr"]
 logFC = result["logfc"]
 pvalue = result["p"]
+
+# Get the summary of result with FDR threshold of 0.05
+summary = get_summary(result, fdr_c=0.05)
+
+# Plot volcano plot from the results
+plot_rots(result, fdr=0.05, type="volcano")
 ```
 
 # Methods
-## rots
+## rots(...)
 Runs the ROTS analysis on the given data. Returns a Python dictionary.
 
 ## Parameters
 - `data`: A pandas dataframe with genes/proteins as rows and samples as columns. (required)
 - `group`: A pandas series with the group labels for each sample. (required)
 - `B`: Number of permutations to perform. Default is 500. (optional)
 - `K`: Top-list size. (optional)
@@ -94,18 +100,57 @@
 - `a2`: Optimized parameter a2
 - `k`: Top list size (*`None` if optimization skipped*)
 - `R`: Reproducibility score (*`None` if optimization skipped*)
 - `Z`: Z-score (*`None` if optimization skipped*)
 - `ztable`: Z-score table
 - `cl`: Group labels for each sample
 
+## get_summary(...)
+Returns a summary of the ROTS results.
+
+## Parameters
+- `rots_res`: The result of the `rots` function. (required)
+- `fdr_c`: The FDR threshold for the summary. Default is `None` (required if `n_features` is not specified)
+- `n_features`: The number of top rows to show in the summary. Default is `None` (required if `fdr` is not specified)
+- `verbose`: Whether to print the summary. Default is `True` (optional)
+
+## Returns
+A pandas dataframe with the following columns:
+- `Row`: The row names of the input dataframe
+- `ROTS Statistic`: The ROTS statistic for each row
+- `pvalue`: The p-value for each row
+- `FDR`: The FDR for each row
+
+## plot(...)
+Plots the ROTS results. 
+
+## Parameters
+- `rots_res`: The result of the `rots` function. (required)
+- `fdr`: The FDR threshold for the plot. Default is `0.05` (required)
+- `type`: The type of plot to generate. (required)
+    - "volcano"
+    - "heatmap"
+    - "ma"
+    - "reproducibility"
+    - "pvalue"
+    - "pca"
+
+
+
 # Acknowledgements
-This package was developed as part of the [EDISS](https://www.master-ediss.eu/) program with the support of Coffey Lab at the [Turku Bioscience](https://bioscience.fi/) center. 
+This package was developed as part of the [EDISS](https://www.master-ediss.eu/) program in collaboration with Coffey Lab at the [Turku Bioscience](https://bioscience.fi/) center.
 
 # Changelog
+## 1.2.0
+- Added `get_summary` function
+- Added `plot_rots` function
+- Modified the import statement to `from rotspy import ...`
+- More optimizations
+- Bug fixes
+
 ## 1.1.0
 - Ported parts of code to Cython for better performance
 - Fixed bugs
 
 ## 1.0.3
 - Bug fixes
```

### Comparing `rots-py-1.1.0/README.md` & `rots-py-1.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,32 +9,38 @@
 # Installation 
 ```
 pip install rots-py
 ```
 
 # Usage
 ```python  
-import rots
+from rotspy import rots, plot_rots, get_summary
 
 # Load data
 data = ...
 group = ...
 
 # Run ROTS
-result = rots.rots(data, group, B=500, log=True, verbose=True, progress=True)
+result = rots(data, group, B=500, log=True, verbose=True, progress=True)
 
 # Get the ranking
 ranking_statistic = result["d"]
 fdr = result["fdr"]
 logFC = result["logfc"]
 pvalue = result["p"]
+
+# Get the summary of result with FDR threshold of 0.05
+summary = get_summary(result, fdr_c=0.05)
+
+# Plot volcano plot from the results
+plot_rots(result, fdr=0.05, type="volcano")
 ```
 
 # Methods
-## rots
+## rots(...)
 Runs the ROTS analysis on the given data. Returns a Python dictionary.
 
 ## Parameters
 - `data`: A pandas dataframe with genes/proteins as rows and samples as columns. (required)
 - `group`: A pandas series with the group labels for each sample. (required)
 - `B`: Number of permutations to perform. Default is 500. (optional)
 - `K`: Top-list size. (optional)
@@ -58,18 +64,57 @@
 - `a2`: Optimized parameter a2
 - `k`: Top list size (*`None` if optimization skipped*)
 - `R`: Reproducibility score (*`None` if optimization skipped*)
 - `Z`: Z-score (*`None` if optimization skipped*)
 - `ztable`: Z-score table
 - `cl`: Group labels for each sample
 
+## get_summary(...)
+Returns a summary of the ROTS results.
+
+## Parameters
+- `rots_res`: The result of the `rots` function. (required)
+- `fdr_c`: The FDR threshold for the summary. Default is `None` (required if `n_features` is not specified)
+- `n_features`: The number of top rows to show in the summary. Default is `None` (required if `fdr` is not specified)
+- `verbose`: Whether to print the summary. Default is `True` (optional)
+
+## Returns
+A pandas dataframe with the following columns:
+- `Row`: The row names of the input dataframe
+- `ROTS Statistic`: The ROTS statistic for each row
+- `pvalue`: The p-value for each row
+- `FDR`: The FDR for each row
+
+## plot(...)
+Plots the ROTS results. 
+
+## Parameters
+- `rots_res`: The result of the `rots` function. (required)
+- `fdr`: The FDR threshold for the plot. Default is `0.05` (required)
+- `type`: The type of plot to generate. (required)
+    - "volcano"
+    - "heatmap"
+    - "ma"
+    - "reproducibility"
+    - "pvalue"
+    - "pca"
+
+
+
 # Acknowledgements
-This package was developed as part of the [EDISS](https://www.master-ediss.eu/) program with the support of Coffey Lab at the [Turku Bioscience](https://bioscience.fi/) center. 
+This package was developed as part of the [EDISS](https://www.master-ediss.eu/) program in collaboration with Coffey Lab at the [Turku Bioscience](https://bioscience.fi/) center.
 
 # Changelog
+## 1.2.0
+- Added `get_summary` function
+- Added `plot_rots` function
+- Modified the import statement to `from rotspy import ...`
+- More optimizations
+- Bug fixes
+
 ## 1.1.0
 - Ported parts of code to Cython for better performance
 - Fixed bugs
 
 ## 1.0.3
 - Bug fixes
```

### Comparing `rots-py-1.1.0/pyproject.toml` & `rots-py-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyproject.toml
 
 [project]
 name = "rots-py"
-version = "1.1.0"
+version = "1.2.0"
 description = "ROTS gene ranking implementation in Python"
 readme = "README.md"
 authors = [{ name = "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq", email = "fmamadbe@abo.fi" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -21,8 +21,8 @@
 ]
 requires-python = ">=3.6"
 
 [project.urls]
 Homepage = "https://github.com/EDISS-intake2-team4/rots-py"
 
 [project.scripts]
-realpython = "rots.__main__:main"
+realpython = "rotspy.__main__:main"
```

### Comparing `rots-py-1.1.0/src/calculateOverlaps1.py` & `rots-py-1.2.0/src/rotspy/calculateOverlaps1.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.1.0/src/calculateOverlaps2.py` & `rots-py-1.2.0/src/rotspy/calculateOverlaps2.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.1.0/src/helpers.py` & `rots-py-1.2.0/src/rotspy/helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from numba import njit, jit
 import pandas as pd
 from tqdm import tqdm
+import warnings
 
 from optim_cy import optim
 
 @jit(nopython=True, error_model='numpy')
 def bootstrapSamples(B, labels, paired):
   samples = np.zeros((B, len(labels)))
   
@@ -34,102 +35,102 @@
   for i in range(B):
     samples[i, :] = np.random.permutation(len(cl))
 
   return samples
 
 
 def testStatistic(paired, samples):
-   # Two groups
-   if len(samples)==2:
-     X = samples[0]
-     Y = samples[1]
-     
-     ## Calculates the test statistic for each row.
-     ## X and Y are the data matrices of the two groups.
-     ## Each row of these two matrices must contain at least TWO not NA values.
-     ## Thus the "variance" always exists.  
-     
-     #ipdb.set_trace(context=6)   ## BREAKPOINT
-
-     ## Row means
-     mX = np.nanmean(X, axis=1, keepdims=True) #rowMeans(X, na.rm=TRUE)
-     mY = np.nanmean(Y, axis=1, keepdims=True) #rowMeans(Y, na.rm=TRUE)
-     
-     #mX[np.isnan(mX)] = 0
-     #mY[np.isnan(mY)] = 0
-
-     ## Pooled standard deviations for each row
-     sX = np.nansum((X - mX)**2, axis=1) #rowSums((X - mX)^2, na.rm=TRUE)
-     sY = np.nansum((Y - mY)**2, axis=1) #rowSums((Y - mY)^2, na.rm=TRUE)
-
-     #sX[np.isnan(sX)] = 0
-     #sY[np.isnan(sY)] = 0
-     
-     if not paired:
-       ## Number of not NA values in each row
-       nX = np.sum(~np.isnan(X), axis=1)
-       nY = np.sum(~np.isnan(Y), axis=1)             
-
-       ## d == difference between the group means for each row (==gene)
-       ## s == pooled standard deviation for each row (==gene)        
-       d = mY - mX
-       s = np.sqrt(((sX + sY) / (nX + nY - 2)) * (1 / nX + 1 / nY))
-       
-       ## Cases with less than two non-missing values.
-       ## Set d = 0, s = 1
-       ind = np.where( (nY < 2) | (nX < 2) )
-       d[ind] = 0
-       s[ind] = 1
-     
-     
-     if paired:
-       ## Add for paired
-       sXY = np.nansum((X - mX)*(Y - mY), axis=1)
-       
-       ## Number of not NA values in each row
-       n = np.sum(~np.isnan(X*Y), axis=1)
-       
-       ## d == difference between the group means for each row (==gene)
-       ## s == pooled standard deviation for each row (==gene)        
-       d = mY - mX
-       s = np.sqrt(((sX + sY) / (n + n - 2)) * (2 / n) - 2/(n*n-n)*sXY)
-       
-       ## Cases with less than two non-missing values.
-       ## Set d = 0, s = 1
-       ind = np.where( n < 2 )
-       d[ind] = 0
-       s[ind] = 1
-     
-     return  {'d': d.reshape(-1), 's': s.reshape(-1)}
+  np.seterr(divide='ignore', invalid='ignore')
+  # Two groups
+  if len(samples)==2:
+    X = samples[0]
+    Y = samples[1]
+    
+    ## Calculates the test statistic for each row.
+    ## X and Y are the data matrices of the two groups.
+    ## Each row of these two matrices must contain at least TWO not NA values.
+    ## Thus the "variance" always exists.      
+
+    with warnings.catch_warnings():
+      warnings.simplefilter("ignore", category=RuntimeWarning)      
+      ## Row means
+      mX = np.nanmean(X, axis=1, keepdims=True) #rowMeans(X, na.rm=TRUE)
+      mY = np.nanmean(Y, axis=1, keepdims=True) #rowMeans(Y, na.rm=TRUE)
+    
+    #mX[np.isnan(mX)] = 0
+    #mY[np.isnan(mY)] = 0
+
+    ## Pooled standard deviations for each row
+    sX = np.nansum((X - mX)**2, axis=1) #rowSums((X - mX)^2, na.rm=TRUE)
+    sY = np.nansum((Y - mY)**2, axis=1) #rowSums((Y - mY)^2, na.rm=TRUE)
+
+    #sX[np.isnan(sX)] = 0
+    #sY[np.isnan(sY)] = 0
+    
+    if not paired:
+      ## Number of not NA values in each row
+      nX = np.sum(~np.isnan(X), axis=1)
+      nY = np.sum(~np.isnan(Y), axis=1)             
+
+      ## d == difference between the group means for each row (==gene)
+      ## s == pooled standard deviation for each row (==gene)        
+      d = mY - mX
+      s = np.sqrt(((sX + sY) / (nX + nY - 2)) * (1 / nX + 1 / nY))
+      
+      ## Cases with less than two non-missing values.
+      ## Set d = 0, s = 1
+      ind = np.where( (nY < 2) | (nX < 2) )
+      d[ind] = 0
+      s[ind] = 1      
+    
+    if paired:
+      ## Add for paired
+      sXY = np.nansum((X - mX)*(Y - mY), axis=1)
+      
+      ## Number of not NA values in each row
+      n = np.sum(~np.isnan(X*Y), axis=1)
+      
+      ## d == difference between the group means for each row (==gene)
+      ## s == pooled standard deviation for each row (==gene)        
+      d = mY - mX
+      s = np.sqrt(((sX + sY) / (n + n - 2)) * (2 / n) - 2/(n*n-n)*sXY)
+      
+      ## Cases with less than two non-missing values.
+      ## Set d = 0, s = 1
+      ind = np.where( n < 2 )
+      d[ind] = 0
+      s[ind] = 1
+    
+    return  {'d': d.reshape(-1), 's': s.reshape(-1)}
    
-   # Multiple groups
-   if len(samples)>2:
-     
-     samples_all = np.concatenate(samples, axis=1) # do.call("cbind",samples)
-     
-     if not paired:
-       sum_cols = np.sum([sample.shape[1] for sample in samples])
-       prod_cols = np.prod([sample.shape[1] for sample in samples])
-       f = sum_cols / prod_cols #f <- sum(sapply(samples, ncol)) / prod(sapply(samples, ncol))
-
-       r = np.zeros(samples_all.shape[0]) #r <- vector(mode="numeric", length=nrow(samples.all))
-       for k in range(len(samples)):
-         r = r + (np.nanmean(samples[k], axis=1)-np.nanmean(samples_all, axis=1))**2 #r <- r + (rowMeans(samples[[k]], na.rm=TRUE)-rowMeans(samples.all, na.rm=TRUE))^2       
-       d = (f*r)**0.5
-       
-       f = 1/np.sum([sample.shape[1] for sample in samples]-1) * np.sum(1/[sample.shape[1] for sample in samples]) #f <- 1/sum(sapply(samples, ncol)-1) * sum(1/sapply(samples, ncol))
-       s = np.zeros(samples_all.shape[0])  # s <- vector(mode="numeric", length=nrow(samples.all))
-       for k in range(len(samples)):
-         s = s + np.sum(np.apply_along_axis(lambda x: (x - np.nanmean(x))**2, axis=1, arr=samples[k,:]), axis=0, where=~np.isnan(samples[k,:]).any(axis=0)) #s <- s + colSums(apply(samples[[k]], 1, function(x) (x-mean(x,na.rm=TRUE))^2), na.rm=TRUE)       
-       s = (f*s)**0.5       
-     
-     if paired:
-       raise ValueError("Multiple paired groups not supported!")     
-     
-     return {'d': d.reshape(-1), 's': s.reshape(-1)}
+  # Multiple groups
+  if len(samples)>2:
+    
+    samples_all = np.concatenate(samples, axis=1) # do.call("cbind",samples)
+    
+    if not paired:
+      sum_cols = np.sum([sample.shape[1] for sample in samples])
+      prod_cols = np.prod([sample.shape[1] for sample in samples])
+      f = sum_cols / prod_cols #f <- sum(sapply(samples, ncol)) / prod(sapply(samples, ncol))
+
+      r = np.zeros(samples_all.shape[0]) #r <- vector(mode="numeric", length=nrow(samples.all))
+      for k in range(len(samples)):
+        r = r + (np.nanmean(samples[k], axis=1)-np.nanmean(samples_all, axis=1))**2 #r <- r + (rowMeans(samples[[k]], na.rm=TRUE)-rowMeans(samples.all, na.rm=TRUE))^2       
+      d = (f*r)**0.5
+      
+      f = 1/np.sum([sample.shape[1] for sample in samples]-1) * np.sum(1/[sample.shape[1] for sample in samples]) #f <- 1/sum(sapply(samples, ncol)-1) * sum(1/sapply(samples, ncol))
+      s = np.zeros(samples_all.shape[0])  # s <- vector(mode="numeric", length=nrow(samples.all))
+      for k in range(len(samples)):
+        s = s + np.sum(np.apply_along_axis(lambda x: (x - np.nanmean(x))**2, axis=1, arr=samples[k,:]), axis=0, where=~np.isnan(samples[k,:]).any(axis=0)) #s <- s + colSums(apply(samples[[k]], 1, function(x) (x-mean(x,na.rm=TRUE))^2), na.rm=TRUE)       
+      s = (f*s)**0.5       
+    
+    if paired:
+      raise ValueError("Multiple paired groups not supported!")     
+    
+    return {'d': d.reshape(-1), 's': s.reshape(-1)}
 
 def calculateP(observed, permuted):  
   # Store order for later use
   observed_order = sorted(range(len(observed)), key=lambda k: abs(observed[k]), reverse=True) # order(abs(observed), decreasing=TRUE)
   
   # Sort observed and permuted values
   observed = -np.sort(-abs(observed)) #sort(abs(observed), decreasing=TRUE)
@@ -151,31 +152,31 @@
 
 def calculateFDR(observed, permuted, progress):
   observed = abs(observed)
   permuted = abs(permuted)
   ord = np.argsort(-observed, kind='mergesort') #order(observed, decreasing=TRUE, na.last=TRUE)
   a = observed[ord]
   
-  A = np.empty((len(a), permuted.shape[1])) #matrix(NA, nrow=length(a), ncol=ncol(permuted))
-  A[:] = np.nan
+  A = np.empty((len(a), permuted.shape[1]))
+  A.fill(np.nan)
   if progress:
-    pb = tqdm(total=A.shape[1]) #txtProgressBar(min=0, max=ncol(A), style=3)
+    pb = tqdm(total=A.shape[1])
   for i in range(A.shape[1]): #seq_len(ncol(A))
     sorted_column = np.sort(permuted[:,i])[::-1] #sort(permuted[,i], decreasing=TRUE, na.last=TRUE)
     a_rand = np.concatenate([sorted_column[~np.isnan(sorted_column)], sorted_column[np.isnan(sorted_column)]])
     n_bigger = biggerN(a, a_rand)
     A[ord,i] = n_bigger/range(1, len(a)+1)
     if progress:
       pb.update()      
 
   if progress:
     pb.close()
   
   
-  FDR = np.apply_along_axis(np.median, 1, A) #apply(A, 1, median)
+  FDR = np.apply_along_axis(np.median, 1, A)
   FDR[FDR>1] = 1
   FDR[ord] = list(reversed([min(FDR[ord][x-1:]) for x in range(len(FDR), 0, -1)])) #rev(sapply(length(FDR):1, function(x) return(min(FDR[ord][x:length(FDR)]))))
 
   return FDR
 
 
 def biggerN(x, y):  
@@ -210,8 +211,54 @@
 
   j = 0
   for i in range(len(observed)):
     while permuted[j] >= observed[i] and j < len(permuted):
       j += 1
     pvalues[i] = float(j) / len(permuted)
 
-  return pvalues.reshape(a.shape)
+  return pvalues.reshape(a.shape)
+
+def get_summary(rots_res, fdr_c=None, n_genes=None, verbose=True):
+  if fdr_c is not None or n_genes is not None:
+    ## Sort ROTS-statistic values (abs)
+    stat = pd.DataFrame(np.abs(rots_res['d']), index=rots_res['data'].index, columns=['statistic'])    
+    sorted_stat = stat.sort_values(by='statistic', ascending=False)
+
+    ## Add feature-names to fdr and ROTS values
+    fdr = pd.DataFrame(rots_res['FDR'], index=rots_res['data'].index)    
+    d = pd.DataFrame(rots_res['d'], index=rots_res['data'].index)    
+    pvalue = pd.DataFrame(rots_res['p'], index=rots_res['data'].index)    
+
+    ## Result matrix, columns are: "Row", "ROTS-statistic", "pvalue" and "FDR" 
+    res = pd.DataFrame(
+      data={
+        'Row': sorted_stat.index, 
+        'ROTS-statistic': d.loc[sorted_stat.index][0], 
+        'pvalue': pvalue.loc[sorted_stat.index][0], 
+        'FDR': fdr.loc[sorted_stat.index][0]})
+    
+    ## Show only num.gene top rows or rows whose false discovery rate <= fdr
+    if n_genes is not None:
+      res = res.iloc[: min(n_genes, len(res))]
+    elif fdr_c is not None:
+      res = res[res['FDR'] <= fdr_c]
+
+    if verbose:
+      print("ROTS results:", "\n")
+      print("Number of resamplings: ", rots_res["B"], "\n")
+      print("a1:                    ", rots_res["a1"])
+      print("a2:                    ", rots_res["a2"])
+      print("Top list size:         ", rots_res["k"])
+      print("Reproducibility value: ", rots_res["R"])
+      print("Z-score:               ", rots_res["Z"], "\n")
+
+      print(len(res), "rows satisfy the condition.")
+      ## Print only the first 10 rows
+      if len(res) > 10:
+          print(" Only ten first rows are", "\n",
+                "displayed, see the return value for the whole output.")
+          print(res[:10])
+          print("...")
+      else:          
+          print(res)
+
+    return res
```

### Comparing `rots-py-1.1.0/src/rots.py` & `rots-py-1.2.0/src/rotspy/rots.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #import ipdb
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 import random
 
-from helpers import bootstrapSamples, permutatedSamples, testStatistic, calculateP, calculateFDR
-from calculateOverlaps1 import calculateOverlaps1
-from calculateOverlaps2 import calculateOverlaps2
+from rotspy.helpers import bootstrapSamples, permutatedSamples, testStatistic, calculateP, calculateFDR
+#from calculateOverlaps1 import calculateOverlaps1
+#from calculateOverlaps2 import calculateOverlaps2
 from optim_cy import optim
 
 def rots(data, groups, B=500, K=None, paired=False, seed=None, a1=None, a2=None, log=False, progress=False, verbose=True):
   #if isinstance(data, pd.DataFrame):
   #  data_val = data.values    
   
   ## Set random number generator seed for reproducibility
@@ -34,14 +34,16 @@
   ))
   N = np.concatenate([
     np.arange(1, 21) * 5,
     np.arange(11, 51) * 10,
     np.arange(21, 41) * 25, 
     np.arange(11, 1001) * 100
   ])
+
+  ssq = np.array(["%.2f" % x for x in ssq])
     
   ## Check for top list size K
   if K is None:
     K = data.shape[0] // 4
     if (verbose):
       print("No top list size K given, using ", K)
 
@@ -53,15 +55,15 @@
   if isinstance(groups[0], str):
     groups = pd.factorize(groups)[0]
     groups_levels = pd.factorize(groups)[1]
   else:
     groups_levels = None
 
   ## Reorder the data according to the group labels and check for NA rows.
-  data = data.iloc[:, np.argsort(groups)]
+  data = data.iloc[:, np.argsort(groups, kind='mergesort')]
   groups = np.sort(groups)
   
   for i in np.unique(groups):
     if np.any(np.sum(np.isnan(data.iloc[:, np.where(groups == i)[0]]), axis=1) >= len(np.where(groups == i)[0]) - 1):
       if groups_levels is None:
         target = i
       else:
@@ -89,15 +91,15 @@
 
   ## Bootstrap samples
   if (verbose): 
     print("Bootstrapping samples")    
 
   samples = bootstrapSamples(2*B, cl, paired)
   ## Permutated samples
-  pSamples = permutatedSamples(len(samples), cl)
+  pSamples = permutatedSamples(samples.shape[0], cl)
 
   ## Test statistics in the bootstrap (permutate) datasets.
   ## For each bootstrap (permutated) dataset, determine the signal log-ratio
   ## (D) and the standard error (S).
   D = np.empty((data.shape[0], samples.shape[0]))
   S = np.empty((data.shape[0], samples.shape[0]))
   pD = np.empty((data.shape[0], samples.shape[0]))
@@ -114,19 +116,20 @@
     ## If a1 and a2 parameters are given, we don't need the bootstrap
     ## dataset
     if a1 == None or a2 == None:
       fit = testStatistic(paired, [data.iloc[:, x].to_numpy() for x in samples_R])
       D[:,i] = fit['d']
       S[:,i] = fit['s']
     
-      
+
     pFit = testStatistic(paired, [data.iloc[:, x].to_numpy() for x in pSamples_R])
     pD[:,i] = pFit['d']
-    pS[:,i] = pFit['s']
-    
+    pS[:,i] = pFit['s']        
+
+    #assert False, "STOP"  
     if progress: 
       pb.update()
     
   if progress: 
     pb.close()
 
   ## ---------------------------------------------------------------------------
@@ -167,31 +170,31 @@
       ## bootrsrap samples and columns corrospond to different top list size.
       ## Repeat for each parameter combination a1 and a2.
       overlaps = np.zeros((B,len(N)))
       overlaps_P = np.zeros((B,len(N)))      
 
       
       cResults = optim.calculateOverlaps1(D, S, pD, pS, len(D), N.astype(int), len(N),
-                        ssq[i], int(B), overlaps, overlaps_P)
+                        float(ssq[i]), int(B), overlaps, overlaps_P)            
       
       ## Colmeans & rowMeans are a lot faster than apply
       #         reprotable[i, ] <- colMeans(overlaps)
       #         reprotable.P[i, ] <- colMeans(overlaps.P)            
       reprotable.iloc[i] = np.mean(cResults["overlaps"], axis=0)
       reprotable_P.iloc[i] = np.mean(cResults["overlaps_P"], axis=0)
       
       ## Standard deviation for each column
       ## same as reprotable.sd[i, ] <- apply(overlaps, 2, sd)
       ## or just sd(overlaps), but a lot faster.
       #         reprotable.sd[i,] <- sqrt(rowSums((t(overlaps) - reprotable[i,])^2) /
       #                                     (nrow(overlaps) - 1))
       #sqrt(rowSums((t(cResults[["overlaps"]]) - reprotable[i,])^2) / (nrow(cResults[["overlaps"]]) - 1)) 
-      #reprotable_sd.iloc[i] = np.std(cResults["overlaps"])
-      reprotable_sd.iloc[i] = np.sqrt(np.sum((cResults["overlaps"].T - reprotable.iloc[i].values[0])**2, axis=1) / 
-                                      (cResults["overlaps"].shape[0] - 1))[0]
+      reprotable_sd.iloc[i] = np.std(cResults["overlaps"], axis=0)
+      #reprotable_sd.iloc[i] = np.sqrt(np.sum((cResults["overlaps"] - reprotable.iloc[i].values)**2, axis=0) / 
+      #                                (cResults["overlaps"].shape[0] - 1))
       
       if progress:
         pb.update()      
 
     if progress: 
       pb.close()
 
@@ -204,45 +207,46 @@
 
     #ipdb.set_trace(context=6)   ## BREAKPOINT
     
     reprotable.iloc[i] = np.mean(cResults["overlaps"], axis=0) 
     reprotable_P.iloc[i] = np.mean(cResults["overlaps_P"], axis=0)
     ## Standard deviation for each column
     #sqrt(rowSums((t(cResults[["overlaps"]]) - reprotable[i,])^2) / (nrow(cResults[["overlaps"]]) - 1))
-    #reprotable_sd.iloc[i] = np.std(cResults["overlaps"])
-    reprotable_sd.iloc[i] = np.sqrt(np.sum((cResults["overlaps"].T - reprotable.iloc[i].values[0])**2, axis=1) / 
-                                      (cResults["overlaps"].shape[0] - 1))[0]
+    reprotable_sd.iloc[i] = np.std(cResults["overlaps"], axis=0)
+    #reprotable_sd.iloc[i] = np.sqrt(np.sum((cResults["overlaps"] - reprotable.iloc[i].values)**2, axis=0) / 
+    #                                  (cResults["overlaps"].shape[0] - 1))
 
     ## -------------------------------------------------------------------------
 
     ## Calculate the Z-statistic and find the top list size and the
     ## (a1,a2)-combination giving the maximal Z-value
     ## Rownames of ztable are c(ssq, "slr") and colnames are N
     ztable = (reprotable - reprotable_P) / reprotable_sd    
     ztable = ztable.infer_objects()    
     
-    sel = np.unravel_index(np.argmax(ztable[np.isfinite(ztable)]), ztable.shape) #np.where(ztable == max(ztable[is.finite(ztable)]), arr.ind=TRUE)
+    indices = np.where(ztable == np.nanmax(ztable[np.isfinite(ztable)]))
+    sel = list(zip(indices[0], indices[1]))#np.unravel_index(np.argmax(ztable[np.isfinite(ztable)]), ztable.shape)
     ## Sel is a matrix containing the location(s) of the largest value (row,
     ## col). If the location of the largest value is not unique then nrow(sel)
     ## > 2 (length(sel) > 2)
     
-    if len(sel) > 2:
-      sel = sel[0:2]
+    if len(sel) > 1:
+      sel = [sel[0]]
 
-    if sel[0] < len(reprotable)-1:
-      a1 = float(reprotable.index[sel[0]])
+    if sel[0][0] < reprotable.shape[0]-1:
+      a1 = float(reprotable.index[sel[0][0]])
       a2 = 1
     
-    if sel[0] == len(reprotable)-1:
+    if sel[0][0] == reprotable.shape[0]-1:
       a1 = 1
       a2 = 0
     
-    k = int(reprotable.columns[sel[1]])
-    R = reprotable.iloc[sel[0],sel[1]]
-    Z = ztable.iloc[sel[0],sel[1]]
+    k = int(reprotable.columns[sel[0][1]])
+    R = reprotable.iloc[sel[0][0],sel[0][1]]
+    Z = ztable.iloc[sel[0][0],sel[0][1]]
    
     ## Calculate the reproducibility-optimized test statistic based on the
     ## reproducibility-maximizing a1, a2 and k values and the corresponding FDR      
     #fit = testStatistic(paired, lapply(split(1:len(cl), cl), function(x) data[:,x]))
     fit = testStatistic(paired, np.split(data.to_numpy(), np.where(np.diff(cl) != 0)[0] + 1, axis=1))
     d = fit['d'] / (a1 + a2 * fit['s'])
     pD = pD/(a1 + a2 * pS)
@@ -253,17 +257,14 @@
     if verbose: 
       print("Calculating p-values")
     p = calculateP(d, pD)
     
     if verbose:
       print("Calculating FDR")
     FDR = calculateFDR(d, pD, progress)
-    
-    ## Free up memory
-    #del pD
 
     ROTS_output = {
       "data": data,
       "B": B,
       "d": d,
       "logfc": logfc,
       "p": p,
```

### Comparing `rots-py-1.1.0/src/rots_py.egg-info/PKG-INFO` & `rots-py-1.2.0/src/rots_py.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rots-py
-Version: 1.1.0
+Version: 1.2.0
 Summary: ROTS gene ranking implementation in Python
 Author-email: "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq" <fmamadbe@abo.fi>
 License: MIT License
         
         Copyright (c) 2023 EDISS-intake2-team4
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,32 +45,38 @@
 # Installation 
 ```
 pip install rots-py
 ```
 
 # Usage
 ```python  
-import rots
+from rotspy import rots, plot_rots, get_summary
 
 # Load data
 data = ...
 group = ...
 
 # Run ROTS
-result = rots.rots(data, group, B=500, log=True, verbose=True, progress=True)
+result = rots(data, group, B=500, log=True, verbose=True, progress=True)
 
 # Get the ranking
 ranking_statistic = result["d"]
 fdr = result["fdr"]
 logFC = result["logfc"]
 pvalue = result["p"]
+
+# Get the summary of result with FDR threshold of 0.05
+summary = get_summary(result, fdr_c=0.05)
+
+# Plot volcano plot from the results
+plot_rots(result, fdr=0.05, type="volcano")
 ```
 
 # Methods
-## rots
+## rots(...)
 Runs the ROTS analysis on the given data. Returns a Python dictionary.
 
 ## Parameters
 - `data`: A pandas dataframe with genes/proteins as rows and samples as columns. (required)
 - `group`: A pandas series with the group labels for each sample. (required)
 - `B`: Number of permutations to perform. Default is 500. (optional)
 - `K`: Top-list size. (optional)
@@ -94,18 +100,57 @@
 - `a2`: Optimized parameter a2
 - `k`: Top list size (*`None` if optimization skipped*)
 - `R`: Reproducibility score (*`None` if optimization skipped*)
 - `Z`: Z-score (*`None` if optimization skipped*)
 - `ztable`: Z-score table
 - `cl`: Group labels for each sample
 
+## get_summary(...)
+Returns a summary of the ROTS results.
+
+## Parameters
+- `rots_res`: The result of the `rots` function. (required)
+- `fdr_c`: The FDR threshold for the summary. Default is `None` (required if `n_features` is not specified)
+- `n_features`: The number of top rows to show in the summary. Default is `None` (required if `fdr` is not specified)
+- `verbose`: Whether to print the summary. Default is `True` (optional)
+
+## Returns
+A pandas dataframe with the following columns:
+- `Row`: The row names of the input dataframe
+- `ROTS Statistic`: The ROTS statistic for each row
+- `pvalue`: The p-value for each row
+- `FDR`: The FDR for each row
+
+## plot(...)
+Plots the ROTS results. 
+
+## Parameters
+- `rots_res`: The result of the `rots` function. (required)
+- `fdr`: The FDR threshold for the plot. Default is `0.05` (required)
+- `type`: The type of plot to generate. (required)
+    - "volcano"
+    - "heatmap"
+    - "ma"
+    - "reproducibility"
+    - "pvalue"
+    - "pca"
+
+
+
 # Acknowledgements
-This package was developed as part of the [EDISS](https://www.master-ediss.eu/) program with the support of Coffey Lab at the [Turku Bioscience](https://bioscience.fi/) center. 
+This package was developed as part of the [EDISS](https://www.master-ediss.eu/) program in collaboration with Coffey Lab at the [Turku Bioscience](https://bioscience.fi/) center.
 
 # Changelog
+## 1.2.0
+- Added `get_summary` function
+- Added `plot_rots` function
+- Modified the import statement to `from rotspy import ...`
+- More optimizations
+- Bug fixes
+
 ## 1.1.0
 - Ported parts of code to Cython for better performance
 - Fixed bugs
 
 ## 1.0.3
 - Bug fixes
```

