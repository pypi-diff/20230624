# Comparing `tmp/mindflow-0.5.2.tar.gz` & `tmp/mindflow-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindflow-0.5.2.tar", last modified: Tue Jun 20 23:53:23 2023, max compression
+gzip compressed data, was "mindflow-0.5.3.tar", last modified: Sat Jun 24 21:52:29 2023, max compression
```

## Comparing `mindflow-0.5.2.tar` & `mindflow-0.5.3.tar`

### file list

```diff
@@ -1,108 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.307656 mindflow-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-20 23:53:13.000000 mindflow-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 23:53:13.000000 mindflow-0.5.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:53:13.000000 mindflow-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-20 23:53:13.000000 mindflow-0.5.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 23:53:23.307656 mindflow-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-20 23:53:13.000000 mindflow-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 23:53:13.000000 mindflow-0.5.2/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.299656 mindflow-0.5.2/mindflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.299656 mindflow-0.5.2/mindflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.299656 mindflow-0.5.2/mindflow/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.299656 mindflow-0.5.2/mindflow/cli/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/mr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/git/push.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/cli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/command_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/commands/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/mr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/git/push.py
--rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/file_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/file_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/file_processing/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/file_processing/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/prompt_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/resolving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/resolving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/resolving/resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/resolving/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/resolving/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/resolving/resolvers/document_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/resolving/resolvers/file_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.303656 mindflow-0.5.2/mindflow/core/text_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/text_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/text_processing/utf8.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/text_processing/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/token_counting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.307656 mindflow-0.5.2/mindflow/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.307656 mindflow-0.5.2/mindflow/core/types/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/mind_flow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/definitions/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/mindflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.307656 mindflow-0.5.2/mindflow/core/types/store_traits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/store_traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/store_traits/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/store_traits/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/core/types/store_traits/static.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.307656 mindflow-0.5.2/mindflow/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/unit_tests/dummy_diff.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/unit_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-06-20 23:53:13.000000 mindflow-0.5.2/mindflow/unit_tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:53:23.299656 mindflow-0.5.2/mindflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 23:53:23.000000 mindflow-0.5.2/mindflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 23:53:13.000000 mindflow-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:53:23.307656 mindflow-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-20 23:53:13.000000 mindflow-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.295261 mindflow-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-24 21:52:14.000000 mindflow-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-24 21:52:14.000000 mindflow-0.5.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:52:14.000000 mindflow-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-24 21:52:14.000000 mindflow-0.5.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-24 21:52:29.295261 mindflow-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-24 21:52:14.000000 mindflow-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-24 21:52:14.000000 mindflow-0.5.3/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.287261 mindflow-0.5.3/mindflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.287261 mindflow-0.5.3/mindflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.287261 mindflow-0.5.3/mindflow/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/cli/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/git/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/cli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/command_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/file_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/file_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/file_processing/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/file_processing/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/prompt_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/resolving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/resolving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/resolving/resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/resolving/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/resolving/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/resolving/resolvers/document_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/resolving/resolvers/file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.291261 mindflow-0.5.3/mindflow/core/text_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/text_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/text_processing/utf8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/text_processing/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/token_counting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.295261 mindflow-0.5.3/mindflow/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.295261 mindflow-0.5.3/mindflow/core/types/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/mind_flow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/definitions/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/mindflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.295261 mindflow-0.5.3/mindflow/core/types/store_traits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/store_traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/store_traits/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/store_traits/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/core/types/store_traits/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.295261 mindflow-0.5.3/mindflow/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/unit_tests/dummy_diff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/unit_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-06-24 21:52:14.000000 mindflow-0.5.3/mindflow/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:52:29.287261 mindflow-0.5.3/mindflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 21:52:29.000000 mindflow-0.5.3/mindflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-24 21:52:14.000000 mindflow-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 21:52:29.295261 mindflow-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-24 21:52:14.000000 mindflow-0.5.3/setup.py
```

### Comparing `mindflow-0.5.2/.gitignore` & `mindflow-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/Makefile` & `mindflow-0.5.3/Makefile`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/PKG-INFO` & `mindflow-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.5.2
+Version: 0.5.3
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
```

### Comparing `mindflow-0.5.2/README.md` & `mindflow-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/cli/cli_main.py` & `mindflow-0.5.3/mindflow/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/cli/commands/chat.py` & `mindflow-0.5.3/mindflow/cli/commands/chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+import asyncio
 import click
 from typing import Tuple
 import os
 
+from result import Result
+
 from mindflow.core.commands.chat import run_chat
 from mindflow.core.commands.index import run_index
 from mindflow.core.commands.query import run_query
+from mindflow.core.settings import Settings
+from mindflow.core.types.model import ModelApiCallError
 from mindflow.core.types.store_traits.json import save_json_store
 from mindflow.core.types.conversation import Conversation
 from mindflow.core.types.definitions.conversation import ConversationID
 
 
 def parse_chat_prompt_and_paths_from_args(prompt_args: Tuple[str]):
     prompt = " ".join(prompt_args)  # include files/directories in prompt
@@ -24,32 +29,39 @@
 @click.command(
     help='Interact with ChatGPT, you can reference files and directories by passing them as arguments. Example: `mf chat "Please summarize this file" path/to/file.txt`'
 )
 @click.option("-s", "--skip-index", type=bool, default=False, is_flag=True)
 @click.argument("prompt_args", nargs=-1, type=str, required=True)
 def chat(prompt_args: Tuple[str], skip_index: bool):
     prompt, paths = parse_chat_prompt_and_paths_from_args(prompt_args)
-
-    if any(os.path.isdir(path) for path in paths):
+    settings = Settings()
+    if paths:
         if skip_index:
             click.echo(
                 "Skipping indexing step, only using the current index for context. You can run `mf index` to pre-index specific paths."
             )
         else:
             click.echo(
                 "Indexing paths... Note: this may take a while, if you want to skip this step, use the `--skip-index` flag. If you do so, you can pre-select specific paths to index with `mf index`.\n"
             )
 
-            run_index(paths)
-            click.echo("")
-        print(run_query(paths, prompt))
+            asyncio.run(run_index(settings, paths))
+
+        run_query_result: Result[str, ModelApiCallError] = asyncio.run(
+            run_query(settings, paths, prompt)
+        )
+        click.echo(run_query_result.value)
+
         save_json_store()
         return
 
-    print(run_chat(paths, prompt))
+    run_chat_result: Result[str, ModelApiCallError] = asyncio.run(
+        run_chat(settings, [], prompt)
+    )
+    click.echo(run_chat_result.value)
     save_json_store()
 
 
 @click.group(help="Manage conversation histories.")
 def history():
     pass
```

### Comparing `mindflow-0.5.2/mindflow/cli/commands/config.py` & `mindflow-0.5.3/mindflow/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/cli/util.py` & `mindflow-0.5.3/mindflow/cli/util.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/core/commands/delete.py` & `mindflow-0.5.3/mindflow/cli/commands/delete.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,29 @@
+import asyncio
 from typing import List
 
-from mindflow.core.types.document import (
-    Document,
-    DocumentChunk,
-    DocumentReference,
-    get_document_chunk_ids,
-    get_document_id,
-)
+import click
+from result import Result
+
+from mindflow.core.commands.delete import run_delete
 from mindflow.core.resolving.resolve import resolve_paths_to_document_references
+from mindflow.core.types.document import DocumentReference, get_document_id
 
 
-def run_delete(document_paths: List[str]) -> str:
-    """Delete documents from MindFlow index."""
+@click.command(help="Delete your MindFlow index")
+@click.argument("document_paths", type=str, nargs=-1)
+def delete(document_paths: List[str]):
     document_references: List[DocumentReference] = resolve_paths_to_document_references(
         document_paths
     )
 
     document_ids = [
         document_id
         for document_id in [
             get_document_id(document_reference.path, document_reference.document_type)
             for document_reference in document_references
         ]
         if document_id is not None
     ]
 
-    if not document_ids:
-        return "No document IDs resolved. Nothing to delete."
-
-    documents = Document.load_bulk_ignore_missing(document_ids)
-    if not documents:
-        return "No documents found to delete."
-
-    document_chunk_ids = get_document_chunk_ids(documents)
-    if not DocumentChunk.load_bulk_ignore_missing(document_chunk_ids):
-        return "No document chunks found to delete."
-
-    Document.delete_bulk(document_ids)
-    DocumentChunk.delete_bulk(document_chunk_ids)
-
-    return "Documents and associated chunks deleted successfully."
+    delete_result: Result[str, str] = asyncio.run(run_delete(document_ids))
+    click.echo(delete_result.value)
```

### Comparing `mindflow-0.5.2/mindflow/core/commands/gen.py` & `mindflow-0.5.3/mindflow/core/commands/gen.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,48 @@
-import os
-from typing import Union
-import click
+from result import Err, Ok, Result
 from mindflow.core.types.conversation import Conversation
 from mindflow.core.types.definitions.conversation import ConversationID
 from mindflow.core.settings import Settings
-from mindflow.core.errors import ModelError
 from mindflow.core.text_processing.xml import get_text_within_xml
 
 from mindflow.core.prompt_builders import (
     Role,
     build_prompt_from_conversation_messages,
     create_conversation_message,
     prune_messages_to_fit_context_window,
 )
 from mindflow.core.token_counting import get_token_count_of_messages_for_model
+from mindflow.core.types.model import ConfiguredTextCompletionModel, ModelApiCallError
 
 
-def run_code_generation(output_path: str, prompt: str) -> str:
-    settings = Settings()
-    completion_model = settings.mindflow_models.query.model
-
-    if os.path.exists(output_path):
-        click.confirm(
-            f"The output path '{output_path}' already exists. Do you want to overwrite it?",
-            abort=True,
-        )
-        os.remove(output_path)
-
-    if len((output_path_dir := os.path.dirname(output_path))) > 0:
-        os.makedirs(output_path_dir, exist_ok=True)
-
+async def run_code_generation(
+    settings: Settings, output_path: str, prompt: str
+) -> Result[str, ModelApiCallError]:
+    query_model: ConfiguredTextCompletionModel = settings.mindflow_models.query
     if (conversation := Conversation.load(ConversationID.CODE_GEN_0.value)) is None:
         conversation = Conversation(
             {"id": ConversationID.CODE_GEN_0.value, "messages": [], "total_tokens": 0}
         )
 
     conversation.messages.append(
         create_conversation_message(
             Role.USER.value,
             f"Generate code for '{output_path}' with the following prompt: '{prompt}'. Do NOT use any special characters or symbols, any additional information must be put in comments. Please put the code within XML tags like <GEN></GEN>.",
         )
     )
     conversation.messages = prune_messages_to_fit_context_window(
-        conversation.messages, completion_model
+        conversation.messages, query_model
     )
 
-    response: Union[ModelError, str] = completion_model(
-        build_prompt_from_conversation_messages(conversation.messages, completion_model)
+    query_model_result: Result[str, ModelApiCallError] = await query_model.call_api(
+        build_prompt_from_conversation_messages(conversation.messages, query_model)
     )
-    if isinstance(response, ModelError):
-        return response.message
-
-    with open(output_path, "w") as f:
-        f.write(get_text_within_xml(response, "GEN"))
+    if isinstance(query_model_result, Err):
+        return query_model_result
 
     conversation.total_tokens = get_token_count_of_messages_for_model(
-        conversation.messages, completion_model
+        query_model.tokenizer, conversation.messages
     )
 
     conversation.save()
 
-    return f"Code generation complete. Your code is ready to go at {output_path}!"
+    return Ok(get_text_within_xml(query_model_result.value, "GEN"))
```

### Comparing `mindflow-0.5.2/mindflow/core/commands/git/mr.py` & `mindflow-0.5.3/mindflow/cli/commands/git/mr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,82 @@
+import asyncio
 import subprocess
 from typing import Optional, Tuple
 
-from mindflow.core.commands.git.pr import create_title_and_body
+import click
+from result import Err
+from mindflow.cli.util import passthrough_command
 from mindflow.core.command_parse import get_flag_values_from_args
-from mindflow.core.execute import execute_command_and_print_without_trace
-
-
-def run_mr(
+from mindflow.core.commands.git.pr import create_gpt_title_and_body
+from mindflow.core.execute import execute_command_without_trace
+from mindflow.core.settings import Settings
+
+
+@click.group()
+def mr():
+    """
+    MR command.
+    """
+    pass
+
+
+@passthrough_command(help="Generate a git pr response by feeding git diff to gpt")
+@click.option(
+    "-t",
+    "--title",
+    help="Don't use mindflow to generate a pr title, use this one instead.",
+    default=None,
+)
+@click.option(
+    "-d",
+    "--description",
+    help="Don't use mindflow to generate a pr body, use this one instead.",
+    default=None,
+)
+def create(
     args: Tuple[str], title: Optional[str] = None, description: Optional[str] = None
 ):
+    if title is not None:
+        click.echo(
+            f"Warning: Using message '{title}' instead of mindflow generated message."
+        )
+        click.echo("It's recommended that you don't use the -t/--title flag.")
+
+    if description is not None:
+        click.echo(
+            f"Warning: Using message '{description}' instead of mindflow generated message."
+        )
+        click.echo("It's recommended that you don't use the -d/--description flag.")
+
     if (
         base_branch_name := get_flag_values_from_args(args, ["--target-branch", "-b"])
     ) is None:
         base_branch_name = (
             subprocess.check_output(["git", "symbolic-ref", "refs/remotes/origin/HEAD"])
             .decode()
             .strip()
             .split("/")[-1]
         )
 
-    if not title or not description:
-        title, description = create_title_and_body(
-            base_branch_name, title, description
-        ) or (
-            None,
-            None,
-        )
+    diff_result = execute_command_without_trace(
+        ["git", "diff", base_branch_name]
+    ).strip()
 
     if not title or not description:
-        return
+        title_and_body_result = asyncio.run(
+            create_gpt_title_and_body(Settings(), diff_result, title, description)
+        )
+        if isinstance(title_and_body_result, Err):
+            click.echo(title_and_body_result.value)
+            return
+        title, description = title_and_body_result.value
 
-    print(
-        execute_command_and_print_without_trace(
+    click.echo(
+        execute_command_without_trace(
             ["glab", "mr", "create"]
             + list(args)
             + ["--title", title, "--description", description]
         )
     )
+
+
+mr.add_command(create)
```

### Comparing `mindflow-0.5.2/mindflow/core/commands/index.py` & `mindflow-0.5.3/mindflow/core/commands/index.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,155 +1,92 @@
-from concurrent.futures import ThreadPoolExecutor
+import asyncio
 import hashlib
 import sys
 
-from typing import List, Optional, TypeVar
+from typing import List, Optional
 
 from alive_progress import alive_bar
 import numpy as np
+from result import Err, Ok, Result
 
 from mindflow.core.types.document import (
     Document,
     DocumentChunk,
     DocumentReference,
     get_document_id,
 )
-from mindflow.core.types.model import ConfiguredModel
+from mindflow.core.types.model import (
+    ConfiguredTextCompletionModel,
+    ConfiguredEmbeddingModel,
+    ModelApiCallError,
+)
 from mindflow.core.types.document import read_document
 from mindflow.core.resolving.resolve import resolve_paths_to_document_references
 from mindflow.core.settings import Settings
 from mindflow.core.prompt_builders import (
     Role,
     build_prompt_from_conversation_messages,
     create_conversation_message,
 )
 from mindflow.core.prompts import INDEX_PROMPT_PREFIX
 from mindflow.core.token_counting import get_token_count_of_text_for_model
 
 
-def run_index(document_paths: List[str]) -> str:
-    settings = Settings()
-    completion_model: ConfiguredModel = settings.mindflow_models.index.model
-    embedding_model: ConfiguredModel = settings.mindflow_models.embedding.model
+async def run_index(settings: Settings, document_paths: List[str]) -> str:
+    index_model: ConfiguredTextCompletionModel = settings.mindflow_models.index
+    embedding_model: ConfiguredEmbeddingModel = settings.mindflow_models.embedding
 
     document_references: List[DocumentReference] = resolve_paths_to_document_references(
         document_paths
     )
 
     if not (
-        indexable_documents := get_indexable_documents(
-            document_references, completion_model
+        indexable_documents := await get_indexable_documents(
+            document_references, index_model
         )
     ):
         return "No documents to index"
 
     print_total_size_of_documents(indexable_documents)
-    print_total_tokens_and_ask_to_continue(indexable_documents, completion_model)
-
-    index_documents(indexable_documents, completion_model, embedding_model)
+    print_total_tokens_and_ask_to_continue(indexable_documents, index_model)
 
-    return "Successfully indexed documents"
+    await index_documents(indexable_documents, index_model, embedding_model)
 
+    return "Indexing complete"
 
-def print_total_size_of_documents(documents: List[Document]):
-    print(
-        f"Total content size: MB {sum([document.size for document in documents]) / 1024 / 1024:.2f}"
-    )
-
-
-def print_total_tokens_and_ask_to_continue(
-    documents: List[Document],
-    completion_model: ConfiguredModel,
-    usd_threshold: float = 0.5,
-):
-    total_tokens = sum([document.tokens for document in documents])
-    print(f"Total tokens: {total_tokens}")
-    total_cost_usd: float = (
-        total_tokens / float(completion_model.token_cost_unit)
-    ) * completion_model.token_cost
-    if total_cost_usd > usd_threshold:
-        print(f"Total cost: ${total_cost_usd:.2f}")
-        while True:
-            if (
-                user_input := input("Would you like to continue? (yes/no): ").lower()
-            ) in ["no", "n"]:
-                sys.exit(0)
-            elif user_input in ["yes", "y"]:
-                break
-            else:
-                print("Invalid input. Please try again.")
-
-
-def index_documents(
-    documents: List[Document],
-    completion_model: ConfiguredModel,
-    embedding_model: ConfiguredModel,
-) -> None:
-    with alive_bar(len(documents), bar="blocks", spinner="twirls") as progress_bar:
-        with ThreadPoolExecutor(max_workers=50) as executor:
-            document_chunk_futures = [
-                executor.submit(
-                    split_document_to_chunks_by_token_count_and_generate_embeddings,
-                    completion_model,
-                    embedding_model,
-                    indexable_document,
-                )
-                for indexable_document in documents
-            ]
-
-            for document, document_chunk_future in zip(
-                documents, document_chunk_futures
-            ):
-                document_chunks = document_chunk_future.result()
-
-                document.num_chunks = len(document_chunks)
-                document.embedding = list(
-                    np.mean(
-                        [
-                            document_chunk.embedding
-                            for document_chunk in document_chunks
-                        ],
-                        axis=0,
-                    )
-                )
 
-                DocumentChunk.save_bulk(document_chunks)
-                document.save()
-
-                progress_bar()
-
-
-def get_indexable_documents(
-    document_references: List[DocumentReference], completion_model: ConfiguredModel
+async def get_indexable_documents(
+    document_references: List[DocumentReference],
+    index_model: ConfiguredTextCompletionModel,
 ) -> List[Document]:
     document_ids = [
         document_id
         for document_id in [
             get_document_id(document_reference.path, document_reference.document_type)
             for document_reference in document_references
         ]
         if document_id is not None
     ]
-    documents: List[Optional[Document]] = Document.load_bulk(document_ids)
+    documents: List[Optional[Document]] = await Document.load_bulk(document_ids)
     return [
         indexable_document
         for document, document_reference in zip(documents, document_references)
         if (
             indexable_document := get_indexable_document(
-                document, document_reference, completion_model
+                document, document_reference, index_model
             )
         )
         is not None
     ]
 
 
 def get_indexable_document(
     document: Optional[Document],
     document_reference: DocumentReference,
-    completion_model: ConfiguredModel,
+    index_model: ConfiguredTextCompletionModel,
 ) -> Optional[Document]:
     if not (
         document_text := read_document(
             document_reference.path, document_reference.document_type
         )
     ):
         return None
@@ -164,216 +101,314 @@
         {
             "id": document_hash,
             "path": document_reference.path,
             "document_type": document_reference.document_type,
             "num_chunks": document.num_chunks if document else 0,
             "size": len(document_text_bytes),
             "tokens": get_token_count_of_text_for_model(
-                completion_model, document_text
+                index_model.tokenizer, document_text
             ),
         }
     )
 
 
-def split_document_to_chunks_by_token_count_and_generate_embeddings(
-    completion_model: ConfiguredModel,
-    embedding_model: ConfiguredModel,
+def print_total_size_of_documents(documents: List[Document]):
+    print(
+        f"Total content size: MB {sum([document.size for document in documents]) / 1024 / 1024:.2f}"
+    )
+
+
+def print_total_tokens_and_ask_to_continue(
+    documents: List[Document],
+    index_model: ConfiguredTextCompletionModel,
+    usd_threshold: float = 0.5,
+):
+    total_tokens = sum([document.tokens for document in documents])
+    print(f"Total tokens: {total_tokens}")
+    total_cost_usd: float = (
+        total_tokens / float(index_model.model.token_cost_unit)
+    ) * index_model.model.token_cost
+    if total_cost_usd > usd_threshold:
+        print(f"Total cost: ${total_cost_usd:.2f}")
+        while True:
+            if (
+                user_input := input("Would you like to continue? (yes/no): ").lower()
+            ) in ["no", "n"]:
+                sys.exit(0)
+            elif user_input in ["yes", "y"]:
+                break
+            print("Invalid input. Please try again.")
+
+
+async def index_documents(
+    documents: List[Document],
+    index_model: ConfiguredTextCompletionModel,
+    embedding_model: ConfiguredEmbeddingModel,
+) -> None:
+    print("Starting to index documents...")
+    with alive_bar(len(documents), bar="blocks", spinner="twirls") as progress_bar:
+        tasks = [
+            index_document(indexable_document, index_model, embedding_model)
+            for indexable_document in documents
+        ]
+
+        for future in asyncio.as_completed(tasks):
+            index_document_result = await future
+            if isinstance(index_document_result, Err):
+                print(f"Failed to index document {index_document_result.value}")
+            progress_bar()
+
+
+async def index_document(
     indexable_document: Document,
-) -> List[DocumentChunk]:
+    index_model: ConfiguredTextCompletionModel,
+    embedding_model: ConfiguredEmbeddingModel,
+) -> Result[bool, ModelApiCallError]:
     if not (
         text := read_document(indexable_document.path, indexable_document.document_type)
     ):
         print("Document staged for indexing could not be read")
         sys.exit(1)
 
-    if (
-        token_count := get_token_count_of_text_for_model(completion_model, text)
-    ) < completion_model.soft_token_limit:
-        return [
-            process_small_document(
-                completion_model,
-                embedding_model,
-                text,
-                indexable_document.id,
-                token_count,
-            )
-        ]
+    partitioned_nodes_result: Result[
+        List[Node], ModelApiCallError
+    ] = await partition_document_into_nodes(text, index_model)
+    if isinstance(partitioned_nodes_result, Err):
+        return partitioned_nodes_result
+
+    hierarchical_summary_tree_result: Result[
+        Node, ModelApiCallError
+    ] = await create_hierarchical_summary_tree(
+        partitioned_nodes_result.value,
+        index_model,
+    )
+    if isinstance(hierarchical_summary_tree_result, Err):
+        return hierarchical_summary_tree_result
 
-    return process_large_document(
-        completion_model, embedding_model, text, indexable_document.id
+    document_chunks_result: Result[
+        List[DocumentChunk], ModelApiCallError
+    ] = await collect_leaves_with_embeddings_from_appended_branch_summaries(
+        indexable_document.id,
+        hierarchical_summary_tree_result.value,
+        embedding_model,
     )
 
+    if isinstance(document_chunks_result, Err):
+        return document_chunks_result
 
-def process_small_document(
-    completion_model: ConfiguredModel,
-    embedding_model: ConfiguredModel,
-    text: str,
-    document_id: str,
-    tokens: int,
-) -> DocumentChunk:
-    summary: str = completion_model(
-        build_prompt_from_conversation_messages(
+    indexable_document.num_chunks = len(document_chunks_result.value)
+    indexable_document.embedding = list(
+        np.mean(
             [
-                create_conversation_message(Role.SYSTEM.value, INDEX_PROMPT_PREFIX),
-                create_conversation_message(Role.USER.value, text),
+                document_chunk.embedding
+                for document_chunk in document_chunks_result.value
             ],
-            completion_model,
+            axis=0,
         )
     )
-    return DocumentChunk(
-        {
-            "id": f"{document_id}_0",
-            "summary": summary,
-            "embedding": embedding_model(summary),
-            "start_pos": 0,
-            "end_pos": len(text),
-            "num_tokens": tokens,
-        }
+
+    await asyncio.gather(
+        *[
+            DocumentChunk.save_bulk(document_chunks_result.value),
+            indexable_document.save(),
+        ]
     )
+    return Ok(True)
 
 
-def process_large_document(
-    completion_model: ConfiguredModel,
-    embedding_model: ConfiguredModel,
-    text: str,
-    document_id: str,
-) -> List[DocumentChunk]:
-    return collect_leaves_with_embeddings_from_appended_branch_summaries(
-        create_hierarchical_summary_tree(
-            split_raw_text_to_document_chunks(
-                completion_model, embedding_model, text, document_id
-            ),
-            completion_model,
-        ),
-        "",
-        embedding_model,
-    )
+class Node:
+    def __init__(
+        self, start_pos: int, end_pos: int, summary: str, children: List["Node"]
+    ):
+        self.start_pos = start_pos
+        self.end_pos = end_pos
+        self.summary = summary
+        self.children = children
+
+    @classmethod
+    async def create_node(
+        cls,
+        text: str,
+        start_pos: int,
+        end_pos: int,
+        index_model: ConfiguredTextCompletionModel,
+        children: List["Node"] = [],
+    ) -> Result["Node", ModelApiCallError]:
+        prompt = build_prompt_from_conversation_messages(
+            [
+                create_conversation_message(Role.SYSTEM.value, INDEX_PROMPT_PREFIX),
+                create_conversation_message(Role.USER.value, f"{text}..."),
+            ],
+            index_model,
+        )
+
+        index_model_result = await index_model.call_api(prompt)
+        if isinstance(index_model_result, Err):
+            return index_model_result
+
+        return Ok(cls(start_pos, end_pos, index_model_result.value, children))
+
+    def __repr__(self):
+        return f"Node(start_pos={self.start_pos}, end_pos={self.end_pos}, summary={self.summary}, children={self.children})"
 
 
-def split_raw_text_to_document_chunks(
-    completion_model: ConfiguredModel,
-    embedding_model: ConfiguredModel,
+async def partition_document_into_nodes(
     text: str,
-    document_hash: str,
-) -> List[DocumentChunk]:
+    index_model: ConfiguredTextCompletionModel,
+) -> Result[List[Node], ModelApiCallError]:
     start = 0
     end = len(text)
-    document_chunks: List[DocumentChunk] = []
+    document_partition_nodes: List[Node] = []
+    tasks: List[asyncio.Task[Result[Node, ModelApiCallError]]] = []
 
     while start < end:
         text_chunk_size = binary_search_max_raw_text_chunk_size_for_token_limit(
-            completion_model, text, start, end
-        )
-
-        text_str = text[start : start + text_chunk_size]
-        summary: str = completion_model(
-            build_prompt_from_conversation_messages(
-                [
-                    create_conversation_message(Role.SYSTEM.value, INDEX_PROMPT_PREFIX),
-                    create_conversation_message(Role.USER.value, text_str),
-                ],
-                completion_model,
-            )
+            text, start, end, index_model
         )
-        document_chunks.append(
-            DocumentChunk(
-                {
-                    "id": f"{document_hash}_{len(document_chunks)}",
-                    "summary": summary,
-                    "embedding": embedding_model(summary),
-                    "start_pos": start,
-                    "end_pos": start + text_chunk_size,
-                    "num_tokens": get_token_count_of_text_for_model(
-                        completion_model, text_str
-                    ),
-                }
+        tasks.append(
+            asyncio.create_task(
+                Node.create_node(
+                    text[start : start + text_chunk_size],
+                    start,
+                    start + text_chunk_size,
+                    index_model,
+                )
             )
         )
-
         start += text_chunk_size
 
-    return document_chunks
+    for future in asyncio.as_completed(tasks):
+        if isinstance(node_result := await future, Err):
+            return node_result
+        document_partition_nodes.append(node_result.value)
+
+    return Ok(document_partition_nodes)
 
 
 def binary_search_max_raw_text_chunk_size_for_token_limit(
-    completion_model: ConfiguredModel, text: str, start: int, end: int
+    text: str, start: int, end: int, index_model: ConfiguredTextCompletionModel
 ) -> int:
     left = 0
     right = end - start
     while left < right:
         mid = (left + right + 1) // 2
         if (
             get_token_count_of_text_for_model(
-                completion_model, text[start : start + mid]
+                index_model.tokenizer, text[start : start + mid]
             )
-            <= completion_model.soft_token_limit
+            <= index_model.config.soft_token_limit
         ):
             left = mid
-        else:
-            right = mid - 1
+            continue
+        right = mid - 1
     return left
 
 
-class Node:
-    def __init__(self, id, summary, children=None):
-        self.id = id
-        self.summary = summary
-        self.children: List[T] = children if children else []
-
-    def __repr__(self):
-        return (
-            f"Node(id={self.id}, summary={self.summary}, children={len(self.children)})"
-        )
-
-
-T = TypeVar("T", Node, DocumentChunk)
+async def create_hierarchical_summary_tree(
+    nodes: List[Node], index_model: ConfiguredTextCompletionModel
+) -> Result[Node, ModelApiCallError]:
+    if len(nodes) == 1:
+        return Ok(nodes[0])
 
-
-def create_hierarchical_summary_tree(
-    nodes: List[T], completion_model: ConfiguredModel
-) -> Node:
     if (
         get_token_count_of_text_for_model(
-            completion_model, (summary := " ".join(node.summary for node in nodes))
+            index_model.tokenizer,
+            (appended_summaries := " ".join(node.summary for node in nodes)),
         )
-        <= completion_model.soft_token_limit
+        <= index_model.config.soft_token_limit
     ):
-        summary = " ".join(node.summary for node in nodes)
-        node_id = f"parent_{nodes[0].id.split('_')[0]}"
-        return Node(node_id, summary, nodes)
+        return await Node.create_node(
+            appended_summaries,
+            nodes[0].start_pos,
+            nodes[-1].end_pos,
+            index_model,
+            nodes,
+        )
 
     mid = len(nodes) // 2
-    left_tree = create_hierarchical_summary_tree(nodes[:mid], completion_model)
-    right_tree = create_hierarchical_summary_tree(nodes[mid:], completion_model)
+    tasks: List[asyncio.Task[Result[Node, ModelApiCallError]]] = [
+        asyncio.create_task(create_hierarchical_summary_tree(nodes[:mid], index_model)),
+        asyncio.create_task(create_hierarchical_summary_tree(nodes[mid:], index_model)),
+    ]
 
-    merged_summary = completion_model(
-        build_prompt_from_conversation_messages(
-            [
-                create_conversation_message(Role.SYSTEM.value, INDEX_PROMPT_PREFIX),
-                create_conversation_message(
-                    Role.USER.value, f"{left_tree.summary} {right_tree.summary}"
-                ),
-            ],
-            completion_model,
-        )
+    tree_result: List[Result[Node, ModelApiCallError]] = await asyncio.gather(*tasks)
+    if isinstance(tree_result[0], Err):
+        return tree_result[0]
+    if isinstance(tree_result[1], Err):
+        return tree_result[1]
+
+    left_tree, right_tree = tree_result[0].value, tree_result[1].value
+    return await Node.create_node(
+        f"{left_tree.summary} {right_tree.summary}",
+        left_tree.start_pos,
+        right_tree.end_pos,
+        index_model,
+        [left_tree, right_tree],
     )
 
-    parent_id = f"parent_{left_tree.id.split('_')[1]}_{right_tree.id.split('_')[1]}"
-    return Node(parent_id, merged_summary, [left_tree, right_tree])
 
+async def create_document_chunk(
+    id: str,
+    start_pos: int,
+    end_pos: int,
+    appended_summaries: str,
+    embedding_model: ConfiguredEmbeddingModel,
+) -> Result[DocumentChunk, ModelApiCallError]:
+    embedding_result = await embedding_model.call_api(appended_summaries)
+    if isinstance(embedding_result, Err):
+        return embedding_result
+
+    return Ok(
+        DocumentChunk(
+            {
+                "id": id,
+                "start_pos": start_pos,
+                "end_pos": end_pos,
+                "summary": appended_summaries,
+                "embedding": list(embedding_result.value),
+            }
+        )
+    )
 
-def collect_leaves_with_embeddings_from_appended_branch_summaries(
-    node: T,
-    ancestor_summaries: str,
-    embedding_model: ConfiguredModel,
-) -> List[DocumentChunk]:
-    if isinstance(node, DocumentChunk):
-        node.embedding = embedding_model(f"{ancestor_summaries} {node.summary}")
-        return [node]
 
-    return [
-        leaf
-        for child in node.children
-        for leaf in collect_leaves_with_embeddings_from_appended_branch_summaries(
-            child, f"{ancestor_summaries} {node.summary}", embedding_model
-        )
-    ]
+async def collect_leaves_with_embeddings_from_appended_branch_summaries(
+    document_hash: str,
+    root_node: Node,
+    embedding_model: ConfiguredEmbeddingModel,
+) -> Result[List[DocumentChunk], ModelApiCallError]:
+    stack = [(root_node, "")]
+    tasks: List[asyncio.Task[Result[DocumentChunk, ModelApiCallError]]] = []
+    document_chunk_id = 0
+    while stack:
+        node, ancestor_summaries = stack.pop()
+        if not node.children:
+            tasks.append(
+                asyncio.create_task(
+                    create_document_chunk(
+                        f"{document_hash}_{document_chunk_id}",
+                        node.start_pos,
+                        node.end_pos,
+                        f"{ancestor_summaries} {node.summary}",
+                        embedding_model,
+                    )
+                )
+            )
+            document_chunk_id += 1
+        else:
+            for child in node.children:
+                stack.append((child, f"{ancestor_summaries} {node.summary}"))
+
+    create_document_chunk_result: List[
+        Result[DocumentChunk, ModelApiCallError]
+    ] = await asyncio.gather(*tasks)
+
+    for result in create_document_chunk_result:
+        if isinstance(result, Err):
+            return result
+
+    return Ok(
+        [
+            result.value
+            for result in create_document_chunk_result
+            if isinstance(result, Ok)
+        ]
+    )
```

### Comparing `mindflow-0.5.2/mindflow/core/commands/inspect.py` & `mindflow-0.5.3/mindflow/cli/commands/inspect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,28 @@
-import json
+import asyncio
 from typing import List
+import click
+from result import Result
 
-from mindflow.core.types.document import (
-    Document,
-    DocumentChunk,
-    DocumentReference,
-    get_document_chunk_ids,
-    get_document_id,
-)
+from mindflow.core.commands.inspect import run_inspect
 from mindflow.core.resolving.resolve import resolve_paths_to_document_references
+from mindflow.core.types.document import DocumentReference, get_document_id
 
 
-def run_inspect(document_paths: List[str]) -> str:
+@click.command(help="Inspect your MindFlow index")
+@click.argument("document_paths", type=str, nargs=-1)
+def inspect(document_paths: List[str]):
     document_references: List[DocumentReference] = resolve_paths_to_document_references(
         document_paths
     )
-    document_ids = document_ids = [
+    document_ids: List[str] = [
         document_id
         for document_reference in document_references
         if (
             document_id := get_document_id(
                 document_reference.path, document_reference.document_type
             )
         )
         is not None
     ]
-
-    if not (
-        document_chunk_ids := get_document_chunk_ids(
-            Document.load_bulk_ignore_missing(document_ids)
-        )
-    ):
-        return "No documents to inspect"
-
-    document_chunks: List[DocumentChunk] = DocumentChunk.load_bulk_ignore_missing(
-        document_chunk_ids
-    )
-
-    inspect_output = json.dumps(
-        {
-            document_chunk.id: {
-                k: v for k, v in document_chunk.__dict__.items() if k != "embedding"
-            }
-            for document_chunk in document_chunks
-            if document_chunk is not None
-        },
-        indent=4,
-    )
-
-    if inspect_output != "null":
-        return inspect_output
-    return "No documents to inspect"
+    inspect_result: Result[str, str] = asyncio.run(run_inspect(document_ids))
+    click.echo(inspect_result.value)
```

### Comparing `mindflow-0.5.2/mindflow/core/commands/login.py` & `mindflow-0.5.3/mindflow/cli/commands/login.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import click
 from mindflow.cli.commands.config import select_option
-from mindflow.core.types.store_traits.json import save_json_store
-from mindflow.core.types.service import ServiceConfig
+
 from mindflow.core.types.definitions.service import ServiceConfigID
+from mindflow.core.types.service import ServiceConfig
+from mindflow.core.types.store_traits.json import save_json_store
 
 
-def run_login():
+@click.command(help="Set your API Key")
+def login():
     service_ids = [
         ServiceConfigID.OPENAI.value,
         ServiceConfigID.ANTHROPIC.value,
         ServiceConfigID.PINECONE.value,
     ]
     service_options = [
         ServiceConfig.load(service_id, False) for service_id in service_ids
```

### Comparing `mindflow-0.5.2/mindflow/core/commands/query.py` & `mindflow-0.5.3/mindflow/core/commands/query.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,133 @@
-import sys
-
-from typing import Dict, List, Union, Tuple
+import asyncio
+from typing import Dict, List, Tuple
+from result import Err, Ok, Result
 
 import numpy as np
 
 from mindflow.core.types.document import (
     Document,
     DocumentChunk,
     get_document_chunk_ids,
     get_document_id,
 )
-from mindflow.core.types.model import ConfiguredModel
 from mindflow.core.resolving.resolve import resolve_paths_to_document_references
 from mindflow.core.settings import Settings
 from mindflow.core.constants import MinimumReservedLength
-from mindflow.core.errors import ModelError
 from mindflow.core.prompt_builders import (
     Role,
     build_prompt_from_conversation_messages,
     create_conversation_message,
 )
 from mindflow.core.prompts import QUERY_PROMPT_PREFIX
 from mindflow.core.token_counting import get_token_count_of_text_for_model
+from mindflow.core.types.model import (
+    ConfiguredModel,
+    ConfiguredTextCompletionModel,
+    ConfiguredEmbeddingModel,
+    ModelApiCallError,
+)
 
 
-def run_query(document_paths: List[str], query: str) -> str:
+async def run_query(
+    settings: Settings, document_paths: List[str], query: str
+) -> Result[str, ModelApiCallError]:
     """Query files, folders, and websites."""
-    settings = Settings()
-    completion_model = settings.mindflow_models.query.model
-    embedding_model = settings.mindflow_models.embedding.model
+    completion_model: ConfiguredTextCompletionModel = settings.mindflow_models.query
+    embedding_model: ConfiguredEmbeddingModel = settings.mindflow_models.embedding
 
     document_hash_to_path: Dict[str, str] = {
         document_id: doc_reference.path
         for doc_reference in resolve_paths_to_document_references(document_paths)
         if (
             document_id := get_document_id(
                 doc_reference.path, doc_reference.document_type
             )
         )
         is not None
     }
 
-    document_chunk_ids: List[str] = get_document_chunk_ids(
-        Document.load_bulk_ignore_missing(list(document_hash_to_path.keys()))
+    # Create two tasks, one for loading the documents and one for loading the query embedding
+    document_task = Document.load_bulk_ignore_missing(
+        list(document_hash_to_path.keys())
+    )
+    query_embedding_task = embedding_model.call_api(query)
+
+    # Now await both tasks at the same time
+    documents, query_embedding_result = await asyncio.gather(
+        document_task, query_embedding_task
     )
 
+    if isinstance(query_embedding_result, Err):
+        return query_embedding_result
+
+    document_chunk_ids: List[str] = get_document_chunk_ids(documents)
     if not (
-        top_document_chunks := DocumentChunk.query(
-            vector=np.array(embedding_model(query)).reshape(1, -1),
+        top_document_chunks := await DocumentChunk.query(
+            vector=np.array(query_embedding_result.value).reshape(1, -1),
             ids=document_chunk_ids,
             top_k=100,
         )
     ):
-        return (
+        return Ok(
             "No index for requested hashes. Please generate index for passed content."
         )
 
     document_selection_batch: List[Tuple[str, DocumentChunk]] = [
         (document_hash_to_path[document_chunk.id.split("_")[0]], document_chunk)
         for document_chunk in top_document_chunks
     ]
 
     trimmed_content: str = select_and_trim_text_to_fit_context_window(
-        query, document_selection_batch, completion_model
+        completion_model, query, document_selection_batch
     )
-    response: Union[ModelError, str] = completion_model(
+    return await completion_model.call_api(
         build_prompt_from_conversation_messages(
             [
                 create_conversation_message(Role.SYSTEM.value, QUERY_PROMPT_PREFIX),
                 create_conversation_message(
                     Role.USER.value, f"{query}\n\n{trimmed_content}"
                 ),
             ],
             completion_model,
         )
     )
-    if isinstance(response, ModelError):
-        return response.query_message
-
-    return response
 
 
 def select_and_trim_text_to_fit_context_window(
+    configured_model: ConfiguredModel,
     query: str,
     top_document_chunks: List[Tuple[str, DocumentChunk]],
-    completion_model: ConfiguredModel,
 ) -> str:
     selected_content: str = ""
     for path, document_chunk in top_document_chunks:
         with open(path, "r", encoding="utf-8") as file:
             file.seek(document_chunk.start_pos)
             selected_content += formatted_chunk(
                 path,
                 document_chunk,
                 file.read(int(document_chunk.end_pos) - int(document_chunk.start_pos)),
             )
             if (
                 get_token_count_of_text_for_model(
-                    completion_model, query + selected_content
+                    configured_model.tokenizer, query + selected_content
                 )
-                > completion_model.hard_token_limit
+                > configured_model.model.hard_token_limit
             ):
                 break
 
     left, right = 0, len(selected_content)
     while left <= right:
         mid = (left + right) // 2
         if (
             get_token_count_of_text_for_model(
-                completion_model, query + selected_content[:mid]
+                configured_model.tokenizer, query + selected_content[:mid]
             )
-            <= completion_model.hard_token_limit - MinimumReservedLength.QUERY.value
+            <= configured_model.model.hard_token_limit
+            - MinimumReservedLength.QUERY.value
         ):
             left = mid + 1
             continue
         right = mid - 1
 
     return selected_content[:right]
```

### Comparing `mindflow-0.5.2/mindflow/core/errors.py` & `mindflow-0.5.3/mindflow/core/errors.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/core/file_processing/extract.py` & `mindflow-0.5.3/mindflow/core/file_processing/extract.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/core/file_processing/git.py` & `mindflow-0.5.3/mindflow/core/file_processing/git.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/core/prompt_builders.py` & `mindflow-0.5.3/mindflow/core/prompt_builders.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 
 def create_conversation_message(role: str, prompt: str) -> Dict[str, str]:
     return {"role": role, "content": prompt}
 
 
 def build_prompt_from_conversation_messages(
-    messages: List[Dict[str, str]], model: ConfiguredModel
+    messages: List[Dict[str, str]], configured_model: ConfiguredModel
 ) -> Union[List[Dict], str]:
-    if model.service == ServiceID.OPENAI.value:
+    if configured_model.model.service == ServiceID.OPENAI.value:
         return messages
 
     prompt_parts = []
     for message in messages:
         role = message["role"]
         prompt = message["content"]
 
@@ -47,19 +47,19 @@
                 + prompt
             )
 
     return "".join(prompt_parts) + anthropic.AI_PROMPT
 
 
 def prune_messages_to_fit_context_window(
-    messages: List[Dict[str, str]], model: ConfiguredModel
+    messages: List[Dict[str, str]], configured_model: ConfiguredModel
 ) -> List[Dict[str, str]]:
     # Improvement can be made on the estimation here for Anthropic system messages
     content = ""
     for i in range(0, len(messages)):
         content += f"{messages[i]['role']}\n\n {messages[i]['content']}"
         if (
-            get_token_count_of_text_for_model(model, content)
-            > model.hard_token_limit - MinimumReservedLength.CHAT.value
+            get_token_count_of_text_for_model(configured_model.tokenizer, content)
+            > configured_model.model.hard_token_limit - MinimumReservedLength.CHAT.value
         ):
             return messages[:i]
     return messages
```

### Comparing `mindflow-0.5.2/mindflow/core/prompts.py` & `mindflow-0.5.3/mindflow/core/prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 CHAT_PROMPT_PREFIX = "You are a helpful virtual assistant responding to a users query using your general knowledge and the text provided below."
 COMMIT_PROMPT_PREFIX = "Please provide a commit message for the following changes. Only respond with a single commit message and nothing else. Put the response within XML tage like <COMMIT></COMMIT>."
 PR_TITLE_PREFIX = "Please provide a title for the following pull request using this git diff summary. Only respond with the title and nothing else."
 PR_BODY_PREFIX = "Please provide a body for the following pull request using this git diff summary. I want you to keep it high level, and give core \
       themes and reasons for changes. Try to include some titles and bullet points. Only respond with the body and nothing else."
 QUERY_PROMPT_PREFIX = "You are a helpful virtual assistant responding to a users query using your general knowledge and the text provided below."
 DEFAULT_CONVERSATION_SYSTEM_PROMPT = "You are a senior software engineer responding to another software engineer's chat messages regarding your codebase, make sure to be polite and helpful, and provide thorough answers with example code when necessary."
-GIT_DIFF_SUMMARIZE_PROMPT = 'What is the higher level purpose of these changes? Keep it short and sweet, don\'t provide any useless or redundant information like "made changes to the code". Do NOT speak in generalities, be specific.'
+GIT_DIFF_SUMMARIZE_PROMPT = 'What is the higher level purpose of these changes? Keep it short and sweet, don\'t provide any useless or redundant information like "made changes to the code". Do NOT speak in generalities about the higher level changes, be specific.'
```

### Comparing `mindflow-0.5.2/mindflow/core/resolving/resolve.py` & `mindflow-0.5.3/mindflow/core/resolving/resolve.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/core/resolving/resolvers/file_resolver.py` & `mindflow-0.5.3/mindflow/core/resolving/resolvers/file_resolver.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/core/token_counting.py` & `mindflow-0.5.3/mindflow/core/token_counting.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 import os
 from typing import Dict, List
-from mindflow.core.types.model import ConfiguredModel
 
+import tiktoken
 
-def get_token_count_of_text_for_model(model: ConfiguredModel, text: str) -> int:
+
+def get_token_count_of_text_for_model(tokenizer: tiktoken.Encoding, text: str) -> int:
     try:
-        return len(model.tokenizer.encode(text))
+        return len(tokenizer.encode(text))
     except Exception:
         return len(text) // 3
 
 
 def get_batch_token_count_of_text_for_model(
-    model: ConfiguredModel, texts: List[str]
+    tokenizer: tiktoken.Encoding, texts: List[str]
 ) -> int:
     try:
-        return sum(len(encoding) for encoding in model.tokenizer.encode_batch(texts))
+        return sum(len(encoding) for encoding in tokenizer.encode_batch(texts))
     except Exception:
         return sum(len(text) // 3 for text in texts)
 
 
 def get_token_count_of_messages_for_model(
+    tokenizer: tiktoken.Encoding,
     messages: List[Dict[str, str]],
-    model: ConfiguredModel,
 ):
     return get_token_count_of_text_for_model(
-        model,
+        tokenizer,
         "\n\n".join(
             [f"{message['role']}\n\n{message['content']}" for message in messages]
         ),
     )
 
 
 def get_token_count_from_document_query_for_model(
+    tokenizer: tiktoken.Encoding,
     document_paths: List[str],
     query: str,
-    model: ConfiguredModel,
     return_texts: bool = False,
 ):
     texts = [query]
     for document_path in document_paths:
         if os.path.isdir(document_path):
             raise NotImplementedError("Directory support not yet implemented.")
 
         if not os.path.exists(document_path):
             raise FileNotFoundError(f"Could not find file at {document_path}")
 
         file_text = {open(document_path, "r").read()}
         texts.append(f"```{file_text}```")
 
-    tokens = get_batch_token_count_of_text_for_model(model, texts)
+    tokens = get_batch_token_count_of_text_for_model(tokenizer, texts)
     if return_texts:
         return tokens, texts
     return tokens
```

### Comparing `mindflow-0.5.2/mindflow/core/types/definitions/mind_flow_model.py` & `mindflow-0.5.3/mindflow/core/types/definitions/mind_flow_model.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/core/types/document.py` & `mindflow-0.5.3/mindflow/core/types/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import hashlib
 from typing import List, Optional, Union
+from mindflow.core.errors import ModelError
+from mindflow.core.types.model import ConfiguredModel
 
 from mindflow.core.types.store_traits.pinecone import PineconeStore
 from mindflow.core.types.definitions.document import DocumentType
 
 
 class DocumentReference:
     path: str
```

### Comparing `mindflow-0.5.2/mindflow/core/types/mindflow_model.py` & `mindflow-0.5.3/mindflow/core/types/mindflow_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from functools import cached_property
 import sys
-from typing import Dict, Generic, TypeVar, cast
+from typing import Dict
 from mindflow.core.types.definitions.model import ModelID
 from mindflow.core.types.store_traits.static import StaticStore
 from mindflow.core.types.store_traits.json import JsonStore
 
 from mindflow.core.types.model import (
-    ConfiguredModel,
+    ConfiguredEmbeddingModel,
     ConfiguredOpenAIChatCompletionModel,
     ConfiguredAnthropicChatCompletionModel,
     ConfiguredOpenAITextEmbeddingModel,
+    ConfiguredTextCompletionModel,
 )
 from mindflow.core.types.service import ConfiguredServices
 from mindflow.core.types.definitions.mind_flow_model import MindFlowModelID
 from mindflow.core.types.definitions.service import (
     ServiceConfigParameterKey,
     ServiceID,
 )
@@ -26,100 +28,94 @@
 
 
 class MindFlowModelConfig(JsonStore):
     id: str
     model: str
 
 
-T = TypeVar("T", bound="ConfiguredModel")
-
-
-class ConfiguredMindFlowModel(Generic[T]):
-    id: str  # index, query, embedding
-    name: str
-    defaults: Dict[str, str]
-    model: T
+class ConfiguredMindFlowModels:
+    def __init__(self, configured_services: ConfiguredServices):
+        self._configured_services = configured_services
 
-    def __init__(self, mindflow_model_id: str, configured_services: ConfiguredServices):
-        self.id = mindflow_model_id
+    @cached_property
+    def index(self) -> ConfiguredTextCompletionModel:
+        if (
+            model_id := getattr(
+                MindFlowModelConfig.load(f"{MindFlowModelID.INDEX.value}_config"),
+                "model",
+                None,
+            )
+        ) is None:
+            mindflow_model = MindFlowModel.load(MindFlowModelID.INDEX.value)
+            model_id = self.get_default_model_id(
+                MindFlowModelID.INDEX.value, mindflow_model.defaults
+            )
 
-        if mind_flow_model := MindFlowModel.load(mindflow_model_id):
-            for key, value in mind_flow_model.__dict__.items():
-                setattr(self, key, value)
+        if model_id in [ModelID.GPT_3_5_TURBO.value, ModelID.GPT_4.value]:
+            return ConfiguredOpenAIChatCompletionModel(model_id)
+        elif model_id in [ModelID.CLAUDE_INSTANT_V1.value, ModelID.CLAUDE_V1.value]:
+            return ConfiguredAnthropicChatCompletionModel(model_id)
+        raise Exception("Unsupported model: " + model_id)
 
+    @cached_property
+    def query(self) -> ConfiguredTextCompletionModel:
         if (
             model_id := getattr(
-                MindFlowModelConfig.load(f"{mindflow_model_id}_config"), "model", None
+                MindFlowModelConfig.load(f"{MindFlowModelID.QUERY.value}_config"),
+                "model",
+                None,
             )
         ) is None:
-            model_id = self.get_default_model_id(mindflow_model_id, configured_services)
+            mindflow_model = MindFlowModel.load(MindFlowModelID.QUERY.value)
+            model_id = self.get_default_model_id(
+                MindFlowModelID.QUERY.value, mindflow_model.defaults
+            )
 
         if model_id in [ModelID.GPT_3_5_TURBO.value, ModelID.GPT_4.value]:
-            self.model = cast(T, ConfiguredOpenAIChatCompletionModel(model_id))
+            return ConfiguredOpenAIChatCompletionModel(model_id)
         elif model_id in [ModelID.CLAUDE_INSTANT_V1.value, ModelID.CLAUDE_V1.value]:
-            self.model = cast(T, ConfiguredAnthropicChatCompletionModel(model_id))
-        elif model_id == ModelID.TEXT_EMBEDDING_ADA_002.value:
-            self.model = cast(T, ConfiguredOpenAITextEmbeddingModel(model_id))
-        else:
-            raise Exception("Unsupported model: " + model_id)
+            return ConfiguredAnthropicChatCompletionModel(model_id)
+        raise Exception("Unsupported model: " + model_id)
+
+    @cached_property
+    def embedding(self) -> ConfiguredEmbeddingModel:
+        if (
+            model_id := getattr(
+                MindFlowModelConfig.load(f"{MindFlowModelID.EMBEDDING.value}_config"),
+                "model",
+                None,
+            )
+        ) is None:
+            mindflow_model = MindFlowModel.load(MindFlowModelID.EMBEDDING.value)
+            model_id = self.get_default_model_id(
+                MindFlowModelID.EMBEDDING.value, mindflow_model.defaults
+            )
+
+        if model_id == ModelID.TEXT_EMBEDDING_ADA_002.value:
+            return ConfiguredOpenAITextEmbeddingModel(model_id)
+        raise Exception("Unsupported model: " + model_id)
 
     def get_default_model_id(
-        self, mindflow_model_id: str, configured_services: ConfiguredServices
+        self, mindflow_model_id: str, defaults: Dict[str, str]
     ) -> str:
         services = {
-            ServiceID.OPENAI.value: configured_services.openai,
-            ServiceID.ANTHROPIC.value: configured_services.anthropic,
+            ServiceID.OPENAI.value: self._configured_services.openai,
+            ServiceID.ANTHROPIC.value: self._configured_services.anthropic,
         }
 
         for service_id, service in services.items():
             if hasattr(service, ServiceConfigParameterKey.API_KEY.value):
-                model_id = self.defaults.get(service_id)
+                model_id = defaults.get(service_id)
                 if model_id is not None:
                     return model_id
                 else:
                     raise Exception(
                         "No default model configured for mindflow model: "
                         + mindflow_model_id
                         + " and service: "
                         + service.id
                     )
 
         print(
             "No service API key configured. Please configure an API key for at least one service."
         )
         sys.exit(1)
-
-
-class ConfiguredMindFlowModels:
-    def __init__(self, configured_services: ConfiguredServices):
-        self._configured_services = configured_services
-        self._mind_flow_models: Dict[str, ConfiguredMindFlowModel] = {}
-
-    @property
-    def index(self):
-        if MindFlowModelID.INDEX.value not in self._mind_flow_models:
-            self._mind_flow_models[
-                MindFlowModelID.INDEX.value
-            ] = ConfiguredMindFlowModel(
-                MindFlowModelID.INDEX.value, self._configured_services
-            )
-        return self._mind_flow_models[MindFlowModelID.INDEX.value]
-
-    @property
-    def query(self):
-        if MindFlowModelID.QUERY.value not in self._mind_flow_models:
-            self._mind_flow_models[
-                MindFlowModelID.QUERY.value
-            ] = ConfiguredMindFlowModel(
-                MindFlowModelID.QUERY.value, self._configured_services
-            )
-        return self._mind_flow_models[MindFlowModelID.QUERY.value]
-
-    @property
-    def embedding(self):
-        if MindFlowModelID.EMBEDDING.value not in self._mind_flow_models:
-            self._mind_flow_models[
-                MindFlowModelID.EMBEDDING.value
-            ] = ConfiguredMindFlowModel(
-                MindFlowModelID.EMBEDDING.value, self._configured_services
-            )
-        return self._mind_flow_models[MindFlowModelID.EMBEDDING.value]
```

### Comparing `mindflow-0.5.2/mindflow/core/types/service.py` & `mindflow-0.5.3/mindflow/core/types/service.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/core/types/store_traits/json.py` & `mindflow-0.5.3/mindflow/core/types/store_traits/json.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/core/types/store_traits/pinecone.py` & `mindflow-0.5.3/mindflow/core/types/store_traits/pinecone.py`

 * *Files 11% similar despite different names*

```diff
@@ -75,57 +75,57 @@
                 key: value
                 for key, value in self.__dict__.items()
                 if key not in ["embedding"]
             },
         )
 
     @classmethod
-    def load(cls: Type[T], object_id: str) -> Optional[T]:
+    async def load(cls: Type[T], object_id: str) -> Optional[T]:
         if not (object := pinecone_db.get_index(cls.__name__).fetch(ids=[object_id])):
             return None
         return cls(cls._convert_pinecone_format_to_object_format(object["matches"][0]))
 
     @classmethod
-    def load_bulk(cls: Type[T], object_ids: List[str]) -> List[Optional[T]]:
+    async def load_bulk(cls: Type[T], object_ids: List[str]) -> List[Optional[T]]:
         vectors = pinecone_db.get_index(cls.__name__).fetch(ids=object_ids)["vectors"]
         vector_list: List[Optional[T]] = [
             cls(cls._convert_pinecone_format_to_object_format(vectors[obj_id]))
             if obj_id in vectors
             else None
             for obj_id in object_ids
         ]
         return vector_list
 
     @classmethod
-    def load_bulk_ignore_missing(cls: Type[T], object_ids: List[str]) -> List[T]:
+    async def load_bulk_ignore_missing(cls: Type[T], object_ids: List[str]) -> List[T]:
         vectors = pinecone_db.get_index(cls.__name__).fetch(ids=object_ids)["vectors"]
         vector_list: List[Optional[T]] = [
             cls(cls._convert_pinecone_format_to_object_format(vectors[obj_id]))
             if obj_id in vectors
             else None
             for obj_id in object_ids
         ]
         return list(filter(None, vector_list))
 
     @classmethod
-    def delete_bulk(cls, object_ids: List[str]):
+    async def delete_bulk(cls, object_ids: List[str]):
         pinecone_db.get_index(cls.__name__).delete(ids=object_ids)
 
-    def save(self):
+    async def save(self):
         pinecone_db.get_index(self.__class__.__name__).upsert(
             vectors=[self._convert_object_to_pinecone_format()]
         )
 
     @classmethod
-    def save_bulk(cls, objects: List[T]):
+    async def save_bulk(cls, objects: List[T]):
         vectors = [object._convert_object_to_pinecone_format() for object in objects]
         pinecone_db.get_index(cls.__name__).upsert(vectors=vectors)
 
     @classmethod
-    def query(
+    async def query(
         cls: Type[T],
         vector: np.ndarray,
         ids: List[str],
         top_k=100,
         include_metadata=True,
     ) -> List[T]:
         results = pinecone_db.get_index(cls.__name__).query(
```

### Comparing `mindflow-0.5.2/mindflow/core/types/store_traits/static.py` & `mindflow-0.5.3/mindflow/core/types/store_traits/static.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/unit_tests/dummy_diff.txt` & `mindflow-0.5.3/mindflow/unit_tests/dummy_diff.txt`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow/unit_tests/test_utils.py` & `mindflow-0.5.3/mindflow/unit_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mindflow-0.5.2/mindflow.egg-info/PKG-INFO` & `mindflow-0.5.3/mindflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindflow
-Version: 0.5.2
+Version: 0.5.3
 Summary: AI-powered search engine for your code!
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # :brain: mindflow :ocean:
 The [ChatGPT](https://openai.com/blog/chatgpt)-powered swiss army knife for the modern developer! We provide an AI-powered CLI git wrapper, boilerplate code generator, code search engine, a conversation history manager, and much more!
```

### Comparing `mindflow-0.5.2/mindflow.egg-info/SOURCES.txt` & `mindflow-0.5.3/mindflow.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -43,23 +43,19 @@
 mindflow/core/token_counting.py
 mindflow/core/commands/__init__.py
 mindflow/core/commands/chat.py
 mindflow/core/commands/delete.py
 mindflow/core/commands/gen.py
 mindflow/core/commands/index.py
 mindflow/core/commands/inspect.py
-mindflow/core/commands/login.py
 mindflow/core/commands/query.py
 mindflow/core/commands/git/__init__.py
-mindflow/core/commands/git/add.py
 mindflow/core/commands/git/commit.py
 mindflow/core/commands/git/diff.py
-mindflow/core/commands/git/mr.py
 mindflow/core/commands/git/pr.py
-mindflow/core/commands/git/push.py
 mindflow/core/file_processing/__init__.py
 mindflow/core/file_processing/extract.py
 mindflow/core/file_processing/git.py
 mindflow/core/resolving/__init__.py
 mindflow/core/resolving/resolve.py
 mindflow/core/resolving/resolvers/__init__.py
 mindflow/core/resolving/resolvers/document_resolver.py
```

### Comparing `mindflow-0.5.2/setup.py` & `mindflow-0.5.3/setup.py`

 * *Files identical despite different names*

