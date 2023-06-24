# Comparing `tmp/deeppipe_api-0.0.7.tar.gz` & `tmp/deeppipe_api-0.0.8.tar.gz`

## Comparing `deeppipe_api-0.0.7.tar` & `deeppipe_api-0.0.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/__init__.py
--rw-r--r--   0        0        0    15014 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/deeppipe.py
--rw-r--r--   0        0        0    21683 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/modules.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/requirements.txt
--rw-r--r--   0        0        0    10091 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/utils.py
--rw-r--r--   0        0        0    15377 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/deep_pipe.py
--rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/meta_test.py
--rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/meta_train.py
--rw-r--r--   0        0        0    21683 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/modules.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/readme.md
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/requirements_all.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/requirements_deep_pipe.txt
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/test_openml.py
--rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/utils.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/automl_baselines/autoprognosis_test.py
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/automl_baselines/oboe_bench_test.py
--rw-r--r--   0        0        0    15033 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/automl_baselines/pmf_bench_test.py
--rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/automl_baselines/rf_bench_test.py
--rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/automl_baselines/tpot_bench_test.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/baselines/bo.py
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/baselines/data_loader.py
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/baselines/rgpe.py
--rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/baselines/surrogates.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/baselines/test.py
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/fmlp/fmlp.py
--rw-r--r--   0        0        0     9700 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/fmlp/fmlp_loaders.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/fmlp/test_fmlp.py
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/fmlp/train_fmlp.py
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/convex_opt.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/linalg.py
--rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/model.py
--rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/pipeline.py
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/qr_computation.py
--rw-r--r--   0        0        0    17528 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/util.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/bo.py
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/gplvm.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/kernels.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/plotting.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/requirements.txt
--rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/run.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/utils.py
--rw-r--r--   0        0        0    55558 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/tensoroboe/auto_learner.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/configurations/DeepPipe.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/src/deeppipe_api/experiments/configurations/DeepPipeTOboe.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/.gitignore
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/LICENSE
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 deeppipe_api-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/__init__.py
+-rw-r--r--   0        0        0    15014 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/deeppipe.py
+-rw-r--r--   0        0        0    21683 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/modules.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/requirements.txt
+-rw-r--r--   0        0        0    10091 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/utils.py
+-rw-r--r--   0        0        0    15377 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/deep_pipe.py
+-rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/meta_test.py
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/meta_train.py
+-rw-r--r--   0        0        0    21683 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/modules.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/readme.md
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/requirements_all.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/requirements_deep_pipe.txt
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/test_openml.py
+-rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/utils.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/automl_baselines/autoprognosis_test.py
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/automl_baselines/oboe_bench_test.py
+-rw-r--r--   0        0        0    15033 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/automl_baselines/pmf_bench_test.py
+-rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/automl_baselines/rf_bench_test.py
+-rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/automl_baselines/tpot_bench_test.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/baselines/bo.py
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/baselines/data_loader.py
+-rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/baselines/rgpe.py
+-rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/baselines/surrogates.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/baselines/test.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/fmlp/fmlp.py
+-rw-r--r--   0        0        0     9700 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/fmlp/fmlp_loaders.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/fmlp/test_fmlp.py
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/fmlp/train_fmlp.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/convex_opt.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/linalg.py
+-rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/model.py
+-rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/pipeline.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/qr_computation.py
+-rw-r--r--   0        0        0    17528 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/util.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/bo.py
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/gplvm.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/kernels.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/plotting.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/requirements.txt
+-rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/run.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/utils.py
+-rw-r--r--   0        0        0    55558 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/tensoroboe/auto_learner.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/configurations/DeepPipe.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/src/deeppipe_api/experiments/configurations/DeepPipeTOboe.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/LICENSE
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 deeppipe_api-0.0.8/PKG-INFO
```

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/deeppipe.py` & `deeppipe_api-0.0.8/src/deeppipe_api/deeppipe.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/modules.py` & `deeppipe_api-0.0.8/src/deeppipe_api/modules.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/utils.py` & `deeppipe_api-0.0.8/src/deeppipe_api/utils.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/deep_pipe.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/deep_pipe.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/meta_test.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/meta_test.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/meta_train.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/meta_train.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/modules.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/modules.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/readme.md` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/readme.md`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/requirements_all.txt` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/requirements_all.txt`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/test_openml.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/test_openml.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/utils.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/automl_baselines/autoprognosis_test.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/automl_baselines/autoprognosis_test.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/automl_baselines/oboe_bench_test.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/automl_baselines/oboe_bench_test.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/automl_baselines/pmf_bench_test.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/automl_baselines/pmf_bench_test.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/automl_baselines/rf_bench_test.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/automl_baselines/rf_bench_test.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/automl_baselines/tpot_bench_test.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/automl_baselines/tpot_bench_test.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/baselines/bo.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/baselines/bo.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/baselines/data_loader.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/baselines/data_loader.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/baselines/rgpe.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/baselines/rgpe.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/baselines/surrogates.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/baselines/surrogates.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/baselines/test.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/baselines/test.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/fmlp/fmlp.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/fmlp/fmlp.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/fmlp/fmlp_loaders.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/fmlp/fmlp_loaders.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/fmlp/test_fmlp.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/fmlp/test_fmlp.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/fmlp/train_fmlp.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/fmlp/train_fmlp.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/convex_opt.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/convex_opt.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/linalg.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/linalg.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/model.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/model.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/pipeline.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/pipeline.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/qr_computation.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/qr_computation.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/oboe/util.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/oboe/util.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/bo.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/bo.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/gplvm.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/gplvm.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/kernels.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/kernels.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/plotting.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/plotting.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/requirements.txt` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/requirements.txt`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/run.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/run.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/pmf/utils.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/pmf/utils.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/src/deeppipe_api/experiments/baselines/tensoroboe/auto_learner.py` & `deeppipe_api-0.0.8/src/deeppipe_api/experiments/baselines/tensoroboe/auto_learner.py`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/LICENSE` & `deeppipe_api-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `deeppipe_api-0.0.7/pyproject.toml` & `deeppipe_api-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "deeppipe-api"
-version = "0.0.7"
+name = "deeppipe_api"
+version = "0.0.8"
 authors = [
   { name="Sebastian Pineda", email="pineda@cs.uni-freiburg.com" },
 ]
 description = "DeepPipe efficiently optimizes Machine Learning Pipelines using meta-learning."
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies=[
```

### Comparing `deeppipe_api-0.0.7/PKG-INFO` & `deeppipe_api-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: deeppipe-api
-Version: 0.0.7
+Name: deeppipe_api
+Version: 0.0.8
 Summary: DeepPipe efficiently optimizes Machine Learning Pipelines using meta-learning.
 Project-URL: Homepage, https://github.com/releaunifreiburg/DeepPipe
 Project-URL: Bug Tracker, https://github.com/releaunifreiburg/DeepPipe/issues
 Author-email: Sebastian Pineda <pineda@cs.uni-freiburg.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

