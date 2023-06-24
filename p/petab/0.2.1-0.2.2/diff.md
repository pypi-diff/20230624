# Comparing `tmp/petab-0.2.1.tar.gz` & `tmp/petab-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petab-0.2.1.tar", last modified: Tue May 16 13:17:02 2023, max compression
+gzip compressed data, was "petab-0.2.2.tar", last modified: Sat Jun 24 08:27:13 2023, max compression
```

## Comparing `petab-0.2.1.tar` & `petab-0.2.2.tar`

### file list

```diff
@@ -1,58 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.761197 petab-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-16 13:16:49.000000 petab-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 13:16:49.000000 petab-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-16 13:17:02.761197 petab-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-16 13:16:49.000000 petab-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.749197 petab-0.2.1/petab/
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-05-16 13:16:50.000000 petab-0.2.1/petab/C.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-16 13:16:50.000000 petab-0.2.1/petab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-16 13:16:50.000000 petab-0.2.1/petab/calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-16 13:16:50.000000 petab-0.2.1/petab/composite_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-16 13:16:50.000000 petab-0.2.1/petab/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-05-16 13:16:50.000000 petab-0.2.1/petab/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:16:50.000000 petab-0.2.1/petab/format_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    38465 2023-05-16 13:16:50.000000 petab-0.2.1/petab/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-16 13:16:50.000000 petab-0.2.1/petab/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-05-16 13:16:50.000000 petab-0.2.1/petab/measurements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.757197 petab-0.2.1/petab/models/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 13:16:50.000000 petab-0.2.1/petab/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-16 13:16:50.000000 petab-0.2.1/petab/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-05-16 13:16:50.000000 petab-0.2.1/petab/models/pysb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-16 13:16:50.000000 petab-0.2.1/petab/models/sbml_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-16 13:16:50.000000 petab-0.2.1/petab/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-05-16 13:16:50.000000 petab-0.2.1/petab/parameter_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-05-16 13:16:50.000000 petab-0.2.1/petab/parameters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4855 2023-05-16 13:16:50.000000 petab-0.2.1/petab/petablint.py
--rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-05-16 13:16:50.000000 petab-0.2.1/petab/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-16 13:16:50.000000 petab-0.2.1/petab/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-16 13:16:50.000000 petab-0.2.1/petab/sbml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.757197 petab-0.2.1/petab/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-16 13:16:50.000000 petab-0.2.1/petab/schemas/petab_schema.v1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-16 13:16:50.000000 petab-0.2.1/petab/schemas/petab_schema.v2.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-16 13:16:50.000000 petab-0.2.1/petab/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-16 13:16:50.000000 petab-0.2.1/petab/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 13:16:50.000000 petab-0.2.1/petab/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.761197 petab-0.2.1/petab/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/data_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/plot_data_and_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/plot_residuals.py
--rw-r--r--   0 runner    (1001) docker     (123)    27093 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    36510 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.761197 petab-0.2.1/petab/visualize/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/templates/mystyle.css
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 13:16:50.000000 petab-0.2.1/petab/visualize/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-05-16 13:16:50.000000 petab-0.2.1/petab/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:17:02.757197 petab-0.2.1/petab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 13:17:02.000000 petab-0.2.1/petab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 13:16:50.000000 petab-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:17:02.761197 petab-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-16 13:16:50.000000 petab-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.469408 petab-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-24 08:27:03.000000 petab-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-24 08:27:03.000000 petab-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-24 08:27:13.469408 petab-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-24 08:27:03.000000 petab-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab/
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-06-24 08:27:03.000000 petab-0.2.2/petab/C.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-24 08:27:03.000000 petab-0.2.2/petab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-06-24 08:27:03.000000 petab-0.2.2/petab/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-24 08:27:03.000000 petab-0.2.2/petab/composite_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-24 08:27:03.000000 petab-0.2.2/petab/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-06-24 08:27:03.000000 petab-0.2.2/petab/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-24 08:27:03.000000 petab-0.2.2/petab/format_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38465 2023-06-24 08:27:03.000000 petab-0.2.2/petab/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-24 08:27:03.000000 petab-0.2.2/petab/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-06-24 08:27:03.000000 petab-0.2.2/petab/measurements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-24 08:27:03.000000 petab-0.2.2/petab/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-24 08:27:03.000000 petab-0.2.2/petab/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-06-24 08:27:03.000000 petab-0.2.2/petab/models/pysb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-24 08:27:03.000000 petab-0.2.2/petab/models/sbml_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-24 08:27:03.000000 petab-0.2.2/petab/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-06-24 08:27:03.000000 petab-0.2.2/petab/parameter_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-06-24 08:27:03.000000 petab-0.2.2/petab/parameters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4855 2023-06-24 08:27:03.000000 petab-0.2.2/petab/petablint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-06-24 08:27:03.000000 petab-0.2.2/petab/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-24 08:27:03.000000 petab-0.2.2/petab/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-06-24 08:27:03.000000 petab-0.2.2/petab/sbml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-24 08:27:03.000000 petab-0.2.2/petab/schemas/petab_schema.v1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-24 08:27:03.000000 petab-0.2.2/petab/schemas/petab_schema.v2.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-24 08:27:03.000000 petab-0.2.2/petab/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-24 08:27:03.000000 petab-0.2.2/petab/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-24 08:27:03.000000 petab-0.2.2/petab/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/data_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/plot_data_and_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/plot_residuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27428 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36510 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab/visualize/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/templates/mystyle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-24 08:27:03.000000 petab-0.2.2/petab/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-24 08:27:03.000000 petab-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 08:27:13.469408 petab-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-24 08:27:03.000000 petab-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.469408 petab-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_model_pysb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21256 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_parameter_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24580 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_petab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_sbml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_visualization_data_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_yaml.py
```

### Comparing `petab-0.2.1/LICENSE` & `petab-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/PKG-INFO` & `petab-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab
-Version: 0.2.1
+Version: 0.2.2
 Summary: Parameter estimation tabular data
 Home-page: https://github.com/PEtab-dev/libpetab-python
 Author: The PEtab developers
 Author-email: daniel.weindl@helmholtz-muenchen.de
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `petab-0.2.1/README.md` & `petab-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/C.py` & `petab-0.2.2/petab/C.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/__init__.py` & `petab-0.2.2/petab/__init__.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/calculate.py` & `petab-0.2.2/petab/calculate.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/composite_problem.py` & `petab-0.2.2/petab/composite_problem.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/conditions.py` & `petab-0.2.2/petab/conditions.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/core.py` & `petab-0.2.2/petab/core.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/lint.py` & `petab-0.2.2/petab/lint.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/mapping.py` & `petab-0.2.2/petab/mapping.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/measurements.py` & `petab-0.2.2/petab/measurements.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/models/model.py` & `petab-0.2.2/petab/models/model.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/models/pysb_model.py` & `petab-0.2.2/petab/models/pysb_model.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/models/sbml_model.py` & `petab-0.2.2/petab/models/sbml_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         if sbml_string:
             self.sbml_reader, self.sbml_document, self.sbml_model = \
                 load_sbml_from_string(sbml_string)
 
         self.__dict__.update(state)
 
     @staticmethod
-    def from_file(filepath_or_buffer, model_id: str):
+    def from_file(filepath_or_buffer, model_id: str = None):
         sbml_reader, sbml_document, sbml_model = get_sbml_model(
             filepath_or_buffer)
         return SbmlModel(
             sbml_model=sbml_model,
             sbml_reader=sbml_reader,
             sbml_document=sbml_document,
             model_id=model_id,
```

### Comparing `petab-0.2.1/petab/observables.py` & `petab-0.2.2/petab/observables.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/parameter_mapping.py` & `petab-0.2.2/petab/parameter_mapping.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/parameters.py` & `petab-0.2.2/petab/parameters.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/petablint.py` & `petab-0.2.2/petab/petablint.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/problem.py` & `petab-0.2.2/petab/problem.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/sampling.py` & `petab-0.2.2/petab/sampling.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/sbml.py` & `petab-0.2.2/petab/sbml.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/schemas/petab_schema.v1.0.0.yaml` & `petab-0.2.2/petab/schemas/petab_schema.v1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/schemas/petab_schema.v2.0.0.yaml` & `petab-0.2.2/petab/schemas/petab_schema.v2.0.0.yaml`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/simplify.py` & `petab-0.2.2/petab/simplify.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/simulate.py` & `petab-0.2.2/petab/simulate.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/visualize/__init__.py` & `petab-0.2.2/petab/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/visualize/cli.py` & `petab-0.2.2/petab/visualize/cli.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/visualize/data_overview.py` & `petab-0.2.2/petab/visualize/data_overview.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/visualize/helper_functions.py` & `petab-0.2.2/petab/visualize/helper_functions.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/visualize/lint.py` & `petab-0.2.2/petab/visualize/lint.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/visualize/plot_data_and_simulation.py` & `petab-0.2.2/petab/visualize/plot_data_and_simulation.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/visualize/plot_residuals.py` & `petab-0.2.2/petab/visualize/plot_residuals.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/visualize/plotter.py` & `petab-0.2.2/petab/visualize/plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,16 @@
                 and not measurements_to_plot.data_to_plot.empty:
             # plotting all measurement data
 
             p = None
             if plotTypeData == REPLICATE:
                 replicates = np.stack(
                     measurements_to_plot.data_to_plot.repl.values)
+                if replicates.ndim == 1:
+                    replicates = np.expand_dims(replicates, axis=1)
 
                 # plot first replicate
                 p = ax.plot(
                     measurements_to_plot.conditions,
                     replicates[:, 0],
                     linestyle='-.',
                     marker='x', markersize=10, label=label_base
@@ -540,14 +542,16 @@
             measurements_data_to_plot_inf = \
                 measurements_to_plot.data_to_plot.loc[np.inf]
 
             if plotTypeData == REPLICATE:
                 p = None
                 if plotTypeData == REPLICATE:
                     replicates = measurements_data_to_plot_inf.repl
+                    if replicates.ndim == 0:
+                        replicates = np.expand_dims(replicates, axis=0)
 
                     # plot first replicate
                     p = ax_inf.plot(
                         timepoints_inf,
                         [replicates[0]]*3,
                         linestyle='-.', marker='x', markersize=10,
                         markevery=[1], label=label_base + " simulation",
@@ -583,14 +587,16 @@
         # plot simulations
         if simulations_to_plot is not None and simulations_to_plot.inf_point:
             simulations_data_to_plot_inf = \
                 simulations_to_plot.data_to_plot.loc[np.inf]
 
             if plotTypeData == REPLICATE:
                 replicates = simulations_data_to_plot_inf.repl
+                if replicates.ndim == 0:
+                    replicates = np.expand_dims(replicates, axis=0)
 
                 # plot first replicate
                 p = ax_inf.plot(
                     timepoints_inf,
                     [replicates[0]] * 3,
                     linestyle='-', marker='o', markevery=[1],
                     label=label_base, color=color
```

### Comparing `petab-0.2.1/petab/visualize/plotting.py` & `petab-0.2.2/petab/visualize/plotting.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/visualize/templates/report.html` & `petab-0.2.2/petab/visualize/templates/report.html`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab/yaml.py` & `petab-0.2.2/petab/yaml.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.1/petab.egg-info/PKG-INFO` & `petab-0.2.2/petab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab
-Version: 0.2.1
+Version: 0.2.2
 Summary: Parameter estimation tabular data
 Home-page: https://github.com/PEtab-dev/libpetab-python
 Author: The PEtab developers
 Author-email: daniel.weindl@helmholtz-muenchen.de
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `petab-0.2.1/setup.py` & `petab-0.2.2/setup.py`

 * *Files identical despite different names*

