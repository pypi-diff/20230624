# Comparing `tmp/bluecast-0.3.1.tar.gz` & `tmp/bluecast-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluecast-0.3.1.tar", max compression
+gzip compressed data, was "bluecast-0.4.tar", max compression
```

## Comparing `bluecast-0.3.1.tar` & `bluecast-0.4.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-0.3.1/LICENSE
--rw-r--r--   0        0        0    16117 2023-06-23 14:09:53.984181 bluecast-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-0.3.1/bluecast/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.3.1/bluecast/blueprints/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-0.3.1/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-0.3.1/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8992 2023-06-23 12:59:49.535433 bluecast-0.3.1/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
--rw-r--r--   0        0        0     7485 2023-06-08 04:50:54.090183 bluecast-0.3.1/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
--rw-r--r--   0        0        0    13297 2023-06-23 12:59:43.723338 bluecast-0.3.1/bluecast/blueprints/cast.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.3.1/bluecast/config/__init__.py
--rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-0.3.1/bluecast/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-0.3.1/bluecast/config/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4476 2023-06-23 11:38:00.335361 bluecast-0.3.1/bluecast/config/__pycache__/training_config.cpython-310.pyc
--rw-r--r--   0        0        0     3347 2023-06-08 04:35:46.974972 bluecast-0.3.1/bluecast/config/__pycache__/training_config.cpython-38.pyc
--rw-r--r--   0        0        0     3469 2023-06-23 11:37:59.119340 bluecast-0.3.1/bluecast/config/training_config.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-0.3.1/bluecast/evaluation/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-0.3.1/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-0.3.1/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2037 2023-06-23 04:30:50.713477 bluecast-0.3.1/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
--rw-r--r--   0        0        0     1585 2023-06-08 04:35:46.978972 bluecast-0.3.1/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
--rw-r--r--   0        0        0     1323 2023-06-09 12:39:11.740235 bluecast-0.3.1/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
--rw-r--r--   0        0        0     1407 2023-06-08 04:35:46.978972 bluecast-0.3.1/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
--rw-r--r--   0        0        0     2478 2023-06-23 04:30:45.253379 bluecast-0.3.1/bluecast/evaluation/eval_metrics.py
--rw-r--r--   0        0        0     1389 2023-06-09 12:39:09.708202 bluecast-0.3.1/bluecast/evaluation/shap_values.py
--rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-0.3.1/bluecast/general_utils/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-0.3.1/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-0.3.1/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2431 2023-06-08 04:36:45.751908 bluecast-0.3.1/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2442 2023-06-08 04:35:46.978972 bluecast-0.3.1/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
--rw-r--r--   0        0        0     2248 2023-06-08 04:28:32.967204 bluecast-0.3.1/bluecast/general_utils/general_utils.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.3.1/bluecast/ml_modelling/__init__.py
--rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-0.3.1/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-0.3.1/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1431 2023-06-08 04:36:46.587922 bluecast-0.3.1/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
--rw-r--r--   0        0        0     1416 2023-06-08 04:35:46.978972 bluecast-0.3.1/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
--rw-r--r--   0        0        0     9011 2023-06-23 11:28:59.858174 bluecast-0.3.1/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
--rw-r--r--   0        0        0     8279 2023-06-08 04:35:46.978972 bluecast-0.3.1/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
--rw-r--r--   0        0        0      982 2023-06-08 04:28:32.971163 bluecast-0.3.1/bluecast/ml_modelling/base_classes.py
--rw-r--r--   0        0        0    13523 2023-06-23 14:22:20.312328 bluecast-0.3.1/bluecast/ml_modelling/xgboost.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.3.1/bluecast/preprocessing/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-0.3.1/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-0.3.1/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1924 2023-06-23 04:26:17.139640 bluecast-0.3.1/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
--rw-r--r--   0        0        0     1534 2023-06-08 04:36:46.587922 bluecast-0.3.1/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
--rw-r--r--   0        0        0     1502 2023-06-08 04:35:46.982972 bluecast-0.3.1/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
--rw-r--r--   0        0        0     3666 2023-06-08 04:36:46.587922 bluecast-0.3.1/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
--rw-r--r--   0        0        0     3656 2023-06-08 04:35:46.982972 bluecast-0.3.1/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
--rw-r--r--   0        0        0     1374 2023-06-23 13:01:03.812637 bluecast-0.3.1/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
--rw-r--r--   0        0        0     4575 2023-06-23 04:26:17.143641 bluecast-0.3.1/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
--rw-r--r--   0        0        0     4561 2023-06-08 04:35:46.982972 bluecast-0.3.1/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
--rw-r--r--   0        0        0     1167 2023-06-08 04:36:46.587922 bluecast-0.3.1/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
--rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-0.3.1/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
--rw-r--r--   0        0        0     1948 2023-06-08 06:48:48.640550 bluecast-0.3.1/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
--rw-r--r--   0        0        0     1929 2023-06-08 04:53:15.604550 bluecast-0.3.1/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
--rw-r--r--   0        0        0     4931 2023-06-08 04:36:46.591922 bluecast-0.3.1/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
--rw-r--r--   0        0        0     5044 2023-06-08 04:35:46.982972 bluecast-0.3.1/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
--rw-r--r--   0        0        0     2352 2023-06-23 04:26:17.187641 bluecast-0.3.1/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
--rw-r--r--   0        0        0     1790 2023-06-08 04:35:46.982972 bluecast-0.3.1/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
--rw-r--r--   0        0        0     1402 2023-06-21 05:07:47.892424 bluecast-0.3.1/bluecast/preprocessing/custom.py
--rw-r--r--   0        0        0     1424 2023-06-08 04:28:32.971163 bluecast-0.3.1/bluecast/preprocessing/datetime_features.py
--rw-r--r--   0        0        0     3122 2023-06-08 04:28:32.971163 bluecast-0.3.1/bluecast/preprocessing/encode_target_labels.py
--rw-r--r--   0        0        0     1354 2023-06-23 13:12:42.063930 bluecast-0.3.1/bluecast/preprocessing/feature_selection.py
--rw-r--r--   0        0        0     6190 2023-06-21 05:07:47.896425 bluecast-0.3.1/bluecast/preprocessing/feature_types.py
--rw-r--r--   0        0        0      862 2023-06-08 04:28:32.971163 bluecast-0.3.1/bluecast/preprocessing/nulls_and_infs.py
--rw-r--r--   0        0        0     1452 2023-06-08 06:48:42.348436 bluecast-0.3.1/bluecast/preprocessing/schema_checks.py
--rw-r--r--   0        0        0     4561 2023-06-08 04:28:32.971163 bluecast-0.3.1/bluecast/preprocessing/target_encoding.py
--rw-r--r--   0        0        0     2871 2023-06-21 05:07:47.896425 bluecast-0.3.1/bluecast/preprocessing/train_test_split.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.3.1/bluecast/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-0.3.1/bluecast/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7699 2023-06-23 12:59:49.139426 bluecast-0.3.1/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3156 2023-06-07 13:42:51.261239 bluecast-0.3.1/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-0.3.1/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1137 2023-06-07 04:38:15.364753 bluecast-0.3.1/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-0.3.1/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4803 2023-06-07 13:42:51.269239 bluecast-0.3.1/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1597 2023-06-09 12:06:35.203065 bluecast-0.3.1/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-0.3.1/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-0.3.1/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-0.3.1/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3994 2023-06-09 12:37:48.738873 bluecast-0.3.1/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-0.3.1/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1449 2023-06-07 04:38:15.376753 bluecast-0.3.1/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-0.3.1/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.3.1/bluecast/tests/make_data/__init__.py
--rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-0.3.1/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-06-07 04:38:15.360753 bluecast-0.3.1/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
--rw-r--r--   0        0        0     1289 2023-06-07 04:18:43.418068 bluecast-0.3.1/bluecast/tests/make_data/create_data.py
--rw-r--r--   0        0        0     5855 2023-06-23 12:58:15.485905 bluecast-0.3.1/bluecast/tests/test_cast.py
--rw-r--r--   0        0        0     1328 2023-06-07 13:40:33.489843 bluecast-0.3.1/bluecast/tests/test_check_gpu_support.py
--rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-0.3.1/bluecast/tests/test_custom_processing_base_class.py
--rw-r--r--   0        0        0     1097 2023-06-07 04:38:03.828575 bluecast-0.3.1/bluecast/tests/test_datetime_features.py
--rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-0.3.1/bluecast/tests/test_encode_target_labels.py
--rw-r--r--   0        0        0     2608 2023-06-07 13:42:39.380960 bluecast-0.3.1/bluecast/tests/test_feature_type_detector.py
--rw-r--r--   0        0        0     1482 2023-06-09 05:52:17.052295 bluecast-0.3.1/bluecast/tests/test_load_for_production.py
--rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-0.3.1/bluecast/tests/test_nulls_and_infs.py
--rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-0.3.1/bluecast/tests/test_save_to_production.py
--rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-0.3.1/bluecast/tests/test_schema_checks.py
--rw-r--r--   0        0        0     2204 2023-06-09 12:36:14.185320 bluecast-0.3.1/bluecast/tests/test_shap_explanations.py
--rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-0.3.1/bluecast/tests/test_target_encoding_binary.py
--rw-r--r--   0        0        0      735 2023-06-07 04:38:03.832575 bluecast-0.3.1/bluecast/tests/test_target_encoding_multiclass.py
--rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-0.3.1/bluecast/tests/test_train_test_split.py
--rw-r--r--   0        0        0     1459 2023-06-23 14:24:03.722020 bluecast-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    17235 1970-01-01 00:00:00.000000 bluecast-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-0.4/LICENSE
+-rw-r--r--   0        0        0    17251 2023-06-24 16:03:48.899672 bluecast-0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-0.4/bluecast/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.4/bluecast/blueprints/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-0.4/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-0.4/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     9579 2023-06-24 15:47:26.068709 bluecast-0.4/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
+-rw-r--r--   0        0        0     7485 2023-06-08 04:50:54.090183 bluecast-0.4/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
+-rw-r--r--   0        0        0    14107 2023-06-24 15:56:41.269653 bluecast-0.4/bluecast/blueprints/cast.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.4/bluecast/config/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-0.4/bluecast/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-0.4/bluecast/config/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4479 2023-06-24 15:42:29.710840 bluecast-0.4/bluecast/config/__pycache__/training_config.cpython-310.pyc
+-rw-r--r--   0        0        0     3347 2023-06-08 04:35:46.974972 bluecast-0.4/bluecast/config/__pycache__/training_config.cpython-38.pyc
+-rw-r--r--   0        0        0     3477 2023-06-24 15:42:22.702820 bluecast-0.4/bluecast/config/training_config.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-0.4/bluecast/evaluation/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-0.4/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-0.4/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2037 2023-06-23 04:30:50.713477 bluecast-0.4/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     1585 2023-06-08 04:35:46.978972 bluecast-0.4/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
+-rw-r--r--   0        0        0     1323 2023-06-09 12:39:11.740235 bluecast-0.4/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
+-rw-r--r--   0        0        0     1407 2023-06-08 04:35:46.978972 bluecast-0.4/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
+-rw-r--r--   0        0        0     2478 2023-06-23 04:30:45.253379 bluecast-0.4/bluecast/evaluation/eval_metrics.py
+-rw-r--r--   0        0        0     1389 2023-06-09 12:39:09.708202 bluecast-0.4/bluecast/evaluation/shap_values.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-0.4/bluecast/general_utils/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-0.4/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-0.4/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2431 2023-06-08 04:36:45.751908 bluecast-0.4/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2442 2023-06-08 04:35:46.978972 bluecast-0.4/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2023-06-08 04:28:32.967204 bluecast-0.4/bluecast/general_utils/general_utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.4/bluecast/ml_modelling/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-0.4/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-0.4/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1431 2023-06-08 04:36:46.587922 bluecast-0.4/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
+-rw-r--r--   0        0        0     1416 2023-06-08 04:35:46.978972 bluecast-0.4/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
+-rw-r--r--   0        0        0     8999 2023-06-24 15:42:30.258842 bluecast-0.4/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
+-rw-r--r--   0        0        0     8279 2023-06-08 04:35:46.978972 bluecast-0.4/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
+-rw-r--r--   0        0        0      982 2023-06-08 04:28:32.971163 bluecast-0.4/bluecast/ml_modelling/base_classes.py
+-rw-r--r--   0        0        0    13523 2023-06-23 14:22:20.312328 bluecast-0.4/bluecast/ml_modelling/xgboost.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.4/bluecast/preprocessing/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-0.4/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-0.4/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1924 2023-06-23 04:26:17.139640 bluecast-0.4/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
+-rw-r--r--   0        0        0     1534 2023-06-08 04:36:46.587922 bluecast-0.4/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
+-rw-r--r--   0        0        0     1502 2023-06-08 04:35:46.982972 bluecast-0.4/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
+-rw-r--r--   0        0        0     3666 2023-06-08 04:36:46.587922 bluecast-0.4/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
+-rw-r--r--   0        0        0     3656 2023-06-08 04:35:46.982972 bluecast-0.4/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
+-rw-r--r--   0        0        0     1771 2023-06-24 15:42:30.438842 bluecast-0.4/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
+-rw-r--r--   0        0        0     4575 2023-06-23 04:26:17.143641 bluecast-0.4/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
+-rw-r--r--   0        0        0     4561 2023-06-08 04:35:46.982972 bluecast-0.4/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
+-rw-r--r--   0        0        0     1167 2023-06-08 04:36:46.587922 bluecast-0.4/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
+-rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-0.4/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
+-rw-r--r--   0        0        0     1948 2023-06-08 06:48:48.640550 bluecast-0.4/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
+-rw-r--r--   0        0        0     1929 2023-06-08 04:53:15.604550 bluecast-0.4/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
+-rw-r--r--   0        0        0     4931 2023-06-08 04:36:46.591922 bluecast-0.4/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
+-rw-r--r--   0        0        0     5044 2023-06-08 04:35:46.982972 bluecast-0.4/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
+-rw-r--r--   0        0        0     2352 2023-06-23 04:26:17.187641 bluecast-0.4/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
+-rw-r--r--   0        0        0     1790 2023-06-08 04:35:46.982972 bluecast-0.4/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
+-rw-r--r--   0        0        0     1402 2023-06-21 05:07:47.892424 bluecast-0.4/bluecast/preprocessing/custom.py
+-rw-r--r--   0        0        0     1424 2023-06-08 04:28:32.971163 bluecast-0.4/bluecast/preprocessing/datetime_features.py
+-rw-r--r--   0        0        0     3122 2023-06-08 04:28:32.971163 bluecast-0.4/bluecast/preprocessing/encode_target_labels.py
+-rw-r--r--   0        0        0     1354 2023-06-23 13:12:42.063930 bluecast-0.4/bluecast/preprocessing/feature_selection.py
+-rw-r--r--   0        0        0     6190 2023-06-21 05:07:47.896425 bluecast-0.4/bluecast/preprocessing/feature_types.py
+-rw-r--r--   0        0        0      862 2023-06-08 04:28:32.971163 bluecast-0.4/bluecast/preprocessing/nulls_and_infs.py
+-rw-r--r--   0        0        0     1452 2023-06-08 06:48:42.348436 bluecast-0.4/bluecast/preprocessing/schema_checks.py
+-rw-r--r--   0        0        0     4561 2023-06-08 04:28:32.971163 bluecast-0.4/bluecast/preprocessing/target_encoding.py
+-rw-r--r--   0        0        0     2871 2023-06-21 05:07:47.896425 bluecast-0.4/bluecast/preprocessing/train_test_split.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.4/bluecast/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-0.4/bluecast/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7694 2023-06-24 15:54:26.806942 bluecast-0.4/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     3156 2023-06-07 13:42:51.261239 bluecast-0.4/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-0.4/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1137 2023-06-07 04:38:15.364753 bluecast-0.4/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-0.4/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4803 2023-06-07 13:42:51.269239 bluecast-0.4/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1597 2023-06-09 12:06:35.203065 bluecast-0.4/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-0.4/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-0.4/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-0.4/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4064 2023-06-24 15:55:25.448209 bluecast-0.4/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-0.4/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1449 2023-06-07 04:38:15.376753 bluecast-0.4/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-0.4/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.4/bluecast/tests/make_data/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-0.4/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-06-07 04:38:15.360753 bluecast-0.4/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
+-rw-r--r--   0        0        0     1289 2023-06-07 04:18:43.418068 bluecast-0.4/bluecast/tests/make_data/create_data.py
+-rw-r--r--   0        0        0     5759 2023-06-24 15:55:49.068680 bluecast-0.4/bluecast/tests/test_cast.py
+-rw-r--r--   0        0        0     1328 2023-06-07 13:40:33.489843 bluecast-0.4/bluecast/tests/test_check_gpu_support.py
+-rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-0.4/bluecast/tests/test_custom_processing_base_class.py
+-rw-r--r--   0        0        0     1097 2023-06-07 04:38:03.828575 bluecast-0.4/bluecast/tests/test_datetime_features.py
+-rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-0.4/bluecast/tests/test_encode_target_labels.py
+-rw-r--r--   0        0        0     2608 2023-06-07 13:42:39.380960 bluecast-0.4/bluecast/tests/test_feature_type_detector.py
+-rw-r--r--   0        0        0     1482 2023-06-09 05:52:17.052295 bluecast-0.4/bluecast/tests/test_load_for_production.py
+-rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-0.4/bluecast/tests/test_nulls_and_infs.py
+-rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-0.4/bluecast/tests/test_save_to_production.py
+-rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-0.4/bluecast/tests/test_schema_checks.py
+-rw-r--r--   0        0        0     2295 2023-06-24 15:55:23.176162 bluecast-0.4/bluecast/tests/test_shap_explanations.py
+-rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-0.4/bluecast/tests/test_target_encoding_binary.py
+-rw-r--r--   0        0        0      735 2023-06-07 04:38:03.832575 bluecast-0.4/bluecast/tests/test_target_encoding_multiclass.py
+-rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-0.4/bluecast/tests/test_train_test_split.py
+-rw-r--r--   0        0        0     1457 2023-06-24 15:42:22.706820 bluecast-0.4/pyproject.toml
+-rw-r--r--   0        0        0    18367 1970-01-01 00:00:00.000000 bluecast-0.4/PKG-INFO
```

### Comparing `bluecast-0.3.1/LICENSE` & `bluecast-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/README.md` & `bluecast-0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -236,26 +236,58 @@
 
 automl.fit(df_train, target_col="target")
 y_probs, y_classes = automl.predict(df_val)
 ```
 
 #### Custom feature selection
 
-As of version 0.3 BlueCast added automated feature selection. Also this
-step can be customized. An instance of `RFECV` is expected for `selection_strategy`.
-Otherwise the pipeline will fail. To disable feature selection set `execute_selection`
-to `False`. To surpass the `RFECV` limitation a custom feature selection algorithm
-can also be passed as part of a custom last mile computation.
+BlueCast offers automated feature selection. On default the feature
+selection is disabled, but BlueCast raises a warning to inform the
+user about this option. The behaviour can be controlled via the
+`TrainingConfig`.
+
+```sh
+from bluecast.blueprints.cast import BlueCast
+from bluecast.preprocessing.custom import CustomPreprocessing
+from bluecast.config.training_config import TrainingConfig
+
+# Create a custom training config and adjust general training parameters
+train_config = TrainingConfig()
+train_config.hyperparameter_tuning_rounds = 10
+train_config.autotune_model = False # we want to run just normal training, no hyperparameter tuning
+train_config.enable_feature_selection = True
+
+# Pass the custom configs to the BlueCast class
+automl = BlueCast(
+        class_problem="binary",
+        target_column="target"
+        conf_training=train_config,
+    )
+
+automl.fit(df_train, target_col="target")
+y_probs, y_classes = automl.predict(df_val)
+```
+
+Also this step can be customized. An instance of `RFECV` is expected for `selection_strategy`.
+Otherwise the pipeline will fail. To surpass the `RFECV` limitation a custom feature
+selection algorithm can also be passed as part of a custom last mile computation.
+Here is an example adjusting the in-built solution via `RFECV`:
 
 ```sh
 from bluecast.config.training_config import FeatureSelectionConfig
+from bluecast.config.training_config import TrainingConfig
 from sklearn.feature_selection import RFECV
 from sklearn.metrics import make_scorer, matthews_corrcoef
 from sklearn.model_selection import StratifiedKFold
 
+
+# Create a custom training config and adjust general training parameters
+train_config = TrainingConfig()
+train_config.enable_feature_selection = True
+
 # add custom feature selection
 custom_feat_sel = FeatureSelectionConfig()
 # custom_feat_sel.execute_selection = False
 custom_feat_sel.selection_strategy = RFECV(
     estimator=xgb.XGBClassifier(),
     step=1,
     cv=StratifiedKFold(10, random_state=0, shuffle=True),
@@ -265,14 +297,15 @@
 )
 
 # Create an instance of the BlueCast class with the custom model
 bluecast = BlueCast(
     class_problem="binary",
     target_column="target",
     conf_feature_selection=custom_feat_sel,
+    conf_training=train_config,
 
 # Create some sample data for testing
 x_train = pd.DataFrame(
     {"feature1": [i for i in range(10)], "feature2": [i for i in range(10)]}
 )
 y_train = pd.Series([0, 1, 0, 1, 0, 1, 0, 1, 0, 1])
 x_test = pd.DataFrame(
```

### Comparing `bluecast-0.3.1/bluecast/blueprints/__pycache__/cast.cpython-310.pyc` & `bluecast-0.4/bluecast/blueprints/__pycache__/cast.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 12:59:43 2023 UTC, .py size: 13297 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3f97 9564 f133 0000  o.......?..d.3..
+00000000: 6f0d 0d0a 0000 0000 0c10 9764 8a36 0000  o..........d.6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 0201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 0100 6401 6403 6c09 5a0a 6401  m.Z...d.d.l.Z.d.
 00000060: 6403 6c0b 5a0c 6401 6404 6c0d 6d0e 5a0e  d.l.Z.d.d.l.m.Z.
 00000070: 6d0f 5a0f 6d10 5a10 6d11 5a11 0100 6401  m.Z.m.Z.m.Z...d.
@@ -245,318 +245,355 @@
 00000f40: 5f3b 0000 0073 2800 0000 060f 0601 0601  _;...s(.........
 00000f50: 0601 0601 0601 0601 0601 0601 0601 0601  ................
 00000f60: 0601 0203 04fe 0603 0601 0601 0601 0601  ................
 00000f70: 0a01 7a11 426c 7565 4361 7374 2e5f 5f69  ..z.BlueCast.__i
 00000f80: 6e69 745f 5fda 0264 66da 0a74 6172 6765  nit__..df..targe
 00000f90: 745f 636f 6cda 0672 6574 7572 6e63 0300  t_col..returnc..
 00000fa0: 0000 0000 0000 0000 0000 0900 0000 0700  ................
-00000fb0: 0000 4300 0000 73ce 0200 0074 0083 0001  ..C...s....t....
+00000fb0: 0000 4300 0000 73f6 0200 0074 0083 0001  ..C...s....t....
 00000fc0: 0074 0183 007d 037c 03a0 027c 01a1 017d  .t...}.|...|...}
 00000fd0: 017c 037c 005f 037c 006a 036a 0472 297c  .|.|._.|.j.j.r)|
 00000fe0: 006a 057c 006a 036a 0476 0072 2974 0683  .j.|.j.j.v.r)t..
 00000ff0: 007c 005f 077c 006a 07a0 087c 017c 006a  .|._.|.j...|.|.j
 00001000: 0519 00a1 017c 017c 006a 053c 007c 006a  .....|.|.j.<.|.j
 00001010: 036a 047c 005f 047c 006a 036a 097c 005f  .j.|._.|.j.j.|._
-00001020: 097c 006a 0a73 3a74 0b83 007c 005f 0a74  .|.j.s:t...|._.t
-00001030: 0c7c 017c 027c 006a 0d7c 006a 0a6a 0e7c  .|.|.|.j.|.j.j.|
-00001040: 006a 0a6a 0f7c 006a 0a6a 1083 065c 047d  .j.j.|.j.j...\.}
-00001050: 047d 057d 067d 077c 006a 1172 927c 006a  .}.}.}.|.j.r.|.j
-00001060: 11a0 127c 047c 06a1 025c 027d 047d 067c  ...|.|...\.}.}.|
-00001070: 006a 116a 137c 057c 0764 0164 028d 035c  .j.j.|.|.d.d...\
-00001080: 027d 057d 0774 0183 007d 037c 03a0 027c  .}.}.t...}.|...|
-00001090: 04a1 017d 087c 046a 1464 0364 048d 017c  ...}.|.j.d.d...|
-000010a0: 066a 1464 0364 048d 0102 027d 047d 067c  .j.d.d.....}.}.|
-000010b0: 056a 1464 0364 048d 017c 076a 1464 0364  .j.d.d...|.j.d.d
-000010c0: 048d 0102 027d 057d 077c 027c 036a 0476  .....}.}.|.|.j.v
-000010d0: 0072 927c 036a 04a0 157c 02a1 0101 0074  .r.|.j...|.....t
-000010e0: 167c 0483 0174 167c 0583 0102 027d 047d  .|...t.|.....}.}
-000010f0: 0574 177c 047c 006a 0983 0274 177c 057c  .t.|.|.j...t.|.|
-00001100: 006a 0983 0202 027d 047d 0574 1883 007c  .j.....}.}.t...|
-00001110: 005f 197c 006a 19a0 1a7c 04a1 0101 007c  ._.|.j...|.....|
-00001120: 006a 19a0 137c 05a1 017d 057c 006a 0464  .j...|...}.|.j.d
-00001130: 0575 0172 d67c 006a 1b64 066b 0272 d674  .u.r.|.j.d.k.r.t
-00001140: 1c7c 036a 0483 017c 005f 1d7c 006a 1da0  .|.j...|._.|.j..
-00001150: 1e7c 047c 06a1 027d 047c 006a 1da0 1f7c  .|.|...}.|.j...|
-00001160: 05a1 017d 056e 1d7c 006a 0464 0575 0172  ...}.n.|.j.d.u.r
-00001170: f37c 006a 1b64 076b 0272 f374 207c 036a  .|.j.d.k.r.t |.j
-00001180: 0483 017c 005f 1d7c 006a 1da0 217c 047c  ...|._.|.j..!|.|
-00001190: 06a1 027d 047c 006a 1da0 227c 05a1 017d  ...}.|.j.."|...}
-000011a0: 057c 006a 2390 0172 0b7c 006a 23a0 127c  .|.j#..r.|.j#..|
-000011b0: 047c 06a1 025c 027d 047d 067c 006a 236a  .|...\.}.}.|.j#j
-000011c0: 137c 057c 0764 0164 028d 035c 027d 057d  .|.|.d.d...\.}.}
-000011d0: 077c 006a 2490 0173 1374 2583 007c 005f  .|.j$..s.t%..|._
-000011e0: 247c 006a 246a 2690 0172 2074 277c 006a  $|.j$j&..r t'|.j
-000011f0: 246a 2864 088d 017c 005f 297c 006a 2990  $j(d...|._)|.j).
-00001200: 0172 367c 006a 246a 2690 0172 367c 006a  .r6|.j$j&..r6|.j
-00001210: 29a0 127c 047c 06a1 027d 047c 006a 29a0  )..|.|...}.|.j).
-00001220: 137c 05a1 017d 057c 006a 2a90 0173 4774  .|...}.|.j*..sGt
-00001230: 2b7c 006a 1b7c 006a 0a7c 006a 2c7c 006a  +|.j.|.j.|.j,|.j
-00001240: 2d64 098d 047c 005f 2a7c 006a 2aa0 1a7c  -d...|._*|.j*..|
-00001250: 047c 057c 067c 07a1 0401 007c 006a 0a90  .|.|.|.....|.j..
-00001260: 0172 627c 006a 0a6a 2e90 0172 6274 2f7c  .rb|.j.j...rbt/|
-00001270: 006a 2a6a 307c 0564 0a83 037c 005f 3164  .j*j0|.d...|._1d
-00001280: 037c 005f 3264 0553 0029 0b7a 1954 7261  .|._2d.S.).z.Tra
-00001290: 696e 2061 2066 756c 6c20 4d4c 2070 6970  in a full ML pip
-000012a0: 656c 696e 652e 46a9 01da 0e70 7265 6469  eline.F....predi
-000012b0: 6374 6f6e 5f6d 6f64 6554 a901 da04 6472  cton_modeT....dr
-000012c0: 6f70 4e72 1d00 0000 721e 0000 0029 01da  opNr....r....)..
-000012d0: 1273 656c 6563 7469 6f6e 5f73 7472 6174  .selection_strat
-000012e0: 6567 7929 0372 2600 0000 7227 0000 0072  egy).r&...r'...r
-000012f0: 2800 0000 da04 7472 6565 2933 720f 0000  (.....tree)3r...
-00001300: 0072 1500 0000 5a1b 6669 745f 7472 616e  .r....Z.fit_tran
-00001310: 7366 6f72 6d5f 6665 6174 7572 655f 7479  sform_feature_ty
-00001320: 7065 7372 2c00 0000 7220 0000 0072 1f00  pesr,...r ...r..
-00001330: 0000 7213 0000 0072 2e00 0000 5a1b 6669  ..r....r....Z.fi
-00001340: 745f 7472 616e 7366 6f72 6d5f 7461 7267  t_transform_targ
-00001350: 6574 5f6c 6162 656c 7372 2100 0000 7226  et_labelsr!...r&
-00001360: 0000 0072 0a00 0000 721a 0000 0072 2200  ...r....r....r".
-00001370: 0000 da0a 7472 6169 6e5f 7369 7a65 5a13  ....train_sizeZ.
-00001380: 676c 6f62 616c 5f72 616e 646f 6d5f 7374  global_random_st
-00001390: 6174 655a 1474 7261 696e 5f73 706c 6974  ateZ.train_split
-000013a0: 5f73 7472 6174 6966 7972 2500 0000 da0d  _stratifyr%.....
-000013b0: 6669 745f 7472 616e 7366 6f72 6dda 0974  fit_transform..t
-000013c0: 7261 6e73 666f 726d da0b 7265 7365 745f  ransform..reset_
-000013d0: 696e 6465 78da 0672 656d 6f76 6572 1600  index..remover..
-000013e0: 0000 7212 0000 0072 1700 0000 722f 0000  ..r....r....r/..
-000013f0: 00da 0366 6974 721c 0000 0072 1800 0000  ...fitr....r....
-00001400: 722d 0000 005a 1e66 6974 5f74 6172 6765  r-...Z.fit_targe
-00001410: 745f 656e 636f 6465 5f62 696e 6172 795f  t_encode_binary_
-00001420: 636c 6173 73da 2474 7261 6e73 666f 726d  class.$transform
-00001430: 5f74 6172 6765 745f 656e 636f 6465 5f62  _target_encode_b
-00001440: 696e 6172 795f 636c 6173 7372 1900 0000  inary_classr....
-00001450: 5a1c 6669 745f 7461 7267 6574 5f65 6e63  Z.fit_target_enc
-00001460: 6f64 655f 6d75 6c74 6963 6c61 7373 da22  ode_multiclass."
-00001470: 7472 616e 7366 6f72 6d5f 7461 7267 6574  transform_target
-00001480: 5f65 6e63 6f64 655f 6d75 6c74 6963 6c61  _encode_multicla
-00001490: 7373 7224 0000 0072 2900 0000 7209 0000  ssr$...r)...r...
-000014a0: 00da 1165 7865 6375 7465 5f73 656c 6563  ...execute_selec
-000014b0: 7469 6f6e 7214 0000 0072 3c00 0000 722b  tionr....r<...r+
-000014c0: 0000 0072 2300 0000 7210 0000 0072 2700  ...r#...r....r'.
-000014d0: 0000 7228 0000 005a 1563 616c 6375 6c61  ..r(...Z.calcula
-000014e0: 7465 5f73 6861 705f 7661 6c75 6573 720e  te_shap_valuesr.
-000014f0: 0000 00da 056d 6f64 656c 7230 0000 0072  .....modelr0...r
-00001500: 2a00 0000 2909 7231 0000 0072 3500 0000  *...).r1...r5...
-00001510: 7236 0000 0072 2c00 0000 da07 785f 7472  r6...r,.....x_tr
-00001520: 6169 6eda 0678 5f74 6573 74da 0779 5f74  ain..x_test..y_t
-00001530: 7261 696e da06 795f 7465 7374 da01 5f72  rain..y_test.._r
-00001540: 3200 0000 7232 0000 0072 3300 0000 7243  2...r2...r3...rC
-00001550: 0000 0060 0000 0073 a400 0000 0602 0601  ...`...s........
-00001560: 0a01 0601 0802 0e01 0801 0603 0801 02ff  ................
-00001570: 02fe 0401 02ff 0a06 0a01 0602 0801 0202  ................
-00001580: 0201 0201 0401 0601 0601 0601 0cfa 0609  ................
-00001590: 1201 0601 0601 0aff 0603 0a01 0e01 0201  ................
-000015a0: 0aff 0e03 0201 0aff 0a03 0c01 1202 0c01  ................
-000015b0: 0601 08ff 0804 0c01 0c01 1402 0c01 0e01  ................
-000015c0: 0e01 1401 0c01 0e01 0c01 0802 0601 0401  ................
-000015d0: 08ff 0603 0601 0aff 0804 0801 0a02 0201  ................
-000015e0: 0601 08ff 1204 0e01 0c01 0802 0201 0401  ................
-000015f0: 0401 0401 0401 08fc 1206 1201 1201 0a01  ................
-00001600: 7a0c 426c 7565 4361 7374 2e66 6974 da07  z.BlueCast.fit..
-00001610: 6466 5f65 7661 6cda 0b74 6172 6765 745f  df_eval..target_
-00001620: 6576 616c 6305 0000 0000 0000 0000 0000  evalc...........
-00001630: 0008 0000 0004 0000 0043 0000 0073 2a00  .........C...s*.
-00001640: 0000 7c00 a000 7c01 7c04 a102 0100 7c00  ..|...|.|.....|.
-00001650: a001 7c02 a101 5c02 7d05 7d06 7402 7c03  ..|...\.}.}.t.|.
-00001660: 6a03 7c06 8302 7d07 7c07 5300 2901 618e  j.|...}.|.S.).a.
-00001670: 0200 0054 7261 696e 2061 2066 756c 6c20  ...Train a full 
-00001680: 4d4c 2070 6970 656c 696e 6520 616e 6420  ML pipeline and 
-00001690: 6576 616c 7561 7465 206f 6e20 6120 686f  evaluate on a ho
-000016a0: 6c64 6f75 7420 7365 742e 0a0a 2020 2020  ldout set...    
-000016b0: 2020 2020 5468 6973 2069 7320 6120 636f      This is a co
-000016c0: 6e76 656e 6965 6e63 6520 6675 6e63 7469  nvenience functi
-000016d0: 6f6e 2074 6f20 7472 6169 6e20 616e 6420  on to train and 
-000016e0: 6576 616c 7561 7465 206f 6e20 6120 686f  evaluate on a ho
-000016f0: 6c64 6f75 7420 7365 742e 2049 7420 6973  ldout set. It is
-00001700: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
-00001710: 7573 6520 7468 6973 2066 6f72 206d 6f64  use this for mod
-00001720: 656c 0a20 2020 2020 2020 2065 7870 6c6f  el.        explo
-00001730: 7261 7469 6f6e 2e20 4f6e 2070 726f 6475  ration. On produ
-00001740: 6374 696f 6e20 7468 6520 7369 6d70 6c65  ction the simple
-00001750: 2066 6974 2829 2066 756e 6374 696f 6e20   fit() function 
-00001760: 7368 6f75 6c64 2062 6520 7573 6564 2e0a  should be used..
-00001770: 2020 2020 2020 2020 3a70 6172 616d 203a          :param :
-00001780: 6466 3a20 5461 6b65 7320 6120 7061 6e64  df: Takes a pand
-00001790: 6173 2044 6174 6146 7261 6d65 2063 6f6e  as DataFrame con
-000017a0: 7461 696e 696e 6720 7468 6520 7472 6169  taining the trai
-000017b0: 6e69 6e67 2064 6174 6120 616e 6420 7468  ning data and th
-000017c0: 6520 7461 7267 6574 732e 0a20 2020 2020  e targets..     
-000017d0: 2020 203a 7061 7261 6d20 3a64 665f 6576     :param :df_ev
-000017e0: 616c 3a20 5461 6b65 7320 6120 7061 6e64  al: Takes a pand
-000017f0: 6173 2044 6174 6146 7261 6d65 2063 6f6e  as DataFrame con
-00001800: 7461 696e 696e 6720 7468 6520 6576 616c  taining the eval
-00001810: 7561 7469 6f6e 2064 6174 612c 2062 7574  uation data, but
-00001820: 206e 6f74 2074 6865 2074 6172 6765 7473   not the targets
-00001830: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00001840: 203a 7461 7267 6574 5f65 7661 6c3a 2054   :target_eval: T
-00001850: 616b 6573 2061 2070 616e 6461 7320 5365  akes a pandas Se
-00001860: 7269 6573 2063 6f6e 7461 696e 696e 6720  ries containing 
-00001870: 7468 6520 6576 616c 7561 7469 6f6e 2074  the evaluation t
-00001880: 6172 6765 7473 2e0a 2020 2020 2020 2020  argets..        
-00001890: 3a70 6172 616d 203a 7461 7267 6574 5f63  :param :target_c
-000018a0: 6f6c 3a20 5461 6b65 7320 6120 7374 7269  ol: Takes a stri
-000018b0: 6e67 2063 6f6e 7461 696e 696e 6720 7468  ng containing th
-000018c0: 6520 6e61 6d65 206f 6620 7468 6520 7461  e name of the ta
-000018d0: 7267 6574 2063 6f6c 756d 6e20 696e 7369  rget column insi
-000018e0: 6465 2074 6865 2074 7261 696e 696e 6720  de the training 
-000018f0: 6461 7461 2064 662e 0a20 2020 2020 2020  data df..       
-00001900: 2029 0472 4300 0000 da07 7072 6564 6963   ).rC.....predic
-00001910: 7472 0d00 0000 da06 7661 6c75 6573 2908  tr......values).
-00001920: 7231 0000 0072 3500 0000 724d 0000 0072  r1...r5...rM...r
-00001930: 4e00 0000 7236 0000 00da 0779 5f70 726f  N...r6.....y_pro
-00001940: 6273 da09 795f 636c 6173 7365 735a 0965  bs..y_classesZ.e
-00001950: 7661 6c5f 6469 6374 7232 0000 0072 3200  val_dictr2...r2.
-00001960: 0000 7233 0000 00da 0866 6974 5f65 7661  ..r3.....fit_eva
-00001970: 6cc1 0000 0073 0800 0000 0c10 0e01 0c01  l....s..........
-00001980: 0401 7a11 426c 7565 4361 7374 2e66 6974  ..z.BlueCast.fit
-00001990: 5f65 7661 6c63 0200 0000 0000 0000 0000  _evalc..........
-000019a0: 0000 0300 0000 0400 0000 4300 0000 7318  ..........C...s.
-000019b0: 0100 0074 0083 0001 007c 006a 0173 0a74  ...t.....|.j.s.t
-000019c0: 0264 0183 0182 017c 006a 016a 037c 017c  .d.....|.j.j.|.|
-000019d0: 006a 0467 0164 028d 027d 017c 006a 0572  .j.g.d...}.|.j.r
-000019e0: 277c 006a 056a 067c 0164 0364 048d 025c  '|.j.j.|.d.d...\
-000019f0: 027d 017d 027c 016a 0764 0364 058d 017d  .}.}.|.j.d.d...}
-00001a00: 0174 087c 0183 017d 0174 097c 017c 006a  .t.|...}.t.|.|.j
-00001a10: 0a83 027d 017c 006a 0b72 3a7c 006a 0ba0  ...}.|.j.r:|.j..
-00001a20: 067c 01a1 017d 017c 006a 0c72 527c 006a  .|...}.|.j.rR|.j
-00001a30: 0d72 527c 006a 0e64 066b 0272 5274 0f7c  .rR|.j.d.k.rRt.|
-00001a40: 006a 0d74 1083 0272 527c 006a 0da0 117c  .j.t...rR|.j...|
-00001a50: 01a1 017d 016e 177c 006a 0c72 697c 006a  ...}.n.|.j.ri|.j
-00001a60: 0d72 697c 006a 0e64 076b 0272 6974 0f7c  .ri|.j.d.k.rit.|
-00001a70: 006a 0d74 1283 0272 697c 006a 0da0 137c  .j.t...ri|.j...|
-00001a80: 01a1 017d 017c 006a 1472 767c 006a 146a  ...}.|.j.rv|.j.j
-00001a90: 067c 0164 0364 048d 025c 027d 017d 027c  .|.d.d...\.}.}.|
-00001aa0: 006a 1573 7d74 1683 007c 005f 157c 006a  .j.s}t...|._.|.j
-00001ab0: 1772 8a7c 006a 156a 1872 8a7c 006a 17a0  .r.|.j.j.r.|.j..
-00001ac0: 067c 01a1 017d 017c 0153 0029 087a 3754  .|...}.|.S.).z7T
-00001ad0: 7261 6e73 666f 726d 206e 6577 2064 6174  ransform new dat
-00001ae0: 6120 6163 636f 7264 696e 6720 746f 2070  a according to p
-00001af0: 7265 7072 6f63 6573 7369 6e67 2070 6970  reprocessing pip
-00001b00: 656c 696e 652e fa2a 4665 6174 7572 6520  eline..*Feature 
-00001b10: 7479 7065 2063 6f6e 7665 7274 6572 2063  type converter c
-00001b20: 6f75 6c64 206e 6f74 2062 6520 666f 756e  ould not be foun
-00001b30: 642e 2901 5a0b 6967 6e6f 7265 5f63 6f6c  d.).Z.ignore_col
-00001b40: 7354 7238 0000 0072 3a00 0000 721d 0000  sTr8...r:...r...
-00001b50: 0072 1e00 0000 2919 720f 0000 0072 2c00  .r....).r....r,.
-00001b60: 0000 da09 4578 6365 7074 696f 6e5a 1774  ....ExceptionZ.t
-00001b70: 7261 6e73 666f 726d 5f66 6561 7475 7265  ransform_feature
-00001b80: 5f74 7970 6573 721f 0000 0072 2500 0000  _typesr....r%...
-00001b90: 7240 0000 0072 4100 0000 7216 0000 0072  r@...rA...r....r
-00001ba0: 1200 0000 7221 0000 0072 2f00 0000 7220  ....r!...r/...r 
-00001bb0: 0000 0072 2d00 0000 721c 0000 00da 0a69  ...r-...r......i
-00001bc0: 7369 6e73 7461 6e63 6572 1800 0000 7244  sinstancer....rD
-00001bd0: 0000 0072 1900 0000 7245 0000 0072 2400  ...r....rE...r$.
-00001be0: 0000 7229 0000 0072 0900 0000 722b 0000  ..r)...r....r+..
-00001bf0: 0072 4600 0000 2903 7231 0000 0072 3500  .rF...).r1...r5.
-00001c00: 0000 724c 0000 0072 3200 0000 7232 0000  ..rL...r2...r2..
-00001c10: 0072 3300 0000 da12 7472 616e 7366 6f72  .r3.....transfor
-00001c20: 6d5f 6e65 775f 6461 7461 d600 0000 7348  m_new_data....sH
-00001c30: 0000 0006 0206 0108 0106 0208 0106 ff06  ................
-00001c40: 0414 010c 0108 020c 0106 020c 0104 0302  ................
-00001c50: ff04 0202 fe0a 030a 0102 ff0e 0304 0202  ................
-00001c60: ff04 0202 fe0a 030a 0102 ff0c 0306 0214  ................
-00001c70: 0106 0208 010e 020c 0104 027a 1b42 6c75  ...........z.Blu
-00001c80: 6543 6173 742e 7472 616e 7366 6f72 6d5f  eCast.transform_
-00001c90: 6e65 775f 6461 7461 6302 0000 0000 0000  new_datac.......
-00001ca0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
-00001cb0: 0073 8000 0000 7c00 6a00 7307 7401 6401  .s....|.j.s.t.d.
-00001cc0: 8301 8201 7c00 6a02 730e 7401 6402 8301  ....|.j.s.t.d...
-00001cd0: 8201 7403 8300 0100 7c00 a004 7c01 a101  ..t.....|...|...
-00001ce0: 7d01 7405 6403 8301 0100 7c00 6a00 a006  }.t.d.....|.j...
-00001cf0: 7c01 a101 5c02 7d02 7d03 7c00 6a02 6a07  |...\.}.}.|.j.j.
-00001d00: 723c 7c00 6a08 7c00 6a02 6a07 7600 723c  r<|.j.|.j.j.v.r<
-00001d10: 7c00 6a09 723c 7c00 6a02 723c 7c00 6a09  |.j.r<|.j.r<|.j.
-00001d20: a00a 740b a00c 7c03 a101 a101 7d03 7c02  ..t...|.....}.|.
-00001d30: 7c03 6602 5300 2904 7a90 5072 6564 6963  |.f.S.).z.Predic
-00001d40: 7420 6f6e 2075 6e73 6565 6e20 6461 7461  t on unseen data
-00001d50: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00001d60: 6e20 7468 6520 7072 6564 6963 7465 6420  n the predicted 
-00001d70: 7072 6f62 6162 696c 6974 6965 7320 616e  probabilities an
-00001d80: 6420 7468 6520 7072 6564 6963 7465 6420  d the predicted 
-00001d90: 636c 6173 7365 733a 0a20 2020 2020 2020  classes:.       
-00001da0: 2079 5f70 726f 6273 2c20 795f 636c 6173   y_probs, y_clas
-00001db0: 7365 7320 3d20 7072 6564 6963 7428 6466  ses = predict(df
-00001dc0: 290a 2020 2020 2020 2020 7a1b 4d6c 206d  ).        z.Ml m
-00001dd0: 6f64 656c 2063 6f75 6c64 206e 6f74 2062  odel could not b
-00001de0: 6520 666f 756e 6472 5400 0000 7a0d 5072  e foundrT...z.Pr
-00001df0: 6564 6963 7469 6e67 2e2e 2e29 0d72 2300  edicting...).r#.
-00001e00: 0000 7255 0000 0072 2c00 0000 720f 0000  ..rU...r,...r...
-00001e10: 0072 5700 0000 da05 7072 696e 7472 4f00  .rW.....printrO.
-00001e20: 0000 7220 0000 0072 1f00 0000 722e 0000  ..r ...r....r...
-00001e30: 005a 1f6c 6162 656c 5f65 6e63 6f64 6572  .Z.label_encoder
-00001e40: 5f72 6576 6572 7365 5f74 7261 6e73 666f  _reverse_transfo
-00001e50: 726d da02 7064 da06 5365 7269 6573 2904  rm..pd..Series).
-00001e60: 7231 0000 0072 3500 0000 7251 0000 0072  r1...r5...rQ...r
-00001e70: 5200 0000 7232 0000 0072 3200 0000 7233  R...r2...r2...r3
-00001e80: 0000 0072 4f00 0000 0401 0000 7324 0000  ...rO.......s$..
-00001e90: 0006 0608 0106 0208 0106 020a 0108 0210  ................
-00001ea0: 0108 020e 0204 0102 ff04 0202 fe06 0408  ................
-00001eb0: 0104 ff08 047a 1042 6c75 6543 6173 742e  .....z.BlueCast.
-00001ec0: 7072 6564 6963 7429 0a4e 4e4e 4e4e 4e4e  predict).NNNNNNN
-00001ed0: 4e4e 4e29 1eda 085f 5f6e 616d 655f 5fda  NNN)...__name__.
-00001ee0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00001ef0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
-00001f00: 5f5f 7205 0000 0072 0800 0000 da03 7374  __r....r......st
-00001f10: 72da 0566 6c6f 6174 da03 696e 7472 0600  r..float..intr..
-00001f20: 0000 7204 0000 0072 1000 0000 7202 0000  ..r....r....r...
-00001f30: 0072 1100 0000 720a 0000 0072 0c00 0000  .r....r....r....
-00001f40: 720b 0000 0072 0900 0000 7234 0000 0072  r....r....r4...r
-00001f50: 5900 0000 da09 4461 7461 4672 616d 6572  Y.....DataFramer
-00001f60: 4300 0000 725a 0000 0072 0300 0000 7253  C...rZ...r....rS
-00001f70: 0000 0072 5700 0000 7207 0000 00da 026e  ...rW...r......n
-00001f80: 70da 076e 6461 7272 6179 724f 0000 0072  p..ndarrayrO...r
-00001f90: 3200 0000 7232 0000 0072 3200 0000 7233  2...r2...r2...r3
-00001fa0: 0000 0072 1b00 0000 2600 0000 7366 0000  ...r....&...sf..
-00001fb0: 0008 0004 0102 1802 0102 0102 0102 0102  ................
-00001fc0: 0102 0102 0102 0102 0104 f306 0202 fe0c  ................
-00001fd0: 0302 fd14 0402 fc14 0502 fb06 0602 fa0e  ................
-00001fe0: 0702 f906 0802 f806 0902 f706 0a02 f606  ................
-00001ff0: 0b02 f506 0c02 f406 0d0a f318 2502 6104  ............%.a.
-00002000: 0202 fe04 0302 fd04 0402 fc02 0502 fb0a  ................
-00002010: 060a fa16 1524 2e72 1b00 0000 292e 725e  .....$.r....).r^
-00002020: 0000 00da 0674 7970 696e 6772 0200 0000  .....typingr....
-00002030: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
-00002040: 0600 0000 7207 0000 0072 0800 0000 da05  ....r....r......
-00002050: 6e75 6d70 7972 6300 0000 da06 7061 6e64  numpyrc.....pand
-00002060: 6173 7259 0000 00da 1f62 6c75 6563 6173  asrY.....bluecas
-00002070: 742e 636f 6e66 6967 2e74 7261 696e 696e  t.config.trainin
-00002080: 675f 636f 6e66 6967 7209 0000 0072 0a00  g_configr....r..
-00002090: 0000 720b 0000 0072 0c00 0000 5a20 626c  ..r....r....Z bl
-000020a0: 7565 6361 7374 2e65 7661 6c75 6174 696f  uecast.evaluatio
-000020b0: 6e2e 6576 616c 5f6d 6574 7269 6373 720d  n.eval_metricsr.
-000020c0: 0000 005a 1f62 6c75 6563 6173 742e 6576  ...Z.bluecast.ev
-000020d0: 616c 7561 7469 6f6e 2e73 6861 705f 7661  aluation.shap_va
-000020e0: 6c75 6573 720e 0000 005a 2462 6c75 6563  luesr....Z$bluec
-000020f0: 6173 742e 6765 6e65 7261 6c5f 7574 696c  ast.general_util
-00002100: 732e 6765 6e65 7261 6c5f 7574 696c 7372  s.general_utilsr
-00002110: 0f00 0000 5a1d 626c 7565 6361 7374 2e6d  ....Z.bluecast.m
-00002120: 6c5f 6d6f 6465 6c6c 696e 672e 7867 626f  l_modelling.xgbo
-00002130: 6f73 7472 1000 0000 da1d 626c 7565 6361  ostr......blueca
-00002140: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
-00002150: 2e63 7573 746f 6d72 1100 0000 5a28 626c  .customr....Z(bl
-00002160: 7565 6361 7374 2e70 7265 7072 6f63 6573  uecast.preproces
-00002170: 7369 6e67 2e64 6174 6574 696d 655f 6665  sing.datetime_fe
-00002180: 6174 7572 6573 7212 0000 005a 2b62 6c75  aturesr....Z+blu
-00002190: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
-000021a0: 696e 672e 656e 636f 6465 5f74 6172 6765  ing.encode_targe
-000021b0: 745f 6c61 6265 6c73 7213 0000 005a 2862  t_labelsr....Z(b
-000021c0: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
-000021d0: 7373 696e 672e 6665 6174 7572 655f 7365  ssing.feature_se
-000021e0: 6c65 6374 696f 6e72 1400 0000 5a24 626c  lectionr....Z$bl
-000021f0: 7565 6361 7374 2e70 7265 7072 6f63 6573  uecast.preproces
-00002200: 7369 6e67 2e66 6561 7475 7265 5f74 7970  sing.feature_typ
-00002210: 6573 7215 0000 005a 2562 6c75 6563 6173  esr....Z%bluecas
-00002220: 742e 7072 6570 726f 6365 7373 696e 672e  t.preprocessing.
-00002230: 6e75 6c6c 735f 616e 645f 696e 6673 7216  nulls_and_infsr.
-00002240: 0000 005a 2462 6c75 6563 6173 742e 7072  ...Z$bluecast.pr
-00002250: 6570 726f 6365 7373 696e 672e 7363 6865  eprocessing.sche
-00002260: 6d61 5f63 6865 636b 7372 1700 0000 5a26  ma_checksr....Z&
-00002270: 626c 7565 6361 7374 2e70 7265 7072 6f63  bluecast.preproc
-00002280: 6573 7369 6e67 2e74 6172 6765 745f 656e  essing.target_en
-00002290: 636f 6469 6e67 7218 0000 0072 1900 0000  codingr....r....
-000022a0: 5a27 626c 7565 6361 7374 2e70 7265 7072  Z'bluecast.prepr
-000022b0: 6f63 6573 7369 6e67 2e74 7261 696e 5f74  ocessing.train_t
-000022c0: 6573 745f 7370 6c69 7472 1a00 0000 721b  est_splitr....r.
-000022d0: 0000 0072 3200 0000 7232 0000 0072 3200  ...r2...r2...r2.
-000022e0: 0000 7233 0000 00da 083c 6d6f 6475 6c65  ..r3.....<module
-000022f0: 3e01 0000 0073 2600 0000 0400 2408 0802  >....s&.....$...
-00002300: 0801 1802 0c06 0c01 0c01 0c01 0c01 0c01  ................
-00002310: 0c01 0c01 0c01 0c01 0c01 1001 0c04 1203  ................
+00001020: 097c 006a 0a73 3a74 0b83 007c 005f 0a7c  .|.j.s:t...|._.|
+00001030: 006a 0a6a 0c73 4274 0d64 0183 0182 017c  .j.j.sBt.d.....|
+00001040: 006a 0a6a 0e64 026b 0272 4c74 0d64 0383  .j.j.d.k.rLt.d..
+00001050: 0182 0174 0f7c 017c 027c 006a 107c 006a  ...t.|.|.|.j.|.j
+00001060: 0a6a 117c 006a 0a6a 127c 006a 0a6a 1383  .j.|.j.j.|.j.j..
+00001070: 065c 047d 047d 057d 067d 077c 006a 1472  .\.}.}.}.}.|.j.r
+00001080: a47c 006a 14a0 157c 047c 06a1 025c 027d  .|.j...|.|...\.}
+00001090: 047d 067c 006a 146a 167c 057c 0764 0464  .}.|.j.j.|.|.d.d
+000010a0: 058d 035c 027d 057d 0774 0183 007d 037c  ...\.}.}.t...}.|
+000010b0: 03a0 027c 04a1 017d 087c 046a 1764 0664  ...|...}.|.j.d.d
+000010c0: 078d 017c 066a 1764 0664 078d 0102 027d  ...|.j.d.d.....}
+000010d0: 047d 067c 056a 1764 0664 078d 017c 076a  .}.|.j.d.d...|.j
+000010e0: 1764 0664 078d 0102 027d 057d 077c 027c  .d.d.....}.}.|.|
+000010f0: 036a 0476 0072 a47c 036a 04a0 187c 02a1  .j.v.r.|.j...|..
+00001100: 0101 0074 197c 0483 0174 197c 0583 0102  ...t.|...t.|....
+00001110: 027d 047d 0574 1a7c 047c 006a 0983 0274  .}.}.t.|.|.j...t
+00001120: 1a7c 057c 006a 0983 0202 027d 047d 0574  .|.|.j.....}.}.t
+00001130: 1b83 007c 005f 1c7c 006a 1ca0 1d7c 04a1  ...|._.|.j...|..
+00001140: 0101 007c 006a 1ca0 167c 05a1 017d 057c  ...|.j...|...}.|
+00001150: 006a 0464 0875 0172 e87c 006a 1e64 096b  .j.d.u.r.|.j.d.k
+00001160: 0272 e874 1f7c 036a 0483 017c 005f 207c  .r.t.|.j...|._ |
+00001170: 006a 20a0 217c 047c 06a1 027d 047c 006a  .j .!|.|...}.|.j
+00001180: 20a0 227c 05a1 017d 056e 1f7c 006a 0464   ."|...}.n.|.j.d
+00001190: 0875 0190 0172 077c 006a 1e64 0a6b 0290  .u...r.|.j.d.k..
+000011a0: 0172 0774 237c 036a 0483 017c 005f 207c  .r.t#|.j...|._ |
+000011b0: 006a 20a0 247c 047c 06a1 027d 047c 006a  .j .$|.|...}.|.j
+000011c0: 20a0 257c 05a1 017d 057c 006a 2690 0172   .%|...}.|.j&..r
+000011d0: 1f7c 006a 26a0 157c 047c 06a1 025c 027d  .|.j&..|.|...\.}
+000011e0: 047d 067c 006a 266a 167c 057c 0764 0464  .}.|.j&j.|.|.d.d
+000011f0: 058d 035c 027d 057d 077c 006a 2790 0173  ...\.}.}.|.j'..s
+00001200: 2774 2883 007c 005f 277c 006a 0a6a 0c90  't(..|._'|.j.j..
+00001210: 0172 3474 297c 006a 276a 2a64 0b8d 017c  .r4t)|.j'j*d...|
+00001220: 005f 2b7c 006a 2b90 0172 4a7c 006a 0a6a  ._+|.j+..rJ|.j.j
+00001230: 0c90 0172 4a7c 006a 2ba0 157c 047c 06a1  ...rJ|.j+..|.|..
+00001240: 027d 047c 006a 2ba0 167c 05a1 017d 057c  .}.|.j+..|...}.|
+00001250: 006a 2c90 0173 5b74 2d7c 006a 1e7c 006a  .j,..s[t-|.j.|.j
+00001260: 0a7c 006a 2e7c 006a 2f64 0c8d 047c 005f  .|.j.|.j/d...|._
+00001270: 2c7c 006a 2ca0 1d7c 047c 057c 067c 07a1  ,|.j,..|.|.|.|..
+00001280: 0401 007c 006a 0a90 0172 767c 006a 0a6a  ...|.j...rv|.j.j
+00001290: 3090 0172 7674 317c 006a 2c6a 327c 0564  0..rvt1|.j,j2|.d
+000012a0: 0d83 037c 005f 3364 067c 005f 3464 0853  ...|._3d.|._4d.S
+000012b0: 0029 0e7a 1954 7261 696e 2061 2066 756c  .).z.Train a ful
+000012c0: 6c20 4d4c 2070 6970 656c 696e 652e 7ade  l ML pipeline.z.
+000012d0: 4665 6174 7572 6520 7365 6c65 6374 696f  Feature selectio
+000012e0: 6e20 6973 2064 6973 6162 6c65 642e 2055  n is disabled. U
+000012f0: 7064 6174 6520 7468 6520 5472 6169 6e69  pdate the Traini
+00001300: 6e67 436f 6e66 6967 2070 6172 616d 2027  ngConfig param '
+00001310: 656e 6162 6c65 5f66 6561 7475 7265 5f73  enable_feature_s
+00001320: 656c 6563 7469 6f6e 270a 2020 2020 2020  election'.      
+00001330: 2020 2020 2020 746f 2065 6e61 626c 6520        to enable 
+00001340: 6974 206f 7220 6d61 6b65 2075 7365 206f  it or make use o
+00001350: 6620 6120 6375 7374 6f6d 2070 7265 7072  f a custom prepr
+00001360: 6f63 6573 736f 7220 746f 2064 6f20 6974  ocessor to do it
+00001370: 206d 616e 7561 6c6c 7920 6475 7269 6e67   manually during
+00001380: 2074 6865 206c 6173 7420 6d69 6c65 2063   the last mile c
+00001390: 6f6d 7075 7461 7469 6f6e 7320 7374 6570  omputations step
+000013a0: 2e0a 2020 2020 2020 2020 2020 2020 e901  ..            ..
+000013b0: 0000 0061 0601 0000 4372 6f73 7320 7661  ...a....Cross va
+000013c0: 6c69 6461 7469 6f6e 2069 7320 6469 7361  lidation is disa
+000013d0: 626c 6564 2e20 5570 6461 7465 2074 6865  bled. Update the
+000013e0: 2054 7261 696e 696e 6743 6f6e 6669 6720   TrainingConfig 
+000013f0: 7061 7261 6d20 2768 7970 6572 7475 6e69  param 'hypertuni
+00001400: 6e67 5f63 765f 666f 6c64 7327 200a 2020  ng_cv_folds' .  
+00001410: 2020 2020 2020 2020 2020 746f 2065 6e61            to ena
+00001420: 626c 6520 6974 2e20 4372 6f73 7320 7661  ble it. Cross va
+00001430: 6c69 6461 7469 6f6e 2069 7320 6469 7361  lidation is disa
+00001440: 626c 6564 206f 6e20 6465 6661 796c 7420  bled on defaylt 
+00001450: 746f 2061 6c6c 6f77 2066 6173 7420 7072  to allow fast pr
+00001460: 6f74 6f74 7970 696e 672e 2046 6f72 2072  ototyping. For r
+00001470: 6f62 7573 7420 6879 7065 7270 6172 616d  obust hyperparam
+00001480: 6574 6572 0a20 2020 2020 2020 2020 2020  eter.           
+00001490: 2074 756e 696e 6720 7573 696e 6720 6174   tuning using at
+000014a0: 206c 6561 7374 2035 2066 6f6c 6473 2069   least 5 folds i
+000014b0: 7320 7265 636f 6d6d 656e 6465 642e 46a9  s recommended.F.
+000014c0: 01da 0e70 7265 6469 6374 6f6e 5f6d 6f64  ...predicton_mod
+000014d0: 6554 a901 da04 6472 6f70 4e72 1d00 0000  eT....dropNr....
+000014e0: 721e 0000 0029 01da 1273 656c 6563 7469  r....)...selecti
+000014f0: 6f6e 5f73 7472 6174 6567 7929 0372 2600  on_strategy).r&.
+00001500: 0000 7227 0000 0072 2800 0000 da04 7472  ..r'...r(.....tr
+00001510: 6565 2935 720f 0000 0072 1500 0000 5a1b  ee)5r....r....Z.
+00001520: 6669 745f 7472 616e 7366 6f72 6d5f 6665  fit_transform_fe
+00001530: 6174 7572 655f 7479 7065 7372 2c00 0000  ature_typesr,...
+00001540: 7220 0000 0072 1f00 0000 7213 0000 0072  r ...r....r....r
+00001550: 2e00 0000 5a1b 6669 745f 7472 616e 7366  ....Z.fit_transf
+00001560: 6f72 6d5f 7461 7267 6574 5f6c 6162 656c  orm_target_label
+00001570: 7372 2100 0000 7226 0000 0072 0a00 0000  sr!...r&...r....
+00001580: da18 656e 6162 6c65 5f66 6561 7475 7265  ..enable_feature
+00001590: 5f73 656c 6563 7469 6f6e da07 5761 726e  _selection..Warn
+000015a0: 696e 675a 1468 7970 6572 7475 6e69 6e67  ingZ.hypertuning
+000015b0: 5f63 765f 666f 6c64 7372 1a00 0000 7222  _cv_foldsr....r"
+000015c0: 0000 00da 0a74 7261 696e 5f73 697a 655a  .....train_sizeZ
+000015d0: 1367 6c6f 6261 6c5f 7261 6e64 6f6d 5f73  .global_random_s
+000015e0: 7461 7465 5a14 7472 6169 6e5f 7370 6c69  tateZ.train_spli
+000015f0: 745f 7374 7261 7469 6679 7225 0000 00da  t_stratifyr%....
+00001600: 0d66 6974 5f74 7261 6e73 666f 726d da09  .fit_transform..
+00001610: 7472 616e 7366 6f72 6dda 0b72 6573 6574  transform..reset
+00001620: 5f69 6e64 6578 da06 7265 6d6f 7665 7216  _index..remover.
+00001630: 0000 0072 1200 0000 7217 0000 0072 2f00  ...r....r....r/.
+00001640: 0000 da03 6669 7472 1c00 0000 7218 0000  ....fitr....r...
+00001650: 0072 2d00 0000 5a1e 6669 745f 7461 7267  .r-...Z.fit_targ
+00001660: 6574 5f65 6e63 6f64 655f 6269 6e61 7279  et_encode_binary
+00001670: 5f63 6c61 7373 da24 7472 616e 7366 6f72  _class.$transfor
+00001680: 6d5f 7461 7267 6574 5f65 6e63 6f64 655f  m_target_encode_
+00001690: 6269 6e61 7279 5f63 6c61 7373 7219 0000  binary_classr...
+000016a0: 005a 1c66 6974 5f74 6172 6765 745f 656e  .Z.fit_target_en
+000016b0: 636f 6465 5f6d 756c 7469 636c 6173 73da  code_multiclass.
+000016c0: 2274 7261 6e73 666f 726d 5f74 6172 6765  "transform_targe
+000016d0: 745f 656e 636f 6465 5f6d 756c 7469 636c  t_encode_multicl
+000016e0: 6173 7372 2400 0000 7229 0000 0072 0900  assr$...r)...r..
+000016f0: 0000 7214 0000 0072 3d00 0000 722b 0000  ..r....r=...r+..
+00001700: 0072 2300 0000 7210 0000 0072 2700 0000  .r#...r....r'...
+00001710: 7228 0000 005a 1563 616c 6375 6c61 7465  r(...Z.calculate
+00001720: 5f73 6861 705f 7661 6c75 6573 720e 0000  _shap_valuesr...
+00001730: 00da 056d 6f64 656c 7230 0000 0072 2a00  ...modelr0...r*.
+00001740: 0000 2909 7231 0000 0072 3500 0000 7236  ..).r1...r5...r6
+00001750: 0000 0072 2c00 0000 da07 785f 7472 6169  ...r,.....x_trai
+00001760: 6eda 0678 5f74 6573 74da 0779 5f74 7261  n..x_test..y_tra
+00001770: 696e da06 795f 7465 7374 da01 5f72 3200  in..y_test.._r2.
+00001780: 0000 7232 0000 0072 3300 0000 7246 0000  ..r2...r3...rF..
+00001790: 0060 0000 0073 ac00 0000 0602 0601 0a01  .`...s..........
+000017a0: 0601 0802 0e01 0801 0603 0801 02ff 02fe  ................
+000017b0: 0401 02ff 0a06 0a01 0602 0801 0802 0801  ................
+000017c0: 0c04 0801 0204 0201 0201 0401 0601 0601  ................
+000017d0: 0601 0cfa 0609 1201 0601 0601 0aff 0603  ................
+000017e0: 0a01 0e01 0201 0aff 0e03 0201 0aff 0a03  ................
+000017f0: 0c01 1202 0c01 0601 08ff 0804 0c01 0c01  ................
+00001800: 1402 0c01 0e01 0e01 1801 0c01 0e01 0c01  ................
+00001810: 0802 0601 0401 08ff 0603 0601 0aff 0804  ................
+00001820: 0801 0a02 0201 0601 08ff 1204 0e01 0c01  ................
+00001830: 0802 0201 0401 0401 0401 0401 08fc 1206  ................
+00001840: 1201 1201 0a01 7a0c 426c 7565 4361 7374  ......z.BlueCast
+00001850: 2e66 6974 da07 6466 5f65 7661 6cda 0b74  .fit..df_eval..t
+00001860: 6172 6765 745f 6576 616c 6305 0000 0000  arget_evalc.....
+00001870: 0000 0000 0000 0008 0000 0004 0000 0043  ...............C
+00001880: 0000 0073 2a00 0000 7c00 a000 7c01 7c04  ...s*...|...|.|.
+00001890: a102 0100 7c00 a001 7c02 a101 5c02 7d05  ....|...|...\.}.
+000018a0: 7d06 7402 7c03 6a03 7c06 8302 7d07 7c07  }.t.|.j.|...}.|.
+000018b0: 5300 2901 618e 0200 0054 7261 696e 2061  S.).a....Train a
+000018c0: 2066 756c 6c20 4d4c 2070 6970 656c 696e   full ML pipelin
+000018d0: 6520 616e 6420 6576 616c 7561 7465 206f  e and evaluate o
+000018e0: 6e20 6120 686f 6c64 6f75 7420 7365 742e  n a holdout set.
+000018f0: 0a0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
+00001900: 7320 6120 636f 6e76 656e 6965 6e63 6520  s a convenience 
+00001910: 6675 6e63 7469 6f6e 2074 6f20 7472 6169  function to trai
+00001920: 6e20 616e 6420 6576 616c 7561 7465 206f  n and evaluate o
+00001930: 6e20 6120 686f 6c64 6f75 7420 7365 742e  n a holdout set.
+00001940: 2049 7420 6973 2072 6563 6f6d 6d65 6e64   It is recommend
+00001950: 6564 2074 6f20 7573 6520 7468 6973 2066  ed to use this f
+00001960: 6f72 206d 6f64 656c 0a20 2020 2020 2020  or model.       
+00001970: 2065 7870 6c6f 7261 7469 6f6e 2e20 4f6e   exploration. On
+00001980: 2070 726f 6475 6374 696f 6e20 7468 6520   production the 
+00001990: 7369 6d70 6c65 2066 6974 2829 2066 756e  simple fit() fun
+000019a0: 6374 696f 6e20 7368 6f75 6c64 2062 6520  ction should be 
+000019b0: 7573 6564 2e0a 2020 2020 2020 2020 3a70  used..        :p
+000019c0: 6172 616d 203a 6466 3a20 5461 6b65 7320  aram :df: Takes 
+000019d0: 6120 7061 6e64 6173 2044 6174 6146 7261  a pandas DataFra
+000019e0: 6d65 2063 6f6e 7461 696e 696e 6720 7468  me containing th
+000019f0: 6520 7472 6169 6e69 6e67 2064 6174 6120  e training data 
+00001a00: 616e 6420 7468 6520 7461 7267 6574 732e  and the targets.
+00001a10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001a20: 3a64 665f 6576 616c 3a20 5461 6b65 7320  :df_eval: Takes 
+00001a30: 6120 7061 6e64 6173 2044 6174 6146 7261  a pandas DataFra
+00001a40: 6d65 2063 6f6e 7461 696e 696e 6720 7468  me containing th
+00001a50: 6520 6576 616c 7561 7469 6f6e 2064 6174  e evaluation dat
+00001a60: 612c 2062 7574 206e 6f74 2074 6865 2074  a, but not the t
+00001a70: 6172 6765 7473 2e0a 2020 2020 2020 2020  argets..        
+00001a80: 3a70 6172 616d 203a 7461 7267 6574 5f65  :param :target_e
+00001a90: 7661 6c3a 2054 616b 6573 2061 2070 616e  val: Takes a pan
+00001aa0: 6461 7320 5365 7269 6573 2063 6f6e 7461  das Series conta
+00001ab0: 696e 696e 6720 7468 6520 6576 616c 7561  ining the evalua
+00001ac0: 7469 6f6e 2074 6172 6765 7473 2e0a 2020  tion targets..  
+00001ad0: 2020 2020 2020 3a70 6172 616d 203a 7461        :param :ta
+00001ae0: 7267 6574 5f63 6f6c 3a20 5461 6b65 7320  rget_col: Takes 
+00001af0: 6120 7374 7269 6e67 2063 6f6e 7461 696e  a string contain
+00001b00: 696e 6720 7468 6520 6e61 6d65 206f 6620  ing the name of 
+00001b10: 7468 6520 7461 7267 6574 2063 6f6c 756d  the target colum
+00001b20: 6e20 696e 7369 6465 2074 6865 2074 7261  n inside the tra
+00001b30: 696e 696e 6720 6461 7461 2064 662e 0a20  ining data df.. 
+00001b40: 2020 2020 2020 2029 0472 4600 0000 da07         ).rF.....
+00001b50: 7072 6564 6963 7472 0d00 0000 da06 7661  predictr......va
+00001b60: 6c75 6573 2908 7231 0000 0072 3500 0000  lues).r1...r5...
+00001b70: 724f 0000 0072 5000 0000 7236 0000 00da  rO...rP...r6....
+00001b80: 0779 5f70 726f 6273 da09 795f 636c 6173  .y_probs..y_clas
+00001b90: 7365 735a 0965 7661 6c5f 6469 6374 7232  sesZ.eval_dictr2
+00001ba0: 0000 0072 3200 0000 7233 0000 00da 0866  ...r2...r3.....f
+00001bb0: 6974 5f65 7661 6ccb 0000 0073 0800 0000  it_eval....s....
+00001bc0: 0c10 0e01 0c01 0401 7a11 426c 7565 4361  ........z.BlueCa
+00001bd0: 7374 2e66 6974 5f65 7661 6c63 0200 0000  st.fit_evalc....
+00001be0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00001bf0: 4300 0000 7318 0100 0074 0083 0001 007c  C...s....t.....|
+00001c00: 006a 0173 0a74 0264 0183 0182 017c 006a  .j.s.t.d.....|.j
+00001c10: 016a 037c 017c 006a 0467 0164 028d 027d  .j.|.|.j.g.d...}
+00001c20: 017c 006a 0572 277c 006a 056a 067c 0164  .|.j.r'|.j.j.|.d
+00001c30: 0364 048d 025c 027d 017d 027c 016a 0764  .d...\.}.}.|.j.d
+00001c40: 0364 058d 017d 0174 087c 0183 017d 0174  .d...}.t.|...}.t
+00001c50: 097c 017c 006a 0a83 027d 017c 006a 0b72  .|.|.j...}.|.j.r
+00001c60: 3a7c 006a 0ba0 067c 01a1 017d 017c 006a  :|.j...|...}.|.j
+00001c70: 0c72 527c 006a 0d72 527c 006a 0e64 066b  .rR|.j.rR|.j.d.k
+00001c80: 0272 5274 0f7c 006a 0d74 1083 0272 527c  .rRt.|.j.t...rR|
+00001c90: 006a 0da0 117c 01a1 017d 016e 177c 006a  .j...|...}.n.|.j
+00001ca0: 0c72 697c 006a 0d72 697c 006a 0e64 076b  .ri|.j.ri|.j.d.k
+00001cb0: 0272 6974 0f7c 006a 0d74 1283 0272 697c  .rit.|.j.t...ri|
+00001cc0: 006a 0da0 137c 01a1 017d 017c 006a 1472  .j...|...}.|.j.r
+00001cd0: 767c 006a 146a 067c 0164 0364 048d 025c  v|.j.j.|.d.d...\
+00001ce0: 027d 017d 027c 006a 1573 7d74 1683 007c  .}.}.|.j.s}t...|
+00001cf0: 005f 157c 006a 1772 8a7c 006a 186a 1972  ._.|.j.r.|.j.j.r
+00001d00: 8a7c 006a 17a0 067c 01a1 017d 017c 0153  .|.j...|...}.|.S
+00001d10: 0029 087a 3754 7261 6e73 666f 726d 206e  .).z7Transform n
+00001d20: 6577 2064 6174 6120 6163 636f 7264 696e  ew data accordin
+00001d30: 6720 746f 2070 7265 7072 6f63 6573 7369  g to preprocessi
+00001d40: 6e67 2070 6970 656c 696e 652e fa2a 4665  ng pipeline..*Fe
+00001d50: 6174 7572 6520 7479 7065 2063 6f6e 7665  ature type conve
+00001d60: 7274 6572 2063 6f75 6c64 206e 6f74 2062  rter could not b
+00001d70: 6520 666f 756e 642e 2901 5a0b 6967 6e6f  e found.).Z.igno
+00001d80: 7265 5f63 6f6c 7354 7239 0000 0072 3b00  re_colsTr9...r;.
+00001d90: 0000 721d 0000 0072 1e00 0000 291a 720f  ..r....r....).r.
+00001da0: 0000 0072 2c00 0000 da09 4578 6365 7074  ...r,.....Except
+00001db0: 696f 6e5a 1774 7261 6e73 666f 726d 5f66  ionZ.transform_f
+00001dc0: 6561 7475 7265 5f74 7970 6573 721f 0000  eature_typesr...
+00001dd0: 0072 2500 0000 7243 0000 0072 4400 0000  .r%...rC...rD...
+00001de0: 7216 0000 0072 1200 0000 7221 0000 0072  r....r....r!...r
+00001df0: 2f00 0000 7220 0000 0072 2d00 0000 721c  /...r ...r-...r.
+00001e00: 0000 00da 0a69 7369 6e73 7461 6e63 6572  .....isinstancer
+00001e10: 1800 0000 7247 0000 0072 1900 0000 7248  ....rG...r....rH
+00001e20: 0000 0072 2400 0000 7229 0000 0072 0900  ...r$...r)...r..
+00001e30: 0000 722b 0000 0072 2600 0000 723f 0000  ..r+...r&...r?..
+00001e40: 0029 0372 3100 0000 7235 0000 0072 4e00  .).r1...r5...rN.
+00001e50: 0000 7232 0000 0072 3200 0000 7233 0000  ..r2...r2...r3..
+00001e60: 00da 1274 7261 6e73 666f 726d 5f6e 6577  ...transform_new
+00001e70: 5f64 6174 61e0 0000 0073 4800 0000 0602  _data....sH.....
+00001e80: 0601 0801 0602 0801 06ff 0604 1401 0c01  ................
+00001e90: 0802 0c01 0602 0c01 0403 02ff 0402 02fe  ................
+00001ea0: 0a03 0a01 02ff 0e03 0402 02ff 0402 02fe  ................
+00001eb0: 0a03 0a01 02ff 0c03 0602 1401 0602 0801  ................
+00001ec0: 0e02 0c01 0402 7a1b 426c 7565 4361 7374  ......z.BlueCast
+00001ed0: 2e74 7261 6e73 666f 726d 5f6e 6577 5f64  .transform_new_d
+00001ee0: 6174 6163 0200 0000 0000 0000 0000 0000  atac............
+00001ef0: 0400 0000 0500 0000 4300 0000 7380 0000  ........C...s...
+00001f00: 007c 006a 0073 0774 0164 0183 0182 017c  .|.j.s.t.d.....|
+00001f10: 006a 0273 0e74 0164 0283 0182 0174 0383  .j.s.t.d.....t..
+00001f20: 0001 007c 00a0 047c 01a1 017d 0174 0564  ...|...|...}.t.d
+00001f30: 0383 0101 007c 006a 00a0 067c 01a1 015c  .....|.j...|...\
+00001f40: 027d 027d 037c 006a 026a 0772 3c7c 006a  .}.}.|.j.j.r<|.j
+00001f50: 087c 006a 026a 0776 0072 3c7c 006a 0972  .|.j.j.v.r<|.j.r
+00001f60: 3c7c 006a 0272 3c7c 006a 09a0 0a74 0ba0  <|.j.r<|.j...t..
+00001f70: 0c7c 03a1 01a1 017d 037c 027c 0366 0253  .|.....}.|.|.f.S
+00001f80: 0029 047a 9050 7265 6469 6374 206f 6e20  .).z.Predict on 
+00001f90: 756e 7365 656e 2064 6174 612e 0a0a 2020  unseen data...  
+00001fa0: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
+00001fb0: 2070 7265 6469 6374 6564 2070 726f 6261   predicted proba
+00001fc0: 6269 6c69 7469 6573 2061 6e64 2074 6865  bilities and the
+00001fd0: 2070 7265 6469 6374 6564 2063 6c61 7373   predicted class
+00001fe0: 6573 3a0a 2020 2020 2020 2020 795f 7072  es:.        y_pr
+00001ff0: 6f62 732c 2079 5f63 6c61 7373 6573 203d  obs, y_classes =
+00002000: 2070 7265 6469 6374 2864 6629 0a20 2020   predict(df).   
+00002010: 2020 2020 207a 1b4d 6c20 6d6f 6465 6c20       z.Ml model 
+00002020: 636f 756c 6420 6e6f 7420 6265 2066 6f75  could not be fou
+00002030: 6e64 7256 0000 007a 0d50 7265 6469 6374  ndrV...z.Predict
+00002040: 696e 672e 2e2e 290d 7223 0000 0072 5700  ing...).r#...rW.
+00002050: 0000 722c 0000 0072 0f00 0000 7259 0000  ..r,...r....rY..
+00002060: 00da 0570 7269 6e74 7251 0000 0072 2000  ...printrQ...r .
+00002070: 0000 721f 0000 0072 2e00 0000 5a1f 6c61  ..r....r....Z.la
+00002080: 6265 6c5f 656e 636f 6465 725f 7265 7665  bel_encoder_reve
+00002090: 7273 655f 7472 616e 7366 6f72 6dda 0270  rse_transform..p
+000020a0: 64da 0653 6572 6965 7329 0472 3100 0000  d..Series).r1...
+000020b0: 7235 0000 0072 5300 0000 7254 0000 0072  r5...rS...rT...r
+000020c0: 3200 0000 7232 0000 0072 3300 0000 7251  2...r2...r3...rQ
+000020d0: 0000 000e 0100 0073 2400 0000 0606 0801  .......s$.......
+000020e0: 0602 0801 0602 0a01 0802 1001 0802 0e02  ................
+000020f0: 0401 02ff 0402 02fe 0604 0801 04ff 0804  ................
+00002100: 7a10 426c 7565 4361 7374 2e70 7265 6469  z.BlueCast.predi
+00002110: 6374 290a 4e4e 4e4e 4e4e 4e4e 4e4e 291e  ct).NNNNNNNNNN).
+00002120: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00002130: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00002140: 6d65 5f5f da07 5f5f 646f 635f 5f72 0500  me__..__doc__r..
+00002150: 0000 7208 0000 00da 0373 7472 da05 666c  ..r......str..fl
+00002160: 6f61 74da 0369 6e74 7206 0000 0072 0400  oat..intr....r..
+00002170: 0000 7210 0000 0072 0200 0000 7211 0000  ..r....r....r...
+00002180: 0072 0a00 0000 720c 0000 0072 0b00 0000  .r....r....r....
+00002190: 7209 0000 0072 3400 0000 725b 0000 00da  r....r4...r[....
+000021a0: 0944 6174 6146 7261 6d65 7246 0000 0072  .DataFramerF...r
+000021b0: 5c00 0000 7203 0000 0072 5500 0000 7259  \...r....rU...rY
+000021c0: 0000 0072 0700 0000 da02 6e70 da07 6e64  ...r......np..nd
+000021d0: 6172 7261 7972 5100 0000 7232 0000 0072  arrayrQ...r2...r
+000021e0: 3200 0000 7232 0000 0072 3300 0000 721b  2...r2...r3...r.
+000021f0: 0000 0026 0000 0073 6600 0000 0800 0401  ...&...sf.......
+00002200: 0218 0201 0201 0201 0201 0201 0201 0201  ................
+00002210: 0201 0201 04f3 0602 02fe 0c03 02fd 1404  ................
+00002220: 02fc 1405 02fb 0606 02fa 0e07 02f9 0608  ................
+00002230: 02f8 0609 02f7 060a 02f6 060b 02f5 060c  ................
+00002240: 02f4 060d 0af3 1825 026b 0402 02fe 0403  .......%.k......
+00002250: 02fd 0404 02fc 0205 02fb 0a06 0afa 1615  ................
+00002260: 242e 721b 0000 0029 2e72 6000 0000 da06  $.r....).r`.....
+00002270: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
+00002280: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
+00002290: 0700 0000 7208 0000 00da 056e 756d 7079  ....r......numpy
+000022a0: 7265 0000 00da 0670 616e 6461 7372 5b00  re.....pandasr[.
+000022b0: 0000 da1f 626c 7565 6361 7374 2e63 6f6e  ....bluecast.con
+000022c0: 6669 672e 7472 6169 6e69 6e67 5f63 6f6e  fig.training_con
+000022d0: 6669 6772 0900 0000 720a 0000 0072 0b00  figr....r....r..
+000022e0: 0000 720c 0000 005a 2062 6c75 6563 6173  ..r....Z bluecas
+000022f0: 742e 6576 616c 7561 7469 6f6e 2e65 7661  t.evaluation.eva
+00002300: 6c5f 6d65 7472 6963 7372 0d00 0000 5a1f  l_metricsr....Z.
+00002310: 626c 7565 6361 7374 2e65 7661 6c75 6174  bluecast.evaluat
+00002320: 696f 6e2e 7368 6170 5f76 616c 7565 7372  ion.shap_valuesr
+00002330: 0e00 0000 5a24 626c 7565 6361 7374 2e67  ....Z$bluecast.g
+00002340: 656e 6572 616c 5f75 7469 6c73 2e67 656e  eneral_utils.gen
+00002350: 6572 616c 5f75 7469 6c73 720f 0000 005a  eral_utilsr....Z
+00002360: 1d62 6c75 6563 6173 742e 6d6c 5f6d 6f64  .bluecast.ml_mod
+00002370: 656c 6c69 6e67 2e78 6762 6f6f 7374 7210  elling.xgboostr.
+00002380: 0000 00da 1d62 6c75 6563 6173 742e 7072  .....bluecast.pr
+00002390: 6570 726f 6365 7373 696e 672e 6375 7374  eprocessing.cust
+000023a0: 6f6d 7211 0000 005a 2862 6c75 6563 6173  omr....Z(bluecas
+000023b0: 742e 7072 6570 726f 6365 7373 696e 672e  t.preprocessing.
+000023c0: 6461 7465 7469 6d65 5f66 6561 7475 7265  datetime_feature
+000023d0: 7372 1200 0000 5a2b 626c 7565 6361 7374  sr....Z+bluecast
+000023e0: 2e70 7265 7072 6f63 6573 7369 6e67 2e65  .preprocessing.e
+000023f0: 6e63 6f64 655f 7461 7267 6574 5f6c 6162  ncode_target_lab
+00002400: 656c 7372 1300 0000 5a28 626c 7565 6361  elsr....Z(blueca
+00002410: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
+00002420: 2e66 6561 7475 7265 5f73 656c 6563 7469  .feature_selecti
+00002430: 6f6e 7214 0000 005a 2462 6c75 6563 6173  onr....Z$bluecas
+00002440: 742e 7072 6570 726f 6365 7373 696e 672e  t.preprocessing.
+00002450: 6665 6174 7572 655f 7479 7065 7372 1500  feature_typesr..
+00002460: 0000 5a25 626c 7565 6361 7374 2e70 7265  ..Z%bluecast.pre
+00002470: 7072 6f63 6573 7369 6e67 2e6e 756c 6c73  processing.nulls
+00002480: 5f61 6e64 5f69 6e66 7372 1600 0000 5a24  _and_infsr....Z$
+00002490: 626c 7565 6361 7374 2e70 7265 7072 6f63  bluecast.preproc
+000024a0: 6573 7369 6e67 2e73 6368 656d 615f 6368  essing.schema_ch
+000024b0: 6563 6b73 7217 0000 005a 2662 6c75 6563  ecksr....Z&bluec
+000024c0: 6173 742e 7072 6570 726f 6365 7373 696e  ast.preprocessin
+000024d0: 672e 7461 7267 6574 5f65 6e63 6f64 696e  g.target_encodin
+000024e0: 6772 1800 0000 7219 0000 005a 2762 6c75  gr....r....Z'blu
+000024f0: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
+00002500: 696e 672e 7472 6169 6e5f 7465 7374 5f73  ing.train_test_s
+00002510: 706c 6974 721a 0000 0072 1b00 0000 7232  plitr....r....r2
+00002520: 0000 0072 3200 0000 7232 0000 0072 3300  ...r2...r2...r3.
+00002530: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00002540: 7326 0000 0004 0024 0808 0208 0118 020c  s&.....$........
+00002550: 060c 010c 010c 010c 010c 010c 010c 010c  ................
+00002560: 010c 010c 0110 010c 0412 03              ...........
```

### Comparing `bluecast-0.3.1/bluecast/blueprints/__pycache__/cast.cpython-38.pyc` & `bluecast-0.4/bluecast/blueprints/__pycache__/cast.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/blueprints/cast.py` & `bluecast-0.4/bluecast/blueprints/cast.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,14 +111,28 @@
 
         self.cat_columns = self.feat_type_detector.cat_columns
         self.date_columns = self.feat_type_detector.date_columns
 
         if not self.conf_training:
             self.conf_training = TrainingConfig()
 
+        if not self.conf_training.enable_feature_selection:
+            raise Warning(
+                """Feature selection is disabled. Update the TrainingConfig param 'enable_feature_selection'
+            to enable it or make use of a custom preprocessor to do it manually during the last mile computations step.
+            """
+            )
+
+        if self.conf_training.hypertuning_cv_folds == 1:
+            raise Warning(
+                """Cross validation is disabled. Update the TrainingConfig param 'hypertuning_cv_folds'
+            to enable it. Cross validation is disabled on defaylt to allow fast prototyping. For robust hyperparameter
+            tuning using at least 5 folds is recommended."""
+            )
+
         x_train, x_test, y_train, y_test = train_test_split(
             df,
             target_col,
             self.time_split_column,
             self.conf_training.train_size,
             self.conf_training.global_random_state,
             self.conf_training.train_split_stratify,
@@ -165,20 +179,20 @@
             x_test, y_test = self.custom_last_mile_computation.transform(
                 x_test, y_test, predicton_mode=False
             )
 
         if not self.conf_feature_selection:
             self.conf_feature_selection = FeatureSelectionConfig()
 
-        if self.conf_feature_selection.execute_selection:
+        if self.conf_training.enable_feature_selection:
             self.feature_selector = FeatureSelector(
                 selection_strategy=self.conf_feature_selection.selection_strategy
             )
 
-        if self.feature_selector and self.conf_feature_selection.execute_selection:
+        if self.feature_selector and self.conf_training.enable_feature_selection:
             x_train = self.feature_selector.fit_transform(x_train, y_train)
             x_test = self.feature_selector.transform(x_test)
 
         if not self.ml_model:
             self.ml_model = XgboostModel(
                 self.class_problem,
                 conf_training=self.conf_training,
@@ -248,15 +262,18 @@
 
         if self.custom_last_mile_computation:
             df, _ = self.custom_last_mile_computation.transform(df, predicton_mode=True)
 
         if not self.conf_feature_selection:
             self.conf_feature_selection = FeatureSelectionConfig()
 
-        if self.feature_selector and self.conf_feature_selection.execute_selection:
+        if not self.conf_training:
+            self.conf_training = TrainingConfig()
+
+        if self.feature_selector and self.conf_training.enable_feature_selection:
             df = self.feature_selector.transform(df)
 
         return df
 
     def predict(self, df: pd.DataFrame) -> Tuple[np.ndarray, np.ndarray]:
         """Predict on unseen data.
```

### Comparing `bluecast-0.3.1/bluecast/config/__pycache__/training_config.cpython-310.pyc` & `bluecast-0.4/bluecast/config/__pycache__/training_config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 11:37:59 2023 UTC, .py size: 3469 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1784 9564 8d0d 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 de0e 9764 950d 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a05 6401 6404 6c06  ..d.d.l.Z.d.d.l.
 00000050: 6d07 5a07 0100 6401 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6407 6c0d 6d0e 5a0e 0100 4700  ..d.d.l.m.Z...G.
@@ -60,221 +60,221 @@
 000003b0: 2f74 686f 6d61 732f 4964 6561 5072 6f6a  /thomas/IdeaProj
 000003c0: 6563 7473 2f42 6c75 6543 6173 742f 626c  ects/BlueCast/bl
 000003d0: 7565 6361 7374 2f63 6f6e 6669 672f 7472  uecast/config/tr
 000003e0: 6169 6e69 6e67 5f63 6f6e 6669 672e 7079  aining_config.py
 000003f0: 7209 0000 0011 0000 0073 0400 0000 0800  r........s......
 00000400: 0801 7209 0000 0063 0000 0000 0000 0000  ..r....c........
 00000410: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000420: 7396 0000 0065 005a 0164 005a 0255 0064  s....e.Z.d.Z.U.d
+00000420: 73a2 0000 0065 005a 0164 005a 0255 0064  s....e.Z.d.Z.U.d
 00000430: 015a 0364 025a 0465 0565 0664 033c 0064  .Z.d.Z.e.e.d.<.d
 00000440: 045a 0765 0865 0664 053c 0064 065a 0965  .Z.e.e.d.<.d.Z.e
 00000450: 0565 0664 073c 0064 085a 0a65 0565 0664  .e.d.<.d.Z.e.e.d
 00000460: 093c 0064 0a5a 0b65 0565 0664 0b3c 0064  .<.d.Z.e.e.d.<.d
 00000470: 025a 0c65 0565 0664 0c3c 0064 045a 0d65  .Z.e.e.d.<.d.Z.e
-00000480: 0865 0664 0d3c 0064 045a 0e65 0865 0664  .e.d.<.d.Z.e.e.d
-00000490: 0e3c 0064 0f5a 0f65 1065 0664 103c 0064  .<.d.Z.e.e.d.<.d
-000004a0: 045a 1165 0865 0664 113c 0064 045a 1265  .Z.e.e.d.<.d.Z.e
-000004b0: 0865 0664 123c 0064 1353 0029 14da 0e54  .e.d.<.d.S.)...T
-000004c0: 7261 696e 696e 6743 6f6e 6669 677a 2344  rainingConfigz#D
-000004d0: 6566 696e 6520 6765 6e65 7261 6c20 7472  efine general tr
-000004e0: 6169 6e69 6e67 2070 6172 616d 6574 6572  aining parameter
-000004f0: 732e e90a 0000 00da 1367 6c6f 6261 6c5f  s........global_
-00000500: 7261 6e64 6f6d 5f73 7461 7465 54da 1773  random_stateT..s
-00000510: 6875 6666 6c65 5f64 7572 696e 675f 7472  huffle_during_tr
-00000520: 6169 6e69 6e67 e964 0000 00da 1c68 7970  aining.d.....hyp
-00000530: 6572 7061 7261 6d65 7465 725f 7475 6e69  erparameter_tuni
-00000540: 6e67 5f72 6f75 6e64 7369 100e 0000 da26  ng_roundsi.....&
-00000550: 6879 7065 7270 6172 616d 6574 6572 5f74  hyperparameter_t
-00000560: 756e 696e 675f 6d61 785f 7275 6e74 696d  uning_max_runtim
-00000570: 655f 7365 6373 e901 0000 00da 1468 7970  e_secs.......hyp
-00000580: 6572 7475 6e69 6e67 5f63 765f 666f 6c64  ertuning_cv_fold
-00000590: 73da 1565 6172 6c79 5f73 746f 7070 696e  s..early_stoppin
-000005a0: 675f 726f 756e 6473 da0e 6175 746f 7475  g_rounds..autotu
-000005b0: 6e65 5f6d 6f64 656c da15 6361 6c63 756c  ne_model..calcul
-000005c0: 6174 655f 7368 6170 5f76 616c 7565 73e7  ate_shap_values.
-000005d0: 9a99 9999 9999 e93f da0a 7472 6169 6e5f  .......?..train_
-000005e0: 7369 7a65 da14 7472 6169 6e5f 7370 6c69  size..train_spli
-000005f0: 745f 7374 7261 7469 6679 da1d 7573 655f  t_stratify..use_
-00000600: 6675 6c6c 5f64 6174 615f 666f 725f 6669  full_data_for_fi
-00000610: 6e61 6c5f 6d6f 6465 6c4e 2913 720a 0000  nal_modelN).r...
-00000620: 0072 0b00 0000 720c 0000 00da 075f 5f64  .r....r......__d
-00000630: 6f63 5f5f 7211 0000 00da 0369 6e74 da0f  oc__r......int..
-00000640: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
-00000650: 1200 0000 da04 626f 6f6c 7214 0000 0072  ......boolr....r
-00000660: 1500 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
-00000670: 0000 0072 1a00 0000 721c 0000 00da 0566  ...r....r......f
-00000680: 6c6f 6174 721d 0000 0072 1e00 0000 720d  loatr....r....r.
-00000690: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-000006a0: 0000 720f 0000 0015 0000 0073 1a00 0000  ..r........s....
-000006b0: 0a00 0402 0c02 0c01 0c01 0c01 0c01 0c01  ................
-000006c0: 0c01 0c01 0c01 0c01 1001 720f 0000 0029  ..........r....)
-000006d0: 01da 0663 6f6e 6669 6763 0000 0000 0000  ...configc......
-000006e0: 0000 0000 0000 0000 0000 0800 0000 4000  ..............@.
-000006f0: 0000 734c 0000 0065 005a 0164 005a 0255  ..sL...e.Z.d.Z.U
-00000700: 0064 015a 0364 025a 0465 0565 0664 033c  .d.Z.d.Z.e.e.d.<
-00000710: 0065 0765 08a0 09a1 0064 0465 0a64 0564  .e.e.....d.e.d.d
-00000720: 0664 0264 078d 0364 0465 0b65 0c83 0164  .d.d...d.e.e...d
-00000730: 0864 098d 065a 0d65 0765 0664 0a3c 0064  .d...Z.e.e.d.<.d
-00000740: 0b53 0029 0cda 1646 6561 7475 7265 5365  .S.)...FeatureSe
-00000750: 6c65 6374 696f 6e43 6f6e 6669 677a 2444  lectionConfigz$D
-00000760: 6566 696e 6520 6665 6174 7572 6520 7365  efine feature se
-00000770: 6c65 6374 696f 6e20 7061 7261 6d65 7465  lection paramete
-00000780: 7273 2e54 da11 6578 6563 7574 655f 7365  rs.T..execute_se
-00000790: 6c65 6374 696f 6e72 1600 0000 e905 0000  lectionr........
-000007a0: 0072 0100 0000 2902 da0c 7261 6e64 6f6d  .r....)...random
-000007b0: 5f73 7461 7465 da07 7368 7566 666c 65e9  _state..shuffle.
-000007c0: 0400 0000 2906 da09 6573 7469 6d61 746f  ....)...estimato
-000007d0: 72da 0473 7465 70da 0263 765a 166d 696e  r..step..cvZ.min
-000007e0: 5f66 6561 7475 7265 735f 746f 5f73 656c  _features_to_sel
-000007f0: 6563 74da 0773 636f 7269 6e67 da06 6e5f  ect..scoring..n_
-00000800: 6a6f 6273 da12 7365 6c65 6374 696f 6e5f  jobs..selection_
-00000810: 7374 7261 7465 6779 4e29 0e72 0a00 0000  strategyN).r....
-00000820: 720b 0000 0072 0c00 0000 721f 0000 0072  r....r....r....r
-00000830: 2600 0000 7222 0000 0072 2100 0000 7205  &...r"...r!...r.
+00000480: 0865 0664 0d3c 0064 0e5a 0e65 0865 0664  .e.d.<.d.Z.e.e.d
+00000490: 0f3c 0064 045a 0f65 0865 0664 103c 0064  .<.d.Z.e.e.d.<.d
+000004a0: 115a 1065 1165 0664 123c 0064 045a 1265  .Z.e.e.d.<.d.Z.e
+000004b0: 0865 0664 133c 0064 045a 1365 0865 0664  .e.d.<.d.Z.e.e.d
+000004c0: 143c 0064 1553 0029 16da 0e54 7261 696e  .<.d.S.)...Train
+000004d0: 696e 6743 6f6e 6669 677a 2344 6566 696e  ingConfigz#Defin
+000004e0: 6520 6765 6e65 7261 6c20 7472 6169 6e69  e general traini
+000004f0: 6e67 2070 6172 616d 6574 6572 732e e90a  ng parameters...
+00000500: 0000 00da 1367 6c6f 6261 6c5f 7261 6e64  .....global_rand
+00000510: 6f6d 5f73 7461 7465 54da 1773 6875 6666  om_stateT..shuff
+00000520: 6c65 5f64 7572 696e 675f 7472 6169 6e69  le_during_traini
+00000530: 6e67 e964 0000 00da 1c68 7970 6572 7061  ng.d.....hyperpa
+00000540: 7261 6d65 7465 725f 7475 6e69 6e67 5f72  rameter_tuning_r
+00000550: 6f75 6e64 7369 100e 0000 da26 6879 7065  oundsi.....&hype
+00000560: 7270 6172 616d 6574 6572 5f74 756e 696e  rparameter_tunin
+00000570: 675f 6d61 785f 7275 6e74 696d 655f 7365  g_max_runtime_se
+00000580: 6373 e901 0000 00da 1468 7970 6572 7475  cs.......hypertu
+00000590: 6e69 6e67 5f63 765f 666f 6c64 73da 1565  ning_cv_folds..e
+000005a0: 6172 6c79 5f73 746f 7070 696e 675f 726f  arly_stopping_ro
+000005b0: 756e 6473 da0e 6175 746f 7475 6e65 5f6d  unds..autotune_m
+000005c0: 6f64 656c 46da 1865 6e61 626c 655f 6665  odelF..enable_fe
+000005d0: 6174 7572 655f 7365 6c65 6374 696f 6eda  ature_selection.
+000005e0: 1563 616c 6375 6c61 7465 5f73 6861 705f  .calculate_shap_
+000005f0: 7661 6c75 6573 e79a 9999 9999 99e9 3fda  values........?.
+00000600: 0a74 7261 696e 5f73 697a 65da 1474 7261  .train_size..tra
+00000610: 696e 5f73 706c 6974 5f73 7472 6174 6966  in_split_stratif
+00000620: 79da 1d75 7365 5f66 756c 6c5f 6461 7461  y..use_full_data
+00000630: 5f66 6f72 5f66 696e 616c 5f6d 6f64 656c  _for_final_model
+00000640: 4e29 1472 0a00 0000 720b 0000 0072 0c00  N).r....r....r..
+00000650: 0000 da07 5f5f 646f 635f 5f72 1100 0000  ....__doc__r....
+00000660: da03 696e 74da 0f5f 5f61 6e6e 6f74 6174  ..int..__annotat
+00000670: 696f 6e73 5f5f 7212 0000 00da 0462 6f6f  ions__r......boo
+00000680: 6c72 1400 0000 7215 0000 0072 1700 0000  lr....r....r....
+00000690: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+000006a0: 1b00 0000 721d 0000 00da 0566 6c6f 6174  ....r......float
+000006b0: 721e 0000 0072 1f00 0000 720d 0000 0072  r....r....r....r
+000006c0: 0d00 0000 720d 0000 0072 0e00 0000 720f  ....r....r....r.
+000006d0: 0000 0015 0000 0073 1c00 0000 0a00 0402  .......s........
+000006e0: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000006f0: 0c01 0c01 0c01 1001 720f 0000 0029 01da  ........r....)..
+00000700: 0663 6f6e 6669 6763 0000 0000 0000 0000  .configc........
+00000710: 0000 0000 0000 0000 0800 0000 4000 0000  ............@...
+00000720: 7340 0000 0065 005a 0164 005a 0255 0064  s@...e.Z.d.Z.U.d
+00000730: 015a 0365 0465 05a0 06a1 0064 0265 0764  .Z.e.e.....d.e.d
+00000740: 0364 0464 0564 068d 0364 0265 0865 0983  .d.d.d...d.e.e..
+00000750: 0164 0764 088d 065a 0a65 0465 0b64 093c  .d.d...Z.e.e.d.<
+00000760: 0064 0a53 0029 0bda 1646 6561 7475 7265  .d.S.)...Feature
+00000770: 5365 6c65 6374 696f 6e43 6f6e 6669 677a  SelectionConfigz
+00000780: 2444 6566 696e 6520 6665 6174 7572 6520  $Define feature 
+00000790: 7365 6c65 6374 696f 6e20 7061 7261 6d65  selection parame
+000007a0: 7465 7273 2e72 1600 0000 e905 0000 0072  ters.r.........r
+000007b0: 0100 0000 5429 02da 0c72 616e 646f 6d5f  ....T)...random_
+000007c0: 7374 6174 65da 0773 6875 6666 6c65 e904  state..shuffle..
+000007d0: 0000 0029 06da 0965 7374 696d 6174 6f72  ...)...estimator
+000007e0: da04 7374 6570 da02 6376 da16 6d69 6e5f  ..step..cv..min_
+000007f0: 6665 6174 7572 6573 5f74 6f5f 7365 6c65  features_to_sele
+00000800: 6374 da07 7363 6f72 696e 67da 066e 5f6a  ct..scoring..n_j
+00000810: 6f62 73da 1273 656c 6563 7469 6f6e 5f73  obs..selection_s
+00000820: 7472 6174 6567 794e 290c 720a 0000 0072  trategyN).r....r
+00000830: 0b00 0000 720c 0000 0072 2000 0000 7205  ....r....r ...r.
 00000840: 0000 00da 0378 6762 da0d 5847 4243 6c61  .....xgb..XGBCla
 00000850: 7373 6966 6965 7272 0800 0000 7206 0000  ssifierr....r...
-00000860: 0072 0700 0000 7230 0000 0072 0d00 0000  .r....r0...r....
-00000870: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00000880: 2500 0000 2600 0000 7316 0000 000a 0004  %...&...s.......
-00000890: 020c 0202 0106 0102 010c 0102 0106 0102  ................
-000008a0: 0112 fa72 2500 0000 6300 0000 0000 0000  ...r%...c.......
-000008b0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-000008c0: 0073 4a01 0000 6500 5a01 6400 5a02 5500  .sJ...e.Z.d.Z.U.
-000008d0: 6401 5a03 6402 5a04 6505 6506 6403 3c00  d.Z.d.Z.e.e.d.<.
-000008e0: 6404 5a07 6505 6506 6405 3c00 6406 5a08  d.Z.e.e.d.<.d.Z.
-000008f0: 6509 6506 6407 3c00 6408 5a0a 6509 6506  e.e.d.<.d.Z.e.e.
-00000900: 6409 3c00 6406 5a0b 6509 6506 640a 3c00  d.<.d.Z.e.e.d.<.
-00000910: 6408 5a0c 6509 6506 640b 3c00 6402 5a0d  d.Z.e.e.d.<.d.Z.
-00000920: 6505 6506 640c 3c00 640d 5a0e 6505 6506  e.e.d.<.d.Z.e.e.
-00000930: 640e 3c00 640f 5a0f 6509 6506 6410 3c00  d.<.d.Z.e.e.d.<.
-00000940: 6406 5a10 6509 6506 6411 3c00 640f 5a11  d.Z.e.e.d.<.d.Z.
-00000950: 6509 6506 6412 3c00 6406 5a12 6509 6506  e.e.d.<.d.Z.e.e.
-00000960: 6413 3c00 640f 5a13 6509 6506 6414 3c00  d.<.d.Z.e.e.d.<.
-00000970: 6406 5a14 6509 6506 6415 3c00 640f 5a15  d.Z.e.e.d.<.d.Z.
-00000980: 6509 6506 6416 3c00 6406 5a16 6509 6506  e.e.d.<.d.Z.e.e.
-00000990: 6417 3c00 6402 5a17 6505 6506 6418 3c00  d.<.d.Z.e.e.d.<.
-000009a0: 6419 5a18 6505 6506 641a 3c00 641b 5a19  d.Z.e.e.d.<.d.Z.
-000009b0: 6509 6506 641c 3c00 6402 5a1a 6505 6506  e.e.d.<.d.Z.e.e.
-000009c0: 641d 3c00 641e 5a1b 6505 6506 641f 3c00  d.<.d.Z.e.e.d.<.
-000009d0: 6420 5a1c 6505 6506 6421 3c00 6404 5a1d  d Z.e.e.d!<.d.Z.
-000009e0: 6505 6506 6422 3c00 6423 5a1e 6505 6506  e.e.d"<.d#Z.e.e.
-000009f0: 6424 3c00 6425 5a1f 6520 6506 6426 3c00  d$<.d%Z.e e.d&<.
-00000a00: 6427 5a21 6520 6506 6428 3c00 6429 5300  d'Z!e e.d(<.d)S.
-00000a10: 292a da17 5867 626f 6f73 7454 756e 6550  )*..XgboostTuneP
-00000a20: 6172 616d 7343 6f6e 6669 677a 2a44 6566  aramsConfigz*Def
-00000a30: 696e 6520 6879 7065 7270 6172 616d 6574  ine hyperparamet
-00000a40: 6572 2074 756e 696e 6720 7365 6172 6368  er tuning search
-00000a50: 2073 7061 6365 2ee9 0200 0000 da0d 6d61   space........ma
-00000a60: 785f 6465 7074 685f 6d69 6ee9 0300 0000  x_depth_min.....
-00000a70: da0d 6d61 785f 6465 7074 685f 6d61 7867  ..max_depth_maxg
-00000a80: 0000 0000 0000 f03f da09 616c 7068 615f  .......?..alpha_
-00000a90: 6d69 6e67 0000 0000 0040 8f40 da09 616c  ming.....@.@..al
-00000aa0: 7068 615f 6d61 78da 0a6c 616d 6264 615f  pha_max..lambda_
-00000ab0: 6d69 6eda 0a6c 616d 6264 615f 6d61 78da  min..lambda_max.
-00000ac0: 0e6e 756d 5f6c 6561 7665 735f 6d69 6ee9  .num_leaves_min.
-00000ad0: 4000 0000 da0e 6e75 6d5f 6c65 6176 6573  @.....num_leaves
-00000ae0: 5f6d 6178 6733 3333 3333 33d3 3fda 0e73  _maxg333333.?..s
-00000af0: 7562 5f73 616d 706c 655f 6d69 6eda 0e73  ub_sample_min..s
-00000b00: 7562 5f73 616d 706c 655f 6d61 78da 1663  ub_sample_max..c
-00000b10: 6f6c 5f73 616d 706c 655f 6279 5f74 7265  ol_sample_by_tre
-00000b20: 655f 6d69 6eda 1663 6f6c 5f73 616d 706c  e_min..col_sampl
-00000b30: 655f 6279 5f74 7265 655f 6d61 78da 1763  e_by_tree_max..c
-00000b40: 6f6c 5f73 616d 706c 655f 6279 5f6c 6576  ol_sample_by_lev
-00000b50: 656c 5f6d 696e da17 636f 6c5f 7361 6d70  el_min..col_samp
-00000b60: 6c65 5f62 795f 6c65 7665 6c5f 6d61 78da  le_by_level_max.
-00000b70: 1663 6f6c 5f73 616d 706c 655f 6279 5f6e  .col_sample_by_n
-00000b80: 6f64 655f 6d69 6eda 1663 6f6c 5f73 616d  ode_min..col_sam
-00000b90: 706c 655f 6279 5f6e 6f64 655f 6d61 78da  ple_by_node_max.
-00000ba0: 156d 696e 5f63 6869 6c64 5f73 616d 706c  .min_child_sampl
-00000bb0: 6573 5f6d 696e e9e8 0300 00da 156d 696e  es_min.......min
-00000bc0: 5f63 6869 6c64 5f73 616d 706c 6573 5f6d  _child_samples_m
-00000bd0: 6178 e79a 9999 9999 99b9 3fda 0365 7461  ax........?..eta
-00000be0: da09 7374 6570 735f 6d69 6e69 50c3 0000  ..steps_miniP...
-00000bf0: da09 7374 6570 735f 6d61 7872 1600 0000  ..steps_maxr....
-00000c00: da15 6e75 6d5f 7061 7261 6c6c 656c 5f74  ..num_parallel_t
-00000c10: 7265 655f 6d69 6eda 156e 756d 5f70 6172  ree_min..num_par
-00000c20: 616c 6c65 6c5f 7472 6565 5f6d 6178 7201  allel_tree_maxr.
-00000c30: 0000 00da 0f6d 6f64 656c 5f76 6572 626f  .....model_verbo
-00000c40: 7369 7479 fa0e 6d75 6c74 693a 736f 6674  sity..multi:soft
-00000c50: 7072 6f62 da0f 6d6f 6465 6c5f 6f62 6a65  prob..model_obje
-00000c60: 6374 6976 65da 086d 6c6f 676c 6f73 73da  ctive..mlogloss.
-00000c70: 116d 6f64 656c 5f65 7661 6c5f 6d65 7472  .model_eval_metr
-00000c80: 6963 4e29 2272 0a00 0000 720b 0000 0072  icN)"r....r....r
-00000c90: 0c00 0000 721f 0000 0072 3500 0000 7220  ....r....r5...r 
-00000ca0: 0000 0072 2100 0000 7237 0000 0072 3800  ...r!...r7...r8.
-00000cb0: 0000 7223 0000 0072 3900 0000 723a 0000  ..r#...r9...r:..
-00000cc0: 0072 3b00 0000 723c 0000 0072 3e00 0000  .r;...r<...r>...
-00000cd0: 723f 0000 0072 4000 0000 7241 0000 0072  r?...r@...rA...r
-00000ce0: 4200 0000 7243 0000 0072 4400 0000 7245  B...rC...rD...rE
-00000cf0: 0000 0072 4600 0000 7247 0000 0072 4900  ...rF...rG...rI.
-00000d00: 0000 724b 0000 0072 4c00 0000 724d 0000  ..rK...rL...rM..
-00000d10: 0072 4e00 0000 724f 0000 0072 5000 0000  .rN...rO...rP...
-00000d20: 7252 0000 00da 0373 7472 7254 0000 0072  rR.....strrT...r
-00000d30: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-00000d40: 0000 0072 3300 0000 3500 0000 7338 0000  ...r3...5...s8..
-00000d50: 000a 0004 020c 020c 010c 010c 010c 010c  ................
-00000d60: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00000d70: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00000d80: 010c 010c 010c 0110 0172 3300 0000 6300  .........r3...c.
-00000d90: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00000da0: 0000 0040 0000 0073 a000 0000 6500 5a01  ...@...s....e.Z.
-00000db0: 6400 5a02 5500 6401 5a03 6900 6402 6403  d.Z.U.d.Z.i.d.d.
-00000dc0: 9301 6404 6405 9301 6406 6407 9301 6408  ..d.d...d.d...d.
-00000dd0: 6409 9301 640a 640b 9301 640c 640d 9301  d...d.d...d.d...
-00000de0: 640e 640f 9301 6410 640f 9301 6411 6412  d.d...d.d...d.d.
-00000df0: 9301 6413 6414 9301 6415 6414 9301 6416  ..d.d...d.d...d.
-00000e00: 6414 9301 6417 6414 9301 6418 6419 9301  d...d.d...d.d...
-00000e10: 641a 640f 9301 641b 641c 9301 641d 641e  d.d...d.d...d.d.
-00000e20: 9301 5a04 641f 5a05 6506 6507 6508 6509  ..Z.d.Z.e.e.e.e.
-00000e30: 6602 1900 1900 650a 6420 3c00 6421 5a0b  f.....e.d <.d!Z.
-00000e40: 6509 650a 6422 3c00 641f 5300 2923 da17  e.e.d"<.d.S.)#..
-00000e50: 5867 626f 6f73 7446 696e 616c 5061 7261  XgboostFinalPara
-00000e60: 6d43 6f6e 6669 677a 1e44 6566 696e 6520  mConfigz.Define 
-00000e70: 6669 6e61 6c20 6879 7065 7220 7061 7261  final hyper para
-00000e80: 6d65 7465 7273 2eda 096f 626a 6563 7469  meters...objecti
-00000e90: 7665 7251 0000 005a 0b65 7661 6c5f 6d65  verQ...Z.eval_me
-00000ea0: 7472 6963 7253 0000 00da 0776 6572 626f  tricrS.....verbo
-00000eb0: 7365 7201 0000 00da 0b74 7265 655f 6d65  ser......tree_me
-00000ec0: 7468 6f64 da05 6578 6163 745a 096e 756d  thod..exactZ.num
-00000ed0: 5f63 6c61 7373 7234 0000 00da 096d 6178  _classr4.....max
-00000ee0: 5f64 6570 7468 7236 0000 00da 0561 6c70  _depthr6.....alp
-00000ef0: 6861 724a 0000 00da 066c 616d 6264 61da  harJ.....lambda.
-00000f00: 0a6e 756d 5f6c 6561 7665 73e9 1000 0000  .num_leaves.....
-00000f10: da09 7375 6273 616d 706c 6572 1b00 0000  ..subsampler....
-00000f20: 5a10 636f 6c73 616d 706c 655f 6279 7472  Z.colsample_bytr
-00000f30: 6565 5a11 636f 6c73 616d 706c 655f 6279  eeZ.colsample_by
-00000f40: 6c65 7665 6c5a 1063 6f6c 7361 6d70 6c65  levelZ.colsample
-00000f50: 5f62 796e 6f64 65da 116d 696e 5f63 6869  _bynode..min_chi
-00000f60: 6c64 5f73 616d 706c 6573 7213 0000 0072  ld_samplesr....r
-00000f70: 4b00 0000 da05 7374 6570 7372 4800 0000  K.....stepsrH...
-00000f80: 5a11 6e75 6d5f 7061 7261 6c6c 656c 5f74  Z.num_parallel_t
-00000f90: 7265 6572 1600 0000 4eda 0d73 616d 706c  reer....N..sampl
-00000fa0: 655f 7765 6967 6874 6700 0000 0000 00e0  e_weightg.......
-00000fb0: 3fda 1863 6c61 7373 6966 6963 6174 696f  ?..classificatio
-00000fc0: 6e5f 7468 7265 7368 6f6c 6429 0c72 0a00  n_threshold).r..
-00000fd0: 0000 720b 0000 0072 0c00 0000 721f 0000  ..r....r....r...
-00000fe0: 00da 0670 6172 616d 7372 6300 0000 7203  ...paramsrc...r.
-00000ff0: 0000 0072 0200 0000 7255 0000 0072 2300  ...r....rU...r#.
-00001000: 0000 7221 0000 0072 6400 0000 720d 0000  ..r!...rd...r...
-00001010: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-00001020: 7256 0000 0055 0000 0073 4e00 0000 0a00  rV...U...sN.....
-00001030: 0402 0202 0401 02ff 0402 02fe 0403 02fd  ................
-00001040: 0404 02fc 0405 02fb 0406 02fa 0407 02f9  ................
-00001050: 0408 02f8 0409 02f7 040a 02f6 040b 02f5  ................
-00001060: 040c 02f4 040d 02f3 040e 02f2 040f 02f1  ................
-00001070: 0410 02f0 0411 04ef 1813 1001 7256 0000  ............rV..
-00001080: 0029 1472 1f00 0000 da06 7479 7069 6e67  .).r......typing
-00001090: 7202 0000 0072 0300 0000 da07 7867 626f  r....r......xgbo
-000010a0: 6f73 7472 3100 0000 5a14 7079 6461 6e74  ostr1...Z.pydant
-000010b0: 6963 2e64 6174 6163 6c61 7373 6573 7204  ic.dataclassesr.
-000010c0: 0000 005a 1973 6b6c 6561 726e 2e66 6561  ...Z.sklearn.fea
-000010d0: 7475 7265 5f73 656c 6563 7469 6f6e 7205  ture_selectionr.
-000010e0: 0000 005a 0f73 6b6c 6561 726e 2e6d 6574  ...Z.sklearn.met
-000010f0: 7269 6373 7206 0000 0072 0700 0000 5a17  ricsr....r....Z.
-00001100: 736b 6c65 6172 6e2e 6d6f 6465 6c5f 7365  sklearn.model_se
-00001110: 6c65 6374 696f 6e72 0800 0000 7209 0000  lectionr....r...
-00001120: 0072 0f00 0000 7225 0000 0072 3300 0000  .r....r%...r3...
-00001130: 7256 0000 0072 0d00 0000 720d 0000 0072  rV...r....r....r
-00001140: 0d00 0000 720e 0000 00da 083c 6d6f 6475  ....r......<modu
-00001150: 6c65 3e01 0000 0073 2000 0000 0400 1007  le>....s .......
-00001160: 0802 0c01 0c01 1001 0c01 0e03 0204 1001  ................
-00001170: 0810 1001 020e 1001 021f 1401            ............
+00000860: 0072 0700 0000 7231 0000 0072 2200 0000  .r....r1...r"...
+00000870: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00000880: 0e00 0000 7226 0000 0027 0000 0073 1400  ....r&...'...s..
+00000890: 0000 0a00 0402 0202 0601 0201 0c01 0201  ................
+000008a0: 0601 0201 12fa 7226 0000 0063 0000 0000  ......r&...c....
+000008b0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+000008c0: 4000 0000 734a 0100 0065 005a 0164 005a  @...sJ...e.Z.d.Z
+000008d0: 0255 0064 015a 0364 025a 0465 0565 0664  .U.d.Z.d.Z.e.e.d
+000008e0: 033c 0064 045a 0765 0565 0664 053c 0064  .<.d.Z.e.e.d.<.d
+000008f0: 065a 0865 0965 0664 073c 0064 085a 0a65  .Z.e.e.d.<.d.Z.e
+00000900: 0965 0664 093c 0064 065a 0b65 0965 0664  .e.d.<.d.Z.e.e.d
+00000910: 0a3c 0064 085a 0c65 0965 0664 0b3c 0064  .<.d.Z.e.e.d.<.d
+00000920: 025a 0d65 0565 0664 0c3c 0064 0d5a 0e65  .Z.e.e.d.<.d.Z.e
+00000930: 0565 0664 0e3c 0064 0f5a 0f65 0965 0664  .e.d.<.d.Z.e.e.d
+00000940: 103c 0064 065a 1065 0965 0664 113c 0064  .<.d.Z.e.e.d.<.d
+00000950: 0f5a 1165 0965 0664 123c 0064 065a 1265  .Z.e.e.d.<.d.Z.e
+00000960: 0965 0664 133c 0064 0f5a 1365 0965 0664  .e.d.<.d.Z.e.e.d
+00000970: 143c 0064 065a 1465 0965 0664 153c 0064  .<.d.Z.e.e.d.<.d
+00000980: 0f5a 1565 0965 0664 163c 0064 065a 1665  .Z.e.e.d.<.d.Z.e
+00000990: 0965 0664 173c 0064 025a 1765 0565 0664  .e.d.<.d.Z.e.e.d
+000009a0: 183c 0064 195a 1865 0565 0664 1a3c 0064  .<.d.Z.e.e.d.<.d
+000009b0: 1b5a 1965 0965 0664 1c3c 0064 025a 1a65  .Z.e.e.d.<.d.Z.e
+000009c0: 0565 0664 1d3c 0064 1e5a 1b65 0565 0664  .e.d.<.d.Z.e.e.d
+000009d0: 1f3c 0064 205a 1c65 0565 0664 213c 0064  .<.d Z.e.e.d!<.d
+000009e0: 045a 1d65 0565 0664 223c 0064 235a 1e65  .Z.e.e.d"<.d#Z.e
+000009f0: 0565 0664 243c 0064 255a 1f65 2065 0664  .e.d$<.d%Z.e e.d
+00000a00: 263c 0064 275a 2165 2065 0664 283c 0064  &<.d'Z!e e.d(<.d
+00000a10: 2953 0029 2ada 1758 6762 6f6f 7374 5475  )S.)*..XgboostTu
+00000a20: 6e65 5061 7261 6d73 436f 6e66 6967 7a2a  neParamsConfigz*
+00000a30: 4465 6669 6e65 2068 7970 6572 7061 7261  Define hyperpara
+00000a40: 6d65 7465 7220 7475 6e69 6e67 2073 6561  meter tuning sea
+00000a50: 7263 6820 7370 6163 652e e902 0000 00da  rch space.......
+00000a60: 0d6d 6178 5f64 6570 7468 5f6d 696e e903  .max_depth_min..
+00000a70: 0000 00da 0d6d 6178 5f64 6570 7468 5f6d  .....max_depth_m
+00000a80: 6178 6700 0000 0000 00f0 3fda 0961 6c70  axg.......?..alp
+00000a90: 6861 5f6d 696e 6700 0000 0000 408f 40da  ha_ming.....@.@.
+00000aa0: 0961 6c70 6861 5f6d 6178 da0a 6c61 6d62  .alpha_max..lamb
+00000ab0: 6461 5f6d 696e da0a 6c61 6d62 6461 5f6d  da_min..lambda_m
+00000ac0: 6178 da0e 6e75 6d5f 6c65 6176 6573 5f6d  ax..num_leaves_m
+00000ad0: 696e e940 0000 00da 0e6e 756d 5f6c 6561  in.@.....num_lea
+00000ae0: 7665 735f 6d61 7867 3333 3333 3333 d33f  ves_maxg333333.?
+00000af0: da0e 7375 625f 7361 6d70 6c65 5f6d 696e  ..sub_sample_min
+00000b00: da0e 7375 625f 7361 6d70 6c65 5f6d 6178  ..sub_sample_max
+00000b10: da16 636f 6c5f 7361 6d70 6c65 5f62 795f  ..col_sample_by_
+00000b20: 7472 6565 5f6d 696e da16 636f 6c5f 7361  tree_min..col_sa
+00000b30: 6d70 6c65 5f62 795f 7472 6565 5f6d 6178  mple_by_tree_max
+00000b40: da17 636f 6c5f 7361 6d70 6c65 5f62 795f  ..col_sample_by_
+00000b50: 6c65 7665 6c5f 6d69 6eda 1763 6f6c 5f73  level_min..col_s
+00000b60: 616d 706c 655f 6279 5f6c 6576 656c 5f6d  ample_by_level_m
+00000b70: 6178 da16 636f 6c5f 7361 6d70 6c65 5f62  ax..col_sample_b
+00000b80: 795f 6e6f 6465 5f6d 696e da16 636f 6c5f  y_node_min..col_
+00000b90: 7361 6d70 6c65 5f62 795f 6e6f 6465 5f6d  sample_by_node_m
+00000ba0: 6178 da15 6d69 6e5f 6368 696c 645f 7361  ax..min_child_sa
+00000bb0: 6d70 6c65 735f 6d69 6ee9 e803 0000 da15  mples_min.......
+00000bc0: 6d69 6e5f 6368 696c 645f 7361 6d70 6c65  min_child_sample
+00000bd0: 735f 6d61 78e7 9a99 9999 9999 b93f da03  s_max........?..
+00000be0: 6574 61da 0973 7465 7073 5f6d 696e 6950  eta..steps_miniP
+00000bf0: c300 00da 0973 7465 7073 5f6d 6178 7216  .....steps_maxr.
+00000c00: 0000 00da 156e 756d 5f70 6172 616c 6c65  .....num_paralle
+00000c10: 6c5f 7472 6565 5f6d 696e da15 6e75 6d5f  l_tree_min..num_
+00000c20: 7061 7261 6c6c 656c 5f74 7265 655f 6d61  parallel_tree_ma
+00000c30: 7872 0100 0000 da0f 6d6f 6465 6c5f 7665  xr......model_ve
+00000c40: 7262 6f73 6974 79fa 0e6d 756c 7469 3a73  rbosity..multi:s
+00000c50: 6f66 7470 726f 62da 0f6d 6f64 656c 5f6f  oftprob..model_o
+00000c60: 626a 6563 7469 7665 da08 6d6c 6f67 6c6f  bjective..mloglo
+00000c70: 7373 da11 6d6f 6465 6c5f 6576 616c 5f6d  ss..model_eval_m
+00000c80: 6574 7269 634e 2922 720a 0000 0072 0b00  etricN)"r....r..
+00000c90: 0000 720c 0000 0072 2000 0000 7236 0000  ..r....r ...r6..
+00000ca0: 0072 2100 0000 7222 0000 0072 3800 0000  .r!...r"...r8...
+00000cb0: 7239 0000 0072 2400 0000 723a 0000 0072  r9...r$...r:...r
+00000cc0: 3b00 0000 723c 0000 0072 3d00 0000 723f  ;...r<...r=...r?
+00000cd0: 0000 0072 4000 0000 7241 0000 0072 4200  ...r@...rA...rB.
+00000ce0: 0000 7243 0000 0072 4400 0000 7245 0000  ..rC...rD...rE..
+00000cf0: 0072 4600 0000 7247 0000 0072 4800 0000  .rF...rG...rH...
+00000d00: 724a 0000 0072 4c00 0000 724d 0000 0072  rJ...rL...rM...r
+00000d10: 4e00 0000 724f 0000 0072 5000 0000 7251  N...rO...rP...rQ
+00000d20: 0000 0072 5300 0000 da03 7374 7272 5500  ...rS.....strrU.
+00000d30: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00000d40: 0072 0e00 0000 7234 0000 0035 0000 0073  .r....r4...5...s
+00000d50: 3800 0000 0a00 0402 0c02 0c01 0c01 0c01  8...............
+00000d60: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000d70: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000d80: 0c01 0c01 0c01 0c01 0c01 1001 7234 0000  ............r4..
+00000d90: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000da0: 0000 0400 0000 4000 0000 73a0 0000 0065  ......@...s....e
+00000db0: 005a 0164 005a 0255 0064 015a 0369 0064  .Z.d.Z.U.d.Z.i.d
+00000dc0: 0264 0393 0164 0464 0593 0164 0664 0793  .d...d.d...d.d..
+00000dd0: 0164 0864 0993 0164 0a64 0b93 0164 0c64  .d.d...d.d...d.d
+00000de0: 0d93 0164 0e64 0f93 0164 1064 0f93 0164  ...d.d...d.d...d
+00000df0: 1164 1293 0164 1364 1493 0164 1564 1493  .d...d.d...d.d..
+00000e00: 0164 1664 1493 0164 1764 1493 0164 1864  .d.d...d.d...d.d
+00000e10: 1993 0164 1a64 0f93 0164 1b64 1c93 0164  ...d.d...d.d...d
+00000e20: 1d64 1e93 015a 0464 1f5a 0565 0665 0765  .d...Z.d.Z.e.e.e
+00000e30: 0865 0966 0219 0019 0065 0a64 203c 0064  .e.f.....e.d <.d
+00000e40: 215a 0b65 0965 0a64 223c 0064 1f53 0029  !Z.e.e.d"<.d.S.)
+00000e50: 23da 1758 6762 6f6f 7374 4669 6e61 6c50  #..XgboostFinalP
+00000e60: 6172 616d 436f 6e66 6967 7a1e 4465 6669  aramConfigz.Defi
+00000e70: 6e65 2066 696e 616c 2068 7970 6572 2070  ne final hyper p
+00000e80: 6172 616d 6574 6572 732e da09 6f62 6a65  arameters...obje
+00000e90: 6374 6976 6572 5200 0000 da0b 6576 616c  ctiverR.....eval
+00000ea0: 5f6d 6574 7269 6372 5400 0000 da07 7665  _metricrT.....ve
+00000eb0: 7262 6f73 6572 0100 0000 da0b 7472 6565  rboser......tree
+00000ec0: 5f6d 6574 686f 64da 0565 7861 6374 da09  _method..exact..
+00000ed0: 6e75 6d5f 636c 6173 7372 3500 0000 da09  num_classr5.....
+00000ee0: 6d61 785f 6465 7074 6872 3700 0000 da05  max_depthr7.....
+00000ef0: 616c 7068 6172 4b00 0000 da06 6c61 6d62  alpharK.....lamb
+00000f00: 6461 da0a 6e75 6d5f 6c65 6176 6573 e910  da..num_leaves..
+00000f10: 0000 00da 0973 7562 7361 6d70 6c65 721c  .....subsampler.
+00000f20: 0000 00da 1063 6f6c 7361 6d70 6c65 5f62  .....colsample_b
+00000f30: 7974 7265 65da 1163 6f6c 7361 6d70 6c65  ytree..colsample
+00000f40: 5f62 796c 6576 656c da10 636f 6c73 616d  _bylevel..colsam
+00000f50: 706c 655f 6279 6e6f 6465 da11 6d69 6e5f  ple_bynode..min_
+00000f60: 6368 696c 645f 7361 6d70 6c65 7372 1300  child_samplesr..
+00000f70: 0000 724c 0000 00da 0573 7465 7073 7249  ..rL.....stepsrI
+00000f80: 0000 00da 116e 756d 5f70 6172 616c 6c65  .....num_paralle
+00000f90: 6c5f 7472 6565 7216 0000 004e da0d 7361  l_treer....N..sa
+00000fa0: 6d70 6c65 5f77 6569 6768 7467 0000 0000  mple_weightg....
+00000fb0: 0000 e03f da18 636c 6173 7369 6669 6361  ...?..classifica
+00000fc0: 7469 6f6e 5f74 6872 6573 686f 6c64 290c  tion_threshold).
+00000fd0: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00000fe0: 2000 0000 da06 7061 7261 6d73 726a 0000   .....paramsrj..
+00000ff0: 0072 0300 0000 7202 0000 0072 5600 0000  .r....r....rV...
+00001000: 7224 0000 0072 2200 0000 726b 0000 0072  r$...r"...rk...r
+00001010: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00001020: 0000 0072 5700 0000 5500 0000 734e 0000  ...rW...U...sN..
+00001030: 000a 0004 0202 0204 0102 ff04 0202 fe04  ................
+00001040: 0302 fd04 0402 fc04 0502 fb04 0602 fa04  ................
+00001050: 0702 f904 0802 f804 0902 f704 0a02 f604  ................
+00001060: 0b02 f504 0c02 f404 0d02 f304 0e02 f204  ................
+00001070: 0f02 f104 1002 f004 1104 ef18 1310 0172  ...............r
+00001080: 5700 0000 2914 7220 0000 00da 0674 7970  W...).r .....typ
+00001090: 696e 6772 0200 0000 7203 0000 00da 0778  ingr....r......x
+000010a0: 6762 6f6f 7374 7232 0000 005a 1470 7964  gboostr2...Z.pyd
+000010b0: 616e 7469 632e 6461 7461 636c 6173 7365  antic.dataclasse
+000010c0: 7372 0400 0000 da19 736b 6c65 6172 6e2e  sr......sklearn.
+000010d0: 6665 6174 7572 655f 7365 6c65 6374 696f  feature_selectio
+000010e0: 6e72 0500 0000 da0f 736b 6c65 6172 6e2e  nr......sklearn.
+000010f0: 6d65 7472 6963 7372 0600 0000 7207 0000  metricsr....r...
+00001100: 00da 1773 6b6c 6561 726e 2e6d 6f64 656c  ...sklearn.model
+00001110: 5f73 656c 6563 7469 6f6e 7208 0000 0072  _selectionr....r
+00001120: 0900 0000 720f 0000 0072 2600 0000 7234  ....r....r&...r4
+00001130: 0000 0072 5700 0000 720d 0000 0072 0d00  ...rW...r....r..
+00001140: 0000 720d 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
+00001150: 6f64 756c 653e 0100 0000 7320 0000 0004  odule>....s ....
+00001160: 0010 0708 020c 010c 0110 010c 010e 0302  ................
+00001170: 0410 0108 1110 0102 0d10 0102 1f14 01    ...............
```

### Comparing `bluecast-0.3.1/bluecast/config/__pycache__/training_config.cpython-38.pyc` & `bluecast-0.4/bluecast/config/__pycache__/training_config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/config/training_config.py` & `bluecast-0.4/bluecast/config/training_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,25 @@
     global_random_state: int = 10
     shuffle_during_training: bool = True
     hyperparameter_tuning_rounds: int = 100
     hyperparameter_tuning_max_runtime_secs: int = 3600
     hypertuning_cv_folds: int = 1
     early_stopping_rounds: int = 10
     autotune_model: bool = True
+    enable_feature_selection: bool = False
     calculate_shap_values: bool = True
     train_size: float = 0.8
     train_split_stratify: bool = True
     use_full_data_for_final_model: bool = True
 
 
 @dataclass(config=Config)
 class FeatureSelectionConfig:
     """Define feature selection parameters."""
 
-    execute_selection: bool = True
     selection_strategy: RFECV = RFECV(
         estimator=xgb.XGBClassifier(),
         step=1,
         cv=StratifiedKFold(5, random_state=0, shuffle=True),
         min_features_to_select=1,
         scoring=make_scorer(matthews_corrcoef),
         n_jobs=4,
```

### Comparing `bluecast-0.3.1/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc` & `bluecast-0.4/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc` & `bluecast-0.4/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc` & `bluecast-0.4/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc` & `bluecast-0.4/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/evaluation/eval_metrics.py` & `bluecast-0.4/bluecast/evaluation/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/evaluation/shap_values.py` & `bluecast-0.4/bluecast/evaluation/shap_values.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc` & `bluecast-0.4/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc` & `bluecast-0.4/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/general_utils/general_utils.py` & `bluecast-0.4/bluecast/general_utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc` & `bluecast-0.4/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc` & `bluecast-0.4/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc` & `bluecast-0.4/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 10:39:10 2023 UTC, .py size: 13556 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4e76 9564 f434 0000  o.......Nv.d.4..
+00000000: 6f0d 0d0a 0000 0000 9caa 9564 d334 0000  o..........d.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6401 6404 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6404 6c09 5a09 6401 6404 6c0a 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6404 6c0c 5a0d 6401 6405 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -149,15 +149,15 @@
 00000940: 0114 0112 0206 0208 0114 0112 0206 0208  ................
 00000950: 0116 0116 027a 1d58 6762 6f6f 7374 4d6f  .....z.XgboostMo
 00000960: 6465 6c2e 6368 6563 6b5f 6c6f 6164 5f63  del.check_load_c
 00000970: 6f6e 6673 da07 785f 7472 6169 6eda 0678  onfs..x_train..x
 00000980: 5f74 6573 74da 0779 5f74 7261 696e da06  _test..y_train..
 00000990: 795f 7465 7374 6305 0000 0000 0000 0000  y_testc.........
 000009a0: 0000 0009 0000 0007 0000 0043 0000 0073  ...........C...s
-000009b0: 4a01 0000 7400 7401 a002 a100 9b00 6401  J...t.t.......d.
+000009b0: 3e01 0000 7400 7401 a002 a100 9b00 6401  >...t.t.......d.
 000009c0: 9d02 8301 0100 7c00 a003 a100 0100 7c00  ......|.......|.
 000009d0: 6a04 7213 7c00 6a05 7317 7406 6402 8301  j.r.|.j.s.t.d...
 000009e0: 8201 7c00 6a05 6a07 7223 7c00 a008 7c01  ..|.j.j.r#|...|.
 000009f0: 7c02 7c03 7c04 a104 0100 7409 6403 8301  |.|.|.....t.d...
 00000a00: 0100 7409 6404 8301 0100 7c00 6a05 6a0a  ..t.d.....|.j.j.
 00000a10: 7246 7400 7401 a002 a100 9b00 6405 9d02  rFt.t.......d...
 00000a20: 8301 0100 740b a00c 7c01 7c02 6702 a101  ....t...|.|.g...
@@ -166,399 +166,398 @@
 00000a50: 7d05 740f 6a10 7c01 7c03 7c05 6406 8d03  }.t.j.|.|.|.d...
 00000a60: 7d06 6e07 740f 6a10 7c01 7c03 6407 8d02  }.n.t.j.|.|.d...
 00000a70: 7d06 740f 6a10 7c02 7c04 6407 8d02 7d07  }.t.j.|.|.d...}.
 00000a80: 7c06 6408 6602 7c07 6409 6602 6702 7d08  |.d.f.|.d.f.g.}.
 00000a90: 7c00 6a05 6a11 640a 6b02 7288 740f 6a12  |.j.j.d.k.r.t.j.
 00000aa0: 7c00 6a04 6a13 7c06 7c00 6a04 6a13 640b  |.j.j.|.|.j.j.d.
 00000ab0: 1900 7c00 6a05 6a14 7c08 640c 8d05 7c00  ..|.j.j.|.d...|.
-00000ac0: 5f15 6e16 740f 6a12 7c00 6a04 6a13 7c06  _.n.t.j.|.j.j.|.
-00000ad0: 7c00 6a04 6a13 640b 1900 7c06 6408 6602  |.j.j.d...|.d.f.
-00000ae0: 7c07 6409 6602 6702 640d 8d04 7c00 5f15  |.d.f.g.d...|._.
-00000af0: 7409 640e 8301 0100 7c00 6a15 5300 290f  t.d.....|.j.S.).
-00000b00: 7a3f 5472 6169 6e20 5867 626f 6f73 7420  z?Train Xgboost 
-00000b10: 6d6f 6465 6c2e 2049 6e63 6c75 6465 7320  model. Includes 
-00000b20: 6879 7065 7270 6172 616d 6574 6572 2074  hyperparameter t
-00000b30: 756e 696e 6720 6f6e 2064 6566 6175 6c74  uning on default
-00000b40: 2e7a 1e3a 2053 7461 7274 2066 6974 7469  .z.: Start fitti
-00000b50: 6e67 2058 6762 6f6f 7374 206d 6f64 656c  ng Xgboost model
-00000b60: 2e7a 2c63 6f6e 665f 7061 7261 6d73 5f78  .z,conf_params_x
-00000b70: 6762 6f6f 7374 206f 7220 636f 6e66 5f74  gboost or conf_t
-00000b80: 7261 696e 696e 6720 6973 204e 6f6e 657a  raining is Nonez
-00000b90: 1e46 696e 6973 6865 6420 6879 7065 7270  .Finished hyperp
-00000ba0: 6172 616d 6574 6572 2074 756e 696e 677a  arameter tuningz
-00000bb0: 0e53 7461 7274 2074 7261 696e 696e 677a  .Start trainingz
-00000bc0: 7f3a 2055 6e69 6f6e 2074 7261 696e 2061  .: Union train a
-00000bd0: 6e64 2074 6573 7420 6461 7461 2066 6f72  nd test data for
-00000be0: 2066 696e 616c 206d 6f64 656c 2074 7261   final model tra
-00000bf0: 696e 696e 6720 6261 7365 6420 6f6e 2054  ining based on T
-00000c00: 7261 696e 696e 6743 6f6e 6669 670a 2020  rainingConfig.  
-00000c10: 2020 2020 2020 2020 2020 2070 6172 616d             param
-00000c20: 2027 7573 655f 6675 6c6c 5f64 6174 615f   'use_full_data_
-00000c30: 666f 725f 6669 6e61 6c5f 6d6f 6465 6c27  for_final_model'
-00000c40: a902 da05 6c61 6265 6cda 0677 6569 6768  ....label..weigh
-00000c50: 74a9 0172 2800 0000 da05 7472 6169 6eda  t..r(.....train.
-00000c60: 0474 6573 74e9 0100 0000 da05 7374 6570  .test.......step
-00000c70: 7329 03da 0f6e 756d 5f62 6f6f 7374 5f72  s)...num_boost_r
-00000c80: 6f75 6e64 da15 6561 726c 795f 7374 6f70  ound..early_stop
-00000c90: 7069 6e67 5f72 6f75 6e64 73da 0565 7661  ping_rounds..eva
-00000ca0: 6c73 2902 722f 0000 00da 0865 7661 6c5f  ls).r/.....eval_
-00000cb0: 7365 747a 1146 696e 6973 6865 6420 7472  setz.Finished tr
-00000cc0: 6169 6e69 6e67 2916 720d 0000 0072 0200  aining).r....r..
-00000cd0: 0000 721e 0000 0072 2200 0000 7215 0000  ..r....r"...r...
-00000ce0: 0072 1300 0000 da0a 5661 6c75 6545 7272  .r......ValueErr
-00000cf0: 6f72 da0e 6175 746f 7475 6e65 5f6d 6f64  or..autotune_mod
-00000d00: 656c da08 6175 746f 7475 6e65 da05 7072  el..autotune..pr
-00000d10: 696e 74da 1d75 7365 5f66 756c 6c5f 6461  int..use_full_da
-00000d20: 7461 5f66 6f72 5f66 696e 616c 5f6d 6f64  ta_for_final_mod
-00000d30: 656c da02 7064 da06 636f 6e63 6174 da0d  el..pd..concat..
-00000d40: 7361 6d70 6c65 5f77 6569 6768 7472 2100  sample_weightr!.
-00000d50: 0000 da03 7867 62da 0744 4d61 7472 6978  ....xgb..DMatrix
-00000d60: da14 6879 7065 7274 756e 696e 675f 6376  ..hypertuning_cv
-00000d70: 5f66 6f6c 6473 722b 0000 00da 0670 6172  _foldsr+.....par
-00000d80: 616d 7372 3000 0000 7216 0000 0029 0972  amsr0...r....).r
-00000d90: 1700 0000 7223 0000 0072 2400 0000 7225  ....r#...r$...r%
-00000da0: 0000 0072 2600 0000 7220 0000 00da 0764  ...r&...r .....d
-00000db0: 5f74 7261 696e da06 645f 7465 7374 7232  _train..d_testr2
-00000dc0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000dd0: 0000 da03 6669 7447 0000 0073 4800 0000  ....fitG...sH...
-00000de0: 1208 0801 0c02 0801 0802 1001 0802 0802  ................
-00000df0: 0801 0201 0c01 04ff 0e04 0e01 0802 0a01  ................
-00000e00: 1201 0e02 0e02 1001 0c02 0401 0601 0201  ................
-00000e10: 0a01 0601 0201 0afb 0408 0601 0201 0a01  ................
-00000e20: 0e01 08fc 0806 0601 7a10 5867 626f 6f73  ........z.Xgboos
-00000e30: 744d 6f64 656c 2e66 6974 6305 0000 0000  tModel.fitc.....
-00000e40: 0000 0000 0000 000b 0000 000a 0000 0003  ................
-00000e50: 0000 0073 c201 0000 7400 7401 a002 a100  ...s....t.t.....
-00000e60: 9b00 6401 9d02 8301 0100 7403 6a04 7c02  ..d.......t.j.|.
-00000e70: 8804 6402 8d02 8900 7405 8300 8902 8801  ..d.....t.......
-00000e80: a006 a100 0100 8801 6a07 7220 8801 6a08  ........j.r ..j.
-00000e90: 7220 8801 6a09 7324 740a 6403 8301 8201  r ..j.s$t.d.....
-00000ea0: 8700 8701 8702 8703 8704 8705 6606 6404  ............f.d.
-00000eb0: 6405 8408 7d05 6406 7d06 740b 6a0c 6a0d  d...}.d.}.t.j.j.
-00000ec0: 6407 8801 6a08 6a0e 6408 8d02 7d07 740b  d...j.j.d...}.t.
-00000ed0: 6a0f 6409 7c07 7c06 9b00 640a 9d02 640b  j.d.|.|...d...d.
-00000ee0: 8d03 7d08 7c08 6a10 7c05 8801 6a08 6a11  ..}.|.j.|...j.j.
-00000ef0: 8801 6a08 6a12 6407 6407 640c 8d05 0100  ..j.j.d.d.d.....
-00000f00: 7a16 740b 6a13 a014 7c08 a101 7d09 7c09  z.t.j...|...}.|.
-00000f10: a015 a100 0100 740b 6a13 a016 7c08 a101  ......t.j...|...
-00000f20: 7d09 7c09 a015 a100 0100 5700 6e0c 0400  }.|.......W.n...
-00000f30: 7417 7418 740a 6603 7976 0100 0100 0100  t.t.t.f.yv......
-00000f40: 5900 6e01 7700 7c08 6a19 6a1a 7d0a 6900  Y.n.w.|.j.j.}.i.
-00000f50: 640d 8801 6a09 6a1b 9301 640e 8801 6a09  d...j.j...d...j.
-00000f60: 6a1c 9301 640f 8801 6a09 6a1d 9301 6410  j...d...j.j...d.
-00000f70: 8802 9301 6411 8805 a01e a100 9301 6412  ....d.........d.
-00000f80: 7c0a 6412 1900 9301 6413 7c0a 6413 1900  |.d.....d.|.d...
-00000f90: 9301 6414 7c0a 6414 1900 9301 6415 7c0a  ..d.|.d.....d.|.
-00000fa0: 6415 1900 9301 6416 7c0a 6416 1900 9301  d.....d.|.d.....
-00000fb0: 6417 7c0a 6417 1900 9301 6418 7c0a 6418  d.|.d.....d.|.d.
-00000fc0: 1900 9301 6419 7c0a 6419 1900 9301 641a  ....d.|.d.....d.
-00000fd0: 7c0a 641a 1900 9301 641b 8801 6a09 6a1f  |.d.....d...j.j.
-00000fe0: 9301 641c 7c0a 641c 1900 9301 641d 7c0a  ..d.|.d.....d.|.
-00000ff0: 641d 1900 9301 8801 6a07 5f1a 7420 641e  d.......j._.t d.
-00001000: 8801 6a07 6a1a 8302 0100 7c0a 641f 1900  ..j.j.....|.d...
-00001010: 8801 6a07 5f21 6420 5300 2921 7a7b 5475  ..j._!d S.)!z{Tu
-00001020: 6e65 2068 7970 6572 7061 7261 6d65 7465  ne hyperparamete
-00001030: 7273 2e0a 0a20 2020 2020 2020 2041 6e20  rs...        An 
-00001040: 616c 7465 726e 6174 6976 6520 636f 6e66  alternative conf
-00001050: 6967 2063 616e 2062 6520 7072 6f76 6964  ig can be provid
-00001060: 6564 2074 6f20 6f76 6572 7772 6974 6520  ed to overwrite 
-00001070: 7468 6520 6879 7065 7270 6172 616d 6574  the hyperparamet
-00001080: 6572 2073 6561 7263 6820 7370 6163 652e  er search space.
-00001090: 0a20 2020 2020 2020 207a 2f3a 2053 7461  .        z/: Sta
-000010a0: 7274 2068 7970 6572 7061 7261 6d65 7465  rt hyperparamete
-000010b0: 7220 7475 6e69 6e67 206f 6620 5867 626f  r tuning of Xgbo
-000010c0: 6f73 7420 6d6f 6465 6c2e 722a 0000 007a  ost model.r*...z
-000010d0: 3941 7420 6c65 6173 7420 6f6e 6520 6f66  9At least one of
-000010e0: 2074 6865 2063 6f6e 6669 6773 2069 7320   the configs is 
-000010f0: 4e6f 6e65 2c20 7768 6963 6820 6973 206e  None, which is n
-00001100: 6f74 2061 6c6c 6f77 6564 6301 0000 0000  ot allowedc.....
-00001110: 0000 0000 0000 000c 0000 000a 0000 0013  ................
-00001120: 0000 0073 3c02 0000 6900 6401 8801 6a00  ...s<...i.d...j.
-00001130: 6a01 9301 6402 8801 6a00 6a02 9301 6403  j...d...j.j...d.
-00001140: 8801 6a00 6a03 9301 6404 8802 9301 6405  ..j.j...d.....d.
-00001150: 8805 a004 a100 9301 6406 7c00 a005 6406  ........d.|...d.
-00001160: 8801 6a00 6a06 8801 6a00 6a07 a103 9301  ..j.j...j.j.....
-00001170: 6407 7c00 a008 6407 8801 6a00 6a09 8801  d.|...d...j.j...
-00001180: 6a00 6a0a a103 9301 6408 7c00 a008 6408  j.j.....d.|...d.
-00001190: 8801 6a00 6a0b 8801 6a00 6a0c a103 9301  ..j.j...j.j.....
-000011a0: 6409 7c00 a005 6409 8801 6a00 6a0d 8801  d.|...d...j.j...
-000011b0: 6a00 6a0e a103 9301 640a 7c00 a008 640a  j.j.....d.|...d.
-000011c0: 8801 6a00 6a0f 8801 6a00 6a10 a103 9301  ..j.j...j.j.....
-000011d0: 640b 7c00 a008 640b 8801 6a00 6a11 8801  d.|...d...j.j...
-000011e0: 6a00 6a12 a103 9301 640c 7c00 a008 640c  j.j.....d.|...d.
-000011f0: 8801 6a00 6a13 8801 6a00 6a14 a103 9301  ..j.j...j.j.....
-00001200: 640d 7c00 a008 640d 8801 6a00 6a15 8801  d.|...d...j.j...
-00001210: 6a00 6a16 a103 9301 640e 7c00 a005 640e  j.j.....d.|...d.
-00001220: 8801 6a00 6a17 8801 6a00 6a18 a103 9301  ..j.j...j.j.....
-00001230: 640f 8801 6a00 6a19 9301 6410 7c00 a005  d...j.j...d.|...
-00001240: 6410 8801 6a00 6a1a 8801 6a00 6a1b a103  d...j.j...j.j...
-00001250: 9301 6411 7c00 a005 6411 8801 6a00 6a1c  ..d.|...d...j.j.
-00001260: 8801 6a00 6a1d a103 9301 7d01 7c00 a01e  ..j.j.....}.|...
-00001270: 6412 6413 6414 6702 a102 7d02 7c02 72ba  d.d.d.g...}.|.r.
-00001280: 8801 a01f 8805 a101 7d03 7420 6a21 8803  ........}.t j!..
-00001290: 8805 7c03 6415 8d03 7d04 6e07 7420 6a21  ..|.d...}.n.t j!
-000012a0: 8803 8805 6416 8d02 7d04 7422 6a23 a024  ....d...}.t"j#.$
-000012b0: 7c00 6417 a102 7d05 8801 6a25 6a26 6418  |.d...}...j%j&d.
-000012c0: 6b02 9001 7202 7c04 6419 6602 8800 641a  k...r.|.d.f...d.
-000012d0: 6602 6702 7d06 7420 6a27 7c01 7c04 7c01  f.g.}.t j'|.|.|.
-000012e0: 6410 1900 8801 6a25 6a28 7c06 7c05 6701  d.....j%j(|.|.g.
-000012f0: 8801 6a00 6a03 641b 8d07 7d07 7c07 a029  ..j.j.d...}.|..)
-00001300: 8800 a101 7d08 742a a02b 641c 641d 8400  ....}.t*.+d.d...
-00001310: 7c08 4400 8301 a101 7d09 742c 8804 7c09  |.D.....}.t,..|.
-00001320: 8302 641e 1400 7d0a 7c0a 5300 7420 6a2d  ..d...}.|.S.t j-
-00001330: 7c01 7c04 7c01 6410 1900 8801 6a25 6a26  |.|.|.d.....j%j&
-00001340: 6413 8801 6a25 6a2e 7c05 6701 8801 6a25  d...j%j.|.g...j%
-00001350: 6a2f 641f 8d08 7d0b 7c0b 6420 1900 a030  j/d...}.|.d ...0
-00001360: a100 5300 2921 4eda 096f 626a 6563 7469  ..S.)!N..objecti
-00001370: 7665 da0b 6576 616c 5f6d 6574 7269 63da  ve..eval_metric.
-00001380: 0776 6572 626f 7365 da0b 7472 6565 5f6d  .verbose..tree_m
-00001390: 6574 686f 64da 096e 756d 5f63 6c61 7373  ethod..num_class
-000013a0: da09 6d61 785f 6465 7074 68da 0561 6c70  ..max_depth..alp
-000013b0: 6861 da06 6c61 6d62 6461 da0a 6e75 6d5f  ha..lambda..num_
-000013c0: 6c65 6176 6573 da09 7375 6273 616d 706c  leaves..subsampl
-000013d0: 65da 1063 6f6c 7361 6d70 6c65 5f62 7974  e..colsample_byt
-000013e0: 7265 65da 1163 6f6c 7361 6d70 6c65 5f62  ree..colsample_b
-000013f0: 796c 6576 656c da10 636f 6c73 616d 706c  ylevel..colsampl
-00001400: 655f 6279 6e6f 6465 da11 6d69 6e5f 6368  e_bynode..min_ch
-00001410: 696c 645f 7361 6d70 6c65 73da 0365 7461  ild_samples..eta
-00001420: 722e 0000 00da 116e 756d 5f70 6172 616c  r......num_paral
-00001430: 6c65 6c5f 7472 6565 723a 0000 0054 4672  lel_treer:...TFr
-00001440: 2700 0000 722a 0000 007a 0d74 6573 742d  '...r*...z.test-
-00001450: 6d6c 6f67 6c6f 7373 722d 0000 0072 2b00  mloglossr-...r+.
-00001460: 0000 722c 0000 0029 0572 2f00 0000 7230  ..r,...).r/...r0
-00001470: 0000 0072 3100 0000 da09 6361 6c6c 6261  ...r1.....callba
-00001480: 636b 73da 0c76 6572 626f 7365 5f65 7661  cks..verbose_eva
-00001490: 6c63 0100 0000 0000 0000 0000 0000 0200  lc..............
-000014a0: 0000 0500 0000 5300 0000 f316 0000 0067  ......S........g
-000014b0: 007c 005d 077d 0174 00a0 017c 01a1 0191  .|.].}.t...|....
-000014c0: 0271 0253 0072 1800 0000 a902 da02 6e70  .q.S.r........np
-000014d0: da06 6172 676d 6178 a902 da02 2e30 da04  ..argmax.....0..
-000014e0: 6c69 6e65 7218 0000 0072 1800 0000 7219  liner....r....r.
-000014f0: 0000 00da 0a3c 6c69 7374 636f 6d70 3ee9  .....<listcomp>.
-00001500: 0000 00f3 0200 0000 1600 7a3c 5867 626f  ..........z<Xgbo
-00001510: 6f73 744d 6f64 656c 2e61 7574 6f74 756e  ostModel.autotun
-00001520: 652e 3c6c 6f63 616c 733e 2e6f 626a 6563  e.<locals>.objec
-00001530: 7469 7665 2e3c 6c6f 6361 6c73 3e2e 3c6c  tive.<locals>.<l
-00001540: 6973 7463 6f6d 703e e9ff ffff ff29 0872  istcomp>.....).r
-00001550: 3e00 0000 da06 6474 7261 696e 722f 0000  >.....dtrainr/..
-00001560: 00da 056e 666f 6c64 da09 6173 5f70 616e  ...nfold..as_pan
-00001570: 6461 73da 0473 6565 6472 5200 0000 da07  das..seedrR.....
-00001580: 7368 7566 666c 657a 1274 6573 742d 6d6c  shufflez.test-ml
-00001590: 6f67 6c6f 7373 2d6d 6561 6e29 3172 1400  ogloss-mean)1r..
-000015a0: 0000 da0f 6d6f 6465 6c5f 6f62 6a65 6374  ....model_object
-000015b0: 6976 65da 116d 6f64 656c 5f65 7661 6c5f  ive..model_eval_
-000015c0: 6d65 7472 6963 da0f 6d6f 6465 6c5f 7665  metric..model_ve
-000015d0: 7262 6f73 6974 79da 076e 756e 6971 7565  rbosity..nunique
-000015e0: 5a0b 7375 6767 6573 745f 696e 74da 0d6d  Z.suggest_int..m
-000015f0: 6178 5f64 6570 7468 5f6d 696e da0d 6d61  ax_depth_min..ma
-00001600: 785f 6465 7074 685f 6d61 785a 0d73 7567  x_depth_maxZ.sug
-00001610: 6765 7374 5f66 6c6f 6174 da09 616c 7068  gest_float..alph
-00001620: 615f 6d69 6eda 0961 6c70 6861 5f6d 6178  a_min..alpha_max
-00001630: da0a 6c61 6d62 6461 5f6d 696e da0a 6c61  ..lambda_min..la
-00001640: 6d62 6461 5f6d 6178 da0e 6e75 6d5f 6c65  mbda_max..num_le
-00001650: 6176 6573 5f6d 696e da0e 6e75 6d5f 6c65  aves_min..num_le
-00001660: 6176 6573 5f6d 6178 da0e 7375 625f 7361  aves_max..sub_sa
-00001670: 6d70 6c65 5f6d 696e da0e 7375 625f 7361  mple_min..sub_sa
-00001680: 6d70 6c65 5f6d 6178 da16 636f 6c5f 7361  mple_max..col_sa
-00001690: 6d70 6c65 5f62 795f 7472 6565 5f6d 696e  mple_by_tree_min
-000016a0: da16 636f 6c5f 7361 6d70 6c65 5f62 795f  ..col_sample_by_
-000016b0: 7472 6565 5f6d 6178 da17 636f 6c5f 7361  tree_max..col_sa
-000016c0: 6d70 6c65 5f62 795f 6c65 7665 6c5f 6d69  mple_by_level_mi
-000016d0: 6eda 1763 6f6c 5f73 616d 706c 655f 6279  n..col_sample_by
-000016e0: 5f6c 6576 656c 5f6d 6178 da16 636f 6c5f  _level_max..col_
-000016f0: 7361 6d70 6c65 5f62 795f 6e6f 6465 5f6d  sample_by_node_m
-00001700: 696e da16 636f 6c5f 7361 6d70 6c65 5f62  in..col_sample_b
-00001710: 795f 6e6f 6465 5f6d 6178 da15 6d69 6e5f  y_node_max..min_
-00001720: 6368 696c 645f 7361 6d70 6c65 735f 6d69  child_samples_mi
-00001730: 6eda 156d 696e 5f63 6869 6c64 5f73 616d  n..min_child_sam
-00001740: 706c 6573 5f6d 6178 7250 0000 00da 0973  ples_maxrP.....s
-00001750: 7465 7073 5f6d 696e da09 7374 6570 735f  teps_min..steps_
-00001760: 6d61 78da 156e 756d 5f70 6172 616c 6c65  max..num_paralle
-00001770: 6c5f 7472 6565 5f6d 696e da15 6e75 6d5f  l_tree_min..num_
-00001780: 7061 7261 6c6c 656c 5f74 7265 655f 6d61  parallel_tree_ma
-00001790: 785a 1373 7567 6765 7374 5f63 6174 6567  xZ.suggest_categ
-000017a0: 6f72 6963 616c 7221 0000 0072 3b00 0000  oricalr!...r;...
-000017b0: 723c 0000 00da 066f 7074 756e 615a 0b69  r<.....optunaZ.i
-000017c0: 6e74 6567 7261 7469 6f6e 5a16 5847 426f  ntegrationZ.XGBo
-000017d0: 6f73 7450 7275 6e69 6e67 4361 6c6c 6261  ostPruningCallba
-000017e0: 636b 7213 0000 0072 3d00 0000 722b 0000  ckr....r=...r+..
-000017f0: 0072 3000 0000 da07 7072 6564 6963 7472  .r0.....predictr
-00001800: 5600 0000 da07 6173 6172 7261 7972 0700  V.....asarrayr..
-00001810: 0000 da02 6376 da13 676c 6f62 616c 5f72  ....cv..global_r
-00001820: 616e 646f 6d5f 7374 6174 65da 1773 6875  andom_state..shu
-00001830: 6666 6c65 5f64 7572 696e 675f 7472 6169  ffle_during_trai
-00001840: 6e69 6e67 da04 6d65 616e 290c da05 7472  ning..mean)...tr
-00001850: 6961 6cda 0570 6172 616d 723a 0000 0072  ial..paramr:...r
-00001860: 2000 0000 723f 0000 005a 1070 7275 6e69   ...r?...Z.pruni
-00001870: 6e67 5f63 616c 6c62 6163 6b72 3200 0000  ng_callbackr2...
-00001880: 7216 0000 00da 0570 7265 6473 da0b 7072  r......preds..pr
-00001890: 6564 5f6c 6162 656c 735a 076d 6174 7468  ed_labelsZ.matth
-000018a0: 6577 da06 7265 7375 6c74 a906 7240 0000  ew..result..r@..
-000018b0: 0072 1700 0000 5a08 7472 6169 6e5f 6f6e  .r....Z.train_on
-000018c0: 7223 0000 0072 2600 0000 7225 0000 0072  r#...r&...r%...r
-000018d0: 1800 0000 7219 0000 0072 4200 0000 9800  ....r....rB.....
-000018e0: 0000 73d6 0000 0002 0108 0102 ff08 0202  ..s.............
-000018f0: fe08 0302 fd04 0402 fc08 0502 fb06 0602  ................
-00001900: 0106 0106 0102 fd02 fa06 0b0e 0102 ff02  ................
-00001910: f506 0e0e 0102 ff02 f206 1102 0106 0106  ................
-00001920: 0102 fd02 ef06 1602 0106 0106 0102 fd02  ................
-00001930: ea06 1b02 0106 0106 0102 fd02 e506 2002  .............. .
-00001940: 0106 0106 0102 fd02 e006 2502 0106 0106  ..........%.....
-00001950: 0102 fd02 db06 2a02 0106 0106 0102 fd02  ......*.........
-00001960: d608 2f02 d106 300e 0102 ff02 d006 3302  ../...0.......3.
-00001970: 0106 0106 0102 fd04 cd10 3904 010a 0112  ..........9.....
-00001980: 010e 0206 0204 0104 ff0e 0410 0104 0102  ................
-00001990: 0102 0106 0106 0102 0104 0106 0106 f90a  ................
-000019a0: 0914 010e 0104 0104 0202 0102 0106 0106  ................
-000019b0: 0202 0106 0104 0106 0106 f70c 0c7a 2858  .............z(X
-000019c0: 6762 6f6f 7374 4d6f 6465 6c2e 6175 746f  gboostModel.auto
-000019d0: 7475 6e65 2e3c 6c6f 6361 6c73 3e2e 6f62  tune.<locals>.ob
-000019e0: 6a65 6374 6976 65da 0778 6762 6f6f 7374  jective..xgboost
-000019f0: 5429 025a 0c6d 756c 7469 7661 7269 6174  T).Z.multivariat
-00001a00: 6572 6100 0000 da08 6d69 6e69 6d69 7a65  era.....minimize
-00001a10: 7a07 2074 756e 696e 6729 03da 0964 6972  z. tuning)...dir
-00001a20: 6563 7469 6f6e da07 7361 6d70 6c65 725a  ection..samplerZ
-00001a30: 0a73 7475 6479 5f6e 616d 6529 04da 086e  .study_name)...n
-00001a40: 5f74 7269 616c 73da 0774 696d 656f 7574  _trials..timeout
-00001a50: 5a0e 6763 5f61 6674 6572 5f74 7269 616c  Z.gc_after_trial
-00001a60: 5a11 7368 6f77 5f70 726f 6772 6573 735f  Z.show_progress_
-00001a70: 6261 7272 4200 0000 7243 0000 0072 4400  barrB...rC...rD.
-00001a80: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
-00001a90: 0072 4800 0000 7249 0000 0072 4a00 0000  .rH...rI...rJ...
-00001aa0: 724b 0000 0072 4c00 0000 724d 0000 0072  rK...rL...rM...r
-00001ab0: 4e00 0000 724f 0000 0072 5000 0000 722e  N...rO...rP...r.
-00001ac0: 0000 0072 5100 0000 7a0d 4265 7374 2070  ...rQ...z.Best p
-00001ad0: 6172 616d 733a 2072 3a00 0000 4e29 2272  arams: r:...N)"r
-00001ae0: 0d00 0000 7202 0000 0072 1e00 0000 723b  ....r....r....r;
-00001af0: 0000 0072 3c00 0000 720c 0000 0072 2200  ...r<...r....r".
-00001b00: 0000 7215 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00001b10: 0072 3300 0000 727d 0000 005a 0873 616d  .r3...r}...Z.sam
-00001b20: 706c 6572 735a 0a54 5045 5361 6d70 6c65  plersZ.TPESample
-00001b30: 7272 8100 0000 5a0c 6372 6561 7465 5f73  rr....Z.create_s
-00001b40: 7475 6479 da08 6f70 7469 6d69 7a65 da1c  tudy..optimize..
-00001b50: 6879 7065 7270 6172 616d 6574 6572 5f74  hyperparameter_t
-00001b60: 756e 696e 675f 726f 756e 6473 da26 6879  uning_rounds.&hy
-00001b70: 7065 7270 6172 616d 6574 6572 5f74 756e  perparameter_tun
-00001b80: 696e 675f 6d61 785f 7275 6e74 696d 655f  ing_max_runtime_
-00001b90: 7365 6373 5a0d 7669 7375 616c 697a 6174  secsZ.visualizat
-00001ba0: 696f 6e5a 1970 6c6f 745f 6f70 7469 6d69  ionZ.plot_optimi
-00001bb0: 7a61 7469 6f6e 5f68 6973 746f 7279 da04  zation_history..
-00001bc0: 7368 6f77 5a16 706c 6f74 5f70 6172 616d  showZ.plot_param
-00001bd0: 5f69 6d70 6f72 7461 6e63 6573 da11 5a65  _importances..Ze
-00001be0: 726f 4469 7669 7369 6f6e 4572 726f 72da  roDivisionError.
-00001bf0: 0c52 756e 7469 6d65 4572 726f 725a 0a62  .RuntimeErrorZ.b
-00001c00: 6573 745f 7472 6961 6c72 3e00 0000 7263  est_trialr>...rc
-00001c10: 0000 0072 6400 0000 7265 0000 0072 6600  ...rd...re...rf.
-00001c20: 0000 7250 0000 0072 3600 0000 723a 0000  ..rP...r6...r:..
-00001c30: 0029 0b72 1700 0000 7223 0000 0072 2400  .).r....r#...r$.
-00001c40: 0000 7225 0000 0072 2600 0000 7242 0000  ..r%...r&...rB..
-00001c50: 00da 0961 6c67 6f72 6974 686d 728d 0000  ...algorithmr...
-00001c60: 005a 0573 7475 6479 da03 6669 675a 1278  .Z.study..figZ.x
-00001c70: 6762 6f6f 7374 5f62 6573 745f 7061 7261  gboost_best_para
-00001c80: 6d72 1800 0000 7289 0000 0072 1900 0000  mr....r....r....
-00001c90: 7235 0000 007e 0000 0073 9c00 0000 120b  r5...~...s......
-00001ca0: 0e01 0601 0802 0403 02ff 0402 02fe 0403  ................
-00001cb0: 02fd 0205 0201 04ff 1604 0463 0601 0801  ...........c....
-00001cc0: 06ff 0403 0201 0201 0801 06fd 0406 0201  ................
-00001cd0: 0601 0601 0201 0201 06fb 0207 0c01 0801  ................
-00001ce0: 0c01 0c01 1201 0401 02ff 0803 0201 0801  ................
-00001cf0: 02ff 0802 02fe 0803 02fd 0404 02fc 0805  ................
-00001d00: 02fb 0406 0201 02ff 02fa 0809 02f7 080a  ................
-00001d10: 02f6 080b 02f5 080c 02f4 080d 02f3 080e  ................
-00001d20: 02f2 080f 02f1 0810 02f0 0811 02ef 0812  ................
-00001d30: 02ee 0813 08ed 0e15 1001 7a15 5867 626f  ..........z.Xgbo
-00001d40: 6f73 744d 6f64 656c 2e61 7574 6f74 756e  ostModel.autotun
-00001d50: 65da 0264 6663 0200 0000 0000 0000 0000  e..dfc..........
-00001d60: 0000 0600 0000 0400 0000 4300 0000 73a0  ..........C...s.
-00001d70: 0000 0074 0074 01a0 02a1 009b 0064 019d  ...t.t.......d..
-00001d80: 0283 0101 0074 0364 0283 0101 0074 04a0  .....t.d.....t..
-00001d90: 057c 01a1 017d 027c 006a 0673 1974 0764  .|...}.|.j.s.t.d
-00001da0: 0383 0182 017c 006a 0873 2074 0764 0483  .....|.j.s t.d..
-00001db0: 0182 017c 006a 06a0 097c 02a1 017d 037c  ...|.j...|...}.|
-00001dc0: 006a 0a64 056b 0272 3c74 0ba0 0c64 0664  .j.d.k.r<t...d.d
-00001dd0: 0784 007c 0344 0083 01a1 017d 047c 047c  ...|.D.....}.|.|
-00001de0: 006a 086a 0d6b 047d 056e 0c7c 037d 0474  .j.j.k.}.n.|.}.t
-00001df0: 0ba0 0c64 0864 0784 007c 0344 0083 01a1  ...d.d...|.D....
-00001e00: 017d 0574 0364 0983 0101 007c 047c 0566  .}.t.d.....|.|.f
-00001e10: 0253 0029 0a7a 1750 7265 6469 6374 206f  .S.).z.Predict o
-00001e20: 6e20 756e 7365 656e 2064 6174 612e 7a33  n unseen data.z3
-00001e30: 3a20 5374 6172 7420 7072 6564 6963 7469  : Start predicti
-00001e40: 6e67 206f 6e20 6e65 7720 6461 7461 2075  ng on new data u
-00001e50: 7369 6e67 2058 6762 6f6f 7374 206d 6f64  sing Xgboost mod
-00001e60: 656c 2e7a 1c2b 2b2b 2b2b 2b2b 2b2b 2b2b  el.z.+++++++++++
-00001e70: 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  ++++++++++++++++
-00001e80: 2b7a 204e 6f20 7472 6169 6e65 6420 6d6f  +z No trained mo
-00001e90: 6465 6c20 6861 7320 6265 656e 2066 6f75  del has been fou
-00001ea0: 6e64 2e7a 2b4e 6f20 6d6f 6465 6c20 636f  nd.z+No model co
-00001eb0: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00001ec0: 2068 6173 2062 6565 6e20 666f 756e 642e   has been found.
-00001ed0: 7211 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00001ee0: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
-00001ef0: 0000 0067 007c 005d 067d 017c 0164 0019  ...g.|.].}.|.d..
-00001f00: 0091 0271 0253 0029 0172 2d00 0000 7218  ...q.S.).r-...r.
-00001f10: 0000 0072 5800 0000 7218 0000 0072 1800  ...rX...r....r..
-00001f20: 0000 7219 0000 0072 5b00 0000 3c01 0000  ..r....r[...<...
-00001f30: 7302 0000 0014 007a 2858 6762 6f6f 7374  s......z(Xgboost
-00001f40: 4d6f 6465 6c2e 7072 6564 6963 742e 3c6c  Model.predict.<l
-00001f50: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00001f60: 3e63 0100 0000 0000 0000 0000 0000 0200  >c..............
-00001f70: 0000 0500 0000 5300 0000 7254 0000 0072  ......S...rT...r
-00001f80: 1800 0000 7255 0000 0072 5800 0000 7218  ....rU...rX...r.
-00001f90: 0000 0072 1800 0000 7219 0000 0072 5b00  ...r....r....r[.
-00001fa0: 0000 4201 0000 725c 0000 007a 1346 696e  ..B...r\...z.Fin
-00001fb0: 6973 6865 6420 7072 6564 6963 7469 6e67  ished predicting
-00001fc0: 290e 720d 0000 0072 0200 0000 721e 0000  ).r....r....r...
-00001fd0: 0072 3600 0000 723b 0000 0072 3c00 0000  .r6...r;...r<...
-00001fe0: 7216 0000 00da 0945 7863 6570 7469 6f6e  r......Exception
-00001ff0: 7215 0000 0072 7e00 0000 7210 0000 0072  r....r~...r....r
-00002000: 5600 0000 727f 0000 00da 1863 6c61 7373  V...r......class
-00002010: 6966 6963 6174 696f 6e5f 7468 7265 7368  ification_thresh
-00002020: 6f6c 6429 0672 1700 0000 7298 0000 0072  old).r....r....r
-00002030: 4000 0000 5a0d 7061 7274 6961 6c5f 7072  @...Z.partial_pr
-00002040: 6f62 735a 0f70 7265 6469 6374 6564 5f70  obsZ.predicted_p
-00002050: 726f 6273 da11 7072 6564 6963 7465 645f  robs..predicted_
-00002060: 636c 6173 7365 7372 1800 0000 7218 0000  classesr....r...
-00002070: 0072 1900 0000 727e 0000 002d 0100 0073  .r....r~...-...s
-00002080: 2400 0000 0202 0c01 04ff 0803 0a01 0601  $...............
-00002090: 0801 0602 0801 0c02 0a01 1401 0a02 04ff  ................
-000020a0: 0404 1401 0801 0801 7a14 5867 626f 6f73  ........z.Xgboos
-000020b0: 744d 6f64 656c 2e70 7265 6469 6374 2903  tModel.predict).
-000020c0: 4e4e 4e29 1ada 085f 5f6e 616d 655f 5fda  NNN)...__name__.
-000020d0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000020e0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
-000020f0: 5f5f 7204 0000 0072 0500 0000 7209 0000  __r....r....r...
-00002100: 0072 0b00 0000 720a 0000 0072 1a00 0000  .r....r....r....
-00002110: 7238 0000 00da 0653 6572 6965 7372 0300  r8.....Seriesr..
-00002120: 0000 da03 7374 72da 0566 6c6f 6174 7221  ....str..floatr!
-00002130: 0000 0072 2200 0000 da09 4461 7461 4672  ...r".....DataFr
-00002140: 616d 6572 3b00 0000 da07 426f 6f73 7465  amer;.....Booste
-00002150: 7272 4100 0000 7235 0000 0072 0600 0000  rrA...r5...r....
-00002160: 7256 0000 00da 076e 6461 7272 6179 727e  rV.....ndarrayr~
-00002170: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
-00002180: 0000 7219 0000 0072 0f00 0000 1a00 0000  ..r....r........
-00002190: 7350 0000 0008 0004 0102 0502 0102 0104  sP..............
-000021a0: fb06 0202 fe06 0302 fd06 0402 fc06 050a  ................
-000021b0: fb1c 0d08 0802 1504 0202 fe04 0302 fd04  ................
-000021c0: 0402 fc04 0502 fb04 060a fa02 3704 0202  ............7...
-000021d0: fe04 0302 fd04 0402 fc04 0502 fb02 060a  ................
-000021e0: fa00 7f24 3072 0f00 0000 291c 729f 0000  ...$0r....).r...
-000021f0: 0072 0200 0000 da06 7479 7069 6e67 7203  .r......typingr.
-00002200: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
-00002210: 0000 da05 6e75 6d70 7972 5600 0000 727d  ....numpyrV...r}
-00002220: 0000 00da 0670 616e 6461 7372 3800 0000  .....pandasr8...
-00002230: 728a 0000 0072 3b00 0000 5a0f 736b 6c65  r....r;...Z.skle
-00002240: 6172 6e2e 6d65 7472 6963 7372 0700 0000  arn.metricsr....
-00002250: da0d 736b 6c65 6172 6e2e 7574 696c 7372  ..sklearn.utilsr
-00002260: 0800 0000 da1f 626c 7565 6361 7374 2e63  ......bluecast.c
-00002270: 6f6e 6669 672e 7472 6169 6e69 6e67 5f63  onfig.training_c
-00002280: 6f6e 6669 6772 0900 0000 720a 0000 0072  onfigr....r....r
-00002290: 0b00 0000 da24 626c 7565 6361 7374 2e67  .....$bluecast.g
-000022a0: 656e 6572 616c 5f75 7469 6c73 2e67 656e  eneral_utils.gen
-000022b0: 6572 616c 5f75 7469 6c73 720c 0000 0072  eral_utilsr....r
-000022c0: 0d00 0000 da22 626c 7565 6361 7374 2e6d  ....."bluecast.m
-000022d0: 6c5f 6d6f 6465 6c6c 696e 672e 6261 7365  l_modelling.base
-000022e0: 5f63 6c61 7373 6573 720e 0000 0072 0f00  _classesr....r..
-000022f0: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
-00002300: 0072 1900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00002310: 0100 0000 731a 0000 0004 000c 0618 0108  ....s...........
-00002320: 0208 0108 0108 010c 010c 0114 0210 050c  ................
-00002330: 0114 03                                  ...
+00000ac0: 5f15 6e10 740f 6a12 7c00 6a04 6a13 7c06  _.n.t.j.|.j.j.|.
+00000ad0: 7c00 6a04 6a13 640b 1900 7c08 640d 8d04  |.j.j.d...|.d...
+00000ae0: 7c00 5f15 7409 640e 8301 0100 7c00 6a15  |._.t.d.....|.j.
+00000af0: 5300 290f 7a3f 5472 6169 6e20 5867 626f  S.).z?Train Xgbo
+00000b00: 6f73 7420 6d6f 6465 6c2e 2049 6e63 6c75  ost model. Inclu
+00000b10: 6465 7320 6879 7065 7270 6172 616d 6574  des hyperparamet
+00000b20: 6572 2074 756e 696e 6720 6f6e 2064 6566  er tuning on def
+00000b30: 6175 6c74 2e7a 1e3a 2053 7461 7274 2066  ault.z.: Start f
+00000b40: 6974 7469 6e67 2058 6762 6f6f 7374 206d  itting Xgboost m
+00000b50: 6f64 656c 2e7a 2c63 6f6e 665f 7061 7261  odel.z,conf_para
+00000b60: 6d73 5f78 6762 6f6f 7374 206f 7220 636f  ms_xgboost or co
+00000b70: 6e66 5f74 7261 696e 696e 6720 6973 204e  nf_training is N
+00000b80: 6f6e 657a 1e46 696e 6973 6865 6420 6879  onez.Finished hy
+00000b90: 7065 7270 6172 616d 6574 6572 2074 756e  perparameter tun
+00000ba0: 696e 677a 0e53 7461 7274 2074 7261 696e  ingz.Start train
+00000bb0: 696e 677a 7f3a 2055 6e69 6f6e 2074 7261  ingz.: Union tra
+00000bc0: 696e 2061 6e64 2074 6573 7420 6461 7461  in and test data
+00000bd0: 2066 6f72 2066 696e 616c 206d 6f64 656c   for final model
+00000be0: 2074 7261 696e 696e 6720 6261 7365 6420   training based 
+00000bf0: 6f6e 2054 7261 696e 696e 6743 6f6e 6669  on TrainingConfi
+00000c00: 670a 2020 2020 2020 2020 2020 2020 2070  g.             p
+00000c10: 6172 616d 2027 7573 655f 6675 6c6c 5f64  aram 'use_full_d
+00000c20: 6174 615f 666f 725f 6669 6e61 6c5f 6d6f  ata_for_final_mo
+00000c30: 6465 6c27 a902 da05 6c61 6265 6cda 0677  del'....label..w
+00000c40: 6569 6768 74a9 0172 2800 0000 da05 7472  eight..r(.....tr
+00000c50: 6169 6eda 0474 6573 74e9 0100 0000 da05  ain..test.......
+00000c60: 7374 6570 7329 03da 0f6e 756d 5f62 6f6f  steps)...num_boo
+00000c70: 7374 5f72 6f75 6e64 da15 6561 726c 795f  st_round..early_
+00000c80: 7374 6f70 7069 6e67 5f72 6f75 6e64 73da  stopping_rounds.
+00000c90: 0565 7661 6c73 2902 722f 0000 0072 3100  .evals).r/...r1.
+00000ca0: 0000 7a11 4669 6e69 7368 6564 2074 7261  ..z.Finished tra
+00000cb0: 696e 696e 6729 1672 0d00 0000 7202 0000  ining).r....r...
+00000cc0: 0072 1e00 0000 7222 0000 0072 1500 0000  .r....r"...r....
+00000cd0: 7213 0000 00da 0a56 616c 7565 4572 726f  r......ValueErro
+00000ce0: 72da 0e61 7574 6f74 756e 655f 6d6f 6465  r..autotune_mode
+00000cf0: 6cda 0861 7574 6f74 756e 65da 0570 7269  l..autotune..pri
+00000d00: 6e74 da1d 7573 655f 6675 6c6c 5f64 6174  nt..use_full_dat
+00000d10: 615f 666f 725f 6669 6e61 6c5f 6d6f 6465  a_for_final_mode
+00000d20: 6cda 0270 64da 0663 6f6e 6361 74da 0d73  l..pd..concat..s
+00000d30: 616d 706c 655f 7765 6967 6874 7221 0000  ample_weightr!..
+00000d40: 00da 0378 6762 da07 444d 6174 7269 78da  ...xgb..DMatrix.
+00000d50: 1468 7970 6572 7475 6e69 6e67 5f63 765f  .hypertuning_cv_
+00000d60: 666f 6c64 7372 2b00 0000 da06 7061 7261  foldsr+.....para
+00000d70: 6d73 7230 0000 0072 1600 0000 2909 7217  msr0...r....).r.
+00000d80: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
+00000d90: 0000 7226 0000 0072 2000 0000 da07 645f  ..r&...r .....d_
+00000da0: 7472 6169 6eda 0664 5f74 6573 74da 0865  train..d_test..e
+00000db0: 7661 6c5f 7365 7472 1800 0000 7218 0000  val_setr....r...
+00000dc0: 0072 1900 0000 da03 6669 7447 0000 0073  .r......fitG...s
+00000dd0: 4800 0000 1208 0801 0c02 0801 0802 1001  H...............
+00000de0: 0802 0802 0801 0201 0c01 04ff 0e04 0e01  ................
+00000df0: 0802 0a01 1201 0e02 0e02 1001 0c02 0401  ................
+00000e00: 0601 0201 0a01 0601 0201 0afb 0408 0601  ................
+00000e10: 0201 0a01 0201 08fc 0806 0601 7a10 5867  ............z.Xg
+00000e20: 626f 6f73 744d 6f64 656c 2e66 6974 6305  boostModel.fitc.
+00000e30: 0000 0000 0000 0000 0000 000b 0000 000a  ................
+00000e40: 0000 0003 0000 0073 c201 0000 7400 7401  .......s....t.t.
+00000e50: a002 a100 9b00 6401 9d02 8301 0100 7403  ......d.......t.
+00000e60: 6a04 7c02 8804 6402 8d02 8900 7405 8300  j.|...d.....t...
+00000e70: 8902 8801 a006 a100 0100 8801 6a07 7220  ............j.r 
+00000e80: 8801 6a08 7220 8801 6a09 7324 740a 6403  ..j.r ..j.s$t.d.
+00000e90: 8301 8201 8700 8701 8702 8703 8704 8705  ................
+00000ea0: 6606 6404 6405 8408 7d05 6406 7d06 740b  f.d.d...}.d.}.t.
+00000eb0: 6a0c 6a0d 6407 8801 6a08 6a0e 6408 8d02  j.j.d...j.j.d...
+00000ec0: 7d07 740b 6a0f 6409 7c07 7c06 9b00 640a  }.t.j.d.|.|...d.
+00000ed0: 9d02 640b 8d03 7d08 7c08 6a10 7c05 8801  ..d...}.|.j.|...
+00000ee0: 6a08 6a11 8801 6a08 6a12 6407 6407 640c  j.j...j.j.d.d.d.
+00000ef0: 8d05 0100 7a16 740b 6a13 a014 7c08 a101  ....z.t.j...|...
+00000f00: 7d09 7c09 a015 a100 0100 740b 6a13 a016  }.|.......t.j...
+00000f10: 7c08 a101 7d09 7c09 a015 a100 0100 5700  |...}.|.......W.
+00000f20: 6e0c 0400 7417 7418 740a 6603 7976 0100  n...t.t.t.f.yv..
+00000f30: 0100 0100 5900 6e01 7700 7c08 6a19 6a1a  ....Y.n.w.|.j.j.
+00000f40: 7d0a 6900 640d 8801 6a09 6a1b 9301 640e  }.i.d...j.j...d.
+00000f50: 8801 6a09 6a1c 9301 640f 8801 6a09 6a1d  ..j.j...d...j.j.
+00000f60: 9301 6410 8802 9301 6411 8805 a01e a100  ..d.....d.......
+00000f70: 9301 6412 7c0a 6412 1900 9301 6413 7c0a  ..d.|.d.....d.|.
+00000f80: 6413 1900 9301 6414 7c0a 6414 1900 9301  d.....d.|.d.....
+00000f90: 6415 7c0a 6415 1900 9301 6416 7c0a 6416  d.|.d.....d.|.d.
+00000fa0: 1900 9301 6417 7c0a 6417 1900 9301 6418  ....d.|.d.....d.
+00000fb0: 7c0a 6418 1900 9301 6419 7c0a 6419 1900  |.d.....d.|.d...
+00000fc0: 9301 641a 7c0a 641a 1900 9301 641b 8801  ..d.|.d.....d...
+00000fd0: 6a09 6a1f 9301 641c 7c0a 641c 1900 9301  j.j...d.|.d.....
+00000fe0: 641d 7c0a 641d 1900 9301 8801 6a07 5f1a  d.|.d.......j._.
+00000ff0: 7420 641e 8801 6a07 6a1a 8302 0100 7c0a  t d...j.j.....|.
+00001000: 641f 1900 8801 6a07 5f21 6420 5300 2921  d.....j._!d S.)!
+00001010: 7a7b 5475 6e65 2068 7970 6572 7061 7261  z{Tune hyperpara
+00001020: 6d65 7465 7273 2e0a 0a20 2020 2020 2020  meters...       
+00001030: 2041 6e20 616c 7465 726e 6174 6976 6520   An alternative 
+00001040: 636f 6e66 6967 2063 616e 2062 6520 7072  config can be pr
+00001050: 6f76 6964 6564 2074 6f20 6f76 6572 7772  ovided to overwr
+00001060: 6974 6520 7468 6520 6879 7065 7270 6172  ite the hyperpar
+00001070: 616d 6574 6572 2073 6561 7263 6820 7370  ameter search sp
+00001080: 6163 652e 0a20 2020 2020 2020 207a 2f3a  ace..        z/:
+00001090: 2053 7461 7274 2068 7970 6572 7061 7261   Start hyperpara
+000010a0: 6d65 7465 7220 7475 6e69 6e67 206f 6620  meter tuning of 
+000010b0: 5867 626f 6f73 7420 6d6f 6465 6c2e 722a  Xgboost model.r*
+000010c0: 0000 007a 3941 7420 6c65 6173 7420 6f6e  ...z9At least on
+000010d0: 6520 6f66 2074 6865 2063 6f6e 6669 6773  e of the configs
+000010e0: 2069 7320 4e6f 6e65 2c20 7768 6963 6820   is None, which 
+000010f0: 6973 206e 6f74 2061 6c6c 6f77 6564 6301  is not allowedc.
+00001100: 0000 0000 0000 0000 0000 000c 0000 000a  ................
+00001110: 0000 0013 0000 0073 3c02 0000 6900 6401  .......s<...i.d.
+00001120: 8801 6a00 6a01 9301 6402 8801 6a00 6a02  ..j.j...d...j.j.
+00001130: 9301 6403 8801 6a00 6a03 9301 6404 8802  ..d...j.j...d...
+00001140: 9301 6405 8805 a004 a100 9301 6406 7c00  ..d.........d.|.
+00001150: a005 6406 8801 6a00 6a06 8801 6a00 6a07  ..d...j.j...j.j.
+00001160: a103 9301 6407 7c00 a008 6407 8801 6a00  ....d.|...d...j.
+00001170: 6a09 8801 6a00 6a0a a103 9301 6408 7c00  j...j.j.....d.|.
+00001180: a008 6408 8801 6a00 6a0b 8801 6a00 6a0c  ..d...j.j...j.j.
+00001190: a103 9301 6409 7c00 a005 6409 8801 6a00  ....d.|...d...j.
+000011a0: 6a0d 8801 6a00 6a0e a103 9301 640a 7c00  j...j.j.....d.|.
+000011b0: a008 640a 8801 6a00 6a0f 8801 6a00 6a10  ..d...j.j...j.j.
+000011c0: a103 9301 640b 7c00 a008 640b 8801 6a00  ....d.|...d...j.
+000011d0: 6a11 8801 6a00 6a12 a103 9301 640c 7c00  j...j.j.....d.|.
+000011e0: a008 640c 8801 6a00 6a13 8801 6a00 6a14  ..d...j.j...j.j.
+000011f0: a103 9301 640d 7c00 a008 640d 8801 6a00  ....d.|...d...j.
+00001200: 6a15 8801 6a00 6a16 a103 9301 640e 7c00  j...j.j.....d.|.
+00001210: a005 640e 8801 6a00 6a17 8801 6a00 6a18  ..d...j.j...j.j.
+00001220: a103 9301 640f 8801 6a00 6a19 9301 6410  ....d...j.j...d.
+00001230: 7c00 a005 6410 8801 6a00 6a1a 8801 6a00  |...d...j.j...j.
+00001240: 6a1b a103 9301 6411 7c00 a005 6411 8801  j.....d.|...d...
+00001250: 6a00 6a1c 8801 6a00 6a1d a103 9301 7d01  j.j...j.j.....}.
+00001260: 7c00 a01e 6412 6413 6414 6702 a102 7d02  |...d.d.d.g...}.
+00001270: 7c02 72ba 8801 a01f 8805 a101 7d03 7420  |.r.........}.t 
+00001280: 6a21 8803 8805 7c03 6415 8d03 7d04 6e07  j!....|.d...}.n.
+00001290: 7420 6a21 8803 8805 6416 8d02 7d04 7422  t j!....d...}.t"
+000012a0: 6a23 a024 7c00 6417 a102 7d05 8801 6a25  j#.$|.d...}...j%
+000012b0: 6a26 6418 6b02 9001 7202 7c04 6419 6602  j&d.k...r.|.d.f.
+000012c0: 8800 641a 6602 6702 7d06 7420 6a27 7c01  ..d.f.g.}.t j'|.
+000012d0: 7c04 7c01 6410 1900 8801 6a25 6a28 7c06  |.|.d.....j%j(|.
+000012e0: 7c05 6701 8801 6a00 6a03 641b 8d07 7d07  |.g...j.j.d...}.
+000012f0: 7c07 a029 8800 a101 7d08 742a a02b 641c  |..)....}.t*.+d.
+00001300: 641d 8400 7c08 4400 8301 a101 7d09 742c  d...|.D.....}.t,
+00001310: 8804 7c09 8302 641e 1400 7d0a 7c0a 5300  ..|...d...}.|.S.
+00001320: 7420 6a2d 7c01 7c04 7c01 6410 1900 8801  t j-|.|.|.d.....
+00001330: 6a25 6a26 6413 8801 6a25 6a2e 7c05 6701  j%j&d...j%j.|.g.
+00001340: 8801 6a25 6a2f 641f 8d08 7d0b 7c0b 6420  ..j%j/d...}.|.d 
+00001350: 1900 a030 a100 5300 2921 4eda 096f 626a  ...0..S.)!N..obj
+00001360: 6563 7469 7665 da0b 6576 616c 5f6d 6574  ective..eval_met
+00001370: 7269 63da 0776 6572 626f 7365 da0b 7472  ric..verbose..tr
+00001380: 6565 5f6d 6574 686f 64da 096e 756d 5f63  ee_method..num_c
+00001390: 6c61 7373 da09 6d61 785f 6465 7074 68da  lass..max_depth.
+000013a0: 0561 6c70 6861 da06 6c61 6d62 6461 da0a  .alpha..lambda..
+000013b0: 6e75 6d5f 6c65 6176 6573 da09 7375 6273  num_leaves..subs
+000013c0: 616d 706c 65da 1063 6f6c 7361 6d70 6c65  ample..colsample
+000013d0: 5f62 7974 7265 65da 1163 6f6c 7361 6d70  _bytree..colsamp
+000013e0: 6c65 5f62 796c 6576 656c da10 636f 6c73  le_bylevel..cols
+000013f0: 616d 706c 655f 6279 6e6f 6465 da11 6d69  ample_bynode..mi
+00001400: 6e5f 6368 696c 645f 7361 6d70 6c65 73da  n_child_samples.
+00001410: 0365 7461 722e 0000 00da 116e 756d 5f70  .etar......num_p
+00001420: 6172 616c 6c65 6c5f 7472 6565 7239 0000  arallel_treer9..
+00001430: 0054 4672 2700 0000 722a 0000 007a 0d74  .TFr'...r*...z.t
+00001440: 6573 742d 6d6c 6f67 6c6f 7373 722d 0000  est-mloglossr-..
+00001450: 0072 2b00 0000 722c 0000 0029 0572 2f00  .r+...r,...).r/.
+00001460: 0000 7230 0000 0072 3100 0000 da09 6361  ..r0...r1.....ca
+00001470: 6c6c 6261 636b 73da 0c76 6572 626f 7365  llbacks..verbose
+00001480: 5f65 7661 6c63 0100 0000 0000 0000 0000  _evalc..........
+00001490: 0000 0200 0000 0500 0000 5300 0000 f316  ..........S.....
+000014a0: 0000 0067 007c 005d 077d 0174 00a0 017c  ...g.|.].}.t...|
+000014b0: 01a1 0191 0271 0253 0072 1800 0000 a902  .....q.S.r......
+000014c0: da02 6e70 da06 6172 676d 6178 a902 da02  ..np..argmax....
+000014d0: 2e30 da04 6c69 6e65 7218 0000 0072 1800  .0..liner....r..
+000014e0: 0000 7219 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
+000014f0: 6d70 3ee9 0000 00f3 0200 0000 1600 7a3c  mp>...........z<
+00001500: 5867 626f 6f73 744d 6f64 656c 2e61 7574  XgboostModel.aut
+00001510: 6f74 756e 652e 3c6c 6f63 616c 733e 2e6f  otune.<locals>.o
+00001520: 626a 6563 7469 7665 2e3c 6c6f 6361 6c73  bjective.<locals
+00001530: 3e2e 3c6c 6973 7463 6f6d 703e e9ff ffff  >.<listcomp>....
+00001540: ff29 0872 3d00 0000 da06 6474 7261 696e  .).r=.....dtrain
+00001550: 722f 0000 00da 056e 666f 6c64 da09 6173  r/.....nfold..as
+00001560: 5f70 616e 6461 73da 0473 6565 6472 5200  _pandas..seedrR.
+00001570: 0000 da07 7368 7566 666c 657a 1274 6573  ....shufflez.tes
+00001580: 742d 6d6c 6f67 6c6f 7373 2d6d 6561 6e29  t-mlogloss-mean)
+00001590: 3172 1400 0000 da0f 6d6f 6465 6c5f 6f62  1r......model_ob
+000015a0: 6a65 6374 6976 65da 116d 6f64 656c 5f65  jective..model_e
+000015b0: 7661 6c5f 6d65 7472 6963 da0f 6d6f 6465  val_metric..mode
+000015c0: 6c5f 7665 7262 6f73 6974 79da 076e 756e  l_verbosity..nun
+000015d0: 6971 7565 5a0b 7375 6767 6573 745f 696e  iqueZ.suggest_in
+000015e0: 74da 0d6d 6178 5f64 6570 7468 5f6d 696e  t..max_depth_min
+000015f0: da0d 6d61 785f 6465 7074 685f 6d61 785a  ..max_depth_maxZ
+00001600: 0d73 7567 6765 7374 5f66 6c6f 6174 da09  .suggest_float..
+00001610: 616c 7068 615f 6d69 6eda 0961 6c70 6861  alpha_min..alpha
+00001620: 5f6d 6178 da0a 6c61 6d62 6461 5f6d 696e  _max..lambda_min
+00001630: da0a 6c61 6d62 6461 5f6d 6178 da0e 6e75  ..lambda_max..nu
+00001640: 6d5f 6c65 6176 6573 5f6d 696e da0e 6e75  m_leaves_min..nu
+00001650: 6d5f 6c65 6176 6573 5f6d 6178 da0e 7375  m_leaves_max..su
+00001660: 625f 7361 6d70 6c65 5f6d 696e da0e 7375  b_sample_min..su
+00001670: 625f 7361 6d70 6c65 5f6d 6178 da16 636f  b_sample_max..co
+00001680: 6c5f 7361 6d70 6c65 5f62 795f 7472 6565  l_sample_by_tree
+00001690: 5f6d 696e da16 636f 6c5f 7361 6d70 6c65  _min..col_sample
+000016a0: 5f62 795f 7472 6565 5f6d 6178 da17 636f  _by_tree_max..co
+000016b0: 6c5f 7361 6d70 6c65 5f62 795f 6c65 7665  l_sample_by_leve
+000016c0: 6c5f 6d69 6eda 1763 6f6c 5f73 616d 706c  l_min..col_sampl
+000016d0: 655f 6279 5f6c 6576 656c 5f6d 6178 da16  e_by_level_max..
+000016e0: 636f 6c5f 7361 6d70 6c65 5f62 795f 6e6f  col_sample_by_no
+000016f0: 6465 5f6d 696e da16 636f 6c5f 7361 6d70  de_min..col_samp
+00001700: 6c65 5f62 795f 6e6f 6465 5f6d 6178 da15  le_by_node_max..
+00001710: 6d69 6e5f 6368 696c 645f 7361 6d70 6c65  min_child_sample
+00001720: 735f 6d69 6eda 156d 696e 5f63 6869 6c64  s_min..min_child
+00001730: 5f73 616d 706c 6573 5f6d 6178 7250 0000  _samples_maxrP..
+00001740: 00da 0973 7465 7073 5f6d 696e da09 7374  ...steps_min..st
+00001750: 6570 735f 6d61 78da 156e 756d 5f70 6172  eps_max..num_par
+00001760: 616c 6c65 6c5f 7472 6565 5f6d 696e da15  allel_tree_min..
+00001770: 6e75 6d5f 7061 7261 6c6c 656c 5f74 7265  num_parallel_tre
+00001780: 655f 6d61 785a 1373 7567 6765 7374 5f63  e_maxZ.suggest_c
+00001790: 6174 6567 6f72 6963 616c 7221 0000 0072  ategoricalr!...r
+000017a0: 3a00 0000 723b 0000 00da 066f 7074 756e  :...r;.....optun
+000017b0: 615a 0b69 6e74 6567 7261 7469 6f6e 5a16  aZ.integrationZ.
+000017c0: 5847 426f 6f73 7450 7275 6e69 6e67 4361  XGBoostPruningCa
+000017d0: 6c6c 6261 636b 7213 0000 0072 3c00 0000  llbackr....r<...
+000017e0: 722b 0000 0072 3000 0000 da07 7072 6564  r+...r0.....pred
+000017f0: 6963 7472 5600 0000 da07 6173 6172 7261  ictrV.....asarra
+00001800: 7972 0700 0000 da02 6376 da13 676c 6f62  yr......cv..glob
+00001810: 616c 5f72 616e 646f 6d5f 7374 6174 65da  al_random_state.
+00001820: 1773 6875 6666 6c65 5f64 7572 696e 675f  .shuffle_during_
+00001830: 7472 6169 6e69 6e67 da04 6d65 616e 290c  training..mean).
+00001840: da05 7472 6961 6cda 0570 6172 616d 7239  ..trial..paramr9
+00001850: 0000 0072 2000 0000 723e 0000 005a 1070  ...r ...r>...Z.p
+00001860: 7275 6e69 6e67 5f63 616c 6c62 6163 6b72  runing_callbackr
+00001870: 4000 0000 7216 0000 00da 0570 7265 6473  @...r......preds
+00001880: da0b 7072 6564 5f6c 6162 656c 735a 076d  ..pred_labelsZ.m
+00001890: 6174 7468 6577 da06 7265 7375 6c74 a906  atthew..result..
+000018a0: 723f 0000 0072 1700 0000 5a08 7472 6169  r?...r....Z.trai
+000018b0: 6e5f 6f6e 7223 0000 0072 2600 0000 7225  n_onr#...r&...r%
+000018c0: 0000 0072 1800 0000 7219 0000 0072 4200  ...r....r....rB.
+000018d0: 0000 9800 0000 73d6 0000 0002 0108 0102  ......s.........
+000018e0: ff08 0202 fe08 0302 fd04 0402 fc08 0502  ................
+000018f0: fb06 0602 0106 0106 0102 fd02 fa06 0b0e  ................
+00001900: 0102 ff02 f506 0e0e 0102 ff02 f206 1102  ................
+00001910: 0106 0106 0102 fd02 ef06 1602 0106 0106  ................
+00001920: 0102 fd02 ea06 1b02 0106 0106 0102 fd02  ................
+00001930: e506 2002 0106 0106 0102 fd02 e006 2502  .. ...........%.
+00001940: 0106 0106 0102 fd02 db06 2a02 0106 0106  ..........*.....
+00001950: 0102 fd02 d608 2f02 d106 300e 0102 ff02  ....../...0.....
+00001960: d006 3302 0106 0106 0102 fd04 cd10 3904  ..3...........9.
+00001970: 010a 0112 010e 0206 0204 0104 ff0e 0410  ................
+00001980: 0104 0102 0102 0106 0106 0102 0104 0106  ................
+00001990: 0106 f90a 0914 010e 0104 0104 0202 0102  ................
+000019a0: 0106 0106 0202 0106 0104 0106 0106 f70c  ................
+000019b0: 0c7a 2858 6762 6f6f 7374 4d6f 6465 6c2e  .z(XgboostModel.
+000019c0: 6175 746f 7475 6e65 2e3c 6c6f 6361 6c73  autotune.<locals
+000019d0: 3e2e 6f62 6a65 6374 6976 65da 0778 6762  >.objective..xgb
+000019e0: 6f6f 7374 5429 025a 0c6d 756c 7469 7661  oostT).Z.multiva
+000019f0: 7269 6174 6572 6100 0000 da08 6d69 6e69  riatera.....mini
+00001a00: 6d69 7a65 7a07 2074 756e 696e 6729 03da  mizez. tuning)..
+00001a10: 0964 6972 6563 7469 6f6e da07 7361 6d70  .direction..samp
+00001a20: 6c65 725a 0a73 7475 6479 5f6e 616d 6529  lerZ.study_name)
+00001a30: 04da 086e 5f74 7269 616c 73da 0774 696d  ...n_trials..tim
+00001a40: 656f 7574 5a0e 6763 5f61 6674 6572 5f74  eoutZ.gc_after_t
+00001a50: 7269 616c 5a11 7368 6f77 5f70 726f 6772  rialZ.show_progr
+00001a60: 6573 735f 6261 7272 4200 0000 7243 0000  ess_barrB...rC..
+00001a70: 0072 4400 0000 7245 0000 0072 4600 0000  .rD...rE...rF...
+00001a80: 7247 0000 0072 4800 0000 7249 0000 0072  rG...rH...rI...r
+00001a90: 4a00 0000 724b 0000 0072 4c00 0000 724d  J...rK...rL...rM
+00001aa0: 0000 0072 4e00 0000 724f 0000 0072 5000  ...rN...rO...rP.
+00001ab0: 0000 722e 0000 0072 5100 0000 7a0d 4265  ..r....rQ...z.Be
+00001ac0: 7374 2070 6172 616d 733a 2072 3900 0000  st params: r9...
+00001ad0: 4e29 2272 0d00 0000 7202 0000 0072 1e00  N)"r....r....r..
+00001ae0: 0000 723a 0000 0072 3b00 0000 720c 0000  ..r:...r;...r...
+00001af0: 0072 2200 0000 7215 0000 0072 1300 0000  .r"...r....r....
+00001b00: 7214 0000 0072 3200 0000 727d 0000 005a  r....r2...r}...Z
+00001b10: 0873 616d 706c 6572 735a 0a54 5045 5361  .samplersZ.TPESa
+00001b20: 6d70 6c65 7272 8100 0000 5a0c 6372 6561  mplerr....Z.crea
+00001b30: 7465 5f73 7475 6479 da08 6f70 7469 6d69  te_study..optimi
+00001b40: 7a65 da1c 6879 7065 7270 6172 616d 6574  ze..hyperparamet
+00001b50: 6572 5f74 756e 696e 675f 726f 756e 6473  er_tuning_rounds
+00001b60: da26 6879 7065 7270 6172 616d 6574 6572  .&hyperparameter
+00001b70: 5f74 756e 696e 675f 6d61 785f 7275 6e74  _tuning_max_runt
+00001b80: 696d 655f 7365 6373 5a0d 7669 7375 616c  ime_secsZ.visual
+00001b90: 697a 6174 696f 6e5a 1970 6c6f 745f 6f70  izationZ.plot_op
+00001ba0: 7469 6d69 7a61 7469 6f6e 5f68 6973 746f  timization_histo
+00001bb0: 7279 da04 7368 6f77 5a16 706c 6f74 5f70  ry..showZ.plot_p
+00001bc0: 6172 616d 5f69 6d70 6f72 7461 6e63 6573  aram_importances
+00001bd0: da11 5a65 726f 4469 7669 7369 6f6e 4572  ..ZeroDivisionEr
+00001be0: 726f 72da 0c52 756e 7469 6d65 4572 726f  ror..RuntimeErro
+00001bf0: 725a 0a62 6573 745f 7472 6961 6c72 3d00  rZ.best_trialr=.
+00001c00: 0000 7263 0000 0072 6400 0000 7265 0000  ..rc...rd...re..
+00001c10: 0072 6600 0000 7250 0000 0072 3500 0000  .rf...rP...r5...
+00001c20: 7239 0000 0029 0b72 1700 0000 7223 0000  r9...).r....r#..
+00001c30: 0072 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
+00001c40: 7242 0000 00da 0961 6c67 6f72 6974 686d  rB.....algorithm
+00001c50: 728d 0000 005a 0573 7475 6479 da03 6669  r....Z.study..fi
+00001c60: 675a 1278 6762 6f6f 7374 5f62 6573 745f  gZ.xgboost_best_
+00001c70: 7061 7261 6d72 1800 0000 7289 0000 0072  paramr....r....r
+00001c80: 1900 0000 7234 0000 007e 0000 0073 9c00  ....r4...~...s..
+00001c90: 0000 120b 0e01 0601 0802 0403 02ff 0402  ................
+00001ca0: 02fe 0403 02fd 0205 0201 04ff 1604 0463  ...............c
+00001cb0: 0601 0801 06ff 0403 0201 0201 0801 06fd  ................
+00001cc0: 0406 0201 0601 0601 0201 0201 06fb 0207  ................
+00001cd0: 0c01 0801 0c01 0c01 1201 0401 02ff 0803  ................
+00001ce0: 0201 0801 02ff 0802 02fe 0803 02fd 0404  ................
+00001cf0: 02fc 0805 02fb 0406 0201 02ff 02fa 0809  ................
+00001d00: 02f7 080a 02f6 080b 02f5 080c 02f4 080d  ................
+00001d10: 02f3 080e 02f2 080f 02f1 0810 02f0 0811  ................
+00001d20: 02ef 0812 02ee 0813 08ed 0e15 1001 7a15  ..............z.
+00001d30: 5867 626f 6f73 744d 6f64 656c 2e61 7574  XgboostModel.aut
+00001d40: 6f74 756e 65da 0264 6663 0200 0000 0000  otune..dfc......
+00001d50: 0000 0000 0000 0600 0000 0400 0000 4300  ..............C.
+00001d60: 0000 73a0 0000 0074 0074 01a0 02a1 009b  ..s....t.t......
+00001d70: 0064 019d 0283 0101 0074 0364 0283 0101  .d.......t.d....
+00001d80: 0074 04a0 057c 01a1 017d 027c 006a 0673  .t...|...}.|.j.s
+00001d90: 1974 0764 0383 0182 017c 006a 0873 2074  .t.d.....|.j.s t
+00001da0: 0764 0483 0182 017c 006a 06a0 097c 02a1  .d.....|.j...|..
+00001db0: 017d 037c 006a 0a64 056b 0272 3c74 0ba0  .}.|.j.d.k.r<t..
+00001dc0: 0c64 0664 0784 007c 0344 0083 01a1 017d  .d.d...|.D.....}
+00001dd0: 047c 047c 006a 086a 0d6b 047d 056e 0c7c  .|.|.j.j.k.}.n.|
+00001de0: 037d 0474 0ba0 0c64 0864 0784 007c 0344  .}.t...d.d...|.D
+00001df0: 0083 01a1 017d 0574 0364 0983 0101 007c  .....}.t.d.....|
+00001e00: 047c 0566 0253 0029 0a7a 1750 7265 6469  .|.f.S.).z.Predi
+00001e10: 6374 206f 6e20 756e 7365 656e 2064 6174  ct on unseen dat
+00001e20: 612e 7a33 3a20 5374 6172 7420 7072 6564  a.z3: Start pred
+00001e30: 6963 7469 6e67 206f 6e20 6e65 7720 6461  icting on new da
+00001e40: 7461 2075 7369 6e67 2058 6762 6f6f 7374  ta using Xgboost
+00001e50: 206d 6f64 656c 2e7a 1c2b 2b2b 2b2b 2b2b   model.z.+++++++
+00001e60: 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  ++++++++++++++++
+00001e70: 2b2b 2b2b 2b7a 204e 6f20 7472 6169 6e65  +++++z No traine
+00001e80: 6420 6d6f 6465 6c20 6861 7320 6265 656e  d model has been
+00001e90: 2066 6f75 6e64 2e7a 2b4e 6f20 6d6f 6465   found.z+No mode
+00001ea0: 6c20 636f 6e66 6967 7572 6174 696f 6e20  l configuration 
+00001eb0: 6669 6c65 2068 6173 2062 6565 6e20 666f  file has been fo
+00001ec0: 756e 642e 7211 0000 0063 0100 0000 0000  und.r....c......
+00001ed0: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
+00001ee0: 0000 7314 0000 0067 007c 005d 067d 017c  ..s....g.|.].}.|
+00001ef0: 0164 0019 0091 0271 0253 0029 0172 2d00  .d.....q.S.).r-.
+00001f00: 0000 7218 0000 0072 5800 0000 7218 0000  ..r....rX...r...
+00001f10: 0072 1800 0000 7219 0000 0072 5b00 0000  .r....r....r[...
+00001f20: 3c01 0000 7302 0000 0014 007a 2858 6762  <...s......z(Xgb
+00001f30: 6f6f 7374 4d6f 6465 6c2e 7072 6564 6963  oostModel.predic
+00001f40: 742e 3c6c 6f63 616c 733e 2e3c 6c69 7374  t.<locals>.<list
+00001f50: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
+00001f60: 0000 0200 0000 0500 0000 5300 0000 7254  ..........S...rT
+00001f70: 0000 0072 1800 0000 7255 0000 0072 5800  ...r....rU...rX.
+00001f80: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00001f90: 0072 5b00 0000 4201 0000 725c 0000 007a  .r[...B...r\...z
+00001fa0: 1346 696e 6973 6865 6420 7072 6564 6963  .Finished predic
+00001fb0: 7469 6e67 290e 720d 0000 0072 0200 0000  ting).r....r....
+00001fc0: 721e 0000 0072 3500 0000 723a 0000 0072  r....r5...r:...r
+00001fd0: 3b00 0000 7216 0000 00da 0945 7863 6570  ;...r......Excep
+00001fe0: 7469 6f6e 7215 0000 0072 7e00 0000 7210  tionr....r~...r.
+00001ff0: 0000 0072 5600 0000 727f 0000 00da 1863  ...rV...r......c
+00002000: 6c61 7373 6966 6963 6174 696f 6e5f 7468  lassification_th
+00002010: 7265 7368 6f6c 6429 0672 1700 0000 7298  reshold).r....r.
+00002020: 0000 0072 3f00 0000 5a0d 7061 7274 6961  ...r?...Z.partia
+00002030: 6c5f 7072 6f62 735a 0f70 7265 6469 6374  l_probsZ.predict
+00002040: 6564 5f70 726f 6273 da11 7072 6564 6963  ed_probs..predic
+00002050: 7465 645f 636c 6173 7365 7372 1800 0000  ted_classesr....
+00002060: 7218 0000 0072 1900 0000 727e 0000 002d  r....r....r~...-
+00002070: 0100 0073 2400 0000 0202 0c01 04ff 0803  ...s$...........
+00002080: 0a01 0601 0801 0602 0801 0c02 0a01 1401  ................
+00002090: 0a02 04ff 0404 1401 0801 0801 7a14 5867  ............z.Xg
+000020a0: 626f 6f73 744d 6f64 656c 2e70 7265 6469  boostModel.predi
+000020b0: 6374 2903 4e4e 4e29 1ada 085f 5f6e 616d  ct).NNN)...__nam
+000020c0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+000020d0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+000020e0: 5f64 6f63 5f5f 7204 0000 0072 0500 0000  _doc__r....r....
+000020f0: 7209 0000 0072 0b00 0000 720a 0000 0072  r....r....r....r
+00002100: 1a00 0000 7237 0000 00da 0653 6572 6965  ....r7.....Serie
+00002110: 7372 0300 0000 da03 7374 72da 0566 6c6f  sr......str..flo
+00002120: 6174 7221 0000 0072 2200 0000 da09 4461  atr!...r".....Da
+00002130: 7461 4672 616d 6572 3a00 0000 da07 426f  taFramer:.....Bo
+00002140: 6f73 7465 7272 4100 0000 7234 0000 0072  osterrA...r4...r
+00002150: 0600 0000 7256 0000 00da 076e 6461 7272  ....rV.....ndarr
+00002160: 6179 727e 0000 0072 1800 0000 7218 0000  ayr~...r....r...
+00002170: 0072 1800 0000 7219 0000 0072 0f00 0000  .r....r....r....
+00002180: 1a00 0000 7350 0000 0008 0004 0102 0502  ....sP..........
+00002190: 0102 0104 fb06 0202 fe06 0302 fd06 0402  ................
+000021a0: fc06 050a fb1c 0d08 0802 1504 0202 fe04  ................
+000021b0: 0302 fd04 0402 fc04 0502 fb04 060a fa02  ................
+000021c0: 3704 0202 fe04 0302 fd04 0402 fc04 0502  7...............
+000021d0: fb02 060a fa00 7f24 3072 0f00 0000 291c  .......$0r....).
+000021e0: 729f 0000 0072 0200 0000 da06 7479 7069  r....r......typi
+000021f0: 6e67 7203 0000 0072 0400 0000 7205 0000  ngr....r....r...
+00002200: 0072 0600 0000 da05 6e75 6d70 7972 5600  .r......numpyrV.
+00002210: 0000 727d 0000 00da 0670 616e 6461 7372  ..r}.....pandasr
+00002220: 3700 0000 728a 0000 0072 3a00 0000 da0f  7...r....r:.....
+00002230: 736b 6c65 6172 6e2e 6d65 7472 6963 7372  sklearn.metricsr
+00002240: 0700 0000 da0d 736b 6c65 6172 6e2e 7574  ......sklearn.ut
+00002250: 696c 7372 0800 0000 da1f 626c 7565 6361  ilsr......blueca
+00002260: 7374 2e63 6f6e 6669 672e 7472 6169 6e69  st.config.traini
+00002270: 6e67 5f63 6f6e 6669 6772 0900 0000 720a  ng_configr....r.
+00002280: 0000 0072 0b00 0000 da24 626c 7565 6361  ...r.....$blueca
+00002290: 7374 2e67 656e 6572 616c 5f75 7469 6c73  st.general_utils
+000022a0: 2e67 656e 6572 616c 5f75 7469 6c73 720c  .general_utilsr.
+000022b0: 0000 0072 0d00 0000 da22 626c 7565 6361  ...r....."blueca
+000022c0: 7374 2e6d 6c5f 6d6f 6465 6c6c 696e 672e  st.ml_modelling.
+000022d0: 6261 7365 5f63 6c61 7373 6573 720e 0000  base_classesr...
+000022e0: 0072 0f00 0000 7218 0000 0072 1800 0000  .r....r....r....
+000022f0: 7218 0000 0072 1900 0000 da08 3c6d 6f64  r....r......<mod
+00002300: 756c 653e 0100 0000 731a 0000 0004 000c  ule>....s.......
+00002310: 0618 0108 0208 0108 0108 010c 010c 0114  ................
+00002320: 0210 050c 0114 03                        .......
```

### Comparing `bluecast-0.3.1/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc` & `bluecast-0.4/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/ml_modelling/base_classes.py` & `bluecast-0.4/bluecast/ml_modelling/base_classes.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/ml_modelling/xgboost.py` & `bluecast-0.4/bluecast/ml_modelling/xgboost.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 13:00:52 2023 UTC, .py size: 965 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,111 @@
-00000000: 6f0d 0d0a 0000 0000 8497 9564 c503 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 4a9a 9564 4a05 0000  o.......J..dJ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 8302 5a07 6402 5300 2907 e900  ..d...Z.d.S.)...
 00000070: 0000 0029 01da 0864 6174 6574 696d 654e  ...)...datetimeN
 00000080: 2901 da16 4665 6174 7572 6553 656c 6563  )...FeatureSelec
 00000090: 7469 6f6e 436f 6e66 6967 2901 da06 6c6f  tionConfig)...lo
 000000a0: 6767 6572 6300 0000 0000 0000 0000 0000  ggerc...........
-000000b0: 0000 0000 0006 0000 0040 0000 0073 4e00  .........@...sN.
-000000c0: 0000 6500 5a01 6400 5a02 6401 6503 6a04  ..e.Z.d.Z.d.e.j.
-000000d0: 6602 6402 6403 8404 5a05 6404 6506 6a07  f.d.d...Z.d.e.j.
-000000e0: 6405 6506 6a08 6406 6506 6a07 6606 6407  d.e.j.d.e.j.f.d.
-000000f0: 6408 8404 5a09 6404 6506 6a07 6406 6506  d...Z.d.e.j.d.e.
-00000100: 6a07 6604 6409 640a 8404 5a0a 640b 5300  j.f.d.d...Z.d.S.
-00000110: 290c da0f 4665 6174 7572 6553 656c 6563  )...FeatureSelec
-00000120: 746f 72da 1273 656c 6563 7469 6f6e 5f73  tor..selection_s
-00000130: 7472 6174 6567 7963 0200 0000 0000 0000  trategyc........
-00000140: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00000150: 7310 0000 0064 007c 005f 007c 017c 005f  s....d.|._.|.|._
-00000160: 0164 0053 00a9 014e 2902 da11 7365 6c65  .d.S...N)...sele
-00000170: 6374 6564 5f66 6561 7475 7265 7372 0600  cted_featuresr..
-00000180: 0000 2902 da04 7365 6c66 7206 0000 00a9  ..)...selfr.....
-00000190: 0072 0a00 0000 fa4e 2f68 6f6d 652f 7468  .r.....N/home/th
-000001a0: 6f6d 6173 2f49 6465 6150 726f 6a65 6374  omas/IdeaProject
-000001b0: 732f 426c 7565 4361 7374 2f62 6c75 6563  s/BlueCast/bluec
-000001c0: 6173 742f 7072 6570 726f 6365 7373 696e  ast/preprocessin
-000001d0: 672f 6665 6174 7572 655f 7365 6c65 6374  g/feature_select
-000001e0: 696f 6e2e 7079 da08 5f5f 696e 6974 5f5f  ion.py..__init__
-000001f0: 0a00 0000 7304 0000 0006 010a 017a 1846  ....s........z.F
-00000200: 6561 7475 7265 5365 6c65 6374 6f72 2e5f  eatureSelector._
-00000210: 5f69 6e69 745f 5fda 0264 66da 0674 6172  _init__..df..tar
-00000220: 6765 74da 0672 6574 7572 6e63 0300 0000  get..returnc....
-00000230: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-00000240: 4300 0000 735c 0000 0074 0074 01a0 02a1  C...s\...t.t....
-00000250: 009b 0064 019d 0283 0101 007c 006a 03a0  ...d.......|.j..
-00000260: 047c 017c 02a1 0201 007c 006a 036a 057c  .|.|.....|.j.j.|
-00000270: 005f 067c 016a 0764 0064 0085 027c 006a  ._.|.j.d.d...|.j
-00000280: 0666 0219 007d 0174 0074 01a0 02a1 009b  .f...}.t.t......
-00000290: 0064 027c 016a 089b 0064 039d 0483 0101  .d.|.j...d......
-000002a0: 007c 0153 0029 044e 7a3f 3a20 5374 6172  .|.S.).Nz?: Star
-000002b0: 7420 6665 6174 7572 6520 7365 6c65 6374  t feature select
-000002c0: 696f 6e20 6173 2064 6566 696e 6564 2069  ion as defined i
-000002d0: 6e20 4665 6174 7572 6553 656c 6563 7469  n FeatureSelecti
-000002e0: 6f6e 436f 6e66 6967 2e7a 183a 2053 656c  onConfig.z.: Sel
-000002f0: 6563 7465 6420 6665 6174 7572 6573 2061  ected features a
-00000300: 7265 20da 012e 2909 7204 0000 0072 0200  re ...).r....r..
-00000310: 0000 da06 7574 636e 6f77 7206 0000 00da  ....utcnowr.....
-00000320: 0366 6974 da08 7375 7070 6f72 745f 7208  .fit..support_r.
-00000330: 0000 00da 036c 6f63 da07 636f 6c75 6d6e  .....loc..column
-00000340: 7329 0372 0900 0000 720d 0000 0072 0e00  s).r....r....r..
-00000350: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00000360: 00da 0d66 6974 5f74 7261 6e73 666f 726d  ...fit_transform
-00000370: 0e00 0000 7310 0000 0002 010c 0104 ff0e  ....s...........
-00000380: 030a 0114 011a 0104 017a 1d46 6561 7475  .........z.Featu
-00000390: 7265 5365 6c65 6374 6f72 2e66 6974 5f74  reSelector.fit_t
-000003a0: 7261 6e73 666f 726d 6302 0000 0000 0000  ransformc.......
-000003b0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-000003c0: 0073 1800 0000 7c01 6a00 6400 6400 8502  .s....|.j.d.d...
-000003d0: 7c00 6a01 6602 1900 7d01 7c01 5300 7207  |.j.f...}.|.S.r.
-000003e0: 0000 0029 0272 1400 0000 7208 0000 0029  ...).r....r....)
-000003f0: 0272 0900 0000 720d 0000 0072 0a00 0000  .r....r....r....
-00000400: 720a 0000 0072 0b00 0000 da09 7472 616e  r....r......tran
-00000410: 7366 6f72 6d18 0000 0073 0400 0000 1401  sform....s......
-00000420: 0401 7a19 4665 6174 7572 6553 656c 6563  ..z.FeatureSelec
-00000430: 746f 722e 7472 616e 7366 6f72 6d4e 290b  tor.transformN).
-00000440: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000450: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000460: 6d65 5f5f 7203 0000 0072 0600 0000 720c  me__r....r....r.
-00000470: 0000 00da 0270 64da 0944 6174 6146 7261  .....pd..DataFra
-00000480: 6d65 da06 5365 7269 6573 7216 0000 0072  me..Seriesr....r
-00000490: 1700 0000 720a 0000 0072 0a00 0000 720a  ....r....r....r.
-000004a0: 0000 0072 0b00 0000 7205 0000 0009 0000  ...r....r.......
-000004b0: 0073 0800 0000 0800 1001 1c04 1a0a 7205  .s............r.
-000004c0: 0000 0029 0872 0200 0000 da06 7061 6e64  ...).r......pand
-000004d0: 6173 721b 0000 00da 1f62 6c75 6563 6173  asr......bluecas
-000004e0: 742e 636f 6e66 6967 2e74 7261 696e 696e  t.config.trainin
-000004f0: 675f 636f 6e66 6967 7203 0000 00da 2462  g_configr.....$b
-00000500: 6c75 6563 6173 742e 6765 6e65 7261 6c5f  luecast.general_
-00000510: 7574 696c 732e 6765 6e65 7261 6c5f 7574  utils.general_ut
-00000520: 696c 7372 0400 0000 7205 0000 0072 0a00  ilsr....r....r..
-00000530: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00000540: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000550: 0a00 0000 0c00 0802 0c02 0c01 1203       ..............
+000000b0: 0000 0000 0006 0000 0040 0000 0073 5200  .........@...sR.
+000000c0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+000000d0: 6504 6a05 6602 6403 6404 8404 5a06 6405  e.j.f.d.d...Z.d.
+000000e0: 6507 6a08 6406 6507 6a09 6407 6507 6a08  e.j.d.e.j.d.e.j.
+000000f0: 6606 6408 6409 8404 5a0a 6405 6507 6a08  f.d.d...Z.d.e.j.
+00000100: 6407 6507 6a08 6604 640a 640b 8404 5a0b  d.e.j.f.d.d...Z.
+00000110: 640c 5300 290d da0f 4665 6174 7572 6553  d.S.)...FeatureS
+00000120: 656c 6563 746f 7261 7901 0000 5365 6c65  electoray...Sele
+00000130: 6374 2074 6f70 2066 6561 7475 7265 7320  ct top features 
+00000140: 6261 7365 6420 6f6e 2073 656c 6563 7469  based on selecti
+00000150: 6f6e 5f73 7472 6174 6567 7920 6465 6669  on_strategy defi
+00000160: 6e65 6420 696e 2046 6561 7475 7265 5365  ned in FeatureSe
+00000170: 6c65 6374 696f 6e43 6f6e 6669 672e 0a0a  lectionConfig...
+00000180: 2020 2020 4f6e 2064 6566 6175 6c74 2063      On default c
+00000190: 726f 7373 2d76 616c 6964 6174 6564 2072  ross-validated r
+000001a0: 6563 7572 7369 7665 2066 6561 7475 7265  ecursive feature
+000001b0: 2065 6c69 6d69 6e61 7469 6f6e 2069 7320   elimination is 
+000001c0: 7573 6564 2e20 496e 2074 6865 2063 6f6e  used. In the con
+000001d0: 6669 6720 6669 6c65 2061 2064 6966 6665  fig file a diffe
+000001e0: 7265 6e74 0a20 2020 2052 4645 4356 2069  rent.    RFECV i
+000001f0: 6e73 7461 6e63 6520 6361 6e20 6265 2064  nstance can be d
+00000200: 6566 696e 6564 2028 7573 696e 6720 6120  efined (using a 
+00000210: 2064 6966 6665 7265 6e74 2063 6c61 7373   different class
+00000220: 6966 6965 722c 2073 636f 7269 6e67 2066  ifier, scoring f
+00000230: 756e 6374 696f 6e2c 2072 616e 646f 6d20  unction, random 
+00000240: 7365 6564 2065 7463 2e29 2e0a 2020 2020  seed etc.)..    
+00000250: 3a70 6172 616d 2073 656c 6563 7469 6f6e  :param selection
+00000260: 5f73 7472 6174 6567 793a 2049 6e73 7461  _strategy: Insta
+00000270: 6e63 6520 6f66 2046 6561 7475 7265 5365  nce of FeatureSe
+00000280: 6c65 6374 696f 6e43 6f6e 6669 672e 7365  lectionConfig.se
+00000290: 6c65 6374 696f 6e5f 7374 7261 7465 6779  lection_strategy
+000002a0: 0a20 2020 20da 1273 656c 6563 7469 6f6e  .    ..selection
+000002b0: 5f73 7472 6174 6567 7963 0200 0000 0000  _strategyc......
+000002c0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+000002d0: 0000 7310 0000 0064 007c 005f 007c 017c  ..s....d.|._.|.|
+000002e0: 005f 0164 0053 00a9 014e 2902 da11 7365  ._.d.S...N)...se
+000002f0: 6c65 6374 6564 5f66 6561 7475 7265 7372  lected_featuresr
+00000300: 0600 0000 2902 da04 7365 6c66 7206 0000  ....)...selfr...
+00000310: 00a9 0072 0a00 0000 fa4e 2f68 6f6d 652f  ...r.....N/home/
+00000320: 7468 6f6d 6173 2f49 6465 6150 726f 6a65  thomas/IdeaProje
+00000330: 6374 732f 426c 7565 4361 7374 2f62 6c75  cts/BlueCast/blu
+00000340: 6563 6173 742f 7072 6570 726f 6365 7373  ecast/preprocess
+00000350: 696e 672f 6665 6174 7572 655f 7365 6c65  ing/feature_sele
+00000360: 6374 696f 6e2e 7079 da08 5f5f 696e 6974  ction.py..__init
+00000370: 5f5f 1100 0000 7304 0000 0006 010a 017a  __....s........z
+00000380: 1846 6561 7475 7265 5365 6c65 6374 6f72  .FeatureSelector
+00000390: 2e5f 5f69 6e69 745f 5fda 0264 66da 0674  .__init__..df..t
+000003a0: 6172 6765 74da 0672 6574 7572 6e63 0300  arget..returnc..
+000003b0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+000003c0: 0000 4300 0000 735c 0000 0074 0074 01a0  ..C...s\...t.t..
+000003d0: 02a1 009b 0064 019d 0283 0101 007c 006a  .....d.......|.j
+000003e0: 03a0 047c 017c 02a1 0201 007c 006a 036a  ...|.|.....|.j.j
+000003f0: 057c 005f 067c 016a 0764 0064 0085 027c  .|._.|.j.d.d...|
+00000400: 006a 0666 0219 007d 0174 0074 01a0 02a1  .j.f...}.t.t....
+00000410: 009b 0064 027c 016a 089b 0064 039d 0483  ...d.|.j...d....
+00000420: 0101 007c 0153 0029 044e 7a3f 3a20 5374  ...|.S.).Nz?: St
+00000430: 6172 7420 6665 6174 7572 6520 7365 6c65  art feature sele
+00000440: 6374 696f 6e20 6173 2064 6566 696e 6564  ction as defined
+00000450: 2069 6e20 4665 6174 7572 6553 656c 6563   in FeatureSelec
+00000460: 7469 6f6e 436f 6e66 6967 2e7a 183a 2053  tionConfig.z.: S
+00000470: 656c 6563 7465 6420 6665 6174 7572 6573  elected features
+00000480: 2061 7265 20da 012e 2909 7204 0000 0072   are ...).r....r
+00000490: 0200 0000 da06 7574 636e 6f77 7206 0000  ......utcnowr...
+000004a0: 00da 0366 6974 da08 7375 7070 6f72 745f  ...fit..support_
+000004b0: 7208 0000 00da 036c 6f63 da07 636f 6c75  r......loc..colu
+000004c0: 6d6e 7329 0372 0900 0000 720d 0000 0072  mns).r....r....r
+000004d0: 0e00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+000004e0: 0000 00da 0d66 6974 5f74 7261 6e73 666f  .....fit_transfo
+000004f0: 726d 1500 0000 7310 0000 0002 010c 0104  rm....s.........
+00000500: ff0e 030a 0114 011a 0104 017a 1d46 6561  ...........z.Fea
+00000510: 7475 7265 5365 6c65 6374 6f72 2e66 6974  tureSelector.fit
+00000520: 5f74 7261 6e73 666f 726d 6302 0000 0000  _transformc.....
+00000530: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00000540: 0000 0073 1800 0000 7c01 6a00 6400 6400  ...s....|.j.d.d.
+00000550: 8502 7c00 6a01 6602 1900 7d01 7c01 5300  ..|.j.f...}.|.S.
+00000560: 7207 0000 0029 0272 1400 0000 7208 0000  r....).r....r...
+00000570: 0029 0272 0900 0000 720d 0000 0072 0a00  .).r....r....r..
+00000580: 0000 720a 0000 0072 0b00 0000 da09 7472  ..r....r......tr
+00000590: 616e 7366 6f72 6d1f 0000 0073 0400 0000  ansform....s....
+000005a0: 1401 0401 7a19 4665 6174 7572 6553 656c  ....z.FeatureSel
+000005b0: 6563 746f 722e 7472 616e 7366 6f72 6d4e  ector.transformN
+000005c0: 290c da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000005d0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000005e0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
+000005f0: 0300 0000 7206 0000 0072 0c00 0000 da02  ....r....r......
+00000600: 7064 da09 4461 7461 4672 616d 65da 0653  pd..DataFrame..S
+00000610: 6572 6965 7372 1600 0000 7217 0000 0072  eriesr....r....r
+00000620: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+00000630: 0000 0072 0500 0000 0900 0000 730a 0000  ...r........s...
+00000640: 0008 0004 0110 071c 041a 0a72 0500 0000  ...........r....
+00000650: 2908 7202 0000 00da 0670 616e 6461 7372  ).r......pandasr
+00000660: 1c00 0000 da1f 626c 7565 6361 7374 2e63  ......bluecast.c
+00000670: 6f6e 6669 672e 7472 6169 6e69 6e67 5f63  onfig.training_c
+00000680: 6f6e 6669 6772 0300 0000 da24 626c 7565  onfigr.....$blue
+00000690: 6361 7374 2e67 656e 6572 616c 5f75 7469  cast.general_uti
+000006a0: 6c73 2e67 656e 6572 616c 5f75 7469 6c73  ls.general_utils
+000006b0: 7204 0000 0072 0500 0000 720a 0000 0072  r....r....r....r
+000006c0: 0a00 0000 720a 0000 0072 0b00 0000 da08  ....r....r......
+000006d0: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
+000006e0: 000c 0008 020c 020c 0112 03              ...........
```

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc` & `bluecast-0.4/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/custom.py` & `bluecast-0.4/bluecast/preprocessing/custom.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/datetime_features.py` & `bluecast-0.4/bluecast/preprocessing/datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/encode_target_labels.py` & `bluecast-0.4/bluecast/preprocessing/encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/feature_selection.py` & `bluecast-0.4/bluecast/preprocessing/feature_selection.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/feature_types.py` & `bluecast-0.4/bluecast/preprocessing/feature_types.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/nulls_and_infs.py` & `bluecast-0.4/bluecast/preprocessing/nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/schema_checks.py` & `bluecast-0.4/bluecast/preprocessing/schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/target_encoding.py` & `bluecast-0.4/bluecast/preprocessing/target_encoding.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/preprocessing/train_test_split.py` & `bluecast-0.4/bluecast/preprocessing/train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 12:58:15 2023 UTC, .py size: 5855 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-00000000: 6f0d 0d0a 0000 0000 e796 9564 df16 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 b211 9764 7f16 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0e01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a0a  Z.m.Z...d.d.l.Z.
 00000060: 6400 6401 6c0b 5a0c 6400 6401 6c0d 5a0d  d.d.l.Z.d.d.l.Z.
-00000070: 6400 6401 6c0e 5a0f 6400 6403 6c10 6d11  d.d.l.Z.d.d.l.m.
-00000080: 5a11 0100 6400 6404 6c12 6d13 5a13 0100  Z...d.d.l.m.Z...
-00000090: 6400 6405 6c14 6d15 5a15 6d16 5a16 0100  d.d.l.m.Z.m.Z...
-000000a0: 6400 6406 6c17 6d18 5a18 0100 6400 6407  d.d.l.m.Z...d.d.
+00000070: 6400 6403 6c0e 6d0f 5a0f 0100 6400 6404  d.d.l.m.Z...d.d.
+00000080: 6c10 6d11 5a11 0100 6400 6405 6c12 6d13  l.m.Z...d.d.l.m.
+00000090: 5a13 6d14 5a14 0100 6400 6406 6c15 6d16  Z.m.Z...d.d.l.m.
+000000a0: 5a16 0100 6400 6401 6c17 5a18 6400 6407  Z...d.d.l.Z.d.d.
 000000b0: 6c19 6d1a 5a1a 0100 6400 6408 6c1b 6d1c  l.m.Z...d.d.l.m.
 000000c0: 5a1c 6d1d 5a1d 6d1e 5a1e 0100 6400 6409  Z.m.Z.m.Z...d.d.
 000000d0: 6c1f 6d20 5a20 6d21 5a21 6d22 5a22 0100  l.m Z m!Z!m"Z"..
 000000e0: 6400 640a 6c23 6d24 5a24 0100 6400 640b  d.d.l#m$Z$..d.d.
 000000f0: 6c25 6d26 5a26 0100 650d 6a27 640c 6508  l%m&Z&..e.j'd.e.
 00000100: 650c 6a28 650c 6a28 6602 1900 6602 640d  e.j(e.j(f...f.d.
 00000110: 640e 8404 8301 5a29 640f 6410 8400 5a2a  d.....Z)d.d...Z*
@@ -48,435 +48,434 @@
 000002f0: 0000 fa3e 2f68 6f6d 652f 7468 6f6d 6173  ...>/home/thomas
 00000300: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
 00000310: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
 00000320: 7465 7374 732f 7465 7374 5f63 6173 742e  tests/test_cast.
 00000330: 7079 da19 7379 6e74 6865 7469 635f 7472  py..synthetic_tr
 00000340: 6169 6e5f 7465 7374 5f64 6174 611b 0000  ain_test_data...
 00000350: 0073 0600 0000 0c02 0c01 0801 721b 0000  .s..........r...
-00000360: 0063 0100 0000 0000 0000 0000 0000 1100  .c..............
-00000370: 0000 0a00 0000 4300 0000 73e2 0200 007c  ......C...s....|
+00000360: 0063 0100 0000 0000 0000 0000 0000 1000  .c..............
+00000370: 0000 0a00 0000 4300 0000 73ba 0200 007c  ......C...s....|
 00000380: 0064 0119 007d 017c 0064 0219 007d 0274  .d...}.|.d...}.t
 00000390: 0083 007d 0364 037c 035f 0164 047c 035f  ...}.d.|._.d.|._
-000003a0: 0274 0383 007d 0464 057c 045f 0474 0583  .t...}.d.|._.t..
-000003b0: 007d 0574 0674 07a0 08a1 0064 0274 0964  .}.t.t.....d.t.d
-000003c0: 0664 0164 0764 088d 0364 0274 0a74 0b83  .d.d.d...d.t.t..
-000003d0: 0164 0264 098d 067c 055f 0c47 0064 0a64  .d.d...|._.G.d.d
-000003e0: 0b84 0064 0b74 0d83 037d 067c 0683 007d  ...d.t...}.|...}
-000003f0: 0774 0e64 0c64 0d7c 047c 037c 077c 0564  .t.d.d.|.|.|.|.d
-00000400: 0e8d 067d 087c 086a 0f7c 0164 0d64 0f8d  ...}.|.j.|.d.d..
-00000410: 0201 0074 1064 1083 0101 007c 08a0 117c  ...t.d.....|...|
-00000420: 026a 1264 0d64 0264 118d 02a1 015c 027d  .j.d.d.d.....\.}
-00000430: 097d 0a74 1064 1283 0101 0074 137c 0983  .}.t.d.....t.|..
-00000440: 017d 0b7c 026a 147d 0c74 137c 0c83 017d  .}.|.j.}.t.|...}
-00000450: 0d7c 0b7c 0d6b 027d 0e7c 0e73 da74 15a0  .|.|.k.}.|.s.t..
-00000460: 1664 137c 0e66 0164 147c 0b7c 0d66 02a1  .d.|.f.d.|.|.f..
-00000470: 0464 1574 17a0 18a1 0076 0073 8474 15a0  .d.t.....v.s.t..
-00000480: 1974 13a1 0172 8974 15a0 1a74 13a1 016e  .t...r.t...t...n
-00000490: 0164 1564 1674 17a0 18a1 0076 0073 9574  .d.d.t.....v.s.t
-000004a0: 15a0 197c 09a1 0172 9a74 15a0 1a7c 09a1  ...|...r.t...|..
-000004b0: 016e 0164 1674 15a0 1a7c 0ba1 0164 1574  .n.d.t...|...d.t
-000004c0: 17a0 18a1 0076 0073 aa74 15a0 1974 13a1  .....v.s.t...t..
-000004d0: 0172 af74 15a0 1a74 13a1 016e 0164 1564  .r.t...t...n.d.d
-000004e0: 1774 17a0 18a1 0076 0073 bb74 15a0 197c  .t.....v.s.t...|
-000004f0: 02a1 0172 c074 15a0 1a7c 02a1 016e 0164  ...r.t...|...n.d
-00000500: 1774 15a0 1a7c 0ca1 0174 15a0 1a7c 0da1  .t...|...t...|..
-00000510: 0164 189c 0716 007d 0f64 1964 1a7c 0f69  .d.....}.d.d.|.i
-00000520: 0116 007d 1074 1b74 15a0 1c7c 10a1 0183  ...}.t.t...|....
-00000530: 0182 0164 1b04 007d 0b04 007d 0e04 007d  ...d...}...}...}
-00000540: 0c7d 0d74 137c 0a83 017d 0b7c 026a 147d  .}.t.|...}.|.j.}
-00000550: 0c74 137c 0c83 017d 0d7c 0b7c 0d6b 027d  .t.|...}.|.|.k.}
-00000560: 0e7c 0e90 0173 6774 15a0 1664 137c 0e66  .|...sgt...d.|.f
-00000570: 0164 147c 0b7c 0d66 02a1 0464 1574 17a0  .d.|.|.f...d.t..
-00000580: 18a1 0076 0090 0173 0b74 15a0 1974 13a1  ...v...s.t...t..
-00000590: 0190 0172 1074 15a0 1a74 13a1 016e 0164  ...r.t...t...n.d
-000005a0: 1564 1c74 17a0 18a1 0076 0090 0173 1e74  .d.t.....v...s.t
-000005b0: 15a0 197c 0aa1 0190 0172 2374 15a0 1a7c  ...|.....r#t...|
-000005c0: 0aa1 016e 0164 1c74 15a0 1a7c 0ba1 0164  ...n.d.t...|...d
-000005d0: 1574 17a0 18a1 0076 0090 0173 3574 15a0  .t.....v...s5t..
-000005e0: 1974 13a1 0190 0172 3a74 15a0 1a74 13a1  .t.....r:t...t..
-000005f0: 016e 0164 1564 1774 17a0 18a1 0076 0090  .n.d.d.t.....v..
-00000600: 0173 4874 15a0 197c 02a1 0190 0172 4d74  .sHt...|.....rMt
-00000610: 15a0 1a7c 02a1 016e 0164 1774 15a0 1a7c  ...|...n.d.t...|
-00000620: 0ca1 0174 15a0 1a7c 0da1 0164 189c 0716  ...t...|...d....
-00000630: 007d 0f64 1964 1a7c 0f69 0116 007d 1074  .}.d.d.|.i...}.t
-00000640: 1b74 15a0 1c7c 10a1 0183 0182 0164 1b04  .t...|.......d..
-00000650: 007d 0b04 007d 0e04 007d 0c7d 0d64 1b53  .}...}...}.}.d.S
-00000660: 0029 1d7a 2254 6573 7420 7468 6174 2074  .).z"Test that t
-00000670: 6573 7473 2074 6865 2042 6c75 6543 6173  ests the BlueCas
-00000680: 7420 636c 6173 7372 0100 0000 e901 0000  t classr........
-00000690: 00e9 6400 0000 e910 0000 00e9 0a00 0000  ..d.............
-000006a0: e902 0000 0054 a902 7215 0000 00da 0773  .....T..r......s
-000006b0: 6875 6666 6c65 a906 5a09 6573 7469 6d61  huffle..Z.estima
-000006c0: 746f 72da 0473 7465 705a 0263 765a 166d  tor..stepZ.cvZ.m
-000006d0: 696e 5f66 6561 7475 7265 735f 746f 5f73  in_features_to_s
-000006e0: 656c 6563 745a 0773 636f 7269 6e67 5a06  electZ.scoringZ.
-000006f0: 6e5f 6a6f 6273 6300 0000 0000 0000 0000  n_jobsc.........
-00000700: 0000 0000 0000 000c 0000 0040 0000 0073  ...........@...s
-00000710: 8000 0000 6500 5a01 6400 5a02 6401 6503  ....e.Z.d.Z.d.e.
-00000720: 6a04 6402 6503 6a04 6604 6403 6404 8404  j.d.e.j.f.d.d...
-00000730: 5a05 6401 6503 6a04 6405 6503 6a06 6402  Z.d.e.j.d.e.j.d.
-00000740: 6507 6503 6a04 6503 6a06 6602 1900 6606  e.e.j.e.j.f...f.
-00000750: 6406 6407 8404 5a08 0908 0909 640d 6401  d.d...Z.....d.d.
-00000760: 6503 6a04 6405 6509 6503 6a06 1900 640a  e.j.d.e.e.j...d.
-00000770: 650a 6402 6507 6503 6a04 6509 6503 6a06  e.d.e.e.j.e.e.j.
-00000780: 1900 6602 1900 6608 640b 640c 8405 5a0b  ..f...f.d.d...Z.
-00000790: 6408 5300 290e 7a3d 7465 7374 5f62 6c75  d.S.).z=test_blu
-000007a0: 6570 7269 6e74 5f78 6762 6f6f 7374 2e3c  eprint_xgboost.<
-000007b0: 6c6f 6361 6c73 3e2e 4d79 4375 7374 6f6d  locals>.MyCustom
-000007c0: 4c61 7374 4d69 6c65 5072 6570 726f 6365  LastMilePreproce
-000007d0: 7373 696e 67da 0264 6672 1300 0000 6302  ssing..dfr....c.
-000007e0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000007f0: 0000 0053 0000 0073 1400 0000 7c01 6401  ...S...s....|.d.
-00000800: 1b00 7d01 6402 7c01 6403 3c00 7c01 5300  ..}.d.|.d.<.|.S.
-00000810: 2904 4e72 2000 0000 e905 0000 005a 0a63  ).Nr ........Z.c
-00000820: 7573 746f 6d5f 636f 6c72 1900 0000 2902  ustom_colr....).
-00000830: da04 7365 6c66 7225 0000 0072 1900 0000  ..selfr%...r....
-00000840: 7219 0000 0072 1a00 0000 da0f 6375 7374  r....r......cust
-00000850: 6f6d 5f66 756e 6374 696f 6e3a 0000 0073  om_function:...s
-00000860: 0600 0000 0801 0801 0401 7a4d 7465 7374  ..........zMtest
-00000870: 5f62 6c75 6570 7269 6e74 5f78 6762 6f6f  _blueprint_xgboo
-00000880: 7374 2e3c 6c6f 6361 6c73 3e2e 4d79 4375  st.<locals>.MyCu
-00000890: 7374 6f6d 4c61 7374 4d69 6c65 5072 6570  stomLastMilePrep
-000008a0: 726f 6365 7373 696e 672e 6375 7374 6f6d  rocessing.custom
-000008b0: 5f66 756e 6374 696f 6eda 0674 6172 6765  _function..targe
-000008c0: 7463 0300 0000 0000 0000 0000 0000 0300  tc..............
-000008d0: 0000 0300 0000 5300 0000 7326 0000 007c  ......S...s&...|
-000008e0: 00a0 007c 01a1 017d 017c 01a0 0164 01a1  ...|...}.|...d..
-000008f0: 017d 017c 02a0 0164 01a1 017d 027c 017c  .}.|...d...}.|.|
-00000900: 0266 0253 0029 024e 69e8 0300 0029 0272  .f.S.).Ni....).r
-00000910: 2800 0000 da04 6865 6164 2903 7227 0000  (.....head).r'..
-00000920: 0072 2500 0000 7229 0000 0072 1900 0000  .r%...r)...r....
-00000930: 7219 0000 0072 1a00 0000 da0d 6669 745f  r....r......fit_
-00000940: 7472 616e 7366 6f72 6d3f 0000 0073 0800  transform?...s..
-00000950: 0000 0a03 0a01 0a01 0801 7a4b 7465 7374  ..........zKtest
-00000960: 5f62 6c75 6570 7269 6e74 5f78 6762 6f6f  _blueprint_xgboo
-00000970: 7374 2e3c 6c6f 6361 6c73 3e2e 4d79 4375  st.<locals>.MyCu
-00000980: 7374 6f6d 4c61 7374 4d69 6c65 5072 6570  stomLastMilePrep
-00000990: 726f 6365 7373 696e 672e 6669 745f 7472  rocessing.fit_tr
-000009a0: 616e 7366 6f72 6d4e 46da 0e70 7265 6469  ansformNF..predi
-000009b0: 6374 6f6e 5f6d 6f64 6563 0400 0000 0000  cton_modec......
-000009c0: 0000 0000 0000 0400 0000 0300 0000 5300  ..............S.
-000009d0: 0000 7336 0000 007c 00a0 007c 01a1 017d  ..s6...|...|...}
-000009e0: 017c 0373 1774 017c 0274 026a 0383 0272  .|.s.t.|.t.j...r
-000009f0: 177c 01a0 0464 01a1 017d 017c 02a0 0464  .|...d...}.|...d
-00000a00: 01a1 017d 027c 017c 0266 0253 0029 024e  ...}.|.|.f.S.).N
-00000a10: 721d 0000 0029 0572 2800 0000 da0a 6973  r....).r(.....is
-00000a20: 696e 7374 616e 6365 da02 7064 da06 5365  instance..pd..Se
-00000a30: 7269 6573 722a 0000 0029 0472 2700 0000  riesr*...).r'...
-00000a40: 7225 0000 0072 2900 0000 722c 0000 0072  r%...r)...r,...r
-00000a50: 1900 0000 7219 0000 0072 1a00 0000 da09  ....r....r......
-00000a60: 7472 616e 7366 6f72 6d47 0000 0073 0a00  transformG...s..
-00000a70: 0000 0a06 1001 0a01 0a01 0801 7a47 7465  ............zGte
-00000a80: 7374 5f62 6c75 6570 7269 6e74 5f78 6762  st_blueprint_xgb
-00000a90: 6f6f 7374 2e3c 6c6f 6361 6c73 3e2e 4d79  oost.<locals>.My
-00000aa0: 4375 7374 6f6d 4c61 7374 4d69 6c65 5072  CustomLastMilePr
-00000ab0: 6570 726f 6365 7373 696e 672e 7472 616e  eprocessing.tran
-00000ac0: 7366 6f72 6d29 024e 4629 0cda 085f 5f6e  sform).NF)...__n
-00000ad0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000ae0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000af0: 2e00 0000 da09 4461 7461 4672 616d 6572  ......DataFramer
-00000b00: 2800 0000 722f 0000 0072 0300 0000 722b  (...r/...r....r+
-00000b10: 0000 0072 0200 0000 da04 626f 6f6c 7230  ...r......boolr0
-00000b20: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
-00000b30: 0000 721a 0000 00da 1d4d 7943 7573 746f  ..r......MyCusto
-00000b40: 6d4c 6173 744d 696c 6550 7265 7072 6f63  mLastMilePreproc
-00000b50: 6573 7369 6e67 3900 0000 7328 0000 0008  essing9...s(....
-00000b60: 0016 0102 0504 0102 ff04 0102 ff0e 020a  ................
-00000b70: fe02 0b02 0104 fc04 0202 fe08 0302 fd02  ................
-00000b80: 0402 fc12 050e fb72 3600 0000 da06 6269  .......r6.....bi
-00000b90: 6e61 7279 7229 0000 0029 06da 0d63 6c61  naryr)...)...cla
-00000ba0: 7373 5f70 726f 626c 656d da0d 7461 7267  ss_problem..targ
-00000bb0: 6574 5f63 6f6c 756d 6e5a 0d63 6f6e 665f  et_columnZ.conf_
-00000bc0: 7472 6169 6e69 6e67 5a0c 636f 6e66 5f78  trainingZ.conf_x
-00000bd0: 6762 6f6f 7374 da1c 6375 7374 6f6d 5f6c  gboost..custom_l
-00000be0: 6173 745f 6d69 6c65 5f63 6f6d 7075 7461  ast_mile_computa
-00000bf0: 7469 6f6e da16 636f 6e66 5f66 6561 7475  tion..conf_featu
-00000c00: 7265 5f73 656c 6563 7469 6f6e 2901 5a0a  re_selection).Z.
-00000c10: 7461 7267 6574 5f63 6f6c 7a16 4175 746f  target_colz.Auto
-00000c20: 7475 6e69 6e67 2073 7563 6365 7373 6675  tuning successfu
-00000c30: 6c2e 2901 5a04 6178 6973 7a16 5072 6564  l.).Z.axisz.Pred
-00000c40: 6963 7469 6e67 2073 7563 6365 7373 6675  icting successfu
-00000c50: 6c2e 2901 fa02 3d3d 2901 7a6b 2528 7079  l.)...==).zk%(py
-00000c60: 3329 730a 7b25 2870 7933 2973 203d 2025  3)s.{%(py3)s = %
-00000c70: 2870 7930 2973 2825 2870 7931 2973 290a  (py0)s(%(py1)s).
-00000c80: 7d20 3d3d 2025 2870 7931 3029 730a 7b25  } == %(py10)s.{%
-00000c90: 2870 7931 3029 7320 3d20 2528 7079 3529  (py10)s = %(py5)
-00000ca0: 7328 2528 7079 3829 730a 7b25 2870 7938  s(%(py8)s.{%(py8
-00000cb0: 2973 203d 2025 2870 7936 2973 2e69 6e64  )s = %(py6)s.ind
-00000cc0: 6578 0a7d 290a 7dda 036c 656e da07 795f  ex.}).}..len..y_
-00000cd0: 7072 6f62 7372 1800 0000 2907 da03 7079  probsr....)...py
-00000ce0: 30da 0370 7931 5a03 7079 335a 0370 7935  0..py1Z.py3Z.py5
-00000cf0: da03 7079 365a 0370 7938 5a04 7079 3130  ..py6Z.py8Z.py10
-00000d00: 7a0f 6173 7365 7274 2025 2870 7931 3229  z.assert %(py12)
-00000d10: 735a 0470 7931 324e da09 795f 636c 6173  sZ.py12N..y_clas
-00000d20: 7365 7329 1d72 0c00 0000 5a09 7374 6570  ses).r....Z.step
-00000d30: 735f 6d61 785a 0e6e 756d 5f6c 6561 7665  s_maxZ.num_leave
-00000d40: 735f 6d61 7872 0b00 0000 5a1c 6879 7065  s_maxr....Z.hype
-00000d50: 7270 6172 616d 6574 6572 5f74 756e 696e  rparameter_tunin
-00000d60: 675f 726f 756e 6473 720a 0000 0072 0500  g_roundsr....r..
-00000d70: 0000 da03 7867 62da 0d58 4742 436c 6173  ....xgb..XGBClas
-00000d80: 7369 6669 6572 7208 0000 0072 0600 0000  sifierr....r....
-00000d90: 7207 0000 00da 1273 656c 6563 7469 6f6e  r......selection
-00000da0: 5f73 7472 6174 6567 7972 1000 0000 7209  _strategyr....r.
-00000db0: 0000 00da 0366 6974 da05 7072 696e 74da  .....fit..print.
-00000dc0: 0770 7265 6469 6374 5a04 6472 6f70 723d  .predictZ.dropr=
-00000dd0: 0000 00da 0569 6e64 6578 da0a 4070 7974  .....index..@pyt
-00000de0: 6573 745f 6172 da11 5f63 616c 6c5f 7265  est_ar.._call_re
-00000df0: 7072 636f 6d70 6172 65da 0c40 7079 5f62  prcompare..@py_b
-00000e00: 7569 6c74 696e 73da 066c 6f63 616c 73da  uiltins..locals.
-00000e10: 185f 7368 6f75 6c64 5f72 6570 725f 676c  ._should_repr_gl
-00000e20: 6f62 616c 5f6e 616d 65da 095f 7361 6665  obal_name.._safe
-00000e30: 7265 7072 da0e 4173 7365 7274 696f 6e45  repr..AssertionE
-00000e40: 7272 6f72 da13 5f66 6f72 6d61 745f 6578  rror.._format_ex
-00000e50: 706c 616e 6174 696f 6e29 1172 1b00 0000  planation).r....
-00000e60: 7217 0000 0072 1800 0000 5a14 7867 626f  r....r....Z.xgbo
-00000e70: 6f73 745f 7061 7261 6d5f 636f 6e66 6967  ost_param_config
-00000e80: 5a0c 7472 6169 6e5f 636f 6e66 6967 da0f  Z.train_config..
-00000e90: 6375 7374 6f6d 5f66 6561 745f 7365 6c72  custom_feat_selr
-00000ea0: 3600 0000 723a 0000 005a 0661 7574 6f6d  6...r:...Z.autom
-00000eb0: 6c72 3e00 0000 7242 0000 005a 0b40 7079  lr>...rB...Z.@py
-00000ec0: 5f61 7373 6572 7432 5a0b 4070 795f 6173  _assert2Z.@py_as
-00000ed0: 7365 7274 375a 0b40 7079 5f61 7373 6572  sert7Z.@py_asser
-00000ee0: 7439 5a0b 4070 795f 6173 7365 7274 345a  t9Z.@py_assert4Z
-00000ef0: 0c40 7079 5f66 6f72 6d61 7431 315a 0c40  .@py_format11Z.@
-00000f00: 7079 5f66 6f72 6d61 7431 3372 1900 0000  py_format13r....
-00000f10: 7219 0000 0072 1a00 0000 da16 7465 7374  r....r......test
-00000f20: 5f62 6c75 6570 7269 6e74 5f78 6762 6f6f  _blueprint_xgboo
-00000f30: 7374 2200 0000 7344 0000 0008 0208 0106  st"...sD........
-00000f40: 0106 0106 0106 0106 0106 0302 0206 0102  ................
-00000f50: 010c 0102 0106 0102 0108 fa10 0a06 1a02  ................
-00000f60: 0202 0102 0102 0102 0102 0102 0106 fa0e  ................
-00000f70: 0808 0118 0108 01fe 010a 00fe 0120 0072  ............. .r
-00000f80: 5300 0000 6300 0000 0000 0000 0000 0000  S...c...........
-00000f90: 0000 0000 000a 0000 0040 0000 0073 5600  .........@...sV.
-00000fa0: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
-00000fb0: 5a03 6403 6504 6a05 6404 6504 6a05 6405  Z.d.e.j.d.e.j.d.
-00000fc0: 6504 6a06 6406 6504 6a06 6407 6408 660a  e.j.d.e.j.d.d.f.
-00000fd0: 6409 640a 8404 5a07 640b 6504 6a05 6407  d.d...Z.d.e.j.d.
-00000fe0: 6508 6509 650a 6602 1900 6604 640c 640d  e.e.e.f...f.d.d.
-00000ff0: 8404 5a0b 6408 5300 290e da0b 4375 7374  ..Z.d.S.)...Cust
-00001000: 6f6d 4d6f 6465 6c63 0100 0000 0000 0000  omModelc........
-00001010: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00001020: 730a 0000 0064 007c 005f 0064 0053 00a9  s....d.|._.d.S..
-00001030: 014e 2901 da05 6d6f 6465 6c29 0172 2700  .N)...model).r'.
-00001040: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00001050: 00da 085f 5f69 6e69 745f 5f66 0000 0073  ...__init__f...s
-00001060: 0200 0000 0a01 7a14 4375 7374 6f6d 4d6f  ......z.CustomMo
-00001070: 6465 6c2e 5f5f 696e 6974 5f5f da07 785f  del.__init__..x_
-00001080: 7472 6169 6eda 0678 5f74 6573 74da 0779  train..x_test..y
-00001090: 5f74 7261 696e da06 795f 7465 7374 7213  _train..y_testr.
-000010a0: 0000 004e 6305 0000 0000 0000 0000 0000  ...Nc...........
-000010b0: 0005 0000 0004 0000 0043 0000 0073 1a00  .........C...s..
-000010c0: 0000 7400 8300 7c00 5f01 7c00 6a01 a002  ..t...|._.|.j...
-000010d0: 7c01 7c03 a102 0100 6400 5300 7255 0000  |.|.....d.S.rU..
-000010e0: 0029 0372 0400 0000 7256 0000 0072 4600  .).r....rV...rF.
-000010f0: 0000 2905 7227 0000 0072 5800 0000 7259  ..).r'...rX...rY
-00001100: 0000 0072 5a00 0000 725b 0000 0072 1900  ...rZ...r[...r..
-00001110: 0000 7219 0000 0072 1a00 0000 7246 0000  ..r....r....rF..
-00001120: 0069 0000 0073 0400 0000 0807 1201 7a0f  .i...s........z.
-00001130: 4375 7374 6f6d 4d6f 6465 6c2e 6669 7472  CustomModel.fitr
-00001140: 2500 0000 6302 0000 0000 0000 0000 0000  %...c...........
-00001150: 0004 0000 0003 0000 0043 0000 0073 2000  .........C...s .
-00001160: 0000 7c00 6a00 a001 7c01 a101 7d02 7c00  ..|.j...|...}.|.
-00001170: 6a00 a002 7c01 a101 7d03 7c02 7c03 6602  j...|...}.|.|.f.
-00001180: 5300 7255 0000 0029 0372 5600 0000 5a0d  S.rU...).rV...Z.
-00001190: 7072 6564 6963 745f 7072 6f62 6172 4800  predict_probarH.
-000011a0: 0000 2904 7227 0000 0072 2500 0000 da10  ..).r'...r%.....
-000011b0: 7072 6564 6963 7465 645f 7072 6f62 6173  predicted_probas
-000011c0: da11 7072 6564 6963 7465 645f 636c 6173  ..predicted_clas
-000011d0: 7365 7372 1900 0000 7219 0000 0072 1a00  sesr....r....r..
-000011e0: 0000 7248 0000 0073 0000 0073 0600 0000  ..rH...s...s....
-000011f0: 0c01 0c01 0801 7a13 4375 7374 6f6d 4d6f  ......z.CustomMo
-00001200: 6465 6c2e 7072 6564 6963 7429 0c72 3100  del.predict).r1.
-00001210: 0000 7232 0000 0072 3300 0000 7257 0000  ..r2...r3...rW..
-00001220: 0072 2e00 0000 7234 0000 0072 2f00 0000  .r....r4...r/...
-00001230: 7246 0000 0072 0300 0000 720f 0000 0072  rF...r....r....r
-00001240: 0e00 0000 7248 0000 0072 1900 0000 7219  ....rH...r....r.
-00001250: 0000 0072 1900 0000 721a 0000 0072 5400  ...r....r....rT.
-00001260: 0000 6500 0000 731c 0000 0008 0008 0102  ..e...s.........
-00001270: 0304 0202 fe04 0302 fd04 0402 fc04 0502  ................
-00001280: fb02 060a fa20 0a72 5400 0000 6300 0000  ..... .rT...c...
-00001290: 0000 0000 0000 0000 000b 0000 000a 0000  ................
-000012a0: 0043 0000 0073 b202 0000 7400 8300 7d00  .C...s....t...}.
-000012b0: 7401 8300 7d01 7402 7403 a004 a100 6401  t...}.t.t.....d.
-000012c0: 7405 6402 6403 6404 6405 8d03 6406 7406  t.d.d.d.d...d.t.
-000012d0: 7407 8301 6401 6407 8d06 7c01 5f08 7409  t...d.d...|._.t.
-000012e0: 6408 6409 7c00 7c01 640a 8d04 7d02 740a  d.d.|.|.d...}.t.
-000012f0: a00b 640b 640c 8400 740c 640d 8301 4400  ..d.d...t.d...D.
-00001300: 8301 640e 640c 8400 740c 640d 8301 4400  ..d.d...t.d...D.
-00001310: 8301 640f 640c 8400 740c 640d 8301 4400  ..d.d...t.d...D.
-00001320: 8301 6410 640c 8400 740c 640d 8301 4400  ..d.d...t.d...D.
-00001330: 8301 6411 640c 8400 740c 640d 8301 4400  ..d.d...t.d...D.
-00001340: 8301 6412 640c 8400 740c 640d 8301 4400  ..d.d...t.d...D.
-00001350: 8301 6413 9c06 a101 7d03 740a a00d 6700  ..d.....}.t...g.
-00001360: 6414 a201 a101 7d04 740a a00b 6415 640c  d.....}.t...d.d.
-00001370: 8400 740c 640d 8301 4400 8301 6416 640c  ..t.d...D...d.d.
-00001380: 8400 740c 640d 8301 4400 8301 6417 640c  ..t.d...D...d.d.
-00001390: 8400 740c 640d 8301 4400 8301 6418 640c  ..t.d...D...d.d.
-000013a0: 8400 740c 640d 8301 4400 8301 6419 640c  ..t.d...D...d.d.
-000013b0: 8400 740c 640d 8301 4400 8301 641a 640c  ..t.d...D...d.d.
-000013c0: 8400 740c 640d 8301 4400 8301 6413 9c06  ..t.d...D...d...
-000013d0: a101 7d05 7c04 7c03 6409 3c00 7c02 a00e  ..}.|.|.d.<.|...
-000013e0: 7c03 6409 a102 0100 7c02 a00f 7c05 a101  |.d.....|...|...
-000013f0: 5c02 7d06 7d07 7410 6a11 7d08 7412 7c06  \.}.}.t.j.}.t.|.
-00001400: 7c08 8302 7d09 7c09 73f7 641b 641c 7413  |...}.|.s.d.d.t.
-00001410: a014 a100 7600 73bc 7415 a016 7412 a101  ....v.s.t...t...
-00001420: 72c1 7415 a017 7412 a101 6e01 641c 641d  r.t...t...n.d.d.
-00001430: 7413 a014 a100 7600 73cd 7415 a016 7c06  t.....v.s.t...|.
-00001440: a101 72d2 7415 a017 7c06 a101 6e01 641d  ..r.t...|...n.d.
-00001450: 641e 7413 a014 a100 7600 73de 7415 a016  d.t.....v.s.t...
-00001460: 7410 a101 72e3 7415 a017 7410 a101 6e01  t...r.t...t...n.
-00001470: 641e 7415 a017 7c08 a101 7415 a017 7c09  d.t...|...t...|.
-00001480: a101 641f 9c05 1600 7d0a 7418 7415 a019  ..d.....}.t.t...
-00001490: 7c0a a101 8301 8201 6400 0400 7d08 7d09  |.......d...}.}.
-000014a0: 7410 6a11 7d08 7412 7c07 7c08 8302 7d09  t.j.}.t.|.|...}.
-000014b0: 7c09 9001 7353 641b 641c 7413 a014 a100  |...sSd.d.t.....
-000014c0: 7600 9001 7314 7415 a016 7412 a101 9001  v...s.t...t.....
-000014d0: 7219 7415 a017 7412 a101 6e01 641c 6420  r.t...t...n.d.d 
-000014e0: 7413 a014 a100 7600 9001 7327 7415 a016  t.....v...s't...
-000014f0: 7c07 a101 9001 722c 7415 a017 7c07 a101  |.....r,t...|...
-00001500: 6e01 6420 641e 7413 a014 a100 7600 9001  n.d d.t.....v...
-00001510: 733a 7415 a016 7410 a101 9001 723f 7415  s:t...t.....r?t.
-00001520: a017 7410 a101 6e01 641e 7415 a017 7c08  ..t...n.d.t...|.
-00001530: a101 7415 a017 7c09 a101 641f 9c05 1600  ..t...|...d.....
-00001540: 7d0a 7418 7415 a019 7c0a a101 8301 8201  }.t.t...|.......
-00001550: 6400 0400 7d08 7d09 6400 5300 2921 4e72  d...}.}.d.S.)!Nr
-00001560: 1c00 0000 7220 0000 0072 0100 0000 5472  ....r ...r....Tr
-00001570: 2100 0000 7226 0000 0072 2300 0000 7237  !...r&...r#...r7
-00001580: 0000 0072 2900 0000 2904 7238 0000 0072  ...r)...).r8...r
-00001590: 3900 0000 5a08 6d6c 5f6d 6f64 656c 723b  9...Z.ml_modelr;
-000015a0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000015b0: 0200 0000 0300 0000 5300 0000 f310 0000  ........S.......
-000015c0: 0067 007c 005d 047d 017c 0191 0271 0253  .g.|.].}.|...q.S
-000015d0: 0072 1900 0000 7219 0000 00a9 02da 022e  .r....r.........
-000015e0: 30da 0169 7219 0000 0072 1900 0000 721a  0..ir....r....r.
-000015f0: 0000 00da 0a3c 6c69 7374 636f 6d70 3e93  .....<listcomp>.
-00001600: 0000 00f3 0200 0000 1000 7a33 7465 7374  ..........z3test
-00001610: 5f62 6c75 6563 6173 745f 7769 7468 5f63  _bluecast_with_c
-00001620: 7573 746f 6d5f 6d6f 6465 6c2e 3c6c 6f63  ustom_model.<loc
-00001630: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
-00001640: 1f00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00001650: 0002 0000 0003 0000 0053 0000 0072 5e00  .........S...r^.
-00001660: 0000 7219 0000 0072 1900 0000 725f 0000  ..r....r....r_..
-00001670: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00001680: 7262 0000 0094 0000 0072 6300 0000 6301  rb.......rc...c.
-00001690: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000016a0: 0000 0053 0000 0072 5e00 0000 7219 0000  ...S...r^...r...
-000016b0: 0072 1900 0000 725f 0000 0072 1900 0000  .r....r_...r....
-000016c0: 7219 0000 0072 1a00 0000 7262 0000 0095  r....r....rb....
-000016d0: 0000 0072 6300 0000 6301 0000 0000 0000  ...rc...c.......
-000016e0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-000016f0: 0072 5e00 0000 7219 0000 0072 1900 0000  .r^...r....r....
-00001700: 725f 0000 0072 1900 0000 7219 0000 0072  r_...r....r....r
-00001710: 1a00 0000 7262 0000 0096 0000 0072 6300  ....rb.......rc.
-00001720: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00001730: 0000 0003 0000 0053 0000 0072 5e00 0000  .......S...r^...
-00001740: 7219 0000 0072 1900 0000 725f 0000 0072  r....r....r_...r
-00001750: 1900 0000 7219 0000 0072 1a00 0000 7262  ....r....r....rb
-00001760: 0000 0097 0000 0072 6300 0000 6301 0000  .......rc...c...
-00001770: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00001780: 0053 0000 0072 5e00 0000 7219 0000 0072  .S...r^...r....r
-00001790: 1900 0000 725f 0000 0072 1900 0000 7219  ....r_...r....r.
-000017a0: 0000 0072 1a00 0000 7262 0000 0098 0000  ...r....rb......
-000017b0: 0072 6300 0000 2906 5a08 6665 6174 7572  .rc...).Z.featur
-000017c0: 6531 5a08 6665 6174 7572 6532 5a08 6665  e1Z.feature2Z.fe
-000017d0: 6174 7572 6533 5a08 6665 6174 7572 6534  ature3Z.feature4
-000017e0: 5a08 6665 6174 7572 6535 5a08 6665 6174  Z.feature5Z.feat
-000017f0: 7572 6536 290a 7201 0000 0072 1c00 0000  ure6).r....r....
-00001800: 7201 0000 0072 1c00 0000 7201 0000 0072  r....r....r....r
-00001810: 1c00 0000 7201 0000 0072 1c00 0000 7201  ....r....r....r.
-00001820: 0000 0072 1c00 0000 6301 0000 0000 0000  ...r....c.......
-00001830: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-00001840: 0072 5e00 0000 7219 0000 0072 1900 0000  .r^...r....r....
-00001850: 725f 0000 0072 1900 0000 7219 0000 0072  r_...r....r....r
-00001860: 1a00 0000 7262 0000 009e 0000 0072 6300  ....rb.......rc.
-00001870: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00001880: 0000 0003 0000 0053 0000 0072 5e00 0000  .......S...r^...
-00001890: 7219 0000 0072 1900 0000 725f 0000 0072  r....r....r_...r
-000018a0: 1900 0000 7219 0000 0072 1a00 0000 7262  ....r....r....rb
-000018b0: 0000 009f 0000 0072 6300 0000 6301 0000  .......rc...c...
-000018c0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-000018d0: 0053 0000 0072 5e00 0000 7219 0000 0072  .S...r^...r....r
-000018e0: 1900 0000 725f 0000 0072 1900 0000 7219  ....r_...r....r.
-000018f0: 0000 0072 1a00 0000 7262 0000 00a0 0000  ...r....rb......
-00001900: 0072 6300 0000 6301 0000 0000 0000 0000  .rc...c.........
-00001910: 0000 0002 0000 0003 0000 0053 0000 0072  ...........S...r
-00001920: 5e00 0000 7219 0000 0072 1900 0000 725f  ^...r....r....r_
-00001930: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00001940: 0000 7262 0000 00a1 0000 0072 6300 0000  ..rb.......rc...
-00001950: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001960: 0003 0000 0053 0000 0072 5e00 0000 7219  .....S...r^...r.
-00001970: 0000 0072 1900 0000 725f 0000 0072 1900  ...r....r_...r..
-00001980: 0000 7219 0000 0072 1a00 0000 7262 0000  ..r....r....rb..
-00001990: 00a2 0000 0072 6300 0000 6301 0000 0000  .....rc...c.....
-000019a0: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
-000019b0: 0000 0072 5e00 0000 7219 0000 0072 1900  ...r^...r....r..
-000019c0: 0000 725f 0000 0072 1900 0000 7219 0000  ..r_...r....r...
-000019d0: 0072 1a00 0000 7262 0000 00a3 0000 0072  .r....rb.......r
-000019e0: 6300 0000 7a52 6173 7365 7274 2025 2870  c...zRassert %(p
-000019f0: 7936 2973 0a7b 2528 7079 3629 7320 3d20  y6)s.{%(py6)s = 
-00001a00: 2528 7079 3029 7328 2528 7079 3129 732c  %(py0)s(%(py1)s,
-00001a10: 2025 2870 7934 2973 0a7b 2528 7079 3429   %(py4)s.{%(py4)
-00001a20: 7320 3d20 2528 7079 3229 732e 6e64 6172  s = %(py2)s.ndar
-00001a30: 7261 790a 7d29 0a7d 722d 0000 0072 5c00  ray.}).}r-...r\.
-00001a40: 0000 da02 6e70 2905 723f 0000 0072 4000  ....np).r?...r@.
-00001a50: 0000 5a03 7079 325a 0370 7934 7241 0000  ..Z.py2Z.py4rA..
-00001a60: 0072 5d00 0000 291a 7254 0000 0072 0a00  .r]...).rT...r..
-00001a70: 0000 7205 0000 0072 4300 0000 7244 0000  ..r....rC...rD..
-00001a80: 0072 0800 0000 7206 0000 0072 0700 0000  .r....r....r....
-00001a90: 7245 0000 0072 0900 0000 722e 0000 0072  rE...r....r....r
-00001aa0: 3400 0000 da05 7261 6e67 6572 2f00 0000  4.....ranger/...
-00001ab0: 7246 0000 0072 4800 0000 7264 0000 00da  rF...rH...rd....
-00001ac0: 076e 6461 7272 6179 722d 0000 0072 4c00  .ndarrayr-...rL.
-00001ad0: 0000 724d 0000 0072 4a00 0000 724e 0000  ..rM...rJ...rN..
-00001ae0: 0072 4f00 0000 7250 0000 0072 5100 0000  .rO...rP...rQ...
-00001af0: 290b 5a0c 6375 7374 6f6d 5f6d 6f64 656c  ).Z.custom_model
-00001b00: 7252 0000 00da 0862 6c75 6563 6173 7472  rR.....bluecastr
-00001b10: 5800 0000 725a 0000 0072 5900 0000 725c  X...rZ...rY...r\
-00001b20: 0000 0072 5d00 0000 5a0b 4070 795f 6173  ...r]...Z.@py_as
-00001b30: 7365 7274 335a 0b40 7079 5f61 7373 6572  sert3Z.@py_asser
-00001b40: 7435 5a0b 4070 795f 666f 726d 6174 3772  t5Z.@py_format7r
-00001b50: 1900 0000 7219 0000 0072 1a00 0000 da1f  ....r....r......
-00001b60: 7465 7374 5f62 6c75 6563 6173 745f 7769  test_bluecast_wi
-00001b70: 7468 5f63 7573 746f 6d5f 6d6f 6465 6c79  th_custom_modely
-00001b80: 0000 0073 5000 0000 0602 0603 0201 0601  ...sP...........
-00001b90: 0201 0c01 0201 0601 0201 08fa 020a 0201  ................
-00001ba0: 0201 0201 0201 06fc 0408 1002 1001 1001  ................
-00001bb0: 1001 1001 1001 04fa 04ff 0e0a 0401 1002  ................
-00001bc0: 1001 1001 1001 1001 1001 04fa 04ff 080b  ................
-00001bd0: 0c03 0e03 aa03 bc01 7268 0000 0029 2dda  ........rh...)-.
-00001be0: 0862 7569 6c74 696e 7372 4c00 0000 da19  .builtinsrL.....
-00001bf0: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
-00001c00: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
-00001c10: 7469 6f6e da07 7265 7772 6974 6572 4a00  tion..rewriterJ.
-00001c20: 0000 da06 7479 7069 6e67 7202 0000 0072  ....typingr....r
-00001c30: 0300 0000 da05 6e75 6d70 7972 6400 0000  ......numpyrd...
-00001c40: 5a06 7061 6e64 6173 722e 0000 00da 0670  Z.pandasr......p
-00001c50: 7974 6573 745a 0778 6762 6f6f 7374 7243  ytestZ.xgboostrC
-00001c60: 0000 005a 1073 6b6c 6561 726e 2e65 6e73  ...Z.sklearn.ens
-00001c70: 656d 626c 6572 0400 0000 5a19 736b 6c65  embler....Z.skle
-00001c80: 6172 6e2e 6665 6174 7572 655f 7365 6c65  arn.feature_sele
-00001c90: 6374 696f 6e72 0500 0000 5a0f 736b 6c65  ctionr....Z.skle
-00001ca0: 6172 6e2e 6d65 7472 6963 7372 0600 0000  arn.metricsr....
-00001cb0: 7207 0000 005a 1773 6b6c 6561 726e 2e6d  r....Z.sklearn.m
-00001cc0: 6f64 656c 5f73 656c 6563 7469 6f6e 7208  odel_selectionr.
-00001cd0: 0000 005a 1862 6c75 6563 6173 742e 626c  ...Z.bluecast.bl
-00001ce0: 7565 7072 696e 7473 2e63 6173 7472 0900  ueprints.castr..
-00001cf0: 0000 5a1f 626c 7565 6361 7374 2e63 6f6e  ..Z.bluecast.con
-00001d00: 6669 672e 7472 6169 6e69 6e67 5f63 6f6e  fig.training_con
-00001d10: 6669 6772 0a00 0000 720b 0000 0072 0c00  figr....r....r..
-00001d20: 0000 5a22 626c 7565 6361 7374 2e6d 6c5f  ..Z"bluecast.ml_
-00001d30: 6d6f 6465 6c6c 696e 672e 6261 7365 5f63  modelling.base_c
-00001d40: 6c61 7373 6573 720d 0000 0072 0e00 0000  lassesr....r....
-00001d50: 720f 0000 005a 1d62 6c75 6563 6173 742e  r....Z.bluecast.
-00001d60: 7072 6570 726f 6365 7373 696e 672e 6375  preprocessing.cu
-00001d70: 7374 6f6d 7210 0000 005a 2462 6c75 6563  stomr....Z$bluec
-00001d80: 6173 742e 7465 7374 732e 6d61 6b65 5f64  ast.tests.make_d
-00001d90: 6174 612e 6372 6561 7465 5f64 6174 6172  ata.create_datar
-00001da0: 1200 0000 da07 6669 7874 7572 6572 3400  ......fixturer4.
-00001db0: 0000 721b 0000 0072 5300 0000 7254 0000  ..r....rS...rT..
-00001dc0: 0072 6800 0000 7219 0000 0072 1900 0000  .rh...r....r....
-00001dd0: 7219 0000 0072 1a00 0000 da08 3c6d 6f64  r....r......<mod
-00001de0: 756c 653e 0100 0000 7326 0000 002a 0008  ule>....s&...*..
-00001df0: 0208 0108 0108 010c 010c 0110 010c 010c  ................
-00001e00: 0214 0114 050c 050c 0104 031c 0108 0610  ................
-00001e10: 430c 14                                  C..
+000003a0: 0274 0383 007d 0464 057c 045f 0464 067c  .t...}.d.|._.d.|
+000003b0: 045f 0564 077c 045f 0647 0064 0864 0984  ._.d.|._.G.d.d..
+000003c0: 0064 0974 0783 037d 057c 0583 007d 0674  .d.t...}.|...}.t
+000003d0: 0864 0a64 0b7c 047c 037c 0664 0c8d 057d  .d.d.|.|.|.d...}
+000003e0: 077c 076a 097c 0164 0b64 0d8d 0201 0074  .|.j.|.d.d.....t
+000003f0: 0a64 0e83 0101 007c 07a0 0b7c 026a 0c64  .d.....|...|.j.d
+00000400: 0b64 0264 0f8d 02a1 015c 027d 087d 0974  .d.d.....\.}.}.t
+00000410: 0a64 1083 0101 0074 0d7c 0883 017d 0a7c  .d.....t.|...}.|
+00000420: 026a 0e7d 0b74 0d7c 0b83 017d 0c7c 0a7c  .j.}.t.|...}.|.|
+00000430: 0c6b 027d 0d7c 0d73 c874 0fa0 1064 117c  .k.}.|.s.t...d.|
+00000440: 0d66 0164 127c 0a7c 0c66 02a1 0464 1374  .f.d.|.|.f...d.t
+00000450: 11a0 12a1 0076 0073 7274 0fa0 1374 0da1  .....v.srt...t..
+00000460: 0172 7774 0fa0 1474 0da1 016e 0164 1364  .rwt...t...n.d.d
+00000470: 1474 11a0 12a1 0076 0073 8374 0fa0 137c  .t.....v.s.t...|
+00000480: 08a1 0172 8874 0fa0 147c 08a1 016e 0164  ...r.t...|...n.d
+00000490: 1474 0fa0 147c 0aa1 0164 1374 11a0 12a1  .t...|...d.t....
+000004a0: 0076 0073 9874 0fa0 1374 0da1 0172 9d74  .v.s.t...t...r.t
+000004b0: 0fa0 1474 0da1 016e 0164 1364 1574 11a0  ...t...n.d.d.t..
+000004c0: 12a1 0076 0073 a974 0fa0 137c 02a1 0172  ...v.s.t...|...r
+000004d0: ae74 0fa0 147c 02a1 016e 0164 1574 0fa0  .t...|...n.d.t..
+000004e0: 147c 0ba1 0174 0fa0 147c 0ca1 0164 169c  .|...t...|...d..
+000004f0: 0716 007d 0e64 1764 187c 0e69 0116 007d  ...}.d.d.|.i...}
+00000500: 0f74 1574 0fa0 167c 0fa1 0183 0182 0164  .t.t...|.......d
+00000510: 1904 007d 0a04 007d 0d04 007d 0b7d 0c74  ...}...}...}.}.t
+00000520: 0d7c 0983 017d 0a7c 026a 0e7d 0b74 0d7c  .|...}.|.j.}.t.|
+00000530: 0b83 017d 0c7c 0a7c 0c6b 027d 0d7c 0d90  ...}.|.|.k.}.|..
+00000540: 0173 5374 0fa0 1064 117c 0d66 0164 127c  .sSt...d.|.f.d.|
+00000550: 0a7c 0c66 02a1 0464 1374 11a0 12a1 0076  .|.f...d.t.....v
+00000560: 0073 f774 0fa0 1374 0da1 0172 fc74 0fa0  .s.t...t...r.t..
+00000570: 1474 0da1 016e 0164 1364 1a74 11a0 12a1  .t...n.d.d.t....
+00000580: 0076 0090 0173 0a74 0fa0 137c 09a1 0190  .v...s.t...|....
+00000590: 0172 0f74 0fa0 147c 09a1 016e 0164 1a74  .r.t...|...n.d.t
+000005a0: 0fa0 147c 0aa1 0164 1374 11a0 12a1 0076  ...|...d.t.....v
+000005b0: 0090 0173 2174 0fa0 1374 0da1 0190 0172  ...s!t...t.....r
+000005c0: 2674 0fa0 1474 0da1 016e 0164 1364 1574  &t...t...n.d.d.t
+000005d0: 11a0 12a1 0076 0090 0173 3474 0fa0 137c  .....v...s4t...|
+000005e0: 02a1 0190 0172 3974 0fa0 147c 02a1 016e  .....r9t...|...n
+000005f0: 0164 1574 0fa0 147c 0ba1 0174 0fa0 147c  .d.t...|...t...|
+00000600: 0ca1 0164 169c 0716 007d 0e64 1764 187c  ...d.....}.d.d.|
+00000610: 0e69 0116 007d 0f74 1574 0fa0 167c 0fa1  .i...}.t.t...|..
+00000620: 0183 0182 0164 1904 007d 0a04 007d 0d04  .....d...}...}..
+00000630: 007d 0b7d 0c64 1953 0029 1b7a 2254 6573  .}.}.d.S.).z"Tes
+00000640: 7420 7468 6174 2074 6573 7473 2074 6865  t that tests the
+00000650: 2042 6c75 6543 6173 7420 636c 6173 7372   BlueCast classr
+00000660: 0100 0000 e901 0000 00e9 6400 0000 e910  ..........d.....
+00000670: 0000 00e9 0a00 0000 54e9 0200 0000 6300  ........T.....c.
+00000680: 0000 0000 0000 0000 0000 0000 0000 000c  ................
+00000690: 0000 0040 0000 0073 8000 0000 6500 5a01  ...@...s....e.Z.
+000006a0: 6400 5a02 6401 6503 6a04 6402 6503 6a04  d.Z.d.e.j.d.e.j.
+000006b0: 6604 6403 6404 8404 5a05 6401 6503 6a04  f.d.d...Z.d.e.j.
+000006c0: 6405 6503 6a06 6402 6507 6503 6a04 6503  d.e.j.d.e.e.j.e.
+000006d0: 6a06 6602 1900 6606 6406 6407 8404 5a08  j.f...f.d.d...Z.
+000006e0: 0908 0909 640d 6401 6503 6a04 6405 6509  ....d.d.e.j.d.e.
+000006f0: 6503 6a06 1900 640a 650a 6402 6507 6503  e.j...d.e.d.e.e.
+00000700: 6a04 6509 6503 6a06 1900 6602 1900 6608  j.e.e.j...f...f.
+00000710: 640b 640c 8405 5a0b 6408 5300 290e 7a3d  d.d...Z.d.S.).z=
+00000720: 7465 7374 5f62 6c75 6570 7269 6e74 5f78  test_blueprint_x
+00000730: 6762 6f6f 7374 2e3c 6c6f 6361 6c73 3e2e  gboost.<locals>.
+00000740: 4d79 4375 7374 6f6d 4c61 7374 4d69 6c65  MyCustomLastMile
+00000750: 5072 6570 726f 6365 7373 696e 67da 0264  Preprocessing..d
+00000760: 6672 1300 0000 6302 0000 0000 0000 0000  fr....c.........
+00000770: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
+00000780: 1400 0000 7c01 6401 1b00 7d01 6402 7c01  ....|.d...}.d.|.
+00000790: 6403 3c00 7c01 5300 2904 4e72 2000 0000  d.<.|.S.).Nr ...
+000007a0: e905 0000 005a 0a63 7573 746f 6d5f 636f  .....Z.custom_co
+000007b0: 6c72 1900 0000 2902 da04 7365 6c66 7221  lr....)...selfr!
+000007c0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+000007d0: 0000 da0f 6375 7374 6f6d 5f66 756e 6374  ....custom_funct
+000007e0: 696f 6e30 0000 0073 0600 0000 0801 0801  ion0...s........
+000007f0: 0401 7a4d 7465 7374 5f62 6c75 6570 7269  ..zMtest_bluepri
+00000800: 6e74 5f78 6762 6f6f 7374 2e3c 6c6f 6361  nt_xgboost.<loca
+00000810: 6c73 3e2e 4d79 4375 7374 6f6d 4c61 7374  ls>.MyCustomLast
+00000820: 4d69 6c65 5072 6570 726f 6365 7373 696e  MilePreprocessin
+00000830: 672e 6375 7374 6f6d 5f66 756e 6374 696f  g.custom_functio
+00000840: 6eda 0674 6172 6765 7463 0300 0000 0000  n..targetc......
+00000850: 0000 0000 0000 0300 0000 0300 0000 5300  ..............S.
+00000860: 0000 7326 0000 007c 00a0 007c 01a1 017d  ..s&...|...|...}
+00000870: 017c 01a0 0164 01a1 017d 017c 02a0 0164  .|...d...}.|...d
+00000880: 01a1 017d 027c 017c 0266 0253 0029 024e  ...}.|.|.f.S.).N
+00000890: 69e8 0300 0029 0272 2400 0000 da04 6865  i....).r$.....he
+000008a0: 6164 2903 7223 0000 0072 2100 0000 7225  ad).r#...r!...r%
+000008b0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+000008c0: 0000 da0d 6669 745f 7472 616e 7366 6f72  ....fit_transfor
+000008d0: 6d35 0000 0073 0800 0000 0a03 0a01 0a01  m5...s..........
+000008e0: 0801 7a4b 7465 7374 5f62 6c75 6570 7269  ..zKtest_bluepri
+000008f0: 6e74 5f78 6762 6f6f 7374 2e3c 6c6f 6361  nt_xgboost.<loca
+00000900: 6c73 3e2e 4d79 4375 7374 6f6d 4c61 7374  ls>.MyCustomLast
+00000910: 4d69 6c65 5072 6570 726f 6365 7373 696e  MilePreprocessin
+00000920: 672e 6669 745f 7472 616e 7366 6f72 6d4e  g.fit_transformN
+00000930: 46da 0e70 7265 6469 6374 6f6e 5f6d 6f64  F..predicton_mod
+00000940: 6563 0400 0000 0000 0000 0000 0000 0400  ec..............
+00000950: 0000 0300 0000 5300 0000 7336 0000 007c  ......S...s6...|
+00000960: 00a0 007c 01a1 017d 017c 0373 1774 017c  ...|...}.|.s.t.|
+00000970: 0274 026a 0383 0272 177c 01a0 0464 01a1  .t.j...r.|...d..
+00000980: 017d 017c 02a0 0464 01a1 017d 027c 017c  .}.|...d...}.|.|
+00000990: 0266 0253 0029 024e 721d 0000 0029 0572  .f.S.).Nr....).r
+000009a0: 2400 0000 da0a 6973 696e 7374 616e 6365  $.....isinstance
+000009b0: da02 7064 da06 5365 7269 6573 7226 0000  ..pd..Seriesr&..
+000009c0: 0029 0472 2300 0000 7221 0000 0072 2500  .).r#...r!...r%.
+000009d0: 0000 7228 0000 0072 1900 0000 7219 0000  ..r(...r....r...
+000009e0: 0072 1a00 0000 da09 7472 616e 7366 6f72  .r......transfor
+000009f0: 6d3d 0000 0073 0a00 0000 0a06 1001 0a01  m=...s..........
+00000a00: 0a01 0801 7a47 7465 7374 5f62 6c75 6570  ....zGtest_bluep
+00000a10: 7269 6e74 5f78 6762 6f6f 7374 2e3c 6c6f  rint_xgboost.<lo
+00000a20: 6361 6c73 3e2e 4d79 4375 7374 6f6d 4c61  cals>.MyCustomLa
+00000a30: 7374 4d69 6c65 5072 6570 726f 6365 7373  stMilePreprocess
+00000a40: 696e 672e 7472 616e 7366 6f72 6d29 024e  ing.transform).N
+00000a50: 4629 0cda 085f 5f6e 616d 655f 5fda 0a5f  F)...__name__.._
+00000a60: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000a70: 6c6e 616d 655f 5f72 2a00 0000 da09 4461  lname__r*.....Da
+00000a80: 7461 4672 616d 6572 2400 0000 722b 0000  taFramer$...r+..
+00000a90: 0072 0300 0000 7227 0000 0072 0200 0000  .r....r'...r....
+00000aa0: da04 626f 6f6c 722c 0000 0072 1900 0000  ..boolr,...r....
+00000ab0: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+00000ac0: 1d4d 7943 7573 746f 6d4c 6173 744d 696c  .MyCustomLastMil
+00000ad0: 6550 7265 7072 6f63 6573 7369 6e67 2f00  ePreprocessing/.
+00000ae0: 0000 7328 0000 0008 0016 0102 0504 0102  ..s(............
+00000af0: ff04 0102 ff0e 020a fe02 0b02 0104 fc04  ................
+00000b00: 0202 fe08 0302 fd02 0402 fc12 050e fb72  ...............r
+00000b10: 3200 0000 da06 6269 6e61 7279 7225 0000  2.....binaryr%..
+00000b20: 0029 05da 0d63 6c61 7373 5f70 726f 626c  .)...class_probl
+00000b30: 656d da0d 7461 7267 6574 5f63 6f6c 756d  em..target_colum
+00000b40: 6eda 0d63 6f6e 665f 7472 6169 6e69 6e67  n..conf_training
+00000b50: 5a0c 636f 6e66 5f78 6762 6f6f 7374 da1c  Z.conf_xgboost..
+00000b60: 6375 7374 6f6d 5f6c 6173 745f 6d69 6c65  custom_last_mile
+00000b70: 5f63 6f6d 7075 7461 7469 6f6e 2901 5a0a  _computation).Z.
+00000b80: 7461 7267 6574 5f63 6f6c 7a16 4175 746f  target_colz.Auto
+00000b90: 7475 6e69 6e67 2073 7563 6365 7373 6675  tuning successfu
+00000ba0: 6c2e 2901 5a04 6178 6973 7a16 5072 6564  l.).Z.axisz.Pred
+00000bb0: 6963 7469 6e67 2073 7563 6365 7373 6675  icting successfu
+00000bc0: 6c2e 2901 fa02 3d3d 2901 7a6b 2528 7079  l.)...==).zk%(py
+00000bd0: 3329 730a 7b25 2870 7933 2973 203d 2025  3)s.{%(py3)s = %
+00000be0: 2870 7930 2973 2825 2870 7931 2973 290a  (py0)s(%(py1)s).
+00000bf0: 7d20 3d3d 2025 2870 7931 3029 730a 7b25  } == %(py10)s.{%
+00000c00: 2870 7931 3029 7320 3d20 2528 7079 3529  (py10)s = %(py5)
+00000c10: 7328 2528 7079 3829 730a 7b25 2870 7938  s(%(py8)s.{%(py8
+00000c20: 2973 203d 2025 2870 7936 2973 2e69 6e64  )s = %(py6)s.ind
+00000c30: 6578 0a7d 290a 7dda 036c 656e da07 795f  ex.}).}..len..y_
+00000c40: 7072 6f62 7372 1800 0000 2907 da03 7079  probsr....)...py
+00000c50: 30da 0370 7931 5a03 7079 335a 0370 7935  0..py1Z.py3Z.py5
+00000c60: da03 7079 365a 0370 7938 5a04 7079 3130  ..py6Z.py8Z.py10
+00000c70: 7a0f 6173 7365 7274 2025 2870 7931 3229  z.assert %(py12)
+00000c80: 735a 0470 7931 324e da09 795f 636c 6173  sZ.py12N..y_clas
+00000c90: 7365 7329 1772 0c00 0000 5a09 7374 6570  ses).r....Z.step
+00000ca0: 735f 6d61 785a 0e6e 756d 5f6c 6561 7665  s_maxZ.num_leave
+00000cb0: 735f 6d61 7872 0b00 0000 da1c 6879 7065  s_maxr......hype
+00000cc0: 7270 6172 616d 6574 6572 5f74 756e 696e  rparameter_tunin
+00000cd0: 675f 726f 756e 6473 da18 656e 6162 6c65  g_rounds..enable
+00000ce0: 5f66 6561 7475 7265 5f73 656c 6563 7469  _feature_selecti
+00000cf0: 6f6e da14 6879 7065 7274 756e 696e 675f  on..hypertuning_
+00000d00: 6376 5f66 6f6c 6473 7210 0000 0072 0900  cv_foldsr....r..
+00000d10: 0000 da03 6669 74da 0570 7269 6e74 da07  ....fit..print..
+00000d20: 7072 6564 6963 745a 0464 726f 7072 3900  predictZ.dropr9.
+00000d30: 0000 da05 696e 6465 78da 0a40 7079 7465  ....index..@pyte
+00000d40: 7374 5f61 72da 115f 6361 6c6c 5f72 6570  st_ar.._call_rep
+00000d50: 7263 6f6d 7061 7265 da0c 4070 795f 6275  rcompare..@py_bu
+00000d60: 696c 7469 6e73 da06 6c6f 6361 6c73 da18  iltins..locals..
+00000d70: 5f73 686f 756c 645f 7265 7072 5f67 6c6f  _should_repr_glo
+00000d80: 6261 6c5f 6e61 6d65 da09 5f73 6166 6572  bal_name.._safer
+00000d90: 6570 72da 0e41 7373 6572 7469 6f6e 4572  epr..AssertionEr
+00000da0: 726f 72da 135f 666f 726d 6174 5f65 7870  ror.._format_exp
+00000db0: 6c61 6e61 7469 6f6e 2910 721b 0000 0072  lanation).r....r
+00000dc0: 1700 0000 7218 0000 005a 1478 6762 6f6f  ....r....Z.xgboo
+00000dd0: 7374 5f70 6172 616d 5f63 6f6e 6669 67da  st_param_config.
+00000de0: 0c74 7261 696e 5f63 6f6e 6669 6772 3200  .train_configr2.
+00000df0: 0000 7237 0000 005a 0661 7574 6f6d 6c72  ..r7...Z.automlr
+00000e00: 3a00 0000 723e 0000 005a 0b40 7079 5f61  :...r>...Z.@py_a
+00000e10: 7373 6572 7432 5a0b 4070 795f 6173 7365  ssert2Z.@py_asse
+00000e20: 7274 375a 0b40 7079 5f61 7373 6572 7439  rt7Z.@py_assert9
+00000e30: 5a0b 4070 795f 6173 7365 7274 345a 0c40  Z.@py_assert4Z.@
+00000e40: 7079 5f66 6f72 6d61 7431 315a 0c40 7079  py_format11Z.@py
+00000e50: 5f66 6f72 6d61 7431 3372 1900 0000 7219  _format13r....r.
+00000e60: 0000 0072 1a00 0000 da16 7465 7374 5f62  ...r......test_b
+00000e70: 6c75 6570 7269 6e74 5f78 6762 6f6f 7374  lueprint_xgboost
+00000e80: 2200 0000 7334 0000 0008 0208 0106 0106  "...s4..........
+00000e90: 0106 0106 0106 0106 0106 0110 0306 1a02  ................
+00000ea0: 0202 0102 0102 0102 0102 0106 fb0e 0708  ................
+00000eb0: 0118 0108 01fe 010a 00fe 011c 0072 4f00  .............rO.
+00000ec0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000ed0: 0000 000a 0000 0040 0000 0073 5600 0000  .......@...sV...
+00000ee0: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
+00000ef0: 6403 6504 6a05 6404 6504 6a05 6405 6504  d.e.j.d.e.j.d.e.
+00000f00: 6a06 6406 6504 6a06 6407 6408 660a 6409  j.d.e.j.d.d.f.d.
+00000f10: 640a 8404 5a07 640b 6504 6a05 6407 6508  d...Z.d.e.j.d.e.
+00000f20: 6509 650a 6602 1900 6604 640c 640d 8404  e.e.f...f.d.d...
+00000f30: 5a0b 6408 5300 290e da0b 4375 7374 6f6d  Z.d.S.)...Custom
+00000f40: 4d6f 6465 6c63 0100 0000 0000 0000 0000  Modelc..........
+00000f50: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
+00000f60: 0000 0064 007c 005f 0064 0053 00a9 014e  ...d.|._.d.S...N
+00000f70: 2901 da05 6d6f 6465 6c29 0172 2300 0000  )...model).r#...
+00000f80: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+00000f90: 085f 5f69 6e69 745f 5f5b 0000 0073 0200  .__init__[...s..
+00000fa0: 0000 0a01 7a14 4375 7374 6f6d 4d6f 6465  ....z.CustomMode
+00000fb0: 6c2e 5f5f 696e 6974 5f5f da07 785f 7472  l.__init__..x_tr
+00000fc0: 6169 6eda 0678 5f74 6573 74da 0779 5f74  ain..x_test..y_t
+00000fd0: 7261 696e da06 795f 7465 7374 7213 0000  rain..y_testr...
+00000fe0: 004e 6305 0000 0000 0000 0000 0000 0005  .Nc.............
+00000ff0: 0000 0004 0000 0043 0000 0073 1a00 0000  .......C...s....
+00001000: 7400 8300 7c00 5f01 7c00 6a01 a002 7c01  t...|._.|.j...|.
+00001010: 7c03 a102 0100 6400 5300 7251 0000 0029  |.....d.S.rQ...)
+00001020: 0372 0400 0000 7252 0000 0072 4200 0000  .r....rR...rB...
+00001030: 2905 7223 0000 0072 5400 0000 7255 0000  ).r#...rT...rU..
+00001040: 0072 5600 0000 7257 0000 0072 1900 0000  .rV...rW...r....
+00001050: 7219 0000 0072 1a00 0000 7242 0000 005e  r....r....rB...^
+00001060: 0000 0073 0400 0000 0807 1201 7a0f 4375  ...s........z.Cu
+00001070: 7374 6f6d 4d6f 6465 6c2e 6669 7472 2100  stomModel.fitr!.
+00001080: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
+00001090: 0000 0003 0000 0043 0000 0073 2000 0000  .......C...s ...
+000010a0: 7c00 6a00 a001 7c01 a101 7d02 7c00 6a00  |.j...|...}.|.j.
+000010b0: a002 7c01 a101 7d03 7c02 7c03 6602 5300  ..|...}.|.|.f.S.
+000010c0: 7251 0000 0029 0372 5200 0000 5a0d 7072  rQ...).rR...Z.pr
+000010d0: 6564 6963 745f 7072 6f62 6172 4400 0000  edict_probarD...
+000010e0: 2904 7223 0000 0072 2100 0000 da10 7072  ).r#...r!.....pr
+000010f0: 6564 6963 7465 645f 7072 6f62 6173 da11  edicted_probas..
+00001100: 7072 6564 6963 7465 645f 636c 6173 7365  predicted_classe
+00001110: 7372 1900 0000 7219 0000 0072 1a00 0000  sr....r....r....
+00001120: 7244 0000 0068 0000 0073 0600 0000 0c01  rD...h...s......
+00001130: 0c01 0801 7a13 4375 7374 6f6d 4d6f 6465  ....z.CustomMode
+00001140: 6c2e 7072 6564 6963 7429 0c72 2d00 0000  l.predict).r-...
+00001150: 722e 0000 0072 2f00 0000 7253 0000 0072  r....r/...rS...r
+00001160: 2a00 0000 7230 0000 0072 2b00 0000 7242  *...r0...r+...rB
+00001170: 0000 0072 0300 0000 720f 0000 0072 0e00  ...r....r....r..
+00001180: 0000 7244 0000 0072 1900 0000 7219 0000  ..rD...r....r...
+00001190: 0072 1900 0000 721a 0000 0072 5000 0000  .r....r....rP...
+000011a0: 5a00 0000 731c 0000 0008 0008 0102 0304  Z...s...........
+000011b0: 0202 fe04 0302 fd04 0402 fc04 0502 fb02  ................
+000011c0: 060a fa20 0a72 5000 0000 6300 0000 0000  ... .rP...c.....
+000011d0: 0000 0000 0000 000c 0000 000a 0000 0043  ...............C
+000011e0: 0000 0073 ce02 0000 7400 8300 7d00 7401  ...s....t...}.t.
+000011f0: 8300 7d01 6401 7c01 5f02 6402 7c01 5f03  ..}.d.|._.d.|._.
+00001200: 6403 7c01 5f04 7405 8300 7d02 7406 7407  d.|._.t...}.t.t.
+00001210: a008 a100 6404 7409 6403 6405 6402 6406  ....d.t.d.d.d.d.
+00001220: 8d03 6404 740a 740b 8301 6404 6407 8d06  ..d.t.t...d.d...
+00001230: 7c02 5f0c 740d 6408 6409 7c00 7c01 7c02  |._.t.d.d.|.|.|.
+00001240: 640a 8d05 7d03 740e a00f 640b 640c 8400  d...}.t...d.d...
+00001250: 7410 6401 8301 4400 8301 640d 640c 8400  t.d...D...d.d...
+00001260: 7410 6401 8301 4400 8301 640e 640c 8400  t.d...D...d.d...
+00001270: 7410 6401 8301 4400 8301 640f 640c 8400  t.d...D...d.d...
+00001280: 7410 6401 8301 4400 8301 6410 640c 8400  t.d...D...d.d...
+00001290: 7410 6401 8301 4400 8301 6411 640c 8400  t.d...D...d.d...
+000012a0: 7410 6401 8301 4400 8301 6412 9c06 a101  t.d...D...d.....
+000012b0: 7d04 740e a011 6700 6413 a201 a101 7d05  }.t...g.d.....}.
+000012c0: 740e a00f 6414 640c 8400 7410 6401 8301  t...d.d...t.d...
+000012d0: 4400 8301 6415 640c 8400 7410 6401 8301  D...d.d...t.d...
+000012e0: 4400 8301 6416 640c 8400 7410 6401 8301  D...d.d...t.d...
+000012f0: 4400 8301 6417 640c 8400 7410 6401 8301  D...d.d...t.d...
+00001300: 4400 8301 6418 640c 8400 7410 6401 8301  D...d.d...t.d...
+00001310: 4400 8301 6419 640c 8400 7410 6401 8301  D...d.d...t.d...
+00001320: 4400 8301 6412 9c06 a101 7d06 7c05 7c04  D...d.....}.|.|.
+00001330: 6409 3c00 7c03 a012 7c04 6409 a102 0100  d.<.|...|.d.....
+00001340: 7c03 a013 7c06 a101 5c02 7d07 7d08 7414  |...|...\.}.}.t.
+00001350: 6a15 7d09 7416 7c07 7c09 8302 7d0a 7c0a  j.}.t.|.|...}.|.
+00001360: 9001 7305 641a 641b 7417 a018 a100 7600  ..s.d.d.t.....v.
+00001370: 73ca 7419 a01a 7416 a101 72cf 7419 a01b  s.t...t...r.t...
+00001380: 7416 a101 6e01 641b 641c 7417 a018 a100  t...n.d.d.t.....
+00001390: 7600 73db 7419 a01a 7c07 a101 72e0 7419  v.s.t...|...r.t.
+000013a0: a01b 7c07 a101 6e01 641c 641d 7417 a018  ..|...n.d.d.t...
+000013b0: a100 7600 73ec 7419 a01a 7414 a101 72f1  ..v.s.t...t...r.
+000013c0: 7419 a01b 7414 a101 6e01 641d 7419 a01b  t...t...n.d.t...
+000013d0: 7c09 a101 7419 a01b 7c0a a101 641e 9c05  |...t...|...d...
+000013e0: 1600 7d0b 741c 7419 a01d 7c0b a101 8301  ..}.t.t...|.....
+000013f0: 8201 6400 0400 7d09 7d0a 7414 6a15 7d09  ..d...}.}.t.j.}.
+00001400: 7416 7c08 7c09 8302 7d0a 7c0a 9001 7361  t.|.|...}.|...sa
+00001410: 641a 641b 7417 a018 a100 7600 9001 7322  d.d.t.....v...s"
+00001420: 7419 a01a 7416 a101 9001 7227 7419 a01b  t...t.....r't...
+00001430: 7416 a101 6e01 641b 641f 7417 a018 a100  t...n.d.d.t.....
+00001440: 7600 9001 7335 7419 a01a 7c08 a101 9001  v...s5t...|.....
+00001450: 723a 7419 a01b 7c08 a101 6e01 641f 641d  r:t...|...n.d.d.
+00001460: 7417 a018 a100 7600 9001 7348 7419 a01a  t.....v...sHt...
+00001470: 7414 a101 9001 724d 7419 a01b 7414 a101  t.....rMt...t...
+00001480: 6e01 641d 7419 a01b 7c09 a101 7419 a01b  n.d.t...|...t...
+00001490: 7c0a a101 641e 9c05 1600 7d0b 741c 7419  |...d.....}.t.t.
+000014a0: a01d 7c0b a101 8301 8201 6400 0400 7d09  ..|.......d...}.
+000014b0: 7d0a 6400 5300 2920 4e72 1f00 0000 5472  }.d.S.) Nr....Tr
+000014c0: 2000 0000 721c 0000 0072 0100 0000 2902   ...r....r....).
+000014d0: 7215 0000 00da 0773 6875 6666 6c65 2906  r......shuffle).
+000014e0: 5a09 6573 7469 6d61 746f 72da 0473 7465  Z.estimator..ste
+000014f0: 705a 0263 765a 166d 696e 5f66 6561 7475  pZ.cvZ.min_featu
+00001500: 7265 735f 746f 5f73 656c 6563 745a 0773  res_to_selectZ.s
+00001510: 636f 7269 6e67 5a06 6e5f 6a6f 6273 7233  coringZ.n_jobsr3
+00001520: 0000 0072 2500 0000 2905 7234 0000 0072  ...r%...).r4...r
+00001530: 3500 0000 5a08 6d6c 5f6d 6f64 656c 7236  5...Z.ml_modelr6
+00001540: 0000 005a 1663 6f6e 665f 6665 6174 7572  ...Z.conf_featur
+00001550: 655f 7365 6c65 6374 696f 6e63 0100 0000  e_selectionc....
+00001560: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00001570: 5300 0000 f310 0000 0067 007c 005d 047d  S........g.|.].}
+00001580: 017c 0191 0271 0253 0072 1900 0000 7219  .|...q.S.r....r.
+00001590: 0000 00a9 02da 022e 30da 0169 7219 0000  ........0..ir...
+000015a0: 0072 1900 0000 721a 0000 00da 0a3c 6c69  .r....r......<li
+000015b0: 7374 636f 6d70 3e8e 0000 00f3 0200 0000  stcomp>.........
+000015c0: 1000 7a33 7465 7374 5f62 6c75 6563 6173  ..z3test_bluecas
+000015d0: 745f 7769 7468 5f63 7573 746f 6d5f 6d6f  t_with_custom_mo
+000015e0: 6465 6c2e 3c6c 6f63 616c 733e 2e3c 6c69  del.<locals>.<li
+000015f0: 7374 636f 6d70 3e63 0100 0000 0000 0000  stcomp>c........
+00001600: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+00001610: 725c 0000 0072 1900 0000 7219 0000 0072  r\...r....r....r
+00001620: 5d00 0000 7219 0000 0072 1900 0000 721a  ]...r....r....r.
+00001630: 0000 0072 6000 0000 8f00 0000 7261 0000  ...r`.......ra..
+00001640: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00001650: 0000 0300 0000 5300 0000 725c 0000 0072  ......S...r\...r
+00001660: 1900 0000 7219 0000 0072 5d00 0000 7219  ....r....r]...r.
+00001670: 0000 0072 1900 0000 721a 0000 0072 6000  ...r....r....r`.
+00001680: 0000 9000 0000 7261 0000 0063 0100 0000  ......ra...c....
+00001690: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000016a0: 5300 0000 725c 0000 0072 1900 0000 7219  S...r\...r....r.
+000016b0: 0000 0072 5d00 0000 7219 0000 0072 1900  ...r]...r....r..
+000016c0: 0000 721a 0000 0072 6000 0000 9100 0000  ..r....r`.......
+000016d0: 7261 0000 0063 0100 0000 0000 0000 0000  ra...c..........
+000016e0: 0000 0200 0000 0300 0000 5300 0000 725c  ..........S...r\
+000016f0: 0000 0072 1900 0000 7219 0000 0072 5d00  ...r....r....r].
+00001700: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
+00001710: 0072 6000 0000 9200 0000 7261 0000 0063  .r`.......ra...c
+00001720: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001730: 0300 0000 5300 0000 725c 0000 0072 1900  ....S...r\...r..
+00001740: 0000 7219 0000 0072 5d00 0000 7219 0000  ..r....r]...r...
+00001750: 0072 1900 0000 721a 0000 0072 6000 0000  .r....r....r`...
+00001760: 9300 0000 7261 0000 0029 065a 0866 6561  ....ra...).Z.fea
+00001770: 7475 7265 315a 0866 6561 7475 7265 325a  ture1Z.feature2Z
+00001780: 0866 6561 7475 7265 335a 0866 6561 7475  .feature3Z.featu
+00001790: 7265 345a 0866 6561 7475 7265 355a 0866  re4Z.feature5Z.f
+000017a0: 6561 7475 7265 3629 0a72 0100 0000 721c  eature6).r....r.
+000017b0: 0000 0072 0100 0000 721c 0000 0072 0100  ...r....r....r..
+000017c0: 0000 721c 0000 0072 0100 0000 721c 0000  ..r....r....r...
+000017d0: 0072 0100 0000 721c 0000 0063 0100 0000  .r....r....c....
+000017e0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000017f0: 5300 0000 725c 0000 0072 1900 0000 7219  S...r\...r....r.
+00001800: 0000 0072 5d00 0000 7219 0000 0072 1900  ...r]...r....r..
+00001810: 0000 721a 0000 0072 6000 0000 9900 0000  ..r....r`.......
+00001820: 7261 0000 0063 0100 0000 0000 0000 0000  ra...c..........
+00001830: 0000 0200 0000 0300 0000 5300 0000 725c  ..........S...r\
+00001840: 0000 0072 1900 0000 7219 0000 0072 5d00  ...r....r....r].
+00001850: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
+00001860: 0072 6000 0000 9a00 0000 7261 0000 0063  .r`.......ra...c
+00001870: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001880: 0300 0000 5300 0000 725c 0000 0072 1900  ....S...r\...r..
+00001890: 0000 7219 0000 0072 5d00 0000 7219 0000  ..r....r]...r...
+000018a0: 0072 1900 0000 721a 0000 0072 6000 0000  .r....r....r`...
+000018b0: 9b00 0000 7261 0000 0063 0100 0000 0000  ....ra...c......
+000018c0: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
+000018d0: 0000 725c 0000 0072 1900 0000 7219 0000  ..r\...r....r...
+000018e0: 0072 5d00 0000 7219 0000 0072 1900 0000  .r]...r....r....
+000018f0: 721a 0000 0072 6000 0000 9c00 0000 7261  r....r`.......ra
+00001900: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001910: 0200 0000 0300 0000 5300 0000 725c 0000  ........S...r\..
+00001920: 0072 1900 0000 7219 0000 0072 5d00 0000  .r....r....r]...
+00001930: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00001940: 6000 0000 9d00 0000 7261 0000 0063 0100  `.......ra...c..
+00001950: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00001960: 0000 5300 0000 725c 0000 0072 1900 0000  ..S...r\...r....
+00001970: 7219 0000 0072 5d00 0000 7219 0000 0072  r....r]...r....r
+00001980: 1900 0000 721a 0000 0072 6000 0000 9e00  ....r....r`.....
+00001990: 0000 7261 0000 007a 5261 7373 6572 7420  ..ra...zRassert 
+000019a0: 2528 7079 3629 730a 7b25 2870 7936 2973  %(py6)s.{%(py6)s
+000019b0: 203d 2025 2870 7930 2973 2825 2870 7931   = %(py0)s(%(py1
+000019c0: 2973 2c20 2528 7079 3429 730a 7b25 2870  )s, %(py4)s.{%(p
+000019d0: 7934 2973 203d 2025 2870 7932 2973 2e6e  y4)s = %(py2)s.n
+000019e0: 6461 7272 6179 0a7d 290a 7d72 2900 0000  darray.}).}r)...
+000019f0: 7258 0000 00da 026e 7029 0572 3b00 0000  rX.....np).r;...
+00001a00: 723c 0000 005a 0370 7932 5a03 7079 3472  r<...Z.py2Z.py4r
+00001a10: 3d00 0000 7259 0000 0029 1e72 5000 0000  =...rY...).rP...
+00001a20: 720b 0000 0072 3f00 0000 7240 0000 0072  r....r?...r@...r
+00001a30: 4100 0000 720a 0000 0072 0500 0000 da03  A...r....r......
+00001a40: 7867 625a 0d58 4742 436c 6173 7369 6669  xgbZ.XGBClassifi
+00001a50: 6572 7208 0000 0072 0600 0000 7207 0000  err....r....r...
+00001a60: 005a 1273 656c 6563 7469 6f6e 5f73 7472  .Z.selection_str
+00001a70: 6174 6567 7972 0900 0000 722a 0000 0072  ategyr....r*...r
+00001a80: 3000 0000 da05 7261 6e67 6572 2b00 0000  0.....ranger+...
+00001a90: 7242 0000 0072 4400 0000 7262 0000 00da  rB...rD...rb....
+00001aa0: 076e 6461 7272 6179 7229 0000 0072 4800  .ndarrayr)...rH.
+00001ab0: 0000 7249 0000 0072 4600 0000 724a 0000  ..rI...rF...rJ..
+00001ac0: 0072 4b00 0000 724c 0000 0072 4d00 0000  .rK...rL...rM...
+00001ad0: 290c 5a0c 6375 7374 6f6d 5f6d 6f64 656c  ).Z.custom_model
+00001ae0: 724e 0000 005a 0f63 7573 746f 6d5f 6665  rN...Z.custom_fe
+00001af0: 6174 5f73 656c da08 626c 7565 6361 7374  at_sel..bluecast
+00001b00: 7254 0000 0072 5600 0000 7255 0000 0072  rT...rV...rU...r
+00001b10: 5800 0000 7259 0000 005a 0b40 7079 5f61  X...rY...Z.@py_a
+00001b20: 7373 6572 7433 5a0b 4070 795f 6173 7365  ssert3Z.@py_asse
+00001b30: 7274 355a 0b40 7079 5f66 6f72 6d61 7437  rt5Z.@py_format7
+00001b40: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+00001b50: 1f74 6573 745f 626c 7565 6361 7374 5f77  .test_bluecast_w
+00001b60: 6974 685f 6375 7374 6f6d 5f6d 6f64 656c  ith_custom_model
+00001b70: 6e00 0000 735a 0000 0006 0206 0106 0106  n...sZ..........
+00001b80: 0106 0106 0302 0206 0102 010c 0102 0106  ................
+00001b90: 0102 0108 fa02 0a02 0102 0102 0102 0102  ................
+00001ba0: 0106 fb04 0910 0210 0110 0110 0110 0110  ................
+00001bb0: 0104 fa04 ff0e 0a04 0110 0210 0110 0110  ................
+00001bc0: 0110 0110 0104 fa04 ff08 0b0c 030e 03ac  ................
+00001bd0: 03bc 0172 6700 0000 292d da08 6275 696c  ...rg...)-..buil
+00001be0: 7469 6e73 7248 0000 00da 195f 7079 7465  tinsrH....._pyte
+00001bf0: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
+00001c00: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
+00001c10: 0772 6577 7269 7465 7246 0000 00da 0674  .rewriterF.....t
+00001c20: 7970 696e 6772 0200 0000 7203 0000 00da  ypingr....r.....
+00001c30: 056e 756d 7079 7262 0000 005a 0670 616e  .numpyrb...Z.pan
+00001c40: 6461 7372 2a00 0000 da06 7079 7465 7374  dasr*.....pytest
+00001c50: 5a10 736b 6c65 6172 6e2e 656e 7365 6d62  Z.sklearn.ensemb
+00001c60: 6c65 7204 0000 005a 1973 6b6c 6561 726e  ler....Z.sklearn
+00001c70: 2e66 6561 7475 7265 5f73 656c 6563 7469  .feature_selecti
+00001c80: 6f6e 7205 0000 005a 0f73 6b6c 6561 726e  onr....Z.sklearn
+00001c90: 2e6d 6574 7269 6373 7206 0000 0072 0700  .metricsr....r..
+00001ca0: 0000 5a17 736b 6c65 6172 6e2e 6d6f 6465  ..Z.sklearn.mode
+00001cb0: 6c5f 7365 6c65 6374 696f 6e72 0800 0000  l_selectionr....
+00001cc0: 5a07 7867 626f 6f73 7472 6300 0000 5a18  Z.xgboostrc...Z.
+00001cd0: 626c 7565 6361 7374 2e62 6c75 6570 7269  bluecast.bluepri
+00001ce0: 6e74 732e 6361 7374 7209 0000 005a 1f62  nts.castr....Z.b
+00001cf0: 6c75 6563 6173 742e 636f 6e66 6967 2e74  luecast.config.t
+00001d00: 7261 696e 696e 675f 636f 6e66 6967 720a  raining_configr.
+00001d10: 0000 0072 0b00 0000 720c 0000 005a 2262  ...r....r....Z"b
+00001d20: 6c75 6563 6173 742e 6d6c 5f6d 6f64 656c  luecast.ml_model
+00001d30: 6c69 6e67 2e62 6173 655f 636c 6173 7365  ling.base_classe
+00001d40: 7372 0d00 0000 720e 0000 0072 0f00 0000  sr....r....r....
+00001d50: 5a1d 626c 7565 6361 7374 2e70 7265 7072  Z.bluecast.prepr
+00001d60: 6f63 6573 7369 6e67 2e63 7573 746f 6d72  ocessing.customr
+00001d70: 1000 0000 5a24 626c 7565 6361 7374 2e74  ....Z$bluecast.t
+00001d80: 6573 7473 2e6d 616b 655f 6461 7461 2e63  ests.make_data.c
+00001d90: 7265 6174 655f 6461 7461 7212 0000 00da  reate_datar.....
+00001da0: 0766 6978 7475 7265 7230 0000 0072 1b00  .fixturer0...r..
+00001db0: 0000 724f 0000 0072 5000 0000 7267 0000  ..rO...rP...rg..
+00001dc0: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
+00001dd0: 721a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00001de0: 0000 0073 2600 0000 2a00 0802 0801 0801  ...s&...*.......
+00001df0: 0c01 0c01 1001 0c01 0801 0c02 1401 1405  ................
+00001e00: 0c05 0c01 0403 1c01 0806 1038 0c14       ...........8..
```

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 12:36:14 2023 UTC, .py size: 2204 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 be1c 8364 9c08 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 eb11 9764 f708 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6401 6c08 5a09 6400 6401  Z...d.d.l.Z.d.d.
 00000060: 6c0a 5a0b 6400 6401 6c0c 5a0c 6400 6403  l.Z.d.d.l.Z.d.d.
 00000070: 6c0d 6d0e 5a0e 0100 6400 6404 6c0f 6d10  l.m.Z...d.d.l.m.
@@ -33,218 +33,222 @@
 00000200: 7079 da0a 6d6f 636b 5f6d 6f64 656c 0e00  py..mock_model..
 00000210: 0000 7302 0000 0008 0272 0b00 0000 6300  ..s......r....c.
 00000220: 0000 0000 0000 0000 0000 0000 0000 0005  ................
 00000230: 0000 0043 0000 0073 1800 0000 7400 a001  ...C...s....t...
 00000240: 6700 6401 a201 6700 6402 a201 6403 9c02  g.d...g.d...d...
 00000250: a101 5300 2904 4e29 03e9 0100 0000 e902  ..S.).N)........
 00000260: 0000 00e9 0300 0000 2903 e904 0000 00e9  ........).......
-00000270: 0500 0000 e906 0000 0029 025a 0866 6561  .........).Z.fea
-00000280: 7475 7265 315a 0866 6561 7475 7265 3229  ture1Z.feature2)
+00000270: 0500 0000 e906 0000 0029 02da 0866 6561  .........)...fea
+00000280: 7475 7265 31da 0866 6561 7475 7265 3229  ture1..feature2)
 00000290: 02da 0270 64da 0944 6174 6146 7261 6d65  ...pd..DataFrame
 000002a0: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
 000002b0: 0a00 0000 da09 7465 7374 5f64 6174 6113  ......test_data.
-000002c0: 0000 0073 0200 0000 1802 7214 0000 0063  ...s......r....c
+000002c0: 0000 0073 0200 0000 1802 7216 0000 0063  ...s......r....c
 000002d0: 0000 0000 0000 0000 0000 0000 0800 0000  ................
-000002e0: 0700 0000 4300 0000 730a 0100 0074 0064  ....C...s....t.d
+000002e0: 0700 0000 4300 0000 7316 0100 0074 0064  ....C...s....t.d
 000002f0: 0164 0264 038d 027d 0074 0064 0464 0564  .d.d...}.t.d.d.d
 00000300: 038d 027d 0174 0183 007d 0264 047c 025f  ...}.t...}.d.|._
 00000310: 0264 067c 025f 0374 0483 007d 0364 077c  .d.|._.t...}.d.|
-00000320: 035f 0574 0664 0864 097c 037c 0264 0a8d  ._.t.d.d.|.|.d..
-00000330: 047d 047c 046a 077c 007c 016a 0864 0964  .}.|.j.|.|.j.d.d
-00000340: 0b64 0c8d 027c 0164 0919 0064 0964 0d8d  .d...|.d...d.d..
-00000350: 047d 0574 097c 0583 0101 0074 0a7c 0574  .}.t.|.....t.|.t
-00000360: 0b83 027d 067c 0673 8164 0e64 0f74 0ca0  ...}.|.s.d.d.t..
-00000370: 0da1 0076 0073 4a74 0ea0 0f74 0aa1 0172  ...v.sJt...t...r
-00000380: 4f74 0ea0 1074 0aa1 016e 0164 0f64 1074  Ot...t...n.d.d.t
-00000390: 0ca0 0da1 0076 0073 5b74 0ea0 0f7c 05a1  .....v.s[t...|..
-000003a0: 0172 6074 0ea0 107c 05a1 016e 0164 1064  .r`t...|...n.d.d
-000003b0: 1174 0ca0 0da1 0076 0073 6c74 0ea0 0f74  .t.....v.slt...t
-000003c0: 0ba1 0172 7174 0ea0 1074 0ba1 016e 0164  ...rqt...t...n.d
-000003d0: 1174 0ea0 107c 06a1 0164 129c 0416 007d  .t...|...d.....}
-000003e0: 0774 1174 0ea0 127c 07a1 0183 0182 0164  .t.t...|.......d
-000003f0: 137d 0664 1353 0029 147a 2254 6573 7420  .}.d.S.).z"Test 
-00000400: 7468 6174 2074 6573 7473 2074 6865 2042  that tests the B
-00000410: 6c75 6543 6173 7420 636c 6173 73e9 c800  lueCast class...
-00000420: 0000 e914 0000 0029 01da 0c72 616e 646f  .......)...rando
-00000430: 6d5f 7374 6174 65e9 6400 0000 e915 0000  m_state.d.......
-00000440: 00e9 1000 0000 e90a 0000 00da 0662 696e  .............bin
-00000450: 6172 79da 0674 6172 6765 7429 04da 0d63  ary..target)...c
-00000460: 6c61 7373 5f70 726f 626c 656d da0d 7461  lass_problem..ta
-00000470: 7267 6574 5f63 6f6c 756d 6eda 0d63 6f6e  rget_column..con
-00000480: 665f 7472 6169 6e69 6e67 da0c 636f 6e66  f_training..conf
-00000490: 5f78 6762 6f6f 7374 720c 0000 0029 01da  _xgboostr....)..
-000004a0: 0461 7869 7329 01da 0a74 6172 6765 745f  .axis)...target_
-000004b0: 636f 6c7a 3561 7373 6572 7420 2528 7079  colz5assert %(py
-000004c0: 3429 730a 7b25 2870 7934 2973 203d 2025  4)s.{%(py4)s = %
-000004d0: 2870 7930 2973 2825 2870 7931 2973 2c20  (py0)s(%(py1)s, 
-000004e0: 2528 7079 3229 7329 0a7d da0a 6973 696e  %(py2)s).}..isin
-000004f0: 7374 616e 6365 da09 6576 616c 5f64 6963  stance..eval_dic
-00000500: 74da 0464 6963 7429 04da 0370 7930 da03  t..dict)...py0..
-00000510: 7079 31da 0370 7932 da03 7079 344e 2913  py1..py2..py4N).
-00000520: 7208 0000 0072 0500 0000 da09 7374 6570  r....r......step
-00000530: 735f 6d61 78da 0e6e 756d 5f6c 6561 7665  s_max..num_leave
-00000540: 735f 6d61 7872 0400 0000 da1c 6879 7065  s_maxr......hype
-00000550: 7270 6172 616d 6574 6572 5f74 756e 696e  rparameter_tunin
-00000560: 675f 726f 756e 6473 7203 0000 00da 0866  g_roundsr......f
-00000570: 6974 5f65 7661 6cda 0464 726f 70da 0570  it_eval..drop..p
-00000580: 7269 6e74 7224 0000 0072 2600 0000 da0c  rintr$...r&.....
-00000590: 4070 795f 6275 696c 7469 6e73 da06 6c6f  @py_builtins..lo
-000005a0: 6361 6c73 da0a 4070 7974 6573 745f 6172  cals..@pytest_ar
-000005b0: da18 5f73 686f 756c 645f 7265 7072 5f67  .._should_repr_g
-000005c0: 6c6f 6261 6c5f 6e61 6d65 da09 5f73 6166  lobal_name.._saf
-000005d0: 6572 6570 72da 0e41 7373 6572 7469 6f6e  erepr..Assertion
-000005e0: 4572 726f 72da 135f 666f 726d 6174 5f65  Error.._format_e
-000005f0: 7870 6c61 6e61 7469 6f6e 2908 da08 6466  xplanation)...df
-00000600: 5f74 7261 696e da06 6466 5f76 616c da14  _train..df_val..
-00000610: 7867 626f 6f73 745f 7061 7261 6d5f 636f  xgboost_param_co
-00000620: 6e66 6967 da0c 7472 6169 6e5f 636f 6e66  nfig..train_conf
-00000630: 6967 da06 6175 746f 6d6c 7225 0000 00da  ig..automlr%....
-00000640: 0b40 7079 5f61 7373 6572 7433 da0b 4070  .@py_assert3..@p
-00000650: 795f 666f 726d 6174 3572 0900 0000 7209  y_format5r....r.
-00000660: 0000 0072 0a00 0000 da16 7465 7374 5f73  ...r......test_s
-00000670: 6861 705f 6578 706c 616e 6174 696f 6e73  hap_explanations
-00000680: 1800 0000 7324 0000 000c 020c 0106 0106  ....s$..........
-00000690: 0106 0106 0106 0102 0202 0102 0102 0102  ................
-000006a0: 0106 fc04 0616 0106 ff08 039c 0172 3f00  .............r?.
-000006b0: 0000 6302 0000 0000 0000 0000 0000 0013  ..c.............
-000006c0: 0000 0009 0000 0043 0000 0073 ee01 0000  .......C...s....
-000006d0: 6401 7d02 7400 a001 6402 a101 8fe6 7d03  d.}.t...d.....}.
-000006e0: 7400 a001 6403 a101 8fc8 7d04 7402 a003  t...d.....}.t...
-000006f0: 6404 6405 6702 6406 6407 6702 6408 6409  d.d.g.d.d.g.d.d.
-00000700: 6702 6703 a101 7c03 6a04 6a05 5f04 7406  g.g...|.j.j._.t.
-00000710: 7c00 7c01 7c02 8303 7d05 7c03 a007 7c00  |.|.|...}.|...|.
-00000720: 6a08 7c01 a102 0100 7c04 a009 a100 0100  j.|.....|.......
-00000730: 6700 7d06 6400 7d07 7c05 7c07 7501 7d08  g.}.d.}.|.|.u.}.
-00000740: 7c08 7d09 7c08 7247 7c05 6a0a 7d0a 640a  |.}.|.rG|.j.}.d.
-00000750: 7d0b 7c0a 7c0b 6b04 7d0c 7c0c 7d09 7c09  }.|.|.k.}.|.}.|.
-00000760: 73c0 740b a00c 640b 7c08 6601 640c 7c05  s.t...d.|.f.d.|.
-00000770: 7c07 6602 a104 640d 740d a00e a100 7600  |.f...d.t.....v.
-00000780: 735e 740b a00f 7c05 a101 7263 740b a010  s^t...|...rct...
-00000790: 7c05 a101 6e01 640d 740b a010 7c07 a101  |...n.d.t...|...
-000007a0: 640e 9c02 1600 7d0d 640f 6410 7c0d 6901  d.....}.d.d.|.i.
-000007b0: 1600 7d0e 7c06 a011 7c0e a101 0100 7c08  ..}.|...|.....|.
-000007c0: 72ab 740b a00c 6411 7c0c 6601 6412 7c0a  r.t...d.|.f.d.|.
-000007d0: 7c0b 6602 a104 640d 740d a00e a100 7600  |.f...d.t.....v.
-000007e0: 738e 740b a00f 7c05 a101 7293 740b a010  s.t...|...r.t...
-000007f0: 7c05 a101 6e01 640d 740b a010 7c0a a101  |...n.d.t...|...
-00000800: 740b a010 7c0b a101 6413 9c03 1600 7d0f  t...|...d.....}.
-00000810: 6414 6415 7c0f 6901 1600 7d10 7c06 a011  d.d.|.i...}.|...
-00000820: 7c10 a101 0100 740b a012 7c06 640a a102  |.....t...|.d...
-00000830: 6900 1600 7d11 6416 6417 7c11 6901 1600  i...}.d.d.|.i...
-00000840: 7d12 7413 740b a014 7c12 a101 8301 8201  }.t.t...|.......
-00000850: 6400 0400 7d09 0400 7d06 0400 7d08 0400  d...}...}...}...
-00000860: 7d07 0400 7d0a 0400 7d0c 7d0b 5700 6400  }...}...}.}.W.d.
-00000870: 0400 0400 8303 0100 6e10 3100 73d8 7701  ........n.1.s.w.
-00000880: 0100 0100 0100 5900 0100 5700 6400 0400  ......Y...W.d...
-00000890: 0400 8303 0100 6400 5300 5700 6400 0400  ......d.S.W.d...
-000008a0: 0400 8303 0100 6400 5300 3100 73f0 7701  ......d.S.1.s.w.
-000008b0: 0100 0100 0100 5900 0100 6400 5300 2918  ......Y...d.S.).
-000008c0: 4eda 056f 7468 6572 7a34 626c 7565 6361  N..otherz4blueca
-000008d0: 7374 2e65 7661 6c75 6174 696f 6e2e 7368  st.evaluation.sh
-000008e0: 6170 5f76 616c 7565 732e 7368 6170 2e4b  ap_values.shap.K
-000008f0: 6572 6e65 6c45 7870 6c61 696e 6572 7a16  ernelExplainerz.
-00000900: 6d61 7470 6c6f 746c 6962 2e70 7970 6c6f  matplotlib.pyplo
-00000910: 742e 7368 6f77 679a 9999 9999 99b9 3f67  t.showg.......?g
-00000920: 9a99 9999 9999 c93f 6733 3333 3333 33d3  .......?g333333.
-00000930: 3f67 9a99 9999 9999 d93f 6700 0000 0000  ?g.......?g.....
-00000940: 00e0 3f67 3333 3333 3333 e33f 7201 0000  ..?g333333.?r...
-00000950: 0029 01fa 0669 7320 6e6f 7429 017a 1625  .)...is not).z.%
-00000960: 2870 7932 2973 2069 7320 6e6f 7420 2528  (py2)s is not %(
-00000970: 7079 3529 73da 0b73 6861 705f 7661 6c75  py5)s..shap_valu
-00000980: 6573 2902 7229 0000 00da 0370 7935 7a07  es).r).....py5z.
-00000990: 2528 7079 3729 73da 0370 7937 2901 fa01  %(py7)s..py7)...
-000009a0: 3e29 017a 2e25 2870 7931 3129 730a 7b25  >).z.%(py11)s.{%
-000009b0: 2870 7931 3129 7320 3d20 2528 7079 3929  (py11)s = %(py9)
-000009c0: 732e 7369 7a65 0a7d 203e 2025 2870 7931  s.size.} > %(py1
-000009d0: 3429 7329 03da 0370 7939 da04 7079 3131  4)s)...py9..py11
-000009e0: da04 7079 3134 7a08 2528 7079 3136 2973  ..py14z.%(py16)s
-000009f0: da04 7079 3136 7a0f 6173 7365 7274 2025  ..py16z.assert %
-00000a00: 2870 7931 3929 735a 0470 7931 3929 1572  (py19)sZ.py19).r
-00000a10: 0200 0000 da05 7061 7463 68da 026e 70da  ......patch..np.
-00000a20: 0561 7272 6179 da0c 7265 7475 726e 5f76  .array..return_v
-00000a30: 616c 7565 7242 0000 0072 0700 0000 5a17  aluerB...r....Z.
-00000a40: 6173 7365 7274 5f63 616c 6c65 645f 6f6e  assert_called_on
-00000a50: 6365 5f77 6974 68da 0770 7265 6469 6374  ce_with..predict
-00000a60: 5a12 6173 7365 7274 5f63 616c 6c65 645f  Z.assert_called_
-00000a70: 6f6e 6365 da04 7369 7a65 7233 0000 00da  once..sizer3....
-00000a80: 115f 6361 6c6c 5f72 6570 7263 6f6d 7061  ._call_reprcompa
-00000a90: 7265 7231 0000 0072 3200 0000 7234 0000  rer1...r2...r4..
-00000aa0: 0072 3500 0000 da06 6170 7065 6e64 da0e  .r5.....append..
-00000ab0: 5f66 6f72 6d61 745f 626f 6f6c 6f70 7236  _format_boolopr6
-00000ac0: 0000 0072 3700 0000 2913 720b 0000 0072  ...r7...).r....r
-00000ad0: 1400 0000 da09 6578 706c 6169 6e65 725a  ......explainerZ
-00000ae0: 156d 6f63 6b5f 6b65 726e 656c 5f65 7870  .mock_kernel_exp
-00000af0: 6c61 696e 6572 5a09 6d6f 636b 5f73 686f  lainerZ.mock_sho
-00000b00: 7772 4200 0000 da0b 4070 795f 6173 7365  wrB.....@py_asse
-00000b10: 7274 31da 0b40 7079 5f61 7373 6572 7434  rt1..@py_assert4
-00000b20: 723d 0000 00da 0b40 7079 5f61 7373 6572  r=.....@py_asser
-00000b30: 7430 da0c 4070 795f 6173 7365 7274 3130  t0..@py_assert10
-00000b40: da0c 4070 795f 6173 7365 7274 3133 da0c  ..@py_assert13..
-00000b50: 4070 795f 6173 7365 7274 3132 da0b 4070  @py_assert12..@p
-00000b60: 795f 666f 726d 6174 36da 0b40 7079 5f66  y_format6..@py_f
-00000b70: 6f72 6d61 7438 5a0c 4070 795f 666f 726d  ormat8Z.@py_form
-00000b80: 6174 3135 da0c 4070 795f 666f 726d 6174  at15..@py_format
-00000b90: 3137 5a0c 4070 795f 666f 726d 6174 3138  17Z.@py_format18
-00000ba0: 5a0c 4070 795f 666f 726d 6174 3230 7209  Z.@py_format20r.
-00000bb0: 0000 0072 0900 0000 720a 0000 00da 1b74  ...r....r......t
-00000bc0: 6573 745f 7368 6170 5f65 7870 6c61 6e61  est_shap_explana
-00000bd0: 7469 6f6e 735f 656c 7365 2f00 0000 7320  tions_else/...s 
-00000be0: 0000 0004 0104 0102 0104 ff0a 0202 fe02  ................
-00000bf0: 0204 0114 010a ff0c 040e 0208 01fe 0240  ...............@
-00000c00: 0050 f472 5d00 0000 6300 0000 0000 0000  .P.r]...c.......
-00000c10: 0000 0000 0007 0000 0007 0000 0043 0000  .............C..
-00000c20: 0073 a200 0000 7400 a001 6700 6401 a201  .s....t...g.d...
-00000c30: a101 7d00 7400 a001 6700 6402 a201 a101  ..}.t...g.d.....
-00000c40: 7d01 7402 7c00 7c01 8302 7d02 6403 7d03  }.t.|.|...}.d.}.
-00000c50: 7c02 7c03 6b02 7d04 7c04 734b 7403 a004  |.|.k.}.|.sKt...
-00000c60: 6404 7c04 6601 6405 7c02 7c03 6602 a104  d.|.f.d.|.|.f...
-00000c70: 6406 7405 a006 a100 7600 7330 7403 a007  d.t.....v.s0t...
-00000c80: 7c02 a101 7235 7403 a008 7c02 a101 6e01  |...r5t...|...n.
-00000c90: 6406 7403 a008 7c03 a101 6407 9c02 1600  d.t...|...d.....
-00000ca0: 7d05 6408 6409 7c05 6901 1600 7d06 7409  }.d.d.|.i...}.t.
-00000cb0: 7403 a00a 7c06 a101 8301 8201 6400 0400  t...|.......d...
-00000cc0: 7d04 7d03 6400 5300 290a 4e29 0472 0100  }.}.d.S.).N).r..
-00000cd0: 0000 7201 0000 0072 0100 0000 7201 0000  ..r....r....r...
-00000ce0: 0029 0472 0c00 0000 720c 0000 0072 0c00  .).r....r....r..
-00000cf0: 0000 720c 0000 0072 0100 0000 2901 fa02  ..r....r....)...
-00000d00: 3d3d 2901 7a12 2528 7079 3029 7320 3d3d  ==).z.%(py0)s ==
-00000d10: 2025 2870 7933 2973 da06 7265 7375 6c74   %(py3)s..result
-00000d20: 2902 7227 0000 00da 0370 7933 7a0e 6173  ).r'.....py3z.as
-00000d30: 7365 7274 2025 2870 7935 2973 7243 0000  sert %(py5)srC..
-00000d40: 0029 0b72 4b00 0000 724c 0000 0072 0600  .).rK...rL...r..
-00000d50: 0000 7233 0000 0072 5000 0000 7231 0000  ..r3...rP...r1..
-00000d60: 0072 3200 0000 7234 0000 0072 3500 0000  .r2...r4...r5...
-00000d70: 7236 0000 0072 3700 0000 2907 da06 795f  r6...r7...)...y_
-00000d80: 7472 7565 da09 795f 636c 6173 7365 7372  true..y_classesr
-00000d90: 5f00 0000 da0b 4070 795f 6173 7365 7274  _.....@py_assert
-00000da0: 3272 5400 0000 da0b 4070 795f 666f 726d  2rT.....@py_form
-00000db0: 6174 3472 5a00 0000 7209 0000 0072 0900  at4rZ...r....r..
-00000dc0: 0000 720a 0000 00da 1b74 6573 745f 6576  ..r......test_ev
-00000dd0: 616c 5f63 6c61 7373 6966 6965 725f 6578  al_classifier_ex
-00000de0: 6365 7074 4000 0000 7308 0000 000e 010e  cept@...s.......
-00000df0: 010a 017c 0172 6500 0000 291e da08 6275  ...|.re...)...bu
-00000e00: 696c 7469 6e73 7231 0000 00da 195f 7079  iltinsr1....._py
-00000e10: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
-00000e20: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
-00000e30: 6eda 0772 6577 7269 7465 7233 0000 00da  n..rewriter3....
-00000e40: 0875 6e69 7474 6573 7472 0200 0000 da05  .unittestr......
-00000e50: 6e75 6d70 7972 4b00 0000 da06 7061 6e64  numpyrK.....pand
-00000e60: 6173 7212 0000 00da 0670 7974 6573 74da  asr......pytest.
-00000e70: 1862 6c75 6563 6173 742e 626c 7565 7072  .bluecast.bluepr
-00000e80: 696e 7473 2e63 6173 7472 0300 0000 da1f  ints.castr......
-00000e90: 626c 7565 6361 7374 2e63 6f6e 6669 672e  bluecast.config.
-00000ea0: 7472 6169 6e69 6e67 5f63 6f6e 6669 6772  training_configr
-00000eb0: 0400 0000 7205 0000 00da 2062 6c75 6563  ....r..... bluec
-00000ec0: 6173 742e 6576 616c 7561 7469 6f6e 2e65  ast.evaluation.e
-00000ed0: 7661 6c5f 6d65 7472 6963 7372 0600 0000  val_metricsr....
-00000ee0: da1f 626c 7565 6361 7374 2e65 7661 6c75  ..bluecast.evalu
-00000ef0: 6174 696f 6e2e 7368 6170 5f76 616c 7565  ation.shap_value
-00000f00: 7372 0700 0000 da24 626c 7565 6361 7374  sr.....$bluecast
-00000f10: 2e74 6573 7473 2e6d 616b 655f 6461 7461  .tests.make_data
-00000f20: 2e63 7265 6174 655f 6461 7461 7208 0000  .create_datar...
-00000f30: 00da 0766 6978 7475 7265 720b 0000 0072  ...fixturer....r
-00000f40: 1400 0000 723f 0000 0072 5d00 0000 7265  ....r?...r]...re
-00000f50: 0000 0072 0900 0000 7209 0000 0072 0900  ...r....r....r..
-00000f60: 0000 720a 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000f70: 3e01 0000 0073 2000 0000 2600 0802 0801  >....s ...&.....
-00000f80: 0801 0c02 1001 0c01 0c01 0c01 0403 0a01  ................
-00000f90: 0404 0a01 0804 0817 0c11                 ..........
+00000320: 035f 0564 087c 035f 0664 097c 035f 0774  ._.d.|._.d.|._.t
+00000330: 0864 0a64 0b7c 037c 0264 0c8d 047d 047c  .d.d.|.|.d...}.|
+00000340: 046a 097c 007c 016a 0a64 0b64 0d64 0e8d  .j.|.|.j.d.d.d..
+00000350: 027c 0164 0b19 0064 0b64 0f8d 047d 0574  .|.d...d.d...}.t
+00000360: 0b7c 0583 0101 0074 0c7c 0574 0d83 027d  .|.....t.|.t...}
+00000370: 067c 0673 8764 1064 1174 0ea0 0fa1 0076  .|.s.d.d.t.....v
+00000380: 0073 5074 10a0 1174 0ca1 0172 5574 10a0  .sPt...t...rUt..
+00000390: 1274 0ca1 016e 0164 1164 1274 0ea0 0fa1  .t...n.d.d.t....
+000003a0: 0076 0073 6174 10a0 117c 05a1 0172 6674  .v.sat...|...rft
+000003b0: 10a0 127c 05a1 016e 0164 1264 1374 0ea0  ...|...n.d.d.t..
+000003c0: 0fa1 0076 0073 7274 10a0 1174 0da1 0172  ...v.srt...t...r
+000003d0: 7774 10a0 1274 0da1 016e 0164 1374 10a0  wt...t...n.d.t..
+000003e0: 127c 06a1 0164 149c 0416 007d 0774 1374  .|...d.....}.t.t
+000003f0: 10a0 147c 07a1 0183 0182 0164 157d 0664  ...|.......d.}.d
+00000400: 1553 0029 167a 2254 6573 7420 7468 6174  .S.).z"Test that
+00000410: 2074 6573 7473 2074 6865 2042 6c75 6543   tests the BlueC
+00000420: 6173 7420 636c 6173 73e9 c800 0000 e914  ast class.......
+00000430: 0000 0029 01da 0c72 616e 646f 6d5f 7374  ...)...random_st
+00000440: 6174 65e9 6400 0000 e915 0000 00e9 1000  ate.d...........
+00000450: 0000 e90a 0000 0054 720d 0000 00da 0662  .......Tr......b
+00000460: 696e 6172 79da 0674 6172 6765 7429 04da  inary..target)..
+00000470: 0d63 6c61 7373 5f70 726f 626c 656d da0d  .class_problem..
+00000480: 7461 7267 6574 5f63 6f6c 756d 6eda 0d63  target_column..c
+00000490: 6f6e 665f 7472 6169 6e69 6e67 da0c 636f  onf_training..co
+000004a0: 6e66 5f78 6762 6f6f 7374 720c 0000 0029  nf_xgboostr....)
+000004b0: 01da 0461 7869 7329 01da 0a74 6172 6765  ...axis)...targe
+000004c0: 745f 636f 6c7a 3561 7373 6572 7420 2528  t_colz5assert %(
+000004d0: 7079 3429 730a 7b25 2870 7934 2973 203d  py4)s.{%(py4)s =
+000004e0: 2025 2870 7930 2973 2825 2870 7931 2973   %(py0)s(%(py1)s
+000004f0: 2c20 2528 7079 3229 7329 0a7d da0a 6973  , %(py2)s).}..is
+00000500: 696e 7374 616e 6365 da09 6576 616c 5f64  instance..eval_d
+00000510: 6963 74da 0464 6963 7429 04da 0370 7930  ict..dict)...py0
+00000520: da03 7079 31da 0370 7932 da03 7079 344e  ..py1..py2..py4N
+00000530: 2915 7208 0000 0072 0500 0000 da09 7374  ).r....r......st
+00000540: 6570 735f 6d61 78da 0e6e 756d 5f6c 6561  eps_max..num_lea
+00000550: 7665 735f 6d61 7872 0400 0000 da1c 6879  ves_maxr......hy
+00000560: 7065 7270 6172 616d 6574 6572 5f74 756e  perparameter_tun
+00000570: 696e 675f 726f 756e 6473 da18 656e 6162  ing_rounds..enab
+00000580: 6c65 5f66 6561 7475 7265 5f73 656c 6563  le_feature_selec
+00000590: 7469 6f6e da14 6879 7065 7274 756e 696e  tion..hypertunin
+000005a0: 675f 6376 5f66 6f6c 6473 7203 0000 00da  g_cv_foldsr.....
+000005b0: 0866 6974 5f65 7661 6cda 0464 726f 70da  .fit_eval..drop.
+000005c0: 0570 7269 6e74 7226 0000 0072 2800 0000  .printr&...r(...
+000005d0: da0c 4070 795f 6275 696c 7469 6e73 da06  ..@py_builtins..
+000005e0: 6c6f 6361 6c73 da0a 4070 7974 6573 745f  locals..@pytest_
+000005f0: 6172 da18 5f73 686f 756c 645f 7265 7072  ar.._should_repr
+00000600: 5f67 6c6f 6261 6c5f 6e61 6d65 da09 5f73  _global_name.._s
+00000610: 6166 6572 6570 72da 0e41 7373 6572 7469  aferepr..Asserti
+00000620: 6f6e 4572 726f 72da 135f 666f 726d 6174  onError.._format
+00000630: 5f65 7870 6c61 6e61 7469 6f6e 2908 da08  _explanation)...
+00000640: 6466 5f74 7261 696e da06 6466 5f76 616c  df_train..df_val
+00000650: da14 7867 626f 6f73 745f 7061 7261 6d5f  ..xgboost_param_
+00000660: 636f 6e66 6967 da0c 7472 6169 6e5f 636f  config..train_co
+00000670: 6e66 6967 da06 6175 746f 6d6c 7227 0000  nfig..automlr'..
+00000680: 00da 0b40 7079 5f61 7373 6572 7433 da0b  ...@py_assert3..
+00000690: 4070 795f 666f 726d 6174 3572 0900 0000  @py_format5r....
+000006a0: 7209 0000 0072 0a00 0000 da16 7465 7374  r....r......test
+000006b0: 5f73 6861 705f 6578 706c 616e 6174 696f  _shap_explanatio
+000006c0: 6e73 1800 0000 7328 0000 000c 020c 0106  ns....s(........
+000006d0: 0106 0106 0106 0106 0106 0106 0102 0202  ................
+000006e0: 0102 0102 0102 0106 fc04 0616 0106 ff08  ................
+000006f0: 039c 0172 4300 0000 6302 0000 0000 0000  ...rC...c.......
+00000700: 0000 0000 0013 0000 0009 0000 0043 0000  .............C..
+00000710: 0073 ee01 0000 6401 7d02 7400 a001 6402  .s....d.}.t...d.
+00000720: a101 8fe6 7d03 7400 a001 6403 a101 8fc8  ....}.t...d.....
+00000730: 7d04 7402 a003 6404 6405 6702 6406 6407  }.t...d.d.g.d.d.
+00000740: 6702 6408 6409 6702 6703 a101 7c03 6a04  g.d.d.g.g...|.j.
+00000750: 6a05 5f04 7406 7c00 7c01 7c02 8303 7d05  j._.t.|.|.|...}.
+00000760: 7c03 a007 7c00 6a08 7c01 a102 0100 7c04  |...|.j.|.....|.
+00000770: a009 a100 0100 6700 7d06 6400 7d07 7c05  ......g.}.d.}.|.
+00000780: 7c07 7501 7d08 7c08 7d09 7c08 7247 7c05  |.u.}.|.}.|.rG|.
+00000790: 6a0a 7d0a 640a 7d0b 7c0a 7c0b 6b04 7d0c  j.}.d.}.|.|.k.}.
+000007a0: 7c0c 7d09 7c09 73c0 740b a00c 640b 7c08  |.}.|.s.t...d.|.
+000007b0: 6601 640c 7c05 7c07 6602 a104 640d 740d  f.d.|.|.f...d.t.
+000007c0: a00e a100 7600 735e 740b a00f 7c05 a101  ....v.s^t...|...
+000007d0: 7263 740b a010 7c05 a101 6e01 640d 740b  rct...|...n.d.t.
+000007e0: a010 7c07 a101 640e 9c02 1600 7d0d 640f  ..|...d.....}.d.
+000007f0: 6410 7c0d 6901 1600 7d0e 7c06 a011 7c0e  d.|.i...}.|...|.
+00000800: a101 0100 7c08 72ab 740b a00c 6411 7c0c  ....|.r.t...d.|.
+00000810: 6601 6412 7c0a 7c0b 6602 a104 640d 740d  f.d.|.|.f...d.t.
+00000820: a00e a100 7600 738e 740b a00f 7c05 a101  ....v.s.t...|...
+00000830: 7293 740b a010 7c05 a101 6e01 640d 740b  r.t...|...n.d.t.
+00000840: a010 7c0a a101 740b a010 7c0b a101 6413  ..|...t...|...d.
+00000850: 9c03 1600 7d0f 6414 6415 7c0f 6901 1600  ....}.d.d.|.i...
+00000860: 7d10 7c06 a011 7c10 a101 0100 740b a012  }.|...|.....t...
+00000870: 7c06 640a a102 6900 1600 7d11 6416 6417  |.d...i...}.d.d.
+00000880: 7c11 6901 1600 7d12 7413 740b a014 7c12  |.i...}.t.t...|.
+00000890: a101 8301 8201 6400 0400 7d09 0400 7d06  ......d...}...}.
+000008a0: 0400 7d08 0400 7d07 0400 7d0a 0400 7d0c  ..}...}...}...}.
+000008b0: 7d0b 5700 6400 0400 0400 8303 0100 6e10  }.W.d.........n.
+000008c0: 3100 73d8 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
+000008d0: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
+000008e0: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
+000008f0: 3100 73f0 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
+00000900: 6400 5300 2918 4eda 056f 7468 6572 7a34  d.S.).N..otherz4
+00000910: 626c 7565 6361 7374 2e65 7661 6c75 6174  bluecast.evaluat
+00000920: 696f 6e2e 7368 6170 5f76 616c 7565 732e  ion.shap_values.
+00000930: 7368 6170 2e4b 6572 6e65 6c45 7870 6c61  shap.KernelExpla
+00000940: 696e 6572 7a16 6d61 7470 6c6f 746c 6962  inerz.matplotlib
+00000950: 2e70 7970 6c6f 742e 7368 6f77 679a 9999  .pyplot.showg...
+00000960: 9999 99b9 3f67 9a99 9999 9999 c93f 6733  ....?g.......?g3
+00000970: 3333 3333 33d3 3f67 9a99 9999 9999 d93f  33333.?g.......?
+00000980: 6700 0000 0000 00e0 3f67 3333 3333 3333  g.......?g333333
+00000990: e33f 7201 0000 0029 01fa 0669 7320 6e6f  .?r....)...is no
+000009a0: 7429 017a 1625 2870 7932 2973 2069 7320  t).z.%(py2)s is 
+000009b0: 6e6f 7420 2528 7079 3529 73da 0b73 6861  not %(py5)s..sha
+000009c0: 705f 7661 6c75 6573 2902 722b 0000 00da  p_values).r+....
+000009d0: 0370 7935 7a07 2528 7079 3729 73da 0370  .py5z.%(py7)s..p
+000009e0: 7937 2901 fa01 3e29 017a 2e25 2870 7931  y7)...>).z.%(py1
+000009f0: 3129 730a 7b25 2870 7931 3129 7320 3d20  1)s.{%(py11)s = 
+00000a00: 2528 7079 3929 732e 7369 7a65 0a7d 203e  %(py9)s.size.} >
+00000a10: 2025 2870 7931 3429 7329 03da 0370 7939   %(py14)s)...py9
+00000a20: da04 7079 3131 da04 7079 3134 7a08 2528  ..py11..py14z.%(
+00000a30: 7079 3136 2973 da04 7079 3136 7a0f 6173  py16)s..py16z.as
+00000a40: 7365 7274 2025 2870 7931 3929 735a 0470  sert %(py19)sZ.p
+00000a50: 7931 3929 1572 0200 0000 da05 7061 7463  y19).r......patc
+00000a60: 68da 026e 70da 0561 7272 6179 da0c 7265  h..np..array..re
+00000a70: 7475 726e 5f76 616c 7565 7246 0000 0072  turn_valuerF...r
+00000a80: 0700 0000 5a17 6173 7365 7274 5f63 616c  ....Z.assert_cal
+00000a90: 6c65 645f 6f6e 6365 5f77 6974 68da 0770  led_once_with..p
+00000aa0: 7265 6469 6374 5a12 6173 7365 7274 5f63  redictZ.assert_c
+00000ab0: 616c 6c65 645f 6f6e 6365 da04 7369 7a65  alled_once..size
+00000ac0: 7237 0000 00da 115f 6361 6c6c 5f72 6570  r7....._call_rep
+00000ad0: 7263 6f6d 7061 7265 7235 0000 0072 3600  rcomparer5...r6.
+00000ae0: 0000 7238 0000 0072 3900 0000 da06 6170  ..r8...r9.....ap
+00000af0: 7065 6e64 da0e 5f66 6f72 6d61 745f 626f  pend.._format_bo
+00000b00: 6f6c 6f70 723a 0000 0072 3b00 0000 2913  olopr:...r;...).
+00000b10: 720b 0000 0072 1600 0000 da09 6578 706c  r....r......expl
+00000b20: 6169 6e65 725a 156d 6f63 6b5f 6b65 726e  ainerZ.mock_kern
+00000b30: 656c 5f65 7870 6c61 696e 6572 5a09 6d6f  el_explainerZ.mo
+00000b40: 636b 5f73 686f 7772 4600 0000 da0b 4070  ck_showrF.....@p
+00000b50: 795f 6173 7365 7274 31da 0b40 7079 5f61  y_assert1..@py_a
+00000b60: 7373 6572 7434 7241 0000 00da 0b40 7079  ssert4rA.....@py
+00000b70: 5f61 7373 6572 7430 da0c 4070 795f 6173  _assert0..@py_as
+00000b80: 7365 7274 3130 da0c 4070 795f 6173 7365  sert10..@py_asse
+00000b90: 7274 3133 da0c 4070 795f 6173 7365 7274  rt13..@py_assert
+00000ba0: 3132 da0b 4070 795f 666f 726d 6174 36da  12..@py_format6.
+00000bb0: 0b40 7079 5f66 6f72 6d61 7438 5a0c 4070  .@py_format8Z.@p
+00000bc0: 795f 666f 726d 6174 3135 da0c 4070 795f  y_format15..@py_
+00000bd0: 666f 726d 6174 3137 5a0c 4070 795f 666f  format17Z.@py_fo
+00000be0: 726d 6174 3138 5a0c 4070 795f 666f 726d  rmat18Z.@py_form
+00000bf0: 6174 3230 7209 0000 0072 0900 0000 720a  at20r....r....r.
+00000c00: 0000 00da 1b74 6573 745f 7368 6170 5f65  .....test_shap_e
+00000c10: 7870 6c61 6e61 7469 6f6e 735f 656c 7365  xplanations_else
+00000c20: 3100 0000 7320 0000 0004 0104 0102 0104  1...s ..........
+00000c30: ff0a 0202 fe02 0204 0114 010a ff0c 040e  ................
+00000c40: 0208 01fe 0240 0050 f472 6100 0000 6300  .....@.P.ra...c.
+00000c50: 0000 0000 0000 0000 0000 0007 0000 0007  ................
+00000c60: 0000 0043 0000 0073 a200 0000 7400 a001  ...C...s....t...
+00000c70: 6700 6401 a201 a101 7d00 7400 a001 6700  g.d.....}.t...g.
+00000c80: 6402 a201 a101 7d01 7402 7c00 7c01 8302  d.....}.t.|.|...
+00000c90: 7d02 6403 7d03 7c02 7c03 6b02 7d04 7c04  }.d.}.|.|.k.}.|.
+00000ca0: 734b 7403 a004 6404 7c04 6601 6405 7c02  sKt...d.|.f.d.|.
+00000cb0: 7c03 6602 a104 6406 7405 a006 a100 7600  |.f...d.t.....v.
+00000cc0: 7330 7403 a007 7c02 a101 7235 7403 a008  s0t...|...r5t...
+00000cd0: 7c02 a101 6e01 6406 7403 a008 7c03 a101  |...n.d.t...|...
+00000ce0: 6407 9c02 1600 7d05 6408 6409 7c05 6901  d.....}.d.d.|.i.
+00000cf0: 1600 7d06 7409 7403 a00a 7c06 a101 8301  ..}.t.t...|.....
+00000d00: 8201 6400 0400 7d04 7d03 6400 5300 290a  ..d...}.}.d.S.).
+00000d10: 4e29 0472 0100 0000 7201 0000 0072 0100  N).r....r....r..
+00000d20: 0000 7201 0000 0029 0472 0c00 0000 720c  ..r....).r....r.
+00000d30: 0000 0072 0c00 0000 720c 0000 0072 0100  ...r....r....r..
+00000d40: 0000 2901 fa02 3d3d 2901 7a12 2528 7079  ..)...==).z.%(py
+00000d50: 3029 7320 3d3d 2025 2870 7933 2973 da06  0)s == %(py3)s..
+00000d60: 7265 7375 6c74 2902 7229 0000 00da 0370  result).r).....p
+00000d70: 7933 7a0e 6173 7365 7274 2025 2870 7935  y3z.assert %(py5
+00000d80: 2973 7247 0000 0029 0b72 4f00 0000 7250  )srG...).rO...rP
+00000d90: 0000 0072 0600 0000 7237 0000 0072 5400  ...r....r7...rT.
+00000da0: 0000 7235 0000 0072 3600 0000 7238 0000  ..r5...r6...r8..
+00000db0: 0072 3900 0000 723a 0000 0072 3b00 0000  .r9...r:...r;...
+00000dc0: 2907 da06 795f 7472 7565 da09 795f 636c  )...y_true..y_cl
+00000dd0: 6173 7365 7372 6300 0000 da0b 4070 795f  assesrc.....@py_
+00000de0: 6173 7365 7274 3272 5800 0000 da0b 4070  assert2rX.....@p
+00000df0: 795f 666f 726d 6174 3472 5e00 0000 7209  y_format4r^...r.
+00000e00: 0000 0072 0900 0000 720a 0000 00da 1b74  ...r....r......t
+00000e10: 6573 745f 6576 616c 5f63 6c61 7373 6966  est_eval_classif
+00000e20: 6965 725f 6578 6365 7074 4200 0000 7308  ier_exceptB...s.
+00000e30: 0000 000e 010e 010a 017c 0172 6900 0000  .........|.ri...
+00000e40: 291e da08 6275 696c 7469 6e73 7235 0000  )...builtinsr5..
+00000e50: 00da 195f 7079 7465 7374 2e61 7373 6572  ..._pytest.asser
+00000e60: 7469 6f6e 2e72 6577 7269 7465 da09 6173  tion.rewrite..as
+00000e70: 7365 7274 696f 6eda 0772 6577 7269 7465  sertion..rewrite
+00000e80: 7237 0000 00da 0875 6e69 7474 6573 7472  r7.....unittestr
+00000e90: 0200 0000 da05 6e75 6d70 7972 4f00 0000  ......numpyrO...
+00000ea0: da06 7061 6e64 6173 7214 0000 00da 0670  ..pandasr......p
+00000eb0: 7974 6573 74da 1862 6c75 6563 6173 742e  ytest..bluecast.
+00000ec0: 626c 7565 7072 696e 7473 2e63 6173 7472  blueprints.castr
+00000ed0: 0300 0000 da1f 626c 7565 6361 7374 2e63  ......bluecast.c
+00000ee0: 6f6e 6669 672e 7472 6169 6e69 6e67 5f63  onfig.training_c
+00000ef0: 6f6e 6669 6772 0400 0000 7205 0000 00da  onfigr....r.....
+00000f00: 2062 6c75 6563 6173 742e 6576 616c 7561   bluecast.evalua
+00000f10: 7469 6f6e 2e65 7661 6c5f 6d65 7472 6963  tion.eval_metric
+00000f20: 7372 0600 0000 da1f 626c 7565 6361 7374  sr......bluecast
+00000f30: 2e65 7661 6c75 6174 696f 6e2e 7368 6170  .evaluation.shap
+00000f40: 5f76 616c 7565 7372 0700 0000 da24 626c  _valuesr.....$bl
+00000f50: 7565 6361 7374 2e74 6573 7473 2e6d 616b  uecast.tests.mak
+00000f60: 655f 6461 7461 2e63 7265 6174 655f 6461  e_data.create_da
+00000f70: 7461 7208 0000 00da 0766 6978 7475 7265  tar......fixture
+00000f80: 720b 0000 0072 1600 0000 7243 0000 0072  r....r....rC...r
+00000f90: 6100 0000 7269 0000 0072 0900 0000 7209  a...ri...r....r.
+00000fa0: 0000 0072 0900 0000 720a 0000 00da 083c  ...r....r......<
+00000fb0: 6d6f 6475 6c65 3e01 0000 0073 2000 0000  module>....s ...
+00000fc0: 2600 0802 0801 0801 0c02 1001 0c01 0c01  &...............
+00000fd0: 0c01 0403 0a01 0404 0a01 0804 0819 0c11  ................
```

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.4/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc` & `bluecast-0.4/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/make_data/create_data.py` & `bluecast-0.4/bluecast/tests/make_data/create_data.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_cast.py` & `bluecast-0.4/bluecast/tests/test_cast.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,26 +36,16 @@
     df_train = synthetic_train_test_data[0]
     df_val = synthetic_train_test_data[1]
     xgboost_param_config = XgboostTuneParamsConfig()
     xgboost_param_config.steps_max = 100
     xgboost_param_config.num_leaves_max = 16
     train_config = TrainingConfig()
     train_config.hyperparameter_tuning_rounds = 10
-
-    # add custom feature selection
-    custom_feat_sel = FeatureSelectionConfig()
-    # custom_feat_sel.execute_selection = False
-    custom_feat_sel.selection_strategy = RFECV(
-        estimator=xgb.XGBClassifier(),
-        step=1,
-        cv=StratifiedKFold(2, random_state=0, shuffle=True),
-        min_features_to_select=1,
-        scoring=make_scorer(matthews_corrcoef),
-        n_jobs=1,
-    )
+    train_config.enable_feature_selection = True
+    train_config.hypertuning_cv_folds = 2
 
     # add custom last mile computation
     class MyCustomLastMilePreprocessing(CustomPreprocessing):
         def custom_function(self, df: pd.DataFrame) -> pd.DataFrame:
             df = df / 2
             df["custom_col"] = 5
             return df
@@ -84,15 +74,14 @@
 
     automl = BlueCast(
         class_problem="binary",
         target_column="target",
         conf_training=train_config,
         conf_xgboost=xgboost_param_config,
         custom_last_mile_computation=custom_last_mile_computation,
-        conf_feature_selection=custom_feat_sel,
     )
     automl.fit(df_train, target_col="target")
     print("Autotuning successful.")
     y_probs, y_classes = automl.predict(df_val.drop("target", axis=1))
     print("Predicting successful.")
     assert len(y_probs) == len(df_val.index)
     assert len(y_classes) == len(df_val.index)
@@ -117,31 +106,37 @@
         predicted_classes = self.model.predict(df)
         return predicted_probas, predicted_classes
 
 
 def test_bluecast_with_custom_model():
     # Create an instance of the custom model
     custom_model = CustomModel()
+    train_config = TrainingConfig()
+    train_config.hyperparameter_tuning_rounds = 10
+    train_config.enable_feature_selection = True
+    train_config.hypertuning_cv_folds = 2
 
     # add custom feature selection
     custom_feat_sel = FeatureSelectionConfig()
+    # custom_feat_sel.execute_selection = False
     custom_feat_sel.selection_strategy = RFECV(
         estimator=xgb.XGBClassifier(),
         step=1,
         cv=StratifiedKFold(2, random_state=0, shuffle=True),
-        min_features_to_select=5,
+        min_features_to_select=1,
         scoring=make_scorer(matthews_corrcoef),
         n_jobs=1,
     )
 
     # Create an instance of the BlueCast class with the custom model
     bluecast = BlueCast(
         class_problem="binary",
         target_column="target",
         ml_model=custom_model,
+        conf_training=train_config,
         conf_feature_selection=custom_feat_sel,
     )
 
     # Create some sample data for testing
     x_train = pd.DataFrame(
         {
             "feature1": [i for i in range(10)],
```

### Comparing `bluecast-0.3.1/bluecast/tests/test_check_gpu_support.py` & `bluecast-0.4/bluecast/tests/test_check_gpu_support.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_custom_processing_base_class.py` & `bluecast-0.4/bluecast/tests/test_custom_processing_base_class.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_datetime_features.py` & `bluecast-0.4/bluecast/tests/test_datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_encode_target_labels.py` & `bluecast-0.4/bluecast/tests/test_encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_feature_type_detector.py` & `bluecast-0.4/bluecast/tests/test_feature_type_detector.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_load_for_production.py` & `bluecast-0.4/bluecast/tests/test_load_for_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_nulls_and_infs.py` & `bluecast-0.4/bluecast/tests/test_nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_save_to_production.py` & `bluecast-0.4/bluecast/tests/test_save_to_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_schema_checks.py` & `bluecast-0.4/bluecast/tests/test_schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_shap_explanations.py` & `bluecast-0.4/bluecast/tests/test_shap_explanations.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     df_train = create_synthetic_dataframe(200, random_state=20)
     df_val = create_synthetic_dataframe(100, random_state=21)
     xgboost_param_config = XgboostTuneParamsConfig()
     xgboost_param_config.steps_max = 100
     xgboost_param_config.num_leaves_max = 16
     train_config = TrainingConfig()
     train_config.hyperparameter_tuning_rounds = 10
+    train_config.enable_feature_selection = True
+    train_config.hypertuning_cv_folds = 2
 
     automl = BlueCast(
         class_problem="binary",
         target_column="target",
         conf_training=train_config,
         conf_xgboost=xgboost_param_config,
     )
```

### Comparing `bluecast-0.3.1/bluecast/tests/test_target_encoding_binary.py` & `bluecast-0.4/bluecast/tests/test_target_encoding_binary.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_target_encoding_multiclass.py` & `bluecast-0.4/bluecast/tests/test_target_encoding_multiclass.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/bluecast/tests/test_train_test_split.py` & `bluecast-0.4/bluecast/tests/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.3.1/pyproject.toml` & `bluecast-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluecast"
-version = "0.3.1"
+version = "0.4"
 description = "A lightweight and fast automl framework"
 authors = ["Thomas Meißner <meissnercorporation@gmx.de>"]
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
```

### Comparing `bluecast-0.3.1/PKG-INFO` & `bluecast-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecast
-Version: 0.3.1
+Version: 0.4
 Summary: A lightweight and fast automl framework
 Home-page: https://github.com/ThomasMeissnerDS/BlueCast
 License: GPL-3.0-only
 Author: Thomas Meißner
 Author-email: meissnercorporation@gmx.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -266,26 +266,58 @@
 
 automl.fit(df_train, target_col="target")
 y_probs, y_classes = automl.predict(df_val)
 ```
 
 #### Custom feature selection
 
-As of version 0.3 BlueCast added automated feature selection. Also this
-step can be customized. An instance of `RFECV` is expected for `selection_strategy`.
-Otherwise the pipeline will fail. To disable feature selection set `execute_selection`
-to `False`. To surpass the `RFECV` limitation a custom feature selection algorithm
-can also be passed as part of a custom last mile computation.
+BlueCast offers automated feature selection. On default the feature
+selection is disabled, but BlueCast raises a warning to inform the
+user about this option. The behaviour can be controlled via the
+`TrainingConfig`.
+
+```sh
+from bluecast.blueprints.cast import BlueCast
+from bluecast.preprocessing.custom import CustomPreprocessing
+from bluecast.config.training_config import TrainingConfig
+
+# Create a custom training config and adjust general training parameters
+train_config = TrainingConfig()
+train_config.hyperparameter_tuning_rounds = 10
+train_config.autotune_model = False # we want to run just normal training, no hyperparameter tuning
+train_config.enable_feature_selection = True
+
+# Pass the custom configs to the BlueCast class
+automl = BlueCast(
+        class_problem="binary",
+        target_column="target"
+        conf_training=train_config,
+    )
+
+automl.fit(df_train, target_col="target")
+y_probs, y_classes = automl.predict(df_val)
+```
+
+Also this step can be customized. An instance of `RFECV` is expected for `selection_strategy`.
+Otherwise the pipeline will fail. To surpass the `RFECV` limitation a custom feature
+selection algorithm can also be passed as part of a custom last mile computation.
+Here is an example adjusting the in-built solution via `RFECV`:
 
 ```sh
 from bluecast.config.training_config import FeatureSelectionConfig
+from bluecast.config.training_config import TrainingConfig
 from sklearn.feature_selection import RFECV
 from sklearn.metrics import make_scorer, matthews_corrcoef
 from sklearn.model_selection import StratifiedKFold
 
+
+# Create a custom training config and adjust general training parameters
+train_config = TrainingConfig()
+train_config.enable_feature_selection = True
+
 # add custom feature selection
 custom_feat_sel = FeatureSelectionConfig()
 # custom_feat_sel.execute_selection = False
 custom_feat_sel.selection_strategy = RFECV(
     estimator=xgb.XGBClassifier(),
     step=1,
     cv=StratifiedKFold(10, random_state=0, shuffle=True),
@@ -295,14 +327,15 @@
 )
 
 # Create an instance of the BlueCast class with the custom model
 bluecast = BlueCast(
     class_problem="binary",
     target_column="target",
     conf_feature_selection=custom_feat_sel,
+    conf_training=train_config,
 
 # Create some sample data for testing
 x_train = pd.DataFrame(
     {"feature1": [i for i in range(10)], "feature2": [i for i in range(10)]}
 )
 y_train = pd.Series([0, 1, 0, 1, 0, 1, 0, 1, 0, 1])
 x_test = pd.DataFrame(
```

