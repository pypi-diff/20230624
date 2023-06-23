# Comparing `tmp/arize-7.0.6.tar.gz` & `tmp/arize-7.0.6rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.0.6.tar", last modified: Fri Jun 23 23:18:18 2023, max compression
+gzip compressed data, was "arize-7.0.6rc2.tar", last modified: Fri Jun 23 22:01:14 2023, max compression
```

## Comparing `arize-7.0.6.tar` & `arize-7.0.6rc2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.165696 arize-7.0.6/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-23 05:09:35.000000 arize-7.0.6/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-23 05:09:35.000000 arize-7.0.6/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-23 23:18:18.166301 arize-7.0.6/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-23 05:09:35.000000 arize-7.0.6/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.046826 arize-7.0.6/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       22 2023-06-23 23:13:32.000000 arize-7.0.6/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    28894 2023-06-23 23:03:21.000000 arize-7.0.6/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-23 05:09:35.000000 arize-7.0.6/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.065660 arize-7.0.6/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-23 05:09:35.000000 arize-7.0.6/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.069277 arize-7.0.6/arize/exporter/
--rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-23 05:09:35.000000 arize-7.0.6/arize/exporter/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.074547 arize-7.0.6/arize/exporter/core/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/exporter/core/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    10940 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/core/client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1343 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/core/query.py
--rw-r--r--   0 kiko       (501) staff       (20)     3464 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/core/session.py
--rw-r--r--   0 kiko       (501) staff       (20)     2406 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/publicexporter_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.079696 arize-7.0.6/arize/exporter/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/exporter/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1422 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)      727 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/utils/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)     5793 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/utils/schema_parser.py
--rw-r--r--   0 kiko       (501) staff       (20)      778 2023-06-23 18:59:38.000000 arize-7.0.6/arize/exporter/utils/validation.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.081758 arize-7.0.6/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.108897 arize-7.0.6/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6988 2023-06-23 18:59:38.000000 arize-7.0.6/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.116670 arize-7.0.6/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.133017 arize-7.0.6/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    22779 2023-06-23 18:59:38.000000 arize-7.0.6/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.135695 arize-7.0.6/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     5090 2023-06-23 18:59:38.000000 arize-7.0.6/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.142782 arize-7.0.6/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-06-23 05:09:35.000000 arize-7.0.6/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    70456 2023-06-23 18:59:38.000000 arize-7.0.6/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)    50888 2023-06-23 23:03:21.000000 arize-7.0.6/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.155145 arize-7.0.6/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      619 2023-06-23 05:09:35.000000 arize-7.0.6/arize/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-23 05:09:35.000000 arize-7.0.6/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-23 05:09:35.000000 arize-7.0.6/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    24659 2023-06-23 18:59:38.000000 arize-7.0.6/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-23 05:09:35.000000 arize-7.0.6/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.054498 arize-7.0.6/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-23 23:18:18.000000 arize-7.0.6/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1879 2023-06-23 23:18:18.000000 arize-7.0.6/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-06-23 23:18:18.000000 arize-7.0.6/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      429 2023-06-23 23:18:18.000000 arize-7.0.6/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-06-23 23:18:18.000000 arize-7.0.6/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-23 05:09:35.000000 arize-7.0.6/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1517 2023-06-23 23:18:18.168879 arize-7.0.6/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 23:18:18.162170 arize-7.0.6/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    49474 2023-06-23 23:03:21.000000 arize-7.0.6/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-23 05:09:35.000000 arize-7.0.6/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.211847 arize-7.0.6rc2/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-23 05:09:35.000000 arize-7.0.6rc2/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-23 05:09:35.000000 arize-7.0.6rc2/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-06-23 22:01:14.212103 arize-7.0.6rc2/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-23 05:09:35.000000 arize-7.0.6rc2/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.106493 arize-7.0.6rc2/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       25 2023-06-23 22:00:52.000000 arize-7.0.6rc2/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    28894 2023-06-23 20:55:39.000000 arize-7.0.6rc2/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.143701 arize-7.0.6rc2/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.146540 arize-7.0.6rc2/arize/exporter/
+-rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/exporter/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.152199 arize-7.0.6rc2/arize/exporter/core/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/exporter/core/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    10940 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/exporter/core/client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1343 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/exporter/core/query.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3464 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/exporter/core/session.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2406 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/exporter/publicexporter_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.157457 arize-7.0.6rc2/arize/exporter/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/exporter/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1422 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/exporter/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)      727 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/exporter/utils/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5793 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/exporter/utils/schema_parser.py
+-rw-r--r--   0 kiko       (501) staff       (20)      778 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/exporter/utils/validation.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.159049 arize-7.0.6rc2/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.190186 arize-7.0.6rc2/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6988 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/embeddings/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.191256 arize-7.0.6rc2/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.193672 arize-7.0.6rc2/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    22779 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.195241 arize-7.0.6rc2/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5090 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.198242 arize-7.0.6rc2/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    70456 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)    50888 2023-06-23 20:55:39.000000 arize-7.0.6rc2/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.208434 arize-7.0.6rc2/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      619 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    24659 2023-06-23 18:59:38.000000 arize-7.0.6rc2/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-23 05:09:35.000000 arize-7.0.6rc2/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.114945 arize-7.0.6rc2/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-06-23 22:01:14.000000 arize-7.0.6rc2/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1879 2023-06-23 22:01:14.000000 arize-7.0.6rc2/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-06-23 22:01:14.000000 arize-7.0.6rc2/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      429 2023-06-23 22:01:14.000000 arize-7.0.6rc2/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-06-23 22:01:14.000000 arize-7.0.6rc2/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-23 05:09:35.000000 arize-7.0.6rc2/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1517 2023-06-23 22:01:14.214184 arize-7.0.6rc2/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 22:01:14.210939 arize-7.0.6rc2/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    49474 2023-06-23 20:55:39.000000 arize-7.0.6rc2/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-23 05:09:35.000000 arize-7.0.6rc2/tests/test_utils.py
```

### Comparing `arize-7.0.6/LICENSE.md` & `arize-7.0.6rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/PKG-INFO` & `arize-7.0.6rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.6
+Version: 7.0.6rc2
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.6/README.md` & `arize-7.0.6rc2/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/api.py` & `arize-7.0.6rc2/arize/api.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/bounded_executor.py` & `arize-7.0.6rc2/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/bulk_client.py` & `arize-7.0.6rc2/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/bulk_client_shap.py` & `arize-7.0.6rc2/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/client_shap_values.py` & `arize-7.0.6rc2/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/log_client.py` & `arize-7.0.6rc2/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/log_pandas_dataframe.py` & `arize-7.0.6rc2/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/examples/preproduction_client.py` & `arize-7.0.6rc2/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/core/client.py` & `arize-7.0.6rc2/arize/exporter/core/client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/core/query.py` & `arize-7.0.6rc2/arize/exporter/core/query.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/core/session.py` & `arize-7.0.6rc2/arize/exporter/core/session.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/publicexporter_pb2.py` & `arize-7.0.6rc2/arize/exporter/publicexporter_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/utils/constants.py` & `arize-7.0.6rc2/arize/exporter/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/utils/errors.py` & `arize-7.0.6rc2/arize/exporter/utils/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/utils/schema_parser.py` & `arize-7.0.6rc2/arize/exporter/utils/schema_parser.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/exporter/utils/validation.py` & `arize-7.0.6rc2/arize/exporter/utils/validation.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/auto_generator.py` & `arize-7.0.6rc2/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/base_generators.py` & `arize-7.0.6rc2/arize/pandas/embeddings/base_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/cv_generators.py` & `arize-7.0.6rc2/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/errors.py` & `arize-7.0.6rc2/arize/pandas/embeddings/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/models.py` & `arize-7.0.6rc2/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/nlp_generators.py` & `arize-7.0.6rc2/arize/pandas/embeddings/nlp_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/embeddings/tabular_generators.py` & `arize-7.0.6rc2/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.0.6rc2/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/logger.py` & `arize-7.0.6rc2/arize/pandas/logger.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.0.6rc2/arize/pandas/surrogate_explainer/mimic.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/validation/errors.py` & `arize-7.0.6rc2/arize/pandas/validation/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/pandas/validation/validator.py` & `arize-7.0.6rc2/arize/pandas/validation/validator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/public_pb2.py` & `arize-7.0.6rc2/arize/public_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/utils/constants.py` & `arize-7.0.6rc2/arize/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/utils/logging.py` & `arize-7.0.6rc2/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/utils/model_mapping.json` & `arize-7.0.6rc2/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/utils/types.py` & `arize-7.0.6rc2/arize/utils/types.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize/utils/utils.py` & `arize-7.0.6rc2/arize/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/arize.egg-info/PKG-INFO` & `arize-7.0.6rc2/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.6
+Version: 7.0.6rc2
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.6/arize.egg-info/SOURCES.txt` & `arize-7.0.6rc2/arize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/setup.cfg` & `arize-7.0.6rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/tests/test_api.py` & `arize-7.0.6rc2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.6/tests/test_utils.py` & `arize-7.0.6rc2/tests/test_utils.py`

 * *Files identical despite different names*

