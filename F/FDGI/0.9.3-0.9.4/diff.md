# Comparing `tmp/FDGI-0.9.3.tar.gz` & `tmp/FDGI-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FDGI-0.9.3.tar", last modified: Fri Feb 17 02:10:15 2023, max compression
+gzip compressed data, was "FDGI-0.9.4.tar", last modified: Fri Jun 23 23:50:18 2023, max compression
```

## Comparing `FDGI-0.9.3.tar` & `FDGI-0.9.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:10:15.365854 FDGI-0.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:10:15.365854 FDGI-0.9.3/FDGI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-02-17 02:10:15.000000 FDGI-0.9.3/FDGI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-17 02:10:15.000000 FDGI-0.9.3/FDGI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 02:10:15.000000 FDGI-0.9.3/FDGI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-17 02:10:15.000000 FDGI-0.9.3/FDGI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-17 02:10:15.000000 FDGI-0.9.3/FDGI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-17 02:10:06.000000 FDGI-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-02-17 02:10:15.365854 FDGI-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-02-17 02:10:06.000000 FDGI-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-17 02:10:06.000000 FDGI-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-17 02:10:15.365854 FDGI-0.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:10:15.365854 FDGI-0.9.3/spook/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-17 02:10:06.000000 FDGI-0.9.3/spook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-02-17 02:10:06.000000 FDGI-0.9.3/spook/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-02-17 02:10:06.000000 FDGI-0.9.3/spook/contraction_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-02-17 02:10:06.000000 FDGI-0.9.3/spook/lin_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-02-17 02:10:06.000000 FDGI-0.9.3/spook/quad_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-02-17 02:10:06.000000 FDGI-0.9.3/spook/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-02-17 02:10:06.000000 FDGI-0.9.3/spook/vmi_special.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:50:18.380570 FDGI-0.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:50:18.380570 FDGI-0.9.4/FDGI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-06-23 23:50:18.000000 FDGI-0.9.4/FDGI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-23 23:50:18.000000 FDGI-0.9.4/FDGI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:50:18.000000 FDGI-0.9.4/FDGI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 23:50:18.000000 FDGI-0.9.4/FDGI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 23:50:18.000000 FDGI-0.9.4/FDGI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-23 23:50:09.000000 FDGI-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-06-23 23:50:18.380570 FDGI-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-06-23 23:50:09.000000 FDGI-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-23 23:50:09.000000 FDGI-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-23 23:50:18.380570 FDGI-0.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:50:18.380570 FDGI-0.9.4/spook/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-23 23:50:09.000000 FDGI-0.9.4/spook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-06-23 23:50:09.000000 FDGI-0.9.4/spook/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-23 23:50:09.000000 FDGI-0.9.4/spook/contraction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-06-23 23:50:09.000000 FDGI-0.9.4/spook/lin_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10867 2023-06-23 23:50:09.000000 FDGI-0.9.4/spook/quad_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-06-23 23:50:09.000000 FDGI-0.9.4/spook/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-06-23 23:50:09.000000 FDGI-0.9.4/spook/vmi_special.py
```

### Comparing `FDGI-0.9.3/FDGI.egg-info/PKG-INFO` & `FDGI-0.9.4/FDGI.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: FDGI
-Version: 0.9.3
-Summary: A package for frequency-domain ghost imaging
+Version: 0.9.4
+Summary: A package for spectral-domain ghost imaging
 Home-page: https://github.com/congzlwag/spook
 Author: Jun Wang
 Author-email: junwang9@stanford.edu
 Project-URL: Bug Tracker, https://github.com/congzlwag/spook/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,33 +17,31 @@
 
 ## Target Problem
 Solve <img src="https://render.githubusercontent.com/render/math?math=(A \otimes G)X = B"> in the least-square way, under [regularizations](#Regularizations). A, G are matrices acting on the two dimensions of X, i.e. 
 ![(AG)X=B](https://latex.codecogs.com/svg.latex?\normalsize&space;\sum_{w,b}A_{iw}G_{bq}X_{wb}=B_{iq}) .
 For spectral-domain ghost imaging, the dimension indexed by <img src="https://render.githubusercontent.com/render/math?math=w"> is photon energy, and the other dimension can be properties of the photoproduct, such as the electron kinetic energy.
 
 `G` is the (optional) linear operator on the dimension indexed by <img src="https://render.githubusercontent.com/render/math?math=b">. By default (`G=None`), it is the identity, in which case this is the conventional Spooktroscopy, i.e. to solve <img src="https://render.githubusercontent.com/render/math?math=AX=B"> under regularizations. 
-`G` can accommodate other linear operations on the $b$ dimension, to solve the two linear inversions in one step. With `mode='raw'`, pass in matrix ![G](https://latex.codecogs.com/svg.latex?\normalsize&space;G_{bq}) to G, and with `mode='contracted'`, pass in matrix ![GtG](https://latex.codecogs.com/svg.latex?\normalsize&space;\sum_qG_{bq}G_{b'q}). For example, for Abel transform in Velocity Map Imaging, [pBasex](https://github.com/e-champenois/CPBASEX) offers this G with `loadG`.
+`G` can accommodate other linear operations on the $b$ dimension, to solve the two linear inversions in one step. 
+
+With `mode='raw'`, pass in matrix $G_{bq}$ to G, and with `mode='contracted'`, pass in matrix $\sum_qG_{bq}G_{b'q}$. For example, for Abel transform in Velocity Map Imaging, [pBasex](https://github.com/e-champenois/CPBASEX) offers this G with `loadG`.
 
 ### Key Advantages
 The key advantages of this package are
 1. Efficient optimization: Contraction over shots is decoupled from optimization. It is **recommended** to input precontracted results when instantiating, or to save the caches using method `save_prectr` of a solver created with raw inputs. Once instantiated, the precontracted results are cached to be reused every time solving with a different hyperparameter. See `spook.contraction_utils.adaptive_contraction` .
 2. Support dimension reduction on the dependent variable B, through basis functions in G. In that case, it is also recommended to contract (B,G) over the dependent variable space (index q) prior to instantiating a spook solver.
 3. Support multiple combinations of regularizations. See [Solvers](#Solvers) .
 4. Support time-dependent measurement (Beta): when each entry in the raw input A is a pair of (photon spectrum, delay bin), index w is the flattened axis of (<img src="https://render.githubusercontent.com/render/math?math=\omega">, <img src="https://render.githubusercontent.com/render/math?math=\tau">). In this case, the third smoothness hyperparameter is for the delay axis.
 
 At the very bottom level, this package depends on either [OSQP](https://osqp.org) to solve a quadratic programming or LAPACK gesv through `numpy.linalg.solve` . 
 
-### Regularizations
-Common regularizations are the following three types, all of which optional, depending on what _a prior_ knowledge one wants to enforce on the problem solving.
+## Installation
+The stable version is on PyPI. Unfortunately in a different name.
 
-1. Nonnegativity: To constrain <img src="https://render.githubusercontent.com/render/math?math=X\succeq 0">
-2. Sparsity: To penalize on <img src="https://render.githubusercontent.com/render/math?math=\|X\|_1"> or <img src="https://render.githubusercontent.com/render/math?math=\|X\|_2^2">
-3. Smoothness: To penalize on roughness of X , along the two indices, independently. For <img src="https://render.githubusercontent.com/render/math?math=\omega">-axis, which is the photon energy axis, the form is fixed <img src="https://render.githubusercontent.com/render/math?math=\|(L_{N_w}\otimes I)X\|_2^2"> where <img src="https://render.githubusercontent.com/render/math?math=L_{N_w}"> is the [laplacian](https://en.wikipedia.org/wiki/Laplace_operator). Roughness along the second axis of X is customizable through parameter `Bsmoother`, which by default is laplacian squared too.
-
-Sparsity and Smoothness are enforced through penalties in the total obejctive function, and the penalties are weighted by hyperparameters `lsparse` and `lsmooth`. `lsmooth` is a 2-tuple that weight roughness penalty along the two axes of X respectively. The hyperparameters can be passed in during instantiation and also updated afterwards. It is recommended to call method `getXopt` with the hyperparameter(s) to be updated, because it will update, solve, and return the optimal X in one step. Calling `solve` with  the hyperparameter(s) to be updated and then calling `getXopt()` without input is effectively the same, and the problem will be solved once as long as there is no update.
+    pip install FDGI
 
 ## Solvers
 
 Different combinations of regularizations can lead to different forms of objective function. Solvers in package always formalize the specific problem into either a [Quadratic Programming](https://en.wikipedia.org/wiki/Quadratic_programming) or a linear equation. Examples can be found in [unit tests](#UnitTests) 
 
 | Nonnegativity | Sparsity            | Smoothness | Solver              | Notes                                                        |
 | ------------- | ------------------- | ---------- | ------------------- | ------------------------------------------------------------ |
@@ -51,39 +49,47 @@
 | True          | L2 squared          | Quadratic  | `SpookPosL2` |                                                              |
 | False         | L2 squared or False | Quadratic  | `SpookLinSolve`     | This solver is so far the work-horse for SpookVMI            |
 | False         | L1                  | Quadratic  | `SpookL1` |                                                              |
 
 
 ### Quadratic Programming
 
-For cases where it can be formalized into a [Quadratic Programming](https://en.wikipedia.org/wiki/Quadratic_programming) , [OSQP](https://osqp.org) does the job. Thus the root numerical method is alternating direction method of multipliers (ADMM). Looking into the [solver settings of OSQP](https://osqp.org/docs/interfaces/solver_settings.html) is always encouraged, but the default settings usually work fine for `spook` . If one needs to pass in settings, the OSQP solver is `SpookQPBase._prob` .
+For cases where it can be formalized into a [Quadratic Programming](https://en.wikipedia.org/wiki/Quadratic_programming) , [OSQP](https://osqp.org) is the weight-lifter. The root numerical method is the alternating direction method of multipliers (ADMM). Looking into the [solver settings of OSQP](https://osqp.org/docs/interfaces/solver_settings.html) is always encouraged, but the default settings usually work fine for `spook` . If one needs to pass in settings, use `spk._prob.update_settings(**osqp_kwargs)` on your solver instance `spk`. 
 
 ### Linear Equation
 
 A rare case that it can be formalized into a linear equation is the third line in the table above: no nonnegativity constraint, and the sparsity is L2 norm squared. This is implemented in `SpookLinSolve` , which calls `numpy.linalg.solve` or `scipy.sparse.linalg.spsolve` .
 
+### Regularizations
+Common regularizations are the following three types, all of which optional, depending on what _a prior_ knowledge one wants to enforce on the problem solving.
+
+1. Nonnegativity: To constrain <img src="https://render.githubusercontent.com/render/math?math=X\succeq 0">
+2. Sparsity: To penalize on <img src="https://render.githubusercontent.com/render/math?math=\|X\|_1"> or <img src="https://render.githubusercontent.com/render/math?math=\|X\|_2^2">
+3. Smoothness: To penalize on roughness of X , along the two indices, independently. For <img src="https://render.githubusercontent.com/render/math?math=\omega">-axis, which is the photon energy axis, the form is fixed <img src="https://render.githubusercontent.com/render/math?math=\|(L_{N_w}\otimes I)X\|_2^2"> where <img src="https://render.githubusercontent.com/render/math?math=L_{N_w}"> is the [laplacian](https://en.wikipedia.org/wiki/Laplace_operator). Roughness along the second axis of X is customizable through parameter `Bsmoother`, which by default is laplacian squared too.
+
+Sparsity and Smoothness are enforced through penalties in the total obejctive function, and the penalties are weighted by hyperparameters `lsparse` and `lsmooth`. `lsmooth` is a 2-tuple that weight roughness penalty along the two axes of X respectively. The hyperparameters can be passed in during instantiation and also updated afterwards. It is recommended to call method `getXopt` with the hyperparameter(s) to be updated, because it will update, solve, and return the optimal X in one step. Calling `solve` with  the hyperparameter(s) to be updated and then calling `getXopt()` without input is effectively the same, and the problem will be solved once as long as there is no update.
 
 ## Normalization Convention
 
 The entries in <img src="https://render.githubusercontent.com/render/math?math=A^TA, G^TG"> are preferred to be on the order of unity, because regularization-related quadratic form matrices have their entries around unity. The scale factors are set as
 
-![normalization](https://latex.codecogs.com/svg.latex?&space;s_a=\sqrt{\frac{1}{N_w}\mathrm{tr}(A^TA)},s_g=\sqrt{\frac{1}{N_q}\mathrm{tr}(G^TG)})
-
-where <img src="https://render.githubusercontent.com/render/math?math=N_w, N_q"> are the dimensions along w-axis and q-axis, respectively. <img src="https://render.githubusercontent.com/render/math?math=s_as_g"> is an accessible property of the solver `AGscale`. To normalize or not is controlled by parameter `pre_normalize` in instanciation. 
+$$s_a=\sqrt{\frac{1}{N_w}\mathrm{tr}(A^TA)},s_g=\sqrt{\frac{1}{N_q}\mathrm{tr}(G^TG)}$$
 
-**By default** `pre_normalize=True`, i.e. `self._AtA` =<img src="https://render.githubusercontent.com/render/math?math=A^TA/s_a^2">, `self._GtG` =<img src="https://render.githubusercontent.com/render/math?math=G^TG/s_g^2">, and `self._Bcontracted` = <img src="https://render.githubusercontent.com/render/math?math=(A^T \otimes G^T)B/(s_as_g)">. In this case, the direct solution `self.res` is scaled as <img src="https://render.githubusercontent.com/render/math?math=s_as_g X_\mathrm{opt}"> , but in `getXopt` the final result of <img src="https://render.githubusercontent.com/render/math?math=X_\mathrm{opt}"> is scaled back before returned.
+where <img src="https://render.githubusercontent.com/render/math?math=N_w, N_q"> are the dimensions along w-axis and q-axis, respectively. <img src="https://render.githubusercontent.com/render/math?math=s_as_g"> is an accessible property of the solver `AGscale`. To normalize or not is controlled by parameter `normalize` in creating a solver. 
 
-The entries in B are not always accessible, because of the option to pass in precontracted results and in `mode='contracted'`. Therefore B is not normalized. 
+**By default** `normalize=True`, i.e. `self._AtA` =<img src="https://render.githubusercontent.com/render/math?math=A^TA/s_a^2">, `self._GtG` =<img src="https://render.githubusercontent.com/render/math?math=G^TG/s_g^2">, and `self._Bcontracted` = <img src="https://render.githubusercontent.com/render/math?math=(A^T \otimes G^T)B/(s_as_g)">, and the normalization is not in-place starting from version 0.9.4 . In this case, the direct solution `self.res` is scaled as <img src="https://render.githubusercontent.com/render/math?math=s_as_g X_\mathrm{opt}"> , but the `getXopt` method returns the unscaled result of <img src="https://render.githubusercontent.com/render/math?math=X_\mathrm{opt}">. In v0.9.3 and before, the normalization is in-place, which means the first two arguments are modified in-place. In-place normalization saves memory but causes confusion when people reuses the precontracted results for other purposes after passing them to create a solver in the contracted mode. Therefore starting from v0.9.4, in-place normalization is only done when requested with `normalize='inplace'` in creating a solver.
 
+## Citing
+Please cite [Wang _et al_ 2023](https://iopscience.iop.org/article/10.1088/1367-2630/acc201) when using this package in your publishable work. If `SpookPosL1`, `SpookPosL2` or `SpookL1` is used, we also **strongly recommend** to cite the original OSQP paper as suggested [here](https://osqp.org/citing/).
 
 ## Unit Tests
 
 `unittest/testPosL1.py` is a good example to play with `SpookPosL1`.
 `unittest/testL1L2.ipynb` include good examples to play with `SpookPosL1`, `SpookPosL2`, and `SpookL1`.
 
 
 ## Dependencies
 
-See `requirements.txt`
+pip installation should manage the dependencies automatically. If not, check `requirements.txt` . 
 
 ## Acknowledgement
 This work was supported by the U.S. Department of Energy (DOE), Office of Science, Office of Basic Energy Sciences (BES), Chemical Sciences, Geosciences, and Biosciences Division (CSGB).
```

### Comparing `FDGI-0.9.3/LICENSE` & `FDGI-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FDGI-0.9.3/PKG-INFO` & `FDGI-0.9.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: FDGI
-Version: 0.9.3
-Summary: A package for frequency-domain ghost imaging
+Version: 0.9.4
+Summary: A package for spectral-domain ghost imaging
 Home-page: https://github.com/congzlwag/spook
 Author: Jun Wang
 Author-email: junwang9@stanford.edu
 Project-URL: Bug Tracker, https://github.com/congzlwag/spook/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,33 +17,31 @@
 
 ## Target Problem
 Solve <img src="https://render.githubusercontent.com/render/math?math=(A \otimes G)X = B"> in the least-square way, under [regularizations](#Regularizations). A, G are matrices acting on the two dimensions of X, i.e. 
 ![(AG)X=B](https://latex.codecogs.com/svg.latex?\normalsize&space;\sum_{w,b}A_{iw}G_{bq}X_{wb}=B_{iq}) .
 For spectral-domain ghost imaging, the dimension indexed by <img src="https://render.githubusercontent.com/render/math?math=w"> is photon energy, and the other dimension can be properties of the photoproduct, such as the electron kinetic energy.
 
 `G` is the (optional) linear operator on the dimension indexed by <img src="https://render.githubusercontent.com/render/math?math=b">. By default (`G=None`), it is the identity, in which case this is the conventional Spooktroscopy, i.e. to solve <img src="https://render.githubusercontent.com/render/math?math=AX=B"> under regularizations. 
-`G` can accommodate other linear operations on the $b$ dimension, to solve the two linear inversions in one step. With `mode='raw'`, pass in matrix ![G](https://latex.codecogs.com/svg.latex?\normalsize&space;G_{bq}) to G, and with `mode='contracted'`, pass in matrix ![GtG](https://latex.codecogs.com/svg.latex?\normalsize&space;\sum_qG_{bq}G_{b'q}). For example, for Abel transform in Velocity Map Imaging, [pBasex](https://github.com/e-champenois/CPBASEX) offers this G with `loadG`.
+`G` can accommodate other linear operations on the $b$ dimension, to solve the two linear inversions in one step. 
+
+With `mode='raw'`, pass in matrix $G_{bq}$ to G, and with `mode='contracted'`, pass in matrix $\sum_qG_{bq}G_{b'q}$. For example, for Abel transform in Velocity Map Imaging, [pBasex](https://github.com/e-champenois/CPBASEX) offers this G with `loadG`.
 
 ### Key Advantages
 The key advantages of this package are
 1. Efficient optimization: Contraction over shots is decoupled from optimization. It is **recommended** to input precontracted results when instantiating, or to save the caches using method `save_prectr` of a solver created with raw inputs. Once instantiated, the precontracted results are cached to be reused every time solving with a different hyperparameter. See `spook.contraction_utils.adaptive_contraction` .
 2. Support dimension reduction on the dependent variable B, through basis functions in G. In that case, it is also recommended to contract (B,G) over the dependent variable space (index q) prior to instantiating a spook solver.
 3. Support multiple combinations of regularizations. See [Solvers](#Solvers) .
 4. Support time-dependent measurement (Beta): when each entry in the raw input A is a pair of (photon spectrum, delay bin), index w is the flattened axis of (<img src="https://render.githubusercontent.com/render/math?math=\omega">, <img src="https://render.githubusercontent.com/render/math?math=\tau">). In this case, the third smoothness hyperparameter is for the delay axis.
 
 At the very bottom level, this package depends on either [OSQP](https://osqp.org) to solve a quadratic programming or LAPACK gesv through `numpy.linalg.solve` . 
 
-### Regularizations
-Common regularizations are the following three types, all of which optional, depending on what _a prior_ knowledge one wants to enforce on the problem solving.
+## Installation
+The stable version is on PyPI. Unfortunately in a different name.
 
-1. Nonnegativity: To constrain <img src="https://render.githubusercontent.com/render/math?math=X\succeq 0">
-2. Sparsity: To penalize on <img src="https://render.githubusercontent.com/render/math?math=\|X\|_1"> or <img src="https://render.githubusercontent.com/render/math?math=\|X\|_2^2">
-3. Smoothness: To penalize on roughness of X , along the two indices, independently. For <img src="https://render.githubusercontent.com/render/math?math=\omega">-axis, which is the photon energy axis, the form is fixed <img src="https://render.githubusercontent.com/render/math?math=\|(L_{N_w}\otimes I)X\|_2^2"> where <img src="https://render.githubusercontent.com/render/math?math=L_{N_w}"> is the [laplacian](https://en.wikipedia.org/wiki/Laplace_operator). Roughness along the second axis of X is customizable through parameter `Bsmoother`, which by default is laplacian squared too.
-
-Sparsity and Smoothness are enforced through penalties in the total obejctive function, and the penalties are weighted by hyperparameters `lsparse` and `lsmooth`. `lsmooth` is a 2-tuple that weight roughness penalty along the two axes of X respectively. The hyperparameters can be passed in during instantiation and also updated afterwards. It is recommended to call method `getXopt` with the hyperparameter(s) to be updated, because it will update, solve, and return the optimal X in one step. Calling `solve` with  the hyperparameter(s) to be updated and then calling `getXopt()` without input is effectively the same, and the problem will be solved once as long as there is no update.
+    pip install FDGI
 
 ## Solvers
 
 Different combinations of regularizations can lead to different forms of objective function. Solvers in package always formalize the specific problem into either a [Quadratic Programming](https://en.wikipedia.org/wiki/Quadratic_programming) or a linear equation. Examples can be found in [unit tests](#UnitTests) 
 
 | Nonnegativity | Sparsity            | Smoothness | Solver              | Notes                                                        |
 | ------------- | ------------------- | ---------- | ------------------- | ------------------------------------------------------------ |
@@ -51,39 +49,47 @@
 | True          | L2 squared          | Quadratic  | `SpookPosL2` |                                                              |
 | False         | L2 squared or False | Quadratic  | `SpookLinSolve`     | This solver is so far the work-horse for SpookVMI            |
 | False         | L1                  | Quadratic  | `SpookL1` |                                                              |
 
 
 ### Quadratic Programming
 
-For cases where it can be formalized into a [Quadratic Programming](https://en.wikipedia.org/wiki/Quadratic_programming) , [OSQP](https://osqp.org) does the job. Thus the root numerical method is alternating direction method of multipliers (ADMM). Looking into the [solver settings of OSQP](https://osqp.org/docs/interfaces/solver_settings.html) is always encouraged, but the default settings usually work fine for `spook` . If one needs to pass in settings, the OSQP solver is `SpookQPBase._prob` .
+For cases where it can be formalized into a [Quadratic Programming](https://en.wikipedia.org/wiki/Quadratic_programming) , [OSQP](https://osqp.org) is the weight-lifter. The root numerical method is the alternating direction method of multipliers (ADMM). Looking into the [solver settings of OSQP](https://osqp.org/docs/interfaces/solver_settings.html) is always encouraged, but the default settings usually work fine for `spook` . If one needs to pass in settings, use `spk._prob.update_settings(**osqp_kwargs)` on your solver instance `spk`. 
 
 ### Linear Equation
 
 A rare case that it can be formalized into a linear equation is the third line in the table above: no nonnegativity constraint, and the sparsity is L2 norm squared. This is implemented in `SpookLinSolve` , which calls `numpy.linalg.solve` or `scipy.sparse.linalg.spsolve` .
 
+### Regularizations
+Common regularizations are the following three types, all of which optional, depending on what _a prior_ knowledge one wants to enforce on the problem solving.
+
+1. Nonnegativity: To constrain <img src="https://render.githubusercontent.com/render/math?math=X\succeq 0">
+2. Sparsity: To penalize on <img src="https://render.githubusercontent.com/render/math?math=\|X\|_1"> or <img src="https://render.githubusercontent.com/render/math?math=\|X\|_2^2">
+3. Smoothness: To penalize on roughness of X , along the two indices, independently. For <img src="https://render.githubusercontent.com/render/math?math=\omega">-axis, which is the photon energy axis, the form is fixed <img src="https://render.githubusercontent.com/render/math?math=\|(L_{N_w}\otimes I)X\|_2^2"> where <img src="https://render.githubusercontent.com/render/math?math=L_{N_w}"> is the [laplacian](https://en.wikipedia.org/wiki/Laplace_operator). Roughness along the second axis of X is customizable through parameter `Bsmoother`, which by default is laplacian squared too.
+
+Sparsity and Smoothness are enforced through penalties in the total obejctive function, and the penalties are weighted by hyperparameters `lsparse` and `lsmooth`. `lsmooth` is a 2-tuple that weight roughness penalty along the two axes of X respectively. The hyperparameters can be passed in during instantiation and also updated afterwards. It is recommended to call method `getXopt` with the hyperparameter(s) to be updated, because it will update, solve, and return the optimal X in one step. Calling `solve` with  the hyperparameter(s) to be updated and then calling `getXopt()` without input is effectively the same, and the problem will be solved once as long as there is no update.
 
 ## Normalization Convention
 
 The entries in <img src="https://render.githubusercontent.com/render/math?math=A^TA, G^TG"> are preferred to be on the order of unity, because regularization-related quadratic form matrices have their entries around unity. The scale factors are set as
 
-![normalization](https://latex.codecogs.com/svg.latex?&space;s_a=\sqrt{\frac{1}{N_w}\mathrm{tr}(A^TA)},s_g=\sqrt{\frac{1}{N_q}\mathrm{tr}(G^TG)})
-
-where <img src="https://render.githubusercontent.com/render/math?math=N_w, N_q"> are the dimensions along w-axis and q-axis, respectively. <img src="https://render.githubusercontent.com/render/math?math=s_as_g"> is an accessible property of the solver `AGscale`. To normalize or not is controlled by parameter `pre_normalize` in instanciation. 
+$$s_a=\sqrt{\frac{1}{N_w}\mathrm{tr}(A^TA)},s_g=\sqrt{\frac{1}{N_q}\mathrm{tr}(G^TG)}$$
 
-**By default** `pre_normalize=True`, i.e. `self._AtA` =<img src="https://render.githubusercontent.com/render/math?math=A^TA/s_a^2">, `self._GtG` =<img src="https://render.githubusercontent.com/render/math?math=G^TG/s_g^2">, and `self._Bcontracted` = <img src="https://render.githubusercontent.com/render/math?math=(A^T \otimes G^T)B/(s_as_g)">. In this case, the direct solution `self.res` is scaled as <img src="https://render.githubusercontent.com/render/math?math=s_as_g X_\mathrm{opt}"> , but in `getXopt` the final result of <img src="https://render.githubusercontent.com/render/math?math=X_\mathrm{opt}"> is scaled back before returned.
+where <img src="https://render.githubusercontent.com/render/math?math=N_w, N_q"> are the dimensions along w-axis and q-axis, respectively. <img src="https://render.githubusercontent.com/render/math?math=s_as_g"> is an accessible property of the solver `AGscale`. To normalize or not is controlled by parameter `normalize` in creating a solver. 
 
-The entries in B are not always accessible, because of the option to pass in precontracted results and in `mode='contracted'`. Therefore B is not normalized. 
+**By default** `normalize=True`, i.e. `self._AtA` =<img src="https://render.githubusercontent.com/render/math?math=A^TA/s_a^2">, `self._GtG` =<img src="https://render.githubusercontent.com/render/math?math=G^TG/s_g^2">, and `self._Bcontracted` = <img src="https://render.githubusercontent.com/render/math?math=(A^T \otimes G^T)B/(s_as_g)">, and the normalization is not in-place starting from version 0.9.4 . In this case, the direct solution `self.res` is scaled as <img src="https://render.githubusercontent.com/render/math?math=s_as_g X_\mathrm{opt}"> , but the `getXopt` method returns the unscaled result of <img src="https://render.githubusercontent.com/render/math?math=X_\mathrm{opt}">. In v0.9.3 and before, the normalization is in-place, which means the first two arguments are modified in-place. In-place normalization saves memory but causes confusion when people reuses the precontracted results for other purposes after passing them to create a solver in the contracted mode. Therefore starting from v0.9.4, in-place normalization is only done when requested with `normalize='inplace'` in creating a solver.
 
+## Citing
+Please cite [Wang _et al_ 2023](https://iopscience.iop.org/article/10.1088/1367-2630/acc201) when using this package in your publishable work. If `SpookPosL1`, `SpookPosL2` or `SpookL1` is used, we also **strongly recommend** to cite the original OSQP paper as suggested [here](https://osqp.org/citing/).
 
 ## Unit Tests
 
 `unittest/testPosL1.py` is a good example to play with `SpookPosL1`.
 `unittest/testL1L2.ipynb` include good examples to play with `SpookPosL1`, `SpookPosL2`, and `SpookL1`.
 
 
 ## Dependencies
 
-See `requirements.txt`
+pip installation should manage the dependencies automatically. If not, check `requirements.txt` . 
 
 ## Acknowledgement
 This work was supported by the U.S. Department of Energy (DOE), Office of Science, Office of Basic Energy Sciences (BES), Chemical Sciences, Geosciences, and Biosciences Division (CSGB).
```

### Comparing `FDGI-0.9.3/README.md` & `FDGI-0.9.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 
 ## Target Problem
 Solve <img src="https://render.githubusercontent.com/render/math?math=(A \otimes G)X = B"> in the least-square way, under [regularizations](#Regularizations). A, G are matrices acting on the two dimensions of X, i.e. 
 ![(AG)X=B](https://latex.codecogs.com/svg.latex?\normalsize&space;\sum_{w,b}A_{iw}G_{bq}X_{wb}=B_{iq}) .
 For spectral-domain ghost imaging, the dimension indexed by <img src="https://render.githubusercontent.com/render/math?math=w"> is photon energy, and the other dimension can be properties of the photoproduct, such as the electron kinetic energy.
 
 `G` is the (optional) linear operator on the dimension indexed by <img src="https://render.githubusercontent.com/render/math?math=b">. By default (`G=None`), it is the identity, in which case this is the conventional Spooktroscopy, i.e. to solve <img src="https://render.githubusercontent.com/render/math?math=AX=B"> under regularizations. 
-`G` can accommodate other linear operations on the $b$ dimension, to solve the two linear inversions in one step. With `mode='raw'`, pass in matrix ![G](https://latex.codecogs.com/svg.latex?\normalsize&space;G_{bq}) to G, and with `mode='contracted'`, pass in matrix ![GtG](https://latex.codecogs.com/svg.latex?\normalsize&space;\sum_qG_{bq}G_{b'q}). For example, for Abel transform in Velocity Map Imaging, [pBasex](https://github.com/e-champenois/CPBASEX) offers this G with `loadG`.
+`G` can accommodate other linear operations on the $b$ dimension, to solve the two linear inversions in one step. 
+
+With `mode='raw'`, pass in matrix $G_{bq}$ to G, and with `mode='contracted'`, pass in matrix $\sum_qG_{bq}G_{b'q}$. For example, for Abel transform in Velocity Map Imaging, [pBasex](https://github.com/e-champenois/CPBASEX) offers this G with `loadG`.
 
 ### Key Advantages
 The key advantages of this package are
 1. Efficient optimization: Contraction over shots is decoupled from optimization. It is **recommended** to input precontracted results when instantiating, or to save the caches using method `save_prectr` of a solver created with raw inputs. Once instantiated, the precontracted results are cached to be reused every time solving with a different hyperparameter. See `spook.contraction_utils.adaptive_contraction` .
 2. Support dimension reduction on the dependent variable B, through basis functions in G. In that case, it is also recommended to contract (B,G) over the dependent variable space (index q) prior to instantiating a spook solver.
 3. Support multiple combinations of regularizations. See [Solvers](#Solvers) .
 4. Support time-dependent measurement (Beta): when each entry in the raw input A is a pair of (photon spectrum, delay bin), index w is the flattened axis of (<img src="https://render.githubusercontent.com/render/math?math=\omega">, <img src="https://render.githubusercontent.com/render/math?math=\tau">). In this case, the third smoothness hyperparameter is for the delay axis.
 
 At the very bottom level, this package depends on either [OSQP](https://osqp.org) to solve a quadratic programming or LAPACK gesv through `numpy.linalg.solve` . 
 
-### Regularizations
-Common regularizations are the following three types, all of which optional, depending on what _a prior_ knowledge one wants to enforce on the problem solving.
+## Installation
+The stable version is on PyPI. Unfortunately in a different name.
 
-1. Nonnegativity: To constrain <img src="https://render.githubusercontent.com/render/math?math=X\succeq 0">
-2. Sparsity: To penalize on <img src="https://render.githubusercontent.com/render/math?math=\|X\|_1"> or <img src="https://render.githubusercontent.com/render/math?math=\|X\|_2^2">
-3. Smoothness: To penalize on roughness of X , along the two indices, independently. For <img src="https://render.githubusercontent.com/render/math?math=\omega">-axis, which is the photon energy axis, the form is fixed <img src="https://render.githubusercontent.com/render/math?math=\|(L_{N_w}\otimes I)X\|_2^2"> where <img src="https://render.githubusercontent.com/render/math?math=L_{N_w}"> is the [laplacian](https://en.wikipedia.org/wiki/Laplace_operator). Roughness along the second axis of X is customizable through parameter `Bsmoother`, which by default is laplacian squared too.
-
-Sparsity and Smoothness are enforced through penalties in the total obejctive function, and the penalties are weighted by hyperparameters `lsparse` and `lsmooth`. `lsmooth` is a 2-tuple that weight roughness penalty along the two axes of X respectively. The hyperparameters can be passed in during instantiation and also updated afterwards. It is recommended to call method `getXopt` with the hyperparameter(s) to be updated, because it will update, solve, and return the optimal X in one step. Calling `solve` with  the hyperparameter(s) to be updated and then calling `getXopt()` without input is effectively the same, and the problem will be solved once as long as there is no update.
+    pip install FDGI
 
 ## Solvers
 
 Different combinations of regularizations can lead to different forms of objective function. Solvers in package always formalize the specific problem into either a [Quadratic Programming](https://en.wikipedia.org/wiki/Quadratic_programming) or a linear equation. Examples can be found in [unit tests](#UnitTests) 
 
 | Nonnegativity | Sparsity            | Smoothness | Solver              | Notes                                                        |
 | ------------- | ------------------- | ---------- | ------------------- | ------------------------------------------------------------ |
@@ -36,39 +34,47 @@
 | True          | L2 squared          | Quadratic  | `SpookPosL2` |                                                              |
 | False         | L2 squared or False | Quadratic  | `SpookLinSolve`     | This solver is so far the work-horse for SpookVMI            |
 | False         | L1                  | Quadratic  | `SpookL1` |                                                              |
 
 
 ### Quadratic Programming
 
-For cases where it can be formalized into a [Quadratic Programming](https://en.wikipedia.org/wiki/Quadratic_programming) , [OSQP](https://osqp.org) does the job. Thus the root numerical method is alternating direction method of multipliers (ADMM). Looking into the [solver settings of OSQP](https://osqp.org/docs/interfaces/solver_settings.html) is always encouraged, but the default settings usually work fine for `spook` . If one needs to pass in settings, the OSQP solver is `SpookQPBase._prob` .
+For cases where it can be formalized into a [Quadratic Programming](https://en.wikipedia.org/wiki/Quadratic_programming) , [OSQP](https://osqp.org) is the weight-lifter. The root numerical method is the alternating direction method of multipliers (ADMM). Looking into the [solver settings of OSQP](https://osqp.org/docs/interfaces/solver_settings.html) is always encouraged, but the default settings usually work fine for `spook` . If one needs to pass in settings, use `spk._prob.update_settings(**osqp_kwargs)` on your solver instance `spk`. 
 
 ### Linear Equation
 
 A rare case that it can be formalized into a linear equation is the third line in the table above: no nonnegativity constraint, and the sparsity is L2 norm squared. This is implemented in `SpookLinSolve` , which calls `numpy.linalg.solve` or `scipy.sparse.linalg.spsolve` .
 
+### Regularizations
+Common regularizations are the following three types, all of which optional, depending on what _a prior_ knowledge one wants to enforce on the problem solving.
+
+1. Nonnegativity: To constrain <img src="https://render.githubusercontent.com/render/math?math=X\succeq 0">
+2. Sparsity: To penalize on <img src="https://render.githubusercontent.com/render/math?math=\|X\|_1"> or <img src="https://render.githubusercontent.com/render/math?math=\|X\|_2^2">
+3. Smoothness: To penalize on roughness of X , along the two indices, independently. For <img src="https://render.githubusercontent.com/render/math?math=\omega">-axis, which is the photon energy axis, the form is fixed <img src="https://render.githubusercontent.com/render/math?math=\|(L_{N_w}\otimes I)X\|_2^2"> where <img src="https://render.githubusercontent.com/render/math?math=L_{N_w}"> is the [laplacian](https://en.wikipedia.org/wiki/Laplace_operator). Roughness along the second axis of X is customizable through parameter `Bsmoother`, which by default is laplacian squared too.
+
+Sparsity and Smoothness are enforced through penalties in the total obejctive function, and the penalties are weighted by hyperparameters `lsparse` and `lsmooth`. `lsmooth` is a 2-tuple that weight roughness penalty along the two axes of X respectively. The hyperparameters can be passed in during instantiation and also updated afterwards. It is recommended to call method `getXopt` with the hyperparameter(s) to be updated, because it will update, solve, and return the optimal X in one step. Calling `solve` with  the hyperparameter(s) to be updated and then calling `getXopt()` without input is effectively the same, and the problem will be solved once as long as there is no update.
 
 ## Normalization Convention
 
 The entries in <img src="https://render.githubusercontent.com/render/math?math=A^TA, G^TG"> are preferred to be on the order of unity, because regularization-related quadratic form matrices have their entries around unity. The scale factors are set as
 
-![normalization](https://latex.codecogs.com/svg.latex?&space;s_a=\sqrt{\frac{1}{N_w}\mathrm{tr}(A^TA)},s_g=\sqrt{\frac{1}{N_q}\mathrm{tr}(G^TG)})
-
-where <img src="https://render.githubusercontent.com/render/math?math=N_w, N_q"> are the dimensions along w-axis and q-axis, respectively. <img src="https://render.githubusercontent.com/render/math?math=s_as_g"> is an accessible property of the solver `AGscale`. To normalize or not is controlled by parameter `pre_normalize` in instanciation. 
+$$s_a=\sqrt{\frac{1}{N_w}\mathrm{tr}(A^TA)},s_g=\sqrt{\frac{1}{N_q}\mathrm{tr}(G^TG)}$$
 
-**By default** `pre_normalize=True`, i.e. `self._AtA` =<img src="https://render.githubusercontent.com/render/math?math=A^TA/s_a^2">, `self._GtG` =<img src="https://render.githubusercontent.com/render/math?math=G^TG/s_g^2">, and `self._Bcontracted` = <img src="https://render.githubusercontent.com/render/math?math=(A^T \otimes G^T)B/(s_as_g)">. In this case, the direct solution `self.res` is scaled as <img src="https://render.githubusercontent.com/render/math?math=s_as_g X_\mathrm{opt}"> , but in `getXopt` the final result of <img src="https://render.githubusercontent.com/render/math?math=X_\mathrm{opt}"> is scaled back before returned.
+where <img src="https://render.githubusercontent.com/render/math?math=N_w, N_q"> are the dimensions along w-axis and q-axis, respectively. <img src="https://render.githubusercontent.com/render/math?math=s_as_g"> is an accessible property of the solver `AGscale`. To normalize or not is controlled by parameter `normalize` in creating a solver. 
 
-The entries in B are not always accessible, because of the option to pass in precontracted results and in `mode='contracted'`. Therefore B is not normalized. 
+**By default** `normalize=True`, i.e. `self._AtA` =<img src="https://render.githubusercontent.com/render/math?math=A^TA/s_a^2">, `self._GtG` =<img src="https://render.githubusercontent.com/render/math?math=G^TG/s_g^2">, and `self._Bcontracted` = <img src="https://render.githubusercontent.com/render/math?math=(A^T \otimes G^T)B/(s_as_g)">, and the normalization is not in-place starting from version 0.9.4 . In this case, the direct solution `self.res` is scaled as <img src="https://render.githubusercontent.com/render/math?math=s_as_g X_\mathrm{opt}"> , but the `getXopt` method returns the unscaled result of <img src="https://render.githubusercontent.com/render/math?math=X_\mathrm{opt}">. In v0.9.3 and before, the normalization is in-place, which means the first two arguments are modified in-place. In-place normalization saves memory but causes confusion when people reuses the precontracted results for other purposes after passing them to create a solver in the contracted mode. Therefore starting from v0.9.4, in-place normalization is only done when requested with `normalize='inplace'` in creating a solver.
 
+## Citing
+Please cite [Wang _et al_ 2023](https://iopscience.iop.org/article/10.1088/1367-2630/acc201) when using this package in your publishable work. If `SpookPosL1`, `SpookPosL2` or `SpookL1` is used, we also **strongly recommend** to cite the original OSQP paper as suggested [here](https://osqp.org/citing/).
 
 ## Unit Tests
 
 `unittest/testPosL1.py` is a good example to play with `SpookPosL1`.
 `unittest/testL1L2.ipynb` include good examples to play with `SpookPosL1`, `SpookPosL2`, and `SpookL1`.
 
 
 ## Dependencies
 
-See `requirements.txt`
+pip installation should manage the dependencies automatically. If not, check `requirements.txt` . 
 
 ## Acknowledgement
 This work was supported by the U.S. Department of Energy (DOE), Office of Science, Office of Basic Energy Sciences (BES), Chemical Sciences, Geosciences, and Biosciences Division (CSGB).
```

### Comparing `FDGI-0.9.3/setup.cfg` & `FDGI-0.9.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = FDGI
-version = 0.9.3
+version = attr: spook.__version__
 author = Jun Wang
 author_email = junwang9@stanford.edu
-description = A package for frequency-domain ghost imaging
+description = A package for spectral-domain ghost imaging
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/congzlwag/spook
 project_urls = 
 	Bug Tracker = https://github.com/congzlwag/spook/issues
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `FDGI-0.9.3/spook/base.py` & `FDGI-0.9.4/spook/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,19 @@
     def __init__(self, B, A, mode="raw", G=None, lsparse=None, lsmooth=None, 
         Bsmoother="laplacian", Asmoother="laplacian", normalize=True):
         """
         :param mode: "raw" or "contracted" (recommended) or "ADraw"
                      In the "contracted" mode, A is AT@A, B is (AT otimes GT)@B, G is GTG
         :param Bsmoother: the quadratic matrix for smoothness
         :param normalize: If True, then normalize ATA, GTG, obtaining scale factors (sA, sG) and then normalize Bcontracted
+                              But it won't be in-place for mode='contracted'
+                          If 'inplace', then the normalizations are done in-place
                           If (sA, sG), then cache the scale factors and do nothing on the contracted results
                           If False, do nothing and set (sA, sG) = (1,1)
+                          
         """
         assert (mode in ['raw', 'contracted', 'ADraw']), f"Unknown mode: {mode}. Must be either 'raw' or 'contracted' or 'ADraw'"
 
         # Make sure the class eventually stores AtA, GtG and (At otimes Gt)B
         # All these are presumably dense, especially A, if not, crop in.
         if isinstance(B, np.ndarray) and B.ndim==1:
             B = B[:, None]
@@ -189,36 +192,38 @@
         return ret
 
     def normalizeAG(self, normalize):
         if normalize == False:
             self.__Ascale, self.__Gscale = (1,1)
         elif isinstance(normalize, tuple):
             self.__Ascale, self.__Gscale = normalize
-        else:
+        else: # normalize in ['inplace', True]
             scaleA2 = np.trace(self._AtA) / (self._AtA.shape[1]) # px-wise mean-square
-            # Actual normalization happens here
-            self._AtA /= scaleA2
             self.__Ascale = scaleA2**0.5
             if self._GtG is None:
                 scaleG2 = 1
             else:
                 if isinstance(self._GtG, np.ndarray):
                     scaleG2 = np.trace(self._GtG) / (self.Ng) # px-wise mean-square
                 else:
                     scaleG2 = self._GtG.diagonal().mean()
                 # Actual normalization happens here
-                self._GtG /= scaleG2
+                if normalize == 'inplace':
+                    self._GtG /= scaleG2
+                else:
+                    self._GtG = self._GtG.copy() / scaleG2
             self.__Gscale = scaleG2**0.5
             # Actual normalization happens here
-            # else:
-            #     scaleAG2 = np.trace(self._AGtAG) / (self._AGtAG.shape[1])
-            #     self._AGtAG /= scaleAG2
-            #     self.__Ascale = scaleAG2**0.5
-            #     self.__Gscale = 1
-            self._Bcontracted /= self.AGscale
+            if normalize == 'inplace':
+                self._AtA /= scaleA2
+                self._Bcontracted /= self.AGscale
+            else:
+                self._AtA = self._AtA.copy() / scaleA2
+                self._Bcontracted = self._Bcontracted.copy() / self.AGscale
+
 
     @property
     def AGscale(self):
         return self.__Ascale*self.__Gscale
 
     @property
     def AGtAG(self):
```

### Comparing `FDGI-0.9.3/spook/contraction_utils.py` & `FDGI-0.9.4/spook/contraction_utils.py`

 * *Files identical despite different names*

### Comparing `FDGI-0.9.3/spook/lin_solve.py` & `FDGI-0.9.4/spook/lin_solve.py`

 * *Files identical despite different names*

### Comparing `FDGI-0.9.3/spook/quad_program.py` & `FDGI-0.9.4/spook/quad_program.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,21 @@
             self._Pcore = sps.triu(self.AGtAG, 0, "csc")
             # self._qhalf = - self._Bcontracted.ravel()
             # To compare a new P with the current one, it is more efficient to
             # compare just the upper triangular part, so self._P just caches the
             # upper triangular part
             self._P = self.calcPtriu()
             # SpookL1 will have self._P in shape (2*Nag, 2*Nag), which has no memory overhead
-            # beacuse the other three blocks are all zeros, and reize does it in situ
+            # beacuse the other three blocks are all zeros, and resize does it in situ
             self._prob = self.setupProb()
         else:
             self._Pcore = sps.triu(self._AtA, 0, "csc")
             self._P = self.calcPtriu()
             self._probs= [self.setupProb(col) for col in range(Ng)]
-
+        self.set_polish(True)
 
     def calc_total_smoother_triu(self):
         """
         CALCULATE Total Smoothness regularization operator
         lsma * (La.T @ La otimes Ib) + lsmb * (Ia otimes Bsmoother)
         
         This method always recalculates
```

### Comparing `FDGI-0.9.3/spook/utils.py` & `FDGI-0.9.4/spook/utils.py`

 * *Files identical despite different names*

### Comparing `FDGI-0.9.3/spook/vmi_special.py` & `FDGI-0.9.4/spook/vmi_special.py`

 * *Files identical despite different names*

