# Comparing `tmp/modularbayes-0.1.3.tar.gz` & `tmp/modularbayes-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modularbayes-0.1.3.tar", last modified: Mon Apr 10 23:43:42 2023, max compression
+gzip compressed data, was "modularbayes-0.1.4.tar", last modified: Sat Jun 24 18:18:00 2023, max compression
```

## Comparing `modularbayes-0.1.3.tar` & `modularbayes-0.1.4.tar`

### file list

```diff
@@ -1,88 +1,87 @@
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.191038 modularbayes-0.1.3/
--rw-r--r--   0 carmona    (501) staff       (20)     1070 2023-04-10 23:31:55.000000 modularbayes-0.1.3/LICENSE
--rw-r--r--   0 carmona    (501) staff       (20)       57 2023-04-10 23:31:55.000000 modularbayes-0.1.3/MANIFEST.in
--rw-r--r--   0 carmona    (501) staff       (20)     5956 2023-04-10 23:43:42.190650 modularbayes-0.1.3/PKG-INFO
--rw-r--r--   0 carmona    (501) staff       (20)     4959 2023-04-10 23:31:55.000000 modularbayes-0.1.3/README.md
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.145299 modularbayes-0.1.3/examples/
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.156129 modularbayes-0.1.3/examples/epidemiology/
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.159996 modularbayes-0.1.3/examples/epidemiology/configs/
--rw-r--r--   0 carmona    (501) staff       (20)     2058 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/flow_mf.py
--rw-r--r--   0 carmona    (501) staff       (20)     2396 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/flow_mf_vmp_map.py
--rw-r--r--   0 carmona    (501) staff       (20)     2467 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf.py
--rw-r--r--   0 carmona    (501) staff       (20)     2675 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf_vmp_flow.py
--rw-r--r--   0 carmona    (501) staff       (20)     2810 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf_vmp_map.py
--rw-r--r--   0 carmona    (501) staff       (20)      742 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/configs/mcmc.py
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.161399 modularbayes-0.1.3/examples/epidemiology/data/
--rw-r--r--   0 carmona    (501) staff       (20)      135 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/data/__init__.py
--rw-r--r--   0 carmona    (501) staff       (20)      822 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/data/load.py
--rw-r--r--   0 carmona    (501) staff       (20)    13927 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/flows.py
--rw-r--r--   0 carmona    (501) staff       (20)     4840 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/log_prob_fun.py
--rw-r--r--   0 carmona    (501) staff       (20)     1637 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/main.py
--rw-r--r--   0 carmona    (501) staff       (20)     6526 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/plot.py
--rw-r--r--   0 carmona    (501) staff       (20)    17477 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/sample_mcmc.py
--rw-r--r--   0 carmona    (501) staff       (20)    14600 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/train_flow.py
--rw-r--r--   0 carmona    (501) staff       (20)    14132 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/train_vmp_flow.py
--rw-r--r--   0 carmona    (501) staff       (20)    14165 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/epidemiology/train_vmp_map.py
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.166036 modularbayes-0.1.3/examples/random_effects/
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.173342 modularbayes-0.1.3/examples/random_effects/configs/
--rw-r--r--   0 carmona    (501) staff       (20)     2595 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut1.py
--rw-r--r--   0 carmona    (501) staff       (20)     2537 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut2.py
--rw-r--r--   0 carmona    (501) staff       (20)     2594 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut3.py
--rw-r--r--   0 carmona    (501) staff       (20)     2512 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_full.py
--rw-r--r--   0 carmona    (501) staff       (20)     3232 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_vmp_flow.py
--rw-r--r--   0 carmona    (501) staff       (20)     3197 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_vmp_map.py
--rw-r--r--   0 carmona    (501) staff       (20)      874 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut1.py
--rw-r--r--   0 carmona    (501) staff       (20)      877 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut2.py
--rw-r--r--   0 carmona    (501) staff       (20)      874 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut3.py
--rw-r--r--   0 carmona    (501) staff       (20)      830 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/configs/mcmc_full.py
--rw-r--r--   0 carmona    (501) staff       (20)    12151 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/flows.py
--rw-r--r--   0 carmona    (501) staff       (20)     3064 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/log_prob_fun.py
--rw-r--r--   0 carmona    (501) staff       (20)     1637 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/main.py
--rw-r--r--   0 carmona    (501) staff       (20)     5650 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/plot.py
--rw-r--r--   0 carmona    (501) staff       (20)    17434 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/sample_mcmc.py
--rw-r--r--   0 carmona    (501) staff       (20)    15350 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/train_flow.py
--rw-r--r--   0 carmona    (501) staff       (20)    14409 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/train_vmp_flow.py
--rw-r--r--   0 carmona    (501) staff       (20)    13460 2023-04-10 23:31:55.000000 modularbayes-0.1.3/examples/random_effects/train_vmp_map.py
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.173791 modularbayes-0.1.3/modularbayes/
--rw-r--r--   0 carmona    (501) staff       (20)     2763 2023-04-10 23:43:16.000000 modularbayes-0.1.3/modularbayes/__init__.py
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.177903 modularbayes-0.1.3/modularbayes/_src/
--rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/__init__.py
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.180741 modularbayes-0.1.3/modularbayes/_src/bijectors/
--rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/__init__.py
--rw-r--r--   0 carmona    (501) staff       (20)     4245 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/blockwise.py
--rw-r--r--   0 carmona    (501) staff       (20)     1663 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_bijector.py
--rw-r--r--   0 carmona    (501) staff       (20)     2456 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_chain.py
--rw-r--r--   0 carmona    (501) staff       (20)     1920 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_masked_coupling.py
--rw-r--r--   0 carmona    (501) staff       (20)     2498 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_masked_coupling_extra.py
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.181407 modularbayes-0.1.3/modularbayes/_src/conditioners/
--rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/conditioners/__init__.py
--rw-r--r--   0 carmona    (501) staff       (20)     2668 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/conditioners/base.py
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.183338 modularbayes-0.1.3/modularbayes/_src/distributions/
--rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/distributions/__init__.py
--rw-r--r--   0 carmona    (501) staff       (20)     2873 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/distributions/conditional_transformed.py
--rw-r--r--   0 carmona    (501) staff       (20)      712 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/distributions/transformed.py
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.184643 modularbayes-0.1.3/modularbayes/_src/metaposterior/
--rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/metaposterior/__init__.py
--rw-r--r--   0 carmona    (501) staff       (20)     2325 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/metaposterior/vmp_map.py
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.187035 modularbayes-0.1.3/modularbayes/_src/smi/
--rw-r--r--   0 carmona    (501) staff       (20)     6183 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/smi/elbo.py
--rw-r--r--   0 carmona    (501) staff       (20)     5131 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/smi/sampling.py
--rw-r--r--   0 carmona    (501) staff       (20)     1313 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/typing.py
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.188383 modularbayes-0.1.3/modularbayes/_src/utils/
--rw-r--r--   0 carmona    (501) staff       (20)        0 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/utils/__init__.py
--rw-r--r--   0 carmona    (501) staff       (20)     3840 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/utils/misc.py
--rw-r--r--   0 carmona    (501) staff       (20)     6007 2023-04-10 23:31:55.000000 modularbayes-0.1.3/modularbayes/_src/utils/training.py
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.176803 modularbayes-0.1.3/modularbayes.egg-info/
--rw-r--r--   0 carmona    (501) staff       (20)     5956 2023-04-10 23:43:42.000000 modularbayes-0.1.3/modularbayes.egg-info/PKG-INFO
--rw-r--r--   0 carmona    (501) staff       (20)     2670 2023-04-10 23:43:42.000000 modularbayes-0.1.3/modularbayes.egg-info/SOURCES.txt
--rw-r--r--   0 carmona    (501) staff       (20)        1 2023-04-10 23:43:42.000000 modularbayes-0.1.3/modularbayes.egg-info/dependency_links.txt
--rw-r--r--   0 carmona    (501) staff       (20)        1 2023-04-10 23:40:56.000000 modularbayes-0.1.3/modularbayes.egg-info/not-zip-safe
--rw-r--r--   0 carmona    (501) staff       (20)       84 2023-04-10 23:43:42.000000 modularbayes-0.1.3/modularbayes.egg-info/requires.txt
--rw-r--r--   0 carmona    (501) staff       (20)       47 2023-04-10 23:43:42.000000 modularbayes-0.1.3/modularbayes.egg-info/top_level.txt
-drwxr-xr-x   0 carmona    (501) staff       (20)        0 2023-04-10 23:43:42.190140 modularbayes-0.1.3/requirements/
--rw-r--r--   0 carmona    (501) staff       (20)       26 2023-04-10 23:31:55.000000 modularbayes-0.1.3/requirements/requirements-devel.txt
--rw-r--r--   0 carmona    (501) staff       (20)       43 2023-04-10 23:31:55.000000 modularbayes-0.1.3/requirements/requirements-setup.txt
--rw-r--r--   0 carmona    (501) staff       (20)       14 2023-04-10 23:31:55.000000 modularbayes-0.1.3/requirements/requirements-tests.txt
--rw-r--r--   0 carmona    (501) staff       (20)       84 2023-04-10 23:31:55.000000 modularbayes-0.1.3/requirements/requirements.txt
--rw-r--r--   0 carmona    (501) staff       (20)       38 2023-04-10 23:43:42.191197 modularbayes-0.1.3/setup.cfg
--rw-r--r--   0 carmona    (501) staff       (20)     2260 2023-04-10 23:31:55.000000 modularbayes-0.1.3/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.016889 modularbayes-0.1.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1070 2022-11-14 17:37:23.000000 modularbayes-0.1.4/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       57 2022-12-03 16:15:38.000000 modularbayes-0.1.4/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5937 2023-06-24 18:18:00.016889 modularbayes-0.1.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4940 2023-04-19 14:30:49.000000 modularbayes-0.1.4/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:17:59.992889 modularbayes-0.1.4/examples/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.000889 modularbayes-0.1.4/examples/epidemiology/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.000889 modularbayes-0.1.4/examples/epidemiology/configs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2058 2023-06-03 20:05:19.000000 modularbayes-0.1.4/examples/epidemiology/configs/flow_mf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2366 2023-04-20 16:29:44.000000 modularbayes-0.1.4/examples/epidemiology/configs/flow_mf_vmp_map.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2467 2023-04-08 12:13:43.000000 modularbayes-0.1.4/examples/epidemiology/configs/flow_nsf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2549 2023-06-24 12:51:41.000000 modularbayes-0.1.4/examples/epidemiology/configs/flow_nsf_vmp_flow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2779 2023-04-20 16:29:57.000000 modularbayes-0.1.4/examples/epidemiology/configs/flow_nsf_vmp_map.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      742 2023-04-08 00:12:30.000000 modularbayes-0.1.4/examples/epidemiology/configs/mcmc.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.000889 modularbayes-0.1.4/examples/epidemiology/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      135 2022-11-14 17:37:23.000000 modularbayes-0.1.4/examples/epidemiology/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      822 2022-11-14 17:37:23.000000 modularbayes-0.1.4/examples/epidemiology/data/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9453 2023-06-24 13:24:59.000000 modularbayes-0.1.4/examples/epidemiology/flows.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4840 2023-06-12 15:56:36.000000 modularbayes-0.1.4/examples/epidemiology/log_prob_fun.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1637 2023-04-10 23:28:32.000000 modularbayes-0.1.4/examples/epidemiology/main.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6526 2023-04-10 23:28:32.000000 modularbayes-0.1.4/examples/epidemiology/plot.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17477 2023-04-09 21:30:40.000000 modularbayes-0.1.4/examples/epidemiology/sample_mcmc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15694 2023-06-24 13:18:29.000000 modularbayes-0.1.4/examples/epidemiology/train_flow.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10767 2023-06-24 13:17:35.000000 modularbayes-0.1.4/examples/epidemiology/train_vmp_flow.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13390 2023-06-23 23:08:47.000000 modularbayes-0.1.4/examples/epidemiology/train_vmp_map.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.004889 modularbayes-0.1.4/examples/random_effects/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.008889 modularbayes-0.1.4/examples/random_effects/configs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2595 2023-04-10 11:48:19.000000 modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_cut1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2537 2023-04-10 11:48:23.000000 modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_cut2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2594 2023-04-10 11:48:25.000000 modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_cut3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2512 2023-04-10 11:48:28.000000 modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_full.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3100 2023-06-24 18:14:35.000000 modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_vmp_flow.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3171 2023-06-24 10:45:36.000000 modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_vmp_map.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      874 2023-04-09 23:51:39.000000 modularbayes-0.1.4/examples/random_effects/configs/mcmc_cut1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2023-04-09 23:51:46.000000 modularbayes-0.1.4/examples/random_effects/configs/mcmc_cut2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      874 2023-04-09 23:51:53.000000 modularbayes-0.1.4/examples/random_effects/configs/mcmc_cut3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      830 2023-04-09 23:52:21.000000 modularbayes-0.1.4/examples/random_effects/configs/mcmc_full.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7639 2023-06-24 13:25:06.000000 modularbayes-0.1.4/examples/random_effects/flows.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3164 2023-04-20 16:18:21.000000 modularbayes-0.1.4/examples/random_effects/log_prob_fun.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1637 2023-04-10 23:28:32.000000 modularbayes-0.1.4/examples/random_effects/main.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5650 2023-04-10 23:28:32.000000 modularbayes-0.1.4/examples/random_effects/plot.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17434 2023-04-10 13:07:24.000000 modularbayes-0.1.4/examples/random_effects/sample_mcmc.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18117 2023-06-24 17:43:50.000000 modularbayes-0.1.4/examples/random_effects/train_flow.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16758 2023-06-24 17:44:02.000000 modularbayes-0.1.4/examples/random_effects/train_vmp_flow.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18590 2023-06-23 23:29:39.000000 modularbayes-0.1.4/examples/random_effects/train_vmp_map.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.008889 modularbayes-0.1.4/modularbayes/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2068 2023-06-24 18:17:48.000000 modularbayes-0.1.4/modularbayes/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.008889 modularbayes-0.1.4/modularbayes/_src/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-14 17:37:23.000000 modularbayes-0.1.4/modularbayes/_src/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.012889 modularbayes-0.1.4/modularbayes/_src/bijectors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-14 17:37:23.000000 modularbayes-0.1.4/modularbayes/_src/bijectors/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4245 2023-04-10 23:28:32.000000 modularbayes-0.1.4/modularbayes/_src/bijectors/blockwise.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1663 2022-12-03 16:52:48.000000 modularbayes-0.1.4/modularbayes/_src/bijectors/conditional_bijector.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2022-12-03 16:46:59.000000 modularbayes-0.1.4/modularbayes/_src/bijectors/conditional_chain.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1920 2022-11-14 17:37:23.000000 modularbayes-0.1.4/modularbayes/_src/bijectors/conditional_masked_coupling.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.012889 modularbayes-0.1.4/modularbayes/_src/conditioners/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-26 22:28:20.000000 modularbayes-0.1.4/modularbayes/_src/conditioners/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2850 2023-06-24 10:29:53.000000 modularbayes-0.1.4/modularbayes/_src/conditioners/base.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.012889 modularbayes-0.1.4/modularbayes/_src/distributions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-14 17:37:23.000000 modularbayes-0.1.4/modularbayes/_src/distributions/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2022-11-14 17:37:23.000000 modularbayes-0.1.4/modularbayes/_src/distributions/conditional_transformed.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      712 2022-12-03 16:39:32.000000 modularbayes-0.1.4/modularbayes/_src/distributions/transformed.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.012889 modularbayes-0.1.4/modularbayes/_src/metaposterior/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-10 13:58:52.000000 modularbayes-0.1.4/modularbayes/_src/metaposterior/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2203 2023-06-24 10:30:03.000000 modularbayes-0.1.4/modularbayes/_src/metaposterior/vmp_map.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.012889 modularbayes-0.1.4/modularbayes/_src/smi/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6252 2023-06-24 13:10:00.000000 modularbayes-0.1.4/modularbayes/_src/smi/elbo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4797 2023-06-24 13:06:11.000000 modularbayes-0.1.4/modularbayes/_src/smi/sampling.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1459 2023-06-12 15:57:46.000000 modularbayes-0.1.4/modularbayes/_src/typing.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.016889 modularbayes-0.1.4/modularbayes/_src/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-14 17:37:23.000000 modularbayes-0.1.4/modularbayes/_src/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3840 2023-04-10 23:07:18.000000 modularbayes-0.1.4/modularbayes/_src/utils/misc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      882 2023-06-10 16:22:06.000000 modularbayes-0.1.4/modularbayes/_src/utils/training.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.008889 modularbayes-0.1.4/modularbayes.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5937 2023-06-24 18:17:59.000000 modularbayes-0.1.4/modularbayes.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2605 2023-06-24 18:17:59.000000 modularbayes-0.1.4/modularbayes.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-24 18:17:59.000000 modularbayes-0.1.4/modularbayes.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-03 16:33:35.000000 modularbayes-0.1.4/modularbayes.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-06-24 18:17:59.000000 modularbayes-0.1.4/modularbayes.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-06-24 18:17:59.000000 modularbayes-0.1.4/modularbayes.egg-info/top_level.txt
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 18:18:00.016889 modularbayes-0.1.4/requirements/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2022-11-14 17:37:23.000000 modularbayes-0.1.4/requirements/requirements-devel.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2022-11-14 17:37:23.000000 modularbayes-0.1.4/requirements/requirements-setup.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2022-12-03 17:43:43.000000 modularbayes-0.1.4/requirements/requirements-tests.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-06-24 10:33:14.000000 modularbayes-0.1.4/requirements/requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-24 18:18:00.016889 modularbayes-0.1.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2260 2022-11-14 17:37:23.000000 modularbayes-0.1.4/setup.py
```

### Comparing `modularbayes-0.1.3/LICENSE` & `modularbayes-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/PKG-INFO` & `modularbayes-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modularbayes
-Version: 0.1.3
+Version: 0.1.4
 Summary: Modular Bayesian Inference.
 Home-page: https://github.com/chriscarmona/modularbayes
 Author: Chris Carmona
 Author-email: carmona@stats.ox.ac.uk
 Maintainer-email: carmona@stats.ox.ac.uk
 License: MIT
 Keywords: modular bayesian inference cut smi posterior probability distribution
@@ -50,16 +50,15 @@
 ```bash
 pip install -Ur examples/requirements.txt
 chmod +x examples/run.sh
 bash examples/run.sh
 ```
 Results produced during the optimization can be monitored in [Tensorboard](https://www.tensorflow.org/tensorboard):
 ```bash
-WORK_DIR=$HOME/modularbayes-output
-tensorboard --logdir=$WORK_DIR
+tensorboard --logdir=$HOME/modularbayes-output
 ```
 
 ## Installation instructions
 
 1. \[Optional] Create a new virtual environment for this project (see [*Create a virtual environment*](#create-a-virtual-environment) below).
 2. Install JAX. This may vary according to your CUDA version (See [JAX installation](https://github.com/google/jax#installation)).
 3. Install the latest released version of `modularbayes` from [Pypi](https://pypi.org/project/modularbayes/) via:
```

### Comparing `modularbayes-0.1.3/README.md` & `modularbayes-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 ```bash
 pip install -Ur examples/requirements.txt
 chmod +x examples/run.sh
 bash examples/run.sh
 ```
 Results produced during the optimization can be monitored in [Tensorboard](https://www.tensorflow.org/tensorboard):
 ```bash
-WORK_DIR=$HOME/modularbayes-output
-tensorboard --logdir=$WORK_DIR
+tensorboard --logdir=$HOME/modularbayes-output
 ```
 
 ## Installation instructions
 
 1. \[Optional] Create a new virtual environment for this project (see [*Create a virtual environment*](#create-a-virtual-environment) below).
 2. Install JAX. This may vary according to your CUDA version (See [JAX installation](https://github.com/google/jax#installation)).
 3. Install the latest released version of `modularbayes` from [Pypi](https://pypi.org/project/modularbayes/) via:
```

### Comparing `modularbayes-0.1.3/examples/epidemiology/configs/flow_mf.py` & `modularbayes-0.1.4/examples/epidemiology/configs/flow_mf.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
   # How often to log images to monitor convergence.
   config.log_img_steps = config.training_steps / 10
 
   # Number of posteriors samples used in the plots.
   config.num_samples_plot = 40_000
 
   # How often to save model checkpoints.
-  config.checkpoint_steps = config.training_steps / 4
+  config.checkpoint_steps = config.training_steps / 2
 
   # How many checkpoints to keep.
   config.checkpoints_keep = 1
 
   config.num_samples_log_prob_test = 10_000
 
   return config
```

### Comparing `modularbayes-0.1.3/examples/epidemiology/configs/flow_mf_vmp_map.py` & `modularbayes-0.1.4/examples/epidemiology/configs/flow_mf_vmp_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   # Defined in `epidemiology.models.flows`.
   config.flow_name = 'mf'
 
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
 
   # Number of posteriors samples to approximate the variational loss (ELBO).
-  config.num_samples_elbo = 50
+  config.num_samples_elbo = 10
 
   # Number of training steps to run.
   config.training_steps = 10_000
 
   # Optimizer.
   config.optim_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.grad_clip_value = 1.0
@@ -69,14 +69,13 @@
 
   # Arguments for the Variational Meta-Posterior map
   config.vmp_map_name = 'MLPVmpMap'
   config.vmp_map_kwargs = ml_collections.ConfigDict()
   config.vmp_map_kwargs.hidden_sizes = [10] * 5
 
   # Number of samples of eta for Meta-Posterior training
-  config.num_samples_eta = 25
   config.eta_sampling_a = 0.2
   config.eta_sampling_b = 1.0
 
   config.vmpmap_curves_idx = [5 * i for i in range(5)]
 
   return config
```

### Comparing `modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf.py` & `modularbayes-0.1.4/examples/epidemiology/configs/flow_nsf.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf_vmp_flow.py` & `modularbayes-0.1.4/examples/epidemiology/configs/flow_nsf_vmp_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,23 @@
   config.prior_hparams.theta0_scale = 100.
   config.prior_hparams.theta1_concentration = 1
   config.prior_hparams.theta1_rate = 0.1
 
   config.method = 'vmp_flow'
 
   # Defined in `epidemiology.models.flows`.
-  config.flow_name = 'meta_nsf'
+  config.flow_name = 'nsf'
 
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
   # Number of layers to use in the flow.
   config.flow_kwargs.num_layers = 4
   # Hidden sizes
   # Hidden sizes of the MLP conditioner.
-  config.flow_kwargs.hidden_sizes_conditioner = [5] * 3
-  # Hidden sizes of the MLP conditioner for eta.
-  config.flow_kwargs.hidden_sizes_conditioner_eta = [5] * 3
+  config.flow_kwargs.hidden_sizes = [5] * 3
   # Number of bins to use in the rational-quadratic spline.
   config.flow_kwargs.num_bins = 10
   # the lower bound of the spline's range
   config.flow_kwargs.range_min = -10.
   # the upper bound of the spline's range
   config.flow_kwargs.range_max = 40.
```

### Comparing `modularbayes-0.1.3/examples/epidemiology/configs/flow_nsf_vmp_map.py` & `modularbayes-0.1.4/examples/epidemiology/configs/flow_nsf_vmp_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   config.flow_kwargs.num_bins = 10
   # the lower bound of the spline's range
   config.flow_kwargs.range_min = -10.
   # the upper bound of the spline's range
   config.flow_kwargs.range_max = 40.
 
   # Number of samples to approximate ELBO's gradient
-  config.num_samples_elbo = 100
+  config.num_samples_elbo = 10
 
   # Number of training steps to run.
   config.training_steps = 20_000
 
   # Optimizer.
   config.optim_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.grad_clip_value = 1.0
@@ -79,14 +79,13 @@
 
   # Arguments for the Variational Meta-Posterior map
   config.vmp_map_name = 'MLPVmpMap'
   config.vmp_map_kwargs = ml_collections.ConfigDict()
   config.vmp_map_kwargs.hidden_sizes = [10] * 5
 
   # Number of samples of eta for Meta-Posterior training
-  config.num_samples_eta = 25
   config.eta_sampling_a = 0.2
   config.eta_sampling_b = 1.0
 
   config.vmpmap_curves_idx = [50 * i for i in range(5)]
 
   return config
```

### Comparing `modularbayes-0.1.3/examples/epidemiology/configs/mcmc.py` & `modularbayes-0.1.4/examples/epidemiology/configs/mcmc.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/epidemiology/data/load.py` & `modularbayes-0.1.4/examples/epidemiology/data/load.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/epidemiology/flows.py` & `modularbayes-0.1.4/examples/epidemiology/flows.py`

 * *Files 20% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 def get_q_nocut_nsf(
     phi_dim: int,
     num_layers: int,
     hidden_sizes: Sequence[int],
     num_bins: int,
     range_min: float = 0.,
     range_max: float = 1.,
+    is_meta: bool = False,
     **_,
 ) -> distrax.Transformed:
   """Creates the Rational Quadratic Flow model.
 
   Args:
   range_min: the lower bound of the spline's range. Below `range_min`, the
     bijector defaults to a linear transformation.
@@ -146,43 +147,63 @@
 
   # Number of parameters for the rational-quadratic spline:
   # - `num_bins` bin widths
   # - `num_bins` bin heights
   # - `num_bins + 1` knot slopes
   # for a total of `3 * num_bins + 1` parameters.
   for _ in range(num_layers):
-    layer = distrax.MaskedCoupling(
-        mask=mask,
-        bijector=bijector_fn,
-        conditioner=modularbayes.MLPConditioner(
-            output_dim=math.prod(event_shape),
-            hidden_sizes=hidden_sizes,
-            num_bijector_params=num_bijector_params,
-            name='conditioner_nocut',
-        ),
-    )
+    if is_meta:
+      layer = modularbayes.ConditionalMaskedCoupling(
+          mask=mask,
+          bijector=bijector_fn,
+          conditioner=modularbayes.MLPConditioner(
+              output_dim=math.prod(event_shape),
+              hidden_sizes=hidden_sizes,
+              num_bijector_params=num_bijector_params,
+              name='conditioner_nocut',
+          ),
+      )
+    else:
+      layer = distrax.MaskedCoupling(
+          mask=mask,
+          bijector=bijector_fn,
+          conditioner=modularbayes.MLPConditioner(
+              output_dim=math.prod(event_shape),
+              hidden_sizes=hidden_sizes,
+              num_bijector_params=num_bijector_params,
+              name='conditioner_nocut',
+          ),
+      )
+
     flow_layers.append(layer)
     # Flip the mask after each layer.
     mask = jnp.logical_not(mask)
 
   # Last layer: Map values to parameter domain
   bij_nocut = bijector_domain_nocut()
   flow_layers.append(bij_nocut)
 
   # Chain all flow layers together
-  flow = distrax.Chain(flow_layers[::-1])
+  if is_meta:
+    flow = modularbayes.ConditionalChain(flow_layers[::-1])
+  else:
+    flow = distrax.Chain(flow_layers[::-1])
 
   # base_distribution = distrax.Independent(
   #     distrax.Uniform(low=jnp.zeros(event_shape), high=jnp.ones(event_shape)),
   #     reinterpreted_batch_ndims=len(event_shape))
 
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
-
-  return modularbayes.Transformed(base_distribution, flow)
+  if is_meta:
+    q_distr = modularbayes.ConditionalTransformed(base_distribution, flow)
+  else:
+    q_distr = modularbayes.Transformed(base_distribution, flow)
+    
+  return q_distr
 
 
 def get_q_cutgivennocut_nsf(
     theta_dim: int,
     num_layers: int,
     hidden_sizes: Sequence[int],
     num_bins: int,
@@ -250,174 +271,14 @@
 
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
   return modularbayes.ConditionalTransformed(base_distribution, flow)
 
 
-def get_q_nocut_meta_nsf(
-    phi_dim: int,
-    num_layers: int,
-    hidden_sizes_conditioner: Sequence[int],
-    hidden_sizes_conditioner_eta: Sequence[int],
-    num_bins: int,
-    range_min: float = 0.,
-    range_max: float = 1.,
-    **_,
-) -> modularbayes.ConditionalTransformed:
-  """Creates the Rational Quadratic Flow model.
-
-  Args:
-  range_min: the lower bound of the spline's range. Below `range_min`, the
-    bijector defaults to a linear transformation.
-  range_max: the upper bound of the spline's range. Above `range_max`, the
-    bijector defaults to a linear transformation.
-  """
-
-  flow_dim = phi_dim
-
-  event_shape = (flow_dim,)
-
-  flow_layers = []
-
-  # Number of parameters required by the bijector (rational quadratic spline)
-  num_bijector_params = 3 * num_bins + 1
-
-  def bijector_fn(params: Array):
-    return distrax.RationalQuadraticSpline(
-        params, range_min=range_min, range_max=range_max)
-
-  # Alternating binary mask.
-  mask = jnp.arange(0, math.prod(event_shape)) % 2
-  mask = jnp.reshape(mask, event_shape)
-  mask = mask.astype(bool)
-
-  # Number of parameters for the rational-quadratic spline:
-  # - `num_bins` bin widths
-  # - `num_bins` bin heights
-  # - `num_bins + 1` knot slopes
-  # for a total of `3 * num_bins + 1` parameters.
-
-  for _ in range(num_layers):
-    layer = modularbayes.EtaConditionalMaskedCoupling(
-        mask=mask,
-        bijector=bijector_fn,
-        conditioner_eta=modularbayes.MLPConditioner(
-            output_dim=math.prod(event_shape),
-            hidden_sizes=hidden_sizes_conditioner_eta,
-            num_bijector_params=num_bijector_params,
-            name='conditioner_eta_nocut',
-        ),
-        conditioner=modularbayes.MLPConditioner(
-            output_dim=math.prod(event_shape),
-            hidden_sizes=hidden_sizes_conditioner,
-            num_bijector_params=num_bijector_params,
-            name='conditioner_nocut',
-        ),
-    )
-    flow_layers.append(layer)
-    # Flip the mask after each layer.
-    mask = jnp.logical_not(mask)
-
-  # Last Layer: Map values to parameter domain
-  bij_nocut = bijector_domain_nocut()
-  flow_layers.append(bij_nocut)
-
-  # Chain all flow layers together
-  flow = modularbayes.ConditionalChain(flow_layers[::-1])
-
-  # base_distribution = distrax.Independent(
-  #     distrax.Uniform(low=jnp.zeros(event_shape), high=jnp.ones(event_shape)),
-  #     reinterpreted_batch_ndims=len(event_shape))
-
-  base_distribution = distrax.MultivariateNormalDiag(
-      loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
-
-  return modularbayes.ConditionalTransformed(base_distribution, flow)
-
-
-def get_q_cutgivennocut_meta_nsf(
-    theta_dim: int,
-    num_layers: int,
-    hidden_sizes_conditioner: Sequence[int],
-    hidden_sizes_conditioner_eta: Sequence[int],
-    num_bins: int,
-    range_min: float = 0.,
-    range_max: float = 1.,
-    **_,
-) -> modularbayes.ConditionalTransformed:
-  """Creates the Rational Quadratic Flow model.
-
-  Args:
-  range_min: the lower bound of the spline's range. Below `range_min`, the
-    bijector defaults to a linear transformation.
-  range_max: the upper bound of the spline's range. Above `range_max`, the
-    bijector defaults to a linear transformation.
-  """
-
-  flow_dim = theta_dim
-  event_shape = (flow_dim,)
-
-  flow_layers = []
-
-  # Number of parameters required by the bijector (rational quadratic spline)
-  num_bijector_params = 3 * num_bins + 1
-
-  def bijector_fn(params: Array):
-    return distrax.RationalQuadraticSpline(
-        params, range_min=range_min, range_max=range_max)
-
-  # Alternating binary mask.
-  mask = jnp.arange(0, math.prod(event_shape)) % 2
-  mask = jnp.reshape(mask, event_shape)
-  mask = mask.astype(bool)
-
-  # Number of parameters for the rational-quadratic spline:
-  # - `num_bins` bin widths
-  # - `num_bins` bin heights
-  # - `num_bins + 1` knot slopes
-  # for a total of `3 * num_bins + 1` parameters.
-
-  for _ in range(num_layers):
-    layer = modularbayes.EtaConditionalMaskedCoupling(
-        mask=mask,
-        bijector=bijector_fn,
-        conditioner_eta=modularbayes.MLPConditioner(
-            output_dim=math.prod(event_shape),
-            hidden_sizes=hidden_sizes_conditioner_eta,
-            num_bijector_params=num_bijector_params,
-            name='conditioner_eta_theta',
-        ),
-        conditioner=modularbayes.MLPConditioner(
-            # input_dim=math.prod(event_shape),
-            output_dim=math.prod(event_shape),
-            hidden_sizes=hidden_sizes_conditioner,
-            num_bijector_params=num_bijector_params,
-            name='conditioner_theta',
-        ),
-    )
-    flow_layers.append(layer)
-    # Flip the mask after each layer.
-    mask = jnp.logical_not(mask)
-
-  # Last layer: Map values to parameter domain
-  bij_cut = bijector_domain_cut()
-  flow_layers.append(bij_cut)
-
-  # Chain all flow layers together
-  flow = modularbayes.ConditionalChain(flow_layers[::-1])
-
-  base_distribution = distrax.MultivariateNormalDiag(
-      loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
-
-  q_distr = modularbayes.ConditionalTransformed(base_distribution, flow)
-
-  return q_distr
-
-
 def split_flow_nocut(
     concat_params: Array,
     phi_dim: int,
     **_,
 ) -> Dict[str, Any]:
   """Get model parameters by splitting samples from the flow."""
```

### Comparing `modularbayes-0.1.3/examples/epidemiology/log_prob_fun.py` & `modularbayes-0.1.4/examples/epidemiology/log_prob_fun.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/epidemiology/main.py` & `modularbayes-0.1.4/examples/epidemiology/main.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/epidemiology/plot.py` & `modularbayes-0.1.4/examples/epidemiology/plot.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/epidemiology/sample_mcmc.py` & `modularbayes-0.1.4/examples/epidemiology/sample_mcmc.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/epidemiology/train_flow.py` & `modularbayes-0.1.4/examples/epidemiology/train_flow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """Training a Normalizing Flow."""
+
 import pathlib
 
 from absl import logging
 
 import numpy as np
+from matplotlib import pyplot as plt
 
 from arviz import InferenceData
 
-from flax.metrics import tensorboard
-
 import jax
 from jax import numpy as jnp
-
+from flax.metrics import tensorboard
+from flax.training.train_state import TrainState
 import haiku as hk
 import optax
+import orbax.checkpoint
 
+import data
 import flows
 from flows import split_flow_nocut, split_flow_cut
-from log_prob_fun import ModelParams, ModelParamsCut, SmiEta, logprob_joint
+from log_prob_fun import logprob_joint, ModelParams, ModelParamsCut, SmiEta
 import plot
-import data
 
-from modularbayes import (sample_q_nocut, sample_q_cutgivennocut, sample_q,
-                          elbo_smi)
-from modularbayes._src.utils.training import TrainState
-from modularbayes import (flatten_dict, initial_state_ckpt, update_states,
-                          save_checkpoint)
+from modularbayes import (elbo_smi, flatten_dict, sample_q_nocut,
+                          sample_q_cutgivennocut, sample_q, train_step)
 from modularbayes._src.typing import (Any, Array, Callable, ConfigDict, Dict,
-                                      List, Optional, PRNGKey, Tuple)
+                                      Optional, PRNGKey, SmiPosteriorStates,
+                                      Tuple)
 
 # Set high precision for matrix multiplication in jax
 jax.config.update('jax_default_matmul_precision', 'float32')
 
 np.set_printoptions(suppress=True, precision=4)
 
 
@@ -42,14 +42,154 @@
           np.split(data.epidemiology.to_numpy(), 4, axis=-1)))
   dataset_dict = {
       key: jnp.array(value.squeeze()) for key, value in dataset_dict.items()
   }
   return dataset_dict
 
 
+def init_state_tuple(
+    prng_key: PRNGKey,
+    config: ConfigDict,
+    flow_get_fn_nocut: Callable,
+    flow_get_fn_cutgivennocut: Callable,
+    sample_shape: Tuple[int],
+    eta_values: Array,
+):
+  """Initialize states of the three normalizing flows."""
+  prng_seq = hk.PRNGSequence(prng_key)
+
+  state_list = []
+
+  # Initialize state of nocut model parameters
+  lambda_nocut_ = sample_q_nocut.init(
+      next(prng_seq),
+      flow_get_fn=flow_get_fn_nocut,
+      flow_kwargs=config.flow_kwargs,
+      split_flow_fn=split_flow_nocut,
+      sample_shape=sample_shape,
+      eta_values=eta_values,
+  )
+  state_list.append(
+      TrainState.create(
+          apply_fn=sample_q_nocut.apply,
+          params=lambda_nocut_,
+          tx=make_optimizer(**config.optim_kwargs),
+      ))
+
+  # Get an initial sample of the base distribution of nocut model params
+  nocut_base_sample_ = state_list[0].apply_fn(
+      state_list[0].params,
+      next(prng_seq),
+      flow_get_fn=flow_get_fn_nocut,
+      flow_kwargs=config.flow_kwargs,
+      split_flow_fn=split_flow_nocut,
+      sample_shape=sample_shape,
+      eta_values=eta_values,
+  )['sample_base']
+
+  # Initialize state of cut model parameters
+  lambda_cut_ = sample_q_cutgivennocut.init(
+      next(prng_seq),
+      flow_get_fn=flow_get_fn_cutgivennocut,
+      flow_kwargs=config.flow_kwargs,
+      split_flow_fn=split_flow_cut,
+      nocut_base_sample=nocut_base_sample_,
+      eta_values=eta_values,
+  )
+  state_list.append(
+      TrainState.create(
+          apply_fn=sample_q_cutgivennocut.apply,
+          params=lambda_cut_,
+          tx=make_optimizer(**config.optim_kwargs),
+      ))
+
+  # Initialize state of cut model parameters, the auxiliary copy
+  state_list.append(
+      TrainState.create(
+          apply_fn=sample_q_cutgivennocut.apply,
+          params=lambda_cut_,
+          tx=make_optimizer(**config.optim_kwargs),
+      ))
+
+  # Simply transform the list into a named tuple
+  state_tuple = SmiPosteriorStates(*state_list)
+
+  return state_tuple
+
+
+def print_trainable_params(
+    state_tuple: Tuple[TrainState],
+    prng_key: PRNGKey,
+    config: ConfigDict,
+    flow_get_fn_nocut: Callable,
+    flow_get_fn_cutgivennocut: Callable,
+    sample_shape: Tuple[int],
+    eta_values: Array,
+) -> None:
+  """Print a summary of the trainable parameters."""
+  prng_seq = hk.PRNGSequence(prng_key)
+
+  logging.info('\nFlow no-cut parameters:\n')
+  tabulate_fn_ = hk.experimental.tabulate(
+      f=lambda state_, prng_key_: state_.apply_fn(
+          state_.params,
+          prng_key_,
+          flow_get_fn=flow_get_fn_nocut,
+          flow_kwargs=config.flow_kwargs,
+          split_flow_fn=split_flow_nocut,
+          sample_shape=sample_shape,
+          eta_values=eta_values,
+      ),
+      columns=(
+          "module",
+          "owned_params",
+          "params_size",
+          "params_bytes",
+      ),
+      filters=("has_params",),
+  )
+  summary = tabulate_fn_(state_tuple[0], next(prng_seq))
+  for line in summary.split("\n"):
+    logging.info(line)
+
+  # Get an initial sample of the base distribution of nocut params
+  nocut_base_sample_ = state_tuple[0].apply_fn(
+      state_tuple[0].params,
+      next(prng_seq),
+      flow_get_fn=flow_get_fn_nocut,
+      flow_kwargs=config.flow_kwargs,
+      split_flow_fn=split_flow_nocut,
+      sample_shape=sample_shape,
+      eta_values=eta_values,
+  )['sample_base']
+
+  logging.info('\nFlow cut parameters:\n')
+  tabulate_fn_ = hk.experimental.tabulate(
+      f=lambda state_, prng_key_: state_.apply_fn(
+          state_.params,
+          prng_key_,
+          flow_get_fn=flow_get_fn_cutgivennocut,
+          flow_kwargs=config.flow_kwargs,
+          split_flow_fn=split_flow_cut,
+          nocut_base_sample=nocut_base_sample_,
+          eta_values=eta_values,
+      ),
+      columns=(
+          "module",
+          "owned_params",
+          "params_size",
+          "params_bytes",
+      ),
+      filters=("has_params",),
+  )
+  summary = tabulate_fn_(state_tuple[1], next(prng_seq))
+  for line in summary.split("\n"):
+    logging.info(line)
+
+
 def make_optimizer(
     lr_schedule_name,
     lr_schedule_kwargs,
     grad_clip_value,
 ) -> optax.GradientTransformation:
   """Define optimizer to train the Flow."""
   schedule = getattr(optax, lr_schedule_name)(**lr_schedule_kwargs)
@@ -57,15 +197,15 @@
   optimizer = optax.chain(*[
       optax.clip_by_global_norm(max_norm=grad_clip_value),
       optax.adabelief(learning_rate=schedule),
   ])
   return optimizer
 
 
-def loss(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
+def loss_fn(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
   """Define training loss function."""
 
   ### Compute ELBO ###
   elbo_dict = elbo_smi(lambda_tuple=params_tuple, *args, **kwargs)
 
   # Our loss is the Negative ELBO
   loss_avg = -(jnp.nanmean(elbo_dict['stage_1'] + elbo_dict['stage_2']))
@@ -76,22 +216,21 @@
 def sample_q_as_az(
     lambda_tuple: Tuple[hk.Params],
     dataset: Dict[str, Any],
     prng_key: PRNGKey,
     flow_get_fn_nocut: Callable,
     flow_get_fn_cutgivennocut: Callable,
     flow_kwargs: Dict[str, Any],
-    sample_shape: Optional[Tuple[int]] = None,
+    sample_shape: Optional[Tuple[int]],
     eta_values: Optional[Array] = None,
 ) -> InferenceData:
   """Plots to monitor during training."""
-  assert sample_shape is not None or eta_values is not None, (
-      'Either sample_shape or eta_values must be provided.')
-  assert sample_shape is None or eta_values is None, (
-      'Only one of sample_shape or eta_values must be provided.')
+  if eta_values is not None:
+    assert eta_values.ndim == 2
+    assert (eta_values.shape[0],) == sample_shape
   # Sample from flow
   q_distr_out = sample_q(
       lambda_tuple=lambda_tuple,
       prng_key=prng_key,
       flow_get_fn_nocut=flow_get_fn_nocut,
       flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
       flow_kwargs=flow_kwargs,
@@ -109,15 +248,15 @@
       dataset=dataset,
       model_params=model_params_az,
   )
   return az_data
 
 
 def train_and_evaluate(config: ConfigDict, workdir: str) -> TrainState:
-  """Execute model training and evaluation loop.
+  """Model training and evaluation.
 
   Args:
     config: Hyperparameter configuration for training and evaluation.
     workdir: Directory where the tensorboard summaries are written to.
 
   Returns:
     Final TrainState.
@@ -157,128 +296,63 @@
 
   # Functions that generate the NF for no-cut params
   flow_get_fn_nocut = getattr(flows, 'get_q_nocut_' + config.flow_name)
   # Functions that generate the NF for cut params (conditional on no-cut params)
   flow_get_fn_cutgivennocut = getattr(flows,
                                       'get_q_cutgivennocut_' + config.flow_name)
 
-  checkpoint_dir = str(pathlib.Path(workdir) / 'checkpoints')
-  state_list = []
-  state_name_list = []
-
-  state_name_list.append('lambda_nocut')
-  state_list.append(
-      initial_state_ckpt(
-          checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-          forward_fn=sample_q_nocut,
-          forward_fn_kwargs={
-              'flow_get_fn': flow_get_fn_nocut,
-              'flow_kwargs': config.flow_kwargs,
-              'split_flow_fn': split_flow_nocut,
-              'sample_shape': (config.num_samples_elbo,),
-          },
-          prng_key=next(prng_seq),
-          optimizer=make_optimizer(**config.optim_kwargs),
-      ))
-
-  # Get an initial sample of the base distribution of nocut params
-  nocut_base_sample_init = sample_q_nocut.apply(
-      state_list[0].params,
-      next(prng_seq),
-      flow_get_fn=flow_get_fn_nocut,
-      flow_kwargs=config.flow_kwargs,
-      split_flow_fn=split_flow_nocut,
+  # Initialize States of the three flows
+  state_tuple = init_state_tuple(
+      prng_key=next(prng_seq),
+      config=config,
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
       sample_shape=(config.num_samples_elbo,),
-  )['sample_base']
-
-  state_name_list.append('lambda_cut')
-  state_list.append(
-      initial_state_ckpt(
-          checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-          forward_fn=sample_q_cutgivennocut,
-          forward_fn_kwargs={
-              'flow_get_fn': flow_get_fn_cutgivennocut,
-              'flow_kwargs': config.flow_kwargs,
-              'split_flow_fn': split_flow_cut,
-              'nocut_base_sample': nocut_base_sample_init,
-          },
-          prng_key=next(prng_seq),
-          optimizer=make_optimizer(**config.optim_kwargs),
-      ))
-  if config.flow_kwargs.is_smi:
-    state_name_list.append('lambda_cut_aux')
-    state_list.append(
-        initial_state_ckpt(
-            checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-            forward_fn=sample_q_cutgivennocut,
-            forward_fn_kwargs={
-                'flow_get_fn': flow_get_fn_cutgivennocut,
-                'flow_kwargs': config.flow_kwargs,
-                'split_flow_fn': split_flow_cut,
-                'nocut_base_sample': nocut_base_sample_init,
-            },
-            prng_key=next(prng_seq),
-            optimizer=make_optimizer(**config.optim_kwargs),
-        ))
-
-  # Print a useful summary of the execution of the flow architecture.
-  logging.info('\nFlow no-cut parameters:\n')
-  tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda params, prng_key: sample_q_nocut.apply(
-          params,
-          prng_key,
-          flow_get_fn=flow_get_fn_nocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_nocut,
-          sample_shape=(config.num_samples_elbo,),
-      ),
-      columns=(
-          "module",
-          "owned_params",
-          "params_size",
-          "params_bytes",
-      ),
-      filters=("has_params",),
+      eta_values=None,
   )
-  summary = tabulate_fn_(state_list[0].params, next(prng_seq))
-  for line in summary.split("\n"):
-    logging.info(line)
 
-  logging.info('\nFlow cut parameters:\n')
-  tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda params, prng_key: sample_q_cutgivennocut.apply(
-          params,
-          prng_key,
-          flow_get_fn=flow_get_fn_cutgivennocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_cut,
-          nocut_base_sample=nocut_base_sample_init,
-      ),
-      columns=(
-          "module",
-          "owned_params",
-          "params_size",
-          "params_bytes",
-      ),
-      filters=("has_params",),
+  # Print a summary of the flow architecture
+  print_trainable_params(
+      state_tuple=state_tuple,
+      prng_key=next(prng_seq),
+      config=config,
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+      sample_shape=(config.num_samples_elbo,),
+      eta_values=None,
   )
-  summary = tabulate_fn_(state_list[1].params, next(prng_seq))
-  for line in summary.split("\n"):
-    logging.info(line)
+
+  # Create checkpoint managers for the three states
+  orbax_ckpt_mngrs = [
+      orbax.checkpoint.CheckpointManager(
+          directory=str(pathlib.Path(workdir) / 'checkpoints' / state_name),
+          checkpointers=orbax.checkpoint.PyTreeCheckpointer(),
+          options=orbax.checkpoint.CheckpointManagerOptions(
+              max_to_keep=1,
+              save_interval_steps=config.checkpoint_steps,
+          ),
+      ) for state_name in state_tuple._asdict()
+  ]
+
+  # Restore existing checkpoint if present
+  if orbax_ckpt_mngrs[0].latest_step() is not None:
+    state_tuple = [
+        mngr.restore(mngr.latest_step(), items=state)
+        for state, mngr in zip(state_tuple, orbax_ckpt_mngrs)
+    ]
 
   # Jit function to update training states
   @jax.jit
-  def update_states_jit(state_list, batch, prng_key, smi_eta):
-    return update_states(
-        state_list=state_list,
+  def train_step_jit(state_tuple, batch, prng_key):
+    return train_step(
+        state_tuple=state_tuple,
         batch=batch,
         prng_key=prng_key,
-        optimizer=make_optimizer(**config.optim_kwargs),
-        loss_fn=loss,
-        loss_fn_kwargs={
+        loss=loss_fn,
+        loss_kwargs={
             'num_samples': config.num_samples_elbo,
             'logprob_joint_fn': logprob_joint,
             'flow_get_fn_nocut': flow_get_fn_nocut,
             'flow_get_fn_cutgivennocut': flow_get_fn_cutgivennocut,
             'flow_kwargs': config.flow_kwargs,
             'prior_hparams': config.prior_hparams,
             'model_params_tupleclass': ModelParams,
@@ -286,17 +360,17 @@
             'split_flow_fn_nocut': split_flow_nocut,
             'split_flow_fn_cut': split_flow_cut,
             'smi_eta': smi_eta,
         },
     )
 
   @jax.jit
-  def elbo_validation_jit(state_list, batch, prng_key, smi_eta):
+  def elbo_validation_jit(state_tuple, batch, prng_key, smi_eta):
     return elbo_smi(
-        lambda_tuple=tuple(state.params for state in state_list),
+        lambda_tuple=tuple(state.params for state in state_tuple),
         batch=batch,
         prng_key=prng_key,
         num_samples=config.num_samples_eval,
         logprob_joint_fn=logprob_joint,
         flow_get_fn_nocut=flow_get_fn_nocut,
         flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
         flow_kwargs=config.flow_kwargs,
@@ -304,28 +378,28 @@
         model_params_tupleclass=ModelParams,
         model_params_cut_tupleclass=ModelParamsCut,
         split_flow_fn_nocut=split_flow_nocut,
         split_flow_fn_cut=split_flow_cut,
         smi_eta=smi_eta,
     )
 
-  if state_list[0].step < config.training_steps:
+  if state_tuple[0].step < config.training_steps:
     logging.info('Training variational posterior...')
 
   # Reset random key sequence
   prng_seq = hk.PRNGSequence(config.seed)
 
-  while state_list[0].step < config.training_steps:
+  while state_tuple[0].step < config.training_steps:
 
     # Plots to monitor training
-    if ((state_list[0].step == 0) or
-        (state_list[0].step % config.log_img_steps == 0)):
-      # print("Logging images...\n")
+    if ((state_tuple[0].step == 0) or
+        (state_tuple[0].step % config.log_img_steps == 0)):
+      logging.info("\t\t Logging plots...")
       az_data = sample_q_as_az(
-          lambda_tuple=tuple(x.params for x in state_list),
+          lambda_tuple=tuple(x.params for x in state_tuple),
           dataset=train_ds,
           prng_key=next(prng_seq),
           flow_get_fn_nocut=flow_get_fn_nocut,
           flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
           flow_kwargs=config.flow_kwargs,
           sample_shape=(config.num_samples_plot,),
       )
@@ -333,88 +407,75 @@
           az_data=az_data,
           show_phi_trace=False,
           show_theta_trace=False,
           show_loglinear_scatter=True,
           show_theta_pairplot=True,
           eta=config.smi_eta_cancer,
           suffix=f"_eta_cancer_{float(config.smi_eta_cancer):.3f}",
-          step=state_list[0].step,
+          step=state_tuple[0].step,
           workdir_png=workdir,
           summary_writer=summary_writer,
       )
+      plt.close()
+      logging.info("\t\t...done logging plots.")
 
     # Log learning rate
     summary_writer.scalar(
         tag='learning_rate',
         value=getattr(optax, config.optim_kwargs.lr_schedule_name)(
-            **config.optim_kwargs.lr_schedule_kwargs)(state_list[0].step),
-        step=state_list[0].step,
+            **config.optim_kwargs.lr_schedule_kwargs)(state_tuple[0].step),
+        step=state_tuple[0].step,
     )
 
     # SGD step
-    state_list, metrics = update_states_jit(
-        state_list=state_list,
+    state_tuple_, metrics = train_step_jit(
+        state_tuple=state_tuple,
         batch=train_ds,
         prng_key=next(prng_seq),
-        smi_eta=smi_eta,
     )
-    # The computed training loss corresponds to the model before update
+    if jax.lax.is_finite(metrics['train_loss']):
+      state_tuple = state_tuple_
+
     summary_writer.scalar(
         tag='train_loss',
         value=metrics['train_loss'],
-        step=state_list[0].step - 1,
+        step=state_tuple[0].step,
     )
 
-    if state_list[0].step == 1:
-      logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
+    if state_tuple[0].step == 1:
+      logging.info("STEP: %5d; training loss: %.3f", state_tuple[0].step,
                    metrics["train_loss"])
 
     # Metrics for evaluation
-    if state_list[0].step % config.eval_steps == 0:
-      logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
+    if state_tuple[0].step % config.eval_steps == 0:
+      logging.info("STEP: %5d; training loss: %.3f", state_tuple[0].step,
                    metrics["train_loss"])
 
       elbo_dict = elbo_validation_jit(
-          state_list=state_list,
+          state_tuple=state_tuple,
           batch=train_ds,
           prng_key=next(prng_seq),
           smi_eta=smi_eta,
       )
       for k, v in elbo_dict.items():
         summary_writer.scalar(
             tag=f'elbo_{k}',
             value=v.mean(),
-            step=state_list[0].step,
+            step=state_tuple[0].step,
         )
 
-    if state_list[0].step % config.checkpoint_steps == 0:
-      for state_i, state_name_i in zip(state_list, state_name_list):
-        save_checkpoint(
-            state=state_i,
-            checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-            keep=config.checkpoints_keep,
-        )
-
-    # Wait until computations are done before the next step
-    # jax.random.normal(jax.random.PRNGKey(0), ()).block_until_ready()
+    # Save checkpoints
+    for state, mngr in zip(state_tuple, orbax_ckpt_mngrs):
+      mngr.save(step=int(state.step), items=state)
 
-  logging.info('Final training step: %i', state_list[0].step)
-
-  # Saving checkpoint at the end of the training process
-  # (in case training_steps is not multiple of checkpoint_steps)
-  for state_i, state_name_i in zip(state_list, state_name_list):
-    save_checkpoint(
-        state=state_i,
-        checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-        keep=config.checkpoints_keep,
-    )
+  logging.info('Final training step: %i', state_tuple[0].step)
 
   # Last plot of posteriors
   az_data = sample_q_as_az(
-      lambda_tuple=tuple(x.params for x in state_list),
+      lambda_tuple=tuple(x.params for x in state_tuple),
       dataset=train_ds,
       prng_key=next(prng_seq),
       flow_get_fn_nocut=flow_get_fn_nocut,
       flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
       flow_kwargs=config.flow_kwargs,
       sample_shape=(config.num_samples_plot,),
   )
@@ -422,20 +483,20 @@
       az_data=az_data,
       show_phi_trace=False,
       show_theta_trace=False,
       show_loglinear_scatter=True,
       show_theta_pairplot=True,
       eta=config.smi_eta_cancer,
       suffix=f"_eta_cancer_{float(config.smi_eta_cancer):.3f}",
-      step=state_list[0].step,
+      step=state_tuple[0].step,
       workdir_png=workdir,
       summary_writer=summary_writer,
   )
 
-  return state_list
+  return state_tuple
 
 
 # # For debugging
 # config = get_config()
 # eta = 1.000
 # import pathlib
 # workdir = str(pathlib.Path.home() / f'modularbayes-output-exp/epidemiology/nsf/eta_{eta:.3f}')
```

### Comparing `modularbayes-0.1.3/examples/epidemiology/train_vmp_flow.py` & `modularbayes-0.1.4/examples/epidemiology/train_vmp_map.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,187 @@
-"""Training a Variational Meta-Posterior, using the VMP flow."""
+"""Training a Variational Meta-Posterior, using the VMP map."""
 
 import pathlib
 
 from absl import logging
 
 import numpy as np
 
-from arviz import InferenceData
-
-from flax.metrics import tensorboard
+from matplotlib import pyplot as plt
 
 import jax
 from jax import numpy as jnp
-
+from flax.metrics import tensorboard
+from flax.training.train_state import TrainState
 import haiku as hk
 import optax
+import orbax.checkpoint
 
 import flows
 from flows import split_flow_nocut, split_flow_cut
-from log_prob_fun import (ModelParams, ModelParamsCut, SmiEta, logprob_joint,
-                          sample_eta_values)
+from log_prob_fun import (logprob_joint, sample_eta_values, ModelParams,
+                          ModelParamsCut, SmiEta)
 import plot
-from train_flow import load_data, make_optimizer, sample_q_as_az
+from train_flow import init_state_tuple, load_data, sample_q_as_az
 
-from modularbayes import (sample_q_nocut, sample_q_cutgivennocut,
-                          elbo_smi_vmpflow)
-from modularbayes._src.utils.training import TrainState
-from modularbayes import (flatten_dict, initial_state_ckpt, update_states,
-                          save_checkpoint)
+import modularbayes
+from modularbayes import (elbo_smi_vmpmap, flatten_dict, plot_to_image,
+                          train_step)
 from modularbayes._src.typing import (Any, Array, Callable, ConfigDict, Dict,
-                                      List, Optional, PRNGKey, Tuple)
+                                      Optional, PRNGKey, SmiPosteriorStates,
+                                      Tuple)
 
 # Set high precision for matrix multiplication in jax
 jax.config.update('jax_default_matmul_precision', 'float32')
 
 np.set_printoptions(suppress=True, precision=4)
 
 
-def loss(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
+def make_optimizer(
+    lr_schedule_name,
+    lr_schedule_kwargs,
+    grad_clip_value,
+) -> optax.GradientTransformation:
+  """Define optimizer to train the VHP map."""
+  schedule = getattr(optax, lr_schedule_name)(**lr_schedule_kwargs)
+
+  optimizer = optax.chain(*[
+      optax.clip_by_global_norm(max_norm=grad_clip_value),
+      optax.adabelief(learning_rate=schedule),
+  ])
+  return optimizer
+
+
+def print_trainable_params(
+    state_tuple: Tuple[TrainState],
+    config: ConfigDict,
+    lambda_init_tuple: Tuple,
+) -> None:
+  """Print a summary of the trainable parameters."""
+  tabulate_fn_ = hk.experimental.tabulate(
+      f=lambda state_i, lambda_init_i: state_i.apply_fn(
+          state_i.params,
+          eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
+          lambda_init=lambda_init_i),
+      columns=(
+          "module",
+          "owned_params",
+          "params_size",
+          "params_bytes",
+      ),
+      filters=("has_params",),
+  )
+  summary = tabulate_fn_(state_tuple[0], lambda_init_tuple[0])
+  logging.info('VMP-MAP no-cut parameters:')
+  for line in summary.split("\n"):
+    logging.info(line)
+
+  summary = tabulate_fn_(state_tuple[1], lambda_init_tuple[1])
+  logging.info('VMP-MAP cut parameters:')
+  for line in summary.split("\n"):
+    logging.info(line)
+
+
+def loss_fn(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
   """Define training loss function."""
 
-  ### Compute ELBO ###
-  elbo_dict = elbo_smi_vmpflow(lambda_tuple=params_tuple, *args, **kwargs)
+  # Compute ELBO.
+  elbo_dict = elbo_smi_vmpmap(alpha_tuple=params_tuple, *args, **kwargs)
 
   # Our loss is the Negative ELBO
   loss_avg = -(jnp.nanmean(elbo_dict['stage_1'] + elbo_dict['stage_2']))
 
   return loss_avg
 
 
 def log_images(
-    state_list: List[TrainState],
+    state_tuple: Tuple[TrainState],
     prng_key: PRNGKey,
     config: ConfigDict,
     dataset: Dict[str, Any],
     num_samples_plot: int,
+    vmpmap_fn: hk.Transformed,
+    lambda_init_tuple: Tuple[hk.Params],
     flow_get_fn_nocut: Callable,
     flow_get_fn_cutgivennocut: Callable,
+    vmpmap_curves_idx: Tuple[int],
     summary_writer: Optional[tensorboard.SummaryWriter] = None,
     workdir_png: Optional[str] = None,
 ) -> None:
   """Plots to monitor during training."""
 
   prng_seq = hk.PRNGSequence(prng_key)
 
   assert len(config.smi_eta_cancer_plot) > 0, 'No eta values to plot'
   assert all((x >= 0.0) and (x <= 1.0)
              for x in config.smi_eta_cancer_plot), 'Invalid eta values'
 
-  # Plot posterior samples
-  for eta_cancer_i in config.smi_eta_cancer_plot:
-    # Define eta with a single value
-    smi_etas = SmiEta(
-        hpv=jnp.ones(num_samples_plot),
-        cancer=eta_cancer_i * jnp.ones(num_samples_plot),
-    )
-    # Sample from flow
+  # We can obtain the variational parameters for all eta values at once
+  smi_etas = SmiEta(
+      hpv=jnp.ones(len(config.smi_eta_cancer_plot)),
+      cancer=jnp.array(config.smi_eta_cancer_plot),
+  )
+  eta_values = (
+      smi_etas[0] if len(smi_etas) == 1 else jnp.stack(smi_etas, axis=-1))
+  # Produce flow parameters as a function of eta
+  lambda_tuple = [
+      state_i.apply_fn(
+          state_i.params,
+          eta_values=eta_values,
+          lambda_init=lambda_i,
+      ) for state_i, lambda_i in zip(state_tuple, lambda_init_tuple)
+  ]
+
+  # Sample from flows and plot, one eta at a time
+  for i, eta_i in enumerate(config.smi_eta_cancer_plot):
     az_data = sample_q_as_az(
-        lambda_tuple=tuple(x.params for x in state_list),
+        lambda_tuple=jax.tree_map(lambda x: x[i], lambda_tuple),
         dataset=dataset,
         prng_key=next(prng_seq),
         flow_get_fn_nocut=flow_get_fn_nocut,
         flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
         flow_kwargs=config.flow_kwargs,
-        eta_values=(smi_etas[0] if len(smi_etas) == 1 else jnp.stack(
-            smi_etas, axis=-1)),
+        sample_shape=(num_samples_plot,),
     )
     plot.posterior_plots(
         az_data=az_data,
         show_phi_trace=False,
         show_theta_trace=False,
         show_loglinear_scatter=True,
         show_theta_pairplot=True,
-        eta=eta_cancer_i,
-        suffix=f"_eta_cancer_{float(eta_cancer_i):.3f}",
-        step=state_list[0].step,
+        eta=eta_i,
+        suffix=f"_eta_cancer_{float(eta_i):.3f}",
+        step=state_tuple[0].step,
         workdir_png=workdir_png,
         summary_writer=summary_writer,
     )
 
+  # Plot a few curves representing the VMP map for the no-cut parameters
+  model_name = 'epidemiology'
+  fig, _ = plot.plot_vmp_map(
+      alpha=state_tuple[0].params,
+      vmpmap_fn=vmpmap_fn,
+      lambda_init=lambda_init_tuple[0],
+      lambda_idx_to_plot=vmpmap_curves_idx,
+      eta_cancer_grid=jnp.linspace(0.0, 1.0, 101).round(3),
+  )
+  fig.suptitle("Example of VMP map curves")
+  fig.tight_layout()
+  if workdir_png:
+    plot_name = f"{model_name}_vmpmap_example_curves"
+    fig.savefig(pathlib.Path(workdir_png) / (plot_name + ".png"))
+  image = plot_to_image(fig)
+  if summary_writer:
+    plot_name = f"{model_name}_vmpmap_example_curves"
+    summary_writer.image(
+        tag=plot_name,
+        image=image,
+        step=state_tuple[0].step,
+    )
+
 
 def train_and_evaluate(config: ConfigDict, workdir: str) -> TrainState:
   """Execute model training and evaluation loop.
 
   Args:
     config: Hyperparameter configuration for training and evaluation.
     workdir: Directory where the tensorboard summaries are written to.
@@ -117,22 +196,18 @@
   # Initialize random keys
   prng_seq = hk.PRNGSequence(config.seed)
 
   # Full dataset used everytime
   # Small data, no need to batch
   train_ds = load_data()
 
-  phi_dim = train_ds['Z'].shape[0]
-  theta_dim = 2
-
   # phi_dim and theta_dim are also arguments of the flow,
   # as they define its dimension
-  config.flow_kwargs.phi_dim = phi_dim
-  config.flow_kwargs.theta_dim = theta_dim
-  # Also is_smi modifies the dimension of the flow, due to the duplicated params
+  config.flow_kwargs.phi_dim = train_ds['Z'].shape[0]
+  config.flow_kwargs.theta_dim = 2
   config.flow_kwargs.is_smi = True
 
   # writer = metric_writers.create_default_writer(
   #     logdir=workdir, just_logging=jax.host_id() != 0)
   if jax.process_index() == 0:
     summary_writer = tensorboard.SummaryWriter(workdir)
     summary_writer.hparams(flatten_dict(config))
@@ -141,288 +216,194 @@
 
   # Functions that generate the NF for no-cut params
   flow_get_fn_nocut = getattr(flows, 'get_q_nocut_' + config.flow_name)
   # Functions that generate the NF for cut params (conditional on no-cut params)
   flow_get_fn_cutgivennocut = getattr(flows,
                                       'get_q_cutgivennocut_' + config.flow_name)
 
-  checkpoint_dir = str(pathlib.Path(workdir) / 'checkpoints')
-  state_list = []
-  state_name_list = []
-
-  state_name_list.append('lambda_nocut')
-  state_list.append(
-      initial_state_ckpt(
-          checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-          forward_fn=sample_q_nocut,
-          forward_fn_kwargs={
-              'flow_get_fn':
-                  flow_get_fn_nocut,
-              'flow_kwargs':
-                  config.flow_kwargs,
-              'split_flow_fn':
-                  split_flow_nocut,
-              'eta_values':
-                  jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
-          },
-          prng_key=next(prng_seq),
-          optimizer=make_optimizer(**config.optim_kwargs),
-      ))
-
-  # Get an initial sample of the base distribution of nocut params
-  nocut_base_sample_init = sample_q_nocut.apply(
-      state_list[0].params,
-      next(prng_seq),
-      flow_get_fn=flow_get_fn_nocut,
-      flow_kwargs=config.flow_kwargs,
-      split_flow_fn=split_flow_nocut,
-      eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
-  )['sample_base']
-
-  state_name_list.append('lambda_cut')
-  state_list.append(
-      initial_state_ckpt(
-          checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-          forward_fn=sample_q_cutgivennocut,
-          forward_fn_kwargs={
-              'flow_get_fn':
-                  flow_get_fn_cutgivennocut,
-              'flow_kwargs':
-                  config.flow_kwargs,
-              'split_flow_fn':
-                  split_flow_cut,
-              'nocut_base_sample':
-                  nocut_base_sample_init,
-              'eta_values':
-                  jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
-          },
-          prng_key=next(prng_seq),
-          optimizer=make_optimizer(**config.optim_kwargs),
-      ))
-  if config.flow_kwargs.is_smi:
-    state_name_list.append('lambda_cut_aux')
-    state_list.append(
-        initial_state_ckpt(
-            checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-            forward_fn=sample_q_cutgivennocut,
-            forward_fn_kwargs={
-                'flow_get_fn':
-                    flow_get_fn_cutgivennocut,
-                'flow_kwargs':
-                    config.flow_kwargs,
-                'split_flow_fn':
-                    split_flow_cut,
-                'nocut_base_sample':
-                    nocut_base_sample_init,
-                'eta_values':
-                    jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
-            },
-            prng_key=next(prng_seq),
-            optimizer=make_optimizer(**config.optim_kwargs),
-        ))
-
-  # Print a useful summary of the execution of the flow architecture.
-  logging.info('\nFlow no-cut parameters:\n')
-  tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda params, prng_key: sample_q_nocut.apply(
-          params,
-          prng_key,
-          flow_get_fn=flow_get_fn_nocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_nocut,
-          eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
-      ),
-      columns=(
-          "module",
-          "owned_params",
-          "params_size",
-          "params_bytes",
-      ),
-      filters=("has_params",),
+  # To initialize the VMP-map, we need one example of its output
+  # The output of the VMP-map is lambda, the parameters of the variational posterior
+  lambda_init_tuple = init_state_tuple(
+      prng_key=next(prng_seq),
+      config=config,
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+      sample_shape=(config.num_samples_elbo,),
+      eta_values=None,
   )
-  summary = tabulate_fn_(state_list[0].params, next(prng_seq))
-  for line in summary.split("\n"):
-    logging.info(line)
+  lambda_init_tuple = [x.params for x in lambda_init_tuple]
 
-  logging.info('\nFlow cut parameters:\n')
-  tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda params, prng_key: sample_q_cutgivennocut.apply(
-          params,
-          prng_key,
-          flow_get_fn=flow_get_fn_cutgivennocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_cut,
-          nocut_base_sample=nocut_base_sample_init,
+  # Define function that produce a tuple of lambda (flow parameters)
+  @hk.without_apply_rng
+  @hk.transform
+  def vmpmap_fn(eta_values, lambda_init):
+    vmpmap = getattr(modularbayes, config.vmp_map_name)(
+        **config.vmp_map_kwargs, params_flow_init=lambda_init)
+    lambda_out = vmpmap(eta_values)
+    return lambda_out
+
+  ### Initialise Variational Meta-Posterior Map ###
+  params_tuple_ = [
+      vmpmap_fn.init(
+          next(prng_seq),
           eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
-      ),
-      columns=(
-          "module",
-          "owned_params",
-          "params_size",
-          "params_bytes",
-      ),
-      filters=("has_params",),
+          lambda_init=lambda_init_) for lambda_init_ in lambda_init_tuple
+  ]
+  state_tuple = SmiPosteriorStates(*[
+      TrainState.create(
+          apply_fn=vmpmap_fn.apply,
+          params=params_,
+          tx=make_optimizer(**config.optim_kwargs),
+      ) for params_ in params_tuple_
+  ])
+
+  print_trainable_params(
+      state_tuple=state_tuple,
+      config=config,
+      lambda_init_tuple=lambda_init_tuple,
   )
-  summary = tabulate_fn_(state_list[1].params, next(prng_seq))
-  for line in summary.split("\n"):
-    logging.info(line)
+
+  # Create checkpoint managers for the three states
+  orbax_ckpt_mngrs = [
+      orbax.checkpoint.CheckpointManager(
+          directory=str(pathlib.Path(workdir) / 'checkpoints' / state_name),
+          checkpointers=orbax.checkpoint.PyTreeCheckpointer(),
+          options=orbax.checkpoint.CheckpointManagerOptions(
+              max_to_keep=1,
+              save_interval_steps=config.checkpoint_steps,
+          ),
+      ) for state_name in state_tuple._asdict()
+  ]
+
+  # Restore existing checkpoint if present
+  if orbax_ckpt_mngrs[0].latest_step() is not None:
+    state_tuple = [
+        mngr.restore(mngr.latest_step(), items=state)
+        for state, mngr in zip(state_tuple, orbax_ckpt_mngrs)
+    ]
 
   # Jit function to update training states
   @jax.jit
-  def update_states_jit(state_list, batch, prng_key):
-    return update_states(
-        state_list=state_list,
+  def train_step_jit(state_tuple, batch, prng_key):
+    return train_step(
+        state_tuple=state_tuple,
         batch=batch,
         prng_key=prng_key,
-        optimizer=make_optimizer(**config.optim_kwargs),
-        loss_fn=loss,
-        loss_fn_kwargs={
+        loss=loss_fn,
+        loss_kwargs={
             'num_samples': config.num_samples_elbo,
-            'logprob_joint_fn': logprob_joint,
-            'flow_get_fn_nocut': flow_get_fn_nocut,
-            'flow_get_fn_cutgivennocut': flow_get_fn_cutgivennocut,
-            'flow_kwargs': config.flow_kwargs,
-            'prior_hparams': config.prior_hparams,
-            'model_params_tupleclass': ModelParams,
-            'model_params_cut_tupleclass': ModelParamsCut,
-            'split_flow_fn_nocut': split_flow_nocut,
-            'split_flow_fn_cut': split_flow_cut,
+            'vmpmap_fn': vmpmap_fn,
+            'lambda_init_tuple': lambda_init_tuple,
             'sample_eta_fn': sample_eta_values,
             'sample_eta_kwargs': {
                 'eta_sampling_a': config.eta_sampling_a,
                 'eta_sampling_b': config.eta_sampling_b
             },
+            'elbo_smi_kwargs': {
+                'logprob_joint_fn': logprob_joint,
+                'flow_get_fn_nocut': flow_get_fn_nocut,
+                'flow_get_fn_cutgivennocut': flow_get_fn_cutgivennocut,
+                'flow_kwargs': config.flow_kwargs,
+                'prior_hparams': config.prior_hparams,
+                'model_params_tupleclass': ModelParams,
+                'model_params_cut_tupleclass': ModelParamsCut,
+                'split_flow_fn_nocut': split_flow_nocut,
+                'split_flow_fn_cut': split_flow_cut,
+            }
         },
     )
 
-  @jax.jit
-  def elbo_validation_jit(state_list, batch, prng_key):
-    return elbo_smi_vmpflow(
-        lambda_tuple=tuple(state.params for state in state_list),
-        batch=batch,
-        prng_key=prng_key,
-        num_samples=config.num_samples_eval,
-        logprob_joint_fn=logprob_joint,
-        flow_get_fn_nocut=flow_get_fn_nocut,
-        flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
-        flow_kwargs=config.flow_kwargs,
-        prior_hparams=config.prior_hparams,
-        model_params_tupleclass=ModelParams,
-        model_params_cut_tupleclass=ModelParamsCut,
-        split_flow_fn_nocut=split_flow_nocut,
-        split_flow_fn_cut=split_flow_cut,
-        sample_eta_fn=sample_eta_values,
-        sample_eta_kwargs={
-            'eta_sampling_a': 1.,
-            'eta_sampling_b': 1.
-        },
-    )
-
-  if state_list[0].step < config.training_steps:
-    logging.info('Training Variational Meta-Posterior (VMP-flow)...')
+  if state_tuple[0].step < config.training_steps:
+    logging.info('Training Variational Meta-Posterior (VMP-map)...')
 
   # Reset random key sequence
   prng_seq = hk.PRNGSequence(config.seed)
 
-  while state_list[0].step < config.training_steps:
+  while state_tuple[0].step < config.training_steps:
 
     # Plots to monitor training
-    if ((state_list[0].step == 0) or
-        (state_list[0].step % config.log_img_steps == 0)):
-      # print("Logging images...\n")
+    if (config.log_img_steps
+        is not None) and (state_tuple[0].step % config.log_img_steps == 0):
+      logging.info("\t\t Logging plots...")
       log_images(
-          state_list=state_list,
+          state_tuple=state_tuple,
           prng_key=next(prng_seq),
           config=config,
           dataset=train_ds,
           num_samples_plot=config.num_samples_plot,
+          vmpmap_fn=vmpmap_fn,
+          lambda_init_tuple=lambda_init_tuple,
           flow_get_fn_nocut=flow_get_fn_nocut,
           flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+          vmpmap_curves_idx=config.vmpmap_curves_idx,
           summary_writer=summary_writer,
           workdir_png=workdir,
       )
+      plt.close()
+      logging.info("\t\t...done logging plots.")
 
     # Log learning rate
     summary_writer.scalar(
         tag='learning_rate',
         value=getattr(optax, config.optim_kwargs.lr_schedule_name)(
-            **config.optim_kwargs.lr_schedule_kwargs)(state_list[0].step),
-        step=state_list[0].step,
+            **config.optim_kwargs.lr_schedule_kwargs)(state_tuple[0].step),
+        step=state_tuple[0].step,
     )
 
     # SGD step
-    state_list, metrics = update_states_jit(
-        state_list=state_list,
+    state_tuple_, metrics = train_step_jit(
+        state_tuple=state_tuple,
         batch=train_ds,
         prng_key=next(prng_seq),
     )
-    # The computed training loss corresponds to the model before update
+    if jax.lax.is_finite(metrics['train_loss']):
+      state_tuple = state_tuple_
+
+    # The computed training loss would correspond to the model before update
     summary_writer.scalar(
         tag='train_loss',
         value=metrics['train_loss'],
-        step=state_list[0].step - 1,
+        step=state_tuple[0].step - 1,
     )
 
-    if state_list[0].step == 1:
-      logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
+    if state_tuple[0].step == 2:
+      logging.info("STEP: %5d; training loss: %.3f", state_tuple[0].step - 1,
                    metrics["train_loss"])
 
-    # Metrics for evaluation
-    if state_list[0].step % config.eval_steps == 0:
-      logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
+    if state_tuple[0].step % config.eval_steps == 0:
+      logging.info("STEP: %5d; training loss: %.3f", state_tuple[0].step - 1,
                    metrics["train_loss"])
 
-      elbo_dict = elbo_validation_jit(
-          state_list=state_list,
-          batch=train_ds,
-          prng_key=next(prng_seq),
-      )
-      for k, v in elbo_dict.items():
-        summary_writer.scalar(
-            tag=f'elbo_{k}',
-            value=v.mean(),
-            step=state_list[0].step,
-        )
-
-    if state_list[0].step % config.checkpoint_steps == 0:
-      for state_i, state_name_i in zip(state_list, state_name_list):
-        save_checkpoint(
-            state=state_i,
-            checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-            keep=config.checkpoints_keep,
-        )
+    # Save checkpoints
+    for state, mngr in zip(state_tuple, orbax_ckpt_mngrs):
+      mngr.save(step=int(state.step), items=state)
 
     # Wait until computations are done before the next step
     # jax.random.normal(jax.random.PRNGKey(0), ()).block_until_ready()
 
-  logging.info('Final training step: %i', state_list[0].step)
-
-  # Saving checkpoint at the end of the training process
-  # (in case training_steps is not multiple of checkpoint_steps)
-  for state_i, state_name_i in zip(state_list, state_name_list):
-    save_checkpoint(
-        state=state_i,
-        checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-        keep=config.checkpoints_keep,
-    )
+  logging.info('Final training step: %i', state_tuple[0].step)
 
   # Last plot of posteriors
   log_images(
-      state_list=state_list,
+      state_tuple=state_tuple,
       prng_key=next(prng_seq),
       config=config,
       dataset=train_ds,
       num_samples_plot=config.num_samples_plot,
+      vmpmap_fn=vmpmap_fn,
+      lambda_init_tuple=lambda_init_tuple,
       flow_get_fn_nocut=flow_get_fn_nocut,
       flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+      vmpmap_curves_idx=config.vmpmap_curves_idx,
       summary_writer=summary_writer,
       workdir_png=workdir,
   )
+  plt.close()
 
-  return state_list
+  return state_tuple
 
 
 # # For debugging
 # config = get_config()
 # import pathlib
-# workdir = str(pathlib.Path.home() / f'modularbayes-output-exp/epidemiology/vmp_nsf')
+# workdir = str(pathlib.Path.home() / f'modularbayes-output-exp/epidemiology/nsf/vmp_map')
 # # train_and_evaluate(config, workdir)
```

### Comparing `modularbayes-0.1.3/examples/epidemiology/train_vmp_map.py` & `modularbayes-0.1.4/examples/epidemiology/train_vmp_flow.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,166 +1,107 @@
-"""Training a Variational Meta-Posterior, using the VMP map."""
+"""Training a Variational Meta-Posterior, using the VMP flow."""
 
 import pathlib
 
 from absl import logging
 
 import numpy as np
-
 from matplotlib import pyplot as plt
 
-from flax.metrics import tensorboard
-
 import jax
 from jax import numpy as jnp
-
+from flax.metrics import tensorboard
+from flax.training.train_state import TrainState
 import haiku as hk
 import optax
-
-from tensorflow_probability.substrates import jax as tfp
+import orbax.checkpoint
 
 import flows
 from flows import split_flow_nocut, split_flow_cut
-import plot
-from train_flow import load_data, sample_q_as_az
 from log_prob_fun import (ModelParams, ModelParamsCut, SmiEta, logprob_joint,
                           sample_eta_values)
-
-import modularbayes
-from modularbayes import (sample_q_nocut, sample_q_cutgivennocut,
-                          elbo_smi_vmpmap)
-from modularbayes import (flatten_dict, plot_to_image, initial_state_ckpt,
-                          update_states, save_checkpoint)
-from modularbayes._src.utils.training import TrainState
+import plot
+from train_flow import (init_state_tuple, load_data, print_trainable_params,
+                        sample_q_as_az)
+from modularbayes import elbo_smi_vmpflow, flatten_dict, train_step
 from modularbayes._src.typing import (Any, Array, Callable, ConfigDict, Dict,
-                                      List, Optional, PRNGKey, Tuple)
-
-kernels = tfp.math.psd_kernels
+                                      Optional, PRNGKey, Tuple)
 
 # Set high precision for matrix multiplication in jax
 jax.config.update('jax_default_matmul_precision', 'float32')
 
 np.set_printoptions(suppress=True, precision=4)
 
 
-def make_optimizer(
-    lr_schedule_name,
-    lr_schedule_kwargs,
-    grad_clip_value,
-) -> optax.GradientTransformation:
-  """Define optimizer to train the VHP map."""
-  schedule = getattr(optax, lr_schedule_name)(**lr_schedule_kwargs)
-
-  optimizer = optax.chain(*[
-      optax.clip_by_global_norm(max_norm=grad_clip_value),
-      optax.adabelief(learning_rate=schedule),
-  ])
-  return optimizer
-
-
-def loss(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
+def loss_fn(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
   """Define training loss function."""
 
-  # Compute ELBO.
-  elbo_dict = elbo_smi_vmpmap(alpha_tuple=params_tuple, *args, **kwargs)
+  ### Compute ELBO ###
+  elbo_dict = elbo_smi_vmpflow(lambda_tuple=params_tuple, *args, **kwargs)
 
   # Our loss is the Negative ELBO
   loss_avg = -(jnp.nanmean(elbo_dict['stage_1'] + elbo_dict['stage_2']))
 
   return loss_avg
 
 
 def log_images(
-    state_list: Tuple[TrainState],
+    state_tuple: Tuple[TrainState],
     prng_key: PRNGKey,
     config: ConfigDict,
     dataset: Dict[str, Any],
     num_samples_plot: int,
-    vmpmap_fn: hk.Transformed,
-    lambda_init_list: List[hk.Params],
     flow_get_fn_nocut: Callable,
     flow_get_fn_cutgivennocut: Callable,
-    vmpmap_curves_idx: Tuple[int],
     summary_writer: Optional[tensorboard.SummaryWriter] = None,
     workdir_png: Optional[str] = None,
 ) -> None:
   """Plots to monitor during training."""
 
   prng_seq = hk.PRNGSequence(prng_key)
 
   assert len(config.smi_eta_cancer_plot) > 0, 'No eta values to plot'
   assert all((x >= 0.0) and (x <= 1.0)
              for x in config.smi_eta_cancer_plot), 'Invalid eta values'
 
-  # We can obtain the variational parameters for all eta values at once
-  smi_etas = SmiEta(
-      hpv=jnp.ones(len(config.smi_eta_cancer_plot)),
-      cancer=jnp.array(config.smi_eta_cancer_plot),
-  )
-  eta_values = (
-      smi_etas[0] if len(smi_etas) == 1 else jnp.stack(smi_etas, axis=-1))
-  # Produce flow parameters as a function of eta
-  lambda_tuple = [
-      vmpmap_fn.apply(
-          state_i.params,
-          eta_values=eta_values,
-          lambda_init=lambda_i,
-      ) for state_i, lambda_i in zip(state_list, lambda_init_list)
-  ]
-
-  # Sample from flows and plot, one eta at a time
-  for i, eta_i in enumerate(config.smi_eta_cancer_plot):
+  # Plot posterior samples
+  for eta_cancer_i in config.smi_eta_cancer_plot:
+    # Define eta with a single value
+    smi_etas = SmiEta(
+        hpv=jnp.ones(num_samples_plot),
+        cancer=eta_cancer_i * jnp.ones(num_samples_plot),
+    )
+    # Sample from flow
     az_data = sample_q_as_az(
-        lambda_tuple=jax.tree_map(lambda x: x[i], lambda_tuple),
+        lambda_tuple=tuple(x.params for x in state_tuple),
         dataset=dataset,
         prng_key=next(prng_seq),
         flow_get_fn_nocut=flow_get_fn_nocut,
         flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
         flow_kwargs=config.flow_kwargs,
         sample_shape=(num_samples_plot,),
+        eta_values=(smi_etas[0] if len(smi_etas) == 1 else jnp.stack(
+            smi_etas, axis=-1)),
     )
     plot.posterior_plots(
         az_data=az_data,
         show_phi_trace=False,
         show_theta_trace=False,
         show_loglinear_scatter=True,
         show_theta_pairplot=True,
-        eta=eta_i,
-        suffix=f"_eta_cancer_{float(eta_i):.3f}",
-        step=state_list[0].step,
+        eta=eta_cancer_i,
+        suffix=f"_eta_cancer_{float(eta_cancer_i):.3f}",
+        step=state_tuple[0].step,
         workdir_png=workdir_png,
         summary_writer=summary_writer,
     )
 
-  # Plot a few curves representing the VMP map for the no-cut parameters
-  model_name = 'epidemiology'
-  fig, _ = plot.plot_vmp_map(
-      alpha=state_list[0].params,
-      vmpmap_fn=vmpmap_fn,
-      lambda_init=lambda_init_list[0],
-      lambda_idx_to_plot=vmpmap_curves_idx,
-      eta_cancer_grid=jnp.linspace(0.0, 1.0, 101).round(3),
-  )
-  fig.suptitle(f"Example of VMP map curves")
-  fig.tight_layout()
-  if workdir_png:
-    plot_name = f"{model_name}_vmpmap_example_curves"
-    fig.savefig(pathlib.Path(workdir_png) / (plot_name + ".png"))
-  image = plot_to_image(fig)
-  if summary_writer:
-    plot_name = f"{model_name}_vmpmap_example_curves"
-    summary_writer.image(
-        tag=plot_name,
-        image=image,
-        step=state_list[0].step,
-    )
-
 
 def train_and_evaluate(config: ConfigDict, workdir: str) -> TrainState:
-  """Execute model training and evaluation loop.
+  """Model training and evaluation.
 
   Args:
     config: Hyperparameter configuration for training and evaluation.
     workdir: Directory where the tensorboard summaries are written to.
 
   Returns:
     Final TrainState.
@@ -172,18 +113,22 @@
   # Initialize random keys
   prng_seq = hk.PRNGSequence(config.seed)
 
   # Full dataset used everytime
   # Small data, no need to batch
   train_ds = load_data()
 
+  phi_dim = train_ds['Z'].shape[0]
+  theta_dim = 2
+
   # phi_dim and theta_dim are also arguments of the flow,
   # as they define its dimension
-  config.flow_kwargs.phi_dim = train_ds['Z'].shape[0]
-  config.flow_kwargs.theta_dim = 2
+  config.flow_kwargs.phi_dim = phi_dim
+  config.flow_kwargs.theta_dim = theta_dim
+  # Also is_smi modifies the dimension of the flow, due to the duplicated params
   config.flow_kwargs.is_smi = True
 
   # writer = metric_writers.create_default_writer(
   #     logdir=workdir, just_logging=jax.host_id() != 0)
   if jax.process_index() == 0:
     summary_writer = tensorboard.SummaryWriter(workdir)
     summary_writer.hparams(flatten_dict(config))
@@ -192,239 +137,193 @@
 
   # Functions that generate the NF for no-cut params
   flow_get_fn_nocut = getattr(flows, 'get_q_nocut_' + config.flow_name)
   # Functions that generate the NF for cut params (conditional on no-cut params)
   flow_get_fn_cutgivennocut = getattr(flows,
                                       'get_q_cutgivennocut_' + config.flow_name)
 
-  checkpoint_dir = str(pathlib.Path(workdir) / 'checkpoints')
-  state_list = []
-  state_name_list = []
-  lambda_init_list = []
-
-  # To initialize the VMP-map, we need one example of its output
-  # The output of the VMP-map is lambda, the parameters of the variational posterior
-  state_name_list.append('alpha_nocut')
-  lambda_init_list.append(
-      sample_q_nocut.init(
-          next(prng_seq),
-          flow_get_fn=flow_get_fn_nocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_nocut,
-          sample_shape=(config.num_samples_elbo,),
-      ))
-  nocut_base_sample_init = sample_q_nocut.apply(
-      lambda_init_list[0],
-      next(prng_seq),
-      flow_get_fn=flow_get_fn_nocut,
-      flow_kwargs=config.flow_kwargs,
-      split_flow_fn=split_flow_nocut,
+  # Initialize States of the three flows
+  state_tuple = init_state_tuple(
+      prng_key=next(prng_seq),
+      config=config,
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
       sample_shape=(config.num_samples_elbo,),
-  )['sample_base']
-  state_name_list.append('alpha_cut')
-  lambda_init_list.append(
-      sample_q_cutgivennocut.init(
-          next(prng_seq),
-          flow_get_fn=flow_get_fn_cutgivennocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_cut,
-          nocut_base_sample=nocut_base_sample_init,
-      ))
-  state_name_list.append('alpha_cut_aux')
-  lambda_init_list.append(
-      sample_q_cutgivennocut.init(
-          next(prng_seq),
-          flow_get_fn=flow_get_fn_cutgivennocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_cut,
-          nocut_base_sample=nocut_base_sample_init,
-      ))
-
-  # Define function that produce a tuple of lambda (flow parameters)
-  @hk.without_apply_rng
-  @hk.transform
-  def vmpmap_fn(eta_values, lambda_init):
-    vmpmap = getattr(modularbayes, config.vmp_map_name)(
-        **config.vmp_map_kwargs, params_flow_init=lambda_init)
-    lambda_out = vmpmap(eta_values)
-    return lambda_out
-
-  ### Initialise Variational Meta-Posterior Map ###
-  state_list = [
-      initial_state_ckpt(
-          checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-          forward_fn=vmpmap_fn,
-          forward_fn_kwargs={
-              'eta_values':
-                  jnp.ones((config.num_samples_eta, config.smi_eta_dim)),
-              'lambda_init':
-                  lambda_init_i
-          },
-          prng_key=next(prng_seq),
-          optimizer=make_optimizer(**config.optim_kwargs),
-      )
-      for state_name_i, lambda_init_i in zip(state_name_list, lambda_init_list)
-  ]
-  # globals().update(forward_fn_kwargs)
+      eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
+  )
 
-  # Print a useful summary of the execution of the VHP-map architecture.
-  tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda state_i, lambda_init_i: vmpmap_fn.apply(
-          state_i.params,
-          eta_values=jnp.ones((config.num_samples_eta, config.smi_eta_dim)),
-          lambda_init=lambda_init_i),
-      columns=(
-          "module",
-          "owned_params",
-          "params_size",
-          "params_bytes",
-      ),
-      filters=("has_params",),
+  # Print a summary of the networks architecture
+  print_trainable_params(
+      state_tuple=state_tuple,
+      prng_key=next(prng_seq),
+      config=config,
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+      sample_shape=(config.num_samples_elbo,),
+      eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
   )
-  summary = tabulate_fn_(state_list[0], lambda_init_list[0])
-  logging.info('VMP-MAP no-cut parameters:')
-  for line in summary.split("\n"):
-    logging.info(line)
-
-  summary = tabulate_fn_(state_list[1], lambda_init_list[1])
-  logging.info('VMP-MAP cut parameters:')
-  for line in summary.split("\n"):
-    logging.info(line)
 
-  ### Training VMP map ###
+  # Create checkpoint managers for the three states
+  orbax_ckpt_mngrs = [
+      orbax.checkpoint.CheckpointManager(
+          directory=str(pathlib.Path(workdir) / 'checkpoints' / state_name),
+          checkpointers=orbax.checkpoint.PyTreeCheckpointer(),
+          options=orbax.checkpoint.CheckpointManagerOptions(
+              max_to_keep=1,
+              save_interval_steps=config.checkpoint_steps,
+          ),
+      ) for state_name in state_tuple._asdict()
+  ]
+
+  # Restore existing checkpoint if present
+  if orbax_ckpt_mngrs[0].latest_step() is not None:
+    state_tuple = [
+        mngr.restore(mngr.latest_step(), items=state)
+        for state, mngr in zip(state_tuple, orbax_ckpt_mngrs)
+    ]
+
+  # Jit function to update training states
   @jax.jit
-  def update_states_jit(state_list, batch, prng_key):
-    return update_states(
-        state_list=state_list,
+  def train_step_jit(state_tuple, batch, prng_key):
+    return train_step(
+        state_tuple=state_tuple,
         batch=batch,
         prng_key=prng_key,
-        optimizer=make_optimizer(**config.optim_kwargs),
-        loss_fn=loss,
-        loss_fn_kwargs={
-            'num_samples': config.num_samples_eta,
-            'vmpmap_fn': vmpmap_fn,
-            'lambda_init_tuple': tuple(lambda_init_list),
+        loss=loss_fn,
+        loss_kwargs={
+            'num_samples': config.num_samples_elbo,
+            'logprob_joint_fn': logprob_joint,
+            'flow_get_fn_nocut': flow_get_fn_nocut,
+            'flow_get_fn_cutgivennocut': flow_get_fn_cutgivennocut,
+            'flow_kwargs': config.flow_kwargs,
+            'prior_hparams': config.prior_hparams,
+            'model_params_tupleclass': ModelParams,
+            'model_params_cut_tupleclass': ModelParamsCut,
+            'split_flow_fn_nocut': split_flow_nocut,
+            'split_flow_fn_cut': split_flow_cut,
             'sample_eta_fn': sample_eta_values,
             'sample_eta_kwargs': {
                 'eta_sampling_a': config.eta_sampling_a,
                 'eta_sampling_b': config.eta_sampling_b
             },
-            'elbo_smi_kwargs': {
-                'logprob_joint_fn': logprob_joint,
-                'flow_get_fn_nocut': flow_get_fn_nocut,
-                'flow_get_fn_cutgivennocut': flow_get_fn_cutgivennocut,
-                'flow_kwargs': config.flow_kwargs,
-                'prior_hparams': config.prior_hparams,
-                'model_params_tupleclass': ModelParams,
-                'model_params_cut_tupleclass': ModelParamsCut,
-                'split_flow_fn_nocut': split_flow_nocut,
-                'split_flow_fn_cut': split_flow_cut,
-            }
         },
     )
 
-  if state_list[0].step < config.training_steps:
-    logging.info('Training Variational Meta-Posterior (VMP-map)...')
+  @jax.jit
+  def elbo_validation_jit(state_tuple, batch, prng_key):
+    return elbo_smi_vmpflow(
+        lambda_tuple=tuple(state.params for state in state_tuple),
+        batch=batch,
+        prng_key=prng_key,
+        num_samples=config.num_samples_eval,
+        logprob_joint_fn=logprob_joint,
+        flow_get_fn_nocut=flow_get_fn_nocut,
+        flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+        flow_kwargs=config.flow_kwargs,
+        prior_hparams=config.prior_hparams,
+        model_params_tupleclass=ModelParams,
+        model_params_cut_tupleclass=ModelParamsCut,
+        split_flow_fn_nocut=split_flow_nocut,
+        split_flow_fn_cut=split_flow_cut,
+        sample_eta_fn=sample_eta_values,
+        sample_eta_kwargs={
+            'eta_sampling_a': 1.,
+            'eta_sampling_b': 1.
+        },
+    )
+
+  if state_tuple[0].step < config.training_steps:
+    logging.info('Training Variational Meta-Posterior (VMP-flow)...')
 
   # Reset random key sequence
   prng_seq = hk.PRNGSequence(config.seed)
 
-  while state_list[0].step < config.training_steps:
+  while state_tuple[0].step < config.training_steps:
 
     # Plots to monitor training
-    if (config.log_img_steps
-        is not None) and ((state_list[0].step == 1) or
-                          (state_list[0].step % config.log_img_steps == 0)):
-      # print("Logging images...\n")
+    if ((state_tuple[0].step == 0) or
+        (state_tuple[0].step % config.log_img_steps == 0)):
+      logging.info("\t\t Logging plots...")
       log_images(
-          state_list=state_list,
+          state_tuple=state_tuple,
           prng_key=next(prng_seq),
           config=config,
           dataset=train_ds,
           num_samples_plot=config.num_samples_plot,
-          vmpmap_fn=vmpmap_fn,
-          lambda_init_list=lambda_init_list,
           flow_get_fn_nocut=flow_get_fn_nocut,
           flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
-          vmpmap_curves_idx=config.vmpmap_curves_idx,
           summary_writer=summary_writer,
           workdir_png=workdir,
       )
       plt.close()
+      logging.info("\t\t...done logging plots.")
 
     # Log learning rate
     summary_writer.scalar(
         tag='learning_rate',
         value=getattr(optax, config.optim_kwargs.lr_schedule_name)(
-            **config.optim_kwargs.lr_schedule_kwargs)(state_list[0].step),
-        step=state_list[0].step,
+            **config.optim_kwargs.lr_schedule_kwargs)(state_tuple[0].step),
+        step=state_tuple[0].step,
     )
 
-    state_list, metrics = update_states_jit(
-        state_list=state_list,
+    # SGD step
+    state_tuple_, metrics = train_step_jit(
+        state_tuple=state_tuple,
         batch=train_ds,
         prng_key=next(prng_seq),
     )
+    if jax.lax.is_finite(metrics['train_loss']):
+      state_tuple = state_tuple_
 
-    # The computed training loss would correspond to the model before update
     summary_writer.scalar(
         tag='train_loss',
         value=metrics['train_loss'],
-        step=state_list[0].step - 1,
+        step=state_tuple[0].step,
     )
 
-    if state_list[0].step == 2:
-      logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
+    if state_tuple[0].step == 1:
+      logging.info("STEP: %5d; training loss: %.3f", state_tuple[0].step,
                    metrics["train_loss"])
 
-    if state_list[0].step % config.eval_steps == 0:
-      logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
+    # Metrics for evaluation
+    if state_tuple[0].step % config.eval_steps == 0:
+      logging.info("STEP: %5d; training loss: %.3f", state_tuple[0].step,
                    metrics["train_loss"])
 
-    # Save checkpoints
-    if (state_list[0].step) % config.checkpoint_steps == 0:
-      for state_i, state_name_i in zip(state_list, state_name_list):
-        save_checkpoint(
-            state=state_i,
-            checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-            keep=config.checkpoints_keep,
+      elbo_dict = elbo_validation_jit(
+          state_tuple=state_tuple,
+          batch=train_ds,
+          prng_key=next(prng_seq),
+      )
+      for k, v in elbo_dict.items():
+        summary_writer.scalar(
+            tag=f'elbo_{k}',
+            value=v.mean(),
+            step=state_tuple[0].step,
         )
 
-    # Wait until computations are done before the next step
-    # jax.random.normal(jax.random.PRNGKey(0), ()).block_until_ready()
-
-  logging.info('Final training step: %i', state_list[0].step)
+    for state, mngr in zip(state_tuple, orbax_ckpt_mngrs):
+      mngr.save(step=int(state.step), items=state)
 
-  # Save checkpoints at the end of the training process
-  # (in case training_steps is not multiple of checkpoint_steps)
-  for state_i, state_name_i in zip(state_list, state_name_list):
-    save_checkpoint(
-        state=state_i,
-        checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-        keep=config.checkpoints_keep,
-    )
+  logging.info('Final training step: %i', state_tuple[0].step)
 
   # Last plot of posteriors
   log_images(
-      state_list=state_list,
+      state_tuple=state_tuple,
       prng_key=next(prng_seq),
       config=config,
       dataset=train_ds,
       num_samples_plot=config.num_samples_plot,
-      vmpmap_fn=vmpmap_fn,
-      lambda_init_list=lambda_init_list,
       flow_get_fn_nocut=flow_get_fn_nocut,
       flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
-      vmpmap_curves_idx=config.vmpmap_curves_idx,
       summary_writer=summary_writer,
       workdir_png=workdir,
   )
-  plt.close()
 
-  return state_list
+  return state_tuple
 
 
 # # For debugging
 # config = get_config()
 # import pathlib
-# workdir = str(pathlib.Path.home() / f'modularbayes-output-exp/epidemiology/nsf/vmp_map')
+# workdir = str(pathlib.Path.home() / f'modularbayes-output-exp/epidemiology/vmp_nsf')
 # # train_and_evaluate(config, workdir)
```

### Comparing `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut1.py` & `modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_cut1.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut2.py` & `modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_cut2.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_cut3.py` & `modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_cut3.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_full.py` & `modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_full.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_vmp_flow.py` & `modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_vmp_flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,36 +15,34 @@
 
   # Model hyper-parameters, defining the prior.
   config.prior_hparams = None
 
   config.method = 'vmp_flow'
 
   # Defined in `flows`.
-  config.flow_name = 'meta_nsf'
+  config.flow_name = 'nsf'
   # kwargs to be passed to the flow
   config.flow_kwargs = ml_collections.ConfigDict()
   # Number of layers to use in the flow.
   config.flow_kwargs.num_layers = 8
   # Hidden sizes
   # Hidden sizes of the MLP conditioner.
-  config.flow_kwargs.hidden_sizes_conditioner = [30] * 3 + [10]
-  # Hidden sizes of the MLP conditioner for eta.
-  config.flow_kwargs.hidden_sizes_conditioner_eta = [30] * 3 + [10]
+  config.flow_kwargs.hidden_sizes = [30] * 3 + [10]
   # Number of bins to use in the rational-quadratic spline.
   config.flow_kwargs.num_bins = 10
   # the lower bound of the spline's range
   config.flow_kwargs.range_min = -10.
   # the upper bound of the spline's range
   config.flow_kwargs.range_max = 40.
 
-  config.num_samples_elbo = 10
+  config.num_samples_elbo = 100
   config.num_samples_eval = 10_000
 
   # Number of training steps to run.
-  config.training_steps = 200_000
+  config.training_steps = 100_000
 
   # Number of SGD steps to find the best eta
   config.eta_star_steps = 5_000
 
   # Optimizer
   config.optim_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.grad_clip_value = 1.0
@@ -74,15 +72,15 @@
 
   # How often to log images to monitor convergence.
   config.log_img_steps = int(config.training_steps / 10)
 
   # Number of posteriors samples used in the plots.
   config.num_samples_plot = 40_000
 
-  config.num_samples_elpd = 1_000
+  config.num_samples_elpd = 40_000
 
   config.smi_eta_dim = config.num_groups
   config.smi_eta_plot = {
       'full': [1. for _ in range(config.smi_eta_dim)],
       'cut1': [0.0001, 1.] + [1. for _ in range(config.smi_eta_dim - 2)],
       'cut2': [0.0001, 0.0001] + [1. for _ in range(config.smi_eta_dim - 2)],
       'cut3': [1., 0.0001] + [1. for _ in range(config.smi_eta_dim - 2)],
```

### Comparing `modularbayes-0.1.3/examples/random_effects/configs/flow_nsf_vmp_map.py` & `modularbayes-0.1.4/examples/random_effects/configs/flow_nsf_vmp_map.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,15 @@
   # Number of bins to use in the rational-quadratic spline.
   config.flow_kwargs.num_bins = 10
   # the lower bound of the spline's range
   config.flow_kwargs.range_min = -10.
   # the upper bound of the spline's range
   config.flow_kwargs.range_max = 40.
 
-  config.num_samples_elbo = 10
-  config.num_samples_eval = 5_000
+  config.num_samples_elbo = 100
 
   # Number of training steps to run.
   config.training_steps = 100_000
 
   # Optimizer
   config.optim_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.grad_clip_value = 1.0
@@ -46,15 +45,15 @@
   config.optim_kwargs.lr_schedule_name = 'warmup_exponential_decay_schedule'
   config.optim_kwargs.lr_schedule_kwargs = ml_collections.ConfigDict()
   config.optim_kwargs.lr_schedule_kwargs = {
       'init_value': 0.,
       'peak_value': 3e-4,
       'warmup_steps': 3_000,
       'transition_steps': 20_000,
-      'decay_rate': 0.5,
+      'decay_rate': 0.8,
       'transition_begin': 0,
       'staircase': False,
       'end_value': None,
   }
 
   # How often to evaluate the model.
   config.eval_steps = int(config.training_steps / 10)
@@ -64,14 +63,16 @@
 
   # How often to log images to monitor convergence.
   config.log_img_steps = int(config.training_steps / 10)
 
   # Number of posteriors samples used in the plots.
   config.num_samples_plot = 40_000
 
+  config.num_samples_elpd = 40_000
+
   config.smi_eta_dim = config.num_groups
   config.smi_eta_plot = {
       'full': [1. for _ in range(config.smi_eta_dim)],
       'cut1': [0.0001, 1.] + [1. for _ in range(config.smi_eta_dim - 2)],
       'cut2': [0.0001, 0.0001] + [1. for _ in range(config.smi_eta_dim - 2)],
       'cut3': [1., 0.0001] + [1. for _ in range(config.smi_eta_dim - 2)],
   }
@@ -84,16 +85,15 @@
 
   # Arguments for the Variational Meta-Posterior map
   config.vmp_map_name = 'MLPVmpMap'
   config.vmp_map_kwargs = ml_collections.ConfigDict()
   eta_dim = config.num_groups
   config.vmp_map_kwargs.hidden_sizes = [eta_dim * 10] * 5 + [20]
 
-  # Number of samples of eta for Meta-Posterior training
-  config.num_samples_eta = 25
+  # Eta sampling distribution for Meta-Posterior training
   config.eta_sampling_a = 0.2
   config.eta_sampling_b = 1.0
 
   config.lambda_idx_plot = [50 * i for i in range(5)]
   config.constant_lambda_ignore_plot = True
 
   return config
```

### Comparing `modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut1.py` & `modularbayes-0.1.4/examples/random_effects/configs/mcmc_cut1.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut2.py` & `modularbayes-0.1.4/examples/random_effects/configs/mcmc_cut2.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/random_effects/configs/mcmc_cut3.py` & `modularbayes-0.1.4/examples/random_effects/configs/mcmc_cut3.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/random_effects/configs/mcmc_full.py` & `modularbayes-0.1.4/examples/random_effects/configs/mcmc_full.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/random_effects/flows.py` & `modularbayes-0.1.4/examples/random_effects/flows.py`

 * *Files 22% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 def get_q_nocut_nsf(
     num_groups: int,
     num_layers: int,
     hidden_sizes: Sequence[int],
     num_bins: int,
     range_min: float = 0.,
     range_max: float = 1.,
+    is_meta: bool = False,
     **_,
 ) -> distrax.Transformed:
   """Creates the Rational Quadratic Flow model.
 
   Args:
   range_min: the lower bound of the spline's range. Below `range_min`, the
     bijector defaults to a linear transformation.
@@ -75,43 +76,62 @@
 
   # Number of parameters for the rational-quadratic spline:
   # - `num_bins` bin widths
   # - `num_bins` bin heights
   # - `num_bins + 1` knot slopes
   # for a total of `3 * num_bins + 1` parameters.
   for _ in range(num_layers):
-    layer = distrax.MaskedCoupling(
-        mask=mask,
-        bijector=bijector_fn,
-        conditioner=modularbayes.MLPConditioner(
-            output_dim=math.prod(event_shape),
-            hidden_sizes=hidden_sizes,
-            num_bijector_params=num_bijector_params,
-            name='conditioner_nocut',
-        ),
-    )
+    if is_meta:
+      layer = modularbayes.ConditionalMaskedCoupling(
+          mask=mask,
+          bijector=bijector_fn,
+          conditioner=modularbayes.MLPConditioner(
+              output_dim=math.prod(event_shape),
+              hidden_sizes=hidden_sizes,
+              num_bijector_params=num_bijector_params,
+              name='conditioner_nocut',
+          ),
+      )
+    else:
+      layer = distrax.MaskedCoupling(
+          mask=mask,
+          bijector=bijector_fn,
+          conditioner=modularbayes.MLPConditioner(
+              output_dim=math.prod(event_shape),
+              hidden_sizes=hidden_sizes,
+              num_bijector_params=num_bijector_params,
+              name='conditioner_nocut',
+          ),
+      )
     flow_layers.append(layer)
     # Flip the mask after each layer.
     mask = jnp.logical_not(mask)
 
   # Last layer: Map values to parameter domain
   bij_nocut = bijector_domain_nocut()
   flow_layers.append(bij_nocut)
 
   # Chain all flow layers together
-  flow = distrax.Chain(flow_layers[::-1])
+  if is_meta:
+    flow = modularbayes.ConditionalChain(flow_layers[::-1])
+  else:
+    flow = distrax.Chain(flow_layers[::-1])
 
   # base_distribution = distrax.Independent(
   #     distrax.Uniform(low=jnp.zeros(event_shape), high=jnp.ones(event_shape)),
   #     reinterpreted_batch_ndims=len(event_shape))
 
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
+  if is_meta:
+    q_distr = modularbayes.ConditionalTransformed(base_distribution, flow)
+  else:
+    q_distr = modularbayes.Transformed(base_distribution, flow)
 
-  return modularbayes.Transformed(base_distribution, flow)
+  return q_distr
 
 
 def get_q_cutgivennocut_nsf(
     num_groups: int,
     num_layers: int,
     hidden_sizes: Sequence[int],
     num_bins: int,
@@ -179,174 +199,14 @@
 
   base_distribution = distrax.MultivariateNormalDiag(
       loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
 
   return modularbayes.ConditionalTransformed(base_distribution, flow)
 
 
-def get_q_nocut_meta_nsf(
-    num_groups: int,
-    num_layers: int,
-    hidden_sizes_conditioner: Sequence[int],
-    hidden_sizes_conditioner_eta: Sequence[int],
-    num_bins: int,
-    range_min: float = 0.,
-    range_max: float = 1.,
-    **_,
-) -> modularbayes.ConditionalTransformed:
-  """Creates the Rational Quadratic Flow model.
-
-  Args:
-  range_min: the lower bound of the spline's range. Below `range_min`, the
-    bijector defaults to a linear transformation.
-  range_max: the upper bound of the spline's range. Above `range_max`, the
-    bijector defaults to a linear transformation.
-  """
-
-  flow_dim = num_groups
-
-  event_shape = (flow_dim,)
-
-  flow_layers = []
-
-  # Number of parameters required by the bijector (rational quadratic spline)
-  num_bijector_params = 3 * num_bins + 1
-
-  def bijector_fn(params: Array):
-    return distrax.RationalQuadraticSpline(
-        params, range_min=range_min, range_max=range_max)
-
-  # Alternating binary mask.
-  mask = jnp.arange(0, math.prod(event_shape)) % 2
-  mask = jnp.reshape(mask, event_shape)
-  mask = mask.astype(bool)
-
-  # Number of parameters for the rational-quadratic spline:
-  # - `num_bins` bin widths
-  # - `num_bins` bin heights
-  # - `num_bins + 1` knot slopes
-  # for a total of `3 * num_bins + 1` parameters.
-
-  for _ in range(num_layers):
-    layer = modularbayes.EtaConditionalMaskedCoupling(
-        mask=mask,
-        bijector=bijector_fn,
-        conditioner_eta=modularbayes.MLPConditioner(
-            output_dim=math.prod(event_shape),
-            hidden_sizes=hidden_sizes_conditioner_eta,
-            num_bijector_params=num_bijector_params,
-            name='conditioner_eta_nocut',
-        ),
-        conditioner=modularbayes.MLPConditioner(
-            output_dim=math.prod(event_shape),
-            hidden_sizes=hidden_sizes_conditioner,
-            num_bijector_params=num_bijector_params,
-            name='conditioner_nocut',
-        ),
-    )
-    flow_layers.append(layer)
-    # Flip the mask after each layer.
-    mask = jnp.logical_not(mask)
-
-  # Last Layer: Map values to parameter domain
-  bij_nocut = bijector_domain_nocut()
-  flow_layers.append(bij_nocut)
-
-  # Chain all flow layers together
-  flow = modularbayes.ConditionalChain(flow_layers[::-1])
-
-  # base_distribution = distrax.Independent(
-  #     distrax.Uniform(low=jnp.zeros(event_shape), high=jnp.ones(event_shape)),
-  #     reinterpreted_batch_ndims=len(event_shape))
-
-  base_distribution = distrax.MultivariateNormalDiag(
-      loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
-
-  return modularbayes.ConditionalTransformed(base_distribution, flow)
-
-
-def get_q_cutgivennocut_meta_nsf(
-    num_groups: int,
-    num_layers: int,
-    hidden_sizes_conditioner: Sequence[int],
-    hidden_sizes_conditioner_eta: Sequence[int],
-    num_bins: int,
-    range_min: float = 0.,
-    range_max: float = 1.,
-    **_,
-) -> modularbayes.ConditionalTransformed:
-  """Creates the Rational Quadratic Flow model.
-
-  Args:
-  range_min: the lower bound of the spline's range. Below `range_min`, the
-    bijector defaults to a linear transformation.
-  range_max: the upper bound of the spline's range. Above `range_max`, the
-    bijector defaults to a linear transformation.
-  """
-
-  flow_dim = num_groups + 1
-  event_shape = (flow_dim,)
-
-  flow_layers = []
-
-  # Number of parameters required by the bijector (rational quadratic spline)
-  num_bijector_params = 3 * num_bins + 1
-
-  def bijector_fn(params: Array):
-    return distrax.RationalQuadraticSpline(
-        params, range_min=range_min, range_max=range_max)
-
-  # Alternating binary mask.
-  mask = jnp.arange(0, math.prod(event_shape)) % 2
-  mask = jnp.reshape(mask, event_shape)
-  mask = mask.astype(bool)
-
-  # Number of parameters for the rational-quadratic spline:
-  # - `num_bins` bin widths
-  # - `num_bins` bin heights
-  # - `num_bins + 1` knot slopes
-  # for a total of `3 * num_bins + 1` parameters.
-
-  for _ in range(num_layers):
-    layer = modularbayes.EtaConditionalMaskedCoupling(
-        mask=mask,
-        bijector=bijector_fn,
-        conditioner_eta=modularbayes.MLPConditioner(
-            output_dim=math.prod(event_shape),
-            hidden_sizes=hidden_sizes_conditioner_eta,
-            num_bijector_params=num_bijector_params,
-            name='conditioner_eta_theta',
-        ),
-        conditioner=modularbayes.MLPConditioner(
-            # input_dim=math.prod(event_shape),
-            output_dim=math.prod(event_shape),
-            hidden_sizes=hidden_sizes_conditioner,
-            num_bijector_params=num_bijector_params,
-            name='conditioner_theta',
-        ),
-    )
-    flow_layers.append(layer)
-    # Flip the mask after each layer.
-    mask = jnp.logical_not(mask)
-
-  # Last layer: Map values to parameter domain
-  bij_cut = bijector_domain_cut(num_groups=num_groups)
-  flow_layers.append(bij_cut)
-
-  # Chain all flow layers together
-  flow = modularbayes.ConditionalChain(flow_layers[::-1])
-
-  base_distribution = distrax.MultivariateNormalDiag(
-      loc=jnp.zeros(event_shape), scale_diag=jnp.ones(event_shape))
-
-  q_distr = modularbayes.ConditionalTransformed(base_distribution, flow)
-
-  return q_distr
-
-
 def split_flow_nocut(
     concat_params: Array,
     num_groups: int,
     **_,
 ) -> Dict[str, Any]:
   """Get model parameters by splitting samples from the flow."""
```

### Comparing `modularbayes-0.1.3/examples/random_effects/log_prob_fun.py` & `modularbayes-0.1.4/examples/random_effects/log_prob_fun.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,14 +95,16 @@
     prng_key: PRNGKey,
     num_samples: int,
     num_groups: int,
     eta_sampling_a: float,
     eta_sampling_b: float,
 ) -> SmiEta:
   """Generate a sample of the smi_eta values applicable to the model."""
-  smi_etas = SmiEta(
-      groups=jax.random.beta(
-          key=prng_key,
-          a=eta_sampling_a,
-          b=eta_sampling_b,
-          shape=(num_samples, num_groups)),)
+  smi_etas = jax.random.beta(
+      key=prng_key,
+      a=eta_sampling_a,
+      b=eta_sampling_b,
+      shape=(num_samples, num_groups))
+  # smi_etas = jnp.concatenate(
+  #     [smi_etas, jnp.ones((num_samples, num_groups - 3))], axis=-1)
+  smi_etas = SmiEta(groups=smi_etas)
   return smi_etas
```

### Comparing `modularbayes-0.1.3/examples/random_effects/main.py` & `modularbayes-0.1.4/examples/random_effects/main.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/random_effects/plot.py` & `modularbayes-0.1.4/examples/random_effects/plot.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/random_effects/sample_mcmc.py` & `modularbayes-0.1.4/examples/random_effects/sample_mcmc.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/examples/random_effects/train_flow.py` & `modularbayes-0.1.4/examples/random_effects/train_vmp_flow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,138 +1,272 @@
-"""Training a Normalizing Flow."""
+"""Training a Variational Meta-Posterior, using the VMP flow."""
+
 import pathlib
 
 from absl import logging
 
 import numpy as np
-
-from arviz import InferenceData
-
-from flax.metrics import tensorboard
+import matplotlib
+from matplotlib import pyplot as plt
 
 import jax
 from jax import numpy as jnp
-
+from flax.metrics import tensorboard
+from flax.training.train_state import TrainState
 import haiku as hk
 import optax
-import distrax
+import orbax.checkpoint
 
 import flows
 from flows import split_flow_nocut, split_flow_cut
-from log_prob_fun import ModelParams, ModelParamsCut, SmiEta, logprob_joint
+from log_prob_fun import (ModelParams, ModelParamsCut, SmiEta, logprob_joint,
+                          sample_eta_values)
 import plot
-
-from modularbayes import (sample_q_nocut, sample_q_cutgivennocut, sample_q,
-                          elbo_smi)
-from modularbayes._src.utils.training import TrainState
-from modularbayes import (flatten_dict, initial_state_ckpt, update_states,
-                          save_checkpoint)
+from train_flow import (elpd_truth_mc, elpd_waic, init_state_tuple, load_data,
+                        print_trainable_params, sample_q_as_az)
+from modularbayes import elbo_smi_vmpflow, sample_q, train_step
+from modularbayes import (flatten_dict, normalize_images, plot_to_image)
 from modularbayes._src.typing import (Any, Array, Callable, ConfigDict, Dict,
                                       List, Optional, PRNGKey, Tuple)
 
 # Set high precision for matrix multiplication in jax
 jax.config.update('jax_default_matmul_precision', 'float32')
 
 np.set_printoptions(suppress=True, precision=4)
 
 
-def load_data(
-    prng_key: PRNGKey,
-    num_obs_groups: Array,
-    loc_groups: Array,
-    scale_groups: Array,
-) -> Dict[str, Array]:
-  """Generate random effects data as in Liu 2009."""
-
-  num_groups = len(num_obs_groups)
-  assert len(loc_groups) == num_groups
-  assert len(scale_groups) == num_groups
-
-  num_obs_groups = jnp.array(num_obs_groups).astype(int)
-  loc_groups = jnp.array(loc_groups)
-  scale_groups = jnp.array(scale_groups)
-
-  loc_pointwise = jnp.repeat(loc_groups, num_obs_groups)
-  scale_pointwise = jnp.repeat(scale_groups, num_obs_groups)
-
-  z = jax.random.normal(key=prng_key, shape=loc_pointwise.shape)
-
-  dataset_dict = {
-      'Y': loc_pointwise + z * scale_pointwise,
-      'group': jnp.repeat(jnp.arange(num_groups), num_obs_groups),
-      'num_obs_groups': num_obs_groups,
-  }
-
-  return dataset_dict
-
-
-def make_optimizer(
-    lr_schedule_name,
-    lr_schedule_kwargs,
-    grad_clip_value,
-) -> optax.GradientTransformation:
-  """Define optimizer to train the Flow."""
-  schedule = getattr(optax, lr_schedule_name)(**lr_schedule_kwargs)
-
-  optimizer = optax.chain(*[
-      optax.clip_by_global_norm(max_norm=grad_clip_value),
-      optax.adabelief(learning_rate=schedule),
-  ])
-  return optimizer
-
-
-def loss(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
+def loss_fn(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
   """Define training loss function."""
 
   ### Compute ELBO ###
-  elbo_dict = elbo_smi(lambda_tuple=params_tuple, *args, **kwargs)
+  elbo_dict = elbo_smi_vmpflow(lambda_tuple=params_tuple, *args, **kwargs)
 
   # Our loss is the Negative ELBO
   loss_avg = -(jnp.nanmean(elbo_dict['stage_1'] + elbo_dict['stage_2']))
 
   return loss_avg
 
 
-def sample_q_as_az(
+def plot_elpd_surface(
     lambda_tuple: Tuple[hk.Params],
     dataset: Dict[str, Any],
     prng_key: PRNGKey,
+    config: ConfigDict,
     flow_get_fn_nocut: Callable,
     flow_get_fn_cutgivennocut: Callable,
-    flow_kwargs: Dict[str, Any],
-    sample_shape: Optional[Tuple[int]] = None,
-    eta_values: Optional[Array] = None,
-) -> InferenceData:
-  """Plots to monitor during training."""
-  assert sample_shape is not None or eta_values is not None, (
-      'Either sample_shape or eta_values must be provided.')
-  assert sample_shape is None or eta_values is None, (
-      'Only one of sample_shape or eta_values must be provided.')
-  # Sample from flow
-  q_distr_out = sample_q(
-      lambda_tuple=lambda_tuple,
-      prng_key=prng_key,
+    eta_grid: Array,
+    eta_grid_x_y_idx: Tuple[int, int],
+    true_params: Optional[ModelParams] = None,
+):
+  """Visualize ELPD surface as function of eta."""
+
+  assert eta_grid.ndim == 3
+  prng_seq = hk.PRNGSequence(prng_key)
+
+  num_groups = eta_grid.shape[-1]
+
+  # Jit functions for speed
+  elpd_waic_jit = jax.jit(elpd_waic)
+  elpd_truth_mc_jit = jax.jit(elpd_truth_mc)
+  sample_q_key_ = next(prng_seq)
+  sample_q_jit = jax.jit(lambda x, y: sample_q(
+      lambda_tuple=x,
+      prng_key=sample_q_key_,  # same seed for all etas, see less variability
       flow_get_fn_nocut=flow_get_fn_nocut,
       flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
-      flow_kwargs=flow_kwargs,
+      flow_kwargs=config.flow_kwargs,
       model_params_tupleclass=ModelParams,
       split_flow_fn_nocut=split_flow_nocut,
       split_flow_fn_cut=split_flow_cut,
-      sample_shape=sample_shape,
-      eta_values=eta_values,
-  )
-  # Add dimension for "chains"
-  model_params_az = jax.tree_map(lambda x: x[None, ...],
-                                 q_distr_out['model_params_sample'])
-  # Create InferenceData object
-  az_data = plot.arviz_from_samples(
-      dataset=dataset,
-      model_params=model_params_az,
+      sample_shape=(y.shape[0],),
+      eta_values=y,
+  )['model_params_sample'])
+
+  # Produce flow parameters as a function of eta
+  if true_params is not None:
+    # Generate data from true model
+    z = jax.random.normal(
+        key=next(prng_seq), shape=(config.num_samples_elpd, num_groups))
+    y_new = true_params.sigma * z + true_params.beta
+  elpd_waic_grid = []
+  if true_params is not None:
+    elpd_grid = []
+  for eta_i in eta_grid.reshape(-1, num_groups):
+    # Sample from flow
+    model_params_sample_i = sample_q_jit(
+        lambda_tuple, jnp.tile(eta_i[None, ...], (config.num_samples_elpd, 1)))
+
+    # Compute ELPD using WAIC
+    elpd_waic_grid.append(
+        elpd_waic_jit(
+            model_params_sample=model_params_sample_i, dataset=dataset))
+    if true_params is not None:
+      # Compute ELPD
+      elpd_grid.append(
+          elpd_truth_mc_jit(
+              model_params_sample=model_params_sample_i, y_new=y_new))
+
+  # Plot the ELPD surface.
+  fig, axs = plt.subplots(
+      nrows=1,
+      ncols=1 if true_params is None else 2,
+      figsize=(4 if true_params is None else 8, 3),
+      subplot_kw={"projection": "3d"},
+      squeeze=False)
+  elpd_waic_grid = jnp.array(elpd_waic_grid).reshape(eta_grid.shape[:-1])
+  axs[0, 0].plot_surface(
+      eta_grid[..., eta_grid_x_y_idx[0]],
+      eta_grid[..., eta_grid_x_y_idx[1]],
+      -elpd_waic_grid,
+      cmap=matplotlib.cm.inferno,
+      # linewidth=0,
+      # antialiased=False,
   )
-  return az_data
+  axs[0, 0].view_init(30, 225)
+  axs[0, 0].set_xlabel(f'eta_{eta_grid_x_y_idx[0]}')
+  axs[0, 0].set_ylabel(f'eta_{eta_grid_x_y_idx[1]}')
+  axs[0, 0].set_title('- ELPD WAIC')
+  if true_params is not None:
+    elpd_grid = jnp.array(elpd_grid).reshape(eta_grid.shape[:-1])
+    axs[0, 1].plot_surface(
+        eta_grid[..., eta_grid_x_y_idx[0]],
+        eta_grid[..., eta_grid_x_y_idx[1]],
+        -elpd_grid,
+        cmap=matplotlib.cm.inferno,
+        # linewidth=0,
+        # antialiased=False,
+    )
+    axs[0, 1].view_init(30, 225)
+    axs[0, 1].set_xlabel(f'eta_{eta_grid_x_y_idx[0]}')
+    axs[0, 1].set_ylabel(f'eta_{eta_grid_x_y_idx[1]}')
+    axs[0, 1].set_title('- ELPD')
+  fig.tight_layout()
+
+  return fig, axs
+
+
+def log_images(
+    state_list: List[TrainState],
+    prng_key: PRNGKey,
+    config: ConfigDict,
+    dataset: Dict[str, Any],
+    num_samples_plot: int,
+    flow_get_fn_nocut: Callable,
+    flow_get_fn_cutgivennocut: Callable,
+    show_elpd_surface: bool,
+    true_params: ModelParams,
+    summary_writer: Optional[tensorboard.SummaryWriter] = None,
+    workdir_png: Optional[str] = None,
+) -> None:
+  """Plots to monitor during training."""
+
+  model_name = 'random_effects'
+
+  prng_seq = hk.PRNGSequence(prng_key)
+
+  assert len(config.smi_eta_plot.keys()) > 0, 'No eta values to plot'
+
+  # Plot posterior samples
+  for suffix, eta_groups_i in config.smi_eta_plot.items():
+    # Define eta
+    eta_groups_i = jnp.array(eta_groups_i)
+    assert all(eta_groups_i >= 0.0) and all(eta_groups_i <= 1.0), (
+        'eta must be in [0, 1]')
+    smi_etas = SmiEta(
+        groups=jnp.broadcast_to(eta_groups_i,
+                                (num_samples_plot,) + eta_groups_i.shape),)
+    # Sample from flow
+    az_data = sample_q_as_az(
+        lambda_tuple=tuple(x.params for x in state_list),
+        dataset=dataset,
+        prng_key=next(prng_seq),
+        flow_get_fn_nocut=flow_get_fn_nocut,
+        flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+        flow_kwargs=config.flow_kwargs,
+        sample_shape=(num_samples_plot,),
+        eta_values=(smi_etas[0] if len(smi_etas) == 1 else jnp.stack(
+            smi_etas, axis=-1)),
+    )
+    plot.posterior_plots(
+        az_data=az_data,
+        show_sigma_trace=False,
+        show_beta_trace=False,
+        show_tau_trace=False,
+        betasigma_pairplot_groups=(0, 1, 2),
+        tausigma_pairplot_groups=(0, 1, 2),
+        suffix=f'_{suffix}',
+        step=state_list[0].step,
+        workdir_png=workdir_png,
+        summary_writer=summary_writer,
+    )
+
+  if show_elpd_surface:
+    eta_grid_len = 10
+    images = []
+
+    # Define elements to grate grid of eta values
+    eta_grid_base = np.tile(
+        np.array([0., 0.] + [1. for _ in range(config.num_groups - 2)]),
+        [eta_grid_len + 1, eta_grid_len + 1, 1])
+    eta_grid_mini = np.stack(
+        np.meshgrid(
+            np.linspace(0, 1, eta_grid_len + 1).round(5),
+            np.linspace(0, 1, eta_grid_len + 1).round(5)),
+        axis=0).T
+
+    # Vary eta_0 and eta_1
+    plot_name = f'{model_name}_elpd_surface_eta_0_1'
+    eta_grid = eta_grid_base.copy()
+    eta_grid_x_y_idx = [0, 1]
+    eta_grid[:, :, eta_grid_x_y_idx] = eta_grid_mini
+    fig, _ = plot_elpd_surface(
+        lambda_tuple=tuple(x.params for x in state_list),
+        dataset=dataset,
+        prng_key=next(prng_seq),
+        config=config,
+        flow_get_fn_nocut=flow_get_fn_nocut,
+        flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+        eta_grid=eta_grid,
+        eta_grid_x_y_idx=eta_grid_x_y_idx,
+        true_params=true_params,
+    )
+    if workdir_png:
+      fig.savefig(pathlib.Path(workdir_png) / (plot_name + ".png"))
+    if summary_writer:
+      images.append(plot_to_image(fig))
+
+    # Vary eta_0 and eta_2
+    plot_name = f'{model_name}_elpd_surface_eta_0_2'
+    eta_grid = eta_grid_base.copy()
+    eta_grid_x_y_idx = [0, 2]
+    eta_grid[:, :, eta_grid_x_y_idx] = eta_grid_mini
+    fig, _ = plot_elpd_surface(
+        lambda_tuple=tuple(x.params for x in state_list),
+        dataset=dataset,
+        prng_key=next(prng_seq),
+        config=config,
+        flow_get_fn_nocut=flow_get_fn_nocut,
+        flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+        eta_grid=eta_grid,
+        eta_grid_x_y_idx=eta_grid_x_y_idx,
+        true_params=true_params,
+    )
+    if workdir_png:
+      fig.savefig(pathlib.Path(workdir_png) / (plot_name + ".png"))
+    if summary_writer:
+      images.append(plot_to_image(fig))
+
+    if summary_writer:
+      plot_name = f"{model_name}_elpd_surface"
+      summary_writer.image(
+          tag=plot_name,
+          image=normalize_images(images),
+          step=state_list[0].step,
+          max_outputs=len(images),
+      )
 
 
 def train_and_evaluate(config: ConfigDict, workdir: str) -> TrainState:
   """Execute model training and evaluation loop.
 
   Args:
     config: Hyperparameter configuration for training and evaluation.
@@ -159,29 +293,19 @@
   train_ds = load_data(
       prng_key=next(prng_seq),
       num_obs_groups=config.num_obs_groups,
       loc_groups=true_params.beta,
       scale_groups=true_params.sigma,
   )
 
-  # Generate new observations from the true generative model
-  y_new = distrax.Normal(
-      loc=true_params.beta[train_ds['group']],
-      scale=true_params.sigma[train_ds['group']],
-  ).sample(
-      seed=next(prng_seq), sample_shape=(config.num_samples_eval,))
-
-  # Set eta for modules
-  smi_eta = SmiEta(groups=jnp.array(config.smi_eta_groups))
-
   # num_groups is also a parameter of the flow,
   # as it define its dimension
   config.flow_kwargs.num_groups = config.num_groups
   # Also is_smi modifies the dimension of the flow, due to the duplicated params
-  config.flow_kwargs.is_smi = (smi_eta is not None)
+  config.flow_kwargs.is_smi = True
 
   # writer = metric_writers.create_default_writer(
   #     logdir=workdir, just_logging=jax.host_id() != 0)
   if jax.process_index() == 0:
     summary_writer = tensorboard.SummaryWriter(workdir)
     summary_writer.hparams(flatten_dict(config))
   else:
@@ -189,285 +313,198 @@
 
   # Functions that generate the NF for no-cut params
   flow_get_fn_nocut = getattr(flows, 'get_q_nocut_' + config.flow_name)
   # Functions that generate the NF for cut params (conditional on no-cut params)
   flow_get_fn_cutgivennocut = getattr(flows,
                                       'get_q_cutgivennocut_' + config.flow_name)
 
-  checkpoint_dir = str(pathlib.Path(workdir) / 'checkpoints')
-  state_list = []
-  state_name_list = []
-
-  state_name_list.append('lambda_nocut')
-  state_list.append(
-      initial_state_ckpt(
-          checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-          forward_fn=sample_q_nocut,
-          forward_fn_kwargs={
-              'flow_get_fn': flow_get_fn_nocut,
-              'flow_kwargs': config.flow_kwargs,
-              'split_flow_fn': split_flow_nocut,
-              'sample_shape': (config.num_samples_elbo,),
-          },
-          prng_key=next(prng_seq),
-          optimizer=make_optimizer(**config.optim_kwargs),
-      ))
-
-  # Get an initial sample of the base distribution of nocut params
-  nocut_base_sample_init = sample_q_nocut.apply(
-      state_list[0].params,
-      next(prng_seq),
-      flow_get_fn=flow_get_fn_nocut,
-      flow_kwargs=config.flow_kwargs,
-      split_flow_fn=split_flow_nocut,
+  # Initialize States of the three flows
+  state_tuple = init_state_tuple(
+      prng_key=next(prng_seq),
+      config=config,
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
       sample_shape=(config.num_samples_elbo,),
-  )['sample_base']
-
-  state_name_list.append('lambda_cut')
-  state_list.append(
-      initial_state_ckpt(
-          checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-          forward_fn=sample_q_cutgivennocut,
-          forward_fn_kwargs={
-              'flow_get_fn': flow_get_fn_cutgivennocut,
-              'flow_kwargs': config.flow_kwargs,
-              'split_flow_fn': split_flow_cut,
-              'nocut_base_sample': nocut_base_sample_init,
-          },
-          prng_key=next(prng_seq),
-          optimizer=make_optimizer(**config.optim_kwargs),
-      ))
-  if config.flow_kwargs.is_smi:
-    state_name_list.append('lambda_cut_aux')
-    state_list.append(
-        initial_state_ckpt(
-            checkpoint_dir=f'{checkpoint_dir}/{state_name_list[-1]}',
-            forward_fn=sample_q_cutgivennocut,
-            forward_fn_kwargs={
-                'flow_get_fn': flow_get_fn_cutgivennocut,
-                'flow_kwargs': config.flow_kwargs,
-                'split_flow_fn': split_flow_cut,
-                'nocut_base_sample': nocut_base_sample_init,
-            },
-            prng_key=next(prng_seq),
-            optimizer=make_optimizer(**config.optim_kwargs),
-        ))
-
-  # Print a useful summary of the execution of the flow architecture.
-  logging.info('\nFlow no-cut parameters:\n')
-  tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda params, prng_key: sample_q_nocut.apply(
-          params,
-          prng_key,
-          flow_get_fn=flow_get_fn_nocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_nocut,
-          sample_shape=(config.num_samples_elbo,),
-      ),
-      columns=(
-          "module",
-          "owned_params",
-          "params_size",
-          "params_bytes",
-      ),
-      filters=("has_params",),
+      eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
   )
-  summary = tabulate_fn_(state_list[0].params, next(prng_seq))
-  for line in summary.split("\n"):
-    logging.info(line)
-
-  logging.info('\nFlow cut parameters:\n')
-  tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda params, prng_key: sample_q_cutgivennocut.apply(
-          params,
-          prng_key,
-          flow_get_fn=flow_get_fn_cutgivennocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_cut,
-          nocut_base_sample=nocut_base_sample_init,
-      ),
-      columns=(
-          "module",
-          "owned_params",
-          "params_size",
-          "params_bytes",
-      ),
-      filters=("has_params",),
+
+  # Print a summary of the networks architecture
+  print_trainable_params(
+      state_tuple=state_tuple,
+      prng_key=next(prng_seq),
+      config=config,
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+      sample_shape=(config.num_samples_elbo,),
+      eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
   )
-  summary = tabulate_fn_(state_list[1].params, next(prng_seq))
-  for line in summary.split("\n"):
-    logging.info(line)
+
+  # Create checkpoint managers for the three states
+  orbax_ckpt_mngrs = [
+      orbax.checkpoint.CheckpointManager(
+          directory=str(pathlib.Path(workdir) / 'checkpoints' / state_name),
+          checkpointers=orbax.checkpoint.PyTreeCheckpointer(),
+          options=orbax.checkpoint.CheckpointManagerOptions(
+              max_to_keep=1,
+              save_interval_steps=config.checkpoint_steps,
+          ),
+      ) for state_name in state_tuple._asdict()
+  ]
+
+  # Restore existing checkpoint if present
+  if orbax_ckpt_mngrs[0].latest_step() is not None:
+    state_tuple = [
+        mngr.restore(mngr.latest_step(), items=state)
+        for state, mngr in zip(state_tuple, orbax_ckpt_mngrs)
+    ]
 
   # Jit function to update training states
   @jax.jit
-  def update_states_jit(state_list, batch, prng_key, smi_eta):
-    return update_states(
-        state_list=state_list,
+  def train_step_jit(state_tuple, batch, prng_key):
+    return train_step(
+        state_tuple=state_tuple,
         batch=batch,
         prng_key=prng_key,
-        optimizer=make_optimizer(**config.optim_kwargs),
-        loss_fn=loss,
-        loss_fn_kwargs={
+        loss=loss_fn,
+        loss_kwargs={
             'num_samples': config.num_samples_elbo,
             'logprob_joint_fn': logprob_joint,
             'flow_get_fn_nocut': flow_get_fn_nocut,
             'flow_get_fn_cutgivennocut': flow_get_fn_cutgivennocut,
             'flow_kwargs': config.flow_kwargs,
             'prior_hparams': config.prior_hparams,
             'model_params_tupleclass': ModelParams,
             'model_params_cut_tupleclass': ModelParamsCut,
             'split_flow_fn_nocut': split_flow_nocut,
             'split_flow_fn_cut': split_flow_cut,
-            'smi_eta': smi_eta,
+            'sample_eta_fn': sample_eta_values,
+            'sample_eta_kwargs': {
+                'num_groups': config.num_groups,
+                'eta_sampling_a': 1.,
+                'eta_sampling_b': 1.
+            },
         },
     )
 
   @jax.jit
-  def elbo_validation_jit(state_list, batch, prng_key, smi_eta):
-    return elbo_smi(
+  def elbo_validation_jit(state_list, batch, prng_key):
+    return elbo_smi_vmpflow(
         lambda_tuple=tuple(state.params for state in state_list),
         batch=batch,
         prng_key=prng_key,
         num_samples=config.num_samples_eval,
         logprob_joint_fn=logprob_joint,
         flow_get_fn_nocut=flow_get_fn_nocut,
         flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
         flow_kwargs=config.flow_kwargs,
         prior_hparams=config.prior_hparams,
         model_params_tupleclass=ModelParams,
         model_params_cut_tupleclass=ModelParamsCut,
         split_flow_fn_nocut=split_flow_nocut,
         split_flow_fn_cut=split_flow_cut,
-        smi_eta=smi_eta,
+        sample_eta_fn=sample_eta_values,
+        sample_eta_kwargs={
+            'num_groups': config.num_groups,
+            'eta_sampling_a': 1.,
+            'eta_sampling_b': 1.
+        },
     )
 
-  if state_list[0].step < config.training_steps:
-    logging.info('Training variational posterior...')
+  if state_tuple[0].step < config.training_steps:
+    logging.info('Training Variational Meta-Posterior (VMP-flow)...')
 
   # Reset random key sequence
   prng_seq = hk.PRNGSequence(config.seed)
 
-  while state_list[0].step < config.training_steps:
+  while state_tuple[0].step < config.training_steps:
 
     # Plots to monitor training
-    if ((state_list[0].step == 0) or
-        (state_list[0].step % config.log_img_steps == 0)):
-      # print("Logging images...\n")
-      az_data = sample_q_as_az(
-          lambda_tuple=tuple(x.params for x in state_list),
-          dataset=train_ds,
+    if ((state_tuple[0].step == 0) or
+        (state_tuple[0].step % config.log_img_steps == 0)):
+      logging.info("\t\t Logging plots...")
+      log_images(
+          state_list=state_tuple,
           prng_key=next(prng_seq),
+          config=config,
+          dataset=train_ds,
+          num_samples_plot=config.num_samples_plot,
           flow_get_fn_nocut=flow_get_fn_nocut,
           flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
-          flow_kwargs=config.flow_kwargs,
-          sample_shape=(config.num_samples_plot,),
-      )
-      plot.posterior_plots(
-          az_data=az_data,
-          show_sigma_trace=False,
-          show_beta_trace=False,
-          show_tau_trace=False,
-          betasigma_pairplot_groups=(0, 1, 2),
-          tausigma_pairplot_groups=(0, 1, 2),
-          suffix=config.plot_suffix,
-          step=state_list[0].step,
-          workdir_png=workdir,
+          show_elpd_surface=True,
+          true_params=true_params,
           summary_writer=summary_writer,
+          workdir_png=workdir,
       )
+      logging.info("\t\t...done logging plots.")
 
     # Log learning rate
     summary_writer.scalar(
         tag='learning_rate',
         value=getattr(optax, config.optim_kwargs.lr_schedule_name)(
-            **config.optim_kwargs.lr_schedule_kwargs)(state_list[0].step),
-        step=state_list[0].step,
+            **config.optim_kwargs.lr_schedule_kwargs)(state_tuple[0].step),
+        step=state_tuple[0].step,
     )
 
     # SGD step
-    state_list, metrics = update_states_jit(
-        state_list=state_list,
+    state_tuple_, metrics = train_step_jit(
+        state_tuple=state_tuple,
         batch=train_ds,
         prng_key=next(prng_seq),
-        smi_eta=smi_eta,
     )
-    # The computed training loss corresponds to the model before update
+    if jax.lax.is_finite(metrics['train_loss']):
+      state_tuple = state_tuple_
+
     summary_writer.scalar(
         tag='train_loss',
         value=metrics['train_loss'],
-        step=state_list[0].step - 1,
+        step=state_tuple[0].step,
     )
 
-    if state_list[0].step == 1:
-      logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
+    if state_tuple[0].step == 1:
+      logging.info("STEP: %5d; training loss: %.3f", state_tuple[0].step,
                    metrics["train_loss"])
 
     # Metrics for evaluation
-    if state_list[0].step % config.eval_steps == 0:
-      logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
+    if state_tuple[0].step % config.eval_steps == 0:
+      logging.info("STEP: %5d; training loss: %.3f", state_tuple[0].step,
                    metrics["train_loss"])
 
       elbo_dict = elbo_validation_jit(
-          state_list=state_list,
+          state_list=state_tuple,
           batch=train_ds,
           prng_key=next(prng_seq),
-          smi_eta=smi_eta,
       )
       for k, v in elbo_dict.items():
         summary_writer.scalar(
             tag=f'elbo_{k}',
             value=v.mean(),
-            step=state_list[0].step,
+            step=state_tuple[0].step,
         )
 
-    if state_list[0].step % config.checkpoint_steps == 0:
-      for state_i, state_name_i in zip(state_list, state_name_list):
-        save_checkpoint(
-            state=state_i,
-            checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-            keep=config.checkpoints_keep,
-        )
-
-    # Wait until computations are done before the next step
-    # jax.random.normal(jax.random.PRNGKey(0), ()).block_until_ready()
+    for state, mngr in zip(state_tuple, orbax_ckpt_mngrs):
+      mngr.save(step=int(state.step), items=state)
 
-  logging.info('Final training step: %i', state_list[0].step)
-
-  # Saving checkpoint at the end of the training process
-  # (in case training_steps is not multiple of checkpoint_steps)
-  for state_i, state_name_i in zip(state_list, state_name_list):
-    save_checkpoint(
-        state=state_i,
-        checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-        keep=config.checkpoints_keep,
-    )
+  logging.info('Final training step: %i', state_tuple[0].step)
 
   # Last plot of posteriors
-  az_data = sample_q_as_az(
-      lambda_tuple=tuple(x.params for x in state_list),
-      dataset=train_ds,
+  log_images(
+      state_list=state_tuple,
       prng_key=next(prng_seq),
+      config=config,
+      dataset=train_ds,
+      num_samples_plot=config.num_samples_plot,
       flow_get_fn_nocut=flow_get_fn_nocut,
       flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
-      flow_kwargs=config.flow_kwargs,
-      sample_shape=(config.num_samples_plot,),
-  )
-  plot.posterior_plots(
-      az_data=az_data,
-      show_sigma_trace=False,
-      show_beta_trace=False,
-      show_tau_trace=False,
-      betasigma_pairplot_groups=(0, 1, 2),
-      tausigma_pairplot_groups=(0, 1, 2),
-      suffix=config.plot_suffix,
-      step=state_list[0].step,
-      workdir_png=workdir,
+      show_elpd_surface=True,
+      true_params=true_params,
       summary_writer=summary_writer,
+      workdir_png=workdir,
   )
 
-  return state_list
+  return state_tuple
 
 
 # # For debugging
 # config = get_config()
 # import pathlib
-# workdir = str(pathlib.Path.home() / f'modularbayes-output-exp/random_effects/nsf/full')
+# workdir = str(pathlib.Path.home() / f'modularbayes-output-exp/random_effects/nsf/vmp_flow')
 # # train_and_evaluate(config, workdir)
```

### Comparing `modularbayes-0.1.3/examples/random_effects/train_vmp_map.py` & `modularbayes-0.1.4/examples/random_effects/train_vmp_map.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,43 +2,39 @@
 
 import pathlib
 
 from absl import logging
 
 import numpy as np
 
+import matplotlib
 from matplotlib import pyplot as plt
 
-from flax.metrics import tensorboard
-
 import jax
 from jax import numpy as jnp
-
+from flax.metrics import tensorboard
+from flax.training.train_state import TrainState
 import haiku as hk
 import optax
-
-from tensorflow_probability.substrates import jax as tfp
+import orbax.checkpoint
 
 import flows
 from flows import split_flow_nocut, split_flow_cut
-import plot
-from train_flow import load_data, sample_q_as_az
 from log_prob_fun import (ModelParams, ModelParamsCut, SmiEta, logprob_joint,
                           sample_eta_values)
+import plot
+from train_flow import (elpd_waic, elpd_truth_mc, init_state_tuple, load_data,
+                        sample_q_as_az)
 
 import modularbayes
-from modularbayes import (sample_q_nocut, sample_q_cutgivennocut,
-                          elbo_smi_vmpmap)
-from modularbayes import (flatten_dict, plot_to_image, initial_state_ckpt,
-                          update_states, save_checkpoint)
-from modularbayes._src.utils.training import TrainState
+from modularbayes import elbo_smi_vmpmap, sample_q, train_step
+from modularbayes import (flatten_dict, plot_to_image, normalize_images)
 from modularbayes._src.typing import (Any, Array, Callable, ConfigDict, Dict,
-                                      List, Optional, PRNGKey, Tuple)
-
-kernels = tfp.math.psd_kernels
+                                      List, Optional, PRNGKey,
+                                      SmiPosteriorStates, Tuple)
 
 # Set high precision for matrix multiplication in jax
 jax.config.update('jax_default_matmul_precision', 'float32')
 
 np.set_printoptions(suppress=True, precision=4)
 
 
@@ -53,56 +49,194 @@
   optimizer = optax.chain(*[
       optax.clip_by_global_norm(max_norm=grad_clip_value),
       optax.adabelief(learning_rate=schedule),
   ])
   return optimizer
 
 
-def loss(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
+def print_trainable_params(
+    state_tuple: Tuple[TrainState],
+    config: ConfigDict,
+    lambda_init_tuple: Tuple,
+) -> None:
+  """Print a summary of the trainable parameters."""
+  tabulate_fn_ = hk.experimental.tabulate(
+      f=lambda state_i, lambda_init_i: state_i.apply_fn(
+          state_i.params,
+          eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
+          lambda_init=lambda_init_i),
+      columns=(
+          "module",
+          "owned_params",
+          "params_size",
+          "params_bytes",
+      ),
+      filters=("has_params",),
+  )
+  summary = tabulate_fn_(state_tuple[0], lambda_init_tuple[0])
+  logging.info('VMP-MAP no-cut parameters:')
+  for line in summary.split("\n"):
+    logging.info(line)
+
+  summary = tabulate_fn_(state_tuple[1], lambda_init_tuple[1])
+  logging.info('VMP-MAP cut parameters:')
+  for line in summary.split("\n"):
+    logging.info(line)
+
+
+def loss_fn(params_tuple: Tuple[hk.Params], *args, **kwargs) -> Array:
   """Define training loss function."""
 
   # Compute ELBO.
   elbo_dict = elbo_smi_vmpmap(alpha_tuple=params_tuple, *args, **kwargs)
 
   # Our loss is the Negative ELBO
   loss_avg = -(jnp.nanmean(elbo_dict['stage_1'] + elbo_dict['stage_2']))
 
   return loss_avg
 
 
+def plot_elpd_surface(
+    state_tuple: Tuple[TrainState],
+    dataset: Dict[str, Any],
+    prng_key: PRNGKey,
+    config: ConfigDict,
+    lambda_init_tuple: Tuple[hk.Params],
+    flow_get_fn_nocut: Callable,
+    flow_get_fn_cutgivennocut: Callable,
+    eta_grid: Array,
+    eta_grid_x_y_idx: Tuple[int, int],
+    true_params: Optional[ModelParams] = None,
+):
+  """Visualize ELPD surface as function of eta."""
+
+  assert eta_grid.ndim == 3
+  prng_seq = hk.PRNGSequence(prng_key)
+
+  num_groups = eta_grid.shape[-1]
+
+  # Jit functions for speed
+  elpd_waic_jit = jax.jit(elpd_waic)
+  elpd_truth_mc_jit = jax.jit(elpd_truth_mc)
+  sample_q_key_ = next(prng_seq)
+  sample_q_jit = jax.jit(lambda x: sample_q(
+      lambda_tuple=x,
+      prng_key=sample_q_key_,  # same seed for all etas, see less variability
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+      flow_kwargs=config.flow_kwargs,
+      model_params_tupleclass=ModelParams,
+      split_flow_fn_nocut=split_flow_nocut,
+      split_flow_fn_cut=split_flow_cut,
+      sample_shape=(config.num_samples_elpd,),
+  )['model_params_sample'])
+
+  # Produce flow parameters as a function of eta
+  lambda_tuple = tuple(
+      state_i.apply_fn(
+          state_i.params,
+          eta_values=eta_grid.reshape(-1, num_groups),
+          lambda_init=lambda_i,
+      ) for state_i, lambda_i in zip(state_tuple, lambda_init_tuple))
+  # state_tuple[0].apply_fn(state_tuple[0].params,eta_values=eta_grid.reshape(-1, num_groups),lambda_init=lambda_init_tuple[0])
+  if true_params is not None:
+    # Generate data from true model
+    z = jax.random.normal(
+        key=next(prng_seq), shape=(config.num_samples_elpd, num_groups))
+    y_new = true_params.sigma * z + true_params.beta
+  elpd_waic_grid = []
+  if true_params is not None:
+    elpd_grid = []
+  for i, eta_i in enumerate(eta_grid.reshape(-1, num_groups)):
+    # Sample from flow
+    model_params_sample_i = sample_q_jit(
+        jax.tree_map(lambda x: x[i], lambda_tuple))
+
+    # Compute ELPD using WAIC
+    elpd_waic_grid.append(
+        elpd_waic_jit(
+            model_params_sample=model_params_sample_i, dataset=dataset))
+    if true_params is not None:
+      # Compute ELPD
+      elpd_grid.append(
+          elpd_truth_mc_jit(
+              model_params_sample=model_params_sample_i, y_new=y_new))
+
+  # Plot the ELPD surface.
+  fig, axs = plt.subplots(
+      nrows=1,
+      ncols=1 if true_params is None else 2,
+      figsize=(4 if true_params is None else 8, 3),
+      subplot_kw={"projection": "3d"},
+      squeeze=False)
+  elpd_waic_grid = jnp.array(elpd_waic_grid).reshape(eta_grid.shape[:-1])
+  axs[0, 0].plot_surface(
+      eta_grid[..., eta_grid_x_y_idx[0]],
+      eta_grid[..., eta_grid_x_y_idx[1]],
+      -elpd_waic_grid,
+      cmap=matplotlib.cm.inferno,
+      # linewidth=0,
+      # antialiased=False,
+  )
+  axs[0, 0].view_init(30, 225)
+  axs[0, 0].set_xlabel(f'eta_{eta_grid_x_y_idx[0]}')
+  axs[0, 0].set_ylabel(f'eta_{eta_grid_x_y_idx[1]}')
+  axs[0, 0].set_title('- ELPD WAIC')
+  if true_params is not None:
+    elpd_grid = jnp.array(elpd_grid).reshape(eta_grid.shape[:-1])
+    axs[0, 1].plot_surface(
+        eta_grid[..., eta_grid_x_y_idx[0]],
+        eta_grid[..., eta_grid_x_y_idx[1]],
+        -elpd_grid,
+        cmap=matplotlib.cm.inferno,
+        # linewidth=0,
+        # antialiased=False,
+    )
+    axs[0, 1].view_init(30, 225)
+    axs[0, 1].set_xlabel(f'eta_{eta_grid_x_y_idx[0]}')
+    axs[0, 1].set_ylabel(f'eta_{eta_grid_x_y_idx[1]}')
+    axs[0, 1].set_title('- ELPD')
+  fig.tight_layout()
+
+  return fig, axs
+
+
 def log_images(
-    state_list: Tuple[TrainState],
+    state_tuple: Tuple[TrainState],
     prng_key: PRNGKey,
     config: ConfigDict,
     dataset: Dict[str, Any],
     num_samples_plot: int,
-    vmpmap_fn: hk.Transformed,
-    lambda_init_list: List[hk.Params],
+    lambda_init_tuple: Tuple[hk.Params],
     flow_get_fn_nocut: Callable,
     flow_get_fn_cutgivennocut: Callable,
+    show_elpd_surface: bool,
+    true_params: ModelParams,
     summary_writer: Optional[tensorboard.SummaryWriter] = None,
     workdir_png: Optional[str] = None,
 ) -> None:
   """Plots to monitor during training."""
 
+  model_name = 'random_effects'
+
   prng_seq = hk.PRNGSequence(prng_key)
 
   assert len(config.smi_eta_plot.keys()) > 0, 'No eta values to plot'
 
   # We can obtain the variational parameters for all eta values at once
   smi_etas = SmiEta(groups=jnp.array(config.smi_eta_plot.values()))
   eta_values = (
       smi_etas[0] if len(smi_etas) == 1 else jnp.stack(smi_etas, axis=-1))
   # Produce flow parameters as a function of eta
   lambda_tuple = [
-      vmpmap_fn.apply(
+      state_i.apply_fn(
           state_i.params,
           eta_values=eta_values,
           lambda_init=lambda_i,
-      ) for state_i, lambda_i in zip(state_list, lambda_init_list)
+      ) for state_i, lambda_i in zip(state_tuple, lambda_init_tuple)
   ]
 
   # Sample from flows and plot, one eta at a time
   for i, suffix in enumerate(config.smi_eta_plot.keys()):
     az_data = sample_q_as_az(
         lambda_tuple=jax.tree_map(lambda x: x[i], lambda_tuple),
         dataset=dataset,
@@ -116,19 +250,86 @@
         az_data=az_data,
         show_sigma_trace=False,
         show_beta_trace=False,
         show_tau_trace=False,
         betasigma_pairplot_groups=(0, 1, 2),
         tausigma_pairplot_groups=(0, 1, 2),
         suffix=f'_{suffix}',
-        step=state_list[0].step,
+        step=state_tuple[0].step,
         workdir_png=workdir_png,
         summary_writer=summary_writer,
     )
 
+  if show_elpd_surface:
+    eta_grid_len = 10
+    images = []
+
+    # Define elements to grate grid of eta values
+    eta_grid_base = np.tile(
+        np.array([0., 0.] + [1. for _ in range(config.num_groups - 2)]),
+        [eta_grid_len + 1, eta_grid_len + 1, 1])
+    eta_grid_mini = np.stack(
+        np.meshgrid(
+            np.linspace(0, 1, eta_grid_len + 1).round(5),
+            np.linspace(0, 1, eta_grid_len + 1).round(5)),
+        axis=0).T
+
+    # Vary eta_0 and eta_1
+    plot_name = f'{model_name}_elpd_surface_eta_0_1'
+    eta_grid = eta_grid_base.copy()
+    eta_grid_x_y_idx = [0, 1]
+    eta_grid[:, :, eta_grid_x_y_idx] = eta_grid_mini
+    fig, _ = plot_elpd_surface(
+        state_tuple=state_tuple,
+        dataset=dataset,
+        prng_key=next(prng_seq),
+        config=config,
+        lambda_init_tuple=lambda_init_tuple,
+        flow_get_fn_nocut=flow_get_fn_nocut,
+        flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+        eta_grid=eta_grid,
+        eta_grid_x_y_idx=eta_grid_x_y_idx,
+        true_params=true_params,
+    )
+    if workdir_png:
+      fig.savefig(pathlib.Path(workdir_png) / (plot_name + ".png"))
+    if summary_writer:
+      images.append(plot_to_image(fig))
+
+    # Vary eta_0 and eta_2
+    plot_name = f'{model_name}_elpd_surface_eta_0_2'
+    eta_grid = eta_grid_base.copy()
+    eta_grid_x_y_idx = [0, 2]
+    eta_grid[:, :, eta_grid_x_y_idx] = eta_grid_mini
+    fig, _ = plot_elpd_surface(
+        state_tuple=state_tuple,
+        dataset=dataset,
+        prng_key=next(prng_seq),
+        config=config,
+        lambda_init_tuple=lambda_init_tuple,
+        flow_get_fn_nocut=flow_get_fn_nocut,
+        flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+        eta_grid=eta_grid,
+        eta_grid_x_y_idx=eta_grid_x_y_idx,
+        true_params=true_params,
+    )
+    if workdir_png:
+      fig.savefig(pathlib.Path(workdir_png) / (plot_name + ".png"))
+    if summary_writer:
+      images.append(plot_to_image(fig))
+
+    if summary_writer:
+      plot_name = f"{model_name}_elpd_surface"
+      summary_writer.image(
+          tag=plot_name,
+          image=normalize_images(images),
+          step=state_tuple[0].step,
+          max_outputs=len(images),
+      )
+
 
 def train_and_evaluate(config: ConfigDict, workdir: str) -> TrainState:
   """Execute model training and evaluation loop.
 
   Args:
     config: Hyperparameter configuration for training and evaluation.
     workdir: Directory where the tensorboard summaries are written to.
@@ -174,121 +375,87 @@
 
   # Functions that generate the NF for no-cut params
   flow_get_fn_nocut = getattr(flows, 'get_q_nocut_' + config.flow_name)
   # Functions that generate the NF for cut params (conditional on no-cut params)
   flow_get_fn_cutgivennocut = getattr(flows,
                                       'get_q_cutgivennocut_' + config.flow_name)
 
-  checkpoint_dir = str(pathlib.Path(workdir) / 'checkpoints')
-  state_list = []
-  state_name_list = []
-  lambda_init_list = []
-
   # To initialize the VMP-map, we need one example of its output
   # The output of the VMP-map is lambda, the parameters of the variational posterior
-  state_name_list.append('alpha_nocut')
-  lambda_init_list.append(
-      sample_q_nocut.init(
-          next(prng_seq),
-          flow_get_fn=flow_get_fn_nocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_nocut,
-          sample_shape=(config.num_samples_elbo,),
-      ))
-  nocut_base_sample_init = sample_q_nocut.apply(
-      lambda_init_list[0],
-      next(prng_seq),
-      flow_get_fn=flow_get_fn_nocut,
-      flow_kwargs=config.flow_kwargs,
-      split_flow_fn=split_flow_nocut,
+  lambda_init_tuple = init_state_tuple(
+      prng_key=next(prng_seq),
+      config=config,
+      flow_get_fn_nocut=flow_get_fn_nocut,
+      flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
       sample_shape=(config.num_samples_elbo,),
-  )['sample_base']
-  state_name_list.append('alpha_cut')
-  lambda_init_list.append(
-      sample_q_cutgivennocut.init(
-          next(prng_seq),
-          flow_get_fn=flow_get_fn_cutgivennocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_cut,
-          nocut_base_sample=nocut_base_sample_init,
-      ))
-  state_name_list.append('alpha_cut_aux')
-  lambda_init_list.append(
-      sample_q_cutgivennocut.init(
-          next(prng_seq),
-          flow_get_fn=flow_get_fn_cutgivennocut,
-          flow_kwargs=config.flow_kwargs,
-          split_flow_fn=split_flow_cut,
-          nocut_base_sample=nocut_base_sample_init,
-      ))
+      eta_values=None,
+  )
+  lambda_init_tuple = [x.params for x in lambda_init_tuple]
 
   # Define function that produce a tuple of lambda (flow parameters)
   @hk.without_apply_rng
   @hk.transform
   def vmpmap_fn(eta_values, lambda_init):
     vmpmap = getattr(modularbayes, config.vmp_map_name)(
         **config.vmp_map_kwargs, params_flow_init=lambda_init)
     lambda_out = vmpmap(eta_values)
     return lambda_out
 
   ### Initialise Variational Meta-Posterior Map ###
-  state_list = [
-      initial_state_ckpt(
-          checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-          forward_fn=vmpmap_fn,
-          forward_fn_kwargs={
-              'eta_values':
-                  jnp.ones((config.num_samples_eta, config.smi_eta_dim)),
-              'lambda_init':
-                  lambda_init_i
-          },
-          prng_key=next(prng_seq),
-          optimizer=make_optimizer(**config.optim_kwargs),
-      )
-      for state_name_i, lambda_init_i in zip(state_name_list, lambda_init_list)
+  params_tuple_ = [
+      vmpmap_fn.init(
+          next(prng_seq),
+          eta_values=jnp.ones((config.num_samples_elbo, config.smi_eta_dim)),
+          lambda_init=lambda_init_) for lambda_init_ in lambda_init_tuple
   ]
-  # globals().update(forward_fn_kwargs)
+  state_tuple = SmiPosteriorStates(*[
+      TrainState.create(
+          apply_fn=vmpmap_fn.apply,
+          params=params_,
+          tx=make_optimizer(**config.optim_kwargs),
+      ) for params_ in params_tuple_
+  ])
 
-  # Print a useful summary of the execution of the VHP-map architecture.
-  tabulate_fn_ = hk.experimental.tabulate(
-      f=lambda state_i, lambda_init_i: vmpmap_fn.apply(
-          state_i.params,
-          eta_values=jnp.ones((config.num_samples_eta, config.smi_eta_dim)),
-          lambda_init=lambda_init_i),
-      columns=(
-          "module",
-          "owned_params",
-          "params_size",
-          "params_bytes",
-      ),
-      filters=("has_params",),
+  print_trainable_params(
+      state_tuple=state_tuple,
+      config=config,
+      lambda_init_tuple=lambda_init_tuple,
   )
-  summary = tabulate_fn_(state_list[0], lambda_init_list[0])
-  logging.info('VMP-MAP no-cut parameters:')
-  for line in summary.split("\n"):
-    logging.info(line)
 
-  summary = tabulate_fn_(state_list[1], lambda_init_list[1])
-  logging.info('VMP-MAP cut parameters:')
-  for line in summary.split("\n"):
-    logging.info(line)
+  # Create checkpoint managers for the three states
+  orbax_ckpt_mngrs = [
+      orbax.checkpoint.CheckpointManager(
+          directory=str(pathlib.Path(workdir) / 'checkpoints' / state_name),
+          checkpointers=orbax.checkpoint.PyTreeCheckpointer(),
+          options=orbax.checkpoint.CheckpointManagerOptions(
+              max_to_keep=1,
+              save_interval_steps=config.checkpoint_steps,
+          ),
+      ) for state_name in state_tuple._asdict()
+  ]
 
-  ### Training VMP map ###
+  # Restore existing checkpoint if present
+  if orbax_ckpt_mngrs[0].latest_step() is not None:
+    state_tuple = [
+        mngr.restore(mngr.latest_step(), items=state)
+        for state, mngr in zip(state_tuple, orbax_ckpt_mngrs)
+    ]
+
+  # Jit function to update training states
   @jax.jit
-  def update_states_jit(state_list, batch, prng_key):
-    return update_states(
-        state_list=state_list,
+  def train_step_jit(state_tuple, batch, prng_key):
+    return train_step(
+        state_tuple=state_tuple,
         batch=batch,
         prng_key=prng_key,
-        optimizer=make_optimizer(**config.optim_kwargs),
-        loss_fn=loss,
-        loss_fn_kwargs={
-            'num_samples': config.num_samples_eta,
+        loss=loss_fn,
+        loss_kwargs={
+            'num_samples': config.num_samples_elbo,
             'vmpmap_fn': vmpmap_fn,
-            'lambda_init_tuple': tuple(lambda_init_list),
+            'lambda_init_tuple': lambda_init_tuple,
             'sample_eta_fn': sample_eta_values,
             'sample_eta_kwargs': {
                 'num_groups': config.num_groups,
                 'eta_sampling_a': config.eta_sampling_a,
                 'eta_sampling_b': config.eta_sampling_b
             },
             'elbo_smi_kwargs': {
@@ -301,111 +468,99 @@
                 'model_params_cut_tupleclass': ModelParamsCut,
                 'split_flow_fn_nocut': split_flow_nocut,
                 'split_flow_fn_cut': split_flow_cut,
             }
         },
     )
 
-  if state_list[0].step < config.training_steps:
+  if state_tuple[0].step < config.training_steps:
     logging.info('Training Variational Meta-Posterior (VMP-map)...')
 
   # Reset random key sequence
   prng_seq = hk.PRNGSequence(config.seed)
 
-  while state_list[0].step < config.training_steps:
+  while state_tuple[0].step < config.training_steps:
 
     # Plots to monitor training
     if (config.log_img_steps
-        is not None) and ((state_list[0].step == 1) or
-                          (state_list[0].step % config.log_img_steps == 0)):
-      # print("Logging images...\n")
+        is not None) and (state_tuple[0].step % config.log_img_steps == 0):
+      logging.info("\t\t Logging plots...")
       log_images(
-          state_list=state_list,
+          state_tuple=state_tuple,
           prng_key=next(prng_seq),
           config=config,
           dataset=train_ds,
           num_samples_plot=config.num_samples_plot,
-          vmpmap_fn=vmpmap_fn,
-          lambda_init_list=lambda_init_list,
+          lambda_init_tuple=lambda_init_tuple,
           flow_get_fn_nocut=flow_get_fn_nocut,
           flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+          show_elpd_surface=True,
+          true_params=true_params,
           summary_writer=summary_writer,
           workdir_png=workdir,
       )
       plt.close()
+      logging.info("\t\t...done logging plots.")
 
     # Log learning rate
     summary_writer.scalar(
         tag='learning_rate',
         value=getattr(optax, config.optim_kwargs.lr_schedule_name)(
-            **config.optim_kwargs.lr_schedule_kwargs)(state_list[0].step),
-        step=state_list[0].step,
+            **config.optim_kwargs.lr_schedule_kwargs)(state_tuple[0].step),
+        step=state_tuple[0].step,
     )
 
-    state_list, metrics = update_states_jit(
-        state_list=state_list,
+    # SGD step
+    state_tuple_, metrics = train_step_jit(
+        state_tuple=state_tuple,
         batch=train_ds,
         prng_key=next(prng_seq),
     )
+    if jax.lax.is_finite(metrics['train_loss']):
+      state_tuple = state_tuple_
 
     # The computed training loss would correspond to the model before update
     summary_writer.scalar(
         tag='train_loss',
         value=metrics['train_loss'],
-        step=state_list[0].step - 1,
+        step=state_tuple[0].step - 1,
     )
 
-    if state_list[0].step == 2:
-      logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
+    if state_tuple[0].step == 2:
+      logging.info("STEP: %5d; training loss: %.3f", state_tuple[0].step - 1,
                    metrics["train_loss"])
 
-    if state_list[0].step % config.eval_steps == 0:
-      logging.info("STEP: %5d; training loss: %.3f", state_list[0].step - 1,
+    if state_tuple[0].step % config.eval_steps == 0:
+      logging.info("STEP: %5d; training loss: %.3f", state_tuple[0].step - 1,
                    metrics["train_loss"])
 
     # Save checkpoints
-    if (state_list[0].step) % config.checkpoint_steps == 0:
-      for state_i, state_name_i in zip(state_list, state_name_list):
-        save_checkpoint(
-            state=state_i,
-            checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-            keep=config.checkpoints_keep,
-        )
-
-    # Wait until computations are done before the next step
-    # jax.random.normal(jax.random.PRNGKey(0), ()).block_until_ready()
-
-  logging.info('Final training step: %i', state_list[0].step)
-
-  # Save checkpoints at the end of the training process
-  # (in case training_steps is not multiple of checkpoint_steps)
-  for state_i, state_name_i in zip(state_list, state_name_list):
-    save_checkpoint(
-        state=state_i,
-        checkpoint_dir=f'{checkpoint_dir}/{state_name_i}',
-        keep=config.checkpoints_keep,
-    )
+    for state, mngr in zip(state_tuple, orbax_ckpt_mngrs):
+      mngr.save(step=int(state.step), items=state)
+
+  logging.info('Final training step: %i', state_tuple[0].step)
 
   # Last plot of posteriors
   log_images(
-      state_list=state_list,
+      state_tuple=state_tuple,
       prng_key=next(prng_seq),
       config=config,
       dataset=train_ds,
       num_samples_plot=config.num_samples_plot,
-      vmpmap_fn=vmpmap_fn,
-      lambda_init_list=lambda_init_list,
+      lambda_init_tuple=lambda_init_tuple,
       flow_get_fn_nocut=flow_get_fn_nocut,
       flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
+      show_elpd_surface=True,
+      true_params=true_params,
       summary_writer=summary_writer,
       workdir_png=workdir,
   )
   plt.close()
 
-  return state_list
+  return state_tuple
 
 
 # # For debugging
 # config = get_config()
 # import pathlib
 # workdir = str(pathlib.Path.home() / f'modularbayes-output-exp/random_effects/nsf/vmp_map')
 # # train_and_evaluate(config, workdir)
```

### Comparing `modularbayes-0.1.3/modularbayes/__init__.py` & `modularbayes-0.1.4/modularbayes/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """modularbayes: Variational methods for Bayesian Semi-Modular Inference."""
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 from modularbayes._src.bijectors.blockwise import Blockwise
 from modularbayes._src.bijectors.conditional_bijector import ConditionalBijector
 from modularbayes._src.bijectors.conditional_chain import ConditionalChain
 from modularbayes._src.bijectors.conditional_masked_coupling import ConditionalMaskedCoupling
-from modularbayes._src.bijectors.conditional_masked_coupling_extra import EtaConditionalMaskedCoupling
 
 from modularbayes._src.conditioners.base import MeanFieldConditioner
 from modularbayes._src.conditioners.base import MLPConditioner
 
 from modularbayes._src.distributions.conditional_transformed import ConditionalTransformed
 from modularbayes._src.distributions.transformed import Transformed
 
@@ -27,29 +26,21 @@
 from modularbayes._src.utils.misc import clean_filename
 from modularbayes._src.utils.misc import colour_fader
 from modularbayes._src.utils.misc import flatten_dict
 from modularbayes._src.utils.misc import list_from_csv
 from modularbayes._src.utils.misc import plot_to_image
 from modularbayes._src.utils.misc import normalize_images
 
-from modularbayes._src.utils.training import TrainState
-from modularbayes._src.utils.training import initial_state
-from modularbayes._src.utils.training import initial_state_ckpt
-from modularbayes._src.utils.training import load_ckpt
-from modularbayes._src.utils.training import save_ckpt
-from modularbayes._src.utils.training import save_checkpoint
-from modularbayes._src.utils.training import update_state
-from modularbayes._src.utils.training import update_states
+from modularbayes._src.utils.training import train_step
 
 __all__ = (
     'Blockwise',
     'ConditionalBijector',
     'ConditionalChain',
     'ConditionalMaskedCoupling',
-    'EtaConditionalMaskedCoupling',
     'MeanFieldConditioner',
     'MLPConditioner',
     'ConditionalTransformed',
     'Transformed',
     'MLPVmpMap',
     'sample_q_nocut',
     'sample_q_cutgivennocut',
@@ -60,16 +51,9 @@
     'cart2pol',
     'clean_filename',
     'colour_fader',
     'flatten_dict',
     'list_from_csv',
     'plot_to_image',
     'normalize_images',
-    'TrainState',
-    'initial_state',
-    'initial_state_ckpt',
-    'load_ckpt',
-    'save_ckpt',
-    'save_checkpoint',
-    'update_state',
-    'update_states',
+    'train_step',
 )
```

### Comparing `modularbayes-0.1.3/modularbayes/_src/bijectors/blockwise.py` & `modularbayes-0.1.4/modularbayes/_src/bijectors/blockwise.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_bijector.py` & `modularbayes-0.1.4/modularbayes/_src/bijectors/conditional_bijector.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_chain.py` & `modularbayes-0.1.4/modularbayes/_src/bijectors/conditional_chain.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/modularbayes/_src/bijectors/conditional_masked_coupling.py` & `modularbayes-0.1.4/modularbayes/_src/bijectors/conditional_masked_coupling.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/modularbayes/_src/conditioners/base.py` & `modularbayes-0.1.4/modularbayes/_src/conditioners/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 2) Bijector: Transform epsilon using a function that depend on the parameters
      produced by the conditioner.
      Eg. Affine transformation: epsilon_t * scale_t + loc_t
 
 In this script we define functions that can be used as conditioners.
 """
 
+import jax
 from jax import numpy as jnp
+
 import haiku as hk
 
 from modularbayes._src.typing import Optional, Sequence
 
 
 class MeanFieldConditioner(hk.Module):
   """Mean Field Conditioner.
@@ -60,25 +62,32 @@
       num_bijector_params: int,
       name: Optional[str] = "nsf_conditioner",
   ):
     super().__init__(name=name)
     self.output_dim = output_dim
     self.hidden_sizes = hidden_sizes
     self.num_bijector_params = num_bijector_params
+    layers = [
+        hk.Flatten(preserve_dims=-1),
+        hk.nets.MLP(
+            output_sizes=self.hidden_sizes,
+            activate_final=True,
+        ),
+        # We initialize this linear layer to zero so that the flow is initialized
+        # to the identity function.
+        hk.Linear(
+            self.output_dim * self.num_bijector_params,
+            w_init=jnp.zeros,
+            b_init=jnp.zeros,
+        ),
+        hk.Reshape(
+            (self.output_dim,) + (self.num_bijector_params,),
+            preserve_dims=-1,
+        )
+    ]
+    self.layers = tuple(layers)
 
   def __call__(self, inputs):
-
-    out = hk.Flatten(preserve_dims=-1)(inputs)
-    out = hk.nets.MLP(self.hidden_sizes, activate_final=True)(out)
-
-    # We initialize this linear layer to zero so that the flow is initialized
-    # to the identity function.
-    out = hk.Linear(
-        self.output_dim * self.num_bijector_params,
-        w_init=jnp.zeros,
-        b_init=jnp.zeros)(
-            out)
-    out = hk.Reshape(
-        (self.output_dim,) + (self.num_bijector_params,), preserve_dims=-1)(
-            out)
-
+    out = inputs
+    for layer in self.layers:
+      out = layer(out)
     return out
```

### Comparing `modularbayes-0.1.3/modularbayes/_src/distributions/conditional_transformed.py` & `modularbayes-0.1.4/modularbayes/_src/distributions/conditional_transformed.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/modularbayes/_src/distributions/transformed.py` & `modularbayes-0.1.4/modularbayes/_src/distributions/transformed.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/modularbayes/_src/metaposterior/vmp_map.py` & `modularbayes-0.1.4/modularbayes/_src/metaposterior/vmp_map.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,32 +35,29 @@
 
     num_eta_new, _ = eta.shape
 
     vmp_map = hk.Sequential([
         hk.Flatten(preserve_dims=-1),
         hk.nets.MLP(
             output_sizes=self.hidden_sizes,
-            activation=jax.nn.leaky_relu,
             activate_final=True,
         ),
         hk.Linear(output_size=self.output_dim),
     ])
     flow_params_merged = jax.vmap(vmp_map)(eta)
 
     # out1 = hk.Flatten(preserve_dims=-1)(eta)
     # out1 = hk.nets.MLP(
     #     self.hidden_sizes,
-    #     activation=jax.nn.leaky_relu,
     #     activate_final=True,
     # )(
     #     out1)
     # out2 = hk.Flatten(preserve_dims=-1)(eta)
     # out2 = hk.nets.MLP(
     #     self.hidden_sizes[-1:],
-    #     activation=jax.nn.leaky_relu,
     #     activate_final=True,
     # )(
     #     out2)
     # flow_params_merged = hk.Linear(output_size=self.output_dim)(out1 + out2)
 
     leaves_eta = []
     for i in range(len(self.params_flow_shapes) - 1):
```

### Comparing `modularbayes-0.1.3/modularbayes/_src/smi/elbo.py` & `modularbayes-0.1.4/modularbayes/_src/smi/elbo.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
       prng_key=prng_key,
       flow_get_fn_nocut=flow_get_fn_nocut,
       flow_get_fn_cutgivennocut=flow_get_fn_cutgivennocut,
       flow_kwargs=flow_kwargs,
       model_params_tupleclass=model_params_tupleclass,
       split_flow_fn_nocut=split_flow_fn_nocut,
       split_flow_fn_cut=split_flow_fn_cut,
+      sample_shape=(num_samples,),
       eta_values=(smi_etas[0] if len(smi_etas) == 1 else jnp.stack(
           smi_etas, axis=-1)),
   )
 
   # ELBO stage 1: Power posterior
   log_prob_joint_stg1 = jax.vmap(lambda x, y: logprob_joint_fn(
       batch=batch,
@@ -196,13 +197,13 @@
   ]
 
   # Compute ELBO.
   elbo_dict = jax.vmap(lambda x, y, z: elbo_smi(
       lambda_tuple=x,
       prng_key=y,
       smi_eta=z,
-      num_samples=1,
+      num_samples=1,  # Only one sample per eta value.
       batch=batch,
       **elbo_smi_kwargs,
   ))(lambda_tuple, jax.random.split(next(prng_seq), num_samples), smi_etas)
 
   return elbo_dict
```

### Comparing `modularbayes-0.1.3/modularbayes/_src/smi/sampling.py` & `modularbayes-0.1.4/modularbayes/_src/smi/sampling.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 """Sampling from the Semi-Modular posterior using normalizing flows."""
 
 import jax
-
+from jax import numpy as jnp
 import haiku as hk
 
 from modularbayes._src.typing import (Any, Array, Callable, Dict, IntLike,
                                       Optional, PRNGKey, Tuple)
 
 
 @hk.transform
 def sample_q_nocut(
     flow_get_fn: Callable,
     flow_kwargs: Dict[str, Any],
     split_flow_fn: Callable,
-    sample_shape: Optional[Tuple[IntLike]] = None,
+    sample_shape: Optional[Tuple[IntLike]],
     eta_values: Optional[Array] = None,
 ) -> Dict[str, Any]:
   """Sample from variational posterior for no-cut parameters."""
 
   q_output = {}
 
   # Define normalizing flows
-  q_distr = flow_get_fn(**flow_kwargs)
+  q_distr = flow_get_fn(is_meta=(eta_values is not None), **flow_kwargs)
 
-  assert sample_shape is not None or eta_values is not None, (
-      'Either sample_shape or eta_values must be provided.')
-  assert sample_shape is None or eta_values is None, (
-      'Only one of sample_shape or eta_values must be provided.')
-
-  if eta_values is None:
-    kwargs_distr_ = {'sample_shape': sample_shape}
-  else:
-    kwargs_distr_ = {
-        'sample_shape': (eta_values.shape[0],),
-        'context': (eta_values, None)
-    }
+  kwargs_distr_ = {'sample_shape': sample_shape}
+  if eta_values is not None:
+    assert eta_values.ndim == 2
+    assert (eta_values.shape[0],) == sample_shape
+    kwargs_distr_['context'] = eta_values
 
   # Sample from flows
   (sample_flow_concat, sample_logprob,
    sample_base) = q_distr.sample_and_log_prob_with_base(
        seed=hk.next_rng_key(), **kwargs_distr_)
 
   # Split flow into model parameters
@@ -66,26 +59,23 @@
     eta_values: Optional[Array] = None,
 ) -> Dict[str, Any]:
   """Sample from variational posterior for cut parameters
   Conditional on values of no-cut parameters."""
 
   q_output = {}
 
-  if eta_values is None:
-    kwargs_distr_ = {
-        'sample_shape': (nocut_base_sample.shape[0],),
-        'context': nocut_base_sample,
-    }
-  else:
+  kwargs_distr_ = {
+      'sample_shape': (nocut_base_sample.shape[0],),
+      'context': nocut_base_sample,
+  }
+  if eta_values is not None:
     assert nocut_base_sample.shape[0] == eta_values.shape[0], (
-        'First diension of nocut_base_sample and eta_valuesmust match.')
-    kwargs_distr_ = {
-        'sample_shape': (nocut_base_sample.shape[0],),
-        'context': (eta_values, nocut_base_sample),
-    }
+        'First dimension of nocut_base_sample and eta_valuesmust match.')
+    kwargs_distr_['context'] = jnp.concatenate([nocut_base_sample, eta_values],
+                                               axis=-1)
 
   # Define normalizing flows
   q_distr = flow_get_fn(**flow_kwargs)
 
   # Sample from flows
   (sample, sample_logprob) = q_distr.sample_and_log_prob(
       seed=hk.next_rng_key(), **kwargs_distr_)
@@ -108,26 +98,25 @@
     prng_key: PRNGKey,
     flow_get_fn_nocut: Callable,
     flow_get_fn_cutgivennocut: Callable,
     flow_kwargs: Dict[str, Any],
     model_params_tupleclass: type,
     split_flow_fn_nocut: Callable,
     split_flow_fn_cut: Callable,
-    sample_shape: Optional[Tuple[IntLike]] = None,
+    sample_shape: Optional[Tuple[IntLike]],
     eta_values: Optional[Array] = None,
 ) -> Dict[str, Any]:
   """Sample from model posterior"""
 
   prng_seq = hk.PRNGSequence(prng_key)
 
-  assert sample_shape is not None or eta_values is not None, (
-      'Either sample_shape or eta_values must be provided.')
-  assert sample_shape is None or eta_values is None, (
-      'Only one of sample_shape or eta_values must be provided.')
-
+  if eta_values is not None:
+    assert eta_values.ndim == 2
+    assert (eta_values.shape[0],) == sample_shape
+    
   q_output = {}
 
   # Sample from q(no_cut_params)
   q_output_nocut_ = sample_q_nocut.apply(
       lambda_tuple[0],
       next(prng_seq),
       flow_get_fn=flow_get_fn_nocut,
```

### Comparing `modularbayes-0.1.3/modularbayes/_src/typing.py` & `modularbayes-0.1.4/modularbayes/_src/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Pytypes for arrays and scalars."""
 
 from typing import (Any, Callable, Dict, Iterable, Iterator, List, Mapping,
                     NamedTuple, Optional, Sequence, Tuple, Union)
 
 from pathlib import Path, PosixPath
 
+from collections import namedtuple
+
 import jax
 
 import numpy as np
 
 from chex import Array, PRNGKey
 
 from collections import OrderedDict
@@ -31,14 +33,19 @@
 Batch = Mapping[str, ArrayNumpy]
 
 RangeFloat = Tuple[float, float]
 RangeInt = Tuple[int, Union[int, None]]
 
 Kernel = tfp.math.psd_kernels.PositiveSemidefiniteKernel
 
+SmiPosteriorStates = namedtuple(
+    "smi_posterior_states",
+    field_names=('no_cut', 'cut', 'cut_aux'),
+)
+
 __all__ = [
     'Any',
     'Array',
     'ArrayNumpy',
     'ArraySharded',
     'BijectorParams',
     'Callable',
```

### Comparing `modularbayes-0.1.3/modularbayes/_src/utils/misc.py` & `modularbayes-0.1.4/modularbayes/_src/utils/misc.py`

 * *Files identical despite different names*

### Comparing `modularbayes-0.1.3/modularbayes.egg-info/PKG-INFO` & `modularbayes-0.1.4/modularbayes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modularbayes
-Version: 0.1.3
+Version: 0.1.4
 Summary: Modular Bayesian Inference.
 Home-page: https://github.com/chriscarmona/modularbayes
 Author: Chris Carmona
 Author-email: carmona@stats.ox.ac.uk
 Maintainer-email: carmona@stats.ox.ac.uk
 License: MIT
 Keywords: modular bayesian inference cut smi posterior probability distribution
@@ -50,16 +50,15 @@
 ```bash
 pip install -Ur examples/requirements.txt
 chmod +x examples/run.sh
 bash examples/run.sh
 ```
 Results produced during the optimization can be monitored in [Tensorboard](https://www.tensorflow.org/tensorboard):
 ```bash
-WORK_DIR=$HOME/modularbayes-output
-tensorboard --logdir=$WORK_DIR
+tensorboard --logdir=$HOME/modularbayes-output
 ```
 
 ## Installation instructions
 
 1. \[Optional] Create a new virtual environment for this project (see [*Create a virtual environment*](#create-a-virtual-environment) below).
 2. Install JAX. This may vary according to your CUDA version (See [JAX installation](https://github.com/google/jax#installation)).
 3. Install the latest released version of `modularbayes` from [Pypi](https://pypi.org/project/modularbayes/) via:
```

### Comparing `modularbayes-0.1.3/modularbayes.egg-info/SOURCES.txt` & `modularbayes-0.1.4/modularbayes.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 modularbayes/_src/__init__.py
 modularbayes/_src/typing.py
 modularbayes/_src/bijectors/__init__.py
 modularbayes/_src/bijectors/blockwise.py
 modularbayes/_src/bijectors/conditional_bijector.py
 modularbayes/_src/bijectors/conditional_chain.py
 modularbayes/_src/bijectors/conditional_masked_coupling.py
-modularbayes/_src/bijectors/conditional_masked_coupling_extra.py
 modularbayes/_src/conditioners/__init__.py
 modularbayes/_src/conditioners/base.py
 modularbayes/_src/distributions/__init__.py
 modularbayes/_src/distributions/conditional_transformed.py
 modularbayes/_src/distributions/transformed.py
 modularbayes/_src/metaposterior/__init__.py
 modularbayes/_src/metaposterior/vmp_map.py
```

### Comparing `modularbayes-0.1.3/setup.py` & `modularbayes-0.1.4/setup.py`

 * *Files identical despite different names*

