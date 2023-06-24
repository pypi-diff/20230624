# Comparing `tmp/tfsim-nightly-0.18.0.dev5.tar.gz` & `tmp/tfsim-nightly-0.18.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfsim-nightly-0.18.0.dev5.tar", last modified: Thu Jun  1 03:23:23 2023, max compression
+gzip compressed data, was "tfsim-nightly-0.18.0.dev6.tar", last modified: Sat Jun 24 03:19:09 2023, max compression
```

## Comparing `tfsim-nightly-0.18.0.dev5.tar` & `tfsim-nightly-0.18.0.dev6.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.047057 tfsim-nightly-0.18.0.dev5/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-01 03:23:23.047057 tfsim-nightly-0.18.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 03:23:23.047057 tfsim-nightly-0.18.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.031057 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-01 03:23:20.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.031057 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.031057 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/architectures/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/architectures/resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/architectures/resnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/architectures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.031057 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.031057 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/cropping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/barlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16121 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/base_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.035056 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/binary_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/classification_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/false_positive_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/negative_predictive_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/distances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.035056 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/evaluators/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/evaluators/memory_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.035056 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/barlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/circle_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/metric_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/multinegrank_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/multisim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/pn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/simsiam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/softnn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/triplet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/vicreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/xbm_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.035056 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/matchers/classification_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/matchers/match_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/matchers/match_nearest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/matchers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.035056 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/models/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39080 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/models/contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31807 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/models/similarity_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.035056 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/bndcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/map_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/precision_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/recall_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/retrieval_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.039057 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/file_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/memory_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/tfdata_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/tfdataset_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/tfrecords_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/schedules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.039057 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/faiss_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/linear_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/nmslib_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.039057 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/cached_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.039057 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/training_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/training_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/training_metrics/distance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/training_metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.039057 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/visualization/confusion_matrix_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/visualization/neighbors_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/visualization/projector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tensorflow_similarity/visualization/vizualize_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.039057 tfsim-nightly-0.18.0.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.043057 tfsim-nightly-0.18.0.dev5/tests/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/architectures/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/architectures/test_resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/architectures/test_resnet50.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.043057 tfsim-nightly-0.18.0.dev5/tests/classification_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/classification_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/classification_metrics/test_classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.043057 tfsim-nightly-0.18.0.dev5/tests/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/evaluators/test_memory_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.043057 tfsim-nightly-0.18.0.dev5/tests/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/losses/test_pn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/losses/test_softnn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/losses/test_triplet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/losses/test_xbm_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.043057 tfsim-nightly-0.18.0.dev5/tests/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/matchers/test_classification_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/matchers/test_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/matchers/test_match_nearest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.043057 tfsim-nightly-0.18.0.dev5/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/models/test_contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/models/test_similarity_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.043057 tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/test_bndcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/test_map_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/test_precision_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/test_recall_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/test_retrieval_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.043057 tfsim-nightly-0.18.0.dev5/tests/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/samplers/test_file_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/samplers/test_memory_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/samplers/test_tfdata_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/samplers/test_tfdataset_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/samplers/test_tfrecord_samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.043057 tfsim-nightly-0.18.0.dev5/tests/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/search/test_faiss_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/search/test_linear_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/search/test_nmslib_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.043057 tfsim-nightly-0.18.0.dev5/tests/stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/stores/test_cached_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/stores/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/stores/test_redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/test_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/test_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/test_schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.043057 tfsim-nightly-0.18.0.dev5/tests/training_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/training_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/training_metrics/test_distance_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.047057 tfsim-nightly-0.18.0.dev5/tests/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/visualization/test_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-01 03:21:24.000000 tfsim-nightly-0.18.0.dev5/tests/visualization/test_neighbors_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:23:23.047057 tfsim-nightly-0.18.0.dev5/tfsim_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-01 03:23:22.000000 tfsim-nightly-0.18.0.dev5/tfsim_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-01 03:23:22.000000 tfsim-nightly-0.18.0.dev5/tfsim_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 03:23:22.000000 tfsim-nightly-0.18.0.dev5/tfsim_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-01 03:23:22.000000 tfsim-nightly-0.18.0.dev5/tfsim_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 03:23:22.000000 tfsim-nightly-0.18.0.dev5/tfsim_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.647595 tfsim-nightly-0.18.0.dev6/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-24 03:19:09.647595 tfsim-nightly-0.18.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 03:19:09.647595 tfsim-nightly-0.18.0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.631594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-24 03:19:08.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.631594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.631594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/architectures/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/architectures/resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/architectures/resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/architectures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.635594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.635594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/cropping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/barlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/base_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.635594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/binary_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/classification_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/false_positive_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/negative_predictive_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/distances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.635594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/evaluators/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/evaluators/memory_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.635594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/barlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/circle_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/metric_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/multinegrank_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/multisim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/pn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/simsiam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/softnn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/triplet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/vicreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/xbm_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.635594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/matchers/classification_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/matchers/match_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/matchers/match_nearest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/matchers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.639594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39080 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/models/contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31807 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/models/similarity_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.639594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/bndcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/map_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/precision_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/recall_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/retrieval_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.639594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/file_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/memory_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/tfdata_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/tfdataset_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/tfrecords_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/schedules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.639594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/faiss_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/linear_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/nmslib_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.639594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/cached_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.639594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/training_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/training_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/training_metrics/distance_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/training_metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.639594 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/visualization/confusion_matrix_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/visualization/neighbors_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/visualization/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tensorflow_similarity/visualization/vizualize_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.643595 tfsim-nightly-0.18.0.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.643595 tfsim-nightly-0.18.0.dev6/tests/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/architectures/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/architectures/test_resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/architectures/test_resnet50.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.643595 tfsim-nightly-0.18.0.dev6/tests/classification_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/classification_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/classification_metrics/test_classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.643595 tfsim-nightly-0.18.0.dev6/tests/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/evaluators/test_memory_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.643595 tfsim-nightly-0.18.0.dev6/tests/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/losses/test_pn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/losses/test_softnn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/losses/test_triplet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/losses/test_xbm_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.643595 tfsim-nightly-0.18.0.dev6/tests/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/matchers/test_classification_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/matchers/test_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/matchers/test_match_nearest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.643595 tfsim-nightly-0.18.0.dev6/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/models/test_contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/models/test_similarity_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.643595 tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/test_bndcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/test_map_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/test_precision_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/test_recall_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/test_retrieval_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.643595 tfsim-nightly-0.18.0.dev6/tests/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/samplers/test_file_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/samplers/test_memory_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/samplers/test_tfdata_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/samplers/test_tfdataset_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/samplers/test_tfrecord_samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.643595 tfsim-nightly-0.18.0.dev6/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/search/test_faiss_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/search/test_linear_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/search/test_nmslib_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.643595 tfsim-nightly-0.18.0.dev6/tests/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/stores/test_cached_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/stores/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/stores/test_redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/test_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/test_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/test_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.647595 tfsim-nightly-0.18.0.dev6/tests/training_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/training_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/training_metrics/test_distance_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.647595 tfsim-nightly-0.18.0.dev6/tests/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/visualization/test_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-24 03:17:18.000000 tfsim-nightly-0.18.0.dev6/tests/visualization/test_neighbors_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 03:19:09.647595 tfsim-nightly-0.18.0.dev6/tfsim_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-24 03:19:09.000000 tfsim-nightly-0.18.0.dev6/tfsim_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-24 03:19:09.000000 tfsim-nightly-0.18.0.dev6/tfsim_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 03:19:09.000000 tfsim-nightly-0.18.0.dev6/tfsim_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-24 03:19:09.000000 tfsim-nightly-0.18.0.dev6/tfsim_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-24 03:19:09.000000 tfsim-nightly-0.18.0.dev6/tfsim_nightly.egg-info/top_level.txt
```

### Comparing `tfsim-nightly-0.18.0.dev5/LICENSE` & `tfsim-nightly-0.18.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/PKG-INFO` & `tfsim-nightly-0.18.0.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfsim-nightly
-Version: 0.18.0.dev5
+Version: 0.18.0.dev6
 Summary: Metric Learning for Humans
 Home-page: https://github.com/tensorflow/similarity
 Author: Tensorflow Similarity authors
 Author-email: tf-similarity@google.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tfsim-nightly-0.18.0.dev5/README.md` & `tfsim-nightly-0.18.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/setup.py` & `tfsim-nightly-0.18.0.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.18.0.dev5"
+__version__ = "0.18.0.dev6"
 
 
 from . import algebra  # noqa
 from . import architectures  # noqa
 from . import augmenters  # noqa
 from . import callbacks  # noqa
 from . import classification_metrics  # noqa
```

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/algebra.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/algebra.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/api/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/architectures/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/architectures/efficientnet.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/architectures/efficientnet.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/architectures/resnet18.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/architectures/resnet18.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/architectures/resnet50.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/architectures/resnet50.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/architectures/utils.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/architectures/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/blur.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/blur.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/cropping.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/cropping.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/flip.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/flip.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmentation_utils/solarize.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmentation_utils/solarize.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/augmenter.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/augmenter.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/barlow.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/barlow.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,14 @@
     def augment(
         self,
         x: Any,
         y: Any = None,
         num_augmentations_per_example: int = 2,
         is_warmup: bool = True,
     ) -> list[Any]:
-
         with tf.device("/cpu:0"):
             if y is None:
                 y = tf.constant([0])
             inputs = tf.stack(x)
             inputs = tf.cast(inputs, dtype="float32")
 
             views = []
@@ -158,15 +157,14 @@
                 blur_max_sigma=self.blur_max_sigma,
                 solarize_probability=self.solarize_probability,
                 solarize_pixel_min=self.solarize_pixel_min,
                 solarize_pixel_max=self.solarize_pixel_max,
                 solarize_thresh=self.solarize_thresh,
             )
             for _ in range(num_augmentations_per_example):
-
                 view = tf.map_fn(
                     lambda img: augment_fn(image=img),
                     inputs,
                     parallel_iterations=self.num_cpu,
                 )
                 views.append(view)
         return views
```

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/contrastive.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/contrastive.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/augmenters/simclr.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/augmenters/simclr.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,14 @@
         jitter_stength: float = 1.0,
         crop: bool = True,
         eval_crop_proportion: float = 0.875,  # imagenet standard
         flip: bool = True,
         version: str = "v2",
         num_cpu: int | None = os.cpu_count(),
     ):
-
         self.width = width
         self.height = height
         self.is_training = is_training
         self.color_distort = color_distort
         self.jitter_stength = jitter_stength
         self.crop = crop
         self.eval_crop_proportion = eval_crop_proportion
@@ -128,15 +127,14 @@
         if self.is_training:
             self.augment_img = self._train_augment_img
         else:
             self.augment_img = self._eval_augment_img
 
     @tf.function
     def augment(self, x: Tensor, y: Tensor, num_views: int, is_warmup: bool) -> list[Tensor]:
-
         with tf.device("/cpu:0"):
             inputs = tf.stack(x)
             inputs = tf.cast(inputs, dtype="float32") / 255.0
             views = []
 
             for _ in range(num_views):
                 # multi-cor augementations
```

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/base_indexer.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/base_indexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,15 +427,14 @@
         Returns
             list of the k nearest neighbors info:
             list[Lookup]
         """
 
     @abstractmethod
     def batch_lookup(self, predictions: FloatTensor, k: int = 5, verbose: int = 1) -> list[list[Lookup]]:
-
         """Find the k closest matches for a set of embeddings
 
         Args:
             predictions: TF similarity model predictions, may be a multi-headed
             output.
 
             k: Number of nearest neighbors to lookup. Defaults to 5.
```

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/callbacks.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/callbacks.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/binary_accuracy.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/binary_accuracy.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/classification_metric.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/classification_metric.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/f1_score.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/f1_score.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/false_positive_rate.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/false_positive_rate.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/negative_predictive_value.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/negative_predictive_value.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/precision.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/precision.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/recall.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/recall.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/classification_metrics/utils.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/classification_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/distances.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/distances.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/evaluators/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/evaluators/evaluator.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/evaluators/evaluator.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/evaluators/memory_evaluator.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/evaluators/memory_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,14 @@
             idx = self._last_argmin(metrics[calibration_metric.name])
 
         optimal_cp = {
             "name": "optimal",
             "value": metrics[calibration_metric.name][idx].item(),
         }
         for metric_name in metrics.keys():
-
             optimal_cp[metric_name] = metrics[metric_name][idx].item()
 
         return optimal_cp
 
     def _target_cutpoints(
         self,
         metrics: dict[str, np.ndarray],
```

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/indexer.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/indexer.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/layers.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/layers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/barlow.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/barlow.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/circle_loss.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/circle_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/metric_loss.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/metric_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/multinegrank_loss.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/multinegrank_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/multisim_loss.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/multisim_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/pn_loss.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/pn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/simclr.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/simclr.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     LARGE_NUM = 1e9
 
     def __init__(self, temperature: float = 0.05, **kwargs):
         super().__init__(**kwargs)
         self.temperature = temperature
 
     def contrast(self, hidden1: FloatTensor, hidden2: FloatTensor) -> FloatTensor:
-
         # local replica batch size
         batch_size = tf.shape(hidden1)[0]
 
         if not tf.distribute.in_cross_replica_context():
             # SimCLR loss computes similarity with 2N-1 other examples, when N is the global_batch_size.
             # In distributed training, each replica sees only N/n_replicas examples and to compare with all 2N-1
             # examples we must first get them from other replicas.
```

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/simsiam.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/simsiam.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/softnn_loss.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/softnn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/triplet_loss.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/triplet_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/utils.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/vicreg.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/vicreg.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/losses/xbm_loss.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/losses/xbm_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/matchers/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/matchers/classification_match.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/matchers/classification_match.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/matchers/match_majority_vote.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/matchers/match_majority_vote.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from .classification_match import ClassificationMatch
 
 
 class MatchMajorityVote(ClassificationMatch):
     """Match metrics for the most common label in a result set."""
 
     def __init__(self, name: str = "majority_vote", **kwargs) -> None:
-
         if "canonical_name" not in kwargs:
             kwargs["canonical_name"] = "match_majority_vote"
 
         super().__init__(name=name, **kwargs)
 
     def derive_match(self, lookup_labels: IntTensor, lookup_distances: FloatTensor) -> tuple[IntTensor, FloatTensor]:
         """Derive a match label and distance from a set of K neighbors.
```

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/matchers/match_nearest.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/matchers/match_nearest.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from .classification_match import ClassificationMatch
 
 
 class MatchNearest(ClassificationMatch):
     """Match metrics for labels at k=1."""
 
     def __init__(self, name: str = "nearest", **kwargs) -> None:
-
         if "canonical_name" not in kwargs:
             kwargs["canonical_name"] = "match_nearest"
 
         super().__init__(name=name, **kwargs)
 
     def derive_match(self, lookup_labels: IntTensor, lookup_distances: FloatTensor) -> tuple[IntTensor, FloatTensor]:
         """Derive a match label and distance from a set of K neighbors.
```

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/matchers/utils.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/matchers/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/models/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/models/contrastive_model.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/models/contrastive_model.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/models/similarity_model.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/models/similarity_model.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/bndcg.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/bndcg.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/map_at_k.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/map_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/precision_at_k.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/precision_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/recall_at_k.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/recall_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/retrieval_metric.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/retrieval_metrics/utils.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/retrieval_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/file_samplers.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/file_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/memory_samplers.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/memory_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/samplers.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/tfdata_sampler.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/tfdata_sampler.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/tfdataset_samplers.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/tfdataset_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/tfrecords_samplers.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/tfrecords_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/samplers/utils.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/samplers/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/schedules.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/schedules.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/faiss_search.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/faiss_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/linear_search.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/linear_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/nmslib_search.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/nmslib_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/search.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/search/utils.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/search/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/cached_store.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/cached_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/memory_store.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/memory_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/redis_store.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/redis_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/store.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/stores/utils.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/stores/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/training_metrics/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/training_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/training_metrics/distance_metrics.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/training_metrics/distance_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         aggregate: str = "mean",
         anchor: str = "positive",
         name: str | None = None,
         positive_mining_strategy: str = "hard",
         negative_mining_strategy: str = "hard",
         **kwargs,
     ):
-
         if not name:
             name = "%s_%s" % (aggregate, anchor[:3])
         super().__init__(name=name, **kwargs)
 
         self.distance = distance_canonicalizer(distance)
 
         if anchor not in ["positive", "negative"]:
@@ -59,15 +58,14 @@
             raise ValueError("Invalid reduction")
         self.aggregate = aggregate
 
         # result variable
         self.aggregated_distances = tf.Variable(0, dtype=tf.keras.backend.floatx())
 
     def update_state(self, labels: IntTensor, embeddings: FloatTensor, sample_weight: FloatTensor) -> None:
-
         # [distances]
         pairwise_distances = self.distance(embeddings, embeddings)
 
         # [mask]
         batch_size = tf.size(labels)
         positive_mask, negative_mask = build_masks(labels, labels, batch_size)
```

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/training_metrics/utils.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/training_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/types.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/types.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/utils.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/visualization/__init__.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/visualization/confusion_matrix_viz.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/visualization/confusion_matrix_viz.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/visualization/neighbors_viz.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/visualization/neighbors_viz.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/visualization/projector.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/visualization/projector.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tensorflow_similarity/visualization/vizualize_views.py` & `tfsim-nightly-0.18.0.dev6/tensorflow_similarity/visualization/vizualize_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     num_col = views_per_col
     num_row = num_imgs // num_col
     num_row = num_row + 1 if num_imgs % num_col else num_row
 
     # Plot the images
     fig, axes = plt.subplots(num_row, num_col, figsize=fig_size)
     for i in range(num_imgs):
-
         # If the number of rows is 1, the axes array is one-dimensional
         if num_row == 1:
             ax = axes[i % num_col]
         else:
             ax = axes[i // num_col, i % num_col]
 
         scale = abs(max_pixel_value - min_pixel_value)
```

### Comparing `tfsim-nightly-0.18.0.dev5/tests/architectures/test_efficientnet.py` & `tfsim-nightly-0.18.0.dev6/tests/architectures/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/architectures/test_resnet18.py` & `tfsim-nightly-0.18.0.dev6/tests/architectures/test_resnet18.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/architectures/test_resnet50.py` & `tfsim-nightly-0.18.0.dev6/tests/architectures/test_resnet50.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/classification_metrics/test_classification_metrics.py` & `tfsim-nightly-0.18.0.dev6/tests/classification_metrics/test_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/evaluators/test_memory_evaluator.py` & `tfsim-nightly-0.18.0.dev6/tests/evaluators/test_memory_evaluator.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/losses/test_pn_loss.py` & `tfsim-nightly-0.18.0.dev6/tests/losses/test_pn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/losses/test_softnn_loss.py` & `tfsim-nightly-0.18.0.dev6/tests/losses/test_softnn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/losses/test_triplet_loss.py` & `tfsim-nightly-0.18.0.dev6/tests/losses/test_triplet_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/losses/test_xbm_loss.py` & `tfsim-nightly-0.18.0.dev6/tests/losses/test_xbm_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/losses/utils.py` & `tfsim-nightly-0.18.0.dev6/tests/losses/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/matchers/test_classification_match.py` & `tfsim-nightly-0.18.0.dev6/tests/matchers/test_classification_match.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/matchers/test_majority_vote.py` & `tfsim-nightly-0.18.0.dev6/tests/matchers/test_majority_vote.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/matchers/test_match_nearest.py` & `tfsim-nightly-0.18.0.dev6/tests/matchers/test_match_nearest.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/models/test_contrastive_model.py` & `tfsim-nightly-0.18.0.dev6/tests/models/test_contrastive_model.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/models/test_similarity_model.py` & `tfsim-nightly-0.18.0.dev6/tests/models/test_similarity_model.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/test_bndcg.py` & `tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/test_bndcg.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/test_map_at_k.py` & `tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/test_map_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/test_precision_at_k.py` & `tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/test_precision_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/test_recall_at_k.py` & `tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/test_recall_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/retrieval_metrics/test_retrieval_metric.py` & `tfsim-nightly-0.18.0.dev6/tests/retrieval_metrics/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/samplers/test_file_samplers.py` & `tfsim-nightly-0.18.0.dev6/tests/samplers/test_file_samplers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,142 @@
 import os
 import re
+import sys
 import tempfile
 
 import numpy as np
 import pytest
 import tensorflow as tf
 
 from tensorflow_similarity.samplers import MultiShotFileSampler
 
 
-def _create_random_image(filename, size=(32, 32)):
-    filepath = os.path.join(tempfile.gettempdir(), filename)
-    image = np.random.random(size + (3,)).astype(np.float32)
-    tf.keras.utils.save_img(filepath, image)
-    return filepath
-
-
-@pytest.mark.parametrize("example_per_class", [2, 20])
-def test_multi_shot_file_sampler(example_per_class):
-    """Test MultiShotFileSampler with various sizes.
-
-    Users may sample with replacement when creating batches, so check that we
-    can handle when elements per class is either less than or greater than the
-    total count of elements in the class.
-    """
-    filenames = ["1.jpg", "2.jpg", "3.jpg", "4.jpg", "5.jpg", "6.jpg"]
-    filepaths = [_create_random_image(filename) for filename in filenames]
-    images = [np.array(tf.keras.utils.load_img(path), dtype=np.float32) / 255 for path in filepaths]
-
-    y = tf.constant([1, 2, 3, 1, 2, 3])
-    x = tf.constant(filepaths)
-    class_per_batch = 2
-    batch_size = example_per_class * class_per_batch
-
-    fs_sampler = MultiShotFileSampler(
-        x=x,
-        y=y,
-        classes_per_batch=class_per_batch,
-        examples_per_class_per_batch=example_per_class,
-    )  # noqa
-
-    batch_x, batch_y = fs_sampler.generate_batch(batch_id=606)
-
-    assert len(batch_y) == batch_size
-    assert len(batch_x) == batch_size
-    num_classes, _ = tf.unique(batch_y)
-    assert len(num_classes) == class_per_batch
-
-    for x, y in zip(batch_x, batch_y):
-        if y == 1:
-            assert np.isclose(x.numpy(), images[0], atol=0.1).all() or np.isclose(x.numpy(), images[3], atol=0.1).all()
-        elif y == 2:
-            assert np.isclose(x.numpy(), images[1], atol=0.1).all() or np.isclose(x.numpy(), images[4], atol=0.1).all()
-        elif y == 3:
-            assert np.isclose(x.numpy(), images[2], atol=0.1).all() or np.isclose(x.numpy(), images[5], atol=0.1).all()
-
-
-def test_msfs_get_slice():
-    """Test the multi shot file sampler get_slice method."""
-    filenames = ["1.jpg", "2.jpg", "3.jpg", "4.jpg"]
-    filepaths = [_create_random_image(filename) for filename in filenames]
-    images = [np.array(tf.keras.utils.load_img(path), dtype=np.float32) / 255 for path in filepaths]
-
-    y = tf.constant(range(4))
-    x = tf.constant(filepaths)
-
-    fs_sampler = MultiShotFileSampler(x=x, y=y)
-    # x and y are randomly shuffled so we fix the values here.
-    fs_sampler._x = x
-    fs_sampler._y = y
-    slice_x, slice_y = fs_sampler.get_slice(1, 2)
-
-    assert slice_x.shape == (2, 32, 32, 3)
-    assert slice_y.shape == (2,)
-
-    assert np.isclose(slice_x[0], images[1], atol=0.1).all()
-    assert np.isclose(slice_x[1], images[2], atol=0.1).all()
-
-    assert slice_y[0] == 1
-    assert slice_y[1] == 2
-
-
-def test_msms_properties():
-    """Test the multi shot file sampler num_examples and shape"""
-    filenames = ["1.jpg", "2.jpg", "3.jpg", "4.jpg"]
-    filepaths = [_create_random_image(filename, (128, 96)) for filename in filenames]
-    y = tf.constant(range(4))
-    x = tf.constant(filepaths)
-
-    fs_sampler = MultiShotFileSampler(x=x, y=y)
-
-    assert fs_sampler.num_examples == 4
-    assert fs_sampler.example_shape == (128, 96, 3)
-
-
-def test_small_class_size(capsys):
-    """Test examples_per_class is > the number of class examples."""
-    filenames = ["1.jpg", "2.jpg", "3.jpg", "4.jpg"]
-    filepaths = [_create_random_image(filename) for filename in filenames]
-
-    y = tf.constant([1, 1, 1, 2])
-    x = tf.constant(filepaths)
-
-    fs_sampler = MultiShotFileSampler(x=x, y=y, classes_per_batch=2, examples_per_class_per_batch=3)
-
-    _, batch_y = fs_sampler.generate_batch(0)
-
-    y, _, class_counts = tf.unique_with_counts(batch_y)
-    assert tf.math.reduce_all(tf.sort(y) == tf.constant([1, 2]))
-    assert tf.math.reduce_all(class_counts == tf.constant([3, 3]))
-
-    captured = capsys.readouterr()
-    expected_msg = (
-        "WARNING: Class 2 only has 1 unique examples, but "
-        "examples_per_class is set to 3. The current batch will sample "
-        "from class examples with replacement, but you may want to "
-        "consider passing an Augmenter function or using the "
-        "SingleShotMemorySampler()."
-    )
-
-    match = re.search(expected_msg, captured.out)
-    assert bool(match)
-
-    _, batch_y = fs_sampler.generate_batch(0)
-
-    y, _, class_counts = tf.unique_with_counts(batch_y)
-    assert tf.math.reduce_all(tf.sort(y) == tf.constant([1, 2]))
-    assert tf.math.reduce_all(class_counts == tf.constant([3, 3]))
-
-    # Subsequent batch should produce the sampler warning.
-    captured = capsys.readouterr()
-    match = re.search(expected_msg, captured.out)
-    assert not bool(match)
+class FileSamplersTest(tf.test.TestCase):
+    def _create_random_image(self, filename, size=(32, 32)):
+        filepath = os.path.join(tempfile.gettempdir(), filename)
+        image = np.random.random(size + (3,)).astype(np.float32)
+        tf.keras.utils.save_img(filepath, image)
+        return filepath
+
+    def test_multi_shot_file_sampler(self):
+        """Test MultiShotFileSampler with various sizes.
+
+        Users may sample with replacement when creating batches, so check that we
+        can handle when elements per class is either less than or greater than the
+        total count of elements in the class.
+        """
+        filenames = ["1.jpg", "2.jpg", "3.jpg", "4.jpg", "5.jpg", "6.jpg"]
+        filepaths = [self._create_random_image(filename) for filename in filenames]
+        examples_per_class = (2, 20)
+        images = [np.array(tf.keras.utils.load_img(path), dtype=np.float32) / 255 for path in filepaths]
+
+        for example_per_class in examples_per_class:
+            y = tf.constant([1, 2, 3, 1, 2, 3])
+            x = tf.constant(filepaths)
+            class_per_batch = 2
+            with self.subTest(example_per_class=example_per_class):
+                batch_size = example_per_class * class_per_batch
+
+                fs_sampler = MultiShotFileSampler(
+                    x=x,
+                    y=y,
+                    classes_per_batch=class_per_batch,
+                    examples_per_class_per_batch=example_per_class,
+                )  # noqa
+
+                batch_x, batch_y = fs_sampler.generate_batch(batch_id=606)
+
+                self.assertLen(batch_y, batch_size)
+                self.assertLen(batch_x, batch_size)
+                num_classes, _ = tf.unique(batch_y)
+                self.assertLen(num_classes, class_per_batch)
+
+                for x, y in zip(batch_x, batch_y):
+                    if y == 1:
+                        assert (
+                            np.isclose(x.numpy(), images[0], atol=0.1).all()
+                            or np.isclose(x.numpy(), images[3], atol=0.1).all()
+                        )
+                    elif y == 2:
+                        assert (
+                            np.isclose(x.numpy(), images[1], atol=0.1).all()
+                            or np.isclose(x.numpy(), images[4], atol=0.1).all()
+                        )
+                    elif y == 3:
+                        assert (
+                            np.isclose(x.numpy(), images[2], atol=0.1).all()
+                            or np.isclose(x.numpy(), images[5], atol=0.1).all()
+                        )
+
+    def test_msfs_get_slice(self):
+        """Test the multi shot file sampler get_slice method."""
+        filenames = ["1.jpg", "2.jpg", "3.jpg", "4.jpg"]
+        filepaths = [self._create_random_image(filename) for filename in filenames]
+        images = [np.array(tf.keras.utils.load_img(path), dtype=np.float32) / 255 for path in filepaths]
+
+        y = tf.constant(range(4))
+        x = tf.constant(filepaths)
+
+        fs_sampler = MultiShotFileSampler(x=x, y=y)
+        # x and y are randomly shuffled so we fix the values here.
+        fs_sampler._x = x
+        fs_sampler._y = y
+        slice_x, slice_y = fs_sampler.get_slice(1, 2)
+
+        self.assertEqual(slice_x.shape, (2, 32, 32, 3))
+        self.assertEqual(slice_y.shape, (2,))
+
+        assert np.isclose(slice_x[0], images[1], atol=0.1).all()
+        assert np.isclose(slice_x[1], images[2], atol=0.1).all()
+
+        self.assertEqual(slice_y[0], 1)
+        self.assertEqual(slice_y[1], 2)
+
+    def test_msms_properties(self):
+        """Test the multi shot file sampler num_examples and shape"""
+        filenames = ["1.jpg", "2.jpg", "3.jpg", "4.jpg"]
+        filepaths = [self._create_random_image(filename, (128, 96)) for filename in filenames]
+        y = tf.constant(range(4))
+        x = tf.constant(filepaths)
+
+        fs_sampler = MultiShotFileSampler(x=x, y=y)
+
+        self.assertEqual(fs_sampler.num_examples, 4)
+        self.assertEqual(fs_sampler.example_shape, (128, 96, 3))
+
+    def test_small_class_size(self):
+        """Test examples_per_class is > the number of class examples."""
+        filenames = ["1.jpg", "2.jpg", "3.jpg", "4.jpg"]
+        filepaths = [self._create_random_image(filename) for filename in filenames]
+
+        y = tf.constant([1, 1, 1, 2])
+        x = tf.constant(filepaths)
+
+        with self.captureWritesToStream(sys.stdout) as captured:
+            ms_sampler = MultiShotFileSampler(x=x, y=y, classes_per_batch=2, examples_per_class_per_batch=3)
+            _, batch_y = ms_sampler.generate_batch(0)
+            y, _, class_counts = tf.unique_with_counts(batch_y)
+
+        self.assertAllEqual(tf.sort(y), tf.constant([1, 2]))
+        self.assertAllEqual(class_counts, tf.constant([3, 3]))
+
+        expected_msg = (
+            "WARNING: Class 2 only has 1 unique examples, but "
+            "examples_per_class is set to 3. The current batch will sample "
+            "from class examples with replacement, but you may want to "
+            "consider passing an Augmenter function or using the "
+            "SingleShotMemorySampler()."
+        )
+
+        match = re.search(expected_msg, captured.contents())
+        self.assertIsNotNone(match)
+
+        with self.captureWritesToStream(sys.stdout) as captured:
+            _, batch_y = ms_sampler.generate_batch(0)
+            y, _, class_counts = tf.unique_with_counts(batch_y)
+
+        self.assertAllEqual(tf.sort(y), tf.constant([1, 2]))
+        self.assertAllEqual(class_counts, tf.constant([3, 3]))
+
+        # Subsequent batch should produce the sampler warning.
+        match = re.search(expected_msg, captured.contents())
+        self.assertIsNone(match)
```

### Comparing `tfsim-nightly-0.18.0.dev5/tests/samplers/test_memory_samplers.py` & `tfsim-nightly-0.18.0.dev6/tests/samplers/test_memory_samplers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,147 +1,148 @@
 import re
+import sys
 
-import pytest
 import tensorflow as tf
 
 from tensorflow_similarity.samplers import MultiShotMemorySampler, select_examples
 
 
-def test_valid_class_numbers():
-    "Check that sampler properly detect if num_class requests >> class avail"
-    y = tf.constant([1, 2, 3, 1, 2, 3, 1])
-    x = tf.constant([10, 20, 30, 10, 20, 30, 10])
-
-    class_per_batch = 42
-
-    with pytest.raises(ValueError):
-        MultiShotMemorySampler(x=x, y=y, classes_per_batch=class_per_batch)
-
-
-@pytest.mark.parametrize("example_per_class", [2, 20])
-def test_select_examples(example_per_class):
-    """Test select_examples with various sizes.
-
-    Users may sample with replacement when creating batches, so check that we
-    can handle when elements per class is either less than or greater than the
-    total count of elements in the class.
-    """
-    y = tf.constant([1, 2, 3, 1, 2, 3, 1])
-    x = tf.constant([10, 20, 30, 10, 20, 30, 10])
-    cls_list = [1, 3]
-    batch_x, batch_y = select_examples(x, y, cls_list, example_per_class)
-
-    assert len(batch_y) == len(cls_list) * example_per_class
-    assert len(batch_x) == len(cls_list) * example_per_class
-
-    for x, y in zip(batch_x, batch_y):
-        assert y in cls_list
-
-        if y == 1:
-            assert x == 10
-        elif y == 3:
-            assert x == 30
-
-
-@pytest.mark.parametrize("example_per_class", [2, 20])
-def test_multi_shot_memory_sampler(example_per_class):
-    """Test MultiShotMemorySampler with various sizes.
-
-    Users may sample with replacement when creating batches, so check that we
-    can handle when elements per class is either less than or greater than the
-    total count of elements in the class.
-    """
-    y = tf.constant([1, 2, 3, 1, 2, 3, 1])
-    x = tf.constant([10, 20, 30, 10, 20, 30, 10])
-    class_per_batch = 2
-    batch_size = example_per_class * class_per_batch
-
-    ms_sampler = MultiShotMemorySampler(
-        x=x,
-        y=y,
-        classes_per_batch=class_per_batch,
-        examples_per_class_per_batch=example_per_class,
-    )  # noqa
-
-    batch_x, batch_y = ms_sampler.generate_batch(batch_id=606)
-
-    assert len(batch_y) == batch_size
-    assert len(batch_x) == batch_size
-    num_classes, _ = tf.unique(batch_y)
-    assert len(num_classes) == class_per_batch
-
-    for x, y in zip(batch_x, batch_y):
-        if y == 1:
-            assert x == 10
-        elif y == 2:
-            assert x == 20
-        elif y == 3:
-            assert x == 30
-
-
-def test_msms_get_slice():
-    """Test the multi shot memory sampler get_slice method."""
-    y = tf.constant(range(4))
-    x = tf.constant([[0] * 10, [1] * 10, [2] * 10, [3] * 10])
-
-    ms_sampler = MultiShotMemorySampler(x=x, y=y)
-    # x and y are randomly shuffled so we fix the values here.
-    ms_sampler._x = x
-    ms_sampler._y = y
-    slice_x, slice_y = ms_sampler.get_slice(1, 2)
-
-    assert slice_x.shape == (2, 10)
-    assert slice_y.shape == (2,)
-
-    assert slice_x[0, 0] == 1
-    assert slice_x[1, 0] == 2
-
-    assert slice_y[0] == 1
-    assert slice_y[1] == 2
-
-
-def test_msms_properties():
-    """Test the multi shot memory sampler num_examples and shape"""
-    y = tf.constant(range(4))
-    x = tf.ones([4, 10, 20, 3])
-
-    ms_sampler = MultiShotMemorySampler(x=x, y=y)
-
-    assert ms_sampler.num_examples == 4
-    assert ms_sampler.example_shape == (10, 20, 3)
-
-
-def test_small_class_size(capsys):
-    """Test examples_per_class is > the number of class examples."""
-    y = tf.constant([1, 1, 1, 2])
-    x = tf.ones([4, 10, 10, 3])
-
-    ms_sampler = MultiShotMemorySampler(x=x, y=y, classes_per_batch=2, examples_per_class_per_batch=3)
-
-    _, batch_y = ms_sampler.generate_batch(0)
-
-    y, _, class_counts = tf.unique_with_counts(batch_y)
-    assert tf.math.reduce_all(tf.sort(y) == tf.constant([1, 2]))
-    assert tf.math.reduce_all(class_counts == tf.constant([3, 3]))
-
-    captured = capsys.readouterr()
-    expected_msg = (
-        "WARNING: Class 2 only has 1 unique examples, but "
-        "examples_per_class is set to 3. The current batch will sample "
-        "from class examples with replacement, but you may want to "
-        "consider passing an Augmenter function or using the "
-        "SingleShotMemorySampler()."
-    )
-
-    match = re.search(expected_msg, captured.out)
-    assert bool(match)
-
-    _, batch_y = ms_sampler.generate_batch(0)
-
-    y, _, class_counts = tf.unique_with_counts(batch_y)
-    assert tf.math.reduce_all(tf.sort(y) == tf.constant([1, 2]))
-    assert tf.math.reduce_all(class_counts == tf.constant([3, 3]))
-
-    # Subsequent batch should produce the sampler warning.
-    captured = capsys.readouterr()
-    match = re.search(expected_msg, captured.out)
-    assert not bool(match)
+class MemorySamplersTest(tf.test.TestCase):
+    def test_valid_class_numbers(self):
+        "Check that sampler properly detect if num_class requests >> class avail"
+        y = tf.constant([1, 2, 3, 1, 2, 3, 1])
+        x = tf.constant([10, 20, 30, 10, 20, 30, 10])
+
+        class_per_batch = 42
+        with self.assertRaises(ValueError):
+            MultiShotMemorySampler(x=x, y=y, classes_per_batch=class_per_batch)
+
+    def test_select_examples(self):
+        """Test select_examples with various sizes.
+
+        Users may sample with replacement when creating batches, so check that we
+        can handle when elements per class is either less than or greater than the
+        total count of elements in the class.
+        """
+
+        examples_per_class = (2, 20)
+
+        for example_per_class in examples_per_class:
+            y = tf.constant([1, 2, 3, 1, 2, 3, 1])
+            x = tf.constant([10, 20, 30, 10, 20, 30, 10])
+            cls_list = [1, 3]
+            with self.subTest(example_per_class=example_per_class):
+                batch_x, batch_y = select_examples(x, y, cls_list, example_per_class)
+
+                self.assertLen(batch_y, len(cls_list) * example_per_class)
+                self.assertLen(batch_x, len(cls_list) * example_per_class)
+
+                for x, y in zip(batch_x, batch_y):
+                    self.assertIn(y, cls_list)
+
+                    if y == 1:
+                        self.assertEqual(x, 10)
+                    elif y == 3:
+                        self.assertEqual(x, 30)
+
+    def test_multi_shot_memory_sampler(self):
+        """Test MultiShotMemorySampler with various sizes.
+
+        Users may sample with replacement when creating batches, so check that we
+        can handle when elements per class is either less than or greater than the
+        total count of elements in the class.
+        """
+
+        examples_per_class = (2, 20)
+
+        for example_per_class in examples_per_class:
+            y = tf.constant([1, 2, 3, 1, 2, 3, 1])
+            x = tf.constant([10, 20, 30, 10, 20, 30, 10])
+            class_per_batch = 2
+            batch_size = example_per_class * class_per_batch
+            with self.subTest(example_per_class=example_per_class):
+                ms_sampler = MultiShotMemorySampler(
+                    x=x,
+                    y=y,
+                    classes_per_batch=class_per_batch,
+                    examples_per_class_per_batch=example_per_class,
+                )  # noqa
+
+                batch_x, batch_y = ms_sampler.generate_batch(batch_id=606)
+
+                self.assertLen(batch_y, batch_size)
+                self.assertLen(batch_x, batch_size)
+                num_classes, _ = tf.unique(batch_y)
+                self.assertLen(num_classes, class_per_batch)
+
+                for x, y in zip(batch_x, batch_y):
+                    if y == 1:
+                        self.assertEqual(x, 10)
+                    elif y == 2:
+                        self.assertEqual(x, 20)
+                    elif y == 3:
+                        self.assertEqual(x, 30)
+
+    def test_msms_get_slice(self):
+        """Test the multi shot memory sampler get_slice method."""
+        y = tf.constant(range(4))
+        x = tf.constant([[0] * 10, [1] * 10, [2] * 10, [3] * 10])
+
+        ms_sampler = MultiShotMemorySampler(x=x, y=y)
+        # x and y are randomly shuffled so we fix the values here.
+        ms_sampler._x = x
+        ms_sampler._y = y
+        slice_x, slice_y = ms_sampler.get_slice(1, 2)
+
+        self.assertEqual(slice_x.shape, (2, 10))
+        self.assertEqual(slice_y.shape, (2,))
+
+        self.assertEqual(slice_x[0, 0], 1)
+        self.assertEqual(slice_x[1, 0], 2)
+
+        self.assertEqual(slice_y[0], 1)
+        self.assertEqual(slice_y[1], 2)
+
+    def test_msms_properties(self):
+        """Test the multi shot memory sampler num_examples and shape"""
+        y = tf.constant(range(4))
+        x = tf.ones([4, 10, 20, 3])
+
+        ms_sampler = MultiShotMemorySampler(x=x, y=y)
+
+        self.assertEqual(ms_sampler.num_examples, 4)
+        self.assertEqual(ms_sampler.example_shape, (10, 20, 3))
+
+    def test_small_class_size(self):
+        """Test examples_per_class is > the number of class examples."""
+        y = tf.constant([1, 1, 1, 2])
+        x = tf.ones([4, 10, 10, 3])
+
+        with self.captureWritesToStream(sys.stdout) as captured:
+            ms_sampler = MultiShotMemorySampler(x=x, y=y, classes_per_batch=2, examples_per_class_per_batch=3)
+            _, batch_y = ms_sampler.generate_batch(0)
+            y, _, class_counts = tf.unique_with_counts(batch_y)
+
+        self.assertAllEqual(tf.sort(y), tf.constant([1, 2]))
+        self.assertAllEqual(class_counts, tf.constant([3, 3]))
+
+        expected_msg = (
+            "WARNING: Class 2 only has 1 unique examples, but "
+            "examples_per_class is set to 3. The current batch will sample "
+            "from class examples with replacement, but you may want to "
+            "consider passing an Augmenter function or using the "
+            "SingleShotMemorySampler()."
+        )
+
+        match = re.search(expected_msg, captured.contents())
+        self.assertIsNotNone(match)
+
+        with self.captureWritesToStream(sys.stdout) as captured:
+            _, batch_y = ms_sampler.generate_batch(0)
+            y, _, class_counts = tf.unique_with_counts(batch_y)
+
+        self.assertAllEqual(tf.sort(y), tf.constant([1, 2]))
+        self.assertAllEqual(class_counts, tf.constant([3, 3]))
+
+        # Subsequent batch should produce the sampler warning.
+        match = re.search(expected_msg, captured.contents())
+        self.assertIsNone(match)
```

### Comparing `tfsim-nightly-0.18.0.dev5/tests/samplers/test_tfdata_sampler.py` & `tfsim-nightly-0.18.0.dev6/tests/samplers/test_tfdata_sampler.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/samplers/test_tfdataset_samplers.py` & `tfsim-nightly-0.18.0.dev6/tests/samplers/test_tfdataset_samplers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pytest
+import tensorflow as tf
 
 from tensorflow_similarity.samplers import TFDatasetMultiShotMemorySampler
 
 
-def test_basic():
-    dataset_name = "mnist"
-    sampler = TFDatasetMultiShotMemorySampler(dataset_name=dataset_name, classes_per_batch=10)
-    batch = sampler.generate_batch(42)
-    assert batch[0].shape == (20, 28, 28, 1)
-
-
-def test_wrong_key():
-    dataset_name = "mnist"
-
-    # X
-    with pytest.raises(ValueError):
-        TFDatasetMultiShotMemorySampler(dataset_name=dataset_name, classes_per_batch=4, x_key="error")
-    # Y
-    with pytest.raises(ValueError):
-        TFDatasetMultiShotMemorySampler(dataset_name=dataset_name, classes_per_batch=4, y_key="error")
+class DatasetSamplersTest(tf.test.TestCase):
+    def test_basic(self):
+        dataset_name = "mnist"
+        sampler = TFDatasetMultiShotMemorySampler(dataset_name=dataset_name, classes_per_batch=10)
+        batch = sampler.generate_batch(42)
+        self.assertEqual(batch[0].shape, (20, 28, 28, 1))
+
+    def test_wrong_key(self):
+        dataset_name = "mnist"
+
+        # X
+        with self.assertRaises(ValueError):
+            TFDatasetMultiShotMemorySampler(dataset_name=dataset_name, classes_per_batch=4, x_key="error")
+        # Y
+        with self.assertRaises(ValueError):
+            TFDatasetMultiShotMemorySampler(dataset_name=dataset_name, classes_per_batch=4, y_key="error")
```

### Comparing `tfsim-nightly-0.18.0.dev5/tests/samplers/test_tfrecord_samplers.py` & `tfsim-nightly-0.18.0.dev6/tests/samplers/test_tfrecord_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/search/test_faiss_search.py` & `tfsim-nightly-0.18.0.dev6/tests/search/test_faiss_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/search/test_linear_search.py` & `tfsim-nightly-0.18.0.dev6/tests/search/test_linear_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/search/test_nmslib_search.py` & `tfsim-nightly-0.18.0.dev6/tests/search/test_nmslib_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/stores/test_cached_store.py` & `tfsim-nightly-0.18.0.dev6/tests/stores/test_cached_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/stores/test_memory_store.py` & `tfsim-nightly-0.18.0.dev6/tests/stores/test_memory_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/stores/test_redis_store.py` & `tfsim-nightly-0.18.0.dev6/tests/stores/test_redis_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/test_algebra.py` & `tfsim-nightly-0.18.0.dev6/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/test_layers.py` & `tfsim-nightly-0.18.0.dev6/tests/test_layers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,210 +1,186 @@
 import math
 from unittest import TestCase
 
 import numpy as np
-import pytest
 import tensorflow as tf
 
 from tensorflow_similarity.layers import (
     GeneralizedMeanPooling1D,
     GeneralizedMeanPooling2D,
     MetricEmbedding,
 )
 
 
-@pytest.fixture
 def input_2d_tensor():
-    # A (1, 3, 3, 2) Tensor.
     return tf.constant(
         [
             [
                 [[0.0, 5.0], [0.0, 5.0], [0.0, 5.0]],
                 [[5.0, 10.0], [5.0, 10.0], [5.0, 10.0]],
                 [[10.0, 15.0], [10.0, 15.0], [10.0, 15.0]],
             ],
         ]
     )
 
 
-def test_generalized_mean_pooling_2d(input_2d_tensor):
-    result = GeneralizedMeanPooling2D(p=1.0)(input_2d_tensor)
-    expected = tf.constant([[5.0, 10.0]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_2d_inf(input_2d_tensor):
-    result = GeneralizedMeanPooling2D(p=math.inf, keepdims=True)(input_2d_tensor)
-    expected = tf.constant([[[[10.0, 15.0]]]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_2d_neg_inf(input_2d_tensor):
-    result = GeneralizedMeanPooling2D(p=-math.inf, keepdims=True)(input_2d_tensor)
-    expected = tf.constant([[[[0.0, 5.0]]]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_2d_zero(input_2d_tensor):
-    result = GeneralizedMeanPooling2D(p=0.0)(input_2d_tensor)
-    expected = tf.constant([[3.0412402, 8.041241]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_2d_keepdims(input_2d_tensor):
-    result = GeneralizedMeanPooling2D(p=1.0, keepdims=True)(input_2d_tensor)
-    expected = tf.constant([[[[5.0, 10.0]]]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_2d_channels_first(input_2d_tensor):
-    result = GeneralizedMeanPooling2D(p=1.0, data_format="channels_first")(input_2d_tensor)
-    # With channels first we expect a (1,3) shape.
-    expected = tf.constant([[2.5, 7.5, 12.5]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_2d_compute_shape():
-    input_shape = tf.constant([1, 2, 3, 4])
-    result = GeneralizedMeanPooling2D().compute_output_shape(input_shape)
-    expected_shape = tf.constant([1, 4])
-    np.testing.assert_allclose(result, expected_shape, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_2d_compute_shape_keepdims():
-    input_shape = tf.constant([1, 2, 3, 4])
-    result = GeneralizedMeanPooling2D(keepdims=True).compute_output_shape(input_shape)
-    expected_shape = tf.constant([1, 1, 1, 4])
-    np.testing.assert_allclose(result, expected_shape, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_2d_compute_shape_dataformat():
-    input_shape = tf.constant([1, 2, 3, 4])
-    result = GeneralizedMeanPooling2D(data_format="channels_first").compute_output_shape(input_shape)
-    expected_shape = tf.constant([1, 2])
-    np.testing.assert_allclose(result, expected_shape, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_2d_get_config():
-    gem = GeneralizedMeanPooling2D(p=3.0, data_format="channels_first", keepdims=True, name="GEM")
-    config = gem.get_config()
-    expected_config = {
-        "p": 3.0,
-        "data_format": "channels_first",
-        "keepdims": True,
-        "name": "GEM",
-        "trainable": True,
-        "dtype": "float32",
-    }
-    TestCase().assertDictEqual(expected_config, config)
-
-
-@pytest.fixture
 def input_1d_tensor():
     # A (1, 3, 1) Tensor.
     x = tf.constant([[1.0, 2.0, 3.0], [4.0, 5.0, 6.0], [7.0, 8.0, 9.0]])
     x = tf.reshape(x, [3, 3, 1])
     return x
 
 
-def test_generalized_mean_pooling_1d(input_1d_tensor):
-    result = GeneralizedMeanPooling1D(p=1.0)(input_1d_tensor)
-    expected = tf.constant([[2.0], [5.0], [8.0]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_1d_inf(input_1d_tensor):
-    result = GeneralizedMeanPooling1D(p=math.inf, keepdims=True)(input_1d_tensor)
-    expected = tf.constant([[[3.0], [3.0], [3.0]], [[6.0], [6.0], [6.0]], [[9.0], [9.0], [9.0]]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_1d_neg_inf(input_1d_tensor):
-    result = GeneralizedMeanPooling1D(p=-math.inf, keepdims=True)(input_1d_tensor)
-    expected = tf.constant([[[1.0], [1.0], [1.0]], [[4.0], [4.0], [4.0]], [[7.0], [7.0], [7.0]]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_1d_zero(input_1d_tensor):
-    result = GeneralizedMeanPooling1D(p=0.0)(input_1d_tensor)
-    expected = tf.constant([[1.8171206], [4.8171206], [7.8171206]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_1d_keepdims(input_1d_tensor):
-    result = GeneralizedMeanPooling1D(p=1.0, keepdims=True)(input_1d_tensor)
-    expected = tf.constant([[[2.0]], [[5.0]], [[8.0]]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_1d_channels_first(input_1d_tensor):
-    input_1d_tensor = tf.reshape(input_1d_tensor, [3, 1, 3])
-    result = GeneralizedMeanPooling1D(p=1.0, data_format="channels_first")(input_1d_tensor)
-    expected = tf.constant([[2.0], [5.0], [8.0]])
-    np.testing.assert_allclose(result, expected, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_1d_compute_shape():
-    input_shape = tf.constant([1, 2, 3])
-    result = GeneralizedMeanPooling1D().compute_output_shape(input_shape)
-    expected_shape = tf.constant([1, 3])
-    np.testing.assert_allclose(result, expected_shape, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_1d_compute_shape_keepdims():
-    input_shape = tf.constant([1, 2, 3])
-    result = GeneralizedMeanPooling1D(keepdims=True).compute_output_shape(input_shape)
-    expected_shape = tf.constant([1, 1, 3])
-    np.testing.assert_allclose(result, expected_shape, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_1d_compute_shape_dataformat():
-    input_shape = tf.constant([1, 2, 3])
-    result = GeneralizedMeanPooling1D(data_format="channels_first").compute_output_shape(input_shape)
-    expected_shape = tf.constant([1, 2])
-    np.testing.assert_allclose(result, expected_shape, rtol=1e-06)
-
-
-def test_generalized_mean_pooling_1d_get_config():
-    gem = GeneralizedMeanPooling1D(p=3.0, data_format="channels_first", keepdims=True, name="GEM")
-    config = gem.get_config()
-    expected_config = {
-        "p": 3.0,
-        "data_format": "channels_first",
-        "keepdims": True,
-        "name": "GEM",
-        "trainable": True,
-        "dtype": "float32",
-    }
-    TestCase().assertDictEqual(expected_config, config)
-
-
-def test_metric_embedding():
-    input_tensor = tf.constant([[4.0, 4.0, 4.0, 4.0], [1.0, 1.0, 1.0, 1.0]])
-    me_layer = MetricEmbedding(4, kernel_initializer=tf.constant_initializer(1.0))
-    result = me_layer(input_tensor)
-    expected_result = tf.constant([[0.5, 0.5, 0.5, 0.5], [0.5, 0.5, 0.5, 0.5]])
-    np.testing.assert_allclose(result, expected_result, rtol=1e-06)
-
-
-def test_metric_embedding_get_config():
-    me_layer = MetricEmbedding(32)
-    config = me_layer.get_config()
-    expected_config = {
-        "name": "metric_embedding_1",
-        "trainable": True,
-        "dtype": "float32",
-        "units": 32,
-        "activation": "linear",
-        "use_bias": True,
-        "kernel_initializer": {
-            "class_name": "GlorotUniform",
-            "config": {"seed": None},
-        },
-        "bias_initializer": {"class_name": "Zeros", "config": {}},
-        "kernel_regularizer": None,
-        "bias_regularizer": None,
-        "activity_regularizer": None,
-        "kernel_constraint": None,
-        "bias_constraint": None,
-    }
-    TestCase().assertDictEqual(expected_config, config)
+class LayersTest(tf.test.TestCase):
+    def test_generalized_mean_pooling_2d(self):
+        result = GeneralizedMeanPooling2D(p=1.0)(input_2d_tensor())
+        expected = tf.constant([[5.0, 10.0]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_2d_inf(self):
+        result = GeneralizedMeanPooling2D(p=math.inf, keepdims=True)(input_2d_tensor())
+        expected = tf.constant([[[[10.0, 15.0]]]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_2d_neg_inf(self):
+        result = GeneralizedMeanPooling2D(p=-math.inf, keepdims=True)(input_2d_tensor())
+        expected = tf.constant([[[[0.0, 5.0]]]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_2d_zero(self):
+        result = GeneralizedMeanPooling2D(p=0.0)(input_2d_tensor())
+        expected = tf.constant([[3.0412402, 8.041241]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_2d_keepdims(self):
+        result = GeneralizedMeanPooling2D(p=1.0, keepdims=True)(input_2d_tensor())
+        expected = tf.constant([[[[5.0, 10.0]]]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_2d_channels_first(self):
+        result = GeneralizedMeanPooling2D(p=1.0, data_format="channels_first")(input_2d_tensor())
+        # With channels first we expect a (1,3) shape.
+        expected = tf.constant([[2.5, 7.5, 12.5]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_2d_compute_shape(self):
+        input_shape = tf.constant([1, 2, 3, 4])
+        result = GeneralizedMeanPooling2D().compute_output_shape(input_shape)
+        expected_shape = tf.constant([1, 4])
+        self.assertAllClose(result, expected_shape, rtol=1e-06)
+
+    def test_generalized_mean_pooling_2d_compute_shape_keepdims(self):
+        input_shape = tf.constant([1, 2, 3, 4])
+        result = GeneralizedMeanPooling2D(keepdims=True).compute_output_shape(input_shape)
+        expected_shape = tf.constant([1, 1, 1, 4])
+        self.assertAllClose(result, expected_shape, rtol=1e-06)
+
+    def test_generalized_mean_pooling_2d_compute_shape_dataformat(self):
+        input_shape = tf.constant([1, 2, 3, 4])
+        result = GeneralizedMeanPooling2D(data_format="channels_first").compute_output_shape(input_shape)
+        expected_shape = tf.constant([1, 2])
+        self.assertAllClose(result, expected_shape, rtol=1e-06)
+
+    def test_generalized_mean_pooling_2d_get_config(self):
+        gem = GeneralizedMeanPooling2D(p=3.0, data_format="channels_first", keepdims=True, name="GEM")
+        config = gem.get_config()
+        expected_config = {
+            "p": 3.0,
+            "data_format": "channels_first",
+            "keepdims": True,
+            "name": "GEM",
+            "trainable": True,
+            "dtype": "float32",
+        }
+        self.assertDictEqual(expected_config, config)
+
+    def test_generalized_mean_pooling_1d(self):
+        result = GeneralizedMeanPooling1D(p=1.0)(input_1d_tensor())
+        expected = tf.constant([[2.0], [5.0], [8.0]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_1d_inf(self):
+        result = GeneralizedMeanPooling1D(p=math.inf, keepdims=True)(input_1d_tensor())
+        expected = tf.constant([[[3.0], [3.0], [3.0]], [[6.0], [6.0], [6.0]], [[9.0], [9.0], [9.0]]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_1d_neg_inf(self):
+        result = GeneralizedMeanPooling1D(p=-math.inf, keepdims=True)(input_1d_tensor())
+        expected = tf.constant([[[1.0], [1.0], [1.0]], [[4.0], [4.0], [4.0]], [[7.0], [7.0], [7.0]]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_1d_zero(self):
+        result = GeneralizedMeanPooling1D(p=0.0)(input_1d_tensor())
+        expected = tf.constant([[1.8171206], [4.8171206], [7.8171206]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_1d_keepdims(self):
+        result = GeneralizedMeanPooling1D(p=1.0, keepdims=True)(input_1d_tensor())
+        expected = tf.constant([[[2.0]], [[5.0]], [[8.0]]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_1d_channels_first(self):
+        input_tensor = tf.reshape(input_1d_tensor(), [3, 1, 3])
+        result = GeneralizedMeanPooling1D(p=1.0, data_format="channels_first")(input_tensor)
+        expected = tf.constant([[2.0], [5.0], [8.0]])
+        self.assertAllClose(result, expected, rtol=1e-06)
+
+    def test_generalized_mean_pooling_1d_compute_shape(self):
+        input_shape = tf.constant([1, 2, 3])
+        result = GeneralizedMeanPooling1D().compute_output_shape(input_shape)
+        expected_shape = tf.constant([1, 3])
+        self.assertAllClose(result, expected_shape, rtol=1e-06)
+
+    def test_generalized_mean_pooling_1d_compute_shape_keepdims(self):
+        input_shape = tf.constant([1, 2, 3])
+        result = GeneralizedMeanPooling1D(keepdims=True).compute_output_shape(input_shape)
+        expected_shape = tf.constant([1, 1, 3])
+        self.assertAllClose(result, expected_shape, rtol=1e-06)
+
+    def test_generalized_mean_pooling_1d_compute_shape_dataformat(self):
+        input_shape = tf.constant([1, 2, 3])
+        result = GeneralizedMeanPooling1D(data_format="channels_first").compute_output_shape(input_shape)
+        expected_shape = tf.constant([1, 2])
+        self.assertAllClose(result, expected_shape, rtol=1e-06)
+
+    def test_generalized_mean_pooling_1d_get_config(self):
+        gem = GeneralizedMeanPooling1D(p=3.0, data_format="channels_first", keepdims=True, name="GEM")
+        config = gem.get_config()
+        expected_config = {
+            "p": 3.0,
+            "data_format": "channels_first",
+            "keepdims": True,
+            "name": "GEM",
+            "trainable": True,
+            "dtype": "float32",
+        }
+        self.assertDictEqual(expected_config, config)
+
+    def test_metric_embedding(self):
+        input_tensor = tf.constant([[4.0, 4.0, 4.0, 4.0], [1.0, 1.0, 1.0, 1.0]])
+        me_layer = MetricEmbedding(4, kernel_initializer=tf.constant_initializer(1.0))
+        result = me_layer(input_tensor)
+        expected_result = tf.constant([[0.5, 0.5, 0.5, 0.5], [0.5, 0.5, 0.5, 0.5]])
+        self.assertAllClose(result, expected_result, rtol=1e-06)
+
+    def test_metric_embedding_get_config(self):
+        me_layer = MetricEmbedding(32)
+        config = me_layer.get_config()
+        expected_config = {
+            "name": "metric_embedding",
+            "trainable": True,
+            "dtype": "float32",
+            "units": 32,
+            "activation": "linear",
+            "use_bias": True,
+            "kernel_initializer": {
+                "class_name": "GlorotUniform",
+                "config": {"seed": None},
+            },
+            "bias_initializer": {"class_name": "Zeros", "config": {}},
+            "kernel_regularizer": None,
+            "bias_regularizer": None,
+            "activity_regularizer": None,
+            "kernel_constraint": None,
+            "bias_constraint": None,
+        }
+        self.assertEqual(expected_config, config)
```

### Comparing `tfsim-nightly-0.18.0.dev5/tests/test_schedules.py` & `tfsim-nightly-0.18.0.dev6/tests/test_schedules.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/test_types.py` & `tfsim-nightly-0.18.0.dev6/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/test_utils.py` & `tfsim-nightly-0.18.0.dev6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/training_metrics/test_distance_metrics.py` & `tfsim-nightly-0.18.0.dev6/tests/training_metrics/test_distance_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     metric.update_state(LABELS, EMBEDDINGS, None)
     metric2.update_state(LABELS, EMBEDDINGS, None)
     assert metric.result() == metric2.result()
 
 
 class DistanceMetricsTest(tf.test.TestCase):
     def test_avg_positive(self):
-
         agg = ["avg", tf.reduce_mean]
 
         # metric computation
         metric_val = compute_metric("cosine", agg[0], LABELS, EMBEDDINGS)
 
         # manual computation
         hard_distances = manual_hard_mining(cosine, EMB1, EMB2)
```

### Comparing `tfsim-nightly-0.18.0.dev5/tests/visualization/test_confusion_matrix.py` & `tfsim-nightly-0.18.0.dev6/tests/visualization/test_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tests/visualization/test_neighbors_viz.py` & `tfsim-nightly-0.18.0.dev6/tests/visualization/test_neighbors_viz.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev5/tfsim_nightly.egg-info/PKG-INFO` & `tfsim-nightly-0.18.0.dev6/tfsim_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfsim-nightly
-Version: 0.18.0.dev5
+Version: 0.18.0.dev6
 Summary: Metric Learning for Humans
 Home-page: https://github.com/tensorflow/similarity
 Author: Tensorflow Similarity authors
 Author-email: tf-similarity@google.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tfsim-nightly-0.18.0.dev5/tfsim_nightly.egg-info/SOURCES.txt` & `tfsim-nightly-0.18.0.dev6/tfsim_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

