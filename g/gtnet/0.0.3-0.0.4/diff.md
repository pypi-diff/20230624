# Comparing `tmp/gtnet-0.0.3.tar.gz` & `tmp/gtnet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtnet-0.0.3.tar", last modified: Wed Jun 14 18:38:35 2023, max compression
+gzip compressed data, was "gtnet-0.0.4.tar", last modified: Sat Jun 24 03:53:30 2023, max compression
```

## Comparing `gtnet-0.0.3.tar` & `gtnet-0.0.4.tar`

### file list

```diff
@@ -1,84 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.765445 gtnet-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 18:38:25.000000 gtnet-0.0.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.749445 gtnet-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.749445 gtnet-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/workflows/codespell.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/workflows/deploy_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/workflows/ruff.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/workflows/run_coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-14 18:38:25.000000 gtnet-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-14 18:38:25.000000 gtnet-0.0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-14 18:38:25.000000 gtnet-0.0.3/Legal.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-14 18:38:35.765445 gtnet-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-14 18:38:25.000000 gtnet-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/data/
--rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-14 18:38:26.000000 gtnet-0.0.3/data/GCA_000006155.2.fna
--rw-r--r--   0 runner    (1001) docker     (123)    61553 2023-06-14 18:38:26.000000 gtnet-0.0.3/data/small.fna
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-14 18:38:26.000000 gtnet-0.0.3/data/small.raw.csv
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 18:38:26.000000 gtnet-0.0.3/data/small.tax.0.05.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)    35955 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/accuracy.png
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/api_docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/gtnet-favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)    32999 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/gtnet.png
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/legal.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/performance.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18491 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/runtime.png
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/training.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-14 18:38:26.000000 gtnet-0.0.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-14 18:38:26.000000 gtnet-0.0.3/fetch_model.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-14 18:38:26.000000 gtnet-0.0.3/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-14 18:38:26.000000 gtnet-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-14 18:38:26.000000 gtnet-0.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-14 18:38:26.000000 gtnet-0.0.3/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 18:38:26.000000 gtnet-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:38:35.765445 gtnet-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.749445 gtnet-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/src/gtnet/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/src/gtnet/data/
--rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/data/GCA_000006155.2.fna
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.765445 gtnet-0.0.3/src/gtnet/deploy_pkg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/class.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/class.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/domain.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/domain.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/family.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/family.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/genus.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/genus.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/last.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/order.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/order.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/phylum.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/phylum.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/species.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/species.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/src/gtnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.765445 gtnet-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/tests/test_lca.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/tests/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-14 18:38:26.000000 gtnet-0.0.3/tests/test_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.451022 gtnet-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-24 03:53:21.000000 gtnet-0.0.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.431022 gtnet-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-24 03:53:21.000000 gtnet-0.0.4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-24 03:53:21.000000 gtnet-0.0.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.431022 gtnet-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-24 03:53:21.000000 gtnet-0.0.4/.github/workflows/codespell.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-24 03:53:21.000000 gtnet-0.0.4/.github/workflows/deploy_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-24 03:53:21.000000 gtnet-0.0.4/.github/workflows/ruff.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-24 03:53:21.000000 gtnet-0.0.4/.github/workflows/run_coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-24 03:53:21.000000 gtnet-0.0.4/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-24 03:53:21.000000 gtnet-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-24 03:53:21.000000 gtnet-0.0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-24 03:53:21.000000 gtnet-0.0.4/Legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-24 03:53:30.451022 gtnet-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-24 03:53:21.000000 gtnet-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.439022 gtnet-0.0.4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-24 03:53:21.000000 gtnet-0.0.4/data/GCA_000006155.2.fna
+-rw-r--r--   0 runner    (1001) docker     (123)    61553 2023-06-24 03:53:21.000000 gtnet-0.0.4/data/small.fna
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-24 03:53:21.000000 gtnet-0.0.4/data/small.raw.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-24 03:53:21.000000 gtnet-0.0.4/data/small.seqs.raw.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-24 03:53:21.000000 gtnet-0.0.4/data/small.seqs.tax.0.05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-24 03:53:21.000000 gtnet-0.0.4/data/small.tax.0.05.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.439022 gtnet-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.439022 gtnet-0.0.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    35955 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/accuracy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/api_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/gtnet-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32999 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/gtnet.png
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/legal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18491 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/runtime.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-24 03:53:21.000000 gtnet-0.0.4/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-24 03:53:21.000000 gtnet-0.0.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-24 03:53:21.000000 gtnet-0.0.4/fetch_model.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-24 03:53:21.000000 gtnet-0.0.4/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-24 03:53:21.000000 gtnet-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-24 03:53:21.000000 gtnet-0.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-24 03:53:21.000000 gtnet-0.0.4/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-24 03:53:21.000000 gtnet-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 03:53:30.451022 gtnet-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.431022 gtnet-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.443022 gtnet-0.0.4/src/gtnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.443022 gtnet-0.0.4/src/gtnet/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/data/GCA_000006155.2.fna
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.447022 gtnet-0.0.4/src/gtnet/deploy_pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.447022 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/class.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/class.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/domain.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/domain.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/family.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/family.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/genus.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/genus.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/order.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/order.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/phylum.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/phylum.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/species.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/bins/species.score.pt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.451022 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/class.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/class.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/domain.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/domain.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/family.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/family.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/genus.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/genus.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/order.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/order.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/phylum.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/phylum.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/species.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/contigs/species.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/last.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/deploy_pkg/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-24 03:53:21.000000 gtnet-0.0.4/src/gtnet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.443022 gtnet-0.0.4/src/gtnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-24 03:53:30.000000 gtnet-0.0.4/src/gtnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-24 03:53:30.000000 gtnet-0.0.4/src/gtnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 03:53:30.000000 gtnet-0.0.4/src/gtnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-24 03:53:30.000000 gtnet-0.0.4/src/gtnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-24 03:53:30.000000 gtnet-0.0.4/src/gtnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 03:53:30.000000 gtnet-0.0.4/src/gtnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:30.451022 gtnet-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/tests/test_lca.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:53:21.000000 gtnet-0.0.4/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-24 03:53:21.000000 gtnet-0.0.4/tests/test_sequence.py
```

### Comparing `gtnet-0.0.3/.github/CODE_OF_CONDUCT.md` & `gtnet-0.0.4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/.github/pull_request_template.md` & `gtnet-0.0.4/.github/pull_request_template.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 ```
 Show how to reproduce the new behavior (can be a bug fix or a new feature)
 ```
 
 ## Checklist
 
 - [ ] Did you update CHANGELOG.md with your changes?
-- [ ] Have you checked our [Contributing](https://github.com/hdmf-dev/hdmf-ml/blob/dev/docs/CONTRIBUTING.rst) document?
+- [ ] Have you checked our [Contributing](https://github.com/exabiome/gtnet/blob/dev/docs/CONTRIBUTING.rst) document?
 - [ ] Have you ensured the PR clearly describes the problem and the solution?
 - [ ] Is your contribution compliant with our coding style? This can be checked running `ruff` from the source directory.
-- [ ] Have you checked to ensure that there aren't other open [Pull Requests](https://github.com/hdmf-dev/hdmf-ml/pulls) for the same change?
+- [ ] Have you checked to ensure that there aren't other open [Pull Requests](https://github.com/exabiome/gtnet/pulls) for the same change?
 - [ ] Have you included the relevant issue number using "Fix #XXX" notation where XXX is the issue number? By including "Fix #XXX" you allow GitHub to close issue #XXX when the PR is merged.
```

### Comparing `gtnet-0.0.3/.github/workflows/deploy_release.yml` & `gtnet-0.0.4/.github/workflows/deploy_release.yml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/.github/workflows/run_coverage.yml` & `gtnet-0.0.4/.github/workflows/run_coverage.yml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/.github/workflows/run_tests.yml` & `gtnet-0.0.4/.github/workflows/run_tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     defaults:
       run:
         shell: bash
     strategy:
       fail-fast: false
       matrix:
         include:
-          - { os: ubuntu-latest }
-          - { os: windows-latest }
-          - { os: macos-latest }
+          - { os: ubuntu-latest , opt_req: true }
+          - { os: windows-latest, opt_req: false }
+          - { os: macos-latest  , opt_req: true }
     steps:
       - name: Cancel non-latest runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           all_but_latest: true
           access_token: ${{ github.token }}
 
@@ -43,21 +43,37 @@
           python -m pip install .  # must install in editable mode for coverage to find sources
           python -m pip list
 
       - name: Run tests
         run: |
           pytest
 
-      - name: Run GTNet Predict
+      - name: Run GTNet Predict on Bins
         run: |
           gtnet predict data/small.fna > data/small.raw.test.csv
           python -c 'import pandas as pd; pd.testing.assert_frame_equal(pd.read_csv("data/small.raw.csv"), pd.read_csv("data/small.raw.test.csv"), check_exact=False, atol=1e-4)'
 
-      - name: Run GTNet Filter
+      - name: Run GTNet Filter on Bins
         run: |
           gtnet filter --fpr 0.05 data/small.raw.csv > data/small.tax.test.csv
           python -c 'import pandas as pd; pd.testing.assert_frame_equal(pd.read_csv("data/small.tax.0.05.csv"), pd.read_csv("data/small.tax.test.csv"), check_exact=False, atol=1e-4)'
 
-      - name: Run GTNet Classify
+      - name: Run GTNet Classify on Bins
         run: |
           gtnet classify --fpr 0.05 data/small.fna > data/small.tax.test.csv
           python -c 'import pandas as pd; pd.testing.assert_frame_equal(pd.read_csv("data/small.tax.0.05.csv"), pd.read_csv("data/small.tax.test.csv"), check_exact=False, atol=1e-4)'
+
+      - name: Run GTNet Predict on Contigs
+        run: |
+          gtnet predict --seqs data/small.fna > data/small.seqs.raw.test.csv
+          python -c 'import pandas as pd; pd.testing.assert_frame_equal(pd.read_csv("data/small.seqs.raw.csv"), pd.read_csv("data/small.seqs.raw.test.csv"), check_exact=False, atol=1e-4)'
+
+      - name: Run GTNet Filter on Contigs
+        run: |
+          gtnet filter --fpr 0.05 data/small.seqs.raw.csv > data/small.seqs.tax.test.csv
+          python -c 'import pandas as pd; pd.testing.assert_frame_equal(pd.read_csv("data/small.seqs.tax.0.05.csv"), pd.read_csv("data/small.seqs.tax.test.csv"), check_exact=False, atol=1e-4)'
+
+      - name: Run GTNet Classify on Bins
+        run: |
+          gtnet classify --seqs --fpr 0.05 data/small.fna > data/small.seqs.tax.test.csv
+          python -c 'import pandas as pd; pd.testing.assert_frame_equal(pd.read_csv("data/small.seqs.tax.0.05.csv"), pd.read_csv("data/small.seqs.tax.test.csv"), check_exact=False, atol=1e-4)'
+
```

### Comparing `gtnet-0.0.3/.gitignore` & `gtnet-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/.readthedocs.yaml` & `gtnet-0.0.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/Legal.txt` & `gtnet-0.0.4/Legal.txt`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/PKG-INFO` & `gtnet-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: gtnet
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for running Genome Taxonomy Network predictions
 Author-email: Andrew Tritt <ajtritt@lbl.gov>, Ryan Ly <rly@lbl.gov>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/exabiome/gtnet
 Project-URL: Bug Tracker, https://github.com/exabiome/gtnet/issues
 Keywords: python,microbiome,microbial-taxonomy,cross-platform,open-data,data-format,open-source,open-science,reproducible-research,machine-learning
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `gtnet-0.0.3/README.rst` & `gtnet-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/data/GCA_000006155.2.fna` & `gtnet-0.0.4/data/GCA_000006155.2.fna`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/data/small.fna` & `gtnet-0.0.4/data/small.fna`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/docs/CONTRIBUTING.rst` & `gtnet-0.0.4/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/docs/Makefile` & `gtnet-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/docs/source/accuracy.png` & `gtnet-0.0.4/docs/source/accuracy.png`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/docs/source/conf.py` & `gtnet-0.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/docs/source/gtnet-favicon.png` & `gtnet-0.0.4/docs/source/gtnet-favicon.png`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/docs/source/gtnet.png` & `gtnet-0.0.4/docs/source/gtnet.png`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/docs/source/index.rst` & `gtnet-0.0.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/docs/source/performance.rst` & `gtnet-0.0.4/docs/source/performance.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/docs/source/runtime.png` & `gtnet-0.0.4/docs/source/runtime.png`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/docs/source/training.rst` & `gtnet-0.0.4/docs/source/training.rst`

 * *Files 12% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 ++++++++++++++++
 Once a model is trained, calibrated, and packaged, the deployment package needs to be made publicly available. GTNet is
 currently carried hosted on `OSF <https://osf.io/cwaqs/>`_.
 
 
 Updating the gtnet software
 ---------------------------
-After training a new model and packaging the model, the DeployPkg class will need to be updated with the new URL
-and checksum of the new deployment package. This can be done starting around
+After training a new model and packaging the model, the :py:class:`~gtnet.utils.DeployPkg` class will need to be
+updated with the new URL and checksum of the new deployment package. This can be done starting around
 `here <https://github.com/exabiome/gtnet/blob/b9ba8a4fb1a63affd9047005c92c12799df9c2b7/src/gtnet/utils.py#L36>`_
 in the code.
```

### Comparing `gtnet-0.0.3/environment.yml` & `gtnet-0.0.4/environment.yml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/license.txt` & `gtnet-0.0.4/license.txt`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/pyproject.toml` & `gtnet-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 name = "gtnet"
 authors = [
   { name="Andrew Tritt", email="ajtritt@lbl.gov" },
   { name="Ryan Ly", email="rly@lbl.gov" },
 ]
 description = "A package for running Genome Taxonomy Network predictions"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: BSD License",
     "Development Status :: 2 - Pre-Alpha",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
@@ -42,16 +40,17 @@
     "numpy>=1.24.3",
     "pandas>=2.0.1",
     "torch>=2.0.1",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.package-data]
-gtnet = ["deploy_pkg/*.npz",
-         "deploy_pkg/*.pt",
+gtnet = ["deploy_pkg/{bins,contigs}/*.npz",
+         "deploy_pkg/{bins,contigs}/*.pt",
+         "deploy_pkg/last.pt",
          "deploy_pkg/manifest.json"]
 
 [project.urls]
 "Homepage" = "https://github.com/exabiome/gtnet"
 "Bug Tracker" = "https://github.com/exabiome/gtnet/issues"
 
 [project.scripts]
```

### Comparing `gtnet-0.0.3/requirements-dev.txt` & `gtnet-0.0.4/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/src/gtnet/classify.py` & `gtnet-0.0.4/src/gtnet/classify.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         The command-line arguments to use for running this command
     """
     desc = "Get filtered taxonomic classification for each sequence in a Fasta file."
     epi = ("This command will output a taxonomic classification filtered to a specified false-positive rate "
            "for each sequence")
 
     parser = argparse.ArgumentParser(description=desc, epilog=epi)
-    parser.add_argument('fasta', type=str, help='the Fasta files to do taxonomic classification on')
+    parser.add_argument('fastas', type=str, nargs='+', help='the Fasta files to do taxonomic classification on')
+    parser.add_argument('-s', '--seqs', action='store_true', help='provide classification for sequences')
     parser.add_argument('-c', '--n_chunks', type=int, default=DEFAULT_N_CHUNKS,
                         help='the number of sequence chunks to process at a time')
     parser.add_argument('-o', '--output', type=str, default=None, help='the output file to save classifications to')
     check_cuda(parser)
     parser.add_argument('-f', '--fpr', default=0.05, type=float, help='the false-positive rate to classify to')
     parser.add_argument('-d', '--debug', action='store_true', default=False,
                         help='print specific information about sequences')
@@ -40,21 +41,21 @@
 
     logger = get_logger()
     if args.debug:
         logger.setLevel(logging.DEBUG)
 
     device = check_device(args)
 
-    model, conf_models, train_conf, vocab, rocs = load_deploy_pkg(for_predict=True, for_filter=True)
+    model, conf_models, train_conf, vocab, rocs = load_deploy_pkg(for_predict=True, for_filter=True, contigs=args.seqs)
 
     window = train_conf['window']
     step = train_conf['step']
 
-    logger.info(f'Getting class predictions for each contig in {args.fasta}')
-    output = run_torchscript_inference(args.fasta, model, conf_models, window, step, vocab,
+    logger.info(f'Getting class predictions for each contig in {",".join(args.fastas)}')
+    output = run_torchscript_inference(args.fastas, model, conf_models, window, step, vocab, seqs=args.seqs,
                                       device=device, logger=logger)
 
     logger.info(f'Getting probability cutoffs for target false-positive rate of {args.fpr}')
     cutoffs = get_cutoffs(rocs, args.fpr)
 
     logger.info('Filtering class predictions')
     output = filter_predictions(output, cutoffs)
```

### Comparing `gtnet-0.0.3/src/gtnet/data/GCA_000006155.2.fna` & `gtnet-0.0.4/src/gtnet/data/GCA_000006155.2.fna`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/src/gtnet/filter.py` & `gtnet-0.0.4/src/gtnet/filter.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,19 +49,26 @@
     before = time()
 
     if args.csv is None:
         args.csv = sys.stdin
 
     logger = get_logger()
 
-    rocs = load_deploy_pkg(for_filter=True)
+    df = pd.read_csv(args.csv)
 
-    cutoffs = get_cutoffs(rocs, args.fpr)
+    if 'ID' in df.columns:
+        seqs = True
+        df = df.set_index(['file', 'ID'])
+    else:
+        df = df.set_index('file')
+        seqs = False
+
+    rocs = load_deploy_pkg(for_filter=True, contigs=seqs)
 
-    df = pd.read_csv(args.csv, index_col='ID')
+    cutoffs = get_cutoffs(rocs, args.fpr)
 
     output = filter_predictions(df, cutoffs)
     write_csv(output, args)
 
     after = time()
     logger.info(f'Took {after - before:.1f} seconds')
```

### Comparing `gtnet-0.0.3/src/gtnet/main.py` & `gtnet-0.0.4/src/gtnet/main.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/src/gtnet/predict.py` & `gtnet-0.0.4/src/gtnet/predict.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+from collections import Counter
 import logging
 from time import time
 
 import pandas as pd
 import torch
 
 from .sequence import FastaReader, FastaSequenceEncoder
@@ -24,15 +25,16 @@
     """
     desc = "Get network predictions for each sequence in a Fasta file"
     epi = ("This command will output the best classification for every sequence at every taxonomic level, including "
            "confidence scores for each taxonomic level. These classifications can be subsequently filtered using the "
            "'filter' command. See the 'classify' command for getting pre-filtered classifications")
 
     parser = argparse.ArgumentParser(description=desc, epilog=epi)
-    parser.add_argument('fasta', type=str, help='the Fasta files to do taxonomic classification on')
+    parser.add_argument('fastas', type=str, nargs='+', help='the Fasta files to do taxonomic classification on')
+    parser.add_argument('-s', '--seqs', action='store_true', help='provide classification for sequences')
     parser.add_argument('-c', '--n_chunks', type=int, default=DEFAULT_N_CHUNKS,
                         help='the number of sequence chunks to process at a time')
     parser.add_argument('-o', '--output', type=str, default=None, help='the output file to save classifications to')
     check_cuda(parser)
     parser.add_argument('-d', '--debug', action='store_true', default=False,
                         help='print specific information about sequences')
 
@@ -42,36 +44,37 @@
 
     logger = get_logger()
     if args.debug:
         logger.setLevel(logging.DEBUG)
 
     device = check_device(args)
 
-    model, conf_models, train_conf, vocab = load_deploy_pkg(for_predict=True)
+    model, conf_models, train_conf, vocab = load_deploy_pkg(for_predict=True, contigs=args.seqs)
 
     window = train_conf['window']
     step = train_conf['step']
 
-    output = run_torchscript_inference(args.fasta, model, conf_models, window, step, vocab, device=device)
+    output = run_torchscript_inference(args.fastas, model, conf_models, window, step, vocab, seqs=args.seqs,
+                                       device=device, logger=logger)
 
     # write out data
     write_csv(output, args)
 
     after = time()
     logger.info(f'Took {after - before:.1f} seconds')
 
 
-def run_torchscript_inference(fasta, model, conf_models, window, step, vocab, n_chunks=DEFAULT_N_CHUNKS,
+def run_torchscript_inference(fastas, model, conf_models, window, step, vocab, seqs=False, n_chunks=DEFAULT_N_CHUNKS,
                               device=torch.device('cpu'), logger=None):
     """Run Torchscript inference
 
     Parameters
     ----------
 
-    fasta : str
+    fastas : str
         The path to the Fasta file with sequences to do inference on
 
     model : RecursiveScriptModule
         The Torchscript model to run inference with
 
     conf_models : dict
         A dictionary with the confidence model for each taxonomic level. Each model should be a RecursiveScriptModule.
@@ -97,55 +100,97 @@
     """
 
     if logger is None:
         logger = get_logger()
         logger.setLevel(logging.CRITICAL)
 
     encoder = FastaSequenceEncoder(window, step, vocab=vocab, device=device)
-    reader = FastaReader(encoder, fasta)
+    reader = FastaReader(encoder, *fastas)
 
     model = model.to(device)
 
     output_size = sum(len(lvl['taxa']) for lvl in conf_models.values())
 
     seqnames = list()
     lengths = list()
+    total_chunks = list()
     filepaths = list()
     aggregated = list()
 
     torch.set_grad_enabled(False)
 
-    logger.info(f'Calculating classifications for all sequences in {fasta}')
+
+    logger.info(f'Calculating classifications for all sequences in {", ".join(fastas)}')
     for file_path, seq_name, seq_len, seq_chunks in reader:
         seqnames.append(seq_name)
         lengths.append(seq_len)
         filepaths.append(file_path)
 
         logger.debug((f'Getting predictions for windows of {seqnames[-1]}, '
                       f'{seq_chunks.shape[1] * 2} chunks, {lengths[-1]} bases'))
         outputs = torch.zeros(output_size, device=device)   # the output from the network for a single sequence
         # sum network outputs from all chunks
-        for s in range(0, len(seq_chunks), n_chunks):
+        for s in range(0, seq_chunks.shape[1], n_chunks):
             e = s + n_chunks
             outputs += model(seq_chunks[0, s:e]).sum(dim=0)
             outputs += model(seq_chunks[1, s:e]).sum(dim=0)
         # divide by the number of seq_chunks we processed to get a mean output
-        outputs /= (seq_chunks.shape[1] * 2)
-        del seq_chunks
-
         aggregated.append(outputs)
+        total_chunks.append(seq_chunks.shape[1] * 2.)
 
-    lengths = torch.tensor(lengths, device=device)
+        del seq_chunks
 
+    total_chunks = torch.tensor(total_chunks, device=device)
 
     # aggregate everything we just pulled from the fasta file
     all_levels_aggregated = torch.row_stack(aggregated)
     del aggregated
 
-    output_data = {'ID': seqnames}
+    if not seqs:
+        logger.info('Calculating classifications for bins')
+
+        ctr = Counter(filepaths)
+        n_ctgs = list(ctr.values())
+        filepaths = list(ctr.keys())
+
+        max_len = list()
+        l50 = list()
+        lengths = torch.tensor(lengths)
+
+        tmp_chunks = list()
+        tmp_aggregated = list()
+
+        s = 0
+        for n in n_ctgs:
+            e = s + n
+            tmp_lens = lengths[s:e].sort(descending=True).values
+            max_len.append(tmp_lens[0])
+            csum = torch.cumsum(tmp_lens, 0)
+            l50.append(tmp_lens[torch.where(csum > (csum[-1] * 0.5))[0][0]])
+            tmp_aggregated.append(all_levels_aggregated[s:e].sum(axis=0))
+            tmp_chunks.append(total_chunks[s:e].sum())
+            s = e
+
+        del total_chunks
+        total_chunks = torch.tensor(tmp_chunks)
+        del tmp_chunks
+
+        del all_levels_aggregated
+        all_levels_aggregated = torch.row_stack(tmp_aggregated)
+        del tmp_aggregated
+
+        features = torch.tensor([n_ctgs, l50, max_len], device=device).T
+        output_data = {'file': filepaths}
+    else:
+        features = torch.tensor(lengths, device=device)[:, None]
+        output_data = {'file': filepaths, 'ID': seqnames}
+
+
+    all_levels_aggregated = ((all_levels_aggregated.T) / total_chunks).T
+    indices = list(output_data.keys())
 
     s = 0
     for lvl, e in zip(model.levels, model.parse):
         conf_model_info = conf_models[lvl]
         taxa = conf_model_info['taxa']
         conf_model = conf_model_info['model'].to(device)
 
@@ -159,17 +204,17 @@
 
         # get prediction and maximum probabilities for confidence scoring
         logger.debug(f'Getting max {top_k} probabilities for {lvl}')
         maxprobs = torch.topk(aggregated, top_k, dim=1, largest=True, sorted=True).values
 
         # build input matrix for confidence model
         logger.debug('Calculating confidence probabilities')
-        conf_input = torch.column_stack([lengths, maxprobs])
+        conf_input = torch.column_stack([features, maxprobs])
 
         output_data[f'{lvl}_prob'] = conf_model(conf_input).cpu().numpy().squeeze()
 
         # set next left bound for all_levels_aggregated
         s = e
 
-    output = pd.DataFrame(output_data).set_index('ID')
+    output = pd.DataFrame(output_data).set_index(indices)
 
     return output
```

### Comparing `gtnet-0.0.3/src/gtnet/sequence.py` & `gtnet-0.0.4/src/gtnet/sequence.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.3/src/gtnet/utils.py` & `gtnet-0.0.4/src/gtnet/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import glob
 import hashlib
 from importlib.resources import files
 import json
 import logging
 import os
 import sys
 import urllib
@@ -30,24 +29,24 @@
 def get_logger():
     return parse_logger('')
 
 
 class DeployPkg:
     """A class to handle loading and manipulating the deployment package"""
 
-    _deploy_pkg_url = "https://osf.io/download/mwgb9/"
+    _deploy_pkg_url = "https://osf.io/download/qf46x/"
 
-    _checksum = "0245fcf825bfe4de0770fcb46798ca90"
+    _checksum = "623aa991fb0d74e874b7d0da25496c26"
+
+    _manifest_name = 'manifest.json'
 
     @classmethod
     def check_pkg(cls):
         deploy_dir = files(__package__).joinpath('deploy_pkg')
-        total = 0
-        for path in glob.glob(f"{deploy_dir}/*"):
-            total += os.path.getsize(path)
+        total = os.path.getsize(os.path.join(deploy_dir, cls._manifest_name))
         if total == 0:
             msg = ("Downloading GTNet deployment package. This will only happen on the first invocation "
                    "of gtnet predict or gtnet classify")
             warnings.warn(msg)
             zip_path = files(__package__).joinpath('deploy_pkg.zip')
             urllib.request.urlretrieve(cls._deploy_pkg_url, zip_path)
             dl_checksum = hashlib.md5(open(zip_path,'rb').read()).hexdigest()
@@ -67,51 +66,54 @@
     def path(self, path):
         """Map paths to be relative to current working directory"""
         return os.path.join(self.deploy_dir, path)
 
     @property
     def manifest(self):
         if self._manifest is None:
-            with open(self.path('manifest.json'), 'r') as f:
+            with open(self.path(self._manifest_name), 'r') as f:
                 self._manifest = json.load(f)
         return self._manifest
 
     def __getitem__(self, key):
         return self.manifest[key]
 
     def __setitem__(self, key, val):
         self.manifest[key] = val
 
 
-def load_deploy_pkg(for_predict=False, for_filter=False):
+def load_deploy_pkg(for_predict=False, for_filter=False, contigs=False):
     if not (for_predict or for_filter):
         for_predict = True
         for_filter = True
 
     pkg = DeployPkg()
+    key = 'contigs' if contigs else 'bins'
 
     ret = list()
     if for_predict:
         tmp_conf_model = dict()
-        for lvl_dat in pkg['conf_model']:
-            lvl_dat['taxa'] = np.array(lvl_dat['taxa'])
+        for cm_data, taxa_data in zip(pkg['conf_model'][key], pkg['taxa']):
+            if cm_data['level'] != taxa_data['level']:
+                raise ValueError("Taxonomic levels are out of order in manifest file")
+            cm_data['taxa'] = np.array(taxa_data['taxa'])
 
-            lvl_dat['model'] = torch.jit.load(pkg.path(lvl_dat.pop('model')))
+            cm_data['model'] = torch.jit.load(pkg.path(cm_data.pop('model')))
 
-            tmp_conf_model[lvl_dat['level']] = lvl_dat
+            tmp_conf_model[cm_data['level']] = cm_data
 
         ret.append(torch.jit.load(pkg.path(pkg['nn_model'])))
         ret.append(tmp_conf_model)
         ret.append(pkg['training_config'])
         ret.append("".join(pkg['vocabulary']))
 
     if for_filter:
         tmp_roc = dict()
-        for lvl_dat in pkg['conf_model']:
-            tmp_roc[lvl_dat['level']] = np.load(pkg.path(lvl_dat['roc']))
+        for cm_data in pkg['conf_model'][key]:
+            tmp_roc[cm_data['level']] = np.load(pkg.path(cm_data['roc']))
         ret.append(tmp_roc)
 
     return tuple(ret) if len(ret) > 1 else ret[0]
 
 
 class GPUModel(nn.Module):
```

### Comparing `gtnet-0.0.3/src/gtnet.egg-info/PKG-INFO` & `gtnet-0.0.4/src/gtnet.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: gtnet
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for running Genome Taxonomy Network predictions
 Author-email: Andrew Tritt <ajtritt@lbl.gov>, Ryan Ly <rly@lbl.gov>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/exabiome/gtnet
 Project-URL: Bug Tracker, https://github.com/exabiome/gtnet/issues
 Keywords: python,microbiome,microbial-taxonomy,cross-platform,open-data,data-format,open-source,open-science,reproducible-research,machine-learning
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `gtnet-0.0.3/tests/test_sequence.py` & `gtnet-0.0.4/tests/test_sequence.py`

 * *Files identical despite different names*

