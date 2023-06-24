# Comparing `tmp/mlpf-0.0.6.tar.gz` & `tmp/mlpf-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpf-0.0.6.tar", last modified: Tue Jun 20 17:12:45 2023, max compression
+gzip compressed data, was "mlpf-0.0.7.tar", last modified: Sat Jun 24 21:34:24 2023, max compression
```

## Comparing `mlpf-0.0.6.tar` & `mlpf-0.0.7.tar`

### file list

```diff
@@ -1,111 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.858739 mlpf-0.0.6/
--rw-rw-rw-   0        0        0      121 2023-06-19 13:08:07.000000 mlpf-0.0.6/CHANGELOG.md
--rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.6/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4394 2023-06-20 17:12:45.858739 mlpf-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3779 2023-06-20 17:11:47.000000 mlpf-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.794703 mlpf-0.0.6/examples/
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.794703 mlpf-0.0.6/examples/data/
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.812711 mlpf-0.0.6/examples/data/analysis/
--rw-rw-rw-   0        0        0     1390 2023-06-20 15:43:08.000000 mlpf-0.0.6/examples/data/analysis/describe_grid.py
--rw-rw-rw-   0        0        0     1238 2023-06-20 15:43:08.000000 mlpf-0.0.6/examples/data/analysis/describe_node.py
--rw-rw-rw-   0        0        0     1332 2023-06-20 15:43:08.000000 mlpf-0.0.6/examples/data/analysis/grid_pdf_estimates.py
--rw-rw-rw-   0        0        0     1249 2023-06-20 15:43:08.000000 mlpf-0.0.6/examples/data/analysis/node_pdf_estimates.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.812711 mlpf-0.0.6/examples/data/generate/
--rw-rw-rw-   0        0        0     1085 2023-06-20 15:43:08.000000 mlpf-0.0.6/examples/data/generate/uniform.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.794703 mlpf-0.0.6/examples/sklearn/
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.812711 mlpf-0.0.6/examples/sklearn/loss/
--rw-rw-rw-   0        0        0      966 2023-06-20 15:43:08.000000 mlpf-0.0.6/examples/sklearn/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.812711 mlpf-0.0.6/examples/sklearn/supervised_power_flow/
--rw-rw-rw-   0        0        0     2985 2023-06-20 13:03:26.000000 mlpf-0.0.6/examples/sklearn/supervised_power_flow/linear_regression.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.802978 mlpf-0.0.6/examples/torch/
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.812711 mlpf-0.0.6/examples/torch/loss/
--rw-rw-rw-   0        0        0     1091 2023-06-20 15:43:08.000000 mlpf-0.0.6/examples/torch/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.812711 mlpf-0.0.6/examples/torch/supervised_power_flow/
--rw-rw-rw-   0        0        0     5287 2023-06-20 13:18:24.000000 mlpf-0.0.6/examples/torch/supervised_power_flow/gcn.py
--rw-rw-rw-   0        0        0     4525 2023-06-20 13:15:42.000000 mlpf-0.0.6/examples/torch/supervised_power_flow/mlp.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.812711 mlpf-0.0.6/mlpf/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.829722 mlpf-0.0.6/mlpf/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.829722 mlpf-0.0.6/mlpf/data/analysis/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.838827 mlpf-0.0.6/mlpf/data/analysis/description/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/analysis/description/__init__.py
--rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/analysis/description/describe.py
--rw-rw-rw-   0        0        0     1447 2023-06-20 15:43:08.000000 mlpf-0.0.6/mlpf/data/analysis/description/describe_grid.py
--rw-rw-rw-   0        0        0     1396 2023-06-20 15:43:08.000000 mlpf-0.0.6/mlpf/data/analysis/description/describe_node.py
--rw-rw-rw-   0        0        0     6433 2023-06-20 15:43:08.000000 mlpf-0.0.6/mlpf/data/analysis/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.838827 mlpf-0.0.6/mlpf/data/analysis/visualization/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/analysis/visualization/__init__.py
--rw-rw-rw-   0        0        0     3420 2023-06-20 15:43:08.000000 mlpf-0.0.6/mlpf/data/analysis/visualization/grid_pdf_estimates.py
--rw-rw-rw-   0        0        0     3473 2023-06-20 15:43:08.000000 mlpf-0.0.6/mlpf/data/analysis/visualization/node_pdf_estimates.py
--rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/analysis/visualization/visualize.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.844735 mlpf-0.0.6/mlpf/data/conversion/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.6/mlpf/data/conversion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.844735 mlpf-0.0.6/mlpf/data/conversion/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.6/mlpf/data/conversion/numpy/__init__.py
--rw-rw-rw-   0        0        0     1788 2023-06-20 14:41:06.000000 mlpf-0.0.6/mlpf/data/conversion/numpy/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.844735 mlpf-0.0.6/mlpf/data/conversion/torch/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.6/mlpf/data/conversion/torch/__init__.py
--rw-rw-rw-   0        0        0     1360 2023-06-20 14:41:06.000000 mlpf-0.0.6/mlpf/data/conversion/torch/power_flow.py
--rw-rw-rw-   0        0        0      475 2023-06-20 14:41:06.000000 mlpf-0.0.6/mlpf/data/conversion/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.844735 mlpf-0.0.6/mlpf/data/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.844735 mlpf-0.0.6/mlpf/data/data/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/data/numpy/__init__.py
--rw-rw-rw-   0        0        0     4001 2023-06-20 14:41:06.000000 mlpf-0.0.6/mlpf/data/data/numpy/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.844735 mlpf-0.0.6/mlpf/data/data/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/data/torch/__init__.py
--rw-rw-rw-   0        0        0     4033 2023-06-20 14:41:06.000000 mlpf-0.0.6/mlpf/data/data/torch/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.844735 mlpf-0.0.6/mlpf/data/generate/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/generate/__init__.py
--rw-rw-rw-   0        0        0     3523 2023-06-20 15:43:08.000000 mlpf-0.0.6/mlpf/data/generate/generate_uniform_data.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.844735 mlpf-0.0.6/mlpf/data/loading/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/loading/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-06-20 14:41:06.000000 mlpf-0.0.6/mlpf/data/loading/load_data.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.844735 mlpf-0.0.6/mlpf/data/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/utils/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/utils/masks.py
--rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/utils/pandapower_networks.py
--rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/data/utils/saving.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.844735 mlpf-0.0.6/mlpf/enumerations/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/enumerations/__init__.py
--rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/enumerations/branch_table.py
--rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/enumerations/bus_table.py
--rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/enumerations/bus_type.py
--rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/enumerations/gencost_table.py
--rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/enumerations/generator_table.py
--rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/enumerations/power_flow_ids.py
--rw-rw-rw-   0        0        0     1254 2023-06-20 15:43:08.000000 mlpf-0.0.6/mlpf/enumerations/ppc_tables.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.844735 mlpf-0.0.6/mlpf/loss/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/loss/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.858739 mlpf-0.0.6/mlpf/loss/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/loss/numpy/__init__.py
--rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/loss/numpy/bound_errors.py
--rw-rw-rw-   0        0        0     3609 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/loss/numpy/power_flow.py
--rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/loss/numpy/utils.py
--rw-rw-rw-   0        0        0     1141 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/loss/relative_values.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.858739 mlpf-0.0.6/mlpf/loss/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/loss/torch/__init__.py
--rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/loss/torch/bound_errors.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.858739 mlpf-0.0.6/mlpf/loss/torch/metrics/
--rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.6/mlpf/loss/torch/metrics/__init__.py
--rw-rw-rw-   0        0        0     2699 2023-06-17 16:14:26.000000 mlpf-0.0.6/mlpf/loss/torch/metrics/power_flow.py
--rw-rw-rw-   0        0        0     5349 2023-06-11 16:38:41.000000 mlpf-0.0.6/mlpf/loss/torch/power_flow.py
--rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/loss/torch/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.858739 mlpf-0.0.6/mlpf/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/utils/__init__.py
--rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/utils/ppc.py
--rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.6/mlpf/utils/standard_scaler.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.829722 mlpf-0.0.6/mlpf.egg-info/
--rw-rw-rw-   0        0        0     4394 2023-06-20 17:12:45.000000 mlpf-0.0.6/mlpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2476 2023-06-20 17:12:45.000000 mlpf-0.0.6/mlpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 17:12:45.000000 mlpf-0.0.6/mlpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-20 17:12:45.000000 mlpf-0.0.6/mlpf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-20 17:12:45.000000 mlpf-0.0.6/mlpf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 17:12:45.858739 mlpf-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      998 2023-06-20 17:10:47.000000 mlpf-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:12:45.858739 mlpf-0.0.6/test/
--rw-rw-rw-   0        0        0     3020 2023-06-20 14:41:06.000000 mlpf-0.0.6/test/test_power_flow_loss.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.691975 mlpf-0.0.7/
+-rw-rw-rw-   0        0        0      479 2023-06-24 21:27:28.000000 mlpf-0.0.7/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5038 2023-06-24 21:34:24.691975 mlpf-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4399 2023-06-24 21:34:11.000000 mlpf-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.442477 mlpf-0.0.7/examples/
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.442477 mlpf-0.0.7/examples/data/
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.473533 mlpf-0.0.7/examples/data/analysis/
+-rw-rw-rw-   0        0        0     1390 2023-06-20 15:43:08.000000 mlpf-0.0.7/examples/data/analysis/describe_grid.py
+-rw-rw-rw-   0        0        0     1238 2023-06-20 15:43:08.000000 mlpf-0.0.7/examples/data/analysis/describe_node.py
+-rw-rw-rw-   0        0        0     1332 2023-06-20 15:43:08.000000 mlpf-0.0.7/examples/data/analysis/grid_pdf_estimates.py
+-rw-rw-rw-   0        0        0     1249 2023-06-20 15:43:08.000000 mlpf-0.0.7/examples/data/analysis/node_pdf_estimates.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.478731 mlpf-0.0.7/examples/data/generate/
+-rw-rw-rw-   0        0        0     1085 2023-06-20 15:43:08.000000 mlpf-0.0.7/examples/data/generate/uniform.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.442477 mlpf-0.0.7/examples/sklearn/
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.481970 mlpf-0.0.7/examples/sklearn/loss/
+-rw-rw-rw-   0        0        0     1016 2023-06-24 10:31:44.000000 mlpf-0.0.7/examples/sklearn/loss/from_arrays.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.486469 mlpf-0.0.7/examples/sklearn/supervised_power_flow/
+-rw-rw-rw-   0        0        0     2985 2023-06-20 13:03:26.000000 mlpf-0.0.7/examples/sklearn/supervised_power_flow/linear_regression.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.443826 mlpf-0.0.7/examples/torch/
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.491469 mlpf-0.0.7/examples/torch/loss/
+-rw-rw-rw-   0        0        0     1141 2023-06-24 10:31:11.000000 mlpf-0.0.7/examples/torch/loss/from_arrays.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.492938 mlpf-0.0.7/examples/torch/supervised_power_flow/
+-rw-rw-rw-   0        0        0     5501 2023-06-24 20:42:49.000000 mlpf-0.0.7/examples/torch/supervised_power_flow/gcn.py
+-rw-rw-rw-   0        0        0     4639 2023-06-24 20:42:49.000000 mlpf-0.0.7/examples/torch/supervised_power_flow/mlp.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.492938 mlpf-0.0.7/examples/torch/unsupervised_power_flow/
+-rw-rw-rw-   0        0        0     4961 2023-06-24 21:04:11.000000 mlpf-0.0.7/examples/torch/unsupervised_power_flow/gcn.py
+-rw-rw-rw-   0        0        0     4048 2023-06-24 20:42:49.000000 mlpf-0.0.7/examples/torch/unsupervised_power_flow/mlp.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.494377 mlpf-0.0.7/mlpf/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.518549 mlpf-0.0.7/mlpf/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.526203 mlpf-0.0.7/mlpf/data/analysis/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.539489 mlpf-0.0.7/mlpf/data/analysis/description/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/analysis/description/__init__.py
+-rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/analysis/description/describe.py
+-rw-rw-rw-   0        0        0     1447 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/analysis/description/describe_grid.py
+-rw-rw-rw-   0        0        0     1396 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/analysis/description/describe_node.py
+-rw-rw-rw-   0        0        0     6433 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/analysis/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.556634 mlpf-0.0.7/mlpf/data/analysis/visualization/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/analysis/visualization/__init__.py
+-rw-rw-rw-   0        0        0     3420 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/analysis/visualization/grid_pdf_estimates.py
+-rw-rw-rw-   0        0        0     3473 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/analysis/visualization/node_pdf_estimates.py
+-rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/analysis/visualization/visualize.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.562558 mlpf-0.0.7/mlpf/data/conversion/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.569287 mlpf-0.0.7/mlpf/data/conversion/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1788 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/numpy/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.574267 mlpf-0.0.7/mlpf/data/conversion/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/torch/__init__.py
+-rw-rw-rw-   0        0        0     1360 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/torch/power_flow.py
+-rw-rw-rw-   0        0        0      475 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/conversion/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.574267 mlpf-0.0.7/mlpf/data/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.579303 mlpf-0.0.7/mlpf/data/data/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/data/numpy/__init__.py
+-rw-rw-rw-   0        0        0     3922 2023-06-24 10:33:25.000000 mlpf-0.0.7/mlpf/data/data/numpy/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.584827 mlpf-0.0.7/mlpf/data/data/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/data/torch/__init__.py
+-rw-rw-rw-   0        0        0     1584 2023-06-24 10:33:25.000000 mlpf-0.0.7/mlpf/data/data/torch/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.585826 mlpf-0.0.7/mlpf/data/generate/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/generate/__init__.py
+-rw-rw-rw-   0        0        0     3523 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/data/generate/generate_uniform_data.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.591798 mlpf-0.0.7/mlpf/data/loading/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/loading/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-06-20 14:41:06.000000 mlpf-0.0.7/mlpf/data/loading/load_data.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.605217 mlpf-0.0.7/mlpf/data/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/utils/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/utils/masks.py
+-rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/utils/pandapower_networks.py
+-rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/data/utils/saving.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.634207 mlpf-0.0.7/mlpf/enumerations/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/branch_table.py
+-rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/bus_table.py
+-rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/bus_type.py
+-rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/gencost_table.py
+-rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/generator_table.py
+-rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/enumerations/power_flow_ids.py
+-rw-rw-rw-   0        0        0     1254 2023-06-20 15:43:08.000000 mlpf-0.0.7/mlpf/enumerations/ppc_tables.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.639855 mlpf-0.0.7/mlpf/loss/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.654217 mlpf-0.0.7/mlpf/loss/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/numpy/__init__.py
+-rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/numpy/bound_errors.py
+-rw-rw-rw-   0        0        0     3828 2023-06-24 10:16:05.000000 mlpf-0.0.7/mlpf/loss/numpy/power_flow.py
+-rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/numpy/utils.py
+-rw-rw-rw-   0        0        0     1465 2023-06-24 10:16:05.000000 mlpf-0.0.7/mlpf/loss/relative_values.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.679814 mlpf-0.0.7/mlpf/loss/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/torch/__init__.py
+-rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/torch/bound_errors.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.682241 mlpf-0.0.7/mlpf/loss/torch/metrics/
+-rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.7/mlpf/loss/torch/metrics/__init__.py
+-rw-rw-rw-   0        0        0     3615 2023-06-24 20:42:49.000000 mlpf-0.0.7/mlpf/loss/torch/metrics/active.py
+-rw-rw-rw-   0        0        0     3711 2023-06-24 20:42:49.000000 mlpf-0.0.7/mlpf/loss/torch/metrics/reactive.py
+-rw-rw-rw-   0        0        0      677 2023-06-24 10:16:05.000000 mlpf-0.0.7/mlpf/loss/torch/metrics/utils.py
+-rw-rw-rw-   0        0        0     3202 2023-06-24 10:30:16.000000 mlpf-0.0.7/mlpf/loss/torch/power_flow.py
+-rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/loss/torch/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.687453 mlpf-0.0.7/mlpf/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/utils/__init__.py
+-rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/utils/ppc.py
+-rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.7/mlpf/utils/standard_scaler.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.518549 mlpf-0.0.7/mlpf.egg-info/
+-rw-rw-rw-   0        0        0     5038 2023-06-24 21:34:24.000000 mlpf-0.0.7/mlpf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2633 2023-06-24 21:34:24.000000 mlpf-0.0.7/mlpf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 21:34:24.000000 mlpf-0.0.7/mlpf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-24 21:34:24.000000 mlpf-0.0.7/mlpf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-24 21:34:24.000000 mlpf-0.0.7/mlpf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 21:34:24.691975 mlpf-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-06-24 21:33:08.000000 mlpf-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:34:24.690969 mlpf-0.0.7/test/
+-rw-rw-rw-   0        0        0     2631 2023-06-24 10:16:05.000000 mlpf-0.0.7/test/test_power_flow_loss.py
```

### Comparing `mlpf-0.0.6/LICENCE.txt` & `mlpf-0.0.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/PKG-INFO` & `mlpf-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.6
+Version: 0.0.7
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
-Keywords: machine learning,power
+Keywords: machine learning,power flow,optimal power flow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
@@ -46,71 +46,63 @@
 ## Usage
 
 1. Load/create data and turn it into the [PYPOWER case format](https://rwl.github.io/PYPOWER/api/pypower.caseformat-module.html)
 2. From then on we provide functionality to express the data as numpy arrays or torch tensors.
 3. Feed that data into your ML (scikit-learn or torch) models and use our tried and tested loss functions to train, validate or monitor your model development.
 
 ```python
-import copy
-
 import pandapower as pp
 import pandapower.networks as pn
 
 from pypower.ppoption import ppoption
 from pypower.runpf import runpf
 
 net = pn.case118()
 
 ppc = pp.converter.to_ppc(net, init="flat")
 
 ppopt = ppoption(OUT_ALL=0, VERBOSE=0)
-ppc, converged = runpf(copy.deepcopy(ppc), ppopt=ppopt)
+ppc, converged = runpf(ppc, ppopt=ppopt)
 ```
 
 ### Loss
 
 #### numpy / scikit-learn
 
 ```python
+import numpy as np
 
 from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
-from mlpf.loss.numpy.power_flow import power_flow_errors
+from mlpf.loss.numpy.power_flow import active_power_errors, reactive_power_errors
 
 edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_arrays(ppc)
 
-active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
-    edge_index,
-    active_powers_pu,
-    reactive_powers_pu,
-    voltages_pu,
-    angles_rad,
-    conductances_pu,
-    susceptances_pu
-)
+active_errors = active_power_errors(edge_index, active_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
+reactive_errors = reactive_power_errors(edge_index, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
+
+print(f"Total P loss = {np.sum(active_errors):.3e} p.u.")
+print(f"Total Q loss = {np.sum(reactive_errors):.3e} p.u.")
 ```
 
 #### torch
 
 ```python
+import torch
 
 from mlpf.data.conversion.torch.power_flow import ppc2power_flow_tensors
-from mlpf.loss.torch.power_flow import power_flow_errors
+from mlpf.loss.torch.power_flow import active_power_errors, reactive_power_errors
 
 # note: going from float64(standard in PYPOWER) to float32(standard in torch) will increase the PF loss significantly
 edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_tensors(ppc, dtype=torch.float64)
 
-active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
-    edge_index,
-    active_powers_pu,
-    reactive_powers_pu,
-    voltages_pu,
-    angles_rad,
-    conductances_pu,
-    susceptances_pu
-)
+active_errors = active_power_errors(edge_index, active_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
+reactive_errors = reactive_power_errors(edge_index, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
+
+print(f"Total P loss = {torch.sum(active_errors):.3e} p.u.")
+print(f"Total Q loss = {torch.sum(reactive_errors):.3e} p.u.")
 ```
 
 ### Data loading
 
 - [ ] TODO
 
 ### Indepth examples
@@ -121,17 +113,24 @@
 * [Torch loss](examples/torch/loss/from_arrays.py)
 
 #### Supervised learning
 
 ##### Power flow
 
 * [scikit-learn linear regression](examples/sklearn/supervised_power_flow/linear_regression.py)
-* [torch linear regression](examples/torch/supervised_power_flow/mlp.py)
+* [torch MLP(multilayer perceptron)](examples/torch/supervised_power_flow/mlp.py)
 * [torch GCN(graph convolutional network)](examples/torch/supervised_power_flow/gcn.py)
 
+#### Supervised learning
+
+##### Power flow
+
+* [torch MLP(multilayer perceptron](examples/torch/unsupervised_power_flow/mlp.py)
+* [torch GCN(graph convolutional network)](examples/torch/unsupervised_power_flow/gcn.py)
+
 ### Development
 
 ```
 git clone https://github.com/viktor-ktorvi/mlpf.git
 cd mlpf
 
 conda env create -f environment.yml
```

### Comparing `mlpf-0.0.6/examples/data/analysis/describe_grid.py` & `mlpf-0.0.7/examples/data/analysis/describe_grid.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/examples/data/analysis/describe_node.py` & `mlpf-0.0.7/examples/data/analysis/describe_node.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/examples/data/analysis/grid_pdf_estimates.py` & `mlpf-0.0.7/examples/data/analysis/grid_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/examples/data/analysis/node_pdf_estimates.py` & `mlpf-0.0.7/examples/data/analysis/node_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/examples/data/generate/uniform.py` & `mlpf-0.0.7/examples/data/generate/uniform.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/examples/sklearn/supervised_power_flow/linear_regression.py` & `mlpf-0.0.7/examples/sklearn/supervised_power_flow/linear_regression.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/examples/torch/supervised_power_flow/gcn.py` & `mlpf-0.0.7/examples/torch/supervised_power_flow/gcn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import torch
 
 import pandapower as pp
 import pandapower.networks as pn
 import torch.nn as nn
 import torch_geometric as pyg
 
-from pandas.io.json._normalize import nested_to_record
 from pypower.ppoption import ppoption
 from pypower.runpf import runpf
 from sklearn.model_selection import train_test_split
 from torch_geometric.loader import DataLoader
 from torchmetrics import MetricCollection, MeanSquaredError, R2Score
 from tqdm import tqdm
 
 from mlpf.data.data.torch.power_flow import power_flow_data
 from mlpf.data.generate.generate_uniform_data import generate_uniform_ppcs
-from mlpf.loss.torch.metrics.power_flow import RelativePowerFlowError
+from mlpf.loss.torch.metrics.active import MeanActivePowerError, MeanRelativeActivePowerError
+from mlpf.loss.torch.metrics.reactive import MeanReactivePowerError, MeanRelativeReactivePowerError
 from mlpf.utils.standard_scaler import StandardScaler
 
 
 class GNN(torch.nn.Module):
     def __init__(self, in_channels, hidden_channels, num_layers, out_channels, standard_scaler):
         super(GNN, self).__init__()
         self.standard_scaler = standard_scaler
@@ -93,24 +93,32 @@
                 out_channels=node_features_stacked.shape[1],
                 standard_scaler=standard_scaler)
     model.to(device)
 
     optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
     criterion = nn.MSELoss()
 
+    # Metrics
+
     metrics_train = MetricCollection(
         MeanSquaredError(),
         R2Score(num_outputs=output_size),
-        RelativePowerFlowError(active_str="rel P", reactive_str="rel Q")
+        MeanActivePowerError(),
+        MeanRelativeActivePowerError(),
+        MeanReactivePowerError(),
+        MeanRelativeReactivePowerError()
     ).to(device)
 
     metrics_val = MetricCollection(
         MeanSquaredError(),
         R2Score(num_outputs=output_size),
-        RelativePowerFlowError(active_str="rel P", reactive_str="rel Q")
+        MeanActivePowerError(),
+        MeanRelativeActivePowerError(),
+        MeanReactivePowerError(),
+        MeanRelativeReactivePowerError()
     ).to(device)
 
     progress_bar = tqdm(range(num_epochs), ascii=True, desc="Training | Validation:")
 
     for epoch in progress_bar:
 
         # Training
@@ -120,31 +128,31 @@
 
             optimizer.zero_grad()
 
             predictions = model(batch)
             loss = criterion(predictions, output_scaler(batch.target_vector))
             loss.backward()
 
-            metrics_train(preds=predictions, target=output_scaler(batch.target_vector), preds_pf=output_scaler.inverse(predictions), batch=batch)
+            metrics_train(preds=predictions, target=output_scaler(batch.target_vector), power_flow_predictions=output_scaler.inverse(predictions), batch=batch)
 
             optimizer.step()
 
         # Validation
         with torch.no_grad():
 
             model.eval()
             for batch in val_loader:
                 batch = batch.to(device)
 
                 predictions = model(batch)
 
-                metrics_val(preds=predictions, target=output_scaler(batch.target_vector), preds_pf=output_scaler.inverse(predictions), batch=batch)
+                metrics_val(preds=predictions, target=output_scaler(batch.target_vector), power_flow_predictions=output_scaler.inverse(predictions), batch=batch)
 
-        overall_metrics_train = nested_to_record(metrics_train.compute(), sep='_')
-        overall_metrics_val = nested_to_record(metrics_val.compute(), sep='_')
+        overall_metrics_train = metrics_train.compute()
+        overall_metrics_val = metrics_val.compute()
 
         description = "Training | Validation:"
 
         for key in overall_metrics_train.keys():
             description += f" {key}: ({overall_metrics_train[key]:2.4f} | {overall_metrics_val[key]:2.4f});"
 
         progress_bar.set_description(description)
```

### Comparing `mlpf-0.0.6/examples/torch/supervised_power_flow/mlp.py` & `mlpf-0.0.7/examples/torch/supervised_power_flow/mlp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import torch
 
 import pandapower as pp
 import pandapower.networks as pn
 import torch.nn as nn
 import torch_geometric as pyg
 
-from pandas.io.json._normalize import nested_to_record
 from pypower.ppoption import ppoption
 from pypower.runpf import runpf
 from sklearn.model_selection import train_test_split
 from torch_geometric.loader import DataLoader
 from torchmetrics import MetricCollection, MeanSquaredError, R2Score
 from tqdm import tqdm
 
 from mlpf.data.data.torch.power_flow import power_flow_data
 from mlpf.data.generate.generate_uniform_data import generate_uniform_ppcs
-from mlpf.loss.torch.metrics.power_flow import RelativePowerFlowError
+from mlpf.loss.torch.metrics.active import MeanActivePowerError, MeanRelativeActivePowerError
+from mlpf.loss.torch.metrics.reactive import MeanReactivePowerError, MeanRelativeReactivePowerError
 from mlpf.utils.standard_scaler import StandardScaler
 
 
 def main():
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     # Random seeds
@@ -71,62 +71,68 @@
         nn.Linear(in_features=input_size, out_features=output_size),
     )
     model.to(device)
 
     optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
     criterion = nn.MSELoss()
 
+    # Metrics
+
     metrics_train = MetricCollection(
         MeanSquaredError(),
         R2Score(num_outputs=output_size),
-        RelativePowerFlowError(active_str="rel P", reactive_str="rel Q")
+        MeanActivePowerError(),
+        MeanRelativeActivePowerError(),
+        MeanReactivePowerError(),
+        MeanRelativeReactivePowerError()
     ).to(device)
 
     metrics_val = MetricCollection(
         MeanSquaredError(),
         R2Score(num_outputs=output_size),
-        RelativePowerFlowError(active_str="rel P", reactive_str="rel Q")
+        MeanActivePowerError(),
+        MeanRelativeActivePowerError(),
+        MeanReactivePowerError(),
+        MeanRelativeReactivePowerError()
     ).to(device)
 
     progress_bar = tqdm(range(num_epochs), ascii=True, desc="Training | Validation:")
 
     for epoch in progress_bar:
 
         # Training
         model.train()
         for batch in train_loader:
+            batch = batch.to(device)
             features, targets = batch.feature_vector, batch.target_vector
-            features = features.to(device)
-            targets = targets.to(device)
 
             optimizer.zero_grad()
 
             predictions = model(features)
             loss = criterion(predictions, output_scaler(targets))
             loss.backward()
 
-            metrics_train(preds=predictions, target=output_scaler(targets), preds_pf=output_scaler.inverse(predictions), batch=batch)
+            metrics_train(preds=predictions, target=output_scaler(targets), power_flow_predictions=output_scaler.inverse(predictions), batch=batch)
 
             optimizer.step()
 
         # Validation
         with torch.no_grad():
 
             model.eval()
             for batch in val_loader:
+                batch = batch.to(device)
                 features, targets = batch.feature_vector, batch.target_vector
-                features = features.to(device)
-                targets = targets.to(device)
 
                 predictions = model(features)
 
-                metrics_val(preds=predictions, target=output_scaler(targets), preds_pf=output_scaler.inverse(predictions), batch=batch)
+                metrics_val(preds=predictions, target=output_scaler(targets), power_flow_predictions=output_scaler.inverse(predictions), batch=batch)
 
-        overall_metrics_train = nested_to_record(metrics_train.compute(), sep='_')
-        overall_metrics_val = nested_to_record(metrics_val.compute(), sep='_')
+        overall_metrics_train = metrics_train.compute()
+        overall_metrics_val = metrics_val.compute()
 
         description = "Training | Validation:"
 
         for key in overall_metrics_train.keys():
             description += f" {key}: ({overall_metrics_train[key]:2.4f} | {overall_metrics_val[key]:2.4f});"
 
         progress_bar.set_description(description)
```

### Comparing `mlpf-0.0.6/mlpf/data/analysis/description/describe.py` & `mlpf-0.0.7/mlpf/data/analysis/description/describe.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/analysis/description/describe_grid.py` & `mlpf-0.0.7/mlpf/data/analysis/description/describe_grid.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/analysis/description/describe_node.py` & `mlpf-0.0.7/mlpf/data/analysis/description/describe_node.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/analysis/utils.py` & `mlpf-0.0.7/mlpf/data/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/analysis/visualization/grid_pdf_estimates.py` & `mlpf-0.0.7/mlpf/data/analysis/visualization/grid_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/analysis/visualization/node_pdf_estimates.py` & `mlpf-0.0.7/mlpf/data/analysis/visualization/node_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/analysis/visualization/visualize.py` & `mlpf-0.0.7/mlpf/data/analysis/visualization/visualize.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/conversion/numpy/power_flow.py` & `mlpf-0.0.7/mlpf/data/conversion/numpy/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/conversion/torch/power_flow.py` & `mlpf-0.0.7/mlpf/data/conversion/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/data/numpy/power_flow.py` & `mlpf-0.0.7/mlpf/data/data/numpy/power_flow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import copy
-from typing import Tuple
 
 import numpy as np
+
 from numpy import ndarray
 from types import SimpleNamespace
+from typing import Tuple
 
 from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
 from mlpf.data.utils.masks import create_feature_mask
 from mlpf.enumerations.bus_table import BusTableIds
 from mlpf.enumerations.power_flow_ids import PowerFlowFeatureIds
-from mlpf.loss.numpy.power_flow import power_flow_errors
+from mlpf.loss.numpy.power_flow import active_power_errors, reactive_power_errors
 from mlpf.loss.relative_values import relative_values
 from mlpf.utils.ppc import ppc_runpf
 
 
 def power_flow_data(ppc: dict, solve: bool = False, dtype: np.dtype = np.float64):
     """
     Extract all the relevant info from the ppc file as ndarrays and pack it into a PyG Data object.
@@ -41,51 +42,43 @@
         conductances_pu=conductances_pu,
         susceptances_pu=susceptances_pu,
         feature_vector=PQVA_matrix[feature_mask],
         target_vector=PQVA_matrix[~feature_mask]
     )
 
 
-def get_power_flow_errors(predictions: ndarray, data: SimpleNamespace) -> Tuple[ndarray, ...]:
+def get_relative_power_flow_errors(predictions: ndarray, data: SimpleNamespace) -> Tuple[ndarray, ...]:
     """
-    Take model predictions and merge them with the corresponding data object.
-    Calculate the power flow errors for the given predictions.
+    Take model predictions and merge them with the corresponding data batch.
+    Calculate the relative power flow errors for the given predictions.
 
     :param predictions: Power flow unknown variable predictions.
     :param data: Data object from which the predictions came from.
-    :return: (active power errors, reactive power errors, active power, reactive power)
+    :return: (relative active power errors, relative reactive power errors)
     """
-
     PQVA_matrix_prediction = copy.deepcopy(data.PQVA_matrix)
     PQVA_matrix_prediction[~data.feature_mask] = predictions.flatten()
 
     active_powers = PQVA_matrix_prediction[:, PowerFlowFeatureIds.active_power]
     reactive_powers = PQVA_matrix_prediction[:, PowerFlowFeatureIds.reactive_power]
 
-    active_power_errors, reactive_power_errors = power_flow_errors(
-        edge_index=data.edge_index,
-        active_powers=active_powers,
-        reactive_powers=reactive_powers,
-        voltages=PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_magnitude],
-        angles_rad=PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_angle],
-        conductances=data.conductances_pu,
-        susceptances=data.susceptances_pu
-    )
-
-    return active_power_errors, reactive_power_errors, active_powers, reactive_powers
+    voltage_magnitudes = PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_magnitude]
+    angles_rad = PQVA_matrix_prediction[:, PowerFlowFeatureIds.voltage_angle]
 
+    active_errors = active_power_errors(edge_index=data.edge_index,
+                                        active_powers=active_powers,
+                                        voltages=voltage_magnitudes,
+                                        angles_rad=angles_rad,
+                                        conductances=data.conductances_pu,
+                                        susceptances=data.susceptances_pu)
+
+    reactive_errors = reactive_power_errors(edge_index=data.edge_index,
+                                            reactive_powers=reactive_powers,
+                                            voltages=voltage_magnitudes,
+                                            angles_rad=angles_rad,
+                                            conductances=data.conductances_pu,
+                                            susceptances=data.susceptances_pu)
 
-def get_relative_power_flow_errors(predictions: ndarray, data: SimpleNamespace) -> Tuple[ndarray, ...]:
-    """
-    Take model predictions and merge them with the corresponding data batch.
-    Calculate the relative power flow errors for the given predictions.
-
-    :param predictions: Power flow unknown variable predictions.
-    :param data: Data object from which the predictions came from.
-    :return: (relative active power errors, relative reactive power errors)
-    """
-    active_power_errors, reactive_power_errors, active_powers, reactive_powers = get_power_flow_errors(predictions, data)
-
-    relative_active_power_errors = np.abs(relative_values(active_power_errors, active_powers))
-    relative_reactive_power_errors = np.abs(relative_values(reactive_power_errors, reactive_powers))
+    relative_active_power_errors = np.abs(relative_values(active_errors, active_powers))
+    relative_reactive_power_errors = np.abs(relative_values(reactive_errors, reactive_powers))
 
     return relative_active_power_errors, relative_reactive_power_errors
```

### Comparing `mlpf-0.0.6/mlpf/data/generate/generate_uniform_data.py` & `mlpf-0.0.7/mlpf/data/generate/generate_uniform_data.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/loading/load_data.py` & `mlpf-0.0.7/mlpf/data/loading/load_data.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/utils/masks.py` & `mlpf-0.0.7/mlpf/data/utils/masks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/utils/pandapower_networks.py` & `mlpf-0.0.7/mlpf/data/utils/pandapower_networks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/data/utils/saving.py` & `mlpf-0.0.7/mlpf/data/utils/saving.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/enumerations/generator_table.py` & `mlpf-0.0.7/mlpf/enumerations/generator_table.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/enumerations/ppc_tables.py` & `mlpf-0.0.7/mlpf/enumerations/ppc_tables.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/loss/numpy/bound_errors.py` & `mlpf-0.0.7/mlpf/loss/numpy/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/loss/numpy/utils.py` & `mlpf-0.0.7/mlpf/loss/numpy/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/loss/relative_values.py` & `mlpf-0.0.7/mlpf/loss/relative_values.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from typing import Any
 
 import numpy as np
+import torch
+from numpy import ndarray
+from torch import Tensor
 
 
 def relative_values(numerator: Any, denominator: Any, eps: float = 1e-9, fill: bool = True):
     # TODO test for arrays and tensors. What happens when fill=False and denominator is all zeros
     """
     Return the relative value of the numerator with respect to the denominator, all while protecting against
     divisions by zero or close to zero values.
@@ -12,15 +15,20 @@
     :param numerator: Array/Tensor to be divided.
     :param denominator: Array/Tensor to divide with.
     :param eps: Absolute value tolerance for being marked as zero value in the denominator.
     :param fill: Whether to fill in the values where there would have been a division by zero or not. In those cases
     returns a 0 relative value.
     :return: Relative values.
     """
-    zero_denominator_mask = np.abs(denominator) < eps
+    if type(denominator) == ndarray:
+        zero_denominator_mask = np.abs(denominator) < eps
+    elif type(denominator) == Tensor:
+        zero_denominator_mask = torch.abs(denominator) < eps
+    else:
+        raise TypeError(f"Expected types 'ndarray' or 'Tensor' but got {type(denominator)} instead.")
 
     if fill:
         denominator[zero_denominator_mask] = 1.0
 
         rel_vals = numerator / denominator
         rel_vals[zero_denominator_mask] = 0.0
```

### Comparing `mlpf-0.0.6/mlpf/loss/torch/bound_errors.py` & `mlpf-0.0.7/mlpf/loss/torch/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/loss/torch/utils.py` & `mlpf-0.0.7/mlpf/loss/torch/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf/utils/standard_scaler.py` & `mlpf-0.0.7/mlpf/utils/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.6/mlpf.egg-info/PKG-INFO` & `mlpf-0.0.7/mlpf.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.6
+Version: 0.0.7
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
-Keywords: machine learning,power
+Keywords: machine learning,power flow,optimal power flow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
@@ -46,71 +46,63 @@
 ## Usage
 
 1. Load/create data and turn it into the [PYPOWER case format](https://rwl.github.io/PYPOWER/api/pypower.caseformat-module.html)
 2. From then on we provide functionality to express the data as numpy arrays or torch tensors.
 3. Feed that data into your ML (scikit-learn or torch) models and use our tried and tested loss functions to train, validate or monitor your model development.
 
 ```python
-import copy
-
 import pandapower as pp
 import pandapower.networks as pn
 
 from pypower.ppoption import ppoption
 from pypower.runpf import runpf
 
 net = pn.case118()
 
 ppc = pp.converter.to_ppc(net, init="flat")
 
 ppopt = ppoption(OUT_ALL=0, VERBOSE=0)
-ppc, converged = runpf(copy.deepcopy(ppc), ppopt=ppopt)
+ppc, converged = runpf(ppc, ppopt=ppopt)
 ```
 
 ### Loss
 
 #### numpy / scikit-learn
 
 ```python
+import numpy as np
 
 from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
-from mlpf.loss.numpy.power_flow import power_flow_errors
+from mlpf.loss.numpy.power_flow import active_power_errors, reactive_power_errors
 
 edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_arrays(ppc)
 
-active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
-    edge_index,
-    active_powers_pu,
-    reactive_powers_pu,
-    voltages_pu,
-    angles_rad,
-    conductances_pu,
-    susceptances_pu
-)
+active_errors = active_power_errors(edge_index, active_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
+reactive_errors = reactive_power_errors(edge_index, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
+
+print(f"Total P loss = {np.sum(active_errors):.3e} p.u.")
+print(f"Total Q loss = {np.sum(reactive_errors):.3e} p.u.")
 ```
 
 #### torch
 
 ```python
+import torch
 
 from mlpf.data.conversion.torch.power_flow import ppc2power_flow_tensors
-from mlpf.loss.torch.power_flow import power_flow_errors
+from mlpf.loss.torch.power_flow import active_power_errors, reactive_power_errors
 
 # note: going from float64(standard in PYPOWER) to float32(standard in torch) will increase the PF loss significantly
 edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_tensors(ppc, dtype=torch.float64)
 
-active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
-    edge_index,
-    active_powers_pu,
-    reactive_powers_pu,
-    voltages_pu,
-    angles_rad,
-    conductances_pu,
-    susceptances_pu
-)
+active_errors = active_power_errors(edge_index, active_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
+reactive_errors = reactive_power_errors(edge_index, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
+
+print(f"Total P loss = {torch.sum(active_errors):.3e} p.u.")
+print(f"Total Q loss = {torch.sum(reactive_errors):.3e} p.u.")
 ```
 
 ### Data loading
 
 - [ ] TODO
 
 ### Indepth examples
@@ -121,17 +113,24 @@
 * [Torch loss](examples/torch/loss/from_arrays.py)
 
 #### Supervised learning
 
 ##### Power flow
 
 * [scikit-learn linear regression](examples/sklearn/supervised_power_flow/linear_regression.py)
-* [torch linear regression](examples/torch/supervised_power_flow/mlp.py)
+* [torch MLP(multilayer perceptron)](examples/torch/supervised_power_flow/mlp.py)
 * [torch GCN(graph convolutional network)](examples/torch/supervised_power_flow/gcn.py)
 
+#### Supervised learning
+
+##### Power flow
+
+* [torch MLP(multilayer perceptron](examples/torch/unsupervised_power_flow/mlp.py)
+* [torch GCN(graph convolutional network)](examples/torch/unsupervised_power_flow/gcn.py)
+
 ### Development
 
 ```
 git clone https://github.com/viktor-ktorvi/mlpf.git
 cd mlpf
 
 conda env create -f environment.yml
```

### Comparing `mlpf-0.0.6/mlpf.egg-info/SOURCES.txt` & `mlpf-0.0.7/mlpf.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 examples/data/analysis/node_pdf_estimates.py
 examples/data/generate/uniform.py
 examples/sklearn/loss/from_arrays.py
 examples/sklearn/supervised_power_flow/linear_regression.py
 examples/torch/loss/from_arrays.py
 examples/torch/supervised_power_flow/gcn.py
 examples/torch/supervised_power_flow/mlp.py
+examples/torch/unsupervised_power_flow/gcn.py
+examples/torch/unsupervised_power_flow/mlp.py
 mlpf/__init__.py
 mlpf.egg-info/PKG-INFO
 mlpf.egg-info/SOURCES.txt
 mlpf.egg-info/dependency_links.txt
 mlpf.egg-info/requires.txt
 mlpf.egg-info/top_level.txt
 mlpf/data/__init__.py
@@ -65,12 +67,14 @@
 mlpf/loss/numpy/power_flow.py
 mlpf/loss/numpy/utils.py
 mlpf/loss/torch/__init__.py
 mlpf/loss/torch/bound_errors.py
 mlpf/loss/torch/power_flow.py
 mlpf/loss/torch/utils.py
 mlpf/loss/torch/metrics/__init__.py
-mlpf/loss/torch/metrics/power_flow.py
+mlpf/loss/torch/metrics/active.py
+mlpf/loss/torch/metrics/reactive.py
+mlpf/loss/torch/metrics/utils.py
 mlpf/utils/__init__.py
 mlpf/utils/ppc.py
 mlpf/utils/standard_scaler.py
 test/test_power_flow_loss.py
```

### Comparing `mlpf-0.0.6/setup.py` & `mlpf-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 ]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mlpf',
-    version='0.0.6',
+    version='0.0.7',
     description='Machine learning for power flow',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     author='Viktor Todosijevic',
     author_email='todosijevicviktor998@gmail.com',
     license='MIT',
     classifiers=classifiers,
-    keywords=['machine learning', 'power'],
+    keywords=['machine learning', 'power flow', 'optimal power flow'],
     packages=find_packages(),
     install_requires=['numpy', 'pandapower', 'PYPOWER', 'scikit-learn', 'scipy', 'tqdm']
 )
```

### Comparing `mlpf-0.0.6/test/test_power_flow_loss.py` & `mlpf-0.0.7/test/test_power_flow_loss.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,64 @@
 import unittest
 import warnings
 from typing import Dict
 
+import numpy as np
 import pandapower as pp
 import torch
 
-from mlpf.data.conversion.torch.power_flow import ppc2power_flow_tensors
 from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
+from mlpf.data.conversion.torch.power_flow import ppc2power_flow_tensors
 from mlpf.data.utils.pandapower_networks import get_all_pandapower_networks
 from mlpf.loss.numpy import power_flow as pf_numpy
 from mlpf.loss.torch import power_flow as pf_torch
 
 
-def torch_get_power_flow_loss(ppc: Dict, method="scatter", dtype: torch.dtype = torch.float64) -> float:
+def torch_get_power_flow_loss(ppc: Dict, dtype: torch.dtype = torch.float64) -> float:
     """
     Get power flow loss from a ppc.
 
     :param ppc: pypower case format
-    :param method: To use scatter operations on arrays or to multiply with sparse matrices.
     :param dtype: torch data type
     :return: loss
     """
     edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_tensors(ppc, dtype)
 
-    active_power_losses_pu, reactive_power_losses_pu = pf_torch.power_flow_errors(
-        edge_index,
-        active_powers_pu,
-        reactive_powers_pu,
-        voltages_pu, angles_rad,
-        conductances_pu,
-        susceptances_pu,
-        method=method
-    )
+    active_errors = pf_torch.active_power_errors(edge_index, active_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
+    reactive_errors = pf_torch.reactive_power_errors(edge_index, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
 
-    return float(pf_torch.scalarize(active_power_losses_pu, reactive_power_losses_pu))
+    return float(torch.sum(active_errors + reactive_errors))
 
 
-def numpy_get_power_flow_loss(ppc: Dict, method="sparse") -> float:
+def numpy_get_power_flow_loss(ppc: Dict) -> float:
     """
     Get power flow loss from a ppc.
 
     :param ppc: pypower case format
-    :param method: To use scatter operations on arrays or to multiply with sparse matrices.
     :return: loss
     """
     edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_arrays(ppc)
 
-    active_power_losses_pu, reactive_power_losses_pu = pf_numpy.power_flow_errors(
-        edge_index,
-        active_powers_pu,
-        reactive_powers_pu,
-        voltages_pu, angles_rad,
-        conductances_pu,
-        susceptances_pu,
-        method=method
-    )
+    active_errors = pf_numpy.active_power_errors(edge_index, active_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
+    reactive_errors = pf_numpy.reactive_power_errors(edge_index, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu)
 
-    return float(pf_numpy.scalarize(active_power_losses_pu, reactive_power_losses_pu))
+    return float(np.sum(active_errors + reactive_errors))
 
 
 class TestPowerFlowLoss(unittest.TestCase):
     def test_many_topologies(self):
         """
         Test for various grids if the power flow loss function calculates near 0 loss for solved ppcs in float64 accuracy.
         :return:
         """
         warnings.filterwarnings("ignore", message="Casting complex values to real discards the imaginary part")
         places = 5
         nets = get_all_pandapower_networks()
         for net in nets:
             print(net)
             pp.runpp(net, tolerance_mva=1e-10, numba=False)
-            self.assertAlmostEqual(torch_get_power_flow_loss(net._ppc, method="scatter"), 0.0, places=places)
-            self.assertAlmostEqual(torch_get_power_flow_loss(net._ppc, method="sparse"), 0.0, places=places)
-
-            self.assertAlmostEqual(numpy_get_power_flow_loss(net._ppc, method="sparse"), 0.0, places=places)
+            self.assertAlmostEqual(torch_get_power_flow_loss(net._ppc), 0.0, places=places)
+            self.assertAlmostEqual(numpy_get_power_flow_loss(net._ppc), 0.0, places=places)
 
 
 if __name__ == '__main__':
     unittest.main()
```

