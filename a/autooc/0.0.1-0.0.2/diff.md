# Comparing `tmp/autooc-0.0.1.tar.gz` & `tmp/autooc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autooc-0.0.1.tar", last modified: Sat Jun 24 14:23:33 2023, max compression
+gzip compressed data, was "autooc-0.0.2.tar", last modified: Sat Jun 24 14:58:15 2023, max compression
```

## Comparing `autooc-0.0.1.tar` & `autooc-0.0.2.tar`

### file list

```diff
@@ -1,122 +1,111 @@
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.218855 autooc-0.0.1/
--rw-r--r--   0 luis      (1000) luis      (1000)     1071 2023-06-24 14:17:33.000000 autooc-0.0.1/LICENSE
--rw-r--r--   0 luis      (1000) luis      (1000)       42 2023-06-24 14:17:33.000000 autooc-0.0.1/MANIFEST.in
--rw-r--r--   0 luis      (1000) luis      (1000)    12388 2023-06-24 14:23:33.218855 autooc-0.0.1/PKG-INFO
--rw-r--r--   0 luis      (1000) luis      (1000)    11783 2023-06-24 14:20:56.000000 autooc-0.0.1/README.md
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.198855 autooc-0.0.1/autooc.egg-info/
--rw-r--r--   0 luis      (1000) luis      (1000)    12388 2023-06-24 14:23:33.000000 autooc-0.0.1/autooc.egg-info/PKG-INFO
--rw-r--r--   0 luis      (1000) luis      (1000)     3507 2023-06-24 14:23:33.000000 autooc-0.0.1/autooc.egg-info/SOURCES.txt
--rw-r--r--   0 luis      (1000) luis      (1000)        1 2023-06-24 14:23:33.000000 autooc-0.0.1/autooc.egg-info/dependency_links.txt
--rw-r--r--   0 luis      (1000) luis      (1000)      156 2023-06-24 14:23:33.000000 autooc-0.0.1/autooc.egg-info/requires.txt
--rw-r--r--   0 luis      (1000) luis      (1000)       13 2023-06-24 14:23:33.000000 autooc-0.0.1/autooc.egg-info/top_level.txt
--rw-r--r--   0 luis      (1000) luis      (1000)      103 2023-06-24 14:23:33.218855 autooc-0.0.1/setup.cfg
--rw-r--r--   0 luis      (1000) luis      (1000)     1357 2023-06-24 14:21:40.000000 autooc-0.0.1/setup.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.198855 autooc-0.0.1/talos/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.198855 autooc-0.0.1/talos/algorithm/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/algorithm/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.198855 autooc-0.0.1/talos/algorithm/distributed_algorithm/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/algorithm/distributed_algorithm/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)      994 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/algorithm/distributed_algorithm/search_loop.py
--rw-r--r--   0 luis      (1000) luis      (1000)      426 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/algorithm/distributed_algorithm/step.py
--rw-r--r--   0 luis      (1000) luis      (1000)     9888 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/algorithm/hill_climbing.py
--rw-r--r--   0 luis      (1000) luis      (1000)    11897 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/algorithm/mapper.py
--rw-r--r--   0 luis      (1000) luis      (1000)    13826 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/algorithm/parameters.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2460 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/algorithm/search_loop.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1643 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/algorithm/step.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.198855 autooc-0.0.1/talos/fitness/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.208855 autooc-0.0.1/talos/fitness/base_ff_classes/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/base_ff_classes/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2130 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/base_ff_classes/base_ff.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2587 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/base_ff_classes/ff_template.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2662 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/base_ff_classes/moo_ff.py
--rw-r--r--   0 luis      (1000) luis      (1000)      484 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/bic.py
--rw-r--r--   0 luis      (1000) luis      (1000)     5108 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/evaluation.py
--rw-r--r--   0 luis      (1000) luis      (1000)      362 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/minimise_nodes.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.208855 autooc-0.0.1/talos/fitness/multi_objective/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/multi_objective/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)      796 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/multi_objective/binary_phenotype_to_float.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3944 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/multi_objective/singlefit_autoencoders.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1845 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/multi_objective/singlefit_multiobj.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1007 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/multi_objective/zdt1.py
--rw-r--r--   0 luis      (1000) luis      (1000)      407 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/num_params.py
--rw-r--r--   0 luis      (1000) luis      (1000)      403 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/predict_time.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6022 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/progsys.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1337 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/pymax.py
--rw-r--r--   0 luis      (1000) luis      (1000)     5886 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/sequence_match.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1038 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/string_match.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.208855 autooc-0.0.1/talos/fitness/supervised_learning/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/supervised_learning/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3731 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/supervised_learning/boolean_problem.py
--rw-r--r--   0 luis      (1000) luis      (1000)      659 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/supervised_learning/classification.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2912 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/supervised_learning/if_else_classifier.py
--rw-r--r--   0 luis      (1000) luis      (1000)      643 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/supervised_learning/regression.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4478 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/supervised_learning/regression_random_polynomial.py
--rw-r--r--   0 luis      (1000) luis      (1000)    10335 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/supervised_learning/supervised_learning.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3627 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/supervised_learning/supervised_learning_backup.py
--rw-r--r--   0 luis      (1000) luis      (1000)      406 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/fitness/training_time.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.208855 autooc-0.0.1/talos/grammars/
--rw-r--r--   0 luis      (1000) luis      (1000)      538 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/grammars/autoencoders.bnf
--rw-r--r--   0 luis      (1000) luis      (1000)      823 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/grammars/autoencoders.pybnf
--rw-r--r--   0 luis      (1000) luis      (1000)     1159 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/grammars/autoencoders_v2.pybnf
--rw-r--r--   0 luis      (1000) luis      (1000)     1148 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/grammars/autoencoders_v3.pybnf
--rw-r--r--   0 luis      (1000) luis      (1000)      962 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/grammars/autoencoders_v4.pybnf
--rw-r--r--   0 luis      (1000) luis      (1000)      465 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/grammars/iforest.pybnf
--rw-r--r--   0 luis      (1000) luis      (1000)      720 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/grammars/lof.pybnf
--rw-r--r--   0 luis      (1000) luis      (1000)     2088 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/grammars/multi_algo.pybnf
--rw-r--r--   0 luis      (1000) luis      (1000)      303 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/grammars/svm.pybnf
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.208855 autooc-0.0.1/talos/operators/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/operators/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    16352 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/operators/crossover.py
--rw-r--r--   0 luis      (1000) luis      (1000)    16207 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/operators/initialisation.py
--rw-r--r--   0 luis      (1000) luis      (1000)     8189 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/operators/mutation.py
--rw-r--r--   0 luis      (1000) luis      (1000)     5351 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/operators/replacement.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4486 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/operators/selection.py
--rw-r--r--   0 luis      (1000) luis      (1000)    28915 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/operators/subtree_parse.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.208855 autooc-0.0.1/talos/representation/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/representation/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    14379 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/representation/derivation.py
--rw-r--r--   0 luis      (1000) luis      (1000)    28989 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/representation/grammar.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6994 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/representation/individual.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6384 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/representation/latent_tree.py
--rw-r--r--   0 luis      (1000) luis      (1000)     8567 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/representation/tree.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.208855 autooc-0.0.1/talos/scripts/
--rw-r--r--   0 luis      (1000) luis      (1000)    13836 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/scripts/GE_LR_parser.py
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/scripts/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3387 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/scripts/baselines.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2532 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/scripts/experiment_manager.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2642 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/scripts/grammar_analyser.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4583 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/scripts/python_script_evaluation.py
--rw-r--r--   0 luis      (1000) luis      (1000)    10267 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/scripts/stats_parser.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.218855 autooc-0.0.1/talos/stats/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/stats/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    13101 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/stats/stats.py
--rw-r--r--   0 luis      (1000) luis      (1000)    25073 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/talos.py
--rw-r--r--   0 luis      (1000) luis      (1000)     5245 2023-06-24 14:17:34.000000 autooc-0.0.1/talos/talos_run.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.218855 autooc-0.0.1/talos/utilities/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.218855 autooc-0.0.1/talos/utilities/algorithm/
--rw-r--r--   0 luis      (1000) luis      (1000)    12775 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/algorithm/NSGA2.py
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/algorithm/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    23627 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/algorithm/command_line_parser.py
--rw-r--r--   0 luis      (1000) luis      (1000)      418 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/algorithm/general.py
--rw-r--r--   0 luis      (1000) luis      (1000)    11564 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/algorithm/initialise_run.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4433 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/algorithm/state.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.218855 autooc-0.0.1/talos/utilities/fitness/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/fitness/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     8348 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/fitness/error_metric.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3663 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/fitness/get_data.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6753 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/fitness/math_functions.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2993 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/fitness/optimize_constants.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.218855 autooc-0.0.1/talos/utilities/representation/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/representation/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    13533 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/representation/check_methods.py
--rw-r--r--   0 luis      (1000) luis      (1000)      720 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/representation/python_filter.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:23:33.218855 autooc-0.0.1/talos/utilities/stats/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/stats/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)      498 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/stats/clean_stats.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6086 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/stats/file_io.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4512 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/stats/save_plots.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1015 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/stats/trackers.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1966 2023-06-24 14:17:35.000000 autooc-0.0.1/talos/utilities/utils.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.688870 autooc-0.0.2/
+-rw-r--r--   0 luis      (1000) luis      (1000)     1071 2023-06-24 14:17:33.000000 autooc-0.0.2/LICENSE
+-rw-r--r--   0 luis      (1000) luis      (1000)       42 2023-06-24 14:17:33.000000 autooc-0.0.2/MANIFEST.in
+-rw-r--r--   0 luis      (1000) luis      (1000)    12343 2023-06-24 14:58:15.688870 autooc-0.0.2/PKG-INFO
+-rw-r--r--   0 luis      (1000) luis      (1000)    11738 2023-06-24 14:29:17.000000 autooc-0.0.2/README.md
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.668870 autooc-0.0.2/autooc/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.678870 autooc-0.0.2/autooc/algorithm/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/algorithm/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.678870 autooc-0.0.2/autooc/algorithm/distributed_algorithm/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/algorithm/distributed_algorithm/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      994 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/algorithm/distributed_algorithm/search_loop.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      426 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/algorithm/distributed_algorithm/step.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     9888 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/algorithm/hill_climbing.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    11897 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/algorithm/mapper.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    13826 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/algorithm/parameters.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2460 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/algorithm/search_loop.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1643 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/algorithm/step.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    25074 2023-06-24 14:30:26.000000 autooc-0.0.2/autooc/autooc.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.678870 autooc-0.0.2/autooc/fitness/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.678870 autooc-0.0.2/autooc/fitness/base_ff_classes/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/base_ff_classes/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2130 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/base_ff_classes/base_ff.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2587 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/base_ff_classes/ff_template.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2662 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/base_ff_classes/moo_ff.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      484 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/bic.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     5108 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/evaluation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      362 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/minimise_nodes.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.678870 autooc-0.0.2/autooc/fitness/multi_objective/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/multi_objective/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      796 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/multi_objective/binary_phenotype_to_float.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3944 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/multi_objective/singlefit_autoencoders.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1845 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/multi_objective/singlefit_multiobj.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1007 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/multi_objective/zdt1.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      407 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/num_params.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      403 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/predict_time.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6022 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/progsys.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1337 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/pymax.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     5886 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/sequence_match.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1038 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/string_match.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.678870 autooc-0.0.2/autooc/fitness/supervised_learning/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/supervised_learning/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3731 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/supervised_learning/boolean_problem.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      659 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/supervised_learning/classification.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2912 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/supervised_learning/if_else_classifier.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      643 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/supervised_learning/regression.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4478 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/supervised_learning/regression_random_polynomial.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    10335 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/supervised_learning/supervised_learning.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3627 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/supervised_learning/supervised_learning_backup.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      406 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/fitness/training_time.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.678870 autooc-0.0.2/autooc/operators/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/operators/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    16352 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/operators/crossover.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    16207 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/operators/initialisation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     8189 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/operators/mutation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     5351 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/operators/replacement.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4486 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/operators/selection.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    28915 2023-06-24 14:17:34.000000 autooc-0.0.2/autooc/operators/subtree_parse.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.688870 autooc-0.0.2/autooc/representation/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/representation/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    14379 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/representation/derivation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    28989 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/representation/grammar.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6994 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/representation/individual.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6384 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/representation/latent_tree.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     8567 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/representation/tree.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.688870 autooc-0.0.2/autooc/scripts/
+-rw-r--r--   0 luis      (1000) luis      (1000)    13836 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/scripts/GE_LR_parser.py
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/scripts/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3387 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/scripts/baselines.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2532 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/scripts/experiment_manager.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2642 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/scripts/grammar_analyser.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4583 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/scripts/python_script_evaluation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    10267 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/scripts/stats_parser.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.688870 autooc-0.0.2/autooc/stats/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/stats/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    13101 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/stats/stats.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.688870 autooc-0.0.2/autooc/utilities/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.688870 autooc-0.0.2/autooc/utilities/algorithm/
+-rw-r--r--   0 luis      (1000) luis      (1000)    12775 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/algorithm/NSGA2.py
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/algorithm/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    23627 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/algorithm/command_line_parser.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      418 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/algorithm/general.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    11564 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/algorithm/initialise_run.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4433 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/algorithm/state.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.688870 autooc-0.0.2/autooc/utilities/fitness/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/fitness/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     8348 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/fitness/error_metric.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3663 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/fitness/get_data.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6753 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/fitness/math_functions.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2993 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/fitness/optimize_constants.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.688870 autooc-0.0.2/autooc/utilities/representation/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/representation/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    13533 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/representation/check_methods.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      720 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/representation/python_filter.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.688870 autooc-0.0.2/autooc/utilities/stats/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/stats/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      498 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/stats/clean_stats.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6086 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/stats/file_io.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4512 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/stats/save_plots.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1015 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/stats/trackers.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1966 2023-06-24 14:17:35.000000 autooc-0.0.2/autooc/utilities/utils.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 14:58:15.678870 autooc-0.0.2/autooc.egg-info/
+-rw-r--r--   0 luis      (1000) luis      (1000)    12343 2023-06-24 14:58:15.000000 autooc-0.0.2/autooc.egg-info/PKG-INFO
+-rw-r--r--   0 luis      (1000) luis      (1000)     3283 2023-06-24 14:58:15.000000 autooc-0.0.2/autooc.egg-info/SOURCES.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)        1 2023-06-24 14:58:15.000000 autooc-0.0.2/autooc.egg-info/dependency_links.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)      137 2023-06-24 14:58:15.000000 autooc-0.0.2/autooc.egg-info/requires.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)        7 2023-06-24 14:58:15.000000 autooc-0.0.2/autooc.egg-info/top_level.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)      103 2023-06-24 14:58:15.688870 autooc-0.0.2/setup.cfg
+-rw-r--r--   0 luis      (1000) luis      (1000)     1327 2023-06-24 14:54:13.000000 autooc-0.0.2/setup.py
```

### Comparing `autooc-0.0.1/LICENSE` & `autooc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/PKG-INFO` & `autooc-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,46 @@
-Metadata-Version: 2.1
-Name: autooc
-Version: 0.0.1
-Summary: AutoOC: Automated Machine Learning (AutoML) library for One-Class Learning
-Home-page: https://github.com/luisferreira97/AutoOC
-Author: Luís Ferreira
-Author-email: luis_ferreira223@hotmail.com
-Keywords: automl,machine learning,one-class learning,one-class classification,autoencoder,isolation forest,one-class svm
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- PROJECT SHIELDS -->
 <!--
 *** I'm using markdown "reference style" links for readability.
 *** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
 *** See the bottom of this document for the declaration of the reference variables
 *** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
-<!--[![Downloads](https://static.pepy.tech/personalized-badge/talos-automl?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/talos-automl)-->
+<!--[![Downloads](https://static.pepy.tech/personalized-badge/autooc?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/autooc)-->
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
-  <!--<a href="https://github.com/luisferreira97/talos">
+  <!--<a href="https://github.com/luisferreira97/AutoOC">
     <img src="images/logo.png" alt="Logo" width="80" height="115">
   </a>-->
 
   <h3 align="center">AutoOC (in Beta)</h3>
 
   <p align="center">
     AutoOC: Automated Machine Learning (AutoML) library focused on One-Class Learning algorithms (AutoEncoders, Isolation Forest and One-Class SVM)
     <br />
-    <a href="https://github.com/luisferreira97/talos"><strong>Explore the docs »</strong></a>
+    <a href="https://github.com/luisferreira97/AutoOC"><strong>Explore the docs »</strong></a>
     <br />
     <br />
-    <a href="https://github.com/luisferreira97/talos">View Demo</a>
+    <a href="https://github.com/luisferreira97/AutoOC">View Demo</a>
     ·
-    <a href="https://github.com/luisferreira97/talos/issues">Report Bug</a>
+    <a href="https://github.com/luisferreira97/AutoOC/issues">Report Bug</a>
     ·
-    <a href="https://github.com/luisferreira97/talos/issues">Request Feature</a>
+    <a href="https://github.com/luisferreira97/AutoOC/issues">Request Feature</a>
   </p>
 </p>
 
 
 
 <!-- TABLE OF CONTENTS -->
 <details open="open">
@@ -114,63 +99,62 @@
 <!-- GETTING STARTED -->
 ## Getting Started
 
 This section presents how the package can be reached and installed.
 
 ### Where to get it
 
-The source code is currently hosted on GitHub at: https://github.com/luisferreira97/talos
+The source code is currently hosted on GitHub at: https://github.com/luisferreira97/AutoOC
 
-Binary installer for the latest released version are available at the Python Package Index (PyPI).
-Note that the PyPI name of the package is `talos-automl` and not `talos`.
+Binary installer for the latest released version are available at the Python Package Index (PyPI). The PyPI name of the package is `autooc`.
 
 ```sh
-pip install talos-automl
+pip install autooc
 ```
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 ### 1. Import the package
-The first step in using the package is, after it has been installed, to import it. The main class from which all the methods are available is ```Talos```.
+The first step in using the package is, after it has been installed, to import it. The main class from which all the methods are available is ```AutoOC```.
 
 ```python
-from talos.talos import Talos
+from autooc.autooc import AutoOC
 ```
 
-### 2. Instantiate a Talos object
-The second step is to instantiate the Talos class with the information about your dataset and context (e.g., normal and anomaly classes, wether to run single-objective or multi-objective, the performance_metric, and the algorithm).
+### 2. Instantiate a AutoOC object
+The second step is to instantiate the AutoOC class with the information about your dataset and context (e.g., normal and anomaly classes, wether to run single-objective or multi-objective, the performance_metric, and the algorithm).
 You can change the ```algorithm``` parameter to select which algorithms are used during the optimization. The options are:
 - "autoencoders": Deep AutoEncoders (from TensorFlow)
 - "iforest": Isolation Forest (from Scikit-Learn)
 - "svm": One-Class SVM (from Scikit-Learn)
 - "all": the optimization is done using the three algorithms above
 
 ```python
-talos = Talos(anomaly_class = 0,
+aoc = AutoOC(anomaly_class = 0,
     normal_class = 1,
     multiobjective=True,
     performance_metric="training_time",
     algorithm = "autoencoder"
 )
 ```
 
 ### 3. Load dataset
 The third step is to load the dataset. Depending on the type of validation you need *train data* (only 'normal' instances), *validation data* (you can use (1) only 'normal' instances or (2) both 'normal' and 'anomaly' instances with the respective labels), and *test data* (both types of instances and labels). You can use the ```load_example_data()``` function to load the popular ECG dataset.
 
 
 ```python
-X_train, X_val, X_test, y_test = talos.load_example_data()
+X_train, X_val, X_test, y_test = aoc.load_example_data()
 ```
 
 ### 4. Train
 The fourth step is to train the model. The ```fit()``` function computes the optimization using the given parameters.
 
 ```python
-run = talos.fit(
+run = aoc.fit(
     X=X_train,
     X_val=X_val,
     pop=10,
     gen=10,
     experiment_name="test",
     epochs=1000
 )
@@ -189,59 +173,59 @@
 - "mean": For each model the threshold value is the sum of the mean reconstruction error obtained on the validation data and one standard deviation.
 - "percentile": For each model the threshold value is the 95th percentile of the reconstruction error obtained on the validation data (you can also use the ```percentile``` parameter to change the percentile).
 - "max": For each model the threshold value is maximum reconstruction error obtained on the validation data.
 - You can also pass an Integer of Float value. In this case, the threshold value is the same for all the models.
 
 
 ```python
-predictions = talos.predict(X_test,
+predictions = aoc.predict(X_test,
     mode="all",
     threshold="default")
 ```
 
 ### 6. Evaluate
 
 You can use the predictions to calculate manually the performance metrics of the model. However, the ```evaluate()``` function is a more convenient way to do it. You can also use the ```mode``` parameter (works similarly to the ```predict()``` function) and use metrics from the ```sklearn.metrics``` package (currently available are "roc_auc", "accuracy", "precision", "recall", and "f1").
 
 ```python
-score = talos.evaluate(X_test,
+score = aoc.evaluate(X_test,
     y_test,
     mode="all",
     metric="roc_auc",
     threshold="default")
 ```
 
 ## Usage
 
 ```python
-from talos.talos import Talos
+from autooc.autooc import AutoOC
 
-talos = Talos(anomaly_class = 0,
+aoc = AutoOC(anomaly_class = 0,
     normal_class = 1,
     multiobjective=True,
     performance_metric="training_time",
     algorithm = "autoencoder"
 )
 
-X_train, X_val, X_test, y_test = talos.load_example_data()
+X_train, X_val, X_test, y_test = aoc.load_example_data()
 
-run = talos.fit(
+run = aoc.fit(
     X=X_train,
     X_val=X_val,
     pop=10,
     gen=10,
     experiment_name="test",
     epochs=1000
 )
 
-predictions = talos.predict(X_test,
+predictions = aoc.predict(X_test,
     mode="all",
     threshold="default")
 
-score = talos.evaluate(X_test,
+score = aoc.evaluate(X_test,
     y_test,
     mode="all",
     metric="roc_auc",
     threshold="default")
 ```
 
 _For more examples, please refer to the [Documentation](https://example.com)_-->
@@ -264,15 +248,15 @@
   url = {https://www.sciencedirect.com/science/article/pii/S1568494622008699}
 }
 ```
 
 <!-- ROADMAP -->
 ## Roadmap
 
-See the [open issues](https://github.com/luisferreira97/talos) for a list of proposed features (and known issues).
+See the [open issues](https://github.com/luisferreira97/AutoOC) for a list of proposed features (and known issues).
 
 
 
 <!-- CONTRIBUTING -->
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.
@@ -293,34 +277,34 @@
 
 
 <!-- CONTACT -->
 ## Contact
 
 Luís Ferreira - [LinkedIn](https://www.linkedin.com/in/luisferreira97/) - luis_ferreira223@hotmail.com
 
-Project Link: [https://github.com/luisferreira97/talos](https://github.com/luisferreira97/talos)
+Project Link: [https://github.com/luisferreira97/AutoOC](https://github.com/luisferreira97/AutoOC)
 
 
 
 <!-- ACKNOWLEDGEMENTS -->
 ## Acknowledgements
 * [PonyGE2](https://github.com/PonyGE/PonyGE2)
 
 
 
 
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
-[contributors-url]: https://github.com/luisferreira97/talos/graphs/contributors
+[contributors-url]: https://github.com/luisferreira97/AutoOC/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
-[forks-url]: https://github.com/luisferreira97/talos/network/members
+[forks-url]: https://github.com/luisferreira97/AutoOC/network/members
 [stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
-[stars-url]: https://github.com/luisferreira97/talos/stargazers
+[stars-url]: https://github.com/luisferreira97/AutoOC/stargazers
 [issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
-[issues-url]: https://github.com/luisferreira97/talos/issues
+[issues-url]: https://github.com/luisferreira97/AutoOC/issues
 [license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
-[license-url]: https://github.com/luisferreira97/talos/blob/master/LICENSE
+[license-url]: https://github.com/luisferreira97/AutoOC/blob/master/LICENSE
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 [linkedin-url]: https://www.linkedin.com/in/luisferreira97/
 [product-screenshot]: images/screenshot.png
```

#### html2text {}

```diff
@@ -1,19 +1,11 @@
-Metadata-Version: 2.1 Name: autooc Version: 0.0.1 Summary: AutoOC: Automated
-Machine Learning (AutoML) library for One-Class Learning Home-page: https://
-github.com/luisferreira97/AutoOC Author: LuÃ­s Ferreira Author-email:
-luis_ferreira223@hotmail.com Keywords: automl,machine learning,one-class
-learning,one-class classification,autoencoder,isolation forest,one-class svm
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE    [![Contributors][contributors-shield]][contributors-url] [![Forks]
-[forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues]
-[issues-shield]][issues-url] [![MIT License][license-shield]][license-url] [!
-[LinkedIn][linkedin-shield]][linkedin-url]
+   [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
+shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
+shield]][issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
+[linkedin-shield]][linkedin-url]
                           **** AutoOC (in Beta) ****
    AutoOC: Automated Machine Learning (AutoML) library focused on One-Class
     Learning algorithms (AutoEncoders, Isolation Forest and One-Class SVM)
                              Explore_the_docs_Â»
 
                   View_Demo Â· Report_Bug Â· Request_Feature
   Table of Contents
@@ -44,104 +36,103 @@
 acknowledgements. ### Built With This section should list any major frameworks
 that you built your project using. Leave any add-ons/plugins for the
 acknowledgements section. Here are a few examples. * [Python](https://
 www.python.org) * [PonyGE2](https://github.com/PonyGE/PonyGE2) * [TensorFlow]
 (https://www.tensorflow.org/) * [Scikit-Learn](https://scikit-learn.org/)  ##
 Getting Started This section presents how the package can be reached and
 installed. ### Where to get it The source code is currently hosted on GitHub
-at: https://github.com/luisferreira97/talos Binary installer for the latest
-released version are available at the Python Package Index (PyPI). Note that
-the PyPI name of the package is `talos-automl` and not `talos`. ```sh pip
-install talos-automl ```  ## Usage ### 1. Import the package The first step in
-using the package is, after it has been installed, to import it. The main class
-from which all the methods are available is ```Talos```. ```python from
-talos.talos import Talos ``` ### 2. Instantiate a Talos object The second step
-is to instantiate the Talos class with the information about your dataset and
-context (e.g., normal and anomaly classes, wether to run single-objective or
-multi-objective, the performance_metric, and the algorithm). You can change the
-```algorithm``` parameter to select which algorithms are used during the
-optimization. The options are: - "autoencoders": Deep AutoEncoders (from
-TensorFlow) - "iforest": Isolation Forest (from Scikit-Learn) - "svm": One-
-Class SVM (from Scikit-Learn) - "all": the optimization is done using the three
-algorithms above ```python talos = Talos(anomaly_class = 0, normal_class = 1,
-multiobjective=True, performance_metric="training_time", algorithm =
-"autoencoder" ) ``` ### 3. Load dataset The third step is to load the dataset.
-Depending on the type of validation you need *train data* (only 'normal'
-instances), *validation data* (you can use (1) only 'normal' instances or (2)
-both 'normal' and 'anomaly' instances with the respective labels), and *test
-data* (both types of instances and labels). You can use the
-```load_example_data()``` function to load the popular ECG dataset. ```python
-X_train, X_val, X_test, y_test = talos.load_example_data() ``` ### 4. Train The
-fourth step is to train the model. The ```fit()``` function computes the
-optimization using the given parameters. ```python run = talos.fit( X=X_train,
-X_val=X_val, pop=10, gen=10, experiment_name="test", epochs=1000 ) ``` ### 5.
-Predict The fifth step is to predict the labels of the test data. You can use
-the ```predict()``` function to predict the labels of the test data. You can
-change the ```mode``` parameter to select which individuals are used to
-predict. - "all": uses all individuals (models) from the last generation -
-"best": uses the from the last generation which achieved the best predictive
-metric - "simplest": uses the from the last generation which achieved the best
-efficiency metric - "pareto": uses the pareto individuals from the last
-generation (only for multiobjective. These are the models that achieved
-simultaneouly the best predictive metric and efficiency metric. Additionally,
-you can use the ```threshold``` parameter (only used for AutoEncoders) to set
-the threshold for the prediction. You can use the following values: -
-"default": uses a different threshold value for each individual (model). For
-each model the threshold value is the associated default value (currently this
-works similar to the "mean" value). - "mean": For each model the threshold
-value is the sum of the mean reconstruction error obtained on the validation
-data and one standard deviation. - "percentile": For each model the threshold
-value is the 95th percentile of the reconstruction error obtained on the
-validation data (you can also use the ```percentile``` parameter to change the
-percentile). - "max": For each model the threshold value is maximum
-reconstruction error obtained on the validation data. - You can also pass an
-Integer of Float value. In this case, the threshold value is the same for all
-the models. ```python predictions = talos.predict(X_test, mode="all",
-threshold="default") ``` ### 6. Evaluate You can use the predictions to
-calculate manually the performance metrics of the model. However, the
-```evaluate()``` function is a more convenient way to do it. You can also use
-the ```mode``` parameter (works similarly to the ```predict()``` function) and
-use metrics from the ```sklearn.metrics``` package (currently available are
-"roc_auc", "accuracy", "precision", "recall", and "f1"). ```python score =
-talos.evaluate(X_test, y_test, mode="all", metric="roc_auc",
-threshold="default") ``` ## Usage ```python from talos.talos import Talos talos
-= Talos(anomaly_class = 0, normal_class = 1, multiobjective=True,
+at: https://github.com/luisferreira97/AutoOC Binary installer for the latest
+released version are available at the Python Package Index (PyPI). The PyPI
+name of the package is `autooc`. ```sh pip install autooc ```  ## Usage ### 1.
+Import the package The first step in using the package is, after it has been
+installed, to import it. The main class from which all the methods are
+available is ```AutoOC```. ```python from autooc.autooc import AutoOC ``` ###
+2. Instantiate a AutoOC object The second step is to instantiate the AutoOC
+class with the information about your dataset and context (e.g., normal and
+anomaly classes, wether to run single-objective or multi-objective, the
+performance_metric, and the algorithm). You can change the ```algorithm```
+parameter to select which algorithms are used during the optimization. The
+options are: - "autoencoders": Deep AutoEncoders (from TensorFlow) - "iforest":
+Isolation Forest (from Scikit-Learn) - "svm": One-Class SVM (from Scikit-Learn)
+- "all": the optimization is done using the three algorithms above ```python
+aoc = AutoOC(anomaly_class = 0, normal_class = 1, multiobjective=True,
+performance_metric="training_time", algorithm = "autoencoder" ) ``` ### 3. Load
+dataset The third step is to load the dataset. Depending on the type of
+validation you need *train data* (only 'normal' instances), *validation data*
+(you can use (1) only 'normal' instances or (2) both 'normal' and 'anomaly'
+instances with the respective labels), and *test data* (both types of instances
+and labels). You can use the ```load_example_data()``` function to load the
+popular ECG dataset. ```python X_train, X_val, X_test, y_test =
+aoc.load_example_data() ``` ### 4. Train The fourth step is to train the model.
+The ```fit()``` function computes the optimization using the given parameters.
+```python run = aoc.fit( X=X_train, X_val=X_val, pop=10, gen=10,
+experiment_name="test", epochs=1000 ) ``` ### 5. Predict The fifth step is to
+predict the labels of the test data. You can use the ```predict()``` function
+to predict the labels of the test data. You can change the ```mode``` parameter
+to select which individuals are used to predict. - "all": uses all individuals
+(models) from the last generation - "best": uses the from the last generation
+which achieved the best predictive metric - "simplest": uses the from the last
+generation which achieved the best efficiency metric - "pareto": uses the
+pareto individuals from the last generation (only for multiobjective. These are
+the models that achieved simultaneouly the best predictive metric and
+efficiency metric. Additionally, you can use the ```threshold``` parameter
+(only used for AutoEncoders) to set the threshold for the prediction. You can
+use the following values: - "default": uses a different threshold value for
+each individual (model). For each model the threshold value is the associated
+default value (currently this works similar to the "mean" value). - "mean": For
+each model the threshold value is the sum of the mean reconstruction error
+obtained on the validation data and one standard deviation. - "percentile": For
+each model the threshold value is the 95th percentile of the reconstruction
+error obtained on the validation data (you can also use the ```percentile```
+parameter to change the percentile). - "max": For each model the threshold
+value is maximum reconstruction error obtained on the validation data. - You
+can also pass an Integer of Float value. In this case, the threshold value is
+the same for all the models. ```python predictions = aoc.predict(X_test,
+mode="all", threshold="default") ``` ### 6. Evaluate You can use the
+predictions to calculate manually the performance metrics of the model.
+However, the ```evaluate()``` function is a more convenient way to do it. You
+can also use the ```mode``` parameter (works similarly to the ```predict()```
+function) and use metrics from the ```sklearn.metrics``` package (currently
+available are "roc_auc", "accuracy", "precision", "recall", and "f1").
+```python score = aoc.evaluate(X_test, y_test, mode="all", metric="roc_auc",
+threshold="default") ``` ## Usage ```python from autooc.autooc import AutoOC
+aoc = AutoOC(anomaly_class = 0, normal_class = 1, multiobjective=True,
 performance_metric="training_time", algorithm = "autoencoder" ) X_train, X_val,
-X_test, y_test = talos.load_example_data() run = talos.fit( X=X_train,
-X_val=X_val, pop=10, gen=10, experiment_name="test", epochs=1000 ) predictions
-= talos.predict(X_test, mode="all", threshold="default") score = talos.evaluate
-(X_test, y_test, mode="all", metric="roc_auc", threshold="default") ``` _For
-more examples, please refer to the [Documentation](https://example.com)_-->  ##
-Citation To cite this work please use: ``` @article{FERREIRA2022109820, author
-= {LuÃ­s Ferreira and AndrÃ© Pilastri and Filipe Romano and Paulo Cortez},
-title = {Using supervised and one-class automated machine learning for
-predictive maintenance}, journal = {Applied Soft Computing}, volume = {131},
-pages = {109820}, year = {2022}, issn = {1568-4946}, doi = {https://doi.org/
-10.1016/j.asoc.2022.109820}, url = {https://www.sciencedirect.com/science/
-article/pii/S1568494622008699} } ```  ## Roadmap See the [open issues](https://
-github.com/luisferreira97/talos) for a list of proposed features (and known
-issues).  ## Contributing Contributions are what make the open source community
-such an amazing place to be learn, inspire, and create. Any contributions you
-make are **greatly appreciated**. 1. Fork the Project 2. Create your Feature
-Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git
-commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin
-feature/AmazingFeature`) 5. Open a Pull Request  ## License Distributed under
-the MIT License. See `LICENSE` for more information.  ## Contact LuÃ­s Ferreira
-- [LinkedIn](https://www.linkedin.com/in/luisferreira97/) -
+X_test, y_test = aoc.load_example_data() run = aoc.fit( X=X_train, X_val=X_val,
+pop=10, gen=10, experiment_name="test", epochs=1000 ) predictions = aoc.predict
+(X_test, mode="all", threshold="default") score = aoc.evaluate(X_test, y_test,
+mode="all", metric="roc_auc", threshold="default") ``` _For more examples,
+please refer to the [Documentation](https://example.com)_-->  ## Citation To
+cite this work please use: ``` @article{FERREIRA2022109820, author = {LuÃ­s
+Ferreira and AndrÃ© Pilastri and Filipe Romano and Paulo Cortez}, title =
+{Using supervised and one-class automated machine learning for predictive
+maintenance}, journal = {Applied Soft Computing}, volume = {131}, pages =
+{109820}, year = {2022}, issn = {1568-4946}, doi = {https://doi.org/10.1016/
+j.asoc.2022.109820}, url = {https://www.sciencedirect.com/science/article/pii/
+S1568494622008699} } ```  ## Roadmap See the [open issues](https://github.com/
+luisferreira97/AutoOC) for a list of proposed features (and known issues).  ##
+Contributing Contributions are what make the open source community such an
+amazing place to be learn, inspire, and create. Any contributions you make are
+**greatly appreciated**. 1. Fork the Project 2. Create your Feature Branch
+(`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
+-m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
+AmazingFeature`) 5. Open a Pull Request  ## License Distributed under the MIT
+License. See `LICENSE` for more information.  ## Contact LuÃ­s Ferreira -
+[LinkedIn](https://www.linkedin.com/in/luisferreira97/) -
 luis_ferreira223@hotmail.com Project Link: [https://github.com/luisferreira97/
-talos](https://github.com/luisferreira97/talos)  ## Acknowledgements *
+AutoOC](https://github.com/luisferreira97/AutoOC)  ## Acknowledgements *
 [PonyGE2](https://github.com/PonyGE/PonyGE2)   [contributors-shield]: https://
 img.shields.io/github/contributors/othneildrew/Best-README-
 Template.svg?style=for-the-badge [contributors-url]: https://github.com/
-luisferreira97/talos/graphs/contributors [forks-shield]: https://
+luisferreira97/AutoOC/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-
-badge [forks-url]: https://github.com/luisferreira97/talos/network/members
+badge [forks-url]: https://github.com/luisferreira97/AutoOC/network/members
 [stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-
 Template.svg?style=for-the-badge [stars-url]: https://github.com/
-luisferreira97/talos/stargazers [issues-shield]: https://img.shields.io/github/
-issues/othneildrew/Best-README-Template.svg?style=for-the-badge [issues-url]:
-https://github.com/luisferreira97/talos/issues [license-shield]: https://
-img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-
-the-badge [license-url]: https://github.com/luisferreira97/talos/blob/master/
+luisferreira97/AutoOC/stargazers [issues-shield]: https://img.shields.io/
+github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge [issues-
+url]: https://github.com/luisferreira97/AutoOC/issues [license-shield]: https:/
+/img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-
+the-badge [license-url]: https://github.com/luisferreira97/AutoOC/blob/master/
 LICENSE [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-
 black.svg?style=for-the-badge&logo=linkedin&colorB=555 [linkedin-url]: https://
 www.linkedin.com/in/luisferreira97/ [product-screenshot]: images/screenshot.png
```

### Comparing `autooc-0.0.1/README.md` & `autooc-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,61 @@
+Metadata-Version: 2.1
+Name: autooc
+Version: 0.0.2
+Summary: AutoOC: Automated Machine Learning (AutoML) library for One-Class Learning
+Home-page: https://github.com/luisferreira97/AutoOC
+Author: Luís Ferreira
+Author-email: luis_ferreira223@hotmail.com
+Keywords: automl,machine learning,one-class learning,one-class classification,autoencoder,isolation forest,one-class svm
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!-- PROJECT SHIELDS -->
 <!--
 *** I'm using markdown "reference style" links for readability.
 *** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
 *** See the bottom of this document for the declaration of the reference variables
 *** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
-<!--[![Downloads](https://static.pepy.tech/personalized-badge/talos-automl?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/talos-automl)-->
+<!--[![Downloads](https://static.pepy.tech/personalized-badge/autooc?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/autooc)-->
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
-  <!--<a href="https://github.com/luisferreira97/talos">
+  <!--<a href="https://github.com/luisferreira97/AutoOC">
     <img src="images/logo.png" alt="Logo" width="80" height="115">
   </a>-->
 
   <h3 align="center">AutoOC (in Beta)</h3>
 
   <p align="center">
     AutoOC: Automated Machine Learning (AutoML) library focused on One-Class Learning algorithms (AutoEncoders, Isolation Forest and One-Class SVM)
     <br />
-    <a href="https://github.com/luisferreira97/talos"><strong>Explore the docs »</strong></a>
+    <a href="https://github.com/luisferreira97/AutoOC"><strong>Explore the docs »</strong></a>
     <br />
     <br />
-    <a href="https://github.com/luisferreira97/talos">View Demo</a>
+    <a href="https://github.com/luisferreira97/AutoOC">View Demo</a>
     ·
-    <a href="https://github.com/luisferreira97/talos/issues">Report Bug</a>
+    <a href="https://github.com/luisferreira97/AutoOC/issues">Report Bug</a>
     ·
-    <a href="https://github.com/luisferreira97/talos/issues">Request Feature</a>
+    <a href="https://github.com/luisferreira97/AutoOC/issues">Request Feature</a>
   </p>
 </p>
 
 
 
 <!-- TABLE OF CONTENTS -->
 <details open="open">
@@ -99,63 +114,62 @@
 <!-- GETTING STARTED -->
 ## Getting Started
 
 This section presents how the package can be reached and installed.
 
 ### Where to get it
 
-The source code is currently hosted on GitHub at: https://github.com/luisferreira97/talos
+The source code is currently hosted on GitHub at: https://github.com/luisferreira97/AutoOC
 
-Binary installer for the latest released version are available at the Python Package Index (PyPI).
-Note that the PyPI name of the package is `talos-automl` and not `talos`.
+Binary installer for the latest released version are available at the Python Package Index (PyPI). The PyPI name of the package is `autooc`.
 
 ```sh
-pip install talos-automl
+pip install autooc
 ```
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 ### 1. Import the package
-The first step in using the package is, after it has been installed, to import it. The main class from which all the methods are available is ```Talos```.
+The first step in using the package is, after it has been installed, to import it. The main class from which all the methods are available is ```AutoOC```.
 
 ```python
-from talos.talos import Talos
+from autooc.autooc import AutoOC
 ```
 
-### 2. Instantiate a Talos object
-The second step is to instantiate the Talos class with the information about your dataset and context (e.g., normal and anomaly classes, wether to run single-objective or multi-objective, the performance_metric, and the algorithm).
+### 2. Instantiate a AutoOC object
+The second step is to instantiate the AutoOC class with the information about your dataset and context (e.g., normal and anomaly classes, wether to run single-objective or multi-objective, the performance_metric, and the algorithm).
 You can change the ```algorithm``` parameter to select which algorithms are used during the optimization. The options are:
 - "autoencoders": Deep AutoEncoders (from TensorFlow)
 - "iforest": Isolation Forest (from Scikit-Learn)
 - "svm": One-Class SVM (from Scikit-Learn)
 - "all": the optimization is done using the three algorithms above
 
 ```python
-talos = Talos(anomaly_class = 0,
+aoc = AutoOC(anomaly_class = 0,
     normal_class = 1,
     multiobjective=True,
     performance_metric="training_time",
     algorithm = "autoencoder"
 )
 ```
 
 ### 3. Load dataset
 The third step is to load the dataset. Depending on the type of validation you need *train data* (only 'normal' instances), *validation data* (you can use (1) only 'normal' instances or (2) both 'normal' and 'anomaly' instances with the respective labels), and *test data* (both types of instances and labels). You can use the ```load_example_data()``` function to load the popular ECG dataset.
 
 
 ```python
-X_train, X_val, X_test, y_test = talos.load_example_data()
+X_train, X_val, X_test, y_test = aoc.load_example_data()
 ```
 
 ### 4. Train
 The fourth step is to train the model. The ```fit()``` function computes the optimization using the given parameters.
 
 ```python
-run = talos.fit(
+run = aoc.fit(
     X=X_train,
     X_val=X_val,
     pop=10,
     gen=10,
     experiment_name="test",
     epochs=1000
 )
@@ -174,59 +188,59 @@
 - "mean": For each model the threshold value is the sum of the mean reconstruction error obtained on the validation data and one standard deviation.
 - "percentile": For each model the threshold value is the 95th percentile of the reconstruction error obtained on the validation data (you can also use the ```percentile``` parameter to change the percentile).
 - "max": For each model the threshold value is maximum reconstruction error obtained on the validation data.
 - You can also pass an Integer of Float value. In this case, the threshold value is the same for all the models.
 
 
 ```python
-predictions = talos.predict(X_test,
+predictions = aoc.predict(X_test,
     mode="all",
     threshold="default")
 ```
 
 ### 6. Evaluate
 
 You can use the predictions to calculate manually the performance metrics of the model. However, the ```evaluate()``` function is a more convenient way to do it. You can also use the ```mode``` parameter (works similarly to the ```predict()``` function) and use metrics from the ```sklearn.metrics``` package (currently available are "roc_auc", "accuracy", "precision", "recall", and "f1").
 
 ```python
-score = talos.evaluate(X_test,
+score = aoc.evaluate(X_test,
     y_test,
     mode="all",
     metric="roc_auc",
     threshold="default")
 ```
 
 ## Usage
 
 ```python
-from talos.talos import Talos
+from autooc.autooc import AutoOC
 
-talos = Talos(anomaly_class = 0,
+aoc = AutoOC(anomaly_class = 0,
     normal_class = 1,
     multiobjective=True,
     performance_metric="training_time",
     algorithm = "autoencoder"
 )
 
-X_train, X_val, X_test, y_test = talos.load_example_data()
+X_train, X_val, X_test, y_test = aoc.load_example_data()
 
-run = talos.fit(
+run = aoc.fit(
     X=X_train,
     X_val=X_val,
     pop=10,
     gen=10,
     experiment_name="test",
     epochs=1000
 )
 
-predictions = talos.predict(X_test,
+predictions = aoc.predict(X_test,
     mode="all",
     threshold="default")
 
-score = talos.evaluate(X_test,
+score = aoc.evaluate(X_test,
     y_test,
     mode="all",
     metric="roc_auc",
     threshold="default")
 ```
 
 _For more examples, please refer to the [Documentation](https://example.com)_-->
@@ -249,15 +263,15 @@
   url = {https://www.sciencedirect.com/science/article/pii/S1568494622008699}
 }
 ```
 
 <!-- ROADMAP -->
 ## Roadmap
 
-See the [open issues](https://github.com/luisferreira97/talos) for a list of proposed features (and known issues).
+See the [open issues](https://github.com/luisferreira97/AutoOC) for a list of proposed features (and known issues).
 
 
 
 <!-- CONTRIBUTING -->
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.
@@ -278,34 +292,34 @@
 
 
 <!-- CONTACT -->
 ## Contact
 
 Luís Ferreira - [LinkedIn](https://www.linkedin.com/in/luisferreira97/) - luis_ferreira223@hotmail.com
 
-Project Link: [https://github.com/luisferreira97/talos](https://github.com/luisferreira97/talos)
+Project Link: [https://github.com/luisferreira97/AutoOC](https://github.com/luisferreira97/AutoOC)
 
 
 
 <!-- ACKNOWLEDGEMENTS -->
 ## Acknowledgements
 * [PonyGE2](https://github.com/PonyGE/PonyGE2)
 
 
 
 
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
-[contributors-url]: https://github.com/luisferreira97/talos/graphs/contributors
+[contributors-url]: https://github.com/luisferreira97/AutoOC/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
-[forks-url]: https://github.com/luisferreira97/talos/network/members
+[forks-url]: https://github.com/luisferreira97/AutoOC/network/members
 [stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
-[stars-url]: https://github.com/luisferreira97/talos/stargazers
+[stars-url]: https://github.com/luisferreira97/AutoOC/stargazers
 [issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
-[issues-url]: https://github.com/luisferreira97/talos/issues
+[issues-url]: https://github.com/luisferreira97/AutoOC/issues
 [license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
-[license-url]: https://github.com/luisferreira97/talos/blob/master/LICENSE
+[license-url]: https://github.com/luisferreira97/AutoOC/blob/master/LICENSE
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 [linkedin-url]: https://www.linkedin.com/in/luisferreira97/
 [product-screenshot]: images/screenshot.png
```

#### html2text {}

```diff
@@ -1,11 +1,19 @@
-   [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
-[linkedin-shield]][linkedin-url]
+Metadata-Version: 2.1 Name: autooc Version: 0.0.2 Summary: AutoOC: Automated
+Machine Learning (AutoML) library for One-Class Learning Home-page: https://
+github.com/luisferreira97/AutoOC Author: LuÃ­s Ferreira Author-email:
+luis_ferreira223@hotmail.com Keywords: automl,machine learning,one-class
+learning,one-class classification,autoencoder,isolation forest,one-class svm
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE    [![Contributors][contributors-shield]][contributors-url] [![Forks]
+[forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues]
+[issues-shield]][issues-url] [![MIT License][license-shield]][license-url] [!
+[LinkedIn][linkedin-shield]][linkedin-url]
                           **** AutoOC (in Beta) ****
    AutoOC: Automated Machine Learning (AutoML) library focused on One-Class
     Learning algorithms (AutoEncoders, Isolation Forest and One-Class SVM)
                              Explore_the_docs_Â»
 
                   View_Demo Â· Report_Bug Â· Request_Feature
   Table of Contents
@@ -36,104 +44,103 @@
 acknowledgements. ### Built With This section should list any major frameworks
 that you built your project using. Leave any add-ons/plugins for the
 acknowledgements section. Here are a few examples. * [Python](https://
 www.python.org) * [PonyGE2](https://github.com/PonyGE/PonyGE2) * [TensorFlow]
 (https://www.tensorflow.org/) * [Scikit-Learn](https://scikit-learn.org/)  ##
 Getting Started This section presents how the package can be reached and
 installed. ### Where to get it The source code is currently hosted on GitHub
-at: https://github.com/luisferreira97/talos Binary installer for the latest
-released version are available at the Python Package Index (PyPI). Note that
-the PyPI name of the package is `talos-automl` and not `talos`. ```sh pip
-install talos-automl ```  ## Usage ### 1. Import the package The first step in
-using the package is, after it has been installed, to import it. The main class
-from which all the methods are available is ```Talos```. ```python from
-talos.talos import Talos ``` ### 2. Instantiate a Talos object The second step
-is to instantiate the Talos class with the information about your dataset and
-context (e.g., normal and anomaly classes, wether to run single-objective or
-multi-objective, the performance_metric, and the algorithm). You can change the
-```algorithm``` parameter to select which algorithms are used during the
-optimization. The options are: - "autoencoders": Deep AutoEncoders (from
-TensorFlow) - "iforest": Isolation Forest (from Scikit-Learn) - "svm": One-
-Class SVM (from Scikit-Learn) - "all": the optimization is done using the three
-algorithms above ```python talos = Talos(anomaly_class = 0, normal_class = 1,
-multiobjective=True, performance_metric="training_time", algorithm =
-"autoencoder" ) ``` ### 3. Load dataset The third step is to load the dataset.
-Depending on the type of validation you need *train data* (only 'normal'
-instances), *validation data* (you can use (1) only 'normal' instances or (2)
-both 'normal' and 'anomaly' instances with the respective labels), and *test
-data* (both types of instances and labels). You can use the
-```load_example_data()``` function to load the popular ECG dataset. ```python
-X_train, X_val, X_test, y_test = talos.load_example_data() ``` ### 4. Train The
-fourth step is to train the model. The ```fit()``` function computes the
-optimization using the given parameters. ```python run = talos.fit( X=X_train,
-X_val=X_val, pop=10, gen=10, experiment_name="test", epochs=1000 ) ``` ### 5.
-Predict The fifth step is to predict the labels of the test data. You can use
-the ```predict()``` function to predict the labels of the test data. You can
-change the ```mode``` parameter to select which individuals are used to
-predict. - "all": uses all individuals (models) from the last generation -
-"best": uses the from the last generation which achieved the best predictive
-metric - "simplest": uses the from the last generation which achieved the best
-efficiency metric - "pareto": uses the pareto individuals from the last
-generation (only for multiobjective. These are the models that achieved
-simultaneouly the best predictive metric and efficiency metric. Additionally,
-you can use the ```threshold``` parameter (only used for AutoEncoders) to set
-the threshold for the prediction. You can use the following values: -
-"default": uses a different threshold value for each individual (model). For
-each model the threshold value is the associated default value (currently this
-works similar to the "mean" value). - "mean": For each model the threshold
-value is the sum of the mean reconstruction error obtained on the validation
-data and one standard deviation. - "percentile": For each model the threshold
-value is the 95th percentile of the reconstruction error obtained on the
-validation data (you can also use the ```percentile``` parameter to change the
-percentile). - "max": For each model the threshold value is maximum
-reconstruction error obtained on the validation data. - You can also pass an
-Integer of Float value. In this case, the threshold value is the same for all
-the models. ```python predictions = talos.predict(X_test, mode="all",
-threshold="default") ``` ### 6. Evaluate You can use the predictions to
-calculate manually the performance metrics of the model. However, the
-```evaluate()``` function is a more convenient way to do it. You can also use
-the ```mode``` parameter (works similarly to the ```predict()``` function) and
-use metrics from the ```sklearn.metrics``` package (currently available are
-"roc_auc", "accuracy", "precision", "recall", and "f1"). ```python score =
-talos.evaluate(X_test, y_test, mode="all", metric="roc_auc",
-threshold="default") ``` ## Usage ```python from talos.talos import Talos talos
-= Talos(anomaly_class = 0, normal_class = 1, multiobjective=True,
+at: https://github.com/luisferreira97/AutoOC Binary installer for the latest
+released version are available at the Python Package Index (PyPI). The PyPI
+name of the package is `autooc`. ```sh pip install autooc ```  ## Usage ### 1.
+Import the package The first step in using the package is, after it has been
+installed, to import it. The main class from which all the methods are
+available is ```AutoOC```. ```python from autooc.autooc import AutoOC ``` ###
+2. Instantiate a AutoOC object The second step is to instantiate the AutoOC
+class with the information about your dataset and context (e.g., normal and
+anomaly classes, wether to run single-objective or multi-objective, the
+performance_metric, and the algorithm). You can change the ```algorithm```
+parameter to select which algorithms are used during the optimization. The
+options are: - "autoencoders": Deep AutoEncoders (from TensorFlow) - "iforest":
+Isolation Forest (from Scikit-Learn) - "svm": One-Class SVM (from Scikit-Learn)
+- "all": the optimization is done using the three algorithms above ```python
+aoc = AutoOC(anomaly_class = 0, normal_class = 1, multiobjective=True,
+performance_metric="training_time", algorithm = "autoencoder" ) ``` ### 3. Load
+dataset The third step is to load the dataset. Depending on the type of
+validation you need *train data* (only 'normal' instances), *validation data*
+(you can use (1) only 'normal' instances or (2) both 'normal' and 'anomaly'
+instances with the respective labels), and *test data* (both types of instances
+and labels). You can use the ```load_example_data()``` function to load the
+popular ECG dataset. ```python X_train, X_val, X_test, y_test =
+aoc.load_example_data() ``` ### 4. Train The fourth step is to train the model.
+The ```fit()``` function computes the optimization using the given parameters.
+```python run = aoc.fit( X=X_train, X_val=X_val, pop=10, gen=10,
+experiment_name="test", epochs=1000 ) ``` ### 5. Predict The fifth step is to
+predict the labels of the test data. You can use the ```predict()``` function
+to predict the labels of the test data. You can change the ```mode``` parameter
+to select which individuals are used to predict. - "all": uses all individuals
+(models) from the last generation - "best": uses the from the last generation
+which achieved the best predictive metric - "simplest": uses the from the last
+generation which achieved the best efficiency metric - "pareto": uses the
+pareto individuals from the last generation (only for multiobjective. These are
+the models that achieved simultaneouly the best predictive metric and
+efficiency metric. Additionally, you can use the ```threshold``` parameter
+(only used for AutoEncoders) to set the threshold for the prediction. You can
+use the following values: - "default": uses a different threshold value for
+each individual (model). For each model the threshold value is the associated
+default value (currently this works similar to the "mean" value). - "mean": For
+each model the threshold value is the sum of the mean reconstruction error
+obtained on the validation data and one standard deviation. - "percentile": For
+each model the threshold value is the 95th percentile of the reconstruction
+error obtained on the validation data (you can also use the ```percentile```
+parameter to change the percentile). - "max": For each model the threshold
+value is maximum reconstruction error obtained on the validation data. - You
+can also pass an Integer of Float value. In this case, the threshold value is
+the same for all the models. ```python predictions = aoc.predict(X_test,
+mode="all", threshold="default") ``` ### 6. Evaluate You can use the
+predictions to calculate manually the performance metrics of the model.
+However, the ```evaluate()``` function is a more convenient way to do it. You
+can also use the ```mode``` parameter (works similarly to the ```predict()```
+function) and use metrics from the ```sklearn.metrics``` package (currently
+available are "roc_auc", "accuracy", "precision", "recall", and "f1").
+```python score = aoc.evaluate(X_test, y_test, mode="all", metric="roc_auc",
+threshold="default") ``` ## Usage ```python from autooc.autooc import AutoOC
+aoc = AutoOC(anomaly_class = 0, normal_class = 1, multiobjective=True,
 performance_metric="training_time", algorithm = "autoencoder" ) X_train, X_val,
-X_test, y_test = talos.load_example_data() run = talos.fit( X=X_train,
-X_val=X_val, pop=10, gen=10, experiment_name="test", epochs=1000 ) predictions
-= talos.predict(X_test, mode="all", threshold="default") score = talos.evaluate
-(X_test, y_test, mode="all", metric="roc_auc", threshold="default") ``` _For
-more examples, please refer to the [Documentation](https://example.com)_-->  ##
-Citation To cite this work please use: ``` @article{FERREIRA2022109820, author
-= {LuÃ­s Ferreira and AndrÃ© Pilastri and Filipe Romano and Paulo Cortez},
-title = {Using supervised and one-class automated machine learning for
-predictive maintenance}, journal = {Applied Soft Computing}, volume = {131},
-pages = {109820}, year = {2022}, issn = {1568-4946}, doi = {https://doi.org/
-10.1016/j.asoc.2022.109820}, url = {https://www.sciencedirect.com/science/
-article/pii/S1568494622008699} } ```  ## Roadmap See the [open issues](https://
-github.com/luisferreira97/talos) for a list of proposed features (and known
-issues).  ## Contributing Contributions are what make the open source community
-such an amazing place to be learn, inspire, and create. Any contributions you
-make are **greatly appreciated**. 1. Fork the Project 2. Create your Feature
-Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git
-commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin
-feature/AmazingFeature`) 5. Open a Pull Request  ## License Distributed under
-the MIT License. See `LICENSE` for more information.  ## Contact LuÃ­s Ferreira
-- [LinkedIn](https://www.linkedin.com/in/luisferreira97/) -
+X_test, y_test = aoc.load_example_data() run = aoc.fit( X=X_train, X_val=X_val,
+pop=10, gen=10, experiment_name="test", epochs=1000 ) predictions = aoc.predict
+(X_test, mode="all", threshold="default") score = aoc.evaluate(X_test, y_test,
+mode="all", metric="roc_auc", threshold="default") ``` _For more examples,
+please refer to the [Documentation](https://example.com)_-->  ## Citation To
+cite this work please use: ``` @article{FERREIRA2022109820, author = {LuÃ­s
+Ferreira and AndrÃ© Pilastri and Filipe Romano and Paulo Cortez}, title =
+{Using supervised and one-class automated machine learning for predictive
+maintenance}, journal = {Applied Soft Computing}, volume = {131}, pages =
+{109820}, year = {2022}, issn = {1568-4946}, doi = {https://doi.org/10.1016/
+j.asoc.2022.109820}, url = {https://www.sciencedirect.com/science/article/pii/
+S1568494622008699} } ```  ## Roadmap See the [open issues](https://github.com/
+luisferreira97/AutoOC) for a list of proposed features (and known issues).  ##
+Contributing Contributions are what make the open source community such an
+amazing place to be learn, inspire, and create. Any contributions you make are
+**greatly appreciated**. 1. Fork the Project 2. Create your Feature Branch
+(`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
+-m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
+AmazingFeature`) 5. Open a Pull Request  ## License Distributed under the MIT
+License. See `LICENSE` for more information.  ## Contact LuÃ­s Ferreira -
+[LinkedIn](https://www.linkedin.com/in/luisferreira97/) -
 luis_ferreira223@hotmail.com Project Link: [https://github.com/luisferreira97/
-talos](https://github.com/luisferreira97/talos)  ## Acknowledgements *
+AutoOC](https://github.com/luisferreira97/AutoOC)  ## Acknowledgements *
 [PonyGE2](https://github.com/PonyGE/PonyGE2)   [contributors-shield]: https://
 img.shields.io/github/contributors/othneildrew/Best-README-
 Template.svg?style=for-the-badge [contributors-url]: https://github.com/
-luisferreira97/talos/graphs/contributors [forks-shield]: https://
+luisferreira97/AutoOC/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-
-badge [forks-url]: https://github.com/luisferreira97/talos/network/members
+badge [forks-url]: https://github.com/luisferreira97/AutoOC/network/members
 [stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-
 Template.svg?style=for-the-badge [stars-url]: https://github.com/
-luisferreira97/talos/stargazers [issues-shield]: https://img.shields.io/github/
-issues/othneildrew/Best-README-Template.svg?style=for-the-badge [issues-url]:
-https://github.com/luisferreira97/talos/issues [license-shield]: https://
-img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-
-the-badge [license-url]: https://github.com/luisferreira97/talos/blob/master/
+luisferreira97/AutoOC/stargazers [issues-shield]: https://img.shields.io/
+github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge [issues-
+url]: https://github.com/luisferreira97/AutoOC/issues [license-shield]: https:/
+/img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-
+the-badge [license-url]: https://github.com/luisferreira97/AutoOC/blob/master/
 LICENSE [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-
 black.svg?style=for-the-badge&logo=linkedin&colorB=555 [linkedin-url]: https://
 www.linkedin.com/in/luisferreira97/ [product-screenshot]: images/screenshot.png
```

### Comparing `autooc-0.0.1/autooc.egg-info/PKG-INFO` & `autooc-0.0.2/autooc.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autooc
-Version: 0.0.1
+Version: 0.0.2
 Summary: AutoOC: Automated Machine Learning (AutoML) library for One-Class Learning
 Home-page: https://github.com/luisferreira97/AutoOC
 Author: Luís Ferreira
 Author-email: luis_ferreira223@hotmail.com
 Keywords: automl,machine learning,one-class learning,one-class classification,autoencoder,isolation forest,one-class svm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,45 +17,45 @@
 <!--
 *** I'm using markdown "reference style" links for readability.
 *** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
 *** See the bottom of this document for the declaration of the reference variables
 *** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
 *** https://www.markdownguide.org/basic-syntax/#reference-style-links
 -->
-<!--[![Downloads](https://static.pepy.tech/personalized-badge/talos-automl?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/talos-automl)-->
+<!--[![Downloads](https://static.pepy.tech/personalized-badge/autooc?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/autooc)-->
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
-  <!--<a href="https://github.com/luisferreira97/talos">
+  <!--<a href="https://github.com/luisferreira97/AutoOC">
     <img src="images/logo.png" alt="Logo" width="80" height="115">
   </a>-->
 
   <h3 align="center">AutoOC (in Beta)</h3>
 
   <p align="center">
     AutoOC: Automated Machine Learning (AutoML) library focused on One-Class Learning algorithms (AutoEncoders, Isolation Forest and One-Class SVM)
     <br />
-    <a href="https://github.com/luisferreira97/talos"><strong>Explore the docs »</strong></a>
+    <a href="https://github.com/luisferreira97/AutoOC"><strong>Explore the docs »</strong></a>
     <br />
     <br />
-    <a href="https://github.com/luisferreira97/talos">View Demo</a>
+    <a href="https://github.com/luisferreira97/AutoOC">View Demo</a>
     ·
-    <a href="https://github.com/luisferreira97/talos/issues">Report Bug</a>
+    <a href="https://github.com/luisferreira97/AutoOC/issues">Report Bug</a>
     ·
-    <a href="https://github.com/luisferreira97/talos/issues">Request Feature</a>
+    <a href="https://github.com/luisferreira97/AutoOC/issues">Request Feature</a>
   </p>
 </p>
 
 
 
 <!-- TABLE OF CONTENTS -->
 <details open="open">
@@ -114,63 +114,62 @@
 <!-- GETTING STARTED -->
 ## Getting Started
 
 This section presents how the package can be reached and installed.
 
 ### Where to get it
 
-The source code is currently hosted on GitHub at: https://github.com/luisferreira97/talos
+The source code is currently hosted on GitHub at: https://github.com/luisferreira97/AutoOC
 
-Binary installer for the latest released version are available at the Python Package Index (PyPI).
-Note that the PyPI name of the package is `talos-automl` and not `talos`.
+Binary installer for the latest released version are available at the Python Package Index (PyPI). The PyPI name of the package is `autooc`.
 
 ```sh
-pip install talos-automl
+pip install autooc
 ```
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 ### 1. Import the package
-The first step in using the package is, after it has been installed, to import it. The main class from which all the methods are available is ```Talos```.
+The first step in using the package is, after it has been installed, to import it. The main class from which all the methods are available is ```AutoOC```.
 
 ```python
-from talos.talos import Talos
+from autooc.autooc import AutoOC
 ```
 
-### 2. Instantiate a Talos object
-The second step is to instantiate the Talos class with the information about your dataset and context (e.g., normal and anomaly classes, wether to run single-objective or multi-objective, the performance_metric, and the algorithm).
+### 2. Instantiate a AutoOC object
+The second step is to instantiate the AutoOC class with the information about your dataset and context (e.g., normal and anomaly classes, wether to run single-objective or multi-objective, the performance_metric, and the algorithm).
 You can change the ```algorithm``` parameter to select which algorithms are used during the optimization. The options are:
 - "autoencoders": Deep AutoEncoders (from TensorFlow)
 - "iforest": Isolation Forest (from Scikit-Learn)
 - "svm": One-Class SVM (from Scikit-Learn)
 - "all": the optimization is done using the three algorithms above
 
 ```python
-talos = Talos(anomaly_class = 0,
+aoc = AutoOC(anomaly_class = 0,
     normal_class = 1,
     multiobjective=True,
     performance_metric="training_time",
     algorithm = "autoencoder"
 )
 ```
 
 ### 3. Load dataset
 The third step is to load the dataset. Depending on the type of validation you need *train data* (only 'normal' instances), *validation data* (you can use (1) only 'normal' instances or (2) both 'normal' and 'anomaly' instances with the respective labels), and *test data* (both types of instances and labels). You can use the ```load_example_data()``` function to load the popular ECG dataset.
 
 
 ```python
-X_train, X_val, X_test, y_test = talos.load_example_data()
+X_train, X_val, X_test, y_test = aoc.load_example_data()
 ```
 
 ### 4. Train
 The fourth step is to train the model. The ```fit()``` function computes the optimization using the given parameters.
 
 ```python
-run = talos.fit(
+run = aoc.fit(
     X=X_train,
     X_val=X_val,
     pop=10,
     gen=10,
     experiment_name="test",
     epochs=1000
 )
@@ -189,59 +188,59 @@
 - "mean": For each model the threshold value is the sum of the mean reconstruction error obtained on the validation data and one standard deviation.
 - "percentile": For each model the threshold value is the 95th percentile of the reconstruction error obtained on the validation data (you can also use the ```percentile``` parameter to change the percentile).
 - "max": For each model the threshold value is maximum reconstruction error obtained on the validation data.
 - You can also pass an Integer of Float value. In this case, the threshold value is the same for all the models.
 
 
 ```python
-predictions = talos.predict(X_test,
+predictions = aoc.predict(X_test,
     mode="all",
     threshold="default")
 ```
 
 ### 6. Evaluate
 
 You can use the predictions to calculate manually the performance metrics of the model. However, the ```evaluate()``` function is a more convenient way to do it. You can also use the ```mode``` parameter (works similarly to the ```predict()``` function) and use metrics from the ```sklearn.metrics``` package (currently available are "roc_auc", "accuracy", "precision", "recall", and "f1").
 
 ```python
-score = talos.evaluate(X_test,
+score = aoc.evaluate(X_test,
     y_test,
     mode="all",
     metric="roc_auc",
     threshold="default")
 ```
 
 ## Usage
 
 ```python
-from talos.talos import Talos
+from autooc.autooc import AutoOC
 
-talos = Talos(anomaly_class = 0,
+aoc = AutoOC(anomaly_class = 0,
     normal_class = 1,
     multiobjective=True,
     performance_metric="training_time",
     algorithm = "autoencoder"
 )
 
-X_train, X_val, X_test, y_test = talos.load_example_data()
+X_train, X_val, X_test, y_test = aoc.load_example_data()
 
-run = talos.fit(
+run = aoc.fit(
     X=X_train,
     X_val=X_val,
     pop=10,
     gen=10,
     experiment_name="test",
     epochs=1000
 )
 
-predictions = talos.predict(X_test,
+predictions = aoc.predict(X_test,
     mode="all",
     threshold="default")
 
-score = talos.evaluate(X_test,
+score = aoc.evaluate(X_test,
     y_test,
     mode="all",
     metric="roc_auc",
     threshold="default")
 ```
 
 _For more examples, please refer to the [Documentation](https://example.com)_-->
@@ -264,15 +263,15 @@
   url = {https://www.sciencedirect.com/science/article/pii/S1568494622008699}
 }
 ```
 
 <!-- ROADMAP -->
 ## Roadmap
 
-See the [open issues](https://github.com/luisferreira97/talos) for a list of proposed features (and known issues).
+See the [open issues](https://github.com/luisferreira97/AutoOC) for a list of proposed features (and known issues).
 
 
 
 <!-- CONTRIBUTING -->
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.
@@ -293,34 +292,34 @@
 
 
 <!-- CONTACT -->
 ## Contact
 
 Luís Ferreira - [LinkedIn](https://www.linkedin.com/in/luisferreira97/) - luis_ferreira223@hotmail.com
 
-Project Link: [https://github.com/luisferreira97/talos](https://github.com/luisferreira97/talos)
+Project Link: [https://github.com/luisferreira97/AutoOC](https://github.com/luisferreira97/AutoOC)
 
 
 
 <!-- ACKNOWLEDGEMENTS -->
 ## Acknowledgements
 * [PonyGE2](https://github.com/PonyGE/PonyGE2)
 
 
 
 
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
-[contributors-url]: https://github.com/luisferreira97/talos/graphs/contributors
+[contributors-url]: https://github.com/luisferreira97/AutoOC/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
-[forks-url]: https://github.com/luisferreira97/talos/network/members
+[forks-url]: https://github.com/luisferreira97/AutoOC/network/members
 [stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
-[stars-url]: https://github.com/luisferreira97/talos/stargazers
+[stars-url]: https://github.com/luisferreira97/AutoOC/stargazers
 [issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
-[issues-url]: https://github.com/luisferreira97/talos/issues
+[issues-url]: https://github.com/luisferreira97/AutoOC/issues
 [license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
-[license-url]: https://github.com/luisferreira97/talos/blob/master/LICENSE
+[license-url]: https://github.com/luisferreira97/AutoOC/blob/master/LICENSE
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 [linkedin-url]: https://www.linkedin.com/in/luisferreira97/
 [product-screenshot]: images/screenshot.png
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autooc Version: 0.0.1 Summary: AutoOC: Automated
+Metadata-Version: 2.1 Name: autooc Version: 0.0.2 Summary: AutoOC: Automated
 Machine Learning (AutoML) library for One-Class Learning Home-page: https://
 github.com/luisferreira97/AutoOC Author: LuÃ­s Ferreira Author-email:
 luis_ferreira223@hotmail.com Keywords: automl,machine learning,one-class
 learning,one-class classification,autoencoder,isolation forest,one-class svm
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
@@ -44,104 +44,103 @@
 acknowledgements. ### Built With This section should list any major frameworks
 that you built your project using. Leave any add-ons/plugins for the
 acknowledgements section. Here are a few examples. * [Python](https://
 www.python.org) * [PonyGE2](https://github.com/PonyGE/PonyGE2) * [TensorFlow]
 (https://www.tensorflow.org/) * [Scikit-Learn](https://scikit-learn.org/)  ##
 Getting Started This section presents how the package can be reached and
 installed. ### Where to get it The source code is currently hosted on GitHub
-at: https://github.com/luisferreira97/talos Binary installer for the latest
-released version are available at the Python Package Index (PyPI). Note that
-the PyPI name of the package is `talos-automl` and not `talos`. ```sh pip
-install talos-automl ```  ## Usage ### 1. Import the package The first step in
-using the package is, after it has been installed, to import it. The main class
-from which all the methods are available is ```Talos```. ```python from
-talos.talos import Talos ``` ### 2. Instantiate a Talos object The second step
-is to instantiate the Talos class with the information about your dataset and
-context (e.g., normal and anomaly classes, wether to run single-objective or
-multi-objective, the performance_metric, and the algorithm). You can change the
-```algorithm``` parameter to select which algorithms are used during the
-optimization. The options are: - "autoencoders": Deep AutoEncoders (from
-TensorFlow) - "iforest": Isolation Forest (from Scikit-Learn) - "svm": One-
-Class SVM (from Scikit-Learn) - "all": the optimization is done using the three
-algorithms above ```python talos = Talos(anomaly_class = 0, normal_class = 1,
-multiobjective=True, performance_metric="training_time", algorithm =
-"autoencoder" ) ``` ### 3. Load dataset The third step is to load the dataset.
-Depending on the type of validation you need *train data* (only 'normal'
-instances), *validation data* (you can use (1) only 'normal' instances or (2)
-both 'normal' and 'anomaly' instances with the respective labels), and *test
-data* (both types of instances and labels). You can use the
-```load_example_data()``` function to load the popular ECG dataset. ```python
-X_train, X_val, X_test, y_test = talos.load_example_data() ``` ### 4. Train The
-fourth step is to train the model. The ```fit()``` function computes the
-optimization using the given parameters. ```python run = talos.fit( X=X_train,
-X_val=X_val, pop=10, gen=10, experiment_name="test", epochs=1000 ) ``` ### 5.
-Predict The fifth step is to predict the labels of the test data. You can use
-the ```predict()``` function to predict the labels of the test data. You can
-change the ```mode``` parameter to select which individuals are used to
-predict. - "all": uses all individuals (models) from the last generation -
-"best": uses the from the last generation which achieved the best predictive
-metric - "simplest": uses the from the last generation which achieved the best
-efficiency metric - "pareto": uses the pareto individuals from the last
-generation (only for multiobjective. These are the models that achieved
-simultaneouly the best predictive metric and efficiency metric. Additionally,
-you can use the ```threshold``` parameter (only used for AutoEncoders) to set
-the threshold for the prediction. You can use the following values: -
-"default": uses a different threshold value for each individual (model). For
-each model the threshold value is the associated default value (currently this
-works similar to the "mean" value). - "mean": For each model the threshold
-value is the sum of the mean reconstruction error obtained on the validation
-data and one standard deviation. - "percentile": For each model the threshold
-value is the 95th percentile of the reconstruction error obtained on the
-validation data (you can also use the ```percentile``` parameter to change the
-percentile). - "max": For each model the threshold value is maximum
-reconstruction error obtained on the validation data. - You can also pass an
-Integer of Float value. In this case, the threshold value is the same for all
-the models. ```python predictions = talos.predict(X_test, mode="all",
-threshold="default") ``` ### 6. Evaluate You can use the predictions to
-calculate manually the performance metrics of the model. However, the
-```evaluate()``` function is a more convenient way to do it. You can also use
-the ```mode``` parameter (works similarly to the ```predict()``` function) and
-use metrics from the ```sklearn.metrics``` package (currently available are
-"roc_auc", "accuracy", "precision", "recall", and "f1"). ```python score =
-talos.evaluate(X_test, y_test, mode="all", metric="roc_auc",
-threshold="default") ``` ## Usage ```python from talos.talos import Talos talos
-= Talos(anomaly_class = 0, normal_class = 1, multiobjective=True,
+at: https://github.com/luisferreira97/AutoOC Binary installer for the latest
+released version are available at the Python Package Index (PyPI). The PyPI
+name of the package is `autooc`. ```sh pip install autooc ```  ## Usage ### 1.
+Import the package The first step in using the package is, after it has been
+installed, to import it. The main class from which all the methods are
+available is ```AutoOC```. ```python from autooc.autooc import AutoOC ``` ###
+2. Instantiate a AutoOC object The second step is to instantiate the AutoOC
+class with the information about your dataset and context (e.g., normal and
+anomaly classes, wether to run single-objective or multi-objective, the
+performance_metric, and the algorithm). You can change the ```algorithm```
+parameter to select which algorithms are used during the optimization. The
+options are: - "autoencoders": Deep AutoEncoders (from TensorFlow) - "iforest":
+Isolation Forest (from Scikit-Learn) - "svm": One-Class SVM (from Scikit-Learn)
+- "all": the optimization is done using the three algorithms above ```python
+aoc = AutoOC(anomaly_class = 0, normal_class = 1, multiobjective=True,
+performance_metric="training_time", algorithm = "autoencoder" ) ``` ### 3. Load
+dataset The third step is to load the dataset. Depending on the type of
+validation you need *train data* (only 'normal' instances), *validation data*
+(you can use (1) only 'normal' instances or (2) both 'normal' and 'anomaly'
+instances with the respective labels), and *test data* (both types of instances
+and labels). You can use the ```load_example_data()``` function to load the
+popular ECG dataset. ```python X_train, X_val, X_test, y_test =
+aoc.load_example_data() ``` ### 4. Train The fourth step is to train the model.
+The ```fit()``` function computes the optimization using the given parameters.
+```python run = aoc.fit( X=X_train, X_val=X_val, pop=10, gen=10,
+experiment_name="test", epochs=1000 ) ``` ### 5. Predict The fifth step is to
+predict the labels of the test data. You can use the ```predict()``` function
+to predict the labels of the test data. You can change the ```mode``` parameter
+to select which individuals are used to predict. - "all": uses all individuals
+(models) from the last generation - "best": uses the from the last generation
+which achieved the best predictive metric - "simplest": uses the from the last
+generation which achieved the best efficiency metric - "pareto": uses the
+pareto individuals from the last generation (only for multiobjective. These are
+the models that achieved simultaneouly the best predictive metric and
+efficiency metric. Additionally, you can use the ```threshold``` parameter
+(only used for AutoEncoders) to set the threshold for the prediction. You can
+use the following values: - "default": uses a different threshold value for
+each individual (model). For each model the threshold value is the associated
+default value (currently this works similar to the "mean" value). - "mean": For
+each model the threshold value is the sum of the mean reconstruction error
+obtained on the validation data and one standard deviation. - "percentile": For
+each model the threshold value is the 95th percentile of the reconstruction
+error obtained on the validation data (you can also use the ```percentile```
+parameter to change the percentile). - "max": For each model the threshold
+value is maximum reconstruction error obtained on the validation data. - You
+can also pass an Integer of Float value. In this case, the threshold value is
+the same for all the models. ```python predictions = aoc.predict(X_test,
+mode="all", threshold="default") ``` ### 6. Evaluate You can use the
+predictions to calculate manually the performance metrics of the model.
+However, the ```evaluate()``` function is a more convenient way to do it. You
+can also use the ```mode``` parameter (works similarly to the ```predict()```
+function) and use metrics from the ```sklearn.metrics``` package (currently
+available are "roc_auc", "accuracy", "precision", "recall", and "f1").
+```python score = aoc.evaluate(X_test, y_test, mode="all", metric="roc_auc",
+threshold="default") ``` ## Usage ```python from autooc.autooc import AutoOC
+aoc = AutoOC(anomaly_class = 0, normal_class = 1, multiobjective=True,
 performance_metric="training_time", algorithm = "autoencoder" ) X_train, X_val,
-X_test, y_test = talos.load_example_data() run = talos.fit( X=X_train,
-X_val=X_val, pop=10, gen=10, experiment_name="test", epochs=1000 ) predictions
-= talos.predict(X_test, mode="all", threshold="default") score = talos.evaluate
-(X_test, y_test, mode="all", metric="roc_auc", threshold="default") ``` _For
-more examples, please refer to the [Documentation](https://example.com)_-->  ##
-Citation To cite this work please use: ``` @article{FERREIRA2022109820, author
-= {LuÃ­s Ferreira and AndrÃ© Pilastri and Filipe Romano and Paulo Cortez},
-title = {Using supervised and one-class automated machine learning for
-predictive maintenance}, journal = {Applied Soft Computing}, volume = {131},
-pages = {109820}, year = {2022}, issn = {1568-4946}, doi = {https://doi.org/
-10.1016/j.asoc.2022.109820}, url = {https://www.sciencedirect.com/science/
-article/pii/S1568494622008699} } ```  ## Roadmap See the [open issues](https://
-github.com/luisferreira97/talos) for a list of proposed features (and known
-issues).  ## Contributing Contributions are what make the open source community
-such an amazing place to be learn, inspire, and create. Any contributions you
-make are **greatly appreciated**. 1. Fork the Project 2. Create your Feature
-Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git
-commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin
-feature/AmazingFeature`) 5. Open a Pull Request  ## License Distributed under
-the MIT License. See `LICENSE` for more information.  ## Contact LuÃ­s Ferreira
-- [LinkedIn](https://www.linkedin.com/in/luisferreira97/) -
+X_test, y_test = aoc.load_example_data() run = aoc.fit( X=X_train, X_val=X_val,
+pop=10, gen=10, experiment_name="test", epochs=1000 ) predictions = aoc.predict
+(X_test, mode="all", threshold="default") score = aoc.evaluate(X_test, y_test,
+mode="all", metric="roc_auc", threshold="default") ``` _For more examples,
+please refer to the [Documentation](https://example.com)_-->  ## Citation To
+cite this work please use: ``` @article{FERREIRA2022109820, author = {LuÃ­s
+Ferreira and AndrÃ© Pilastri and Filipe Romano and Paulo Cortez}, title =
+{Using supervised and one-class automated machine learning for predictive
+maintenance}, journal = {Applied Soft Computing}, volume = {131}, pages =
+{109820}, year = {2022}, issn = {1568-4946}, doi = {https://doi.org/10.1016/
+j.asoc.2022.109820}, url = {https://www.sciencedirect.com/science/article/pii/
+S1568494622008699} } ```  ## Roadmap See the [open issues](https://github.com/
+luisferreira97/AutoOC) for a list of proposed features (and known issues).  ##
+Contributing Contributions are what make the open source community such an
+amazing place to be learn, inspire, and create. Any contributions you make are
+**greatly appreciated**. 1. Fork the Project 2. Create your Feature Branch
+(`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
+-m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
+AmazingFeature`) 5. Open a Pull Request  ## License Distributed under the MIT
+License. See `LICENSE` for more information.  ## Contact LuÃ­s Ferreira -
+[LinkedIn](https://www.linkedin.com/in/luisferreira97/) -
 luis_ferreira223@hotmail.com Project Link: [https://github.com/luisferreira97/
-talos](https://github.com/luisferreira97/talos)  ## Acknowledgements *
+AutoOC](https://github.com/luisferreira97/AutoOC)  ## Acknowledgements *
 [PonyGE2](https://github.com/PonyGE/PonyGE2)   [contributors-shield]: https://
 img.shields.io/github/contributors/othneildrew/Best-README-
 Template.svg?style=for-the-badge [contributors-url]: https://github.com/
-luisferreira97/talos/graphs/contributors [forks-shield]: https://
+luisferreira97/AutoOC/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-
-badge [forks-url]: https://github.com/luisferreira97/talos/network/members
+badge [forks-url]: https://github.com/luisferreira97/AutoOC/network/members
 [stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-
 Template.svg?style=for-the-badge [stars-url]: https://github.com/
-luisferreira97/talos/stargazers [issues-shield]: https://img.shields.io/github/
-issues/othneildrew/Best-README-Template.svg?style=for-the-badge [issues-url]:
-https://github.com/luisferreira97/talos/issues [license-shield]: https://
-img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-
-the-badge [license-url]: https://github.com/luisferreira97/talos/blob/master/
+luisferreira97/AutoOC/stargazers [issues-shield]: https://img.shields.io/
+github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge [issues-
+url]: https://github.com/luisferreira97/AutoOC/issues [license-shield]: https:/
+/img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-
+the-badge [license-url]: https://github.com/luisferreira97/AutoOC/blob/master/
 LICENSE [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-
 black.svg?style=for-the-badge&logo=linkedin&colorB=555 [linkedin-url]: https://
 www.linkedin.com/in/luisferreira97/ [product-screenshot]: images/screenshot.png
```

### Comparing `autooc-0.0.1/setup.py` & `autooc-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="autooc",
-    version="0.0.1",
+    version="0.0.2",
     author_email="luis_ferreira223@hotmail.com",
     author="Luís Ferreira",
     description="AutoOC: Automated Machine Learning (AutoML) library for One-Class Learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/luisferreira97/AutoOC",
@@ -30,14 +30,13 @@
     include_package_data=True,
     #package_dir={"": "src/talos"},
     install_requires=[
         'keras==2.6.0',
         'matplotlib==3.4.1',
         'mlflow==1.15.0',
         'pandas==1.2.4',
-        'pre-commit==2.15.0',
         'scikit-learn==1.0',
         'tensorflow==2.6.0',
         'tensorflow-estimator==2.6.0',
         'tqdm==4.60.0'
     ]
 )
```

### Comparing `autooc-0.0.1/talos/algorithm/distributed_algorithm/search_loop.py` & `autooc-0.0.2/autooc/algorithm/distributed_algorithm/search_loop.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/algorithm/hill_climbing.py` & `autooc-0.0.2/autooc/algorithm/hill_climbing.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/algorithm/mapper.py` & `autooc-0.0.2/autooc/algorithm/mapper.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/algorithm/parameters.py` & `autooc-0.0.2/autooc/algorithm/parameters.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/algorithm/search_loop.py` & `autooc-0.0.2/autooc/algorithm/search_loop.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/algorithm/step.py` & `autooc-0.0.2/autooc/algorithm/step.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/base_ff_classes/base_ff.py` & `autooc-0.0.2/autooc/fitness/base_ff_classes/base_ff.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/base_ff_classes/ff_template.py` & `autooc-0.0.2/autooc/fitness/base_ff_classes/ff_template.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/base_ff_classes/moo_ff.py` & `autooc-0.0.2/autooc/fitness/base_ff_classes/moo_ff.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/evaluation.py` & `autooc-0.0.2/autooc/fitness/evaluation.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/multi_objective/binary_phenotype_to_float.py` & `autooc-0.0.2/autooc/fitness/multi_objective/binary_phenotype_to_float.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/multi_objective/singlefit_autoencoders.py` & `autooc-0.0.2/autooc/fitness/multi_objective/singlefit_autoencoders.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/multi_objective/singlefit_multiobj.py` & `autooc-0.0.2/autooc/fitness/multi_objective/singlefit_multiobj.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/multi_objective/zdt1.py` & `autooc-0.0.2/autooc/fitness/multi_objective/zdt1.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/progsys.py` & `autooc-0.0.2/autooc/fitness/progsys.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/pymax.py` & `autooc-0.0.2/autooc/fitness/pymax.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/sequence_match.py` & `autooc-0.0.2/autooc/fitness/sequence_match.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/string_match.py` & `autooc-0.0.2/autooc/fitness/string_match.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/supervised_learning/boolean_problem.py` & `autooc-0.0.2/autooc/fitness/supervised_learning/boolean_problem.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/supervised_learning/classification.py` & `autooc-0.0.2/autooc/fitness/supervised_learning/classification.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/supervised_learning/if_else_classifier.py` & `autooc-0.0.2/autooc/fitness/supervised_learning/if_else_classifier.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/supervised_learning/regression.py` & `autooc-0.0.2/autooc/fitness/supervised_learning/regression.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/supervised_learning/regression_random_polynomial.py` & `autooc-0.0.2/autooc/fitness/supervised_learning/regression_random_polynomial.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/supervised_learning/supervised_learning.py` & `autooc-0.0.2/autooc/fitness/supervised_learning/supervised_learning.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/fitness/supervised_learning/supervised_learning_backup.py` & `autooc-0.0.2/autooc/fitness/supervised_learning/supervised_learning_backup.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/operators/crossover.py` & `autooc-0.0.2/autooc/operators/crossover.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/operators/initialisation.py` & `autooc-0.0.2/autooc/operators/initialisation.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/operators/mutation.py` & `autooc-0.0.2/autooc/operators/mutation.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/operators/replacement.py` & `autooc-0.0.2/autooc/operators/replacement.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/operators/selection.py` & `autooc-0.0.2/autooc/operators/selection.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/operators/subtree_parse.py` & `autooc-0.0.2/autooc/operators/subtree_parse.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/representation/derivation.py` & `autooc-0.0.2/autooc/representation/derivation.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/representation/grammar.py` & `autooc-0.0.2/autooc/representation/grammar.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/representation/individual.py` & `autooc-0.0.2/autooc/representation/individual.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/representation/latent_tree.py` & `autooc-0.0.2/autooc/representation/latent_tree.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/representation/tree.py` & `autooc-0.0.2/autooc/representation/tree.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/scripts/GE_LR_parser.py` & `autooc-0.0.2/autooc/scripts/GE_LR_parser.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/scripts/baselines.py` & `autooc-0.0.2/autooc/scripts/baselines.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/scripts/experiment_manager.py` & `autooc-0.0.2/autooc/scripts/experiment_manager.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/scripts/grammar_analyser.py` & `autooc-0.0.2/autooc/scripts/grammar_analyser.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/scripts/python_script_evaluation.py` & `autooc-0.0.2/autooc/scripts/python_script_evaluation.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/scripts/stats_parser.py` & `autooc-0.0.2/autooc/scripts/stats_parser.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/stats/stats.py` & `autooc-0.0.2/autooc/stats/stats.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/talos.py` & `autooc-0.0.2/autooc/autooc.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from talos.utilities.algorithm.general import check_python_version
 from talos.utilities.algorithm.initialise_run import initialise_run_params
 from talos.utilities.algorithm.NSGA2 import compute_pareto_metrics
 
 check_python_version()
 
 
-class Talos(object):
+class AutoOC(object):
     def __init__(self, anomaly_class: str, normal_class: str, multiobjective: bool = False, algorithm: str = "all", performance_metric: str = "num_params", multicore: bool = False):
         #self.params = params.copy()
         self.params = params
         self.population = []
         self.population_dict = {}
         self.stats = {}
         self.fitted = False
```

### Comparing `autooc-0.0.1/talos/utilities/algorithm/NSGA2.py` & `autooc-0.0.2/autooc/utilities/algorithm/NSGA2.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/algorithm/command_line_parser.py` & `autooc-0.0.2/autooc/utilities/algorithm/command_line_parser.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/algorithm/initialise_run.py` & `autooc-0.0.2/autooc/utilities/algorithm/initialise_run.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/algorithm/state.py` & `autooc-0.0.2/autooc/utilities/algorithm/state.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/fitness/error_metric.py` & `autooc-0.0.2/autooc/utilities/fitness/error_metric.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/fitness/get_data.py` & `autooc-0.0.2/autooc/utilities/fitness/get_data.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/fitness/math_functions.py` & `autooc-0.0.2/autooc/utilities/fitness/math_functions.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/fitness/optimize_constants.py` & `autooc-0.0.2/autooc/utilities/fitness/optimize_constants.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/representation/check_methods.py` & `autooc-0.0.2/autooc/utilities/representation/check_methods.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/representation/python_filter.py` & `autooc-0.0.2/autooc/utilities/representation/python_filter.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/stats/file_io.py` & `autooc-0.0.2/autooc/utilities/stats/file_io.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/stats/save_plots.py` & `autooc-0.0.2/autooc/utilities/stats/save_plots.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/stats/trackers.py` & `autooc-0.0.2/autooc/utilities/stats/trackers.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.1/talos/utilities/utils.py` & `autooc-0.0.2/autooc/utilities/utils.py`

 * *Files identical despite different names*

