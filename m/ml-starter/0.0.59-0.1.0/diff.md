# Comparing `tmp/ml-starter-0.0.59.tar.gz` & `tmp/ml-starter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.59.tar", last modified: Wed Jun 14 06:53:13 2023, max compression
+gzip compressed data, was "ml-starter-0.1.0.tar", last modified: Sat Jun 24 19:27:45 2023, max compression
```

## Comparing `ml-starter-0.0.59.tar` & `ml-starter-0.1.0.tar`

### file list

```diff
@@ -1,167 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.606784 ml-starter-0.0.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 06:53:00.000000 ml-starter-0.0.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 06:53:00.000000 ml-starter-0.0.59/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 06:53:13.606784 ml-starter-0.0.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-14 06:53:00.000000 ml-starter-0.0.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.578784 ml-starter-0.0.59/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.578784 ml-starter-0.0.59/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.578784 ml-starter-0.0.59/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.582784 ml-starter-0.0.59/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.582784 ml-starter-0.0.59/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.582784 ml-starter-0.0.59/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.586784 ml-starter-0.0.59/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.586784 ml-starter-0.0.59/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.590784 ml-starter-0.0.59/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.590784 ml-starter-0.0.59/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.590784 ml-starter-0.0.59/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.590784 ml-starter-0.0.59/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.594784 ml-starter-0.0.59/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.594784 ml-starter-0.0.59/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.594784 ml-starter-0.0.59/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.594784 ml-starter-0.0.59/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.598784 ml-starter-0.0.59/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.602784 ml-starter-0.0.59/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.602784 ml-starter-0.0.59/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.606784 ml-starter-0.0.59/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.606784 ml-starter-0.0.59/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 06:53:13.000000 ml-starter-0.0.59/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-14 06:53:13.000000 ml-starter-0.0.59/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 06:53:13.000000 ml-starter-0.0.59/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-14 06:53:13.000000 ml-starter-0.0.59/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 06:53:13.000000 ml-starter-0.0.59/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-14 06:53:00.000000 ml-starter-0.0.59/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 06:53:00.000000 ml-starter-0.0.59/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 06:53:00.000000 ml-starter-0.0.59/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-14 06:53:00.000000 ml-starter-0.0.59/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-14 06:53:13.606784 ml-starter-0.0.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-14 06:53:00.000000 ml-starter-0.0.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.218369 ml-starter-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-24 19:27:31.000000 ml-starter-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-24 19:27:31.000000 ml-starter-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-24 19:27:45.218369 ml-starter-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-24 19:27:31.000000 ml-starter-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.190369 ml-starter-0.1.0/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.190369 ml-starter-0.1.0/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.190369 ml-starter-0.1.0/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.194369 ml-starter-0.1.0/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.194369 ml-starter-0.1.0/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.194369 ml-starter-0.1.0/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.198369 ml-starter-0.1.0/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.198369 ml-starter-0.1.0/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.198369 ml-starter-0.1.0/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.202369 ml-starter-0.1.0/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.202369 ml-starter-0.1.0/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.202369 ml-starter-0.1.0/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.202369 ml-starter-0.1.0/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.206369 ml-starter-0.1.0/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.206369 ml-starter-0.1.0/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.206369 ml-starter-0.1.0/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.210369 ml-starter-0.1.0/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.214369 ml-starter-0.1.0/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.214369 ml-starter-0.1.0/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.214369 ml-starter-0.1.0/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-06-24 19:27:31.000000 ml-starter-0.1.0/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:27:45.218369 ml-starter-0.1.0/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-24 19:27:45.000000 ml-starter-0.1.0/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-24 19:27:45.000000 ml-starter-0.1.0/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:27:45.000000 ml-starter-0.1.0/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-24 19:27:45.000000 ml-starter-0.1.0/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-24 19:27:45.000000 ml-starter-0.1.0/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-24 19:27:31.000000 ml-starter-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-24 19:27:31.000000 ml-starter-0.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-24 19:27:31.000000 ml-starter-0.1.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-24 19:27:31.000000 ml-starter-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-24 19:27:45.218369 ml-starter-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-24 19:27:31.000000 ml-starter-0.1.0/setup.py
```

### Comparing `ml-starter-0.0.59/LICENSE` & `ml-starter-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/PKG-INFO` & `ml-starter-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.59
+Version: 0.1.0
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.59/README.md` & `ml-starter-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/api.py` & `ml-starter-0.1.0/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/core/common_types.py` & `ml-starter-0.1.0/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/core/config.py` & `ml-starter-0.1.0/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/core/env.py` & `ml-starter-0.1.0/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/core/registry.py` & `ml-starter-0.1.0/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/core/state.py` & `ml-starter-0.1.0/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/launchers/base.py` & `ml-starter-0.1.0/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/launchers/mp.py` & `ml-starter-0.1.0/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/launchers/slurm.py` & `ml-starter-0.1.0/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/launchers/torchrun.py` & `ml-starter-0.1.0/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/loggers/base.py` & `ml-starter-0.1.0/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/loggers/meter.py` & `ml-starter-0.1.0/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/loggers/multi.py` & `ml-starter-0.1.0/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/loggers/stdout.py` & `ml-starter-0.1.0/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/loggers/tensorboard.py` & `ml-starter-0.1.0/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/lr_schedulers/base.py` & `ml-starter-0.1.0/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/lr_schedulers/constant.py` & `ml-starter-0.1.0/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.0/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.0/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/lr_schedulers/linear.py` & `ml-starter-0.1.0/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.0/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.0/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/models/activations.py` & `ml-starter-0.1.0/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/models/base.py` & `ml-starter-0.1.0/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/models/embeddings.py` & `ml-starter-0.1.0/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/models/init.py` & `ml-starter-0.1.0/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/models/kmeans.py` & `ml-starter-0.1.0/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/models/lora.py` & `ml-starter-0.1.0/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/models/norms.py` & `ml-starter-0.1.0/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/models/parallel.py` & `ml-starter-0.1.0/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/optimizers/adam.py` & `ml-starter-0.1.0/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/optimizers/adamw.py` & `ml-starter-0.1.0/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/optimizers/adan.py` & `ml-starter-0.1.0/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/optimizers/base.py` & `ml-starter-0.1.0/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/optimizers/common.py` & `ml-starter-0.1.0/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/optimizers/lion.py` & `ml-starter-0.1.0/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/optimizers/sgd.py` & `ml-starter-0.1.0/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/optimizers/shampoo.py` & `ml-starter-0.1.0/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/scripts/cli.py` & `ml-starter-0.1.0/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/scripts/stage.py` & `ml-starter-0.1.0/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/scripts/train.py` & `ml-starter-0.1.0/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/base.py` & `ml-starter-0.1.0/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.0/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.0/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/datasets/collate.py` & `ml-starter-0.1.0/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.0/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.0/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.0/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.0/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.0/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/datasets/utils.py` & `ml-starter-0.1.0/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.0/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/environments/base.py` & `ml-starter-0.1.0/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/environments/utils.py` & `ml-starter-0.1.0/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/environments/worker.py` & `ml-starter-0.1.0/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/losses/reduce.py` & `ml-starter-0.1.0/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/rl/base.py` & `ml-starter-0.1.0/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/rl/replay.py` & `ml-starter-0.1.0/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/tasks/sl/base.py` & `ml-starter-0.1.0/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/trainers/base.py` & `ml-starter-0.1.0/ml/trainers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,14 @@
             if isinstance(ckpt, (str, Path)):
                 try:
                     ckpt = cast(dict, torch.load(ckpt, weights_only=weights_only))
                 except UnpicklingError:
                     if weights_only:
                         logger.warning("Failed to load checkpoint using `weights_only` flag, retrying without it")
                         ckpt = cast(dict, torch.load(cast(str | Path, ckpt), weights_only=False))
-                        raise  # TODO: Remove later
                     else:
                         raise
 
             task.on_after_load_checkpoint(ckpt)
             if "model" in ckpt:
                 model.load_state_dict(ckpt["model"])
             else:
```

### Comparing `ml-starter-0.0.59/ml/trainers/learning.py` & `ml-starter-0.1.0/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/trainers/mixins/compile.py` & `ml-starter-0.1.0/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.0/ml/trainers/mixins/cpu_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,16 +138,16 @@
         time.sleep(ping_interval)
 
 
 class CPUStatsMonitor:
     def __init__(self, ping_interval: float, manager: SyncManager) -> None:
         self._ping_interval = ping_interval
         self._manager = manager
-        self._monitor_event = manager.Event()
-        self._start_event = manager.Event()
+        self._monitor_event = self._manager.Event()
+        self._start_event = self._manager.Event()
         self._cpu_stats_smem = self._manager.Value(
             CPUStats,
             CPUStats(
                 cpu_percent=0.0,
                 mem_percent=0.0,
                 mem_rss=0,
                 mem_vms=0,
@@ -203,15 +203,18 @@
 
 class CPUStatsMixin(MonitorProcessMixin[CPUStatsConfigT, ModelT, TaskT]):
     """Defines a trainer mixin for getting CPU statistics."""
 
     def __init__(self, config: CPUStatsConfigT) -> None:
         super().__init__(config)
 
-        self._cpu_stats_monitor = CPUStatsMonitor(self.config.cpu_stats_ping_interval, self._mp_manager)
+        self._cpu_stats_monitor = CPUStatsMonitor(
+            ping_interval=self.config.cpu_stats_ping_interval,
+            manager=self._mp_manager,
+        )
 
     def on_training_start(
         self,
         state: State,
         task: TaskT,
         model: ModelT,
         optim: Optimizer,
```

### Comparing `ml-starter-0.0.59/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.0/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.0/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.1.0/ml/trainers/mixins/grad_clipping.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,44 +32,44 @@
 from ml.trainers.mixins.mixed_precision import (
     MixedPrecisionTrainerConfig,
     MixedPrecisionTrainerMixin,
 )
 
 
 @dataclass
-class GradientClipping:
+class GradientClippingConfig(MixedPrecisionTrainerConfig, BaseTrainerConfig):
     clip_grad_norm: float | None = conf_field(None, help="What to clip the gradient norm to")
     clip_grad_value: float | None = conf_field(None, help="What to clip the gradient value to")
-    norm_type: Any = conf_field(2, help="Type of norm to use")
-
-
-@dataclass
-class GradientClippingConfig(MixedPrecisionTrainerConfig, BaseTrainerConfig):
-    grad_clipping: GradientClipping = conf_field(GradientClipping(), help="Gradient clipping configuration")
+    clip_grad_norm_type: Any = conf_field(2, help="Type of norm to use")
 
 
 GradientClippingConfigT = TypeVar("GradientClippingConfigT", bound=GradientClippingConfig)
 
 
 class GradientClippingTrainerMixin(
     MixedPrecisionTrainerMixin[GradientClippingConfigT, ModelT, TaskT],
     BaseTrainer[GradientClippingConfigT, ModelT, TaskT],
 ):
     """Defines a trainer mixin for doing gradient clipping."""
 
     def clip_grads(self, model: nn.Module, optim: Optimizer) -> None:
-        clip_norm = self.config.grad_clipping.clip_grad_norm
-        clip_value = self.config.grad_clipping.clip_grad_value
-        norm_type = self.config.grad_clipping.norm_type
+        clip_norm = self.config.clip_grad_norm
+        clip_value = self.config.clip_grad_value
+        norm_type = self.config.clip_grad_norm_type
+        unscaled = False
 
         if clip_norm is not None:
             if isinstance(model, FSDP):
                 total_norm = model.clip_grad_norm_(clip_norm, norm_type)
                 self.logger.log_scalar("total_norm", total_norm.item(), namespace="optim")
             else:
-                self.unscale_mixed_precision(optim)
+                if not unscaled:
+                    self.unscale_mixed_precision(optim)
+                    unscaled = True
                 total_norm = nn.utils.clip_grad.clip_grad_norm_(model.parameters(), clip_norm, norm_type)
                 self.logger.log_scalar("total_norm", total_norm.item(), namespace="optim")
 
         if clip_value is not None:
-            self.unscale_mixed_precision(optim)
+            if not unscaled:
+                self.unscale_mixed_precision(optim)
+                unscaled = True
             nn.utils.clip_grad.clip_grad_value_(model.parameters(), clip_value)
```

### Comparing `ml-starter-0.0.59/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.0/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.0/ml/trainers/mixins/mixed_precision.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,44 +15,44 @@
 from torch.optim import Optimizer
 
 from ml.core.config import conf_field
 from ml.trainers.base import BaseTrainer, BaseTrainerConfig, ModelT, TaskT
 
 
 @dataclass
-class FP16:
+class MixedPrecisionConfig:
     enabled: bool = conf_field(True, help="If set, should FP16 training be enabled")
     init_scale: float = conf_field(2.0**16, help="Initial scaling factor")
     growth_factor: float = conf_field(2.0, help="Factor by which the scale is multiplied if no gradient NaNs occur")
     backoff_factor: float = conf_field(0.5, help="Factor by which the scale is multiplied if gradient NaNs occur")
     growth_interval: int = conf_field(2000, help="How often to grow the scale")
 
 
 @dataclass
 class MixedPrecisionTrainerConfig(BaseTrainerConfig):
-    fp16: FP16 = conf_field(FP16(), help="Mixed precision configuration")
+    mixed_precision: MixedPrecisionConfig = conf_field(MixedPrecisionConfig(), help="Mixed precision configuration")
 
 
 MixedPrecisionConfigT = TypeVar("MixedPrecisionConfigT", bound=MixedPrecisionTrainerConfig)
 
 
 class MixedPrecisionTrainerMixin(BaseTrainer[MixedPrecisionConfigT, ModelT, TaskT]):
     """Defines a trainer mixin for doing FP16 scaling."""
 
     def __init__(self, config: MixedPrecisionConfigT) -> None:
         super().__init__(config)
 
         self.grad_scaler: torch.cuda.amp.GradScaler | None
-        if self._device_type == "cuda" and self.config.fp16.enabled:
+        if self._device_type == "cuda" and self.config.mixed_precision.enabled:
             self.grad_scaler = torch.cuda.amp.GradScaler(
-                init_scale=self.config.fp16.init_scale,
-                growth_factor=self.config.fp16.growth_factor,
-                backoff_factor=self.config.fp16.backoff_factor,
-                growth_interval=self.config.fp16.growth_interval,
-                enabled=self.config.fp16.enabled and self._device.supports_grad_scaler(),
+                init_scale=self.config.mixed_precision.init_scale,
+                growth_factor=self.config.mixed_precision.growth_factor,
+                backoff_factor=self.config.mixed_precision.backoff_factor,
+                growth_interval=self.config.mixed_precision.growth_interval,
+                enabled=self.config.mixed_precision.enabled and self._device.supports_grad_scaler(),
             )
         else:
             self.grad_scaler = None
 
     def scale_mixed_precision(self, tensor: Tensor) -> Tensor:
         if self.grad_scaler is not None:
             return self.grad_scaler.scale(tensor)
@@ -85,8 +85,8 @@
             assert "grad_scaler" not in ckpt
 
             ckpt["grad_scaler"] = self.grad_scaler.state_dict()
 
         super().update_state_dict(ckpt)
 
     def autocast_context(self) -> ContextManager:
-        return self._device.autocast_context(enabled=self.config.fp16.enabled)
+        return self._device.autocast_context(enabled=self.config.mixed_precision.enabled)
```

### Comparing `ml-starter-0.0.59/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.0/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.0/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.0/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/trainers/rl.py` & `ml-starter-0.1.0/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/trainers/sl.py` & `ml-starter-0.1.0/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/argparse.py` & `ml-starter-0.1.0/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/atomic.py` & `ml-starter-0.1.0/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/audio.py` & `ml-starter-0.1.0/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/augmentation.py` & `ml-starter-0.1.0/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/caching.py` & `ml-starter-0.1.0/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/checkpoint.py` & `ml-starter-0.1.0/ml/utils/checkpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 and checkpoint. Note that there might be some issues if you move the checkpoint
 around places.
 """
 
 import logging
 import tempfile
 from pathlib import Path
-from typing import Mapping, TypeVar, cast
+from typing import Any, Mapping, TypeVar, cast
 
 import torch
-from omegaconf import DictConfig, OmegaConf
+from omegaconf import MISSING, Container, DictConfig, OmegaConf
 from torchvision.datasets.utils import download_url
 
 from ml.core.env import get_model_dir
 from ml.core.registry import Objects, register_model, register_task
 from ml.models.base import BaseModel
 from ml.tasks.base import BaseTask
 from ml.trainers.base import BaseTrainer
@@ -24,14 +24,34 @@
 from ml.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
+def is_missing(cfg: Any, key: str) -> bool:  # noqa: ANN401
+    """Utility function for checking if a config key is missing.
+
+    This is for cases when you are using a raw dataclass rather than an
+    OmegaConf container but want to treat them the same way.
+
+    Args:
+        cfg: The config to check
+        key: The key to check
+
+    Returns:
+        Whether or not the key is missing a value in the config
+    """
+    if isinstance(cfg, Container) and OmegaConf.is_missing(cfg, key):
+        return True
+    if getattr(cfg, key) is MISSING:
+        return True
+    return False
+
+
 def instantiate_config(config: str | Path | DictConfig | dict) -> Objects:
     """Builds the objects from the raw config.
 
     Args:
         config: The config to use. If a string or a Path, it is expected to
             be a path to a YAML file.
```

### Comparing `ml-starter-0.0.59/ml/utils/cli.py` & `ml-starter-0.1.0/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/colors.py` & `ml-starter-0.1.0/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/data.py` & `ml-starter-0.1.0/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/datetime.py` & `ml-starter-0.1.0/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/device/auto.py` & `ml-starter-0.1.0/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/device/base.py` & `ml-starter-0.1.0/ml/utils/device/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -245,12 +245,16 @@
     @classmethod
     def autocast_context(cls, enabled: bool = True) -> ContextManager:
         device_type = cls.get_device().type
         if device_type == "mps":
             device_type = "cpu"
         if device_type not in ("cpu", "cuda"):
             return contextlib.nullcontext()
-        return torch.autocast(device_type, enabled=enabled)
+        return torch.autocast(
+            device_type=device_type,
+            dtype=cls.get_floating_point_type(),
+            enabled=enabled,
+        )
 
     @classmethod
     def supports_grad_scaler(cls) -> bool:
         return False
```

### Comparing `ml-starter-0.0.59/ml/utils/device/cpu.py` & `ml-starter-0.1.0/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/device/gpu.py` & `ml-starter-0.1.0/ml/utils/device/gpu.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 variables:
 
 - ``USE_FP64``: Use FP64
 - ``USE_FP32``: Use FP32
 - ``USE_BF16``: Use BF16
 """
 
+import functools
 import logging
 import os
 from typing import Callable
 
 import torch
 
 from ml.core.env import is_gpu_disabled
@@ -30,34 +31,43 @@
     """Mixin to support single-GPU training."""
 
     @classmethod
     def has_device(cls) -> bool:
         return torch.cuda.is_available() and torch.cuda.device_count() > 0 and not is_gpu_disabled()
 
     @classmethod
+    @functools.lru_cache(maxsize=None)
     def get_device(cls) -> torch.device:
         return torch.device("cuda")
 
     @classmethod
+    @functools.lru_cache(maxsize=None)
     def get_floating_point_type(cls) -> torch.dtype:
+        # Allows users to override the default floating point type.
+        use_fp16 = get_env_bool("USE_FP16")
         use_bf16 = get_env_bool("USE_BF16")
         use_fp32 = get_env_bool("USE_FP32")
         use_fp64 = get_env_bool("USE_FP64")
         if use_fp64:
             return torch.float64
         elif use_fp32:
             return torch.float32
         elif use_bf16:
             return torch.bfloat16
-        else:
+        elif use_fp16:
             return torch.float16
 
+        # By default, use BF16 if the GPU supports it, otherwise FP16.
+        if torch.cuda.get_device_capability()[0] >= 8:
+            return torch.bfloat16
+        return torch.float16
+
     @classmethod
     def get_torch_compile_backend(cls) -> str | Callable:
         capability = torch.cuda.get_device_capability()
         if capability >= (7, 0):
             return "inductor"
         return "aot_ts_nvfuser"
 
     @classmethod
     def supports_grad_scaler(cls) -> bool:
-        return cls.get_floating_point_type() == torch.float16
+        return cls.get_floating_point_type() not in (torch.float32, torch.float64)
```

### Comparing `ml-starter-0.0.59/ml/utils/device/metal.py` & `ml-starter-0.1.0/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/distributed.py` & `ml-starter-0.1.0/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/image.py` & `ml-starter-0.1.0/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/large_models.py` & `ml-starter-0.1.0/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/logging.py` & `ml-starter-0.1.0/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/meter.py` & `ml-starter-0.1.0/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/parallel.py` & `ml-starter-0.1.0/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/staging.py` & `ml-starter-0.1.0/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/timer.py` & `ml-starter-0.1.0/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/tokens.py` & `ml-starter-0.1.0/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml/utils/torch_distributed.py` & `ml-starter-0.1.0/ml/utils/torch_distributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import torch
 import torch.distributed as dist
 import torch.multiprocessing as mp
 from omegaconf import MISSING
 
 from ml.core.config import conf_field
-from ml.utils.config import is_missing
+from ml.utils.checkpoint import is_missing
 from ml.utils.distributed import get_init_method, get_rank, get_world_size, set_dist
 from ml.utils.logging import INFOALL, configure_logging
 from ml.utils.networking import get_unused_port
 from ml.utils.parallel import init_parallelism
 
 logger: logging.Logger = logging.getLogger(__name__)
```

### Comparing `ml-starter-0.0.59/ml/utils/triton/kmeans.py` & `ml-starter-0.1.0/ml/utils/triton/kmeans.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# mypy: disable-error-code="import"
+# mypy: disable-error-code="import, no-untyped-def"
 # ruff: noqa: ANN001, ANN201, ANN202, N803, N806
 """Implements a Triton kernel for computing K-Means cluster IDs."""
 
 import torch
 import triton
 import triton.language as tl
 from torch import Tensor
 
 
 @triton.jit
-def kmeans_kernel(  # type: ignore[no-untyped-def]
+def kmeans_kernel(
     x_ptr,
     centers_ptr,
     centers_norm_ptr,
     cluster_ids_ptr,
     n_features,
     n_clusters,
     BLOCK_SIZE_F: tl.constexpr,
```

### Comparing `ml-starter-0.0.59/ml/utils/triton/lion.py` & `ml-starter-0.1.0/ml/utils/triton/lion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# mypy: disable-error-code="import"
+# mypy: disable-error-code="import, no-untyped-def"
 # ruff: noqa: ANN001, ANN201, ANN202, N803, N806
 """Implements a Triton kernel for the Lion optimizer."""
 
 from typing import Any
 
 import triton
 import triton.language as tl
 from torch import Tensor, nn
 
 
 @triton.jit
-def update_fn_kernel(  # type: ignore[no-untyped-def]
+def update_fn_kernel(
     p_ptr,
     grad_ptr,
     exp_avg_ptr,
     lr,
     wd,
     beta1,
     beta2,
```

### Comparing `ml-starter-0.0.59/ml/utils/video.py` & `ml-starter-0.1.0/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.0/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.59
+Version: 0.1.0
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.59/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.0/ml_starter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
 ml/utils/audio.py
 ml/utils/augmentation.py
 ml/utils/caching.py
 ml/utils/checkpoint.py
 ml/utils/checks.py
 ml/utils/cli.py
 ml/utils/colors.py
-ml/utils/config.py
 ml/utils/data.py
 ml/utils/datetime.py
 ml/utils/distributed.py
 ml/utils/image.py
 ml/utils/large_models.py
 ml/utils/logging.py
 ml/utils/meter.py
```

### Comparing `ml-starter-0.0.59/pyproject.toml` & `ml-starter-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.59/setup.py` & `ml-starter-0.1.0/setup.py`

 * *Files identical despite different names*

