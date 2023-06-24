# Comparing `tmp/gadapt-0.2.19.tar.gz` & `tmp/gadapt-0.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gadapt-0.2.19.tar", last modified: Sun Jun 18 18:17:44 2023, max compression
+gzip compressed data, was "dist\gadapt-0.2.20.tar", last modified: Sat Jun 24 15:22:50 2023, max compression
```

## Comparing `gadapt-0.2.19.tar` & `gadapt-0.2.20.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.296217 gadapt-0.2.19/
--rw-rw-rw-   0        0        0    22014 2023-06-18 18:17:44.296716 gadapt-0.2.19/PKG-INFO
--rw-rw-rw-   0        0        0    19628 2023-06-18 18:14:25.000000 gadapt-0.2.19/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.180213 gadapt-0.2.19/gadapt/
--rw-rw-rw-   0        0        0       34 2023-06-18 17:04:48.000000 gadapt-0.2.19/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.209214 gadapt-0.2.19/gadapt/cost_finding/
--rw-rw-rw-   0        0        0       64 2023-06-18 16:13:43.000000 gadapt-0.2.19/gadapt/cost_finding/__init__.py
--rw-rw-rw-   0        0        0      783 2023-06-03 19:52:53.000000 gadapt-0.2.19/gadapt/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     2169 2023-06-03 19:53:08.000000 gadapt-0.2.19/gadapt/cost_finding/common_cost_finder.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.213214 gadapt-0.2.19/gadapt/crossover/
--rw-rw-rw-   0        0        0       33 2023-06-18 16:13:59.000000 gadapt-0.2.19/gadapt/crossover/__init__.py
--rw-rw-rw-   0        0        0     7080 2023-06-03 19:52:23.000000 gadapt-0.2.19/gadapt/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1300 2023-06-03 19:52:35.000000 gadapt-0.2.19/gadapt/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.217214 gadapt-0.2.19/gadapt/execution/
--rw-rw-rw-   0        0        0       48 2023-06-18 16:27:33.000000 gadapt-0.2.19/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3302 2023-06-03 20:49:46.000000 gadapt-0.2.19/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.223213 gadapt-0.2.19/gadapt/exit_check/
--rw-rw-rw-   0        0        0       56 2023-06-18 16:29:21.000000 gadapt-0.2.19/gadapt/exit_check/__init__.py
--rw-rw-rw-   0        0        0      379 2023-06-03 19:51:29.000000 gadapt-0.2.19/gadapt/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1113 2023-06-03 19:50:16.000000 gadapt-0.2.19/gadapt/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      365 2023-06-03 19:51:48.000000 gadapt-0.2.19/gadapt/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      449 2023-06-03 19:51:58.000000 gadapt-0.2.19/gadapt/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.225715 gadapt-0.2.19/gadapt/factory/
--rw-rw-rw-   0        0        0       74 2023-06-18 16:31:20.000000 gadapt-0.2.19/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0    10398 2023-06-18 16:54:21.000000 gadapt-0.2.19/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0    26501 2023-06-03 20:44:22.000000 gadapt-0.2.19/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.228714 gadapt-0.2.19/gadapt/ga_logging/
--rw-rw-rw-   0        0        0       26 2023-06-18 16:31:46.000000 gadapt-0.2.19/gadapt/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2188 2023-06-03 19:19:12.000000 gadapt-0.2.19/gadapt/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.241214 gadapt-0.2.19/gadapt/ga_model/
--rw-rw-rw-   0        0        0       33 2023-06-18 16:32:02.000000 gadapt-0.2.19/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     8611 2023-06-03 20:28:37.000000 gadapt-0.2.19/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0      723 2023-06-03 20:31:30.000000 gadapt-0.2.19/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     6427 2023-06-03 20:15:33.000000 gadapt-0.2.19/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     2137 2023-06-03 20:09:38.000000 gadapt-0.2.19/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1472 2023-06-03 20:05:45.000000 gadapt-0.2.19/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0     2704 2023-06-03 20:06:52.000000 gadapt-0.2.19/gadapt/ga_model/genetic_variable.py
--rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.19/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    12730 2023-06-03 20:00:59.000000 gadapt-0.2.19/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0      881 2023-06-03 20:04:36.000000 gadapt-0.2.19/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.245215 gadapt-0.2.19/gadapt/gene_combination/
--rw-rw-rw-   0        0        0       91 2023-06-18 16:44:14.000000 gadapt-0.2.19/gadapt/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      367 2023-06-03 19:46:03.000000 gadapt-0.2.19/gadapt/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0     1102 2023-06-18 16:36:56.000000 gadapt-0.2.19/gadapt/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.247214 gadapt-0.2.19/gadapt/immigration/
--rw-rw-rw-   0        0        0       54 2023-06-18 16:45:34.000000 gadapt-0.2.19/gadapt/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.250214 gadapt-0.2.19/gadapt/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0       69 2023-06-18 16:45:47.000000 gadapt-0.2.19/gadapt/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      676 2023-06-03 19:42:17.000000 gadapt-0.2.19/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      407 2023-06-03 19:43:54.000000 gadapt-0.2.19/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.254215 gadapt-0.2.19/gadapt/immigration/population_immigration/
--rw-rw-rw-   0        0        0       79 2023-06-18 16:46:42.000000 gadapt-0.2.19/gadapt/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      239 2023-06-03 19:44:12.000000 gadapt-0.2.19/gadapt/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0      993 2023-06-03 19:45:35.000000 gadapt-0.2.19/gadapt/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.256215 gadapt-0.2.19/gadapt/mutation/
--rw-rw-rw-   0        0        0       38 2023-06-18 16:47:20.000000 gadapt-0.2.19/gadapt/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.261715 gadapt-0.2.19/gadapt/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0       42 2023-06-18 16:47:50.000000 gadapt-0.2.19/gadapt/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0      956 2023-06-03 19:39:26.000000 gadapt-0.2.19/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
--rw-rw-rw-   0        0        0     3031 2023-06-03 19:37:17.000000 gadapt-0.2.19/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
--rw-rw-rw-   0        0        0     1009 2023-06-03 19:37:53.000000 gadapt-0.2.19/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.267716 gadapt-0.2.19/gadapt/mutation/population_mutation/
--rw-rw-rw-   0        0        0       51 2023-06-18 17:07:55.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-06-03 19:39:16.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/base_population_mutator.py
--rw-rw-rw-   0        0        0     1365 2023-06-03 19:40:00.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/composed_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.271216 gadapt-0.2.19/gadapt/mutation/population_mutation/cost_diversity/
--rw-rw-rw-   0        0        0       56 2023-06-18 17:07:58.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-06-03 19:41:44.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     2045 2023-06-03 19:40:53.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     1130 2023-06-03 19:41:22.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/random_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.275216 gadapt-0.2.19/gadapt/parent_selection/
--rw-rw-rw-   0        0        0       37 2023-06-18 16:59:38.000000 gadapt-0.2.19/gadapt/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      395 2023-06-03 19:27:41.000000 gadapt-0.2.19/gadapt/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0     1172 2023-06-03 19:31:52.000000 gadapt-0.2.19/gadapt/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.281216 gadapt-0.2.19/gadapt/sampling/
--rw-rw-rw-   0        0        0      128 2023-06-18 17:00:39.000000 gadapt-0.2.19/gadapt/sampling/__init__.py
--rw-rw-rw-   0        0        0      793 2023-06-03 19:32:22.000000 gadapt-0.2.19/gadapt/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      534 2023-06-03 19:33:37.000000 gadapt-0.2.19/gadapt/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      512 2023-06-03 19:33:50.000000 gadapt-0.2.19/gadapt/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1954 2023-06-03 19:34:36.000000 gadapt-0.2.19/gadapt/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2717 2023-06-03 19:35:01.000000 gadapt-0.2.19/gadapt/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.284215 gadapt-0.2.19/gadapt/string_operation/
--rw-rw-rw-   0        0        0       90 2023-06-18 17:02:51.000000 gadapt-0.2.19/gadapt/string_operation/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-06-03 20:30:52.000000 gadapt-0.2.19/gadapt/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.288215 gadapt-0.2.19/gadapt/utils/
--rw-rw-rw-   0        0        0      281 2023-06-03 20:30:21.000000 gadapt-0.2.19/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0       35 2023-06-18 17:03:05.000000 gadapt-0.2.19/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     1313 2023-06-03 20:30:37.000000 gadapt-0.2.19/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.290717 gadapt-0.2.19/gadapt/validation/
--rw-rw-rw-   0        0        0       31 2023-06-18 17:03:27.000000 gadapt-0.2.19/gadapt/validation/__init__.py
--rw-rw-rw-   0        0        0      846 2023-06-03 20:29:38.000000 gadapt-0.2.19/gadapt/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    17474 2023-06-03 20:29:54.000000 gadapt-0.2.19/gadapt/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.295216 gadapt-0.2.19/gadapt/variable_update/
--rw-rw-rw-   0        0        0       53 2023-06-18 17:04:05.000000 gadapt-0.2.19/gadapt/variable_update/__init__.py
--rw-rw-rw-   0        0        0      234 2023-06-03 20:28:58.000000 gadapt-0.2.19/gadapt/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2052 2023-06-03 20:29:16.000000 gadapt-0.2.19/gadapt/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.202713 gadapt-0.2.19/gadapt.egg-info/
--rw-rw-rw-   0        0        0    22014 2023-06-18 18:17:44.000000 gadapt-0.2.19/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3180 2023-06-18 18:17:44.000000 gadapt-0.2.19/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 18:17:44.000000 gadapt-0.2.19/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-18 18:17:44.000000 gadapt-0.2.19/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-06-18 18:17:44.298716 gadapt-0.2.19/setup.cfg
--rw-rw-rw-   0        0        0      465 2023-06-18 17:45:52.000000 gadapt-0.2.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.075689 gadapt-0.2.20/
+-rw-rw-rw-   0        0        0    22014 2023-06-24 15:22:50.076189 gadapt-0.2.20/PKG-INFO
+-rw-rw-rw-   0        0        0    19628 2023-06-18 18:14:25.000000 gadapt-0.2.20/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.924689 gadapt-0.2.20/gadapt/
+-rw-rw-rw-   0        0        0       34 2023-06-18 17:04:48.000000 gadapt-0.2.20/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.944688 gadapt-0.2.20/gadapt/cost_finding/
+-rw-rw-rw-   0        0        0       64 2023-06-18 16:13:43.000000 gadapt-0.2.20/gadapt/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0     1283 2023-06-24 14:49:47.000000 gadapt-0.2.20/gadapt/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     2173 2023-06-24 14:49:47.000000 gadapt-0.2.20/gadapt/cost_finding/common_cost_finder.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.949689 gadapt-0.2.20/gadapt/crossover/
+-rw-rw-rw-   0        0        0       33 2023-06-18 16:13:59.000000 gadapt-0.2.20/gadapt/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7304 2023-06-24 14:50:30.000000 gadapt-0.2.20/gadapt/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1325 2023-06-24 13:16:01.000000 gadapt-0.2.20/gadapt/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.951690 gadapt-0.2.20/gadapt/execution/
+-rw-rw-rw-   0        0        0       48 2023-06-18 16:27:33.000000 gadapt-0.2.20/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3547 2023-06-18 20:10:51.000000 gadapt-0.2.20/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.958189 gadapt-0.2.20/gadapt/exit_check/
+-rw-rw-rw-   0        0        0       56 2023-06-18 16:29:21.000000 gadapt-0.2.20/gadapt/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      506 2023-06-24 14:40:03.000000 gadapt-0.2.20/gadapt/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1341 2023-06-24 14:35:53.000000 gadapt-0.2.20/gadapt/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      469 2023-06-24 14:40:21.000000 gadapt-0.2.20/gadapt/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      516 2023-06-24 14:41:55.000000 gadapt-0.2.20/gadapt/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.960689 gadapt-0.2.20/gadapt/factory/
+-rw-rw-rw-   0        0        0       74 2023-06-18 16:31:20.000000 gadapt-0.2.20/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0    10157 2023-06-24 14:43:21.000000 gadapt-0.2.20/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0    27186 2023-06-18 20:13:29.000000 gadapt-0.2.20/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.962690 gadapt-0.2.20/gadapt/ga_logging/
+-rw-rw-rw-   0        0        0       26 2023-06-18 16:31:46.000000 gadapt-0.2.20/gadapt/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2188 2023-06-03 19:19:12.000000 gadapt-0.2.20/gadapt/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.981689 gadapt-0.2.20/gadapt/ga_model/
+-rw-rw-rw-   0        0        0       33 2023-06-18 16:32:02.000000 gadapt-0.2.20/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     9007 2023-06-24 14:52:04.000000 gadapt-0.2.20/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0      723 2023-06-03 20:31:30.000000 gadapt-0.2.20/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     6470 2023-06-18 19:03:50.000000 gadapt-0.2.20/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     2198 2023-06-18 19:04:11.000000 gadapt-0.2.20/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1488 2023-06-18 19:04:24.000000 gadapt-0.2.20/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0     2873 2023-06-18 19:16:48.000000 gadapt-0.2.20/gadapt/ga_model/genetic_variable.py
+-rw-rw-rw-   0        0        0       81 2023-06-18 19:04:47.000000 gadapt-0.2.20/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    12752 2023-06-18 19:43:36.000000 gadapt-0.2.20/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0      902 2023-06-19 11:38:06.000000 gadapt-0.2.20/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.987190 gadapt-0.2.20/gadapt/gene_combination/
+-rw-rw-rw-   0        0        0       91 2023-06-18 16:44:14.000000 gadapt-0.2.20/gadapt/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      367 2023-06-03 19:46:03.000000 gadapt-0.2.20/gadapt/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0     1102 2023-06-18 16:36:56.000000 gadapt-0.2.20/gadapt/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.989189 gadapt-0.2.20/gadapt/immigration/
+-rw-rw-rw-   0        0        0       54 2023-06-18 16:45:34.000000 gadapt-0.2.20/gadapt/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.993689 gadapt-0.2.20/gadapt/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0       69 2023-06-18 16:45:47.000000 gadapt-0.2.20/gadapt/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      677 2023-06-18 19:20:05.000000 gadapt-0.2.20/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      407 2023-06-03 19:43:54.000000 gadapt-0.2.20/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.003190 gadapt-0.2.20/gadapt/immigration/population_immigration/
+-rw-rw-rw-   0        0        0       79 2023-06-18 16:46:42.000000 gadapt-0.2.20/gadapt/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0      239 2023-06-03 19:44:12.000000 gadapt-0.2.20/gadapt/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0      993 2023-06-24 14:50:25.000000 gadapt-0.2.20/gadapt/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.005189 gadapt-0.2.20/gadapt/mutation/
+-rw-rw-rw-   0        0        0       38 2023-06-18 16:47:20.000000 gadapt-0.2.20/gadapt/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.011689 gadapt-0.2.20/gadapt/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:47:50.000000 gadapt-0.2.20/gadapt/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0     1115 2023-06-18 19:26:41.000000 gadapt-0.2.20/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
+-rw-rw-rw-   0        0        0     3033 2023-06-19 11:44:21.000000 gadapt-0.2.20/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
+-rw-rw-rw-   0        0        0     1009 2023-06-03 19:37:53.000000 gadapt-0.2.20/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.019689 gadapt-0.2.20/gadapt/mutation/population_mutation/
+-rw-rw-rw-   0        0        0       51 2023-06-18 17:07:55.000000 gadapt-0.2.20/gadapt/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-06-24 14:50:25.000000 gadapt-0.2.20/gadapt/mutation/population_mutation/base_population_mutator.py
+-rw-rw-rw-   0        0        0     1365 2023-06-03 19:40:00.000000 gadapt-0.2.20/gadapt/mutation/population_mutation/composed_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.021690 gadapt-0.2.20/gadapt/mutation/population_mutation/cost_diversity/
+-rw-rw-rw-   0        0        0       56 2023-06-18 17:07:58.000000 gadapt-0.2.20/gadapt/mutation/population_mutation/cost_diversity/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-06-03 19:41:44.000000 gadapt-0.2.20/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     2047 2023-06-19 11:44:41.000000 gadapt-0.2.20/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     1130 2023-06-03 19:41:22.000000 gadapt-0.2.20/gadapt/mutation/population_mutation/random_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.025692 gadapt-0.2.20/gadapt/parent_selection/
+-rw-rw-rw-   0        0        0       37 2023-06-18 16:59:38.000000 gadapt-0.2.20/gadapt/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-06-03 19:27:41.000000 gadapt-0.2.20/gadapt/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0     1174 2023-06-19 11:45:22.000000 gadapt-0.2.20/gadapt/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.032189 gadapt-0.2.20/gadapt/sampling/
+-rw-rw-rw-   0        0        0      128 2023-06-18 17:00:39.000000 gadapt-0.2.20/gadapt/sampling/__init__.py
+-rw-rw-rw-   0        0        0      793 2023-06-03 19:32:22.000000 gadapt-0.2.20/gadapt/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      530 2023-06-19 11:37:03.000000 gadapt-0.2.20/gadapt/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      508 2023-06-19 11:36:47.000000 gadapt-0.2.20/gadapt/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1954 2023-06-03 19:34:36.000000 gadapt-0.2.20/gadapt/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2725 2023-06-19 11:46:50.000000 gadapt-0.2.20/gadapt/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.036689 gadapt-0.2.20/gadapt/string_operation/
+-rw-rw-rw-   0        0        0       90 2023-06-18 17:02:51.000000 gadapt-0.2.20/gadapt/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-06-03 20:30:52.000000 gadapt-0.2.20/gadapt/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.040189 gadapt-0.2.20/gadapt/utils/
+-rw-rw-rw-   0        0        0      281 2023-06-03 20:30:21.000000 gadapt-0.2.20/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0       35 2023-06-18 17:03:05.000000 gadapt-0.2.20/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1313 2023-06-03 20:30:37.000000 gadapt-0.2.20/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.071189 gadapt-0.2.20/gadapt/validation/
+-rw-rw-rw-   0        0        0       31 2023-06-18 17:03:27.000000 gadapt-0.2.20/gadapt/validation/__init__.py
+-rw-rw-rw-   0        0        0      846 2023-06-03 20:29:38.000000 gadapt-0.2.20/gadapt/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    17474 2023-06-03 20:29:54.000000 gadapt-0.2.20/gadapt/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:50.074689 gadapt-0.2.20/gadapt/variable_update/
+-rw-rw-rw-   0        0        0       53 2023-06-18 17:04:05.000000 gadapt-0.2.20/gadapt/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      234 2023-06-03 20:28:58.000000 gadapt-0.2.20/gadapt/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2052 2023-06-03 20:29:16.000000 gadapt-0.2.20/gadapt/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:22:49.941689 gadapt-0.2.20/gadapt.egg-info/
+-rw-rw-rw-   0        0        0    22014 2023-06-24 15:22:49.000000 gadapt-0.2.20/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-06-24 15:22:49.000000 gadapt-0.2.20/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 15:22:49.000000 gadapt-0.2.20/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 15:22:49.000000 gadapt-0.2.20/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-06-24 15:22:50.077688 gadapt-0.2.20/setup.cfg
+-rw-rw-rw-   0        0        0      465 2023-06-24 15:22:38.000000 gadapt-0.2.20/setup.py
```

### Comparing `gadapt-0.2.19/PKG-INFO` & `gadapt-0.2.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.2.19
+Version: 0.2.20
 Summary: GAdapt: A Python Library for Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 License: UNKNOWN
 Description: # GAdapt: Self-Adaptive Genetic Algorithm
         [GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
```

### Comparing `gadapt-0.2.19/README.md` & `gadapt-0.2.20/README.md`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/cost_finding/common_cost_finder.py` & `gadapt-0.2.20/gadapt/cost_finding/common_cost_finder.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 class CommonCostFinder(BaseCostFinder):
 
     """
     Common class for cost finding
     """
 
-    def find_costs_for_chromosome(self, population: Population):
+    def find_costs_for_population(self, population: Population):
         if (population is None):
             raise Exception("population must not be null!")
         chromosomes_for_execution: List[Chromosome] = [
             c for c in population if (math.isnan(c.cost_value)) or (c.is_immigrant and c.population_generation == population.population_generation)]
         for c in chromosomes_for_execution:
             self.execute_function(population.options.cost_function, c)        
         better_chromosomes: List[Chromosome] = population.get_sorted(key=lambda x: x.cost_value)[:
             population.options.keep_number]        
         population.best_individual = better_chromosomes[0]       
         population.min_cost = (min(
             better_chromosomes, key=lambda x: x.cost_value)).cost_value
         better_chromosomes_without_immigrants = better_chromosomes[:population.options.keep_number - population.options.immigration_number]
         population.avg_cost = sum(
             [c.cost_value for c in better_chromosomes_without_immigrants]) / len(better_chromosomes_without_immigrants)
-        self.log_population(population)
+        self._log_population(population)
         population.clear_and_add_chromosomes(better_chromosomes)
         population.update_variables()
-        self.cost_found_first_time(population, better_chromosomes)
+        self._cost_found_first_time(population, better_chromosomes)
         
-    def cost_found_first_time(self, population: Population, better_chromosomes: List[Chromosome] ):
+    def _cost_found_first_time(self, population: Population, better_chromosomes: List[Chromosome] ):
         if math.isnan(population.first_cost):
             population.first_cost = ga_utils.average([c.cost_value for c in better_chromosomes])
             population.population_mutator.after_first_execution(population)
 
-    def log_population(self, population: Population):
+    def _log_population(self, population: Population):
         if population.options.logging:
             logging.info(str(population))
```

### Comparing `gadapt-0.2.19/gadapt/crossover/base_crossover.py` & `gadapt-0.2.20/gadapt/crossover/base_crossover.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,100 +6,93 @@
 import gadapt.utils.ga_utils as ga_utils
 import gadapt.ga_model.definitions as definitions
 
 class BaseCrossover:
 
     """
     Base Crossover Class
-    """
     
-    def __init__(self, gene_combination: BaseGeneCombination, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator):
+    Parameters
+    ------------
+        gene_combination: BaseGeneCombination
+            the algorithm for how genes are to be combined
+        mutator: BaseChromosomeMutator
+            mutation algorithm to be passed to offspring chromosomes
+        immigrator: BaseChromosomeImmigrator
+            immigration algorithm to be passed to offspring chromosomes
+        mutation_on_both_sides: bool
+            indicates if offspring chromosomes should be mutated on both sides with the same probability
+    """
+    def __init__(self, gene_combination: BaseGeneCombination, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator, mutation_on_both_sides: bool = True):
         self._mutation_on_both_sides = True
-        self.gene_combination = gene_combination
-        self.mutator = mutator
-        self.immigrator = immigrator
-    
-    @property
-    def gene_combination(self) -> BaseGeneCombination:
-        return self._gene_combination
-    
-    @gene_combination.setter
-    def gene_combination(self, value: BaseGeneCombination):
-        self._gene_combination = value
-
-    @property
-    def mutator(self) -> BaseChromosomeMutator:
-        return self._mutator
-    
-    @mutator.setter
-    def mutator(self, value: BaseChromosomeMutator):
-        self._mutator = value
-
-    @property
-    def immigrator(self) -> BaseChromosomeImmigrator:
-        return self._immigrator
-    
-    @immigrator.setter
-    def immigrator(self, value: BaseChromosomeImmigrator):
-        self._immigrator = value
-
-    
-    @property
-    def mutation_on_both_sides(self) -> bool:
-        return self._mutation_on_both_sides
-    
-    @mutation_on_both_sides.setter
-    def mutation_on_both_sides(self, value: bool):
-        self._mutation_on_both_sides = value    
+        self._gene_combination = gene_combination
+        self._mutator = mutator
+        self._immigrator = immigrator
+        self._mutation_on_both_sides = mutation_on_both_sides
+  
     
     def mate(self, mother: Chromosome, father: Chromosome, population_generation: int):
+        """ Returns two offspring chromosomes using parents' genetic material
+        
+        Parameters
+        ------------
+            mother: Chromosome
+                The first chromosome for mating
+            father: Chromosome
+                The second chromosome for mating
+            population_generation: int
+                Current generation in the population
+
+        Return
+        -----------
+            offspring1 : Chromosome
+                the first offspring chromosome
+            offspring2 : Chromosome
+                the second offspring chromosome
+        """
         def get_genetic_diversity(g_m: Gene, g_f: Gene) -> float:
             return abs(g_m.variable_value - g_f.variable_value) / (g_f.genetic_variable.max_value - g_f.genetic_variable.min_value)
 
-        self.mate_init()
         if (len(mother) != len(father)):
             raise Exception("Mother and father must have the same number of genes!")
-        offspring1 = Chromosome(self.mutator, self.immigrator, population_generation)
-        offspring2 = Chromosome(self.mutator, self.immigrator, population_generation)
+        offspring1 = Chromosome(self._mutator, self._immigrator, population_generation)
+        offspring2 = Chromosome(self._mutator, self._immigrator, population_generation)
         self.number_of_genes = len(father)
         genetic_diversity = []
-        for self.current_gene_number in range(self.number_of_genes):
-            mother_gene, father_gene = self.get_mother_father_genes(mother, father)
+        for self._current_gene_number in range(self.number_of_genes):
+            mother_gene, father_gene = self._get_mother_father_genes(mother, father)
             self.genetic_variable_father = father_gene.genetic_variable
             genetic_variable_mother = mother_gene.genetic_variable
             if (self.genetic_variable_father != genetic_variable_mother):
                 genetic_variable_mother = next((item.genetic_variable for item in mother if item.genetic_variable == self.genetic_variable), None)
             if (genetic_variable_mother is None):
                 raise Exception("chromosomes in crossover do not have the same structure!")
             genetic_diversity.append(get_genetic_diversity(mother_gene, father_gene))
-            var1, var2 = self.combine(mother_gene, father_gene)
+            var1, var2 = self._combine(mother_gene, father_gene)
             offspring1.add_gene(self.genetic_variable_father, var1)
             offspring2.add_gene(self.genetic_variable_father, var2)
         parrents_diversity = round(ga_utils.average(genetic_diversity), 2)
         offspring1.parent_diversity = parrents_diversity
         offspring2.parent_diversity = parrents_diversity
-        offspring1.mutation_on_both_sides = self.mutation_on_both_sides
-        offspring2.mutation_on_both_sides = self.mutation_on_both_sides
+        offspring1.mutation_on_both_sides = self._mutation_on_both_sides
+        offspring2.mutation_on_both_sides = self._mutation_on_both_sides
         offspring1.mother_id = mother.chromosome_id
         offspring2.mother_id = mother.chromosome_id
         offspring1.father_id = father.chromosome_id
         offspring2.father_id = father.chromosome_id
-        self.increase_generation(offspring1, offspring2, mother, father)
+        self._increase_generation(offspring1, offspring2, mother, father)
         return offspring1, offspring2
-    
-    def mate_init(self):
-        pass
 
-    def get_mother_father_genes(self, mother: Chromosome, father: Chromosome):
+    def _get_mother_father_genes(self, mother: Chromosome, father: Chromosome):
         raise Exception(definitions.NOT_IMPLEMENTED)
 
-    def combine(self, mother_gene: Gene, father_gene: Gene):
+    def _combine(self, mother_gene: Gene, father_gene: Gene):
         raise Exception(definitions.NOT_IMPLEMENTED)
     
-    def increase_generation(self, offspring1: Chromosome, offspring2: Chromosome, mother: Chromosome, father: Chromosome):
+    def _increase_generation(self, offspring1: Chromosome, offspring2: Chromosome, mother: Chromosome, father: Chromosome):
         current_generation = mother.chromosome_generation
         if current_generation == 0 or current_generation < father.chromosome_generation:
             current_generation = father.chromosome_generation
         current_generation += 1
         offspring1.chromosome_generation = current_generation 
         offspring2.chromosome_generation = current_generation
```

### Comparing `gadapt-0.2.19/gadapt/crossover/uniform_crossover.py` & `gadapt-0.2.20/gadapt/crossover/uniform_crossover.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from gadapt.immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
 from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
 from gadapt.gene_combination.base_gene_combination import BaseGeneCombination
 
 class UniformCrossover(BaseCrossover):
 
     """
-    Uniform Crossover
+    Uniform Crossover.
+    Genes from parents' chromosomes are combined in a uniform way
     """
     
     def __init__(self, var_combination: BaseGeneCombination, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator):
         super(UniformCrossover, self).__init__(var_combination, mutator, immigrator)
-        self.gene_combination = var_combination
     
-    def get_mother_father_genes(self, mother: Chromosome, father: Chromosome):
-        father_gene = father[self.current_gene_number]
-        mother_gene = mother[self.current_gene_number]
+    def _get_mother_father_genes(self, mother: Chromosome, father: Chromosome):
+        father_gene = father[self._current_gene_number]
+        mother_gene = mother[self._current_gene_number]
         return mother_gene, father_gene
     
-    def combine(self, mother_gene: Gene, father_gene: Gene):
-        if self.gene_combination is None:
+    def _combine(self, mother_gene: Gene, father_gene: Gene):
+        if self._gene_combination is None:
             raise Exception("gene_combination must not be null!")
-        return self.gene_combination.combine(mother_gene, father_gene)
+        return self._gene_combination.combine(mother_gene, father_gene)
```

### Comparing `gadapt-0.2.19/gadapt/execution/ga_executor.py` & `gadapt-0.2.20/gadapt/execution/ga_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,33 @@
 from gadapt.ga_model.population import Population
 import gadapt.ga_model.message_levels as message_levels
 
 class GAExecutor:
 
     """
     Executor for the genetic algorithm
+    
+    Parameters
+    ------------
+        ga_options: GAOptions
+            Options for GA execution
+        factory: GAFactory
+            Factory for objects creation
     """
 
     def __init__(self, ga_options: GAOptions, factory: GAFactory) -> None:
         if (not ga_options is None):
             self.ga_options = ga_options    
         self.factory = factory          
 
 
     def execute(self) -> GAResults:
+        """
+        Executes the genetic algorithm
+        """
         results = GAResults()
         try: 
             init_logging(self.ga_options.logging)                           
         except Exception as ex:
             results.messages.append((message_levels.WARNING, "Logging failed. Error message: {exc}".format(exc=str(ex))))
             self.ga_options.logging = False        
         try:
```

### Comparing `gadapt-0.2.19/gadapt/exit_check/base_exit_checker.py` & `gadapt-0.2.20/gadapt/exit_check/base_exit_checker.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from datetime import datetime
 import gadapt.ga_model.definitions as definitions
 
 class BaseExitChecker:
 
     """
     Base class for exit check
+    Parameters
+    ------------
+        max_attempt_no: int
+            Maximal number of attempts with no improvement, for the given criteria.
+            After this number of attempts with no improvements, the GA exits
     """
 
     def __init__(self, max_attempt_no: int) -> None:
         self.max_attempt_no = max_attempt_no
         self.attempt_no = 0              
     
     @property
@@ -21,18 +26,18 @@
         self._attempt_no = value
 
     def check(self, population):
         time_diff = (datetime.now() - population.start_time).total_seconds()
         if time_diff >= population.options.timeout:
             population.timeout_expired = True
             return True
-        if self.is_exit(population):
+        if self._is_exit(population):
             self.attempt_no += 1
         else:
             self.attempt_no = 0
         if self.attempt_no >= self.max_attempt_no:
             logging.info("function exit.")
             return True
         return False
     
-    def is_exit(self, population) -> bool:
+    def _is_exit(self, population) -> bool:
         raise Exception(definitions.NOT_IMPLEMENTED)
```

### Comparing `gadapt-0.2.19/gadapt/factory/ga_factory.py` & `gadapt-0.2.20/gadapt/factory/ga_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,32 +33,16 @@
 
 
 class GAFactory:
     """
     Factory for creating  class instances based on GA options
     """
     def __init__(self, ga, options: GAOptions) -> None:
-        self.ga = ga
-        self.options = options
-
-    @property
-    def ga(self):
-        return self._ga
-
-    @ga.setter
-    def ga(self, value):
-        self._ga = value
-
-    @property
-    def options(self):
-        return self._options
-
-    @options.setter
-    def options(self, value):
-        self._options = value
+        self._ga = ga
+        self._options = options
 
     def get_cost_finder(self) -> BaseCostFinder:
         """
         Cost Finder instance
         """
         return CommonCostFinder()
 
@@ -74,100 +58,100 @@
         """
         return RandomChromosomeImmigrator()
 
     def get_chromosome_mutator(self) -> BaseChromosomeMutator:
         """
         Chromosome Mutator Instance
         """
-        if self.ga.chromosome_mutation.strip() == definitions.CROSS_DIVERSITY:
-            return CrossDiversityChromosomeMutator(self.get_sampling_method(self.ga.cross_diversity_mutation_gene_selection))
-        elif self.ga.chromosome_mutation.strip() == definitions.RANDOM:
+        if self._ga.chromosome_mutation.strip() == definitions.CROSS_DIVERSITY:
+            return CrossDiversityChromosomeMutator(self._get_sampling_method(self._ga.cross_diversity_mutation_gene_selection))
+        elif self._ga.chromosome_mutation.strip() == definitions.RANDOM:
             return RandomChromosomeMutator()
         else:
             raise Exception("unknown chromosome mutation")
 
-    def population_mutator_options_validation(self):
+    def _population_mutator_options_validation(self):
         """
         Validates population mutator options
         """
-        mutator_strings = self.ga.population_mutation.split(definitions.PARAM_SEPARATOR)
+        mutator_strings = self._ga.population_mutation.split(definitions.PARAM_SEPARATOR)
         for s in mutator_strings:
             if not s.strip() in definitions.POPULATION_MUTATOR_STRINGS:
                 raise Exception(s + " is not defined as option for population mutation")
 
     def get_population_mutator(self, population_mutator_string=None) -> BasePopulationMutator:
         """
         Population Mutator Instance
         """
-        self.population_mutator_options_validation()
+        self._population_mutator_options_validation()
         if population_mutator_string is None:
-            population_mutator_string = self.ga.population_mutation.strip()
+            population_mutator_string = self._ga.population_mutation.strip()
         if population_mutator_string.find(definitions.PARAM_SEPARATOR) > -1:
             return self.get_population_mutator_combined()
         elif population_mutator_string == definitions.COST_DIVERSITY:
-            return CostDiversityPopulationMutator(self.options, ParentDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options))
+            return CostDiversityPopulationMutator(self._options, ParentDiversityPopulationMutator(self._get_sampling_method(self._ga.parent_diversity_mutation_chromosome_selection), self._options))
         elif population_mutator_string == definitions.PARENT_DIVERSITY:
-            return ParentDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options)
+            return ParentDiversityPopulationMutator(self._get_sampling_method(self._ga.parent_diversity_mutation_chromosome_selection), self._options)
         elif population_mutator_string == definitions.RANDOM:
-            return RandomPopulationMutator(self.options)
+            return RandomPopulationMutator(self._options)
         else:
             raise Exception("unknown population mutation")
 
     def get_population_mutator_combined(self) -> ComposedPopulationMutator:
         """
         Population Mutator Instance - combined
         """
-        mutator_strings = [ms.strip() for ms in self.ga.population_mutation.split(definitions.PARAM_SEPARATOR)]
-        if (self.is_cost_diversity_random(mutator_strings)):
-            return CostDiversityPopulationMutator(self.options, RandomPopulationMutator(self.options))
-        if (self.is_cost_diversity_parent_diversity(mutator_strings)):
-            return CostDiversityPopulationMutator(self.options, ParentDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options))
-        if self.is_cost_diversity_parent_diversity_random(mutator_strings):
-            composedPopulationMutator = ComposedPopulationMutator(self.options)
-            composedPopulationMutator.append(ParentDiversityPopulationMutator(self.get_sampling_method(
-                self.ga.parent_diversity_mutation_chromosome_selection), self.options))
+        mutator_strings = [ms.strip() for ms in self._ga.population_mutation.split(definitions.PARAM_SEPARATOR)]
+        if (self._is_cost_diversity_random(mutator_strings)):
+            return CostDiversityPopulationMutator(self._options, RandomPopulationMutator(self._options))
+        if (self._is_cost_diversity_parent_diversity(mutator_strings)):
+            return CostDiversityPopulationMutator(self._options, ParentDiversityPopulationMutator(self._get_sampling_method(self._ga.parent_diversity_mutation_chromosome_selection), self._options))
+        if self._is_cost_diversity_parent_diversity_random(mutator_strings):
+            composedPopulationMutator = ComposedPopulationMutator(self._options)
+            composedPopulationMutator.append(ParentDiversityPopulationMutator(self._get_sampling_method(
+                self._ga.parent_diversity_mutation_chromosome_selection), self._options))
             composedPopulationMutator.append(
-                RandomPopulationMutator(self.options))
-            return CostDiversityPopulationMutator(self.options, composedPopulationMutator)
-        composedPopulationMutator = ComposedPopulationMutator(self.options)
+                RandomPopulationMutator(self._options))
+            return CostDiversityPopulationMutator(self._options, composedPopulationMutator)
+        composedPopulationMutator = ComposedPopulationMutator(self._options)
         for ms in mutator_strings:
             composedPopulationMutator.append(self.get_population_mutator(ms))
         return composedPopulationMutator
 
-    def is_cost_diversity_random(self, mutator_strings: list):
+    def _is_cost_diversity_random(self, mutator_strings: list):
         """
         Is population mutator cost diversity and random
         """
         if len(mutator_strings) == 2 and definitions.COST_DIVERSITY in mutator_strings and definitions.RANDOM in mutator_strings:
             return True
         return False
 
-    def is_cost_diversity_parent_diversity(self, mutator_strings: list):
+    def _is_cost_diversity_parent_diversity(self, mutator_strings: list):
         """
         Is population mutator cost diversity and parent diversity
         """
         if len(mutator_strings) == 2 and definitions.COST_DIVERSITY in mutator_strings and definitions.PARENT_DIVERSITY in mutator_strings:
             return True
         return False
 
-    def is_cost_diversity_parent_diversity_random(self, mutator_strings: list):
+    def _is_cost_diversity_parent_diversity_random(self, mutator_strings: list):
         """
         Is population mutator cost diversity, parent diversity and random
         """
         if len(mutator_strings) == 3 and definitions.COST_DIVERSITY in mutator_strings and definitions.PARENT_DIVERSITY in mutator_strings and definitions.RANDOM in mutator_strings:
             return True
         return False
 
     def get_parent_selector(self) -> BaseParentSelector:
         """
         Parent Selector Instance
         """
-        return SamplingParentSelector(self.get_sampling_method(self.ga.parent_selection))
+        return SamplingParentSelector(self._get_sampling_method(self._ga.parent_selection))
 
-    def get_sampling_method(self, str) -> BaseSampling:
+    def _get_sampling_method(self, str) -> BaseSampling:
         """
         Sampling Methos Instance
         """
         str_value = str
         sampling_method_strings = str.split(definitions.PARAM_SEPARATOR)
         other_value = None
         if len(sampling_method_strings) > 1:
@@ -190,19 +174,19 @@
         """
         return BlendingGeneCombination()
 
     def get_exit_checker(self) -> BaseExitChecker:
         """
         Exit Checker Instance
         """
-        if self.ga.exit_check == definitions.AVG_COST:
-            return AvgCostExitChecker(self.ga.max_attempt_no)
-        if self.ga.exit_check == definitions.MIN_COST:
-            return MinCostExitChecker(self.ga.max_attempt_no)
-        return RequestedCostExitChecker(self.ga.requested_cost)
+        if self._ga.exit_check == definitions.AVG_COST:
+            return AvgCostExitChecker(self._ga.max_attempt_no)
+        if self._ga.exit_check == definitions.MIN_COST:
+            return MinCostExitChecker(self._ga.max_attempt_no)
+        return RequestedCostExitChecker(self._ga.requested_cost)
 
     def get_crossover(self, gene_combination: BaseGeneCombination, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator) -> BaseCrossover:
         """
         Crossover Instance
         """
         return UniformCrossover(gene_combination, mutator, immigrator)
```

### Comparing `gadapt-0.2.19/gadapt/ga.py` & `gadapt-0.2.20/gadapt/ga.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+"""
+The main genetic algorithm module
+"""
 import sys
 from gadapt.execution.ga_executor import GAExecutor
 from gadapt.factory.ga_factory import GAFactory
 from gadapt.ga_model.genetic_variable import GeneticVariable
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.ga_model.ga_results import GAResults
 from gadapt.ga_model.population import Population
 import gadapt.utils.ga_utils as ga_utils
 import gadapt.ga_model.definitions as definitions
 from gadapt.validation.common_options_validator import CommonOptionsValidator
 
 class GA:
-    """The main genetic algorithm class"""
+    """
+    The main genetic algorithm class
+    """
 
 
     def __init__(self,
                  cost_function = None,
                  population_size = 64, 
                  exit_check = definitions.AVG_COST,
                  requested_cost = sys.float_info.max,
@@ -31,70 +36,90 @@
                  cross_diversity_mutation_gene_selection = definitions.ROULETTE_WHEEL,
                  immigration_number = 0,                                                                                   
                  logging = False,                                                              
                  timeout = 120
                  ) -> None:                     
         """
         The constructor of the GA class accepts all parameters required to create an instance of the GA class. It validates such parameters.
-
-        cost_function: Custom function for the cost calculation (fitness). The optimisation goal is minimising the output of the cost function. 
-        cost_function must be the function with one argument - a dictionary of values, where the key is an index (the ordinal of adding parameters) and the key is the parameter's value to be optimised.
-        When adding parameters, there should be as many parameters as the function uses. The cost_function is the only mandatory parameter.
-        
-        population_size: Number of chromosomes in the population.
-        
-        exit_check:  A criteria for the exit for the genetic algorithm
-        
-        requested_cost: This parameter only takes place when exit_check has value “requested”. It determines the requested value which causes the exit from the genetic algorithm
-        
-        max_attempt_no: This parameter only takes place when exit_check has value “avg_cost” or “min_cost”. It determines the number of generations in which there is no improvement in the average/minimal cost.
-        
-        parent_selection: The algorithm for parent selection.
-        
-        population_mutation: A type of mutation for the entire population.
-        Based on the value of this parameter, the number of mutation chromosomes can be determined, along with how chromosomes for the mutation will be selected.
-        
-        number_of_mutation_chromosomes: The number of mutation chromosomes in the population. 
-        In case it's value is equal to or higher than 0, it overrides percentage_of_mutation_chromosomes.
-        This value is the upper bound - the actual number of mutated chromosomes can vary from 1 to number_of_mutation_chromosomes.
-        
-        percentage_of_mutation_chromosomes:  The percentage of mutated chromosomes in the population.
-        This value is applied to the population_size value and rounded to an integer value, giving the number of mutation chromosomes.
-        For example, if population_size has a value of 32, and percentage_of_mutation_chromosomes has a value of 10, the number of mutation chromosomes will be 3.
-        The calculated value is an upper bound - the actual number of mutated chromosomes can vary from 1 to the calculated value.
-        percentage_of_mutation_chromosomes only applies if number_of_mutation_chromosomes does not have a valid integer value equal to or higher than 0.
-        
-        parent_diversity_mutation_chromosome_selection: The selection algorithm for mutating chromosomes when population_mutation contains value “parent_diversity”.
-        It only applies when population_mutation has value “parent_diversity”. It determines the way how chromosomes are to be selected based on the diversity of their parents.
-        
-        must_mutate_for_same_parents:  Indicates if completely the same parents must influence mutation for their children.
-        In other words, each child will be mutated if it has parents with a diversity value of 0.
-        If must_mutate_for_same_parents has the value True, the number of mutated chromosomes can outreach value determined by number_of_mutation_chromosomes or percentage_of_mutation_chromosomes
-        
-        chromosome_mutation: The type of mutation of genes in chromosomes.
-        
-        number_of_mutation_genes: The number of mutated genes in each chromosome.
-        In case it's value is equal to or higher than 0, it overrides percentage_of_mutation_genes.
-        This value is the upper bound - the number of mutated genes can vary from 1 to number_of_mutation_genes.
-        
-        percentage_of_mutation_genes: The percentage of mutated genes in each chromosome.
-        It applies to the chromosome size (number of genes in each chromosome), and the calculated value rounds to an integer value.
-        The calculated value is the upper bound - the actual number of mutated genes can vary from 1 to the calculated value.
-        percentage_of_mutation_genes only applies if number_of_mutations_genes does not have a valid integer value equal to or higher than 0.
-        
-        cross_diversity_mutation_gene_selection: The selection algorithm for mutating chromosomes when chromosome_mutation has value “cross_diversity”.
-        It only applies when chromosome_mutation has value “cross_diversity” . It determines the way how genes are to be selected based on the cross-diversity.
-        
-        immigration_number: Refers to the “Random Immigrants” concepts. This strategy introduces a certain number of individuals into the population during the evolution process.
-        These new individuals are generated randomly and injected into the population.
-        
-        logging:  If this parameter has a True value, the log file will be created in the current working directory.
-        The log file contains the flow of genetic algorithm execution, along with values of chromosomes, genes and cost functions in each generation
         
-        timeout: A number of seconds after which the genetic algorithm optimisation will exit, regardless of whether exit_check criteria is reached.
+        Parameters
+        ------------
+            cost_function
+                Custom function for the cost calculation (fitness). The optimisation goal is minimising the output of the cost function. 
+                cost_function must be the function with one argument - a dictionary of values, where the key is an index (the ordinal of adding parameters) and the key is the parameter's value to be optimised.
+                When adding parameters, there should be as many parameters as the function uses. The cost_function is the only mandatory parameter.
+            
+            population_size
+                Number of chromosomes in the population.
+            
+            exit_check
+                A criteria for the exit for the genetic algorithm
+            
+            requested_cost
+                This parameter only takes place when exit_check has value “requested”. It determines the requested value which causes the exit from the genetic algorithm
+            
+            max_attempt_no
+                This parameter only takes place when exit_check has value “avg_cost” or “min_cost”. It determines the number of generations in which there is no improvement in the average/minimal cost.
+            
+            parent_selection
+                The algorithm for parent selection.
+            
+            population_mutation
+                A type of mutation for the entire population.
+                Based on the value of this parameter, the number of mutation chromosomes can be determined, along with how chromosomes for the mutation will be selected.
+            
+            number_of_mutation_chromosomes
+                The number of mutation chromosomes in the population. 
+                In case it's value is equal to or higher than 0, it overrides percentage_of_mutation_chromosomes.
+                This value is the upper bound - the actual number of mutated chromosomes can vary from 1 to number_of_mutation_chromosomes.
+            
+            percentage_of_mutation_chromosomes
+                The percentage of mutated chromosomes in the population.
+                This value is applied to the population_size value and rounded to an integer value, giving the number of mutation chromosomes.
+                For example, if population_size has a value of 32, and percentage_of_mutation_chromosomes has a value of 10, the number of mutation chromosomes will be 3.
+                The calculated value is an upper bound - the actual number of mutated chromosomes can vary from 1 to the calculated value.
+                percentage_of_mutation_chromosomes only applies if number_of_mutation_chromosomes does not have a valid integer value equal to or higher than 0.
+            
+            parent_diversity_mutation_chromosome_selection
+                The selection algorithm for mutating chromosomes when population_mutation contains value “parent_diversity”.
+                It only applies when population_mutation has value “parent_diversity”. It determines the way how chromosomes are to be selected based on the diversity of their parents.
+            
+            must_mutate_for_same_parents
+                Indicates if completely the same parents must influence mutation for their children.
+                In other words, each child will be mutated if it has parents with a diversity value of 0.
+                If must_mutate_for_same_parents has the value True, the number of mutated chromosomes can outreach value determined by number_of_mutation_chromosomes or percentage_of_mutation_chromosomes
+            
+            chromosome_mutation
+                The type of mutation of genes in chromosomes.
+            
+            number_of_mutation_genes
+                The number of mutated genes in each chromosome.
+                In case it's value is equal to or higher than 0, it overrides percentage_of_mutation_genes.
+                This value is the upper bound - the number of mutated genes can vary from 1 to number_of_mutation_genes.
+            
+            percentage_of_mutation_genes
+                The percentage of mutated genes in each chromosome.
+                It applies to the chromosome size (number of genes in each chromosome), and the calculated value rounds to an integer value.
+                The calculated value is the upper bound - the actual number of mutated genes can vary from 1 to the calculated value.
+                percentage_of_mutation_genes only applies if number_of_mutations_genes does not have a valid integer value equal to or higher than 0.
+            
+            cross_diversity_mutation_gene_selection
+                The selection algorithm for mutating chromosomes when chromosome_mutation has value “cross_diversity”.
+                It only applies when chromosome_mutation has value “cross_diversity” . It determines the way how genes are to be selected based on the cross-diversity.
+            
+            immigration_number
+                Refers to the “Random Immigrants” concepts. This strategy introduces a certain number of individuals into the population during the evolution process.
+                These new individuals are generated randomly and injected into the population.
+            
+            logging
+                If this parameter has a True value, the log file will be created in the current working directory.
+                The log file contains the flow of genetic algorithm execution, along with values of chromosomes, genes and cost functions in each generation
+            
+            timeout
+                A number of seconds after which the genetic algorithm optimisation will exit, regardless of whether exit_check criteria is reached.
         """
         self.cost_function = cost_function
         self.population_size = population_size
         self.exit_check = exit_check 
         self.requested_cost = requested_cost 
         self.max_attempt_no = max_attempt_no
         self.parent_selection = parent_selection
@@ -243,17 +268,17 @@
     
     @property
     def population_mutation(self) -> str:
         """
         A type of mutation for the entire population.
         
         Supported values:
-            - “cost_diversity” - It applies to the number of mutation chromosomes. “cost_diversity” determines the number of mutated chromosomes adaptively, using the diversity of costs in the population. Lower cost diversity means a higher number of mutated chromosomes. The minimal value of mutated chromosomes is 0, and the maximal value is determined by the value of number_of_mutation_chromosomes or percentage_of_mutation_chromosomes parameters. If population_mutation has a value other than “cost_diversity”, the number of mutation chromosomes is a random value from 1 to number_of_mutation_chromosomes value (or to value determined by percentage_of_mutation_chromosomes value). “cost_diversity” means that the “parent_diversity” method is selected to select chromosomes to be mutated. This method only determines the number of mutated chromosomes, but not how chromosomes are selected for the mutation.
-            - “parent_diversity” - It applies to the way how mutation chromosomes will be selected. “parent_diversity” selects chromosomes to be mutated using the diversity of their parents. The more similar parents (lower parent diversity) mean a higher probability of mutation for the child. Based on the calculated parent diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the parent_diversity_mutation_chromosome_selection parameter.
-            - “random” - It applies to the number of mutation chromosomes and to the way how mutation chromosomes will be selected. “random” selects chromosomes to be mutated randomly, and randomly determines the number of mutated chromosomes (with the upper bound of number_of_mutation_chromosomes)
+            “cost_diversity” - It applies to the number of mutation chromosomes. “cost_diversity” determines the number of mutated chromosomes adaptively, using the diversity of costs in the population. Lower cost diversity means a higher number of mutated chromosomes. The minimal value of mutated chromosomes is 0, and the maximal value is determined by the value of number_of_mutation_chromosomes or percentage_of_mutation_chromosomes parameters. If population_mutation has a value other than “cost_diversity”, the number of mutation chromosomes is a random value from 1 to number_of_mutation_chromosomes value (or to value determined by percentage_of_mutation_chromosomes value). “cost_diversity” means that the “parent_diversity” method is selected to select chromosomes to be mutated. This method only determines the number of mutated chromosomes, but not how chromosomes are selected for the mutation.
+            “parent_diversity” - It applies to the way how mutation chromosomes will be selected. “parent_diversity” selects chromosomes to be mutated using the diversity of their parents. The more similar parents (lower parent diversity) mean a higher probability of mutation for the child. Based on the calculated parent diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the parent_diversity_mutation_chromosome_selection parameter.
+            “random” - It applies to the number of mutation chromosomes and to the way how mutation chromosomes will be selected. “random” selects chromosomes to be mutated randomly, and randomly determines the number of mutated chromosomes (with the upper bound of number_of_mutation_chromosomes)
         """
         return self._population_mutation
 
     @population_mutation.setter
     def population_mutation(self, value: str):
         self._population_mutation = ga_utils.prepare_string(value)
```

### Comparing `gadapt-0.2.19/gadapt/ga_logging/logging_settings.py` & `gadapt-0.2.20/gadapt/ga_logging/logging_settings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/ga_model/chromosome.py` & `gadapt-0.2.20/gadapt/ga_model/chromosome.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Chromosome
+"""
 from typing import List
 from gadapt.ga_model.gene import Gene
 from gadapt.ga_model.genetic_variable import GeneticVariable
 from gadapt.ga_model.ranking_model import RankingModel
 from gadapt.immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
 from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
 import gadapt.ga_model.definitions as definitions
@@ -13,65 +16,70 @@
     Chromosome is a part of the Population. Chromosome consists of Genes
     """
     
     def __init__(self, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator, population_generation: int):
         super().__init__()
         self._mutator = mutator
         self._immigrator = immigrator
-        self.cost_value = definitions.FLOAT_NAN
+        self._cost_value = definitions.FLOAT_NAN
         self._is_immigrant = False
-        self.population_generation = population_generation
+        self._population_generation = population_generation
         self._chromosome_id = None
         self._mutated_variables_id_list = []
-        self.first_mutant_generation = 0
-        self.first_immigrant_generation = 0
-        self.last_mutant_generation = 0
-        self.last_immigrant_generation = 0
+        self._first_mutant_generation = 0
+        self._first_immigrant_generation = 0
+        self._last_mutant_generation = 0
+        self._last_immigrant_generation = 0
         self._chromosome_string = None
         self._mother_id = -1
-        self.father_id = -1
+        self._father_id = -1
         self._is_mutated = False
         self._is_immigrant = False
-        self.genes = []
+        self._genes = []
         
     def __str__(self):
-        return self.get_chromosome_string()
+        return self._get_chromosome_string()
     
     def __getitem__(self, index):
-        return self.genes[index]
+        return self._genes[index]
 
     def __next__(self):
-        return next(self.genes)
+        return next(self._genes)
 
     def __len__(self):
-        return len(self.genes)
+        return len(self._genes)
 
-    def get_sorted(self, key: None = None, reverse: bool = False):
-        return sorted(self.genes, key=key, reverse=reverse)
+    def _get_sorted(self, key: None = None, reverse: bool = False):
+        return sorted(self._genes, key=key, reverse=reverse)
 
     def append(self, g: Gene):
         """
         Appends a new gene into the chromosom
         """
-        self.genes.append(g)
+        self._genes.append(g)
 
     def clear(self):
         """
         Clears all genes from the chromosome
         """
-        self.genes.clear()
+        self._genes.clear()
 
     def to_string(self):
+        """
+        Converts the chromosome to the string
+        """
         return ga_strings.chromosome_to_string(self)
+    
+    def set_chromosome_string_none(self):
+        """
+        Sets the chromosome string to None
+        """
+        self._chromosome_string  = None 
 
-    def set_chromosome_string(self, value: str):
-        if value is None:
-           self._chromosome_string  = None 
-
-    def get_chromosome_string(self):
+    def _get_chromosome_string(self):
         if self._chromosome_string is None:
             self._chromosome_string = self.to_string()
         return self._chromosome_string
 
     @property
     def mutator(self) -> BaseChromosomeMutator:
         """
@@ -168,14 +176,17 @@
         return self._father_id
     
     @father_id.setter
     def father_id(self, value: int):
         self._father_id = value
 
     def add_gene(self, gen_var: GeneticVariable, gen_var_value: float = definitions.FLOAT_NAN):
+        """
+        Adds a gene to the chromosome
+        """
         g = Gene(gen_var, gen_var_value)
         self.append(g)
 
     @property
     def parent_diversity(self) -> float:
         """
         Diversity of parents
@@ -255,17 +266,20 @@
 
     @property
     def mutation_on_both_sides(self) -> bool:
         """
         Indicates if mutation should be applied on both sides
         """
         return self._mutation_on_both_sides
-    
+        
     @mutation_on_both_sides.setter
     def mutation_on_both_sides(self, value: bool):
+        """
+        Indicates if mutation of the chromosome shouls be applied with the same probability of lower and higher value comparing with the current value
+        """
         self._mutation_on_both_sides = value
 
     @property
     def succ(self) -> bool:   
         """
         Indicates if cost function execution succeded
         """
```

### Comparing `gadapt-0.2.19/gadapt/ga_model/definitions.py` & `gadapt-0.2.20/gadapt/ga_model/definitions.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/ga_model/ga_options.py` & `gadapt-0.2.20/gadapt/ga_model/ga_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""
+Genetic algorithm options
+"""
 from typing import List
 from gadapt.ga_model.genetic_variable import GeneticVariable
 class GAOptions():
    
     """
-    Genetic algorithm options
+    Genetic algorithm options class
     """
     
     def __init__(self, ga) -> None:
         super().__init__()           
         self._population_size = ga.population_size
         self._cost_function = ga.cost_function                
         self._immigration_number = ga.immigration_number
```

### Comparing `gadapt-0.2.19/gadapt/ga_model/ga_results.py` & `gadapt-0.2.20/gadapt/ga_model/ga_results.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""
+Results for the genetic algorithm execution
+"""
 import gadapt.string_operation.ga_strings as ga_strings
 
 class GAResults:
 
     """
-    Results for the genetic algorithm execution
+    Results class for the genetic algorithm execution
     """
 
     def __init__(self) -> None:
         self._success = True
         self.result_values = {}
         self._messages = []
```

### Comparing `gadapt-0.2.19/gadapt/ga_model/gene.py` & `gadapt-0.2.20/gadapt/ga_model/gene.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Gene
+"""
 import math
 from gadapt.ga_model.genetic_variable import GeneticVariable
 from gadapt.ga_model.ranking_model import RankingModel
 import gadapt.string_operation.ga_strings as ga_strings
 import gadapt.ga_model.definitions as definitions
 class Gene(RankingModel):
```

### Comparing `gadapt-0.2.19/gadapt/ga_model/genetic_variable.py` & `gadapt-0.2.20/gadapt/ga_model/genetic_variable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,111 @@
+"""
+Genetic variable
+"""
 import random
 import gadapt.ga_model.definitions as definitions
 class GeneticVariable:
 
     """
     Genetic variable class defines genes.
-    It contains common values for genes: variable id, maximal value, minimal value, step.
+    Each gene has a reference to one genetic variable.
+    Genetic variable contains common values for genes: variable id, maximal value, minimal value, step.
     """
     
     def __init__(self, id: int) -> None:
         self.variable_id = id
         self._standard_deviation = definitions.FLOAT_NAN
     
     def __eq__(self, other):
         if not isinstance(other, GeneticVariable):
             return False
         return self.variable_id == other.variable_id
     
     def __hash__(self) -> int:
         return self.variable_id
     
+    """
+    Unique ID for genetic variable
+    """
     @property
     def variable_id(self) -> int:
         return self._variable_id
     
     @variable_id.setter
     def variable_id(self, value: int):
         self._variable_id = value
-    
-    @property
-    def variable_name(self) -> str:
-        return self._variable_name
-    
-    @variable_name.setter
-    def variable_name(self, value: str):
-        self._variable_name = value
-
-    @property
-    def initial_value(self) -> float:
-        return self._initial_value
-    
-    @initial_value.setter
-    def initial_value(self, value: float):
-        self._initial_value = value
 
+    """
+    Max gene value
+    """
     @property
     def max_value(self) -> float:
         return self._max_value
     
     @max_value.setter
     def max_value(self, value: float):
         self._max_value = value
 
+    """
+    Min gene value
+    """
     @property
     def min_value(self) -> float:
         return self._min_value
     
     @min_value.setter
     def min_value(self, value: float):
         self._min_value = value
 
+    """
+    Optimization step
+    """
     @property
     def step(self) -> float:
         return self._step
     
     @step.setter
     def step(self, value: float):
-        self._decimal_places = self.get_decimal_places(value)
+        self._decimal_places = self._get_decimal_places(value)
         self._step = value
 
-    def get_decimal_places(self, f: float) -> int:
+    def _get_decimal_places(self, f: float) -> int:
         dp = str(f)[::-1].find('.')
         if dp == -1:
             return 0
         return dp
 
+    """
+    Number of decimal places of the gene value
+    """
     @property
     def decimal_places(self) -> int:
         return self._decimal_places
 
+    """
+    Indicates if all genes have the same value for the same genetic variable
+    """
     @property
     def stacked(self) -> bool:
         return self._stacked
     
     @stacked.setter
     def stacked(self, value: bool):
         self._stacked = value
 
+    """
+    Relative standard deviation of all genes for the same genetic variable
+    """
     @property
     def relative_standard_deviation(self) -> float:
         return self._standard_deviation
     
     @relative_standard_deviation.setter
     def relative_standard_deviation(self, value: float):
         self._standard_deviation = value        
 
+    """
+    Make random value for the gene
+    """
     def make_random_value(self):
         number_of_steps = random.randint(0, round((self.max_value - self.min_value) / self.step))
         return self.min_value + number_of_steps * self.step
```

### Comparing `gadapt-0.2.19/gadapt/ga_model/population.py` & `gadapt-0.2.20/gadapt/ga_model/population.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Population
+"""
 from typing import List, Tuple
 from gadapt.exit_check.base_exit_checker import BaseExitChecker
 from gadapt.cost_finding.base_cost_finder import BaseCostFinder
 from gadapt.crossover.base_crossover import BaseCrossover
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.ga_model.gene import Gene
@@ -352,15 +355,15 @@
 
     def find_costs(self):
         """
         Finds costs for chromosomes
         """
         self.previous_avg_cost = self.avg_cost
         self.previous_min_cost = self.min_cost
-        self.cost_finder.find_costs_for_chromosome(self)
+        self.cost_finder.find_costs_for_population(self)
 
     def clear(self):
         """
         Clears all chromosomes
         """
         self.chromosomes.clear()
```

### Comparing `gadapt-0.2.19/gadapt/ga_model/ranking_model.py` & `gadapt-0.2.20/gadapt/ga_model/ranking_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Ranking model
+"""
 import gadapt.ga_model.definitions as definitions
 class RankingModel:
 
     """
     Base class for the object that can be ranked (chromosomes and genes)
     """
 
@@ -21,14 +24,14 @@
     def cummulative_probability(self):
         return self._cummulative_probability
     
     @cummulative_probability.setter
     def cummulative_probability(self, value):
         self._cummulative_probability = value
 
-    def replace_rank(self, rank):
+    def set_rank(self, rank):
         self.rank = rank
         return self
 
     def reset_for_sampling(self):
         self._rank = -1
         self._cummulative_probability = definitions.FLOAT_NAN
```

### Comparing `gadapt-0.2.19/gadapt/gene_combination/blending_gene_combination.py` & `gadapt-0.2.20/gadapt/gene_combination/blending_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py` & `gadapt-0.2.20/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     def chromosome_immigrated(self, c):
         c.is_immigrant = True
         if c.first_immigrant_generation == 0:
             c.first_immigrant_generation += 1
         c.last_immigrant_generation = 1
         c.first_mutant_generation = 0
         c.last_mutant_generation = 0
-        c.set_chromosome_string(None)
+        c.set_chromosome_string_none()
```

### Comparing `gadapt-0.2.19/gadapt/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.2.20/gadapt/immigration/population_immigration/common_population_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py` & `gadapt-0.2.20/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     """
     Base class for the mutation of chromosome.
     Mutates specific genes in the chromosome.
     """ 
     
     def mutate(self, c, number_of_mutation_genes: int):
+        """
+        Mutates genes in the chromosome.
+        Number of mutated genes is determined by the parameter "number_of_mutation_genes"
+        """
         self.before_mutated(c)
         self.mutate_chromosome(c, number_of_mutation_genes)
         self.chromosome_mutated(c)
     
     def mutate_chromosome(self, c, number_of_mutation_genes: int):
         raise Exception(definitions.NOT_IMPLEMENTED)
```

### Comparing `gadapt-0.2.19/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py` & `gadapt-0.2.20/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,25 @@
                     
     """
     Class for the mutation of chromosome based on cross diversity.
     """ 
     
     def __init__(self, sampling: BaseSampling) -> None:
         super().__init__()
-        self.sampling = sampling
+        self._sampling = sampling
     
     def mutate_chromosome(self, c: Chromosome, number_of_mutation_genes: int):
         if number_of_mutation_genes == 0:
             return
         x_genes = [g for g in c]
         x_genes.sort(key = lambda g: -g.genetic_variable.relative_standard_deviation)   
         if number_of_mutation_genes > len(x_genes):
             number_of_mutation_genes = len(x_genes)
         number_of_mutation_genes = random.randint(1, number_of_mutation_genes)
-        genes_for_mutation = self.sampling.get_sample(x_genes, number_of_mutation_genes, lambda g: g.genetic_variable.relative_standard_deviation)        
+        genes_for_mutation = self._sampling.get_sample(x_genes, number_of_mutation_genes, lambda g: g.genetic_variable.relative_standard_deviation)        
         for g in genes_for_mutation:
             self.make_mutation(g, c)        
     
     def make_random_value_below(self, g: Gene):
         if g.variable_value == g.genetic_variable.min_value:
             return g.genetic_variable.make_random_value()
         number_of_steps = random.randint(0, round((g.variable_value - g.genetic_variable.min_value) / g.genetic_variable.step))
```

### Comparing `gadapt-0.2.19/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py` & `gadapt-0.2.20/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/mutation/population_mutation/base_population_mutator.py` & `gadapt-0.2.20/gadapt/mutation/population_mutation/base_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/mutation/population_mutation/composed_population_mutator.py` & `gadapt-0.2.20/gadapt/mutation/population_mutation/composed_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py` & `gadapt-0.2.20/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py` & `gadapt-0.2.20/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     """
     Population mutator based on parent diversity
     """
         
     def __init__(self, sampling: BaseSampling, options: GAOptions) -> None:
         super().__init__(options)
-        self.sampling = sampling
+        self._sampling = sampling
             
     def sort_key_parent_diversity_random(self, c: Chromosome):
         return (c.parent_diversity, random.random())      
     
     def mutate_population(self, population, number_of_mutation_chromosomes):
         if population is None:
             raise Exception("Population must not be null")
@@ -30,11 +30,11 @@
         chromosomes_for_mutation_count = len(chromosomes_for_mutation)
         rest_number = number_of_mutation_chromosomes - chromosomes_for_mutation_count
         if rest_number > 0:
             if self.options.must_mutate_for_same_parents:
                 chromosomes_for_mutation = [c for c in unallocated_chromosomes if (not c.parent_diversity == 0)]
             else:
                 chromosomes_for_mutation = [c for c in unallocated_chromosomes]
-            chromosomes_for_mutation = self.sampling.get_sample(chromosomes_for_mutation, rest_number, lambda c: c.parent_diversity)       
+            chromosomes_for_mutation = self._sampling.get_sample(chromosomes_for_mutation, rest_number, lambda c: c.parent_diversity)       
         for c in chromosomes_for_mutation:
             c.mutate(self.options.number_of_mutation_genes)
         return len(chromosomes_for_mutation)
```

### Comparing `gadapt-0.2.19/gadapt/mutation/population_mutation/random_population_mutator.py` & `gadapt-0.2.20/gadapt/mutation/population_mutation/random_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/parent_selection/sampling_parent_selector.py` & `gadapt-0.2.20/gadapt/parent_selection/sampling_parent_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
     In this case sampling depends on cost value.
 
     Selects mates for mating from the population
     """
     
     def __init__(self, sampling: BaseSampling) -> None:
         super().__init__()
-        self.sampling = sampling
+        self._sampling = sampling
 
     def select_mates(self, population) -> List[Tuple[Chromosome, Chromosome]]:
-        working_chromosomes = self.sampling.get_sample(
+        working_chromosomes = self._sampling.get_sample(
             population.chromosomes, len(population), lambda c: c.cost_value)
         list_of_mates: List[Tuple[Chromosome, Chromosome]] = []
         while len(working_chromosomes) > 1:
             c1 = working_chromosomes.pop(0)
             c2 = working_chromosomes.pop(0)
             list_of_mates.append((c1, c2))
         return list_of_mates
```

### Comparing `gadapt-0.2.19/gadapt/sampling/base_sampling.py` & `gadapt-0.2.20/gadapt/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/sampling/from_top_to_bottom_sampling.py` & `gadapt-0.2.20/gadapt/sampling/from_top_to_bottom_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 
     """
     "From Top To Bottom" algorithm for extracting a sample from the population.
     """
 
     def prepare_sample(self, lst: List[RankingModel]) -> List[RankingModel]:
         members_for_action = sorted(lst, key=self.sort_key)
-        return [m.replace_rank(rank) for rank, m in enumerate(members_for_action[:self.max_num])]
+        return [m.set_rank(rank) for rank, m in enumerate(members_for_action[:self.max_num])]
```

### Comparing `gadapt-0.2.19/gadapt/sampling/roulette_wheel_sampling.py` & `gadapt-0.2.20/gadapt/sampling/roulette_wheel_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/sampling/tournament_sampling.py` & `gadapt-0.2.20/gadapt/sampling/tournament_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,23 @@
     def __init__(self, group_size = None) -> None:
         super().__init__()
         self.group_size = group_size
     
     def prepare_sample(self, lst: List[RankingModel]) -> List[RankingModel]:
         ls = []
         ls = sorted(lst, key=self.sort_key)
-        groups = self.get_groups(ls)
-        self.play_tournament(groups, self.sort_key)
-        return self.make_ranking(groups)
+        groups = self._get_groups(ls)
+        self._play_tournament(groups, self.sort_key)
+        return self._make_ranking(groups)
     
-    def get_groups(self, lst: List[RankingModel]) -> List[List[RankingModel]]:
+    def _get_groups(self, lst: List[RankingModel]) -> List[List[RankingModel]]:
         size = len(lst)
         ls = [rm for rm in lst]
         if self.group_size is None or self.group_size > len(ls):
-            self.group_size = self.calculate_group_size(ls)
+            self.group_size = self._calculate_group_size(ls)
         num_of_groups = size // self.group_size
         #if size % self.group_size > 0:
         #    num_of_groups += 1
         groups = []
         for i in range(num_of_groups):
             l: list[RankingModel] = []
             groups.append(l)
@@ -41,30 +41,30 @@
                     break
             if len(ls) == 0:
                 break
         if len(ls) > 0:
             groups.append(ls)
         return groups
     
-    def calculate_group_size(self, ls: List[RankingModel]):
+    def _calculate_group_size(self, ls: List[RankingModel]):
         size = len(ls)
         if size <= 3:
             return len(ls)
         group_size = 2
         if size >= 9:
             group_size += 1
         if size >= 12:
             group_size += 1
         return group_size
 
-    def play_tournament(self, groups: List[List[RankingModel]], sort_key):
+    def _play_tournament(self, groups: List[List[RankingModel]], sort_key):
         for g in groups:
             g.sort(key=sort_key)
 
-    def make_ranking(self,  groups: List[List[RankingModel]]):
+    def _make_ranking(self,  groups: List[List[RankingModel]]):
         rank = 0
         members_for_action = []
         number_of_groups = len(groups)
         while rank < self.max_num:
             number_of_empty_groups = 0
             for g in groups:
                 if len(g) == 0:
```

### Comparing `gadapt-0.2.19/gadapt/string_operation/ga_strings.py` & `gadapt-0.2.20/gadapt/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/utils/ga_utils.py` & `gadapt-0.2.20/gadapt/utils/ga_utils.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/validation/base_options_validator.py` & `gadapt-0.2.20/gadapt/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/validation/common_options_validator.py` & `gadapt-0.2.20/gadapt/validation/common_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt/variable_update/common_variable_updater.py` & `gadapt-0.2.20/gadapt/variable_update/common_variable_updater.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.19/gadapt.egg-info/PKG-INFO` & `gadapt-0.2.20/gadapt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.2.19
+Version: 0.2.20
 Summary: GAdapt: A Python Library for Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 License: UNKNOWN
 Description: # GAdapt: Self-Adaptive Genetic Algorithm
         [GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
```

### Comparing `gadapt-0.2.19/gadapt.egg-info/SOURCES.txt` & `gadapt-0.2.20/gadapt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

