# Comparing `tmp/waffle_hub-0.2.4.tar.gz` & `tmp/waffle_hub-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.2.4.tar", last modified: Fri Jun 16 03:50:04 2023, max compression
+gzip compressed data, was "waffle_hub-0.2.5.tar", last modified: Sat Jun 24 03:57:50 2023, max compression
```

## Comparing `waffle_hub-0.2.4.tar` & `waffle_hub-0.2.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/LICENSE
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4430 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3349 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      386 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2935 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7890 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/tests/test_cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    14759 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/tests/test_dataset.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3169 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/tests/test_ddp.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10512 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/tests/test_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2042 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/dataset/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/dataset/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/dataset/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      239 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/dataset/adapter/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3267 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/adapter/autocare_dlt.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2956 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/adapter/coco.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4859 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/adapter/transformers.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7226 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/adapter/yolo.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      633 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    59902 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/dataset/dataset.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/experimental/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/experimental/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/experimental/auto_label/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/experimental/auto_label/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/experimental/auto_label/grounding_dino.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/experimental/serve.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       39 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10228 2023-06-16 03:37:26.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4376 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/config.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5865 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       77 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2160 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/config.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8490 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/train_input_helper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10453 2023-06-16 03:37:26.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/transformers_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3932 2023-06-16 03:37:26.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/config.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    12669 2023-06-16 03:37:26.000000 waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      585 2023-06-16 03:34:36.000000 waffle_hub-0.2.4/waffle_hub/hub/cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    46376 2023-06-16 03:37:26.000000 waffle_hub-0.2.4/waffle_hub/hub/hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/hub/model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/hub/model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    13840 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/hub/model/wrapper.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/schema/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1169 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/base_schema.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1699 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/configs.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      378 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/schema/evaluate.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/schema/fields/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/fields/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    17217 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/fields/annotation.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1455 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/fields/base_field.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7241 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/fields/category.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2599 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/fields/image.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      496 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/schema/result.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3462 2023-06-16 03:34:37.000000 waffle_hub-0.2.4/waffle_hub/utils/base_cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/utils/callback.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1686 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/utils/conversion.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5650 2023-06-12 07:00:05.000000 waffle_hub-0.2.4/waffle_hub/utils/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4200 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/utils/draw.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4420 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/utils/evaluate.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      631 2023-06-12 07:51:09.000000 waffle_hub-0.2.4/waffle_hub/utils/process.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-16 03:50:04.413252 waffle_hub-0.2.4/waffle_hub.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4430 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2242 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      224 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      308 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-06-16 03:50:04.000000 waffle_hub-0.2.4/waffle_hub.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/LICENSE
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4430 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3349 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      386 2023-06-24 03:55:49.000000 waffle_hub-0.2.5/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2935 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7833 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/tests/test_cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    14759 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/tests/test_dataset.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4581 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/tests/test_ddp.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10437 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/tests/test_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2292 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/dataset/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/dataset/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/dataset/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      239 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/dataset/adapter/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3267 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/dataset/adapter/autocare_dlt.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2956 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/dataset/adapter/coco.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4859 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/dataset/adapter/transformers.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7226 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/dataset/adapter/yolo.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      633 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/dataset/cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    59997 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/dataset/dataset.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/experimental/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/experimental/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/experimental/auto_label/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/experimental/auto_label/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/experimental/serve.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       39 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10235 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4515 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/config.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5865 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       77 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2220 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/config.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     9156 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/train_input_helper.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10577 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/transformers_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/adapter/ultralytics/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4027 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/ultralytics/config.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    12669 2023-06-16 03:37:26.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      585 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/hub/cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    49030 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/model/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    13900 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/model/wrapper.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/schema/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1169 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/base_schema.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1699 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/configs.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      378 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/schema/evaluate.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/schema/fields/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/fields/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    17217 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/fields/annotation.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1455 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/fields/base_field.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7241 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/fields/category.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2599 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/fields/image.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      537 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/schema/result.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3462 2023-06-16 03:34:37.000000 waffle_hub-0.2.5/waffle_hub/utils/base_cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/utils/callback.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1686 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/utils/conversion.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5616 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/utils/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4200 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/utils/draw.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4420 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/utils/evaluate.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      631 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/utils/process.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4430 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2242 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      224 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      308 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.2.4/LICENSE` & `waffle_hub-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/PKG-INFO` & `waffle_hub-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.2.4
+Version: 0.2.5
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.4 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.5 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.4/README.md` & `waffle_hub-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/setup.py` & `waffle_hub-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/tests/test_cli.py` & `waffle_hub-0.2.5/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     assert (test_dir / "hubs" / "test").exists()
 
 
 def test_hub_train(test_dir: Path):
     cmd = f'python -m waffle_hub.hub.cli train \
         --root-dir {test_dir / "hubs"} \
         --name test \
-        --dataset-path {test_dir / "datasets" / "from_coco" / "exports" / "YOLO" } \
+        --dataset {test_dir / "datasets" / "from_coco"} \
         --epochs 1 \
         --batch-size 4 \
         --image-size 16 \
         --learning-rate 0.001 \
         --letter-box \
         --device cpu \
         --workers 0 \
@@ -237,16 +237,15 @@
     assert (test_dir / "hubs" / "test" / "inferences").exists()
 
 
 def test_hub_evaluate(test_dir: Path):
     cmd = f'python -m waffle_hub.hub.cli evaluate \
         --name test \
         --root-dir {test_dir / "hubs"} \
-        --dataset-name from_coco \
-        --dataset-root-dir {test_dir / "datasets"} \
+        --dataset {test_dir / "datasets" / "from_coco"} \
         --set-name test \
         --device cpu \
         --workers 0 \
     '
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "hubs" / "test" / "evaluate.json").exists()
```

### Comparing `waffle_hub-0.2.4/tests/test_dataset.py` & `waffle_hub-0.2.5/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/tests/test_hub.py` & `waffle_hub-0.2.5/tests/test_hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     InferenceResult,
     TrainResult,
 )
 
 
 def _train(hub, dataset: Dataset, image_size: int, hold: bool = True):
     result: TrainResult = hub.train(
-        dataset_path=dataset.export(hub.backend),
+        dataset=dataset,
         epochs=1,
         image_size=image_size,
         batch_size=4,
         pretrained_model=None,
         device="cpu",
         workers=0,
         hold=hold,
@@ -29,40 +29,39 @@
     if not hold:
         assert hasattr(result, "callback")
         while not result.callback.is_finished() and not result.callback.is_failed():
             time.sleep(1)
         assert result.callback.is_finished()
         assert not result.callback.is_failed()
 
-    print(hub.metric_file, result.metrics)
     assert len(result.metrics) >= 1
+    assert len(result.eval_metrics) >= 1
     assert Path(result.best_ckpt_file).exists()
     # assert Path(result.last_ckpt_file).exists()
 
     return result
 
 
 def _evaluate(hub, dataset: Dataset, hold: bool = True):
 
     result: EvaluateResult = hub.evaluate(
-        dataset_name=dataset.name,
-        dataset_root_dir=dataset.root_dir,
+        dataset=dataset,
         device="cpu",
         workers=0,
         hold=hold,
     )
 
     if not hold:
         assert hasattr(result, "callback")
         while not result.callback.is_finished() and not result.callback.is_failed():
             time.sleep(1)
         assert result.callback.is_finished()
         assert not result.callback.is_failed()
 
-    assert len(result.metrics) >= 1
+    assert len(result.eval_metrics) >= 1
 
     return result
 
 
 def _inference(hub, source: str, hold: bool = True):
 
     result: InferenceResult = hub.inference(
```

### Comparing `waffle_hub-0.2.4/waffle_hub/__init__.py` & `waffle_hub-0.2.5/waffle_hub/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 import enum
 from collections import OrderedDict
 
-
-BACKEND_MAP = OrderedDict({
-    "ultralytics": {
-        "import_path": "waffle_hub.hub.adapter.ultralytics",
-        "class_name": "UltralyticsHub",
-    },
-    "autocare_dlt": {
-        "import_path": "waffle_hub.hub.adapter.autocare_dlt",
-        "class_name": "AutocareDLTHub",
-    },
-    "transformers": {
-        "import_path": "waffle_hub.hub.adapter.transformers",
-        "class_name": "TransformersHub",
-    },
-})
+BACKEND_MAP = OrderedDict(
+    {
+        "ultralytics": {
+            "import_path": "waffle_hub.hub.adapter.ultralytics",
+            "class_name": "UltralyticsHub",
+        },
+        "autocare_dlt": {
+            "import_path": "waffle_hub.hub.adapter.autocare_dlt",
+            "class_name": "AutocareDLTHub",
+        },
+        "transformers": {
+            "import_path": "waffle_hub.hub.adapter.transformers",
+            "class_name": "TransformersHub",
+        },
+    }
+)
 
 
 class CustomEnumMeta(enum.EnumMeta):
     def __contains__(cls, item):
         if isinstance(item, str):
             return item.upper() in cls._member_names_
         return super().__contains__(item)
@@ -85,7 +86,16 @@
     TEXT_RECOGNITION = enum.auto()
     REGRESSION = enum.auto()
 
 
 class SplitMethod(BaseEnum):
     RANDOM = enum.auto()
     STRATIFIED = enum.auto()
+
+
+EXPORT_MAP = {
+    DataType.YOLO: "YOLO",
+    DataType.ULTRALYTICS: "YOLO",
+    DataType.COCO: "COCO",
+    DataType.AUTOCARE_DLT: "AUTOCARE_DLT",
+    DataType.TRANSFORMERS: "TRANSFORMERS",
+}
```

### Comparing `waffle_hub-0.2.4/waffle_hub/dataset/adapter/autocare_dlt.py` & `waffle_hub-0.2.5/waffle_hub/dataset/adapter/autocare_dlt.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/dataset/adapter/coco.py` & `waffle_hub-0.2.5/waffle_hub/dataset/adapter/coco.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/dataset/adapter/transformers.py` & `waffle_hub-0.2.5/waffle_hub/dataset/adapter/transformers.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/dataset/adapter/yolo.py` & `waffle_hub-0.2.5/waffle_hub/dataset/adapter/yolo.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/dataset/cli.py` & `waffle_hub-0.2.5/waffle_hub/dataset/cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/dataset/dataset.py` & `waffle_hub-0.2.5/waffle_hub/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import logging
+import os
 import random
 import shutil
-import sys
 import warnings
-from collections import Counter, OrderedDict, defaultdict
+from collections import Counter, defaultdict
 from functools import cached_property
 from pathlib import Path
 from tempfile import mkdtemp
 from typing import Union
 
 import cv2
 import PIL.Image
@@ -17,15 +17,15 @@
 from waffle_utils.file import io, network
 from waffle_utils.file.search import get_files, get_image_files
 from waffle_utils.log import datetime_now
 from waffle_utils.utils import type_validator
 
 from datasets import Dataset as HFDataset
 from datasets import DatasetDict, load_from_disk
-from waffle_hub import DataType, SplitMethod, TaskType
+from waffle_hub import EXPORT_MAP, DataType, SplitMethod, TaskType
 from waffle_hub.dataset.adapter import (
     export_autocare_dlt,
     export_coco,
     export_transformers,
     export_yolo,
 )
 from waffle_hub.schema import Annotation, Category, DatasetInfo, Image
@@ -59,15 +59,15 @@
         created: str = None,
         root_dir: str = None,
     ):
         self.name = name
         self.task = task
         self.created = created
 
-        self.root_dir = Path(root_dir) if root_dir else Dataset.DEFAULT_DATASET_ROOT_DIR
+        self.root_dir = root_dir
 
     def __repr__(self):
         return self.get_dataset_info().__repr__()
 
     # properties
     @property
     def name(self):
@@ -80,34 +80,45 @@
 
     @property
     def task(self):
         return self.__task
 
     @task.setter
     def task(self, v):
+        v = str(v).upper()
         if v not in TaskType:
             raise ValueError(f"Invalid task type: {v}" f"Available task types: {list(TaskType)}")
-        self.__task = str(v).upper()
+        self.__task = v
 
     @property
     def created(self):
         return self.__created
 
     @created.setter
     def created(self, v):
         self.__created = v or datetime_now()
 
     @property
-    def root_dir(self):
+    def root_dir(self) -> Path:
         return self.__root_dir
 
     @root_dir.setter
-    @type_validator(Path)
+    @type_validator(Path, strict=False)
     def root_dir(self, v):
-        self.__root_dir = v
+        self.__root_dir = Dataset.parse_root_dir(v)
+        logger.info(f"Dataset root directory: {self.__root_dir}")
+
+    @classmethod
+    def parse_root_dir(cls, v):
+        if v:
+            return Path(v)
+        elif os.getenv("WAFFLE_DATASET_ROOT_DIR", None):
+            return Path(os.getenv("WAFFLE_DATASET_ROOT_DIR"))
+        else:
+            return Dataset.DEFAULT_DATASET_ROOT_DIR
 
     # cached properties
     @cached_property
     def dataset_dir(self) -> Path:
         return self.root_dir / self.name
 
     @cached_property
@@ -441,15 +452,15 @@
             >>> ds = Dataset.load("my_dataset")
             >>> ds.name
             'my_dataset'  # dataset name
 
         Returns:
             Dataset: Dataset Class
         """
-        root_dir = Path(root_dir) if root_dir else Dataset.DEFAULT_DATASET_ROOT_DIR
+        root_dir = Dataset.parse_root_dir(root_dir)
         dataset_info_file = root_dir / name / Dataset.DATASET_INFO_FILE_NAME
         if not dataset_info_file.exists():
             raise FileNotFoundError(f"{dataset_info_file} has not been created.")
         dataset_info = DatasetInfo.load(dataset_info_file)
         return cls(**dataset_info.to_dict(), root_dir=root_dir)
 
     @classmethod
@@ -1009,17 +1020,17 @@
                     )
                     ds.add_annotations([annotation])
 
                 # raw
                 dst = ds.raw_image_dir / f"{image_id}{image_path.suffix}"
                 io.copy_file(image_path, dst)
 
-        if task == "object_detection":
+        if task == TaskType.OBJECT_DETECTION:
             _import = _import_object_detection
-        elif task == "classification":
+        elif task == TaskType.CLASSIFICATION:
             _import = _import_classification
         else:
             raise ValueError(f"Unsupported task: {task}")
 
         info = io.load_yaml(yaml_path)
         yolo_root_dir = Path(info["path"])
 
@@ -1081,15 +1092,15 @@
             is_splited = True
         elif isinstance(dataset, HFDataset):
             is_splited = False
         else:
             raise ValueError("dataset should be Dataset or DatasetDict")
 
         def _import(dataset: HFDataset, task: str, image_ids: list[int]):
-            if task == "object_detection":
+            if task == TaskType.OBJECT_DETECTION:
                 if not ds.get_categories():
                     categories = dataset.features["objects"].feature["category"].names
                     for category_id, category_name in enumerate(categories):
                         category = Category.object_detection(
                             category_id=category_id + 1,
                             supercategory="object",
                             name=category_name,
@@ -1119,15 +1130,15 @@
                             image_id=image.image_id,
                             category_id=category_id + 1,
                             area=area,
                             bbox=bbox,
                         )
                         ds.add_annotations([annotation])
 
-            elif task == "classification":
+            elif task == TaskType.CLASSIFICATION:
                 if not ds.get_categories():
                     categories = dataset.features["label"].names
                     for category_id, category_name in enumerate(categories):
                         category = Category.classification(
                             category_id=category_id + 1,
                             supercategory="object",
                             name=category_name,
@@ -1224,15 +1235,15 @@
 
         Args:
             root_dir (str, optional): dataset root directory. Defaults to None.
 
         Returns:
             list[str]: dataset name list.
         """
-        root_dir = Path(root_dir if root_dir else Dataset.DEFAULT_DATASET_ROOT_DIR)
+        root_dir = Dataset.parse_root_dir(root_dir)
 
         if not root_dir.exists():
             return []
 
         dataset_name_list = []
         for dataset_dir in root_dir.iterdir():
             if dataset_dir.is_dir():
@@ -1590,25 +1601,22 @@
 
         Returns:
             str: exported dataset directory
         """
 
         self.check_trainable()
 
+        export_dir: Path = self.export_dir / EXPORT_MAP[data_type.upper()]
         if data_type in [DataType.YOLO, DataType.ULTRALYTICS]:
-            export_dir: Path = self.export_dir / str(DataType.YOLO)
             export_function = export_yolo
         elif data_type in [DataType.COCO]:
-            export_dir: Path = self.export_dir / str(DataType.COCO)
             export_function = export_coco
         elif data_type in [DataType.AUTOCARE_DLT]:
-            export_dir: Path = self.export_dir / str(DataType.AUTOCARE_DLT)
             export_function = export_autocare_dlt
         elif data_type in [DataType.TRANSFORMERS]:
-            export_dir: Path = self.export_dir / str(DataType.TRANSFORMERS)
             export_function = export_transformers
 
         else:
             raise ValueError(f"Invalid data_type: {data_type}")
 
         try:
             if export_dir.exists():
```

### Comparing `waffle_hub-0.2.4/waffle_hub/experimental/auto_label/grounding_dino.py` & `waffle_hub-0.2.5/waffle_hub/experimental/auto_label/grounding_dino.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/experimental/serve.py` & `waffle_hub-0.2.5/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py` & `waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         if self.model_type == "LicencePlateRecognition":
             data_config["data"]["mode"] = "lpr"
 
         cfg.data_config = self.artifact_dir / "data.json"
         io.save_json(data_config, cfg.data_config, create_directory=True)
         categories = (
             self.categories
-            if self._Hub__task == "classification"
+            if self._Hub__task == TaskType.CLASSIFICATION
             else [x["name"] for x in self.categories]
         )
 
         model_config = get_model_config(
             self.model_type,
             self.model_size,
             categories,
```

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/config.py` & `waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,58 @@
+from waffle_hub import TaskType
 from waffle_hub.schema.configs import TrainConfig
 
 # Common
 MODEL_TYPES = {
-    "object_detection": {"YOLOv5": list("sml")},
-    "classification": {"Classifier": list("sml")},
-    "text_recognition": {"TextRecognition": list("sml"), "LicencePlateRecognition": list("sml")},
+    TaskType.OBJECT_DETECTION: {"YOLOv5": list("sml")},
+    TaskType.CLASSIFICATION: {"Classifier": list("sml")},
+    TaskType.TEXT_RECOGNITION: {
+        "TextRecognition": list("sml"),
+        "LicencePlateRecognition": list("sml"),
+    },
 }
 
 # Backend Specifics
 DATA_TYPE_MAP = {
-    "object_detection": "COCODetectionDataset",
-    "classification": "COCOClassificationDataset",
-    "text_recognition": "COCOTextRecognitionDataset",
+    TaskType.OBJECT_DETECTION: "COCODetectionDataset",
+    TaskType.CLASSIFICATION: "COCOClassificationDataset",
+    TaskType.TEXT_RECOGNITION: "COCOTextRecognitionDataset",
 }
 
 WEIGHT_PATH = {
-    "object_detection": {
+    TaskType.OBJECT_DETECTION: {
         "YOLOv5": {
             "s": "temp/autocare_dlt/detectors/small/model.pth",
             "m": "temp/autocare_dlt/detectors/medium/model.pth",
             "l": "temp/autocare_dlt/detectors/large/model.pth",
         }
     },
-    "classification": {
+    TaskType.CLASSIFICATION: {
         "Classifier": {
             "s": "temp/autocare_dlt/classifiers/small/model.pth",
             "m": "temp/autocare_dlt/classifiers/medium/model.pth",
             "l": "temp/autocare_dlt/classifiers/large/model.pth",
         }
     },
-    "text_recognition": {
+    TaskType.TEXT_RECOGNITION: {
         "TextRecognition": {
             "s": "temp/autocare_dlt/text_recognizers/small/model.pth",
             "m": "temp/autocare_dlt/text_recognizers/small/model.pth",
             "l": "temp/autocare_dlt/text_recognizers/small/model.pth",
         },
         "LicencePlateRecognition": {
             "s": "temp/autocare_dlt/text_recognizers/small/model.pth",
             "m": "temp/autocare_dlt/text_recognizers/small/model.pth",
             "l": "temp/autocare_dlt/text_recognizers/small/model.pth",
         },
     },
 }
 
 DEFAULT_PARAMS = {
-    "object_detection": {
+    TaskType.OBJECT_DETECTION: {
         "YOLOv5": {
             "s": TrainConfig(
                 epochs=50,
                 image_size=[640, 640],
                 learning_rate=0.01,
                 letter_box=True,
                 batch_size=32,
@@ -65,15 +69,15 @@
                 image_size=[640, 640],
                 learning_rate=0.01,
                 letter_box=True,
                 batch_size=8,
             ),
         }
     },
-    "classification": {
+    TaskType.CLASSIFICATION: {
         "Classifier": {
             "s": TrainConfig(
                 epochs=50,
                 image_size=[224, 224],
                 learning_rate=0.01,
                 letter_box=False,
                 batch_size=256,
@@ -90,15 +94,15 @@
                 image_size=[224, 224],
                 learning_rate=0.01,
                 letter_box=False,
                 batch_size=64,
             ),
         }
     },
-    "text_recognition": {
+    TaskType.TEXT_RECOGNITION: {
         "TextRecognition": {
             "s": TrainConfig(
                 epochs=50,
                 image_size=[224, 224],
                 learning_rate=0.01,
                 letter_box=False,
                 batch_size=256,
```

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py` & `waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py` & `waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/config.py` & `waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,34 @@
+from waffle_hub import TaskType
 from waffle_hub.schema.configs import TrainConfig
 
 # Common
 MODEL_TYPES = {
-    "object_detection": {
+    TaskType.OBJECT_DETECTION: {
         "DETA": {
             "base": "jozhang97/deta-resnet-50",
         },
         "DETR": {
             "base": "facebook/detr-resnet-50",
             "large": "facebook/detr-resnet-101",
         },
         "YOLOS": {
             "tiny": "hustvl/yolos-tiny",
         },
     },
-    "classification": {
+    TaskType.CLASSIFICATION: {
         "ViT": {
             "tiny": "WinKawaks/vit-tiny-patch16-224",
             "base": "google/vit-base-patch16-224",
         }
     },
 }
 
 DEFAULT_PARAMS = {
-    "object_detection": {
+    TaskType.OBJECT_DETECTION: {
         "DETA": {
             "base": TrainConfig(
                 epochs=50,
                 image_size=[800, 800],
                 learning_rate=5e-05,  # TODO: implement letter_box
                 letter_box=True,
                 batch_size=1,
@@ -55,15 +56,15 @@
                 image_size=[800, 800],
                 learning_rate=5e-05,
                 letter_box=True,  # TODO: implement letter_box
                 batch_size=16,
             ),
         },
     },
-    "classification": {
+    TaskType.CLASSIFICATION: {
         "ViT": {
             "tiny": TrainConfig(
                 epochs=50,
                 image_size=[224, 224],
                 learning_rate=5e-05,
                 letter_box=False,
                 batch_size=128,
```

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/train_input_helper.py` & `waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/train_input_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,38 @@
     image_processor: AutoImageProcessor = None
     training_args: TrainingArguments = None
     collator: Callable = None
     model: _BaseAutoModelClass = None
     compute_metrics: Callable = None
 
 
+class customTrainingArguments(TrainingArguments):
+    def __init__(self, *args, **kwargs):
+        self._device = kwargs.pop("device")
+        super().__init__(*args, **kwargs)
+
+    @property
+    def device(self) -> "torch.device":
+        if self._device == "cpu":
+            return torch.device("cpu")
+        elif "," in self._device:
+            return torch.device("cuda")
+        else:
+            return torch.device(f"cuda:{self._device}")
+
+    @property
+    def n_gpu(self) -> int:
+        if self._device == "cpu":
+            return 0
+        elif "," in self._device:
+            return len(self._device.split(","))
+        else:
+            return 1
+
+
 class TrainInputHelper(ABC):
     """
     This class is designed to assist with passing arguments to the Transformers's Trainer function.
     """
 
     def __init__(self, pretrained_model: str, image_size: Union[int, list[int]]) -> None:
         self.pretrained_model = pretrained_model
```

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/adapter/transformers/transformers_hub.py` & `waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/transformers_hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 from torchvision import transforms as T
 from transformers import (
     AutoImageProcessor,
     AutoModelForImageClassification,
     AutoModelForObjectDetection,
     Trainer,
     TrainerCallback,
-    TrainingArguments,
 )
 from transformers.utils import ModelOutput
 from waffle_utils.file import io
 
 from datasets import load_from_disk
 from waffle_hub import TaskType
 from waffle_hub.hub import Hub
 from waffle_hub.hub.adapter.transformers.train_input_helper import (
     ClassifierInputHelper,
     ObjectDetectionInputHelper,
+    customTrainingArguments,
 )
 from waffle_hub.hub.model.wrapper import ModelWrapper
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 
 from .config import DEFAULT_PARAMS, MODEL_TYPES
 
@@ -137,54 +137,54 @@
             root_dir=root_dir,
         )
 
     def on_train_start(self, cfg: TrainConfig):
         # overwrite train config with default config
         cfg.pretrained_model = self.MODEL_TYPES[self.task][self.model_type][self.model_size]
 
-        # setting
-        if cfg.device != "cpu":
-            os.environ["CUDA_VISIBLE_DEVICES"] = cfg.device
-        else:
-            os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
-
         dataset = load_from_disk(cfg.dataset_path)
 
-        if self.task == "classification":
+        if self.task == TaskType.CLASSIFICATION:
             helper = ClassifierInputHelper(cfg.pretrained_model, cfg.image_size)
             cfg.train_input = helper.get_train_input()
             categories = dataset["train"].features["label"].names
             id2label = {index: x for index, x in enumerate(categories, start=0)}
             cfg.train_input.model = AutoModelForImageClassification.from_pretrained(
                 cfg.pretrained_model,
                 num_labels=len(id2label),
                 ignore_mismatched_sizes=True,
             )
 
-        elif self.task == "object_detection":
+        elif self.task == TaskType.OBJECT_DETECTION:
             helper = ObjectDetectionInputHelper(cfg.pretrained_model, cfg.image_size)
             cfg.train_input = helper.get_train_input()
             categories = dataset["train"].features["objects"].feature["category"].names
             id2label = {index: x for index, x in enumerate(categories, start=0)}
             label2id = {x: index for index, x in enumerate(categories, start=0)}
             cfg.train_input.model = AutoModelForObjectDetection.from_pretrained(
                 cfg.pretrained_model,
                 id2label=id2label,
                 label2id=label2id,
                 ignore_mismatched_sizes=True,
             )
         else:
             raise NotImplementedError
 
+        if cfg.device == "cpu":
+            os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
+            cfg.train_input.model = cfg.train_input.model.to("cpu")
+        elif "," in cfg.device:
+            os.environ["CUDA_VISIBLE_DEVICES"] = cfg.device
+
         transforms = helper.get_transforms()
         dataset["train"] = dataset["train"].with_transform(transforms)
         dataset["val"] = dataset["val"].with_transform(transforms)
         cfg.train_input.dataset = dataset
 
-        cfg.train_input.training_args = TrainingArguments(
+        cfg.train_input.training_args = customTrainingArguments(
             output_dir=str(self.artifact_dir),
             per_device_train_batch_size=cfg.batch_size,
             num_train_epochs=cfg.epochs,
             remove_unused_columns=False,
             push_to_hub=False,
             logging_strategy="epoch" if cfg.verbose else "no",
             evaluation_strategy="epoch",
@@ -192,18 +192,18 @@
             learning_rate=cfg.learning_rate,
             dataloader_num_workers=cfg.workers,
             seed=cfg.seed,
             metric_for_best_model="eval_loss",
             greater_is_better=False,
             save_total_limit=1,
             load_best_model_at_end=False,
+            device=cfg.device,
         )
 
     def training(self, cfg: TrainConfig, callback: TrainCallback):
-
         trainer = Trainer(
             model=cfg.train_input.model,
             args=cfg.train_input.training_args,
             data_collator=cfg.train_input.collator,
             train_dataset=cfg.train_input.dataset["train"],
             eval_dataset=cfg.train_input.dataset["val"],
             tokenizer=cfg.train_input.image_processor,
```

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/config.py` & `waffle_hub-0.2.5/waffle_hub/hub/adapter/ultralytics/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
+from waffle_hub import TaskType
 from waffle_hub.schema.configs import TrainConfig
 
 # Common
 MODEL_TYPES = {
-    "object_detection": {"yolov8": list("nsmlx")},
-    "classification": {"yolov8": list("nsmlx")},
-    "instance_segmentation": {"yolov8": list("nsmlx")},
+    TaskType.OBJECT_DETECTION: {"yolov8": list("nsmlx")},
+    TaskType.CLASSIFICATION: {"yolov8": list("nsmlx")},
+    TaskType.INSTANCE_SEGMENTATION: {"yolov8": list("nsmlx")},
     # "keypoint_detection": {"yolov8": list("nsmlx")},
 }
 
 # Backend Specifics
 TASK_MAP = {
-    "object_detection": "detect",
-    "classification": "classify",
-    "instance_segmentation": "segment"
+    TaskType.OBJECT_DETECTION: "detect",
+    TaskType.CLASSIFICATION: "classify",
+    TaskType.INSTANCE_SEGMENTATION: "segment"
     # "keypoint_detection": "pose"
 }
 TASK_SUFFIX = {
     "detect": "",
     "classify": "-cls",
     "segment": "-seg",
 }
 
 DEFAULT_PARAMS = {
-    "object_detection": {
+    TaskType.OBJECT_DETECTION: {
         "yolov8": {
             "n": TrainConfig(
                 epochs=50,
                 image_size=[640, 640],
                 learning_rate=0.01,
                 letter_box=True,
                 batch_size=64,
@@ -57,15 +58,15 @@
                 image_size=[640, 640],
                 learning_rate=0.01,
                 letter_box=True,
                 batch_size=8,
             ),
         }
     },
-    "classification": {
+    TaskType.CLASSIFICATION: {
         "yolov8": {
             "n": TrainConfig(
                 epochs=50,
                 image_size=[224, 224],
                 learning_rate=0.01,
                 letter_box=False,
                 batch_size=512,
@@ -96,15 +97,15 @@
                 image_size=[224, 224],
                 learning_rate=0.01,
                 letter_box=False,
                 batch_size=64,
             ),
         }
     },
-    "instance_segmentation": {
+    TaskType.INSTANCE_SEGMENTATION: {
         "yolov8": {
             "n": TrainConfig(
                 epochs=50,
                 image_size=[640, 640],
                 learning_rate=0.01,
                 letter_box=True,
                 batch_size=32,
```

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.2.5/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/cli.py` & `waffle_hub-0.2.5/waffle_hub/hub/cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/hub.py` & `waffle_hub-0.2.5/waffle_hub/hub/hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import cv2
 import numpy as np
 import torch
 import tqdm
 from waffle_utils.file import io
 from waffle_utils.utils import type_validator
 
-from waffle_hub import BACKEND_MAP, TaskType
+from waffle_hub import BACKEND_MAP, EXPORT_MAP, TaskType
 from waffle_hub.dataset import Dataset
 from waffle_hub.hub.model.wrapper import get_parser
 from waffle_hub.schema.configs import (
     EvaluateConfig,
     ExportConfig,
     InferenceConfig,
     ModelConfig,
@@ -59,15 +59,15 @@
     # Hub Spec. must have
     BACKEND_NAME = None
     MODEL_TYPES = None
     MULTI_GPU_TRAIN = None
     DEFAULT_PARAMS = None
 
     # directory settings
-    DEFAULT_ROOT_DIR = Path("./hubs")
+    DEFAULT_HUB_ROOT_DIR = Path("./hubs")
 
     ARTIFACT_DIR = Path("artifacts")
 
     INFERENCE_DIR = Path("inferences")
     EXPORT_DIR = Path("exports")
 
     DRAW_DIR = Path("draws")
@@ -115,15 +115,15 @@
             raise AttributeError("DEFAULT_PARAMS must be specified.")
 
         self.name: str = name
         self.task: str = task
         self.model_type: str = model_type
         self.model_size: str = model_size
         self.categories: list[dict] = categories
-        self.root_dir: Path = Path(root_dir) if root_dir else None
+        self.root_dir: Path = root_dir
 
         self.backend: str = backend
         self.version: str = version
 
         # check task supports
         if self.task not in self.MODEL_TYPES:
             io.remove_directory()
@@ -300,15 +300,15 @@
         Returns:
             Hub: Hub instance
         """
         if name in cls.get_hub_list(root_dir):
             raise ValueError(f"{name} already exists. Try another name.")
 
         backend = backend if backend else cls.get_available_backends()[0]
-        task = task if task else cls.get_available_tasks(backend)[0]
+        task = str(task).upper() if task else cls.get_available_tasks(backend)[0]
         model_type = model_type if model_type else cls.get_available_model_types(backend, task)[0]
         model_size = (
             model_size if model_size else cls.get_available_model_sizes(backend, task, model_type)[0]
         )
 
         return cls.get_hub_class(backend)(
             name=name,
@@ -329,15 +329,15 @@
 
         Raises:
             FileNotFoundError: if hub is not exist in root_dir
 
         Returns:
             Hub: Hub instance
         """
-        root_dir = Path(root_dir if root_dir else Hub.DEFAULT_ROOT_DIR)
+        root_dir = Hub.parse_root_dir(root_dir)
         model_config_file = root_dir / name / Hub.MODEL_CONFIG_FILE
         if not model_config_file.exists():
             raise FileNotFoundError(f"Model[{name}] does not exists. {model_config_file}")
         model_config = ModelConfig.load(model_config_file)
         return cls.get_hub_class(model_config.backend)(
             **{
                 **model_config.to_dict(),
@@ -376,15 +376,15 @@
 
         Args:
             root_dir (str, optional): hub root directory. Defaults to None.
 
         Returns:
             list[str]: hub name list
         """
-        root_dir = Path(root_dir if root_dir else Hub.DEFAULT_ROOT_DIR)
+        root_dir = Hub.parse_root_dir(root_dir)
 
         if not root_dir.exists():
             return []
 
         hub_name_list = []
         for hub_dir in root_dir.iterdir():
             if hub_dir.is_dir():
@@ -408,24 +408,34 @@
     def root_dir(self) -> Path:
         """Root Directory"""
         return self.__root_dir
 
     @root_dir.setter
     @type_validator(Path, strict=False)
     def root_dir(self, v):
-        self.__root_dir = Path(v) if v else Hub.DEFAULT_ROOT_DIR
+        self.__root_dir = Hub.parse_root_dir(v)
+        logger.info(f"Hub root directory: {self.root_dir}")
+
+    @classmethod
+    def parse_root_dir(cls, v):
+        if v:
+            return Path(v)
+        elif os.getenv("WAFFLE_HUB_ROOT_DIR", None):
+            return Path(os.getenv("WAFFLE_HUB_ROOT_DIR"))
+        else:
+            return Hub.DEFAULT_HUB_ROOT_DIR
 
     @property
     def task(self) -> str:
         """Task Name"""
         return self.__task
 
     @task.setter
     def task(self, v):
-        v = str(v).lower()  # TODO: MODEL_TYPES should be enum
+        v = str(v).upper()
         if v not in self.MODEL_TYPES:
             raise ValueError(f"Task {v} is not supported. Choose one of {self.MODEL_TYPES}")
         self.__task = v
 
     @property
     def model_type(self) -> str:
         """Model Type"""
@@ -477,14 +487,16 @@
     @property
     def categories(self) -> list[dict]:
         return self.__categories
 
     @categories.setter
     @type_validator(list)
     def categories(self, v):
+        if v is None:
+            raise ValueError("Categories must be specified.")
         if not isinstance(v[0], dict):
             v = [{"supercategory": "object", "name": str(n)} for n in v]
         self.__categories = v
 
     @cached_property
     def hub_dir(self) -> Path:
         """Hub(Model) Directory"""
@@ -608,16 +620,19 @@
                 ],
             ]
 
         Returns:
             list[dict]: metrics per epoch
         """
         if not self.metric_file.exists():
-            warnings.warn("Metric file is not exist. Train first!")
-            return []
+            raise FileNotFoundError("Metric file is not exist. Train first!")
+
+        if not self.evaluate_file.exists():
+            raise FileNotFoundError("Evaluate file is not exist. Train first!")
+
         return io.load_json(self.metric_file)
 
     def get_evaluate_result(self) -> list[dict]:
         """Get evaluate result from evaluate file.
 
         Example:
             >>> hub.get_evaluate_result()
@@ -744,18 +759,20 @@
     def on_train_end(self, cfg: TrainConfig):
         pass
 
     def after_train(self, cfg: TrainConfig, result: TrainResult):
         result.best_ckpt_file = self.best_ckpt_file
         result.last_ckpt_file = self.last_ckpt_file
         result.metrics = self.get_metrics()
+        result.eval_metrics = self.get_evaluate_result()
 
     def train(
         self,
-        dataset_path: str,
+        dataset: Union[Dataset, str],
+        dataset_root_dir: str = None,
         epochs: int = None,
         batch_size: int = None,
         image_size: Union[int, list[int]] = None,
         learning_rate: float = None,
         letter_box: bool = None,
         pretrained_model: str = None,
         device: str = "0",
@@ -763,15 +780,16 @@
         seed: int = 0,
         verbose: bool = True,
         hold: bool = True,
     ) -> TrainResult:
         """Start Train
 
         Args:
-            dataset_path (str): dataset path
+            dataset (Union[Dataset, str]): Waffle Dataset object or path or name.
+            dataset_root_dir (str, optional): Waffle Dataset root directory. Defaults to None.
             epochs (int, optional): number of epochs. None to use default. Defaults to None.
             batch_size (int, optional): batch size. None to use default. Defaults to None.
             image_size (Union[int, list[int]], optional): image size. None to use default. Defaults to None.
             learning_rate (float, optional): learning rate. None to use default. Defaults to None.
             letter_box (bool, optional): letter box. None to use default. Defaults to None.
             pretrained_model (str, optional): pretrained model. None to use default. Defaults to None.
             device (str, optional):
@@ -785,15 +803,15 @@
             FileExistsError: if trained artifact exists.
             FileNotFoundError: if can not detect appropriate dataset.
             ValueError: if can not detect appropriate dataset.
             e: something gone wrong with ultralytics
 
         Example:
             >>> train_result = hub.train(
-                    dataset_path=dataset_path,
+                    dataset=dataset,
                     epochs=100,
                     batch_size=16,
                     image_size=640,
                     learning_rate=0.001,
                     letterbox=False,
                     device="0",  # use gpu 0
                     # device="0,1,2,3",  # use gpu 0,1,2,3
@@ -813,25 +831,54 @@
         def inner(callback: TrainCallback, result: TrainResult):
             try:
                 self.before_train(cfg)
                 self.on_train_start(cfg)
                 self.save_train_config(cfg)
                 self.training(cfg, callback)
                 self.on_train_end(cfg)
+                self.evaluate(
+                    dataset=dataset,
+                    batch_size=cfg.batch_size,
+                    image_size=cfg.image_size,
+                    letter_box=cfg.letter_box,
+                    device=cfg.device,
+                    workers=cfg.workers,
+                )
                 self.after_train(cfg, result)
                 callback.force_finish()
             except Exception as e:
                 if self.artifact_dir.exists():
                     io.remove_directory(self.artifact_dir)
                 callback.force_finish()
                 callback.set_failed()
                 raise e
 
+        if isinstance(dataset, (str, Path)):
+            if Path(dataset).exists():
+                dataset = Path(dataset)
+                dataset = Dataset.load(
+                    name=dataset.parts[-1], root_dir=dataset.parents[0].absolute()
+                )
+            elif dataset in Dataset.get_dataset_list(dataset_root_dir):
+                dataset = Dataset.load(name=dataset, root_dir=dataset_root_dir)
+            else:
+                raise FileNotFoundError(f"Dataset {dataset} is not exist.")
+
+        if dataset.task.upper() != self.task.upper():
+            raise ValueError(
+                f"Dataset task is not matched with hub task. Dataset task: {dataset.task}, Hub task: {self.task}"
+            )
+
+        export_dir = dataset.export_dir / EXPORT_MAP[self.backend.upper()]
+        if not export_dir.exists():
+            export_dir = dataset.export(self.backend)
+            logger.info(f"Dataset exported to {export_dir}")
+
         cfg = TrainConfig(
-            dataset_path=dataset_path,
+            dataset_path=export_dir,
             epochs=epochs,
             batch_size=batch_size,
             image_size=image_size,
             learning_rate=learning_rate,
             letter_box=letter_box,
             pretrained_model=pretrained_model,
             device=device,
@@ -918,55 +965,55 @@
             self.evaluate_file,
         )
 
     def on_evaluate_end(self, cfg: EvaluateConfig):
         pass
 
     def after_evaluate(self, cfg: EvaluateConfig, result: EvaluateResult):
-        result.metrics = self.get_evaluate_result()
+        result.eval_metrics = self.get_evaluate_result()
 
     def evaluate(
         self,
-        dataset_name: str,
+        dataset: Union[Dataset, str],
+        dataset_root_dir: str = None,
         set_name: str = "test",
         batch_size: int = 4,
         image_size: Union[int, list[int]] = None,
         letter_box: bool = None,
         confidence_threshold: float = 0.25,
         iou_threshold: float = 0.5,
         half: bool = False,
         workers: int = 2,
         device: str = "0",
         draw: bool = False,
-        dataset_root_dir: str = None,
         hold: bool = True,
     ) -> EvaluateResult:
         """Start Evaluate
 
         Args:
-            dataset_name (str): waffle dataset name.
+            dataset (Union[Dataset, str]): Waffle Dataset object or path or name.
+            dataset_root_dir (str, optional): Waffle Dataset root directory. Defaults to None.
             batch_size (int, optional): batch size. Defaults to 4.
             image_size (Union[int, list[int]], optional): image size. Defaults to None.
             letter_box (bool, optional): letter box. Defaults to None.
             confidence_threshold (float, optional): confidence threshold. Defaults to 0.25.
             iou_threshold (float, optional): iou threshold. Defaults to 0.5.
             half (bool, optional): half. Defaults to False.
             workers (int, optional): workers. Defaults to 2.
             device (str, optional): device. Defaults to "0".
             draw (bool, optional): draw. Defaults to False.
-            dataset_root_dir (str, optional): dataset root dir. Defaults to None.
             hold (bool, optional): hold. Defaults to True.
 
         Raises:
             FileNotFoundError: if can not detect appropriate dataset.
             e: something gone wrong with ultralytics
 
         Examples:
             >>> evaluate_result = hub.evaluate(
-                    dataset_name="detection_dataset",
+                    dataset=detection_dataset,
                     batch_size=4,
                     image_size=640,
                     letterbox=False,
                     confidence_threshold=0.25,
                     iou_threshold=0.5,
                     workers=4,
                     device="0",
@@ -996,27 +1043,42 @@
             except Exception as e:
                 if self.evaluate_file.exists():
                     io.remove_file(self.evaluate_file)
                 callback.force_finish()
                 callback.set_failed()
                 raise e
 
+        if "," in device:
+            warnings.warn("multi-gpu is not supported in evaluation. use first gpu only.")
+            device = device.split(",")[0]
+
+        if isinstance(dataset, (str, Path)):
+            if Path(dataset).exists():
+                dataset = Path(dataset)
+                dataset = Dataset.load(
+                    name=dataset.parts[-1], root_dir=dataset.parents[0].absolute()
+                )
+            elif dataset in Dataset.get_dataset_list(dataset_root_dir):
+                dataset = Dataset.load(name=dataset, root_dir=dataset_root_dir)
+            else:
+                raise FileNotFoundError(f"Dataset {dataset} is not exist.")
+
         cfg = EvaluateConfig(
-            dataset_name=dataset_name,
+            dataset_name=dataset.name,
             set_name=set_name,
             batch_size=batch_size,
             image_size=image_size,
             letter_box=letter_box,
             confidence_threshold=confidence_threshold,
             iou_threshold=iou_threshold,
             half=half,
             workers=workers,
             device="cpu" if device == "cpu" else f"cuda:{device}",
             draw=draw,
-            dataset_root_dir=dataset_root_dir,
+            dataset_root_dir=dataset.root_dir,
         )
 
         callback = EvaluateCallback(100)  # dummy step
         result = EvaluateResult()
         result.callback = callback
 
         if hold:
@@ -1208,21 +1270,21 @@
         image_size = cfg.image_size
         image_size = [image_size, image_size] if isinstance(image_size, int) else image_size
 
         model = self.get_model().half() if cfg.half else self.get_model()
         model = model.to(cfg.device)
 
         input_name = ["inputs"]
-        if self.task == "object_detection":
+        if self.task == TaskType.OBJECT_DETECTION:
             output_names = ["bbox", "conf", "class_id"]
-        elif self.task == "classification":
+        elif self.task == TaskType.CLASSIFICATION:
             output_names = ["predictions"]
-        elif self.task == "instance_segmentation":
+        elif self.task == TaskType.INSTANCE_SEGMENTATION:
             output_names = ["bbox", "conf", "class_id", "masks"]
-        elif self.task == "text_recognition":
+        elif self.task == TaskType.TEXT_RECOGNITION:
             output_names = ["class_ids", "confs"]
         else:
             raise NotImplementedError(f"{self.task} does not support export yet.")
 
         dummy_input = torch.randn(
             cfg.batch_size, 3, *image_size, dtype=torch.float16 if cfg.half else torch.float32
         )
```

### Comparing `waffle_hub-0.2.4/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.2.5/waffle_hub/hub/model/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Union
 
 import numpy as np
 import torch
 import torch.nn.functional as F
 from torchvision.ops import batched_nms
 
+from waffle_hub import TaskType
 from waffle_hub.schema.data import ImageInfo
 from waffle_hub.schema.fields import Annotation
 from waffle_hub.utils.conversion import convert_mask_to_polygon
 
 
 class PreprocessFunction:
     pass
@@ -216,21 +217,21 @@
             )
             parseds.append(parsed)
 
         return parseds
 
 
 def get_parser(task: str):
-    if task == "classification":
+    if task == TaskType.CLASSIFICATION:
         return ClassificationResultParser
-    elif task == "object_detection":
+    elif task == TaskType.OBJECT_DETECTION:
         return ObjectDetectionResultParser
-    elif task == "instance_segmentation":
+    elif task == TaskType.INSTANCE_SEGMENTATION:
         return InstanceSegmentationResultParser
-    elif task == "text_recognition":
+    elif task == TaskType.TEXT_RECOGNITION:
         return TextRecognitionResultParser
 
 
 class ModelWrapper(torch.nn.Module):
     def __init__(
         self,
         model: torch.nn.Module,
```

### Comparing `waffle_hub-0.2.4/waffle_hub/schema/base_schema.py` & `waffle_hub-0.2.5/waffle_hub/schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/schema/configs.py` & `waffle_hub-0.2.5/waffle_hub/schema/configs.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/schema/data.py` & `waffle_hub-0.2.5/waffle_hub/schema/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/schema/fields/annotation.py` & `waffle_hub-0.2.5/waffle_hub/schema/fields/annotation.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/schema/fields/base_field.py` & `waffle_hub-0.2.5/waffle_hub/schema/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/schema/fields/category.py` & `waffle_hub-0.2.5/waffle_hub/schema/fields/category.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/schema/fields/image.py` & `waffle_hub-0.2.5/waffle_hub/schema/fields/image.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/utils/base_cli.py` & `waffle_hub-0.2.5/waffle_hub/utils/base_cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/utils/callback.py` & `waffle_hub-0.2.5/waffle_hub/utils/callback.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/utils/conversion.py` & `waffle_hub-0.2.5/waffle_hub/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/utils/data.py` & `waffle_hub-0.2.5/waffle_hub/utils/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 from waffle_hub.dataset import Dataset
 from waffle_hub.schema.data import ImageInfo
 from waffle_hub.schema.fields import Annotation, Category, Image
 
 
 def get_images(d, recursive: bool = True) -> list[str]:
     exp = "**/*" if recursive else "*"
+    image_paths = []
+    for ext in ["png", "jpg", "jpeg", "bmp", "tif", "tiff"]:
+        image_paths += list(Path(d).glob(exp.lower() + "." + ext))
+        image_paths += list(Path(d).glob(exp.upper() + "." + ext))
     return list(
         set(
             map(
                 str,
-                list(Path(d).glob(exp + ".png"))
-                + list(Path(d).glob(exp + ".jpg"))
-                + list(Path(d).glob(exp + ".PNG"))
-                + list(Path(d).glob(exp + ".JPG")),
+                image_paths,
             )
         )
     )
 
 
 def resize_image(
     image: np.ndarray, image_size: list[int], letter_box: bool = False
@@ -62,41 +63,35 @@
 
             total_pad = h_ - w_
             left = total_pad // 2
             right = total_pad - left
             top, bottom = 0, 0
 
         image = cv2.resize(image, (w_, h_), interpolation=cv2.INTER_CUBIC)
-        image = cv2.copyMakeBorder(
-            image, top, bottom, left, right, None, value=(114, 114, 114)
-        )
+        image = cv2.copyMakeBorder(image, top, bottom, left, right, None, value=(114, 114, 114))
 
     else:
         w_, h_ = W, H
         left, top = 0, 0
         image = cv2.resize(image, (w_, h_), interpolation=cv2.INTER_CUBIC)
 
     return image, ImageInfo(
         ori_shape=(w, h),
         new_shape=(w_, h_),
         input_shape=(W, H),
         pad=(left, top),
     )
 
 
-def get_image_transform(
-    image_size: Union[int, list[int]], letter_box: bool = False
-):
+def get_image_transform(image_size: Union[int, list[int]], letter_box: bool = False):
 
     if isinstance(image_size, int):
         image_size = [image_size, image_size]
 
-    def transform(
-        image: Union[np.ndarray, str]
-    ) -> tuple[torch.Tensor, ImageInfo]:
+    def transform(image: Union[np.ndarray, str]) -> tuple[torch.Tensor, ImageInfo]:
         if isinstance(image, str):
             image = cv2.imread(image)
         image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
         image, image_info = resize_image(image, image_size, letter_box)
         return T.ToTensor()(image), image_info
 
     return transform
@@ -164,29 +159,26 @@
         else:
             set_file = None
 
         self.images: list[Image] = self.dataset.get_images(
             io.load_json(set_file) if set_file else None
         )
         self.image_to_annotations: dict[int, list[Annotation]] = {
-            image.image_id: self.dataset.get_annotations(image.image_id)
-            for image in self.images
+            image.image_id: self.dataset.get_annotations(image.image_id) for image in self.images
         }
 
         self.transform = get_image_transform(image_size, letter_box)
 
     def __len__(self):
         return len(self.images)
 
     def __getitem__(self, idx):
         image = self.images[idx]
         image_path = str(self.image_dir / image.file_name)
-        annotations: list[Annotation] = self.image_to_annotations[
-            image.image_id
-        ]
+        annotations: list[Annotation] = self.image_to_annotations[image.image_id]
 
         image, image_info = self.transform(image_path)
         image_info.image_path = image_path
 
         return image, image_info, annotations
 
     def collate_fn(self, batch):
```

### Comparing `waffle_hub-0.2.4/waffle_hub/utils/draw.py` & `waffle_hub-0.2.5/waffle_hub/utils/draw.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/utils/evaluate.py` & `waffle_hub-0.2.5/waffle_hub/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub/utils/process.py` & `waffle_hub-0.2.5/waffle_hub/utils/process.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.4/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.2.5/waffle_hub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.2.4
+Version: 0.2.5
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.4 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.5 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.4/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.2.5/waffle_hub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

