# Comparing `tmp/refuel-autolabel-0.0.4.tar.gz` & `tmp/refuel-autolabel-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refuel-autolabel-0.0.4.tar", last modified: Sun Jun 18 19:49:40 2023, max compression
+gzip compressed data, was "refuel-autolabel-0.0.5.tar", last modified: Fri Jun 23 23:32:07 2023, max compression
```

## Comparing `refuel-autolabel-0.0.4.tar` & `refuel-autolabel-0.0.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.071488 refuel-autolabel-0.0.4/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1066 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/LICENSE
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11014 2023-06-18 19:49:40.071267 refuel-autolabel-0.0.4/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9005 2023-06-15 15:29:16.000000 refuel-autolabel-0.0.4/README.md
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1922 2023-06-18 19:45:44.000000 refuel-autolabel-0.0.4/pyproject.toml
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       38 2023-06-18 19:49:40.071532 refuel-autolabel-0.0.4/setup.cfg
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.058118 refuel-autolabel-0.0.4/src/
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.062657 refuel-autolabel-0.0.4/src/autolabel/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       63 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/__init__.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.063613 refuel-autolabel-0.0.4/src/autolabel/cache/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       74 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/cache/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      924 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.4/src/autolabel/cache/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1817 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/cache/sqlalchemy_cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9137 2023-06-15 00:37:32.000000 refuel-autolabel-0.0.4/src/autolabel/confidence.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.064262 refuel-autolabel-0.0.4/src/autolabel/configs/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       65 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/configs/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1515 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/configs/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     5880 2023-06-15 01:06:20.000000 refuel-autolabel-0.0.4/src/autolabel/configs/config.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.065966 refuel-autolabel-0.0.4/src/autolabel/data_models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      195 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2001 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/annotation.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       71 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2036 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1071 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/dataset.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      928 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/task.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2625 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/task_run.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.066545 refuel-autolabel-0.0.4/src/autolabel/database/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       77 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/database/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      410 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.4/src/autolabel/database/engine.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2788 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/database/state_manager.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     6592 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/dataset_loader.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.067208 refuel-autolabel-0.0.4/src/autolabel/few_shot/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2429 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/few_shot/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1295 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/few_shot/fixed_example_selector.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11031 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.4/src/autolabel/few_shot/vector_store.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    19407 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/labeler.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.068816 refuel-autolabel-0.0.4/src/autolabel/models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1965 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2496 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/models/anthropic.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4150 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3037 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/models/hf_pipeline.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4026 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/models/openai.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3599 2023-06-15 01:29:24.000000 refuel-autolabel-0.0.4/src/autolabel/models/palm.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3569 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/models/refuel.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4625 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.4/src/autolabel/schema.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.070229 refuel-autolabel-0.0.4/src/autolabel/tasks/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1160 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3889 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7299 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/classification.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7309 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/entity_matching.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    12517 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/named_entity_recognition.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7398 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/question_answering.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1574 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/utils.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8888 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.4/src/autolabel/utils.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.071054 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11014 2023-06-18 19:49:40.000000 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1571 2023-06-18 19:49:40.000000 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-06-18 19:49:40.000000 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      641 2023-06-18 19:49:40.000000 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/requires.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       10 2023-06-18 19:49:40.000000 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/top_level.txt
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.793369 refuel-autolabel-0.0.5/
+-rw-r--r--   0 nihit      (501) staff       (20)     1066 2023-05-11 06:24:46.000000 refuel-autolabel-0.0.5/LICENSE
+-rw-r--r--   0 nihit      (501) staff       (20)    10926 2023-06-23 23:32:07.793181 refuel-autolabel-0.0.5/PKG-INFO
+-rw-r--r--   0 nihit      (501) staff       (20)     8902 2023-06-23 16:52:52.000000 refuel-autolabel-0.0.5/README.md
+-rw-r--r--   0 nihit      (501) staff       (20)     2134 2023-06-23 23:30:09.000000 refuel-autolabel-0.0.5/pyproject.toml
+-rw-r--r--   0 nihit      (501) staff       (20)       38 2023-06-23 23:32:07.793418 refuel-autolabel-0.0.5/setup.cfg
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.782307 refuel-autolabel-0.0.5/src/
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.784280 refuel-autolabel-0.0.5/src/autolabel/
+-rw-r--r--   0 nihit      (501) staff       (20)       63 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/__init__.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.785045 refuel-autolabel-0.0.5/src/autolabel/cache/
+-rw-r--r--   0 nihit      (501) staff       (20)       74 2023-05-16 00:22:56.000000 refuel-autolabel-0.0.5/src/autolabel/cache/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)      924 2023-06-08 20:27:49.000000 refuel-autolabel-0.0.5/src/autolabel/cache/base.py
+-rw-r--r--   0 nihit      (501) staff       (20)     1817 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/cache/sqlalchemy_cache.py
+-rw-r--r--   0 nihit      (501) staff       (20)     9137 2023-06-15 00:40:46.000000 refuel-autolabel-0.0.5/src/autolabel/confidence.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.785708 refuel-autolabel-0.0.5/src/autolabel/configs/
+-rw-r--r--   0 nihit      (501) staff       (20)       65 2023-05-29 00:22:31.000000 refuel-autolabel-0.0.5/src/autolabel/configs/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)     1515 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/configs/base.py
+-rw-r--r--   0 nihit      (501) staff       (20)     5886 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.5/src/autolabel/configs/config.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.787277 refuel-autolabel-0.0.5/src/autolabel/data_models/
+-rw-r--r--   0 nihit      (501) staff       (20)      195 2023-05-16 00:22:56.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)     2001 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/annotation.py
+-rw-r--r--   0 nihit      (501) staff       (20)       71 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/base.py
+-rw-r--r--   0 nihit      (501) staff       (20)     2036 2023-06-10 22:44:42.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/cache.py
+-rw-r--r--   0 nihit      (501) staff       (20)     1071 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/dataset.py
+-rw-r--r--   0 nihit      (501) staff       (20)      928 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/task.py
+-rw-r--r--   0 nihit      (501) staff       (20)     2625 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/data_models/task_run.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.787851 refuel-autolabel-0.0.5/src/autolabel/database/
+-rw-r--r--   0 nihit      (501) staff       (20)       77 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.5/src/autolabel/database/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)      410 2023-06-10 22:44:42.000000 refuel-autolabel-0.0.5/src/autolabel/database/engine.py
+-rw-r--r--   0 nihit      (501) staff       (20)     2788 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/database/state_manager.py
+-rw-r--r--   0 nihit      (501) staff       (20)     8085 2023-06-23 23:23:54.000000 refuel-autolabel-0.0.5/src/autolabel/dataset_loader.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.788486 refuel-autolabel-0.0.5/src/autolabel/few_shot/
+-rw-r--r--   0 nihit      (501) staff       (20)     2429 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/few_shot/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)     1295 2023-05-14 02:11:15.000000 refuel-autolabel-0.0.5/src/autolabel/few_shot/fixed_example_selector.py
+-rw-r--r--   0 nihit      (501) staff       (20)    11031 2023-06-09 05:14:40.000000 refuel-autolabel-0.0.5/src/autolabel/few_shot/vector_store.py
+-rw-r--r--   0 nihit      (501) staff       (20)    19406 2023-06-23 23:23:54.000000 refuel-autolabel-0.0.5/src/autolabel/labeler.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.790398 refuel-autolabel-0.0.5/src/autolabel/models/
+-rw-r--r--   0 nihit      (501) staff       (20)     1965 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/models/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)     2496 2023-05-29 00:22:31.000000 refuel-autolabel-0.0.5/src/autolabel/models/anthropic.py
+-rw-r--r--   0 nihit      (501) staff       (20)     4150 2023-05-29 00:22:31.000000 refuel-autolabel-0.0.5/src/autolabel/models/base.py
+-rw-r--r--   0 nihit      (501) staff       (20)     3132 2023-06-23 04:22:30.000000 refuel-autolabel-0.0.5/src/autolabel/models/hf_pipeline.py
+-rw-r--r--   0 nihit      (501) staff       (20)     4404 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.5/src/autolabel/models/openai.py
+-rw-r--r--   0 nihit      (501) staff       (20)     3920 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.5/src/autolabel/models/palm.py
+-rw-r--r--   0 nihit      (501) staff       (20)     3575 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.5/src/autolabel/models/refuel.py
+-rw-r--r--   0 nihit      (501) staff       (20)     4625 2023-06-14 21:52:44.000000 refuel-autolabel-0.0.5/src/autolabel/schema.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.791922 refuel-autolabel-0.0.5/src/autolabel/tasks/
+-rw-r--r--   0 nihit      (501) staff       (20)     1160 2023-06-14 01:40:05.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/__init__.py
+-rw-r--r--   0 nihit      (501) staff       (20)     4319 2023-06-20 23:17:06.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/base.py
+-rw-r--r--   0 nihit      (501) staff       (20)     7409 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/classification.py
+-rw-r--r--   0 nihit      (501) staff       (20)     7419 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/entity_matching.py
+-rw-r--r--   0 nihit      (501) staff       (20)    12627 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/named_entity_recognition.py
+-rw-r--r--   0 nihit      (501) staff       (20)     7508 2023-06-19 23:05:19.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/question_answering.py
+-rw-r--r--   0 nihit      (501) staff       (20)     1574 2023-06-08 20:27:49.000000 refuel-autolabel-0.0.5/src/autolabel/tasks/utils.py
+-rw-r--r--   0 nihit      (501) staff       (20)     9773 2023-06-22 21:37:13.000000 refuel-autolabel-0.0.5/src/autolabel/utils.py
+drwxr-xr-x   0 nihit      (501) staff       (20)        0 2023-06-23 23:32:07.792946 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/
+-rw-r--r--   0 nihit      (501) staff       (20)    10926 2023-06-23 23:32:07.000000 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/PKG-INFO
+-rw-r--r--   0 nihit      (501) staff       (20)     1571 2023-06-23 23:32:07.000000 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/SOURCES.txt
+-rw-r--r--   0 nihit      (501) staff       (20)        1 2023-06-23 23:32:07.000000 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/dependency_links.txt
+-rw-r--r--   0 nihit      (501) staff       (20)      782 2023-06-23 23:32:07.000000 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/requires.txt
+-rw-r--r--   0 nihit      (501) staff       (20)       10 2023-06-23 23:32:07.000000 refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/top_level.txt
```

### Comparing `refuel-autolabel-0.0.4/LICENSE` & `refuel-autolabel-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/PKG-INFO` & `refuel-autolabel-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.4
-Summary: Library for LLM powered labeling
+Version: 0.0.5
+Summary: Label, clean and enrich text datasets with LLMs
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,29 +40,25 @@
 Provides-Extra: huggingface
 Provides-Extra: google
 Provides-Extra: all
 License-File: LICENSE
 
 <img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
 
-<p align="center">
-    <b>Clean, labeled data at the speed of thought</b>.
-</p>
 
 <h4 align="center">
-  <a href="https://docs.refuel.ai/guide/overview/getting-started/">Getting started</a> |
   <a href="https://docs.refuel.ai/">Docs</a> |
   <a href="https://discord.gg/fweVnRx6CU">Discord</a> |
   <a href="https://twitter.com/RefuelAI">Twitter</a> |
   <a href="https://www.refuel.ai/">Website</a>
 </h4>
 
 <div align="center" style="width:800px">
 
-[![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [![License: MIT](https://badgen.net/badge/license/MIT/blue)](https://opensource.org/licenses/MIT)
+[![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [![open in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-E?usp=sharing)
 </div>
 
 ## ⚡ Quick Install
 
 `pip install refuel-autolabel`
 
 ## 🏷 What is Autolabel
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.4 Summary: Library
-for LLM powered labeling Author-email: "Refuel.ai"
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.5 Summary: Label,
+clean and enrich text datasets with LLMs Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -19,24 +19,24 @@
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.6 Description-Content-Type: text/
 markdown Provides-Extra: dev Provides-Extra: openai Provides-Extra: anthropic
 Provides-Extra: huggingface Provides-Extra: google Provides-Extra: all License-
 File: LICENSE [Refuel logo]
-                 Clean, labeled data at the speed of thought.
-         *** Getting_started | Docs | Discord | Twitter | Website ***
+                  *** Docs | Discord | Twitter | Website ***
  [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/
      badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/
 black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/
    workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/
       github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://
 img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [!
-      [License: MIT](https://badgen.net/badge/license/MIT/blue)](https://
-                         opensource.org/licenses/MIT)
+  [open in colab](https://colab.research.google.com/assets/colab-badge.svg)]
+   (https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-
+                                E?usp=sharing)
 ## â¡ Quick Install `pip install refuel-autolabel` ## ð· What is Autolabel
 Access to [large, clean and diverse](https://twitter.com/karpathy/status/
 1528443124577513472?lang=en) labeled datasets is a critical component for any
 machine learning effort to be successful. State-of-the-art LLMs like GPT-4 are
 able to [automatically label data](https://arxiv.org/abs/2303.15056) with [high
 accuracy](https://arxiv.org/abs/2303.16854), and at a fraction of the cost and
 time compared to manual labeling. Autolabel is a Python library to label, clean
```

### Comparing `refuel-autolabel-0.0.4/README.md` & `refuel-autolabel-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 <img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
 
-<p align="center">
-    <b>Clean, labeled data at the speed of thought</b>.
-</p>
 
 <h4 align="center">
-  <a href="https://docs.refuel.ai/guide/overview/getting-started/">Getting started</a> |
   <a href="https://docs.refuel.ai/">Docs</a> |
   <a href="https://discord.gg/fweVnRx6CU">Discord</a> |
   <a href="https://twitter.com/RefuelAI">Twitter</a> |
   <a href="https://www.refuel.ai/">Website</a>
 </h4>
 
 <div align="center" style="width:800px">
 
-[![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [![License: MIT](https://badgen.net/badge/license/MIT/blue)](https://opensource.org/licenses/MIT)
+[![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [![open in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-E?usp=sharing)
 </div>
 
 ## ⚡ Quick Install
 
 `pip install refuel-autolabel`
 
 ## 🏷 What is Autolabel
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 [Refuel logo]
-                 Clean, labeled data at the speed of thought.
-         *** Getting_started | Docs | Discord | Twitter | Website ***
+                  *** Docs | Discord | Twitter | Website ***
  [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/
      badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/
 black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/
    workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/
       github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://
 img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [!
-      [License: MIT](https://badgen.net/badge/license/MIT/blue)](https://
-                         opensource.org/licenses/MIT)
+  [open in colab](https://colab.research.google.com/assets/colab-badge.svg)]
+   (https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-
+                                E?usp=sharing)
 ## â¡ Quick Install `pip install refuel-autolabel` ## ð· What is Autolabel
 Access to [large, clean and diverse](https://twitter.com/karpathy/status/
 1528443124577513472?lang=en) labeled datasets is a critical component for any
 machine learning effort to be successful. State-of-the-art LLMs like GPT-4 are
 able to [automatically label data](https://arxiv.org/abs/2303.15056) with [high
 accuracy](https://arxiv.org/abs/2303.16854), and at a fraction of the cost and
 time compared to manual labeling. Autolabel is a Python library to label, clean
```

### Comparing `refuel-autolabel-0.0.4/pyproject.toml` & `refuel-autolabel-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=65.0.0", "wheel >= 0.38"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "refuel-autolabel"
-version = "0.0.4"
-description = "Library for LLM powered labeling"
+version = "0.0.5"
+description = "Label, clean and enrich text datasets with LLMs"
 readme = "README.md"
 authors = [{ name = "Refuel.ai", email = "support@refuel.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -18,15 +18,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "loguru >= 0.5.0",
     "numpy >= 1.23.0",
     "requests >= 2.27.0",
     "datasets >= 2.7.0",
-    "langchain >= 0.0.190",
+    "langchain == 0.0.210",
     "nervaluate >= 0.1.8",
     "pandas >= 1.3.0",
     "scikit-learn >= 1.0.0",
     "tenacity >= 8.2.2",
     "SQLAlchemy == 1.4.47",
     "regex >= 2023.6.3",
     "rich >= 13.3.5",
@@ -38,14 +38,22 @@
 ]
 requires-python = ">=3.6"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "bumpver",
+    "mkdocs",
+    "mkdocs-autorefs",
+    "mkdocs-jupyter",
+    "mkdocs-material",
+    "mkdocs-material-extensions",
+    "mkdocs-table-reader-plugin",
+    "mkdocstrings",
+    "mkdocstrings-python",
     "pip-tools",
     "pytest",
     "pytest-mock",
     "pre-commit"
 ]
 openai = [
     "openai >= 0.27.4",
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/cache/base.py` & `refuel-autolabel-0.0.5/src/autolabel/cache/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/cache/sqlalchemy_cache.py` & `refuel-autolabel-0.0.5/src/autolabel/cache/sqlalchemy_cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/confidence.py` & `refuel-autolabel-0.0.5/src/autolabel/confidence.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/configs/base.py` & `refuel-autolabel-0.0.5/src/autolabel/configs/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/configs/config.py` & `refuel-autolabel-0.0.5/src/autolabel/configs/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         """Returns true if the model is able to return a confidence score along with its predictions"""
         return self._model_config.get(self.COMPUTE_CONFIDENCE_KEY, False)
 
     # Prompt config
     def task_guidelines(self) -> str:
         return self._prompt_config.get(self.TASK_GUIDELINE_KEY, "")
 
-    def labels_list(self) -> str:
+    def labels_list(self) -> List[str]:
         """Returns a list of valid labels"""
         return self._prompt_config.get(self.VALID_LABELS_KEY, [])
 
     def few_shot_example_set(self) -> Union[str, List]:
         """Returns examples of how data should be labeled, used to guide context to the model about the task it is performing"""
         return self._prompt_config.get(self.FEW_SHOT_EXAMPLE_SET_KEY, [])
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/data_models/annotation.py` & `refuel-autolabel-0.0.5/src/autolabel/data_models/annotation.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/data_models/cache.py` & `refuel-autolabel-0.0.5/src/autolabel/data_models/cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/data_models/dataset.py` & `refuel-autolabel-0.0.5/src/autolabel/data_models/dataset.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/data_models/task.py` & `refuel-autolabel-0.0.5/src/autolabel/data_models/task.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/data_models/task_run.py` & `refuel-autolabel-0.0.5/src/autolabel/data_models/task_run.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/database/state_manager.py` & `refuel-autolabel-0.0.5/src/autolabel/database/state_manager.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/few_shot/__init__.py` & `refuel-autolabel-0.0.5/src/autolabel/few_shot/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/few_shot/fixed_example_selector.py` & `refuel-autolabel-0.0.5/src/autolabel/few_shot/fixed_example_selector.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/few_shot/vector_store.py` & `refuel-autolabel-0.0.5/src/autolabel/few_shot/vector_store.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/labeler.py` & `refuel-autolabel-0.0.5/src/autolabel/labeler.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,80 +62,81 @@
 
         Args:
             dataset: path to CSV dataset to be annotated
             max_items: maximum items in dataset to be annotated
             output_name: custom name of output CSV file
             start_index: skips annotating [0, start_index)
         """
+        dataset_loader = DatasetLoader(dataset, self.config, max_items, start_index)
 
         self.db.initialize()
         self.dataset = self.db.initialize_dataset(
-            dataset, self.config, start_index, max_items
+            dataset_loader.dat, self.config, start_index, max_items
         )
         self.task_object = self.db.initialize_task(self.config)
-        csv_file_name = (
-            output_name if output_name else f"{dataset.replace('.csv','')}_labeled.csv"
-        )
         if isinstance(dataset, str):
-            df, inputs, gt_labels = DatasetLoader.read_file(
-                dataset, self.config, max_items, start_index
-            )
-        elif isinstance(dataset, pd.DataFrame):
-            df, inputs, gt_labels = DatasetLoader.read_dataframe(
-                dataset, self.config, max_items, start_index
+            csv_file_name = (
+                output_name
+                if output_name
+                else f"{dataset.replace('.csv','')}_labeled.csv"
             )
+        else:
+            csv_file_name = f"{self.config.task_name()}_labeled.csv"
 
         # Initialize task run and check if it already exists
         self.task_run = self.db.get_task_run(self.task_object.id, self.dataset.id)
         # Resume/Delete the task if it already exists or create a new task run
         if self.task_run:
             logger.info("Task run already exists.")
             self.task_run = self.handle_existing_task_run(
-                self.task_run, csv_file_name, gt_labels=gt_labels
+                self.task_run, csv_file_name, gt_labels=dataset_loader.gt_labels
             )
         else:
             self.task_run = self.db.create_task_run(
                 csv_file_name, self.task_object.id, self.dataset.id
             )
 
         # Get the seed examples from the dataset config
         seed_examples = self.config.few_shot_example_set()
 
         # If this dataset config is a string, read the corrresponding csv file
         if isinstance(seed_examples, str):
-            _, seed_examples, _ = DatasetLoader.read_csv(seed_examples, self.config)
+            seed_loader = DatasetLoader(seed_examples, self.config)
+            seed_examples = seed_loader.inputs
 
         # Check explanations are present in data if explanation_column is passed in
         if (
             self.config.explanation_column()
             and len(seed_examples) > 0
             and self.config.explanation_column() not in list(seed_examples[0].keys())
         ):
             raise ValueError(
                 f"Explanation column {self.config.explanation_column()} not found in dataset.\nMake sure that explanations were generated using labeler.generate_explanations(seed_file)."
             )
 
         self.example_selector = ExampleSelectorFactory.initialize_selector(
-            self.config, seed_examples, df.keys().tolist()
+            self.config, seed_examples, dataset_loader.dat.keys().tolist()
         )
 
         num_failures = 0
         current_index = self.task_run.current_index
         cost = 0.0
         postfix_dict = {}
 
-        indices = range(current_index, len(inputs), self.CHUNK_SIZE)
+        indices = range(current_index, len(dataset_loader.inputs), self.CHUNK_SIZE)
         for current_index in track_with_stats(
             indices,
             postfix_dict,
-            total=len(inputs) - current_index,
+            total=len(dataset_loader.inputs) - current_index,
             advance=self.CHUNK_SIZE,
             console=console,
         ):
-            chunk = inputs[current_index : current_index + self.CHUNK_SIZE]
+            chunk = dataset_loader.inputs[
+                current_index : current_index + self.CHUNK_SIZE
+            ]
             final_prompts = []
             for i, input_i in enumerate(chunk):
                 # Fetch few-shot seed examples
                 if self.example_selector:
                     examples = self.example_selector.select_examples(input_i)
                 else:
                     examples = []
@@ -202,17 +203,17 @@
 
             # Evaluate the task every eval_every examples
             if (current_index + self.CHUNK_SIZE) % eval_every == 0:
                 db_result = AnnotationModel.get_annotations_by_task_run_id(
                     self.db.session, self.task_run.id
                 )
                 llm_labels = [LLMAnnotation(**a.llm_annotation) for a in db_result]
-                if gt_labels:
+                if dataset_loader.gt_labels:
                     eval_result = self.task.eval(
-                        llm_labels, gt_labels[: len(llm_labels)]
+                        llm_labels, dataset_loader.gt_labels[: len(llm_labels)]
                     )
 
                     for m in eval_result:
                         if not isinstance(m.value, list) or len(m.value) < 1:
                             continue
                         elif isinstance(m.value[0], float):
                             postfix_dict[m.name] = f"{m.value[0]:.4f}"
@@ -228,28 +229,30 @@
 
         db_result = AnnotationModel.get_annotations_by_task_run_id(
             self.db.session, self.task_run.id
         )
         llm_labels = [LLMAnnotation(**a.llm_annotation) for a in db_result]
         eval_result = None
         # if true labels are provided, evaluate accuracy of predictions
-        if gt_labels:
-            eval_result = self.task.eval(llm_labels, gt_labels[: len(llm_labels)])
+        if dataset_loader.gt_labels:
+            eval_result = self.task.eval(
+                llm_labels, dataset_loader.gt_labels[: len(llm_labels)]
+            )
             table = {}
             # TODO: serialize and write to file
             for m in eval_result:
                 if isinstance(m.value, list) and len(m.value) > 0:
                     table[m.name] = m.value
                 else:
                     print(f"Metric: {m.name}: {maybe_round(m.value)}")
             print(f"Actual Cost: {maybe_round(cost)}")
             print_table(table, console=console, default_style=METRIC_TABLE_STYLE)
 
         # Write output to CSV
-        output_df = df.copy()
+        output_df = dataset_loader.dat.copy()
         output_df[self.config.task_name() + "_llm_labeled_successfully"] = [
             l.successfully_labeled for l in llm_labels
         ]
         output_df[self.config.task_name() + "_llm_label"] = [
             l.label for l in llm_labels
         ]
         if self.config.confidence():
@@ -294,50 +297,44 @@
     ) -> None:
         """Calculates and prints the cost of calling autolabel.run() on a given dataset
 
         Args:
             dataset: path to a CSV dataset
         """
 
-        if isinstance(dataset, str):
-            df, inputs, _ = DatasetLoader.read_file(
-                dataset, self.config, max_items, start_index
-            )
-        elif isinstance(dataset, pd.DataFrame):
-            df, inputs, _ = DatasetLoader.read_dataframe(
-                dataset, self.config, max_items, start_index
-            )
+        dataset_loader = DatasetLoader(dataset, self.config, max_items, start_index)
 
         prompt_list = []
         total_cost = 0
 
         # Get the seed examples from the dataset config
         seed_examples = self.config.few_shot_example_set()
 
         # If this dataset config is a string, read the corrresponding csv file
         if isinstance(seed_examples, str):
-            _, seed_examples, _ = DatasetLoader.read_file(seed_examples, self.config)
+            seed_loader = DatasetLoader(seed_examples, self.config)
+            seed_examples = seed_loader.inputs
 
         # Check explanations are present in data if explanation_column is passed in
         if (
             self.config.explanation_column()
             and len(seed_examples) > 0
             and self.config.explanation_column() not in list(seed_examples[0].keys())
         ):
             raise ValueError(
                 f"Explanation column {self.config.explanation_column()} not found in dataset.\nMake sure that explanations were generated using labeler.generate_explanations(seed_file)."
             )
 
         self.example_selector = ExampleSelectorFactory.initialize_selector(
-            self.config, seed_examples, df.keys().tolist()
+            self.config, seed_examples, dataset_loader.dat.keys().tolist()
         )
 
-        input_limit = min(len(inputs), 100)
+        input_limit = min(len(dataset_loader.inputs), 100)
         for input_i in track(
-            inputs[:input_limit],
+            dataset_loader.inputs[:input_limit],
             description="Generating Prompts...",
             console=console,
         ):
             # TODO: Check if this needs to use the example selector
             if self.example_selector:
                 examples = self.example_selector.select_examples(input_i)
             else:
@@ -345,19 +342,19 @@
             final_prompt = self.task.construct_prompt(input_i, examples)
             prompt_list.append(final_prompt)
 
             # Calculate the number of tokens
             curr_cost = self.llm.get_cost(prompt=final_prompt, label="")
             total_cost += curr_cost
 
-        total_cost = total_cost * (len(inputs) / input_limit)
+        total_cost = total_cost * (len(dataset_loader.inputs) / input_limit)
         table = {
             "Total Estimated Cost": f"${maybe_round(total_cost)}",
-            "Number of Examples": len(inputs),
-            "Average cost per example": f"${maybe_round(total_cost / len(inputs))}",
+            "Number of Examples": len(dataset_loader.inputs),
+            "Average cost per example": f"${maybe_round(total_cost / len(dataset_loader.inputs))}",
         }
         table = {"parameter": list(table.keys()), "value": list(table.values())}
         print_table(table, show_header=False, console=console, styles=COST_TABLE_STYLES)
 
         console.rule("Prompt Example")
         print(f"{prompt_list[0]}")
         console.rule()
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/models/__init__.py` & `refuel-autolabel-0.0.5/src/autolabel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/models/anthropic.py` & `refuel-autolabel-0.0.5/src/autolabel/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/models/base.py` & `refuel-autolabel-0.0.5/src/autolabel/models/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/models/hf_pipeline.py` & `refuel-autolabel-0.0.5/src/autolabel/models/hf_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from autolabel.models import BaseModel
 from autolabel.configs import AutolabelConfig
 from autolabel.cache import BaseCache
 
 
 class HFPipelineLLM(BaseModel):
     DEFAULT_MODEL = "google/flan-t5-xxl"
-    DEFAULT_PARAMS = {"max_new_tokens": 1000, "temperature": 0.0, "quantize": 8}
+    DEFAULT_PARAMS = {"temperature": 0.0, "quantize": 8}
 
     def __init__(self, config: AutolabelConfig, cache: BaseCache = None) -> None:
         try:
             from transformers import AutoModelForSeq2SeqLM, AutoTokenizer, pipeline
         except ImportError:
             raise ValueError(
                 "Could not import transformers python package. "
@@ -34,15 +34,17 @@
         # populate model params
         model_params = config.model_params()
         self.model_params = {**self.DEFAULT_PARAMS, **model_params}
 
         # initialize HF pipeline
         tokenizer = AutoTokenizer.from_pretrained(self.model_name)
         quantize_bits = self.model_params["quantize"]
-        if quantize_bits == 8:
+        if not torch.cuda.is_available():
+            model = AutoModelForSeq2SeqLM.from_pretrained(self.model_name)
+        elif quantize_bits == 8:
             model = AutoModelForSeq2SeqLM.from_pretrained(
                 self.model_name, load_in_8bit=True, device_map="auto"
             )
         elif quantize_bits == "16":
             model = AutoModelForSeq2SeqLM.from_pretrained(
                 self.model_name, torch_dtype=torch.float16, device_map="auto"
             )
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/models/openai.py` & `refuel-autolabel-0.0.5/src/autolabel/models/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 
 
 class OpenAILLM(BaseModel):
     CHAT_ENGINE_MODELS = [
         "gpt-3.5-turbo",
         "gpt-3.5-turbo-0613",
         "gpt-3.5-turbo-16k",
+        "gpt-3.5-turbo-16k-0613",
         "gpt-4",
+        "gpt-4-0613",
+        "gpt-4-32k",
+        "gpt-4-32k-0613",
     ]
     MODELS_WITH_TOKEN_PROBS = ["text-curie-001", "text-davinci-003"]
 
     # Default parameters for OpenAILLM
     DEFAULT_MODEL = "gpt-3.5-turbo"
     DEFAULT_PARAMS_COMPLETION_ENGINE = {
         "max_tokens": 1000,
@@ -35,23 +39,31 @@
     # Reference: https://openai.com/pricing
     COST_PER_PROMPT_TOKEN = {
         "text-davinci-003": 0.02 / 1000,
         "text-curie-001": 0.002 / 1000,
         "gpt-3.5-turbo": 0.0015 / 1000,
         "gpt-3.5-turbo-0613": 0.0015 / 1000,
         "gpt-3.5-turbo-16k": 0.003 / 1000,
+        "gpt-3.5-turbo-16k-0613": 0.003 / 1000,
         "gpt-4": 0.03 / 1000,
+        "gpt-4-0613": 0.03 / 1000,
+        "gpt-4-32k": 0.06 / 1000,
+        "gpt-4-32k-0613": 0.06 / 1000,
     }
     COST_PER_COMPLETION_TOKEN = {
         "text-davinci-003": 0.02 / 1000,
         "text-curie-001": 0.002 / 1000,
         "gpt-3.5-turbo": 0.002 / 1000,
         "gpt-3.5-turbo-0613": 0.002 / 1000,
         "gpt-3.5-turbo-16k": 0.004 / 1000,
-        "gpt-4": 0.06 / 1000,  # $0.06 per 1000 tokens in response
+        "gpt-3.5-turbo-16k-0613": 0.004 / 1000,
+        "gpt-4": 0.06 / 1000,
+        "gpt-4-0613": 0.06 / 1000,
+        "gpt-4-32k": 0.12 / 1000,
+        "gpt-4-32k-0613": 0.12 / 1000,
     }
 
     @cached_property
     def _engine(self) -> str:
         if self.model_name is not None and self.model_name in self.CHAT_ENGINE_MODELS:
             return "chat"
         else:
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/models/palm.py` & `refuel-autolabel-0.0.5/src/autolabel/models/palm.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,27 @@
 from langchain.llms import VertexAI
 from langchain.schema import LLMResult, HumanMessage, Generation
 
 from autolabel.models import BaseModel
 from autolabel.configs import AutolabelConfig
 from autolabel.cache import BaseCache
 
+from tenacity import (
+    before_sleep_log,
+    retry,
+    stop_after_attempt,
+    wait_exponential,
+)
+
 logger = logging.getLogger(__name__)
 
 
 class PaLMLLM(BaseModel):
     SEP_REPLACEMENT_TOKEN = "@@"
     CHAT_ENGINE_MODELS = ["chat-bison@001"]
-    NUM_TRIES = 5
 
     DEFAULT_MODEL = "text-bison@001"
     DEFAULT_PARAMS = {"temperature": 0}
 
     # Reference: https://cloud.google.com/vertex-ai/pricing
     COST_PER_CHARACTER = {
         "text-bison@001": 0.001 / 1000,
@@ -47,14 +53,23 @@
             **model_params,
         }
         if self._engine == "chat":
             self.llm = ChatVertexAI(model_name=self.model_name, **self.model_params)
         else:
             self.llm = VertexAI(model_name=self.model_name, **self.model_params)
 
+    @retry(
+        reraise=True,
+        stop=stop_after_attempt(5),
+        wait=wait_exponential(multiplier=1, min=2, max=10),
+        before_sleep=before_sleep_log(logger, logging.WARNING),
+    )
+    def _label_with_retry(self, prompts: List[str]) -> LLMResult:
+        return self.llm.generate(prompts)
+
     def _label(self, prompts: List[str]) -> LLMResult:
         for prompt in prompts:
             if self.SEP_REPLACEMENT_TOKEN in prompt:
                 logger.warning(
                     f"""Current prompt contains {self.SEP_REPLACEMENT_TOKEN} 
                                 which is currently used as a separator token by refuel
                                 llm. It is highly recommended to avoid having any
@@ -66,25 +81,24 @@
         ]
         if self._engine == "chat":
             # Need to convert list[prompts] -> list[messages]
             # Currently the entire prompt is stuck into the "human message"
             # We might consider breaking this up into human vs system message in future
             prompts = [[HumanMessage(content=prompt)] for prompt in prompts]
 
-        for _ in range(self.NUM_TRIES):
-            try:
-                result = self.llm.generate(prompts)
-                for generations in result.generations:
-                    for generation in generations:
-                        generation.text = generation.text.replace(
-                            self.SEP_REPLACEMENT_TOKEN, "\n"
-                        )
-                return result
-            except Exception as e:
-                logger.error(f"Error generating from LLM: {e}.")
+        try:
+            result = self._label_with_retry(prompts)
+            for generations in result.generations:
+                for generation in generations:
+                    generation.text = generation.text.replace(
+                        self.SEP_REPLACEMENT_TOKEN, "\n"
+                    )
+            return result
+        except Exception as e:
+            logger.error(f"Error generating from LLM: {e}.")
         generations = [[Generation(text="")] for _ in prompts]
         return LLMResult(generations=generations)
 
     def get_cost(self, prompt: str, label: Optional[str] = "") -> float:
         if self.model_name is None:
             return 0.0
         cost_per_char = self.COST_PER_CHARACTER.get(self.model_name, 0.0)
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/models/refuel.py` & `refuel-autolabel-0.0.5/src/autolabel/models/refuel.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 f" `{self.REFUEL_API_ENV}` which contains it"
             )
 
     @retry(
         reraise=True,
         stop=stop_after_attempt(5),
         wait=wait_exponential(multiplier=1, min=2, max=10),
-        before_sleep=before_sleep_log(logger, "WARNING"),
+        before_sleep=before_sleep_log(logger, logging.WARNING),
     )
     def _label_with_retry(self, prompt: str) -> requests.Response:
         payload = {
             "data": {"model_input": prompt, "model_params": {**self.model_params}},
             "task": "generate",
         }
         headers = {"refuel_api_key": self.REFUEL_API_KEY}
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/schema.py` & `refuel-autolabel-0.0.5/src/autolabel/schema.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/tasks/__init__.py` & `refuel-autolabel-0.0.5/src/autolabel/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/tasks/base.py` & `refuel-autolabel-0.0.5/src/autolabel/tasks/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict, List
 import logging
 import json
 
 from langchain.prompts.prompt import PromptTemplate
 from langchain.schema import Generation
 from autolabel.configs import AutolabelConfig
-from autolabel.schema import LLMAnnotation, MetricResult, FewShotAlgorithm
+from autolabel.schema import LLMAnnotation, MetricResult, FewShotAlgorithm, TaskType
 from autolabel.utils import get_format_variables, extract_valid_json_substring
 
 logger = logging.getLogger(__name__)
 
 
 class BaseTask(ABC):
     ZERO_SHOT_TEMPLATE = "{task_guidelines}\n\n{output_guidelines}\n\nNow I want you to label the following example:\n{current_example}"
@@ -82,16 +82,26 @@
             llm_label = self.NULL_LABEL_TOKEN
             logger.warning(f"LLM response is empty")
         elif not completion_text:
             successfully_labeled = False
             llm_label = self.NULL_LABEL_TOKEN
             logger.error(f"Error parsing LLM response: {response.text}")
         else:
-            successfully_labeled = True
             llm_label = completion_text.strip()
+            if self.config.task_type() in [
+                TaskType.CLASSIFICATION,
+                TaskType.ENTITY_MATCHING,
+            ]:
+                if llm_label in self.config.labels_list():
+                    successfully_labeled = True
+                else:
+                    logger.warning(f"LLM response is not in the labels list")
+                    successfully_labeled = False
+            else:
+                successfully_labeled = True
 
         return LLMAnnotation(
             successfully_labeled=successfully_labeled,
             label=llm_label,
             generation_info=response.generation_info,
             raw_response=response.text,
             prompt=prompt,
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/tasks/classification.py` & `refuel-autolabel-0.0.5/src/autolabel/tasks/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,34 +127,36 @@
 
         Returns:
             List[MetricResult]: list of metrics and corresponding values
         """
 
         eval_metrics_map = {
             Metric.SUPPORT: [],
-            Metric.THRESHOLD: [],
             Metric.ACCURACY: [],
             Metric.COMPLETION_RATE: [],
         }
         eval_metrics = []
-        thresholds = [float("-inf")]
+        thresholds = []
 
         if self.config.confidence():
+            eval_metrics_map[Metric.THRESHOLD] = []
             labels, confidences = self.auroc_score_labels(gt_labels, llm_labels)
             value, meaningful_thresholds = ConfidenceCalculator.compute_auroc(
                 labels, confidences
             )
             thresholds.extend(meaningful_thresholds)
             eval_metrics.append(
                 MetricResult(
                     metric_type=Metric.AUROC,
                     name="auroc",
                     value=value,
                 )
             )
+        else:
+            thresholds.append(float("-inf"))
 
         for index, threshold in enumerate(thresholds):
             (
                 curr_gt_labels,
                 curr_llm_labels,
             ) = self.get_labels_predictions_with_threshold(
                 gt_labels, llm_labels, threshold
@@ -167,15 +169,17 @@
             eval_metrics_map[Metric.SUPPORT].append(len(curr_gt_labels))
             if len(curr_gt_labels) > 0:
                 eval_metrics_map[Metric.ACCURACY].append(
                     accuracy_score(curr_gt_labels, curr_llm_labels)
                 )
             else:
                 eval_metrics_map[Metric.ACCURACY].append(0.0)
-            eval_metrics_map[Metric.THRESHOLD].append(threshold)
+
+            if self.config.confidence():
+                eval_metrics_map[Metric.THRESHOLD].append(threshold)
 
         eval_metrics.extend(
             [
                 MetricResult(
                     metric_type=i,
                     name=i.value,
                     value=eval_metrics_map[i],
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/tasks/entity_matching.py` & `refuel-autolabel-0.0.5/src/autolabel/tasks/entity_matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,34 +126,36 @@
 
         Returns:
             List[MetricResult]: list of metrics and corresponding values
         """
 
         eval_metrics_map = {
             Metric.SUPPORT: [],
-            Metric.THRESHOLD: [],
             Metric.ACCURACY: [],
             Metric.COMPLETION_RATE: [],
         }
         eval_metrics = []
-        thresholds = [float("-inf")]
+        thresholds = []
 
         if self.config.confidence():
+            eval_metrics_map[Metric.THRESHOLD] = []
             labels, confidences = self.auroc_score_labels(gt_labels, llm_labels)
             value, meaningful_thresholds = ConfidenceCalculator.compute_auroc(
                 labels, confidences
             )
             thresholds.extend(meaningful_thresholds)
             eval_metrics.append(
                 MetricResult(
                     metric_type=Metric.AUROC,
                     name="auroc",
                     value=value,
                 )
             )
+        else:
+            thresholds.append(float("-inf"))
 
         for index, threshold in enumerate(thresholds):
             (
                 curr_gt_labels,
                 curr_llm_labels,
             ) = self.get_labels_predictions_with_threshold(
                 gt_labels, llm_labels, threshold
@@ -165,15 +167,17 @@
             eval_metrics_map[Metric.SUPPORT].append(len(curr_gt_labels))
             if len(curr_gt_labels) > 0:
                 eval_metrics_map[Metric.ACCURACY].append(
                     accuracy_score(curr_gt_labels, curr_llm_labels)
                 )
             else:
                 eval_metrics_map[Metric.ACCURACY].append(0.0)
-            eval_metrics_map[Metric.THRESHOLD].append(threshold)
+
+            if self.config.confidence():
+                eval_metrics_map[Metric.THRESHOLD].append(threshold)
 
         eval_metrics.extend(
             [
                 MetricResult(
                     metric_type=i,
                     name=i.value,
                     value=eval_metrics_map[i],
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/tasks/named_entity_recognition.py` & `refuel-autolabel-0.0.5/src/autolabel/tasks/named_entity_recognition.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,22 +266,22 @@
             )
             for index in range(len(gt_labels))
         ]
 
         eval_metrics_map = {
             Metric.F1: [],
             Metric.SUPPORT: [],
-            Metric.THRESHOLD: [],
             Metric.ACCURACY: [],
             Metric.COMPLETION_RATE: [],
         }
         eval_metrics = []
-        thresholds = [float("-inf")]
+        thresholds = []
 
         if self.config.confidence():
+            eval_metrics_map[Metric.THRESHOLD] = []
             all_gt_labels, all_llm_preds = self.get_labels_predictions_with_threshold(
                 gt_labels, llm_labels, float("-inf")
             )
             labels, confidences = self.auroc_score_labels(all_gt_labels, all_llm_preds)
             value, meaningful_thresholds = ConfidenceCalculator.compute_auroc(
                 labels, confidences
             )
@@ -289,14 +289,16 @@
             eval_metrics.append(
                 MetricResult(
                     metric_type=Metric.AUROC,
                     name="auroc",
                     value=value,
                 )
             )
+        else:
+            thresholds.append(float("-inf"))
 
         for index, threshold in enumerate(thresholds):
             (
                 curr_gt_labels,
                 curr_llm_labels,
             ) = self.get_labels_predictions_with_threshold(
                 gt_labels, llm_labels, threshold
@@ -320,15 +322,17 @@
 
             for metric in curr_threshold_metrics:
                 eval_metrics_map[metric.metric_type].append(metric.value)
 
             eval_metrics_map[Metric.COMPLETION_RATE].append(
                 len(curr_llm_labels) / float(len(gt_labels))
             )
-            eval_metrics_map[Metric.THRESHOLD].append(threshold)
+
+            if self.config.confidence():
+                eval_metrics_map[Metric.THRESHOLD].append(threshold)
         eval_metrics.extend(
             [
                 MetricResult(
                     metric_type=i,
                     name=i.value,
                     value=eval_metrics_map[i],
                 )
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/tasks/question_answering.py` & `refuel-autolabel-0.0.5/src/autolabel/tasks/question_answering.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,34 +116,36 @@
         Returns:
             List[MetricResult]: list of metrics and corresponding values
         """
 
         eval_metrics_map = {
             Metric.F1: [],
             Metric.SUPPORT: [],
-            Metric.THRESHOLD: [],
             Metric.ACCURACY: [],
             Metric.COMPLETION_RATE: [],
         }
         eval_metrics = []
-        thresholds = [float("-inf")]
+        thresholds = []
 
         if self.config.confidence():
+            eval_metrics_map[Metric.THRESHOLD] = []
             labels, confidences = self.auroc_score_labels(gt_labels, llm_labels)
             value, meaningful_thresholds = ConfidenceCalculator.compute_auroc(
                 labels, confidences
             )
             thresholds.extend(meaningful_thresholds)
             eval_metrics.append(
                 MetricResult(
                     metric_type=Metric.AUROC,
                     name="auroc",
                     value=value,
                 )
             )
+        else:
+            thresholds.append(float("-inf"))
 
         for index, threshold in enumerate(thresholds):
             (
                 curr_gt_labels,
                 curr_llm_labels,
             ) = self.get_labels_predictions_with_threshold(
                 gt_labels, llm_labels, threshold
@@ -156,15 +158,17 @@
             eval_metrics_map[Metric.SUPPORT].append(len(curr_gt_labels))
             if len(curr_gt_labels) > 0:
                 eval_metrics_map[Metric.ACCURACY].append(
                     accuracy_score(curr_gt_labels, curr_llm_labels)
                 )
             else:
                 eval_metrics_map[Metric.ACCURACY].append(0.0)
-            eval_metrics_map[Metric.THRESHOLD].append(threshold)
+
+            if self.config.confidence():
+                eval_metrics_map[Metric.THRESHOLD].append(threshold)
 
             f1 = sum(
                 [
                     compute_f1(curr_llm_labels[index], curr_gt_labels[index])
                     for index in range(len(curr_llm_labels))
                 ]
             )
```

### Comparing `refuel-autolabel-0.0.4/src/autolabel/tasks/utils.py` & `refuel-autolabel-0.0.5/src/autolabel/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/autolabel/utils.py` & `refuel-autolabel-0.0.5/src/autolabel/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import hashlib
+import os
 import json
 import logging
 from string import Formatter
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Union
+import shutil
 
 import regex
 import wget
 from rich.console import Console, Group
 from rich.live import Live
 from rich.progress import (
     BarColumn,
@@ -246,25 +248,48 @@
         table.add_column(key, style=styles.get(key, default_style))
     for i, row in enumerate(zip(*data.values())):
         table.add_row(*row)
     console = console or Console()
     console.print(table)
 
 
-def get_data(dataset_name: str):
+def get_data(dataset_name: str, force: bool = False):
+    """Download Datasets
+
+    Args:
+        dataset_name (str): dataset name
+        force (bool, optional): if set to True, downloads and overwrites the local test and seed files
+            if false then downloads onlyif the files are not present locally
+    """
+
+    def download_bar(current, total, width=80):
+        """custom progress bar for downloading data"""
+        width = shutil.get_terminal_size()[0] // 2
+        print(
+            f"{current//total*100}% [{'.' * (current//total * int(width))}] [{current}/{total}] bytes",
+            end="\r",
+        )
+
+    def download(url: str) -> None:
+        """Downloads the data given an url"""
+        file_name = os.path.basename(url)
+        if force and os.path.exists(file_name):
+            print(f"File {file_name} exists. Removing")
+            os.remove(file_name)
+
+        if not os.path.exists(file_name):
+            print(f"Downloading example dataset from {url} to {file_name}...")
+            wget.download(url, bar=download_bar)
+
     if dataset_name not in EXAMPLE_DATASETS:
         logger.error(
             f"{dataset_name} not in list of available datasets: {str(EXAMPLE_DATASETS)}. Exiting..."
         )
         return
     seed_url = DATASET_URL.format(dataset=dataset_name, partition="seed")
     test_url = DATASET_URL.format(dataset=dataset_name, partition="test")
-
     try:
         if dataset_name not in NO_SEED_DATASET:
-            print('Downloading seed example dataset to "seed.csv"...')
-            wget.download(seed_url)
-            print("\n")
-        print('Downloading test dataset to "test.csv"...')
-        wget.download(test_url)
+            download(seed_url)
+        download(test_url)
     except Exception as e:
         logger.error(f"Error downloading dataset: {e}")
```

### Comparing `refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/PKG-INFO` & `refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.4
-Summary: Library for LLM powered labeling
+Version: 0.0.5
+Summary: Label, clean and enrich text datasets with LLMs
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,29 +40,25 @@
 Provides-Extra: huggingface
 Provides-Extra: google
 Provides-Extra: all
 License-File: LICENSE
 
 <img alt="Refuel logo" src="https://raw.githubusercontent.com/refuel-ai/autolabel/main/docs/assets/Autolabel_blk_w_background.png">
 
-<p align="center">
-    <b>Clean, labeled data at the speed of thought</b>.
-</p>
 
 <h4 align="center">
-  <a href="https://docs.refuel.ai/guide/overview/getting-started/">Getting started</a> |
   <a href="https://docs.refuel.ai/">Docs</a> |
   <a href="https://discord.gg/fweVnRx6CU">Discord</a> |
   <a href="https://twitter.com/RefuelAI">Twitter</a> |
   <a href="https://www.refuel.ai/">Website</a>
 </h4>
 
 <div align="center" style="width:800px">
 
-[![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [![License: MIT](https://badgen.net/badge/license/MIT/blue)](https://opensource.org/licenses/MIT)
+[![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [![open in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-E?usp=sharing)
 </div>
 
 ## ⚡ Quick Install
 
 `pip install refuel-autolabel`
 
 ## 🏷 What is Autolabel
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.4 Summary: Library
-for LLM powered labeling Author-email: "Refuel.ai"
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.5 Summary: Label,
+clean and enrich text datasets with LLMs Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -19,24 +19,24 @@
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.6 Description-Content-Type: text/
 markdown Provides-Extra: dev Provides-Extra: openai Provides-Extra: anthropic
 Provides-Extra: huggingface Provides-Extra: google Provides-Extra: all License-
 File: LICENSE [Refuel logo]
-                 Clean, labeled data at the speed of thought.
-         *** Getting_started | Docs | Discord | Twitter | Website ***
+                  *** Docs | Discord | Twitter | Website ***
  [![lint](https://github.com/refuel-ai/autolabel/actions/workflows/black.yaml/
      badge.svg)](https://github.com/refuel-ai/autolabel/actions/workflows/
 black.yaml/badge.svg) ![Tests](https://github.com/refuel-ai/autolabel/actions/
    workflows/test.yaml/badge.svg) ![Commit Activity](https://img.shields.io/
       github/commit-activity/m/refuel-ai/autolabel) [![Discord](https://
 img.shields.io/discord/1098746693152931901)](https://discord.gg/fweVnRx6CU) [!
-      [License: MIT](https://badgen.net/badge/license/MIT/blue)](https://
-                         opensource.org/licenses/MIT)
+  [open in colab](https://colab.research.google.com/assets/colab-badge.svg)]
+   (https://colab.research.google.com/drive/1t-9vNLkyoyySAG_0w3eR98biBOXlMO-
+                                E?usp=sharing)
 ## â¡ Quick Install `pip install refuel-autolabel` ## ð· What is Autolabel
 Access to [large, clean and diverse](https://twitter.com/karpathy/status/
 1528443124577513472?lang=en) labeled datasets is a critical component for any
 machine learning effort to be successful. State-of-the-art LLMs like GPT-4 are
 able to [automatically label data](https://arxiv.org/abs/2303.15056) with [high
 accuracy](https://arxiv.org/abs/2303.16854), and at a fraction of the cost and
 time compared to manual labeling. Autolabel is a Python library to label, clean
```

### Comparing `refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/SOURCES.txt` & `refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/requires.txt` & `refuel-autolabel-0.0.5/src/refuel_autolabel.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 loguru>=0.5.0
 numpy>=1.23.0
 requests>=2.27.0
 datasets>=2.7.0
-langchain>=0.0.190
+langchain==0.0.210
 nervaluate>=0.1.8
 pandas>=1.3.0
 scikit-learn>=1.0.0
 tenacity>=8.2.2
 SQLAlchemy==1.4.47
 regex>=2023.6.3
 rich>=13.3.5
@@ -31,14 +31,22 @@
 
 [anthropic]
 anthropic>=0.2.6
 
 [dev]
 black
 bumpver
+mkdocs
+mkdocs-autorefs
+mkdocs-jupyter
+mkdocs-material
+mkdocs-material-extensions
+mkdocs-table-reader-plugin
+mkdocstrings
+mkdocstrings-python
 pip-tools
 pytest
 pytest-mock
 pre-commit
 
 [google]
 google-cloud-aiplatform>=1.25.0
```

