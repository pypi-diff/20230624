# Comparing `tmp/autooc-0.0.4.tar.gz` & `tmp/autooc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autooc-0.0.4.tar", last modified: Sat Jun 24 15:01:50 2023, max compression
+gzip compressed data, was "autooc-0.0.5.tar", last modified: Sat Jun 24 15:03:15 2023, max compression
```

## Comparing `autooc-0.0.4.tar` & `autooc-0.0.5.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.168871 autooc-0.0.4/
--rw-r--r--   0 luis      (1000) luis      (1000)     1071 2023-06-24 14:17:33.000000 autooc-0.0.4/LICENSE
--rw-r--r--   0 luis      (1000) luis      (1000)       42 2023-06-24 14:17:33.000000 autooc-0.0.4/MANIFEST.in
--rw-r--r--   0 luis      (1000) luis      (1000)    12343 2023-06-24 15:01:50.168871 autooc-0.0.4/PKG-INFO
--rw-r--r--   0 luis      (1000) luis      (1000)    11738 2023-06-24 14:29:17.000000 autooc-0.0.4/README.md
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.148872 autooc-0.0.4/autooc/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.148872 autooc-0.0.4/autooc/algorithm/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/algorithm/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.148872 autooc-0.0.4/autooc/algorithm/distributed_algorithm/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/algorithm/distributed_algorithm/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)      994 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/algorithm/distributed_algorithm/search_loop.py
--rw-r--r--   0 luis      (1000) luis      (1000)      426 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/algorithm/distributed_algorithm/step.py
--rw-r--r--   0 luis      (1000) luis      (1000)     9888 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/algorithm/hill_climbing.py
--rw-r--r--   0 luis      (1000) luis      (1000)    11897 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/algorithm/mapper.py
--rw-r--r--   0 luis      (1000) luis      (1000)    13826 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/algorithm/parameters.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2460 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/algorithm/search_loop.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1643 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/algorithm/step.py
--rw-r--r--   0 luis      (1000) luis      (1000)    25074 2023-06-24 14:30:26.000000 autooc-0.0.4/autooc/autooc.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.148872 autooc-0.0.4/autooc/fitness/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.148872 autooc-0.0.4/autooc/fitness/base_ff_classes/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/base_ff_classes/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2130 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/base_ff_classes/base_ff.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2587 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/base_ff_classes/ff_template.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2662 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/base_ff_classes/moo_ff.py
--rw-r--r--   0 luis      (1000) luis      (1000)      484 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/bic.py
--rw-r--r--   0 luis      (1000) luis      (1000)     5108 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/evaluation.py
--rw-r--r--   0 luis      (1000) luis      (1000)      362 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/minimise_nodes.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.158872 autooc-0.0.4/autooc/fitness/multi_objective/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/multi_objective/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)      796 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/multi_objective/binary_phenotype_to_float.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3944 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/multi_objective/singlefit_autoencoders.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1845 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/multi_objective/singlefit_multiobj.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1007 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/multi_objective/zdt1.py
--rw-r--r--   0 luis      (1000) luis      (1000)      407 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/num_params.py
--rw-r--r--   0 luis      (1000) luis      (1000)      403 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/predict_time.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6022 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/progsys.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1337 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/pymax.py
--rw-r--r--   0 luis      (1000) luis      (1000)     5886 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/sequence_match.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1038 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/string_match.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.158872 autooc-0.0.4/autooc/fitness/supervised_learning/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/supervised_learning/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3731 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/supervised_learning/boolean_problem.py
--rw-r--r--   0 luis      (1000) luis      (1000)      659 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/supervised_learning/classification.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2912 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/supervised_learning/if_else_classifier.py
--rw-r--r--   0 luis      (1000) luis      (1000)      643 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/supervised_learning/regression.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4478 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/supervised_learning/regression_random_polynomial.py
--rw-r--r--   0 luis      (1000) luis      (1000)    10335 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/supervised_learning/supervised_learning.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3627 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/supervised_learning/supervised_learning_backup.py
--rw-r--r--   0 luis      (1000) luis      (1000)      406 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/fitness/training_time.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.158872 autooc-0.0.4/autooc/operators/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/operators/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    16352 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/operators/crossover.py
--rw-r--r--   0 luis      (1000) luis      (1000)    16207 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/operators/initialisation.py
--rw-r--r--   0 luis      (1000) luis      (1000)     8189 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/operators/mutation.py
--rw-r--r--   0 luis      (1000) luis      (1000)     5351 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/operators/replacement.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4486 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/operators/selection.py
--rw-r--r--   0 luis      (1000) luis      (1000)    28915 2023-06-24 14:17:34.000000 autooc-0.0.4/autooc/operators/subtree_parse.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.158872 autooc-0.0.4/autooc/representation/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/representation/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    14379 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/representation/derivation.py
--rw-r--r--   0 luis      (1000) luis      (1000)    28989 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/representation/grammar.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6994 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/representation/individual.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6384 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/representation/latent_tree.py
--rw-r--r--   0 luis      (1000) luis      (1000)     8567 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/representation/tree.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.158872 autooc-0.0.4/autooc/scripts/
--rw-r--r--   0 luis      (1000) luis      (1000)    13836 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/scripts/GE_LR_parser.py
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/scripts/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3387 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/scripts/baselines.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2532 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/scripts/experiment_manager.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2642 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/scripts/grammar_analyser.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4583 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/scripts/python_script_evaluation.py
--rw-r--r--   0 luis      (1000) luis      (1000)    10267 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/scripts/stats_parser.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.158872 autooc-0.0.4/autooc/stats/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/stats/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    13101 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/stats/stats.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.158872 autooc-0.0.4/autooc/utilities/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.158872 autooc-0.0.4/autooc/utilities/algorithm/
--rw-r--r--   0 luis      (1000) luis      (1000)    12775 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/algorithm/NSGA2.py
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/algorithm/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    23627 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/algorithm/command_line_parser.py
--rw-r--r--   0 luis      (1000) luis      (1000)      418 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/algorithm/general.py
--rw-r--r--   0 luis      (1000) luis      (1000)    11564 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/algorithm/initialise_run.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4433 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/algorithm/state.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.158872 autooc-0.0.4/autooc/utilities/fitness/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/fitness/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     8348 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/fitness/error_metric.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3663 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/fitness/get_data.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6753 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/fitness/math_functions.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2993 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/fitness/optimize_constants.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.168871 autooc-0.0.4/autooc/utilities/representation/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/representation/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    13533 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/representation/check_methods.py
--rw-r--r--   0 luis      (1000) luis      (1000)      720 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/representation/python_filter.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.168871 autooc-0.0.4/autooc/utilities/stats/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/stats/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)      498 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/stats/clean_stats.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6086 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/stats/file_io.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4512 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/stats/save_plots.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1015 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/stats/trackers.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1966 2023-06-24 14:17:35.000000 autooc-0.0.4/autooc/utilities/utils.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:01:50.148872 autooc-0.0.4/autooc.egg-info/
--rw-r--r--   0 luis      (1000) luis      (1000)    12343 2023-06-24 15:01:50.000000 autooc-0.0.4/autooc.egg-info/PKG-INFO
--rw-r--r--   0 luis      (1000) luis      (1000)     3283 2023-06-24 15:01:50.000000 autooc-0.0.4/autooc.egg-info/SOURCES.txt
--rw-r--r--   0 luis      (1000) luis      (1000)        1 2023-06-24 15:01:50.000000 autooc-0.0.4/autooc.egg-info/dependency_links.txt
--rw-r--r--   0 luis      (1000) luis      (1000)      164 2023-06-24 15:01:50.000000 autooc-0.0.4/autooc.egg-info/requires.txt
--rw-r--r--   0 luis      (1000) luis      (1000)        7 2023-06-24 15:01:50.000000 autooc-0.0.4/autooc.egg-info/top_level.txt
--rw-r--r--   0 luis      (1000) luis      (1000)      103 2023-06-24 15:01:50.168871 autooc-0.0.4/setup.cfg
--rw-r--r--   0 luis      (1000) luis      (1000)     1375 2023-06-24 15:01:48.000000 autooc-0.0.4/setup.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.428872 autooc-0.0.5/
+-rw-r--r--   0 luis      (1000) luis      (1000)     1071 2023-06-24 14:17:33.000000 autooc-0.0.5/LICENSE
+-rw-r--r--   0 luis      (1000) luis      (1000)       42 2023-06-24 14:17:33.000000 autooc-0.0.5/MANIFEST.in
+-rw-r--r--   0 luis      (1000) luis      (1000)    12343 2023-06-24 15:03:15.428872 autooc-0.0.5/PKG-INFO
+-rw-r--r--   0 luis      (1000) luis      (1000)    11738 2023-06-24 14:29:17.000000 autooc-0.0.5/README.md
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.408872 autooc-0.0.5/autooc/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.408872 autooc-0.0.5/autooc/algorithm/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/algorithm/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.408872 autooc-0.0.5/autooc/algorithm/distributed_algorithm/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/algorithm/distributed_algorithm/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      994 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/algorithm/distributed_algorithm/search_loop.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      426 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/algorithm/distributed_algorithm/step.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     9888 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/algorithm/hill_climbing.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    11897 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/algorithm/mapper.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    13826 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/algorithm/parameters.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2460 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/algorithm/search_loop.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1643 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/algorithm/step.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    25074 2023-06-24 14:30:26.000000 autooc-0.0.5/autooc/autooc.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.408872 autooc-0.0.5/autooc/fitness/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.408872 autooc-0.0.5/autooc/fitness/base_ff_classes/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/base_ff_classes/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2130 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/base_ff_classes/base_ff.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2587 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/base_ff_classes/ff_template.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2662 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/base_ff_classes/moo_ff.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      484 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/bic.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     5108 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/evaluation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      362 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/minimise_nodes.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.418872 autooc-0.0.5/autooc/fitness/multi_objective/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/multi_objective/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      796 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/multi_objective/binary_phenotype_to_float.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3944 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/multi_objective/singlefit_autoencoders.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1845 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/multi_objective/singlefit_multiobj.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1007 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/multi_objective/zdt1.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      407 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/num_params.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      403 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/predict_time.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6022 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/progsys.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1337 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/pymax.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     5886 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/sequence_match.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1038 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/string_match.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.418872 autooc-0.0.5/autooc/fitness/supervised_learning/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/supervised_learning/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3731 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/supervised_learning/boolean_problem.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      659 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/supervised_learning/classification.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2912 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/supervised_learning/if_else_classifier.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      643 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/supervised_learning/regression.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4478 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/supervised_learning/regression_random_polynomial.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    10335 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/supervised_learning/supervised_learning.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3627 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/supervised_learning/supervised_learning_backup.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      406 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/fitness/training_time.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.418872 autooc-0.0.5/autooc/operators/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/operators/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    16352 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/operators/crossover.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    16207 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/operators/initialisation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     8189 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/operators/mutation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     5351 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/operators/replacement.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4486 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/operators/selection.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    28915 2023-06-24 14:17:34.000000 autooc-0.0.5/autooc/operators/subtree_parse.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.418872 autooc-0.0.5/autooc/representation/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/representation/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    14379 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/representation/derivation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    28989 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/representation/grammar.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6994 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/representation/individual.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6384 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/representation/latent_tree.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     8567 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/representation/tree.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.418872 autooc-0.0.5/autooc/scripts/
+-rw-r--r--   0 luis      (1000) luis      (1000)    13836 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/scripts/GE_LR_parser.py
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/scripts/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3387 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/scripts/baselines.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2532 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/scripts/experiment_manager.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2642 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/scripts/grammar_analyser.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4583 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/scripts/python_script_evaluation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    10267 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/scripts/stats_parser.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.418872 autooc-0.0.5/autooc/stats/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/stats/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    13101 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/stats/stats.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.418872 autooc-0.0.5/autooc/utilities/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.418872 autooc-0.0.5/autooc/utilities/algorithm/
+-rw-r--r--   0 luis      (1000) luis      (1000)    12775 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/algorithm/NSGA2.py
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/algorithm/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    23627 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/algorithm/command_line_parser.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      418 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/algorithm/general.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    11564 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/algorithm/initialise_run.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4433 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/algorithm/state.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.428872 autooc-0.0.5/autooc/utilities/fitness/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/fitness/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     8348 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/fitness/error_metric.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3663 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/fitness/get_data.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6753 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/fitness/math_functions.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2993 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/fitness/optimize_constants.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.428872 autooc-0.0.5/autooc/utilities/representation/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/representation/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    13533 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/representation/check_methods.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      720 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/representation/python_filter.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.428872 autooc-0.0.5/autooc/utilities/stats/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/stats/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      498 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/stats/clean_stats.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6086 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/stats/file_io.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4512 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/stats/save_plots.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1015 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/stats/trackers.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1966 2023-06-24 14:17:35.000000 autooc-0.0.5/autooc/utilities/utils.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:03:15.408872 autooc-0.0.5/autooc.egg-info/
+-rw-r--r--   0 luis      (1000) luis      (1000)    12343 2023-06-24 15:03:15.000000 autooc-0.0.5/autooc.egg-info/PKG-INFO
+-rw-r--r--   0 luis      (1000) luis      (1000)     3283 2023-06-24 15:03:15.000000 autooc-0.0.5/autooc.egg-info/SOURCES.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)        1 2023-06-24 15:03:15.000000 autooc-0.0.5/autooc.egg-info/dependency_links.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)      164 2023-06-24 15:03:15.000000 autooc-0.0.5/autooc.egg-info/requires.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)        7 2023-06-24 15:03:15.000000 autooc-0.0.5/autooc.egg-info/top_level.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)      103 2023-06-24 15:03:15.428872 autooc-0.0.5/setup.cfg
+-rw-r--r--   0 luis      (1000) luis      (1000)     1375 2023-06-24 15:03:14.000000 autooc-0.0.5/setup.py
```

### Comparing `autooc-0.0.4/LICENSE` & `autooc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/PKG-INFO` & `autooc-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autooc
-Version: 0.0.4
+Version: 0.0.5
 Summary: AutoOC: Automated Machine Learning (AutoML) library for One-Class Learning
 Home-page: https://github.com/luisferreira97/AutoOC
 Author: Luís Ferreira
 Author-email: luis_ferreira223@hotmail.com
 Keywords: automl,machine learning,one-class learning,one-class classification,autoencoder,isolation forest,one-class svm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autooc Version: 0.0.4 Summary: AutoOC: Automated
+Metadata-Version: 2.1 Name: autooc Version: 0.0.5 Summary: AutoOC: Automated
 Machine Learning (AutoML) library for One-Class Learning Home-page: https://
 github.com/luisferreira97/AutoOC Author: LuÃ­s Ferreira Author-email:
 luis_ferreira223@hotmail.com Keywords: automl,machine learning,one-class
 learning,one-class classification,autoencoder,isolation forest,one-class svm
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
```

### Comparing `autooc-0.0.4/README.md` & `autooc-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/algorithm/distributed_algorithm/search_loop.py` & `autooc-0.0.5/autooc/algorithm/distributed_algorithm/search_loop.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/algorithm/hill_climbing.py` & `autooc-0.0.5/autooc/algorithm/hill_climbing.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/algorithm/mapper.py` & `autooc-0.0.5/autooc/algorithm/mapper.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/algorithm/parameters.py` & `autooc-0.0.5/autooc/algorithm/parameters.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/algorithm/search_loop.py` & `autooc-0.0.5/autooc/algorithm/search_loop.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/algorithm/step.py` & `autooc-0.0.5/autooc/algorithm/step.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/autooc.py` & `autooc-0.0.5/autooc/autooc.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/base_ff_classes/base_ff.py` & `autooc-0.0.5/autooc/fitness/base_ff_classes/base_ff.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/base_ff_classes/ff_template.py` & `autooc-0.0.5/autooc/fitness/base_ff_classes/ff_template.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/base_ff_classes/moo_ff.py` & `autooc-0.0.5/autooc/fitness/base_ff_classes/moo_ff.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/evaluation.py` & `autooc-0.0.5/autooc/fitness/evaluation.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/multi_objective/binary_phenotype_to_float.py` & `autooc-0.0.5/autooc/fitness/multi_objective/binary_phenotype_to_float.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/multi_objective/singlefit_autoencoders.py` & `autooc-0.0.5/autooc/fitness/multi_objective/singlefit_autoencoders.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/multi_objective/singlefit_multiobj.py` & `autooc-0.0.5/autooc/fitness/multi_objective/singlefit_multiobj.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/multi_objective/zdt1.py` & `autooc-0.0.5/autooc/fitness/multi_objective/zdt1.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/progsys.py` & `autooc-0.0.5/autooc/fitness/progsys.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/pymax.py` & `autooc-0.0.5/autooc/fitness/pymax.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/sequence_match.py` & `autooc-0.0.5/autooc/fitness/sequence_match.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/string_match.py` & `autooc-0.0.5/autooc/fitness/string_match.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/supervised_learning/boolean_problem.py` & `autooc-0.0.5/autooc/fitness/supervised_learning/boolean_problem.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/supervised_learning/classification.py` & `autooc-0.0.5/autooc/fitness/supervised_learning/classification.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/supervised_learning/if_else_classifier.py` & `autooc-0.0.5/autooc/fitness/supervised_learning/if_else_classifier.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/supervised_learning/regression.py` & `autooc-0.0.5/autooc/fitness/supervised_learning/regression.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/supervised_learning/regression_random_polynomial.py` & `autooc-0.0.5/autooc/fitness/supervised_learning/regression_random_polynomial.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/supervised_learning/supervised_learning.py` & `autooc-0.0.5/autooc/fitness/supervised_learning/supervised_learning.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/fitness/supervised_learning/supervised_learning_backup.py` & `autooc-0.0.5/autooc/fitness/supervised_learning/supervised_learning_backup.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/operators/crossover.py` & `autooc-0.0.5/autooc/operators/crossover.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/operators/initialisation.py` & `autooc-0.0.5/autooc/operators/initialisation.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/operators/mutation.py` & `autooc-0.0.5/autooc/operators/mutation.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/operators/replacement.py` & `autooc-0.0.5/autooc/operators/replacement.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/operators/selection.py` & `autooc-0.0.5/autooc/operators/selection.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/operators/subtree_parse.py` & `autooc-0.0.5/autooc/operators/subtree_parse.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/representation/derivation.py` & `autooc-0.0.5/autooc/representation/derivation.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/representation/grammar.py` & `autooc-0.0.5/autooc/representation/grammar.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/representation/individual.py` & `autooc-0.0.5/autooc/representation/individual.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/representation/latent_tree.py` & `autooc-0.0.5/autooc/representation/latent_tree.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/representation/tree.py` & `autooc-0.0.5/autooc/representation/tree.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/scripts/GE_LR_parser.py` & `autooc-0.0.5/autooc/scripts/GE_LR_parser.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/scripts/baselines.py` & `autooc-0.0.5/autooc/scripts/baselines.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/scripts/experiment_manager.py` & `autooc-0.0.5/autooc/scripts/experiment_manager.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/scripts/grammar_analyser.py` & `autooc-0.0.5/autooc/scripts/grammar_analyser.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/scripts/python_script_evaluation.py` & `autooc-0.0.5/autooc/scripts/python_script_evaluation.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/scripts/stats_parser.py` & `autooc-0.0.5/autooc/scripts/stats_parser.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/stats/stats.py` & `autooc-0.0.5/autooc/stats/stats.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/algorithm/NSGA2.py` & `autooc-0.0.5/autooc/utilities/algorithm/NSGA2.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/algorithm/command_line_parser.py` & `autooc-0.0.5/autooc/utilities/algorithm/command_line_parser.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/algorithm/initialise_run.py` & `autooc-0.0.5/autooc/utilities/algorithm/initialise_run.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/algorithm/state.py` & `autooc-0.0.5/autooc/utilities/algorithm/state.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/fitness/error_metric.py` & `autooc-0.0.5/autooc/utilities/fitness/error_metric.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/fitness/get_data.py` & `autooc-0.0.5/autooc/utilities/fitness/get_data.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/fitness/math_functions.py` & `autooc-0.0.5/autooc/utilities/fitness/math_functions.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/fitness/optimize_constants.py` & `autooc-0.0.5/autooc/utilities/fitness/optimize_constants.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/representation/check_methods.py` & `autooc-0.0.5/autooc/utilities/representation/check_methods.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/representation/python_filter.py` & `autooc-0.0.5/autooc/utilities/representation/python_filter.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/stats/file_io.py` & `autooc-0.0.5/autooc/utilities/stats/file_io.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/stats/save_plots.py` & `autooc-0.0.5/autooc/utilities/stats/save_plots.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/stats/trackers.py` & `autooc-0.0.5/autooc/utilities/stats/trackers.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc/utilities/utils.py` & `autooc-0.0.5/autooc/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/autooc.egg-info/PKG-INFO` & `autooc-0.0.5/autooc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autooc
-Version: 0.0.4
+Version: 0.0.5
 Summary: AutoOC: Automated Machine Learning (AutoML) library for One-Class Learning
 Home-page: https://github.com/luisferreira97/AutoOC
 Author: Luís Ferreira
 Author-email: luis_ferreira223@hotmail.com
 Keywords: automl,machine learning,one-class learning,one-class classification,autoencoder,isolation forest,one-class svm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autooc Version: 0.0.4 Summary: AutoOC: Automated
+Metadata-Version: 2.1 Name: autooc Version: 0.0.5 Summary: AutoOC: Automated
 Machine Learning (AutoML) library for One-Class Learning Home-page: https://
 github.com/luisferreira97/AutoOC Author: LuÃ­s Ferreira Author-email:
 luis_ferreira223@hotmail.com Keywords: automl,machine learning,one-class
 learning,one-class classification,autoencoder,isolation forest,one-class svm
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
```

### Comparing `autooc-0.0.4/autooc.egg-info/SOURCES.txt` & `autooc-0.0.5/autooc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autooc-0.0.4/setup.py` & `autooc-0.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="autooc",
-    version="0.0.4",
+    version="0.0.5",
     author_email="luis_ferreira223@hotmail.com",
     author="Luís Ferreira",
     description="AutoOC: Automated Machine Learning (AutoML) library for One-Class Learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/luisferreira97/AutoOC",
@@ -31,14 +31,14 @@
     #package_dir={"": "src/talos"},
     install_requires=[
         'keras==2.6.0',
         'matplotlib==3.4.1',
         'mlflow==1.15.0',
         'pandas==1.2.4',
         'pydot==1.4.2',
-        'pygmo==2.19.0',
+        'pygmo==2.19.5',
         'scikit-learn==1.0',
         'tensorflow==2.6.0',
         'tensorflow-estimator==2.6.0',
         'tqdm==4.60.0'
     ]
 )
```

